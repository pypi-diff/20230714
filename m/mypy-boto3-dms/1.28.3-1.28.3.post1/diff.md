# Comparing `tmp/mypy-boto3-dms-1.28.3.tar.gz` & `tmp/mypy-boto3-dms-1.28.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dms-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
+gzip compressed data, was "mypy-boto3-dms-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
```

## Comparing `mypy-boto3-dms-1.28.3.tar` & `mypy-boto3-dms-1.28.3.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.665227 mypy-boto3-dms-1.28.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29436 2023-07-13 19:49:12.653227 mypy-boto3-dms-1.28.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-dms-1.28.3/mypy_boto3_dms/
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73220 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    73114 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   103553 2023-07-13 19:47:17.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103490 2023-07-13 19:47:16.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-13 19:47:14.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29436 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 19:49:12.000000 mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.665227 mypy-boto3-dms-1.28.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-13 19:47:13.000000 mypy-boto3-dms-1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.899361 mypy-boto3-dms-1.28.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30941 2023-07-14 16:17:59.895360 mypy-boto3-dms-1.28.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29445 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74110 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74004 2023-07-14 16:15:37.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17287 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   119853 2023-07-14 16:15:41.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119790 2023-07-14 16:15:39.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.895360 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30941 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.899361 mypy-boto3-dms-1.28.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/setup.py
```

### Comparing `mypy-boto3-dms-1.28.3/LICENSE` & `mypy-boto3-dms-1.28.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3/PKG-INFO` & `mypy-boto3-dms-1.28.3.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-dms
-Version: 1.28.3
-Summary: Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with mypy-boto3-builder 7.14.6
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 dms type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-dms"></a>
 
 # mypy-boto3-dms
 
 [![PyPI - mypy-boto3-dms](https://img.shields.io/pypi/v/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/)
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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -472,26 +440,27 @@
 ### Typed dictionaries
 
 `mypy_boto3_dms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
-    AccountQuotaTypeDef,
+    AccountQuotaOutputTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    AvailabilityZoneTypeDef,
-    BatchStartRecommendationsErrorEntryTypeDef,
+    AvailabilityZoneOutputTypeDef,
+    BatchStartRecommendationsErrorEntryOutputTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
-    CertificateTypeDef,
-    CollectorHealthCheckTypeDef,
-    InventoryDataTypeDef,
-    CollectorShortInfoResponseTypeDef,
+    CertificateOutputTypeDef,
+    CollectorHealthCheckOutputTypeDef,
+    InventoryDataOutputTypeDef,
+    CollectorShortInfoResponseOutputTypeDef,
+    ComputeConfigOutputTypeDef,
     ComputeConfigTypeDef,
-    ConnectionTypeDef,
+    ConnectionOutputTypeDef,
     DmsTransferSettingsTypeDef,
     DocDbSettingsTypeDef,
     DynamoDbSettingsTypeDef,
     ElasticsearchSettingsTypeDef,
     GcpMySQLSettingsTypeDef,
     IBMDb2SettingsTypeDef,
     KafkaSettingsTypeDef,
@@ -503,124 +472,143 @@
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     TimestreamSettingsTypeDef,
-    EventSubscriptionTypeDef,
+    EventSubscriptionOutputTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
-    DatabaseInstanceSoftwareDetailsResponseTypeDef,
-    ServerShortInfoResponseTypeDef,
-    DatabaseShortInfoResponseTypeDef,
+    CreateFleetAdvisorCollectorResponseOutputTypeDef,
+    DatabaseInstanceSoftwareDetailsResponseOutputTypeDef,
+    ServerShortInfoResponseOutputTypeDef,
+    DatabaseShortInfoResponseOutputTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
+    DeleteFleetAdvisorDatabasesResponseOutputTypeDef,
     DeleteReplicationConfigMessageRequestTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseOutputTypeDef,
     FilterTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
-    EndpointSettingTypeDef,
-    SupportedEndpointTypeTypeDef,
-    EventCategoryGroupTypeDef,
-    EventTypeDef,
+    EndpointSettingOutputTypeDef,
+    SupportedEndpointTypeOutputTypeDef,
+    EventCategoryGroupOutputTypeDef,
+    EventOutputTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
-    FleetAdvisorLsaAnalysisResponseTypeDef,
-    FleetAdvisorSchemaObjectResponseTypeDef,
+    FleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    FleetAdvisorSchemaObjectResponseOutputTypeDef,
     DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
-    OrderableReplicationInstanceTypeDef,
-    LimitationTypeDef,
+    OrderableReplicationInstanceOutputTypeDef,
+    LimitationOutputTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
-    RefreshSchemasStatusTypeDef,
+    RefreshSchemasStatusOutputTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
-    ReplicationInstanceTaskLogTypeDef,
-    TableStatisticsTypeDef,
+    ReplicationInstanceTaskLogOutputTypeDef,
+    TableStatisticsOutputTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
-    ReplicationTaskAssessmentResultTypeDef,
-    ReplicationTaskIndividualAssessmentTypeDef,
+    ReplicationTaskAssessmentResultOutputTypeDef,
+    ReplicationTaskIndividualAssessmentOutputTypeDef,
     DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
-    DescribeSchemasResponseTypeDef,
+    DescribeSchemasResponseOutputTypeDef,
+    DmsTransferSettingsOutputTypeDef,
+    DocDbSettingsOutputTypeDef,
+    DynamoDbSettingsOutputTypeDef,
+    ElasticsearchSettingsOutputTypeDef,
     EmptyResponseMetadataTypeDef,
+    GcpMySQLSettingsOutputTypeDef,
+    IBMDb2SettingsOutputTypeDef,
+    KafkaSettingsOutputTypeDef,
+    KinesisSettingsOutputTypeDef,
+    MicrosoftSQLServerSettingsOutputTypeDef,
+    MongoDbSettingsOutputTypeDef,
+    MySQLSettingsOutputTypeDef,
+    NeptuneSettingsOutputTypeDef,
+    OracleSettingsOutputTypeDef,
+    PostgreSQLSettingsOutputTypeDef,
+    RedisSettingsOutputTypeDef,
+    RedshiftSettingsOutputTypeDef,
+    S3SettingsOutputTypeDef,
+    SybaseSettingsOutputTypeDef,
+    TimestreamSettingsOutputTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    TagOutputTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
     PaginatorConfigTypeDef,
-    PendingMaintenanceActionTypeDef,
-    ProvisionDataTypeDef,
-    RdsConfigurationTypeDef,
-    RdsRequirementsTypeDef,
+    PendingMaintenanceActionOutputTypeDef,
+    ProvisionDataOutputTypeDef,
+    RdsConfigurationOutputTypeDef,
+    RdsRequirementsOutputTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
+    RecommendationSettingsOutputTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
-    ReloadReplicationTablesResponseTypeDef,
-    ReloadTablesResponseTypeDef,
+    ReloadReplicationTablesResponseOutputTypeDef,
+    ReloadTablesResponseOutputTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ReplicationPendingModifiedValuesTypeDef,
-    VpcSecurityGroupMembershipTypeDef,
-    ReplicationStatsTypeDef,
-    ReplicationTaskAssessmentRunProgressTypeDef,
-    ReplicationTaskStatsTypeDef,
+    ReplicationPendingModifiedValuesOutputTypeDef,
+    VpcSecurityGroupMembershipOutputTypeDef,
+    ReplicationStatsOutputTypeDef,
+    ReplicationTaskAssessmentRunProgressOutputTypeDef,
+    ReplicationTaskStatsOutputTypeDef,
     ResponseMetadataTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
-    SchemaShortInfoResponseTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    SchemaShortInfoResponseOutputTypeDef,
     StartReplicationMessageRequestTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseOutputTypeDef,
+    DescribeAccountAttributesResponseOutputTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SubnetTypeDef,
-    BatchStartRecommendationsResponseTypeDef,
-    DeleteCertificateResponseTypeDef,
-    DescribeCertificatesResponseTypeDef,
-    ImportCertificateResponseTypeDef,
-    CollectorResponseTypeDef,
+    SubnetOutputTypeDef,
+    BatchStartRecommendationsResponseOutputTypeDef,
+    DeleteCertificateResponseOutputTypeDef,
+    DescribeCertificatesResponseOutputTypeDef,
+    ImportCertificateResponseOutputTypeDef,
+    CollectorResponseOutputTypeDef,
+    ReplicationConfigOutputTypeDef,
     CreateReplicationConfigMessageRequestTypeDef,
     ModifyReplicationConfigMessageRequestTypeDef,
-    ReplicationConfigTypeDef,
-    DeleteConnectionResponseTypeDef,
-    DescribeConnectionsResponseTypeDef,
-    TestConnectionResponseTypeDef,
+    DeleteConnectionResponseOutputTypeDef,
+    DescribeConnectionsResponseOutputTypeDef,
+    TestConnectionResponseOutputTypeDef,
     CreateEndpointMessageRequestTypeDef,
-    EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
-    CreateEventSubscriptionResponseTypeDef,
-    DeleteEventSubscriptionResponseTypeDef,
-    DescribeEventSubscriptionsResponseTypeDef,
-    ModifyEventSubscriptionResponseTypeDef,
-    DatabaseResponseTypeDef,
+    CreateEventSubscriptionResponseOutputTypeDef,
+    DeleteEventSubscriptionResponseOutputTypeDef,
+    DescribeEventSubscriptionsResponseOutputTypeDef,
+    ModifyEventSubscriptionResponseOutputTypeDef,
+    DatabaseResponseOutputTypeDef,
     DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
     DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
     DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
@@ -654,85 +642,87 @@
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef,
-    DescribeEndpointSettingsResponseTypeDef,
-    DescribeEndpointTypesResponseTypeDef,
-    DescribeEventCategoriesResponseTypeDef,
-    DescribeEventsResponseTypeDef,
-    DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
-    DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
-    DescribeOrderableReplicationInstancesResponseTypeDef,
-    DescribeRecommendationLimitationsResponseTypeDef,
-    DescribeRefreshSchemasStatusResponseTypeDef,
-    RefreshSchemasResponseTypeDef,
-    DescribeReplicationInstanceTaskLogsResponseTypeDef,
-    DescribeReplicationTableStatisticsResponseTypeDef,
-    DescribeTableStatisticsResponseTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
-    DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
-    ResourcePendingMaintenanceActionsTypeDef,
-    RdsRecommendationTypeDef,
+    DescribeEndpointSettingsResponseOutputTypeDef,
+    DescribeEndpointTypesResponseOutputTypeDef,
+    DescribeEventCategoriesResponseOutputTypeDef,
+    DescribeEventsResponseOutputTypeDef,
+    DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef,
+    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
+    DescribeRecommendationLimitationsResponseOutputTypeDef,
+    DescribeRefreshSchemasStatusResponseOutputTypeDef,
+    RefreshSchemasResponseOutputTypeDef,
+    DescribeReplicationInstanceTaskLogsResponseOutputTypeDef,
+    DescribeReplicationTableStatisticsResponseOutputTypeDef,
+    DescribeTableStatisticsResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
+    DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef,
+    EndpointOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ResourcePendingMaintenanceActionsOutputTypeDef,
+    RdsRecommendationOutputTypeDef,
     StartRecommendationsRequestEntryTypeDef,
     StartRecommendationsRequestRequestTypeDef,
     ReloadReplicationTablesMessageRequestTypeDef,
     ReloadTablesMessageRequestTypeDef,
-    ReplicationTypeDef,
-    ReplicationTaskAssessmentRunTypeDef,
-    ReplicationTaskTypeDef,
-    SchemaResponseTypeDef,
-    ReplicationSubnetGroupTypeDef,
-    DescribeFleetAdvisorCollectorsResponseTypeDef,
-    CreateReplicationConfigResponseTypeDef,
-    DeleteReplicationConfigResponseTypeDef,
-    DescribeReplicationConfigsResponseTypeDef,
-    ModifyReplicationConfigResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    DeleteEndpointResponseTypeDef,
-    DescribeEndpointsResponseTypeDef,
-    ModifyEndpointResponseTypeDef,
-    DescribeFleetAdvisorDatabasesResponseTypeDef,
-    ApplyPendingMaintenanceActionResponseTypeDef,
-    DescribePendingMaintenanceActionsResponseTypeDef,
-    RecommendationDataTypeDef,
+    ReplicationOutputTypeDef,
+    ReplicationTaskAssessmentRunOutputTypeDef,
+    ReplicationTaskOutputTypeDef,
+    SchemaResponseOutputTypeDef,
+    ReplicationSubnetGroupOutputTypeDef,
+    DescribeFleetAdvisorCollectorsResponseOutputTypeDef,
+    CreateReplicationConfigResponseOutputTypeDef,
+    DeleteReplicationConfigResponseOutputTypeDef,
+    DescribeReplicationConfigsResponseOutputTypeDef,
+    ModifyReplicationConfigResponseOutputTypeDef,
+    DescribeFleetAdvisorDatabasesResponseOutputTypeDef,
+    CreateEndpointResponseOutputTypeDef,
+    DeleteEndpointResponseOutputTypeDef,
+    DescribeEndpointsResponseOutputTypeDef,
+    ModifyEndpointResponseOutputTypeDef,
+    ApplyPendingMaintenanceActionResponseOutputTypeDef,
+    DescribePendingMaintenanceActionsResponseOutputTypeDef,
+    RecommendationDataOutputTypeDef,
     BatchStartRecommendationsRequestRequestTypeDef,
-    DescribeReplicationsResponseTypeDef,
-    StartReplicationResponseTypeDef,
-    StopReplicationResponseTypeDef,
-    CancelReplicationTaskAssessmentRunResponseTypeDef,
-    DeleteReplicationTaskAssessmentRunResponseTypeDef,
-    DescribeReplicationTaskAssessmentRunsResponseTypeDef,
-    StartReplicationTaskAssessmentRunResponseTypeDef,
-    CreateReplicationTaskResponseTypeDef,
-    DeleteReplicationTaskResponseTypeDef,
-    DescribeReplicationTasksResponseTypeDef,
-    ModifyReplicationTaskResponseTypeDef,
-    MoveReplicationTaskResponseTypeDef,
-    StartReplicationTaskAssessmentResponseTypeDef,
-    StartReplicationTaskResponseTypeDef,
-    StopReplicationTaskResponseTypeDef,
-    DescribeFleetAdvisorSchemasResponseTypeDef,
-    CreateReplicationSubnetGroupResponseTypeDef,
-    DescribeReplicationSubnetGroupsResponseTypeDef,
-    ModifyReplicationSubnetGroupResponseTypeDef,
-    ReplicationInstanceTypeDef,
-    RecommendationTypeDef,
-    CreateReplicationInstanceResponseTypeDef,
-    DeleteReplicationInstanceResponseTypeDef,
-    DescribeReplicationInstancesResponseTypeDef,
-    ModifyReplicationInstanceResponseTypeDef,
-    RebootReplicationInstanceResponseTypeDef,
-    DescribeRecommendationsResponseTypeDef,
+    DescribeReplicationsResponseOutputTypeDef,
+    StartReplicationResponseOutputTypeDef,
+    StopReplicationResponseOutputTypeDef,
+    CancelReplicationTaskAssessmentRunResponseOutputTypeDef,
+    DeleteReplicationTaskAssessmentRunResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef,
+    StartReplicationTaskAssessmentRunResponseOutputTypeDef,
+    CreateReplicationTaskResponseOutputTypeDef,
+    DeleteReplicationTaskResponseOutputTypeDef,
+    DescribeReplicationTasksResponseOutputTypeDef,
+    ModifyReplicationTaskResponseOutputTypeDef,
+    MoveReplicationTaskResponseOutputTypeDef,
+    StartReplicationTaskAssessmentResponseOutputTypeDef,
+    StartReplicationTaskResponseOutputTypeDef,
+    StopReplicationTaskResponseOutputTypeDef,
+    DescribeFleetAdvisorSchemasResponseOutputTypeDef,
+    CreateReplicationSubnetGroupResponseOutputTypeDef,
+    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
+    ModifyReplicationSubnetGroupResponseOutputTypeDef,
+    ReplicationInstanceOutputTypeDef,
+    RecommendationOutputTypeDef,
+    CreateReplicationInstanceResponseOutputTypeDef,
+    DeleteReplicationInstanceResponseOutputTypeDef,
+    DescribeReplicationInstancesResponseOutputTypeDef,
+    ModifyReplicationInstanceResponseOutputTypeDef,
+    RebootReplicationInstanceResponseOutputTypeDef,
+    DescribeRecommendationsResponseOutputTypeDef,
 )
 
 
-def get_structure() -> AccountQuotaTypeDef:
+def get_structure() -> AccountQuotaOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dms-1.28.3/README.md` & `mypy-boto3-dms-1.28.3.post1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-dms
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 dms type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-dms"></a>
 
 # mypy-boto3-dms
 
 [![PyPI - mypy-boto3-dms](https://img.shields.io/pypi/v/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/)
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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -440,26 +472,27 @@
 ### Typed dictionaries
 
 `mypy_boto3_dms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
-    AccountQuotaTypeDef,
+    AccountQuotaOutputTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    AvailabilityZoneTypeDef,
-    BatchStartRecommendationsErrorEntryTypeDef,
+    AvailabilityZoneOutputTypeDef,
+    BatchStartRecommendationsErrorEntryOutputTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
-    CertificateTypeDef,
-    CollectorHealthCheckTypeDef,
-    InventoryDataTypeDef,
-    CollectorShortInfoResponseTypeDef,
+    CertificateOutputTypeDef,
+    CollectorHealthCheckOutputTypeDef,
+    InventoryDataOutputTypeDef,
+    CollectorShortInfoResponseOutputTypeDef,
+    ComputeConfigOutputTypeDef,
     ComputeConfigTypeDef,
-    ConnectionTypeDef,
+    ConnectionOutputTypeDef,
     DmsTransferSettingsTypeDef,
     DocDbSettingsTypeDef,
     DynamoDbSettingsTypeDef,
     ElasticsearchSettingsTypeDef,
     GcpMySQLSettingsTypeDef,
     IBMDb2SettingsTypeDef,
     KafkaSettingsTypeDef,
@@ -471,124 +504,143 @@
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     TimestreamSettingsTypeDef,
-    EventSubscriptionTypeDef,
+    EventSubscriptionOutputTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
-    DatabaseInstanceSoftwareDetailsResponseTypeDef,
-    ServerShortInfoResponseTypeDef,
-    DatabaseShortInfoResponseTypeDef,
+    CreateFleetAdvisorCollectorResponseOutputTypeDef,
+    DatabaseInstanceSoftwareDetailsResponseOutputTypeDef,
+    ServerShortInfoResponseOutputTypeDef,
+    DatabaseShortInfoResponseOutputTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
+    DeleteFleetAdvisorDatabasesResponseOutputTypeDef,
     DeleteReplicationConfigMessageRequestTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseOutputTypeDef,
     FilterTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
-    EndpointSettingTypeDef,
-    SupportedEndpointTypeTypeDef,
-    EventCategoryGroupTypeDef,
-    EventTypeDef,
+    EndpointSettingOutputTypeDef,
+    SupportedEndpointTypeOutputTypeDef,
+    EventCategoryGroupOutputTypeDef,
+    EventOutputTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
-    FleetAdvisorLsaAnalysisResponseTypeDef,
-    FleetAdvisorSchemaObjectResponseTypeDef,
+    FleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    FleetAdvisorSchemaObjectResponseOutputTypeDef,
     DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
-    OrderableReplicationInstanceTypeDef,
-    LimitationTypeDef,
+    OrderableReplicationInstanceOutputTypeDef,
+    LimitationOutputTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
-    RefreshSchemasStatusTypeDef,
+    RefreshSchemasStatusOutputTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
-    ReplicationInstanceTaskLogTypeDef,
-    TableStatisticsTypeDef,
+    ReplicationInstanceTaskLogOutputTypeDef,
+    TableStatisticsOutputTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
-    ReplicationTaskAssessmentResultTypeDef,
-    ReplicationTaskIndividualAssessmentTypeDef,
+    ReplicationTaskAssessmentResultOutputTypeDef,
+    ReplicationTaskIndividualAssessmentOutputTypeDef,
     DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
-    DescribeSchemasResponseTypeDef,
+    DescribeSchemasResponseOutputTypeDef,
+    DmsTransferSettingsOutputTypeDef,
+    DocDbSettingsOutputTypeDef,
+    DynamoDbSettingsOutputTypeDef,
+    ElasticsearchSettingsOutputTypeDef,
     EmptyResponseMetadataTypeDef,
+    GcpMySQLSettingsOutputTypeDef,
+    IBMDb2SettingsOutputTypeDef,
+    KafkaSettingsOutputTypeDef,
+    KinesisSettingsOutputTypeDef,
+    MicrosoftSQLServerSettingsOutputTypeDef,
+    MongoDbSettingsOutputTypeDef,
+    MySQLSettingsOutputTypeDef,
+    NeptuneSettingsOutputTypeDef,
+    OracleSettingsOutputTypeDef,
+    PostgreSQLSettingsOutputTypeDef,
+    RedisSettingsOutputTypeDef,
+    RedshiftSettingsOutputTypeDef,
+    S3SettingsOutputTypeDef,
+    SybaseSettingsOutputTypeDef,
+    TimestreamSettingsOutputTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    TagOutputTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
     PaginatorConfigTypeDef,
-    PendingMaintenanceActionTypeDef,
-    ProvisionDataTypeDef,
-    RdsConfigurationTypeDef,
-    RdsRequirementsTypeDef,
+    PendingMaintenanceActionOutputTypeDef,
+    ProvisionDataOutputTypeDef,
+    RdsConfigurationOutputTypeDef,
+    RdsRequirementsOutputTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
+    RecommendationSettingsOutputTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
-    ReloadReplicationTablesResponseTypeDef,
-    ReloadTablesResponseTypeDef,
+    ReloadReplicationTablesResponseOutputTypeDef,
+    ReloadTablesResponseOutputTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ReplicationPendingModifiedValuesTypeDef,
-    VpcSecurityGroupMembershipTypeDef,
-    ReplicationStatsTypeDef,
-    ReplicationTaskAssessmentRunProgressTypeDef,
-    ReplicationTaskStatsTypeDef,
+    ReplicationPendingModifiedValuesOutputTypeDef,
+    VpcSecurityGroupMembershipOutputTypeDef,
+    ReplicationStatsOutputTypeDef,
+    ReplicationTaskAssessmentRunProgressOutputTypeDef,
+    ReplicationTaskStatsOutputTypeDef,
     ResponseMetadataTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
-    SchemaShortInfoResponseTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    SchemaShortInfoResponseOutputTypeDef,
     StartReplicationMessageRequestTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseOutputTypeDef,
+    DescribeAccountAttributesResponseOutputTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SubnetTypeDef,
-    BatchStartRecommendationsResponseTypeDef,
-    DeleteCertificateResponseTypeDef,
-    DescribeCertificatesResponseTypeDef,
-    ImportCertificateResponseTypeDef,
-    CollectorResponseTypeDef,
+    SubnetOutputTypeDef,
+    BatchStartRecommendationsResponseOutputTypeDef,
+    DeleteCertificateResponseOutputTypeDef,
+    DescribeCertificatesResponseOutputTypeDef,
+    ImportCertificateResponseOutputTypeDef,
+    CollectorResponseOutputTypeDef,
+    ReplicationConfigOutputTypeDef,
     CreateReplicationConfigMessageRequestTypeDef,
     ModifyReplicationConfigMessageRequestTypeDef,
-    ReplicationConfigTypeDef,
-    DeleteConnectionResponseTypeDef,
-    DescribeConnectionsResponseTypeDef,
-    TestConnectionResponseTypeDef,
+    DeleteConnectionResponseOutputTypeDef,
+    DescribeConnectionsResponseOutputTypeDef,
+    TestConnectionResponseOutputTypeDef,
     CreateEndpointMessageRequestTypeDef,
-    EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
-    CreateEventSubscriptionResponseTypeDef,
-    DeleteEventSubscriptionResponseTypeDef,
-    DescribeEventSubscriptionsResponseTypeDef,
-    ModifyEventSubscriptionResponseTypeDef,
-    DatabaseResponseTypeDef,
+    CreateEventSubscriptionResponseOutputTypeDef,
+    DeleteEventSubscriptionResponseOutputTypeDef,
+    DescribeEventSubscriptionsResponseOutputTypeDef,
+    ModifyEventSubscriptionResponseOutputTypeDef,
+    DatabaseResponseOutputTypeDef,
     DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
     DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
     DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
@@ -622,85 +674,87 @@
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef,
-    DescribeEndpointSettingsResponseTypeDef,
-    DescribeEndpointTypesResponseTypeDef,
-    DescribeEventCategoriesResponseTypeDef,
-    DescribeEventsResponseTypeDef,
-    DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
-    DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
-    DescribeOrderableReplicationInstancesResponseTypeDef,
-    DescribeRecommendationLimitationsResponseTypeDef,
-    DescribeRefreshSchemasStatusResponseTypeDef,
-    RefreshSchemasResponseTypeDef,
-    DescribeReplicationInstanceTaskLogsResponseTypeDef,
-    DescribeReplicationTableStatisticsResponseTypeDef,
-    DescribeTableStatisticsResponseTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
-    DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
-    ResourcePendingMaintenanceActionsTypeDef,
-    RdsRecommendationTypeDef,
+    DescribeEndpointSettingsResponseOutputTypeDef,
+    DescribeEndpointTypesResponseOutputTypeDef,
+    DescribeEventCategoriesResponseOutputTypeDef,
+    DescribeEventsResponseOutputTypeDef,
+    DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef,
+    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
+    DescribeRecommendationLimitationsResponseOutputTypeDef,
+    DescribeRefreshSchemasStatusResponseOutputTypeDef,
+    RefreshSchemasResponseOutputTypeDef,
+    DescribeReplicationInstanceTaskLogsResponseOutputTypeDef,
+    DescribeReplicationTableStatisticsResponseOutputTypeDef,
+    DescribeTableStatisticsResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
+    DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef,
+    EndpointOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ResourcePendingMaintenanceActionsOutputTypeDef,
+    RdsRecommendationOutputTypeDef,
     StartRecommendationsRequestEntryTypeDef,
     StartRecommendationsRequestRequestTypeDef,
     ReloadReplicationTablesMessageRequestTypeDef,
     ReloadTablesMessageRequestTypeDef,
-    ReplicationTypeDef,
-    ReplicationTaskAssessmentRunTypeDef,
-    ReplicationTaskTypeDef,
-    SchemaResponseTypeDef,
-    ReplicationSubnetGroupTypeDef,
-    DescribeFleetAdvisorCollectorsResponseTypeDef,
-    CreateReplicationConfigResponseTypeDef,
-    DeleteReplicationConfigResponseTypeDef,
-    DescribeReplicationConfigsResponseTypeDef,
-    ModifyReplicationConfigResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    DeleteEndpointResponseTypeDef,
-    DescribeEndpointsResponseTypeDef,
-    ModifyEndpointResponseTypeDef,
-    DescribeFleetAdvisorDatabasesResponseTypeDef,
-    ApplyPendingMaintenanceActionResponseTypeDef,
-    DescribePendingMaintenanceActionsResponseTypeDef,
-    RecommendationDataTypeDef,
+    ReplicationOutputTypeDef,
+    ReplicationTaskAssessmentRunOutputTypeDef,
+    ReplicationTaskOutputTypeDef,
+    SchemaResponseOutputTypeDef,
+    ReplicationSubnetGroupOutputTypeDef,
+    DescribeFleetAdvisorCollectorsResponseOutputTypeDef,
+    CreateReplicationConfigResponseOutputTypeDef,
+    DeleteReplicationConfigResponseOutputTypeDef,
+    DescribeReplicationConfigsResponseOutputTypeDef,
+    ModifyReplicationConfigResponseOutputTypeDef,
+    DescribeFleetAdvisorDatabasesResponseOutputTypeDef,
+    CreateEndpointResponseOutputTypeDef,
+    DeleteEndpointResponseOutputTypeDef,
+    DescribeEndpointsResponseOutputTypeDef,
+    ModifyEndpointResponseOutputTypeDef,
+    ApplyPendingMaintenanceActionResponseOutputTypeDef,
+    DescribePendingMaintenanceActionsResponseOutputTypeDef,
+    RecommendationDataOutputTypeDef,
     BatchStartRecommendationsRequestRequestTypeDef,
-    DescribeReplicationsResponseTypeDef,
-    StartReplicationResponseTypeDef,
-    StopReplicationResponseTypeDef,
-    CancelReplicationTaskAssessmentRunResponseTypeDef,
-    DeleteReplicationTaskAssessmentRunResponseTypeDef,
-    DescribeReplicationTaskAssessmentRunsResponseTypeDef,
-    StartReplicationTaskAssessmentRunResponseTypeDef,
-    CreateReplicationTaskResponseTypeDef,
-    DeleteReplicationTaskResponseTypeDef,
-    DescribeReplicationTasksResponseTypeDef,
-    ModifyReplicationTaskResponseTypeDef,
-    MoveReplicationTaskResponseTypeDef,
-    StartReplicationTaskAssessmentResponseTypeDef,
-    StartReplicationTaskResponseTypeDef,
-    StopReplicationTaskResponseTypeDef,
-    DescribeFleetAdvisorSchemasResponseTypeDef,
-    CreateReplicationSubnetGroupResponseTypeDef,
-    DescribeReplicationSubnetGroupsResponseTypeDef,
-    ModifyReplicationSubnetGroupResponseTypeDef,
-    ReplicationInstanceTypeDef,
-    RecommendationTypeDef,
-    CreateReplicationInstanceResponseTypeDef,
-    DeleteReplicationInstanceResponseTypeDef,
-    DescribeReplicationInstancesResponseTypeDef,
-    ModifyReplicationInstanceResponseTypeDef,
-    RebootReplicationInstanceResponseTypeDef,
-    DescribeRecommendationsResponseTypeDef,
+    DescribeReplicationsResponseOutputTypeDef,
+    StartReplicationResponseOutputTypeDef,
+    StopReplicationResponseOutputTypeDef,
+    CancelReplicationTaskAssessmentRunResponseOutputTypeDef,
+    DeleteReplicationTaskAssessmentRunResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef,
+    StartReplicationTaskAssessmentRunResponseOutputTypeDef,
+    CreateReplicationTaskResponseOutputTypeDef,
+    DeleteReplicationTaskResponseOutputTypeDef,
+    DescribeReplicationTasksResponseOutputTypeDef,
+    ModifyReplicationTaskResponseOutputTypeDef,
+    MoveReplicationTaskResponseOutputTypeDef,
+    StartReplicationTaskAssessmentResponseOutputTypeDef,
+    StartReplicationTaskResponseOutputTypeDef,
+    StopReplicationTaskResponseOutputTypeDef,
+    DescribeFleetAdvisorSchemasResponseOutputTypeDef,
+    CreateReplicationSubnetGroupResponseOutputTypeDef,
+    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
+    ModifyReplicationSubnetGroupResponseOutputTypeDef,
+    ReplicationInstanceOutputTypeDef,
+    RecommendationOutputTypeDef,
+    CreateReplicationInstanceResponseOutputTypeDef,
+    DeleteReplicationInstanceResponseOutputTypeDef,
+    DescribeReplicationInstancesResponseOutputTypeDef,
+    ModifyReplicationInstanceResponseOutputTypeDef,
+    RebootReplicationInstanceResponseOutputTypeDef,
+    DescribeRecommendationsResponseOutputTypeDef,
 )
 
 
-def get_structure() -> AccountQuotaTypeDef:
+def get_structure() -> AccountQuotaOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/__init__.py` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/__init__.pyi` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/__main__.py` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.DatabaseMigrationService 1.28.3\nVersion:        "
-        " 1.28.3\nBuilder version: 7.14.6\nDocs:           "
+        " 1.28.3.post1\nBuilder version: 7.14.7\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService\nOther"
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

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/client.py` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,113 +39,113 @@
     DescribeReplicationSubnetGroupsPaginator,
     DescribeReplicationTaskAssessmentResultsPaginator,
     DescribeReplicationTasksPaginator,
     DescribeSchemasPaginator,
     DescribeTableStatisticsPaginator,
 )
 from .type_defs import (
-    ApplyPendingMaintenanceActionResponseTypeDef,
-    BatchStartRecommendationsResponseTypeDef,
-    CancelReplicationTaskAssessmentRunResponseTypeDef,
+    ApplyPendingMaintenanceActionResponseOutputTypeDef,
+    BatchStartRecommendationsResponseOutputTypeDef,
+    CancelReplicationTaskAssessmentRunResponseOutputTypeDef,
     ComputeConfigTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreateEventSubscriptionResponseTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
-    CreateReplicationConfigResponseTypeDef,
-    CreateReplicationInstanceResponseTypeDef,
-    CreateReplicationSubnetGroupResponseTypeDef,
-    CreateReplicationTaskResponseTypeDef,
-    DeleteCertificateResponseTypeDef,
-    DeleteConnectionResponseTypeDef,
-    DeleteEndpointResponseTypeDef,
-    DeleteEventSubscriptionResponseTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
-    DeleteReplicationConfigResponseTypeDef,
-    DeleteReplicationInstanceResponseTypeDef,
-    DeleteReplicationTaskAssessmentRunResponseTypeDef,
-    DeleteReplicationTaskResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
-    DescribeCertificatesResponseTypeDef,
-    DescribeConnectionsResponseTypeDef,
-    DescribeEndpointSettingsResponseTypeDef,
-    DescribeEndpointsResponseTypeDef,
-    DescribeEndpointTypesResponseTypeDef,
-    DescribeEventCategoriesResponseTypeDef,
-    DescribeEventsResponseTypeDef,
-    DescribeEventSubscriptionsResponseTypeDef,
-    DescribeFleetAdvisorCollectorsResponseTypeDef,
-    DescribeFleetAdvisorDatabasesResponseTypeDef,
-    DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
-    DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
-    DescribeFleetAdvisorSchemasResponseTypeDef,
-    DescribeOrderableReplicationInstancesResponseTypeDef,
-    DescribePendingMaintenanceActionsResponseTypeDef,
-    DescribeRecommendationLimitationsResponseTypeDef,
-    DescribeRecommendationsResponseTypeDef,
-    DescribeRefreshSchemasStatusResponseTypeDef,
-    DescribeReplicationConfigsResponseTypeDef,
-    DescribeReplicationInstancesResponseTypeDef,
-    DescribeReplicationInstanceTaskLogsResponseTypeDef,
-    DescribeReplicationsResponseTypeDef,
-    DescribeReplicationSubnetGroupsResponseTypeDef,
-    DescribeReplicationTableStatisticsResponseTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
-    DescribeReplicationTaskAssessmentRunsResponseTypeDef,
-    DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
-    DescribeReplicationTasksResponseTypeDef,
-    DescribeSchemasResponseTypeDef,
-    DescribeTableStatisticsResponseTypeDef,
+    CreateEndpointResponseOutputTypeDef,
+    CreateEventSubscriptionResponseOutputTypeDef,
+    CreateFleetAdvisorCollectorResponseOutputTypeDef,
+    CreateReplicationConfigResponseOutputTypeDef,
+    CreateReplicationInstanceResponseOutputTypeDef,
+    CreateReplicationSubnetGroupResponseOutputTypeDef,
+    CreateReplicationTaskResponseOutputTypeDef,
+    DeleteCertificateResponseOutputTypeDef,
+    DeleteConnectionResponseOutputTypeDef,
+    DeleteEndpointResponseOutputTypeDef,
+    DeleteEventSubscriptionResponseOutputTypeDef,
+    DeleteFleetAdvisorDatabasesResponseOutputTypeDef,
+    DeleteReplicationConfigResponseOutputTypeDef,
+    DeleteReplicationInstanceResponseOutputTypeDef,
+    DeleteReplicationTaskAssessmentRunResponseOutputTypeDef,
+    DeleteReplicationTaskResponseOutputTypeDef,
+    DescribeAccountAttributesResponseOutputTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseOutputTypeDef,
+    DescribeCertificatesResponseOutputTypeDef,
+    DescribeConnectionsResponseOutputTypeDef,
+    DescribeEndpointSettingsResponseOutputTypeDef,
+    DescribeEndpointsResponseOutputTypeDef,
+    DescribeEndpointTypesResponseOutputTypeDef,
+    DescribeEventCategoriesResponseOutputTypeDef,
+    DescribeEventsResponseOutputTypeDef,
+    DescribeEventSubscriptionsResponseOutputTypeDef,
+    DescribeFleetAdvisorCollectorsResponseOutputTypeDef,
+    DescribeFleetAdvisorDatabasesResponseOutputTypeDef,
+    DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef,
+    DescribeFleetAdvisorSchemasResponseOutputTypeDef,
+    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
+    DescribePendingMaintenanceActionsResponseOutputTypeDef,
+    DescribeRecommendationLimitationsResponseOutputTypeDef,
+    DescribeRecommendationsResponseOutputTypeDef,
+    DescribeRefreshSchemasStatusResponseOutputTypeDef,
+    DescribeReplicationConfigsResponseOutputTypeDef,
+    DescribeReplicationInstancesResponseOutputTypeDef,
+    DescribeReplicationInstanceTaskLogsResponseOutputTypeDef,
+    DescribeReplicationsResponseOutputTypeDef,
+    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
+    DescribeReplicationTableStatisticsResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef,
+    DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef,
+    DescribeReplicationTasksResponseOutputTypeDef,
+    DescribeSchemasResponseOutputTypeDef,
+    DescribeTableStatisticsResponseOutputTypeDef,
     DmsTransferSettingsTypeDef,
     DocDbSettingsTypeDef,
     DynamoDbSettingsTypeDef,
     ElasticsearchSettingsTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GcpMySQLSettingsTypeDef,
     IBMDb2SettingsTypeDef,
-    ImportCertificateResponseTypeDef,
+    ImportCertificateResponseOutputTypeDef,
     KafkaSettingsTypeDef,
     KinesisSettingsTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     MicrosoftSQLServerSettingsTypeDef,
-    ModifyEndpointResponseTypeDef,
-    ModifyEventSubscriptionResponseTypeDef,
-    ModifyReplicationConfigResponseTypeDef,
-    ModifyReplicationInstanceResponseTypeDef,
-    ModifyReplicationSubnetGroupResponseTypeDef,
-    ModifyReplicationTaskResponseTypeDef,
+    ModifyEndpointResponseOutputTypeDef,
+    ModifyEventSubscriptionResponseOutputTypeDef,
+    ModifyReplicationConfigResponseOutputTypeDef,
+    ModifyReplicationInstanceResponseOutputTypeDef,
+    ModifyReplicationSubnetGroupResponseOutputTypeDef,
+    ModifyReplicationTaskResponseOutputTypeDef,
     MongoDbSettingsTypeDef,
-    MoveReplicationTaskResponseTypeDef,
+    MoveReplicationTaskResponseOutputTypeDef,
     MySQLSettingsTypeDef,
     NeptuneSettingsTypeDef,
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
-    RebootReplicationInstanceResponseTypeDef,
+    RebootReplicationInstanceResponseOutputTypeDef,
     RecommendationSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
-    RefreshSchemasResponseTypeDef,
-    ReloadReplicationTablesResponseTypeDef,
-    ReloadTablesResponseTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
+    RefreshSchemasResponseOutputTypeDef,
+    ReloadReplicationTablesResponseOutputTypeDef,
+    ReloadTablesResponseOutputTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseOutputTypeDef,
     S3SettingsTypeDef,
     StartRecommendationsRequestEntryTypeDef,
-    StartReplicationResponseTypeDef,
-    StartReplicationTaskAssessmentResponseTypeDef,
-    StartReplicationTaskAssessmentRunResponseTypeDef,
-    StartReplicationTaskResponseTypeDef,
-    StopReplicationResponseTypeDef,
-    StopReplicationTaskResponseTypeDef,
+    StartReplicationResponseOutputTypeDef,
+    StartReplicationTaskAssessmentResponseOutputTypeDef,
+    StartReplicationTaskAssessmentRunResponseOutputTypeDef,
+    StartReplicationTaskResponseOutputTypeDef,
+    StopReplicationResponseOutputTypeDef,
+    StopReplicationTaskResponseOutputTypeDef,
     SybaseSettingsTypeDef,
     TableToReloadTypeDef,
     TagTypeDef,
-    TestConnectionResponseTypeDef,
+    TestConnectionResponseOutputTypeDef,
     TimestreamSettingsTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseOutputTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     ReplicationInstanceAvailableWaiter,
     ReplicationInstanceDeletedWaiter,
     ReplicationTaskDeletedWaiter,
     ReplicationTaskReadyWaiter,
@@ -226,26 +226,26 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.add_tags_to_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#add_tags_to_resource)
         """
 
     def apply_pending_maintenance_action(
         self, *, ReplicationInstanceArn: str, ApplyAction: str, OptInType: str
-    ) -> ApplyPendingMaintenanceActionResponseTypeDef:
+    ) -> ApplyPendingMaintenanceActionResponseOutputTypeDef:
         """
         Applies a pending maintenance action to a resource (for example, to a
         replication instance).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.apply_pending_maintenance_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#apply_pending_maintenance_action)
         """
 
     def batch_start_recommendations(
         self, *, Data: Sequence[StartRecommendationsRequestEntryTypeDef] = ...
-    ) -> BatchStartRecommendationsResponseTypeDef:
+    ) -> BatchStartRecommendationsResponseOutputTypeDef:
         """
         Starts the analysis of up to 20 source databases to recommend target engines for
         each source database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.batch_start_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#batch_start_recommendations)
         """
@@ -256,15 +256,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#can_paginate)
         """
 
     def cancel_replication_task_assessment_run(
         self, *, ReplicationTaskAssessmentRunArn: str
-    ) -> CancelReplicationTaskAssessmentRunResponseTypeDef:
+    ) -> CancelReplicationTaskAssessmentRunResponseOutputTypeDef:
         """
         Cancels a single premigration assessment run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.cancel_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#cancel_replication_task_assessment_run)
         """
 
@@ -310,15 +310,15 @@
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
         TimestreamSettings: TimestreamSettingsTypeDef = ...
-    ) -> CreateEndpointResponseTypeDef:
+    ) -> CreateEndpointResponseOutputTypeDef:
         """
         Creates an endpoint using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_endpoint)
         """
 
@@ -328,30 +328,30 @@
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEventSubscriptionResponseTypeDef:
+    ) -> CreateEventSubscriptionResponseOutputTypeDef:
         """
         Creates an DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_event_subscription)
         """
 
     def create_fleet_advisor_collector(
         self,
         *,
         CollectorName: str,
         ServiceAccessRoleArn: str,
         S3BucketName: str,
         Description: str = ...
-    ) -> CreateFleetAdvisorCollectorResponseTypeDef:
+    ) -> CreateFleetAdvisorCollectorResponseOutputTypeDef:
         """
         Creates a Fleet Advisor collector using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_fleet_advisor_collector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_fleet_advisor_collector)
         """
 
@@ -364,15 +364,15 @@
         ComputeConfig: ComputeConfigTypeDef,
         ReplicationType: MigrationTypeValueType,
         TableMappings: str,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ResourceIdentifier: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateReplicationConfigResponseTypeDef:
+    ) -> CreateReplicationConfigResponseOutputTypeDef:
         """
         Creates a configuration that you can later provide to configure and start an DMS
         Serverless replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_config)
         """
@@ -392,30 +392,30 @@
         AutoMinorVersionUpgrade: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         PubliclyAccessible: bool = ...,
         DnsNameServers: str = ...,
         ResourceIdentifier: str = ...,
         NetworkType: str = ...
-    ) -> CreateReplicationInstanceResponseTypeDef:
+    ) -> CreateReplicationInstanceResponseOutputTypeDef:
         """
         Creates the replication instance using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_instance)
         """
 
     def create_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         ReplicationSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateReplicationSubnetGroupResponseTypeDef:
+    ) -> CreateReplicationSubnetGroupResponseOutputTypeDef:
         """
         Creates a replication subnet group given a list of the subnet IDs in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_subnet_group)
         """
 
@@ -431,51 +431,51 @@
         ReplicationTaskSettings: str = ...,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TaskData: str = ...,
         ResourceIdentifier: str = ...
-    ) -> CreateReplicationTaskResponseTypeDef:
+    ) -> CreateReplicationTaskResponseOutputTypeDef:
         """
         Creates a replication task using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_task)
         """
 
-    def delete_certificate(self, *, CertificateArn: str) -> DeleteCertificateResponseTypeDef:
+    def delete_certificate(self, *, CertificateArn: str) -> DeleteCertificateResponseOutputTypeDef:
         """
         Deletes the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_certificate)
         """
 
     def delete_connection(
         self, *, EndpointArn: str, ReplicationInstanceArn: str
-    ) -> DeleteConnectionResponseTypeDef:
+    ) -> DeleteConnectionResponseOutputTypeDef:
         """
         Deletes the connection between a replication instance and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_connection)
         """
 
-    def delete_endpoint(self, *, EndpointArn: str) -> DeleteEndpointResponseTypeDef:
+    def delete_endpoint(self, *, EndpointArn: str) -> DeleteEndpointResponseOutputTypeDef:
         """
         Deletes the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_endpoint)
         """
 
     def delete_event_subscription(
         self, *, SubscriptionName: str
-    ) -> DeleteEventSubscriptionResponseTypeDef:
+    ) -> DeleteEventSubscriptionResponseOutputTypeDef:
         """
         Deletes an DMS event subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_event_subscription)
         """
 
@@ -487,35 +487,35 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_fleet_advisor_collector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_fleet_advisor_collector)
         """
 
     def delete_fleet_advisor_databases(
         self, *, DatabaseIds: Sequence[str]
-    ) -> DeleteFleetAdvisorDatabasesResponseTypeDef:
+    ) -> DeleteFleetAdvisorDatabasesResponseOutputTypeDef:
         """
         Deletes the specified Fleet Advisor collector databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_fleet_advisor_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_fleet_advisor_databases)
         """
 
     def delete_replication_config(
         self, *, ReplicationConfigArn: str
-    ) -> DeleteReplicationConfigResponseTypeDef:
+    ) -> DeleteReplicationConfigResponseOutputTypeDef:
         """
         Deletes an DMS Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_config)
         """
 
     def delete_replication_instance(
         self, *, ReplicationInstanceArn: str
-    ) -> DeleteReplicationInstanceResponseTypeDef:
+    ) -> DeleteReplicationInstanceResponseOutputTypeDef:
         """
         Deletes the specified replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_instance)
         """
 
@@ -527,33 +527,33 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_subnet_group)
         """
 
     def delete_replication_task(
         self, *, ReplicationTaskArn: str
-    ) -> DeleteReplicationTaskResponseTypeDef:
+    ) -> DeleteReplicationTaskResponseOutputTypeDef:
         """
         Deletes the specified replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_task)
         """
 
     def delete_replication_task_assessment_run(
         self, *, ReplicationTaskAssessmentRunArn: str
-    ) -> DeleteReplicationTaskAssessmentRunResponseTypeDef:
+    ) -> DeleteReplicationTaskAssessmentRunResponseOutputTypeDef:
         """
         Deletes the record of a single premigration assessment run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_task_assessment_run)
         """
 
-    def describe_account_attributes(self) -> DescribeAccountAttributesResponseTypeDef:
+    def describe_account_attributes(self) -> DescribeAccountAttributesResponseOutputTypeDef:
         """
         Lists all of the DMS attributes for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_account_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_account_attributes)
         """
 
@@ -563,78 +563,78 @@
         ReplicationTaskArn: str = ...,
         ReplicationInstanceArn: str = ...,
         SourceEngineName: str = ...,
         TargetEngineName: str = ...,
         MigrationType: MigrationTypeValueType = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeApplicableIndividualAssessmentsResponseTypeDef:
+    ) -> DescribeApplicableIndividualAssessmentsResponseOutputTypeDef:
         """
         Provides a list of individual assessments that you can specify for a new
         premigration assessment run, given one or more parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_applicable_individual_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_applicable_individual_assessments)
         """
 
     def describe_certificates(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeCertificatesResponseTypeDef:
+    ) -> DescribeCertificatesResponseOutputTypeDef:
         """
         Provides a description of the certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_certificates)
         """
 
     def describe_connections(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeConnectionsResponseTypeDef:
+    ) -> DescribeConnectionsResponseOutputTypeDef:
         """
         Describes the status of the connections that have been made between the
         replication instance and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_connections)
         """
 
     def describe_endpoint_settings(
         self, *, EngineName: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointSettingsResponseTypeDef:
+    ) -> DescribeEndpointSettingsResponseOutputTypeDef:
         """
         Returns information about the possible endpoint settings available when you
         create an endpoint for a specific database engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoint_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoint_settings)
         """
 
     def describe_endpoint_types(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointTypesResponseTypeDef:
+    ) -> DescribeEndpointTypesResponseOutputTypeDef:
         """
         Returns information about the type of endpoints available.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoint_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoint_types)
         """
 
     def describe_endpoints(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointsResponseTypeDef:
+    ) -> DescribeEndpointsResponseOutputTypeDef:
         """
         Returns information about the endpoints for your account in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoints)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoints)
         """
 
     def describe_event_categories(
         self, *, SourceType: str = ..., Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeEventCategoriesResponseTypeDef:
+    ) -> DescribeEventCategoriesResponseOutputTypeDef:
         """
         Lists categories for all event source types, or, if specified, for a specified
         source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_event_categories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_event_categories)
         """
@@ -642,15 +642,15 @@
     def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeEventSubscriptionsResponseTypeDef:
+    ) -> DescribeEventSubscriptionsResponseOutputTypeDef:
         """
         Lists all the event subscriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_event_subscriptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_event_subscriptions)
         """
 
@@ -662,77 +662,77 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeEventsResponseTypeDef:
+    ) -> DescribeEventsResponseOutputTypeDef:
         """
         Lists events for a given source identifier and source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_events)
         """
 
     def describe_fleet_advisor_collectors(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorCollectorsResponseTypeDef:
+    ) -> DescribeFleetAdvisorCollectorsResponseOutputTypeDef:
         """
         Returns a list of the Fleet Advisor collectors in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_collectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_collectors)
         """
 
     def describe_fleet_advisor_databases(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorDatabasesResponseTypeDef:
+    ) -> DescribeFleetAdvisorDatabasesResponseOutputTypeDef:
         """
         Returns a list of Fleet Advisor databases in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_databases)
         """
 
     def describe_fleet_advisor_lsa_analysis(
         self, *, MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorLsaAnalysisResponseTypeDef:
+    ) -> DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef:
         """
         Provides descriptions of large-scale assessment (LSA) analyses produced by your
         Fleet Advisor collectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_lsa_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_lsa_analysis)
         """
 
     def describe_fleet_advisor_schema_object_summary(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef:
+    ) -> DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef:
         """
         Provides descriptions of the schemas discovered by your Fleet Advisor
         collectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_schema_object_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_schema_object_summary)
         """
 
     def describe_fleet_advisor_schemas(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorSchemasResponseTypeDef:
+    ) -> DescribeFleetAdvisorSchemasResponseOutputTypeDef:
         """
         Returns a list of schemas detected by Fleet Advisor Collectors in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_schemas)
         """
 
     def describe_orderable_replication_instances(
         self, *, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeOrderableReplicationInstancesResponseTypeDef:
+    ) -> DescribeOrderableReplicationInstancesResponseOutputTypeDef:
         """
         Returns information about the replication instance types that can be created in
         the specified region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_orderable_replication_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_orderable_replication_instances)
         """
@@ -740,190 +740,190 @@
     def describe_pending_maintenance_actions(
         self,
         *,
         ReplicationInstanceArn: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...
-    ) -> DescribePendingMaintenanceActionsResponseTypeDef:
+    ) -> DescribePendingMaintenanceActionsResponseOutputTypeDef:
         """
         For internal use only See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/dms-2016-01-01/DescribePendingMaintenanceActions).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_pending_maintenance_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_pending_maintenance_actions)
         """
 
     def describe_recommendation_limitations(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeRecommendationLimitationsResponseTypeDef:
+    ) -> DescribeRecommendationLimitationsResponseOutputTypeDef:
         """
         Returns a paginated list of limitations for recommendations of target Amazon Web
         Services engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_recommendation_limitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_recommendation_limitations)
         """
 
     def describe_recommendations(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeRecommendationsResponseTypeDef:
+    ) -> DescribeRecommendationsResponseOutputTypeDef:
         """
         Returns a paginated list of target engine recommendations for your source
         databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_recommendations)
         """
 
     def describe_refresh_schemas_status(
         self, *, EndpointArn: str
-    ) -> DescribeRefreshSchemasStatusResponseTypeDef:
+    ) -> DescribeRefreshSchemasStatusResponseOutputTypeDef:
         """
         Returns the status of the RefreshSchemas operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_refresh_schemas_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_refresh_schemas_status)
         """
 
     def describe_replication_configs(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationConfigsResponseTypeDef:
+    ) -> DescribeReplicationConfigsResponseOutputTypeDef:
         """
         Returns one or more existing DMS Serverless replication configurations as a list
         of structures.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_configs)
         """
 
     def describe_replication_instance_task_logs(
         self, *, ReplicationInstanceArn: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationInstanceTaskLogsResponseTypeDef:
+    ) -> DescribeReplicationInstanceTaskLogsResponseOutputTypeDef:
         """
         Returns information about the task logs for the specified task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_instance_task_logs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_instance_task_logs)
         """
 
     def describe_replication_instances(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationInstancesResponseTypeDef:
+    ) -> DescribeReplicationInstancesResponseOutputTypeDef:
         """
         Returns information about replication instances for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_instances)
         """
 
     def describe_replication_subnet_groups(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationSubnetGroupsResponseTypeDef:
+    ) -> DescribeReplicationSubnetGroupsResponseOutputTypeDef:
         """
         Returns information about the replication subnet groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_subnet_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_subnet_groups)
         """
 
     def describe_replication_table_statistics(
         self,
         *,
         ReplicationConfigArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeReplicationTableStatisticsResponseTypeDef:
+    ) -> DescribeReplicationTableStatisticsResponseOutputTypeDef:
         """
         Returns table and schema statistics for one or more provisioned replications
         that use a given DMS Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_table_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_table_statistics)
         """
 
     def describe_replication_task_assessment_results(
         self, *, ReplicationTaskArn: str = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskAssessmentResultsResponseTypeDef:
+    ) -> DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef:
         """
         Returns the task assessment results from the Amazon S3 bucket that DMS creates
         in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_assessment_results)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_assessment_results)
         """
 
     def describe_replication_task_assessment_runs(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskAssessmentRunsResponseTypeDef:
+    ) -> DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef:
         """
         Returns a paginated list of premigration assessment runs based on filter
         settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_assessment_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_assessment_runs)
         """
 
     def describe_replication_task_individual_assessments(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskIndividualAssessmentsResponseTypeDef:
+    ) -> DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef:
         """
         Returns a paginated list of individual assessments based on filter settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_individual_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_individual_assessments)
         """
 
     def describe_replication_tasks(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...
-    ) -> DescribeReplicationTasksResponseTypeDef:
+    ) -> DescribeReplicationTasksResponseOutputTypeDef:
         """
         Returns information about replication tasks for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_tasks)
         """
 
     def describe_replications(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationsResponseTypeDef:
+    ) -> DescribeReplicationsResponseOutputTypeDef:
         """
         Provides details on replication progress by returning status information for one
         or more provisioned DMS Serverless replications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replications)
         """
 
     def describe_schemas(
         self, *, EndpointArn: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeSchemasResponseTypeDef:
+    ) -> DescribeSchemasResponseOutputTypeDef:
         """
         Returns information about the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_schemas)
         """
 
     def describe_table_statistics(
         self,
         *,
         ReplicationTaskArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeTableStatisticsResponseTypeDef:
+    ) -> DescribeTableStatisticsResponseOutputTypeDef:
         """
         Returns table statistics on the database migration task, including table name,
         rows inserted, rows updated, and rows deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_table_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_table_statistics)
         """
@@ -945,25 +945,25 @@
     def import_certificate(
         self,
         *,
         CertificateIdentifier: str,
         CertificatePem: str = ...,
         CertificateWallet: Union[str, bytes, IO[Any], StreamingBody] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> ImportCertificateResponseTypeDef:
+    ) -> ImportCertificateResponseOutputTypeDef:
         """
         Uploads the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.import_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#import_certificate)
         """
 
     def list_tags_for_resource(
         self, *, ResourceArn: str = ..., ResourceArnList: Sequence[str] = ...
-    ) -> ListTagsForResourceResponseTypeDef:
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Lists all metadata tags attached to an DMS resource, including replication
         instance, endpoint, subnet group, and migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#list_tags_for_resource)
         """
@@ -1001,15 +1001,15 @@
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
         TimestreamSettings: TimestreamSettingsTypeDef = ...
-    ) -> ModifyEndpointResponseTypeDef:
+    ) -> ModifyEndpointResponseOutputTypeDef:
         """
         Modifies the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_endpoint)
         """
 
@@ -1017,15 +1017,15 @@
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         Enabled: bool = ...
-    ) -> ModifyEventSubscriptionResponseTypeDef:
+    ) -> ModifyEventSubscriptionResponseOutputTypeDef:
         """
         Modifies an existing DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_event_subscription)
         """
 
@@ -1037,15 +1037,15 @@
         ReplicationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ComputeConfig: ComputeConfigTypeDef = ...,
         SourceEndpointArn: str = ...,
         TargetEndpointArn: str = ...
-    ) -> ModifyReplicationConfigResponseTypeDef:
+    ) -> ModifyReplicationConfigResponseOutputTypeDef:
         """
         Modifies an existing DMS Serverless replication configuration that you can use
         to start a replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_config)
         """
@@ -1061,29 +1061,29 @@
         PreferredMaintenanceWindow: str = ...,
         MultiAZ: bool = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...,
         AutoMinorVersionUpgrade: bool = ...,
         ReplicationInstanceIdentifier: str = ...,
         NetworkType: str = ...
-    ) -> ModifyReplicationInstanceResponseTypeDef:
+    ) -> ModifyReplicationInstanceResponseOutputTypeDef:
         """
         Modifies the replication instance to apply new settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_instance)
         """
 
     def modify_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         SubnetIds: Sequence[str],
         ReplicationSubnetGroupDescription: str = ...
-    ) -> ModifyReplicationSubnetGroupResponseTypeDef:
+    ) -> ModifyReplicationSubnetGroupResponseOutputTypeDef:
         """
         Modifies the settings for the specified replication subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_subnet_group)
         """
 
@@ -1095,79 +1095,79 @@
         MigrationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationTaskSettings: str = ...,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         TaskData: str = ...
-    ) -> ModifyReplicationTaskResponseTypeDef:
+    ) -> ModifyReplicationTaskResponseOutputTypeDef:
         """
         Modifies the specified replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_task)
         """
 
     def move_replication_task(
         self, *, ReplicationTaskArn: str, TargetReplicationInstanceArn: str
-    ) -> MoveReplicationTaskResponseTypeDef:
+    ) -> MoveReplicationTaskResponseOutputTypeDef:
         """
         Moves a replication task from its current replication instance to a different
         target replication instance using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.move_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#move_replication_task)
         """
 
     def reboot_replication_instance(
         self,
         *,
         ReplicationInstanceArn: str,
         ForceFailover: bool = ...,
         ForcePlannedFailover: bool = ...
-    ) -> RebootReplicationInstanceResponseTypeDef:
+    ) -> RebootReplicationInstanceResponseOutputTypeDef:
         """
         Reboots a replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reboot_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reboot_replication_instance)
         """
 
     def refresh_schemas(
         self, *, EndpointArn: str, ReplicationInstanceArn: str
-    ) -> RefreshSchemasResponseTypeDef:
+    ) -> RefreshSchemasResponseOutputTypeDef:
         """
         Populates the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.refresh_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#refresh_schemas)
         """
 
     def reload_replication_tables(
         self,
         *,
         ReplicationConfigArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
         ReloadOption: ReloadOptionValueType = ...
-    ) -> ReloadReplicationTablesResponseTypeDef:
+    ) -> ReloadReplicationTablesResponseOutputTypeDef:
         """
         Reloads the target database table with the source data for a given DMS
         Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_replication_tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reload_replication_tables)
         """
 
     def reload_tables(
         self,
         *,
         ReplicationTaskArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
         ReloadOption: ReloadOptionValueType = ...
-    ) -> ReloadTablesResponseTypeDef:
+    ) -> ReloadTablesResponseOutputTypeDef:
         """
         Reloads the target database table with the source data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reload_tables)
         """
 
@@ -1178,15 +1178,15 @@
         Removes metadata tags from an DMS resource, including replication instance,
         endpoint, subnet group, and migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.remove_tags_from_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#remove_tags_from_resource)
         """
 
-    def run_fleet_advisor_lsa_analysis(self) -> RunFleetAdvisorLsaAnalysisResponseTypeDef:
+    def run_fleet_advisor_lsa_analysis(self) -> RunFleetAdvisorLsaAnalysisResponseOutputTypeDef:
         """
         Runs large-scale assessment (LSA) analysis on every Fleet Advisor collector in
         your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.run_fleet_advisor_lsa_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#run_fleet_advisor_lsa_analysis)
         """
@@ -1206,15 +1206,15 @@
         self,
         *,
         ReplicationConfigArn: str,
         StartReplicationType: str,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...
-    ) -> StartReplicationResponseTypeDef:
+    ) -> StartReplicationResponseOutputTypeDef:
         """
         For a given DMS Serverless replication configuration, DMS connects to the source
         endpoint and collects the metadata to analyze the replication workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication)
         """
@@ -1223,25 +1223,25 @@
         self,
         *,
         ReplicationTaskArn: str,
         StartReplicationTaskType: StartReplicationTaskTypeValueType,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...
-    ) -> StartReplicationTaskResponseTypeDef:
+    ) -> StartReplicationTaskResponseOutputTypeDef:
         """
         Starts the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task)
         """
 
     def start_replication_task_assessment(
         self, *, ReplicationTaskArn: str
-    ) -> StartReplicationTaskAssessmentResponseTypeDef:
+    ) -> StartReplicationTaskAssessmentResponseOutputTypeDef:
         """
         Starts the replication task assessment for unsupported data types in the source
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task_assessment)
         """
@@ -1254,55 +1254,57 @@
         ResultLocationBucket: str,
         AssessmentRunName: str,
         ResultLocationFolder: str = ...,
         ResultEncryptionMode: str = ...,
         ResultKmsKeyArn: str = ...,
         IncludeOnly: Sequence[str] = ...,
         Exclude: Sequence[str] = ...
-    ) -> StartReplicationTaskAssessmentRunResponseTypeDef:
+    ) -> StartReplicationTaskAssessmentRunResponseOutputTypeDef:
         """
         Starts a new premigration assessment run for one or more individual assessments
         of a migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task_assessment_run)
         """
 
-    def stop_replication(self, *, ReplicationConfigArn: str) -> StopReplicationResponseTypeDef:
+    def stop_replication(
+        self, *, ReplicationConfigArn: str
+    ) -> StopReplicationResponseOutputTypeDef:
         """
         For a given DMS Serverless replication configuration, DMS stops any and all
         ongoing DMS Serverless replications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#stop_replication)
         """
 
     def stop_replication_task(
         self, *, ReplicationTaskArn: str
-    ) -> StopReplicationTaskResponseTypeDef:
+    ) -> StopReplicationTaskResponseOutputTypeDef:
         """
         Stops the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#stop_replication_task)
         """
 
     def test_connection(
         self, *, ReplicationInstanceArn: str, EndpointArn: str
-    ) -> TestConnectionResponseTypeDef:
+    ) -> TestConnectionResponseOutputTypeDef:
         """
         Tests the connection between the replication instance and the endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.test_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#test_connection)
         """
 
     def update_subscriptions_to_event_bridge(
         self, *, ForceMove: bool = ...
-    ) -> UpdateSubscriptionsToEventBridgeResponseTypeDef:
+    ) -> UpdateSubscriptionsToEventBridgeResponseOutputTypeDef:
         """
         Migrates 10 active and enabled Amazon SNS subscriptions at a time and converts
         them to corresponding Amazon EventBridge rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.update_subscriptions_to_event_bridge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#update_subscriptions_to_event_bridge)
         """
```

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/client.pyi` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -39,113 +39,113 @@
     DescribeReplicationSubnetGroupsPaginator,
     DescribeReplicationTaskAssessmentResultsPaginator,
     DescribeReplicationTasksPaginator,
     DescribeSchemasPaginator,
     DescribeTableStatisticsPaginator,
 )
 from .type_defs import (
-    ApplyPendingMaintenanceActionResponseTypeDef,
-    BatchStartRecommendationsResponseTypeDef,
-    CancelReplicationTaskAssessmentRunResponseTypeDef,
+    ApplyPendingMaintenanceActionResponseOutputTypeDef,
+    BatchStartRecommendationsResponseOutputTypeDef,
+    CancelReplicationTaskAssessmentRunResponseOutputTypeDef,
     ComputeConfigTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreateEventSubscriptionResponseTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
-    CreateReplicationConfigResponseTypeDef,
-    CreateReplicationInstanceResponseTypeDef,
-    CreateReplicationSubnetGroupResponseTypeDef,
-    CreateReplicationTaskResponseTypeDef,
-    DeleteCertificateResponseTypeDef,
-    DeleteConnectionResponseTypeDef,
-    DeleteEndpointResponseTypeDef,
-    DeleteEventSubscriptionResponseTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
-    DeleteReplicationConfigResponseTypeDef,
-    DeleteReplicationInstanceResponseTypeDef,
-    DeleteReplicationTaskAssessmentRunResponseTypeDef,
-    DeleteReplicationTaskResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
-    DescribeCertificatesResponseTypeDef,
-    DescribeConnectionsResponseTypeDef,
-    DescribeEndpointSettingsResponseTypeDef,
-    DescribeEndpointsResponseTypeDef,
-    DescribeEndpointTypesResponseTypeDef,
-    DescribeEventCategoriesResponseTypeDef,
-    DescribeEventsResponseTypeDef,
-    DescribeEventSubscriptionsResponseTypeDef,
-    DescribeFleetAdvisorCollectorsResponseTypeDef,
-    DescribeFleetAdvisorDatabasesResponseTypeDef,
-    DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
-    DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
-    DescribeFleetAdvisorSchemasResponseTypeDef,
-    DescribeOrderableReplicationInstancesResponseTypeDef,
-    DescribePendingMaintenanceActionsResponseTypeDef,
-    DescribeRecommendationLimitationsResponseTypeDef,
-    DescribeRecommendationsResponseTypeDef,
-    DescribeRefreshSchemasStatusResponseTypeDef,
-    DescribeReplicationConfigsResponseTypeDef,
-    DescribeReplicationInstancesResponseTypeDef,
-    DescribeReplicationInstanceTaskLogsResponseTypeDef,
-    DescribeReplicationsResponseTypeDef,
-    DescribeReplicationSubnetGroupsResponseTypeDef,
-    DescribeReplicationTableStatisticsResponseTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
-    DescribeReplicationTaskAssessmentRunsResponseTypeDef,
-    DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
-    DescribeReplicationTasksResponseTypeDef,
-    DescribeSchemasResponseTypeDef,
-    DescribeTableStatisticsResponseTypeDef,
+    CreateEndpointResponseOutputTypeDef,
+    CreateEventSubscriptionResponseOutputTypeDef,
+    CreateFleetAdvisorCollectorResponseOutputTypeDef,
+    CreateReplicationConfigResponseOutputTypeDef,
+    CreateReplicationInstanceResponseOutputTypeDef,
+    CreateReplicationSubnetGroupResponseOutputTypeDef,
+    CreateReplicationTaskResponseOutputTypeDef,
+    DeleteCertificateResponseOutputTypeDef,
+    DeleteConnectionResponseOutputTypeDef,
+    DeleteEndpointResponseOutputTypeDef,
+    DeleteEventSubscriptionResponseOutputTypeDef,
+    DeleteFleetAdvisorDatabasesResponseOutputTypeDef,
+    DeleteReplicationConfigResponseOutputTypeDef,
+    DeleteReplicationInstanceResponseOutputTypeDef,
+    DeleteReplicationTaskAssessmentRunResponseOutputTypeDef,
+    DeleteReplicationTaskResponseOutputTypeDef,
+    DescribeAccountAttributesResponseOutputTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseOutputTypeDef,
+    DescribeCertificatesResponseOutputTypeDef,
+    DescribeConnectionsResponseOutputTypeDef,
+    DescribeEndpointSettingsResponseOutputTypeDef,
+    DescribeEndpointsResponseOutputTypeDef,
+    DescribeEndpointTypesResponseOutputTypeDef,
+    DescribeEventCategoriesResponseOutputTypeDef,
+    DescribeEventsResponseOutputTypeDef,
+    DescribeEventSubscriptionsResponseOutputTypeDef,
+    DescribeFleetAdvisorCollectorsResponseOutputTypeDef,
+    DescribeFleetAdvisorDatabasesResponseOutputTypeDef,
+    DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef,
+    DescribeFleetAdvisorSchemasResponseOutputTypeDef,
+    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
+    DescribePendingMaintenanceActionsResponseOutputTypeDef,
+    DescribeRecommendationLimitationsResponseOutputTypeDef,
+    DescribeRecommendationsResponseOutputTypeDef,
+    DescribeRefreshSchemasStatusResponseOutputTypeDef,
+    DescribeReplicationConfigsResponseOutputTypeDef,
+    DescribeReplicationInstancesResponseOutputTypeDef,
+    DescribeReplicationInstanceTaskLogsResponseOutputTypeDef,
+    DescribeReplicationsResponseOutputTypeDef,
+    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
+    DescribeReplicationTableStatisticsResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef,
+    DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef,
+    DescribeReplicationTasksResponseOutputTypeDef,
+    DescribeSchemasResponseOutputTypeDef,
+    DescribeTableStatisticsResponseOutputTypeDef,
     DmsTransferSettingsTypeDef,
     DocDbSettingsTypeDef,
     DynamoDbSettingsTypeDef,
     ElasticsearchSettingsTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GcpMySQLSettingsTypeDef,
     IBMDb2SettingsTypeDef,
-    ImportCertificateResponseTypeDef,
+    ImportCertificateResponseOutputTypeDef,
     KafkaSettingsTypeDef,
     KinesisSettingsTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     MicrosoftSQLServerSettingsTypeDef,
-    ModifyEndpointResponseTypeDef,
-    ModifyEventSubscriptionResponseTypeDef,
-    ModifyReplicationConfigResponseTypeDef,
-    ModifyReplicationInstanceResponseTypeDef,
-    ModifyReplicationSubnetGroupResponseTypeDef,
-    ModifyReplicationTaskResponseTypeDef,
+    ModifyEndpointResponseOutputTypeDef,
+    ModifyEventSubscriptionResponseOutputTypeDef,
+    ModifyReplicationConfigResponseOutputTypeDef,
+    ModifyReplicationInstanceResponseOutputTypeDef,
+    ModifyReplicationSubnetGroupResponseOutputTypeDef,
+    ModifyReplicationTaskResponseOutputTypeDef,
     MongoDbSettingsTypeDef,
-    MoveReplicationTaskResponseTypeDef,
+    MoveReplicationTaskResponseOutputTypeDef,
     MySQLSettingsTypeDef,
     NeptuneSettingsTypeDef,
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
-    RebootReplicationInstanceResponseTypeDef,
+    RebootReplicationInstanceResponseOutputTypeDef,
     RecommendationSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
-    RefreshSchemasResponseTypeDef,
-    ReloadReplicationTablesResponseTypeDef,
-    ReloadTablesResponseTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
+    RefreshSchemasResponseOutputTypeDef,
+    ReloadReplicationTablesResponseOutputTypeDef,
+    ReloadTablesResponseOutputTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseOutputTypeDef,
     S3SettingsTypeDef,
     StartRecommendationsRequestEntryTypeDef,
-    StartReplicationResponseTypeDef,
-    StartReplicationTaskAssessmentResponseTypeDef,
-    StartReplicationTaskAssessmentRunResponseTypeDef,
-    StartReplicationTaskResponseTypeDef,
-    StopReplicationResponseTypeDef,
-    StopReplicationTaskResponseTypeDef,
+    StartReplicationResponseOutputTypeDef,
+    StartReplicationTaskAssessmentResponseOutputTypeDef,
+    StartReplicationTaskAssessmentRunResponseOutputTypeDef,
+    StartReplicationTaskResponseOutputTypeDef,
+    StopReplicationResponseOutputTypeDef,
+    StopReplicationTaskResponseOutputTypeDef,
     SybaseSettingsTypeDef,
     TableToReloadTypeDef,
     TagTypeDef,
-    TestConnectionResponseTypeDef,
+    TestConnectionResponseOutputTypeDef,
     TimestreamSettingsTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseOutputTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     ReplicationInstanceAvailableWaiter,
     ReplicationInstanceDeletedWaiter,
     ReplicationTaskDeletedWaiter,
     ReplicationTaskReadyWaiter,
@@ -220,25 +220,25 @@
         subnet group, and migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.add_tags_to_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#add_tags_to_resource)
         """
     def apply_pending_maintenance_action(
         self, *, ReplicationInstanceArn: str, ApplyAction: str, OptInType: str
-    ) -> ApplyPendingMaintenanceActionResponseTypeDef:
+    ) -> ApplyPendingMaintenanceActionResponseOutputTypeDef:
         """
         Applies a pending maintenance action to a resource (for example, to a
         replication instance).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.apply_pending_maintenance_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#apply_pending_maintenance_action)
         """
     def batch_start_recommendations(
         self, *, Data: Sequence[StartRecommendationsRequestEntryTypeDef] = ...
-    ) -> BatchStartRecommendationsResponseTypeDef:
+    ) -> BatchStartRecommendationsResponseOutputTypeDef:
         """
         Starts the analysis of up to 20 source databases to recommend target engines for
         each source database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.batch_start_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#batch_start_recommendations)
         """
@@ -247,15 +247,15 @@
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#can_paginate)
         """
     def cancel_replication_task_assessment_run(
         self, *, ReplicationTaskAssessmentRunArn: str
-    ) -> CancelReplicationTaskAssessmentRunResponseTypeDef:
+    ) -> CancelReplicationTaskAssessmentRunResponseOutputTypeDef:
         """
         Cancels a single premigration assessment run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.cancel_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#cancel_replication_task_assessment_run)
         """
     def close(self) -> None:
@@ -299,15 +299,15 @@
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
         TimestreamSettings: TimestreamSettingsTypeDef = ...
-    ) -> CreateEndpointResponseTypeDef:
+    ) -> CreateEndpointResponseOutputTypeDef:
         """
         Creates an endpoint using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_endpoint)
         """
     def create_event_subscription(
@@ -316,29 +316,29 @@
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEventSubscriptionResponseTypeDef:
+    ) -> CreateEventSubscriptionResponseOutputTypeDef:
         """
         Creates an DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_event_subscription)
         """
     def create_fleet_advisor_collector(
         self,
         *,
         CollectorName: str,
         ServiceAccessRoleArn: str,
         S3BucketName: str,
         Description: str = ...
-    ) -> CreateFleetAdvisorCollectorResponseTypeDef:
+    ) -> CreateFleetAdvisorCollectorResponseOutputTypeDef:
         """
         Creates a Fleet Advisor collector using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_fleet_advisor_collector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_fleet_advisor_collector)
         """
     def create_replication_config(
@@ -350,15 +350,15 @@
         ComputeConfig: ComputeConfigTypeDef,
         ReplicationType: MigrationTypeValueType,
         TableMappings: str,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ResourceIdentifier: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateReplicationConfigResponseTypeDef:
+    ) -> CreateReplicationConfigResponseOutputTypeDef:
         """
         Creates a configuration that you can later provide to configure and start an DMS
         Serverless replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_config)
         """
@@ -377,29 +377,29 @@
         AutoMinorVersionUpgrade: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         PubliclyAccessible: bool = ...,
         DnsNameServers: str = ...,
         ResourceIdentifier: str = ...,
         NetworkType: str = ...
-    ) -> CreateReplicationInstanceResponseTypeDef:
+    ) -> CreateReplicationInstanceResponseOutputTypeDef:
         """
         Creates the replication instance using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_instance)
         """
     def create_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         ReplicationSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateReplicationSubnetGroupResponseTypeDef:
+    ) -> CreateReplicationSubnetGroupResponseOutputTypeDef:
         """
         Creates a replication subnet group given a list of the subnet IDs in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_subnet_group)
         """
     def create_replication_task(
@@ -414,47 +414,47 @@
         ReplicationTaskSettings: str = ...,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TaskData: str = ...,
         ResourceIdentifier: str = ...
-    ) -> CreateReplicationTaskResponseTypeDef:
+    ) -> CreateReplicationTaskResponseOutputTypeDef:
         """
         Creates a replication task using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_task)
         """
-    def delete_certificate(self, *, CertificateArn: str) -> DeleteCertificateResponseTypeDef:
+    def delete_certificate(self, *, CertificateArn: str) -> DeleteCertificateResponseOutputTypeDef:
         """
         Deletes the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_certificate)
         """
     def delete_connection(
         self, *, EndpointArn: str, ReplicationInstanceArn: str
-    ) -> DeleteConnectionResponseTypeDef:
+    ) -> DeleteConnectionResponseOutputTypeDef:
         """
         Deletes the connection between a replication instance and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_connection)
         """
-    def delete_endpoint(self, *, EndpointArn: str) -> DeleteEndpointResponseTypeDef:
+    def delete_endpoint(self, *, EndpointArn: str) -> DeleteEndpointResponseOutputTypeDef:
         """
         Deletes the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_endpoint)
         """
     def delete_event_subscription(
         self, *, SubscriptionName: str
-    ) -> DeleteEventSubscriptionResponseTypeDef:
+    ) -> DeleteEventSubscriptionResponseOutputTypeDef:
         """
         Deletes an DMS event subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_event_subscription)
         """
     def delete_fleet_advisor_collector(
@@ -464,33 +464,33 @@
         Deletes the specified Fleet Advisor collector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_fleet_advisor_collector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_fleet_advisor_collector)
         """
     def delete_fleet_advisor_databases(
         self, *, DatabaseIds: Sequence[str]
-    ) -> DeleteFleetAdvisorDatabasesResponseTypeDef:
+    ) -> DeleteFleetAdvisorDatabasesResponseOutputTypeDef:
         """
         Deletes the specified Fleet Advisor collector databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_fleet_advisor_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_fleet_advisor_databases)
         """
     def delete_replication_config(
         self, *, ReplicationConfigArn: str
-    ) -> DeleteReplicationConfigResponseTypeDef:
+    ) -> DeleteReplicationConfigResponseOutputTypeDef:
         """
         Deletes an DMS Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_config)
         """
     def delete_replication_instance(
         self, *, ReplicationInstanceArn: str
-    ) -> DeleteReplicationInstanceResponseTypeDef:
+    ) -> DeleteReplicationInstanceResponseOutputTypeDef:
         """
         Deletes the specified replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_instance)
         """
     def delete_replication_subnet_group(
@@ -500,31 +500,31 @@
         Deletes a subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_subnet_group)
         """
     def delete_replication_task(
         self, *, ReplicationTaskArn: str
-    ) -> DeleteReplicationTaskResponseTypeDef:
+    ) -> DeleteReplicationTaskResponseOutputTypeDef:
         """
         Deletes the specified replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_task)
         """
     def delete_replication_task_assessment_run(
         self, *, ReplicationTaskAssessmentRunArn: str
-    ) -> DeleteReplicationTaskAssessmentRunResponseTypeDef:
+    ) -> DeleteReplicationTaskAssessmentRunResponseOutputTypeDef:
         """
         Deletes the record of a single premigration assessment run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_task_assessment_run)
         """
-    def describe_account_attributes(self) -> DescribeAccountAttributesResponseTypeDef:
+    def describe_account_attributes(self) -> DescribeAccountAttributesResponseOutputTypeDef:
         """
         Lists all of the DMS attributes for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_account_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_account_attributes)
         """
     def describe_applicable_individual_assessments(
@@ -533,87 +533,87 @@
         ReplicationTaskArn: str = ...,
         ReplicationInstanceArn: str = ...,
         SourceEngineName: str = ...,
         TargetEngineName: str = ...,
         MigrationType: MigrationTypeValueType = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeApplicableIndividualAssessmentsResponseTypeDef:
+    ) -> DescribeApplicableIndividualAssessmentsResponseOutputTypeDef:
         """
         Provides a list of individual assessments that you can specify for a new
         premigration assessment run, given one or more parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_applicable_individual_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_applicable_individual_assessments)
         """
     def describe_certificates(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeCertificatesResponseTypeDef:
+    ) -> DescribeCertificatesResponseOutputTypeDef:
         """
         Provides a description of the certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_certificates)
         """
     def describe_connections(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeConnectionsResponseTypeDef:
+    ) -> DescribeConnectionsResponseOutputTypeDef:
         """
         Describes the status of the connections that have been made between the
         replication instance and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_connections)
         """
     def describe_endpoint_settings(
         self, *, EngineName: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointSettingsResponseTypeDef:
+    ) -> DescribeEndpointSettingsResponseOutputTypeDef:
         """
         Returns information about the possible endpoint settings available when you
         create an endpoint for a specific database engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoint_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoint_settings)
         """
     def describe_endpoint_types(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointTypesResponseTypeDef:
+    ) -> DescribeEndpointTypesResponseOutputTypeDef:
         """
         Returns information about the type of endpoints available.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoint_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoint_types)
         """
     def describe_endpoints(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointsResponseTypeDef:
+    ) -> DescribeEndpointsResponseOutputTypeDef:
         """
         Returns information about the endpoints for your account in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoints)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoints)
         """
     def describe_event_categories(
         self, *, SourceType: str = ..., Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeEventCategoriesResponseTypeDef:
+    ) -> DescribeEventCategoriesResponseOutputTypeDef:
         """
         Lists categories for all event source types, or, if specified, for a specified
         source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_event_categories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_event_categories)
         """
     def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeEventSubscriptionsResponseTypeDef:
+    ) -> DescribeEventSubscriptionsResponseOutputTypeDef:
         """
         Lists all the event subscriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_event_subscriptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_event_subscriptions)
         """
     def describe_events(
@@ -624,246 +624,246 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeEventsResponseTypeDef:
+    ) -> DescribeEventsResponseOutputTypeDef:
         """
         Lists events for a given source identifier and source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_events)
         """
     def describe_fleet_advisor_collectors(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorCollectorsResponseTypeDef:
+    ) -> DescribeFleetAdvisorCollectorsResponseOutputTypeDef:
         """
         Returns a list of the Fleet Advisor collectors in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_collectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_collectors)
         """
     def describe_fleet_advisor_databases(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorDatabasesResponseTypeDef:
+    ) -> DescribeFleetAdvisorDatabasesResponseOutputTypeDef:
         """
         Returns a list of Fleet Advisor databases in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_databases)
         """
     def describe_fleet_advisor_lsa_analysis(
         self, *, MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorLsaAnalysisResponseTypeDef:
+    ) -> DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef:
         """
         Provides descriptions of large-scale assessment (LSA) analyses produced by your
         Fleet Advisor collectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_lsa_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_lsa_analysis)
         """
     def describe_fleet_advisor_schema_object_summary(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef:
+    ) -> DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef:
         """
         Provides descriptions of the schemas discovered by your Fleet Advisor
         collectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_schema_object_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_schema_object_summary)
         """
     def describe_fleet_advisor_schemas(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorSchemasResponseTypeDef:
+    ) -> DescribeFleetAdvisorSchemasResponseOutputTypeDef:
         """
         Returns a list of schemas detected by Fleet Advisor Collectors in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_schemas)
         """
     def describe_orderable_replication_instances(
         self, *, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeOrderableReplicationInstancesResponseTypeDef:
+    ) -> DescribeOrderableReplicationInstancesResponseOutputTypeDef:
         """
         Returns information about the replication instance types that can be created in
         the specified region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_orderable_replication_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_orderable_replication_instances)
         """
     def describe_pending_maintenance_actions(
         self,
         *,
         ReplicationInstanceArn: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...
-    ) -> DescribePendingMaintenanceActionsResponseTypeDef:
+    ) -> DescribePendingMaintenanceActionsResponseOutputTypeDef:
         """
         For internal use only See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/dms-2016-01-01/DescribePendingMaintenanceActions).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_pending_maintenance_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_pending_maintenance_actions)
         """
     def describe_recommendation_limitations(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeRecommendationLimitationsResponseTypeDef:
+    ) -> DescribeRecommendationLimitationsResponseOutputTypeDef:
         """
         Returns a paginated list of limitations for recommendations of target Amazon Web
         Services engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_recommendation_limitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_recommendation_limitations)
         """
     def describe_recommendations(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeRecommendationsResponseTypeDef:
+    ) -> DescribeRecommendationsResponseOutputTypeDef:
         """
         Returns a paginated list of target engine recommendations for your source
         databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_recommendations)
         """
     def describe_refresh_schemas_status(
         self, *, EndpointArn: str
-    ) -> DescribeRefreshSchemasStatusResponseTypeDef:
+    ) -> DescribeRefreshSchemasStatusResponseOutputTypeDef:
         """
         Returns the status of the RefreshSchemas operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_refresh_schemas_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_refresh_schemas_status)
         """
     def describe_replication_configs(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationConfigsResponseTypeDef:
+    ) -> DescribeReplicationConfigsResponseOutputTypeDef:
         """
         Returns one or more existing DMS Serverless replication configurations as a list
         of structures.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_configs)
         """
     def describe_replication_instance_task_logs(
         self, *, ReplicationInstanceArn: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationInstanceTaskLogsResponseTypeDef:
+    ) -> DescribeReplicationInstanceTaskLogsResponseOutputTypeDef:
         """
         Returns information about the task logs for the specified task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_instance_task_logs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_instance_task_logs)
         """
     def describe_replication_instances(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationInstancesResponseTypeDef:
+    ) -> DescribeReplicationInstancesResponseOutputTypeDef:
         """
         Returns information about replication instances for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_instances)
         """
     def describe_replication_subnet_groups(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationSubnetGroupsResponseTypeDef:
+    ) -> DescribeReplicationSubnetGroupsResponseOutputTypeDef:
         """
         Returns information about the replication subnet groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_subnet_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_subnet_groups)
         """
     def describe_replication_table_statistics(
         self,
         *,
         ReplicationConfigArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeReplicationTableStatisticsResponseTypeDef:
+    ) -> DescribeReplicationTableStatisticsResponseOutputTypeDef:
         """
         Returns table and schema statistics for one or more provisioned replications
         that use a given DMS Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_table_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_table_statistics)
         """
     def describe_replication_task_assessment_results(
         self, *, ReplicationTaskArn: str = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskAssessmentResultsResponseTypeDef:
+    ) -> DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef:
         """
         Returns the task assessment results from the Amazon S3 bucket that DMS creates
         in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_assessment_results)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_assessment_results)
         """
     def describe_replication_task_assessment_runs(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskAssessmentRunsResponseTypeDef:
+    ) -> DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef:
         """
         Returns a paginated list of premigration assessment runs based on filter
         settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_assessment_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_assessment_runs)
         """
     def describe_replication_task_individual_assessments(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskIndividualAssessmentsResponseTypeDef:
+    ) -> DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef:
         """
         Returns a paginated list of individual assessments based on filter settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_individual_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_individual_assessments)
         """
     def describe_replication_tasks(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...
-    ) -> DescribeReplicationTasksResponseTypeDef:
+    ) -> DescribeReplicationTasksResponseOutputTypeDef:
         """
         Returns information about replication tasks for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_tasks)
         """
     def describe_replications(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationsResponseTypeDef:
+    ) -> DescribeReplicationsResponseOutputTypeDef:
         """
         Provides details on replication progress by returning status information for one
         or more provisioned DMS Serverless replications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replications)
         """
     def describe_schemas(
         self, *, EndpointArn: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeSchemasResponseTypeDef:
+    ) -> DescribeSchemasResponseOutputTypeDef:
         """
         Returns information about the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_schemas)
         """
     def describe_table_statistics(
         self,
         *,
         ReplicationTaskArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeTableStatisticsResponseTypeDef:
+    ) -> DescribeTableStatisticsResponseOutputTypeDef:
         """
         Returns table statistics on the database migration task, including table name,
         rows inserted, rows updated, and rows deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_table_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_table_statistics)
         """
@@ -883,24 +883,24 @@
     def import_certificate(
         self,
         *,
         CertificateIdentifier: str,
         CertificatePem: str = ...,
         CertificateWallet: Union[str, bytes, IO[Any], StreamingBody] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> ImportCertificateResponseTypeDef:
+    ) -> ImportCertificateResponseOutputTypeDef:
         """
         Uploads the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.import_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#import_certificate)
         """
     def list_tags_for_resource(
         self, *, ResourceArn: str = ..., ResourceArnList: Sequence[str] = ...
-    ) -> ListTagsForResourceResponseTypeDef:
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Lists all metadata tags attached to an DMS resource, including replication
         instance, endpoint, subnet group, and migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#list_tags_for_resource)
         """
@@ -937,30 +937,30 @@
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
         TimestreamSettings: TimestreamSettingsTypeDef = ...
-    ) -> ModifyEndpointResponseTypeDef:
+    ) -> ModifyEndpointResponseOutputTypeDef:
         """
         Modifies the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_endpoint)
         """
     def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         Enabled: bool = ...
-    ) -> ModifyEventSubscriptionResponseTypeDef:
+    ) -> ModifyEventSubscriptionResponseOutputTypeDef:
         """
         Modifies an existing DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_event_subscription)
         """
     def modify_replication_config(
@@ -971,15 +971,15 @@
         ReplicationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ComputeConfig: ComputeConfigTypeDef = ...,
         SourceEndpointArn: str = ...,
         TargetEndpointArn: str = ...
-    ) -> ModifyReplicationConfigResponseTypeDef:
+    ) -> ModifyReplicationConfigResponseOutputTypeDef:
         """
         Modifies an existing DMS Serverless replication configuration that you can use
         to start a replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_config)
         """
@@ -994,28 +994,28 @@
         PreferredMaintenanceWindow: str = ...,
         MultiAZ: bool = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...,
         AutoMinorVersionUpgrade: bool = ...,
         ReplicationInstanceIdentifier: str = ...,
         NetworkType: str = ...
-    ) -> ModifyReplicationInstanceResponseTypeDef:
+    ) -> ModifyReplicationInstanceResponseOutputTypeDef:
         """
         Modifies the replication instance to apply new settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_instance)
         """
     def modify_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         SubnetIds: Sequence[str],
         ReplicationSubnetGroupDescription: str = ...
-    ) -> ModifyReplicationSubnetGroupResponseTypeDef:
+    ) -> ModifyReplicationSubnetGroupResponseOutputTypeDef:
         """
         Modifies the settings for the specified replication subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_subnet_group)
         """
     def modify_replication_task(
@@ -1026,74 +1026,74 @@
         MigrationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationTaskSettings: str = ...,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         TaskData: str = ...
-    ) -> ModifyReplicationTaskResponseTypeDef:
+    ) -> ModifyReplicationTaskResponseOutputTypeDef:
         """
         Modifies the specified replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_task)
         """
     def move_replication_task(
         self, *, ReplicationTaskArn: str, TargetReplicationInstanceArn: str
-    ) -> MoveReplicationTaskResponseTypeDef:
+    ) -> MoveReplicationTaskResponseOutputTypeDef:
         """
         Moves a replication task from its current replication instance to a different
         target replication instance using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.move_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#move_replication_task)
         """
     def reboot_replication_instance(
         self,
         *,
         ReplicationInstanceArn: str,
         ForceFailover: bool = ...,
         ForcePlannedFailover: bool = ...
-    ) -> RebootReplicationInstanceResponseTypeDef:
+    ) -> RebootReplicationInstanceResponseOutputTypeDef:
         """
         Reboots a replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reboot_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reboot_replication_instance)
         """
     def refresh_schemas(
         self, *, EndpointArn: str, ReplicationInstanceArn: str
-    ) -> RefreshSchemasResponseTypeDef:
+    ) -> RefreshSchemasResponseOutputTypeDef:
         """
         Populates the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.refresh_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#refresh_schemas)
         """
     def reload_replication_tables(
         self,
         *,
         ReplicationConfigArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
         ReloadOption: ReloadOptionValueType = ...
-    ) -> ReloadReplicationTablesResponseTypeDef:
+    ) -> ReloadReplicationTablesResponseOutputTypeDef:
         """
         Reloads the target database table with the source data for a given DMS
         Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_replication_tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reload_replication_tables)
         """
     def reload_tables(
         self,
         *,
         ReplicationTaskArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
         ReloadOption: ReloadOptionValueType = ...
-    ) -> ReloadTablesResponseTypeDef:
+    ) -> ReloadTablesResponseOutputTypeDef:
         """
         Reloads the target database table with the source data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reload_tables)
         """
     def remove_tags_from_resource(
@@ -1102,15 +1102,15 @@
         """
         Removes metadata tags from an DMS resource, including replication instance,
         endpoint, subnet group, and migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.remove_tags_from_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#remove_tags_from_resource)
         """
-    def run_fleet_advisor_lsa_analysis(self) -> RunFleetAdvisorLsaAnalysisResponseTypeDef:
+    def run_fleet_advisor_lsa_analysis(self) -> RunFleetAdvisorLsaAnalysisResponseOutputTypeDef:
         """
         Runs large-scale assessment (LSA) analysis on every Fleet Advisor collector in
         your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.run_fleet_advisor_lsa_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#run_fleet_advisor_lsa_analysis)
         """
@@ -1128,15 +1128,15 @@
         self,
         *,
         ReplicationConfigArn: str,
         StartReplicationType: str,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...
-    ) -> StartReplicationResponseTypeDef:
+    ) -> StartReplicationResponseOutputTypeDef:
         """
         For a given DMS Serverless replication configuration, DMS connects to the source
         endpoint and collects the metadata to analyze the replication workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication)
         """
@@ -1144,24 +1144,24 @@
         self,
         *,
         ReplicationTaskArn: str,
         StartReplicationTaskType: StartReplicationTaskTypeValueType,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...
-    ) -> StartReplicationTaskResponseTypeDef:
+    ) -> StartReplicationTaskResponseOutputTypeDef:
         """
         Starts the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task)
         """
     def start_replication_task_assessment(
         self, *, ReplicationTaskArn: str
-    ) -> StartReplicationTaskAssessmentResponseTypeDef:
+    ) -> StartReplicationTaskAssessmentResponseOutputTypeDef:
         """
         Starts the replication task assessment for unsupported data types in the source
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task_assessment)
         """
@@ -1173,51 +1173,53 @@
         ResultLocationBucket: str,
         AssessmentRunName: str,
         ResultLocationFolder: str = ...,
         ResultEncryptionMode: str = ...,
         ResultKmsKeyArn: str = ...,
         IncludeOnly: Sequence[str] = ...,
         Exclude: Sequence[str] = ...
-    ) -> StartReplicationTaskAssessmentRunResponseTypeDef:
+    ) -> StartReplicationTaskAssessmentRunResponseOutputTypeDef:
         """
         Starts a new premigration assessment run for one or more individual assessments
         of a migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task_assessment_run)
         """
-    def stop_replication(self, *, ReplicationConfigArn: str) -> StopReplicationResponseTypeDef:
+    def stop_replication(
+        self, *, ReplicationConfigArn: str
+    ) -> StopReplicationResponseOutputTypeDef:
         """
         For a given DMS Serverless replication configuration, DMS stops any and all
         ongoing DMS Serverless replications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#stop_replication)
         """
     def stop_replication_task(
         self, *, ReplicationTaskArn: str
-    ) -> StopReplicationTaskResponseTypeDef:
+    ) -> StopReplicationTaskResponseOutputTypeDef:
         """
         Stops the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#stop_replication_task)
         """
     def test_connection(
         self, *, ReplicationInstanceArn: str, EndpointArn: str
-    ) -> TestConnectionResponseTypeDef:
+    ) -> TestConnectionResponseOutputTypeDef:
         """
         Tests the connection between the replication instance and the endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.test_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#test_connection)
         """
     def update_subscriptions_to_event_bridge(
         self, *, ForceMove: bool = ...
-    ) -> UpdateSubscriptionsToEventBridgeResponseTypeDef:
+    ) -> UpdateSubscriptionsToEventBridgeResponseOutputTypeDef:
         """
         Migrates 10 active and enabled Amazon SNS subscriptions at a time and converts
         them to corresponding Amazon EventBridge rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.update_subscriptions_to_event_bridge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#update_subscriptions_to_event_bridge)
         """
```

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/literals.py` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/literals.pyi` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/paginator.py` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,27 +46,27 @@
 import sys
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeCertificatesResponseTypeDef,
-    DescribeConnectionsResponseTypeDef,
-    DescribeEndpointsResponseTypeDef,
-    DescribeEndpointTypesResponseTypeDef,
-    DescribeEventsResponseTypeDef,
-    DescribeEventSubscriptionsResponseTypeDef,
-    DescribeOrderableReplicationInstancesResponseTypeDef,
-    DescribeReplicationInstancesResponseTypeDef,
-    DescribeReplicationSubnetGroupsResponseTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
-    DescribeReplicationTasksResponseTypeDef,
-    DescribeSchemasResponseTypeDef,
-    DescribeTableStatisticsResponseTypeDef,
+    DescribeCertificatesResponseOutputTypeDef,
+    DescribeConnectionsResponseOutputTypeDef,
+    DescribeEndpointsResponseOutputTypeDef,
+    DescribeEndpointTypesResponseOutputTypeDef,
+    DescribeEventsResponseOutputTypeDef,
+    DescribeEventSubscriptionsResponseOutputTypeDef,
+    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
+    DescribeReplicationInstancesResponseOutputTypeDef,
+    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
+    DescribeReplicationTasksResponseOutputTypeDef,
+    DescribeSchemasResponseOutputTypeDef,
+    DescribeTableStatisticsResponseOutputTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -107,15 +107,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeCertificatesResponseTypeDef]:
+    ) -> _PageIterator[DescribeCertificatesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
         """
 
 
 class DescribeConnectionsPaginator(Paginator):
@@ -125,15 +125,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeConnectionsResponseTypeDef]:
+    ) -> _PageIterator[DescribeConnectionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
         """
 
 
 class DescribeEndpointTypesPaginator(Paginator):
@@ -143,15 +143,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEndpointTypesResponseTypeDef]:
+    ) -> _PageIterator[DescribeEndpointTypesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
         """
 
 
 class DescribeEndpointsPaginator(Paginator):
@@ -161,15 +161,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
+    ) -> _PageIterator[DescribeEndpointsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
         """
 
 
 class DescribeEventSubscriptionsPaginator(Paginator):
@@ -180,15 +180,15 @@
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEventSubscriptionsResponseTypeDef]:
+    ) -> _PageIterator[DescribeEventSubscriptionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
 
 class DescribeEventsPaginator(Paginator):
@@ -204,30 +204,30 @@
         SourceType: Literal["replication-instance"] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEventsResponseTypeDef]:
+    ) -> _PageIterator[DescribeEventsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventspaginator)
         """
 
 
 class DescribeOrderableReplicationInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:
+    ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
         """
 
 
 class DescribeReplicationInstancesPaginator(Paginator):
@@ -237,15 +237,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationInstancesResponseTypeDef]:
+    ) -> _PageIterator[DescribeReplicationInstancesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
         """
 
 
 class DescribeReplicationSubnetGroupsPaginator(Paginator):
@@ -255,30 +255,30 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
+    ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
 
 class DescribeReplicationTaskAssessmentResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
     """
 
     def paginate(
         self, *, ReplicationTaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:
+    ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
         """
 
 
 class DescribeReplicationTasksPaginator(Paginator):
@@ -289,30 +289,30 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationTasksResponseTypeDef]:
+    ) -> _PageIterator[DescribeReplicationTasksResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskspaginator)
         """
 
 
 class DescribeSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
     """
 
     def paginate(
         self, *, EndpointArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeSchemasResponseTypeDef]:
+    ) -> _PageIterator[DescribeSchemasResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
         """
 
 
 class DescribeTableStatisticsPaginator(Paginator):
@@ -323,12 +323,12 @@
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeTableStatisticsResponseTypeDef]:
+    ) -> _PageIterator[DescribeTableStatisticsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/paginator.pyi` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,27 +46,27 @@
 import sys
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeCertificatesResponseTypeDef,
-    DescribeConnectionsResponseTypeDef,
-    DescribeEndpointsResponseTypeDef,
-    DescribeEndpointTypesResponseTypeDef,
-    DescribeEventsResponseTypeDef,
-    DescribeEventSubscriptionsResponseTypeDef,
-    DescribeOrderableReplicationInstancesResponseTypeDef,
-    DescribeReplicationInstancesResponseTypeDef,
-    DescribeReplicationSubnetGroupsResponseTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
-    DescribeReplicationTasksResponseTypeDef,
-    DescribeSchemasResponseTypeDef,
-    DescribeTableStatisticsResponseTypeDef,
+    DescribeCertificatesResponseOutputTypeDef,
+    DescribeConnectionsResponseOutputTypeDef,
+    DescribeEndpointsResponseOutputTypeDef,
+    DescribeEndpointTypesResponseOutputTypeDef,
+    DescribeEventsResponseOutputTypeDef,
+    DescribeEventSubscriptionsResponseOutputTypeDef,
+    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
+    DescribeReplicationInstancesResponseOutputTypeDef,
+    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
+    DescribeReplicationTasksResponseOutputTypeDef,
+    DescribeSchemasResponseOutputTypeDef,
+    DescribeTableStatisticsResponseOutputTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -103,15 +103,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeCertificatesResponseTypeDef]:
+    ) -> _PageIterator[DescribeCertificatesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
         """
 
 class DescribeConnectionsPaginator(Paginator):
     """
@@ -120,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeConnectionsResponseTypeDef]:
+    ) -> _PageIterator[DescribeConnectionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
         """
 
 class DescribeEndpointTypesPaginator(Paginator):
     """
@@ -137,15 +137,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEndpointTypesResponseTypeDef]:
+    ) -> _PageIterator[DescribeEndpointTypesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
         """
 
 class DescribeEndpointsPaginator(Paginator):
     """
@@ -154,15 +154,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
+    ) -> _PageIterator[DescribeEndpointsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(Paginator):
     """
@@ -172,15 +172,15 @@
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEventSubscriptionsResponseTypeDef]:
+    ) -> _PageIterator[DescribeEventSubscriptionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
     """
@@ -195,29 +195,29 @@
         SourceType: Literal["replication-instance"] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEventsResponseTypeDef]:
+    ) -> _PageIterator[DescribeEventsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventspaginator)
         """
 
 class DescribeOrderableReplicationInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:
+    ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
         """
 
 class DescribeReplicationInstancesPaginator(Paginator):
     """
@@ -226,15 +226,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationInstancesResponseTypeDef]:
+    ) -> _PageIterator[DescribeReplicationInstancesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
         """
 
 class DescribeReplicationSubnetGroupsPaginator(Paginator):
     """
@@ -243,29 +243,29 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
+    ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
 class DescribeReplicationTaskAssessmentResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
     """
 
     def paginate(
         self, *, ReplicationTaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:
+    ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
         """
 
 class DescribeReplicationTasksPaginator(Paginator):
     """
@@ -275,29 +275,29 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationTasksResponseTypeDef]:
+    ) -> _PageIterator[DescribeReplicationTasksResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskspaginator)
         """
 
 class DescribeSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
     """
 
     def paginate(
         self, *, EndpointArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeSchemasResponseTypeDef]:
+    ) -> _PageIterator[DescribeSchemasResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
         """
 
 class DescribeTableStatisticsPaginator(Paginator):
     """
@@ -307,12 +307,12 @@
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeTableStatisticsResponseTypeDef]:
+    ) -> _PageIterator[DescribeTableStatisticsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/type_defs.py` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/type_defs.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dms.type_defs import AccountQuotaTypeDef
+    from mypy_boto3_dms.type_defs import AccountQuotaOutputTypeDef
 
-    data: AccountQuotaTypeDef = {...}
+    data: AccountQuotaOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -59,28 +59,28 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "AccountQuotaTypeDef",
+    "AccountQuotaOutputTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
-    "AvailabilityZoneTypeDef",
-    "BatchStartRecommendationsErrorEntryTypeDef",
+    "AvailabilityZoneOutputTypeDef",
+    "BatchStartRecommendationsErrorEntryOutputTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
-    "CertificateTypeDef",
-    "CollectorHealthCheckTypeDef",
-    "InventoryDataTypeDef",
-    "CollectorShortInfoResponseTypeDef",
+    "CertificateOutputTypeDef",
+    "CollectorHealthCheckOutputTypeDef",
+    "InventoryDataOutputTypeDef",
+    "CollectorShortInfoResponseOutputTypeDef",
+    "ComputeConfigOutputTypeDef",
     "ComputeConfigTypeDef",
-    "ConnectionTypeDef",
+    "ConnectionOutputTypeDef",
     "DmsTransferSettingsTypeDef",
     "DocDbSettingsTypeDef",
     "DynamoDbSettingsTypeDef",
     "ElasticsearchSettingsTypeDef",
     "GcpMySQLSettingsTypeDef",
     "IBMDb2SettingsTypeDef",
     "KafkaSettingsTypeDef",
@@ -92,124 +92,143 @@
     "OracleSettingsTypeDef",
     "PostgreSQLSettingsTypeDef",
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
     "TimestreamSettingsTypeDef",
-    "EventSubscriptionTypeDef",
+    "EventSubscriptionOutputTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    "DatabaseInstanceSoftwareDetailsResponseTypeDef",
-    "ServerShortInfoResponseTypeDef",
-    "DatabaseShortInfoResponseTypeDef",
+    "CreateFleetAdvisorCollectorResponseOutputTypeDef",
+    "DatabaseInstanceSoftwareDetailsResponseOutputTypeDef",
+    "ServerShortInfoResponseOutputTypeDef",
+    "DatabaseShortInfoResponseOutputTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
+    "DeleteFleetAdvisorDatabasesResponseOutputTypeDef",
     "DeleteReplicationConfigMessageRequestTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
+    "DescribeApplicableIndividualAssessmentsResponseOutputTypeDef",
     "FilterTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
-    "EndpointSettingTypeDef",
-    "SupportedEndpointTypeTypeDef",
-    "EventCategoryGroupTypeDef",
-    "EventTypeDef",
+    "EndpointSettingOutputTypeDef",
+    "SupportedEndpointTypeOutputTypeDef",
+    "EventCategoryGroupOutputTypeDef",
+    "EventOutputTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
-    "FleetAdvisorLsaAnalysisResponseTypeDef",
-    "FleetAdvisorSchemaObjectResponseTypeDef",
+    "FleetAdvisorLsaAnalysisResponseOutputTypeDef",
+    "FleetAdvisorSchemaObjectResponseOutputTypeDef",
     "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
-    "OrderableReplicationInstanceTypeDef",
-    "LimitationTypeDef",
+    "OrderableReplicationInstanceOutputTypeDef",
+    "LimitationOutputTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
-    "RefreshSchemasStatusTypeDef",
+    "RefreshSchemasStatusOutputTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
-    "ReplicationInstanceTaskLogTypeDef",
-    "TableStatisticsTypeDef",
+    "ReplicationInstanceTaskLogOutputTypeDef",
+    "TableStatisticsOutputTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
-    "ReplicationTaskAssessmentResultTypeDef",
-    "ReplicationTaskIndividualAssessmentTypeDef",
+    "ReplicationTaskAssessmentResultOutputTypeDef",
+    "ReplicationTaskIndividualAssessmentOutputTypeDef",
     "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
-    "DescribeSchemasResponseTypeDef",
+    "DescribeSchemasResponseOutputTypeDef",
+    "DmsTransferSettingsOutputTypeDef",
+    "DocDbSettingsOutputTypeDef",
+    "DynamoDbSettingsOutputTypeDef",
+    "ElasticsearchSettingsOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "GcpMySQLSettingsOutputTypeDef",
+    "IBMDb2SettingsOutputTypeDef",
+    "KafkaSettingsOutputTypeDef",
+    "KinesisSettingsOutputTypeDef",
+    "MicrosoftSQLServerSettingsOutputTypeDef",
+    "MongoDbSettingsOutputTypeDef",
+    "MySQLSettingsOutputTypeDef",
+    "NeptuneSettingsOutputTypeDef",
+    "OracleSettingsOutputTypeDef",
+    "PostgreSQLSettingsOutputTypeDef",
+    "RedisSettingsOutputTypeDef",
+    "RedshiftSettingsOutputTypeDef",
+    "S3SettingsOutputTypeDef",
+    "SybaseSettingsOutputTypeDef",
+    "TimestreamSettingsOutputTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
+    "TagOutputTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "PendingMaintenanceActionTypeDef",
-    "ProvisionDataTypeDef",
-    "RdsConfigurationTypeDef",
-    "RdsRequirementsTypeDef",
+    "PendingMaintenanceActionOutputTypeDef",
+    "ProvisionDataOutputTypeDef",
+    "RdsConfigurationOutputTypeDef",
+    "RdsRequirementsOutputTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
+    "RecommendationSettingsOutputTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
-    "ReloadReplicationTablesResponseTypeDef",
-    "ReloadTablesResponseTypeDef",
+    "ReloadReplicationTablesResponseOutputTypeDef",
+    "ReloadTablesResponseOutputTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ReplicationPendingModifiedValuesTypeDef",
-    "VpcSecurityGroupMembershipTypeDef",
-    "ReplicationStatsTypeDef",
-    "ReplicationTaskAssessmentRunProgressTypeDef",
-    "ReplicationTaskStatsTypeDef",
+    "ReplicationPendingModifiedValuesOutputTypeDef",
+    "VpcSecurityGroupMembershipOutputTypeDef",
+    "ReplicationStatsOutputTypeDef",
+    "ReplicationTaskAssessmentRunProgressOutputTypeDef",
+    "ReplicationTaskStatsOutputTypeDef",
     "ResponseMetadataTypeDef",
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    "SchemaShortInfoResponseTypeDef",
+    "RunFleetAdvisorLsaAnalysisResponseOutputTypeDef",
+    "SchemaShortInfoResponseOutputTypeDef",
     "StartReplicationMessageRequestTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
     "StartReplicationTaskMessageRequestTypeDef",
     "StopReplicationMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
+    "UpdateSubscriptionsToEventBridgeResponseOutputTypeDef",
+    "DescribeAccountAttributesResponseOutputTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ImportCertificateMessageRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "SubnetTypeDef",
-    "BatchStartRecommendationsResponseTypeDef",
-    "DeleteCertificateResponseTypeDef",
-    "DescribeCertificatesResponseTypeDef",
-    "ImportCertificateResponseTypeDef",
-    "CollectorResponseTypeDef",
+    "SubnetOutputTypeDef",
+    "BatchStartRecommendationsResponseOutputTypeDef",
+    "DeleteCertificateResponseOutputTypeDef",
+    "DescribeCertificatesResponseOutputTypeDef",
+    "ImportCertificateResponseOutputTypeDef",
+    "CollectorResponseOutputTypeDef",
+    "ReplicationConfigOutputTypeDef",
     "CreateReplicationConfigMessageRequestTypeDef",
     "ModifyReplicationConfigMessageRequestTypeDef",
-    "ReplicationConfigTypeDef",
-    "DeleteConnectionResponseTypeDef",
-    "DescribeConnectionsResponseTypeDef",
-    "TestConnectionResponseTypeDef",
+    "DeleteConnectionResponseOutputTypeDef",
+    "DescribeConnectionsResponseOutputTypeDef",
+    "TestConnectionResponseOutputTypeDef",
     "CreateEndpointMessageRequestTypeDef",
-    "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
-    "CreateEventSubscriptionResponseTypeDef",
-    "DeleteEventSubscriptionResponseTypeDef",
-    "DescribeEventSubscriptionsResponseTypeDef",
-    "ModifyEventSubscriptionResponseTypeDef",
-    "DatabaseResponseTypeDef",
+    "CreateEventSubscriptionResponseOutputTypeDef",
+    "DeleteEventSubscriptionResponseOutputTypeDef",
+    "DescribeEventSubscriptionsResponseOutputTypeDef",
+    "ModifyEventSubscriptionResponseOutputTypeDef",
+    "DatabaseResponseOutputTypeDef",
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
     "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
     "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
     "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
@@ -243,85 +262,87 @@
     "DescribeEndpointsMessageEndpointDeletedWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef",
-    "DescribeEndpointSettingsResponseTypeDef",
-    "DescribeEndpointTypesResponseTypeDef",
-    "DescribeEventCategoriesResponseTypeDef",
-    "DescribeEventsResponseTypeDef",
-    "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
-    "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
-    "DescribeOrderableReplicationInstancesResponseTypeDef",
-    "DescribeRecommendationLimitationsResponseTypeDef",
-    "DescribeRefreshSchemasStatusResponseTypeDef",
-    "RefreshSchemasResponseTypeDef",
-    "DescribeReplicationInstanceTaskLogsResponseTypeDef",
-    "DescribeReplicationTableStatisticsResponseTypeDef",
-    "DescribeTableStatisticsResponseTypeDef",
-    "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
-    "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
-    "ResourcePendingMaintenanceActionsTypeDef",
-    "RdsRecommendationTypeDef",
+    "DescribeEndpointSettingsResponseOutputTypeDef",
+    "DescribeEndpointTypesResponseOutputTypeDef",
+    "DescribeEventCategoriesResponseOutputTypeDef",
+    "DescribeEventsResponseOutputTypeDef",
+    "DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef",
+    "DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef",
+    "DescribeOrderableReplicationInstancesResponseOutputTypeDef",
+    "DescribeRecommendationLimitationsResponseOutputTypeDef",
+    "DescribeRefreshSchemasStatusResponseOutputTypeDef",
+    "RefreshSchemasResponseOutputTypeDef",
+    "DescribeReplicationInstanceTaskLogsResponseOutputTypeDef",
+    "DescribeReplicationTableStatisticsResponseOutputTypeDef",
+    "DescribeTableStatisticsResponseOutputTypeDef",
+    "DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef",
+    "DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef",
+    "EndpointOutputTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
+    "ResourcePendingMaintenanceActionsOutputTypeDef",
+    "RdsRecommendationOutputTypeDef",
     "StartRecommendationsRequestEntryTypeDef",
     "StartRecommendationsRequestRequestTypeDef",
     "ReloadReplicationTablesMessageRequestTypeDef",
     "ReloadTablesMessageRequestTypeDef",
-    "ReplicationTypeDef",
-    "ReplicationTaskAssessmentRunTypeDef",
-    "ReplicationTaskTypeDef",
-    "SchemaResponseTypeDef",
-    "ReplicationSubnetGroupTypeDef",
-    "DescribeFleetAdvisorCollectorsResponseTypeDef",
-    "CreateReplicationConfigResponseTypeDef",
-    "DeleteReplicationConfigResponseTypeDef",
-    "DescribeReplicationConfigsResponseTypeDef",
-    "ModifyReplicationConfigResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
-    "DeleteEndpointResponseTypeDef",
-    "DescribeEndpointsResponseTypeDef",
-    "ModifyEndpointResponseTypeDef",
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
-    "ApplyPendingMaintenanceActionResponseTypeDef",
-    "DescribePendingMaintenanceActionsResponseTypeDef",
-    "RecommendationDataTypeDef",
+    "ReplicationOutputTypeDef",
+    "ReplicationTaskAssessmentRunOutputTypeDef",
+    "ReplicationTaskOutputTypeDef",
+    "SchemaResponseOutputTypeDef",
+    "ReplicationSubnetGroupOutputTypeDef",
+    "DescribeFleetAdvisorCollectorsResponseOutputTypeDef",
+    "CreateReplicationConfigResponseOutputTypeDef",
+    "DeleteReplicationConfigResponseOutputTypeDef",
+    "DescribeReplicationConfigsResponseOutputTypeDef",
+    "ModifyReplicationConfigResponseOutputTypeDef",
+    "DescribeFleetAdvisorDatabasesResponseOutputTypeDef",
+    "CreateEndpointResponseOutputTypeDef",
+    "DeleteEndpointResponseOutputTypeDef",
+    "DescribeEndpointsResponseOutputTypeDef",
+    "ModifyEndpointResponseOutputTypeDef",
+    "ApplyPendingMaintenanceActionResponseOutputTypeDef",
+    "DescribePendingMaintenanceActionsResponseOutputTypeDef",
+    "RecommendationDataOutputTypeDef",
     "BatchStartRecommendationsRequestRequestTypeDef",
-    "DescribeReplicationsResponseTypeDef",
-    "StartReplicationResponseTypeDef",
-    "StopReplicationResponseTypeDef",
-    "CancelReplicationTaskAssessmentRunResponseTypeDef",
-    "DeleteReplicationTaskAssessmentRunResponseTypeDef",
-    "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
-    "StartReplicationTaskAssessmentRunResponseTypeDef",
-    "CreateReplicationTaskResponseTypeDef",
-    "DeleteReplicationTaskResponseTypeDef",
-    "DescribeReplicationTasksResponseTypeDef",
-    "ModifyReplicationTaskResponseTypeDef",
-    "MoveReplicationTaskResponseTypeDef",
-    "StartReplicationTaskAssessmentResponseTypeDef",
-    "StartReplicationTaskResponseTypeDef",
-    "StopReplicationTaskResponseTypeDef",
-    "DescribeFleetAdvisorSchemasResponseTypeDef",
-    "CreateReplicationSubnetGroupResponseTypeDef",
-    "DescribeReplicationSubnetGroupsResponseTypeDef",
-    "ModifyReplicationSubnetGroupResponseTypeDef",
-    "ReplicationInstanceTypeDef",
-    "RecommendationTypeDef",
-    "CreateReplicationInstanceResponseTypeDef",
-    "DeleteReplicationInstanceResponseTypeDef",
-    "DescribeReplicationInstancesResponseTypeDef",
-    "ModifyReplicationInstanceResponseTypeDef",
-    "RebootReplicationInstanceResponseTypeDef",
-    "DescribeRecommendationsResponseTypeDef",
+    "DescribeReplicationsResponseOutputTypeDef",
+    "StartReplicationResponseOutputTypeDef",
+    "StopReplicationResponseOutputTypeDef",
+    "CancelReplicationTaskAssessmentRunResponseOutputTypeDef",
+    "DeleteReplicationTaskAssessmentRunResponseOutputTypeDef",
+    "DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef",
+    "StartReplicationTaskAssessmentRunResponseOutputTypeDef",
+    "CreateReplicationTaskResponseOutputTypeDef",
+    "DeleteReplicationTaskResponseOutputTypeDef",
+    "DescribeReplicationTasksResponseOutputTypeDef",
+    "ModifyReplicationTaskResponseOutputTypeDef",
+    "MoveReplicationTaskResponseOutputTypeDef",
+    "StartReplicationTaskAssessmentResponseOutputTypeDef",
+    "StartReplicationTaskResponseOutputTypeDef",
+    "StopReplicationTaskResponseOutputTypeDef",
+    "DescribeFleetAdvisorSchemasResponseOutputTypeDef",
+    "CreateReplicationSubnetGroupResponseOutputTypeDef",
+    "DescribeReplicationSubnetGroupsResponseOutputTypeDef",
+    "ModifyReplicationSubnetGroupResponseOutputTypeDef",
+    "ReplicationInstanceOutputTypeDef",
+    "RecommendationOutputTypeDef",
+    "CreateReplicationInstanceResponseOutputTypeDef",
+    "DeleteReplicationInstanceResponseOutputTypeDef",
+    "DescribeReplicationInstancesResponseOutputTypeDef",
+    "ModifyReplicationInstanceResponseOutputTypeDef",
+    "RebootReplicationInstanceResponseOutputTypeDef",
+    "DescribeRecommendationsResponseOutputTypeDef",
 )
 
-AccountQuotaTypeDef = TypedDict(
-    "AccountQuotaTypeDef",
+AccountQuotaOutputTypeDef = TypedDict(
+    "AccountQuotaOutputTypeDef",
     {
         "AccountQuotaName": str,
         "Used": int,
         "Max": int,
     },
 )
 
@@ -340,79 +361,94 @@
     {
         "ReplicationInstanceArn": str,
         "ApplyAction": str,
         "OptInType": str,
     },
 )
 
-AvailabilityZoneTypeDef = TypedDict(
-    "AvailabilityZoneTypeDef",
+AvailabilityZoneOutputTypeDef = TypedDict(
+    "AvailabilityZoneOutputTypeDef",
     {
         "Name": str,
     },
 )
 
-BatchStartRecommendationsErrorEntryTypeDef = TypedDict(
-    "BatchStartRecommendationsErrorEntryTypeDef",
+BatchStartRecommendationsErrorEntryOutputTypeDef = TypedDict(
+    "BatchStartRecommendationsErrorEntryOutputTypeDef",
     {
         "DatabaseId": str,
         "Message": str,
         "Code": str,
     },
 )
 
 CancelReplicationTaskAssessmentRunMessageRequestTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
     },
 )
 
-CertificateTypeDef = TypedDict(
-    "CertificateTypeDef",
+CertificateOutputTypeDef = TypedDict(
+    "CertificateOutputTypeDef",
     {
         "CertificateIdentifier": str,
         "CertificateCreationDate": datetime,
         "CertificatePem": str,
         "CertificateWallet": bytes,
         "CertificateArn": str,
         "CertificateOwner": str,
         "ValidFromDate": datetime,
         "ValidToDate": datetime,
         "SigningAlgorithm": str,
         "KeyLength": int,
     },
 )
 
-CollectorHealthCheckTypeDef = TypedDict(
-    "CollectorHealthCheckTypeDef",
+CollectorHealthCheckOutputTypeDef = TypedDict(
+    "CollectorHealthCheckOutputTypeDef",
     {
         "CollectorStatus": CollectorStatusType,
         "LocalCollectorS3Access": bool,
         "WebCollectorS3Access": bool,
         "WebCollectorGrantedRoleBasedAccess": bool,
     },
 )
 
-InventoryDataTypeDef = TypedDict(
-    "InventoryDataTypeDef",
+InventoryDataOutputTypeDef = TypedDict(
+    "InventoryDataOutputTypeDef",
     {
         "NumberOfDatabases": int,
         "NumberOfSchemas": int,
     },
 )
 
-CollectorShortInfoResponseTypeDef = TypedDict(
-    "CollectorShortInfoResponseTypeDef",
+CollectorShortInfoResponseOutputTypeDef = TypedDict(
+    "CollectorShortInfoResponseOutputTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
     },
 )
 
+ComputeConfigOutputTypeDef = TypedDict(
+    "ComputeConfigOutputTypeDef",
+    {
+        "AvailabilityZone": str,
+        "DnsNameServers": str,
+        "KmsKeyId": str,
+        "MaxCapacityUnits": int,
+        "MinCapacityUnits": int,
+        "MultiAZ": bool,
+        "PreferredMaintenanceWindow": str,
+        "ReplicationSubnetGroupId": str,
+        "VpcSecurityGroupIds": List[str],
+    },
+)
+
 ComputeConfigTypeDef = TypedDict(
     "ComputeConfigTypeDef",
     {
         "AvailabilityZone": str,
         "DnsNameServers": str,
         "KmsKeyId": str,
         "MaxCapacityUnits": int,
@@ -421,16 +457,16 @@
         "PreferredMaintenanceWindow": str,
         "ReplicationSubnetGroupId": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-ConnectionTypeDef = TypedDict(
-    "ConnectionTypeDef",
+ConnectionOutputTypeDef = TypedDict(
+    "ConnectionOutputTypeDef",
     {
         "ReplicationInstanceArn": str,
         "EndpointArn": str,
         "Status": str,
         "LastFailureMessage": str,
         "EndpointIdentifier": str,
         "ReplicationInstanceIdentifier": str,
@@ -486,21 +522,19 @@
         "FullLoadErrorPercentage": int,
         "ErrorRetryDuration": int,
         "UseNewMappingType": bool,
     },
     total=False,
 )
 
-
 class ElasticsearchSettingsTypeDef(
     _RequiredElasticsearchSettingsTypeDef, _OptionalElasticsearchSettingsTypeDef
 ):
     pass
 
-
 GcpMySQLSettingsTypeDef = TypedDict(
     "GcpMySQLSettingsTypeDef",
     {
         "AfterConnectScript": str,
         "CleanSourceMetadataOnMismatch": bool,
         "DatabaseName": str,
         "EventsPollInterval": int,
@@ -662,19 +696,17 @@
         "MaxFileSize": int,
         "MaxRetryCount": int,
         "IamAuthEnabled": bool,
     },
     total=False,
 )
 
-
 class NeptuneSettingsTypeDef(_RequiredNeptuneSettingsTypeDef, _OptionalNeptuneSettingsTypeDef):
     pass
 
-
 OracleSettingsTypeDef = TypedDict(
     "OracleSettingsTypeDef",
     {
         "AddSupplementalLogging": bool,
         "ArchivedLogDestId": int,
         "AdditionalArchivedLogDestId": int,
         "ExtraArchivedLogDestIds": Sequence[int],
@@ -767,19 +799,17 @@
         "AuthUserName": str,
         "AuthPassword": str,
         "SslCaCertificateArn": str,
     },
     total=False,
 )
 
-
 class RedisSettingsTypeDef(_RequiredRedisSettingsTypeDef, _OptionalRedisSettingsTypeDef):
     pass
 
-
 RedshiftSettingsTypeDef = TypedDict(
     "RedshiftSettingsTypeDef",
     {
         "AcceptAnyDate": bool,
         "AfterConnectScript": str,
         "BucketFolder": str,
         "BucketName": str,
@@ -889,23 +919,21 @@
     {
         "CdcInsertsAndUpdates": bool,
         "EnableMagneticStoreWrites": bool,
     },
     total=False,
 )
 
-
 class TimestreamSettingsTypeDef(
     _RequiredTimestreamSettingsTypeDef, _OptionalTimestreamSettingsTypeDef
 ):
     pass
 
-
-EventSubscriptionTypeDef = TypedDict(
-    "EventSubscriptionTypeDef",
+EventSubscriptionOutputTypeDef = TypedDict(
+    "EventSubscriptionOutputTypeDef",
     {
         "CustomerAwsId": str,
         "CustSubscriptionId": str,
         "SnsTopicArn": str,
         "Status": str,
         "SubscriptionCreationTime": str,
         "SourceType": str,
@@ -927,58 +955,56 @@
     "_OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateFleetAdvisorCollectorRequestRequestTypeDef(
     _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef,
     _OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef,
 ):
     pass
 
-
-CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
-    "CreateFleetAdvisorCollectorResponseTypeDef",
+CreateFleetAdvisorCollectorResponseOutputTypeDef = TypedDict(
+    "CreateFleetAdvisorCollectorResponseOutputTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
         "Description": str,
         "ServiceAccessRoleArn": str,
         "S3BucketName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatabaseInstanceSoftwareDetailsResponseTypeDef = TypedDict(
-    "DatabaseInstanceSoftwareDetailsResponseTypeDef",
+DatabaseInstanceSoftwareDetailsResponseOutputTypeDef = TypedDict(
+    "DatabaseInstanceSoftwareDetailsResponseOutputTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "EngineEdition": str,
         "ServicePack": str,
         "SupportLevel": str,
         "OsArchitecture": int,
         "Tooltip": str,
     },
 )
 
-ServerShortInfoResponseTypeDef = TypedDict(
-    "ServerShortInfoResponseTypeDef",
+ServerShortInfoResponseOutputTypeDef = TypedDict(
+    "ServerShortInfoResponseOutputTypeDef",
     {
         "ServerId": str,
         "IpAddress": str,
         "ServerName": str,
     },
 )
 
-DatabaseShortInfoResponseTypeDef = TypedDict(
-    "DatabaseShortInfoResponseTypeDef",
+DatabaseShortInfoResponseOutputTypeDef = TypedDict(
+    "DatabaseShortInfoResponseOutputTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
         "DatabaseEngine": str,
     },
 )
@@ -1022,16 +1048,16 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
-DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
+DeleteFleetAdvisorDatabasesResponseOutputTypeDef = TypedDict(
+    "DeleteFleetAdvisorDatabasesResponseOutputTypeDef",
     {
         "DatabaseIds": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationConfigMessageRequestTypeDef = TypedDict(
@@ -1079,16 +1105,16 @@
         "MigrationType": MigrationTypeValueType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
+DescribeApplicableIndividualAssessmentsResponseOutputTypeDef = TypedDict(
+    "DescribeApplicableIndividualAssessmentsResponseOutputTypeDef",
     {
         "IndividualAssessmentNames": List[str],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1120,58 +1146,56 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeEndpointSettingsMessageRequestTypeDef(
     _RequiredDescribeEndpointSettingsMessageRequestTypeDef,
     _OptionalDescribeEndpointSettingsMessageRequestTypeDef,
 ):
     pass
 
-
-EndpointSettingTypeDef = TypedDict(
-    "EndpointSettingTypeDef",
+EndpointSettingOutputTypeDef = TypedDict(
+    "EndpointSettingOutputTypeDef",
     {
         "Name": str,
         "Type": EndpointSettingTypeValueType,
         "EnumValues": List[str],
         "Sensitive": bool,
         "Units": str,
         "Applicability": str,
         "IntValueMin": int,
         "IntValueMax": int,
         "DefaultValue": str,
     },
 )
 
-SupportedEndpointTypeTypeDef = TypedDict(
-    "SupportedEndpointTypeTypeDef",
+SupportedEndpointTypeOutputTypeDef = TypedDict(
+    "SupportedEndpointTypeOutputTypeDef",
     {
         "EngineName": str,
         "SupportsCDC": bool,
         "EndpointType": ReplicationEndpointTypeValueType,
         "ReplicationInstanceEngineMinimumVersion": str,
         "EngineDisplayName": str,
     },
 )
 
-EventCategoryGroupTypeDef = TypedDict(
-    "EventCategoryGroupTypeDef",
+EventCategoryGroupOutputTypeDef = TypedDict(
+    "EventCategoryGroupOutputTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
 )
 
-EventTypeDef = TypedDict(
-    "EventTypeDef",
+EventOutputTypeDef = TypedDict(
+    "EventOutputTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
     },
@@ -1182,24 +1206,24 @@
     {
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-FleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "FleetAdvisorLsaAnalysisResponseTypeDef",
+FleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
+    "FleetAdvisorLsaAnalysisResponseOutputTypeDef",
     {
         "LsaAnalysisId": str,
         "Status": str,
     },
 )
 
-FleetAdvisorSchemaObjectResponseTypeDef = TypedDict(
-    "FleetAdvisorSchemaObjectResponseTypeDef",
+FleetAdvisorSchemaObjectResponseOutputTypeDef = TypedDict(
+    "FleetAdvisorSchemaObjectResponseOutputTypeDef",
     {
         "SchemaId": str,
         "ObjectType": str,
         "NumberOfObjects": int,
         "CodeLineCount": int,
         "CodeSize": int,
     },
@@ -1218,31 +1242,31 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-OrderableReplicationInstanceTypeDef = TypedDict(
-    "OrderableReplicationInstanceTypeDef",
+OrderableReplicationInstanceOutputTypeDef = TypedDict(
+    "OrderableReplicationInstanceOutputTypeDef",
     {
         "EngineVersion": str,
         "ReplicationInstanceClass": str,
         "StorageType": str,
         "MinAllocatedStorage": int,
         "MaxAllocatedStorage": int,
         "DefaultAllocatedStorage": int,
         "IncludedAllocatedStorage": int,
         "AvailabilityZones": List[str],
         "ReleaseStatus": ReleaseStatusValuesType,
     },
 )
 
-LimitationTypeDef = TypedDict(
-    "LimitationTypeDef",
+LimitationOutputTypeDef = TypedDict(
+    "LimitationOutputTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "Name": str,
         "Description": str,
         "Impact": str,
         "Type": str,
@@ -1252,16 +1276,16 @@
 DescribeRefreshSchemasStatusMessageRequestTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
-RefreshSchemasStatusTypeDef = TypedDict(
-    "RefreshSchemasStatusTypeDef",
+RefreshSchemasStatusOutputTypeDef = TypedDict(
+    "RefreshSchemasStatusOutputTypeDef",
     {
         "EndpointArn": str,
         "ReplicationInstanceArn": str,
         "Status": RefreshSchemasStatusTypeValueType,
         "LastRefreshDate": datetime,
         "LastFailureMessage": str,
     },
@@ -1278,33 +1302,31 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeReplicationInstanceTaskLogsMessageRequestTypeDef(
     _RequiredDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     _OptionalDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
 ):
     pass
 
-
-ReplicationInstanceTaskLogTypeDef = TypedDict(
-    "ReplicationInstanceTaskLogTypeDef",
+ReplicationInstanceTaskLogOutputTypeDef = TypedDict(
+    "ReplicationInstanceTaskLogOutputTypeDef",
     {
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
 )
 
-TableStatisticsTypeDef = TypedDict(
-    "TableStatisticsTypeDef",
+TableStatisticsOutputTypeDef = TypedDict(
+    "TableStatisticsOutputTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
         "Inserts": int,
         "Deletes": int,
         "Updates": int,
         "Ddls": int,
@@ -1343,29 +1365,29 @@
         "ReplicationTaskArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-ReplicationTaskAssessmentResultTypeDef = TypedDict(
-    "ReplicationTaskAssessmentResultTypeDef",
+ReplicationTaskAssessmentResultOutputTypeDef = TypedDict(
+    "ReplicationTaskAssessmentResultOutputTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "ReplicationTaskArn": str,
         "ReplicationTaskLastAssessmentDate": datetime,
         "AssessmentStatus": str,
         "AssessmentResultsFile": str,
         "AssessmentResults": str,
         "S3ObjectUrl": str,
     },
 )
 
-ReplicationTaskIndividualAssessmentTypeDef = TypedDict(
-    "ReplicationTaskIndividualAssessmentTypeDef",
+ReplicationTaskIndividualAssessmentOutputTypeDef = TypedDict(
+    "ReplicationTaskIndividualAssessmentOutputTypeDef",
     {
         "ReplicationTaskIndividualAssessmentArn": str,
         "ReplicationTaskAssessmentRunArn": str,
         "IndividualAssessmentName": str,
         "Status": str,
         "ReplicationTaskIndividualAssessmentStartDate": datetime,
     },
@@ -1381,22 +1403,20 @@
     "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
     _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeSchemasMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemasMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalDescribeSchemasMessageRequestTypeDef = TypedDict(
@@ -1404,46 +1424,454 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
-
-DescribeSchemasResponseTypeDef = TypedDict(
-    "DescribeSchemasResponseTypeDef",
+DescribeSchemasResponseOutputTypeDef = TypedDict(
+    "DescribeSchemasResponseOutputTypeDef",
     {
         "Marker": str,
         "Schemas": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DmsTransferSettingsOutputTypeDef = TypedDict(
+    "DmsTransferSettingsOutputTypeDef",
+    {
+        "ServiceAccessRoleArn": str,
+        "BucketName": str,
+    },
+)
+
+DocDbSettingsOutputTypeDef = TypedDict(
+    "DocDbSettingsOutputTypeDef",
+    {
+        "Username": str,
+        "Password": str,
+        "ServerName": str,
+        "Port": int,
+        "DatabaseName": str,
+        "NestingLevel": NestingLevelValueType,
+        "ExtractDocId": bool,
+        "DocsToInvestigate": int,
+        "KmsKeyId": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "UseUpdateLookUp": bool,
+        "ReplicateShardCollections": bool,
+    },
+)
+
+DynamoDbSettingsOutputTypeDef = TypedDict(
+    "DynamoDbSettingsOutputTypeDef",
+    {
+        "ServiceAccessRoleArn": str,
+    },
+)
+
+ElasticsearchSettingsOutputTypeDef = TypedDict(
+    "ElasticsearchSettingsOutputTypeDef",
+    {
+        "ServiceAccessRoleArn": str,
+        "EndpointUri": str,
+        "FullLoadErrorPercentage": int,
+        "ErrorRetryDuration": int,
+        "UseNewMappingType": bool,
+    },
+)
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GcpMySQLSettingsOutputTypeDef = TypedDict(
+    "GcpMySQLSettingsOutputTypeDef",
+    {
+        "AfterConnectScript": str,
+        "CleanSourceMetadataOnMismatch": bool,
+        "DatabaseName": str,
+        "EventsPollInterval": int,
+        "TargetDbType": TargetDbTypeType,
+        "MaxFileSize": int,
+        "ParallelLoadThreads": int,
+        "Password": str,
+        "Port": int,
+        "ServerName": str,
+        "ServerTimezone": str,
+        "Username": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+    },
+)
+
+IBMDb2SettingsOutputTypeDef = TypedDict(
+    "IBMDb2SettingsOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "Password": str,
+        "Port": int,
+        "ServerName": str,
+        "SetDataCaptureChanges": bool,
+        "CurrentLsn": str,
+        "MaxKBytesPerRead": int,
+        "Username": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+    },
+)
+
+KafkaSettingsOutputTypeDef = TypedDict(
+    "KafkaSettingsOutputTypeDef",
+    {
+        "Broker": str,
+        "Topic": str,
+        "MessageFormat": MessageFormatValueType,
+        "IncludeTransactionDetails": bool,
+        "IncludePartitionValue": bool,
+        "PartitionIncludeSchemaTable": bool,
+        "IncludeTableAlterOperations": bool,
+        "IncludeControlDetails": bool,
+        "MessageMaxBytes": int,
+        "IncludeNullAndEmpty": bool,
+        "SecurityProtocol": KafkaSecurityProtocolType,
+        "SslClientCertificateArn": str,
+        "SslClientKeyArn": str,
+        "SslClientKeyPassword": str,
+        "SslCaCertificateArn": str,
+        "SaslUsername": str,
+        "SaslPassword": str,
+        "NoHexPrefix": bool,
+        "SaslMechanism": KafkaSaslMechanismType,
+        "SslEndpointIdentificationAlgorithm": KafkaSslEndpointIdentificationAlgorithmType,
+    },
+)
+
+KinesisSettingsOutputTypeDef = TypedDict(
+    "KinesisSettingsOutputTypeDef",
+    {
+        "StreamArn": str,
+        "MessageFormat": MessageFormatValueType,
+        "ServiceAccessRoleArn": str,
+        "IncludeTransactionDetails": bool,
+        "IncludePartitionValue": bool,
+        "PartitionIncludeSchemaTable": bool,
+        "IncludeTableAlterOperations": bool,
+        "IncludeControlDetails": bool,
+        "IncludeNullAndEmpty": bool,
+        "NoHexPrefix": bool,
+    },
+)
+
+MicrosoftSQLServerSettingsOutputTypeDef = TypedDict(
+    "MicrosoftSQLServerSettingsOutputTypeDef",
+    {
+        "Port": int,
+        "BcpPacketSize": int,
+        "DatabaseName": str,
+        "ControlTablesFileGroup": str,
+        "Password": str,
+        "QuerySingleAlwaysOnNode": bool,
+        "ReadBackupOnly": bool,
+        "SafeguardPolicy": SafeguardPolicyType,
+        "ServerName": str,
+        "Username": str,
+        "UseBcpFullLoad": bool,
+        "UseThirdPartyBackupDevice": bool,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "TrimSpaceInChar": bool,
+        "TlogAccessMode": TlogAccessModeType,
+        "ForceLobLookup": bool,
+    },
+)
+
+MongoDbSettingsOutputTypeDef = TypedDict(
+    "MongoDbSettingsOutputTypeDef",
+    {
+        "Username": str,
+        "Password": str,
+        "ServerName": str,
+        "Port": int,
+        "DatabaseName": str,
+        "AuthType": AuthTypeValueType,
+        "AuthMechanism": AuthMechanismValueType,
+        "NestingLevel": NestingLevelValueType,
+        "ExtractDocId": str,
+        "DocsToInvestigate": str,
+        "AuthSource": str,
+        "KmsKeyId": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "UseUpdateLookUp": bool,
+        "ReplicateShardCollections": bool,
+    },
+)
+
+MySQLSettingsOutputTypeDef = TypedDict(
+    "MySQLSettingsOutputTypeDef",
+    {
+        "AfterConnectScript": str,
+        "CleanSourceMetadataOnMismatch": bool,
+        "DatabaseName": str,
+        "EventsPollInterval": int,
+        "TargetDbType": TargetDbTypeType,
+        "MaxFileSize": int,
+        "ParallelLoadThreads": int,
+        "Password": str,
+        "Port": int,
+        "ServerName": str,
+        "ServerTimezone": str,
+        "Username": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+    },
+)
+
+NeptuneSettingsOutputTypeDef = TypedDict(
+    "NeptuneSettingsOutputTypeDef",
+    {
+        "ServiceAccessRoleArn": str,
+        "S3BucketName": str,
+        "S3BucketFolder": str,
+        "ErrorRetryDuration": int,
+        "MaxFileSize": int,
+        "MaxRetryCount": int,
+        "IamAuthEnabled": bool,
+    },
+)
+
+OracleSettingsOutputTypeDef = TypedDict(
+    "OracleSettingsOutputTypeDef",
+    {
+        "AddSupplementalLogging": bool,
+        "ArchivedLogDestId": int,
+        "AdditionalArchivedLogDestId": int,
+        "ExtraArchivedLogDestIds": List[int],
+        "AllowSelectNestedTables": bool,
+        "ParallelAsmReadThreads": int,
+        "ReadAheadBlocks": int,
+        "AccessAlternateDirectly": bool,
+        "UseAlternateFolderForOnline": bool,
+        "OraclePathPrefix": str,
+        "UsePathPrefix": str,
+        "ReplacePathPrefix": bool,
+        "EnableHomogenousTablespace": bool,
+        "DirectPathNoLog": bool,
+        "ArchivedLogsOnly": bool,
+        "AsmPassword": str,
+        "AsmServer": str,
+        "AsmUser": str,
+        "CharLengthSemantics": CharLengthSemanticsType,
+        "DatabaseName": str,
+        "DirectPathParallelLoad": bool,
+        "FailTasksOnLobTruncation": bool,
+        "NumberDatatypeScale": int,
+        "Password": str,
+        "Port": int,
+        "ReadTableSpaceName": bool,
+        "RetryInterval": int,
+        "SecurityDbEncryption": str,
+        "SecurityDbEncryptionName": str,
+        "ServerName": str,
+        "SpatialDataOptionToGeoJsonFunctionName": str,
+        "StandbyDelayTime": int,
+        "Username": str,
+        "UseBFile": bool,
+        "UseDirectPathFullLoad": bool,
+        "UseLogminerReader": bool,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "SecretsManagerOracleAsmAccessRoleArn": str,
+        "SecretsManagerOracleAsmSecretId": str,
+        "TrimSpaceInChar": bool,
+        "ConvertTimestampWithZoneToUTC": bool,
+        "OpenTransactionWindow": int,
+    },
+)
+
+PostgreSQLSettingsOutputTypeDef = TypedDict(
+    "PostgreSQLSettingsOutputTypeDef",
+    {
+        "AfterConnectScript": str,
+        "CaptureDdls": bool,
+        "MaxFileSize": int,
+        "DatabaseName": str,
+        "DdlArtifactsSchema": str,
+        "ExecuteTimeout": int,
+        "FailTasksOnLobTruncation": bool,
+        "HeartbeatEnable": bool,
+        "HeartbeatSchema": str,
+        "HeartbeatFrequency": int,
+        "Password": str,
+        "Port": int,
+        "ServerName": str,
+        "Username": str,
+        "SlotName": str,
+        "PluginName": PluginNameValueType,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "TrimSpaceInChar": bool,
+        "MapBooleanAsBoolean": bool,
+        "MapJsonbAsClob": bool,
+        "MapLongVarcharAs": LongVarcharMappingTypeType,
+        "DatabaseMode": DatabaseModeType,
+        "BabelfishDatabaseName": str,
+    },
+)
+
+RedisSettingsOutputTypeDef = TypedDict(
+    "RedisSettingsOutputTypeDef",
+    {
+        "ServerName": str,
+        "Port": int,
+        "SslSecurityProtocol": SslSecurityProtocolValueType,
+        "AuthType": RedisAuthTypeValueType,
+        "AuthUserName": str,
+        "AuthPassword": str,
+        "SslCaCertificateArn": str,
+    },
+)
+
+RedshiftSettingsOutputTypeDef = TypedDict(
+    "RedshiftSettingsOutputTypeDef",
+    {
+        "AcceptAnyDate": bool,
+        "AfterConnectScript": str,
+        "BucketFolder": str,
+        "BucketName": str,
+        "CaseSensitiveNames": bool,
+        "CompUpdate": bool,
+        "ConnectionTimeout": int,
+        "DatabaseName": str,
+        "DateFormat": str,
+        "EmptyAsNull": bool,
+        "EncryptionMode": EncryptionModeValueType,
+        "ExplicitIds": bool,
+        "FileTransferUploadStreams": int,
+        "LoadTimeout": int,
+        "MaxFileSize": int,
+        "Password": str,
+        "Port": int,
+        "RemoveQuotes": bool,
+        "ReplaceInvalidChars": str,
+        "ReplaceChars": str,
+        "ServerName": str,
+        "ServiceAccessRoleArn": str,
+        "ServerSideEncryptionKmsKeyId": str,
+        "TimeFormat": str,
+        "TrimBlanks": bool,
+        "TruncateColumns": bool,
+        "Username": str,
+        "WriteBufferSize": int,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "MapBooleanAsBoolean": bool,
+    },
+)
+
+S3SettingsOutputTypeDef = TypedDict(
+    "S3SettingsOutputTypeDef",
+    {
+        "ServiceAccessRoleArn": str,
+        "ExternalTableDefinition": str,
+        "CsvRowDelimiter": str,
+        "CsvDelimiter": str,
+        "BucketFolder": str,
+        "BucketName": str,
+        "CompressionType": CompressionTypeValueType,
+        "EncryptionMode": EncryptionModeValueType,
+        "ServerSideEncryptionKmsKeyId": str,
+        "DataFormat": DataFormatValueType,
+        "EncodingType": EncodingTypeValueType,
+        "DictPageSizeLimit": int,
+        "RowGroupLength": int,
+        "DataPageSize": int,
+        "ParquetVersion": ParquetVersionValueType,
+        "EnableStatistics": bool,
+        "IncludeOpForFullLoad": bool,
+        "CdcInsertsOnly": bool,
+        "TimestampColumnName": str,
+        "ParquetTimestampInMillisecond": bool,
+        "CdcInsertsAndUpdates": bool,
+        "DatePartitionEnabled": bool,
+        "DatePartitionSequence": DatePartitionSequenceValueType,
+        "DatePartitionDelimiter": DatePartitionDelimiterValueType,
+        "UseCsvNoSupValue": bool,
+        "CsvNoSupValue": str,
+        "PreserveTransactions": bool,
+        "CdcPath": str,
+        "UseTaskStartTimeForFullLoadTimestamp": bool,
+        "CannedAclForObjects": CannedAclForObjectsValueType,
+        "AddColumnName": bool,
+        "CdcMaxBatchInterval": int,
+        "CdcMinFileSize": int,
+        "CsvNullValue": str,
+        "IgnoreHeaderRows": int,
+        "MaxFileSize": int,
+        "Rfc4180": bool,
+        "DatePartitionTimezone": str,
+        "AddTrailingPaddingCharacter": bool,
+        "ExpectedBucketOwner": str,
+        "GlueCatalogGeneration": bool,
+    },
+)
+
+SybaseSettingsOutputTypeDef = TypedDict(
+    "SybaseSettingsOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "Password": str,
+        "Port": int,
+        "ServerName": str,
+        "Username": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+    },
+)
+
+TimestreamSettingsOutputTypeDef = TypedDict(
+    "TimestreamSettingsOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "MemoryDuration": int,
+        "MagneticDuration": int,
+        "CdcInsertsAndUpdates": bool,
+        "EnableMagneticStoreWrites": bool,
+    },
+)
+
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
     },
 )
 _OptionalModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
@@ -1453,22 +1881,20 @@
         "SourceType": str,
         "EventCategories": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class ModifyEventSubscriptionMessageRequestTypeDef(
     _RequiredModifyEventSubscriptionMessageRequestTypeDef,
     _OptionalModifyEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
 )
 _OptionalModifyReplicationInstanceMessageRequestTypeDef = TypedDict(
@@ -1485,22 +1911,20 @@
         "AutoMinorVersionUpgrade": bool,
         "ReplicationInstanceIdentifier": str,
         "NetworkType": str,
     },
     total=False,
 )
 
-
 class ModifyReplicationInstanceMessageRequestTypeDef(
     _RequiredModifyReplicationInstanceMessageRequestTypeDef,
     _OptionalModifyReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyReplicationSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -1508,22 +1932,20 @@
     "_OptionalModifyReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupDescription": str,
     },
     total=False,
 )
 
-
 class ModifyReplicationSubnetGroupMessageRequestTypeDef(
     _RequiredModifyReplicationSubnetGroupMessageRequestTypeDef,
     _OptionalModifyReplicationSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyReplicationTaskMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
 _OptionalModifyReplicationTaskMessageRequestTypeDef = TypedDict(
@@ -1537,22 +1959,20 @@
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "TaskData": str,
     },
     total=False,
 )
 
-
 class ModifyReplicationTaskMessageRequestTypeDef(
     _RequiredModifyReplicationTaskMessageRequestTypeDef,
     _OptionalModifyReplicationTaskMessageRequestTypeDef,
 ):
     pass
 
-
 MoveReplicationTaskMessageRequestTypeDef = TypedDict(
     "MoveReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TargetReplicationInstanceArn": str,
     },
 )
@@ -1563,55 +1983,55 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-PendingMaintenanceActionTypeDef = TypedDict(
-    "PendingMaintenanceActionTypeDef",
+PendingMaintenanceActionOutputTypeDef = TypedDict(
+    "PendingMaintenanceActionOutputTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
 )
 
-ProvisionDataTypeDef = TypedDict(
-    "ProvisionDataTypeDef",
+ProvisionDataOutputTypeDef = TypedDict(
+    "ProvisionDataOutputTypeDef",
     {
         "ProvisionState": str,
         "ProvisionedCapacityUnits": int,
         "DateProvisioned": datetime,
         "IsNewProvisioningAvailable": bool,
         "DateNewProvisioningDataAvailable": datetime,
         "ReasonForNewProvisioningData": str,
     },
 )
 
-RdsConfigurationTypeDef = TypedDict(
-    "RdsConfigurationTypeDef",
+RdsConfigurationOutputTypeDef = TypedDict(
+    "RdsConfigurationOutputTypeDef",
     {
         "EngineEdition": str,
         "InstanceType": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageType": str,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
         "EngineVersion": str,
     },
 )
 
-RdsRequirementsTypeDef = TypedDict(
-    "RdsRequirementsTypeDef",
+RdsRequirementsOutputTypeDef = TypedDict(
+    "RdsRequirementsOutputTypeDef",
     {
         "EngineEdition": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
@@ -1630,21 +2050,27 @@
     {
         "ForceFailover": bool,
         "ForcePlannedFailover": bool,
     },
     total=False,
 )
 
-
 class RebootReplicationInstanceMessageRequestTypeDef(
     _RequiredRebootReplicationInstanceMessageRequestTypeDef,
     _OptionalRebootReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
+RecommendationSettingsOutputTypeDef = TypedDict(
+    "RecommendationSettingsOutputTypeDef",
+    {
+        "InstanceSizingType": str,
+        "WorkloadType": str,
+    },
+)
 
 RecommendationSettingsTypeDef = TypedDict(
     "RecommendationSettingsTypeDef",
     {
         "InstanceSizingType": str,
         "WorkloadType": str,
     },
@@ -1662,59 +2088,59 @@
     "TableToReloadTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
     },
 )
 
-ReloadReplicationTablesResponseTypeDef = TypedDict(
-    "ReloadReplicationTablesResponseTypeDef",
+ReloadReplicationTablesResponseOutputTypeDef = TypedDict(
+    "ReloadReplicationTablesResponseOutputTypeDef",
     {
         "ReplicationConfigArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReloadTablesResponseTypeDef = TypedDict(
-    "ReloadTablesResponseTypeDef",
+ReloadTablesResponseOutputTypeDef = TypedDict(
+    "ReloadTablesResponseOutputTypeDef",
     {
         "ReplicationTaskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RemoveTagsFromResourceMessageRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ReplicationPendingModifiedValuesTypeDef = TypedDict(
-    "ReplicationPendingModifiedValuesTypeDef",
+ReplicationPendingModifiedValuesOutputTypeDef = TypedDict(
+    "ReplicationPendingModifiedValuesOutputTypeDef",
     {
         "ReplicationInstanceClass": str,
         "AllocatedStorage": int,
         "MultiAZ": bool,
         "EngineVersion": str,
         "NetworkType": str,
     },
 )
 
-VpcSecurityGroupMembershipTypeDef = TypedDict(
-    "VpcSecurityGroupMembershipTypeDef",
+VpcSecurityGroupMembershipOutputTypeDef = TypedDict(
+    "VpcSecurityGroupMembershipOutputTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
 )
 
-ReplicationStatsTypeDef = TypedDict(
-    "ReplicationStatsTypeDef",
+ReplicationStatsOutputTypeDef = TypedDict(
+    "ReplicationStatsOutputTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
         "TablesLoaded": int,
         "TablesLoading": int,
         "TablesQueued": int,
         "TablesErrored": int,
@@ -1722,24 +2148,24 @@
         "StartDate": datetime,
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
     },
 )
 
-ReplicationTaskAssessmentRunProgressTypeDef = TypedDict(
-    "ReplicationTaskAssessmentRunProgressTypeDef",
+ReplicationTaskAssessmentRunProgressOutputTypeDef = TypedDict(
+    "ReplicationTaskAssessmentRunProgressOutputTypeDef",
     {
         "IndividualAssessmentCount": int,
         "IndividualAssessmentCompletedCount": int,
     },
 )
 
-ReplicationTaskStatsTypeDef = TypedDict(
-    "ReplicationTaskStatsTypeDef",
+ReplicationTaskStatsOutputTypeDef = TypedDict(
+    "ReplicationTaskStatsOutputTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
         "TablesLoaded": int,
         "TablesLoading": int,
         "TablesQueued": int,
         "TablesErrored": int,
@@ -1758,25 +2184,25 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+RunFleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
+    "RunFleetAdvisorLsaAnalysisResponseOutputTypeDef",
     {
         "LsaAnalysisId": str,
         "Status": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SchemaShortInfoResponseTypeDef = TypedDict(
-    "SchemaShortInfoResponseTypeDef",
+SchemaShortInfoResponseOutputTypeDef = TypedDict(
+    "SchemaShortInfoResponseOutputTypeDef",
     {
         "SchemaId": str,
         "SchemaName": str,
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
     },
@@ -1795,21 +2221,19 @@
         "CdcStartTime": Union[datetime, str],
         "CdcStartPosition": str,
         "CdcStopPosition": str,
     },
     total=False,
 )
 
-
 class StartReplicationMessageRequestTypeDef(
     _RequiredStartReplicationMessageRequestTypeDef, _OptionalStartReplicationMessageRequestTypeDef
 ):
     pass
 
-
 StartReplicationTaskAssessmentMessageRequestTypeDef = TypedDict(
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
 
@@ -1830,22 +2254,20 @@
         "ResultKmsKeyArn": str,
         "IncludeOnly": Sequence[str],
         "Exclude": Sequence[str],
     },
     total=False,
 )
 
-
 class StartReplicationTaskAssessmentRunMessageRequestTypeDef(
     _RequiredStartReplicationTaskAssessmentRunMessageRequestTypeDef,
     _OptionalStartReplicationTaskAssessmentRunMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartReplicationTaskMessageRequestTypeDef = TypedDict(
     "_RequiredStartReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "StartReplicationTaskType": StartReplicationTaskTypeValueType,
     },
 )
@@ -1855,22 +2277,20 @@
         "CdcStartTime": Union[datetime, str],
         "CdcStartPosition": str,
         "CdcStopPosition": str,
     },
     total=False,
 )
 
-
 class StartReplicationTaskMessageRequestTypeDef(
     _RequiredStartReplicationTaskMessageRequestTypeDef,
     _OptionalStartReplicationTaskMessageRequestTypeDef,
 ):
     pass
 
-
 StopReplicationMessageRequestTypeDef = TypedDict(
     "StopReplicationMessageRequestTypeDef",
     {
         "ReplicationConfigArn": str,
     },
 )
 
@@ -1893,26 +2313,26 @@
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     {
         "ForceMove": bool,
     },
     total=False,
 )
 
-UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+UpdateSubscriptionsToEventBridgeResponseOutputTypeDef = TypedDict(
+    "UpdateSubscriptionsToEventBridgeResponseOutputTypeDef",
     {
         "Result": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
+DescribeAccountAttributesResponseOutputTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseOutputTypeDef",
     {
-        "AccountQuotas": List[AccountQuotaTypeDef],
+        "AccountQuotas": List[AccountQuotaOutputTypeDef],
         "UniqueAccountIdentifier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
@@ -1937,22 +2357,20 @@
         "SourceIds": Sequence[str],
         "Enabled": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
         "ReplicationInstanceClass": str,
     },
 )
@@ -1973,22 +2391,20 @@
         "DnsNameServers": str,
         "ResourceIdentifier": str,
         "NetworkType": str,
     },
     total=False,
 )
 
-
 class CreateReplicationInstanceMessageRequestTypeDef(
     _RequiredCreateReplicationInstanceMessageRequestTypeDef,
     _OptionalCreateReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateReplicationSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "ReplicationSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -1997,22 +2413,20 @@
     "_OptionalCreateReplicationSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateReplicationSubnetGroupMessageRequestTypeDef(
     _RequiredCreateReplicationSubnetGroupMessageRequestTypeDef,
     _OptionalCreateReplicationSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateReplicationTaskMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationInstanceArn": str,
@@ -2030,22 +2444,20 @@
         "Tags": Sequence[TagTypeDef],
         "TaskData": str,
         "ResourceIdentifier": str,
     },
     total=False,
 )
 
-
 class CreateReplicationTaskMessageRequestTypeDef(
     _RequiredCreateReplicationTaskMessageRequestTypeDef,
     _OptionalCreateReplicationTaskMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredImportCertificateMessageRequestTypeDef = TypedDict(
     "_RequiredImportCertificateMessageRequestTypeDef",
     {
         "CertificateIdentifier": str,
     },
 )
 _OptionalImportCertificateMessageRequestTypeDef = TypedDict(
@@ -2054,87 +2466,94 @@
         "CertificatePem": str,
         "CertificateWallet": Union[str, bytes, IO[Any], StreamingBody],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ImportCertificateMessageRequestTypeDef(
     _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SubnetTypeDef = TypedDict(
-    "SubnetTypeDef",
+SubnetOutputTypeDef = TypedDict(
+    "SubnetOutputTypeDef",
     {
         "SubnetIdentifier": str,
-        "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
+        "SubnetAvailabilityZone": AvailabilityZoneOutputTypeDef,
         "SubnetStatus": str,
     },
 )
 
-BatchStartRecommendationsResponseTypeDef = TypedDict(
-    "BatchStartRecommendationsResponseTypeDef",
+BatchStartRecommendationsResponseOutputTypeDef = TypedDict(
+    "BatchStartRecommendationsResponseOutputTypeDef",
     {
-        "ErrorEntries": List[BatchStartRecommendationsErrorEntryTypeDef],
+        "ErrorEntries": List[BatchStartRecommendationsErrorEntryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteCertificateResponseTypeDef = TypedDict(
-    "DeleteCertificateResponseTypeDef",
+DeleteCertificateResponseOutputTypeDef = TypedDict(
+    "DeleteCertificateResponseOutputTypeDef",
     {
-        "Certificate": CertificateTypeDef,
+        "Certificate": CertificateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeCertificatesResponseTypeDef = TypedDict(
-    "DescribeCertificatesResponseTypeDef",
+DescribeCertificatesResponseOutputTypeDef = TypedDict(
+    "DescribeCertificatesResponseOutputTypeDef",
     {
         "Marker": str,
-        "Certificates": List[CertificateTypeDef],
+        "Certificates": List[CertificateOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ImportCertificateResponseTypeDef = TypedDict(
-    "ImportCertificateResponseTypeDef",
+ImportCertificateResponseOutputTypeDef = TypedDict(
+    "ImportCertificateResponseOutputTypeDef",
     {
-        "Certificate": CertificateTypeDef,
+        "Certificate": CertificateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CollectorResponseTypeDef = TypedDict(
-    "CollectorResponseTypeDef",
+CollectorResponseOutputTypeDef = TypedDict(
+    "CollectorResponseOutputTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
         "CollectorVersion": str,
         "VersionStatus": VersionStatusType,
         "Description": str,
         "S3BucketName": str,
         "ServiceAccessRoleArn": str,
-        "CollectorHealthCheck": CollectorHealthCheckTypeDef,
+        "CollectorHealthCheck": CollectorHealthCheckOutputTypeDef,
         "LastDataReceived": str,
         "RegisteredDate": str,
         "CreatedDate": str,
         "ModifiedDate": str,
-        "InventoryData": InventoryDataTypeDef,
+        "InventoryData": InventoryDataOutputTypeDef,
+    },
+)
+
+ReplicationConfigOutputTypeDef = TypedDict(
+    "ReplicationConfigOutputTypeDef",
+    {
+        "ReplicationConfigIdentifier": str,
+        "ReplicationConfigArn": str,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+        "ReplicationType": MigrationTypeValueType,
+        "ComputeConfig": ComputeConfigOutputTypeDef,
+        "ReplicationSettings": str,
+        "SupplementalSettings": str,
+        "TableMappings": str,
+        "ReplicationConfigCreateTime": datetime,
+        "ReplicationConfigUpdateTime": datetime,
     },
 )
 
 _RequiredCreateReplicationConfigMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationConfigMessageRequestTypeDef",
     {
         "ReplicationConfigIdentifier": str,
@@ -2152,22 +2571,20 @@
         "SupplementalSettings": str,
         "ResourceIdentifier": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateReplicationConfigMessageRequestTypeDef(
     _RequiredCreateReplicationConfigMessageRequestTypeDef,
     _OptionalCreateReplicationConfigMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyReplicationConfigMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationConfigMessageRequestTypeDef",
     {
         "ReplicationConfigArn": str,
     },
 )
 _OptionalModifyReplicationConfigMessageRequestTypeDef = TypedDict(
@@ -2181,60 +2598,41 @@
         "ComputeConfig": ComputeConfigTypeDef,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
     },
     total=False,
 )
 
-
 class ModifyReplicationConfigMessageRequestTypeDef(
     _RequiredModifyReplicationConfigMessageRequestTypeDef,
     _OptionalModifyReplicationConfigMessageRequestTypeDef,
 ):
     pass
 
-
-ReplicationConfigTypeDef = TypedDict(
-    "ReplicationConfigTypeDef",
-    {
-        "ReplicationConfigIdentifier": str,
-        "ReplicationConfigArn": str,
-        "SourceEndpointArn": str,
-        "TargetEndpointArn": str,
-        "ReplicationType": MigrationTypeValueType,
-        "ComputeConfig": ComputeConfigTypeDef,
-        "ReplicationSettings": str,
-        "SupplementalSettings": str,
-        "TableMappings": str,
-        "ReplicationConfigCreateTime": datetime,
-        "ReplicationConfigUpdateTime": datetime,
-    },
-)
-
-DeleteConnectionResponseTypeDef = TypedDict(
-    "DeleteConnectionResponseTypeDef",
+DeleteConnectionResponseOutputTypeDef = TypedDict(
+    "DeleteConnectionResponseOutputTypeDef",
     {
-        "Connection": ConnectionTypeDef,
+        "Connection": ConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeConnectionsResponseTypeDef = TypedDict(
-    "DescribeConnectionsResponseTypeDef",
+DescribeConnectionsResponseOutputTypeDef = TypedDict(
+    "DescribeConnectionsResponseOutputTypeDef",
     {
         "Marker": str,
-        "Connections": List[ConnectionTypeDef],
+        "Connections": List[ConnectionOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TestConnectionResponseTypeDef = TypedDict(
-    "TestConnectionResponseTypeDef",
+TestConnectionResponseOutputTypeDef = TypedDict(
+    "TestConnectionResponseOutputTypeDef",
     {
-        "Connection": ConnectionTypeDef,
+        "Connection": ConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointMessageRequestTypeDef",
     {
@@ -2278,63 +2676,19 @@
         "RedisSettings": RedisSettingsTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
         "TimestreamSettings": TimestreamSettingsTypeDef,
     },
     total=False,
 )
 
-
 class CreateEndpointMessageRequestTypeDef(
     _RequiredCreateEndpointMessageRequestTypeDef, _OptionalCreateEndpointMessageRequestTypeDef
 ):
     pass
 
-
-EndpointTypeDef = TypedDict(
-    "EndpointTypeDef",
-    {
-        "EndpointIdentifier": str,
-        "EndpointType": ReplicationEndpointTypeValueType,
-        "EngineName": str,
-        "EngineDisplayName": str,
-        "Username": str,
-        "ServerName": str,
-        "Port": int,
-        "DatabaseName": str,
-        "ExtraConnectionAttributes": str,
-        "Status": str,
-        "KmsKeyId": str,
-        "EndpointArn": str,
-        "CertificateArn": str,
-        "SslMode": DmsSslModeValueType,
-        "ServiceAccessRoleArn": str,
-        "ExternalTableDefinition": str,
-        "ExternalId": str,
-        "DynamoDbSettings": DynamoDbSettingsTypeDef,
-        "S3Settings": S3SettingsTypeDef,
-        "DmsTransferSettings": DmsTransferSettingsTypeDef,
-        "MongoDbSettings": MongoDbSettingsTypeDef,
-        "KinesisSettings": KinesisSettingsTypeDef,
-        "KafkaSettings": KafkaSettingsTypeDef,
-        "ElasticsearchSettings": ElasticsearchSettingsTypeDef,
-        "NeptuneSettings": NeptuneSettingsTypeDef,
-        "RedshiftSettings": RedshiftSettingsTypeDef,
-        "PostgreSQLSettings": PostgreSQLSettingsTypeDef,
-        "MySQLSettings": MySQLSettingsTypeDef,
-        "OracleSettings": OracleSettingsTypeDef,
-        "SybaseSettings": SybaseSettingsTypeDef,
-        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
-        "IBMDb2Settings": IBMDb2SettingsTypeDef,
-        "DocDbSettings": DocDbSettingsTypeDef,
-        "RedisSettings": RedisSettingsTypeDef,
-        "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
-        "TimestreamSettings": TimestreamSettingsTypeDef,
-    },
-)
-
 _RequiredModifyEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalModifyEndpointMessageRequestTypeDef = TypedDict(
@@ -2373,64 +2727,62 @@
         "ExactSettings": bool,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
         "TimestreamSettings": TimestreamSettingsTypeDef,
     },
     total=False,
 )
 
-
 class ModifyEndpointMessageRequestTypeDef(
     _RequiredModifyEndpointMessageRequestTypeDef, _OptionalModifyEndpointMessageRequestTypeDef
 ):
     pass
 
-
-CreateEventSubscriptionResponseTypeDef = TypedDict(
-    "CreateEventSubscriptionResponseTypeDef",
+CreateEventSubscriptionResponseOutputTypeDef = TypedDict(
+    "CreateEventSubscriptionResponseOutputTypeDef",
     {
-        "EventSubscription": EventSubscriptionTypeDef,
+        "EventSubscription": EventSubscriptionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEventSubscriptionResponseTypeDef = TypedDict(
-    "DeleteEventSubscriptionResponseTypeDef",
+DeleteEventSubscriptionResponseOutputTypeDef = TypedDict(
+    "DeleteEventSubscriptionResponseOutputTypeDef",
     {
-        "EventSubscription": EventSubscriptionTypeDef,
+        "EventSubscription": EventSubscriptionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventSubscriptionsResponseTypeDef = TypedDict(
-    "DescribeEventSubscriptionsResponseTypeDef",
+DescribeEventSubscriptionsResponseOutputTypeDef = TypedDict(
+    "DescribeEventSubscriptionsResponseOutputTypeDef",
     {
         "Marker": str,
-        "EventSubscriptionsList": List[EventSubscriptionTypeDef],
+        "EventSubscriptionsList": List[EventSubscriptionOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyEventSubscriptionResponseTypeDef = TypedDict(
-    "ModifyEventSubscriptionResponseTypeDef",
+ModifyEventSubscriptionResponseOutputTypeDef = TypedDict(
+    "ModifyEventSubscriptionResponseOutputTypeDef",
     {
-        "EventSubscription": EventSubscriptionTypeDef,
+        "EventSubscription": EventSubscriptionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatabaseResponseTypeDef = TypedDict(
-    "DatabaseResponseTypeDef",
+DatabaseResponseOutputTypeDef = TypedDict(
+    "DatabaseResponseOutputTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "IpAddress": str,
         "NumberOfSchemas": int,
-        "Server": ServerShortInfoResponseTypeDef,
-        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
-        "Collectors": List[CollectorShortInfoResponseTypeDef],
+        "Server": ServerShortInfoResponseOutputTypeDef,
+        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseOutputTypeDef,
+        "Collectors": List[CollectorShortInfoResponseOutputTypeDef],
     },
 )
 
 DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -2698,22 +3050,20 @@
         "MaxRecords": int,
         "Marker": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
 class DescribeReplicationTableStatisticsMessageRequestTypeDef(
     _RequiredDescribeReplicationTableStatisticsMessageRequestTypeDef,
     _OptionalDescribeReplicationTableStatisticsMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2772,22 +3122,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
     _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
     _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
 _OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
@@ -2796,22 +3144,20 @@
         "MaxRecords": int,
         "Marker": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
 class DescribeTableStatisticsMessageRequestTypeDef(
     _RequiredDescribeTableStatisticsMessageRequestTypeDef,
     _OptionalDescribeTableStatisticsMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef = TypedDict(
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
@@ -2896,163 +3242,215 @@
         "Marker": str,
         "WithoutSettings": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEndpointSettingsResponseTypeDef = TypedDict(
-    "DescribeEndpointSettingsResponseTypeDef",
+DescribeEndpointSettingsResponseOutputTypeDef = TypedDict(
+    "DescribeEndpointSettingsResponseOutputTypeDef",
     {
         "Marker": str,
-        "EndpointSettings": List[EndpointSettingTypeDef],
+        "EndpointSettings": List[EndpointSettingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEndpointTypesResponseTypeDef = TypedDict(
-    "DescribeEndpointTypesResponseTypeDef",
+DescribeEndpointTypesResponseOutputTypeDef = TypedDict(
+    "DescribeEndpointTypesResponseOutputTypeDef",
     {
         "Marker": str,
-        "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
+        "SupportedEndpointTypes": List[SupportedEndpointTypeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventCategoriesResponseTypeDef = TypedDict(
-    "DescribeEventCategoriesResponseTypeDef",
+DescribeEventCategoriesResponseOutputTypeDef = TypedDict(
+    "DescribeEventCategoriesResponseOutputTypeDef",
     {
-        "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
+        "EventCategoryGroupList": List[EventCategoryGroupOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventsResponseTypeDef = TypedDict(
-    "DescribeEventsResponseTypeDef",
+DescribeEventsResponseOutputTypeDef = TypedDict(
+    "DescribeEventsResponseOutputTypeDef",
     {
         "Marker": str,
-        "Events": List[EventTypeDef],
+        "Events": List[EventOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
+DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
+    "DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef",
     {
-        "Analysis": List[FleetAdvisorLsaAnalysisResponseTypeDef],
+        "Analysis": List[FleetAdvisorLsaAnalysisResponseOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
+DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef = TypedDict(
+    "DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef",
     {
-        "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseTypeDef],
+        "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeOrderableReplicationInstancesResponseTypeDef = TypedDict(
-    "DescribeOrderableReplicationInstancesResponseTypeDef",
+DescribeOrderableReplicationInstancesResponseOutputTypeDef = TypedDict(
+    "DescribeOrderableReplicationInstancesResponseOutputTypeDef",
     {
-        "OrderableReplicationInstances": List[OrderableReplicationInstanceTypeDef],
+        "OrderableReplicationInstances": List[OrderableReplicationInstanceOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecommendationLimitationsResponseTypeDef = TypedDict(
-    "DescribeRecommendationLimitationsResponseTypeDef",
+DescribeRecommendationLimitationsResponseOutputTypeDef = TypedDict(
+    "DescribeRecommendationLimitationsResponseOutputTypeDef",
     {
         "NextToken": str,
-        "Limitations": List[LimitationTypeDef],
+        "Limitations": List[LimitationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRefreshSchemasStatusResponseTypeDef = TypedDict(
-    "DescribeRefreshSchemasStatusResponseTypeDef",
+DescribeRefreshSchemasStatusResponseOutputTypeDef = TypedDict(
+    "DescribeRefreshSchemasStatusResponseOutputTypeDef",
     {
-        "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
+        "RefreshSchemasStatus": RefreshSchemasStatusOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RefreshSchemasResponseTypeDef = TypedDict(
-    "RefreshSchemasResponseTypeDef",
+RefreshSchemasResponseOutputTypeDef = TypedDict(
+    "RefreshSchemasResponseOutputTypeDef",
     {
-        "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
+        "RefreshSchemasStatus": RefreshSchemasStatusOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationInstanceTaskLogsResponseTypeDef = TypedDict(
-    "DescribeReplicationInstanceTaskLogsResponseTypeDef",
+DescribeReplicationInstanceTaskLogsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationInstanceTaskLogsResponseOutputTypeDef",
     {
         "ReplicationInstanceArn": str,
-        "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
+        "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTableStatisticsResponseTypeDef = TypedDict(
-    "DescribeReplicationTableStatisticsResponseTypeDef",
+DescribeReplicationTableStatisticsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationTableStatisticsResponseOutputTypeDef",
     {
         "ReplicationConfigArn": str,
         "Marker": str,
-        "ReplicationTableStatistics": List[TableStatisticsTypeDef],
+        "ReplicationTableStatistics": List[TableStatisticsOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeTableStatisticsResponseTypeDef = TypedDict(
-    "DescribeTableStatisticsResponseTypeDef",
+DescribeTableStatisticsResponseOutputTypeDef = TypedDict(
+    "DescribeTableStatisticsResponseOutputTypeDef",
     {
         "ReplicationTaskArn": str,
-        "TableStatistics": List[TableStatisticsTypeDef],
+        "TableStatistics": List[TableStatisticsOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
+DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef",
     {
         "Marker": str,
         "BucketName": str,
-        "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
+        "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskIndividualAssessmentsResponseTypeDef = TypedDict(
-    "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
+DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
+        "ReplicationTaskIndividualAssessments": List[
+            ReplicationTaskIndividualAssessmentOutputTypeDef
+        ],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResourcePendingMaintenanceActionsTypeDef = TypedDict(
-    "ResourcePendingMaintenanceActionsTypeDef",
+EndpointOutputTypeDef = TypedDict(
+    "EndpointOutputTypeDef",
+    {
+        "EndpointIdentifier": str,
+        "EndpointType": ReplicationEndpointTypeValueType,
+        "EngineName": str,
+        "EngineDisplayName": str,
+        "Username": str,
+        "ServerName": str,
+        "Port": int,
+        "DatabaseName": str,
+        "ExtraConnectionAttributes": str,
+        "Status": str,
+        "KmsKeyId": str,
+        "EndpointArn": str,
+        "CertificateArn": str,
+        "SslMode": DmsSslModeValueType,
+        "ServiceAccessRoleArn": str,
+        "ExternalTableDefinition": str,
+        "ExternalId": str,
+        "DynamoDbSettings": DynamoDbSettingsOutputTypeDef,
+        "S3Settings": S3SettingsOutputTypeDef,
+        "DmsTransferSettings": DmsTransferSettingsOutputTypeDef,
+        "MongoDbSettings": MongoDbSettingsOutputTypeDef,
+        "KinesisSettings": KinesisSettingsOutputTypeDef,
+        "KafkaSettings": KafkaSettingsOutputTypeDef,
+        "ElasticsearchSettings": ElasticsearchSettingsOutputTypeDef,
+        "NeptuneSettings": NeptuneSettingsOutputTypeDef,
+        "RedshiftSettings": RedshiftSettingsOutputTypeDef,
+        "PostgreSQLSettings": PostgreSQLSettingsOutputTypeDef,
+        "MySQLSettings": MySQLSettingsOutputTypeDef,
+        "OracleSettings": OracleSettingsOutputTypeDef,
+        "SybaseSettings": SybaseSettingsOutputTypeDef,
+        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsOutputTypeDef,
+        "IBMDb2Settings": IBMDb2SettingsOutputTypeDef,
+        "DocDbSettings": DocDbSettingsOutputTypeDef,
+        "RedisSettings": RedisSettingsOutputTypeDef,
+        "GcpMySQLSettings": GcpMySQLSettingsOutputTypeDef,
+        "TimestreamSettings": TimestreamSettingsOutputTypeDef,
+    },
+)
+
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ResourcePendingMaintenanceActionsOutputTypeDef = TypedDict(
+    "ResourcePendingMaintenanceActionsOutputTypeDef",
     {
         "ResourceIdentifier": str,
-        "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
+        "PendingMaintenanceActionDetails": List[PendingMaintenanceActionOutputTypeDef],
     },
 )
 
-RdsRecommendationTypeDef = TypedDict(
-    "RdsRecommendationTypeDef",
+RdsRecommendationOutputTypeDef = TypedDict(
+    "RdsRecommendationOutputTypeDef",
     {
-        "RequirementsToTarget": RdsRequirementsTypeDef,
-        "TargetConfiguration": RdsConfigurationTypeDef,
+        "RequirementsToTarget": RdsRequirementsOutputTypeDef,
+        "TargetConfiguration": RdsConfigurationOutputTypeDef,
     },
 )
 
 StartRecommendationsRequestEntryTypeDef = TypedDict(
     "StartRecommendationsRequestEntryTypeDef",
     {
         "DatabaseId": str,
@@ -3079,22 +3477,20 @@
     "_OptionalReloadReplicationTablesMessageRequestTypeDef",
     {
         "ReloadOption": ReloadOptionValueType,
     },
     total=False,
 )
 
-
 class ReloadReplicationTablesMessageRequestTypeDef(
     _RequiredReloadReplicationTablesMessageRequestTypeDef,
     _OptionalReloadReplicationTablesMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredReloadTablesMessageRequestTypeDef = TypedDict(
     "_RequiredReloadTablesMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TablesToReload": Sequence[TableToReloadTypeDef],
     },
 )
@@ -3102,65 +3498,63 @@
     "_OptionalReloadTablesMessageRequestTypeDef",
     {
         "ReloadOption": ReloadOptionValueType,
     },
     total=False,
 )
 
-
 class ReloadTablesMessageRequestTypeDef(
     _RequiredReloadTablesMessageRequestTypeDef, _OptionalReloadTablesMessageRequestTypeDef
 ):
     pass
 
-
-ReplicationTypeDef = TypedDict(
-    "ReplicationTypeDef",
+ReplicationOutputTypeDef = TypedDict(
+    "ReplicationOutputTypeDef",
     {
         "ReplicationConfigIdentifier": str,
         "ReplicationConfigArn": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationType": MigrationTypeValueType,
         "Status": str,
-        "ProvisionData": ProvisionDataTypeDef,
+        "ProvisionData": ProvisionDataOutputTypeDef,
         "StopReason": str,
         "FailureMessages": List[str],
-        "ReplicationStats": ReplicationStatsTypeDef,
+        "ReplicationStats": ReplicationStatsOutputTypeDef,
         "StartReplicationType": str,
         "CdcStartTime": datetime,
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationCreateTime": datetime,
         "ReplicationUpdateTime": datetime,
         "ReplicationLastStopTime": datetime,
     },
 )
 
-ReplicationTaskAssessmentRunTypeDef = TypedDict(
-    "ReplicationTaskAssessmentRunTypeDef",
+ReplicationTaskAssessmentRunOutputTypeDef = TypedDict(
+    "ReplicationTaskAssessmentRunOutputTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
         "ReplicationTaskArn": str,
         "Status": str,
         "ReplicationTaskAssessmentRunCreationDate": datetime,
-        "AssessmentProgress": ReplicationTaskAssessmentRunProgressTypeDef,
+        "AssessmentProgress": ReplicationTaskAssessmentRunProgressOutputTypeDef,
         "LastFailureMessage": str,
         "ServiceAccessRoleArn": str,
         "ResultLocationBucket": str,
         "ResultLocationFolder": str,
         "ResultEncryptionMode": str,
         "ResultKmsKeyArn": str,
         "AssessmentRunName": str,
     },
 )
 
-ReplicationTaskTypeDef = TypedDict(
-    "ReplicationTaskTypeDef",
+ReplicationTaskOutputTypeDef = TypedDict(
+    "ReplicationTaskOutputTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationInstanceArn": str,
         "MigrationType": MigrationTypeValueType,
         "TableMappings": str,
@@ -3170,333 +3564,333 @@
         "StopReason": str,
         "ReplicationTaskCreationDate": datetime,
         "ReplicationTaskStartDate": datetime,
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationTaskArn": str,
-        "ReplicationTaskStats": ReplicationTaskStatsTypeDef,
+        "ReplicationTaskStats": ReplicationTaskStatsOutputTypeDef,
         "TaskData": str,
         "TargetReplicationInstanceArn": str,
     },
 )
 
-SchemaResponseTypeDef = TypedDict(
-    "SchemaResponseTypeDef",
+SchemaResponseOutputTypeDef = TypedDict(
+    "SchemaResponseOutputTypeDef",
     {
         "CodeLineCount": int,
         "CodeSize": int,
         "Complexity": str,
-        "Server": ServerShortInfoResponseTypeDef,
-        "DatabaseInstance": DatabaseShortInfoResponseTypeDef,
+        "Server": ServerShortInfoResponseOutputTypeDef,
+        "DatabaseInstance": DatabaseShortInfoResponseOutputTypeDef,
         "SchemaId": str,
         "SchemaName": str,
-        "OriginalSchema": SchemaShortInfoResponseTypeDef,
+        "OriginalSchema": SchemaShortInfoResponseOutputTypeDef,
         "Similarity": float,
     },
 )
 
-ReplicationSubnetGroupTypeDef = TypedDict(
-    "ReplicationSubnetGroupTypeDef",
+ReplicationSubnetGroupOutputTypeDef = TypedDict(
+    "ReplicationSubnetGroupOutputTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "ReplicationSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
-        "Subnets": List[SubnetTypeDef],
+        "Subnets": List[SubnetOutputTypeDef],
         "SupportedNetworkTypes": List[str],
     },
 )
 
-DescribeFleetAdvisorCollectorsResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorCollectorsResponseTypeDef",
+DescribeFleetAdvisorCollectorsResponseOutputTypeDef = TypedDict(
+    "DescribeFleetAdvisorCollectorsResponseOutputTypeDef",
     {
-        "Collectors": List[CollectorResponseTypeDef],
+        "Collectors": List[CollectorResponseOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationConfigResponseTypeDef = TypedDict(
-    "CreateReplicationConfigResponseTypeDef",
+CreateReplicationConfigResponseOutputTypeDef = TypedDict(
+    "CreateReplicationConfigResponseOutputTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationConfigResponseTypeDef = TypedDict(
-    "DeleteReplicationConfigResponseTypeDef",
+DeleteReplicationConfigResponseOutputTypeDef = TypedDict(
+    "DeleteReplicationConfigResponseOutputTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationConfigsResponseTypeDef = TypedDict(
-    "DescribeReplicationConfigsResponseTypeDef",
+DescribeReplicationConfigsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationConfigsResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationConfigs": List[ReplicationConfigTypeDef],
+        "ReplicationConfigs": List[ReplicationConfigOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationConfigResponseTypeDef = TypedDict(
-    "ModifyReplicationConfigResponseTypeDef",
+ModifyReplicationConfigResponseOutputTypeDef = TypedDict(
+    "ModifyReplicationConfigResponseOutputTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
+DescribeFleetAdvisorDatabasesResponseOutputTypeDef = TypedDict(
+    "DescribeFleetAdvisorDatabasesResponseOutputTypeDef",
     {
-        "Endpoint": EndpointTypeDef,
+        "Databases": List[DatabaseResponseOutputTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEndpointResponseTypeDef = TypedDict(
-    "DeleteEndpointResponseTypeDef",
+CreateEndpointResponseOutputTypeDef = TypedDict(
+    "CreateEndpointResponseOutputTypeDef",
     {
-        "Endpoint": EndpointTypeDef,
+        "Endpoint": EndpointOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEndpointsResponseTypeDef = TypedDict(
-    "DescribeEndpointsResponseTypeDef",
+DeleteEndpointResponseOutputTypeDef = TypedDict(
+    "DeleteEndpointResponseOutputTypeDef",
     {
-        "Marker": str,
-        "Endpoints": List[EndpointTypeDef],
+        "Endpoint": EndpointOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyEndpointResponseTypeDef = TypedDict(
-    "ModifyEndpointResponseTypeDef",
+DescribeEndpointsResponseOutputTypeDef = TypedDict(
+    "DescribeEndpointsResponseOutputTypeDef",
     {
-        "Endpoint": EndpointTypeDef,
+        "Marker": str,
+        "Endpoints": List[EndpointOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
+ModifyEndpointResponseOutputTypeDef = TypedDict(
+    "ModifyEndpointResponseOutputTypeDef",
     {
-        "Databases": List[DatabaseResponseTypeDef],
-        "NextToken": str,
+        "Endpoint": EndpointOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
-    "ApplyPendingMaintenanceActionResponseTypeDef",
+ApplyPendingMaintenanceActionResponseOutputTypeDef = TypedDict(
+    "ApplyPendingMaintenanceActionResponseOutputTypeDef",
     {
-        "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
+        "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribePendingMaintenanceActionsResponseTypeDef = TypedDict(
-    "DescribePendingMaintenanceActionsResponseTypeDef",
+DescribePendingMaintenanceActionsResponseOutputTypeDef = TypedDict(
+    "DescribePendingMaintenanceActionsResponseOutputTypeDef",
     {
-        "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
+        "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecommendationDataTypeDef = TypedDict(
-    "RecommendationDataTypeDef",
+RecommendationDataOutputTypeDef = TypedDict(
+    "RecommendationDataOutputTypeDef",
     {
-        "RdsEngine": RdsRecommendationTypeDef,
+        "RdsEngine": RdsRecommendationOutputTypeDef,
     },
 )
 
 BatchStartRecommendationsRequestRequestTypeDef = TypedDict(
     "BatchStartRecommendationsRequestRequestTypeDef",
     {
         "Data": Sequence[StartRecommendationsRequestEntryTypeDef],
     },
     total=False,
 )
 
-DescribeReplicationsResponseTypeDef = TypedDict(
-    "DescribeReplicationsResponseTypeDef",
+DescribeReplicationsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationsResponseOutputTypeDef",
     {
         "Marker": str,
-        "Replications": List[ReplicationTypeDef],
+        "Replications": List[ReplicationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationResponseTypeDef = TypedDict(
-    "StartReplicationResponseTypeDef",
+StartReplicationResponseOutputTypeDef = TypedDict(
+    "StartReplicationResponseOutputTypeDef",
     {
-        "Replication": ReplicationTypeDef,
+        "Replication": ReplicationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopReplicationResponseTypeDef = TypedDict(
-    "StopReplicationResponseTypeDef",
+StopReplicationResponseOutputTypeDef = TypedDict(
+    "StopReplicationResponseOutputTypeDef",
     {
-        "Replication": ReplicationTypeDef,
+        "Replication": ReplicationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
-    "CancelReplicationTaskAssessmentRunResponseTypeDef",
+CancelReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
+    "CancelReplicationTaskAssessmentRunResponseOutputTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
-    "DeleteReplicationTaskAssessmentRunResponseTypeDef",
+DeleteReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
+    "DeleteReplicationTaskAssessmentRunResponseOutputTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskAssessmentRunsResponseTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
+DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunTypeDef],
+        "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
-    "StartReplicationTaskAssessmentRunResponseTypeDef",
+StartReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
+    "StartReplicationTaskAssessmentRunResponseOutputTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationTaskResponseTypeDef = TypedDict(
-    "CreateReplicationTaskResponseTypeDef",
+CreateReplicationTaskResponseOutputTypeDef = TypedDict(
+    "CreateReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationTaskResponseTypeDef = TypedDict(
-    "DeleteReplicationTaskResponseTypeDef",
+DeleteReplicationTaskResponseOutputTypeDef = TypedDict(
+    "DeleteReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTasksResponseTypeDef = TypedDict(
-    "DescribeReplicationTasksResponseTypeDef",
+DescribeReplicationTasksResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationTasksResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationTasks": List[ReplicationTaskTypeDef],
+        "ReplicationTasks": List[ReplicationTaskOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationTaskResponseTypeDef = TypedDict(
-    "ModifyReplicationTaskResponseTypeDef",
+ModifyReplicationTaskResponseOutputTypeDef = TypedDict(
+    "ModifyReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-MoveReplicationTaskResponseTypeDef = TypedDict(
-    "MoveReplicationTaskResponseTypeDef",
+MoveReplicationTaskResponseOutputTypeDef = TypedDict(
+    "MoveReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskAssessmentResponseTypeDef = TypedDict(
-    "StartReplicationTaskAssessmentResponseTypeDef",
+StartReplicationTaskAssessmentResponseOutputTypeDef = TypedDict(
+    "StartReplicationTaskAssessmentResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskResponseTypeDef = TypedDict(
-    "StartReplicationTaskResponseTypeDef",
+StartReplicationTaskResponseOutputTypeDef = TypedDict(
+    "StartReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopReplicationTaskResponseTypeDef = TypedDict(
-    "StopReplicationTaskResponseTypeDef",
+StopReplicationTaskResponseOutputTypeDef = TypedDict(
+    "StopReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorSchemasResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorSchemasResponseTypeDef",
+DescribeFleetAdvisorSchemasResponseOutputTypeDef = TypedDict(
+    "DescribeFleetAdvisorSchemasResponseOutputTypeDef",
     {
-        "FleetAdvisorSchemas": List[SchemaResponseTypeDef],
+        "FleetAdvisorSchemas": List[SchemaResponseOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationSubnetGroupResponseTypeDef = TypedDict(
-    "CreateReplicationSubnetGroupResponseTypeDef",
+CreateReplicationSubnetGroupResponseOutputTypeDef = TypedDict(
+    "CreateReplicationSubnetGroupResponseOutputTypeDef",
     {
-        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationSubnetGroupsResponseTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsResponseTypeDef",
+DescribeReplicationSubnetGroupsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationSubnetGroups": List[ReplicationSubnetGroupTypeDef],
+        "ReplicationSubnetGroups": List[ReplicationSubnetGroupOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationSubnetGroupResponseTypeDef = TypedDict(
-    "ModifyReplicationSubnetGroupResponseTypeDef",
+ModifyReplicationSubnetGroupResponseOutputTypeDef = TypedDict(
+    "ModifyReplicationSubnetGroupResponseOutputTypeDef",
     {
-        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReplicationInstanceTypeDef = TypedDict(
-    "ReplicationInstanceTypeDef",
+ReplicationInstanceOutputTypeDef = TypedDict(
+    "ReplicationInstanceOutputTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
         "ReplicationInstanceClass": str,
         "ReplicationInstanceStatus": str,
         "AllocatedStorage": int,
         "InstanceCreateTime": datetime,
-        "VpcSecurityGroups": List[VpcSecurityGroupMembershipTypeDef],
+        "VpcSecurityGroups": List[VpcSecurityGroupMembershipOutputTypeDef],
         "AvailabilityZone": str,
-        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
         "PreferredMaintenanceWindow": str,
-        "PendingModifiedValues": ReplicationPendingModifiedValuesTypeDef,
+        "PendingModifiedValues": ReplicationPendingModifiedValuesOutputTypeDef,
         "MultiAZ": bool,
         "EngineVersion": str,
         "AutoMinorVersionUpgrade": bool,
         "KmsKeyId": str,
         "ReplicationInstanceArn": str,
         "ReplicationInstancePublicIpAddress": str,
         "ReplicationInstancePrivateIpAddress": str,
@@ -3507,69 +3901,69 @@
         "SecondaryAvailabilityZone": str,
         "FreeUntil": datetime,
         "DnsNameServers": str,
         "NetworkType": str,
     },
 )
 
-RecommendationTypeDef = TypedDict(
-    "RecommendationTypeDef",
+RecommendationOutputTypeDef = TypedDict(
+    "RecommendationOutputTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "CreatedDate": str,
         "Status": str,
         "Preferred": bool,
-        "Settings": RecommendationSettingsTypeDef,
-        "Data": RecommendationDataTypeDef,
+        "Settings": RecommendationSettingsOutputTypeDef,
+        "Data": RecommendationDataOutputTypeDef,
     },
 )
 
-CreateReplicationInstanceResponseTypeDef = TypedDict(
-    "CreateReplicationInstanceResponseTypeDef",
+CreateReplicationInstanceResponseOutputTypeDef = TypedDict(
+    "CreateReplicationInstanceResponseOutputTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceTypeDef,
+        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationInstanceResponseTypeDef = TypedDict(
-    "DeleteReplicationInstanceResponseTypeDef",
+DeleteReplicationInstanceResponseOutputTypeDef = TypedDict(
+    "DeleteReplicationInstanceResponseOutputTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceTypeDef,
+        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationInstancesResponseTypeDef = TypedDict(
-    "DescribeReplicationInstancesResponseTypeDef",
+DescribeReplicationInstancesResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationInstancesResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationInstances": List[ReplicationInstanceTypeDef],
+        "ReplicationInstances": List[ReplicationInstanceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationInstanceResponseTypeDef = TypedDict(
-    "ModifyReplicationInstanceResponseTypeDef",
+ModifyReplicationInstanceResponseOutputTypeDef = TypedDict(
+    "ModifyReplicationInstanceResponseOutputTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceTypeDef,
+        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RebootReplicationInstanceResponseTypeDef = TypedDict(
-    "RebootReplicationInstanceResponseTypeDef",
+RebootReplicationInstanceResponseOutputTypeDef = TypedDict(
+    "RebootReplicationInstanceResponseOutputTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceTypeDef,
+        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecommendationsResponseTypeDef = TypedDict(
-    "DescribeRecommendationsResponseTypeDef",
+DescribeRecommendationsResponseOutputTypeDef = TypedDict(
+    "DescribeRecommendationsResponseOutputTypeDef",
     {
         "NextToken": str,
-        "Recommendations": List[RecommendationTypeDef],
+        "Recommendations": List[RecommendationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/type_defs.pyi` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/type_defs.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dms.type_defs import AccountQuotaTypeDef
+    from mypy_boto3_dms.type_defs import AccountQuotaOutputTypeDef
 
-    data: AccountQuotaTypeDef = {...}
+    data: AccountQuotaOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -59,27 +59,29 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "AccountQuotaTypeDef",
+    "AccountQuotaOutputTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
-    "AvailabilityZoneTypeDef",
-    "BatchStartRecommendationsErrorEntryTypeDef",
+    "AvailabilityZoneOutputTypeDef",
+    "BatchStartRecommendationsErrorEntryOutputTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
-    "CertificateTypeDef",
-    "CollectorHealthCheckTypeDef",
-    "InventoryDataTypeDef",
-    "CollectorShortInfoResponseTypeDef",
+    "CertificateOutputTypeDef",
+    "CollectorHealthCheckOutputTypeDef",
+    "InventoryDataOutputTypeDef",
+    "CollectorShortInfoResponseOutputTypeDef",
+    "ComputeConfigOutputTypeDef",
     "ComputeConfigTypeDef",
-    "ConnectionTypeDef",
+    "ConnectionOutputTypeDef",
     "DmsTransferSettingsTypeDef",
     "DocDbSettingsTypeDef",
     "DynamoDbSettingsTypeDef",
     "ElasticsearchSettingsTypeDef",
     "GcpMySQLSettingsTypeDef",
     "IBMDb2SettingsTypeDef",
     "KafkaSettingsTypeDef",
@@ -91,124 +93,143 @@
     "OracleSettingsTypeDef",
     "PostgreSQLSettingsTypeDef",
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
     "TimestreamSettingsTypeDef",
-    "EventSubscriptionTypeDef",
+    "EventSubscriptionOutputTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    "DatabaseInstanceSoftwareDetailsResponseTypeDef",
-    "ServerShortInfoResponseTypeDef",
-    "DatabaseShortInfoResponseTypeDef",
+    "CreateFleetAdvisorCollectorResponseOutputTypeDef",
+    "DatabaseInstanceSoftwareDetailsResponseOutputTypeDef",
+    "ServerShortInfoResponseOutputTypeDef",
+    "DatabaseShortInfoResponseOutputTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
+    "DeleteFleetAdvisorDatabasesResponseOutputTypeDef",
     "DeleteReplicationConfigMessageRequestTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
+    "DescribeApplicableIndividualAssessmentsResponseOutputTypeDef",
     "FilterTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
-    "EndpointSettingTypeDef",
-    "SupportedEndpointTypeTypeDef",
-    "EventCategoryGroupTypeDef",
-    "EventTypeDef",
+    "EndpointSettingOutputTypeDef",
+    "SupportedEndpointTypeOutputTypeDef",
+    "EventCategoryGroupOutputTypeDef",
+    "EventOutputTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
-    "FleetAdvisorLsaAnalysisResponseTypeDef",
-    "FleetAdvisorSchemaObjectResponseTypeDef",
+    "FleetAdvisorLsaAnalysisResponseOutputTypeDef",
+    "FleetAdvisorSchemaObjectResponseOutputTypeDef",
     "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
-    "OrderableReplicationInstanceTypeDef",
-    "LimitationTypeDef",
+    "OrderableReplicationInstanceOutputTypeDef",
+    "LimitationOutputTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
-    "RefreshSchemasStatusTypeDef",
+    "RefreshSchemasStatusOutputTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
-    "ReplicationInstanceTaskLogTypeDef",
-    "TableStatisticsTypeDef",
+    "ReplicationInstanceTaskLogOutputTypeDef",
+    "TableStatisticsOutputTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
-    "ReplicationTaskAssessmentResultTypeDef",
-    "ReplicationTaskIndividualAssessmentTypeDef",
+    "ReplicationTaskAssessmentResultOutputTypeDef",
+    "ReplicationTaskIndividualAssessmentOutputTypeDef",
     "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
-    "DescribeSchemasResponseTypeDef",
+    "DescribeSchemasResponseOutputTypeDef",
+    "DmsTransferSettingsOutputTypeDef",
+    "DocDbSettingsOutputTypeDef",
+    "DynamoDbSettingsOutputTypeDef",
+    "ElasticsearchSettingsOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "GcpMySQLSettingsOutputTypeDef",
+    "IBMDb2SettingsOutputTypeDef",
+    "KafkaSettingsOutputTypeDef",
+    "KinesisSettingsOutputTypeDef",
+    "MicrosoftSQLServerSettingsOutputTypeDef",
+    "MongoDbSettingsOutputTypeDef",
+    "MySQLSettingsOutputTypeDef",
+    "NeptuneSettingsOutputTypeDef",
+    "OracleSettingsOutputTypeDef",
+    "PostgreSQLSettingsOutputTypeDef",
+    "RedisSettingsOutputTypeDef",
+    "RedshiftSettingsOutputTypeDef",
+    "S3SettingsOutputTypeDef",
+    "SybaseSettingsOutputTypeDef",
+    "TimestreamSettingsOutputTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
+    "TagOutputTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "PendingMaintenanceActionTypeDef",
-    "ProvisionDataTypeDef",
-    "RdsConfigurationTypeDef",
-    "RdsRequirementsTypeDef",
+    "PendingMaintenanceActionOutputTypeDef",
+    "ProvisionDataOutputTypeDef",
+    "RdsConfigurationOutputTypeDef",
+    "RdsRequirementsOutputTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
+    "RecommendationSettingsOutputTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
-    "ReloadReplicationTablesResponseTypeDef",
-    "ReloadTablesResponseTypeDef",
+    "ReloadReplicationTablesResponseOutputTypeDef",
+    "ReloadTablesResponseOutputTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ReplicationPendingModifiedValuesTypeDef",
-    "VpcSecurityGroupMembershipTypeDef",
-    "ReplicationStatsTypeDef",
-    "ReplicationTaskAssessmentRunProgressTypeDef",
-    "ReplicationTaskStatsTypeDef",
+    "ReplicationPendingModifiedValuesOutputTypeDef",
+    "VpcSecurityGroupMembershipOutputTypeDef",
+    "ReplicationStatsOutputTypeDef",
+    "ReplicationTaskAssessmentRunProgressOutputTypeDef",
+    "ReplicationTaskStatsOutputTypeDef",
     "ResponseMetadataTypeDef",
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    "SchemaShortInfoResponseTypeDef",
+    "RunFleetAdvisorLsaAnalysisResponseOutputTypeDef",
+    "SchemaShortInfoResponseOutputTypeDef",
     "StartReplicationMessageRequestTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
     "StartReplicationTaskMessageRequestTypeDef",
     "StopReplicationMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
+    "UpdateSubscriptionsToEventBridgeResponseOutputTypeDef",
+    "DescribeAccountAttributesResponseOutputTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ImportCertificateMessageRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "SubnetTypeDef",
-    "BatchStartRecommendationsResponseTypeDef",
-    "DeleteCertificateResponseTypeDef",
-    "DescribeCertificatesResponseTypeDef",
-    "ImportCertificateResponseTypeDef",
-    "CollectorResponseTypeDef",
+    "SubnetOutputTypeDef",
+    "BatchStartRecommendationsResponseOutputTypeDef",
+    "DeleteCertificateResponseOutputTypeDef",
+    "DescribeCertificatesResponseOutputTypeDef",
+    "ImportCertificateResponseOutputTypeDef",
+    "CollectorResponseOutputTypeDef",
+    "ReplicationConfigOutputTypeDef",
     "CreateReplicationConfigMessageRequestTypeDef",
     "ModifyReplicationConfigMessageRequestTypeDef",
-    "ReplicationConfigTypeDef",
-    "DeleteConnectionResponseTypeDef",
-    "DescribeConnectionsResponseTypeDef",
-    "TestConnectionResponseTypeDef",
+    "DeleteConnectionResponseOutputTypeDef",
+    "DescribeConnectionsResponseOutputTypeDef",
+    "TestConnectionResponseOutputTypeDef",
     "CreateEndpointMessageRequestTypeDef",
-    "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
-    "CreateEventSubscriptionResponseTypeDef",
-    "DeleteEventSubscriptionResponseTypeDef",
-    "DescribeEventSubscriptionsResponseTypeDef",
-    "ModifyEventSubscriptionResponseTypeDef",
-    "DatabaseResponseTypeDef",
+    "CreateEventSubscriptionResponseOutputTypeDef",
+    "DeleteEventSubscriptionResponseOutputTypeDef",
+    "DescribeEventSubscriptionsResponseOutputTypeDef",
+    "ModifyEventSubscriptionResponseOutputTypeDef",
+    "DatabaseResponseOutputTypeDef",
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
     "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
     "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
     "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
@@ -242,85 +263,87 @@
     "DescribeEndpointsMessageEndpointDeletedWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef",
-    "DescribeEndpointSettingsResponseTypeDef",
-    "DescribeEndpointTypesResponseTypeDef",
-    "DescribeEventCategoriesResponseTypeDef",
-    "DescribeEventsResponseTypeDef",
-    "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
-    "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
-    "DescribeOrderableReplicationInstancesResponseTypeDef",
-    "DescribeRecommendationLimitationsResponseTypeDef",
-    "DescribeRefreshSchemasStatusResponseTypeDef",
-    "RefreshSchemasResponseTypeDef",
-    "DescribeReplicationInstanceTaskLogsResponseTypeDef",
-    "DescribeReplicationTableStatisticsResponseTypeDef",
-    "DescribeTableStatisticsResponseTypeDef",
-    "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
-    "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
-    "ResourcePendingMaintenanceActionsTypeDef",
-    "RdsRecommendationTypeDef",
+    "DescribeEndpointSettingsResponseOutputTypeDef",
+    "DescribeEndpointTypesResponseOutputTypeDef",
+    "DescribeEventCategoriesResponseOutputTypeDef",
+    "DescribeEventsResponseOutputTypeDef",
+    "DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef",
+    "DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef",
+    "DescribeOrderableReplicationInstancesResponseOutputTypeDef",
+    "DescribeRecommendationLimitationsResponseOutputTypeDef",
+    "DescribeRefreshSchemasStatusResponseOutputTypeDef",
+    "RefreshSchemasResponseOutputTypeDef",
+    "DescribeReplicationInstanceTaskLogsResponseOutputTypeDef",
+    "DescribeReplicationTableStatisticsResponseOutputTypeDef",
+    "DescribeTableStatisticsResponseOutputTypeDef",
+    "DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef",
+    "DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef",
+    "EndpointOutputTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
+    "ResourcePendingMaintenanceActionsOutputTypeDef",
+    "RdsRecommendationOutputTypeDef",
     "StartRecommendationsRequestEntryTypeDef",
     "StartRecommendationsRequestRequestTypeDef",
     "ReloadReplicationTablesMessageRequestTypeDef",
     "ReloadTablesMessageRequestTypeDef",
-    "ReplicationTypeDef",
-    "ReplicationTaskAssessmentRunTypeDef",
-    "ReplicationTaskTypeDef",
-    "SchemaResponseTypeDef",
-    "ReplicationSubnetGroupTypeDef",
-    "DescribeFleetAdvisorCollectorsResponseTypeDef",
-    "CreateReplicationConfigResponseTypeDef",
-    "DeleteReplicationConfigResponseTypeDef",
-    "DescribeReplicationConfigsResponseTypeDef",
-    "ModifyReplicationConfigResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
-    "DeleteEndpointResponseTypeDef",
-    "DescribeEndpointsResponseTypeDef",
-    "ModifyEndpointResponseTypeDef",
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
-    "ApplyPendingMaintenanceActionResponseTypeDef",
-    "DescribePendingMaintenanceActionsResponseTypeDef",
-    "RecommendationDataTypeDef",
+    "ReplicationOutputTypeDef",
+    "ReplicationTaskAssessmentRunOutputTypeDef",
+    "ReplicationTaskOutputTypeDef",
+    "SchemaResponseOutputTypeDef",
+    "ReplicationSubnetGroupOutputTypeDef",
+    "DescribeFleetAdvisorCollectorsResponseOutputTypeDef",
+    "CreateReplicationConfigResponseOutputTypeDef",
+    "DeleteReplicationConfigResponseOutputTypeDef",
+    "DescribeReplicationConfigsResponseOutputTypeDef",
+    "ModifyReplicationConfigResponseOutputTypeDef",
+    "DescribeFleetAdvisorDatabasesResponseOutputTypeDef",
+    "CreateEndpointResponseOutputTypeDef",
+    "DeleteEndpointResponseOutputTypeDef",
+    "DescribeEndpointsResponseOutputTypeDef",
+    "ModifyEndpointResponseOutputTypeDef",
+    "ApplyPendingMaintenanceActionResponseOutputTypeDef",
+    "DescribePendingMaintenanceActionsResponseOutputTypeDef",
+    "RecommendationDataOutputTypeDef",
     "BatchStartRecommendationsRequestRequestTypeDef",
-    "DescribeReplicationsResponseTypeDef",
-    "StartReplicationResponseTypeDef",
-    "StopReplicationResponseTypeDef",
-    "CancelReplicationTaskAssessmentRunResponseTypeDef",
-    "DeleteReplicationTaskAssessmentRunResponseTypeDef",
-    "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
-    "StartReplicationTaskAssessmentRunResponseTypeDef",
-    "CreateReplicationTaskResponseTypeDef",
-    "DeleteReplicationTaskResponseTypeDef",
-    "DescribeReplicationTasksResponseTypeDef",
-    "ModifyReplicationTaskResponseTypeDef",
-    "MoveReplicationTaskResponseTypeDef",
-    "StartReplicationTaskAssessmentResponseTypeDef",
-    "StartReplicationTaskResponseTypeDef",
-    "StopReplicationTaskResponseTypeDef",
-    "DescribeFleetAdvisorSchemasResponseTypeDef",
-    "CreateReplicationSubnetGroupResponseTypeDef",
-    "DescribeReplicationSubnetGroupsResponseTypeDef",
-    "ModifyReplicationSubnetGroupResponseTypeDef",
-    "ReplicationInstanceTypeDef",
-    "RecommendationTypeDef",
-    "CreateReplicationInstanceResponseTypeDef",
-    "DeleteReplicationInstanceResponseTypeDef",
-    "DescribeReplicationInstancesResponseTypeDef",
-    "ModifyReplicationInstanceResponseTypeDef",
-    "RebootReplicationInstanceResponseTypeDef",
-    "DescribeRecommendationsResponseTypeDef",
+    "DescribeReplicationsResponseOutputTypeDef",
+    "StartReplicationResponseOutputTypeDef",
+    "StopReplicationResponseOutputTypeDef",
+    "CancelReplicationTaskAssessmentRunResponseOutputTypeDef",
+    "DeleteReplicationTaskAssessmentRunResponseOutputTypeDef",
+    "DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef",
+    "StartReplicationTaskAssessmentRunResponseOutputTypeDef",
+    "CreateReplicationTaskResponseOutputTypeDef",
+    "DeleteReplicationTaskResponseOutputTypeDef",
+    "DescribeReplicationTasksResponseOutputTypeDef",
+    "ModifyReplicationTaskResponseOutputTypeDef",
+    "MoveReplicationTaskResponseOutputTypeDef",
+    "StartReplicationTaskAssessmentResponseOutputTypeDef",
+    "StartReplicationTaskResponseOutputTypeDef",
+    "StopReplicationTaskResponseOutputTypeDef",
+    "DescribeFleetAdvisorSchemasResponseOutputTypeDef",
+    "CreateReplicationSubnetGroupResponseOutputTypeDef",
+    "DescribeReplicationSubnetGroupsResponseOutputTypeDef",
+    "ModifyReplicationSubnetGroupResponseOutputTypeDef",
+    "ReplicationInstanceOutputTypeDef",
+    "RecommendationOutputTypeDef",
+    "CreateReplicationInstanceResponseOutputTypeDef",
+    "DeleteReplicationInstanceResponseOutputTypeDef",
+    "DescribeReplicationInstancesResponseOutputTypeDef",
+    "ModifyReplicationInstanceResponseOutputTypeDef",
+    "RebootReplicationInstanceResponseOutputTypeDef",
+    "DescribeRecommendationsResponseOutputTypeDef",
 )
 
-AccountQuotaTypeDef = TypedDict(
-    "AccountQuotaTypeDef",
+AccountQuotaOutputTypeDef = TypedDict(
+    "AccountQuotaOutputTypeDef",
     {
         "AccountQuotaName": str,
         "Used": int,
         "Max": int,
     },
 )
 
@@ -339,79 +362,94 @@
     {
         "ReplicationInstanceArn": str,
         "ApplyAction": str,
         "OptInType": str,
     },
 )
 
-AvailabilityZoneTypeDef = TypedDict(
-    "AvailabilityZoneTypeDef",
+AvailabilityZoneOutputTypeDef = TypedDict(
+    "AvailabilityZoneOutputTypeDef",
     {
         "Name": str,
     },
 )
 
-BatchStartRecommendationsErrorEntryTypeDef = TypedDict(
-    "BatchStartRecommendationsErrorEntryTypeDef",
+BatchStartRecommendationsErrorEntryOutputTypeDef = TypedDict(
+    "BatchStartRecommendationsErrorEntryOutputTypeDef",
     {
         "DatabaseId": str,
         "Message": str,
         "Code": str,
     },
 )
 
 CancelReplicationTaskAssessmentRunMessageRequestTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
     },
 )
 
-CertificateTypeDef = TypedDict(
-    "CertificateTypeDef",
+CertificateOutputTypeDef = TypedDict(
+    "CertificateOutputTypeDef",
     {
         "CertificateIdentifier": str,
         "CertificateCreationDate": datetime,
         "CertificatePem": str,
         "CertificateWallet": bytes,
         "CertificateArn": str,
         "CertificateOwner": str,
         "ValidFromDate": datetime,
         "ValidToDate": datetime,
         "SigningAlgorithm": str,
         "KeyLength": int,
     },
 )
 
-CollectorHealthCheckTypeDef = TypedDict(
-    "CollectorHealthCheckTypeDef",
+CollectorHealthCheckOutputTypeDef = TypedDict(
+    "CollectorHealthCheckOutputTypeDef",
     {
         "CollectorStatus": CollectorStatusType,
         "LocalCollectorS3Access": bool,
         "WebCollectorS3Access": bool,
         "WebCollectorGrantedRoleBasedAccess": bool,
     },
 )
 
-InventoryDataTypeDef = TypedDict(
-    "InventoryDataTypeDef",
+InventoryDataOutputTypeDef = TypedDict(
+    "InventoryDataOutputTypeDef",
     {
         "NumberOfDatabases": int,
         "NumberOfSchemas": int,
     },
 )
 
-CollectorShortInfoResponseTypeDef = TypedDict(
-    "CollectorShortInfoResponseTypeDef",
+CollectorShortInfoResponseOutputTypeDef = TypedDict(
+    "CollectorShortInfoResponseOutputTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
     },
 )
 
+ComputeConfigOutputTypeDef = TypedDict(
+    "ComputeConfigOutputTypeDef",
+    {
+        "AvailabilityZone": str,
+        "DnsNameServers": str,
+        "KmsKeyId": str,
+        "MaxCapacityUnits": int,
+        "MinCapacityUnits": int,
+        "MultiAZ": bool,
+        "PreferredMaintenanceWindow": str,
+        "ReplicationSubnetGroupId": str,
+        "VpcSecurityGroupIds": List[str],
+    },
+)
+
 ComputeConfigTypeDef = TypedDict(
     "ComputeConfigTypeDef",
     {
         "AvailabilityZone": str,
         "DnsNameServers": str,
         "KmsKeyId": str,
         "MaxCapacityUnits": int,
@@ -420,16 +458,16 @@
         "PreferredMaintenanceWindow": str,
         "ReplicationSubnetGroupId": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-ConnectionTypeDef = TypedDict(
-    "ConnectionTypeDef",
+ConnectionOutputTypeDef = TypedDict(
+    "ConnectionOutputTypeDef",
     {
         "ReplicationInstanceArn": str,
         "EndpointArn": str,
         "Status": str,
         "LastFailureMessage": str,
         "EndpointIdentifier": str,
         "ReplicationInstanceIdentifier": str,
@@ -485,19 +523,21 @@
         "FullLoadErrorPercentage": int,
         "ErrorRetryDuration": int,
         "UseNewMappingType": bool,
     },
     total=False,
 )
 
+
 class ElasticsearchSettingsTypeDef(
     _RequiredElasticsearchSettingsTypeDef, _OptionalElasticsearchSettingsTypeDef
 ):
     pass
 
+
 GcpMySQLSettingsTypeDef = TypedDict(
     "GcpMySQLSettingsTypeDef",
     {
         "AfterConnectScript": str,
         "CleanSourceMetadataOnMismatch": bool,
         "DatabaseName": str,
         "EventsPollInterval": int,
@@ -659,17 +699,19 @@
         "MaxFileSize": int,
         "MaxRetryCount": int,
         "IamAuthEnabled": bool,
     },
     total=False,
 )
 
+
 class NeptuneSettingsTypeDef(_RequiredNeptuneSettingsTypeDef, _OptionalNeptuneSettingsTypeDef):
     pass
 
+
 OracleSettingsTypeDef = TypedDict(
     "OracleSettingsTypeDef",
     {
         "AddSupplementalLogging": bool,
         "ArchivedLogDestId": int,
         "AdditionalArchivedLogDestId": int,
         "ExtraArchivedLogDestIds": Sequence[int],
@@ -762,17 +804,19 @@
         "AuthUserName": str,
         "AuthPassword": str,
         "SslCaCertificateArn": str,
     },
     total=False,
 )
 
+
 class RedisSettingsTypeDef(_RequiredRedisSettingsTypeDef, _OptionalRedisSettingsTypeDef):
     pass
 
+
 RedshiftSettingsTypeDef = TypedDict(
     "RedshiftSettingsTypeDef",
     {
         "AcceptAnyDate": bool,
         "AfterConnectScript": str,
         "BucketFolder": str,
         "BucketName": str,
@@ -882,21 +926,23 @@
     {
         "CdcInsertsAndUpdates": bool,
         "EnableMagneticStoreWrites": bool,
     },
     total=False,
 )
 
+
 class TimestreamSettingsTypeDef(
     _RequiredTimestreamSettingsTypeDef, _OptionalTimestreamSettingsTypeDef
 ):
     pass
 
-EventSubscriptionTypeDef = TypedDict(
-    "EventSubscriptionTypeDef",
+
+EventSubscriptionOutputTypeDef = TypedDict(
+    "EventSubscriptionOutputTypeDef",
     {
         "CustomerAwsId": str,
         "CustSubscriptionId": str,
         "SnsTopicArn": str,
         "Status": str,
         "SubscriptionCreationTime": str,
         "SourceType": str,
@@ -918,56 +964,58 @@
     "_OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateFleetAdvisorCollectorRequestRequestTypeDef(
     _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef,
     _OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef,
 ):
     pass
 
-CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
-    "CreateFleetAdvisorCollectorResponseTypeDef",
+
+CreateFleetAdvisorCollectorResponseOutputTypeDef = TypedDict(
+    "CreateFleetAdvisorCollectorResponseOutputTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
         "Description": str,
         "ServiceAccessRoleArn": str,
         "S3BucketName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatabaseInstanceSoftwareDetailsResponseTypeDef = TypedDict(
-    "DatabaseInstanceSoftwareDetailsResponseTypeDef",
+DatabaseInstanceSoftwareDetailsResponseOutputTypeDef = TypedDict(
+    "DatabaseInstanceSoftwareDetailsResponseOutputTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "EngineEdition": str,
         "ServicePack": str,
         "SupportLevel": str,
         "OsArchitecture": int,
         "Tooltip": str,
     },
 )
 
-ServerShortInfoResponseTypeDef = TypedDict(
-    "ServerShortInfoResponseTypeDef",
+ServerShortInfoResponseOutputTypeDef = TypedDict(
+    "ServerShortInfoResponseOutputTypeDef",
     {
         "ServerId": str,
         "IpAddress": str,
         "ServerName": str,
     },
 )
 
-DatabaseShortInfoResponseTypeDef = TypedDict(
-    "DatabaseShortInfoResponseTypeDef",
+DatabaseShortInfoResponseOutputTypeDef = TypedDict(
+    "DatabaseShortInfoResponseOutputTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
         "DatabaseEngine": str,
     },
 )
@@ -1011,16 +1059,16 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
-DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
+DeleteFleetAdvisorDatabasesResponseOutputTypeDef = TypedDict(
+    "DeleteFleetAdvisorDatabasesResponseOutputTypeDef",
     {
         "DatabaseIds": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationConfigMessageRequestTypeDef = TypedDict(
@@ -1068,16 +1116,16 @@
         "MigrationType": MigrationTypeValueType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
+DescribeApplicableIndividualAssessmentsResponseOutputTypeDef = TypedDict(
+    "DescribeApplicableIndividualAssessmentsResponseOutputTypeDef",
     {
         "IndividualAssessmentNames": List[str],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1109,56 +1157,58 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeEndpointSettingsMessageRequestTypeDef(
     _RequiredDescribeEndpointSettingsMessageRequestTypeDef,
     _OptionalDescribeEndpointSettingsMessageRequestTypeDef,
 ):
     pass
 
-EndpointSettingTypeDef = TypedDict(
-    "EndpointSettingTypeDef",
+
+EndpointSettingOutputTypeDef = TypedDict(
+    "EndpointSettingOutputTypeDef",
     {
         "Name": str,
         "Type": EndpointSettingTypeValueType,
         "EnumValues": List[str],
         "Sensitive": bool,
         "Units": str,
         "Applicability": str,
         "IntValueMin": int,
         "IntValueMax": int,
         "DefaultValue": str,
     },
 )
 
-SupportedEndpointTypeTypeDef = TypedDict(
-    "SupportedEndpointTypeTypeDef",
+SupportedEndpointTypeOutputTypeDef = TypedDict(
+    "SupportedEndpointTypeOutputTypeDef",
     {
         "EngineName": str,
         "SupportsCDC": bool,
         "EndpointType": ReplicationEndpointTypeValueType,
         "ReplicationInstanceEngineMinimumVersion": str,
         "EngineDisplayName": str,
     },
 )
 
-EventCategoryGroupTypeDef = TypedDict(
-    "EventCategoryGroupTypeDef",
+EventCategoryGroupOutputTypeDef = TypedDict(
+    "EventCategoryGroupOutputTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
 )
 
-EventTypeDef = TypedDict(
-    "EventTypeDef",
+EventOutputTypeDef = TypedDict(
+    "EventOutputTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
     },
@@ -1169,24 +1219,24 @@
     {
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-FleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "FleetAdvisorLsaAnalysisResponseTypeDef",
+FleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
+    "FleetAdvisorLsaAnalysisResponseOutputTypeDef",
     {
         "LsaAnalysisId": str,
         "Status": str,
     },
 )
 
-FleetAdvisorSchemaObjectResponseTypeDef = TypedDict(
-    "FleetAdvisorSchemaObjectResponseTypeDef",
+FleetAdvisorSchemaObjectResponseOutputTypeDef = TypedDict(
+    "FleetAdvisorSchemaObjectResponseOutputTypeDef",
     {
         "SchemaId": str,
         "ObjectType": str,
         "NumberOfObjects": int,
         "CodeLineCount": int,
         "CodeSize": int,
     },
@@ -1205,31 +1255,31 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-OrderableReplicationInstanceTypeDef = TypedDict(
-    "OrderableReplicationInstanceTypeDef",
+OrderableReplicationInstanceOutputTypeDef = TypedDict(
+    "OrderableReplicationInstanceOutputTypeDef",
     {
         "EngineVersion": str,
         "ReplicationInstanceClass": str,
         "StorageType": str,
         "MinAllocatedStorage": int,
         "MaxAllocatedStorage": int,
         "DefaultAllocatedStorage": int,
         "IncludedAllocatedStorage": int,
         "AvailabilityZones": List[str],
         "ReleaseStatus": ReleaseStatusValuesType,
     },
 )
 
-LimitationTypeDef = TypedDict(
-    "LimitationTypeDef",
+LimitationOutputTypeDef = TypedDict(
+    "LimitationOutputTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "Name": str,
         "Description": str,
         "Impact": str,
         "Type": str,
@@ -1239,16 +1289,16 @@
 DescribeRefreshSchemasStatusMessageRequestTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
-RefreshSchemasStatusTypeDef = TypedDict(
-    "RefreshSchemasStatusTypeDef",
+RefreshSchemasStatusOutputTypeDef = TypedDict(
+    "RefreshSchemasStatusOutputTypeDef",
     {
         "EndpointArn": str,
         "ReplicationInstanceArn": str,
         "Status": RefreshSchemasStatusTypeValueType,
         "LastRefreshDate": datetime,
         "LastFailureMessage": str,
     },
@@ -1265,31 +1315,33 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeReplicationInstanceTaskLogsMessageRequestTypeDef(
     _RequiredDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     _OptionalDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
 ):
     pass
 
-ReplicationInstanceTaskLogTypeDef = TypedDict(
-    "ReplicationInstanceTaskLogTypeDef",
+
+ReplicationInstanceTaskLogOutputTypeDef = TypedDict(
+    "ReplicationInstanceTaskLogOutputTypeDef",
     {
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
 )
 
-TableStatisticsTypeDef = TypedDict(
-    "TableStatisticsTypeDef",
+TableStatisticsOutputTypeDef = TypedDict(
+    "TableStatisticsOutputTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
         "Inserts": int,
         "Deletes": int,
         "Updates": int,
         "Ddls": int,
@@ -1328,29 +1380,29 @@
         "ReplicationTaskArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-ReplicationTaskAssessmentResultTypeDef = TypedDict(
-    "ReplicationTaskAssessmentResultTypeDef",
+ReplicationTaskAssessmentResultOutputTypeDef = TypedDict(
+    "ReplicationTaskAssessmentResultOutputTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "ReplicationTaskArn": str,
         "ReplicationTaskLastAssessmentDate": datetime,
         "AssessmentStatus": str,
         "AssessmentResultsFile": str,
         "AssessmentResults": str,
         "S3ObjectUrl": str,
     },
 )
 
-ReplicationTaskIndividualAssessmentTypeDef = TypedDict(
-    "ReplicationTaskIndividualAssessmentTypeDef",
+ReplicationTaskIndividualAssessmentOutputTypeDef = TypedDict(
+    "ReplicationTaskIndividualAssessmentOutputTypeDef",
     {
         "ReplicationTaskIndividualAssessmentArn": str,
         "ReplicationTaskAssessmentRunArn": str,
         "IndividualAssessmentName": str,
         "Status": str,
         "ReplicationTaskIndividualAssessmentStartDate": datetime,
     },
@@ -1366,20 +1418,22 @@
     "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
     _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeSchemasMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemasMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalDescribeSchemasMessageRequestTypeDef = TypedDict(
@@ -1387,44 +1441,456 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
-DescribeSchemasResponseTypeDef = TypedDict(
-    "DescribeSchemasResponseTypeDef",
+
+DescribeSchemasResponseOutputTypeDef = TypedDict(
+    "DescribeSchemasResponseOutputTypeDef",
     {
         "Marker": str,
         "Schemas": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DmsTransferSettingsOutputTypeDef = TypedDict(
+    "DmsTransferSettingsOutputTypeDef",
+    {
+        "ServiceAccessRoleArn": str,
+        "BucketName": str,
+    },
+)
+
+DocDbSettingsOutputTypeDef = TypedDict(
+    "DocDbSettingsOutputTypeDef",
+    {
+        "Username": str,
+        "Password": str,
+        "ServerName": str,
+        "Port": int,
+        "DatabaseName": str,
+        "NestingLevel": NestingLevelValueType,
+        "ExtractDocId": bool,
+        "DocsToInvestigate": int,
+        "KmsKeyId": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "UseUpdateLookUp": bool,
+        "ReplicateShardCollections": bool,
+    },
+)
+
+DynamoDbSettingsOutputTypeDef = TypedDict(
+    "DynamoDbSettingsOutputTypeDef",
+    {
+        "ServiceAccessRoleArn": str,
+    },
+)
+
+ElasticsearchSettingsOutputTypeDef = TypedDict(
+    "ElasticsearchSettingsOutputTypeDef",
+    {
+        "ServiceAccessRoleArn": str,
+        "EndpointUri": str,
+        "FullLoadErrorPercentage": int,
+        "ErrorRetryDuration": int,
+        "UseNewMappingType": bool,
+    },
+)
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GcpMySQLSettingsOutputTypeDef = TypedDict(
+    "GcpMySQLSettingsOutputTypeDef",
+    {
+        "AfterConnectScript": str,
+        "CleanSourceMetadataOnMismatch": bool,
+        "DatabaseName": str,
+        "EventsPollInterval": int,
+        "TargetDbType": TargetDbTypeType,
+        "MaxFileSize": int,
+        "ParallelLoadThreads": int,
+        "Password": str,
+        "Port": int,
+        "ServerName": str,
+        "ServerTimezone": str,
+        "Username": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+    },
+)
+
+IBMDb2SettingsOutputTypeDef = TypedDict(
+    "IBMDb2SettingsOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "Password": str,
+        "Port": int,
+        "ServerName": str,
+        "SetDataCaptureChanges": bool,
+        "CurrentLsn": str,
+        "MaxKBytesPerRead": int,
+        "Username": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+    },
+)
+
+KafkaSettingsOutputTypeDef = TypedDict(
+    "KafkaSettingsOutputTypeDef",
+    {
+        "Broker": str,
+        "Topic": str,
+        "MessageFormat": MessageFormatValueType,
+        "IncludeTransactionDetails": bool,
+        "IncludePartitionValue": bool,
+        "PartitionIncludeSchemaTable": bool,
+        "IncludeTableAlterOperations": bool,
+        "IncludeControlDetails": bool,
+        "MessageMaxBytes": int,
+        "IncludeNullAndEmpty": bool,
+        "SecurityProtocol": KafkaSecurityProtocolType,
+        "SslClientCertificateArn": str,
+        "SslClientKeyArn": str,
+        "SslClientKeyPassword": str,
+        "SslCaCertificateArn": str,
+        "SaslUsername": str,
+        "SaslPassword": str,
+        "NoHexPrefix": bool,
+        "SaslMechanism": KafkaSaslMechanismType,
+        "SslEndpointIdentificationAlgorithm": KafkaSslEndpointIdentificationAlgorithmType,
+    },
+)
+
+KinesisSettingsOutputTypeDef = TypedDict(
+    "KinesisSettingsOutputTypeDef",
+    {
+        "StreamArn": str,
+        "MessageFormat": MessageFormatValueType,
+        "ServiceAccessRoleArn": str,
+        "IncludeTransactionDetails": bool,
+        "IncludePartitionValue": bool,
+        "PartitionIncludeSchemaTable": bool,
+        "IncludeTableAlterOperations": bool,
+        "IncludeControlDetails": bool,
+        "IncludeNullAndEmpty": bool,
+        "NoHexPrefix": bool,
+    },
+)
+
+MicrosoftSQLServerSettingsOutputTypeDef = TypedDict(
+    "MicrosoftSQLServerSettingsOutputTypeDef",
+    {
+        "Port": int,
+        "BcpPacketSize": int,
+        "DatabaseName": str,
+        "ControlTablesFileGroup": str,
+        "Password": str,
+        "QuerySingleAlwaysOnNode": bool,
+        "ReadBackupOnly": bool,
+        "SafeguardPolicy": SafeguardPolicyType,
+        "ServerName": str,
+        "Username": str,
+        "UseBcpFullLoad": bool,
+        "UseThirdPartyBackupDevice": bool,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "TrimSpaceInChar": bool,
+        "TlogAccessMode": TlogAccessModeType,
+        "ForceLobLookup": bool,
+    },
+)
+
+MongoDbSettingsOutputTypeDef = TypedDict(
+    "MongoDbSettingsOutputTypeDef",
+    {
+        "Username": str,
+        "Password": str,
+        "ServerName": str,
+        "Port": int,
+        "DatabaseName": str,
+        "AuthType": AuthTypeValueType,
+        "AuthMechanism": AuthMechanismValueType,
+        "NestingLevel": NestingLevelValueType,
+        "ExtractDocId": str,
+        "DocsToInvestigate": str,
+        "AuthSource": str,
+        "KmsKeyId": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "UseUpdateLookUp": bool,
+        "ReplicateShardCollections": bool,
+    },
+)
+
+MySQLSettingsOutputTypeDef = TypedDict(
+    "MySQLSettingsOutputTypeDef",
+    {
+        "AfterConnectScript": str,
+        "CleanSourceMetadataOnMismatch": bool,
+        "DatabaseName": str,
+        "EventsPollInterval": int,
+        "TargetDbType": TargetDbTypeType,
+        "MaxFileSize": int,
+        "ParallelLoadThreads": int,
+        "Password": str,
+        "Port": int,
+        "ServerName": str,
+        "ServerTimezone": str,
+        "Username": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+    },
+)
+
+NeptuneSettingsOutputTypeDef = TypedDict(
+    "NeptuneSettingsOutputTypeDef",
+    {
+        "ServiceAccessRoleArn": str,
+        "S3BucketName": str,
+        "S3BucketFolder": str,
+        "ErrorRetryDuration": int,
+        "MaxFileSize": int,
+        "MaxRetryCount": int,
+        "IamAuthEnabled": bool,
+    },
+)
+
+OracleSettingsOutputTypeDef = TypedDict(
+    "OracleSettingsOutputTypeDef",
+    {
+        "AddSupplementalLogging": bool,
+        "ArchivedLogDestId": int,
+        "AdditionalArchivedLogDestId": int,
+        "ExtraArchivedLogDestIds": List[int],
+        "AllowSelectNestedTables": bool,
+        "ParallelAsmReadThreads": int,
+        "ReadAheadBlocks": int,
+        "AccessAlternateDirectly": bool,
+        "UseAlternateFolderForOnline": bool,
+        "OraclePathPrefix": str,
+        "UsePathPrefix": str,
+        "ReplacePathPrefix": bool,
+        "EnableHomogenousTablespace": bool,
+        "DirectPathNoLog": bool,
+        "ArchivedLogsOnly": bool,
+        "AsmPassword": str,
+        "AsmServer": str,
+        "AsmUser": str,
+        "CharLengthSemantics": CharLengthSemanticsType,
+        "DatabaseName": str,
+        "DirectPathParallelLoad": bool,
+        "FailTasksOnLobTruncation": bool,
+        "NumberDatatypeScale": int,
+        "Password": str,
+        "Port": int,
+        "ReadTableSpaceName": bool,
+        "RetryInterval": int,
+        "SecurityDbEncryption": str,
+        "SecurityDbEncryptionName": str,
+        "ServerName": str,
+        "SpatialDataOptionToGeoJsonFunctionName": str,
+        "StandbyDelayTime": int,
+        "Username": str,
+        "UseBFile": bool,
+        "UseDirectPathFullLoad": bool,
+        "UseLogminerReader": bool,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "SecretsManagerOracleAsmAccessRoleArn": str,
+        "SecretsManagerOracleAsmSecretId": str,
+        "TrimSpaceInChar": bool,
+        "ConvertTimestampWithZoneToUTC": bool,
+        "OpenTransactionWindow": int,
+    },
+)
+
+PostgreSQLSettingsOutputTypeDef = TypedDict(
+    "PostgreSQLSettingsOutputTypeDef",
+    {
+        "AfterConnectScript": str,
+        "CaptureDdls": bool,
+        "MaxFileSize": int,
+        "DatabaseName": str,
+        "DdlArtifactsSchema": str,
+        "ExecuteTimeout": int,
+        "FailTasksOnLobTruncation": bool,
+        "HeartbeatEnable": bool,
+        "HeartbeatSchema": str,
+        "HeartbeatFrequency": int,
+        "Password": str,
+        "Port": int,
+        "ServerName": str,
+        "Username": str,
+        "SlotName": str,
+        "PluginName": PluginNameValueType,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "TrimSpaceInChar": bool,
+        "MapBooleanAsBoolean": bool,
+        "MapJsonbAsClob": bool,
+        "MapLongVarcharAs": LongVarcharMappingTypeType,
+        "DatabaseMode": DatabaseModeType,
+        "BabelfishDatabaseName": str,
+    },
+)
+
+RedisSettingsOutputTypeDef = TypedDict(
+    "RedisSettingsOutputTypeDef",
+    {
+        "ServerName": str,
+        "Port": int,
+        "SslSecurityProtocol": SslSecurityProtocolValueType,
+        "AuthType": RedisAuthTypeValueType,
+        "AuthUserName": str,
+        "AuthPassword": str,
+        "SslCaCertificateArn": str,
+    },
+)
+
+RedshiftSettingsOutputTypeDef = TypedDict(
+    "RedshiftSettingsOutputTypeDef",
+    {
+        "AcceptAnyDate": bool,
+        "AfterConnectScript": str,
+        "BucketFolder": str,
+        "BucketName": str,
+        "CaseSensitiveNames": bool,
+        "CompUpdate": bool,
+        "ConnectionTimeout": int,
+        "DatabaseName": str,
+        "DateFormat": str,
+        "EmptyAsNull": bool,
+        "EncryptionMode": EncryptionModeValueType,
+        "ExplicitIds": bool,
+        "FileTransferUploadStreams": int,
+        "LoadTimeout": int,
+        "MaxFileSize": int,
+        "Password": str,
+        "Port": int,
+        "RemoveQuotes": bool,
+        "ReplaceInvalidChars": str,
+        "ReplaceChars": str,
+        "ServerName": str,
+        "ServiceAccessRoleArn": str,
+        "ServerSideEncryptionKmsKeyId": str,
+        "TimeFormat": str,
+        "TrimBlanks": bool,
+        "TruncateColumns": bool,
+        "Username": str,
+        "WriteBufferSize": int,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "MapBooleanAsBoolean": bool,
+    },
+)
+
+S3SettingsOutputTypeDef = TypedDict(
+    "S3SettingsOutputTypeDef",
+    {
+        "ServiceAccessRoleArn": str,
+        "ExternalTableDefinition": str,
+        "CsvRowDelimiter": str,
+        "CsvDelimiter": str,
+        "BucketFolder": str,
+        "BucketName": str,
+        "CompressionType": CompressionTypeValueType,
+        "EncryptionMode": EncryptionModeValueType,
+        "ServerSideEncryptionKmsKeyId": str,
+        "DataFormat": DataFormatValueType,
+        "EncodingType": EncodingTypeValueType,
+        "DictPageSizeLimit": int,
+        "RowGroupLength": int,
+        "DataPageSize": int,
+        "ParquetVersion": ParquetVersionValueType,
+        "EnableStatistics": bool,
+        "IncludeOpForFullLoad": bool,
+        "CdcInsertsOnly": bool,
+        "TimestampColumnName": str,
+        "ParquetTimestampInMillisecond": bool,
+        "CdcInsertsAndUpdates": bool,
+        "DatePartitionEnabled": bool,
+        "DatePartitionSequence": DatePartitionSequenceValueType,
+        "DatePartitionDelimiter": DatePartitionDelimiterValueType,
+        "UseCsvNoSupValue": bool,
+        "CsvNoSupValue": str,
+        "PreserveTransactions": bool,
+        "CdcPath": str,
+        "UseTaskStartTimeForFullLoadTimestamp": bool,
+        "CannedAclForObjects": CannedAclForObjectsValueType,
+        "AddColumnName": bool,
+        "CdcMaxBatchInterval": int,
+        "CdcMinFileSize": int,
+        "CsvNullValue": str,
+        "IgnoreHeaderRows": int,
+        "MaxFileSize": int,
+        "Rfc4180": bool,
+        "DatePartitionTimezone": str,
+        "AddTrailingPaddingCharacter": bool,
+        "ExpectedBucketOwner": str,
+        "GlueCatalogGeneration": bool,
+    },
+)
+
+SybaseSettingsOutputTypeDef = TypedDict(
+    "SybaseSettingsOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "Password": str,
+        "Port": int,
+        "ServerName": str,
+        "Username": str,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+    },
+)
+
+TimestreamSettingsOutputTypeDef = TypedDict(
+    "TimestreamSettingsOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "MemoryDuration": int,
+        "MagneticDuration": int,
+        "CdcInsertsAndUpdates": bool,
+        "EnableMagneticStoreWrites": bool,
+    },
+)
+
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
     },
 )
 _OptionalModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
@@ -1434,20 +1900,22 @@
         "SourceType": str,
         "EventCategories": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class ModifyEventSubscriptionMessageRequestTypeDef(
     _RequiredModifyEventSubscriptionMessageRequestTypeDef,
     _OptionalModifyEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
 )
 _OptionalModifyReplicationInstanceMessageRequestTypeDef = TypedDict(
@@ -1464,20 +1932,22 @@
         "AutoMinorVersionUpgrade": bool,
         "ReplicationInstanceIdentifier": str,
         "NetworkType": str,
     },
     total=False,
 )
 
+
 class ModifyReplicationInstanceMessageRequestTypeDef(
     _RequiredModifyReplicationInstanceMessageRequestTypeDef,
     _OptionalModifyReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyReplicationSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -1485,20 +1955,22 @@
     "_OptionalModifyReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupDescription": str,
     },
     total=False,
 )
 
+
 class ModifyReplicationSubnetGroupMessageRequestTypeDef(
     _RequiredModifyReplicationSubnetGroupMessageRequestTypeDef,
     _OptionalModifyReplicationSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyReplicationTaskMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
 _OptionalModifyReplicationTaskMessageRequestTypeDef = TypedDict(
@@ -1512,20 +1984,22 @@
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "TaskData": str,
     },
     total=False,
 )
 
+
 class ModifyReplicationTaskMessageRequestTypeDef(
     _RequiredModifyReplicationTaskMessageRequestTypeDef,
     _OptionalModifyReplicationTaskMessageRequestTypeDef,
 ):
     pass
 
+
 MoveReplicationTaskMessageRequestTypeDef = TypedDict(
     "MoveReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TargetReplicationInstanceArn": str,
     },
 )
@@ -1536,55 +2010,55 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-PendingMaintenanceActionTypeDef = TypedDict(
-    "PendingMaintenanceActionTypeDef",
+PendingMaintenanceActionOutputTypeDef = TypedDict(
+    "PendingMaintenanceActionOutputTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
 )
 
-ProvisionDataTypeDef = TypedDict(
-    "ProvisionDataTypeDef",
+ProvisionDataOutputTypeDef = TypedDict(
+    "ProvisionDataOutputTypeDef",
     {
         "ProvisionState": str,
         "ProvisionedCapacityUnits": int,
         "DateProvisioned": datetime,
         "IsNewProvisioningAvailable": bool,
         "DateNewProvisioningDataAvailable": datetime,
         "ReasonForNewProvisioningData": str,
     },
 )
 
-RdsConfigurationTypeDef = TypedDict(
-    "RdsConfigurationTypeDef",
+RdsConfigurationOutputTypeDef = TypedDict(
+    "RdsConfigurationOutputTypeDef",
     {
         "EngineEdition": str,
         "InstanceType": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageType": str,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
         "EngineVersion": str,
     },
 )
 
-RdsRequirementsTypeDef = TypedDict(
-    "RdsRequirementsTypeDef",
+RdsRequirementsOutputTypeDef = TypedDict(
+    "RdsRequirementsOutputTypeDef",
     {
         "EngineEdition": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
@@ -1603,20 +2077,30 @@
     {
         "ForceFailover": bool,
         "ForcePlannedFailover": bool,
     },
     total=False,
 )
 
+
 class RebootReplicationInstanceMessageRequestTypeDef(
     _RequiredRebootReplicationInstanceMessageRequestTypeDef,
     _OptionalRebootReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
+
+RecommendationSettingsOutputTypeDef = TypedDict(
+    "RecommendationSettingsOutputTypeDef",
+    {
+        "InstanceSizingType": str,
+        "WorkloadType": str,
+    },
+)
+
 RecommendationSettingsTypeDef = TypedDict(
     "RecommendationSettingsTypeDef",
     {
         "InstanceSizingType": str,
         "WorkloadType": str,
     },
 )
@@ -1633,59 +2117,59 @@
     "TableToReloadTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
     },
 )
 
-ReloadReplicationTablesResponseTypeDef = TypedDict(
-    "ReloadReplicationTablesResponseTypeDef",
+ReloadReplicationTablesResponseOutputTypeDef = TypedDict(
+    "ReloadReplicationTablesResponseOutputTypeDef",
     {
         "ReplicationConfigArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReloadTablesResponseTypeDef = TypedDict(
-    "ReloadTablesResponseTypeDef",
+ReloadTablesResponseOutputTypeDef = TypedDict(
+    "ReloadTablesResponseOutputTypeDef",
     {
         "ReplicationTaskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RemoveTagsFromResourceMessageRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ReplicationPendingModifiedValuesTypeDef = TypedDict(
-    "ReplicationPendingModifiedValuesTypeDef",
+ReplicationPendingModifiedValuesOutputTypeDef = TypedDict(
+    "ReplicationPendingModifiedValuesOutputTypeDef",
     {
         "ReplicationInstanceClass": str,
         "AllocatedStorage": int,
         "MultiAZ": bool,
         "EngineVersion": str,
         "NetworkType": str,
     },
 )
 
-VpcSecurityGroupMembershipTypeDef = TypedDict(
-    "VpcSecurityGroupMembershipTypeDef",
+VpcSecurityGroupMembershipOutputTypeDef = TypedDict(
+    "VpcSecurityGroupMembershipOutputTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
 )
 
-ReplicationStatsTypeDef = TypedDict(
-    "ReplicationStatsTypeDef",
+ReplicationStatsOutputTypeDef = TypedDict(
+    "ReplicationStatsOutputTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
         "TablesLoaded": int,
         "TablesLoading": int,
         "TablesQueued": int,
         "TablesErrored": int,
@@ -1693,24 +2177,24 @@
         "StartDate": datetime,
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
     },
 )
 
-ReplicationTaskAssessmentRunProgressTypeDef = TypedDict(
-    "ReplicationTaskAssessmentRunProgressTypeDef",
+ReplicationTaskAssessmentRunProgressOutputTypeDef = TypedDict(
+    "ReplicationTaskAssessmentRunProgressOutputTypeDef",
     {
         "IndividualAssessmentCount": int,
         "IndividualAssessmentCompletedCount": int,
     },
 )
 
-ReplicationTaskStatsTypeDef = TypedDict(
-    "ReplicationTaskStatsTypeDef",
+ReplicationTaskStatsOutputTypeDef = TypedDict(
+    "ReplicationTaskStatsOutputTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
         "TablesLoaded": int,
         "TablesLoading": int,
         "TablesQueued": int,
         "TablesErrored": int,
@@ -1729,25 +2213,25 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+RunFleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
+    "RunFleetAdvisorLsaAnalysisResponseOutputTypeDef",
     {
         "LsaAnalysisId": str,
         "Status": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SchemaShortInfoResponseTypeDef = TypedDict(
-    "SchemaShortInfoResponseTypeDef",
+SchemaShortInfoResponseOutputTypeDef = TypedDict(
+    "SchemaShortInfoResponseOutputTypeDef",
     {
         "SchemaId": str,
         "SchemaName": str,
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
     },
@@ -1766,19 +2250,21 @@
         "CdcStartTime": Union[datetime, str],
         "CdcStartPosition": str,
         "CdcStopPosition": str,
     },
     total=False,
 )
 
+
 class StartReplicationMessageRequestTypeDef(
     _RequiredStartReplicationMessageRequestTypeDef, _OptionalStartReplicationMessageRequestTypeDef
 ):
     pass
 
+
 StartReplicationTaskAssessmentMessageRequestTypeDef = TypedDict(
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
 
@@ -1799,20 +2285,22 @@
         "ResultKmsKeyArn": str,
         "IncludeOnly": Sequence[str],
         "Exclude": Sequence[str],
     },
     total=False,
 )
 
+
 class StartReplicationTaskAssessmentRunMessageRequestTypeDef(
     _RequiredStartReplicationTaskAssessmentRunMessageRequestTypeDef,
     _OptionalStartReplicationTaskAssessmentRunMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartReplicationTaskMessageRequestTypeDef = TypedDict(
     "_RequiredStartReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "StartReplicationTaskType": StartReplicationTaskTypeValueType,
     },
 )
@@ -1822,20 +2310,22 @@
         "CdcStartTime": Union[datetime, str],
         "CdcStartPosition": str,
         "CdcStopPosition": str,
     },
     total=False,
 )
 
+
 class StartReplicationTaskMessageRequestTypeDef(
     _RequiredStartReplicationTaskMessageRequestTypeDef,
     _OptionalStartReplicationTaskMessageRequestTypeDef,
 ):
     pass
 
+
 StopReplicationMessageRequestTypeDef = TypedDict(
     "StopReplicationMessageRequestTypeDef",
     {
         "ReplicationConfigArn": str,
     },
 )
 
@@ -1858,26 +2348,26 @@
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     {
         "ForceMove": bool,
     },
     total=False,
 )
 
-UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+UpdateSubscriptionsToEventBridgeResponseOutputTypeDef = TypedDict(
+    "UpdateSubscriptionsToEventBridgeResponseOutputTypeDef",
     {
         "Result": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
+DescribeAccountAttributesResponseOutputTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseOutputTypeDef",
     {
-        "AccountQuotas": List[AccountQuotaTypeDef],
+        "AccountQuotas": List[AccountQuotaOutputTypeDef],
         "UniqueAccountIdentifier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
@@ -1902,20 +2392,22 @@
         "SourceIds": Sequence[str],
         "Enabled": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
         "ReplicationInstanceClass": str,
     },
 )
@@ -1936,20 +2428,22 @@
         "DnsNameServers": str,
         "ResourceIdentifier": str,
         "NetworkType": str,
     },
     total=False,
 )
 
+
 class CreateReplicationInstanceMessageRequestTypeDef(
     _RequiredCreateReplicationInstanceMessageRequestTypeDef,
     _OptionalCreateReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateReplicationSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "ReplicationSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -1958,20 +2452,22 @@
     "_OptionalCreateReplicationSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateReplicationSubnetGroupMessageRequestTypeDef(
     _RequiredCreateReplicationSubnetGroupMessageRequestTypeDef,
     _OptionalCreateReplicationSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateReplicationTaskMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationInstanceArn": str,
@@ -1989,20 +2485,22 @@
         "Tags": Sequence[TagTypeDef],
         "TaskData": str,
         "ResourceIdentifier": str,
     },
     total=False,
 )
 
+
 class CreateReplicationTaskMessageRequestTypeDef(
     _RequiredCreateReplicationTaskMessageRequestTypeDef,
     _OptionalCreateReplicationTaskMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredImportCertificateMessageRequestTypeDef = TypedDict(
     "_RequiredImportCertificateMessageRequestTypeDef",
     {
         "CertificateIdentifier": str,
     },
 )
 _OptionalImportCertificateMessageRequestTypeDef = TypedDict(
@@ -2011,85 +2509,96 @@
         "CertificatePem": str,
         "CertificateWallet": Union[str, bytes, IO[Any], StreamingBody],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ImportCertificateMessageRequestTypeDef(
     _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-SubnetTypeDef = TypedDict(
-    "SubnetTypeDef",
+SubnetOutputTypeDef = TypedDict(
+    "SubnetOutputTypeDef",
     {
         "SubnetIdentifier": str,
-        "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
+        "SubnetAvailabilityZone": AvailabilityZoneOutputTypeDef,
         "SubnetStatus": str,
     },
 )
 
-BatchStartRecommendationsResponseTypeDef = TypedDict(
-    "BatchStartRecommendationsResponseTypeDef",
+BatchStartRecommendationsResponseOutputTypeDef = TypedDict(
+    "BatchStartRecommendationsResponseOutputTypeDef",
     {
-        "ErrorEntries": List[BatchStartRecommendationsErrorEntryTypeDef],
+        "ErrorEntries": List[BatchStartRecommendationsErrorEntryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteCertificateResponseTypeDef = TypedDict(
-    "DeleteCertificateResponseTypeDef",
+DeleteCertificateResponseOutputTypeDef = TypedDict(
+    "DeleteCertificateResponseOutputTypeDef",
     {
-        "Certificate": CertificateTypeDef,
+        "Certificate": CertificateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeCertificatesResponseTypeDef = TypedDict(
-    "DescribeCertificatesResponseTypeDef",
+DescribeCertificatesResponseOutputTypeDef = TypedDict(
+    "DescribeCertificatesResponseOutputTypeDef",
     {
         "Marker": str,
-        "Certificates": List[CertificateTypeDef],
+        "Certificates": List[CertificateOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ImportCertificateResponseTypeDef = TypedDict(
-    "ImportCertificateResponseTypeDef",
+ImportCertificateResponseOutputTypeDef = TypedDict(
+    "ImportCertificateResponseOutputTypeDef",
     {
-        "Certificate": CertificateTypeDef,
+        "Certificate": CertificateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CollectorResponseTypeDef = TypedDict(
-    "CollectorResponseTypeDef",
+CollectorResponseOutputTypeDef = TypedDict(
+    "CollectorResponseOutputTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
         "CollectorVersion": str,
         "VersionStatus": VersionStatusType,
         "Description": str,
         "S3BucketName": str,
         "ServiceAccessRoleArn": str,
-        "CollectorHealthCheck": CollectorHealthCheckTypeDef,
+        "CollectorHealthCheck": CollectorHealthCheckOutputTypeDef,
         "LastDataReceived": str,
         "RegisteredDate": str,
         "CreatedDate": str,
         "ModifiedDate": str,
-        "InventoryData": InventoryDataTypeDef,
+        "InventoryData": InventoryDataOutputTypeDef,
+    },
+)
+
+ReplicationConfigOutputTypeDef = TypedDict(
+    "ReplicationConfigOutputTypeDef",
+    {
+        "ReplicationConfigIdentifier": str,
+        "ReplicationConfigArn": str,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+        "ReplicationType": MigrationTypeValueType,
+        "ComputeConfig": ComputeConfigOutputTypeDef,
+        "ReplicationSettings": str,
+        "SupplementalSettings": str,
+        "TableMappings": str,
+        "ReplicationConfigCreateTime": datetime,
+        "ReplicationConfigUpdateTime": datetime,
     },
 )
 
 _RequiredCreateReplicationConfigMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationConfigMessageRequestTypeDef",
     {
         "ReplicationConfigIdentifier": str,
@@ -2107,20 +2616,22 @@
         "SupplementalSettings": str,
         "ResourceIdentifier": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateReplicationConfigMessageRequestTypeDef(
     _RequiredCreateReplicationConfigMessageRequestTypeDef,
     _OptionalCreateReplicationConfigMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyReplicationConfigMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationConfigMessageRequestTypeDef",
     {
         "ReplicationConfigArn": str,
     },
 )
 _OptionalModifyReplicationConfigMessageRequestTypeDef = TypedDict(
@@ -2134,58 +2645,43 @@
         "ComputeConfig": ComputeConfigTypeDef,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
     },
     total=False,
 )
 
+
 class ModifyReplicationConfigMessageRequestTypeDef(
     _RequiredModifyReplicationConfigMessageRequestTypeDef,
     _OptionalModifyReplicationConfigMessageRequestTypeDef,
 ):
     pass
 
-ReplicationConfigTypeDef = TypedDict(
-    "ReplicationConfigTypeDef",
-    {
-        "ReplicationConfigIdentifier": str,
-        "ReplicationConfigArn": str,
-        "SourceEndpointArn": str,
-        "TargetEndpointArn": str,
-        "ReplicationType": MigrationTypeValueType,
-        "ComputeConfig": ComputeConfigTypeDef,
-        "ReplicationSettings": str,
-        "SupplementalSettings": str,
-        "TableMappings": str,
-        "ReplicationConfigCreateTime": datetime,
-        "ReplicationConfigUpdateTime": datetime,
-    },
-)
 
-DeleteConnectionResponseTypeDef = TypedDict(
-    "DeleteConnectionResponseTypeDef",
+DeleteConnectionResponseOutputTypeDef = TypedDict(
+    "DeleteConnectionResponseOutputTypeDef",
     {
-        "Connection": ConnectionTypeDef,
+        "Connection": ConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeConnectionsResponseTypeDef = TypedDict(
-    "DescribeConnectionsResponseTypeDef",
+DescribeConnectionsResponseOutputTypeDef = TypedDict(
+    "DescribeConnectionsResponseOutputTypeDef",
     {
         "Marker": str,
-        "Connections": List[ConnectionTypeDef],
+        "Connections": List[ConnectionOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TestConnectionResponseTypeDef = TypedDict(
-    "TestConnectionResponseTypeDef",
+TestConnectionResponseOutputTypeDef = TypedDict(
+    "TestConnectionResponseOutputTypeDef",
     {
-        "Connection": ConnectionTypeDef,
+        "Connection": ConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointMessageRequestTypeDef",
     {
@@ -2229,60 +2725,20 @@
         "RedisSettings": RedisSettingsTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
         "TimestreamSettings": TimestreamSettingsTypeDef,
     },
     total=False,
 )
 
+
 class CreateEndpointMessageRequestTypeDef(
     _RequiredCreateEndpointMessageRequestTypeDef, _OptionalCreateEndpointMessageRequestTypeDef
 ):
     pass
 
-EndpointTypeDef = TypedDict(
-    "EndpointTypeDef",
-    {
-        "EndpointIdentifier": str,
-        "EndpointType": ReplicationEndpointTypeValueType,
-        "EngineName": str,
-        "EngineDisplayName": str,
-        "Username": str,
-        "ServerName": str,
-        "Port": int,
-        "DatabaseName": str,
-        "ExtraConnectionAttributes": str,
-        "Status": str,
-        "KmsKeyId": str,
-        "EndpointArn": str,
-        "CertificateArn": str,
-        "SslMode": DmsSslModeValueType,
-        "ServiceAccessRoleArn": str,
-        "ExternalTableDefinition": str,
-        "ExternalId": str,
-        "DynamoDbSettings": DynamoDbSettingsTypeDef,
-        "S3Settings": S3SettingsTypeDef,
-        "DmsTransferSettings": DmsTransferSettingsTypeDef,
-        "MongoDbSettings": MongoDbSettingsTypeDef,
-        "KinesisSettings": KinesisSettingsTypeDef,
-        "KafkaSettings": KafkaSettingsTypeDef,
-        "ElasticsearchSettings": ElasticsearchSettingsTypeDef,
-        "NeptuneSettings": NeptuneSettingsTypeDef,
-        "RedshiftSettings": RedshiftSettingsTypeDef,
-        "PostgreSQLSettings": PostgreSQLSettingsTypeDef,
-        "MySQLSettings": MySQLSettingsTypeDef,
-        "OracleSettings": OracleSettingsTypeDef,
-        "SybaseSettings": SybaseSettingsTypeDef,
-        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
-        "IBMDb2Settings": IBMDb2SettingsTypeDef,
-        "DocDbSettings": DocDbSettingsTypeDef,
-        "RedisSettings": RedisSettingsTypeDef,
-        "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
-        "TimestreamSettings": TimestreamSettingsTypeDef,
-    },
-)
 
 _RequiredModifyEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
@@ -2322,62 +2778,64 @@
         "ExactSettings": bool,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
         "TimestreamSettings": TimestreamSettingsTypeDef,
     },
     total=False,
 )
 
+
 class ModifyEndpointMessageRequestTypeDef(
     _RequiredModifyEndpointMessageRequestTypeDef, _OptionalModifyEndpointMessageRequestTypeDef
 ):
     pass
 
-CreateEventSubscriptionResponseTypeDef = TypedDict(
-    "CreateEventSubscriptionResponseTypeDef",
+
+CreateEventSubscriptionResponseOutputTypeDef = TypedDict(
+    "CreateEventSubscriptionResponseOutputTypeDef",
     {
-        "EventSubscription": EventSubscriptionTypeDef,
+        "EventSubscription": EventSubscriptionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEventSubscriptionResponseTypeDef = TypedDict(
-    "DeleteEventSubscriptionResponseTypeDef",
+DeleteEventSubscriptionResponseOutputTypeDef = TypedDict(
+    "DeleteEventSubscriptionResponseOutputTypeDef",
     {
-        "EventSubscription": EventSubscriptionTypeDef,
+        "EventSubscription": EventSubscriptionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventSubscriptionsResponseTypeDef = TypedDict(
-    "DescribeEventSubscriptionsResponseTypeDef",
+DescribeEventSubscriptionsResponseOutputTypeDef = TypedDict(
+    "DescribeEventSubscriptionsResponseOutputTypeDef",
     {
         "Marker": str,
-        "EventSubscriptionsList": List[EventSubscriptionTypeDef],
+        "EventSubscriptionsList": List[EventSubscriptionOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyEventSubscriptionResponseTypeDef = TypedDict(
-    "ModifyEventSubscriptionResponseTypeDef",
+ModifyEventSubscriptionResponseOutputTypeDef = TypedDict(
+    "ModifyEventSubscriptionResponseOutputTypeDef",
     {
-        "EventSubscription": EventSubscriptionTypeDef,
+        "EventSubscription": EventSubscriptionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatabaseResponseTypeDef = TypedDict(
-    "DatabaseResponseTypeDef",
+DatabaseResponseOutputTypeDef = TypedDict(
+    "DatabaseResponseOutputTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "IpAddress": str,
         "NumberOfSchemas": int,
-        "Server": ServerShortInfoResponseTypeDef,
-        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
-        "Collectors": List[CollectorShortInfoResponseTypeDef],
+        "Server": ServerShortInfoResponseOutputTypeDef,
+        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseOutputTypeDef,
+        "Collectors": List[CollectorShortInfoResponseOutputTypeDef],
     },
 )
 
 DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -2645,20 +3103,22 @@
         "MaxRecords": int,
         "Marker": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+
 class DescribeReplicationTableStatisticsMessageRequestTypeDef(
     _RequiredDescribeReplicationTableStatisticsMessageRequestTypeDef,
     _OptionalDescribeReplicationTableStatisticsMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2717,20 +3177,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
     _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
     _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
 _OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
@@ -2739,20 +3201,22 @@
         "MaxRecords": int,
         "Marker": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+
 class DescribeTableStatisticsMessageRequestTypeDef(
     _RequiredDescribeTableStatisticsMessageRequestTypeDef,
     _OptionalDescribeTableStatisticsMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef = TypedDict(
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
@@ -2837,163 +3301,215 @@
         "Marker": str,
         "WithoutSettings": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEndpointSettingsResponseTypeDef = TypedDict(
-    "DescribeEndpointSettingsResponseTypeDef",
+DescribeEndpointSettingsResponseOutputTypeDef = TypedDict(
+    "DescribeEndpointSettingsResponseOutputTypeDef",
     {
         "Marker": str,
-        "EndpointSettings": List[EndpointSettingTypeDef],
+        "EndpointSettings": List[EndpointSettingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEndpointTypesResponseTypeDef = TypedDict(
-    "DescribeEndpointTypesResponseTypeDef",
+DescribeEndpointTypesResponseOutputTypeDef = TypedDict(
+    "DescribeEndpointTypesResponseOutputTypeDef",
     {
         "Marker": str,
-        "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
+        "SupportedEndpointTypes": List[SupportedEndpointTypeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventCategoriesResponseTypeDef = TypedDict(
-    "DescribeEventCategoriesResponseTypeDef",
+DescribeEventCategoriesResponseOutputTypeDef = TypedDict(
+    "DescribeEventCategoriesResponseOutputTypeDef",
     {
-        "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
+        "EventCategoryGroupList": List[EventCategoryGroupOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventsResponseTypeDef = TypedDict(
-    "DescribeEventsResponseTypeDef",
+DescribeEventsResponseOutputTypeDef = TypedDict(
+    "DescribeEventsResponseOutputTypeDef",
     {
         "Marker": str,
-        "Events": List[EventTypeDef],
+        "Events": List[EventOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
+DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
+    "DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef",
     {
-        "Analysis": List[FleetAdvisorLsaAnalysisResponseTypeDef],
+        "Analysis": List[FleetAdvisorLsaAnalysisResponseOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
+DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef = TypedDict(
+    "DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef",
     {
-        "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseTypeDef],
+        "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeOrderableReplicationInstancesResponseTypeDef = TypedDict(
-    "DescribeOrderableReplicationInstancesResponseTypeDef",
+DescribeOrderableReplicationInstancesResponseOutputTypeDef = TypedDict(
+    "DescribeOrderableReplicationInstancesResponseOutputTypeDef",
     {
-        "OrderableReplicationInstances": List[OrderableReplicationInstanceTypeDef],
+        "OrderableReplicationInstances": List[OrderableReplicationInstanceOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecommendationLimitationsResponseTypeDef = TypedDict(
-    "DescribeRecommendationLimitationsResponseTypeDef",
+DescribeRecommendationLimitationsResponseOutputTypeDef = TypedDict(
+    "DescribeRecommendationLimitationsResponseOutputTypeDef",
     {
         "NextToken": str,
-        "Limitations": List[LimitationTypeDef],
+        "Limitations": List[LimitationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRefreshSchemasStatusResponseTypeDef = TypedDict(
-    "DescribeRefreshSchemasStatusResponseTypeDef",
+DescribeRefreshSchemasStatusResponseOutputTypeDef = TypedDict(
+    "DescribeRefreshSchemasStatusResponseOutputTypeDef",
     {
-        "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
+        "RefreshSchemasStatus": RefreshSchemasStatusOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RefreshSchemasResponseTypeDef = TypedDict(
-    "RefreshSchemasResponseTypeDef",
+RefreshSchemasResponseOutputTypeDef = TypedDict(
+    "RefreshSchemasResponseOutputTypeDef",
     {
-        "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
+        "RefreshSchemasStatus": RefreshSchemasStatusOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationInstanceTaskLogsResponseTypeDef = TypedDict(
-    "DescribeReplicationInstanceTaskLogsResponseTypeDef",
+DescribeReplicationInstanceTaskLogsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationInstanceTaskLogsResponseOutputTypeDef",
     {
         "ReplicationInstanceArn": str,
-        "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
+        "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTableStatisticsResponseTypeDef = TypedDict(
-    "DescribeReplicationTableStatisticsResponseTypeDef",
+DescribeReplicationTableStatisticsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationTableStatisticsResponseOutputTypeDef",
     {
         "ReplicationConfigArn": str,
         "Marker": str,
-        "ReplicationTableStatistics": List[TableStatisticsTypeDef],
+        "ReplicationTableStatistics": List[TableStatisticsOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeTableStatisticsResponseTypeDef = TypedDict(
-    "DescribeTableStatisticsResponseTypeDef",
+DescribeTableStatisticsResponseOutputTypeDef = TypedDict(
+    "DescribeTableStatisticsResponseOutputTypeDef",
     {
         "ReplicationTaskArn": str,
-        "TableStatistics": List[TableStatisticsTypeDef],
+        "TableStatistics": List[TableStatisticsOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
+DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef",
     {
         "Marker": str,
         "BucketName": str,
-        "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
+        "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskIndividualAssessmentsResponseTypeDef = TypedDict(
-    "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
+DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
+        "ReplicationTaskIndividualAssessments": List[
+            ReplicationTaskIndividualAssessmentOutputTypeDef
+        ],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EndpointOutputTypeDef = TypedDict(
+    "EndpointOutputTypeDef",
+    {
+        "EndpointIdentifier": str,
+        "EndpointType": ReplicationEndpointTypeValueType,
+        "EngineName": str,
+        "EngineDisplayName": str,
+        "Username": str,
+        "ServerName": str,
+        "Port": int,
+        "DatabaseName": str,
+        "ExtraConnectionAttributes": str,
+        "Status": str,
+        "KmsKeyId": str,
+        "EndpointArn": str,
+        "CertificateArn": str,
+        "SslMode": DmsSslModeValueType,
+        "ServiceAccessRoleArn": str,
+        "ExternalTableDefinition": str,
+        "ExternalId": str,
+        "DynamoDbSettings": DynamoDbSettingsOutputTypeDef,
+        "S3Settings": S3SettingsOutputTypeDef,
+        "DmsTransferSettings": DmsTransferSettingsOutputTypeDef,
+        "MongoDbSettings": MongoDbSettingsOutputTypeDef,
+        "KinesisSettings": KinesisSettingsOutputTypeDef,
+        "KafkaSettings": KafkaSettingsOutputTypeDef,
+        "ElasticsearchSettings": ElasticsearchSettingsOutputTypeDef,
+        "NeptuneSettings": NeptuneSettingsOutputTypeDef,
+        "RedshiftSettings": RedshiftSettingsOutputTypeDef,
+        "PostgreSQLSettings": PostgreSQLSettingsOutputTypeDef,
+        "MySQLSettings": MySQLSettingsOutputTypeDef,
+        "OracleSettings": OracleSettingsOutputTypeDef,
+        "SybaseSettings": SybaseSettingsOutputTypeDef,
+        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsOutputTypeDef,
+        "IBMDb2Settings": IBMDb2SettingsOutputTypeDef,
+        "DocDbSettings": DocDbSettingsOutputTypeDef,
+        "RedisSettings": RedisSettingsOutputTypeDef,
+        "GcpMySQLSettings": GcpMySQLSettingsOutputTypeDef,
+        "TimestreamSettings": TimestreamSettingsOutputTypeDef,
+    },
+)
+
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResourcePendingMaintenanceActionsTypeDef = TypedDict(
-    "ResourcePendingMaintenanceActionsTypeDef",
+ResourcePendingMaintenanceActionsOutputTypeDef = TypedDict(
+    "ResourcePendingMaintenanceActionsOutputTypeDef",
     {
         "ResourceIdentifier": str,
-        "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
+        "PendingMaintenanceActionDetails": List[PendingMaintenanceActionOutputTypeDef],
     },
 )
 
-RdsRecommendationTypeDef = TypedDict(
-    "RdsRecommendationTypeDef",
+RdsRecommendationOutputTypeDef = TypedDict(
+    "RdsRecommendationOutputTypeDef",
     {
-        "RequirementsToTarget": RdsRequirementsTypeDef,
-        "TargetConfiguration": RdsConfigurationTypeDef,
+        "RequirementsToTarget": RdsRequirementsOutputTypeDef,
+        "TargetConfiguration": RdsConfigurationOutputTypeDef,
     },
 )
 
 StartRecommendationsRequestEntryTypeDef = TypedDict(
     "StartRecommendationsRequestEntryTypeDef",
     {
         "DatabaseId": str,
@@ -3020,20 +3536,22 @@
     "_OptionalReloadReplicationTablesMessageRequestTypeDef",
     {
         "ReloadOption": ReloadOptionValueType,
     },
     total=False,
 )
 
+
 class ReloadReplicationTablesMessageRequestTypeDef(
     _RequiredReloadReplicationTablesMessageRequestTypeDef,
     _OptionalReloadReplicationTablesMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredReloadTablesMessageRequestTypeDef = TypedDict(
     "_RequiredReloadTablesMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TablesToReload": Sequence[TableToReloadTypeDef],
     },
 )
@@ -3041,63 +3559,65 @@
     "_OptionalReloadTablesMessageRequestTypeDef",
     {
         "ReloadOption": ReloadOptionValueType,
     },
     total=False,
 )
 
+
 class ReloadTablesMessageRequestTypeDef(
     _RequiredReloadTablesMessageRequestTypeDef, _OptionalReloadTablesMessageRequestTypeDef
 ):
     pass
 
-ReplicationTypeDef = TypedDict(
-    "ReplicationTypeDef",
+
+ReplicationOutputTypeDef = TypedDict(
+    "ReplicationOutputTypeDef",
     {
         "ReplicationConfigIdentifier": str,
         "ReplicationConfigArn": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationType": MigrationTypeValueType,
         "Status": str,
-        "ProvisionData": ProvisionDataTypeDef,
+        "ProvisionData": ProvisionDataOutputTypeDef,
         "StopReason": str,
         "FailureMessages": List[str],
-        "ReplicationStats": ReplicationStatsTypeDef,
+        "ReplicationStats": ReplicationStatsOutputTypeDef,
         "StartReplicationType": str,
         "CdcStartTime": datetime,
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationCreateTime": datetime,
         "ReplicationUpdateTime": datetime,
         "ReplicationLastStopTime": datetime,
     },
 )
 
-ReplicationTaskAssessmentRunTypeDef = TypedDict(
-    "ReplicationTaskAssessmentRunTypeDef",
+ReplicationTaskAssessmentRunOutputTypeDef = TypedDict(
+    "ReplicationTaskAssessmentRunOutputTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
         "ReplicationTaskArn": str,
         "Status": str,
         "ReplicationTaskAssessmentRunCreationDate": datetime,
-        "AssessmentProgress": ReplicationTaskAssessmentRunProgressTypeDef,
+        "AssessmentProgress": ReplicationTaskAssessmentRunProgressOutputTypeDef,
         "LastFailureMessage": str,
         "ServiceAccessRoleArn": str,
         "ResultLocationBucket": str,
         "ResultLocationFolder": str,
         "ResultEncryptionMode": str,
         "ResultKmsKeyArn": str,
         "AssessmentRunName": str,
     },
 )
 
-ReplicationTaskTypeDef = TypedDict(
-    "ReplicationTaskTypeDef",
+ReplicationTaskOutputTypeDef = TypedDict(
+    "ReplicationTaskOutputTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationInstanceArn": str,
         "MigrationType": MigrationTypeValueType,
         "TableMappings": str,
@@ -3107,333 +3627,333 @@
         "StopReason": str,
         "ReplicationTaskCreationDate": datetime,
         "ReplicationTaskStartDate": datetime,
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationTaskArn": str,
-        "ReplicationTaskStats": ReplicationTaskStatsTypeDef,
+        "ReplicationTaskStats": ReplicationTaskStatsOutputTypeDef,
         "TaskData": str,
         "TargetReplicationInstanceArn": str,
     },
 )
 
-SchemaResponseTypeDef = TypedDict(
-    "SchemaResponseTypeDef",
+SchemaResponseOutputTypeDef = TypedDict(
+    "SchemaResponseOutputTypeDef",
     {
         "CodeLineCount": int,
         "CodeSize": int,
         "Complexity": str,
-        "Server": ServerShortInfoResponseTypeDef,
-        "DatabaseInstance": DatabaseShortInfoResponseTypeDef,
+        "Server": ServerShortInfoResponseOutputTypeDef,
+        "DatabaseInstance": DatabaseShortInfoResponseOutputTypeDef,
         "SchemaId": str,
         "SchemaName": str,
-        "OriginalSchema": SchemaShortInfoResponseTypeDef,
+        "OriginalSchema": SchemaShortInfoResponseOutputTypeDef,
         "Similarity": float,
     },
 )
 
-ReplicationSubnetGroupTypeDef = TypedDict(
-    "ReplicationSubnetGroupTypeDef",
+ReplicationSubnetGroupOutputTypeDef = TypedDict(
+    "ReplicationSubnetGroupOutputTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "ReplicationSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
-        "Subnets": List[SubnetTypeDef],
+        "Subnets": List[SubnetOutputTypeDef],
         "SupportedNetworkTypes": List[str],
     },
 )
 
-DescribeFleetAdvisorCollectorsResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorCollectorsResponseTypeDef",
+DescribeFleetAdvisorCollectorsResponseOutputTypeDef = TypedDict(
+    "DescribeFleetAdvisorCollectorsResponseOutputTypeDef",
     {
-        "Collectors": List[CollectorResponseTypeDef],
+        "Collectors": List[CollectorResponseOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationConfigResponseTypeDef = TypedDict(
-    "CreateReplicationConfigResponseTypeDef",
+CreateReplicationConfigResponseOutputTypeDef = TypedDict(
+    "CreateReplicationConfigResponseOutputTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationConfigResponseTypeDef = TypedDict(
-    "DeleteReplicationConfigResponseTypeDef",
+DeleteReplicationConfigResponseOutputTypeDef = TypedDict(
+    "DeleteReplicationConfigResponseOutputTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationConfigsResponseTypeDef = TypedDict(
-    "DescribeReplicationConfigsResponseTypeDef",
+DescribeReplicationConfigsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationConfigsResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationConfigs": List[ReplicationConfigTypeDef],
+        "ReplicationConfigs": List[ReplicationConfigOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationConfigResponseTypeDef = TypedDict(
-    "ModifyReplicationConfigResponseTypeDef",
+ModifyReplicationConfigResponseOutputTypeDef = TypedDict(
+    "ModifyReplicationConfigResponseOutputTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
+DescribeFleetAdvisorDatabasesResponseOutputTypeDef = TypedDict(
+    "DescribeFleetAdvisorDatabasesResponseOutputTypeDef",
     {
-        "Endpoint": EndpointTypeDef,
+        "Databases": List[DatabaseResponseOutputTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEndpointResponseTypeDef = TypedDict(
-    "DeleteEndpointResponseTypeDef",
+CreateEndpointResponseOutputTypeDef = TypedDict(
+    "CreateEndpointResponseOutputTypeDef",
     {
-        "Endpoint": EndpointTypeDef,
+        "Endpoint": EndpointOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEndpointsResponseTypeDef = TypedDict(
-    "DescribeEndpointsResponseTypeDef",
+DeleteEndpointResponseOutputTypeDef = TypedDict(
+    "DeleteEndpointResponseOutputTypeDef",
     {
-        "Marker": str,
-        "Endpoints": List[EndpointTypeDef],
+        "Endpoint": EndpointOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyEndpointResponseTypeDef = TypedDict(
-    "ModifyEndpointResponseTypeDef",
+DescribeEndpointsResponseOutputTypeDef = TypedDict(
+    "DescribeEndpointsResponseOutputTypeDef",
     {
-        "Endpoint": EndpointTypeDef,
+        "Marker": str,
+        "Endpoints": List[EndpointOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
+ModifyEndpointResponseOutputTypeDef = TypedDict(
+    "ModifyEndpointResponseOutputTypeDef",
     {
-        "Databases": List[DatabaseResponseTypeDef],
-        "NextToken": str,
+        "Endpoint": EndpointOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
-    "ApplyPendingMaintenanceActionResponseTypeDef",
+ApplyPendingMaintenanceActionResponseOutputTypeDef = TypedDict(
+    "ApplyPendingMaintenanceActionResponseOutputTypeDef",
     {
-        "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
+        "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribePendingMaintenanceActionsResponseTypeDef = TypedDict(
-    "DescribePendingMaintenanceActionsResponseTypeDef",
+DescribePendingMaintenanceActionsResponseOutputTypeDef = TypedDict(
+    "DescribePendingMaintenanceActionsResponseOutputTypeDef",
     {
-        "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
+        "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecommendationDataTypeDef = TypedDict(
-    "RecommendationDataTypeDef",
+RecommendationDataOutputTypeDef = TypedDict(
+    "RecommendationDataOutputTypeDef",
     {
-        "RdsEngine": RdsRecommendationTypeDef,
+        "RdsEngine": RdsRecommendationOutputTypeDef,
     },
 )
 
 BatchStartRecommendationsRequestRequestTypeDef = TypedDict(
     "BatchStartRecommendationsRequestRequestTypeDef",
     {
         "Data": Sequence[StartRecommendationsRequestEntryTypeDef],
     },
     total=False,
 )
 
-DescribeReplicationsResponseTypeDef = TypedDict(
-    "DescribeReplicationsResponseTypeDef",
+DescribeReplicationsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationsResponseOutputTypeDef",
     {
         "Marker": str,
-        "Replications": List[ReplicationTypeDef],
+        "Replications": List[ReplicationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationResponseTypeDef = TypedDict(
-    "StartReplicationResponseTypeDef",
+StartReplicationResponseOutputTypeDef = TypedDict(
+    "StartReplicationResponseOutputTypeDef",
     {
-        "Replication": ReplicationTypeDef,
+        "Replication": ReplicationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopReplicationResponseTypeDef = TypedDict(
-    "StopReplicationResponseTypeDef",
+StopReplicationResponseOutputTypeDef = TypedDict(
+    "StopReplicationResponseOutputTypeDef",
     {
-        "Replication": ReplicationTypeDef,
+        "Replication": ReplicationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
-    "CancelReplicationTaskAssessmentRunResponseTypeDef",
+CancelReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
+    "CancelReplicationTaskAssessmentRunResponseOutputTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
-    "DeleteReplicationTaskAssessmentRunResponseTypeDef",
+DeleteReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
+    "DeleteReplicationTaskAssessmentRunResponseOutputTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskAssessmentRunsResponseTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
+DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunTypeDef],
+        "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
-    "StartReplicationTaskAssessmentRunResponseTypeDef",
+StartReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
+    "StartReplicationTaskAssessmentRunResponseOutputTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationTaskResponseTypeDef = TypedDict(
-    "CreateReplicationTaskResponseTypeDef",
+CreateReplicationTaskResponseOutputTypeDef = TypedDict(
+    "CreateReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationTaskResponseTypeDef = TypedDict(
-    "DeleteReplicationTaskResponseTypeDef",
+DeleteReplicationTaskResponseOutputTypeDef = TypedDict(
+    "DeleteReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTasksResponseTypeDef = TypedDict(
-    "DescribeReplicationTasksResponseTypeDef",
+DescribeReplicationTasksResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationTasksResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationTasks": List[ReplicationTaskTypeDef],
+        "ReplicationTasks": List[ReplicationTaskOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationTaskResponseTypeDef = TypedDict(
-    "ModifyReplicationTaskResponseTypeDef",
+ModifyReplicationTaskResponseOutputTypeDef = TypedDict(
+    "ModifyReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-MoveReplicationTaskResponseTypeDef = TypedDict(
-    "MoveReplicationTaskResponseTypeDef",
+MoveReplicationTaskResponseOutputTypeDef = TypedDict(
+    "MoveReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskAssessmentResponseTypeDef = TypedDict(
-    "StartReplicationTaskAssessmentResponseTypeDef",
+StartReplicationTaskAssessmentResponseOutputTypeDef = TypedDict(
+    "StartReplicationTaskAssessmentResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskResponseTypeDef = TypedDict(
-    "StartReplicationTaskResponseTypeDef",
+StartReplicationTaskResponseOutputTypeDef = TypedDict(
+    "StartReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopReplicationTaskResponseTypeDef = TypedDict(
-    "StopReplicationTaskResponseTypeDef",
+StopReplicationTaskResponseOutputTypeDef = TypedDict(
+    "StopReplicationTaskResponseOutputTypeDef",
     {
-        "ReplicationTask": ReplicationTaskTypeDef,
+        "ReplicationTask": ReplicationTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorSchemasResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorSchemasResponseTypeDef",
+DescribeFleetAdvisorSchemasResponseOutputTypeDef = TypedDict(
+    "DescribeFleetAdvisorSchemasResponseOutputTypeDef",
     {
-        "FleetAdvisorSchemas": List[SchemaResponseTypeDef],
+        "FleetAdvisorSchemas": List[SchemaResponseOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationSubnetGroupResponseTypeDef = TypedDict(
-    "CreateReplicationSubnetGroupResponseTypeDef",
+CreateReplicationSubnetGroupResponseOutputTypeDef = TypedDict(
+    "CreateReplicationSubnetGroupResponseOutputTypeDef",
     {
-        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationSubnetGroupsResponseTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsResponseTypeDef",
+DescribeReplicationSubnetGroupsResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationSubnetGroups": List[ReplicationSubnetGroupTypeDef],
+        "ReplicationSubnetGroups": List[ReplicationSubnetGroupOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationSubnetGroupResponseTypeDef = TypedDict(
-    "ModifyReplicationSubnetGroupResponseTypeDef",
+ModifyReplicationSubnetGroupResponseOutputTypeDef = TypedDict(
+    "ModifyReplicationSubnetGroupResponseOutputTypeDef",
     {
-        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReplicationInstanceTypeDef = TypedDict(
-    "ReplicationInstanceTypeDef",
+ReplicationInstanceOutputTypeDef = TypedDict(
+    "ReplicationInstanceOutputTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
         "ReplicationInstanceClass": str,
         "ReplicationInstanceStatus": str,
         "AllocatedStorage": int,
         "InstanceCreateTime": datetime,
-        "VpcSecurityGroups": List[VpcSecurityGroupMembershipTypeDef],
+        "VpcSecurityGroups": List[VpcSecurityGroupMembershipOutputTypeDef],
         "AvailabilityZone": str,
-        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
         "PreferredMaintenanceWindow": str,
-        "PendingModifiedValues": ReplicationPendingModifiedValuesTypeDef,
+        "PendingModifiedValues": ReplicationPendingModifiedValuesOutputTypeDef,
         "MultiAZ": bool,
         "EngineVersion": str,
         "AutoMinorVersionUpgrade": bool,
         "KmsKeyId": str,
         "ReplicationInstanceArn": str,
         "ReplicationInstancePublicIpAddress": str,
         "ReplicationInstancePrivateIpAddress": str,
@@ -3444,69 +3964,69 @@
         "SecondaryAvailabilityZone": str,
         "FreeUntil": datetime,
         "DnsNameServers": str,
         "NetworkType": str,
     },
 )
 
-RecommendationTypeDef = TypedDict(
-    "RecommendationTypeDef",
+RecommendationOutputTypeDef = TypedDict(
+    "RecommendationOutputTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "CreatedDate": str,
         "Status": str,
         "Preferred": bool,
-        "Settings": RecommendationSettingsTypeDef,
-        "Data": RecommendationDataTypeDef,
+        "Settings": RecommendationSettingsOutputTypeDef,
+        "Data": RecommendationDataOutputTypeDef,
     },
 )
 
-CreateReplicationInstanceResponseTypeDef = TypedDict(
-    "CreateReplicationInstanceResponseTypeDef",
+CreateReplicationInstanceResponseOutputTypeDef = TypedDict(
+    "CreateReplicationInstanceResponseOutputTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceTypeDef,
+        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationInstanceResponseTypeDef = TypedDict(
-    "DeleteReplicationInstanceResponseTypeDef",
+DeleteReplicationInstanceResponseOutputTypeDef = TypedDict(
+    "DeleteReplicationInstanceResponseOutputTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceTypeDef,
+        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationInstancesResponseTypeDef = TypedDict(
-    "DescribeReplicationInstancesResponseTypeDef",
+DescribeReplicationInstancesResponseOutputTypeDef = TypedDict(
+    "DescribeReplicationInstancesResponseOutputTypeDef",
     {
         "Marker": str,
-        "ReplicationInstances": List[ReplicationInstanceTypeDef],
+        "ReplicationInstances": List[ReplicationInstanceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationInstanceResponseTypeDef = TypedDict(
-    "ModifyReplicationInstanceResponseTypeDef",
+ModifyReplicationInstanceResponseOutputTypeDef = TypedDict(
+    "ModifyReplicationInstanceResponseOutputTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceTypeDef,
+        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RebootReplicationInstanceResponseTypeDef = TypedDict(
-    "RebootReplicationInstanceResponseTypeDef",
+RebootReplicationInstanceResponseOutputTypeDef = TypedDict(
+    "RebootReplicationInstanceResponseOutputTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceTypeDef,
+        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecommendationsResponseTypeDef = TypedDict(
-    "DescribeRecommendationsResponseTypeDef",
+DescribeRecommendationsResponseOutputTypeDef = TypedDict(
+    "DescribeRecommendationsResponseOutputTypeDef",
     {
         "NextToken": str,
-        "Recommendations": List[RecommendationTypeDef],
+        "Recommendations": List[RecommendationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/waiter.py` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms/waiter.pyi` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/PKG-INFO` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dms
-Version: 1.28.3
-Summary: Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/
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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -472,26 +472,27 @@
 ### Typed dictionaries
 
 `mypy_boto3_dms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
-    AccountQuotaTypeDef,
+    AccountQuotaOutputTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    AvailabilityZoneTypeDef,
-    BatchStartRecommendationsErrorEntryTypeDef,
+    AvailabilityZoneOutputTypeDef,
+    BatchStartRecommendationsErrorEntryOutputTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
-    CertificateTypeDef,
-    CollectorHealthCheckTypeDef,
-    InventoryDataTypeDef,
-    CollectorShortInfoResponseTypeDef,
+    CertificateOutputTypeDef,
+    CollectorHealthCheckOutputTypeDef,
+    InventoryDataOutputTypeDef,
+    CollectorShortInfoResponseOutputTypeDef,
+    ComputeConfigOutputTypeDef,
     ComputeConfigTypeDef,
-    ConnectionTypeDef,
+    ConnectionOutputTypeDef,
     DmsTransferSettingsTypeDef,
     DocDbSettingsTypeDef,
     DynamoDbSettingsTypeDef,
     ElasticsearchSettingsTypeDef,
     GcpMySQLSettingsTypeDef,
     IBMDb2SettingsTypeDef,
     KafkaSettingsTypeDef,
@@ -503,124 +504,143 @@
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     TimestreamSettingsTypeDef,
-    EventSubscriptionTypeDef,
+    EventSubscriptionOutputTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
-    DatabaseInstanceSoftwareDetailsResponseTypeDef,
-    ServerShortInfoResponseTypeDef,
-    DatabaseShortInfoResponseTypeDef,
+    CreateFleetAdvisorCollectorResponseOutputTypeDef,
+    DatabaseInstanceSoftwareDetailsResponseOutputTypeDef,
+    ServerShortInfoResponseOutputTypeDef,
+    DatabaseShortInfoResponseOutputTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
+    DeleteFleetAdvisorDatabasesResponseOutputTypeDef,
     DeleteReplicationConfigMessageRequestTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseOutputTypeDef,
     FilterTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
-    EndpointSettingTypeDef,
-    SupportedEndpointTypeTypeDef,
-    EventCategoryGroupTypeDef,
-    EventTypeDef,
+    EndpointSettingOutputTypeDef,
+    SupportedEndpointTypeOutputTypeDef,
+    EventCategoryGroupOutputTypeDef,
+    EventOutputTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
-    FleetAdvisorLsaAnalysisResponseTypeDef,
-    FleetAdvisorSchemaObjectResponseTypeDef,
+    FleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    FleetAdvisorSchemaObjectResponseOutputTypeDef,
     DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
-    OrderableReplicationInstanceTypeDef,
-    LimitationTypeDef,
+    OrderableReplicationInstanceOutputTypeDef,
+    LimitationOutputTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
-    RefreshSchemasStatusTypeDef,
+    RefreshSchemasStatusOutputTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
-    ReplicationInstanceTaskLogTypeDef,
-    TableStatisticsTypeDef,
+    ReplicationInstanceTaskLogOutputTypeDef,
+    TableStatisticsOutputTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
-    ReplicationTaskAssessmentResultTypeDef,
-    ReplicationTaskIndividualAssessmentTypeDef,
+    ReplicationTaskAssessmentResultOutputTypeDef,
+    ReplicationTaskIndividualAssessmentOutputTypeDef,
     DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
-    DescribeSchemasResponseTypeDef,
+    DescribeSchemasResponseOutputTypeDef,
+    DmsTransferSettingsOutputTypeDef,
+    DocDbSettingsOutputTypeDef,
+    DynamoDbSettingsOutputTypeDef,
+    ElasticsearchSettingsOutputTypeDef,
     EmptyResponseMetadataTypeDef,
+    GcpMySQLSettingsOutputTypeDef,
+    IBMDb2SettingsOutputTypeDef,
+    KafkaSettingsOutputTypeDef,
+    KinesisSettingsOutputTypeDef,
+    MicrosoftSQLServerSettingsOutputTypeDef,
+    MongoDbSettingsOutputTypeDef,
+    MySQLSettingsOutputTypeDef,
+    NeptuneSettingsOutputTypeDef,
+    OracleSettingsOutputTypeDef,
+    PostgreSQLSettingsOutputTypeDef,
+    RedisSettingsOutputTypeDef,
+    RedshiftSettingsOutputTypeDef,
+    S3SettingsOutputTypeDef,
+    SybaseSettingsOutputTypeDef,
+    TimestreamSettingsOutputTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    TagOutputTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
     PaginatorConfigTypeDef,
-    PendingMaintenanceActionTypeDef,
-    ProvisionDataTypeDef,
-    RdsConfigurationTypeDef,
-    RdsRequirementsTypeDef,
+    PendingMaintenanceActionOutputTypeDef,
+    ProvisionDataOutputTypeDef,
+    RdsConfigurationOutputTypeDef,
+    RdsRequirementsOutputTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
+    RecommendationSettingsOutputTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
-    ReloadReplicationTablesResponseTypeDef,
-    ReloadTablesResponseTypeDef,
+    ReloadReplicationTablesResponseOutputTypeDef,
+    ReloadTablesResponseOutputTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ReplicationPendingModifiedValuesTypeDef,
-    VpcSecurityGroupMembershipTypeDef,
-    ReplicationStatsTypeDef,
-    ReplicationTaskAssessmentRunProgressTypeDef,
-    ReplicationTaskStatsTypeDef,
+    ReplicationPendingModifiedValuesOutputTypeDef,
+    VpcSecurityGroupMembershipOutputTypeDef,
+    ReplicationStatsOutputTypeDef,
+    ReplicationTaskAssessmentRunProgressOutputTypeDef,
+    ReplicationTaskStatsOutputTypeDef,
     ResponseMetadataTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
-    SchemaShortInfoResponseTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    SchemaShortInfoResponseOutputTypeDef,
     StartReplicationMessageRequestTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseOutputTypeDef,
+    DescribeAccountAttributesResponseOutputTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SubnetTypeDef,
-    BatchStartRecommendationsResponseTypeDef,
-    DeleteCertificateResponseTypeDef,
-    DescribeCertificatesResponseTypeDef,
-    ImportCertificateResponseTypeDef,
-    CollectorResponseTypeDef,
+    SubnetOutputTypeDef,
+    BatchStartRecommendationsResponseOutputTypeDef,
+    DeleteCertificateResponseOutputTypeDef,
+    DescribeCertificatesResponseOutputTypeDef,
+    ImportCertificateResponseOutputTypeDef,
+    CollectorResponseOutputTypeDef,
+    ReplicationConfigOutputTypeDef,
     CreateReplicationConfigMessageRequestTypeDef,
     ModifyReplicationConfigMessageRequestTypeDef,
-    ReplicationConfigTypeDef,
-    DeleteConnectionResponseTypeDef,
-    DescribeConnectionsResponseTypeDef,
-    TestConnectionResponseTypeDef,
+    DeleteConnectionResponseOutputTypeDef,
+    DescribeConnectionsResponseOutputTypeDef,
+    TestConnectionResponseOutputTypeDef,
     CreateEndpointMessageRequestTypeDef,
-    EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
-    CreateEventSubscriptionResponseTypeDef,
-    DeleteEventSubscriptionResponseTypeDef,
-    DescribeEventSubscriptionsResponseTypeDef,
-    ModifyEventSubscriptionResponseTypeDef,
-    DatabaseResponseTypeDef,
+    CreateEventSubscriptionResponseOutputTypeDef,
+    DeleteEventSubscriptionResponseOutputTypeDef,
+    DescribeEventSubscriptionsResponseOutputTypeDef,
+    ModifyEventSubscriptionResponseOutputTypeDef,
+    DatabaseResponseOutputTypeDef,
     DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
     DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
     DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
@@ -654,85 +674,87 @@
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef,
-    DescribeEndpointSettingsResponseTypeDef,
-    DescribeEndpointTypesResponseTypeDef,
-    DescribeEventCategoriesResponseTypeDef,
-    DescribeEventsResponseTypeDef,
-    DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
-    DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
-    DescribeOrderableReplicationInstancesResponseTypeDef,
-    DescribeRecommendationLimitationsResponseTypeDef,
-    DescribeRefreshSchemasStatusResponseTypeDef,
-    RefreshSchemasResponseTypeDef,
-    DescribeReplicationInstanceTaskLogsResponseTypeDef,
-    DescribeReplicationTableStatisticsResponseTypeDef,
-    DescribeTableStatisticsResponseTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
-    DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
-    ResourcePendingMaintenanceActionsTypeDef,
-    RdsRecommendationTypeDef,
+    DescribeEndpointSettingsResponseOutputTypeDef,
+    DescribeEndpointTypesResponseOutputTypeDef,
+    DescribeEventCategoriesResponseOutputTypeDef,
+    DescribeEventsResponseOutputTypeDef,
+    DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef,
+    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
+    DescribeRecommendationLimitationsResponseOutputTypeDef,
+    DescribeRefreshSchemasStatusResponseOutputTypeDef,
+    RefreshSchemasResponseOutputTypeDef,
+    DescribeReplicationInstanceTaskLogsResponseOutputTypeDef,
+    DescribeReplicationTableStatisticsResponseOutputTypeDef,
+    DescribeTableStatisticsResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
+    DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef,
+    EndpointOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ResourcePendingMaintenanceActionsOutputTypeDef,
+    RdsRecommendationOutputTypeDef,
     StartRecommendationsRequestEntryTypeDef,
     StartRecommendationsRequestRequestTypeDef,
     ReloadReplicationTablesMessageRequestTypeDef,
     ReloadTablesMessageRequestTypeDef,
-    ReplicationTypeDef,
-    ReplicationTaskAssessmentRunTypeDef,
-    ReplicationTaskTypeDef,
-    SchemaResponseTypeDef,
-    ReplicationSubnetGroupTypeDef,
-    DescribeFleetAdvisorCollectorsResponseTypeDef,
-    CreateReplicationConfigResponseTypeDef,
-    DeleteReplicationConfigResponseTypeDef,
-    DescribeReplicationConfigsResponseTypeDef,
-    ModifyReplicationConfigResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    DeleteEndpointResponseTypeDef,
-    DescribeEndpointsResponseTypeDef,
-    ModifyEndpointResponseTypeDef,
-    DescribeFleetAdvisorDatabasesResponseTypeDef,
-    ApplyPendingMaintenanceActionResponseTypeDef,
-    DescribePendingMaintenanceActionsResponseTypeDef,
-    RecommendationDataTypeDef,
+    ReplicationOutputTypeDef,
+    ReplicationTaskAssessmentRunOutputTypeDef,
+    ReplicationTaskOutputTypeDef,
+    SchemaResponseOutputTypeDef,
+    ReplicationSubnetGroupOutputTypeDef,
+    DescribeFleetAdvisorCollectorsResponseOutputTypeDef,
+    CreateReplicationConfigResponseOutputTypeDef,
+    DeleteReplicationConfigResponseOutputTypeDef,
+    DescribeReplicationConfigsResponseOutputTypeDef,
+    ModifyReplicationConfigResponseOutputTypeDef,
+    DescribeFleetAdvisorDatabasesResponseOutputTypeDef,
+    CreateEndpointResponseOutputTypeDef,
+    DeleteEndpointResponseOutputTypeDef,
+    DescribeEndpointsResponseOutputTypeDef,
+    ModifyEndpointResponseOutputTypeDef,
+    ApplyPendingMaintenanceActionResponseOutputTypeDef,
+    DescribePendingMaintenanceActionsResponseOutputTypeDef,
+    RecommendationDataOutputTypeDef,
     BatchStartRecommendationsRequestRequestTypeDef,
-    DescribeReplicationsResponseTypeDef,
-    StartReplicationResponseTypeDef,
-    StopReplicationResponseTypeDef,
-    CancelReplicationTaskAssessmentRunResponseTypeDef,
-    DeleteReplicationTaskAssessmentRunResponseTypeDef,
-    DescribeReplicationTaskAssessmentRunsResponseTypeDef,
-    StartReplicationTaskAssessmentRunResponseTypeDef,
-    CreateReplicationTaskResponseTypeDef,
-    DeleteReplicationTaskResponseTypeDef,
-    DescribeReplicationTasksResponseTypeDef,
-    ModifyReplicationTaskResponseTypeDef,
-    MoveReplicationTaskResponseTypeDef,
-    StartReplicationTaskAssessmentResponseTypeDef,
-    StartReplicationTaskResponseTypeDef,
-    StopReplicationTaskResponseTypeDef,
-    DescribeFleetAdvisorSchemasResponseTypeDef,
-    CreateReplicationSubnetGroupResponseTypeDef,
-    DescribeReplicationSubnetGroupsResponseTypeDef,
-    ModifyReplicationSubnetGroupResponseTypeDef,
-    ReplicationInstanceTypeDef,
-    RecommendationTypeDef,
-    CreateReplicationInstanceResponseTypeDef,
-    DeleteReplicationInstanceResponseTypeDef,
-    DescribeReplicationInstancesResponseTypeDef,
-    ModifyReplicationInstanceResponseTypeDef,
-    RebootReplicationInstanceResponseTypeDef,
-    DescribeRecommendationsResponseTypeDef,
+    DescribeReplicationsResponseOutputTypeDef,
+    StartReplicationResponseOutputTypeDef,
+    StopReplicationResponseOutputTypeDef,
+    CancelReplicationTaskAssessmentRunResponseOutputTypeDef,
+    DeleteReplicationTaskAssessmentRunResponseOutputTypeDef,
+    DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef,
+    StartReplicationTaskAssessmentRunResponseOutputTypeDef,
+    CreateReplicationTaskResponseOutputTypeDef,
+    DeleteReplicationTaskResponseOutputTypeDef,
+    DescribeReplicationTasksResponseOutputTypeDef,
+    ModifyReplicationTaskResponseOutputTypeDef,
+    MoveReplicationTaskResponseOutputTypeDef,
+    StartReplicationTaskAssessmentResponseOutputTypeDef,
+    StartReplicationTaskResponseOutputTypeDef,
+    StopReplicationTaskResponseOutputTypeDef,
+    DescribeFleetAdvisorSchemasResponseOutputTypeDef,
+    CreateReplicationSubnetGroupResponseOutputTypeDef,
+    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
+    ModifyReplicationSubnetGroupResponseOutputTypeDef,
+    ReplicationInstanceOutputTypeDef,
+    RecommendationOutputTypeDef,
+    CreateReplicationInstanceResponseOutputTypeDef,
+    DeleteReplicationInstanceResponseOutputTypeDef,
+    DescribeReplicationInstancesResponseOutputTypeDef,
+    ModifyReplicationInstanceResponseOutputTypeDef,
+    RebootReplicationInstanceResponseOutputTypeDef,
+    DescribeRecommendationsResponseOutputTypeDef,
 )
 
 
-def get_structure() -> AccountQuotaTypeDef:
+def get_structure() -> AccountQuotaOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dms-1.28.3/mypy_boto3_dms.egg-info/SOURCES.txt` & `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3/setup.py` & `mypy-boto3-dms-1.28.3.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dms",
-    version="1.28.3",
+    version="1.28.3.post1",
     packages=["mypy_boto3_dms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with"
-        " mypy-boto3-builder 7.14.6"
+        " mypy-boto3-builder 7.14.7"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

