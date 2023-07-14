# Comparing `tmp/mypy-boto3-connect-1.28.3.tar.gz` & `tmp/mypy-boto3-connect-1.28.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connect-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
+gzip compressed data, was "mypy-boto3-connect-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
```

## Comparing `mypy-boto3-connect-1.28.3.tar` & `mypy-boto3-connect-1.28.3.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.665227 mypy-boto3-connect-1.28.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    45384 2023-07-13 19:49:12.665227 mypy-boto3-connect-1.28.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43899 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-connect-1.28.3/mypy_boto3_connect/
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   151314 2023-07-13 19:47:01.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   151066 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25344 2023-07-13 19:47:02.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-13 19:47:02.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-13 19:47:02.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    54267 2023-07-13 19:47:02.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   215088 2023-07-13 19:47:08.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   214775 2023-07-13 19:47:05.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.665227 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45384 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.665227 mypy-boto3-connect-1.28.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.903361 mypy-boto3-connect-1.28.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:15:21.000000 mypy-boto3-connect-1.28.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    49019 2023-07-14 16:17:59.899361 mypy-boto3-connect-1.28.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    47528 2023-07-14 16:15:21.000000 mypy-boto3-connect-1.28.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-14 16:15:22.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-14 16:15:22.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-14 16:15:22.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152776 2023-07-14 16:15:23.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152528 2023-07-14 16:15:22.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25344 2023-07-14 16:15:24.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-14 16:15:24.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    54854 2023-07-14 16:15:24.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54807 2023-07-14 16:15:24.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:22.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   234700 2023-07-14 16:15:31.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234387 2023-07-14 16:15:27.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:15:21.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.899361 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49019 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.903361 mypy-boto3-connect-1.28.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-14 16:15:21.000000 mypy-boto3-connect-1.28.3.post1/setup.py
```

### Comparing `mypy-boto3-connect-1.28.3/LICENSE` & `mypy-boto3-connect-1.28.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3/PKG-INFO` & `mypy-boto3-connect-1.28.3.post1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.28.3
-Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
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
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -578,101 +578,103 @@
 ### Typed dictionaries
 
 `mypy_boto3_connect.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connect.type_defs import (
-    ActionSummaryTypeDef,
+    ActionSummaryOutputTypeDef,
     ActivateEvaluationFormRequestRequestTypeDef,
-    ActivateEvaluationFormResponseTypeDef,
-    AgentContactReferenceTypeDef,
-    AgentInfoTypeDef,
-    AgentStatusReferenceTypeDef,
-    AgentStatusSummaryTypeDef,
-    AgentStatusTypeDef,
+    ActivateEvaluationFormResponseOutputTypeDef,
+    AgentContactReferenceOutputTypeDef,
+    AgentInfoOutputTypeDef,
+    AgentStatusOutputTypeDef,
+    AgentStatusReferenceOutputTypeDef,
+    AgentStatusSummaryOutputTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     AssociateApprovedOriginRequestRequestTypeDef,
     AssociateBotRequestRequestTypeDef,
     AssociateDefaultVocabularyRequestRequestTypeDef,
     AssociateInstanceStorageConfigRequestRequestTypeDef,
-    AssociateInstanceStorageConfigResponseTypeDef,
+    AssociateInstanceStorageConfigResponseOutputTypeDef,
     AssociateLambdaFunctionRequestRequestTypeDef,
     AssociateLexBotRequestRequestTypeDef,
     AssociatePhoneNumberContactFlowRequestRequestTypeDef,
     AssociateQueueQuickConnectsRequestRequestTypeDef,
     AssociateRoutingProfileQueuesRequestRequestTypeDef,
     AssociateSecurityKeyRequestRequestTypeDef,
-    AssociateSecurityKeyResponseTypeDef,
-    AttachmentReferenceTypeDef,
-    AttributeTypeDef,
-    AvailableNumberSummaryTypeDef,
+    AssociateSecurityKeyResponseOutputTypeDef,
+    AttachmentReferenceOutputTypeDef,
+    AttributeOutputTypeDef,
+    AvailableNumberSummaryOutputTypeDef,
     ChatMessageTypeDef,
     ChatParticipantRoleConfigTypeDef,
     ChatStreamingConfigurationTypeDef,
     ClaimPhoneNumberRequestRequestTypeDef,
-    ClaimPhoneNumberResponseTypeDef,
-    ClaimedPhoneNumberSummaryTypeDef,
+    ClaimPhoneNumberResponseOutputTypeDef,
+    ClaimedPhoneNumberSummaryOutputTypeDef,
     ContactFilterTypeDef,
-    ContactFlowModuleSummaryTypeDef,
-    ContactFlowModuleTypeDef,
-    ContactFlowSummaryTypeDef,
-    ContactFlowTypeDef,
-    ContactTypeDef,
+    ContactFlowModuleOutputTypeDef,
+    ContactFlowModuleSummaryOutputTypeDef,
+    ContactFlowOutputTypeDef,
+    ContactFlowSummaryOutputTypeDef,
+    ContactOutputTypeDef,
     ControlPlaneTagFilterTypeDef,
     CreateAgentStatusRequestRequestTypeDef,
-    CreateAgentStatusResponseTypeDef,
+    CreateAgentStatusResponseOutputTypeDef,
     CreateContactFlowModuleRequestRequestTypeDef,
-    CreateContactFlowModuleResponseTypeDef,
+    CreateContactFlowModuleResponseOutputTypeDef,
     CreateContactFlowRequestRequestTypeDef,
-    CreateContactFlowResponseTypeDef,
+    CreateContactFlowResponseOutputTypeDef,
     CreateEvaluationFormRequestRequestTypeDef,
-    CreateEvaluationFormResponseTypeDef,
+    CreateEvaluationFormResponseOutputTypeDef,
     CreateHoursOfOperationRequestRequestTypeDef,
-    CreateHoursOfOperationResponseTypeDef,
+    CreateHoursOfOperationResponseOutputTypeDef,
     CreateInstanceRequestRequestTypeDef,
-    CreateInstanceResponseTypeDef,
+    CreateInstanceResponseOutputTypeDef,
     CreateIntegrationAssociationRequestRequestTypeDef,
-    CreateIntegrationAssociationResponseTypeDef,
+    CreateIntegrationAssociationResponseOutputTypeDef,
     CreateParticipantRequestRequestTypeDef,
-    CreateParticipantResponseTypeDef,
+    CreateParticipantResponseOutputTypeDef,
     CreatePromptRequestRequestTypeDef,
-    CreatePromptResponseTypeDef,
+    CreatePromptResponseOutputTypeDef,
     CreateQueueRequestRequestTypeDef,
-    CreateQueueResponseTypeDef,
+    CreateQueueResponseOutputTypeDef,
     CreateQuickConnectRequestRequestTypeDef,
-    CreateQuickConnectResponseTypeDef,
+    CreateQuickConnectResponseOutputTypeDef,
     CreateRoutingProfileRequestRequestTypeDef,
-    CreateRoutingProfileResponseTypeDef,
+    CreateRoutingProfileResponseOutputTypeDef,
     CreateRuleRequestRequestTypeDef,
-    CreateRuleResponseTypeDef,
+    CreateRuleResponseOutputTypeDef,
     CreateSecurityProfileRequestRequestTypeDef,
-    CreateSecurityProfileResponseTypeDef,
+    CreateSecurityProfileResponseOutputTypeDef,
     CreateTaskTemplateRequestRequestTypeDef,
-    CreateTaskTemplateResponseTypeDef,
+    CreateTaskTemplateResponseOutputTypeDef,
     CreateTrafficDistributionGroupRequestRequestTypeDef,
-    CreateTrafficDistributionGroupResponseTypeDef,
+    CreateTrafficDistributionGroupResponseOutputTypeDef,
     CreateUseCaseRequestRequestTypeDef,
-    CreateUseCaseResponseTypeDef,
+    CreateUseCaseResponseOutputTypeDef,
     CreateUserHierarchyGroupRequestRequestTypeDef,
-    CreateUserHierarchyGroupResponseTypeDef,
+    CreateUserHierarchyGroupResponseOutputTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseTypeDef,
+    CreateUserResponseOutputTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    CreateVocabularyResponseTypeDef,
-    CredentialsTypeDef,
+    CreateVocabularyResponseOutputTypeDef,
+    CredentialsOutputTypeDef,
+    CrossChannelBehaviorOutputTypeDef,
     CrossChannelBehaviorTypeDef,
-    CurrentMetricDataTypeDef,
-    CurrentMetricResultTypeDef,
+    CurrentMetricDataOutputTypeDef,
+    CurrentMetricOutputTypeDef,
+    CurrentMetricResultOutputTypeDef,
     CurrentMetricSortCriteriaTypeDef,
     CurrentMetricTypeDef,
-    DateReferenceTypeDef,
+    DateReferenceOutputTypeDef,
     DeactivateEvaluationFormRequestRequestTypeDef,
-    DeactivateEvaluationFormResponseTypeDef,
-    DefaultVocabularyTypeDef,
+    DeactivateEvaluationFormResponseOutputTypeDef,
+    DefaultVocabularyOutputTypeDef,
     DeleteContactEvaluationRequestRequestTypeDef,
     DeleteContactFlowModuleRequestRequestTypeDef,
     DeleteContactFlowRequestRequestTypeDef,
     DeleteEvaluationFormRequestRequestTypeDef,
     DeleteHoursOfOperationRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteIntegrationAssociationRequestRequestTypeDef,
@@ -684,460 +686,516 @@
     DeleteSecurityProfileRequestRequestTypeDef,
     DeleteTaskTemplateRequestRequestTypeDef,
     DeleteTrafficDistributionGroupRequestRequestTypeDef,
     DeleteUseCaseRequestRequestTypeDef,
     DeleteUserHierarchyGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
-    DeleteVocabularyResponseTypeDef,
+    DeleteVocabularyResponseOutputTypeDef,
     DescribeAgentStatusRequestRequestTypeDef,
-    DescribeAgentStatusResponseTypeDef,
+    DescribeAgentStatusResponseOutputTypeDef,
     DescribeContactEvaluationRequestRequestTypeDef,
-    DescribeContactEvaluationResponseTypeDef,
+    DescribeContactEvaluationResponseOutputTypeDef,
     DescribeContactFlowModuleRequestRequestTypeDef,
-    DescribeContactFlowModuleResponseTypeDef,
+    DescribeContactFlowModuleResponseOutputTypeDef,
     DescribeContactFlowRequestRequestTypeDef,
-    DescribeContactFlowResponseTypeDef,
+    DescribeContactFlowResponseOutputTypeDef,
     DescribeContactRequestRequestTypeDef,
-    DescribeContactResponseTypeDef,
+    DescribeContactResponseOutputTypeDef,
     DescribeEvaluationFormRequestRequestTypeDef,
-    DescribeEvaluationFormResponseTypeDef,
+    DescribeEvaluationFormResponseOutputTypeDef,
     DescribeHoursOfOperationRequestRequestTypeDef,
-    DescribeHoursOfOperationResponseTypeDef,
+    DescribeHoursOfOperationResponseOutputTypeDef,
     DescribeInstanceAttributeRequestRequestTypeDef,
-    DescribeInstanceAttributeResponseTypeDef,
+    DescribeInstanceAttributeResponseOutputTypeDef,
     DescribeInstanceRequestRequestTypeDef,
-    DescribeInstanceResponseTypeDef,
+    DescribeInstanceResponseOutputTypeDef,
     DescribeInstanceStorageConfigRequestRequestTypeDef,
-    DescribeInstanceStorageConfigResponseTypeDef,
+    DescribeInstanceStorageConfigResponseOutputTypeDef,
     DescribePhoneNumberRequestRequestTypeDef,
-    DescribePhoneNumberResponseTypeDef,
+    DescribePhoneNumberResponseOutputTypeDef,
     DescribePromptRequestRequestTypeDef,
-    DescribePromptResponseTypeDef,
+    DescribePromptResponseOutputTypeDef,
     DescribeQueueRequestRequestTypeDef,
-    DescribeQueueResponseTypeDef,
+    DescribeQueueResponseOutputTypeDef,
     DescribeQuickConnectRequestRequestTypeDef,
-    DescribeQuickConnectResponseTypeDef,
+    DescribeQuickConnectResponseOutputTypeDef,
     DescribeRoutingProfileRequestRequestTypeDef,
-    DescribeRoutingProfileResponseTypeDef,
+    DescribeRoutingProfileResponseOutputTypeDef,
     DescribeRuleRequestRequestTypeDef,
-    DescribeRuleResponseTypeDef,
+    DescribeRuleResponseOutputTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
-    DescribeSecurityProfileResponseTypeDef,
+    DescribeSecurityProfileResponseOutputTypeDef,
     DescribeTrafficDistributionGroupRequestRequestTypeDef,
-    DescribeTrafficDistributionGroupResponseTypeDef,
+    DescribeTrafficDistributionGroupResponseOutputTypeDef,
     DescribeUserHierarchyGroupRequestRequestTypeDef,
-    DescribeUserHierarchyGroupResponseTypeDef,
+    DescribeUserHierarchyGroupResponseOutputTypeDef,
     DescribeUserHierarchyStructureRequestRequestTypeDef,
-    DescribeUserHierarchyStructureResponseTypeDef,
+    DescribeUserHierarchyStructureResponseOutputTypeDef,
     DescribeUserRequestRequestTypeDef,
-    DescribeUserResponseTypeDef,
+    DescribeUserResponseOutputTypeDef,
     DescribeVocabularyRequestRequestTypeDef,
-    DescribeVocabularyResponseTypeDef,
-    DimensionsTypeDef,
+    DescribeVocabularyResponseOutputTypeDef,
+    DimensionsOutputTypeDef,
     DisassociateApprovedOriginRequestRequestTypeDef,
     DisassociateBotRequestRequestTypeDef,
     DisassociateInstanceStorageConfigRequestRequestTypeDef,
     DisassociateLambdaFunctionRequestRequestTypeDef,
     DisassociateLexBotRequestRequestTypeDef,
     DisassociatePhoneNumberContactFlowRequestRequestTypeDef,
     DisassociateQueueQuickConnectsRequestRequestTypeDef,
     DisassociateRoutingProfileQueuesRequestRequestTypeDef,
     DisassociateSecurityKeyRequestRequestTypeDef,
     DismissUserContactRequestRequestTypeDef,
+    DistributionOutputTypeDef,
     DistributionTypeDef,
-    EmailReferenceTypeDef,
+    EmailReferenceOutputTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    EvaluationAnswerDataOutputTypeDef,
     EvaluationAnswerDataTypeDef,
     EvaluationAnswerInputTypeDef,
-    EvaluationAnswerOutputTypeDef,
-    EvaluationFormContentTypeDef,
+    EvaluationAnswerOutputOutputTypeDef,
+    EvaluationFormContentOutputTypeDef,
+    EvaluationFormItemOutputTypeDef,
     EvaluationFormItemTypeDef,
+    EvaluationFormNumericQuestionAutomationOutputTypeDef,
     EvaluationFormNumericQuestionAutomationTypeDef,
+    EvaluationFormNumericQuestionOptionOutputTypeDef,
     EvaluationFormNumericQuestionOptionTypeDef,
+    EvaluationFormNumericQuestionPropertiesOutputTypeDef,
     EvaluationFormNumericQuestionPropertiesTypeDef,
+    EvaluationFormOutputTypeDef,
+    EvaluationFormQuestionOutputTypeDef,
     EvaluationFormQuestionTypeDef,
+    EvaluationFormQuestionTypePropertiesOutputTypeDef,
     EvaluationFormQuestionTypePropertiesTypeDef,
+    EvaluationFormScoringStrategyOutputTypeDef,
     EvaluationFormScoringStrategyTypeDef,
+    EvaluationFormSectionOutputTypeDef,
     EvaluationFormSectionTypeDef,
+    EvaluationFormSingleSelectQuestionAutomationOptionOutputTypeDef,
     EvaluationFormSingleSelectQuestionAutomationOptionTypeDef,
+    EvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
     EvaluationFormSingleSelectQuestionAutomationTypeDef,
+    EvaluationFormSingleSelectQuestionOptionOutputTypeDef,
     EvaluationFormSingleSelectQuestionOptionTypeDef,
+    EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
     EvaluationFormSingleSelectQuestionPropertiesTypeDef,
-    EvaluationFormSummaryTypeDef,
-    EvaluationFormTypeDef,
-    EvaluationFormVersionSummaryTypeDef,
-    EvaluationMetadataTypeDef,
+    EvaluationFormSummaryOutputTypeDef,
+    EvaluationFormVersionSummaryOutputTypeDef,
+    EvaluationMetadataOutputTypeDef,
+    EvaluationNoteOutputTypeDef,
     EvaluationNoteTypeDef,
-    EvaluationScoreTypeDef,
-    EvaluationSummaryTypeDef,
-    EvaluationTypeDef,
+    EvaluationOutputTypeDef,
+    EvaluationScoreOutputTypeDef,
+    EvaluationSummaryOutputTypeDef,
+    EventBridgeActionDefinitionOutputTypeDef,
     EventBridgeActionDefinitionTypeDef,
     FilterV2TypeDef,
     FiltersTypeDef,
     GetContactAttributesRequestRequestTypeDef,
-    GetContactAttributesResponseTypeDef,
+    GetContactAttributesResponseOutputTypeDef,
     GetCurrentMetricDataRequestRequestTypeDef,
-    GetCurrentMetricDataResponseTypeDef,
+    GetCurrentMetricDataResponseOutputTypeDef,
     GetCurrentUserDataRequestRequestTypeDef,
-    GetCurrentUserDataResponseTypeDef,
+    GetCurrentUserDataResponseOutputTypeDef,
     GetFederationTokenRequestRequestTypeDef,
-    GetFederationTokenResponseTypeDef,
+    GetFederationTokenResponseOutputTypeDef,
     GetMetricDataRequestGetMetricDataPaginateTypeDef,
     GetMetricDataRequestRequestTypeDef,
-    GetMetricDataResponseTypeDef,
+    GetMetricDataResponseOutputTypeDef,
     GetMetricDataV2RequestRequestTypeDef,
-    GetMetricDataV2ResponseTypeDef,
+    GetMetricDataV2ResponseOutputTypeDef,
     GetPromptFileRequestRequestTypeDef,
-    GetPromptFileResponseTypeDef,
+    GetPromptFileResponseOutputTypeDef,
     GetTaskTemplateRequestRequestTypeDef,
-    GetTaskTemplateResponseTypeDef,
+    GetTaskTemplateResponseOutputTypeDef,
     GetTrafficDistributionRequestRequestTypeDef,
-    GetTrafficDistributionResponseTypeDef,
+    GetTrafficDistributionResponseOutputTypeDef,
     HierarchyGroupConditionTypeDef,
-    HierarchyGroupSummaryReferenceTypeDef,
-    HierarchyGroupSummaryTypeDef,
-    HierarchyGroupTypeDef,
-    HierarchyLevelTypeDef,
+    HierarchyGroupOutputTypeDef,
+    HierarchyGroupSummaryOutputTypeDef,
+    HierarchyGroupSummaryReferenceOutputTypeDef,
+    HierarchyLevelOutputTypeDef,
     HierarchyLevelUpdateTypeDef,
-    HierarchyPathReferenceTypeDef,
-    HierarchyPathTypeDef,
-    HierarchyStructureTypeDef,
+    HierarchyPathOutputTypeDef,
+    HierarchyPathReferenceOutputTypeDef,
+    HierarchyStructureOutputTypeDef,
     HierarchyStructureUpdateTypeDef,
-    HistoricalMetricDataTypeDef,
-    HistoricalMetricResultTypeDef,
+    HistoricalMetricDataOutputTypeDef,
+    HistoricalMetricOutputTypeDef,
+    HistoricalMetricResultOutputTypeDef,
     HistoricalMetricTypeDef,
+    HoursOfOperationConfigOutputTypeDef,
     HoursOfOperationConfigTypeDef,
+    HoursOfOperationOutputTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
-    HoursOfOperationSummaryTypeDef,
+    HoursOfOperationSummaryOutputTypeDef,
+    HoursOfOperationTimeSliceOutputTypeDef,
     HoursOfOperationTimeSliceTypeDef,
-    HoursOfOperationTypeDef,
-    InstanceStatusReasonTypeDef,
+    InstanceOutputTypeDef,
+    InstanceStatusReasonOutputTypeDef,
+    InstanceStorageConfigOutputTypeDef,
     InstanceStorageConfigTypeDef,
-    InstanceSummaryTypeDef,
-    InstanceTypeDef,
-    IntegrationAssociationSummaryTypeDef,
+    InstanceSummaryOutputTypeDef,
+    IntegrationAssociationSummaryOutputTypeDef,
+    InvisibleFieldInfoOutputTypeDef,
     InvisibleFieldInfoTypeDef,
+    KinesisFirehoseConfigOutputTypeDef,
     KinesisFirehoseConfigTypeDef,
+    KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
+    KinesisVideoStreamConfigOutputTypeDef,
     KinesisVideoStreamConfigTypeDef,
-    LexBotConfigTypeDef,
+    LexBotConfigOutputTypeDef,
+    LexBotOutputTypeDef,
     LexBotTypeDef,
+    LexV2BotOutputTypeDef,
     LexV2BotTypeDef,
     ListAgentStatusRequestListAgentStatusesPaginateTypeDef,
     ListAgentStatusRequestRequestTypeDef,
-    ListAgentStatusResponseTypeDef,
+    ListAgentStatusResponseOutputTypeDef,
     ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
     ListApprovedOriginsRequestRequestTypeDef,
-    ListApprovedOriginsResponseTypeDef,
+    ListApprovedOriginsResponseOutputTypeDef,
     ListBotsRequestListBotsPaginateTypeDef,
     ListBotsRequestRequestTypeDef,
-    ListBotsResponseTypeDef,
+    ListBotsResponseOutputTypeDef,
     ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
     ListContactEvaluationsRequestRequestTypeDef,
-    ListContactEvaluationsResponseTypeDef,
+    ListContactEvaluationsResponseOutputTypeDef,
     ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
     ListContactFlowModulesRequestRequestTypeDef,
-    ListContactFlowModulesResponseTypeDef,
+    ListContactFlowModulesResponseOutputTypeDef,
     ListContactFlowsRequestListContactFlowsPaginateTypeDef,
     ListContactFlowsRequestRequestTypeDef,
-    ListContactFlowsResponseTypeDef,
+    ListContactFlowsResponseOutputTypeDef,
     ListContactReferencesRequestListContactReferencesPaginateTypeDef,
     ListContactReferencesRequestRequestTypeDef,
-    ListContactReferencesResponseTypeDef,
+    ListContactReferencesResponseOutputTypeDef,
     ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
     ListDefaultVocabulariesRequestRequestTypeDef,
-    ListDefaultVocabulariesResponseTypeDef,
+    ListDefaultVocabulariesResponseOutputTypeDef,
     ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
     ListEvaluationFormVersionsRequestRequestTypeDef,
-    ListEvaluationFormVersionsResponseTypeDef,
+    ListEvaluationFormVersionsResponseOutputTypeDef,
     ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
     ListEvaluationFormsRequestRequestTypeDef,
-    ListEvaluationFormsResponseTypeDef,
+    ListEvaluationFormsResponseOutputTypeDef,
     ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
     ListHoursOfOperationsRequestRequestTypeDef,
-    ListHoursOfOperationsResponseTypeDef,
+    ListHoursOfOperationsResponseOutputTypeDef,
     ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
     ListInstanceAttributesRequestRequestTypeDef,
-    ListInstanceAttributesResponseTypeDef,
+    ListInstanceAttributesResponseOutputTypeDef,
     ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
     ListInstanceStorageConfigsRequestRequestTypeDef,
-    ListInstanceStorageConfigsResponseTypeDef,
+    ListInstanceStorageConfigsResponseOutputTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
-    ListInstancesResponseTypeDef,
+    ListInstancesResponseOutputTypeDef,
     ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
     ListIntegrationAssociationsRequestRequestTypeDef,
-    ListIntegrationAssociationsResponseTypeDef,
+    ListIntegrationAssociationsResponseOutputTypeDef,
     ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
     ListLambdaFunctionsRequestRequestTypeDef,
-    ListLambdaFunctionsResponseTypeDef,
+    ListLambdaFunctionsResponseOutputTypeDef,
     ListLexBotsRequestListLexBotsPaginateTypeDef,
     ListLexBotsRequestRequestTypeDef,
-    ListLexBotsResponseTypeDef,
+    ListLexBotsResponseOutputTypeDef,
     ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
-    ListPhoneNumbersResponseTypeDef,
-    ListPhoneNumbersSummaryTypeDef,
+    ListPhoneNumbersResponseOutputTypeDef,
+    ListPhoneNumbersSummaryOutputTypeDef,
     ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef,
     ListPhoneNumbersV2RequestRequestTypeDef,
-    ListPhoneNumbersV2ResponseTypeDef,
+    ListPhoneNumbersV2ResponseOutputTypeDef,
     ListPromptsRequestListPromptsPaginateTypeDef,
     ListPromptsRequestRequestTypeDef,
-    ListPromptsResponseTypeDef,
+    ListPromptsResponseOutputTypeDef,
     ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
     ListQueueQuickConnectsRequestRequestTypeDef,
-    ListQueueQuickConnectsResponseTypeDef,
+    ListQueueQuickConnectsResponseOutputTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResponseTypeDef,
+    ListQueuesResponseOutputTypeDef,
     ListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
     ListQuickConnectsRequestRequestTypeDef,
-    ListQuickConnectsResponseTypeDef,
+    ListQuickConnectsResponseOutputTypeDef,
     ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
     ListRoutingProfileQueuesRequestRequestTypeDef,
-    ListRoutingProfileQueuesResponseTypeDef,
+    ListRoutingProfileQueuesResponseOutputTypeDef,
     ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
     ListRoutingProfilesRequestRequestTypeDef,
-    ListRoutingProfilesResponseTypeDef,
+    ListRoutingProfilesResponseOutputTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListRulesResponseTypeDef,
+    ListRulesResponseOutputTypeDef,
     ListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
     ListSecurityKeysRequestRequestTypeDef,
-    ListSecurityKeysResponseTypeDef,
+    ListSecurityKeysResponseOutputTypeDef,
     ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
     ListSecurityProfilePermissionsRequestRequestTypeDef,
-    ListSecurityProfilePermissionsResponseTypeDef,
+    ListSecurityProfilePermissionsResponseOutputTypeDef,
     ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
-    ListSecurityProfilesResponseTypeDef,
+    ListSecurityProfilesResponseOutputTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
     ListTaskTemplatesRequestRequestTypeDef,
-    ListTaskTemplatesResponseTypeDef,
+    ListTaskTemplatesResponseOutputTypeDef,
     ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef,
     ListTrafficDistributionGroupsRequestRequestTypeDef,
-    ListTrafficDistributionGroupsResponseTypeDef,
+    ListTrafficDistributionGroupsResponseOutputTypeDef,
     ListUseCasesRequestListUseCasesPaginateTypeDef,
     ListUseCasesRequestRequestTypeDef,
-    ListUseCasesResponseTypeDef,
+    ListUseCasesResponseOutputTypeDef,
     ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
     ListUserHierarchyGroupsRequestRequestTypeDef,
-    ListUserHierarchyGroupsResponseTypeDef,
+    ListUserHierarchyGroupsResponseOutputTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListUsersResponseTypeDef,
+    ListUsersResponseOutputTypeDef,
+    MediaConcurrencyOutputTypeDef,
     MediaConcurrencyTypeDef,
-    MetricDataV2TypeDef,
+    MetricDataV2OutputTypeDef,
+    MetricFilterV2OutputTypeDef,
     MetricFilterV2TypeDef,
-    MetricResultV2TypeDef,
+    MetricResultV2OutputTypeDef,
+    MetricV2OutputTypeDef,
     MetricV2TypeDef,
     MonitorContactRequestRequestTypeDef,
-    MonitorContactResponseTypeDef,
+    MonitorContactResponseOutputTypeDef,
+    NotificationRecipientTypeOutputTypeDef,
     NotificationRecipientTypeTypeDef,
-    NumberReferenceTypeDef,
+    NumberReferenceOutputTypeDef,
+    NumericQuestionPropertyValueAutomationOutputTypeDef,
     NumericQuestionPropertyValueAutomationTypeDef,
+    OutboundCallerConfigOutputTypeDef,
     OutboundCallerConfigTypeDef,
     PaginatorConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     ParticipantTimerConfigurationTypeDef,
     ParticipantTimerValueTypeDef,
-    ParticipantTokenCredentialsTypeDef,
+    ParticipantTokenCredentialsOutputTypeDef,
     PersistentChatTypeDef,
+    PhoneNumberQuickConnectConfigOutputTypeDef,
     PhoneNumberQuickConnectConfigTypeDef,
-    PhoneNumberStatusTypeDef,
-    PhoneNumberSummaryTypeDef,
+    PhoneNumberStatusOutputTypeDef,
+    PhoneNumberSummaryOutputTypeDef,
+    PromptOutputTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
-    PromptSummaryTypeDef,
-    PromptTypeDef,
+    PromptSummaryOutputTypeDef,
     PutUserStatusRequestRequestTypeDef,
-    QueueInfoTypeDef,
+    QueueInfoOutputTypeDef,
+    QueueOutputTypeDef,
+    QueueQuickConnectConfigOutputTypeDef,
     QueueQuickConnectConfigTypeDef,
-    QueueReferenceTypeDef,
+    QueueReferenceOutputTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
-    QueueSummaryTypeDef,
-    QueueTypeDef,
+    QueueSummaryOutputTypeDef,
+    QuickConnectConfigOutputTypeDef,
     QuickConnectConfigTypeDef,
+    QuickConnectOutputTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
-    QuickConnectSummaryTypeDef,
-    QuickConnectTypeDef,
+    QuickConnectSummaryOutputTypeDef,
+    ReadOnlyFieldInfoOutputTypeDef,
     ReadOnlyFieldInfoTypeDef,
-    ReferenceSummaryTypeDef,
+    ReferenceOutputTypeDef,
+    ReferenceSummaryOutputTypeDef,
     ReferenceTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
     ReplicateInstanceRequestRequestTypeDef,
-    ReplicateInstanceResponseTypeDef,
+    ReplicateInstanceResponseOutputTypeDef,
+    RequiredFieldInfoOutputTypeDef,
     RequiredFieldInfoTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     ResponseMetadataTypeDef,
     ResumeContactRecordingRequestRequestTypeDef,
-    RoutingProfileQueueConfigSummaryTypeDef,
+    RoutingProfileOutputTypeDef,
+    RoutingProfileQueueConfigSummaryOutputTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
-    RoutingProfileReferenceTypeDef,
+    RoutingProfileReferenceOutputTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    RoutingProfileSummaryTypeDef,
-    RoutingProfileTypeDef,
+    RoutingProfileSummaryOutputTypeDef,
+    RuleActionOutputTypeDef,
     RuleActionTypeDef,
-    RuleSummaryTypeDef,
+    RuleOutputTypeDef,
+    RuleSummaryOutputTypeDef,
+    RuleTriggerEventSourceOutputTypeDef,
     RuleTriggerEventSourceTypeDef,
-    RuleTypeDef,
+    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseOutputTypeDef,
     SearchHoursOfOperationsRequestRequestTypeDef,
     SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
-    SearchHoursOfOperationsResponseTypeDef,
+    SearchHoursOfOperationsResponseOutputTypeDef,
     SearchPromptsRequestRequestTypeDef,
     SearchPromptsRequestSearchPromptsPaginateTypeDef,
-    SearchPromptsResponseTypeDef,
+    SearchPromptsResponseOutputTypeDef,
     SearchQueuesRequestRequestTypeDef,
     SearchQueuesRequestSearchQueuesPaginateTypeDef,
-    SearchQueuesResponseTypeDef,
+    SearchQueuesResponseOutputTypeDef,
     SearchQuickConnectsRequestRequestTypeDef,
     SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
-    SearchQuickConnectsResponseTypeDef,
+    SearchQuickConnectsResponseOutputTypeDef,
     SearchResourceTagsRequestRequestTypeDef,
     SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
-    SearchResourceTagsResponseTypeDef,
+    SearchResourceTagsResponseOutputTypeDef,
     SearchRoutingProfilesRequestRequestTypeDef,
     SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
-    SearchRoutingProfilesResponseTypeDef,
+    SearchRoutingProfilesResponseOutputTypeDef,
     SearchSecurityProfilesRequestRequestTypeDef,
     SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
-    SearchSecurityProfilesResponseTypeDef,
+    SearchSecurityProfilesResponseOutputTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchUsersRequestSearchUsersPaginateTypeDef,
-    SearchUsersResponseTypeDef,
+    SearchUsersResponseOutputTypeDef,
     SearchVocabulariesRequestRequestTypeDef,
     SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
-    SearchVocabulariesResponseTypeDef,
-    SecurityKeyTypeDef,
+    SearchVocabulariesResponseOutputTypeDef,
+    SecurityKeyOutputTypeDef,
+    SecurityProfileOutputTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
-    SecurityProfileSearchSummaryTypeDef,
-    SecurityProfileSummaryTypeDef,
-    SecurityProfileTypeDef,
+    SecurityProfileSearchSummaryOutputTypeDef,
+    SecurityProfileSummaryOutputTypeDef,
     SecurityProfilesSearchFilterTypeDef,
+    SendNotificationActionDefinitionOutputTypeDef,
     SendNotificationActionDefinitionTypeDef,
+    SingleSelectQuestionRuleCategoryAutomationOutputTypeDef,
     SingleSelectQuestionRuleCategoryAutomationTypeDef,
     StartChatContactRequestRequestTypeDef,
-    StartChatContactResponseTypeDef,
+    StartChatContactResponseOutputTypeDef,
     StartContactEvaluationRequestRequestTypeDef,
-    StartContactEvaluationResponseTypeDef,
+    StartContactEvaluationResponseOutputTypeDef,
     StartContactRecordingRequestRequestTypeDef,
     StartContactStreamingRequestRequestTypeDef,
-    StartContactStreamingResponseTypeDef,
+    StartContactStreamingResponseOutputTypeDef,
     StartOutboundVoiceContactRequestRequestTypeDef,
-    StartOutboundVoiceContactResponseTypeDef,
+    StartOutboundVoiceContactResponseOutputTypeDef,
     StartTaskContactRequestRequestTypeDef,
-    StartTaskContactResponseTypeDef,
+    StartTaskContactResponseOutputTypeDef,
     StopContactRecordingRequestRequestTypeDef,
     StopContactRequestRequestTypeDef,
     StopContactStreamingRequestRequestTypeDef,
     StringConditionTypeDef,
-    StringReferenceTypeDef,
+    StringReferenceOutputTypeDef,
     SubmitContactEvaluationRequestRequestTypeDef,
-    SubmitContactEvaluationResponseTypeDef,
+    SubmitContactEvaluationResponseOutputTypeDef,
     SuspendContactRecordingRequestRequestTypeDef,
     TagConditionTypeDef,
     TagResourceRequestRequestTypeDef,
     TagSearchConditionTypeDef,
-    TagSetTypeDef,
+    TagSetOutputTypeDef,
+    TaskActionDefinitionOutputTypeDef,
     TaskActionDefinitionTypeDef,
+    TaskTemplateConstraintsOutputTypeDef,
     TaskTemplateConstraintsTypeDef,
+    TaskTemplateDefaultFieldValueOutputTypeDef,
     TaskTemplateDefaultFieldValueTypeDef,
+    TaskTemplateDefaultsOutputTypeDef,
     TaskTemplateDefaultsTypeDef,
+    TaskTemplateFieldIdentifierOutputTypeDef,
     TaskTemplateFieldIdentifierTypeDef,
+    TaskTemplateFieldOutputTypeDef,
     TaskTemplateFieldTypeDef,
-    TaskTemplateMetadataTypeDef,
+    TaskTemplateMetadataOutputTypeDef,
+    TelephonyConfigOutputTypeDef,
     TelephonyConfigTypeDef,
+    ThresholdOutputTypeDef,
     ThresholdTypeDef,
+    ThresholdV2OutputTypeDef,
     ThresholdV2TypeDef,
-    TrafficDistributionGroupSummaryTypeDef,
-    TrafficDistributionGroupTypeDef,
+    TrafficDistributionGroupOutputTypeDef,
+    TrafficDistributionGroupSummaryOutputTypeDef,
     TransferContactRequestRequestTypeDef,
-    TransferContactResponseTypeDef,
+    TransferContactResponseOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     UpdateContactAttributesRequestRequestTypeDef,
     UpdateContactEvaluationRequestRequestTypeDef,
-    UpdateContactEvaluationResponseTypeDef,
+    UpdateContactEvaluationResponseOutputTypeDef,
     UpdateContactFlowContentRequestRequestTypeDef,
     UpdateContactFlowMetadataRequestRequestTypeDef,
     UpdateContactFlowModuleContentRequestRequestTypeDef,
     UpdateContactFlowModuleMetadataRequestRequestTypeDef,
     UpdateContactFlowNameRequestRequestTypeDef,
     UpdateContactRequestRequestTypeDef,
     UpdateContactScheduleRequestRequestTypeDef,
     UpdateEvaluationFormRequestRequestTypeDef,
-    UpdateEvaluationFormResponseTypeDef,
+    UpdateEvaluationFormResponseOutputTypeDef,
     UpdateHoursOfOperationRequestRequestTypeDef,
     UpdateInstanceAttributeRequestRequestTypeDef,
     UpdateInstanceStorageConfigRequestRequestTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     UpdateParticipantRoleConfigRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
-    UpdatePhoneNumberResponseTypeDef,
+    UpdatePhoneNumberResponseOutputTypeDef,
     UpdatePromptRequestRequestTypeDef,
-    UpdatePromptResponseTypeDef,
+    UpdatePromptResponseOutputTypeDef,
     UpdateQueueHoursOfOperationRequestRequestTypeDef,
     UpdateQueueMaxContactsRequestRequestTypeDef,
     UpdateQueueNameRequestRequestTypeDef,
     UpdateQueueOutboundCallerConfigRequestRequestTypeDef,
     UpdateQueueStatusRequestRequestTypeDef,
     UpdateQuickConnectConfigRequestRequestTypeDef,
     UpdateQuickConnectNameRequestRequestTypeDef,
     UpdateRoutingProfileConcurrencyRequestRequestTypeDef,
     UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef,
     UpdateRoutingProfileNameRequestRequestTypeDef,
     UpdateRoutingProfileQueuesRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
     UpdateSecurityProfileRequestRequestTypeDef,
     UpdateTaskTemplateRequestRequestTypeDef,
-    UpdateTaskTemplateResponseTypeDef,
+    UpdateTaskTemplateResponseOutputTypeDef,
     UpdateTrafficDistributionRequestRequestTypeDef,
     UpdateUserHierarchyGroupNameRequestRequestTypeDef,
     UpdateUserHierarchyRequestRequestTypeDef,
     UpdateUserHierarchyStructureRequestRequestTypeDef,
     UpdateUserIdentityInfoRequestRequestTypeDef,
     UpdateUserPhoneConfigRequestRequestTypeDef,
     UpdateUserRoutingProfileRequestRequestTypeDef,
     UpdateUserSecurityProfilesRequestRequestTypeDef,
-    UrlReferenceTypeDef,
-    UseCaseTypeDef,
+    UrlReferenceOutputTypeDef,
+    UseCaseOutputTypeDef,
     UserDataFiltersTypeDef,
-    UserDataTypeDef,
-    UserIdentityInfoLiteTypeDef,
+    UserDataOutputTypeDef,
+    UserIdentityInfoLiteOutputTypeDef,
+    UserIdentityInfoOutputTypeDef,
     UserIdentityInfoTypeDef,
+    UserOutputTypeDef,
+    UserPhoneConfigOutputTypeDef,
     UserPhoneConfigTypeDef,
+    UserQuickConnectConfigOutputTypeDef,
     UserQuickConnectConfigTypeDef,
-    UserReferenceTypeDef,
+    UserReferenceOutputTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
-    UserSearchSummaryTypeDef,
-    UserSummaryTypeDef,
-    UserTypeDef,
-    VocabularySummaryTypeDef,
-    VocabularyTypeDef,
+    UserSearchSummaryOutputTypeDef,
+    UserSummaryOutputTypeDef,
+    VocabularyOutputTypeDef,
+    VocabularySummaryOutputTypeDef,
     VoiceRecordingConfigurationTypeDef,
-    WisdomInfoTypeDef,
+    WisdomInfoOutputTypeDef,
 )
 
 
-def get_structure() -> ActionSummaryTypeDef:
+def get_structure() -> ActionSummaryOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connect-1.28.3/README.md` & `mypy-boto3-connect-1.28.3.post1/README.md`

 * *Files 15% similar despite different names*

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
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -546,101 +546,103 @@
 ### Typed dictionaries
 
 `mypy_boto3_connect.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connect.type_defs import (
-    ActionSummaryTypeDef,
+    ActionSummaryOutputTypeDef,
     ActivateEvaluationFormRequestRequestTypeDef,
-    ActivateEvaluationFormResponseTypeDef,
-    AgentContactReferenceTypeDef,
-    AgentInfoTypeDef,
-    AgentStatusReferenceTypeDef,
-    AgentStatusSummaryTypeDef,
-    AgentStatusTypeDef,
+    ActivateEvaluationFormResponseOutputTypeDef,
+    AgentContactReferenceOutputTypeDef,
+    AgentInfoOutputTypeDef,
+    AgentStatusOutputTypeDef,
+    AgentStatusReferenceOutputTypeDef,
+    AgentStatusSummaryOutputTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     AssociateApprovedOriginRequestRequestTypeDef,
     AssociateBotRequestRequestTypeDef,
     AssociateDefaultVocabularyRequestRequestTypeDef,
     AssociateInstanceStorageConfigRequestRequestTypeDef,
-    AssociateInstanceStorageConfigResponseTypeDef,
+    AssociateInstanceStorageConfigResponseOutputTypeDef,
     AssociateLambdaFunctionRequestRequestTypeDef,
     AssociateLexBotRequestRequestTypeDef,
     AssociatePhoneNumberContactFlowRequestRequestTypeDef,
     AssociateQueueQuickConnectsRequestRequestTypeDef,
     AssociateRoutingProfileQueuesRequestRequestTypeDef,
     AssociateSecurityKeyRequestRequestTypeDef,
-    AssociateSecurityKeyResponseTypeDef,
-    AttachmentReferenceTypeDef,
-    AttributeTypeDef,
-    AvailableNumberSummaryTypeDef,
+    AssociateSecurityKeyResponseOutputTypeDef,
+    AttachmentReferenceOutputTypeDef,
+    AttributeOutputTypeDef,
+    AvailableNumberSummaryOutputTypeDef,
     ChatMessageTypeDef,
     ChatParticipantRoleConfigTypeDef,
     ChatStreamingConfigurationTypeDef,
     ClaimPhoneNumberRequestRequestTypeDef,
-    ClaimPhoneNumberResponseTypeDef,
-    ClaimedPhoneNumberSummaryTypeDef,
+    ClaimPhoneNumberResponseOutputTypeDef,
+    ClaimedPhoneNumberSummaryOutputTypeDef,
     ContactFilterTypeDef,
-    ContactFlowModuleSummaryTypeDef,
-    ContactFlowModuleTypeDef,
-    ContactFlowSummaryTypeDef,
-    ContactFlowTypeDef,
-    ContactTypeDef,
+    ContactFlowModuleOutputTypeDef,
+    ContactFlowModuleSummaryOutputTypeDef,
+    ContactFlowOutputTypeDef,
+    ContactFlowSummaryOutputTypeDef,
+    ContactOutputTypeDef,
     ControlPlaneTagFilterTypeDef,
     CreateAgentStatusRequestRequestTypeDef,
-    CreateAgentStatusResponseTypeDef,
+    CreateAgentStatusResponseOutputTypeDef,
     CreateContactFlowModuleRequestRequestTypeDef,
-    CreateContactFlowModuleResponseTypeDef,
+    CreateContactFlowModuleResponseOutputTypeDef,
     CreateContactFlowRequestRequestTypeDef,
-    CreateContactFlowResponseTypeDef,
+    CreateContactFlowResponseOutputTypeDef,
     CreateEvaluationFormRequestRequestTypeDef,
-    CreateEvaluationFormResponseTypeDef,
+    CreateEvaluationFormResponseOutputTypeDef,
     CreateHoursOfOperationRequestRequestTypeDef,
-    CreateHoursOfOperationResponseTypeDef,
+    CreateHoursOfOperationResponseOutputTypeDef,
     CreateInstanceRequestRequestTypeDef,
-    CreateInstanceResponseTypeDef,
+    CreateInstanceResponseOutputTypeDef,
     CreateIntegrationAssociationRequestRequestTypeDef,
-    CreateIntegrationAssociationResponseTypeDef,
+    CreateIntegrationAssociationResponseOutputTypeDef,
     CreateParticipantRequestRequestTypeDef,
-    CreateParticipantResponseTypeDef,
+    CreateParticipantResponseOutputTypeDef,
     CreatePromptRequestRequestTypeDef,
-    CreatePromptResponseTypeDef,
+    CreatePromptResponseOutputTypeDef,
     CreateQueueRequestRequestTypeDef,
-    CreateQueueResponseTypeDef,
+    CreateQueueResponseOutputTypeDef,
     CreateQuickConnectRequestRequestTypeDef,
-    CreateQuickConnectResponseTypeDef,
+    CreateQuickConnectResponseOutputTypeDef,
     CreateRoutingProfileRequestRequestTypeDef,
-    CreateRoutingProfileResponseTypeDef,
+    CreateRoutingProfileResponseOutputTypeDef,
     CreateRuleRequestRequestTypeDef,
-    CreateRuleResponseTypeDef,
+    CreateRuleResponseOutputTypeDef,
     CreateSecurityProfileRequestRequestTypeDef,
-    CreateSecurityProfileResponseTypeDef,
+    CreateSecurityProfileResponseOutputTypeDef,
     CreateTaskTemplateRequestRequestTypeDef,
-    CreateTaskTemplateResponseTypeDef,
+    CreateTaskTemplateResponseOutputTypeDef,
     CreateTrafficDistributionGroupRequestRequestTypeDef,
-    CreateTrafficDistributionGroupResponseTypeDef,
+    CreateTrafficDistributionGroupResponseOutputTypeDef,
     CreateUseCaseRequestRequestTypeDef,
-    CreateUseCaseResponseTypeDef,
+    CreateUseCaseResponseOutputTypeDef,
     CreateUserHierarchyGroupRequestRequestTypeDef,
-    CreateUserHierarchyGroupResponseTypeDef,
+    CreateUserHierarchyGroupResponseOutputTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseTypeDef,
+    CreateUserResponseOutputTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    CreateVocabularyResponseTypeDef,
-    CredentialsTypeDef,
+    CreateVocabularyResponseOutputTypeDef,
+    CredentialsOutputTypeDef,
+    CrossChannelBehaviorOutputTypeDef,
     CrossChannelBehaviorTypeDef,
-    CurrentMetricDataTypeDef,
-    CurrentMetricResultTypeDef,
+    CurrentMetricDataOutputTypeDef,
+    CurrentMetricOutputTypeDef,
+    CurrentMetricResultOutputTypeDef,
     CurrentMetricSortCriteriaTypeDef,
     CurrentMetricTypeDef,
-    DateReferenceTypeDef,
+    DateReferenceOutputTypeDef,
     DeactivateEvaluationFormRequestRequestTypeDef,
-    DeactivateEvaluationFormResponseTypeDef,
-    DefaultVocabularyTypeDef,
+    DeactivateEvaluationFormResponseOutputTypeDef,
+    DefaultVocabularyOutputTypeDef,
     DeleteContactEvaluationRequestRequestTypeDef,
     DeleteContactFlowModuleRequestRequestTypeDef,
     DeleteContactFlowRequestRequestTypeDef,
     DeleteEvaluationFormRequestRequestTypeDef,
     DeleteHoursOfOperationRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteIntegrationAssociationRequestRequestTypeDef,
@@ -652,460 +654,516 @@
     DeleteSecurityProfileRequestRequestTypeDef,
     DeleteTaskTemplateRequestRequestTypeDef,
     DeleteTrafficDistributionGroupRequestRequestTypeDef,
     DeleteUseCaseRequestRequestTypeDef,
     DeleteUserHierarchyGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
-    DeleteVocabularyResponseTypeDef,
+    DeleteVocabularyResponseOutputTypeDef,
     DescribeAgentStatusRequestRequestTypeDef,
-    DescribeAgentStatusResponseTypeDef,
+    DescribeAgentStatusResponseOutputTypeDef,
     DescribeContactEvaluationRequestRequestTypeDef,
-    DescribeContactEvaluationResponseTypeDef,
+    DescribeContactEvaluationResponseOutputTypeDef,
     DescribeContactFlowModuleRequestRequestTypeDef,
-    DescribeContactFlowModuleResponseTypeDef,
+    DescribeContactFlowModuleResponseOutputTypeDef,
     DescribeContactFlowRequestRequestTypeDef,
-    DescribeContactFlowResponseTypeDef,
+    DescribeContactFlowResponseOutputTypeDef,
     DescribeContactRequestRequestTypeDef,
-    DescribeContactResponseTypeDef,
+    DescribeContactResponseOutputTypeDef,
     DescribeEvaluationFormRequestRequestTypeDef,
-    DescribeEvaluationFormResponseTypeDef,
+    DescribeEvaluationFormResponseOutputTypeDef,
     DescribeHoursOfOperationRequestRequestTypeDef,
-    DescribeHoursOfOperationResponseTypeDef,
+    DescribeHoursOfOperationResponseOutputTypeDef,
     DescribeInstanceAttributeRequestRequestTypeDef,
-    DescribeInstanceAttributeResponseTypeDef,
+    DescribeInstanceAttributeResponseOutputTypeDef,
     DescribeInstanceRequestRequestTypeDef,
-    DescribeInstanceResponseTypeDef,
+    DescribeInstanceResponseOutputTypeDef,
     DescribeInstanceStorageConfigRequestRequestTypeDef,
-    DescribeInstanceStorageConfigResponseTypeDef,
+    DescribeInstanceStorageConfigResponseOutputTypeDef,
     DescribePhoneNumberRequestRequestTypeDef,
-    DescribePhoneNumberResponseTypeDef,
+    DescribePhoneNumberResponseOutputTypeDef,
     DescribePromptRequestRequestTypeDef,
-    DescribePromptResponseTypeDef,
+    DescribePromptResponseOutputTypeDef,
     DescribeQueueRequestRequestTypeDef,
-    DescribeQueueResponseTypeDef,
+    DescribeQueueResponseOutputTypeDef,
     DescribeQuickConnectRequestRequestTypeDef,
-    DescribeQuickConnectResponseTypeDef,
+    DescribeQuickConnectResponseOutputTypeDef,
     DescribeRoutingProfileRequestRequestTypeDef,
-    DescribeRoutingProfileResponseTypeDef,
+    DescribeRoutingProfileResponseOutputTypeDef,
     DescribeRuleRequestRequestTypeDef,
-    DescribeRuleResponseTypeDef,
+    DescribeRuleResponseOutputTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
-    DescribeSecurityProfileResponseTypeDef,
+    DescribeSecurityProfileResponseOutputTypeDef,
     DescribeTrafficDistributionGroupRequestRequestTypeDef,
-    DescribeTrafficDistributionGroupResponseTypeDef,
+    DescribeTrafficDistributionGroupResponseOutputTypeDef,
     DescribeUserHierarchyGroupRequestRequestTypeDef,
-    DescribeUserHierarchyGroupResponseTypeDef,
+    DescribeUserHierarchyGroupResponseOutputTypeDef,
     DescribeUserHierarchyStructureRequestRequestTypeDef,
-    DescribeUserHierarchyStructureResponseTypeDef,
+    DescribeUserHierarchyStructureResponseOutputTypeDef,
     DescribeUserRequestRequestTypeDef,
-    DescribeUserResponseTypeDef,
+    DescribeUserResponseOutputTypeDef,
     DescribeVocabularyRequestRequestTypeDef,
-    DescribeVocabularyResponseTypeDef,
-    DimensionsTypeDef,
+    DescribeVocabularyResponseOutputTypeDef,
+    DimensionsOutputTypeDef,
     DisassociateApprovedOriginRequestRequestTypeDef,
     DisassociateBotRequestRequestTypeDef,
     DisassociateInstanceStorageConfigRequestRequestTypeDef,
     DisassociateLambdaFunctionRequestRequestTypeDef,
     DisassociateLexBotRequestRequestTypeDef,
     DisassociatePhoneNumberContactFlowRequestRequestTypeDef,
     DisassociateQueueQuickConnectsRequestRequestTypeDef,
     DisassociateRoutingProfileQueuesRequestRequestTypeDef,
     DisassociateSecurityKeyRequestRequestTypeDef,
     DismissUserContactRequestRequestTypeDef,
+    DistributionOutputTypeDef,
     DistributionTypeDef,
-    EmailReferenceTypeDef,
+    EmailReferenceOutputTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    EvaluationAnswerDataOutputTypeDef,
     EvaluationAnswerDataTypeDef,
     EvaluationAnswerInputTypeDef,
-    EvaluationAnswerOutputTypeDef,
-    EvaluationFormContentTypeDef,
+    EvaluationAnswerOutputOutputTypeDef,
+    EvaluationFormContentOutputTypeDef,
+    EvaluationFormItemOutputTypeDef,
     EvaluationFormItemTypeDef,
+    EvaluationFormNumericQuestionAutomationOutputTypeDef,
     EvaluationFormNumericQuestionAutomationTypeDef,
+    EvaluationFormNumericQuestionOptionOutputTypeDef,
     EvaluationFormNumericQuestionOptionTypeDef,
+    EvaluationFormNumericQuestionPropertiesOutputTypeDef,
     EvaluationFormNumericQuestionPropertiesTypeDef,
+    EvaluationFormOutputTypeDef,
+    EvaluationFormQuestionOutputTypeDef,
     EvaluationFormQuestionTypeDef,
+    EvaluationFormQuestionTypePropertiesOutputTypeDef,
     EvaluationFormQuestionTypePropertiesTypeDef,
+    EvaluationFormScoringStrategyOutputTypeDef,
     EvaluationFormScoringStrategyTypeDef,
+    EvaluationFormSectionOutputTypeDef,
     EvaluationFormSectionTypeDef,
+    EvaluationFormSingleSelectQuestionAutomationOptionOutputTypeDef,
     EvaluationFormSingleSelectQuestionAutomationOptionTypeDef,
+    EvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
     EvaluationFormSingleSelectQuestionAutomationTypeDef,
+    EvaluationFormSingleSelectQuestionOptionOutputTypeDef,
     EvaluationFormSingleSelectQuestionOptionTypeDef,
+    EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
     EvaluationFormSingleSelectQuestionPropertiesTypeDef,
-    EvaluationFormSummaryTypeDef,
-    EvaluationFormTypeDef,
-    EvaluationFormVersionSummaryTypeDef,
-    EvaluationMetadataTypeDef,
+    EvaluationFormSummaryOutputTypeDef,
+    EvaluationFormVersionSummaryOutputTypeDef,
+    EvaluationMetadataOutputTypeDef,
+    EvaluationNoteOutputTypeDef,
     EvaluationNoteTypeDef,
-    EvaluationScoreTypeDef,
-    EvaluationSummaryTypeDef,
-    EvaluationTypeDef,
+    EvaluationOutputTypeDef,
+    EvaluationScoreOutputTypeDef,
+    EvaluationSummaryOutputTypeDef,
+    EventBridgeActionDefinitionOutputTypeDef,
     EventBridgeActionDefinitionTypeDef,
     FilterV2TypeDef,
     FiltersTypeDef,
     GetContactAttributesRequestRequestTypeDef,
-    GetContactAttributesResponseTypeDef,
+    GetContactAttributesResponseOutputTypeDef,
     GetCurrentMetricDataRequestRequestTypeDef,
-    GetCurrentMetricDataResponseTypeDef,
+    GetCurrentMetricDataResponseOutputTypeDef,
     GetCurrentUserDataRequestRequestTypeDef,
-    GetCurrentUserDataResponseTypeDef,
+    GetCurrentUserDataResponseOutputTypeDef,
     GetFederationTokenRequestRequestTypeDef,
-    GetFederationTokenResponseTypeDef,
+    GetFederationTokenResponseOutputTypeDef,
     GetMetricDataRequestGetMetricDataPaginateTypeDef,
     GetMetricDataRequestRequestTypeDef,
-    GetMetricDataResponseTypeDef,
+    GetMetricDataResponseOutputTypeDef,
     GetMetricDataV2RequestRequestTypeDef,
-    GetMetricDataV2ResponseTypeDef,
+    GetMetricDataV2ResponseOutputTypeDef,
     GetPromptFileRequestRequestTypeDef,
-    GetPromptFileResponseTypeDef,
+    GetPromptFileResponseOutputTypeDef,
     GetTaskTemplateRequestRequestTypeDef,
-    GetTaskTemplateResponseTypeDef,
+    GetTaskTemplateResponseOutputTypeDef,
     GetTrafficDistributionRequestRequestTypeDef,
-    GetTrafficDistributionResponseTypeDef,
+    GetTrafficDistributionResponseOutputTypeDef,
     HierarchyGroupConditionTypeDef,
-    HierarchyGroupSummaryReferenceTypeDef,
-    HierarchyGroupSummaryTypeDef,
-    HierarchyGroupTypeDef,
-    HierarchyLevelTypeDef,
+    HierarchyGroupOutputTypeDef,
+    HierarchyGroupSummaryOutputTypeDef,
+    HierarchyGroupSummaryReferenceOutputTypeDef,
+    HierarchyLevelOutputTypeDef,
     HierarchyLevelUpdateTypeDef,
-    HierarchyPathReferenceTypeDef,
-    HierarchyPathTypeDef,
-    HierarchyStructureTypeDef,
+    HierarchyPathOutputTypeDef,
+    HierarchyPathReferenceOutputTypeDef,
+    HierarchyStructureOutputTypeDef,
     HierarchyStructureUpdateTypeDef,
-    HistoricalMetricDataTypeDef,
-    HistoricalMetricResultTypeDef,
+    HistoricalMetricDataOutputTypeDef,
+    HistoricalMetricOutputTypeDef,
+    HistoricalMetricResultOutputTypeDef,
     HistoricalMetricTypeDef,
+    HoursOfOperationConfigOutputTypeDef,
     HoursOfOperationConfigTypeDef,
+    HoursOfOperationOutputTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
-    HoursOfOperationSummaryTypeDef,
+    HoursOfOperationSummaryOutputTypeDef,
+    HoursOfOperationTimeSliceOutputTypeDef,
     HoursOfOperationTimeSliceTypeDef,
-    HoursOfOperationTypeDef,
-    InstanceStatusReasonTypeDef,
+    InstanceOutputTypeDef,
+    InstanceStatusReasonOutputTypeDef,
+    InstanceStorageConfigOutputTypeDef,
     InstanceStorageConfigTypeDef,
-    InstanceSummaryTypeDef,
-    InstanceTypeDef,
-    IntegrationAssociationSummaryTypeDef,
+    InstanceSummaryOutputTypeDef,
+    IntegrationAssociationSummaryOutputTypeDef,
+    InvisibleFieldInfoOutputTypeDef,
     InvisibleFieldInfoTypeDef,
+    KinesisFirehoseConfigOutputTypeDef,
     KinesisFirehoseConfigTypeDef,
+    KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
+    KinesisVideoStreamConfigOutputTypeDef,
     KinesisVideoStreamConfigTypeDef,
-    LexBotConfigTypeDef,
+    LexBotConfigOutputTypeDef,
+    LexBotOutputTypeDef,
     LexBotTypeDef,
+    LexV2BotOutputTypeDef,
     LexV2BotTypeDef,
     ListAgentStatusRequestListAgentStatusesPaginateTypeDef,
     ListAgentStatusRequestRequestTypeDef,
-    ListAgentStatusResponseTypeDef,
+    ListAgentStatusResponseOutputTypeDef,
     ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
     ListApprovedOriginsRequestRequestTypeDef,
-    ListApprovedOriginsResponseTypeDef,
+    ListApprovedOriginsResponseOutputTypeDef,
     ListBotsRequestListBotsPaginateTypeDef,
     ListBotsRequestRequestTypeDef,
-    ListBotsResponseTypeDef,
+    ListBotsResponseOutputTypeDef,
     ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
     ListContactEvaluationsRequestRequestTypeDef,
-    ListContactEvaluationsResponseTypeDef,
+    ListContactEvaluationsResponseOutputTypeDef,
     ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
     ListContactFlowModulesRequestRequestTypeDef,
-    ListContactFlowModulesResponseTypeDef,
+    ListContactFlowModulesResponseOutputTypeDef,
     ListContactFlowsRequestListContactFlowsPaginateTypeDef,
     ListContactFlowsRequestRequestTypeDef,
-    ListContactFlowsResponseTypeDef,
+    ListContactFlowsResponseOutputTypeDef,
     ListContactReferencesRequestListContactReferencesPaginateTypeDef,
     ListContactReferencesRequestRequestTypeDef,
-    ListContactReferencesResponseTypeDef,
+    ListContactReferencesResponseOutputTypeDef,
     ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
     ListDefaultVocabulariesRequestRequestTypeDef,
-    ListDefaultVocabulariesResponseTypeDef,
+    ListDefaultVocabulariesResponseOutputTypeDef,
     ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
     ListEvaluationFormVersionsRequestRequestTypeDef,
-    ListEvaluationFormVersionsResponseTypeDef,
+    ListEvaluationFormVersionsResponseOutputTypeDef,
     ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
     ListEvaluationFormsRequestRequestTypeDef,
-    ListEvaluationFormsResponseTypeDef,
+    ListEvaluationFormsResponseOutputTypeDef,
     ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
     ListHoursOfOperationsRequestRequestTypeDef,
-    ListHoursOfOperationsResponseTypeDef,
+    ListHoursOfOperationsResponseOutputTypeDef,
     ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
     ListInstanceAttributesRequestRequestTypeDef,
-    ListInstanceAttributesResponseTypeDef,
+    ListInstanceAttributesResponseOutputTypeDef,
     ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
     ListInstanceStorageConfigsRequestRequestTypeDef,
-    ListInstanceStorageConfigsResponseTypeDef,
+    ListInstanceStorageConfigsResponseOutputTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
-    ListInstancesResponseTypeDef,
+    ListInstancesResponseOutputTypeDef,
     ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
     ListIntegrationAssociationsRequestRequestTypeDef,
-    ListIntegrationAssociationsResponseTypeDef,
+    ListIntegrationAssociationsResponseOutputTypeDef,
     ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
     ListLambdaFunctionsRequestRequestTypeDef,
-    ListLambdaFunctionsResponseTypeDef,
+    ListLambdaFunctionsResponseOutputTypeDef,
     ListLexBotsRequestListLexBotsPaginateTypeDef,
     ListLexBotsRequestRequestTypeDef,
-    ListLexBotsResponseTypeDef,
+    ListLexBotsResponseOutputTypeDef,
     ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
-    ListPhoneNumbersResponseTypeDef,
-    ListPhoneNumbersSummaryTypeDef,
+    ListPhoneNumbersResponseOutputTypeDef,
+    ListPhoneNumbersSummaryOutputTypeDef,
     ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef,
     ListPhoneNumbersV2RequestRequestTypeDef,
-    ListPhoneNumbersV2ResponseTypeDef,
+    ListPhoneNumbersV2ResponseOutputTypeDef,
     ListPromptsRequestListPromptsPaginateTypeDef,
     ListPromptsRequestRequestTypeDef,
-    ListPromptsResponseTypeDef,
+    ListPromptsResponseOutputTypeDef,
     ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
     ListQueueQuickConnectsRequestRequestTypeDef,
-    ListQueueQuickConnectsResponseTypeDef,
+    ListQueueQuickConnectsResponseOutputTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResponseTypeDef,
+    ListQueuesResponseOutputTypeDef,
     ListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
     ListQuickConnectsRequestRequestTypeDef,
-    ListQuickConnectsResponseTypeDef,
+    ListQuickConnectsResponseOutputTypeDef,
     ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
     ListRoutingProfileQueuesRequestRequestTypeDef,
-    ListRoutingProfileQueuesResponseTypeDef,
+    ListRoutingProfileQueuesResponseOutputTypeDef,
     ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
     ListRoutingProfilesRequestRequestTypeDef,
-    ListRoutingProfilesResponseTypeDef,
+    ListRoutingProfilesResponseOutputTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListRulesResponseTypeDef,
+    ListRulesResponseOutputTypeDef,
     ListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
     ListSecurityKeysRequestRequestTypeDef,
-    ListSecurityKeysResponseTypeDef,
+    ListSecurityKeysResponseOutputTypeDef,
     ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
     ListSecurityProfilePermissionsRequestRequestTypeDef,
-    ListSecurityProfilePermissionsResponseTypeDef,
+    ListSecurityProfilePermissionsResponseOutputTypeDef,
     ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
-    ListSecurityProfilesResponseTypeDef,
+    ListSecurityProfilesResponseOutputTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
     ListTaskTemplatesRequestRequestTypeDef,
-    ListTaskTemplatesResponseTypeDef,
+    ListTaskTemplatesResponseOutputTypeDef,
     ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef,
     ListTrafficDistributionGroupsRequestRequestTypeDef,
-    ListTrafficDistributionGroupsResponseTypeDef,
+    ListTrafficDistributionGroupsResponseOutputTypeDef,
     ListUseCasesRequestListUseCasesPaginateTypeDef,
     ListUseCasesRequestRequestTypeDef,
-    ListUseCasesResponseTypeDef,
+    ListUseCasesResponseOutputTypeDef,
     ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
     ListUserHierarchyGroupsRequestRequestTypeDef,
-    ListUserHierarchyGroupsResponseTypeDef,
+    ListUserHierarchyGroupsResponseOutputTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListUsersResponseTypeDef,
+    ListUsersResponseOutputTypeDef,
+    MediaConcurrencyOutputTypeDef,
     MediaConcurrencyTypeDef,
-    MetricDataV2TypeDef,
+    MetricDataV2OutputTypeDef,
+    MetricFilterV2OutputTypeDef,
     MetricFilterV2TypeDef,
-    MetricResultV2TypeDef,
+    MetricResultV2OutputTypeDef,
+    MetricV2OutputTypeDef,
     MetricV2TypeDef,
     MonitorContactRequestRequestTypeDef,
-    MonitorContactResponseTypeDef,
+    MonitorContactResponseOutputTypeDef,
+    NotificationRecipientTypeOutputTypeDef,
     NotificationRecipientTypeTypeDef,
-    NumberReferenceTypeDef,
+    NumberReferenceOutputTypeDef,
+    NumericQuestionPropertyValueAutomationOutputTypeDef,
     NumericQuestionPropertyValueAutomationTypeDef,
+    OutboundCallerConfigOutputTypeDef,
     OutboundCallerConfigTypeDef,
     PaginatorConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     ParticipantTimerConfigurationTypeDef,
     ParticipantTimerValueTypeDef,
-    ParticipantTokenCredentialsTypeDef,
+    ParticipantTokenCredentialsOutputTypeDef,
     PersistentChatTypeDef,
+    PhoneNumberQuickConnectConfigOutputTypeDef,
     PhoneNumberQuickConnectConfigTypeDef,
-    PhoneNumberStatusTypeDef,
-    PhoneNumberSummaryTypeDef,
+    PhoneNumberStatusOutputTypeDef,
+    PhoneNumberSummaryOutputTypeDef,
+    PromptOutputTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
-    PromptSummaryTypeDef,
-    PromptTypeDef,
+    PromptSummaryOutputTypeDef,
     PutUserStatusRequestRequestTypeDef,
-    QueueInfoTypeDef,
+    QueueInfoOutputTypeDef,
+    QueueOutputTypeDef,
+    QueueQuickConnectConfigOutputTypeDef,
     QueueQuickConnectConfigTypeDef,
-    QueueReferenceTypeDef,
+    QueueReferenceOutputTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
-    QueueSummaryTypeDef,
-    QueueTypeDef,
+    QueueSummaryOutputTypeDef,
+    QuickConnectConfigOutputTypeDef,
     QuickConnectConfigTypeDef,
+    QuickConnectOutputTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
-    QuickConnectSummaryTypeDef,
-    QuickConnectTypeDef,
+    QuickConnectSummaryOutputTypeDef,
+    ReadOnlyFieldInfoOutputTypeDef,
     ReadOnlyFieldInfoTypeDef,
-    ReferenceSummaryTypeDef,
+    ReferenceOutputTypeDef,
+    ReferenceSummaryOutputTypeDef,
     ReferenceTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
     ReplicateInstanceRequestRequestTypeDef,
-    ReplicateInstanceResponseTypeDef,
+    ReplicateInstanceResponseOutputTypeDef,
+    RequiredFieldInfoOutputTypeDef,
     RequiredFieldInfoTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     ResponseMetadataTypeDef,
     ResumeContactRecordingRequestRequestTypeDef,
-    RoutingProfileQueueConfigSummaryTypeDef,
+    RoutingProfileOutputTypeDef,
+    RoutingProfileQueueConfigSummaryOutputTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
-    RoutingProfileReferenceTypeDef,
+    RoutingProfileReferenceOutputTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    RoutingProfileSummaryTypeDef,
-    RoutingProfileTypeDef,
+    RoutingProfileSummaryOutputTypeDef,
+    RuleActionOutputTypeDef,
     RuleActionTypeDef,
-    RuleSummaryTypeDef,
+    RuleOutputTypeDef,
+    RuleSummaryOutputTypeDef,
+    RuleTriggerEventSourceOutputTypeDef,
     RuleTriggerEventSourceTypeDef,
-    RuleTypeDef,
+    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseOutputTypeDef,
     SearchHoursOfOperationsRequestRequestTypeDef,
     SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
-    SearchHoursOfOperationsResponseTypeDef,
+    SearchHoursOfOperationsResponseOutputTypeDef,
     SearchPromptsRequestRequestTypeDef,
     SearchPromptsRequestSearchPromptsPaginateTypeDef,
-    SearchPromptsResponseTypeDef,
+    SearchPromptsResponseOutputTypeDef,
     SearchQueuesRequestRequestTypeDef,
     SearchQueuesRequestSearchQueuesPaginateTypeDef,
-    SearchQueuesResponseTypeDef,
+    SearchQueuesResponseOutputTypeDef,
     SearchQuickConnectsRequestRequestTypeDef,
     SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
-    SearchQuickConnectsResponseTypeDef,
+    SearchQuickConnectsResponseOutputTypeDef,
     SearchResourceTagsRequestRequestTypeDef,
     SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
-    SearchResourceTagsResponseTypeDef,
+    SearchResourceTagsResponseOutputTypeDef,
     SearchRoutingProfilesRequestRequestTypeDef,
     SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
-    SearchRoutingProfilesResponseTypeDef,
+    SearchRoutingProfilesResponseOutputTypeDef,
     SearchSecurityProfilesRequestRequestTypeDef,
     SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
-    SearchSecurityProfilesResponseTypeDef,
+    SearchSecurityProfilesResponseOutputTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchUsersRequestSearchUsersPaginateTypeDef,
-    SearchUsersResponseTypeDef,
+    SearchUsersResponseOutputTypeDef,
     SearchVocabulariesRequestRequestTypeDef,
     SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
-    SearchVocabulariesResponseTypeDef,
-    SecurityKeyTypeDef,
+    SearchVocabulariesResponseOutputTypeDef,
+    SecurityKeyOutputTypeDef,
+    SecurityProfileOutputTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
-    SecurityProfileSearchSummaryTypeDef,
-    SecurityProfileSummaryTypeDef,
-    SecurityProfileTypeDef,
+    SecurityProfileSearchSummaryOutputTypeDef,
+    SecurityProfileSummaryOutputTypeDef,
     SecurityProfilesSearchFilterTypeDef,
+    SendNotificationActionDefinitionOutputTypeDef,
     SendNotificationActionDefinitionTypeDef,
+    SingleSelectQuestionRuleCategoryAutomationOutputTypeDef,
     SingleSelectQuestionRuleCategoryAutomationTypeDef,
     StartChatContactRequestRequestTypeDef,
-    StartChatContactResponseTypeDef,
+    StartChatContactResponseOutputTypeDef,
     StartContactEvaluationRequestRequestTypeDef,
-    StartContactEvaluationResponseTypeDef,
+    StartContactEvaluationResponseOutputTypeDef,
     StartContactRecordingRequestRequestTypeDef,
     StartContactStreamingRequestRequestTypeDef,
-    StartContactStreamingResponseTypeDef,
+    StartContactStreamingResponseOutputTypeDef,
     StartOutboundVoiceContactRequestRequestTypeDef,
-    StartOutboundVoiceContactResponseTypeDef,
+    StartOutboundVoiceContactResponseOutputTypeDef,
     StartTaskContactRequestRequestTypeDef,
-    StartTaskContactResponseTypeDef,
+    StartTaskContactResponseOutputTypeDef,
     StopContactRecordingRequestRequestTypeDef,
     StopContactRequestRequestTypeDef,
     StopContactStreamingRequestRequestTypeDef,
     StringConditionTypeDef,
-    StringReferenceTypeDef,
+    StringReferenceOutputTypeDef,
     SubmitContactEvaluationRequestRequestTypeDef,
-    SubmitContactEvaluationResponseTypeDef,
+    SubmitContactEvaluationResponseOutputTypeDef,
     SuspendContactRecordingRequestRequestTypeDef,
     TagConditionTypeDef,
     TagResourceRequestRequestTypeDef,
     TagSearchConditionTypeDef,
-    TagSetTypeDef,
+    TagSetOutputTypeDef,
+    TaskActionDefinitionOutputTypeDef,
     TaskActionDefinitionTypeDef,
+    TaskTemplateConstraintsOutputTypeDef,
     TaskTemplateConstraintsTypeDef,
+    TaskTemplateDefaultFieldValueOutputTypeDef,
     TaskTemplateDefaultFieldValueTypeDef,
+    TaskTemplateDefaultsOutputTypeDef,
     TaskTemplateDefaultsTypeDef,
+    TaskTemplateFieldIdentifierOutputTypeDef,
     TaskTemplateFieldIdentifierTypeDef,
+    TaskTemplateFieldOutputTypeDef,
     TaskTemplateFieldTypeDef,
-    TaskTemplateMetadataTypeDef,
+    TaskTemplateMetadataOutputTypeDef,
+    TelephonyConfigOutputTypeDef,
     TelephonyConfigTypeDef,
+    ThresholdOutputTypeDef,
     ThresholdTypeDef,
+    ThresholdV2OutputTypeDef,
     ThresholdV2TypeDef,
-    TrafficDistributionGroupSummaryTypeDef,
-    TrafficDistributionGroupTypeDef,
+    TrafficDistributionGroupOutputTypeDef,
+    TrafficDistributionGroupSummaryOutputTypeDef,
     TransferContactRequestRequestTypeDef,
-    TransferContactResponseTypeDef,
+    TransferContactResponseOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     UpdateContactAttributesRequestRequestTypeDef,
     UpdateContactEvaluationRequestRequestTypeDef,
-    UpdateContactEvaluationResponseTypeDef,
+    UpdateContactEvaluationResponseOutputTypeDef,
     UpdateContactFlowContentRequestRequestTypeDef,
     UpdateContactFlowMetadataRequestRequestTypeDef,
     UpdateContactFlowModuleContentRequestRequestTypeDef,
     UpdateContactFlowModuleMetadataRequestRequestTypeDef,
     UpdateContactFlowNameRequestRequestTypeDef,
     UpdateContactRequestRequestTypeDef,
     UpdateContactScheduleRequestRequestTypeDef,
     UpdateEvaluationFormRequestRequestTypeDef,
-    UpdateEvaluationFormResponseTypeDef,
+    UpdateEvaluationFormResponseOutputTypeDef,
     UpdateHoursOfOperationRequestRequestTypeDef,
     UpdateInstanceAttributeRequestRequestTypeDef,
     UpdateInstanceStorageConfigRequestRequestTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     UpdateParticipantRoleConfigRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
-    UpdatePhoneNumberResponseTypeDef,
+    UpdatePhoneNumberResponseOutputTypeDef,
     UpdatePromptRequestRequestTypeDef,
-    UpdatePromptResponseTypeDef,
+    UpdatePromptResponseOutputTypeDef,
     UpdateQueueHoursOfOperationRequestRequestTypeDef,
     UpdateQueueMaxContactsRequestRequestTypeDef,
     UpdateQueueNameRequestRequestTypeDef,
     UpdateQueueOutboundCallerConfigRequestRequestTypeDef,
     UpdateQueueStatusRequestRequestTypeDef,
     UpdateQuickConnectConfigRequestRequestTypeDef,
     UpdateQuickConnectNameRequestRequestTypeDef,
     UpdateRoutingProfileConcurrencyRequestRequestTypeDef,
     UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef,
     UpdateRoutingProfileNameRequestRequestTypeDef,
     UpdateRoutingProfileQueuesRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
     UpdateSecurityProfileRequestRequestTypeDef,
     UpdateTaskTemplateRequestRequestTypeDef,
-    UpdateTaskTemplateResponseTypeDef,
+    UpdateTaskTemplateResponseOutputTypeDef,
     UpdateTrafficDistributionRequestRequestTypeDef,
     UpdateUserHierarchyGroupNameRequestRequestTypeDef,
     UpdateUserHierarchyRequestRequestTypeDef,
     UpdateUserHierarchyStructureRequestRequestTypeDef,
     UpdateUserIdentityInfoRequestRequestTypeDef,
     UpdateUserPhoneConfigRequestRequestTypeDef,
     UpdateUserRoutingProfileRequestRequestTypeDef,
     UpdateUserSecurityProfilesRequestRequestTypeDef,
-    UrlReferenceTypeDef,
-    UseCaseTypeDef,
+    UrlReferenceOutputTypeDef,
+    UseCaseOutputTypeDef,
     UserDataFiltersTypeDef,
-    UserDataTypeDef,
-    UserIdentityInfoLiteTypeDef,
+    UserDataOutputTypeDef,
+    UserIdentityInfoLiteOutputTypeDef,
+    UserIdentityInfoOutputTypeDef,
     UserIdentityInfoTypeDef,
+    UserOutputTypeDef,
+    UserPhoneConfigOutputTypeDef,
     UserPhoneConfigTypeDef,
+    UserQuickConnectConfigOutputTypeDef,
     UserQuickConnectConfigTypeDef,
-    UserReferenceTypeDef,
+    UserReferenceOutputTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
-    UserSearchSummaryTypeDef,
-    UserSummaryTypeDef,
-    UserTypeDef,
-    VocabularySummaryTypeDef,
-    VocabularyTypeDef,
+    UserSearchSummaryOutputTypeDef,
+    UserSummaryOutputTypeDef,
+    VocabularyOutputTypeDef,
+    VocabularySummaryOutputTypeDef,
     VoiceRecordingConfigurationTypeDef,
-    WisdomInfoTypeDef,
+    WisdomInfoOutputTypeDef,
 )
 
 
-def get_structure() -> ActionSummaryTypeDef:
+def get_structure() -> ActionSummaryOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect/__init__.py` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect/__init__.pyi` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect/__main__.py` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Connect 1.28.3\nVersion:         1.28.3\nBuilder version:"
-        " 7.14.6\nDocs:           "
+        "Type annotations for boto3.Connect 1.28.3\nVersion:         1.28.3.post1\nBuilder version:"
+        " 7.14.7\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\nOther"
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

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect/client.py` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,178 +91,178 @@
     SearchResourceTagsPaginator,
     SearchRoutingProfilesPaginator,
     SearchSecurityProfilesPaginator,
     SearchUsersPaginator,
     SearchVocabulariesPaginator,
 )
 from .type_defs import (
-    ActivateEvaluationFormResponseTypeDef,
+    ActivateEvaluationFormResponseOutputTypeDef,
     AnswerMachineDetectionConfigTypeDef,
-    AssociateInstanceStorageConfigResponseTypeDef,
-    AssociateSecurityKeyResponseTypeDef,
+    AssociateInstanceStorageConfigResponseOutputTypeDef,
+    AssociateSecurityKeyResponseOutputTypeDef,
     ChatMessageTypeDef,
     ChatStreamingConfigurationTypeDef,
-    ClaimPhoneNumberResponseTypeDef,
-    CreateAgentStatusResponseTypeDef,
-    CreateContactFlowModuleResponseTypeDef,
-    CreateContactFlowResponseTypeDef,
-    CreateEvaluationFormResponseTypeDef,
-    CreateHoursOfOperationResponseTypeDef,
-    CreateInstanceResponseTypeDef,
-    CreateIntegrationAssociationResponseTypeDef,
-    CreateParticipantResponseTypeDef,
-    CreatePromptResponseTypeDef,
-    CreateQueueResponseTypeDef,
-    CreateQuickConnectResponseTypeDef,
-    CreateRoutingProfileResponseTypeDef,
-    CreateRuleResponseTypeDef,
-    CreateSecurityProfileResponseTypeDef,
-    CreateTaskTemplateResponseTypeDef,
-    CreateTrafficDistributionGroupResponseTypeDef,
-    CreateUseCaseResponseTypeDef,
-    CreateUserHierarchyGroupResponseTypeDef,
-    CreateUserResponseTypeDef,
-    CreateVocabularyResponseTypeDef,
+    ClaimPhoneNumberResponseOutputTypeDef,
+    CreateAgentStatusResponseOutputTypeDef,
+    CreateContactFlowModuleResponseOutputTypeDef,
+    CreateContactFlowResponseOutputTypeDef,
+    CreateEvaluationFormResponseOutputTypeDef,
+    CreateHoursOfOperationResponseOutputTypeDef,
+    CreateInstanceResponseOutputTypeDef,
+    CreateIntegrationAssociationResponseOutputTypeDef,
+    CreateParticipantResponseOutputTypeDef,
+    CreatePromptResponseOutputTypeDef,
+    CreateQueueResponseOutputTypeDef,
+    CreateQuickConnectResponseOutputTypeDef,
+    CreateRoutingProfileResponseOutputTypeDef,
+    CreateRuleResponseOutputTypeDef,
+    CreateSecurityProfileResponseOutputTypeDef,
+    CreateTaskTemplateResponseOutputTypeDef,
+    CreateTrafficDistributionGroupResponseOutputTypeDef,
+    CreateUseCaseResponseOutputTypeDef,
+    CreateUserHierarchyGroupResponseOutputTypeDef,
+    CreateUserResponseOutputTypeDef,
+    CreateVocabularyResponseOutputTypeDef,
     CurrentMetricSortCriteriaTypeDef,
     CurrentMetricTypeDef,
-    DeactivateEvaluationFormResponseTypeDef,
-    DeleteVocabularyResponseTypeDef,
-    DescribeAgentStatusResponseTypeDef,
-    DescribeContactEvaluationResponseTypeDef,
-    DescribeContactFlowModuleResponseTypeDef,
-    DescribeContactFlowResponseTypeDef,
-    DescribeContactResponseTypeDef,
-    DescribeEvaluationFormResponseTypeDef,
-    DescribeHoursOfOperationResponseTypeDef,
-    DescribeInstanceAttributeResponseTypeDef,
-    DescribeInstanceResponseTypeDef,
-    DescribeInstanceStorageConfigResponseTypeDef,
-    DescribePhoneNumberResponseTypeDef,
-    DescribePromptResponseTypeDef,
-    DescribeQueueResponseTypeDef,
-    DescribeQuickConnectResponseTypeDef,
-    DescribeRoutingProfileResponseTypeDef,
-    DescribeRuleResponseTypeDef,
-    DescribeSecurityProfileResponseTypeDef,
-    DescribeTrafficDistributionGroupResponseTypeDef,
-    DescribeUserHierarchyGroupResponseTypeDef,
-    DescribeUserHierarchyStructureResponseTypeDef,
-    DescribeUserResponseTypeDef,
-    DescribeVocabularyResponseTypeDef,
+    DeactivateEvaluationFormResponseOutputTypeDef,
+    DeleteVocabularyResponseOutputTypeDef,
+    DescribeAgentStatusResponseOutputTypeDef,
+    DescribeContactEvaluationResponseOutputTypeDef,
+    DescribeContactFlowModuleResponseOutputTypeDef,
+    DescribeContactFlowResponseOutputTypeDef,
+    DescribeContactResponseOutputTypeDef,
+    DescribeEvaluationFormResponseOutputTypeDef,
+    DescribeHoursOfOperationResponseOutputTypeDef,
+    DescribeInstanceAttributeResponseOutputTypeDef,
+    DescribeInstanceResponseOutputTypeDef,
+    DescribeInstanceStorageConfigResponseOutputTypeDef,
+    DescribePhoneNumberResponseOutputTypeDef,
+    DescribePromptResponseOutputTypeDef,
+    DescribeQueueResponseOutputTypeDef,
+    DescribeQuickConnectResponseOutputTypeDef,
+    DescribeRoutingProfileResponseOutputTypeDef,
+    DescribeRuleResponseOutputTypeDef,
+    DescribeSecurityProfileResponseOutputTypeDef,
+    DescribeTrafficDistributionGroupResponseOutputTypeDef,
+    DescribeUserHierarchyGroupResponseOutputTypeDef,
+    DescribeUserHierarchyStructureResponseOutputTypeDef,
+    DescribeUserResponseOutputTypeDef,
+    DescribeVocabularyResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationAnswerInputTypeDef,
     EvaluationFormItemTypeDef,
     EvaluationFormScoringStrategyTypeDef,
     EvaluationNoteTypeDef,
     FiltersTypeDef,
     FilterV2TypeDef,
-    GetContactAttributesResponseTypeDef,
-    GetCurrentMetricDataResponseTypeDef,
-    GetCurrentUserDataResponseTypeDef,
-    GetFederationTokenResponseTypeDef,
-    GetMetricDataResponseTypeDef,
-    GetMetricDataV2ResponseTypeDef,
-    GetPromptFileResponseTypeDef,
-    GetTaskTemplateResponseTypeDef,
-    GetTrafficDistributionResponseTypeDef,
+    GetContactAttributesResponseOutputTypeDef,
+    GetCurrentMetricDataResponseOutputTypeDef,
+    GetCurrentUserDataResponseOutputTypeDef,
+    GetFederationTokenResponseOutputTypeDef,
+    GetMetricDataResponseOutputTypeDef,
+    GetMetricDataV2ResponseOutputTypeDef,
+    GetPromptFileResponseOutputTypeDef,
+    GetTaskTemplateResponseOutputTypeDef,
+    GetTrafficDistributionResponseOutputTypeDef,
     HierarchyStructureUpdateTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationConfigTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
     InstanceStorageConfigTypeDef,
     LexBotTypeDef,
     LexV2BotTypeDef,
-    ListAgentStatusResponseTypeDef,
-    ListApprovedOriginsResponseTypeDef,
-    ListBotsResponseTypeDef,
-    ListContactEvaluationsResponseTypeDef,
-    ListContactFlowModulesResponseTypeDef,
-    ListContactFlowsResponseTypeDef,
-    ListContactReferencesResponseTypeDef,
-    ListDefaultVocabulariesResponseTypeDef,
-    ListEvaluationFormsResponseTypeDef,
-    ListEvaluationFormVersionsResponseTypeDef,
-    ListHoursOfOperationsResponseTypeDef,
-    ListInstanceAttributesResponseTypeDef,
-    ListInstancesResponseTypeDef,
-    ListInstanceStorageConfigsResponseTypeDef,
-    ListIntegrationAssociationsResponseTypeDef,
-    ListLambdaFunctionsResponseTypeDef,
-    ListLexBotsResponseTypeDef,
-    ListPhoneNumbersResponseTypeDef,
-    ListPhoneNumbersV2ResponseTypeDef,
-    ListPromptsResponseTypeDef,
-    ListQueueQuickConnectsResponseTypeDef,
-    ListQueuesResponseTypeDef,
-    ListQuickConnectsResponseTypeDef,
-    ListRoutingProfileQueuesResponseTypeDef,
-    ListRoutingProfilesResponseTypeDef,
-    ListRulesResponseTypeDef,
-    ListSecurityKeysResponseTypeDef,
-    ListSecurityProfilePermissionsResponseTypeDef,
-    ListSecurityProfilesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTaskTemplatesResponseTypeDef,
-    ListTrafficDistributionGroupsResponseTypeDef,
-    ListUseCasesResponseTypeDef,
-    ListUserHierarchyGroupsResponseTypeDef,
-    ListUsersResponseTypeDef,
+    ListAgentStatusResponseOutputTypeDef,
+    ListApprovedOriginsResponseOutputTypeDef,
+    ListBotsResponseOutputTypeDef,
+    ListContactEvaluationsResponseOutputTypeDef,
+    ListContactFlowModulesResponseOutputTypeDef,
+    ListContactFlowsResponseOutputTypeDef,
+    ListContactReferencesResponseOutputTypeDef,
+    ListDefaultVocabulariesResponseOutputTypeDef,
+    ListEvaluationFormsResponseOutputTypeDef,
+    ListEvaluationFormVersionsResponseOutputTypeDef,
+    ListHoursOfOperationsResponseOutputTypeDef,
+    ListInstanceAttributesResponseOutputTypeDef,
+    ListInstancesResponseOutputTypeDef,
+    ListInstanceStorageConfigsResponseOutputTypeDef,
+    ListIntegrationAssociationsResponseOutputTypeDef,
+    ListLambdaFunctionsResponseOutputTypeDef,
+    ListLexBotsResponseOutputTypeDef,
+    ListPhoneNumbersResponseOutputTypeDef,
+    ListPhoneNumbersV2ResponseOutputTypeDef,
+    ListPromptsResponseOutputTypeDef,
+    ListQueueQuickConnectsResponseOutputTypeDef,
+    ListQueuesResponseOutputTypeDef,
+    ListQuickConnectsResponseOutputTypeDef,
+    ListRoutingProfileQueuesResponseOutputTypeDef,
+    ListRoutingProfilesResponseOutputTypeDef,
+    ListRulesResponseOutputTypeDef,
+    ListSecurityKeysResponseOutputTypeDef,
+    ListSecurityProfilePermissionsResponseOutputTypeDef,
+    ListSecurityProfilesResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListTaskTemplatesResponseOutputTypeDef,
+    ListTrafficDistributionGroupsResponseOutputTypeDef,
+    ListUseCasesResponseOutputTypeDef,
+    ListUserHierarchyGroupsResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
     MediaConcurrencyTypeDef,
     MetricV2TypeDef,
-    MonitorContactResponseTypeDef,
+    MonitorContactResponseOutputTypeDef,
     OutboundCallerConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     PersistentChatTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectConfigTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
     ReferenceTypeDef,
-    ReplicateInstanceResponseTypeDef,
+    ReplicateInstanceResponseOutputTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
     RuleActionTypeDef,
     RuleTriggerEventSourceTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
-    SearchHoursOfOperationsResponseTypeDef,
-    SearchPromptsResponseTypeDef,
-    SearchQueuesResponseTypeDef,
-    SearchQuickConnectsResponseTypeDef,
-    SearchResourceTagsResponseTypeDef,
-    SearchRoutingProfilesResponseTypeDef,
-    SearchSecurityProfilesResponseTypeDef,
-    SearchUsersResponseTypeDef,
-    SearchVocabulariesResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseOutputTypeDef,
+    SearchHoursOfOperationsResponseOutputTypeDef,
+    SearchPromptsResponseOutputTypeDef,
+    SearchQueuesResponseOutputTypeDef,
+    SearchQuickConnectsResponseOutputTypeDef,
+    SearchResourceTagsResponseOutputTypeDef,
+    SearchRoutingProfilesResponseOutputTypeDef,
+    SearchSecurityProfilesResponseOutputTypeDef,
+    SearchUsersResponseOutputTypeDef,
+    SearchVocabulariesResponseOutputTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     SecurityProfilesSearchFilterTypeDef,
-    StartChatContactResponseTypeDef,
-    StartContactEvaluationResponseTypeDef,
-    StartContactStreamingResponseTypeDef,
-    StartOutboundVoiceContactResponseTypeDef,
-    StartTaskContactResponseTypeDef,
-    SubmitContactEvaluationResponseTypeDef,
+    StartChatContactResponseOutputTypeDef,
+    StartContactEvaluationResponseOutputTypeDef,
+    StartContactStreamingResponseOutputTypeDef,
+    StartOutboundVoiceContactResponseOutputTypeDef,
+    StartTaskContactResponseOutputTypeDef,
+    SubmitContactEvaluationResponseOutputTypeDef,
     TaskTemplateConstraintsTypeDef,
     TaskTemplateDefaultsTypeDef,
     TaskTemplateFieldTypeDef,
     TelephonyConfigTypeDef,
-    TransferContactResponseTypeDef,
-    UpdateContactEvaluationResponseTypeDef,
-    UpdateEvaluationFormResponseTypeDef,
+    TransferContactResponseOutputTypeDef,
+    UpdateContactEvaluationResponseOutputTypeDef,
+    UpdateEvaluationFormResponseOutputTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
-    UpdatePhoneNumberResponseTypeDef,
-    UpdatePromptResponseTypeDef,
-    UpdateTaskTemplateResponseTypeDef,
+    UpdatePhoneNumberResponseOutputTypeDef,
+    UpdatePromptResponseOutputTypeDef,
+    UpdateTaskTemplateResponseOutputTypeDef,
     UserDataFiltersTypeDef,
     UserIdentityInfoTypeDef,
     UserPhoneConfigTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
     VoiceRecordingConfigurationTypeDef,
 )
@@ -325,15 +325,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#exceptions)
         """
 
     def activate_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int
-    ) -> ActivateEvaluationFormResponseTypeDef:
+    ) -> ActivateEvaluationFormResponseOutputTypeDef:
         """
         Activates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.activate_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#activate_evaluation_form)
         """
 
@@ -369,15 +369,15 @@
 
     def associate_instance_storage_config(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         StorageConfig: "InstanceStorageConfigTypeDef"
-    ) -> AssociateInstanceStorageConfigResponseTypeDef:
+    ) -> AssociateInstanceStorageConfigResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_instance_storage_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_instance_storage_config)
         """
 
@@ -433,15 +433,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_routing_profile_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_routing_profile_queues)
         """
 
     def associate_security_key(
         self, *, InstanceId: str, Key: str
-    ) -> AssociateSecurityKeyResponseTypeDef:
+    ) -> AssociateSecurityKeyResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_security_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_security_key)
         """
 
@@ -457,15 +457,15 @@
         self,
         *,
         TargetArn: str,
         PhoneNumber: str,
         PhoneNumberDescription: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...
-    ) -> ClaimPhoneNumberResponseTypeDef:
+    ) -> ClaimPhoneNumberResponseOutputTypeDef:
         """
         Claims an available phone number to your Amazon Connect instance or traffic
         distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.claim_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#claim_phone_number)
         """
@@ -483,15 +483,15 @@
         *,
         InstanceId: str,
         Name: str,
         State: AgentStatusStateType,
         Description: str = ...,
         DisplayOrder: int = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateAgentStatusResponseTypeDef:
+    ) -> CreateAgentStatusResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_agent_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_agent_status)
         """
 
@@ -500,15 +500,15 @@
         *,
         InstanceId: str,
         Name: str,
         Type: ContactFlowTypeType,
         Content: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateContactFlowResponseTypeDef:
+    ) -> CreateContactFlowResponseOutputTypeDef:
         """
         Creates a flow for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_contact_flow)
         """
 
@@ -517,15 +517,15 @@
         *,
         InstanceId: str,
         Name: str,
         Content: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...
-    ) -> CreateContactFlowModuleResponseTypeDef:
+    ) -> CreateContactFlowModuleResponseOutputTypeDef:
         """
         Creates a flow module for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow_module)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_contact_flow_module)
         """
 
@@ -534,15 +534,15 @@
         *,
         InstanceId: str,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         Description: str = ...,
         ScoringStrategy: "EvaluationFormScoringStrategyTypeDef" = ...,
         ClientToken: str = ...
-    ) -> CreateEvaluationFormResponseTypeDef:
+    ) -> CreateEvaluationFormResponseOutputTypeDef:
         """
         Creates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_evaluation_form)
         """
 
@@ -551,15 +551,15 @@
         *,
         InstanceId: str,
         Name: str,
         TimeZone: str,
         Config: Sequence["HoursOfOperationConfigTypeDef"],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateHoursOfOperationResponseTypeDef:
+    ) -> CreateHoursOfOperationResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_hours_of_operation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_hours_of_operation)
         """
 
@@ -568,15 +568,15 @@
         *,
         IdentityManagementType: DirectoryTypeType,
         InboundCallsEnabled: bool,
         OutboundCallsEnabled: bool,
         ClientToken: str = ...,
         InstanceAlias: str = ...,
         DirectoryId: str = ...
-    ) -> CreateInstanceResponseTypeDef:
+    ) -> CreateInstanceResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_instance)
         """
 
@@ -586,15 +586,15 @@
         InstanceId: str,
         IntegrationType: IntegrationTypeType,
         IntegrationArn: str,
         SourceApplicationUrl: str = ...,
         SourceApplicationName: str = ...,
         SourceType: SourceTypeType = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateIntegrationAssociationResponseTypeDef:
+    ) -> CreateIntegrationAssociationResponseOutputTypeDef:
         """
         Creates an Amazon Web Services resource association with an Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_integration_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_integration_association)
         """
@@ -602,15 +602,15 @@
     def create_participant(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ParticipantDetails: "ParticipantDetailsToAddTypeDef",
         ClientToken: str = ...
-    ) -> CreateParticipantResponseTypeDef:
+    ) -> CreateParticipantResponseOutputTypeDef:
         """
         Adds a new participant into an on-going chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_participant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_participant)
         """
 
@@ -618,15 +618,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         S3Uri: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreatePromptResponseTypeDef:
+    ) -> CreatePromptResponseOutputTypeDef:
         """
         Creates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_prompt)
         """
 
@@ -637,15 +637,15 @@
         Name: str,
         HoursOfOperationId: str,
         Description: str = ...,
         OutboundCallerConfig: "OutboundCallerConfigTypeDef" = ...,
         MaxContacts: int = ...,
         QuickConnectIds: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateQueueResponseTypeDef:
+    ) -> CreateQueueResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_queue)
         """
 
@@ -653,15 +653,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         QuickConnectConfig: "QuickConnectConfigTypeDef",
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateQuickConnectResponseTypeDef:
+    ) -> CreateQuickConnectResponseOutputTypeDef:
         """
         Creates a quick connect for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_quick_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_quick_connect)
         """
 
@@ -671,15 +671,15 @@
         InstanceId: str,
         Name: str,
         Description: str,
         DefaultOutboundQueueId: str,
         MediaConcurrencies: Sequence["MediaConcurrencyTypeDef"],
         QueueConfigs: Sequence["RoutingProfileQueueConfigTypeDef"] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateRoutingProfileResponseTypeDef:
+    ) -> CreateRoutingProfileResponseOutputTypeDef:
         """
         Creates a new routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_routing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_routing_profile)
         """
 
@@ -689,15 +689,15 @@
         InstanceId: str,
         Name: str,
         TriggerEventSource: "RuleTriggerEventSourceTypeDef",
         Function: str,
         Actions: Sequence["RuleActionTypeDef"],
         PublishStatus: RulePublishStatusType,
         ClientToken: str = ...
-    ) -> CreateRuleResponseTypeDef:
+    ) -> CreateRuleResponseOutputTypeDef:
         """
         Creates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_rule)
         """
 
@@ -707,15 +707,15 @@
         SecurityProfileName: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...
-    ) -> CreateSecurityProfileResponseTypeDef:
+    ) -> CreateSecurityProfileResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_security_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_security_profile)
         """
 
@@ -727,15 +727,15 @@
         Fields: Sequence["TaskTemplateFieldTypeDef"],
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: "TaskTemplateConstraintsTypeDef" = ...,
         Defaults: "TaskTemplateDefaultsTypeDef" = ...,
         Status: TaskTemplateStatusType = ...,
         ClientToken: str = ...
-    ) -> CreateTaskTemplateResponseTypeDef:
+    ) -> CreateTaskTemplateResponseOutputTypeDef:
         """
         Creates a new task template in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_task_template)
         """
 
@@ -743,15 +743,15 @@
         self,
         *,
         Name: str,
         InstanceId: str,
         Description: str = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateTrafficDistributionGroupResponseTypeDef:
+    ) -> CreateTrafficDistributionGroupResponseOutputTypeDef:
         """
         Creates a traffic distribution group given an Amazon Connect instance that has
         been replicated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_traffic_distribution_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_traffic_distribution_group)
         """
@@ -759,15 +759,15 @@
     def create_use_case(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         UseCaseType: UseCaseTypeType,
         Tags: Mapping[str, str] = ...
-    ) -> CreateUseCaseResponseTypeDef:
+    ) -> CreateUseCaseResponseOutputTypeDef:
         """
         Creates a use case for an integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_use_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_use_case)
         """
 
@@ -780,25 +780,25 @@
         RoutingProfileId: str,
         InstanceId: str,
         Password: str = ...,
         IdentityInfo: "UserIdentityInfoTypeDef" = ...,
         DirectoryUserId: str = ...,
         HierarchyGroupId: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateUserResponseTypeDef:
+    ) -> CreateUserResponseOutputTypeDef:
         """
         Creates a user account for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_user)
         """
 
     def create_user_hierarchy_group(
         self, *, Name: str, InstanceId: str, ParentGroupId: str = ..., Tags: Mapping[str, str] = ...
-    ) -> CreateUserHierarchyGroupResponseTypeDef:
+    ) -> CreateUserHierarchyGroupResponseOutputTypeDef:
         """
         Creates a new user hierarchy group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_user_hierarchy_group)
         """
 
@@ -807,25 +807,25 @@
         *,
         InstanceId: str,
         VocabularyName: str,
         LanguageCode: VocabularyLanguageCodeType,
         Content: str,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateVocabularyResponseTypeDef:
+    ) -> CreateVocabularyResponseOutputTypeDef:
         """
         Creates a custom vocabulary associated with your Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_vocabulary)
         """
 
     def deactivate_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int
-    ) -> DeactivateEvaluationFormResponseTypeDef:
+    ) -> DeactivateEvaluationFormResponseOutputTypeDef:
         """
         Deactivates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.deactivate_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#deactivate_evaluation_form)
         """
 
@@ -994,224 +994,230 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_user_hierarchy_group)
         """
 
     def delete_vocabulary(
         self, *, InstanceId: str, VocabularyId: str
-    ) -> DeleteVocabularyResponseTypeDef:
+    ) -> DeleteVocabularyResponseOutputTypeDef:
         """
         Deletes the vocabulary that has the given identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_vocabulary)
         """
 
     def describe_agent_status(
         self, *, InstanceId: str, AgentStatusId: str
-    ) -> DescribeAgentStatusResponseTypeDef:
+    ) -> DescribeAgentStatusResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_agent_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_agent_status)
         """
 
     def describe_contact(
         self, *, InstanceId: str, ContactId: str
-    ) -> DescribeContactResponseTypeDef:
+    ) -> DescribeContactResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact)
         """
 
     def describe_contact_evaluation(
         self, *, InstanceId: str, EvaluationId: str
-    ) -> DescribeContactEvaluationResponseTypeDef:
+    ) -> DescribeContactEvaluationResponseOutputTypeDef:
         """
         Describes a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_evaluation)
         """
 
     def describe_contact_flow(
         self, *, InstanceId: str, ContactFlowId: str
-    ) -> DescribeContactFlowResponseTypeDef:
+    ) -> DescribeContactFlowResponseOutputTypeDef:
         """
         Describes the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_flow)
         """
 
     def describe_contact_flow_module(
         self, *, InstanceId: str, ContactFlowModuleId: str
-    ) -> DescribeContactFlowModuleResponseTypeDef:
+    ) -> DescribeContactFlowModuleResponseOutputTypeDef:
         """
         Describes the specified flow module.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_flow_module)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_flow_module)
         """
 
     def describe_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int = ...
-    ) -> DescribeEvaluationFormResponseTypeDef:
+    ) -> DescribeEvaluationFormResponseOutputTypeDef:
         """
         Describes an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_evaluation_form)
         """
 
     def describe_hours_of_operation(
         self, *, InstanceId: str, HoursOfOperationId: str
-    ) -> DescribeHoursOfOperationResponseTypeDef:
+    ) -> DescribeHoursOfOperationResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_hours_of_operation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_hours_of_operation)
         """
 
-    def describe_instance(self, *, InstanceId: str) -> DescribeInstanceResponseTypeDef:
+    def describe_instance(self, *, InstanceId: str) -> DescribeInstanceResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance)
         """
 
     def describe_instance_attribute(
         self, *, InstanceId: str, AttributeType: InstanceAttributeTypeType
-    ) -> DescribeInstanceAttributeResponseTypeDef:
+    ) -> DescribeInstanceAttributeResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_attribute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance_attribute)
         """
 
     def describe_instance_storage_config(
         self, *, InstanceId: str, AssociationId: str, ResourceType: InstanceStorageResourceTypeType
-    ) -> DescribeInstanceStorageConfigResponseTypeDef:
+    ) -> DescribeInstanceStorageConfigResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_storage_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance_storage_config)
         """
 
-    def describe_phone_number(self, *, PhoneNumberId: str) -> DescribePhoneNumberResponseTypeDef:
+    def describe_phone_number(
+        self, *, PhoneNumberId: str
+    ) -> DescribePhoneNumberResponseOutputTypeDef:
         """
         Gets details and status of a phone number that’s claimed to your Amazon Connect
         instance or traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_phone_number)
         """
 
-    def describe_prompt(self, *, InstanceId: str, PromptId: str) -> DescribePromptResponseTypeDef:
+    def describe_prompt(
+        self, *, InstanceId: str, PromptId: str
+    ) -> DescribePromptResponseOutputTypeDef:
         """
         Describes the prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_prompt)
         """
 
-    def describe_queue(self, *, InstanceId: str, QueueId: str) -> DescribeQueueResponseTypeDef:
+    def describe_queue(
+        self, *, InstanceId: str, QueueId: str
+    ) -> DescribeQueueResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_queue)
         """
 
     def describe_quick_connect(
         self, *, InstanceId: str, QuickConnectId: str
-    ) -> DescribeQuickConnectResponseTypeDef:
+    ) -> DescribeQuickConnectResponseOutputTypeDef:
         """
         Describes the quick connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_quick_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_quick_connect)
         """
 
     def describe_routing_profile(
         self, *, InstanceId: str, RoutingProfileId: str
-    ) -> DescribeRoutingProfileResponseTypeDef:
+    ) -> DescribeRoutingProfileResponseOutputTypeDef:
         """
         Describes the specified routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_routing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_routing_profile)
         """
 
-    def describe_rule(self, *, InstanceId: str, RuleId: str) -> DescribeRuleResponseTypeDef:
+    def describe_rule(self, *, InstanceId: str, RuleId: str) -> DescribeRuleResponseOutputTypeDef:
         """
         Describes a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_rule)
         """
 
     def describe_security_profile(
         self, *, SecurityProfileId: str, InstanceId: str
-    ) -> DescribeSecurityProfileResponseTypeDef:
+    ) -> DescribeSecurityProfileResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_security_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_security_profile)
         """
 
     def describe_traffic_distribution_group(
         self, *, TrafficDistributionGroupId: str
-    ) -> DescribeTrafficDistributionGroupResponseTypeDef:
+    ) -> DescribeTrafficDistributionGroupResponseOutputTypeDef:
         """
         Gets details and status of a traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_traffic_distribution_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_traffic_distribution_group)
         """
 
-    def describe_user(self, *, UserId: str, InstanceId: str) -> DescribeUserResponseTypeDef:
+    def describe_user(self, *, UserId: str, InstanceId: str) -> DescribeUserResponseOutputTypeDef:
         """
         Describes the specified user account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user)
         """
 
     def describe_user_hierarchy_group(
         self, *, HierarchyGroupId: str, InstanceId: str
-    ) -> DescribeUserHierarchyGroupResponseTypeDef:
+    ) -> DescribeUserHierarchyGroupResponseOutputTypeDef:
         """
         Describes the specified hierarchy group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user_hierarchy_group)
         """
 
     def describe_user_hierarchy_structure(
         self, *, InstanceId: str
-    ) -> DescribeUserHierarchyStructureResponseTypeDef:
+    ) -> DescribeUserHierarchyStructureResponseOutputTypeDef:
         """
         Describes the hierarchy structure of the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user_hierarchy_structure)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user_hierarchy_structure)
         """
 
     def describe_vocabulary(
         self, *, InstanceId: str, VocabularyId: str
-    ) -> DescribeVocabularyResponseTypeDef:
+    ) -> DescribeVocabularyResponseOutputTypeDef:
         """
         Describes the specified vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_vocabulary)
         """
 
@@ -1333,15 +1339,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#generate_presigned_url)
         """
 
     def get_contact_attributes(
         self, *, InstanceId: str, InitialContactId: str
-    ) -> GetContactAttributesResponseTypeDef:
+    ) -> GetContactAttributesResponseOutputTypeDef:
         """
         Retrieves the contact attributes for the specified contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_contact_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_contact_attributes)
         """
 
@@ -1351,38 +1357,38 @@
         InstanceId: str,
         Filters: "FiltersTypeDef",
         CurrentMetrics: Sequence["CurrentMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortCriteria: Sequence["CurrentMetricSortCriteriaTypeDef"] = ...
-    ) -> GetCurrentMetricDataResponseTypeDef:
+    ) -> GetCurrentMetricDataResponseOutputTypeDef:
         """
         Gets the real-time metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_current_metric_data)
         """
 
     def get_current_user_data(
         self,
         *,
         InstanceId: str,
         Filters: "UserDataFiltersTypeDef",
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetCurrentUserDataResponseTypeDef:
+    ) -> GetCurrentUserDataResponseOutputTypeDef:
         """
         Gets the real-time active user data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_user_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_current_user_data)
         """
 
-    def get_federation_token(self, *, InstanceId: str) -> GetFederationTokenResponseTypeDef:
+    def get_federation_token(self, *, InstanceId: str) -> GetFederationTokenResponseOutputTypeDef:
         """
         Retrieves a token for federation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_federation_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_federation_token)
         """
 
@@ -1393,15 +1399,15 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: "FiltersTypeDef",
         HistoricalMetrics: Sequence["HistoricalMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetMetricDataResponseTypeDef:
+    ) -> GetMetricDataResponseOutputTypeDef:
         """
         Gets historical metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data)
         """
 
@@ -1412,42 +1418,44 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: Sequence["FilterV2TypeDef"],
         Metrics: Sequence["MetricV2TypeDef"],
         Groupings: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetMetricDataV2ResponseTypeDef:
+    ) -> GetMetricDataV2ResponseOutputTypeDef:
         """
         Gets metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data_v2)
         """
 
-    def get_prompt_file(self, *, InstanceId: str, PromptId: str) -> GetPromptFileResponseTypeDef:
+    def get_prompt_file(
+        self, *, InstanceId: str, PromptId: str
+    ) -> GetPromptFileResponseOutputTypeDef:
         """
         Gets the prompt file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_prompt_file)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_prompt_file)
         """
 
     def get_task_template(
         self, *, InstanceId: str, TaskTemplateId: str, SnapshotVersion: str = ...
-    ) -> GetTaskTemplateResponseTypeDef:
+    ) -> GetTaskTemplateResponseOutputTypeDef:
         """
         Gets details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_task_template)
         """
 
-    def get_traffic_distribution(self, *, Id: str) -> GetTrafficDistributionResponseTypeDef:
+    def get_traffic_distribution(self, *, Id: str) -> GetTrafficDistributionResponseOutputTypeDef:
         """
         Retrieves the current traffic distribution for a given traffic distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_traffic_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_traffic_distribution)
         """
@@ -1455,65 +1463,65 @@
     def list_agent_statuses(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         AgentStatusTypes: Sequence[AgentStatusTypeType] = ...
-    ) -> ListAgentStatusResponseTypeDef:
+    ) -> ListAgentStatusResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_agent_statuses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_agent_statuses)
         """
 
     def list_approved_origins(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListApprovedOriginsResponseTypeDef:
+    ) -> ListApprovedOriginsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_approved_origins)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_approved_origins)
         """
 
     def list_bots(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListBotsResponseTypeDef:
+    ) -> ListBotsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_bots)
         """
 
     def list_contact_evaluations(
         self, *, InstanceId: str, ContactId: str, NextToken: str = ...
-    ) -> ListContactEvaluationsResponseTypeDef:
+    ) -> ListContactEvaluationsResponseOutputTypeDef:
         """
         Lists contact evaluations in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_evaluations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_evaluations)
         """
 
     def list_contact_flow_modules(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         ContactFlowModuleState: ContactFlowModuleStateType = ...
-    ) -> ListContactFlowModulesResponseTypeDef:
+    ) -> ListContactFlowModulesResponseOutputTypeDef:
         """
         Provides information about the flow modules for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flow_modules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_flow_modules)
         """
@@ -1521,147 +1529,147 @@
     def list_contact_flows(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListContactFlowsResponseTypeDef:
+    ) -> ListContactFlowsResponseOutputTypeDef:
         """
         Provides information about the flows for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_flows)
         """
 
     def list_contact_references(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
         NextToken: str = ...
-    ) -> ListContactReferencesResponseTypeDef:
+    ) -> ListContactReferencesResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_references)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_references)
         """
 
     def list_default_vocabularies(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> ListDefaultVocabulariesResponseTypeDef:
+    ) -> ListDefaultVocabulariesResponseOutputTypeDef:
         """
         Lists the default vocabularies for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_default_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_default_vocabularies)
         """
 
     def list_evaluation_form_versions(
         self, *, InstanceId: str, EvaluationFormId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListEvaluationFormVersionsResponseTypeDef:
+    ) -> ListEvaluationFormVersionsResponseOutputTypeDef:
         """
         Lists versions of an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_evaluation_form_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_evaluation_form_versions)
         """
 
     def list_evaluation_forms(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListEvaluationFormsResponseTypeDef:
+    ) -> ListEvaluationFormsResponseOutputTypeDef:
         """
         Lists evaluation forms in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_evaluation_forms)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_evaluation_forms)
         """
 
     def list_hours_of_operations(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListHoursOfOperationsResponseTypeDef:
+    ) -> ListHoursOfOperationsResponseOutputTypeDef:
         """
         Provides information about the hours of operation for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_hours_of_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_hours_of_operations)
         """
 
     def list_instance_attributes(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListInstanceAttributesResponseTypeDef:
+    ) -> ListInstanceAttributesResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instance_attributes)
         """
 
     def list_instance_storage_configs(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListInstanceStorageConfigsResponseTypeDef:
+    ) -> ListInstanceStorageConfigsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_storage_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instance_storage_configs)
         """
 
     def list_instances(
         self, *, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListInstancesResponseTypeDef:
+    ) -> ListInstancesResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instances)
         """
 
     def list_integration_associations(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListIntegrationAssociationsResponseTypeDef:
+    ) -> ListIntegrationAssociationsResponseOutputTypeDef:
         """
         Provides summary information about the Amazon Web Services resource associations
         for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_integration_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_integration_associations)
         """
 
     def list_lambda_functions(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListLambdaFunctionsResponseTypeDef:
+    ) -> ListLambdaFunctionsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_lambda_functions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_lambda_functions)
         """
 
     def list_lex_bots(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListLexBotsResponseTypeDef:
+    ) -> ListLexBotsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_lex_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_lex_bots)
         """
 
@@ -1669,15 +1677,15 @@
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListPhoneNumbersResponseTypeDef:
+    ) -> ListPhoneNumbersResponseOutputTypeDef:
         """
         Provides information about the phone numbers for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_phone_numbers)
         """
@@ -1687,88 +1695,88 @@
         *,
         TargetArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberPrefix: str = ...
-    ) -> ListPhoneNumbersV2ResponseTypeDef:
+    ) -> ListPhoneNumbersV2ResponseOutputTypeDef:
         """
         Lists phone numbers claimed to your Amazon Connect instance or traffic
         distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_phone_numbers_v2)
         """
 
     def list_prompts(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListPromptsResponseTypeDef:
+    ) -> ListPromptsResponseOutputTypeDef:
         """
         Provides information about the prompts for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_prompts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_prompts)
         """
 
     def list_queue_quick_connects(
         self, *, InstanceId: str, QueueId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListQueueQuickConnectsResponseTypeDef:
+    ) -> ListQueueQuickConnectsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queue_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_queue_quick_connects)
         """
 
     def list_queues(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListQueuesResponseTypeDef:
+    ) -> ListQueuesResponseOutputTypeDef:
         """
         Provides information about the queues for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_queues)
         """
 
     def list_quick_connects(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         QuickConnectTypes: Sequence[QuickConnectTypeType] = ...
-    ) -> ListQuickConnectsResponseTypeDef:
+    ) -> ListQuickConnectsResponseOutputTypeDef:
         """
         Provides information about the quick connects for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_quick_connects)
         """
 
     def list_routing_profile_queues(
         self, *, InstanceId: str, RoutingProfileId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListRoutingProfileQueuesResponseTypeDef:
+    ) -> ListRoutingProfileQueuesResponseOutputTypeDef:
         """
         Lists the queues associated with a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_routing_profile_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_routing_profile_queues)
         """
 
     def list_routing_profiles(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListRoutingProfilesResponseTypeDef:
+    ) -> ListRoutingProfilesResponseOutputTypeDef:
         """
         Provides summary information about the routing profiles for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_routing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_routing_profiles)
         """
@@ -1777,59 +1785,61 @@
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> ListRulesResponseTypeDef:
+    ) -> ListRulesResponseOutputTypeDef:
         """
         List all rules for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_rules)
         """
 
     def list_security_keys(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListSecurityKeysResponseTypeDef:
+    ) -> ListSecurityKeysResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_keys)
         """
 
     def list_security_profile_permissions(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListSecurityProfilePermissionsResponseTypeDef:
+    ) -> ListSecurityProfilePermissionsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profile_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_profile_permissions)
         """
 
     def list_security_profiles(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListSecurityProfilesResponseTypeDef:
+    ) -> ListSecurityProfilesResponseOutputTypeDef:
         """
         Provides summary information about the security profiles for the specified
         Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_profiles)
         """
 
-    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
+    def list_tags_for_resource(
+        self, *, resourceArn: str
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_tags_for_resource)
         """
 
@@ -1837,61 +1847,61 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: TaskTemplateStatusType = ...,
         Name: str = ...
-    ) -> ListTaskTemplatesResponseTypeDef:
+    ) -> ListTaskTemplatesResponseOutputTypeDef:
         """
         Lists task templates for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_task_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_task_templates)
         """
 
     def list_traffic_distribution_groups(
         self, *, MaxResults: int = ..., NextToken: str = ..., InstanceId: str = ...
-    ) -> ListTrafficDistributionGroupsResponseTypeDef:
+    ) -> ListTrafficDistributionGroupsResponseOutputTypeDef:
         """
         Lists traffic distribution groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_traffic_distribution_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_traffic_distribution_groups)
         """
 
     def list_use_cases(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListUseCasesResponseTypeDef:
+    ) -> ListUseCasesResponseOutputTypeDef:
         """
         Lists the use cases for the integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_use_cases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_use_cases)
         """
 
     def list_user_hierarchy_groups(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListUserHierarchyGroupsResponseTypeDef:
+    ) -> ListUserHierarchyGroupsResponseOutputTypeDef:
         """
         Provides summary information about the hierarchy groups for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_user_hierarchy_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_user_hierarchy_groups)
         """
 
     def list_users(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListUsersResponseTypeDef:
+    ) -> ListUsersResponseOutputTypeDef:
         """
         Provides summary information about the users for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_users)
         """
@@ -1900,15 +1910,15 @@
         self,
         *,
         InstanceId: str,
         ContactId: str,
         UserId: str,
         AllowedMonitorCapabilities: Sequence[MonitorCapabilityType] = ...,
         ClientToken: str = ...
-    ) -> MonitorContactResponseTypeDef:
+    ) -> MonitorContactResponseOutputTypeDef:
         """
         Initiates silent monitoring of a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.monitor_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#monitor_contact)
         """
 
@@ -1931,15 +1941,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.release_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#release_phone_number)
         """
 
     def replicate_instance(
         self, *, InstanceId: str, ReplicaRegion: str, ReplicaAlias: str, ClientToken: str = ...
-    ) -> ReplicateInstanceResponseTypeDef:
+    ) -> ReplicateInstanceResponseOutputTypeDef:
         """
         Replicates an Amazon Connect instance in the specified Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.replicate_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#replicate_instance)
         """
@@ -1960,15 +1970,15 @@
         *,
         TargetArn: str,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         PhoneNumberPrefix: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> SearchAvailablePhoneNumbersResponseTypeDef:
+    ) -> SearchAvailablePhoneNumbersResponseOutputTypeDef:
         """
         Searches for available phone numbers that you can claim to your Amazon Connect
         instance or traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_available_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_available_phone_numbers)
         """
@@ -1977,15 +1987,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "HoursOfOperationSearchFilterTypeDef" = ...,
         SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...
-    ) -> SearchHoursOfOperationsResponseTypeDef:
+    ) -> SearchHoursOfOperationsResponseOutputTypeDef:
         """
         Searches the hours of operation in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_hours_of_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_hours_of_operations)
         """
@@ -1994,15 +2004,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "PromptSearchFilterTypeDef" = ...,
         SearchCriteria: "PromptSearchCriteriaTypeDef" = ...
-    ) -> SearchPromptsResponseTypeDef:
+    ) -> SearchPromptsResponseOutputTypeDef:
         """
         Searches prompts in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_prompts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_prompts)
         """
 
@@ -2010,15 +2020,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "QueueSearchFilterTypeDef" = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...
-    ) -> SearchQueuesResponseTypeDef:
+    ) -> SearchQueuesResponseOutputTypeDef:
         """
         Searches queues in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_queues)
         """
 
@@ -2026,15 +2036,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "QuickConnectSearchFilterTypeDef" = ...,
         SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...
-    ) -> SearchQuickConnectsResponseTypeDef:
+    ) -> SearchQuickConnectsResponseOutputTypeDef:
         """
         Searches quick connects in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_quick_connects)
         """
 
@@ -2042,15 +2052,15 @@
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "ResourceTagsSearchCriteriaTypeDef" = ...
-    ) -> SearchResourceTagsResponseTypeDef:
+    ) -> SearchResourceTagsResponseOutputTypeDef:
         """
         Searches tags used in an Amazon Connect instance using optional search criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_resource_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_resource_tags)
         """
 
@@ -2058,15 +2068,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "RoutingProfileSearchFilterTypeDef" = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...
-    ) -> SearchRoutingProfilesResponseTypeDef:
+    ) -> SearchRoutingProfilesResponseOutputTypeDef:
         """
         Searches routing profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_routing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_routing_profiles)
         """
@@ -2075,15 +2085,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: "SecurityProfilesSearchFilterTypeDef" = ...
-    ) -> SearchSecurityProfilesResponseTypeDef:
+    ) -> SearchSecurityProfilesResponseOutputTypeDef:
         """
         Searches security profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_security_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_security_profiles)
         """
@@ -2092,15 +2102,15 @@
         self,
         *,
         InstanceId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "UserSearchFilterTypeDef" = ...,
         SearchCriteria: "UserSearchCriteriaTypeDef" = ...
-    ) -> SearchUsersResponseTypeDef:
+    ) -> SearchUsersResponseOutputTypeDef:
         """
         Searches users in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_users)
         """
 
@@ -2109,15 +2119,15 @@
         *,
         InstanceId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
         LanguageCode: VocabularyLanguageCodeType = ...
-    ) -> SearchVocabulariesResponseTypeDef:
+    ) -> SearchVocabulariesResponseOutputTypeDef:
         """
         Searches for vocabularies within a specific Amazon Connect instance using
         `State`, `NameStartsWith`, and `LanguageCode`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_vocabularies)
         """
@@ -2131,25 +2141,25 @@
         Attributes: Mapping[str, str] = ...,
         InitialMessage: "ChatMessageTypeDef" = ...,
         ClientToken: str = ...,
         ChatDurationInMinutes: int = ...,
         SupportedMessagingContentTypes: Sequence[str] = ...,
         PersistentChat: "PersistentChatTypeDef" = ...,
         RelatedContactId: str = ...
-    ) -> StartChatContactResponseTypeDef:
+    ) -> StartChatContactResponseOutputTypeDef:
         """
         Initiates a flow to start a new chat for the customer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_chat_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_chat_contact)
         """
 
     def start_contact_evaluation(
         self, *, InstanceId: str, ContactId: str, EvaluationFormId: str, ClientToken: str = ...
-    ) -> StartContactEvaluationResponseTypeDef:
+    ) -> StartContactEvaluationResponseOutputTypeDef:
         """
         Starts an empty evaluation in the specified Amazon Connect instance, using the
         given evaluation form for the particular contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_contact_evaluation)
         """
@@ -2173,15 +2183,15 @@
     def start_contact_streaming(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ChatStreamingConfiguration: "ChatStreamingConfigurationTypeDef",
         ClientToken: str
-    ) -> StartContactStreamingResponseTypeDef:
+    ) -> StartContactStreamingResponseOutputTypeDef:
         """
         Initiates real-time message streaming for a new chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_streaming)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_contact_streaming)
         """
 
@@ -2194,15 +2204,15 @@
         ClientToken: str = ...,
         SourcePhoneNumber: str = ...,
         QueueId: str = ...,
         Attributes: Mapping[str, str] = ...,
         AnswerMachineDetectionConfig: "AnswerMachineDetectionConfigTypeDef" = ...,
         CampaignId: str = ...,
         TrafficType: TrafficTypeType = ...
-    ) -> StartOutboundVoiceContactResponseTypeDef:
+    ) -> StartOutboundVoiceContactResponseOutputTypeDef:
         """
         Places an outbound call to a contact, and then initiates the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_outbound_voice_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_outbound_voice_contact)
         """
 
@@ -2217,15 +2227,15 @@
         References: Mapping[str, "ReferenceTypeDef"] = ...,
         Description: str = ...,
         ClientToken: str = ...,
         ScheduledTime: Union[datetime, str] = ...,
         TaskTemplateId: str = ...,
         QuickConnectId: str = ...,
         RelatedContactId: str = ...
-    ) -> StartTaskContactResponseTypeDef:
+    ) -> StartTaskContactResponseOutputTypeDef:
         """
         Initiates a flow to start a new task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_task_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_task_contact)
         """
 
@@ -2260,15 +2270,15 @@
     def submit_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, "EvaluationAnswerInputTypeDef"] = ...,
         Notes: Mapping[str, "EvaluationNoteTypeDef"] = ...
-    ) -> SubmitContactEvaluationResponseTypeDef:
+    ) -> SubmitContactEvaluationResponseOutputTypeDef:
         """
         Submits a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.submit_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#submit_contact_evaluation)
         """
 
@@ -2298,15 +2308,15 @@
         *,
         InstanceId: str,
         ContactId: str,
         ContactFlowId: str,
         QueueId: str = ...,
         UserId: str = ...,
         ClientToken: str = ...
-    ) -> TransferContactResponseTypeDef:
+    ) -> TransferContactResponseOutputTypeDef:
         """
         Transfers contacts from one agent or queue to another agent or queue at any
         point after a contact is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.transfer_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#transfer_contact)
         """
@@ -2369,15 +2379,15 @@
     def update_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, "EvaluationAnswerInputTypeDef"] = ...,
         Notes: Mapping[str, "EvaluationNoteTypeDef"] = ...
-    ) -> UpdateContactEvaluationResponseTypeDef:
+    ) -> UpdateContactEvaluationResponseOutputTypeDef:
         """
         Updates details about a contact evaluation in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_contact_evaluation)
         """
@@ -2462,15 +2472,15 @@
         EvaluationFormVersion: int,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         CreateNewVersion: bool = ...,
         Description: str = ...,
         ScoringStrategy: "EvaluationFormScoringStrategyTypeDef" = ...,
         ClientToken: str = ...
-    ) -> UpdateEvaluationFormResponseTypeDef:
+    ) -> UpdateEvaluationFormResponseOutputTypeDef:
         """
         Updates details about a specific evaluation form version in the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_evaluation_form)
         """
@@ -2530,15 +2540,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_participant_role_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_participant_role_config)
         """
 
     def update_phone_number(
         self, *, PhoneNumberId: str, TargetArn: str, ClientToken: str = ...
-    ) -> UpdatePhoneNumberResponseTypeDef:
+    ) -> UpdatePhoneNumberResponseOutputTypeDef:
         """
         Updates your claimed phone number from its current Amazon Connect instance or
         traffic distribution group to another Amazon Connect instance or traffic
         distribution group in the same Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_phone_number)
@@ -2548,15 +2558,15 @@
         self,
         *,
         InstanceId: str,
         PromptId: str,
         Name: str = ...,
         Description: str = ...,
         S3Uri: str = ...
-    ) -> UpdatePromptResponseTypeDef:
+    ) -> UpdatePromptResponseOutputTypeDef:
         """
         Updates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_prompt)
         """
 
@@ -2725,15 +2735,15 @@
         Name: str = ...,
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: "TaskTemplateConstraintsTypeDef" = ...,
         Defaults: "TaskTemplateDefaultsTypeDef" = ...,
         Status: TaskTemplateStatusType = ...,
         Fields: Sequence["TaskTemplateFieldTypeDef"] = ...
-    ) -> UpdateTaskTemplateResponseTypeDef:
+    ) -> UpdateTaskTemplateResponseOutputTypeDef:
         """
         Updates details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_task_template)
         """
```

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect/client.pyi` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -91,178 +91,178 @@
     SearchResourceTagsPaginator,
     SearchRoutingProfilesPaginator,
     SearchSecurityProfilesPaginator,
     SearchUsersPaginator,
     SearchVocabulariesPaginator,
 )
 from .type_defs import (
-    ActivateEvaluationFormResponseTypeDef,
+    ActivateEvaluationFormResponseOutputTypeDef,
     AnswerMachineDetectionConfigTypeDef,
-    AssociateInstanceStorageConfigResponseTypeDef,
-    AssociateSecurityKeyResponseTypeDef,
+    AssociateInstanceStorageConfigResponseOutputTypeDef,
+    AssociateSecurityKeyResponseOutputTypeDef,
     ChatMessageTypeDef,
     ChatStreamingConfigurationTypeDef,
-    ClaimPhoneNumberResponseTypeDef,
-    CreateAgentStatusResponseTypeDef,
-    CreateContactFlowModuleResponseTypeDef,
-    CreateContactFlowResponseTypeDef,
-    CreateEvaluationFormResponseTypeDef,
-    CreateHoursOfOperationResponseTypeDef,
-    CreateInstanceResponseTypeDef,
-    CreateIntegrationAssociationResponseTypeDef,
-    CreateParticipantResponseTypeDef,
-    CreatePromptResponseTypeDef,
-    CreateQueueResponseTypeDef,
-    CreateQuickConnectResponseTypeDef,
-    CreateRoutingProfileResponseTypeDef,
-    CreateRuleResponseTypeDef,
-    CreateSecurityProfileResponseTypeDef,
-    CreateTaskTemplateResponseTypeDef,
-    CreateTrafficDistributionGroupResponseTypeDef,
-    CreateUseCaseResponseTypeDef,
-    CreateUserHierarchyGroupResponseTypeDef,
-    CreateUserResponseTypeDef,
-    CreateVocabularyResponseTypeDef,
+    ClaimPhoneNumberResponseOutputTypeDef,
+    CreateAgentStatusResponseOutputTypeDef,
+    CreateContactFlowModuleResponseOutputTypeDef,
+    CreateContactFlowResponseOutputTypeDef,
+    CreateEvaluationFormResponseOutputTypeDef,
+    CreateHoursOfOperationResponseOutputTypeDef,
+    CreateInstanceResponseOutputTypeDef,
+    CreateIntegrationAssociationResponseOutputTypeDef,
+    CreateParticipantResponseOutputTypeDef,
+    CreatePromptResponseOutputTypeDef,
+    CreateQueueResponseOutputTypeDef,
+    CreateQuickConnectResponseOutputTypeDef,
+    CreateRoutingProfileResponseOutputTypeDef,
+    CreateRuleResponseOutputTypeDef,
+    CreateSecurityProfileResponseOutputTypeDef,
+    CreateTaskTemplateResponseOutputTypeDef,
+    CreateTrafficDistributionGroupResponseOutputTypeDef,
+    CreateUseCaseResponseOutputTypeDef,
+    CreateUserHierarchyGroupResponseOutputTypeDef,
+    CreateUserResponseOutputTypeDef,
+    CreateVocabularyResponseOutputTypeDef,
     CurrentMetricSortCriteriaTypeDef,
     CurrentMetricTypeDef,
-    DeactivateEvaluationFormResponseTypeDef,
-    DeleteVocabularyResponseTypeDef,
-    DescribeAgentStatusResponseTypeDef,
-    DescribeContactEvaluationResponseTypeDef,
-    DescribeContactFlowModuleResponseTypeDef,
-    DescribeContactFlowResponseTypeDef,
-    DescribeContactResponseTypeDef,
-    DescribeEvaluationFormResponseTypeDef,
-    DescribeHoursOfOperationResponseTypeDef,
-    DescribeInstanceAttributeResponseTypeDef,
-    DescribeInstanceResponseTypeDef,
-    DescribeInstanceStorageConfigResponseTypeDef,
-    DescribePhoneNumberResponseTypeDef,
-    DescribePromptResponseTypeDef,
-    DescribeQueueResponseTypeDef,
-    DescribeQuickConnectResponseTypeDef,
-    DescribeRoutingProfileResponseTypeDef,
-    DescribeRuleResponseTypeDef,
-    DescribeSecurityProfileResponseTypeDef,
-    DescribeTrafficDistributionGroupResponseTypeDef,
-    DescribeUserHierarchyGroupResponseTypeDef,
-    DescribeUserHierarchyStructureResponseTypeDef,
-    DescribeUserResponseTypeDef,
-    DescribeVocabularyResponseTypeDef,
+    DeactivateEvaluationFormResponseOutputTypeDef,
+    DeleteVocabularyResponseOutputTypeDef,
+    DescribeAgentStatusResponseOutputTypeDef,
+    DescribeContactEvaluationResponseOutputTypeDef,
+    DescribeContactFlowModuleResponseOutputTypeDef,
+    DescribeContactFlowResponseOutputTypeDef,
+    DescribeContactResponseOutputTypeDef,
+    DescribeEvaluationFormResponseOutputTypeDef,
+    DescribeHoursOfOperationResponseOutputTypeDef,
+    DescribeInstanceAttributeResponseOutputTypeDef,
+    DescribeInstanceResponseOutputTypeDef,
+    DescribeInstanceStorageConfigResponseOutputTypeDef,
+    DescribePhoneNumberResponseOutputTypeDef,
+    DescribePromptResponseOutputTypeDef,
+    DescribeQueueResponseOutputTypeDef,
+    DescribeQuickConnectResponseOutputTypeDef,
+    DescribeRoutingProfileResponseOutputTypeDef,
+    DescribeRuleResponseOutputTypeDef,
+    DescribeSecurityProfileResponseOutputTypeDef,
+    DescribeTrafficDistributionGroupResponseOutputTypeDef,
+    DescribeUserHierarchyGroupResponseOutputTypeDef,
+    DescribeUserHierarchyStructureResponseOutputTypeDef,
+    DescribeUserResponseOutputTypeDef,
+    DescribeVocabularyResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationAnswerInputTypeDef,
     EvaluationFormItemTypeDef,
     EvaluationFormScoringStrategyTypeDef,
     EvaluationNoteTypeDef,
     FiltersTypeDef,
     FilterV2TypeDef,
-    GetContactAttributesResponseTypeDef,
-    GetCurrentMetricDataResponseTypeDef,
-    GetCurrentUserDataResponseTypeDef,
-    GetFederationTokenResponseTypeDef,
-    GetMetricDataResponseTypeDef,
-    GetMetricDataV2ResponseTypeDef,
-    GetPromptFileResponseTypeDef,
-    GetTaskTemplateResponseTypeDef,
-    GetTrafficDistributionResponseTypeDef,
+    GetContactAttributesResponseOutputTypeDef,
+    GetCurrentMetricDataResponseOutputTypeDef,
+    GetCurrentUserDataResponseOutputTypeDef,
+    GetFederationTokenResponseOutputTypeDef,
+    GetMetricDataResponseOutputTypeDef,
+    GetMetricDataV2ResponseOutputTypeDef,
+    GetPromptFileResponseOutputTypeDef,
+    GetTaskTemplateResponseOutputTypeDef,
+    GetTrafficDistributionResponseOutputTypeDef,
     HierarchyStructureUpdateTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationConfigTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
     InstanceStorageConfigTypeDef,
     LexBotTypeDef,
     LexV2BotTypeDef,
-    ListAgentStatusResponseTypeDef,
-    ListApprovedOriginsResponseTypeDef,
-    ListBotsResponseTypeDef,
-    ListContactEvaluationsResponseTypeDef,
-    ListContactFlowModulesResponseTypeDef,
-    ListContactFlowsResponseTypeDef,
-    ListContactReferencesResponseTypeDef,
-    ListDefaultVocabulariesResponseTypeDef,
-    ListEvaluationFormsResponseTypeDef,
-    ListEvaluationFormVersionsResponseTypeDef,
-    ListHoursOfOperationsResponseTypeDef,
-    ListInstanceAttributesResponseTypeDef,
-    ListInstancesResponseTypeDef,
-    ListInstanceStorageConfigsResponseTypeDef,
-    ListIntegrationAssociationsResponseTypeDef,
-    ListLambdaFunctionsResponseTypeDef,
-    ListLexBotsResponseTypeDef,
-    ListPhoneNumbersResponseTypeDef,
-    ListPhoneNumbersV2ResponseTypeDef,
-    ListPromptsResponseTypeDef,
-    ListQueueQuickConnectsResponseTypeDef,
-    ListQueuesResponseTypeDef,
-    ListQuickConnectsResponseTypeDef,
-    ListRoutingProfileQueuesResponseTypeDef,
-    ListRoutingProfilesResponseTypeDef,
-    ListRulesResponseTypeDef,
-    ListSecurityKeysResponseTypeDef,
-    ListSecurityProfilePermissionsResponseTypeDef,
-    ListSecurityProfilesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTaskTemplatesResponseTypeDef,
-    ListTrafficDistributionGroupsResponseTypeDef,
-    ListUseCasesResponseTypeDef,
-    ListUserHierarchyGroupsResponseTypeDef,
-    ListUsersResponseTypeDef,
+    ListAgentStatusResponseOutputTypeDef,
+    ListApprovedOriginsResponseOutputTypeDef,
+    ListBotsResponseOutputTypeDef,
+    ListContactEvaluationsResponseOutputTypeDef,
+    ListContactFlowModulesResponseOutputTypeDef,
+    ListContactFlowsResponseOutputTypeDef,
+    ListContactReferencesResponseOutputTypeDef,
+    ListDefaultVocabulariesResponseOutputTypeDef,
+    ListEvaluationFormsResponseOutputTypeDef,
+    ListEvaluationFormVersionsResponseOutputTypeDef,
+    ListHoursOfOperationsResponseOutputTypeDef,
+    ListInstanceAttributesResponseOutputTypeDef,
+    ListInstancesResponseOutputTypeDef,
+    ListInstanceStorageConfigsResponseOutputTypeDef,
+    ListIntegrationAssociationsResponseOutputTypeDef,
+    ListLambdaFunctionsResponseOutputTypeDef,
+    ListLexBotsResponseOutputTypeDef,
+    ListPhoneNumbersResponseOutputTypeDef,
+    ListPhoneNumbersV2ResponseOutputTypeDef,
+    ListPromptsResponseOutputTypeDef,
+    ListQueueQuickConnectsResponseOutputTypeDef,
+    ListQueuesResponseOutputTypeDef,
+    ListQuickConnectsResponseOutputTypeDef,
+    ListRoutingProfileQueuesResponseOutputTypeDef,
+    ListRoutingProfilesResponseOutputTypeDef,
+    ListRulesResponseOutputTypeDef,
+    ListSecurityKeysResponseOutputTypeDef,
+    ListSecurityProfilePermissionsResponseOutputTypeDef,
+    ListSecurityProfilesResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListTaskTemplatesResponseOutputTypeDef,
+    ListTrafficDistributionGroupsResponseOutputTypeDef,
+    ListUseCasesResponseOutputTypeDef,
+    ListUserHierarchyGroupsResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
     MediaConcurrencyTypeDef,
     MetricV2TypeDef,
-    MonitorContactResponseTypeDef,
+    MonitorContactResponseOutputTypeDef,
     OutboundCallerConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     PersistentChatTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectConfigTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
     ReferenceTypeDef,
-    ReplicateInstanceResponseTypeDef,
+    ReplicateInstanceResponseOutputTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
     RuleActionTypeDef,
     RuleTriggerEventSourceTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
-    SearchHoursOfOperationsResponseTypeDef,
-    SearchPromptsResponseTypeDef,
-    SearchQueuesResponseTypeDef,
-    SearchQuickConnectsResponseTypeDef,
-    SearchResourceTagsResponseTypeDef,
-    SearchRoutingProfilesResponseTypeDef,
-    SearchSecurityProfilesResponseTypeDef,
-    SearchUsersResponseTypeDef,
-    SearchVocabulariesResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseOutputTypeDef,
+    SearchHoursOfOperationsResponseOutputTypeDef,
+    SearchPromptsResponseOutputTypeDef,
+    SearchQueuesResponseOutputTypeDef,
+    SearchQuickConnectsResponseOutputTypeDef,
+    SearchResourceTagsResponseOutputTypeDef,
+    SearchRoutingProfilesResponseOutputTypeDef,
+    SearchSecurityProfilesResponseOutputTypeDef,
+    SearchUsersResponseOutputTypeDef,
+    SearchVocabulariesResponseOutputTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     SecurityProfilesSearchFilterTypeDef,
-    StartChatContactResponseTypeDef,
-    StartContactEvaluationResponseTypeDef,
-    StartContactStreamingResponseTypeDef,
-    StartOutboundVoiceContactResponseTypeDef,
-    StartTaskContactResponseTypeDef,
-    SubmitContactEvaluationResponseTypeDef,
+    StartChatContactResponseOutputTypeDef,
+    StartContactEvaluationResponseOutputTypeDef,
+    StartContactStreamingResponseOutputTypeDef,
+    StartOutboundVoiceContactResponseOutputTypeDef,
+    StartTaskContactResponseOutputTypeDef,
+    SubmitContactEvaluationResponseOutputTypeDef,
     TaskTemplateConstraintsTypeDef,
     TaskTemplateDefaultsTypeDef,
     TaskTemplateFieldTypeDef,
     TelephonyConfigTypeDef,
-    TransferContactResponseTypeDef,
-    UpdateContactEvaluationResponseTypeDef,
-    UpdateEvaluationFormResponseTypeDef,
+    TransferContactResponseOutputTypeDef,
+    UpdateContactEvaluationResponseOutputTypeDef,
+    UpdateEvaluationFormResponseOutputTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
-    UpdatePhoneNumberResponseTypeDef,
-    UpdatePromptResponseTypeDef,
-    UpdateTaskTemplateResponseTypeDef,
+    UpdatePhoneNumberResponseOutputTypeDef,
+    UpdatePromptResponseOutputTypeDef,
+    UpdateTaskTemplateResponseOutputTypeDef,
     UserDataFiltersTypeDef,
     UserIdentityInfoTypeDef,
     UserPhoneConfigTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
     VoiceRecordingConfigurationTypeDef,
 )
@@ -320,15 +320,15 @@
         ConnectClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#exceptions)
         """
     def activate_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int
-    ) -> ActivateEvaluationFormResponseTypeDef:
+    ) -> ActivateEvaluationFormResponseOutputTypeDef:
         """
         Activates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.activate_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#activate_evaluation_form)
         """
     def associate_approved_origin(
@@ -360,15 +360,15 @@
         """
     def associate_instance_storage_config(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         StorageConfig: "InstanceStorageConfigTypeDef"
-    ) -> AssociateInstanceStorageConfigResponseTypeDef:
+    ) -> AssociateInstanceStorageConfigResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_instance_storage_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_instance_storage_config)
         """
     def associate_lambda_function(
@@ -418,15 +418,15 @@
         Associates a set of queues with a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_routing_profile_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_routing_profile_queues)
         """
     def associate_security_key(
         self, *, InstanceId: str, Key: str
-    ) -> AssociateSecurityKeyResponseTypeDef:
+    ) -> AssociateSecurityKeyResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_security_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_security_key)
         """
     def can_paginate(self, operation_name: str) -> bool:
@@ -440,15 +440,15 @@
         self,
         *,
         TargetArn: str,
         PhoneNumber: str,
         PhoneNumberDescription: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...
-    ) -> ClaimPhoneNumberResponseTypeDef:
+    ) -> ClaimPhoneNumberResponseOutputTypeDef:
         """
         Claims an available phone number to your Amazon Connect instance or traffic
         distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.claim_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#claim_phone_number)
         """
@@ -464,15 +464,15 @@
         *,
         InstanceId: str,
         Name: str,
         State: AgentStatusStateType,
         Description: str = ...,
         DisplayOrder: int = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateAgentStatusResponseTypeDef:
+    ) -> CreateAgentStatusResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_agent_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_agent_status)
         """
     def create_contact_flow(
@@ -480,15 +480,15 @@
         *,
         InstanceId: str,
         Name: str,
         Type: ContactFlowTypeType,
         Content: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateContactFlowResponseTypeDef:
+    ) -> CreateContactFlowResponseOutputTypeDef:
         """
         Creates a flow for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_contact_flow)
         """
     def create_contact_flow_module(
@@ -496,15 +496,15 @@
         *,
         InstanceId: str,
         Name: str,
         Content: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...
-    ) -> CreateContactFlowModuleResponseTypeDef:
+    ) -> CreateContactFlowModuleResponseOutputTypeDef:
         """
         Creates a flow module for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow_module)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_contact_flow_module)
         """
     def create_evaluation_form(
@@ -512,15 +512,15 @@
         *,
         InstanceId: str,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         Description: str = ...,
         ScoringStrategy: "EvaluationFormScoringStrategyTypeDef" = ...,
         ClientToken: str = ...
-    ) -> CreateEvaluationFormResponseTypeDef:
+    ) -> CreateEvaluationFormResponseOutputTypeDef:
         """
         Creates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_evaluation_form)
         """
     def create_hours_of_operation(
@@ -528,15 +528,15 @@
         *,
         InstanceId: str,
         Name: str,
         TimeZone: str,
         Config: Sequence["HoursOfOperationConfigTypeDef"],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateHoursOfOperationResponseTypeDef:
+    ) -> CreateHoursOfOperationResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_hours_of_operation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_hours_of_operation)
         """
     def create_instance(
@@ -544,15 +544,15 @@
         *,
         IdentityManagementType: DirectoryTypeType,
         InboundCallsEnabled: bool,
         OutboundCallsEnabled: bool,
         ClientToken: str = ...,
         InstanceAlias: str = ...,
         DirectoryId: str = ...
-    ) -> CreateInstanceResponseTypeDef:
+    ) -> CreateInstanceResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_instance)
         """
     def create_integration_association(
@@ -561,45 +561,45 @@
         InstanceId: str,
         IntegrationType: IntegrationTypeType,
         IntegrationArn: str,
         SourceApplicationUrl: str = ...,
         SourceApplicationName: str = ...,
         SourceType: SourceTypeType = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateIntegrationAssociationResponseTypeDef:
+    ) -> CreateIntegrationAssociationResponseOutputTypeDef:
         """
         Creates an Amazon Web Services resource association with an Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_integration_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_integration_association)
         """
     def create_participant(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ParticipantDetails: "ParticipantDetailsToAddTypeDef",
         ClientToken: str = ...
-    ) -> CreateParticipantResponseTypeDef:
+    ) -> CreateParticipantResponseOutputTypeDef:
         """
         Adds a new participant into an on-going chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_participant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_participant)
         """
     def create_prompt(
         self,
         *,
         InstanceId: str,
         Name: str,
         S3Uri: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreatePromptResponseTypeDef:
+    ) -> CreatePromptResponseOutputTypeDef:
         """
         Creates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_prompt)
         """
     def create_queue(
@@ -609,30 +609,30 @@
         Name: str,
         HoursOfOperationId: str,
         Description: str = ...,
         OutboundCallerConfig: "OutboundCallerConfigTypeDef" = ...,
         MaxContacts: int = ...,
         QuickConnectIds: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateQueueResponseTypeDef:
+    ) -> CreateQueueResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_queue)
         """
     def create_quick_connect(
         self,
         *,
         InstanceId: str,
         Name: str,
         QuickConnectConfig: "QuickConnectConfigTypeDef",
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateQuickConnectResponseTypeDef:
+    ) -> CreateQuickConnectResponseOutputTypeDef:
         """
         Creates a quick connect for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_quick_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_quick_connect)
         """
     def create_routing_profile(
@@ -641,15 +641,15 @@
         InstanceId: str,
         Name: str,
         Description: str,
         DefaultOutboundQueueId: str,
         MediaConcurrencies: Sequence["MediaConcurrencyTypeDef"],
         QueueConfigs: Sequence["RoutingProfileQueueConfigTypeDef"] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateRoutingProfileResponseTypeDef:
+    ) -> CreateRoutingProfileResponseOutputTypeDef:
         """
         Creates a new routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_routing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_routing_profile)
         """
     def create_rule(
@@ -658,15 +658,15 @@
         InstanceId: str,
         Name: str,
         TriggerEventSource: "RuleTriggerEventSourceTypeDef",
         Function: str,
         Actions: Sequence["RuleActionTypeDef"],
         PublishStatus: RulePublishStatusType,
         ClientToken: str = ...
-    ) -> CreateRuleResponseTypeDef:
+    ) -> CreateRuleResponseOutputTypeDef:
         """
         Creates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_rule)
         """
     def create_security_profile(
@@ -675,15 +675,15 @@
         SecurityProfileName: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...
-    ) -> CreateSecurityProfileResponseTypeDef:
+    ) -> CreateSecurityProfileResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_security_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_security_profile)
         """
     def create_task_template(
@@ -694,45 +694,45 @@
         Fields: Sequence["TaskTemplateFieldTypeDef"],
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: "TaskTemplateConstraintsTypeDef" = ...,
         Defaults: "TaskTemplateDefaultsTypeDef" = ...,
         Status: TaskTemplateStatusType = ...,
         ClientToken: str = ...
-    ) -> CreateTaskTemplateResponseTypeDef:
+    ) -> CreateTaskTemplateResponseOutputTypeDef:
         """
         Creates a new task template in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_task_template)
         """
     def create_traffic_distribution_group(
         self,
         *,
         Name: str,
         InstanceId: str,
         Description: str = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateTrafficDistributionGroupResponseTypeDef:
+    ) -> CreateTrafficDistributionGroupResponseOutputTypeDef:
         """
         Creates a traffic distribution group given an Amazon Connect instance that has
         been replicated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_traffic_distribution_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_traffic_distribution_group)
         """
     def create_use_case(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         UseCaseType: UseCaseTypeType,
         Tags: Mapping[str, str] = ...
-    ) -> CreateUseCaseResponseTypeDef:
+    ) -> CreateUseCaseResponseOutputTypeDef:
         """
         Creates a use case for an integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_use_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_use_case)
         """
     def create_user(
@@ -744,24 +744,24 @@
         RoutingProfileId: str,
         InstanceId: str,
         Password: str = ...,
         IdentityInfo: "UserIdentityInfoTypeDef" = ...,
         DirectoryUserId: str = ...,
         HierarchyGroupId: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateUserResponseTypeDef:
+    ) -> CreateUserResponseOutputTypeDef:
         """
         Creates a user account for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_user)
         """
     def create_user_hierarchy_group(
         self, *, Name: str, InstanceId: str, ParentGroupId: str = ..., Tags: Mapping[str, str] = ...
-    ) -> CreateUserHierarchyGroupResponseTypeDef:
+    ) -> CreateUserHierarchyGroupResponseOutputTypeDef:
         """
         Creates a new user hierarchy group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_user_hierarchy_group)
         """
     def create_vocabulary(
@@ -769,24 +769,24 @@
         *,
         InstanceId: str,
         VocabularyName: str,
         LanguageCode: VocabularyLanguageCodeType,
         Content: str,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateVocabularyResponseTypeDef:
+    ) -> CreateVocabularyResponseOutputTypeDef:
         """
         Creates a custom vocabulary associated with your Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_vocabulary)
         """
     def deactivate_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int
-    ) -> DeactivateEvaluationFormResponseTypeDef:
+    ) -> DeactivateEvaluationFormResponseOutputTypeDef:
         """
         Deactivates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.deactivate_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#deactivate_evaluation_form)
         """
     def delete_contact_evaluation(
@@ -936,202 +936,208 @@
         Deletes an existing user hierarchy group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_user_hierarchy_group)
         """
     def delete_vocabulary(
         self, *, InstanceId: str, VocabularyId: str
-    ) -> DeleteVocabularyResponseTypeDef:
+    ) -> DeleteVocabularyResponseOutputTypeDef:
         """
         Deletes the vocabulary that has the given identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_vocabulary)
         """
     def describe_agent_status(
         self, *, InstanceId: str, AgentStatusId: str
-    ) -> DescribeAgentStatusResponseTypeDef:
+    ) -> DescribeAgentStatusResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_agent_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_agent_status)
         """
     def describe_contact(
         self, *, InstanceId: str, ContactId: str
-    ) -> DescribeContactResponseTypeDef:
+    ) -> DescribeContactResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact)
         """
     def describe_contact_evaluation(
         self, *, InstanceId: str, EvaluationId: str
-    ) -> DescribeContactEvaluationResponseTypeDef:
+    ) -> DescribeContactEvaluationResponseOutputTypeDef:
         """
         Describes a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_evaluation)
         """
     def describe_contact_flow(
         self, *, InstanceId: str, ContactFlowId: str
-    ) -> DescribeContactFlowResponseTypeDef:
+    ) -> DescribeContactFlowResponseOutputTypeDef:
         """
         Describes the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_flow)
         """
     def describe_contact_flow_module(
         self, *, InstanceId: str, ContactFlowModuleId: str
-    ) -> DescribeContactFlowModuleResponseTypeDef:
+    ) -> DescribeContactFlowModuleResponseOutputTypeDef:
         """
         Describes the specified flow module.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_flow_module)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_flow_module)
         """
     def describe_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int = ...
-    ) -> DescribeEvaluationFormResponseTypeDef:
+    ) -> DescribeEvaluationFormResponseOutputTypeDef:
         """
         Describes an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_evaluation_form)
         """
     def describe_hours_of_operation(
         self, *, InstanceId: str, HoursOfOperationId: str
-    ) -> DescribeHoursOfOperationResponseTypeDef:
+    ) -> DescribeHoursOfOperationResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_hours_of_operation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_hours_of_operation)
         """
-    def describe_instance(self, *, InstanceId: str) -> DescribeInstanceResponseTypeDef:
+    def describe_instance(self, *, InstanceId: str) -> DescribeInstanceResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance)
         """
     def describe_instance_attribute(
         self, *, InstanceId: str, AttributeType: InstanceAttributeTypeType
-    ) -> DescribeInstanceAttributeResponseTypeDef:
+    ) -> DescribeInstanceAttributeResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_attribute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance_attribute)
         """
     def describe_instance_storage_config(
         self, *, InstanceId: str, AssociationId: str, ResourceType: InstanceStorageResourceTypeType
-    ) -> DescribeInstanceStorageConfigResponseTypeDef:
+    ) -> DescribeInstanceStorageConfigResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_storage_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance_storage_config)
         """
-    def describe_phone_number(self, *, PhoneNumberId: str) -> DescribePhoneNumberResponseTypeDef:
+    def describe_phone_number(
+        self, *, PhoneNumberId: str
+    ) -> DescribePhoneNumberResponseOutputTypeDef:
         """
         Gets details and status of a phone number that’s claimed to your Amazon Connect
         instance or traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_phone_number)
         """
-    def describe_prompt(self, *, InstanceId: str, PromptId: str) -> DescribePromptResponseTypeDef:
+    def describe_prompt(
+        self, *, InstanceId: str, PromptId: str
+    ) -> DescribePromptResponseOutputTypeDef:
         """
         Describes the prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_prompt)
         """
-    def describe_queue(self, *, InstanceId: str, QueueId: str) -> DescribeQueueResponseTypeDef:
+    def describe_queue(
+        self, *, InstanceId: str, QueueId: str
+    ) -> DescribeQueueResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_queue)
         """
     def describe_quick_connect(
         self, *, InstanceId: str, QuickConnectId: str
-    ) -> DescribeQuickConnectResponseTypeDef:
+    ) -> DescribeQuickConnectResponseOutputTypeDef:
         """
         Describes the quick connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_quick_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_quick_connect)
         """
     def describe_routing_profile(
         self, *, InstanceId: str, RoutingProfileId: str
-    ) -> DescribeRoutingProfileResponseTypeDef:
+    ) -> DescribeRoutingProfileResponseOutputTypeDef:
         """
         Describes the specified routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_routing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_routing_profile)
         """
-    def describe_rule(self, *, InstanceId: str, RuleId: str) -> DescribeRuleResponseTypeDef:
+    def describe_rule(self, *, InstanceId: str, RuleId: str) -> DescribeRuleResponseOutputTypeDef:
         """
         Describes a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_rule)
         """
     def describe_security_profile(
         self, *, SecurityProfileId: str, InstanceId: str
-    ) -> DescribeSecurityProfileResponseTypeDef:
+    ) -> DescribeSecurityProfileResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_security_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_security_profile)
         """
     def describe_traffic_distribution_group(
         self, *, TrafficDistributionGroupId: str
-    ) -> DescribeTrafficDistributionGroupResponseTypeDef:
+    ) -> DescribeTrafficDistributionGroupResponseOutputTypeDef:
         """
         Gets details and status of a traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_traffic_distribution_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_traffic_distribution_group)
         """
-    def describe_user(self, *, UserId: str, InstanceId: str) -> DescribeUserResponseTypeDef:
+    def describe_user(self, *, UserId: str, InstanceId: str) -> DescribeUserResponseOutputTypeDef:
         """
         Describes the specified user account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user)
         """
     def describe_user_hierarchy_group(
         self, *, HierarchyGroupId: str, InstanceId: str
-    ) -> DescribeUserHierarchyGroupResponseTypeDef:
+    ) -> DescribeUserHierarchyGroupResponseOutputTypeDef:
         """
         Describes the specified hierarchy group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user_hierarchy_group)
         """
     def describe_user_hierarchy_structure(
         self, *, InstanceId: str
-    ) -> DescribeUserHierarchyStructureResponseTypeDef:
+    ) -> DescribeUserHierarchyStructureResponseOutputTypeDef:
         """
         Describes the hierarchy structure of the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user_hierarchy_structure)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user_hierarchy_structure)
         """
     def describe_vocabulary(
         self, *, InstanceId: str, VocabularyId: str
-    ) -> DescribeVocabularyResponseTypeDef:
+    ) -> DescribeVocabularyResponseOutputTypeDef:
         """
         Describes the specified vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_vocabulary)
         """
     def disassociate_approved_origin(
@@ -1241,15 +1247,15 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#generate_presigned_url)
         """
     def get_contact_attributes(
         self, *, InstanceId: str, InitialContactId: str
-    ) -> GetContactAttributesResponseTypeDef:
+    ) -> GetContactAttributesResponseOutputTypeDef:
         """
         Retrieves the contact attributes for the specified contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_contact_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_contact_attributes)
         """
     def get_current_metric_data(
@@ -1258,36 +1264,36 @@
         InstanceId: str,
         Filters: "FiltersTypeDef",
         CurrentMetrics: Sequence["CurrentMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortCriteria: Sequence["CurrentMetricSortCriteriaTypeDef"] = ...
-    ) -> GetCurrentMetricDataResponseTypeDef:
+    ) -> GetCurrentMetricDataResponseOutputTypeDef:
         """
         Gets the real-time metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_current_metric_data)
         """
     def get_current_user_data(
         self,
         *,
         InstanceId: str,
         Filters: "UserDataFiltersTypeDef",
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetCurrentUserDataResponseTypeDef:
+    ) -> GetCurrentUserDataResponseOutputTypeDef:
         """
         Gets the real-time active user data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_user_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_current_user_data)
         """
-    def get_federation_token(self, *, InstanceId: str) -> GetFederationTokenResponseTypeDef:
+    def get_federation_token(self, *, InstanceId: str) -> GetFederationTokenResponseOutputTypeDef:
         """
         Retrieves a token for federation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_federation_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_federation_token)
         """
     def get_metric_data(
@@ -1297,15 +1303,15 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: "FiltersTypeDef",
         HistoricalMetrics: Sequence["HistoricalMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetMetricDataResponseTypeDef:
+    ) -> GetMetricDataResponseOutputTypeDef:
         """
         Gets historical metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data)
         """
     def get_metric_data_v2(
@@ -1315,251 +1321,253 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: Sequence["FilterV2TypeDef"],
         Metrics: Sequence["MetricV2TypeDef"],
         Groupings: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetMetricDataV2ResponseTypeDef:
+    ) -> GetMetricDataV2ResponseOutputTypeDef:
         """
         Gets metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data_v2)
         """
-    def get_prompt_file(self, *, InstanceId: str, PromptId: str) -> GetPromptFileResponseTypeDef:
+    def get_prompt_file(
+        self, *, InstanceId: str, PromptId: str
+    ) -> GetPromptFileResponseOutputTypeDef:
         """
         Gets the prompt file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_prompt_file)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_prompt_file)
         """
     def get_task_template(
         self, *, InstanceId: str, TaskTemplateId: str, SnapshotVersion: str = ...
-    ) -> GetTaskTemplateResponseTypeDef:
+    ) -> GetTaskTemplateResponseOutputTypeDef:
         """
         Gets details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_task_template)
         """
-    def get_traffic_distribution(self, *, Id: str) -> GetTrafficDistributionResponseTypeDef:
+    def get_traffic_distribution(self, *, Id: str) -> GetTrafficDistributionResponseOutputTypeDef:
         """
         Retrieves the current traffic distribution for a given traffic distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_traffic_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_traffic_distribution)
         """
     def list_agent_statuses(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         AgentStatusTypes: Sequence[AgentStatusTypeType] = ...
-    ) -> ListAgentStatusResponseTypeDef:
+    ) -> ListAgentStatusResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_agent_statuses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_agent_statuses)
         """
     def list_approved_origins(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListApprovedOriginsResponseTypeDef:
+    ) -> ListApprovedOriginsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_approved_origins)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_approved_origins)
         """
     def list_bots(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListBotsResponseTypeDef:
+    ) -> ListBotsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_bots)
         """
     def list_contact_evaluations(
         self, *, InstanceId: str, ContactId: str, NextToken: str = ...
-    ) -> ListContactEvaluationsResponseTypeDef:
+    ) -> ListContactEvaluationsResponseOutputTypeDef:
         """
         Lists contact evaluations in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_evaluations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_evaluations)
         """
     def list_contact_flow_modules(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         ContactFlowModuleState: ContactFlowModuleStateType = ...
-    ) -> ListContactFlowModulesResponseTypeDef:
+    ) -> ListContactFlowModulesResponseOutputTypeDef:
         """
         Provides information about the flow modules for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flow_modules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_flow_modules)
         """
     def list_contact_flows(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListContactFlowsResponseTypeDef:
+    ) -> ListContactFlowsResponseOutputTypeDef:
         """
         Provides information about the flows for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_flows)
         """
     def list_contact_references(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
         NextToken: str = ...
-    ) -> ListContactReferencesResponseTypeDef:
+    ) -> ListContactReferencesResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_references)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_references)
         """
     def list_default_vocabularies(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> ListDefaultVocabulariesResponseTypeDef:
+    ) -> ListDefaultVocabulariesResponseOutputTypeDef:
         """
         Lists the default vocabularies for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_default_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_default_vocabularies)
         """
     def list_evaluation_form_versions(
         self, *, InstanceId: str, EvaluationFormId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListEvaluationFormVersionsResponseTypeDef:
+    ) -> ListEvaluationFormVersionsResponseOutputTypeDef:
         """
         Lists versions of an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_evaluation_form_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_evaluation_form_versions)
         """
     def list_evaluation_forms(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListEvaluationFormsResponseTypeDef:
+    ) -> ListEvaluationFormsResponseOutputTypeDef:
         """
         Lists evaluation forms in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_evaluation_forms)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_evaluation_forms)
         """
     def list_hours_of_operations(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListHoursOfOperationsResponseTypeDef:
+    ) -> ListHoursOfOperationsResponseOutputTypeDef:
         """
         Provides information about the hours of operation for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_hours_of_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_hours_of_operations)
         """
     def list_instance_attributes(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListInstanceAttributesResponseTypeDef:
+    ) -> ListInstanceAttributesResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instance_attributes)
         """
     def list_instance_storage_configs(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListInstanceStorageConfigsResponseTypeDef:
+    ) -> ListInstanceStorageConfigsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_storage_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instance_storage_configs)
         """
     def list_instances(
         self, *, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListInstancesResponseTypeDef:
+    ) -> ListInstancesResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instances)
         """
     def list_integration_associations(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListIntegrationAssociationsResponseTypeDef:
+    ) -> ListIntegrationAssociationsResponseOutputTypeDef:
         """
         Provides summary information about the Amazon Web Services resource associations
         for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_integration_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_integration_associations)
         """
     def list_lambda_functions(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListLambdaFunctionsResponseTypeDef:
+    ) -> ListLambdaFunctionsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_lambda_functions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_lambda_functions)
         """
     def list_lex_bots(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListLexBotsResponseTypeDef:
+    ) -> ListLexBotsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_lex_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_lex_bots)
         """
     def list_phone_numbers(
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListPhoneNumbersResponseTypeDef:
+    ) -> ListPhoneNumbersResponseOutputTypeDef:
         """
         Provides information about the phone numbers for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_phone_numbers)
         """
@@ -1568,82 +1576,82 @@
         *,
         TargetArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberPrefix: str = ...
-    ) -> ListPhoneNumbersV2ResponseTypeDef:
+    ) -> ListPhoneNumbersV2ResponseOutputTypeDef:
         """
         Lists phone numbers claimed to your Amazon Connect instance or traffic
         distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_phone_numbers_v2)
         """
     def list_prompts(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListPromptsResponseTypeDef:
+    ) -> ListPromptsResponseOutputTypeDef:
         """
         Provides information about the prompts for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_prompts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_prompts)
         """
     def list_queue_quick_connects(
         self, *, InstanceId: str, QueueId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListQueueQuickConnectsResponseTypeDef:
+    ) -> ListQueueQuickConnectsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queue_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_queue_quick_connects)
         """
     def list_queues(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListQueuesResponseTypeDef:
+    ) -> ListQueuesResponseOutputTypeDef:
         """
         Provides information about the queues for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_queues)
         """
     def list_quick_connects(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         QuickConnectTypes: Sequence[QuickConnectTypeType] = ...
-    ) -> ListQuickConnectsResponseTypeDef:
+    ) -> ListQuickConnectsResponseOutputTypeDef:
         """
         Provides information about the quick connects for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_quick_connects)
         """
     def list_routing_profile_queues(
         self, *, InstanceId: str, RoutingProfileId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListRoutingProfileQueuesResponseTypeDef:
+    ) -> ListRoutingProfileQueuesResponseOutputTypeDef:
         """
         Lists the queues associated with a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_routing_profile_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_routing_profile_queues)
         """
     def list_routing_profiles(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListRoutingProfilesResponseTypeDef:
+    ) -> ListRoutingProfilesResponseOutputTypeDef:
         """
         Provides summary information about the routing profiles for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_routing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_routing_profiles)
         """
@@ -1651,112 +1659,114 @@
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> ListRulesResponseTypeDef:
+    ) -> ListRulesResponseOutputTypeDef:
         """
         List all rules for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_rules)
         """
     def list_security_keys(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListSecurityKeysResponseTypeDef:
+    ) -> ListSecurityKeysResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_keys)
         """
     def list_security_profile_permissions(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListSecurityProfilePermissionsResponseTypeDef:
+    ) -> ListSecurityProfilePermissionsResponseOutputTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profile_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_profile_permissions)
         """
     def list_security_profiles(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListSecurityProfilesResponseTypeDef:
+    ) -> ListSecurityProfilesResponseOutputTypeDef:
         """
         Provides summary information about the security profiles for the specified
         Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_profiles)
         """
-    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
+    def list_tags_for_resource(
+        self, *, resourceArn: str
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_tags_for_resource)
         """
     def list_task_templates(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: TaskTemplateStatusType = ...,
         Name: str = ...
-    ) -> ListTaskTemplatesResponseTypeDef:
+    ) -> ListTaskTemplatesResponseOutputTypeDef:
         """
         Lists task templates for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_task_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_task_templates)
         """
     def list_traffic_distribution_groups(
         self, *, MaxResults: int = ..., NextToken: str = ..., InstanceId: str = ...
-    ) -> ListTrafficDistributionGroupsResponseTypeDef:
+    ) -> ListTrafficDistributionGroupsResponseOutputTypeDef:
         """
         Lists traffic distribution groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_traffic_distribution_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_traffic_distribution_groups)
         """
     def list_use_cases(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListUseCasesResponseTypeDef:
+    ) -> ListUseCasesResponseOutputTypeDef:
         """
         Lists the use cases for the integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_use_cases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_use_cases)
         """
     def list_user_hierarchy_groups(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListUserHierarchyGroupsResponseTypeDef:
+    ) -> ListUserHierarchyGroupsResponseOutputTypeDef:
         """
         Provides summary information about the hierarchy groups for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_user_hierarchy_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_user_hierarchy_groups)
         """
     def list_users(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListUsersResponseTypeDef:
+    ) -> ListUsersResponseOutputTypeDef:
         """
         Provides summary information about the users for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_users)
         """
@@ -1764,15 +1774,15 @@
         self,
         *,
         InstanceId: str,
         ContactId: str,
         UserId: str,
         AllowedMonitorCapabilities: Sequence[MonitorCapabilityType] = ...,
         ClientToken: str = ...
-    ) -> MonitorContactResponseTypeDef:
+    ) -> MonitorContactResponseOutputTypeDef:
         """
         Initiates silent monitoring of a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.monitor_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#monitor_contact)
         """
     def put_user_status(
@@ -1792,15 +1802,15 @@
         traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.release_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#release_phone_number)
         """
     def replicate_instance(
         self, *, InstanceId: str, ReplicaRegion: str, ReplicaAlias: str, ClientToken: str = ...
-    ) -> ReplicateInstanceResponseTypeDef:
+    ) -> ReplicateInstanceResponseOutputTypeDef:
         """
         Replicates an Amazon Connect instance in the specified Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.replicate_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#replicate_instance)
         """
@@ -1819,15 +1829,15 @@
         *,
         TargetArn: str,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         PhoneNumberPrefix: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> SearchAvailablePhoneNumbersResponseTypeDef:
+    ) -> SearchAvailablePhoneNumbersResponseOutputTypeDef:
         """
         Searches for available phone numbers that you can claim to your Amazon Connect
         instance or traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_available_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_available_phone_numbers)
         """
@@ -1835,15 +1845,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "HoursOfOperationSearchFilterTypeDef" = ...,
         SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...
-    ) -> SearchHoursOfOperationsResponseTypeDef:
+    ) -> SearchHoursOfOperationsResponseOutputTypeDef:
         """
         Searches the hours of operation in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_hours_of_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_hours_of_operations)
         """
@@ -1851,75 +1861,75 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "PromptSearchFilterTypeDef" = ...,
         SearchCriteria: "PromptSearchCriteriaTypeDef" = ...
-    ) -> SearchPromptsResponseTypeDef:
+    ) -> SearchPromptsResponseOutputTypeDef:
         """
         Searches prompts in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_prompts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_prompts)
         """
     def search_queues(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "QueueSearchFilterTypeDef" = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...
-    ) -> SearchQueuesResponseTypeDef:
+    ) -> SearchQueuesResponseOutputTypeDef:
         """
         Searches queues in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_queues)
         """
     def search_quick_connects(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "QuickConnectSearchFilterTypeDef" = ...,
         SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...
-    ) -> SearchQuickConnectsResponseTypeDef:
+    ) -> SearchQuickConnectsResponseOutputTypeDef:
         """
         Searches quick connects in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_quick_connects)
         """
     def search_resource_tags(
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "ResourceTagsSearchCriteriaTypeDef" = ...
-    ) -> SearchResourceTagsResponseTypeDef:
+    ) -> SearchResourceTagsResponseOutputTypeDef:
         """
         Searches tags used in an Amazon Connect instance using optional search criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_resource_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_resource_tags)
         """
     def search_routing_profiles(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "RoutingProfileSearchFilterTypeDef" = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...
-    ) -> SearchRoutingProfilesResponseTypeDef:
+    ) -> SearchRoutingProfilesResponseOutputTypeDef:
         """
         Searches routing profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_routing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_routing_profiles)
         """
@@ -1927,15 +1937,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: "SecurityProfilesSearchFilterTypeDef" = ...
-    ) -> SearchSecurityProfilesResponseTypeDef:
+    ) -> SearchSecurityProfilesResponseOutputTypeDef:
         """
         Searches security profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_security_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_security_profiles)
         """
@@ -1943,15 +1953,15 @@
         self,
         *,
         InstanceId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "UserSearchFilterTypeDef" = ...,
         SearchCriteria: "UserSearchCriteriaTypeDef" = ...
-    ) -> SearchUsersResponseTypeDef:
+    ) -> SearchUsersResponseOutputTypeDef:
         """
         Searches users in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_users)
         """
     def search_vocabularies(
@@ -1959,15 +1969,15 @@
         *,
         InstanceId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
         LanguageCode: VocabularyLanguageCodeType = ...
-    ) -> SearchVocabulariesResponseTypeDef:
+    ) -> SearchVocabulariesResponseOutputTypeDef:
         """
         Searches for vocabularies within a specific Amazon Connect instance using
         `State`, `NameStartsWith`, and `LanguageCode`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_vocabularies)
         """
@@ -1980,24 +1990,24 @@
         Attributes: Mapping[str, str] = ...,
         InitialMessage: "ChatMessageTypeDef" = ...,
         ClientToken: str = ...,
         ChatDurationInMinutes: int = ...,
         SupportedMessagingContentTypes: Sequence[str] = ...,
         PersistentChat: "PersistentChatTypeDef" = ...,
         RelatedContactId: str = ...
-    ) -> StartChatContactResponseTypeDef:
+    ) -> StartChatContactResponseOutputTypeDef:
         """
         Initiates a flow to start a new chat for the customer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_chat_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_chat_contact)
         """
     def start_contact_evaluation(
         self, *, InstanceId: str, ContactId: str, EvaluationFormId: str, ClientToken: str = ...
-    ) -> StartContactEvaluationResponseTypeDef:
+    ) -> StartContactEvaluationResponseOutputTypeDef:
         """
         Starts an empty evaluation in the specified Amazon Connect instance, using the
         given evaluation form for the particular contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_contact_evaluation)
         """
@@ -2019,15 +2029,15 @@
     def start_contact_streaming(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ChatStreamingConfiguration: "ChatStreamingConfigurationTypeDef",
         ClientToken: str
-    ) -> StartContactStreamingResponseTypeDef:
+    ) -> StartContactStreamingResponseOutputTypeDef:
         """
         Initiates real-time message streaming for a new chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_streaming)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_contact_streaming)
         """
     def start_outbound_voice_contact(
@@ -2039,15 +2049,15 @@
         ClientToken: str = ...,
         SourcePhoneNumber: str = ...,
         QueueId: str = ...,
         Attributes: Mapping[str, str] = ...,
         AnswerMachineDetectionConfig: "AnswerMachineDetectionConfigTypeDef" = ...,
         CampaignId: str = ...,
         TrafficType: TrafficTypeType = ...
-    ) -> StartOutboundVoiceContactResponseTypeDef:
+    ) -> StartOutboundVoiceContactResponseOutputTypeDef:
         """
         Places an outbound call to a contact, and then initiates the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_outbound_voice_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_outbound_voice_contact)
         """
     def start_task_contact(
@@ -2061,15 +2071,15 @@
         References: Mapping[str, "ReferenceTypeDef"] = ...,
         Description: str = ...,
         ClientToken: str = ...,
         ScheduledTime: Union[datetime, str] = ...,
         TaskTemplateId: str = ...,
         QuickConnectId: str = ...,
         RelatedContactId: str = ...
-    ) -> StartTaskContactResponseTypeDef:
+    ) -> StartTaskContactResponseOutputTypeDef:
         """
         Initiates a flow to start a new task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_task_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_task_contact)
         """
     def stop_contact(self, *, ContactId: str, InstanceId: str) -> Dict[str, Any]:
@@ -2100,15 +2110,15 @@
     def submit_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, "EvaluationAnswerInputTypeDef"] = ...,
         Notes: Mapping[str, "EvaluationNoteTypeDef"] = ...
-    ) -> SubmitContactEvaluationResponseTypeDef:
+    ) -> SubmitContactEvaluationResponseOutputTypeDef:
         """
         Submits a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.submit_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#submit_contact_evaluation)
         """
     def suspend_contact_recording(
@@ -2135,15 +2145,15 @@
         *,
         InstanceId: str,
         ContactId: str,
         ContactFlowId: str,
         QueueId: str = ...,
         UserId: str = ...,
         ClientToken: str = ...
-    ) -> TransferContactResponseTypeDef:
+    ) -> TransferContactResponseOutputTypeDef:
         """
         Transfers contacts from one agent or queue to another agent or queue at any
         point after a contact is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.transfer_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#transfer_contact)
         """
@@ -2201,15 +2211,15 @@
     def update_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, "EvaluationAnswerInputTypeDef"] = ...,
         Notes: Mapping[str, "EvaluationNoteTypeDef"] = ...
-    ) -> UpdateContactEvaluationResponseTypeDef:
+    ) -> UpdateContactEvaluationResponseOutputTypeDef:
         """
         Updates details about a contact evaluation in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_contact_evaluation)
         """
@@ -2287,15 +2297,15 @@
         EvaluationFormVersion: int,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         CreateNewVersion: bool = ...,
         Description: str = ...,
         ScoringStrategy: "EvaluationFormScoringStrategyTypeDef" = ...,
         ClientToken: str = ...
-    ) -> UpdateEvaluationFormResponseTypeDef:
+    ) -> UpdateEvaluationFormResponseOutputTypeDef:
         """
         Updates details about a specific evaluation form version in the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_evaluation_form)
         """
@@ -2350,15 +2360,15 @@
         when agents are automatically disconnected from a chat due to idleness.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_participant_role_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_participant_role_config)
         """
     def update_phone_number(
         self, *, PhoneNumberId: str, TargetArn: str, ClientToken: str = ...
-    ) -> UpdatePhoneNumberResponseTypeDef:
+    ) -> UpdatePhoneNumberResponseOutputTypeDef:
         """
         Updates your claimed phone number from its current Amazon Connect instance or
         traffic distribution group to another Amazon Connect instance or traffic
         distribution group in the same Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_phone_number)
@@ -2367,15 +2377,15 @@
         self,
         *,
         InstanceId: str,
         PromptId: str,
         Name: str = ...,
         Description: str = ...,
         S3Uri: str = ...
-    ) -> UpdatePromptResponseTypeDef:
+    ) -> UpdatePromptResponseOutputTypeDef:
         """
         Updates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_prompt)
         """
     def update_queue_hours_of_operation(
@@ -2530,15 +2540,15 @@
         Name: str = ...,
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: "TaskTemplateConstraintsTypeDef" = ...,
         Defaults: "TaskTemplateDefaultsTypeDef" = ...,
         Status: TaskTemplateStatusType = ...,
         Fields: Sequence["TaskTemplateFieldTypeDef"] = ...
-    ) -> UpdateTaskTemplateResponseTypeDef:
+    ) -> UpdateTaskTemplateResponseOutputTypeDef:
         """
         Updates details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_task_template)
         """
```

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect/literals.py` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect/literals.pyi` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect/paginator.py` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -129,72 +129,72 @@
     RulePublishStatusType,
     TaskTemplateStatusType,
     VocabularyLanguageCodeType,
     VocabularyStateType,
 )
 from .type_defs import (
     FiltersTypeDef,
-    GetMetricDataResponseTypeDef,
+    GetMetricDataResponseOutputTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
-    ListAgentStatusResponseTypeDef,
-    ListApprovedOriginsResponseTypeDef,
-    ListBotsResponseTypeDef,
-    ListContactEvaluationsResponseTypeDef,
-    ListContactFlowModulesResponseTypeDef,
-    ListContactFlowsResponseTypeDef,
-    ListContactReferencesResponseTypeDef,
-    ListDefaultVocabulariesResponseTypeDef,
-    ListEvaluationFormsResponseTypeDef,
-    ListEvaluationFormVersionsResponseTypeDef,
-    ListHoursOfOperationsResponseTypeDef,
-    ListInstanceAttributesResponseTypeDef,
-    ListInstancesResponseTypeDef,
-    ListInstanceStorageConfigsResponseTypeDef,
-    ListIntegrationAssociationsResponseTypeDef,
-    ListLambdaFunctionsResponseTypeDef,
-    ListLexBotsResponseTypeDef,
-    ListPhoneNumbersResponseTypeDef,
-    ListPhoneNumbersV2ResponseTypeDef,
-    ListPromptsResponseTypeDef,
-    ListQueueQuickConnectsResponseTypeDef,
-    ListQueuesResponseTypeDef,
-    ListQuickConnectsResponseTypeDef,
-    ListRoutingProfileQueuesResponseTypeDef,
-    ListRoutingProfilesResponseTypeDef,
-    ListRulesResponseTypeDef,
-    ListSecurityKeysResponseTypeDef,
-    ListSecurityProfilePermissionsResponseTypeDef,
-    ListSecurityProfilesResponseTypeDef,
-    ListTaskTemplatesResponseTypeDef,
-    ListTrafficDistributionGroupsResponseTypeDef,
-    ListUseCasesResponseTypeDef,
-    ListUserHierarchyGroupsResponseTypeDef,
-    ListUsersResponseTypeDef,
+    ListAgentStatusResponseOutputTypeDef,
+    ListApprovedOriginsResponseOutputTypeDef,
+    ListBotsResponseOutputTypeDef,
+    ListContactEvaluationsResponseOutputTypeDef,
+    ListContactFlowModulesResponseOutputTypeDef,
+    ListContactFlowsResponseOutputTypeDef,
+    ListContactReferencesResponseOutputTypeDef,
+    ListDefaultVocabulariesResponseOutputTypeDef,
+    ListEvaluationFormsResponseOutputTypeDef,
+    ListEvaluationFormVersionsResponseOutputTypeDef,
+    ListHoursOfOperationsResponseOutputTypeDef,
+    ListInstanceAttributesResponseOutputTypeDef,
+    ListInstancesResponseOutputTypeDef,
+    ListInstanceStorageConfigsResponseOutputTypeDef,
+    ListIntegrationAssociationsResponseOutputTypeDef,
+    ListLambdaFunctionsResponseOutputTypeDef,
+    ListLexBotsResponseOutputTypeDef,
+    ListPhoneNumbersResponseOutputTypeDef,
+    ListPhoneNumbersV2ResponseOutputTypeDef,
+    ListPromptsResponseOutputTypeDef,
+    ListQueueQuickConnectsResponseOutputTypeDef,
+    ListQueuesResponseOutputTypeDef,
+    ListQuickConnectsResponseOutputTypeDef,
+    ListRoutingProfileQueuesResponseOutputTypeDef,
+    ListRoutingProfilesResponseOutputTypeDef,
+    ListRulesResponseOutputTypeDef,
+    ListSecurityKeysResponseOutputTypeDef,
+    ListSecurityProfilePermissionsResponseOutputTypeDef,
+    ListSecurityProfilesResponseOutputTypeDef,
+    ListTaskTemplatesResponseOutputTypeDef,
+    ListTrafficDistributionGroupsResponseOutputTypeDef,
+    ListUseCasesResponseOutputTypeDef,
+    ListUserHierarchyGroupsResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
     PaginatorConfigTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
-    SearchHoursOfOperationsResponseTypeDef,
-    SearchPromptsResponseTypeDef,
-    SearchQueuesResponseTypeDef,
-    SearchQuickConnectsResponseTypeDef,
-    SearchResourceTagsResponseTypeDef,
-    SearchRoutingProfilesResponseTypeDef,
-    SearchSecurityProfilesResponseTypeDef,
-    SearchUsersResponseTypeDef,
-    SearchVocabulariesResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseOutputTypeDef,
+    SearchHoursOfOperationsResponseOutputTypeDef,
+    SearchPromptsResponseOutputTypeDef,
+    SearchQueuesResponseOutputTypeDef,
+    SearchQuickConnectsResponseOutputTypeDef,
+    SearchResourceTagsResponseOutputTypeDef,
+    SearchRoutingProfilesResponseOutputTypeDef,
+    SearchSecurityProfilesResponseOutputTypeDef,
+    SearchUsersResponseOutputTypeDef,
+    SearchVocabulariesResponseOutputTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     SecurityProfilesSearchFilterTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
 )
 
 __all__ = (
@@ -241,25 +241,22 @@
     "SearchResourceTagsPaginator",
     "SearchRoutingProfilesPaginator",
     "SearchSecurityProfilesPaginator",
     "SearchUsersPaginator",
     "SearchVocabulariesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetMetricDataPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.GetMetricData)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#getmetricdatapaginator)
     """
 
     def paginate(
@@ -268,802 +265,758 @@
         InstanceId: str,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: "FiltersTypeDef",
         HistoricalMetrics: Sequence["HistoricalMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetMetricDataResponseTypeDef]:
+    ) -> _PageIterator[GetMetricDataResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.GetMetricData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#getmetricdatapaginator)
         """
 
-
 class ListAgentStatusesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListAgentStatuses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listagentstatusespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         AgentStatusTypes: Sequence[AgentStatusTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAgentStatusResponseTypeDef]:
+    ) -> _PageIterator[ListAgentStatusResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListAgentStatuses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listagentstatusespaginator)
         """
 
-
 class ListApprovedOriginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListApprovedOrigins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listapprovedoriginspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListApprovedOriginsResponseTypeDef]:
+    ) -> _PageIterator[ListApprovedOriginsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListApprovedOrigins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listapprovedoriginspaginator)
         """
 
-
 class ListBotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListBots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listbotspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBotsResponseTypeDef]:
+    ) -> _PageIterator[ListBotsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listbotspaginator)
         """
 
-
 class ListContactEvaluationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactEvaluations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactevaluationspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactEvaluationsResponseTypeDef]:
+    ) -> _PageIterator[ListContactEvaluationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactevaluationspaginator)
         """
 
-
 class ListContactFlowModulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlowModules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowmodulespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowModuleState: ContactFlowModuleStateType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactFlowModulesResponseTypeDef]:
+    ) -> _PageIterator[ListContactFlowModulesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlowModules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowmodulespaginator)
         """
 
-
 class ListContactFlowsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlows)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactFlowsResponseTypeDef]:
+    ) -> _PageIterator[ListContactFlowsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowspaginator)
         """
 
-
 class ListContactReferencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactReferences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactreferencespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactReferencesResponseTypeDef]:
+    ) -> _PageIterator[ListContactReferencesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactReferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactreferencespaginator)
         """
 
-
 class ListDefaultVocabulariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListDefaultVocabularies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listdefaultvocabulariespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDefaultVocabulariesResponseTypeDef]:
+    ) -> _PageIterator[ListDefaultVocabulariesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListDefaultVocabularies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listdefaultvocabulariespaginator)
         """
 
-
 class ListEvaluationFormVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationFormVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformversionspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         EvaluationFormId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEvaluationFormVersionsResponseTypeDef]:
+    ) -> _PageIterator[ListEvaluationFormVersionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationFormVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformversionspaginator)
         """
 
-
 class ListEvaluationFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEvaluationFormsResponseTypeDef]:
+    ) -> _PageIterator[ListEvaluationFormsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformspaginator)
         """
 
-
 class ListHoursOfOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListHoursOfOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listhoursofoperationspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListHoursOfOperationsResponseTypeDef]:
+    ) -> _PageIterator[ListHoursOfOperationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListHoursOfOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listhoursofoperationspaginator)
         """
 
-
 class ListInstanceAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstanceattributespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceAttributesResponseTypeDef]:
+    ) -> _PageIterator[ListInstanceAttributesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstanceattributespaginator)
         """
 
-
 class ListInstanceStorageConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceStorageConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancestorageconfigspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceStorageConfigsResponseTypeDef]:
+    ) -> _PageIterator[ListInstanceStorageConfigsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceStorageConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancestorageconfigspaginator)
         """
 
-
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstancesResponseTypeDef]:
+    ) -> _PageIterator[ListInstancesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancespaginator)
         """
 
-
 class ListIntegrationAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListIntegrationAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listintegrationassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListIntegrationAssociationsResponseTypeDef]:
+    ) -> _PageIterator[ListIntegrationAssociationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListIntegrationAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listintegrationassociationspaginator)
         """
 
-
 class ListLambdaFunctionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLambdaFunctions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlambdafunctionspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLambdaFunctionsResponseTypeDef]:
+    ) -> _PageIterator[ListLambdaFunctionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLambdaFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlambdafunctionspaginator)
         """
 
-
 class ListLexBotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLexBots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlexbotspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLexBotsResponseTypeDef]:
+    ) -> _PageIterator[ListLexBotsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLexBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlexbotspaginator)
         """
 
-
 class ListPhoneNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumberspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPhoneNumbersResponseTypeDef]:
+    ) -> _PageIterator[ListPhoneNumbersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumberspaginator)
         """
 
-
 class ListPhoneNumbersV2Paginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbersV2)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumbersv2paginator)
     """
 
     def paginate(
         self,
         *,
         TargetArn: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPhoneNumbersV2ResponseTypeDef]:
+    ) -> _PageIterator[ListPhoneNumbersV2ResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbersV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumbersv2paginator)
         """
 
-
 class ListPromptsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPrompts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listpromptspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPromptsResponseTypeDef]:
+    ) -> _PageIterator[ListPromptsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPrompts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listpromptspaginator)
         """
 
-
 class ListQueueQuickConnectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueueQuickConnects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuequickconnectspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, QueueId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQueueQuickConnectsResponseTypeDef]:
+    ) -> _PageIterator[ListQueueQuickConnectsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueueQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuequickconnectspaginator)
         """
 
-
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQueuesResponseTypeDef]:
+    ) -> _PageIterator[ListQueuesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuespaginator)
         """
 
-
 class ListQuickConnectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQuickConnects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listquickconnectspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QuickConnectTypes: Sequence[QuickConnectTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQuickConnectsResponseTypeDef]:
+    ) -> _PageIterator[ListQuickConnectsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listquickconnectspaginator)
         """
 
-
 class ListRoutingProfileQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfileQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilequeuespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoutingProfileQueuesResponseTypeDef]:
+    ) -> _PageIterator[ListRoutingProfileQueuesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfileQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilequeuespaginator)
         """
 
-
 class ListRoutingProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoutingProfilesResponseTypeDef]:
+    ) -> _PageIterator[ListRoutingProfilesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilespaginator)
         """
 
-
 class ListRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listrulespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRulesResponseTypeDef]:
+    ) -> _PageIterator[ListRulesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listrulespaginator)
         """
 
-
 class ListSecurityKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecuritykeyspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityKeysResponseTypeDef]:
+    ) -> _PageIterator[ListSecurityKeysResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecuritykeyspaginator)
         """
 
-
 class ListSecurityProfilePermissionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfilePermissions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilepermissionspaginator)
     """
 
     def paginate(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityProfilePermissionsResponseTypeDef]:
+    ) -> _PageIterator[ListSecurityProfilePermissionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfilePermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilepermissionspaginator)
         """
 
-
 class ListSecurityProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityProfilesResponseTypeDef]:
+    ) -> _PageIterator[ListSecurityProfilesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilespaginator)
         """
 
-
 class ListTaskTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTaskTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtasktemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Status: TaskTemplateStatusType = ...,
         Name: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTaskTemplatesResponseTypeDef]:
+    ) -> _PageIterator[ListTaskTemplatesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTaskTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtasktemplatespaginator)
         """
 
-
 class ListTrafficDistributionGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTrafficDistributionGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtrafficdistributiongroupspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTrafficDistributionGroupsResponseTypeDef]:
+    ) -> _PageIterator[ListTrafficDistributionGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTrafficDistributionGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtrafficdistributiongroupspaginator)
         """
 
-
 class ListUseCasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUseCases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listusecasespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUseCasesResponseTypeDef]:
+    ) -> _PageIterator[ListUseCasesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUseCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listusecasespaginator)
         """
 
-
 class ListUserHierarchyGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUserHierarchyGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserhierarchygroupspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserHierarchyGroupsResponseTypeDef]:
+    ) -> _PageIterator[ListUserHierarchyGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUserHierarchyGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserhierarchygroupspaginator)
         """
 
-
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUsersResponseTypeDef]:
+    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserspaginator)
         """
 
-
 class SearchAvailablePhoneNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchAvailablePhoneNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchavailablephonenumberspaginator)
     """
 
     def paginate(
         self,
         *,
         TargetArn: str,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         PhoneNumberPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchAvailablePhoneNumbersResponseTypeDef]:
+    ) -> _PageIterator[SearchAvailablePhoneNumbersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchAvailablePhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchavailablephonenumberspaginator)
         """
 
-
 class SearchHoursOfOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchHoursOfOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchhoursofoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "HoursOfOperationSearchFilterTypeDef" = ...,
         SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchHoursOfOperationsResponseTypeDef]:
+    ) -> _PageIterator[SearchHoursOfOperationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchHoursOfOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchhoursofoperationspaginator)
         """
 
-
 class SearchPromptsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchPrompts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchpromptspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "PromptSearchFilterTypeDef" = ...,
         SearchCriteria: "PromptSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchPromptsResponseTypeDef]:
+    ) -> _PageIterator[SearchPromptsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchPrompts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchpromptspaginator)
         """
 
-
 class SearchQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchqueuespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "QueueSearchFilterTypeDef" = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchQueuesResponseTypeDef]:
+    ) -> _PageIterator[SearchQueuesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchqueuespaginator)
         """
 
-
 class SearchQuickConnectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQuickConnects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchquickconnectspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "QuickConnectSearchFilterTypeDef" = ...,
         SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchQuickConnectsResponseTypeDef]:
+    ) -> _PageIterator[SearchQuickConnectsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchquickconnectspaginator)
         """
 
-
 class SearchResourceTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchResourceTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchresourcetagspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         SearchCriteria: "ResourceTagsSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchResourceTagsResponseTypeDef]:
+    ) -> _PageIterator[SearchResourceTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchResourceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchresourcetagspaginator)
         """
 
-
 class SearchRoutingProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchRoutingProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchroutingprofilespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "RoutingProfileSearchFilterTypeDef" = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchRoutingProfilesResponseTypeDef]:
+    ) -> _PageIterator[SearchRoutingProfilesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchRoutingProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchroutingprofilespaginator)
         """
 
-
 class SearchSecurityProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchSecurityProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchsecurityprofilespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: "SecurityProfilesSearchFilterTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchSecurityProfilesResponseTypeDef]:
+    ) -> _PageIterator[SearchSecurityProfilesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchSecurityProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchsecurityprofilespaginator)
         """
 
-
 class SearchUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchuserspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str = ...,
         SearchFilter: "UserSearchFilterTypeDef" = ...,
         SearchCriteria: "UserSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchUsersResponseTypeDef]:
+    ) -> _PageIterator[SearchUsersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchuserspaginator)
         """
 
-
 class SearchVocabulariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchVocabularies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchvocabulariespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
         LanguageCode: VocabularyLanguageCodeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchVocabulariesResponseTypeDef]:
+    ) -> _PageIterator[SearchVocabulariesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchVocabularies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchvocabulariespaginator)
         """
```

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect/paginator.pyi` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -129,72 +129,72 @@
     RulePublishStatusType,
     TaskTemplateStatusType,
     VocabularyLanguageCodeType,
     VocabularyStateType,
 )
 from .type_defs import (
     FiltersTypeDef,
-    GetMetricDataResponseTypeDef,
+    GetMetricDataResponseOutputTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
-    ListAgentStatusResponseTypeDef,
-    ListApprovedOriginsResponseTypeDef,
-    ListBotsResponseTypeDef,
-    ListContactEvaluationsResponseTypeDef,
-    ListContactFlowModulesResponseTypeDef,
-    ListContactFlowsResponseTypeDef,
-    ListContactReferencesResponseTypeDef,
-    ListDefaultVocabulariesResponseTypeDef,
-    ListEvaluationFormsResponseTypeDef,
-    ListEvaluationFormVersionsResponseTypeDef,
-    ListHoursOfOperationsResponseTypeDef,
-    ListInstanceAttributesResponseTypeDef,
-    ListInstancesResponseTypeDef,
-    ListInstanceStorageConfigsResponseTypeDef,
-    ListIntegrationAssociationsResponseTypeDef,
-    ListLambdaFunctionsResponseTypeDef,
-    ListLexBotsResponseTypeDef,
-    ListPhoneNumbersResponseTypeDef,
-    ListPhoneNumbersV2ResponseTypeDef,
-    ListPromptsResponseTypeDef,
-    ListQueueQuickConnectsResponseTypeDef,
-    ListQueuesResponseTypeDef,
-    ListQuickConnectsResponseTypeDef,
-    ListRoutingProfileQueuesResponseTypeDef,
-    ListRoutingProfilesResponseTypeDef,
-    ListRulesResponseTypeDef,
-    ListSecurityKeysResponseTypeDef,
-    ListSecurityProfilePermissionsResponseTypeDef,
-    ListSecurityProfilesResponseTypeDef,
-    ListTaskTemplatesResponseTypeDef,
-    ListTrafficDistributionGroupsResponseTypeDef,
-    ListUseCasesResponseTypeDef,
-    ListUserHierarchyGroupsResponseTypeDef,
-    ListUsersResponseTypeDef,
+    ListAgentStatusResponseOutputTypeDef,
+    ListApprovedOriginsResponseOutputTypeDef,
+    ListBotsResponseOutputTypeDef,
+    ListContactEvaluationsResponseOutputTypeDef,
+    ListContactFlowModulesResponseOutputTypeDef,
+    ListContactFlowsResponseOutputTypeDef,
+    ListContactReferencesResponseOutputTypeDef,
+    ListDefaultVocabulariesResponseOutputTypeDef,
+    ListEvaluationFormsResponseOutputTypeDef,
+    ListEvaluationFormVersionsResponseOutputTypeDef,
+    ListHoursOfOperationsResponseOutputTypeDef,
+    ListInstanceAttributesResponseOutputTypeDef,
+    ListInstancesResponseOutputTypeDef,
+    ListInstanceStorageConfigsResponseOutputTypeDef,
+    ListIntegrationAssociationsResponseOutputTypeDef,
+    ListLambdaFunctionsResponseOutputTypeDef,
+    ListLexBotsResponseOutputTypeDef,
+    ListPhoneNumbersResponseOutputTypeDef,
+    ListPhoneNumbersV2ResponseOutputTypeDef,
+    ListPromptsResponseOutputTypeDef,
+    ListQueueQuickConnectsResponseOutputTypeDef,
+    ListQueuesResponseOutputTypeDef,
+    ListQuickConnectsResponseOutputTypeDef,
+    ListRoutingProfileQueuesResponseOutputTypeDef,
+    ListRoutingProfilesResponseOutputTypeDef,
+    ListRulesResponseOutputTypeDef,
+    ListSecurityKeysResponseOutputTypeDef,
+    ListSecurityProfilePermissionsResponseOutputTypeDef,
+    ListSecurityProfilesResponseOutputTypeDef,
+    ListTaskTemplatesResponseOutputTypeDef,
+    ListTrafficDistributionGroupsResponseOutputTypeDef,
+    ListUseCasesResponseOutputTypeDef,
+    ListUserHierarchyGroupsResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
     PaginatorConfigTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
-    SearchHoursOfOperationsResponseTypeDef,
-    SearchPromptsResponseTypeDef,
-    SearchQueuesResponseTypeDef,
-    SearchQuickConnectsResponseTypeDef,
-    SearchResourceTagsResponseTypeDef,
-    SearchRoutingProfilesResponseTypeDef,
-    SearchSecurityProfilesResponseTypeDef,
-    SearchUsersResponseTypeDef,
-    SearchVocabulariesResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseOutputTypeDef,
+    SearchHoursOfOperationsResponseOutputTypeDef,
+    SearchPromptsResponseOutputTypeDef,
+    SearchQueuesResponseOutputTypeDef,
+    SearchQuickConnectsResponseOutputTypeDef,
+    SearchResourceTagsResponseOutputTypeDef,
+    SearchRoutingProfilesResponseOutputTypeDef,
+    SearchSecurityProfilesResponseOutputTypeDef,
+    SearchUsersResponseOutputTypeDef,
+    SearchVocabulariesResponseOutputTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     SecurityProfilesSearchFilterTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
 )
 
 __all__ = (
@@ -241,22 +241,25 @@
     "SearchResourceTagsPaginator",
     "SearchRoutingProfilesPaginator",
     "SearchSecurityProfilesPaginator",
     "SearchUsersPaginator",
     "SearchVocabulariesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetMetricDataPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.GetMetricData)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#getmetricdatapaginator)
     """
 
     def paginate(
@@ -265,758 +268,802 @@
         InstanceId: str,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: "FiltersTypeDef",
         HistoricalMetrics: Sequence["HistoricalMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetMetricDataResponseTypeDef]:
+    ) -> _PageIterator[GetMetricDataResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.GetMetricData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#getmetricdatapaginator)
         """
 
+
 class ListAgentStatusesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListAgentStatuses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listagentstatusespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         AgentStatusTypes: Sequence[AgentStatusTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAgentStatusResponseTypeDef]:
+    ) -> _PageIterator[ListAgentStatusResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListAgentStatuses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listagentstatusespaginator)
         """
 
+
 class ListApprovedOriginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListApprovedOrigins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listapprovedoriginspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListApprovedOriginsResponseTypeDef]:
+    ) -> _PageIterator[ListApprovedOriginsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListApprovedOrigins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listapprovedoriginspaginator)
         """
 
+
 class ListBotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListBots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listbotspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBotsResponseTypeDef]:
+    ) -> _PageIterator[ListBotsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listbotspaginator)
         """
 
+
 class ListContactEvaluationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactEvaluations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactevaluationspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactEvaluationsResponseTypeDef]:
+    ) -> _PageIterator[ListContactEvaluationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactevaluationspaginator)
         """
 
+
 class ListContactFlowModulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlowModules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowmodulespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowModuleState: ContactFlowModuleStateType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactFlowModulesResponseTypeDef]:
+    ) -> _PageIterator[ListContactFlowModulesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlowModules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowmodulespaginator)
         """
 
+
 class ListContactFlowsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlows)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactFlowsResponseTypeDef]:
+    ) -> _PageIterator[ListContactFlowsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowspaginator)
         """
 
+
 class ListContactReferencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactReferences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactreferencespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactReferencesResponseTypeDef]:
+    ) -> _PageIterator[ListContactReferencesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactReferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactreferencespaginator)
         """
 
+
 class ListDefaultVocabulariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListDefaultVocabularies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listdefaultvocabulariespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDefaultVocabulariesResponseTypeDef]:
+    ) -> _PageIterator[ListDefaultVocabulariesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListDefaultVocabularies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listdefaultvocabulariespaginator)
         """
 
+
 class ListEvaluationFormVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationFormVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformversionspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         EvaluationFormId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEvaluationFormVersionsResponseTypeDef]:
+    ) -> _PageIterator[ListEvaluationFormVersionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationFormVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformversionspaginator)
         """
 
+
 class ListEvaluationFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEvaluationFormsResponseTypeDef]:
+    ) -> _PageIterator[ListEvaluationFormsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformspaginator)
         """
 
+
 class ListHoursOfOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListHoursOfOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listhoursofoperationspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListHoursOfOperationsResponseTypeDef]:
+    ) -> _PageIterator[ListHoursOfOperationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListHoursOfOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listhoursofoperationspaginator)
         """
 
+
 class ListInstanceAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstanceattributespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceAttributesResponseTypeDef]:
+    ) -> _PageIterator[ListInstanceAttributesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstanceattributespaginator)
         """
 
+
 class ListInstanceStorageConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceStorageConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancestorageconfigspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceStorageConfigsResponseTypeDef]:
+    ) -> _PageIterator[ListInstanceStorageConfigsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceStorageConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancestorageconfigspaginator)
         """
 
+
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstancesResponseTypeDef]:
+    ) -> _PageIterator[ListInstancesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancespaginator)
         """
 
+
 class ListIntegrationAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListIntegrationAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listintegrationassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListIntegrationAssociationsResponseTypeDef]:
+    ) -> _PageIterator[ListIntegrationAssociationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListIntegrationAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listintegrationassociationspaginator)
         """
 
+
 class ListLambdaFunctionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLambdaFunctions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlambdafunctionspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLambdaFunctionsResponseTypeDef]:
+    ) -> _PageIterator[ListLambdaFunctionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLambdaFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlambdafunctionspaginator)
         """
 
+
 class ListLexBotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLexBots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlexbotspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLexBotsResponseTypeDef]:
+    ) -> _PageIterator[ListLexBotsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLexBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlexbotspaginator)
         """
 
+
 class ListPhoneNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumberspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPhoneNumbersResponseTypeDef]:
+    ) -> _PageIterator[ListPhoneNumbersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumberspaginator)
         """
 
+
 class ListPhoneNumbersV2Paginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbersV2)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumbersv2paginator)
     """
 
     def paginate(
         self,
         *,
         TargetArn: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPhoneNumbersV2ResponseTypeDef]:
+    ) -> _PageIterator[ListPhoneNumbersV2ResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbersV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumbersv2paginator)
         """
 
+
 class ListPromptsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPrompts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listpromptspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPromptsResponseTypeDef]:
+    ) -> _PageIterator[ListPromptsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPrompts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listpromptspaginator)
         """
 
+
 class ListQueueQuickConnectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueueQuickConnects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuequickconnectspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, QueueId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQueueQuickConnectsResponseTypeDef]:
+    ) -> _PageIterator[ListQueueQuickConnectsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueueQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuequickconnectspaginator)
         """
 
+
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQueuesResponseTypeDef]:
+    ) -> _PageIterator[ListQueuesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuespaginator)
         """
 
+
 class ListQuickConnectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQuickConnects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listquickconnectspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QuickConnectTypes: Sequence[QuickConnectTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQuickConnectsResponseTypeDef]:
+    ) -> _PageIterator[ListQuickConnectsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listquickconnectspaginator)
         """
 
+
 class ListRoutingProfileQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfileQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilequeuespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoutingProfileQueuesResponseTypeDef]:
+    ) -> _PageIterator[ListRoutingProfileQueuesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfileQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilequeuespaginator)
         """
 
+
 class ListRoutingProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoutingProfilesResponseTypeDef]:
+    ) -> _PageIterator[ListRoutingProfilesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilespaginator)
         """
 
+
 class ListRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listrulespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRulesResponseTypeDef]:
+    ) -> _PageIterator[ListRulesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listrulespaginator)
         """
 
+
 class ListSecurityKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecuritykeyspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityKeysResponseTypeDef]:
+    ) -> _PageIterator[ListSecurityKeysResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecuritykeyspaginator)
         """
 
+
 class ListSecurityProfilePermissionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfilePermissions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilepermissionspaginator)
     """
 
     def paginate(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityProfilePermissionsResponseTypeDef]:
+    ) -> _PageIterator[ListSecurityProfilePermissionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfilePermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilepermissionspaginator)
         """
 
+
 class ListSecurityProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityProfilesResponseTypeDef]:
+    ) -> _PageIterator[ListSecurityProfilesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilespaginator)
         """
 
+
 class ListTaskTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTaskTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtasktemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Status: TaskTemplateStatusType = ...,
         Name: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTaskTemplatesResponseTypeDef]:
+    ) -> _PageIterator[ListTaskTemplatesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTaskTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtasktemplatespaginator)
         """
 
+
 class ListTrafficDistributionGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTrafficDistributionGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtrafficdistributiongroupspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTrafficDistributionGroupsResponseTypeDef]:
+    ) -> _PageIterator[ListTrafficDistributionGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTrafficDistributionGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtrafficdistributiongroupspaginator)
         """
 
+
 class ListUseCasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUseCases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listusecasespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUseCasesResponseTypeDef]:
+    ) -> _PageIterator[ListUseCasesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUseCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listusecasespaginator)
         """
 
+
 class ListUserHierarchyGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUserHierarchyGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserhierarchygroupspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserHierarchyGroupsResponseTypeDef]:
+    ) -> _PageIterator[ListUserHierarchyGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUserHierarchyGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserhierarchygroupspaginator)
         """
 
+
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUsersResponseTypeDef]:
+    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserspaginator)
         """
 
+
 class SearchAvailablePhoneNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchAvailablePhoneNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchavailablephonenumberspaginator)
     """
 
     def paginate(
         self,
         *,
         TargetArn: str,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         PhoneNumberPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchAvailablePhoneNumbersResponseTypeDef]:
+    ) -> _PageIterator[SearchAvailablePhoneNumbersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchAvailablePhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchavailablephonenumberspaginator)
         """
 
+
 class SearchHoursOfOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchHoursOfOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchhoursofoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "HoursOfOperationSearchFilterTypeDef" = ...,
         SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchHoursOfOperationsResponseTypeDef]:
+    ) -> _PageIterator[SearchHoursOfOperationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchHoursOfOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchhoursofoperationspaginator)
         """
 
+
 class SearchPromptsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchPrompts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchpromptspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "PromptSearchFilterTypeDef" = ...,
         SearchCriteria: "PromptSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchPromptsResponseTypeDef]:
+    ) -> _PageIterator[SearchPromptsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchPrompts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchpromptspaginator)
         """
 
+
 class SearchQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchqueuespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "QueueSearchFilterTypeDef" = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchQueuesResponseTypeDef]:
+    ) -> _PageIterator[SearchQueuesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchqueuespaginator)
         """
 
+
 class SearchQuickConnectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQuickConnects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchquickconnectspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "QuickConnectSearchFilterTypeDef" = ...,
         SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchQuickConnectsResponseTypeDef]:
+    ) -> _PageIterator[SearchQuickConnectsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchquickconnectspaginator)
         """
 
+
 class SearchResourceTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchResourceTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchresourcetagspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         SearchCriteria: "ResourceTagsSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchResourceTagsResponseTypeDef]:
+    ) -> _PageIterator[SearchResourceTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchResourceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchresourcetagspaginator)
         """
 
+
 class SearchRoutingProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchRoutingProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchroutingprofilespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "RoutingProfileSearchFilterTypeDef" = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchRoutingProfilesResponseTypeDef]:
+    ) -> _PageIterator[SearchRoutingProfilesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchRoutingProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchroutingprofilespaginator)
         """
 
+
 class SearchSecurityProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchSecurityProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchsecurityprofilespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: "SecurityProfilesSearchFilterTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchSecurityProfilesResponseTypeDef]:
+    ) -> _PageIterator[SearchSecurityProfilesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchSecurityProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchsecurityprofilespaginator)
         """
 
+
 class SearchUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchuserspaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str = ...,
         SearchFilter: "UserSearchFilterTypeDef" = ...,
         SearchCriteria: "UserSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchUsersResponseTypeDef]:
+    ) -> _PageIterator[SearchUsersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchuserspaginator)
         """
 
+
 class SearchVocabulariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchVocabularies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchvocabulariespaginator)
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
         LanguageCode: VocabularyLanguageCodeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchVocabulariesResponseTypeDef]:
+    ) -> _PageIterator[SearchVocabulariesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchVocabularies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchvocabulariespaginator)
         """
```

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect/type_defs.py` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for connect service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_connect.type_defs import ActionSummaryTypeDef
+    from mypy_boto3_connect.type_defs import ActionSummaryOutputTypeDef
 
-    data: ActionSummaryTypeDef = {...}
+    data: ActionSummaryOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -83,103 +83,104 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "ActionSummaryTypeDef",
+    "ActionSummaryOutputTypeDef",
     "ActivateEvaluationFormRequestRequestTypeDef",
-    "ActivateEvaluationFormResponseTypeDef",
-    "AgentContactReferenceTypeDef",
-    "AgentInfoTypeDef",
-    "AgentStatusReferenceTypeDef",
-    "AgentStatusSummaryTypeDef",
-    "AgentStatusTypeDef",
+    "ActivateEvaluationFormResponseOutputTypeDef",
+    "AgentContactReferenceOutputTypeDef",
+    "AgentInfoOutputTypeDef",
+    "AgentStatusOutputTypeDef",
+    "AgentStatusReferenceOutputTypeDef",
+    "AgentStatusSummaryOutputTypeDef",
     "AnswerMachineDetectionConfigTypeDef",
     "AssociateApprovedOriginRequestRequestTypeDef",
     "AssociateBotRequestRequestTypeDef",
     "AssociateDefaultVocabularyRequestRequestTypeDef",
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
-    "AssociateInstanceStorageConfigResponseTypeDef",
+    "AssociateInstanceStorageConfigResponseOutputTypeDef",
     "AssociateLambdaFunctionRequestRequestTypeDef",
     "AssociateLexBotRequestRequestTypeDef",
     "AssociatePhoneNumberContactFlowRequestRequestTypeDef",
     "AssociateQueueQuickConnectsRequestRequestTypeDef",
     "AssociateRoutingProfileQueuesRequestRequestTypeDef",
     "AssociateSecurityKeyRequestRequestTypeDef",
-    "AssociateSecurityKeyResponseTypeDef",
-    "AttachmentReferenceTypeDef",
-    "AttributeTypeDef",
-    "AvailableNumberSummaryTypeDef",
+    "AssociateSecurityKeyResponseOutputTypeDef",
+    "AttachmentReferenceOutputTypeDef",
+    "AttributeOutputTypeDef",
+    "AvailableNumberSummaryOutputTypeDef",
     "ChatMessageTypeDef",
     "ChatParticipantRoleConfigTypeDef",
     "ChatStreamingConfigurationTypeDef",
     "ClaimPhoneNumberRequestRequestTypeDef",
-    "ClaimPhoneNumberResponseTypeDef",
-    "ClaimedPhoneNumberSummaryTypeDef",
+    "ClaimPhoneNumberResponseOutputTypeDef",
+    "ClaimedPhoneNumberSummaryOutputTypeDef",
     "ContactFilterTypeDef",
-    "ContactFlowModuleSummaryTypeDef",
-    "ContactFlowModuleTypeDef",
-    "ContactFlowSummaryTypeDef",
-    "ContactFlowTypeDef",
-    "ContactTypeDef",
+    "ContactFlowModuleOutputTypeDef",
+    "ContactFlowModuleSummaryOutputTypeDef",
+    "ContactFlowOutputTypeDef",
+    "ContactFlowSummaryOutputTypeDef",
+    "ContactOutputTypeDef",
     "ControlPlaneTagFilterTypeDef",
     "CreateAgentStatusRequestRequestTypeDef",
-    "CreateAgentStatusResponseTypeDef",
+    "CreateAgentStatusResponseOutputTypeDef",
     "CreateContactFlowModuleRequestRequestTypeDef",
-    "CreateContactFlowModuleResponseTypeDef",
+    "CreateContactFlowModuleResponseOutputTypeDef",
     "CreateContactFlowRequestRequestTypeDef",
-    "CreateContactFlowResponseTypeDef",
+    "CreateContactFlowResponseOutputTypeDef",
     "CreateEvaluationFormRequestRequestTypeDef",
-    "CreateEvaluationFormResponseTypeDef",
+    "CreateEvaluationFormResponseOutputTypeDef",
     "CreateHoursOfOperationRequestRequestTypeDef",
-    "CreateHoursOfOperationResponseTypeDef",
+    "CreateHoursOfOperationResponseOutputTypeDef",
     "CreateInstanceRequestRequestTypeDef",
-    "CreateInstanceResponseTypeDef",
+    "CreateInstanceResponseOutputTypeDef",
     "CreateIntegrationAssociationRequestRequestTypeDef",
-    "CreateIntegrationAssociationResponseTypeDef",
+    "CreateIntegrationAssociationResponseOutputTypeDef",
     "CreateParticipantRequestRequestTypeDef",
-    "CreateParticipantResponseTypeDef",
+    "CreateParticipantResponseOutputTypeDef",
     "CreatePromptRequestRequestTypeDef",
-    "CreatePromptResponseTypeDef",
+    "CreatePromptResponseOutputTypeDef",
     "CreateQueueRequestRequestTypeDef",
-    "CreateQueueResponseTypeDef",
+    "CreateQueueResponseOutputTypeDef",
     "CreateQuickConnectRequestRequestTypeDef",
-    "CreateQuickConnectResponseTypeDef",
+    "CreateQuickConnectResponseOutputTypeDef",
     "CreateRoutingProfileRequestRequestTypeDef",
-    "CreateRoutingProfileResponseTypeDef",
+    "CreateRoutingProfileResponseOutputTypeDef",
     "CreateRuleRequestRequestTypeDef",
-    "CreateRuleResponseTypeDef",
+    "CreateRuleResponseOutputTypeDef",
     "CreateSecurityProfileRequestRequestTypeDef",
-    "CreateSecurityProfileResponseTypeDef",
+    "CreateSecurityProfileResponseOutputTypeDef",
     "CreateTaskTemplateRequestRequestTypeDef",
-    "CreateTaskTemplateResponseTypeDef",
+    "CreateTaskTemplateResponseOutputTypeDef",
     "CreateTrafficDistributionGroupRequestRequestTypeDef",
-    "CreateTrafficDistributionGroupResponseTypeDef",
+    "CreateTrafficDistributionGroupResponseOutputTypeDef",
     "CreateUseCaseRequestRequestTypeDef",
-    "CreateUseCaseResponseTypeDef",
+    "CreateUseCaseResponseOutputTypeDef",
     "CreateUserHierarchyGroupRequestRequestTypeDef",
-    "CreateUserHierarchyGroupResponseTypeDef",
+    "CreateUserHierarchyGroupResponseOutputTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "CreateUserResponseTypeDef",
+    "CreateUserResponseOutputTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
-    "CreateVocabularyResponseTypeDef",
-    "CredentialsTypeDef",
+    "CreateVocabularyResponseOutputTypeDef",
+    "CredentialsOutputTypeDef",
+    "CrossChannelBehaviorOutputTypeDef",
     "CrossChannelBehaviorTypeDef",
-    "CurrentMetricDataTypeDef",
-    "CurrentMetricResultTypeDef",
+    "CurrentMetricDataOutputTypeDef",
+    "CurrentMetricOutputTypeDef",
+    "CurrentMetricResultOutputTypeDef",
     "CurrentMetricSortCriteriaTypeDef",
     "CurrentMetricTypeDef",
-    "DateReferenceTypeDef",
+    "DateReferenceOutputTypeDef",
     "DeactivateEvaluationFormRequestRequestTypeDef",
-    "DeactivateEvaluationFormResponseTypeDef",
-    "DefaultVocabularyTypeDef",
+    "DeactivateEvaluationFormResponseOutputTypeDef",
+    "DefaultVocabularyOutputTypeDef",
     "DeleteContactEvaluationRequestRequestTypeDef",
     "DeleteContactFlowModuleRequestRequestTypeDef",
     "DeleteContactFlowRequestRequestTypeDef",
     "DeleteEvaluationFormRequestRequestTypeDef",
     "DeleteHoursOfOperationRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteIntegrationAssociationRequestRequestTypeDef",
@@ -191,538 +192,594 @@
     "DeleteSecurityProfileRequestRequestTypeDef",
     "DeleteTaskTemplateRequestRequestTypeDef",
     "DeleteTrafficDistributionGroupRequestRequestTypeDef",
     "DeleteUseCaseRequestRequestTypeDef",
     "DeleteUserHierarchyGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteVocabularyRequestRequestTypeDef",
-    "DeleteVocabularyResponseTypeDef",
+    "DeleteVocabularyResponseOutputTypeDef",
     "DescribeAgentStatusRequestRequestTypeDef",
-    "DescribeAgentStatusResponseTypeDef",
+    "DescribeAgentStatusResponseOutputTypeDef",
     "DescribeContactEvaluationRequestRequestTypeDef",
-    "DescribeContactEvaluationResponseTypeDef",
+    "DescribeContactEvaluationResponseOutputTypeDef",
     "DescribeContactFlowModuleRequestRequestTypeDef",
-    "DescribeContactFlowModuleResponseTypeDef",
+    "DescribeContactFlowModuleResponseOutputTypeDef",
     "DescribeContactFlowRequestRequestTypeDef",
-    "DescribeContactFlowResponseTypeDef",
+    "DescribeContactFlowResponseOutputTypeDef",
     "DescribeContactRequestRequestTypeDef",
-    "DescribeContactResponseTypeDef",
+    "DescribeContactResponseOutputTypeDef",
     "DescribeEvaluationFormRequestRequestTypeDef",
-    "DescribeEvaluationFormResponseTypeDef",
+    "DescribeEvaluationFormResponseOutputTypeDef",
     "DescribeHoursOfOperationRequestRequestTypeDef",
-    "DescribeHoursOfOperationResponseTypeDef",
+    "DescribeHoursOfOperationResponseOutputTypeDef",
     "DescribeInstanceAttributeRequestRequestTypeDef",
-    "DescribeInstanceAttributeResponseTypeDef",
+    "DescribeInstanceAttributeResponseOutputTypeDef",
     "DescribeInstanceRequestRequestTypeDef",
-    "DescribeInstanceResponseTypeDef",
+    "DescribeInstanceResponseOutputTypeDef",
     "DescribeInstanceStorageConfigRequestRequestTypeDef",
-    "DescribeInstanceStorageConfigResponseTypeDef",
+    "DescribeInstanceStorageConfigResponseOutputTypeDef",
     "DescribePhoneNumberRequestRequestTypeDef",
-    "DescribePhoneNumberResponseTypeDef",
+    "DescribePhoneNumberResponseOutputTypeDef",
     "DescribePromptRequestRequestTypeDef",
-    "DescribePromptResponseTypeDef",
+    "DescribePromptResponseOutputTypeDef",
     "DescribeQueueRequestRequestTypeDef",
-    "DescribeQueueResponseTypeDef",
+    "DescribeQueueResponseOutputTypeDef",
     "DescribeQuickConnectRequestRequestTypeDef",
-    "DescribeQuickConnectResponseTypeDef",
+    "DescribeQuickConnectResponseOutputTypeDef",
     "DescribeRoutingProfileRequestRequestTypeDef",
-    "DescribeRoutingProfileResponseTypeDef",
+    "DescribeRoutingProfileResponseOutputTypeDef",
     "DescribeRuleRequestRequestTypeDef",
-    "DescribeRuleResponseTypeDef",
+    "DescribeRuleResponseOutputTypeDef",
     "DescribeSecurityProfileRequestRequestTypeDef",
-    "DescribeSecurityProfileResponseTypeDef",
+    "DescribeSecurityProfileResponseOutputTypeDef",
     "DescribeTrafficDistributionGroupRequestRequestTypeDef",
-    "DescribeTrafficDistributionGroupResponseTypeDef",
+    "DescribeTrafficDistributionGroupResponseOutputTypeDef",
     "DescribeUserHierarchyGroupRequestRequestTypeDef",
-    "DescribeUserHierarchyGroupResponseTypeDef",
+    "DescribeUserHierarchyGroupResponseOutputTypeDef",
     "DescribeUserHierarchyStructureRequestRequestTypeDef",
-    "DescribeUserHierarchyStructureResponseTypeDef",
+    "DescribeUserHierarchyStructureResponseOutputTypeDef",
     "DescribeUserRequestRequestTypeDef",
-    "DescribeUserResponseTypeDef",
+    "DescribeUserResponseOutputTypeDef",
     "DescribeVocabularyRequestRequestTypeDef",
-    "DescribeVocabularyResponseTypeDef",
-    "DimensionsTypeDef",
+    "DescribeVocabularyResponseOutputTypeDef",
+    "DimensionsOutputTypeDef",
     "DisassociateApprovedOriginRequestRequestTypeDef",
     "DisassociateBotRequestRequestTypeDef",
     "DisassociateInstanceStorageConfigRequestRequestTypeDef",
     "DisassociateLambdaFunctionRequestRequestTypeDef",
     "DisassociateLexBotRequestRequestTypeDef",
     "DisassociatePhoneNumberContactFlowRequestRequestTypeDef",
     "DisassociateQueueQuickConnectsRequestRequestTypeDef",
     "DisassociateRoutingProfileQueuesRequestRequestTypeDef",
     "DisassociateSecurityKeyRequestRequestTypeDef",
     "DismissUserContactRequestRequestTypeDef",
+    "DistributionOutputTypeDef",
     "DistributionTypeDef",
-    "EmailReferenceTypeDef",
+    "EmailReferenceOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
+    "EvaluationAnswerDataOutputTypeDef",
     "EvaluationAnswerDataTypeDef",
     "EvaluationAnswerInputTypeDef",
-    "EvaluationAnswerOutputTypeDef",
-    "EvaluationFormContentTypeDef",
+    "EvaluationAnswerOutputOutputTypeDef",
+    "EvaluationFormContentOutputTypeDef",
+    "EvaluationFormItemOutputTypeDef",
     "EvaluationFormItemTypeDef",
+    "EvaluationFormNumericQuestionAutomationOutputTypeDef",
     "EvaluationFormNumericQuestionAutomationTypeDef",
+    "EvaluationFormNumericQuestionOptionOutputTypeDef",
     "EvaluationFormNumericQuestionOptionTypeDef",
+    "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
     "EvaluationFormNumericQuestionPropertiesTypeDef",
+    "EvaluationFormOutputTypeDef",
+    "EvaluationFormQuestionOutputTypeDef",
     "EvaluationFormQuestionTypeDef",
+    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
     "EvaluationFormQuestionTypePropertiesTypeDef",
+    "EvaluationFormScoringStrategyOutputTypeDef",
     "EvaluationFormScoringStrategyTypeDef",
+    "EvaluationFormSectionOutputTypeDef",
     "EvaluationFormSectionTypeDef",
+    "EvaluationFormSingleSelectQuestionAutomationOptionOutputTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationOptionTypeDef",
+    "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationTypeDef",
+    "EvaluationFormSingleSelectQuestionOptionOutputTypeDef",
     "EvaluationFormSingleSelectQuestionOptionTypeDef",
+    "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
     "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
-    "EvaluationFormSummaryTypeDef",
-    "EvaluationFormTypeDef",
-    "EvaluationFormVersionSummaryTypeDef",
-    "EvaluationMetadataTypeDef",
+    "EvaluationFormSummaryOutputTypeDef",
+    "EvaluationFormVersionSummaryOutputTypeDef",
+    "EvaluationMetadataOutputTypeDef",
+    "EvaluationNoteOutputTypeDef",
     "EvaluationNoteTypeDef",
-    "EvaluationScoreTypeDef",
-    "EvaluationSummaryTypeDef",
-    "EvaluationTypeDef",
+    "EvaluationOutputTypeDef",
+    "EvaluationScoreOutputTypeDef",
+    "EvaluationSummaryOutputTypeDef",
+    "EventBridgeActionDefinitionOutputTypeDef",
     "EventBridgeActionDefinitionTypeDef",
     "FilterV2TypeDef",
     "FiltersTypeDef",
     "GetContactAttributesRequestRequestTypeDef",
-    "GetContactAttributesResponseTypeDef",
+    "GetContactAttributesResponseOutputTypeDef",
     "GetCurrentMetricDataRequestRequestTypeDef",
-    "GetCurrentMetricDataResponseTypeDef",
+    "GetCurrentMetricDataResponseOutputTypeDef",
     "GetCurrentUserDataRequestRequestTypeDef",
-    "GetCurrentUserDataResponseTypeDef",
+    "GetCurrentUserDataResponseOutputTypeDef",
     "GetFederationTokenRequestRequestTypeDef",
-    "GetFederationTokenResponseTypeDef",
+    "GetFederationTokenResponseOutputTypeDef",
     "GetMetricDataRequestGetMetricDataPaginateTypeDef",
     "GetMetricDataRequestRequestTypeDef",
-    "GetMetricDataResponseTypeDef",
+    "GetMetricDataResponseOutputTypeDef",
     "GetMetricDataV2RequestRequestTypeDef",
-    "GetMetricDataV2ResponseTypeDef",
+    "GetMetricDataV2ResponseOutputTypeDef",
     "GetPromptFileRequestRequestTypeDef",
-    "GetPromptFileResponseTypeDef",
+    "GetPromptFileResponseOutputTypeDef",
     "GetTaskTemplateRequestRequestTypeDef",
-    "GetTaskTemplateResponseTypeDef",
+    "GetTaskTemplateResponseOutputTypeDef",
     "GetTrafficDistributionRequestRequestTypeDef",
-    "GetTrafficDistributionResponseTypeDef",
+    "GetTrafficDistributionResponseOutputTypeDef",
     "HierarchyGroupConditionTypeDef",
-    "HierarchyGroupSummaryReferenceTypeDef",
-    "HierarchyGroupSummaryTypeDef",
-    "HierarchyGroupTypeDef",
-    "HierarchyLevelTypeDef",
+    "HierarchyGroupOutputTypeDef",
+    "HierarchyGroupSummaryOutputTypeDef",
+    "HierarchyGroupSummaryReferenceOutputTypeDef",
+    "HierarchyLevelOutputTypeDef",
     "HierarchyLevelUpdateTypeDef",
-    "HierarchyPathReferenceTypeDef",
-    "HierarchyPathTypeDef",
-    "HierarchyStructureTypeDef",
+    "HierarchyPathOutputTypeDef",
+    "HierarchyPathReferenceOutputTypeDef",
+    "HierarchyStructureOutputTypeDef",
     "HierarchyStructureUpdateTypeDef",
-    "HistoricalMetricDataTypeDef",
-    "HistoricalMetricResultTypeDef",
+    "HistoricalMetricDataOutputTypeDef",
+    "HistoricalMetricOutputTypeDef",
+    "HistoricalMetricResultOutputTypeDef",
     "HistoricalMetricTypeDef",
+    "HoursOfOperationConfigOutputTypeDef",
     "HoursOfOperationConfigTypeDef",
+    "HoursOfOperationOutputTypeDef",
     "HoursOfOperationSearchCriteriaTypeDef",
     "HoursOfOperationSearchFilterTypeDef",
-    "HoursOfOperationSummaryTypeDef",
+    "HoursOfOperationSummaryOutputTypeDef",
+    "HoursOfOperationTimeSliceOutputTypeDef",
     "HoursOfOperationTimeSliceTypeDef",
-    "HoursOfOperationTypeDef",
-    "InstanceStatusReasonTypeDef",
+    "InstanceOutputTypeDef",
+    "InstanceStatusReasonOutputTypeDef",
+    "InstanceStorageConfigOutputTypeDef",
     "InstanceStorageConfigTypeDef",
-    "InstanceSummaryTypeDef",
-    "InstanceTypeDef",
-    "IntegrationAssociationSummaryTypeDef",
+    "InstanceSummaryOutputTypeDef",
+    "IntegrationAssociationSummaryOutputTypeDef",
+    "InvisibleFieldInfoOutputTypeDef",
     "InvisibleFieldInfoTypeDef",
+    "KinesisFirehoseConfigOutputTypeDef",
     "KinesisFirehoseConfigTypeDef",
+    "KinesisStreamConfigOutputTypeDef",
     "KinesisStreamConfigTypeDef",
+    "KinesisVideoStreamConfigOutputTypeDef",
     "KinesisVideoStreamConfigTypeDef",
-    "LexBotConfigTypeDef",
+    "LexBotConfigOutputTypeDef",
+    "LexBotOutputTypeDef",
     "LexBotTypeDef",
+    "LexV2BotOutputTypeDef",
     "LexV2BotTypeDef",
     "ListAgentStatusRequestListAgentStatusesPaginateTypeDef",
     "ListAgentStatusRequestRequestTypeDef",
-    "ListAgentStatusResponseTypeDef",
+    "ListAgentStatusResponseOutputTypeDef",
     "ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     "ListApprovedOriginsRequestRequestTypeDef",
-    "ListApprovedOriginsResponseTypeDef",
+    "ListApprovedOriginsResponseOutputTypeDef",
     "ListBotsRequestListBotsPaginateTypeDef",
     "ListBotsRequestRequestTypeDef",
-    "ListBotsResponseTypeDef",
+    "ListBotsResponseOutputTypeDef",
     "ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     "ListContactEvaluationsRequestRequestTypeDef",
-    "ListContactEvaluationsResponseTypeDef",
+    "ListContactEvaluationsResponseOutputTypeDef",
     "ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
     "ListContactFlowModulesRequestRequestTypeDef",
-    "ListContactFlowModulesResponseTypeDef",
+    "ListContactFlowModulesResponseOutputTypeDef",
     "ListContactFlowsRequestListContactFlowsPaginateTypeDef",
     "ListContactFlowsRequestRequestTypeDef",
-    "ListContactFlowsResponseTypeDef",
+    "ListContactFlowsResponseOutputTypeDef",
     "ListContactReferencesRequestListContactReferencesPaginateTypeDef",
     "ListContactReferencesRequestRequestTypeDef",
-    "ListContactReferencesResponseTypeDef",
+    "ListContactReferencesResponseOutputTypeDef",
     "ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef",
     "ListDefaultVocabulariesRequestRequestTypeDef",
-    "ListDefaultVocabulariesResponseTypeDef",
+    "ListDefaultVocabulariesResponseOutputTypeDef",
     "ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
     "ListEvaluationFormVersionsRequestRequestTypeDef",
-    "ListEvaluationFormVersionsResponseTypeDef",
+    "ListEvaluationFormVersionsResponseOutputTypeDef",
     "ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
     "ListEvaluationFormsRequestRequestTypeDef",
-    "ListEvaluationFormsResponseTypeDef",
+    "ListEvaluationFormsResponseOutputTypeDef",
     "ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
     "ListHoursOfOperationsRequestRequestTypeDef",
-    "ListHoursOfOperationsResponseTypeDef",
+    "ListHoursOfOperationsResponseOutputTypeDef",
     "ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
     "ListInstanceAttributesRequestRequestTypeDef",
-    "ListInstanceAttributesResponseTypeDef",
+    "ListInstanceAttributesResponseOutputTypeDef",
     "ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
     "ListInstanceStorageConfigsRequestRequestTypeDef",
-    "ListInstanceStorageConfigsResponseTypeDef",
+    "ListInstanceStorageConfigsResponseOutputTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
-    "ListInstancesResponseTypeDef",
+    "ListInstancesResponseOutputTypeDef",
     "ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef",
     "ListIntegrationAssociationsRequestRequestTypeDef",
-    "ListIntegrationAssociationsResponseTypeDef",
+    "ListIntegrationAssociationsResponseOutputTypeDef",
     "ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
     "ListLambdaFunctionsRequestRequestTypeDef",
-    "ListLambdaFunctionsResponseTypeDef",
+    "ListLambdaFunctionsResponseOutputTypeDef",
     "ListLexBotsRequestListLexBotsPaginateTypeDef",
     "ListLexBotsRequestRequestTypeDef",
-    "ListLexBotsResponseTypeDef",
+    "ListLexBotsResponseOutputTypeDef",
     "ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
-    "ListPhoneNumbersResponseTypeDef",
-    "ListPhoneNumbersSummaryTypeDef",
+    "ListPhoneNumbersResponseOutputTypeDef",
+    "ListPhoneNumbersSummaryOutputTypeDef",
     "ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef",
     "ListPhoneNumbersV2RequestRequestTypeDef",
-    "ListPhoneNumbersV2ResponseTypeDef",
+    "ListPhoneNumbersV2ResponseOutputTypeDef",
     "ListPromptsRequestListPromptsPaginateTypeDef",
     "ListPromptsRequestRequestTypeDef",
-    "ListPromptsResponseTypeDef",
+    "ListPromptsResponseOutputTypeDef",
     "ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
     "ListQueueQuickConnectsRequestRequestTypeDef",
-    "ListQueueQuickConnectsResponseTypeDef",
+    "ListQueueQuickConnectsResponseOutputTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "ListQueuesResponseTypeDef",
+    "ListQueuesResponseOutputTypeDef",
     "ListQuickConnectsRequestListQuickConnectsPaginateTypeDef",
     "ListQuickConnectsRequestRequestTypeDef",
-    "ListQuickConnectsResponseTypeDef",
+    "ListQuickConnectsResponseOutputTypeDef",
     "ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
     "ListRoutingProfileQueuesRequestRequestTypeDef",
-    "ListRoutingProfileQueuesResponseTypeDef",
+    "ListRoutingProfileQueuesResponseOutputTypeDef",
     "ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     "ListRoutingProfilesRequestRequestTypeDef",
-    "ListRoutingProfilesResponseTypeDef",
+    "ListRoutingProfilesResponseOutputTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
-    "ListRulesResponseTypeDef",
+    "ListRulesResponseOutputTypeDef",
     "ListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
     "ListSecurityKeysRequestRequestTypeDef",
-    "ListSecurityKeysResponseTypeDef",
+    "ListSecurityKeysResponseOutputTypeDef",
     "ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
     "ListSecurityProfilePermissionsRequestRequestTypeDef",
-    "ListSecurityProfilePermissionsResponseTypeDef",
+    "ListSecurityProfilePermissionsResponseOutputTypeDef",
     "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     "ListSecurityProfilesRequestRequestTypeDef",
-    "ListSecurityProfilesResponseTypeDef",
+    "ListSecurityProfilesResponseOutputTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
     "ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef",
     "ListTaskTemplatesRequestRequestTypeDef",
-    "ListTaskTemplatesResponseTypeDef",
+    "ListTaskTemplatesResponseOutputTypeDef",
     "ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef",
     "ListTrafficDistributionGroupsRequestRequestTypeDef",
-    "ListTrafficDistributionGroupsResponseTypeDef",
+    "ListTrafficDistributionGroupsResponseOutputTypeDef",
     "ListUseCasesRequestListUseCasesPaginateTypeDef",
     "ListUseCasesRequestRequestTypeDef",
-    "ListUseCasesResponseTypeDef",
+    "ListUseCasesResponseOutputTypeDef",
     "ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
     "ListUserHierarchyGroupsRequestRequestTypeDef",
-    "ListUserHierarchyGroupsResponseTypeDef",
+    "ListUserHierarchyGroupsResponseOutputTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
-    "ListUsersResponseTypeDef",
+    "ListUsersResponseOutputTypeDef",
+    "MediaConcurrencyOutputTypeDef",
     "MediaConcurrencyTypeDef",
-    "MetricDataV2TypeDef",
+    "MetricDataV2OutputTypeDef",
+    "MetricFilterV2OutputTypeDef",
     "MetricFilterV2TypeDef",
-    "MetricResultV2TypeDef",
+    "MetricResultV2OutputTypeDef",
+    "MetricV2OutputTypeDef",
     "MetricV2TypeDef",
     "MonitorContactRequestRequestTypeDef",
-    "MonitorContactResponseTypeDef",
+    "MonitorContactResponseOutputTypeDef",
+    "NotificationRecipientTypeOutputTypeDef",
     "NotificationRecipientTypeTypeDef",
-    "NumberReferenceTypeDef",
+    "NumberReferenceOutputTypeDef",
+    "NumericQuestionPropertyValueAutomationOutputTypeDef",
     "NumericQuestionPropertyValueAutomationTypeDef",
+    "OutboundCallerConfigOutputTypeDef",
     "OutboundCallerConfigTypeDef",
     "PaginatorConfigTypeDef",
     "ParticipantDetailsToAddTypeDef",
     "ParticipantDetailsTypeDef",
     "ParticipantTimerConfigurationTypeDef",
     "ParticipantTimerValueTypeDef",
-    "ParticipantTokenCredentialsTypeDef",
+    "ParticipantTokenCredentialsOutputTypeDef",
     "PersistentChatTypeDef",
+    "PhoneNumberQuickConnectConfigOutputTypeDef",
     "PhoneNumberQuickConnectConfigTypeDef",
-    "PhoneNumberStatusTypeDef",
-    "PhoneNumberSummaryTypeDef",
+    "PhoneNumberStatusOutputTypeDef",
+    "PhoneNumberSummaryOutputTypeDef",
+    "PromptOutputTypeDef",
     "PromptSearchCriteriaTypeDef",
     "PromptSearchFilterTypeDef",
-    "PromptSummaryTypeDef",
-    "PromptTypeDef",
+    "PromptSummaryOutputTypeDef",
     "PutUserStatusRequestRequestTypeDef",
-    "QueueInfoTypeDef",
+    "QueueInfoOutputTypeDef",
+    "QueueOutputTypeDef",
+    "QueueQuickConnectConfigOutputTypeDef",
     "QueueQuickConnectConfigTypeDef",
-    "QueueReferenceTypeDef",
+    "QueueReferenceOutputTypeDef",
     "QueueSearchCriteriaTypeDef",
     "QueueSearchFilterTypeDef",
-    "QueueSummaryTypeDef",
-    "QueueTypeDef",
+    "QueueSummaryOutputTypeDef",
+    "QuickConnectConfigOutputTypeDef",
     "QuickConnectConfigTypeDef",
+    "QuickConnectOutputTypeDef",
     "QuickConnectSearchCriteriaTypeDef",
     "QuickConnectSearchFilterTypeDef",
-    "QuickConnectSummaryTypeDef",
-    "QuickConnectTypeDef",
+    "QuickConnectSummaryOutputTypeDef",
+    "ReadOnlyFieldInfoOutputTypeDef",
     "ReadOnlyFieldInfoTypeDef",
-    "ReferenceSummaryTypeDef",
+    "ReferenceOutputTypeDef",
+    "ReferenceSummaryOutputTypeDef",
     "ReferenceTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
     "ReplicateInstanceRequestRequestTypeDef",
-    "ReplicateInstanceResponseTypeDef",
+    "ReplicateInstanceResponseOutputTypeDef",
+    "RequiredFieldInfoOutputTypeDef",
     "RequiredFieldInfoTypeDef",
     "ResourceTagsSearchCriteriaTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeContactRecordingRequestRequestTypeDef",
-    "RoutingProfileQueueConfigSummaryTypeDef",
+    "RoutingProfileOutputTypeDef",
+    "RoutingProfileQueueConfigSummaryOutputTypeDef",
     "RoutingProfileQueueConfigTypeDef",
     "RoutingProfileQueueReferenceTypeDef",
-    "RoutingProfileReferenceTypeDef",
+    "RoutingProfileReferenceOutputTypeDef",
     "RoutingProfileSearchCriteriaTypeDef",
     "RoutingProfileSearchFilterTypeDef",
-    "RoutingProfileSummaryTypeDef",
-    "RoutingProfileTypeDef",
+    "RoutingProfileSummaryOutputTypeDef",
+    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
-    "RuleSummaryTypeDef",
+    "RuleOutputTypeDef",
+    "RuleSummaryOutputTypeDef",
+    "RuleTriggerEventSourceOutputTypeDef",
     "RuleTriggerEventSourceTypeDef",
-    "RuleTypeDef",
+    "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
+    "SearchAvailablePhoneNumbersResponseOutputTypeDef",
     "SearchHoursOfOperationsRequestRequestTypeDef",
     "SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef",
-    "SearchHoursOfOperationsResponseTypeDef",
+    "SearchHoursOfOperationsResponseOutputTypeDef",
     "SearchPromptsRequestRequestTypeDef",
     "SearchPromptsRequestSearchPromptsPaginateTypeDef",
-    "SearchPromptsResponseTypeDef",
+    "SearchPromptsResponseOutputTypeDef",
     "SearchQueuesRequestRequestTypeDef",
     "SearchQueuesRequestSearchQueuesPaginateTypeDef",
-    "SearchQueuesResponseTypeDef",
+    "SearchQueuesResponseOutputTypeDef",
     "SearchQuickConnectsRequestRequestTypeDef",
     "SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef",
-    "SearchQuickConnectsResponseTypeDef",
+    "SearchQuickConnectsResponseOutputTypeDef",
     "SearchResourceTagsRequestRequestTypeDef",
     "SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
-    "SearchResourceTagsResponseTypeDef",
+    "SearchResourceTagsResponseOutputTypeDef",
     "SearchRoutingProfilesRequestRequestTypeDef",
     "SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef",
-    "SearchRoutingProfilesResponseTypeDef",
+    "SearchRoutingProfilesResponseOutputTypeDef",
     "SearchSecurityProfilesRequestRequestTypeDef",
     "SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef",
-    "SearchSecurityProfilesResponseTypeDef",
+    "SearchSecurityProfilesResponseOutputTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchUsersRequestSearchUsersPaginateTypeDef",
-    "SearchUsersResponseTypeDef",
+    "SearchUsersResponseOutputTypeDef",
     "SearchVocabulariesRequestRequestTypeDef",
     "SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef",
-    "SearchVocabulariesResponseTypeDef",
-    "SecurityKeyTypeDef",
+    "SearchVocabulariesResponseOutputTypeDef",
+    "SecurityKeyOutputTypeDef",
+    "SecurityProfileOutputTypeDef",
     "SecurityProfileSearchCriteriaTypeDef",
-    "SecurityProfileSearchSummaryTypeDef",
-    "SecurityProfileSummaryTypeDef",
-    "SecurityProfileTypeDef",
+    "SecurityProfileSearchSummaryOutputTypeDef",
+    "SecurityProfileSummaryOutputTypeDef",
     "SecurityProfilesSearchFilterTypeDef",
+    "SendNotificationActionDefinitionOutputTypeDef",
     "SendNotificationActionDefinitionTypeDef",
+    "SingleSelectQuestionRuleCategoryAutomationOutputTypeDef",
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     "StartChatContactRequestRequestTypeDef",
-    "StartChatContactResponseTypeDef",
+    "StartChatContactResponseOutputTypeDef",
     "StartContactEvaluationRequestRequestTypeDef",
-    "StartContactEvaluationResponseTypeDef",
+    "StartContactEvaluationResponseOutputTypeDef",
     "StartContactRecordingRequestRequestTypeDef",
     "StartContactStreamingRequestRequestTypeDef",
-    "StartContactStreamingResponseTypeDef",
+    "StartContactStreamingResponseOutputTypeDef",
     "StartOutboundVoiceContactRequestRequestTypeDef",
-    "StartOutboundVoiceContactResponseTypeDef",
+    "StartOutboundVoiceContactResponseOutputTypeDef",
     "StartTaskContactRequestRequestTypeDef",
-    "StartTaskContactResponseTypeDef",
+    "StartTaskContactResponseOutputTypeDef",
     "StopContactRecordingRequestRequestTypeDef",
     "StopContactRequestRequestTypeDef",
     "StopContactStreamingRequestRequestTypeDef",
     "StringConditionTypeDef",
-    "StringReferenceTypeDef",
+    "StringReferenceOutputTypeDef",
     "SubmitContactEvaluationRequestRequestTypeDef",
-    "SubmitContactEvaluationResponseTypeDef",
+    "SubmitContactEvaluationResponseOutputTypeDef",
     "SuspendContactRecordingRequestRequestTypeDef",
     "TagConditionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TagSearchConditionTypeDef",
-    "TagSetTypeDef",
+    "TagSetOutputTypeDef",
+    "TaskActionDefinitionOutputTypeDef",
     "TaskActionDefinitionTypeDef",
+    "TaskTemplateConstraintsOutputTypeDef",
     "TaskTemplateConstraintsTypeDef",
+    "TaskTemplateDefaultFieldValueOutputTypeDef",
     "TaskTemplateDefaultFieldValueTypeDef",
+    "TaskTemplateDefaultsOutputTypeDef",
     "TaskTemplateDefaultsTypeDef",
+    "TaskTemplateFieldIdentifierOutputTypeDef",
     "TaskTemplateFieldIdentifierTypeDef",
+    "TaskTemplateFieldOutputTypeDef",
     "TaskTemplateFieldTypeDef",
-    "TaskTemplateMetadataTypeDef",
+    "TaskTemplateMetadataOutputTypeDef",
+    "TelephonyConfigOutputTypeDef",
     "TelephonyConfigTypeDef",
+    "ThresholdOutputTypeDef",
     "ThresholdTypeDef",
+    "ThresholdV2OutputTypeDef",
     "ThresholdV2TypeDef",
-    "TrafficDistributionGroupSummaryTypeDef",
-    "TrafficDistributionGroupTypeDef",
+    "TrafficDistributionGroupOutputTypeDef",
+    "TrafficDistributionGroupSummaryOutputTypeDef",
     "TransferContactRequestRequestTypeDef",
-    "TransferContactResponseTypeDef",
+    "TransferContactResponseOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
     "UpdateContactAttributesRequestRequestTypeDef",
     "UpdateContactEvaluationRequestRequestTypeDef",
-    "UpdateContactEvaluationResponseTypeDef",
+    "UpdateContactEvaluationResponseOutputTypeDef",
     "UpdateContactFlowContentRequestRequestTypeDef",
     "UpdateContactFlowMetadataRequestRequestTypeDef",
     "UpdateContactFlowModuleContentRequestRequestTypeDef",
     "UpdateContactFlowModuleMetadataRequestRequestTypeDef",
     "UpdateContactFlowNameRequestRequestTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "UpdateContactScheduleRequestRequestTypeDef",
     "UpdateEvaluationFormRequestRequestTypeDef",
-    "UpdateEvaluationFormResponseTypeDef",
+    "UpdateEvaluationFormResponseOutputTypeDef",
     "UpdateHoursOfOperationRequestRequestTypeDef",
     "UpdateInstanceAttributeRequestRequestTypeDef",
     "UpdateInstanceStorageConfigRequestRequestTypeDef",
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
-    "UpdatePhoneNumberResponseTypeDef",
+    "UpdatePhoneNumberResponseOutputTypeDef",
     "UpdatePromptRequestRequestTypeDef",
-    "UpdatePromptResponseTypeDef",
+    "UpdatePromptResponseOutputTypeDef",
     "UpdateQueueHoursOfOperationRequestRequestTypeDef",
     "UpdateQueueMaxContactsRequestRequestTypeDef",
     "UpdateQueueNameRequestRequestTypeDef",
     "UpdateQueueOutboundCallerConfigRequestRequestTypeDef",
     "UpdateQueueStatusRequestRequestTypeDef",
     "UpdateQuickConnectConfigRequestRequestTypeDef",
     "UpdateQuickConnectNameRequestRequestTypeDef",
     "UpdateRoutingProfileConcurrencyRequestRequestTypeDef",
     "UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef",
     "UpdateRoutingProfileNameRequestRequestTypeDef",
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "UpdateSecurityProfileRequestRequestTypeDef",
     "UpdateTaskTemplateRequestRequestTypeDef",
-    "UpdateTaskTemplateResponseTypeDef",
+    "UpdateTaskTemplateResponseOutputTypeDef",
     "UpdateTrafficDistributionRequestRequestTypeDef",
     "UpdateUserHierarchyGroupNameRequestRequestTypeDef",
     "UpdateUserHierarchyRequestRequestTypeDef",
     "UpdateUserHierarchyStructureRequestRequestTypeDef",
     "UpdateUserIdentityInfoRequestRequestTypeDef",
     "UpdateUserPhoneConfigRequestRequestTypeDef",
     "UpdateUserRoutingProfileRequestRequestTypeDef",
     "UpdateUserSecurityProfilesRequestRequestTypeDef",
-    "UrlReferenceTypeDef",
-    "UseCaseTypeDef",
+    "UrlReferenceOutputTypeDef",
+    "UseCaseOutputTypeDef",
     "UserDataFiltersTypeDef",
-    "UserDataTypeDef",
-    "UserIdentityInfoLiteTypeDef",
+    "UserDataOutputTypeDef",
+    "UserIdentityInfoLiteOutputTypeDef",
+    "UserIdentityInfoOutputTypeDef",
     "UserIdentityInfoTypeDef",
+    "UserOutputTypeDef",
+    "UserPhoneConfigOutputTypeDef",
     "UserPhoneConfigTypeDef",
+    "UserQuickConnectConfigOutputTypeDef",
     "UserQuickConnectConfigTypeDef",
-    "UserReferenceTypeDef",
+    "UserReferenceOutputTypeDef",
     "UserSearchCriteriaTypeDef",
     "UserSearchFilterTypeDef",
-    "UserSearchSummaryTypeDef",
-    "UserSummaryTypeDef",
-    "UserTypeDef",
-    "VocabularySummaryTypeDef",
-    "VocabularyTypeDef",
+    "UserSearchSummaryOutputTypeDef",
+    "UserSummaryOutputTypeDef",
+    "VocabularyOutputTypeDef",
+    "VocabularySummaryOutputTypeDef",
     "VoiceRecordingConfigurationTypeDef",
-    "WisdomInfoTypeDef",
+    "WisdomInfoOutputTypeDef",
 )
 
-ActionSummaryTypeDef = TypedDict(
-    "ActionSummaryTypeDef",
+ActionSummaryOutputTypeDef = TypedDict(
+    "ActionSummaryOutputTypeDef",
     {
         "ActionType": ActionTypeType,
     },
 )
 
 ActivateEvaluationFormRequestRequestTypeDef = TypedDict(
     "ActivateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
     },
 )
 
-ActivateEvaluationFormResponseTypeDef = TypedDict(
-    "ActivateEvaluationFormResponseTypeDef",
+ActivateEvaluationFormResponseOutputTypeDef = TypedDict(
+    "ActivateEvaluationFormResponseOutputTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AgentContactReferenceTypeDef = TypedDict(
-    "AgentContactReferenceTypeDef",
+AgentContactReferenceOutputTypeDef = TypedDict(
+    "AgentContactReferenceOutputTypeDef",
     {
         "ContactId": str,
         "Channel": ChannelType,
         "InitiationMethod": ContactInitiationMethodType,
         "AgentContactState": ContactStateType,
         "StateStartTimestamp": datetime,
         "ConnectedToAgentTimestamp": datetime,
-        "Queue": "QueueReferenceTypeDef",
+        "Queue": "QueueReferenceOutputTypeDef",
     },
 )
 
-AgentInfoTypeDef = TypedDict(
-    "AgentInfoTypeDef",
+AgentInfoOutputTypeDef = TypedDict(
+    "AgentInfoOutputTypeDef",
     {
         "Id": str,
         "ConnectedToAgentTimestamp": datetime,
     },
 )
 
-AgentStatusReferenceTypeDef = TypedDict(
-    "AgentStatusReferenceTypeDef",
+AgentStatusOutputTypeDef = TypedDict(
+    "AgentStatusOutputTypeDef",
+    {
+        "AgentStatusARN": str,
+        "AgentStatusId": str,
+        "Name": str,
+        "Description": str,
+        "Type": AgentStatusTypeType,
+        "DisplayOrder": int,
+        "State": AgentStatusStateType,
+        "Tags": Dict[str, str],
+    },
+)
+
+AgentStatusReferenceOutputTypeDef = TypedDict(
+    "AgentStatusReferenceOutputTypeDef",
     {
         "StatusStartTimestamp": datetime,
         "StatusArn": str,
         "StatusName": str,
     },
 )
 
-AgentStatusSummaryTypeDef = TypedDict(
-    "AgentStatusSummaryTypeDef",
+AgentStatusSummaryOutputTypeDef = TypedDict(
+    "AgentStatusSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": AgentStatusTypeType,
     },
 )
 
-AgentStatusTypeDef = TypedDict(
-    "AgentStatusTypeDef",
-    {
-        "AgentStatusARN": str,
-        "AgentStatusId": str,
-        "Name": str,
-        "Description": str,
-        "Type": AgentStatusTypeType,
-        "DisplayOrder": int,
-        "State": AgentStatusStateType,
-        "Tags": Dict[str, str],
-    },
-)
-
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "EnableAnswerMachineDetection": bool,
         "AwaitAnswerMachinePrompt": bool,
     },
     total=False,
@@ -747,21 +804,19 @@
     {
         "LexBot": "LexBotTypeDef",
         "LexV2Bot": "LexV2BotTypeDef",
     },
     total=False,
 )
 
-
 class AssociateBotRequestRequestTypeDef(
     _RequiredAssociateBotRequestRequestTypeDef, _OptionalAssociateBotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAssociateDefaultVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateDefaultVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LanguageCode": VocabularyLanguageCodeType,
     },
 )
@@ -769,33 +824,31 @@
     "_OptionalAssociateDefaultVocabularyRequestRequestTypeDef",
     {
         "VocabularyId": str,
     },
     total=False,
 )
 
-
 class AssociateDefaultVocabularyRequestRequestTypeDef(
     _RequiredAssociateDefaultVocabularyRequestRequestTypeDef,
     _OptionalAssociateDefaultVocabularyRequestRequestTypeDef,
 ):
     pass
 
-
 AssociateInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
         "StorageConfig": "InstanceStorageConfigTypeDef",
     },
 )
 
-AssociateInstanceStorageConfigResponseTypeDef = TypedDict(
-    "AssociateInstanceStorageConfigResponseTypeDef",
+AssociateInstanceStorageConfigResponseOutputTypeDef = TypedDict(
+    "AssociateInstanceStorageConfigResponseOutputTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateLambdaFunctionRequestRequestTypeDef = TypedDict(
@@ -845,41 +898,41 @@
     "AssociateSecurityKeyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Key": str,
     },
 )
 
-AssociateSecurityKeyResponseTypeDef = TypedDict(
-    "AssociateSecurityKeyResponseTypeDef",
+AssociateSecurityKeyResponseOutputTypeDef = TypedDict(
+    "AssociateSecurityKeyResponseOutputTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachmentReferenceTypeDef = TypedDict(
-    "AttachmentReferenceTypeDef",
+AttachmentReferenceOutputTypeDef = TypedDict(
+    "AttachmentReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
         "Status": ReferenceStatusType,
     },
 )
 
-AttributeTypeDef = TypedDict(
-    "AttributeTypeDef",
+AttributeOutputTypeDef = TypedDict(
+    "AttributeOutputTypeDef",
     {
         "AttributeType": InstanceAttributeTypeType,
         "Value": str,
     },
 )
 
-AvailableNumberSummaryTypeDef = TypedDict(
-    "AvailableNumberSummaryTypeDef",
+AvailableNumberSummaryOutputTypeDef = TypedDict(
+    "AvailableNumberSummaryOutputTypeDef",
     {
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
 )
 
@@ -918,121 +971,119 @@
         "PhoneNumberDescription": str,
         "Tags": Mapping[str, str],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class ClaimPhoneNumberRequestRequestTypeDef(
     _RequiredClaimPhoneNumberRequestRequestTypeDef, _OptionalClaimPhoneNumberRequestRequestTypeDef
 ):
     pass
 
-
-ClaimPhoneNumberResponseTypeDef = TypedDict(
-    "ClaimPhoneNumberResponseTypeDef",
+ClaimPhoneNumberResponseOutputTypeDef = TypedDict(
+    "ClaimPhoneNumberResponseOutputTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ClaimedPhoneNumberSummaryTypeDef = TypedDict(
-    "ClaimedPhoneNumberSummaryTypeDef",
+ClaimedPhoneNumberSummaryOutputTypeDef = TypedDict(
+    "ClaimedPhoneNumberSummaryOutputTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberDescription": str,
         "TargetArn": str,
         "Tags": Dict[str, str],
-        "PhoneNumberStatus": "PhoneNumberStatusTypeDef",
+        "PhoneNumberStatus": "PhoneNumberStatusOutputTypeDef",
     },
 )
 
 ContactFilterTypeDef = TypedDict(
     "ContactFilterTypeDef",
     {
         "ContactStates": Sequence[ContactStateType],
     },
     total=False,
 )
 
-ContactFlowModuleSummaryTypeDef = TypedDict(
-    "ContactFlowModuleSummaryTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "State": ContactFlowModuleStateType,
-    },
-)
-
-ContactFlowModuleTypeDef = TypedDict(
-    "ContactFlowModuleTypeDef",
+ContactFlowModuleOutputTypeDef = TypedDict(
+    "ContactFlowModuleOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Content": str,
         "Description": str,
         "State": ContactFlowModuleStateType,
         "Status": ContactFlowModuleStatusType,
         "Tags": Dict[str, str],
     },
 )
 
-ContactFlowSummaryTypeDef = TypedDict(
-    "ContactFlowSummaryTypeDef",
+ContactFlowModuleSummaryOutputTypeDef = TypedDict(
+    "ContactFlowModuleSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
-        "ContactFlowType": ContactFlowTypeType,
-        "ContactFlowState": ContactFlowStateType,
+        "State": ContactFlowModuleStateType,
     },
 )
 
-ContactFlowTypeDef = TypedDict(
-    "ContactFlowTypeDef",
+ContactFlowOutputTypeDef = TypedDict(
+    "ContactFlowOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Type": ContactFlowTypeType,
         "State": ContactFlowStateType,
         "Description": str,
         "Content": str,
         "Tags": Dict[str, str],
     },
 )
 
-ContactTypeDef = TypedDict(
-    "ContactTypeDef",
+ContactFlowSummaryOutputTypeDef = TypedDict(
+    "ContactFlowSummaryOutputTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "ContactFlowType": ContactFlowTypeType,
+        "ContactFlowState": ContactFlowStateType,
+    },
+)
+
+ContactOutputTypeDef = TypedDict(
+    "ContactOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "InitialContactId": str,
         "PreviousContactId": str,
         "InitiationMethod": ContactInitiationMethodType,
         "Name": str,
         "Description": str,
         "Channel": ChannelType,
-        "QueueInfo": "QueueInfoTypeDef",
-        "AgentInfo": "AgentInfoTypeDef",
+        "QueueInfo": "QueueInfoOutputTypeDef",
+        "AgentInfo": "AgentInfoOutputTypeDef",
         "InitiationTimestamp": datetime,
         "DisconnectTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "ScheduledTimestamp": datetime,
         "RelatedContactId": str,
-        "WisdomInfo": "WisdomInfoTypeDef",
+        "WisdomInfo": "WisdomInfoOutputTypeDef",
     },
 )
 
 ControlPlaneTagFilterTypeDef = TypedDict(
     "ControlPlaneTagFilterTypeDef",
     {
         "OrConditions": Sequence[Sequence["TagConditionTypeDef"]],
@@ -1056,23 +1107,21 @@
         "Description": str,
         "DisplayOrder": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAgentStatusRequestRequestTypeDef(
     _RequiredCreateAgentStatusRequestRequestTypeDef, _OptionalCreateAgentStatusRequestRequestTypeDef
 ):
     pass
 
-
-CreateAgentStatusResponseTypeDef = TypedDict(
-    "CreateAgentStatusResponseTypeDef",
+CreateAgentStatusResponseOutputTypeDef = TypedDict(
+    "CreateAgentStatusResponseOutputTypeDef",
     {
         "AgentStatusARN": str,
         "AgentStatusId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1090,24 +1139,22 @@
         "Description": str,
         "Tags": Mapping[str, str],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateContactFlowModuleRequestRequestTypeDef(
     _RequiredCreateContactFlowModuleRequestRequestTypeDef,
     _OptionalCreateContactFlowModuleRequestRequestTypeDef,
 ):
     pass
 
-
-CreateContactFlowModuleResponseTypeDef = TypedDict(
-    "CreateContactFlowModuleResponseTypeDef",
+CreateContactFlowModuleResponseOutputTypeDef = TypedDict(
+    "CreateContactFlowModuleResponseOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1125,23 +1172,21 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateContactFlowRequestRequestTypeDef(
     _RequiredCreateContactFlowRequestRequestTypeDef, _OptionalCreateContactFlowRequestRequestTypeDef
 ):
     pass
 
-
-CreateContactFlowResponseTypeDef = TypedDict(
-    "CreateContactFlowResponseTypeDef",
+CreateContactFlowResponseOutputTypeDef = TypedDict(
+    "CreateContactFlowResponseOutputTypeDef",
     {
         "ContactFlowId": str,
         "ContactFlowArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1159,24 +1204,22 @@
         "Description": str,
         "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateEvaluationFormRequestRequestTypeDef(
     _RequiredCreateEvaluationFormRequestRequestTypeDef,
     _OptionalCreateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-
-CreateEvaluationFormResponseTypeDef = TypedDict(
-    "CreateEvaluationFormResponseTypeDef",
+CreateEvaluationFormResponseOutputTypeDef = TypedDict(
+    "CreateEvaluationFormResponseOutputTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1194,24 +1237,22 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateHoursOfOperationRequestRequestTypeDef(
     _RequiredCreateHoursOfOperationRequestRequestTypeDef,
     _OptionalCreateHoursOfOperationRequestRequestTypeDef,
 ):
     pass
 
-
-CreateHoursOfOperationResponseTypeDef = TypedDict(
-    "CreateHoursOfOperationResponseTypeDef",
+CreateHoursOfOperationResponseOutputTypeDef = TypedDict(
+    "CreateHoursOfOperationResponseOutputTypeDef",
     {
         "HoursOfOperationId": str,
         "HoursOfOperationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1229,23 +1270,21 @@
         "ClientToken": str,
         "InstanceAlias": str,
         "DirectoryId": str,
     },
     total=False,
 )
 
-
 class CreateInstanceRequestRequestTypeDef(
     _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
 ):
     pass
 
-
-CreateInstanceResponseTypeDef = TypedDict(
-    "CreateInstanceResponseTypeDef",
+CreateInstanceResponseOutputTypeDef = TypedDict(
+    "CreateInstanceResponseOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1264,24 +1303,22 @@
         "SourceApplicationName": str,
         "SourceType": SourceTypeType,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateIntegrationAssociationRequestRequestTypeDef(
     _RequiredCreateIntegrationAssociationRequestRequestTypeDef,
     _OptionalCreateIntegrationAssociationRequestRequestTypeDef,
 ):
     pass
 
-
-CreateIntegrationAssociationResponseTypeDef = TypedDict(
-    "CreateIntegrationAssociationResponseTypeDef",
+CreateIntegrationAssociationResponseOutputTypeDef = TypedDict(
+    "CreateIntegrationAssociationResponseOutputTypeDef",
     {
         "IntegrationAssociationId": str,
         "IntegrationAssociationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1297,25 +1334,23 @@
     "_OptionalCreateParticipantRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateParticipantRequestRequestTypeDef(
     _RequiredCreateParticipantRequestRequestTypeDef, _OptionalCreateParticipantRequestRequestTypeDef
 ):
     pass
 
-
-CreateParticipantResponseTypeDef = TypedDict(
-    "CreateParticipantResponseTypeDef",
+CreateParticipantResponseOutputTypeDef = TypedDict(
+    "CreateParticipantResponseOutputTypeDef",
     {
-        "ParticipantCredentials": "ParticipantTokenCredentialsTypeDef",
+        "ParticipantCredentials": "ParticipantTokenCredentialsOutputTypeDef",
         "ParticipantId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePromptRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePromptRequestRequestTypeDef",
@@ -1330,23 +1365,21 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreatePromptRequestRequestTypeDef(
     _RequiredCreatePromptRequestRequestTypeDef, _OptionalCreatePromptRequestRequestTypeDef
 ):
     pass
 
-
-CreatePromptResponseTypeDef = TypedDict(
-    "CreatePromptResponseTypeDef",
+CreatePromptResponseOutputTypeDef = TypedDict(
+    "CreatePromptResponseOutputTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1366,23 +1399,21 @@
         "MaxContacts": int,
         "QuickConnectIds": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateQueueRequestRequestTypeDef(
     _RequiredCreateQueueRequestRequestTypeDef, _OptionalCreateQueueRequestRequestTypeDef
 ):
     pass
 
-
-CreateQueueResponseTypeDef = TypedDict(
-    "CreateQueueResponseTypeDef",
+CreateQueueResponseOutputTypeDef = TypedDict(
+    "CreateQueueResponseOutputTypeDef",
     {
         "QueueArn": str,
         "QueueId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1399,24 +1430,22 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateQuickConnectRequestRequestTypeDef(
     _RequiredCreateQuickConnectRequestRequestTypeDef,
     _OptionalCreateQuickConnectRequestRequestTypeDef,
 ):
     pass
 
-
-CreateQuickConnectResponseTypeDef = TypedDict(
-    "CreateQuickConnectResponseTypeDef",
+CreateQuickConnectResponseOutputTypeDef = TypedDict(
+    "CreateQuickConnectResponseOutputTypeDef",
     {
         "QuickConnectARN": str,
         "QuickConnectId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1435,24 +1464,22 @@
     {
         "QueueConfigs": Sequence["RoutingProfileQueueConfigTypeDef"],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateRoutingProfileRequestRequestTypeDef(
     _RequiredCreateRoutingProfileRequestRequestTypeDef,
     _OptionalCreateRoutingProfileRequestRequestTypeDef,
 ):
     pass
 
-
-CreateRoutingProfileResponseTypeDef = TypedDict(
-    "CreateRoutingProfileResponseTypeDef",
+CreateRoutingProfileResponseOutputTypeDef = TypedDict(
+    "CreateRoutingProfileResponseOutputTypeDef",
     {
         "RoutingProfileArn": str,
         "RoutingProfileId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1471,23 +1498,21 @@
     "_OptionalCreateRuleRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateRuleRequestRequestTypeDef(
     _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
 ):
     pass
 
-
-CreateRuleResponseTypeDef = TypedDict(
-    "CreateRuleResponseTypeDef",
+CreateRuleResponseOutputTypeDef = TypedDict(
+    "CreateRuleResponseOutputTypeDef",
     {
         "RuleArn": str,
         "RuleId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1506,24 +1531,22 @@
         "Tags": Mapping[str, str],
         "AllowedAccessControlTags": Mapping[str, str],
         "TagRestrictedResources": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateSecurityProfileRequestRequestTypeDef(
     _RequiredCreateSecurityProfileRequestRequestTypeDef,
     _OptionalCreateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
-
-CreateSecurityProfileResponseTypeDef = TypedDict(
-    "CreateSecurityProfileResponseTypeDef",
+CreateSecurityProfileResponseOutputTypeDef = TypedDict(
+    "CreateSecurityProfileResponseOutputTypeDef",
     {
         "SecurityProfileId": str,
         "SecurityProfileArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1544,24 +1567,22 @@
         "Defaults": "TaskTemplateDefaultsTypeDef",
         "Status": TaskTemplateStatusType,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateTaskTemplateRequestRequestTypeDef(
     _RequiredCreateTaskTemplateRequestRequestTypeDef,
     _OptionalCreateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
-
-CreateTaskTemplateResponseTypeDef = TypedDict(
-    "CreateTaskTemplateResponseTypeDef",
+CreateTaskTemplateResponseOutputTypeDef = TypedDict(
+    "CreateTaskTemplateResponseOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1578,24 +1599,22 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateTrafficDistributionGroupRequestRequestTypeDef(
     _RequiredCreateTrafficDistributionGroupRequestRequestTypeDef,
     _OptionalCreateTrafficDistributionGroupRequestRequestTypeDef,
 ):
     pass
 
-
-CreateTrafficDistributionGroupResponseTypeDef = TypedDict(
-    "CreateTrafficDistributionGroupResponseTypeDef",
+CreateTrafficDistributionGroupResponseOutputTypeDef = TypedDict(
+    "CreateTrafficDistributionGroupResponseOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1611,23 +1630,21 @@
     "_OptionalCreateUseCaseRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateUseCaseRequestRequestTypeDef(
     _RequiredCreateUseCaseRequestRequestTypeDef, _OptionalCreateUseCaseRequestRequestTypeDef
 ):
     pass
 
-
-CreateUseCaseResponseTypeDef = TypedDict(
-    "CreateUseCaseResponseTypeDef",
+CreateUseCaseResponseOutputTypeDef = TypedDict(
+    "CreateUseCaseResponseOutputTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1643,24 +1660,22 @@
     {
         "ParentGroupId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateUserHierarchyGroupRequestRequestTypeDef(
     _RequiredCreateUserHierarchyGroupRequestRequestTypeDef,
     _OptionalCreateUserHierarchyGroupRequestRequestTypeDef,
 ):
     pass
 
-
-CreateUserHierarchyGroupResponseTypeDef = TypedDict(
-    "CreateUserHierarchyGroupResponseTypeDef",
+CreateUserHierarchyGroupResponseOutputTypeDef = TypedDict(
+    "CreateUserHierarchyGroupResponseOutputTypeDef",
     {
         "HierarchyGroupId": str,
         "HierarchyGroupArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1682,23 +1697,21 @@
         "DirectoryUserId": str,
         "HierarchyGroupId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
+CreateUserResponseOutputTypeDef = TypedDict(
+    "CreateUserResponseOutputTypeDef",
     {
         "UserId": str,
         "UserArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1716,61 +1729,74 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
-
-CreateVocabularyResponseTypeDef = TypedDict(
-    "CreateVocabularyResponseTypeDef",
+CreateVocabularyResponseOutputTypeDef = TypedDict(
+    "CreateVocabularyResponseOutputTypeDef",
     {
         "VocabularyArn": str,
         "VocabularyId": str,
         "State": VocabularyStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CredentialsTypeDef = TypedDict(
-    "CredentialsTypeDef",
+CredentialsOutputTypeDef = TypedDict(
+    "CredentialsOutputTypeDef",
     {
         "AccessToken": str,
         "AccessTokenExpiration": datetime,
         "RefreshToken": str,
         "RefreshTokenExpiration": datetime,
     },
 )
 
+CrossChannelBehaviorOutputTypeDef = TypedDict(
+    "CrossChannelBehaviorOutputTypeDef",
+    {
+        "BehaviorType": BehaviorTypeType,
+    },
+)
+
 CrossChannelBehaviorTypeDef = TypedDict(
     "CrossChannelBehaviorTypeDef",
     {
         "BehaviorType": BehaviorTypeType,
     },
 )
 
-CurrentMetricDataTypeDef = TypedDict(
-    "CurrentMetricDataTypeDef",
+CurrentMetricDataOutputTypeDef = TypedDict(
+    "CurrentMetricDataOutputTypeDef",
     {
-        "Metric": "CurrentMetricTypeDef",
+        "Metric": "CurrentMetricOutputTypeDef",
         "Value": float,
     },
 )
 
-CurrentMetricResultTypeDef = TypedDict(
-    "CurrentMetricResultTypeDef",
+CurrentMetricOutputTypeDef = TypedDict(
+    "CurrentMetricOutputTypeDef",
+    {
+        "Name": CurrentMetricNameType,
+        "Unit": UnitType,
+    },
+)
+
+CurrentMetricResultOutputTypeDef = TypedDict(
+    "CurrentMetricResultOutputTypeDef",
     {
-        "Dimensions": "DimensionsTypeDef",
-        "Collections": List["CurrentMetricDataTypeDef"],
+        "Dimensions": "DimensionsOutputTypeDef",
+        "Collections": List["CurrentMetricDataOutputTypeDef"],
     },
 )
 
 CurrentMetricSortCriteriaTypeDef = TypedDict(
     "CurrentMetricSortCriteriaTypeDef",
     {
         "SortByMetric": CurrentMetricNameType,
@@ -1784,16 +1810,16 @@
     {
         "Name": CurrentMetricNameType,
         "Unit": UnitType,
     },
     total=False,
 )
 
-DateReferenceTypeDef = TypedDict(
-    "DateReferenceTypeDef",
+DateReferenceOutputTypeDef = TypedDict(
+    "DateReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 DeactivateEvaluationFormRequestRequestTypeDef = TypedDict(
@@ -1801,26 +1827,26 @@
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
     },
 )
 
-DeactivateEvaluationFormResponseTypeDef = TypedDict(
-    "DeactivateEvaluationFormResponseTypeDef",
+DeactivateEvaluationFormResponseOutputTypeDef = TypedDict(
+    "DeactivateEvaluationFormResponseOutputTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DefaultVocabularyTypeDef = TypedDict(
-    "DefaultVocabularyTypeDef",
+DefaultVocabularyOutputTypeDef = TypedDict(
+    "DefaultVocabularyOutputTypeDef",
     {
         "InstanceId": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "VocabularyId": str,
         "VocabularyName": str,
     },
 )
@@ -1860,22 +1886,20 @@
     "_OptionalDeleteEvaluationFormRequestRequestTypeDef",
     {
         "EvaluationFormVersion": int,
     },
     total=False,
 )
 
-
 class DeleteEvaluationFormRequestRequestTypeDef(
     _RequiredDeleteEvaluationFormRequestRequestTypeDef,
     _OptionalDeleteEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteHoursOfOperationRequestRequestTypeDef = TypedDict(
     "DeleteHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "HoursOfOperationId": str,
     },
 )
@@ -1987,16 +2011,16 @@
     "DeleteVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "VocabularyId": str,
     },
 )
 
-DeleteVocabularyResponseTypeDef = TypedDict(
-    "DeleteVocabularyResponseTypeDef",
+DeleteVocabularyResponseOutputTypeDef = TypedDict(
+    "DeleteVocabularyResponseOutputTypeDef",
     {
         "VocabularyArn": str,
         "VocabularyId": str,
         "State": VocabularyStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2005,83 +2029,83 @@
     "DescribeAgentStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AgentStatusId": str,
     },
 )
 
-DescribeAgentStatusResponseTypeDef = TypedDict(
-    "DescribeAgentStatusResponseTypeDef",
+DescribeAgentStatusResponseOutputTypeDef = TypedDict(
+    "DescribeAgentStatusResponseOutputTypeDef",
     {
-        "AgentStatus": "AgentStatusTypeDef",
+        "AgentStatus": "AgentStatusOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactEvaluationRequestRequestTypeDef = TypedDict(
     "DescribeContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
     },
 )
 
-DescribeContactEvaluationResponseTypeDef = TypedDict(
-    "DescribeContactEvaluationResponseTypeDef",
+DescribeContactEvaluationResponseOutputTypeDef = TypedDict(
+    "DescribeContactEvaluationResponseOutputTypeDef",
     {
-        "Evaluation": "EvaluationTypeDef",
-        "EvaluationForm": "EvaluationFormContentTypeDef",
+        "Evaluation": "EvaluationOutputTypeDef",
+        "EvaluationForm": "EvaluationFormContentOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactFlowModuleRequestRequestTypeDef = TypedDict(
     "DescribeContactFlowModuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowModuleId": str,
     },
 )
 
-DescribeContactFlowModuleResponseTypeDef = TypedDict(
-    "DescribeContactFlowModuleResponseTypeDef",
+DescribeContactFlowModuleResponseOutputTypeDef = TypedDict(
+    "DescribeContactFlowModuleResponseOutputTypeDef",
     {
-        "ContactFlowModule": "ContactFlowModuleTypeDef",
+        "ContactFlowModule": "ContactFlowModuleOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactFlowRequestRequestTypeDef = TypedDict(
     "DescribeContactFlowRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowId": str,
     },
 )
 
-DescribeContactFlowResponseTypeDef = TypedDict(
-    "DescribeContactFlowResponseTypeDef",
+DescribeContactFlowResponseOutputTypeDef = TypedDict(
+    "DescribeContactFlowResponseOutputTypeDef",
     {
-        "ContactFlow": "ContactFlowTypeDef",
+        "ContactFlow": "ContactFlowOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactRequestRequestTypeDef = TypedDict(
     "DescribeContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
 
-DescribeContactResponseTypeDef = TypedDict(
-    "DescribeContactResponseTypeDef",
+DescribeContactResponseOutputTypeDef = TypedDict(
+    "DescribeContactResponseOutputTypeDef",
     {
-        "Contact": "ContactTypeDef",
+        "Contact": "ContactOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeEvaluationFormRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEvaluationFormRequestRequestTypeDef",
     {
@@ -2093,289 +2117,287 @@
     "_OptionalDescribeEvaluationFormRequestRequestTypeDef",
     {
         "EvaluationFormVersion": int,
     },
     total=False,
 )
 
-
 class DescribeEvaluationFormRequestRequestTypeDef(
     _RequiredDescribeEvaluationFormRequestRequestTypeDef,
     _OptionalDescribeEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeEvaluationFormResponseTypeDef = TypedDict(
-    "DescribeEvaluationFormResponseTypeDef",
+DescribeEvaluationFormResponseOutputTypeDef = TypedDict(
+    "DescribeEvaluationFormResponseOutputTypeDef",
     {
-        "EvaluationForm": "EvaluationFormTypeDef",
+        "EvaluationForm": "EvaluationFormOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeHoursOfOperationRequestRequestTypeDef = TypedDict(
     "DescribeHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "HoursOfOperationId": str,
     },
 )
 
-DescribeHoursOfOperationResponseTypeDef = TypedDict(
-    "DescribeHoursOfOperationResponseTypeDef",
+DescribeHoursOfOperationResponseOutputTypeDef = TypedDict(
+    "DescribeHoursOfOperationResponseOutputTypeDef",
     {
-        "HoursOfOperation": "HoursOfOperationTypeDef",
+        "HoursOfOperation": "HoursOfOperationOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceAttributeRequestRequestTypeDef = TypedDict(
     "DescribeInstanceAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AttributeType": InstanceAttributeTypeType,
     },
 )
 
-DescribeInstanceAttributeResponseTypeDef = TypedDict(
-    "DescribeInstanceAttributeResponseTypeDef",
+DescribeInstanceAttributeResponseOutputTypeDef = TypedDict(
+    "DescribeInstanceAttributeResponseOutputTypeDef",
     {
-        "Attribute": "AttributeTypeDef",
+        "Attribute": "AttributeOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceRequestRequestTypeDef = TypedDict(
     "DescribeInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-DescribeInstanceResponseTypeDef = TypedDict(
-    "DescribeInstanceResponseTypeDef",
+DescribeInstanceResponseOutputTypeDef = TypedDict(
+    "DescribeInstanceResponseOutputTypeDef",
     {
-        "Instance": "InstanceTypeDef",
+        "Instance": "InstanceOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "DescribeInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AssociationId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
 )
 
-DescribeInstanceStorageConfigResponseTypeDef = TypedDict(
-    "DescribeInstanceStorageConfigResponseTypeDef",
+DescribeInstanceStorageConfigResponseOutputTypeDef = TypedDict(
+    "DescribeInstanceStorageConfigResponseOutputTypeDef",
     {
-        "StorageConfig": "InstanceStorageConfigTypeDef",
+        "StorageConfig": "InstanceStorageConfigOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePhoneNumberRequestRequestTypeDef = TypedDict(
     "DescribePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-DescribePhoneNumberResponseTypeDef = TypedDict(
-    "DescribePhoneNumberResponseTypeDef",
+DescribePhoneNumberResponseOutputTypeDef = TypedDict(
+    "DescribePhoneNumberResponseOutputTypeDef",
     {
-        "ClaimedPhoneNumberSummary": "ClaimedPhoneNumberSummaryTypeDef",
+        "ClaimedPhoneNumberSummary": "ClaimedPhoneNumberSummaryOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePromptRequestRequestTypeDef = TypedDict(
     "DescribePromptRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
-DescribePromptResponseTypeDef = TypedDict(
-    "DescribePromptResponseTypeDef",
+DescribePromptResponseOutputTypeDef = TypedDict(
+    "DescribePromptResponseOutputTypeDef",
     {
-        "Prompt": "PromptTypeDef",
+        "Prompt": "PromptOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueueRequestRequestTypeDef = TypedDict(
     "DescribeQueueRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
 
-DescribeQueueResponseTypeDef = TypedDict(
-    "DescribeQueueResponseTypeDef",
+DescribeQueueResponseOutputTypeDef = TypedDict(
+    "DescribeQueueResponseOutputTypeDef",
     {
-        "Queue": "QueueTypeDef",
+        "Queue": "QueueOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQuickConnectRequestRequestTypeDef = TypedDict(
     "DescribeQuickConnectRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QuickConnectId": str,
     },
 )
 
-DescribeQuickConnectResponseTypeDef = TypedDict(
-    "DescribeQuickConnectResponseTypeDef",
+DescribeQuickConnectResponseOutputTypeDef = TypedDict(
+    "DescribeQuickConnectResponseOutputTypeDef",
     {
-        "QuickConnect": "QuickConnectTypeDef",
+        "QuickConnect": "QuickConnectOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRoutingProfileRequestRequestTypeDef = TypedDict(
     "DescribeRoutingProfileRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
     },
 )
 
-DescribeRoutingProfileResponseTypeDef = TypedDict(
-    "DescribeRoutingProfileResponseTypeDef",
+DescribeRoutingProfileResponseOutputTypeDef = TypedDict(
+    "DescribeRoutingProfileResponseOutputTypeDef",
     {
-        "RoutingProfile": "RoutingProfileTypeDef",
+        "RoutingProfile": "RoutingProfileOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRuleRequestRequestTypeDef = TypedDict(
     "DescribeRuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RuleId": str,
     },
 )
 
-DescribeRuleResponseTypeDef = TypedDict(
-    "DescribeRuleResponseTypeDef",
+DescribeRuleResponseOutputTypeDef = TypedDict(
+    "DescribeRuleResponseOutputTypeDef",
     {
-        "Rule": "RuleTypeDef",
+        "Rule": "RuleOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSecurityProfileRequestRequestTypeDef = TypedDict(
     "DescribeSecurityProfileRequestRequestTypeDef",
     {
         "SecurityProfileId": str,
         "InstanceId": str,
     },
 )
 
-DescribeSecurityProfileResponseTypeDef = TypedDict(
-    "DescribeSecurityProfileResponseTypeDef",
+DescribeSecurityProfileResponseOutputTypeDef = TypedDict(
+    "DescribeSecurityProfileResponseOutputTypeDef",
     {
-        "SecurityProfile": "SecurityProfileTypeDef",
+        "SecurityProfile": "SecurityProfileOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrafficDistributionGroupRequestRequestTypeDef = TypedDict(
     "DescribeTrafficDistributionGroupRequestRequestTypeDef",
     {
         "TrafficDistributionGroupId": str,
     },
 )
 
-DescribeTrafficDistributionGroupResponseTypeDef = TypedDict(
-    "DescribeTrafficDistributionGroupResponseTypeDef",
+DescribeTrafficDistributionGroupResponseOutputTypeDef = TypedDict(
+    "DescribeTrafficDistributionGroupResponseOutputTypeDef",
     {
-        "TrafficDistributionGroup": "TrafficDistributionGroupTypeDef",
+        "TrafficDistributionGroup": "TrafficDistributionGroupOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserHierarchyGroupRequestRequestTypeDef = TypedDict(
     "DescribeUserHierarchyGroupRequestRequestTypeDef",
     {
         "HierarchyGroupId": str,
         "InstanceId": str,
     },
 )
 
-DescribeUserHierarchyGroupResponseTypeDef = TypedDict(
-    "DescribeUserHierarchyGroupResponseTypeDef",
+DescribeUserHierarchyGroupResponseOutputTypeDef = TypedDict(
+    "DescribeUserHierarchyGroupResponseOutputTypeDef",
     {
-        "HierarchyGroup": "HierarchyGroupTypeDef",
+        "HierarchyGroup": "HierarchyGroupOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserHierarchyStructureRequestRequestTypeDef = TypedDict(
     "DescribeUserHierarchyStructureRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-DescribeUserHierarchyStructureResponseTypeDef = TypedDict(
-    "DescribeUserHierarchyStructureResponseTypeDef",
+DescribeUserHierarchyStructureResponseOutputTypeDef = TypedDict(
+    "DescribeUserHierarchyStructureResponseOutputTypeDef",
     {
-        "HierarchyStructure": "HierarchyStructureTypeDef",
+        "HierarchyStructure": "HierarchyStructureOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
     },
 )
 
-DescribeUserResponseTypeDef = TypedDict(
-    "DescribeUserResponseTypeDef",
+DescribeUserResponseOutputTypeDef = TypedDict(
+    "DescribeUserResponseOutputTypeDef",
     {
-        "User": "UserTypeDef",
+        "User": "UserOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVocabularyRequestRequestTypeDef = TypedDict(
     "DescribeVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "VocabularyId": str,
     },
 )
 
-DescribeVocabularyResponseTypeDef = TypedDict(
-    "DescribeVocabularyResponseTypeDef",
+DescribeVocabularyResponseOutputTypeDef = TypedDict(
+    "DescribeVocabularyResponseOutputTypeDef",
     {
-        "Vocabulary": "VocabularyTypeDef",
+        "Vocabulary": "VocabularyOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DimensionsTypeDef = TypedDict(
-    "DimensionsTypeDef",
+DimensionsOutputTypeDef = TypedDict(
+    "DimensionsOutputTypeDef",
     {
-        "Queue": "QueueReferenceTypeDef",
+        "Queue": "QueueReferenceOutputTypeDef",
         "Channel": ChannelType,
-        "RoutingProfile": "RoutingProfileReferenceTypeDef",
+        "RoutingProfile": "RoutingProfileReferenceOutputTypeDef",
     },
 )
 
 DisassociateApprovedOriginRequestRequestTypeDef = TypedDict(
     "DisassociateApprovedOriginRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -2394,21 +2416,19 @@
     {
         "LexBot": "LexBotTypeDef",
         "LexV2Bot": "LexV2BotTypeDef",
     },
     total=False,
 )
 
-
 class DisassociateBotRequestRequestTypeDef(
     _RequiredDisassociateBotRequestRequestTypeDef, _OptionalDisassociateBotRequestRequestTypeDef
 ):
     pass
 
-
 DisassociateInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "DisassociateInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AssociationId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
@@ -2470,100 +2490,151 @@
     {
         "UserId": str,
         "InstanceId": str,
         "ContactId": str,
     },
 )
 
+DistributionOutputTypeDef = TypedDict(
+    "DistributionOutputTypeDef",
+    {
+        "Region": str,
+        "Percentage": int,
+    },
+)
+
 DistributionTypeDef = TypedDict(
     "DistributionTypeDef",
     {
         "Region": str,
         "Percentage": int,
     },
 )
 
-EmailReferenceTypeDef = TypedDict(
-    "EmailReferenceTypeDef",
+EmailReferenceOutputTypeDef = TypedDict(
+    "EmailReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
+    {
+        "EncryptionType": Literal["KMS"],
+        "KeyId": str,
+    },
+)
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "EncryptionType": Literal["KMS"],
         "KeyId": str,
     },
 )
 
+EvaluationAnswerDataOutputTypeDef = TypedDict(
+    "EvaluationAnswerDataOutputTypeDef",
+    {
+        "StringValue": str,
+        "NumericValue": float,
+        "NotApplicable": bool,
+    },
+)
+
 EvaluationAnswerDataTypeDef = TypedDict(
     "EvaluationAnswerDataTypeDef",
     {
         "StringValue": str,
         "NumericValue": float,
         "NotApplicable": bool,
     },
+    total=False,
 )
 
 EvaluationAnswerInputTypeDef = TypedDict(
     "EvaluationAnswerInputTypeDef",
     {
         "Value": "EvaluationAnswerDataTypeDef",
     },
     total=False,
 )
 
-EvaluationAnswerOutputTypeDef = TypedDict(
-    "EvaluationAnswerOutputTypeDef",
+EvaluationAnswerOutputOutputTypeDef = TypedDict(
+    "EvaluationAnswerOutputOutputTypeDef",
     {
-        "Value": "EvaluationAnswerDataTypeDef",
-        "SystemSuggestedValue": "EvaluationAnswerDataTypeDef",
+        "Value": "EvaluationAnswerDataOutputTypeDef",
+        "SystemSuggestedValue": "EvaluationAnswerDataOutputTypeDef",
     },
 )
 
-EvaluationFormContentTypeDef = TypedDict(
-    "EvaluationFormContentTypeDef",
+EvaluationFormContentOutputTypeDef = TypedDict(
+    "EvaluationFormContentOutputTypeDef",
     {
         "EvaluationFormVersion": int,
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "Description": str,
-        "Items": List["EvaluationFormItemTypeDef"],
-        "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
+        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "ScoringStrategy": "EvaluationFormScoringStrategyOutputTypeDef",
+    },
+)
+
+EvaluationFormItemOutputTypeDef = TypedDict(
+    "EvaluationFormItemOutputTypeDef",
+    {
+        "Section": Dict[str, Any],
+        "Question": "EvaluationFormQuestionOutputTypeDef",
     },
 )
 
 EvaluationFormItemTypeDef = TypedDict(
     "EvaluationFormItemTypeDef",
     {
         "Section": Dict[str, Any],
         "Question": "EvaluationFormQuestionTypeDef",
     },
     total=False,
 )
 
+EvaluationFormNumericQuestionAutomationOutputTypeDef = TypedDict(
+    "EvaluationFormNumericQuestionAutomationOutputTypeDef",
+    {
+        "PropertyValue": "NumericQuestionPropertyValueAutomationOutputTypeDef",
+    },
+)
+
 EvaluationFormNumericQuestionAutomationTypeDef = TypedDict(
     "EvaluationFormNumericQuestionAutomationTypeDef",
     {
         "PropertyValue": "NumericQuestionPropertyValueAutomationTypeDef",
     },
     total=False,
 )
 
+EvaluationFormNumericQuestionOptionOutputTypeDef = TypedDict(
+    "EvaluationFormNumericQuestionOptionOutputTypeDef",
+    {
+        "MinValue": int,
+        "MaxValue": int,
+        "Score": int,
+        "AutomaticFail": bool,
+    },
+)
+
 _RequiredEvaluationFormNumericQuestionOptionTypeDef = TypedDict(
     "_RequiredEvaluationFormNumericQuestionOptionTypeDef",
     {
         "MinValue": int,
         "MaxValue": int,
     },
 )
@@ -2572,21 +2643,29 @@
     {
         "Score": int,
         "AutomaticFail": bool,
     },
     total=False,
 )
 
-
 class EvaluationFormNumericQuestionOptionTypeDef(
     _RequiredEvaluationFormNumericQuestionOptionTypeDef,
     _OptionalEvaluationFormNumericQuestionOptionTypeDef,
 ):
     pass
 
+EvaluationFormNumericQuestionPropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
+    {
+        "MinValue": int,
+        "MaxValue": int,
+        "Options": List["EvaluationFormNumericQuestionOptionOutputTypeDef"],
+        "Automation": "EvaluationFormNumericQuestionAutomationOutputTypeDef",
+    },
+)
 
 _RequiredEvaluationFormNumericQuestionPropertiesTypeDef = TypedDict(
     "_RequiredEvaluationFormNumericQuestionPropertiesTypeDef",
     {
         "MinValue": int,
         "MaxValue": int,
     },
@@ -2596,21 +2675,52 @@
     {
         "Options": Sequence["EvaluationFormNumericQuestionOptionTypeDef"],
         "Automation": "EvaluationFormNumericQuestionAutomationTypeDef",
     },
     total=False,
 )
 
-
 class EvaluationFormNumericQuestionPropertiesTypeDef(
     _RequiredEvaluationFormNumericQuestionPropertiesTypeDef,
     _OptionalEvaluationFormNumericQuestionPropertiesTypeDef,
 ):
     pass
 
+EvaluationFormOutputTypeDef = TypedDict(
+    "EvaluationFormOutputTypeDef",
+    {
+        "EvaluationFormId": str,
+        "EvaluationFormVersion": int,
+        "Locked": bool,
+        "EvaluationFormArn": str,
+        "Title": str,
+        "Description": str,
+        "Status": EvaluationFormVersionStatusType,
+        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "ScoringStrategy": "EvaluationFormScoringStrategyOutputTypeDef",
+        "CreatedTime": datetime,
+        "CreatedBy": str,
+        "LastModifiedTime": datetime,
+        "LastModifiedBy": str,
+        "Tags": Dict[str, str],
+    },
+)
+
+EvaluationFormQuestionOutputTypeDef = TypedDict(
+    "EvaluationFormQuestionOutputTypeDef",
+    {
+        "Title": str,
+        "Instructions": str,
+        "RefId": str,
+        "NotApplicableEnabled": bool,
+        "QuestionType": EvaluationFormQuestionTypeType,
+        "QuestionTypeProperties": "EvaluationFormQuestionTypePropertiesOutputTypeDef",
+        "Weight": float,
+    },
+)
 
 _RequiredEvaluationFormQuestionTypeDef = TypedDict(
     "_RequiredEvaluationFormQuestionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "QuestionType": EvaluationFormQuestionTypeType,
@@ -2623,38 +2733,63 @@
         "NotApplicableEnabled": bool,
         "QuestionTypeProperties": "EvaluationFormQuestionTypePropertiesTypeDef",
         "Weight": float,
     },
     total=False,
 )
 
-
 class EvaluationFormQuestionTypeDef(
     _RequiredEvaluationFormQuestionTypeDef, _OptionalEvaluationFormQuestionTypeDef
 ):
     pass
 
+EvaluationFormQuestionTypePropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
+    {
+        "Numeric": "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
+        "SingleSelect": "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
+    },
+)
 
 EvaluationFormQuestionTypePropertiesTypeDef = TypedDict(
     "EvaluationFormQuestionTypePropertiesTypeDef",
     {
         "Numeric": "EvaluationFormNumericQuestionPropertiesTypeDef",
         "SingleSelect": "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
     },
     total=False,
 )
 
+EvaluationFormScoringStrategyOutputTypeDef = TypedDict(
+    "EvaluationFormScoringStrategyOutputTypeDef",
+    {
+        "Mode": EvaluationFormScoringModeType,
+        "Status": EvaluationFormScoringStatusType,
+    },
+)
+
 EvaluationFormScoringStrategyTypeDef = TypedDict(
     "EvaluationFormScoringStrategyTypeDef",
     {
         "Mode": EvaluationFormScoringModeType,
         "Status": EvaluationFormScoringStatusType,
     },
 )
 
+EvaluationFormSectionOutputTypeDef = TypedDict(
+    "EvaluationFormSectionOutputTypeDef",
+    {
+        "Title": str,
+        "RefId": str,
+        "Instructions": str,
+        "Items": List[Dict[str, Any]],
+        "Weight": float,
+    },
+)
+
 _RequiredEvaluationFormSectionTypeDef = TypedDict(
     "_RequiredEvaluationFormSectionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "Items": Sequence[Dict[str, Any]],
     },
@@ -2664,50 +2799,71 @@
     {
         "Instructions": str,
         "Weight": float,
     },
     total=False,
 )
 
-
 class EvaluationFormSectionTypeDef(
     _RequiredEvaluationFormSectionTypeDef, _OptionalEvaluationFormSectionTypeDef
 ):
     pass
 
+EvaluationFormSingleSelectQuestionAutomationOptionOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionAutomationOptionOutputTypeDef",
+    {
+        "RuleCategory": "SingleSelectQuestionRuleCategoryAutomationOutputTypeDef",
+    },
+)
 
 EvaluationFormSingleSelectQuestionAutomationOptionTypeDef = TypedDict(
     "EvaluationFormSingleSelectQuestionAutomationOptionTypeDef",
     {
         "RuleCategory": "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     },
     total=False,
 )
 
+EvaluationFormSingleSelectQuestionAutomationOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
+    {
+        "Options": List["EvaluationFormSingleSelectQuestionAutomationOptionOutputTypeDef"],
+        "DefaultOptionRefId": str,
+    },
+)
+
 _RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef = TypedDict(
     "_RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef",
     {
         "Options": Sequence["EvaluationFormSingleSelectQuestionAutomationOptionTypeDef"],
     },
 )
 _OptionalEvaluationFormSingleSelectQuestionAutomationTypeDef = TypedDict(
     "_OptionalEvaluationFormSingleSelectQuestionAutomationTypeDef",
     {
         "DefaultOptionRefId": str,
     },
     total=False,
 )
 
-
 class EvaluationFormSingleSelectQuestionAutomationTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionAutomationTypeDef,
 ):
     pass
 
+EvaluationFormSingleSelectQuestionOptionOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionOptionOutputTypeDef",
+    {
+        "RefId": str,
+        "Text": str,
+        "Score": int,
+        "AutomaticFail": bool,
+    },
+)
 
 _RequiredEvaluationFormSingleSelectQuestionOptionTypeDef = TypedDict(
     "_RequiredEvaluationFormSingleSelectQuestionOptionTypeDef",
     {
         "RefId": str,
         "Text": str,
     },
@@ -2717,21 +2873,28 @@
     {
         "Score": int,
         "AutomaticFail": bool,
     },
     total=False,
 )
 
-
 class EvaluationFormSingleSelectQuestionOptionTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionOptionTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionOptionTypeDef,
 ):
     pass
 
+EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
+    {
+        "Options": List["EvaluationFormSingleSelectQuestionOptionOutputTypeDef"],
+        "DisplayAs": EvaluationFormSingleSelectQuestionDisplayModeType,
+        "Automation": "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
+    },
+)
 
 _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef = TypedDict(
     "_RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef",
     {
         "Options": Sequence["EvaluationFormSingleSelectQuestionOptionTypeDef"],
     },
 )
@@ -2740,24 +2903,22 @@
     {
         "DisplayAs": EvaluationFormSingleSelectQuestionDisplayModeType,
         "Automation": "EvaluationFormSingleSelectQuestionAutomationTypeDef",
     },
     total=False,
 )
 
-
 class EvaluationFormSingleSelectQuestionPropertiesTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionPropertiesTypeDef,
 ):
     pass
 
-
-EvaluationFormSummaryTypeDef = TypedDict(
-    "EvaluationFormSummaryTypeDef",
+EvaluationFormSummaryOutputTypeDef = TypedDict(
+    "EvaluationFormSummaryOutputTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
@@ -2765,103 +2926,98 @@
         "LastActivatedTime": datetime,
         "LastActivatedBy": str,
         "LatestVersion": int,
         "ActiveVersion": int,
     },
 )
 
-EvaluationFormTypeDef = TypedDict(
-    "EvaluationFormTypeDef",
-    {
-        "EvaluationFormId": str,
-        "EvaluationFormVersion": int,
-        "Locked": bool,
-        "EvaluationFormArn": str,
-        "Title": str,
-        "Description": str,
-        "Status": EvaluationFormVersionStatusType,
-        "Items": List["EvaluationFormItemTypeDef"],
-        "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
-        "CreatedTime": datetime,
-        "CreatedBy": str,
-        "LastModifiedTime": datetime,
-        "LastModifiedBy": str,
-        "Tags": Dict[str, str],
-    },
-)
-
-EvaluationFormVersionSummaryTypeDef = TypedDict(
-    "EvaluationFormVersionSummaryTypeDef",
+EvaluationFormVersionSummaryOutputTypeDef = TypedDict(
+    "EvaluationFormVersionSummaryOutputTypeDef",
     {
         "EvaluationFormArn": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
         "Status": EvaluationFormVersionStatusType,
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
     },
 )
 
-EvaluationMetadataTypeDef = TypedDict(
-    "EvaluationMetadataTypeDef",
+EvaluationMetadataOutputTypeDef = TypedDict(
+    "EvaluationMetadataOutputTypeDef",
     {
         "ContactId": str,
         "EvaluatorArn": str,
         "ContactAgentId": str,
-        "Score": "EvaluationScoreTypeDef",
+        "Score": "EvaluationScoreOutputTypeDef",
+    },
+)
+
+EvaluationNoteOutputTypeDef = TypedDict(
+    "EvaluationNoteOutputTypeDef",
+    {
+        "Value": str,
     },
 )
 
 EvaluationNoteTypeDef = TypedDict(
     "EvaluationNoteTypeDef",
     {
         "Value": str,
     },
+    total=False,
+)
+
+EvaluationOutputTypeDef = TypedDict(
+    "EvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "EvaluationArn": str,
+        "Metadata": "EvaluationMetadataOutputTypeDef",
+        "Answers": Dict[str, "EvaluationAnswerOutputOutputTypeDef"],
+        "Notes": Dict[str, "EvaluationNoteOutputTypeDef"],
+        "Status": EvaluationStatusType,
+        "Scores": Dict[str, "EvaluationScoreOutputTypeDef"],
+        "CreatedTime": datetime,
+        "LastModifiedTime": datetime,
+        "Tags": Dict[str, str],
+    },
 )
 
-EvaluationScoreTypeDef = TypedDict(
-    "EvaluationScoreTypeDef",
+EvaluationScoreOutputTypeDef = TypedDict(
+    "EvaluationScoreOutputTypeDef",
     {
         "Percentage": float,
         "NotApplicable": bool,
         "AutomaticFail": bool,
     },
 )
 
-EvaluationSummaryTypeDef = TypedDict(
-    "EvaluationSummaryTypeDef",
+EvaluationSummaryOutputTypeDef = TypedDict(
+    "EvaluationSummaryOutputTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "EvaluationFormTitle": str,
         "EvaluationFormId": str,
         "Status": EvaluationStatusType,
         "EvaluatorArn": str,
-        "Score": "EvaluationScoreTypeDef",
+        "Score": "EvaluationScoreOutputTypeDef",
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
     },
 )
 
-EvaluationTypeDef = TypedDict(
-    "EvaluationTypeDef",
+EventBridgeActionDefinitionOutputTypeDef = TypedDict(
+    "EventBridgeActionDefinitionOutputTypeDef",
     {
-        "EvaluationId": str,
-        "EvaluationArn": str,
-        "Metadata": "EvaluationMetadataTypeDef",
-        "Answers": Dict[str, "EvaluationAnswerOutputTypeDef"],
-        "Notes": Dict[str, "EvaluationNoteTypeDef"],
-        "Status": EvaluationStatusType,
-        "Scores": Dict[str, "EvaluationScoreTypeDef"],
-        "CreatedTime": datetime,
-        "LastModifiedTime": datetime,
-        "Tags": Dict[str, str],
+        "Name": str,
     },
 )
 
 EventBridgeActionDefinitionTypeDef = TypedDict(
     "EventBridgeActionDefinitionTypeDef",
     {
         "Name": str,
@@ -2891,16 +3047,16 @@
     "GetContactAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "InitialContactId": str,
     },
 )
 
-GetContactAttributesResponseTypeDef = TypedDict(
-    "GetContactAttributesResponseTypeDef",
+GetContactAttributesResponseOutputTypeDef = TypedDict(
+    "GetContactAttributesResponseOutputTypeDef",
     {
         "Attributes": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetCurrentMetricDataRequestRequestTypeDef = TypedDict(
@@ -2918,27 +3074,25 @@
         "NextToken": str,
         "MaxResults": int,
         "SortCriteria": Sequence["CurrentMetricSortCriteriaTypeDef"],
     },
     total=False,
 )
 
-
 class GetCurrentMetricDataRequestRequestTypeDef(
     _RequiredGetCurrentMetricDataRequestRequestTypeDef,
     _OptionalGetCurrentMetricDataRequestRequestTypeDef,
 ):
     pass
 
-
-GetCurrentMetricDataResponseTypeDef = TypedDict(
-    "GetCurrentMetricDataResponseTypeDef",
+GetCurrentMetricDataResponseOutputTypeDef = TypedDict(
+    "GetCurrentMetricDataResponseOutputTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["CurrentMetricResultTypeDef"],
+        "MetricResults": List["CurrentMetricResultOutputTypeDef"],
         "DataSnapshotTime": datetime,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetCurrentUserDataRequestRequestTypeDef = TypedDict(
@@ -2953,43 +3107,41 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetCurrentUserDataRequestRequestTypeDef(
     _RequiredGetCurrentUserDataRequestRequestTypeDef,
     _OptionalGetCurrentUserDataRequestRequestTypeDef,
 ):
     pass
 
-
-GetCurrentUserDataResponseTypeDef = TypedDict(
-    "GetCurrentUserDataResponseTypeDef",
+GetCurrentUserDataResponseOutputTypeDef = TypedDict(
+    "GetCurrentUserDataResponseOutputTypeDef",
     {
         "NextToken": str,
-        "UserDataList": List["UserDataTypeDef"],
+        "UserDataList": List["UserDataOutputTypeDef"],
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFederationTokenRequestRequestTypeDef = TypedDict(
     "GetFederationTokenRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-GetFederationTokenResponseTypeDef = TypedDict(
-    "GetFederationTokenResponseTypeDef",
+GetFederationTokenResponseOutputTypeDef = TypedDict(
+    "GetFederationTokenResponseOutputTypeDef",
     {
-        "Credentials": "CredentialsTypeDef",
+        "Credentials": "CredentialsOutputTypeDef",
         "SignInUrl": str,
         "UserArn": str,
         "UserId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -3008,22 +3160,20 @@
     {
         "Groupings": Sequence[GroupingType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetMetricDataRequestGetMetricDataPaginateTypeDef(
     _RequiredGetMetricDataRequestGetMetricDataPaginateTypeDef,
     _OptionalGetMetricDataRequestGetMetricDataPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetMetricDataRequestRequestTypeDef = TypedDict(
     "_RequiredGetMetricDataRequestRequestTypeDef",
     {
         "InstanceId": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Filters": "FiltersTypeDef",
@@ -3036,26 +3186,24 @@
         "Groupings": Sequence[GroupingType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetMetricDataRequestRequestTypeDef(
     _RequiredGetMetricDataRequestRequestTypeDef, _OptionalGetMetricDataRequestRequestTypeDef
 ):
     pass
 
-
-GetMetricDataResponseTypeDef = TypedDict(
-    "GetMetricDataResponseTypeDef",
+GetMetricDataResponseOutputTypeDef = TypedDict(
+    "GetMetricDataResponseOutputTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["HistoricalMetricResultTypeDef"],
+        "MetricResults": List["HistoricalMetricResultOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetMetricDataV2RequestRequestTypeDef = TypedDict(
     "_RequiredGetMetricDataV2RequestRequestTypeDef",
     {
@@ -3072,40 +3220,38 @@
         "Groupings": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetMetricDataV2RequestRequestTypeDef(
     _RequiredGetMetricDataV2RequestRequestTypeDef, _OptionalGetMetricDataV2RequestRequestTypeDef
 ):
     pass
 
-
-GetMetricDataV2ResponseTypeDef = TypedDict(
-    "GetMetricDataV2ResponseTypeDef",
+GetMetricDataV2ResponseOutputTypeDef = TypedDict(
+    "GetMetricDataV2ResponseOutputTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["MetricResultV2TypeDef"],
+        "MetricResults": List["MetricResultV2OutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPromptFileRequestRequestTypeDef = TypedDict(
     "GetPromptFileRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
-GetPromptFileResponseTypeDef = TypedDict(
-    "GetPromptFileResponseTypeDef",
+GetPromptFileResponseOutputTypeDef = TypedDict(
+    "GetPromptFileResponseOutputTypeDef",
     {
         "PromptPresignedUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTaskTemplateRequestRequestTypeDef = TypedDict(
@@ -3119,33 +3265,31 @@
     "_OptionalGetTaskTemplateRequestRequestTypeDef",
     {
         "SnapshotVersion": str,
     },
     total=False,
 )
 
-
 class GetTaskTemplateRequestRequestTypeDef(
     _RequiredGetTaskTemplateRequestRequestTypeDef, _OptionalGetTaskTemplateRequestRequestTypeDef
 ):
     pass
 
-
-GetTaskTemplateResponseTypeDef = TypedDict(
-    "GetTaskTemplateResponseTypeDef",
+GetTaskTemplateResponseOutputTypeDef = TypedDict(
+    "GetTaskTemplateResponseOutputTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
-        "Constraints": "TaskTemplateConstraintsTypeDef",
-        "Defaults": "TaskTemplateDefaultsTypeDef",
-        "Fields": List["TaskTemplateFieldTypeDef"],
+        "Constraints": "TaskTemplateConstraintsOutputTypeDef",
+        "Defaults": "TaskTemplateDefaultsOutputTypeDef",
+        "Fields": List["TaskTemplateFieldOutputTypeDef"],
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3153,18 +3297,18 @@
 GetTrafficDistributionRequestRequestTypeDef = TypedDict(
     "GetTrafficDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetTrafficDistributionResponseTypeDef = TypedDict(
-    "GetTrafficDistributionResponseTypeDef",
+GetTrafficDistributionResponseOutputTypeDef = TypedDict(
+    "GetTrafficDistributionResponseOutputTypeDef",
     {
-        "TelephonyConfig": "TelephonyConfigTypeDef",
+        "TelephonyConfig": "TelephonyConfigOutputTypeDef",
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HierarchyGroupConditionTypeDef = TypedDict(
@@ -3172,89 +3316,89 @@
     {
         "Value": str,
         "HierarchyGroupMatchType": HierarchyGroupMatchTypeType,
     },
     total=False,
 )
 
-HierarchyGroupSummaryReferenceTypeDef = TypedDict(
-    "HierarchyGroupSummaryReferenceTypeDef",
+HierarchyGroupOutputTypeDef = TypedDict(
+    "HierarchyGroupOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
+        "Name": str,
+        "LevelId": str,
+        "HierarchyPath": "HierarchyPathOutputTypeDef",
+        "Tags": Dict[str, str],
     },
 )
 
-HierarchyGroupSummaryTypeDef = TypedDict(
-    "HierarchyGroupSummaryTypeDef",
+HierarchyGroupSummaryOutputTypeDef = TypedDict(
+    "HierarchyGroupSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
-HierarchyGroupTypeDef = TypedDict(
-    "HierarchyGroupTypeDef",
+HierarchyGroupSummaryReferenceOutputTypeDef = TypedDict(
+    "HierarchyGroupSummaryReferenceOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
-        "Name": str,
-        "LevelId": str,
-        "HierarchyPath": "HierarchyPathTypeDef",
-        "Tags": Dict[str, str],
     },
 )
 
-HierarchyLevelTypeDef = TypedDict(
-    "HierarchyLevelTypeDef",
+HierarchyLevelOutputTypeDef = TypedDict(
+    "HierarchyLevelOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
 HierarchyLevelUpdateTypeDef = TypedDict(
     "HierarchyLevelUpdateTypeDef",
     {
         "Name": str,
     },
 )
 
-HierarchyPathReferenceTypeDef = TypedDict(
-    "HierarchyPathReferenceTypeDef",
+HierarchyPathOutputTypeDef = TypedDict(
+    "HierarchyPathOutputTypeDef",
     {
-        "LevelOne": "HierarchyGroupSummaryReferenceTypeDef",
-        "LevelTwo": "HierarchyGroupSummaryReferenceTypeDef",
-        "LevelThree": "HierarchyGroupSummaryReferenceTypeDef",
-        "LevelFour": "HierarchyGroupSummaryReferenceTypeDef",
-        "LevelFive": "HierarchyGroupSummaryReferenceTypeDef",
+        "LevelOne": "HierarchyGroupSummaryOutputTypeDef",
+        "LevelTwo": "HierarchyGroupSummaryOutputTypeDef",
+        "LevelThree": "HierarchyGroupSummaryOutputTypeDef",
+        "LevelFour": "HierarchyGroupSummaryOutputTypeDef",
+        "LevelFive": "HierarchyGroupSummaryOutputTypeDef",
     },
 )
 
-HierarchyPathTypeDef = TypedDict(
-    "HierarchyPathTypeDef",
+HierarchyPathReferenceOutputTypeDef = TypedDict(
+    "HierarchyPathReferenceOutputTypeDef",
     {
-        "LevelOne": "HierarchyGroupSummaryTypeDef",
-        "LevelTwo": "HierarchyGroupSummaryTypeDef",
-        "LevelThree": "HierarchyGroupSummaryTypeDef",
-        "LevelFour": "HierarchyGroupSummaryTypeDef",
-        "LevelFive": "HierarchyGroupSummaryTypeDef",
+        "LevelOne": "HierarchyGroupSummaryReferenceOutputTypeDef",
+        "LevelTwo": "HierarchyGroupSummaryReferenceOutputTypeDef",
+        "LevelThree": "HierarchyGroupSummaryReferenceOutputTypeDef",
+        "LevelFour": "HierarchyGroupSummaryReferenceOutputTypeDef",
+        "LevelFive": "HierarchyGroupSummaryReferenceOutputTypeDef",
     },
 )
 
-HierarchyStructureTypeDef = TypedDict(
-    "HierarchyStructureTypeDef",
+HierarchyStructureOutputTypeDef = TypedDict(
+    "HierarchyStructureOutputTypeDef",
     {
-        "LevelOne": "HierarchyLevelTypeDef",
-        "LevelTwo": "HierarchyLevelTypeDef",
-        "LevelThree": "HierarchyLevelTypeDef",
-        "LevelFour": "HierarchyLevelTypeDef",
-        "LevelFive": "HierarchyLevelTypeDef",
+        "LevelOne": "HierarchyLevelOutputTypeDef",
+        "LevelTwo": "HierarchyLevelOutputTypeDef",
+        "LevelThree": "HierarchyLevelOutputTypeDef",
+        "LevelFour": "HierarchyLevelOutputTypeDef",
+        "LevelFive": "HierarchyLevelOutputTypeDef",
     },
 )
 
 HierarchyStructureUpdateTypeDef = TypedDict(
     "HierarchyStructureUpdateTypeDef",
     {
         "LevelOne": "HierarchyLevelUpdateTypeDef",
@@ -3262,50 +3406,82 @@
         "LevelThree": "HierarchyLevelUpdateTypeDef",
         "LevelFour": "HierarchyLevelUpdateTypeDef",
         "LevelFive": "HierarchyLevelUpdateTypeDef",
     },
     total=False,
 )
 
-HistoricalMetricDataTypeDef = TypedDict(
-    "HistoricalMetricDataTypeDef",
+HistoricalMetricDataOutputTypeDef = TypedDict(
+    "HistoricalMetricDataOutputTypeDef",
     {
-        "Metric": "HistoricalMetricTypeDef",
+        "Metric": "HistoricalMetricOutputTypeDef",
         "Value": float,
     },
 )
 
-HistoricalMetricResultTypeDef = TypedDict(
-    "HistoricalMetricResultTypeDef",
+HistoricalMetricOutputTypeDef = TypedDict(
+    "HistoricalMetricOutputTypeDef",
+    {
+        "Name": HistoricalMetricNameType,
+        "Threshold": "ThresholdOutputTypeDef",
+        "Statistic": StatisticType,
+        "Unit": UnitType,
+    },
+)
+
+HistoricalMetricResultOutputTypeDef = TypedDict(
+    "HistoricalMetricResultOutputTypeDef",
     {
-        "Dimensions": "DimensionsTypeDef",
-        "Collections": List["HistoricalMetricDataTypeDef"],
+        "Dimensions": "DimensionsOutputTypeDef",
+        "Collections": List["HistoricalMetricDataOutputTypeDef"],
     },
 )
 
 HistoricalMetricTypeDef = TypedDict(
     "HistoricalMetricTypeDef",
     {
         "Name": HistoricalMetricNameType,
         "Threshold": "ThresholdTypeDef",
         "Statistic": StatisticType,
         "Unit": UnitType,
     },
     total=False,
 )
 
+HoursOfOperationConfigOutputTypeDef = TypedDict(
+    "HoursOfOperationConfigOutputTypeDef",
+    {
+        "Day": HoursOfOperationDaysType,
+        "StartTime": "HoursOfOperationTimeSliceOutputTypeDef",
+        "EndTime": "HoursOfOperationTimeSliceOutputTypeDef",
+    },
+)
+
 HoursOfOperationConfigTypeDef = TypedDict(
     "HoursOfOperationConfigTypeDef",
     {
         "Day": HoursOfOperationDaysType,
         "StartTime": "HoursOfOperationTimeSliceTypeDef",
         "EndTime": "HoursOfOperationTimeSliceTypeDef",
     },
 )
 
+HoursOfOperationOutputTypeDef = TypedDict(
+    "HoursOfOperationOutputTypeDef",
+    {
+        "HoursOfOperationId": str,
+        "HoursOfOperationArn": str,
+        "Name": str,
+        "Description": str,
+        "TimeZone": str,
+        "Config": List["HoursOfOperationConfigOutputTypeDef"],
+        "Tags": Dict[str, str],
+    },
+)
+
 HoursOfOperationSearchCriteriaTypeDef = TypedDict(
     "HoursOfOperationSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
@@ -3316,51 +3492,75 @@
     "HoursOfOperationSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-HoursOfOperationSummaryTypeDef = TypedDict(
-    "HoursOfOperationSummaryTypeDef",
+HoursOfOperationSummaryOutputTypeDef = TypedDict(
+    "HoursOfOperationSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
+HoursOfOperationTimeSliceOutputTypeDef = TypedDict(
+    "HoursOfOperationTimeSliceOutputTypeDef",
+    {
+        "Hours": int,
+        "Minutes": int,
+    },
+)
+
 HoursOfOperationTimeSliceTypeDef = TypedDict(
     "HoursOfOperationTimeSliceTypeDef",
     {
         "Hours": int,
         "Minutes": int,
     },
 )
 
-HoursOfOperationTypeDef = TypedDict(
-    "HoursOfOperationTypeDef",
+InstanceOutputTypeDef = TypedDict(
+    "InstanceOutputTypeDef",
     {
-        "HoursOfOperationId": str,
-        "HoursOfOperationArn": str,
-        "Name": str,
-        "Description": str,
-        "TimeZone": str,
-        "Config": List["HoursOfOperationConfigTypeDef"],
-        "Tags": Dict[str, str],
+        "Id": str,
+        "Arn": str,
+        "IdentityManagementType": DirectoryTypeType,
+        "InstanceAlias": str,
+        "CreatedTime": datetime,
+        "ServiceRole": str,
+        "InstanceStatus": InstanceStatusType,
+        "StatusReason": "InstanceStatusReasonOutputTypeDef",
+        "InboundCallsEnabled": bool,
+        "OutboundCallsEnabled": bool,
+        "InstanceAccessUrl": str,
     },
 )
 
-InstanceStatusReasonTypeDef = TypedDict(
-    "InstanceStatusReasonTypeDef",
+InstanceStatusReasonOutputTypeDef = TypedDict(
+    "InstanceStatusReasonOutputTypeDef",
     {
         "Message": str,
     },
 )
 
+InstanceStorageConfigOutputTypeDef = TypedDict(
+    "InstanceStorageConfigOutputTypeDef",
+    {
+        "AssociationId": str,
+        "StorageType": StorageTypeType,
+        "S3Config": "S3ConfigOutputTypeDef",
+        "KinesisVideoStreamConfig": "KinesisVideoStreamConfigOutputTypeDef",
+        "KinesisStreamConfig": "KinesisStreamConfigOutputTypeDef",
+        "KinesisFirehoseConfig": "KinesisFirehoseConfigOutputTypeDef",
+    },
+)
+
 _RequiredInstanceStorageConfigTypeDef = TypedDict(
     "_RequiredInstanceStorageConfigTypeDef",
     {
         "StorageType": StorageTypeType,
     },
 )
 _OptionalInstanceStorageConfigTypeDef = TypedDict(
@@ -3371,115 +3571,141 @@
         "KinesisVideoStreamConfig": "KinesisVideoStreamConfigTypeDef",
         "KinesisStreamConfig": "KinesisStreamConfigTypeDef",
         "KinesisFirehoseConfig": "KinesisFirehoseConfigTypeDef",
     },
     total=False,
 )
 
-
 class InstanceStorageConfigTypeDef(
     _RequiredInstanceStorageConfigTypeDef, _OptionalInstanceStorageConfigTypeDef
 ):
     pass
 
-
-InstanceSummaryTypeDef = TypedDict(
-    "InstanceSummaryTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "IdentityManagementType": DirectoryTypeType,
-        "InstanceAlias": str,
-        "CreatedTime": datetime,
-        "ServiceRole": str,
-        "InstanceStatus": InstanceStatusType,
-        "InboundCallsEnabled": bool,
-        "OutboundCallsEnabled": bool,
-        "InstanceAccessUrl": str,
-    },
-)
-
-InstanceTypeDef = TypedDict(
-    "InstanceTypeDef",
+InstanceSummaryOutputTypeDef = TypedDict(
+    "InstanceSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "IdentityManagementType": DirectoryTypeType,
         "InstanceAlias": str,
         "CreatedTime": datetime,
         "ServiceRole": str,
         "InstanceStatus": InstanceStatusType,
-        "StatusReason": "InstanceStatusReasonTypeDef",
         "InboundCallsEnabled": bool,
         "OutboundCallsEnabled": bool,
         "InstanceAccessUrl": str,
     },
 )
 
-IntegrationAssociationSummaryTypeDef = TypedDict(
-    "IntegrationAssociationSummaryTypeDef",
+IntegrationAssociationSummaryOutputTypeDef = TypedDict(
+    "IntegrationAssociationSummaryOutputTypeDef",
     {
         "IntegrationAssociationId": str,
         "IntegrationAssociationArn": str,
         "InstanceId": str,
         "IntegrationType": IntegrationTypeType,
         "IntegrationArn": str,
         "SourceApplicationUrl": str,
         "SourceApplicationName": str,
         "SourceType": SourceTypeType,
     },
 )
 
+InvisibleFieldInfoOutputTypeDef = TypedDict(
+    "InvisibleFieldInfoOutputTypeDef",
+    {
+        "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
+    },
+)
+
 InvisibleFieldInfoTypeDef = TypedDict(
     "InvisibleFieldInfoTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
     total=False,
 )
 
+KinesisFirehoseConfigOutputTypeDef = TypedDict(
+    "KinesisFirehoseConfigOutputTypeDef",
+    {
+        "FirehoseArn": str,
+    },
+)
+
 KinesisFirehoseConfigTypeDef = TypedDict(
     "KinesisFirehoseConfigTypeDef",
     {
         "FirehoseArn": str,
     },
 )
 
+KinesisStreamConfigOutputTypeDef = TypedDict(
+    "KinesisStreamConfigOutputTypeDef",
+    {
+        "StreamArn": str,
+    },
+)
+
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "StreamArn": str,
     },
 )
 
+KinesisVideoStreamConfigOutputTypeDef = TypedDict(
+    "KinesisVideoStreamConfigOutputTypeDef",
+    {
+        "Prefix": str,
+        "RetentionPeriodHours": int,
+        "EncryptionConfig": "EncryptionConfigOutputTypeDef",
+    },
+)
+
 KinesisVideoStreamConfigTypeDef = TypedDict(
     "KinesisVideoStreamConfigTypeDef",
     {
         "Prefix": str,
         "RetentionPeriodHours": int,
         "EncryptionConfig": "EncryptionConfigTypeDef",
     },
 )
 
-LexBotConfigTypeDef = TypedDict(
-    "LexBotConfigTypeDef",
+LexBotConfigOutputTypeDef = TypedDict(
+    "LexBotConfigOutputTypeDef",
     {
-        "LexBot": "LexBotTypeDef",
-        "LexV2Bot": "LexV2BotTypeDef",
+        "LexBot": "LexBotOutputTypeDef",
+        "LexV2Bot": "LexV2BotOutputTypeDef",
+    },
+)
+
+LexBotOutputTypeDef = TypedDict(
+    "LexBotOutputTypeDef",
+    {
+        "Name": str,
+        "LexRegion": str,
     },
 )
 
 LexBotTypeDef = TypedDict(
     "LexBotTypeDef",
     {
         "Name": str,
         "LexRegion": str,
     },
 )
 
+LexV2BotOutputTypeDef = TypedDict(
+    "LexV2BotOutputTypeDef",
+    {
+        "AliasArn": str,
+    },
+)
+
 LexV2BotTypeDef = TypedDict(
     "LexV2BotTypeDef",
     {
         "AliasArn": str,
     },
     total=False,
 )
@@ -3495,22 +3721,20 @@
     {
         "AgentStatusTypes": Sequence[AgentStatusTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListAgentStatusRequestListAgentStatusesPaginateTypeDef(
     _RequiredListAgentStatusRequestListAgentStatusesPaginateTypeDef,
     _OptionalListAgentStatusRequestListAgentStatusesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAgentStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListAgentStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListAgentStatusRequestRequestTypeDef = TypedDict(
@@ -3519,26 +3743,24 @@
         "NextToken": str,
         "MaxResults": int,
         "AgentStatusTypes": Sequence[AgentStatusTypeType],
     },
     total=False,
 )
 
-
 class ListAgentStatusRequestRequestTypeDef(
     _RequiredListAgentStatusRequestRequestTypeDef, _OptionalListAgentStatusRequestRequestTypeDef
 ):
     pass
 
-
-ListAgentStatusResponseTypeDef = TypedDict(
-    "ListAgentStatusResponseTypeDef",
+ListAgentStatusResponseOutputTypeDef = TypedDict(
+    "ListAgentStatusResponseOutputTypeDef",
     {
         "NextToken": str,
-        "AgentStatusSummaryList": List["AgentStatusSummaryTypeDef"],
+        "AgentStatusSummaryList": List["AgentStatusSummaryOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef = TypedDict(
     "_RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     {
@@ -3549,22 +3771,20 @@
     "_OptionalListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef(
     _RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
     _OptionalListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListApprovedOriginsRequestRequestTypeDef = TypedDict(
     "_RequiredListApprovedOriginsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListApprovedOriginsRequestRequestTypeDef = TypedDict(
@@ -3572,24 +3792,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListApprovedOriginsRequestRequestTypeDef(
     _RequiredListApprovedOriginsRequestRequestTypeDef,
     _OptionalListApprovedOriginsRequestRequestTypeDef,
 ):
     pass
 
-
-ListApprovedOriginsResponseTypeDef = TypedDict(
-    "ListApprovedOriginsResponseTypeDef",
+ListApprovedOriginsResponseOutputTypeDef = TypedDict(
+    "ListApprovedOriginsResponseOutputTypeDef",
     {
         "Origins": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -3604,21 +3822,19 @@
     "_OptionalListBotsRequestListBotsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListBotsRequestListBotsPaginateTypeDef(
     _RequiredListBotsRequestListBotsPaginateTypeDef, _OptionalListBotsRequestListBotsPaginateTypeDef
 ):
     pass
 
-
 _RequiredListBotsRequestRequestTypeDef = TypedDict(
     "_RequiredListBotsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LexVersion": LexVersionType,
     },
 )
@@ -3627,25 +3843,23 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListBotsRequestRequestTypeDef(
     _RequiredListBotsRequestRequestTypeDef, _OptionalListBotsRequestRequestTypeDef
 ):
     pass
 
-
-ListBotsResponseTypeDef = TypedDict(
-    "ListBotsResponseTypeDef",
+ListBotsResponseOutputTypeDef = TypedDict(
+    "ListBotsResponseOutputTypeDef",
     {
-        "LexBots": List["LexBotConfigTypeDef"],
+        "LexBots": List["LexBotConfigOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef = TypedDict(
     "_RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
@@ -3658,22 +3872,20 @@
     "_OptionalListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef(
     _RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
     _OptionalListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListContactEvaluationsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactEvaluationsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
@@ -3681,26 +3893,24 @@
     "_OptionalListContactEvaluationsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListContactEvaluationsRequestRequestTypeDef(
     _RequiredListContactEvaluationsRequestRequestTypeDef,
     _OptionalListContactEvaluationsRequestRequestTypeDef,
 ):
     pass
 
-
-ListContactEvaluationsResponseTypeDef = TypedDict(
-    "ListContactEvaluationsResponseTypeDef",
+ListContactEvaluationsResponseOutputTypeDef = TypedDict(
+    "ListContactEvaluationsResponseOutputTypeDef",
     {
-        "EvaluationSummaryList": List["EvaluationSummaryTypeDef"],
+        "EvaluationSummaryList": List["EvaluationSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
@@ -3713,22 +3923,20 @@
     {
         "ContactFlowModuleState": ContactFlowModuleStateType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef(
     _RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
     _OptionalListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListContactFlowModulesRequestRequestTypeDef = TypedDict(
     "_RequiredListContactFlowModulesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowModulesRequestRequestTypeDef = TypedDict(
@@ -3737,26 +3945,24 @@
         "NextToken": str,
         "MaxResults": int,
         "ContactFlowModuleState": ContactFlowModuleStateType,
     },
     total=False,
 )
 
-
 class ListContactFlowModulesRequestRequestTypeDef(
     _RequiredListContactFlowModulesRequestRequestTypeDef,
     _OptionalListContactFlowModulesRequestRequestTypeDef,
 ):
     pass
 
-
-ListContactFlowModulesResponseTypeDef = TypedDict(
-    "ListContactFlowModulesResponseTypeDef",
+ListContactFlowModulesResponseOutputTypeDef = TypedDict(
+    "ListContactFlowModulesResponseOutputTypeDef",
     {
-        "ContactFlowModulesSummaryList": List["ContactFlowModuleSummaryTypeDef"],
+        "ContactFlowModulesSummaryList": List["ContactFlowModuleSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef",
@@ -3769,22 +3975,20 @@
     {
         "ContactFlowTypes": Sequence[ContactFlowTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListContactFlowsRequestListContactFlowsPaginateTypeDef(
     _RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef,
     _OptionalListContactFlowsRequestListContactFlowsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListContactFlowsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactFlowsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowsRequestRequestTypeDef = TypedDict(
@@ -3793,25 +3997,23 @@
         "ContactFlowTypes": Sequence[ContactFlowTypeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListContactFlowsRequestRequestTypeDef(
     _RequiredListContactFlowsRequestRequestTypeDef, _OptionalListContactFlowsRequestRequestTypeDef
 ):
     pass
 
-
-ListContactFlowsResponseTypeDef = TypedDict(
-    "ListContactFlowsResponseTypeDef",
+ListContactFlowsResponseOutputTypeDef = TypedDict(
+    "ListContactFlowsResponseOutputTypeDef",
     {
-        "ContactFlowSummaryList": List["ContactFlowSummaryTypeDef"],
+        "ContactFlowSummaryList": List["ContactFlowSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef = TypedDict(
     "_RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef",
@@ -3825,22 +4027,20 @@
     "_OptionalListContactReferencesRequestListContactReferencesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListContactReferencesRequestListContactReferencesPaginateTypeDef(
     _RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef,
     _OptionalListContactReferencesRequestListContactReferencesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListContactReferencesRequestRequestTypeDef = TypedDict(
     "_RequiredListContactReferencesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ReferenceTypes": Sequence[ReferenceTypeType],
     },
@@ -3849,26 +4049,24 @@
     "_OptionalListContactReferencesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListContactReferencesRequestRequestTypeDef(
     _RequiredListContactReferencesRequestRequestTypeDef,
     _OptionalListContactReferencesRequestRequestTypeDef,
 ):
     pass
 
-
-ListContactReferencesResponseTypeDef = TypedDict(
-    "ListContactReferencesResponseTypeDef",
+ListContactReferencesResponseOutputTypeDef = TypedDict(
+    "ListContactReferencesResponseOutputTypeDef",
     {
-        "ReferenceSummaryList": List["ReferenceSummaryTypeDef"],
+        "ReferenceSummaryList": List["ReferenceSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef = TypedDict(
     "_RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef",
@@ -3881,22 +4079,20 @@
     {
         "LanguageCode": VocabularyLanguageCodeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef(
     _RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
     _OptionalListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDefaultVocabulariesRequestRequestTypeDef = TypedDict(
     "_RequiredListDefaultVocabulariesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListDefaultVocabulariesRequestRequestTypeDef = TypedDict(
@@ -3905,26 +4101,24 @@
         "LanguageCode": VocabularyLanguageCodeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDefaultVocabulariesRequestRequestTypeDef(
     _RequiredListDefaultVocabulariesRequestRequestTypeDef,
     _OptionalListDefaultVocabulariesRequestRequestTypeDef,
 ):
     pass
 
-
-ListDefaultVocabulariesResponseTypeDef = TypedDict(
-    "ListDefaultVocabulariesResponseTypeDef",
+ListDefaultVocabulariesResponseOutputTypeDef = TypedDict(
+    "ListDefaultVocabulariesResponseOutputTypeDef",
     {
-        "DefaultVocabularyList": List["DefaultVocabularyTypeDef"],
+        "DefaultVocabularyList": List["DefaultVocabularyOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
@@ -3937,22 +4131,20 @@
     "_OptionalListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef(
     _RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
     _OptionalListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListEvaluationFormVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListEvaluationFormVersionsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
     },
 )
@@ -3961,26 +4153,24 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListEvaluationFormVersionsRequestRequestTypeDef(
     _RequiredListEvaluationFormVersionsRequestRequestTypeDef,
     _OptionalListEvaluationFormVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListEvaluationFormVersionsResponseTypeDef = TypedDict(
-    "ListEvaluationFormVersionsResponseTypeDef",
+ListEvaluationFormVersionsResponseOutputTypeDef = TypedDict(
+    "ListEvaluationFormVersionsResponseOutputTypeDef",
     {
-        "EvaluationFormVersionSummaryList": List["EvaluationFormVersionSummaryTypeDef"],
+        "EvaluationFormVersionSummaryList": List["EvaluationFormVersionSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
@@ -3992,22 +4182,20 @@
     "_OptionalListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef(
     _RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
     _OptionalListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListEvaluationFormsRequestRequestTypeDef = TypedDict(
     "_RequiredListEvaluationFormsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListEvaluationFormsRequestRequestTypeDef = TypedDict(
@@ -4015,26 +4203,24 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListEvaluationFormsRequestRequestTypeDef(
     _RequiredListEvaluationFormsRequestRequestTypeDef,
     _OptionalListEvaluationFormsRequestRequestTypeDef,
 ):
     pass
 
-
-ListEvaluationFormsResponseTypeDef = TypedDict(
-    "ListEvaluationFormsResponseTypeDef",
+ListEvaluationFormsResponseOutputTypeDef = TypedDict(
+    "ListEvaluationFormsResponseOutputTypeDef",
     {
-        "EvaluationFormSummaryList": List["EvaluationFormSummaryTypeDef"],
+        "EvaluationFormSummaryList": List["EvaluationFormSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef = TypedDict(
     "_RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
@@ -4046,22 +4232,20 @@
     "_OptionalListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef(
     _RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
     _OptionalListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListHoursOfOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListHoursOfOperationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListHoursOfOperationsRequestRequestTypeDef = TypedDict(
@@ -4069,26 +4253,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListHoursOfOperationsRequestRequestTypeDef(
     _RequiredListHoursOfOperationsRequestRequestTypeDef,
     _OptionalListHoursOfOperationsRequestRequestTypeDef,
 ):
     pass
 
-
-ListHoursOfOperationsResponseTypeDef = TypedDict(
-    "ListHoursOfOperationsResponseTypeDef",
+ListHoursOfOperationsResponseOutputTypeDef = TypedDict(
+    "ListHoursOfOperationsResponseOutputTypeDef",
     {
-        "HoursOfOperationSummaryList": List["HoursOfOperationSummaryTypeDef"],
+        "HoursOfOperationSummaryList": List["HoursOfOperationSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef = TypedDict(
     "_RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
@@ -4100,22 +4282,20 @@
     "_OptionalListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef(
     _RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
     _OptionalListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInstanceAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListInstanceAttributesRequestRequestTypeDef = TypedDict(
@@ -4123,26 +4303,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListInstanceAttributesRequestRequestTypeDef(
     _RequiredListInstanceAttributesRequestRequestTypeDef,
     _OptionalListInstanceAttributesRequestRequestTypeDef,
 ):
     pass
 
-
-ListInstanceAttributesResponseTypeDef = TypedDict(
-    "ListInstanceAttributesResponseTypeDef",
+ListInstanceAttributesResponseOutputTypeDef = TypedDict(
+    "ListInstanceAttributesResponseOutputTypeDef",
     {
-        "Attributes": List["AttributeTypeDef"],
+        "Attributes": List["AttributeOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef = TypedDict(
     "_RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
@@ -4155,22 +4333,20 @@
     "_OptionalListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef(
     _RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
     _OptionalListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInstanceStorageConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceStorageConfigsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
 )
@@ -4179,26 +4355,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListInstanceStorageConfigsRequestRequestTypeDef(
     _RequiredListInstanceStorageConfigsRequestRequestTypeDef,
     _OptionalListInstanceStorageConfigsRequestRequestTypeDef,
 ):
     pass
 
-
-ListInstanceStorageConfigsResponseTypeDef = TypedDict(
-    "ListInstanceStorageConfigsResponseTypeDef",
+ListInstanceStorageConfigsResponseOutputTypeDef = TypedDict(
+    "ListInstanceStorageConfigsResponseOutputTypeDef",
     {
-        "StorageConfigs": List["InstanceStorageConfigTypeDef"],
+        "StorageConfigs": List["InstanceStorageConfigOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
     "ListInstancesRequestListInstancesPaginateTypeDef",
@@ -4213,18 +4387,18 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListInstancesResponseTypeDef = TypedDict(
-    "ListInstancesResponseTypeDef",
+ListInstancesResponseOutputTypeDef = TypedDict(
+    "ListInstancesResponseOutputTypeDef",
     {
-        "InstanceSummaryList": List["InstanceSummaryTypeDef"],
+        "InstanceSummaryList": List["InstanceSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef = TypedDict(
     "_RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef",
@@ -4237,22 +4411,20 @@
     {
         "IntegrationType": IntegrationTypeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef(
     _RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
     _OptionalListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListIntegrationAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListIntegrationAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListIntegrationAssociationsRequestRequestTypeDef = TypedDict(
@@ -4261,26 +4433,24 @@
         "IntegrationType": IntegrationTypeType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
-ListIntegrationAssociationsResponseTypeDef = TypedDict(
-    "ListIntegrationAssociationsResponseTypeDef",
+ListIntegrationAssociationsResponseOutputTypeDef = TypedDict(
+    "ListIntegrationAssociationsResponseOutputTypeDef",
     {
-        "IntegrationAssociationSummaryList": List["IntegrationAssociationSummaryTypeDef"],
+        "IntegrationAssociationSummaryList": List["IntegrationAssociationSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef = TypedDict(
     "_RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
@@ -4292,22 +4462,20 @@
     "_OptionalListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef(
     _RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
     _OptionalListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListLambdaFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLambdaFunctionsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLambdaFunctionsRequestRequestTypeDef = TypedDict(
@@ -4315,24 +4483,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListLambdaFunctionsRequestRequestTypeDef(
     _RequiredListLambdaFunctionsRequestRequestTypeDef,
     _OptionalListLambdaFunctionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListLambdaFunctionsResponseTypeDef = TypedDict(
-    "ListLambdaFunctionsResponseTypeDef",
+ListLambdaFunctionsResponseOutputTypeDef = TypedDict(
+    "ListLambdaFunctionsResponseOutputTypeDef",
     {
         "LambdaFunctions": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4346,22 +4512,20 @@
     "_OptionalListLexBotsRequestListLexBotsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListLexBotsRequestListLexBotsPaginateTypeDef(
     _RequiredListLexBotsRequestListLexBotsPaginateTypeDef,
     _OptionalListLexBotsRequestListLexBotsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListLexBotsRequestRequestTypeDef = TypedDict(
     "_RequiredListLexBotsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLexBotsRequestRequestTypeDef = TypedDict(
@@ -4369,25 +4533,23 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListLexBotsRequestRequestTypeDef(
     _RequiredListLexBotsRequestRequestTypeDef, _OptionalListLexBotsRequestRequestTypeDef
 ):
     pass
 
-
-ListLexBotsResponseTypeDef = TypedDict(
-    "ListLexBotsResponseTypeDef",
+ListLexBotsResponseOutputTypeDef = TypedDict(
+    "ListLexBotsResponseOutputTypeDef",
     {
-        "LexBots": List["LexBotTypeDef"],
+        "LexBots": List["LexBotOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef = TypedDict(
     "_RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef",
@@ -4401,22 +4563,20 @@
         "PhoneNumberTypes": Sequence[PhoneNumberTypeType],
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef(
     _RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
     _OptionalListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListPhoneNumbersRequestRequestTypeDef = TypedDict(
     "_RequiredListPhoneNumbersRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListPhoneNumbersRequestRequestTypeDef = TypedDict(
@@ -4426,32 +4586,30 @@
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListPhoneNumbersRequestRequestTypeDef(
     _RequiredListPhoneNumbersRequestRequestTypeDef, _OptionalListPhoneNumbersRequestRequestTypeDef
 ):
     pass
 
-
-ListPhoneNumbersResponseTypeDef = TypedDict(
-    "ListPhoneNumbersResponseTypeDef",
+ListPhoneNumbersResponseOutputTypeDef = TypedDict(
+    "ListPhoneNumbersResponseOutputTypeDef",
     {
-        "PhoneNumberSummaryList": List["PhoneNumberSummaryTypeDef"],
+        "PhoneNumberSummaryList": List["PhoneNumberSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPhoneNumbersSummaryTypeDef = TypedDict(
-    "ListPhoneNumbersSummaryTypeDef",
+ListPhoneNumbersSummaryOutputTypeDef = TypedDict(
+    "ListPhoneNumbersSummaryOutputTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "TargetArn": str,
@@ -4479,19 +4637,19 @@
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "PhoneNumberTypes": Sequence[PhoneNumberTypeType],
         "PhoneNumberPrefix": str,
     },
     total=False,
 )
 
-ListPhoneNumbersV2ResponseTypeDef = TypedDict(
-    "ListPhoneNumbersV2ResponseTypeDef",
+ListPhoneNumbersV2ResponseOutputTypeDef = TypedDict(
+    "ListPhoneNumbersV2ResponseOutputTypeDef",
     {
         "NextToken": str,
-        "ListPhoneNumbersSummaryList": List["ListPhoneNumbersSummaryTypeDef"],
+        "ListPhoneNumbersSummaryList": List["ListPhoneNumbersSummaryOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListPromptsRequestListPromptsPaginateTypeDef = TypedDict(
     "_RequiredListPromptsRequestListPromptsPaginateTypeDef",
     {
@@ -4502,22 +4660,20 @@
     "_OptionalListPromptsRequestListPromptsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListPromptsRequestListPromptsPaginateTypeDef(
     _RequiredListPromptsRequestListPromptsPaginateTypeDef,
     _OptionalListPromptsRequestListPromptsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListPromptsRequestRequestTypeDef = TypedDict(
     "_RequiredListPromptsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListPromptsRequestRequestTypeDef = TypedDict(
@@ -4525,25 +4681,23 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListPromptsRequestRequestTypeDef(
     _RequiredListPromptsRequestRequestTypeDef, _OptionalListPromptsRequestRequestTypeDef
 ):
     pass
 
-
-ListPromptsResponseTypeDef = TypedDict(
-    "ListPromptsResponseTypeDef",
+ListPromptsResponseOutputTypeDef = TypedDict(
+    "ListPromptsResponseOutputTypeDef",
     {
-        "PromptSummaryList": List["PromptSummaryTypeDef"],
+        "PromptSummaryList": List["PromptSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
@@ -4556,22 +4710,20 @@
     "_OptionalListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef(
     _RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
     _OptionalListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListQueueQuickConnectsRequestRequestTypeDef = TypedDict(
     "_RequiredListQueueQuickConnectsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
@@ -4580,27 +4732,25 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListQueueQuickConnectsRequestRequestTypeDef(
     _RequiredListQueueQuickConnectsRequestRequestTypeDef,
     _OptionalListQueueQuickConnectsRequestRequestTypeDef,
 ):
     pass
 
-
-ListQueueQuickConnectsResponseTypeDef = TypedDict(
-    "ListQueueQuickConnectsResponseTypeDef",
+ListQueueQuickConnectsResponseOutputTypeDef = TypedDict(
+    "ListQueueQuickConnectsResponseOutputTypeDef",
     {
         "NextToken": str,
-        "QuickConnectSummaryList": List["QuickConnectSummaryTypeDef"],
+        "QuickConnectSummaryList": List["QuickConnectSummaryOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
     "_RequiredListQueuesRequestListQueuesPaginateTypeDef",
     {
@@ -4612,22 +4762,20 @@
     {
         "QueueTypes": Sequence[QueueTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListQueuesRequestListQueuesPaginateTypeDef(
     _RequiredListQueuesRequestListQueuesPaginateTypeDef,
     _OptionalListQueuesRequestListQueuesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListQueuesRequestRequestTypeDef = TypedDict(
@@ -4636,25 +4784,23 @@
         "QueueTypes": Sequence[QueueTypeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListQueuesRequestRequestTypeDef(
     _RequiredListQueuesRequestRequestTypeDef, _OptionalListQueuesRequestRequestTypeDef
 ):
     pass
 
-
-ListQueuesResponseTypeDef = TypedDict(
-    "ListQueuesResponseTypeDef",
+ListQueuesResponseOutputTypeDef = TypedDict(
+    "ListQueuesResponseOutputTypeDef",
     {
-        "QueueSummaryList": List["QueueSummaryTypeDef"],
+        "QueueSummaryList": List["QueueSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef",
@@ -4667,22 +4813,20 @@
     {
         "QuickConnectTypes": Sequence[QuickConnectTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListQuickConnectsRequestListQuickConnectsPaginateTypeDef(
     _RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
     _OptionalListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListQuickConnectsRequestRequestTypeDef = TypedDict(
     "_RequiredListQuickConnectsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListQuickConnectsRequestRequestTypeDef = TypedDict(
@@ -4691,25 +4835,23 @@
         "NextToken": str,
         "MaxResults": int,
         "QuickConnectTypes": Sequence[QuickConnectTypeType],
     },
     total=False,
 )
 
-
 class ListQuickConnectsRequestRequestTypeDef(
     _RequiredListQuickConnectsRequestRequestTypeDef, _OptionalListQuickConnectsRequestRequestTypeDef
 ):
     pass
 
-
-ListQuickConnectsResponseTypeDef = TypedDict(
-    "ListQuickConnectsResponseTypeDef",
+ListQuickConnectsResponseOutputTypeDef = TypedDict(
+    "ListQuickConnectsResponseOutputTypeDef",
     {
-        "QuickConnectSummaryList": List["QuickConnectSummaryTypeDef"],
+        "QuickConnectSummaryList": List["QuickConnectSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
@@ -4722,22 +4864,20 @@
     "_OptionalListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef(
     _RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
     _OptionalListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRoutingProfileQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutingProfileQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
     },
 )
@@ -4746,27 +4886,27 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListRoutingProfileQueuesRequestRequestTypeDef(
     _RequiredListRoutingProfileQueuesRequestRequestTypeDef,
     _OptionalListRoutingProfileQueuesRequestRequestTypeDef,
 ):
     pass
 
-
-ListRoutingProfileQueuesResponseTypeDef = TypedDict(
-    "ListRoutingProfileQueuesResponseTypeDef",
+ListRoutingProfileQueuesResponseOutputTypeDef = TypedDict(
+    "ListRoutingProfileQueuesResponseOutputTypeDef",
     {
         "NextToken": str,
-        "RoutingProfileQueueConfigSummaryList": List["RoutingProfileQueueConfigSummaryTypeDef"],
+        "RoutingProfileQueueConfigSummaryList": List[
+            "RoutingProfileQueueConfigSummaryOutputTypeDef"
+        ],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     {
@@ -4777,22 +4917,20 @@
     "_OptionalListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef(
     _RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
     _OptionalListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRoutingProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutingProfilesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListRoutingProfilesRequestRequestTypeDef = TypedDict(
@@ -4800,26 +4938,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListRoutingProfilesRequestRequestTypeDef(
     _RequiredListRoutingProfilesRequestRequestTypeDef,
     _OptionalListRoutingProfilesRequestRequestTypeDef,
 ):
     pass
 
-
-ListRoutingProfilesResponseTypeDef = TypedDict(
-    "ListRoutingProfilesResponseTypeDef",
+ListRoutingProfilesResponseOutputTypeDef = TypedDict(
+    "ListRoutingProfilesResponseOutputTypeDef",
     {
-        "RoutingProfileSummaryList": List["RoutingProfileSummaryTypeDef"],
+        "RoutingProfileSummaryList": List["RoutingProfileSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
     "_RequiredListRulesRequestListRulesPaginateTypeDef",
@@ -4833,22 +4969,20 @@
         "PublishStatus": RulePublishStatusType,
         "EventSourceName": EventSourceNameType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListRulesRequestListRulesPaginateTypeDef(
     _RequiredListRulesRequestListRulesPaginateTypeDef,
     _OptionalListRulesRequestListRulesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListRulesRequestRequestTypeDef = TypedDict(
@@ -4858,25 +4992,23 @@
         "EventSourceName": EventSourceNameType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListRulesRequestRequestTypeDef(
     _RequiredListRulesRequestRequestTypeDef, _OptionalListRulesRequestRequestTypeDef
 ):
     pass
 
-
-ListRulesResponseTypeDef = TypedDict(
-    "ListRulesResponseTypeDef",
+ListRulesResponseOutputTypeDef = TypedDict(
+    "ListRulesResponseOutputTypeDef",
     {
-        "RuleSummaryList": List["RuleSummaryTypeDef"],
+        "RuleSummaryList": List["RuleSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef = TypedDict(
     "_RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
@@ -4888,22 +5020,20 @@
     "_OptionalListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListSecurityKeysRequestListSecurityKeysPaginateTypeDef(
     _RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
     _OptionalListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListSecurityKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityKeysRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityKeysRequestRequestTypeDef = TypedDict(
@@ -4911,25 +5041,23 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListSecurityKeysRequestRequestTypeDef(
     _RequiredListSecurityKeysRequestRequestTypeDef, _OptionalListSecurityKeysRequestRequestTypeDef
 ):
     pass
 
-
-ListSecurityKeysResponseTypeDef = TypedDict(
-    "ListSecurityKeysResponseTypeDef",
+ListSecurityKeysResponseOutputTypeDef = TypedDict(
+    "ListSecurityKeysResponseOutputTypeDef",
     {
-        "SecurityKeys": List["SecurityKeyTypeDef"],
+        "SecurityKeys": List["SecurityKeyOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef = TypedDict(
     "_RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
@@ -4942,22 +5070,20 @@
     "_OptionalListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef(
     _RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
     _OptionalListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListSecurityProfilePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityProfilePermissionsRequestRequestTypeDef",
     {
         "SecurityProfileId": str,
         "InstanceId": str,
     },
 )
@@ -4966,24 +5092,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListSecurityProfilePermissionsRequestRequestTypeDef(
     _RequiredListSecurityProfilePermissionsRequestRequestTypeDef,
     _OptionalListSecurityProfilePermissionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListSecurityProfilePermissionsResponseTypeDef = TypedDict(
-    "ListSecurityProfilePermissionsResponseTypeDef",
+ListSecurityProfilePermissionsResponseOutputTypeDef = TypedDict(
+    "ListSecurityProfilePermissionsResponseOutputTypeDef",
     {
         "Permissions": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4997,22 +5121,20 @@
     "_OptionalListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef(
     _RequiredListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     _OptionalListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListSecurityProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityProfilesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityProfilesRequestRequestTypeDef = TypedDict(
@@ -5020,40 +5142,38 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListSecurityProfilesRequestRequestTypeDef(
     _RequiredListSecurityProfilesRequestRequestTypeDef,
     _OptionalListSecurityProfilesRequestRequestTypeDef,
 ):
     pass
 
-
-ListSecurityProfilesResponseTypeDef = TypedDict(
-    "ListSecurityProfilesResponseTypeDef",
+ListSecurityProfilesResponseOutputTypeDef = TypedDict(
+    "ListSecurityProfilesResponseOutputTypeDef",
     {
-        "SecurityProfileSummaryList": List["SecurityProfileSummaryTypeDef"],
+        "SecurityProfileSummaryList": List["SecurityProfileSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef = TypedDict(
@@ -5068,22 +5188,20 @@
         "Status": TaskTemplateStatusType,
         "Name": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef(
     _RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
     _OptionalListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTaskTemplatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTaskTemplatesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListTaskTemplatesRequestRequestTypeDef = TypedDict(
@@ -5093,25 +5211,23 @@
         "MaxResults": int,
         "Status": TaskTemplateStatusType,
         "Name": str,
     },
     total=False,
 )
 
-
 class ListTaskTemplatesRequestRequestTypeDef(
     _RequiredListTaskTemplatesRequestRequestTypeDef, _OptionalListTaskTemplatesRequestRequestTypeDef
 ):
     pass
 
-
-ListTaskTemplatesResponseTypeDef = TypedDict(
-    "ListTaskTemplatesResponseTypeDef",
+ListTaskTemplatesResponseOutputTypeDef = TypedDict(
+    "ListTaskTemplatesResponseOutputTypeDef",
     {
-        "TaskTemplates": List["TaskTemplateMetadataTypeDef"],
+        "TaskTemplates": List["TaskTemplateMetadataOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef = TypedDict(
     "ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef",
@@ -5128,19 +5244,19 @@
         "MaxResults": int,
         "NextToken": str,
         "InstanceId": str,
     },
     total=False,
 )
 
-ListTrafficDistributionGroupsResponseTypeDef = TypedDict(
-    "ListTrafficDistributionGroupsResponseTypeDef",
+ListTrafficDistributionGroupsResponseOutputTypeDef = TypedDict(
+    "ListTrafficDistributionGroupsResponseOutputTypeDef",
     {
         "NextToken": str,
-        "TrafficDistributionGroupSummaryList": List["TrafficDistributionGroupSummaryTypeDef"],
+        "TrafficDistributionGroupSummaryList": List["TrafficDistributionGroupSummaryOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUseCasesRequestListUseCasesPaginateTypeDef = TypedDict(
     "_RequiredListUseCasesRequestListUseCasesPaginateTypeDef",
     {
@@ -5152,22 +5268,20 @@
     "_OptionalListUseCasesRequestListUseCasesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListUseCasesRequestListUseCasesPaginateTypeDef(
     _RequiredListUseCasesRequestListUseCasesPaginateTypeDef,
     _OptionalListUseCasesRequestListUseCasesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListUseCasesRequestRequestTypeDef = TypedDict(
     "_RequiredListUseCasesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IntegrationAssociationId": str,
     },
 )
@@ -5176,25 +5290,23 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListUseCasesRequestRequestTypeDef(
     _RequiredListUseCasesRequestRequestTypeDef, _OptionalListUseCasesRequestRequestTypeDef
 ):
     pass
 
-
-ListUseCasesResponseTypeDef = TypedDict(
-    "ListUseCasesResponseTypeDef",
+ListUseCasesResponseOutputTypeDef = TypedDict(
+    "ListUseCasesResponseOutputTypeDef",
     {
-        "UseCaseSummaryList": List["UseCaseTypeDef"],
+        "UseCaseSummaryList": List["UseCaseOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef = TypedDict(
     "_RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
@@ -5206,22 +5318,20 @@
     "_OptionalListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef(
     _RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
     _OptionalListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListUserHierarchyGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserHierarchyGroupsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListUserHierarchyGroupsRequestRequestTypeDef = TypedDict(
@@ -5229,26 +5339,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListUserHierarchyGroupsRequestRequestTypeDef(
     _RequiredListUserHierarchyGroupsRequestRequestTypeDef,
     _OptionalListUserHierarchyGroupsRequestRequestTypeDef,
 ):
     pass
 
-
-ListUserHierarchyGroupsResponseTypeDef = TypedDict(
-    "ListUserHierarchyGroupsResponseTypeDef",
+ListUserHierarchyGroupsResponseOutputTypeDef = TypedDict(
+    "ListUserHierarchyGroupsResponseOutputTypeDef",
     {
-        "UserHierarchyGroupSummaryList": List["HierarchyGroupSummaryTypeDef"],
+        "UserHierarchyGroupSummaryList": List["HierarchyGroupSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
@@ -5260,22 +5368,20 @@
     "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -5283,30 +5389,37 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-
-ListUsersResponseTypeDef = TypedDict(
-    "ListUsersResponseTypeDef",
+ListUsersResponseOutputTypeDef = TypedDict(
+    "ListUsersResponseOutputTypeDef",
     {
-        "UserSummaryList": List["UserSummaryTypeDef"],
+        "UserSummaryList": List["UserSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MediaConcurrencyOutputTypeDef = TypedDict(
+    "MediaConcurrencyOutputTypeDef",
+    {
+        "Channel": ChannelType,
+        "Concurrency": int,
+        "CrossChannelBehavior": "CrossChannelBehaviorOutputTypeDef",
+    },
+)
+
 _RequiredMediaConcurrencyTypeDef = TypedDict(
     "_RequiredMediaConcurrencyTypeDef",
     {
         "Channel": ChannelType,
         "Concurrency": int,
     },
 )
@@ -5314,41 +5427,56 @@
     "_OptionalMediaConcurrencyTypeDef",
     {
         "CrossChannelBehavior": "CrossChannelBehaviorTypeDef",
     },
     total=False,
 )
 
-
 class MediaConcurrencyTypeDef(_RequiredMediaConcurrencyTypeDef, _OptionalMediaConcurrencyTypeDef):
     pass
 
-
-MetricDataV2TypeDef = TypedDict(
-    "MetricDataV2TypeDef",
+MetricDataV2OutputTypeDef = TypedDict(
+    "MetricDataV2OutputTypeDef",
     {
-        "Metric": "MetricV2TypeDef",
+        "Metric": "MetricV2OutputTypeDef",
         "Value": float,
     },
 )
 
+MetricFilterV2OutputTypeDef = TypedDict(
+    "MetricFilterV2OutputTypeDef",
+    {
+        "MetricFilterKey": str,
+        "MetricFilterValues": List[str],
+    },
+)
+
 MetricFilterV2TypeDef = TypedDict(
     "MetricFilterV2TypeDef",
     {
         "MetricFilterKey": str,
         "MetricFilterValues": Sequence[str],
     },
     total=False,
 )
 
-MetricResultV2TypeDef = TypedDict(
-    "MetricResultV2TypeDef",
+MetricResultV2OutputTypeDef = TypedDict(
+    "MetricResultV2OutputTypeDef",
     {
         "Dimensions": Dict[str, str],
-        "Collections": List["MetricDataV2TypeDef"],
+        "Collections": List["MetricDataV2OutputTypeDef"],
+    },
+)
+
+MetricV2OutputTypeDef = TypedDict(
+    "MetricV2OutputTypeDef",
+    {
+        "Name": str,
+        "Threshold": List["ThresholdV2OutputTypeDef"],
+        "MetricFilters": List["MetricFilterV2OutputTypeDef"],
     },
 )
 
 MetricV2TypeDef = TypedDict(
     "MetricV2TypeDef",
     {
         "Name": str,
@@ -5371,54 +5499,76 @@
     {
         "AllowedMonitorCapabilities": Sequence[MonitorCapabilityType],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class MonitorContactRequestRequestTypeDef(
     _RequiredMonitorContactRequestRequestTypeDef, _OptionalMonitorContactRequestRequestTypeDef
 ):
     pass
 
-
-MonitorContactResponseTypeDef = TypedDict(
-    "MonitorContactResponseTypeDef",
+MonitorContactResponseOutputTypeDef = TypedDict(
+    "MonitorContactResponseOutputTypeDef",
     {
         "ContactId": str,
         "ContactArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+NotificationRecipientTypeOutputTypeDef = TypedDict(
+    "NotificationRecipientTypeOutputTypeDef",
+    {
+        "UserTags": Dict[str, str],
+        "UserIds": List[str],
+    },
+)
+
 NotificationRecipientTypeTypeDef = TypedDict(
     "NotificationRecipientTypeTypeDef",
     {
         "UserTags": Mapping[str, str],
         "UserIds": Sequence[str],
     },
     total=False,
 )
 
-NumberReferenceTypeDef = TypedDict(
-    "NumberReferenceTypeDef",
+NumberReferenceOutputTypeDef = TypedDict(
+    "NumberReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+NumericQuestionPropertyValueAutomationOutputTypeDef = TypedDict(
+    "NumericQuestionPropertyValueAutomationOutputTypeDef",
+    {
+        "Label": NumericQuestionPropertyAutomationLabelType,
+    },
+)
+
 NumericQuestionPropertyValueAutomationTypeDef = TypedDict(
     "NumericQuestionPropertyValueAutomationTypeDef",
     {
         "Label": NumericQuestionPropertyAutomationLabelType,
     },
 )
 
+OutboundCallerConfigOutputTypeDef = TypedDict(
+    "OutboundCallerConfigOutputTypeDef",
+    {
+        "OutboundCallerIdName": str,
+        "OutboundCallerIdNumberId": str,
+        "OutboundFlowId": str,
+    },
+)
+
 OutboundCallerConfigTypeDef = TypedDict(
     "OutboundCallerConfigTypeDef",
     {
         "OutboundCallerIdName": str,
         "OutboundCallerIdNumberId": str,
         "OutboundFlowId": str,
     },
@@ -5465,16 +5615,16 @@
     {
         "ParticipantTimerAction": Literal["Unset"],
         "ParticipantTimerDurationInMinutes": int,
     },
     total=False,
 )
 
-ParticipantTokenCredentialsTypeDef = TypedDict(
-    "ParticipantTokenCredentialsTypeDef",
+ParticipantTokenCredentialsOutputTypeDef = TypedDict(
+    "ParticipantTokenCredentialsOutputTypeDef",
     {
         "ParticipantToken": str,
         "Expiry": str,
     },
 )
 
 PersistentChatTypeDef = TypedDict(
@@ -5482,40 +5632,58 @@
     {
         "RehydrationType": RehydrationTypeType,
         "SourceContactId": str,
     },
     total=False,
 )
 
+PhoneNumberQuickConnectConfigOutputTypeDef = TypedDict(
+    "PhoneNumberQuickConnectConfigOutputTypeDef",
+    {
+        "PhoneNumber": str,
+    },
+)
+
 PhoneNumberQuickConnectConfigTypeDef = TypedDict(
     "PhoneNumberQuickConnectConfigTypeDef",
     {
         "PhoneNumber": str,
     },
 )
 
-PhoneNumberStatusTypeDef = TypedDict(
-    "PhoneNumberStatusTypeDef",
+PhoneNumberStatusOutputTypeDef = TypedDict(
+    "PhoneNumberStatusOutputTypeDef",
     {
         "Status": PhoneNumberWorkflowStatusType,
         "Message": str,
     },
 )
 
-PhoneNumberSummaryTypeDef = TypedDict(
-    "PhoneNumberSummaryTypeDef",
+PhoneNumberSummaryOutputTypeDef = TypedDict(
+    "PhoneNumberSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PhoneNumber": str,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
     },
 )
 
+PromptOutputTypeDef = TypedDict(
+    "PromptOutputTypeDef",
+    {
+        "PromptARN": str,
+        "PromptId": str,
+        "Name": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+    },
+)
+
 PromptSearchCriteriaTypeDef = TypedDict(
     "PromptSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
@@ -5526,61 +5694,73 @@
     "PromptSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-PromptSummaryTypeDef = TypedDict(
-    "PromptSummaryTypeDef",
+PromptSummaryOutputTypeDef = TypedDict(
+    "PromptSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
-PromptTypeDef = TypedDict(
-    "PromptTypeDef",
-    {
-        "PromptARN": str,
-        "PromptId": str,
-        "Name": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-    },
-)
-
 PutUserStatusRequestRequestTypeDef = TypedDict(
     "PutUserStatusRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
         "AgentStatusId": str,
     },
 )
 
-QueueInfoTypeDef = TypedDict(
-    "QueueInfoTypeDef",
+QueueInfoOutputTypeDef = TypedDict(
+    "QueueInfoOutputTypeDef",
     {
         "Id": str,
         "EnqueueTimestamp": datetime,
     },
 )
 
+QueueOutputTypeDef = TypedDict(
+    "QueueOutputTypeDef",
+    {
+        "Name": str,
+        "QueueArn": str,
+        "QueueId": str,
+        "Description": str,
+        "OutboundCallerConfig": "OutboundCallerConfigOutputTypeDef",
+        "HoursOfOperationId": str,
+        "MaxContacts": int,
+        "Status": QueueStatusType,
+        "Tags": Dict[str, str],
+    },
+)
+
+QueueQuickConnectConfigOutputTypeDef = TypedDict(
+    "QueueQuickConnectConfigOutputTypeDef",
+    {
+        "QueueId": str,
+        "ContactFlowId": str,
+    },
+)
+
 QueueQuickConnectConfigTypeDef = TypedDict(
     "QueueQuickConnectConfigTypeDef",
     {
         "QueueId": str,
         "ContactFlowId": str,
     },
 )
 
-QueueReferenceTypeDef = TypedDict(
-    "QueueReferenceTypeDef",
+QueueReferenceOutputTypeDef = TypedDict(
+    "QueueReferenceOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 QueueSearchCriteriaTypeDef = TypedDict(
@@ -5598,36 +5778,31 @@
     "QueueSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-QueueSummaryTypeDef = TypedDict(
-    "QueueSummaryTypeDef",
+QueueSummaryOutputTypeDef = TypedDict(
+    "QueueSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QueueType": QueueTypeType,
     },
 )
 
-QueueTypeDef = TypedDict(
-    "QueueTypeDef",
+QuickConnectConfigOutputTypeDef = TypedDict(
+    "QuickConnectConfigOutputTypeDef",
     {
-        "Name": str,
-        "QueueArn": str,
-        "QueueId": str,
-        "Description": str,
-        "OutboundCallerConfig": "OutboundCallerConfigTypeDef",
-        "HoursOfOperationId": str,
-        "MaxContacts": int,
-        "Status": QueueStatusType,
-        "Tags": Dict[str, str],
+        "QuickConnectType": QuickConnectTypeType,
+        "UserConfig": "UserQuickConnectConfigOutputTypeDef",
+        "QueueConfig": "QueueQuickConnectConfigOutputTypeDef",
+        "PhoneConfig": "PhoneNumberQuickConnectConfigOutputTypeDef",
     },
 )
 
 _RequiredQuickConnectConfigTypeDef = TypedDict(
     "_RequiredQuickConnectConfigTypeDef",
     {
         "QuickConnectType": QuickConnectTypeType,
@@ -5639,20 +5814,30 @@
         "UserConfig": "UserQuickConnectConfigTypeDef",
         "QueueConfig": "QueueQuickConnectConfigTypeDef",
         "PhoneConfig": "PhoneNumberQuickConnectConfigTypeDef",
     },
     total=False,
 )
 
-
 class QuickConnectConfigTypeDef(
     _RequiredQuickConnectConfigTypeDef, _OptionalQuickConnectConfigTypeDef
 ):
     pass
 
+QuickConnectOutputTypeDef = TypedDict(
+    "QuickConnectOutputTypeDef",
+    {
+        "QuickConnectARN": str,
+        "QuickConnectId": str,
+        "Name": str,
+        "Description": str,
+        "QuickConnectConfig": "QuickConnectConfigOutputTypeDef",
+        "Tags": Dict[str, str],
+    },
+)
 
 QuickConnectSearchCriteriaTypeDef = TypedDict(
     "QuickConnectSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
@@ -5664,53 +5849,56 @@
     "QuickConnectSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-QuickConnectSummaryTypeDef = TypedDict(
-    "QuickConnectSummaryTypeDef",
+QuickConnectSummaryOutputTypeDef = TypedDict(
+    "QuickConnectSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QuickConnectType": QuickConnectTypeType,
     },
 )
 
-QuickConnectTypeDef = TypedDict(
-    "QuickConnectTypeDef",
+ReadOnlyFieldInfoOutputTypeDef = TypedDict(
+    "ReadOnlyFieldInfoOutputTypeDef",
     {
-        "QuickConnectARN": str,
-        "QuickConnectId": str,
-        "Name": str,
-        "Description": str,
-        "QuickConnectConfig": "QuickConnectConfigTypeDef",
-        "Tags": Dict[str, str],
+        "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
     },
 )
 
 ReadOnlyFieldInfoTypeDef = TypedDict(
     "ReadOnlyFieldInfoTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
     total=False,
 )
 
-ReferenceSummaryTypeDef = TypedDict(
-    "ReferenceSummaryTypeDef",
+ReferenceOutputTypeDef = TypedDict(
+    "ReferenceOutputTypeDef",
+    {
+        "Value": str,
+        "Type": ReferenceTypeType,
+    },
+)
+
+ReferenceSummaryOutputTypeDef = TypedDict(
+    "ReferenceSummaryOutputTypeDef",
     {
-        "Url": "UrlReferenceTypeDef",
-        "Attachment": "AttachmentReferenceTypeDef",
-        "String": "StringReferenceTypeDef",
-        "Number": "NumberReferenceTypeDef",
-        "Date": "DateReferenceTypeDef",
-        "Email": "EmailReferenceTypeDef",
+        "Url": "UrlReferenceOutputTypeDef",
+        "Attachment": "AttachmentReferenceOutputTypeDef",
+        "String": "StringReferenceOutputTypeDef",
+        "Number": "NumberReferenceOutputTypeDef",
+        "Date": "DateReferenceOutputTypeDef",
+        "Email": "EmailReferenceOutputTypeDef",
     },
 )
 
 ReferenceTypeDef = TypedDict(
     "ReferenceTypeDef",
     {
         "Value": str,
@@ -5728,22 +5916,20 @@
     "_OptionalReleasePhoneNumberRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class ReleasePhoneNumberRequestRequestTypeDef(
     _RequiredReleasePhoneNumberRequestRequestTypeDef,
     _OptionalReleasePhoneNumberRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredReplicateInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ReplicaRegion": str,
         "ReplicaAlias": str,
     },
@@ -5752,30 +5938,35 @@
     "_OptionalReplicateInstanceRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class ReplicateInstanceRequestRequestTypeDef(
     _RequiredReplicateInstanceRequestRequestTypeDef, _OptionalReplicateInstanceRequestRequestTypeDef
 ):
     pass
 
-
-ReplicateInstanceResponseTypeDef = TypedDict(
-    "ReplicateInstanceResponseTypeDef",
+ReplicateInstanceResponseOutputTypeDef = TypedDict(
+    "ReplicateInstanceResponseOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RequiredFieldInfoOutputTypeDef = TypedDict(
+    "RequiredFieldInfoOutputTypeDef",
+    {
+        "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
+    },
+)
+
 RequiredFieldInfoTypeDef = TypedDict(
     "RequiredFieldInfoTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
     total=False,
 )
@@ -5804,16 +5995,32 @@
     {
         "InstanceId": str,
         "ContactId": str,
         "InitialContactId": str,
     },
 )
 
-RoutingProfileQueueConfigSummaryTypeDef = TypedDict(
-    "RoutingProfileQueueConfigSummaryTypeDef",
+RoutingProfileOutputTypeDef = TypedDict(
+    "RoutingProfileOutputTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "RoutingProfileArn": str,
+        "RoutingProfileId": str,
+        "Description": str,
+        "MediaConcurrencies": List["MediaConcurrencyOutputTypeDef"],
+        "DefaultOutboundQueueId": str,
+        "Tags": Dict[str, str],
+        "NumberOfAssociatedQueues": int,
+        "NumberOfAssociatedUsers": int,
+    },
+)
+
+RoutingProfileQueueConfigSummaryOutputTypeDef = TypedDict(
+    "RoutingProfileQueueConfigSummaryOutputTypeDef",
     {
         "QueueId": str,
         "QueueArn": str,
         "QueueName": str,
         "Priority": int,
         "Delay": int,
         "Channel": ChannelType,
@@ -5833,16 +6040,16 @@
     "RoutingProfileQueueReferenceTypeDef",
     {
         "QueueId": str,
         "Channel": ChannelType,
     },
 )
 
-RoutingProfileReferenceTypeDef = TypedDict(
-    "RoutingProfileReferenceTypeDef",
+RoutingProfileReferenceOutputTypeDef = TypedDict(
+    "RoutingProfileReferenceOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 RoutingProfileSearchCriteriaTypeDef = TypedDict(
@@ -5859,36 +6066,31 @@
     "RoutingProfileSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-RoutingProfileSummaryTypeDef = TypedDict(
-    "RoutingProfileSummaryTypeDef",
+RoutingProfileSummaryOutputTypeDef = TypedDict(
+    "RoutingProfileSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
-RoutingProfileTypeDef = TypedDict(
-    "RoutingProfileTypeDef",
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
     {
-        "InstanceId": str,
-        "Name": str,
-        "RoutingProfileArn": str,
-        "RoutingProfileId": str,
-        "Description": str,
-        "MediaConcurrencies": List["MediaConcurrencyTypeDef"],
-        "DefaultOutboundQueueId": str,
-        "Tags": Dict[str, str],
-        "NumberOfAssociatedQueues": int,
-        "NumberOfAssociatedUsers": int,
+        "ActionType": ActionTypeType,
+        "TaskAction": "TaskActionDefinitionOutputTypeDef",
+        "EventBridgeAction": "EventBridgeActionDefinitionOutputTypeDef",
+        "AssignContactCategoryAction": Dict[str, Any],
+        "SendNotificationAction": "SendNotificationActionDefinitionOutputTypeDef",
     },
 )
 
 _RequiredRuleActionTypeDef = TypedDict(
     "_RequiredRuleActionTypeDef",
     {
         "ActionType": ActionTypeType,
@@ -5901,68 +6103,81 @@
         "EventBridgeAction": "EventBridgeActionDefinitionTypeDef",
         "AssignContactCategoryAction": Mapping[str, Any],
         "SendNotificationAction": "SendNotificationActionDefinitionTypeDef",
     },
     total=False,
 )
 
-
 class RuleActionTypeDef(_RequiredRuleActionTypeDef, _OptionalRuleActionTypeDef):
     pass
 
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "Name": str,
+        "RuleId": str,
+        "RuleArn": str,
+        "TriggerEventSource": "RuleTriggerEventSourceOutputTypeDef",
+        "Function": str,
+        "Actions": List["RuleActionOutputTypeDef"],
+        "PublishStatus": RulePublishStatusType,
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "LastUpdatedBy": str,
+        "Tags": Dict[str, str],
+    },
+)
 
-RuleSummaryTypeDef = TypedDict(
-    "RuleSummaryTypeDef",
+RuleSummaryOutputTypeDef = TypedDict(
+    "RuleSummaryOutputTypeDef",
     {
         "Name": str,
         "RuleId": str,
         "RuleArn": str,
         "EventSourceName": EventSourceNameType,
         "PublishStatus": RulePublishStatusType,
-        "ActionSummaries": List["ActionSummaryTypeDef"],
+        "ActionSummaries": List["ActionSummaryOutputTypeDef"],
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
     },
 )
 
+RuleTriggerEventSourceOutputTypeDef = TypedDict(
+    "RuleTriggerEventSourceOutputTypeDef",
+    {
+        "EventSourceName": EventSourceNameType,
+        "IntegrationAssociationId": str,
+    },
+)
+
 _RequiredRuleTriggerEventSourceTypeDef = TypedDict(
     "_RequiredRuleTriggerEventSourceTypeDef",
     {
         "EventSourceName": EventSourceNameType,
     },
 )
 _OptionalRuleTriggerEventSourceTypeDef = TypedDict(
     "_OptionalRuleTriggerEventSourceTypeDef",
     {
         "IntegrationAssociationId": str,
     },
     total=False,
 )
 
-
 class RuleTriggerEventSourceTypeDef(
     _RequiredRuleTriggerEventSourceTypeDef, _OptionalRuleTriggerEventSourceTypeDef
 ):
     pass
 
-
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
+S3ConfigOutputTypeDef = TypedDict(
+    "S3ConfigOutputTypeDef",
     {
-        "Name": str,
-        "RuleId": str,
-        "RuleArn": str,
-        "TriggerEventSource": "RuleTriggerEventSourceTypeDef",
-        "Function": str,
-        "Actions": List["RuleActionTypeDef"],
-        "PublishStatus": RulePublishStatusType,
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "LastUpdatedBy": str,
-        "Tags": Dict[str, str],
+        "BucketName": str,
+        "BucketPrefix": str,
+        "EncryptionConfig": "EncryptionConfigOutputTypeDef",
     },
 )
 
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "BucketName": str,
@@ -5973,19 +6188,17 @@
     "_OptionalS3ConfigTypeDef",
     {
         "EncryptionConfig": "EncryptionConfigTypeDef",
     },
     total=False,
 )
 
-
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
-
 _RequiredSearchAvailablePhoneNumbersRequestRequestTypeDef = TypedDict(
     "_RequiredSearchAvailablePhoneNumbersRequestRequestTypeDef",
     {
         "TargetArn": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
@@ -5996,22 +6209,20 @@
         "PhoneNumberPrefix": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SearchAvailablePhoneNumbersRequestRequestTypeDef(
     _RequiredSearchAvailablePhoneNumbersRequestRequestTypeDef,
     _OptionalSearchAvailablePhoneNumbersRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef = TypedDict(
     "_RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef",
     {
         "TargetArn": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
@@ -6021,27 +6232,25 @@
     {
         "PhoneNumberPrefix": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef(
     _RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
     _OptionalSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
 ):
     pass
 
-
-SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseTypeDef",
+SearchAvailablePhoneNumbersResponseOutputTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseOutputTypeDef",
     {
         "NextToken": str,
-        "AvailableNumbersList": List["AvailableNumberSummaryTypeDef"],
+        "AvailableNumbersList": List["AvailableNumberSummaryOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchHoursOfOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchHoursOfOperationsRequestRequestTypeDef",
     {
@@ -6055,22 +6264,20 @@
         "MaxResults": int,
         "SearchFilter": "HoursOfOperationSearchFilterTypeDef",
         "SearchCriteria": "HoursOfOperationSearchCriteriaTypeDef",
     },
     total=False,
 )
 
-
 class SearchHoursOfOperationsRequestRequestTypeDef(
     _RequiredSearchHoursOfOperationsRequestRequestTypeDef,
     _OptionalSearchHoursOfOperationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef = TypedDict(
     "_RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef = TypedDict(
@@ -6079,26 +6286,24 @@
         "SearchFilter": "HoursOfOperationSearchFilterTypeDef",
         "SearchCriteria": "HoursOfOperationSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef(
     _RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
     _OptionalSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
 ):
     pass
 
-
-SearchHoursOfOperationsResponseTypeDef = TypedDict(
-    "SearchHoursOfOperationsResponseTypeDef",
+SearchHoursOfOperationsResponseOutputTypeDef = TypedDict(
+    "SearchHoursOfOperationsResponseOutputTypeDef",
     {
-        "HoursOfOperations": List["HoursOfOperationTypeDef"],
+        "HoursOfOperations": List["HoursOfOperationOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchPromptsRequestRequestTypeDef = TypedDict(
@@ -6114,21 +6319,19 @@
         "MaxResults": int,
         "SearchFilter": "PromptSearchFilterTypeDef",
         "SearchCriteria": "PromptSearchCriteriaTypeDef",
     },
     total=False,
 )
 
-
 class SearchPromptsRequestRequestTypeDef(
     _RequiredSearchPromptsRequestRequestTypeDef, _OptionalSearchPromptsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef = TypedDict(
     "_RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchPromptsRequestSearchPromptsPaginateTypeDef = TypedDict(
@@ -6137,26 +6340,24 @@
         "SearchFilter": "PromptSearchFilterTypeDef",
         "SearchCriteria": "PromptSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchPromptsRequestSearchPromptsPaginateTypeDef(
     _RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef,
     _OptionalSearchPromptsRequestSearchPromptsPaginateTypeDef,
 ):
     pass
 
-
-SearchPromptsResponseTypeDef = TypedDict(
-    "SearchPromptsResponseTypeDef",
+SearchPromptsResponseOutputTypeDef = TypedDict(
+    "SearchPromptsResponseOutputTypeDef",
     {
-        "Prompts": List["PromptTypeDef"],
+        "Prompts": List["PromptOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchQueuesRequestRequestTypeDef = TypedDict(
@@ -6172,21 +6373,19 @@
         "MaxResults": int,
         "SearchFilter": "QueueSearchFilterTypeDef",
         "SearchCriteria": "QueueSearchCriteriaTypeDef",
     },
     total=False,
 )
 
-
 class SearchQueuesRequestRequestTypeDef(
     _RequiredSearchQueuesRequestRequestTypeDef, _OptionalSearchQueuesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef = TypedDict(
     "_RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQueuesRequestSearchQueuesPaginateTypeDef = TypedDict(
@@ -6195,26 +6394,24 @@
         "SearchFilter": "QueueSearchFilterTypeDef",
         "SearchCriteria": "QueueSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchQueuesRequestSearchQueuesPaginateTypeDef(
     _RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef,
     _OptionalSearchQueuesRequestSearchQueuesPaginateTypeDef,
 ):
     pass
 
-
-SearchQueuesResponseTypeDef = TypedDict(
-    "SearchQueuesResponseTypeDef",
+SearchQueuesResponseOutputTypeDef = TypedDict(
+    "SearchQueuesResponseOutputTypeDef",
     {
-        "Queues": List["QueueTypeDef"],
+        "Queues": List["QueueOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchQuickConnectsRequestRequestTypeDef = TypedDict(
@@ -6230,22 +6427,20 @@
         "MaxResults": int,
         "SearchFilter": "QuickConnectSearchFilterTypeDef",
         "SearchCriteria": "QuickConnectSearchCriteriaTypeDef",
     },
     total=False,
 )
 
-
 class SearchQuickConnectsRequestRequestTypeDef(
     _RequiredSearchQuickConnectsRequestRequestTypeDef,
     _OptionalSearchQuickConnectsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef = TypedDict(
@@ -6254,26 +6449,24 @@
         "SearchFilter": "QuickConnectSearchFilterTypeDef",
         "SearchCriteria": "QuickConnectSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef(
     _RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
     _OptionalSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
 ):
     pass
 
-
-SearchQuickConnectsResponseTypeDef = TypedDict(
-    "SearchQuickConnectsResponseTypeDef",
+SearchQuickConnectsResponseOutputTypeDef = TypedDict(
+    "SearchQuickConnectsResponseOutputTypeDef",
     {
-        "QuickConnects": List["QuickConnectTypeDef"],
+        "QuickConnects": List["QuickConnectOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchResourceTagsRequestRequestTypeDef = TypedDict(
@@ -6289,22 +6482,20 @@
         "NextToken": str,
         "MaxResults": int,
         "SearchCriteria": "ResourceTagsSearchCriteriaTypeDef",
     },
     total=False,
 )
 
-
 class SearchResourceTagsRequestRequestTypeDef(
     _RequiredSearchResourceTagsRequestRequestTypeDef,
     _OptionalSearchResourceTagsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef = TypedDict(
     "_RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef = TypedDict(
@@ -6313,26 +6504,24 @@
         "ResourceTypes": Sequence[str],
         "SearchCriteria": "ResourceTagsSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef(
     _RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
     _OptionalSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
 ):
     pass
 
-
-SearchResourceTagsResponseTypeDef = TypedDict(
-    "SearchResourceTagsResponseTypeDef",
+SearchResourceTagsResponseOutputTypeDef = TypedDict(
+    "SearchResourceTagsResponseOutputTypeDef",
     {
-        "Tags": List["TagSetTypeDef"],
+        "Tags": List["TagSetOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchRoutingProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRoutingProfilesRequestRequestTypeDef",
@@ -6347,22 +6536,20 @@
         "MaxResults": int,
         "SearchFilter": "RoutingProfileSearchFilterTypeDef",
         "SearchCriteria": "RoutingProfileSearchCriteriaTypeDef",
     },
     total=False,
 )
 
-
 class SearchRoutingProfilesRequestRequestTypeDef(
     _RequiredSearchRoutingProfilesRequestRequestTypeDef,
     _OptionalSearchRoutingProfilesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef = TypedDict(
     "_RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef = TypedDict(
@@ -6371,26 +6558,24 @@
         "SearchFilter": "RoutingProfileSearchFilterTypeDef",
         "SearchCriteria": "RoutingProfileSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef(
     _RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
     _OptionalSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
 ):
     pass
 
-
-SearchRoutingProfilesResponseTypeDef = TypedDict(
-    "SearchRoutingProfilesResponseTypeDef",
+SearchRoutingProfilesResponseOutputTypeDef = TypedDict(
+    "SearchRoutingProfilesResponseOutputTypeDef",
     {
-        "RoutingProfiles": List["RoutingProfileTypeDef"],
+        "RoutingProfiles": List["RoutingProfileOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchSecurityProfilesRequestRequestTypeDef = TypedDict(
@@ -6406,22 +6591,20 @@
         "MaxResults": int,
         "SearchCriteria": "SecurityProfileSearchCriteriaTypeDef",
         "SearchFilter": "SecurityProfilesSearchFilterTypeDef",
     },
     total=False,
 )
 
-
 class SearchSecurityProfilesRequestRequestTypeDef(
     _RequiredSearchSecurityProfilesRequestRequestTypeDef,
     _OptionalSearchSecurityProfilesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef = TypedDict(
     "_RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef = TypedDict(
@@ -6430,26 +6613,24 @@
         "SearchCriteria": "SecurityProfileSearchCriteriaTypeDef",
         "SearchFilter": "SecurityProfilesSearchFilterTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef(
     _RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
     _OptionalSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
 ):
     pass
 
-
-SearchSecurityProfilesResponseTypeDef = TypedDict(
-    "SearchSecurityProfilesResponseTypeDef",
+SearchSecurityProfilesResponseOutputTypeDef = TypedDict(
+    "SearchSecurityProfilesResponseOutputTypeDef",
     {
-        "SecurityProfiles": List["SecurityProfileSearchSummaryTypeDef"],
+        "SecurityProfiles": List["SecurityProfileSearchSummaryOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchUsersRequestRequestTypeDef = TypedDict(
@@ -6471,18 +6652,18 @@
         "SearchFilter": "UserSearchFilterTypeDef",
         "SearchCriteria": "UserSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-SearchUsersResponseTypeDef = TypedDict(
-    "SearchUsersResponseTypeDef",
+SearchUsersResponseOutputTypeDef = TypedDict(
+    "SearchUsersResponseOutputTypeDef",
     {
-        "Users": List["UserSearchSummaryTypeDef"],
+        "Users": List["UserSearchSummaryOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchVocabulariesRequestRequestTypeDef = TypedDict(
@@ -6499,22 +6680,20 @@
         "State": VocabularyStateType,
         "NameStartsWith": str,
         "LanguageCode": VocabularyLanguageCodeType,
     },
     total=False,
 )
 
-
 class SearchVocabulariesRequestRequestTypeDef(
     _RequiredSearchVocabulariesRequestRequestTypeDef,
     _OptionalSearchVocabulariesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef = TypedDict(
     "_RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef = TypedDict(
@@ -6524,93 +6703,102 @@
         "NameStartsWith": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef(
     _RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
     _OptionalSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
 ):
     pass
 
-
-SearchVocabulariesResponseTypeDef = TypedDict(
-    "SearchVocabulariesResponseTypeDef",
+SearchVocabulariesResponseOutputTypeDef = TypedDict(
+    "SearchVocabulariesResponseOutputTypeDef",
     {
-        "VocabularySummaryList": List["VocabularySummaryTypeDef"],
+        "VocabularySummaryList": List["VocabularySummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SecurityKeyTypeDef = TypedDict(
-    "SecurityKeyTypeDef",
+SecurityKeyOutputTypeDef = TypedDict(
+    "SecurityKeyOutputTypeDef",
     {
         "AssociationId": str,
         "Key": str,
         "CreationTime": datetime,
     },
 )
 
+SecurityProfileOutputTypeDef = TypedDict(
+    "SecurityProfileOutputTypeDef",
+    {
+        "Id": str,
+        "OrganizationResourceId": str,
+        "Arn": str,
+        "SecurityProfileName": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "AllowedAccessControlTags": Dict[str, str],
+        "TagRestrictedResources": List[str],
+    },
+)
+
 SecurityProfileSearchCriteriaTypeDef = TypedDict(
     "SecurityProfileSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
     total=False,
 )
 
-SecurityProfileSearchSummaryTypeDef = TypedDict(
-    "SecurityProfileSearchSummaryTypeDef",
+SecurityProfileSearchSummaryOutputTypeDef = TypedDict(
+    "SecurityProfileSearchSummaryOutputTypeDef",
     {
         "Id": str,
         "OrganizationResourceId": str,
         "Arn": str,
         "SecurityProfileName": str,
         "Description": str,
         "Tags": Dict[str, str],
     },
 )
 
-SecurityProfileSummaryTypeDef = TypedDict(
-    "SecurityProfileSummaryTypeDef",
+SecurityProfileSummaryOutputTypeDef = TypedDict(
+    "SecurityProfileSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
-SecurityProfileTypeDef = TypedDict(
-    "SecurityProfileTypeDef",
-    {
-        "Id": str,
-        "OrganizationResourceId": str,
-        "Arn": str,
-        "SecurityProfileName": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "AllowedAccessControlTags": Dict[str, str],
-        "TagRestrictedResources": List[str],
-    },
-)
-
 SecurityProfilesSearchFilterTypeDef = TypedDict(
     "SecurityProfilesSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
+SendNotificationActionDefinitionOutputTypeDef = TypedDict(
+    "SendNotificationActionDefinitionOutputTypeDef",
+    {
+        "DeliveryMethod": Literal["EMAIL"],
+        "Subject": str,
+        "Content": str,
+        "ContentType": Literal["PLAIN_TEXT"],
+        "Recipient": "NotificationRecipientTypeOutputTypeDef",
+    },
+)
+
 _RequiredSendNotificationActionDefinitionTypeDef = TypedDict(
     "_RequiredSendNotificationActionDefinitionTypeDef",
     {
         "DeliveryMethod": Literal["EMAIL"],
         "Content": str,
         "ContentType": Literal["PLAIN_TEXT"],
         "Recipient": "NotificationRecipientTypeTypeDef",
@@ -6620,21 +6808,28 @@
     "_OptionalSendNotificationActionDefinitionTypeDef",
     {
         "Subject": str,
     },
     total=False,
 )
 
-
 class SendNotificationActionDefinitionTypeDef(
     _RequiredSendNotificationActionDefinitionTypeDef,
     _OptionalSendNotificationActionDefinitionTypeDef,
 ):
     pass
 
+SingleSelectQuestionRuleCategoryAutomationOutputTypeDef = TypedDict(
+    "SingleSelectQuestionRuleCategoryAutomationOutputTypeDef",
+    {
+        "Category": str,
+        "Condition": SingleSelectQuestionRuleCategoryAutomationConditionType,
+        "OptionRefId": str,
+    },
+)
 
 SingleSelectQuestionRuleCategoryAutomationTypeDef = TypedDict(
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     {
         "Category": str,
         "Condition": SingleSelectQuestionRuleCategoryAutomationConditionType,
         "OptionRefId": str,
@@ -6659,23 +6854,21 @@
         "SupportedMessagingContentTypes": Sequence[str],
         "PersistentChat": "PersistentChatTypeDef",
         "RelatedContactId": str,
     },
     total=False,
 )
 
-
 class StartChatContactRequestRequestTypeDef(
     _RequiredStartChatContactRequestRequestTypeDef, _OptionalStartChatContactRequestRequestTypeDef
 ):
     pass
 
-
-StartChatContactResponseTypeDef = TypedDict(
-    "StartChatContactResponseTypeDef",
+StartChatContactResponseOutputTypeDef = TypedDict(
+    "StartChatContactResponseOutputTypeDef",
     {
         "ContactId": str,
         "ParticipantId": str,
         "ParticipantToken": str,
         "ContinuedFromContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -6693,24 +6886,22 @@
     "_OptionalStartContactEvaluationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartContactEvaluationRequestRequestTypeDef(
     _RequiredStartContactEvaluationRequestRequestTypeDef,
     _OptionalStartContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-
-StartContactEvaluationResponseTypeDef = TypedDict(
-    "StartContactEvaluationResponseTypeDef",
+StartContactEvaluationResponseOutputTypeDef = TypedDict(
+    "StartContactEvaluationResponseOutputTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -6730,16 +6921,16 @@
         "InstanceId": str,
         "ContactId": str,
         "ChatStreamingConfiguration": "ChatStreamingConfigurationTypeDef",
         "ClientToken": str,
     },
 )
 
-StartContactStreamingResponseTypeDef = TypedDict(
-    "StartContactStreamingResponseTypeDef",
+StartContactStreamingResponseOutputTypeDef = TypedDict(
+    "StartContactStreamingResponseOutputTypeDef",
     {
         "StreamingId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartOutboundVoiceContactRequestRequestTypeDef = TypedDict(
@@ -6760,24 +6951,22 @@
         "AnswerMachineDetectionConfig": "AnswerMachineDetectionConfigTypeDef",
         "CampaignId": str,
         "TrafficType": TrafficTypeType,
     },
     total=False,
 )
 
-
 class StartOutboundVoiceContactRequestRequestTypeDef(
     _RequiredStartOutboundVoiceContactRequestRequestTypeDef,
     _OptionalStartOutboundVoiceContactRequestRequestTypeDef,
 ):
     pass
 
-
-StartOutboundVoiceContactResponseTypeDef = TypedDict(
-    "StartOutboundVoiceContactResponseTypeDef",
+StartOutboundVoiceContactResponseOutputTypeDef = TypedDict(
+    "StartOutboundVoiceContactResponseOutputTypeDef",
     {
         "ContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTaskContactRequestRequestTypeDef = TypedDict(
@@ -6800,23 +6989,21 @@
         "TaskTemplateId": str,
         "QuickConnectId": str,
         "RelatedContactId": str,
     },
     total=False,
 )
 
-
 class StartTaskContactRequestRequestTypeDef(
     _RequiredStartTaskContactRequestRequestTypeDef, _OptionalStartTaskContactRequestRequestTypeDef
 ):
     pass
 
-
-StartTaskContactResponseTypeDef = TypedDict(
-    "StartTaskContactResponseTypeDef",
+StartTaskContactResponseOutputTypeDef = TypedDict(
+    "StartTaskContactResponseOutputTypeDef",
     {
         "ContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopContactRecordingRequestRequestTypeDef = TypedDict(
@@ -6851,16 +7038,16 @@
         "FieldName": str,
         "Value": str,
         "ComparisonType": StringComparisonTypeType,
     },
     total=False,
 )
 
-StringReferenceTypeDef = TypedDict(
-    "StringReferenceTypeDef",
+StringReferenceOutputTypeDef = TypedDict(
+    "StringReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 _RequiredSubmitContactEvaluationRequestRequestTypeDef = TypedDict(
@@ -6875,24 +7062,22 @@
     {
         "Answers": Mapping[str, "EvaluationAnswerInputTypeDef"],
         "Notes": Mapping[str, "EvaluationNoteTypeDef"],
     },
     total=False,
 )
 
-
 class SubmitContactEvaluationRequestRequestTypeDef(
     _RequiredSubmitContactEvaluationRequestRequestTypeDef,
     _OptionalSubmitContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-
-SubmitContactEvaluationResponseTypeDef = TypedDict(
-    "SubmitContactEvaluationResponseTypeDef",
+SubmitContactEvaluationResponseOutputTypeDef = TypedDict(
+    "SubmitContactEvaluationResponseOutputTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -6929,22 +7114,32 @@
         "tagValue": str,
         "tagKeyComparisonType": StringComparisonTypeType,
         "tagValueComparisonType": StringComparisonTypeType,
     },
     total=False,
 )
 
-TagSetTypeDef = TypedDict(
-    "TagSetTypeDef",
+TagSetOutputTypeDef = TypedDict(
+    "TagSetOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+TaskActionDefinitionOutputTypeDef = TypedDict(
+    "TaskActionDefinitionOutputTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "ContactFlowId": str,
+        "References": Dict[str, "ReferenceOutputTypeDef"],
+    },
+)
+
 _RequiredTaskActionDefinitionTypeDef = TypedDict(
     "_RequiredTaskActionDefinitionTypeDef",
     {
         "Name": str,
         "ContactFlowId": str,
     },
 )
@@ -6953,56 +7148,95 @@
     {
         "Description": str,
         "References": Mapping[str, "ReferenceTypeDef"],
     },
     total=False,
 )
 
-
 class TaskActionDefinitionTypeDef(
     _RequiredTaskActionDefinitionTypeDef, _OptionalTaskActionDefinitionTypeDef
 ):
     pass
 
+TaskTemplateConstraintsOutputTypeDef = TypedDict(
+    "TaskTemplateConstraintsOutputTypeDef",
+    {
+        "RequiredFields": List["RequiredFieldInfoOutputTypeDef"],
+        "ReadOnlyFields": List["ReadOnlyFieldInfoOutputTypeDef"],
+        "InvisibleFields": List["InvisibleFieldInfoOutputTypeDef"],
+    },
+)
 
 TaskTemplateConstraintsTypeDef = TypedDict(
     "TaskTemplateConstraintsTypeDef",
     {
         "RequiredFields": Sequence["RequiredFieldInfoTypeDef"],
         "ReadOnlyFields": Sequence["ReadOnlyFieldInfoTypeDef"],
         "InvisibleFields": Sequence["InvisibleFieldInfoTypeDef"],
     },
     total=False,
 )
 
+TaskTemplateDefaultFieldValueOutputTypeDef = TypedDict(
+    "TaskTemplateDefaultFieldValueOutputTypeDef",
+    {
+        "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
+        "DefaultValue": str,
+    },
+)
+
 TaskTemplateDefaultFieldValueTypeDef = TypedDict(
     "TaskTemplateDefaultFieldValueTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
         "DefaultValue": str,
     },
     total=False,
 )
 
+TaskTemplateDefaultsOutputTypeDef = TypedDict(
+    "TaskTemplateDefaultsOutputTypeDef",
+    {
+        "DefaultFieldValues": List["TaskTemplateDefaultFieldValueOutputTypeDef"],
+    },
+)
+
 TaskTemplateDefaultsTypeDef = TypedDict(
     "TaskTemplateDefaultsTypeDef",
     {
         "DefaultFieldValues": Sequence["TaskTemplateDefaultFieldValueTypeDef"],
     },
     total=False,
 )
 
+TaskTemplateFieldIdentifierOutputTypeDef = TypedDict(
+    "TaskTemplateFieldIdentifierOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 TaskTemplateFieldIdentifierTypeDef = TypedDict(
     "TaskTemplateFieldIdentifierTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+TaskTemplateFieldOutputTypeDef = TypedDict(
+    "TaskTemplateFieldOutputTypeDef",
+    {
+        "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
+        "Description": str,
+        "Type": TaskTemplateFieldTypeType,
+        "SingleSelectOptions": List[str],
+    },
+)
+
 _RequiredTaskTemplateFieldTypeDef = TypedDict(
     "_RequiredTaskTemplateFieldTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
 )
 _OptionalTaskTemplateFieldTypeDef = TypedDict(
@@ -7011,80 +7245,101 @@
         "Description": str,
         "Type": TaskTemplateFieldTypeType,
         "SingleSelectOptions": Sequence[str],
     },
     total=False,
 )
 
-
 class TaskTemplateFieldTypeDef(
     _RequiredTaskTemplateFieldTypeDef, _OptionalTaskTemplateFieldTypeDef
 ):
     pass
 
-
-TaskTemplateMetadataTypeDef = TypedDict(
-    "TaskTemplateMetadataTypeDef",
+TaskTemplateMetadataOutputTypeDef = TypedDict(
+    "TaskTemplateMetadataOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
     },
 )
 
+TelephonyConfigOutputTypeDef = TypedDict(
+    "TelephonyConfigOutputTypeDef",
+    {
+        "Distributions": List["DistributionOutputTypeDef"],
+    },
+)
+
 TelephonyConfigTypeDef = TypedDict(
     "TelephonyConfigTypeDef",
     {
-        "Distributions": List["DistributionTypeDef"],
+        "Distributions": Sequence["DistributionTypeDef"],
+    },
+)
+
+ThresholdOutputTypeDef = TypedDict(
+    "ThresholdOutputTypeDef",
+    {
+        "Comparison": Literal["LT"],
+        "ThresholdValue": float,
     },
 )
 
 ThresholdTypeDef = TypedDict(
     "ThresholdTypeDef",
     {
         "Comparison": Literal["LT"],
         "ThresholdValue": float,
     },
     total=False,
 )
 
+ThresholdV2OutputTypeDef = TypedDict(
+    "ThresholdV2OutputTypeDef",
+    {
+        "Comparison": str,
+        "ThresholdValue": float,
+    },
+)
+
 ThresholdV2TypeDef = TypedDict(
     "ThresholdV2TypeDef",
     {
         "Comparison": str,
         "ThresholdValue": float,
     },
     total=False,
 )
 
-TrafficDistributionGroupSummaryTypeDef = TypedDict(
-    "TrafficDistributionGroupSummaryTypeDef",
+TrafficDistributionGroupOutputTypeDef = TypedDict(
+    "TrafficDistributionGroupOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
+        "Description": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
+        "Tags": Dict[str, str],
     },
 )
 
-TrafficDistributionGroupTypeDef = TypedDict(
-    "TrafficDistributionGroupTypeDef",
+TrafficDistributionGroupSummaryOutputTypeDef = TypedDict(
+    "TrafficDistributionGroupSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
-        "Description": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
-        "Tags": Dict[str, str],
     },
 )
 
 _RequiredTransferContactRequestRequestTypeDef = TypedDict(
     "_RequiredTransferContactRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -7098,23 +7353,21 @@
         "QueueId": str,
         "UserId": str,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class TransferContactRequestRequestTypeDef(
     _RequiredTransferContactRequestRequestTypeDef, _OptionalTransferContactRequestRequestTypeDef
 ):
     pass
 
-
-TransferContactResponseTypeDef = TypedDict(
-    "TransferContactResponseTypeDef",
+TransferContactResponseOutputTypeDef = TypedDict(
+    "TransferContactResponseOutputTypeDef",
     {
         "ContactId": str,
         "ContactArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7141,21 +7394,19 @@
         "State": AgentStatusStateType,
         "DisplayOrder": int,
         "ResetOrderNumber": bool,
     },
     total=False,
 )
 
-
 class UpdateAgentStatusRequestRequestTypeDef(
     _RequiredUpdateAgentStatusRequestRequestTypeDef, _OptionalUpdateAgentStatusRequestRequestTypeDef
 ):
     pass
 
-
 UpdateContactAttributesRequestRequestTypeDef = TypedDict(
     "UpdateContactAttributesRequestRequestTypeDef",
     {
         "InitialContactId": str,
         "InstanceId": str,
         "Attributes": Mapping[str, str],
     },
@@ -7173,24 +7424,22 @@
     {
         "Answers": Mapping[str, "EvaluationAnswerInputTypeDef"],
         "Notes": Mapping[str, "EvaluationNoteTypeDef"],
     },
     total=False,
 )
 
-
 class UpdateContactEvaluationRequestRequestTypeDef(
     _RequiredUpdateContactEvaluationRequestRequestTypeDef,
     _OptionalUpdateContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateContactEvaluationResponseTypeDef = TypedDict(
-    "UpdateContactEvaluationResponseTypeDef",
+UpdateContactEvaluationResponseOutputTypeDef = TypedDict(
+    "UpdateContactEvaluationResponseOutputTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7216,22 +7465,20 @@
         "Name": str,
         "Description": str,
         "ContactFlowState": ContactFlowStateType,
     },
     total=False,
 )
 
-
 class UpdateContactFlowMetadataRequestRequestTypeDef(
     _RequiredUpdateContactFlowMetadataRequestRequestTypeDef,
     _OptionalUpdateContactFlowMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateContactFlowModuleContentRequestRequestTypeDef = TypedDict(
     "UpdateContactFlowModuleContentRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowModuleId": str,
         "Content": str,
     },
@@ -7250,22 +7497,20 @@
         "Name": str,
         "Description": str,
         "State": ContactFlowModuleStateType,
     },
     total=False,
 )
 
-
 class UpdateContactFlowModuleMetadataRequestRequestTypeDef(
     _RequiredUpdateContactFlowModuleMetadataRequestRequestTypeDef,
     _OptionalUpdateContactFlowModuleMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateContactFlowNameRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactFlowNameRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowId": str,
     },
 )
@@ -7274,22 +7519,20 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateContactFlowNameRequestRequestTypeDef(
     _RequiredUpdateContactFlowNameRequestRequestTypeDef,
     _OptionalUpdateContactFlowNameRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
@@ -7299,21 +7542,19 @@
         "Name": str,
         "Description": str,
         "References": Mapping[str, "ReferenceTypeDef"],
     },
     total=False,
 )
 
-
 class UpdateContactRequestRequestTypeDef(
     _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
 ):
     pass
 
-
 UpdateContactScheduleRequestRequestTypeDef = TypedDict(
     "UpdateContactScheduleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ScheduledTime": Union[datetime, str],
     },
@@ -7336,24 +7577,22 @@
         "Description": str,
         "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class UpdateEvaluationFormRequestRequestTypeDef(
     _RequiredUpdateEvaluationFormRequestRequestTypeDef,
     _OptionalUpdateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateEvaluationFormResponseTypeDef = TypedDict(
-    "UpdateEvaluationFormResponseTypeDef",
+UpdateEvaluationFormResponseOutputTypeDef = TypedDict(
+    "UpdateEvaluationFormResponseOutputTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -7372,22 +7611,20 @@
         "Description": str,
         "TimeZone": str,
         "Config": Sequence["HoursOfOperationConfigTypeDef"],
     },
     total=False,
 )
 
-
 class UpdateHoursOfOperationRequestRequestTypeDef(
     _RequiredUpdateHoursOfOperationRequestRequestTypeDef,
     _OptionalUpdateHoursOfOperationRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateInstanceAttributeRequestRequestTypeDef = TypedDict(
     "UpdateInstanceAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AttributeType": InstanceAttributeTypeType,
         "Value": str,
     },
@@ -7431,23 +7668,21 @@
     "_OptionalUpdatePhoneNumberRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
-
-UpdatePhoneNumberResponseTypeDef = TypedDict(
-    "UpdatePhoneNumberResponseTypeDef",
+UpdatePhoneNumberResponseOutputTypeDef = TypedDict(
+    "UpdatePhoneNumberResponseOutputTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7464,23 +7699,21 @@
         "Name": str,
         "Description": str,
         "S3Uri": str,
     },
     total=False,
 )
 
-
 class UpdatePromptRequestRequestTypeDef(
     _RequiredUpdatePromptRequestRequestTypeDef, _OptionalUpdatePromptRequestRequestTypeDef
 ):
     pass
 
-
-UpdatePromptResponseTypeDef = TypedDict(
-    "UpdatePromptResponseTypeDef",
+UpdatePromptResponseOutputTypeDef = TypedDict(
+    "UpdatePromptResponseOutputTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7504,22 +7737,20 @@
     "_OptionalUpdateQueueMaxContactsRequestRequestTypeDef",
     {
         "MaxContacts": int,
     },
     total=False,
 )
 
-
 class UpdateQueueMaxContactsRequestRequestTypeDef(
     _RequiredUpdateQueueMaxContactsRequestRequestTypeDef,
     _OptionalUpdateQueueMaxContactsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateQueueNameRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateQueueNameRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
@@ -7528,21 +7759,19 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateQueueNameRequestRequestTypeDef(
     _RequiredUpdateQueueNameRequestRequestTypeDef, _OptionalUpdateQueueNameRequestRequestTypeDef
 ):
     pass
 
-
 UpdateQueueOutboundCallerConfigRequestRequestTypeDef = TypedDict(
     "UpdateQueueOutboundCallerConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
         "OutboundCallerConfig": "OutboundCallerConfigTypeDef",
     },
@@ -7578,22 +7807,20 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateQuickConnectNameRequestRequestTypeDef(
     _RequiredUpdateQuickConnectNameRequestRequestTypeDef,
     _OptionalUpdateQuickConnectNameRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateRoutingProfileConcurrencyRequestRequestTypeDef = TypedDict(
     "UpdateRoutingProfileConcurrencyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
         "MediaConcurrencies": Sequence["MediaConcurrencyTypeDef"],
     },
@@ -7620,22 +7847,20 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateRoutingProfileNameRequestRequestTypeDef(
     _RequiredUpdateRoutingProfileNameRequestRequestTypeDef,
     _OptionalUpdateRoutingProfileNameRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateRoutingProfileQueuesRequestRequestTypeDef = TypedDict(
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
         "QueueConfigs": Sequence["RoutingProfileQueueConfigTypeDef"],
     },
@@ -7667,22 +7892,20 @@
         "Permissions": Sequence[str],
         "AllowedAccessControlTags": Mapping[str, str],
         "TagRestrictedResources": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateSecurityProfileRequestRequestTypeDef(
     _RequiredUpdateSecurityProfileRequestRequestTypeDef,
     _OptionalUpdateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateTaskTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTaskTemplateRequestRequestTypeDef",
     {
         "TaskTemplateId": str,
         "InstanceId": str,
     },
 )
@@ -7696,34 +7919,32 @@
         "Defaults": "TaskTemplateDefaultsTypeDef",
         "Status": TaskTemplateStatusType,
         "Fields": Sequence["TaskTemplateFieldTypeDef"],
     },
     total=False,
 )
 
-
 class UpdateTaskTemplateRequestRequestTypeDef(
     _RequiredUpdateTaskTemplateRequestRequestTypeDef,
     _OptionalUpdateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateTaskTemplateResponseTypeDef = TypedDict(
-    "UpdateTaskTemplateResponseTypeDef",
+UpdateTaskTemplateResponseOutputTypeDef = TypedDict(
+    "UpdateTaskTemplateResponseOutputTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
-        "Constraints": "TaskTemplateConstraintsTypeDef",
-        "Defaults": "TaskTemplateDefaultsTypeDef",
-        "Fields": List["TaskTemplateFieldTypeDef"],
+        "Constraints": "TaskTemplateConstraintsOutputTypeDef",
+        "Defaults": "TaskTemplateDefaultsOutputTypeDef",
+        "Fields": List["TaskTemplateFieldOutputTypeDef"],
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7737,22 +7958,20 @@
     "_OptionalUpdateTrafficDistributionRequestRequestTypeDef",
     {
         "TelephonyConfig": "TelephonyConfigTypeDef",
     },
     total=False,
 )
 
-
 class UpdateTrafficDistributionRequestRequestTypeDef(
     _RequiredUpdateTrafficDistributionRequestRequestTypeDef,
     _OptionalUpdateTrafficDistributionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateUserHierarchyGroupNameRequestRequestTypeDef = TypedDict(
     "UpdateUserHierarchyGroupNameRequestRequestTypeDef",
     {
         "Name": str,
         "HierarchyGroupId": str,
         "InstanceId": str,
     },
@@ -7769,22 +7988,20 @@
     "_OptionalUpdateUserHierarchyRequestRequestTypeDef",
     {
         "HierarchyGroupId": str,
     },
     total=False,
 )
 
-
 class UpdateUserHierarchyRequestRequestTypeDef(
     _RequiredUpdateUserHierarchyRequestRequestTypeDef,
     _OptionalUpdateUserHierarchyRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateUserHierarchyStructureRequestRequestTypeDef = TypedDict(
     "UpdateUserHierarchyStructureRequestRequestTypeDef",
     {
         "HierarchyStructure": "HierarchyStructureUpdateTypeDef",
         "InstanceId": str,
     },
 )
@@ -7821,24 +8038,24 @@
     {
         "SecurityProfileIds": Sequence[str],
         "UserId": str,
         "InstanceId": str,
     },
 )
 
-UrlReferenceTypeDef = TypedDict(
-    "UrlReferenceTypeDef",
+UrlReferenceOutputTypeDef = TypedDict(
+    "UrlReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-UseCaseTypeDef = TypedDict(
-    "UseCaseTypeDef",
+UseCaseOutputTypeDef = TypedDict(
+    "UseCaseOutputTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "UseCaseType": UseCaseTypeType,
     },
 )
 
@@ -7850,49 +8067,86 @@
         "RoutingProfiles": Sequence[str],
         "Agents": Sequence[str],
         "UserHierarchyGroups": Sequence[str],
     },
     total=False,
 )
 
-UserDataTypeDef = TypedDict(
-    "UserDataTypeDef",
+UserDataOutputTypeDef = TypedDict(
+    "UserDataOutputTypeDef",
     {
-        "User": "UserReferenceTypeDef",
-        "RoutingProfile": "RoutingProfileReferenceTypeDef",
-        "HierarchyPath": "HierarchyPathReferenceTypeDef",
-        "Status": "AgentStatusReferenceTypeDef",
+        "User": "UserReferenceOutputTypeDef",
+        "RoutingProfile": "RoutingProfileReferenceOutputTypeDef",
+        "HierarchyPath": "HierarchyPathReferenceOutputTypeDef",
+        "Status": "AgentStatusReferenceOutputTypeDef",
         "AvailableSlotsByChannel": Dict[ChannelType, int],
         "MaxSlotsByChannel": Dict[ChannelType, int],
         "ActiveSlotsByChannel": Dict[ChannelType, int],
-        "Contacts": List["AgentContactReferenceTypeDef"],
+        "Contacts": List["AgentContactReferenceOutputTypeDef"],
         "NextStatus": str,
     },
 )
 
-UserIdentityInfoLiteTypeDef = TypedDict(
-    "UserIdentityInfoLiteTypeDef",
+UserIdentityInfoLiteOutputTypeDef = TypedDict(
+    "UserIdentityInfoLiteOutputTypeDef",
     {
         "FirstName": str,
         "LastName": str,
     },
 )
 
+UserIdentityInfoOutputTypeDef = TypedDict(
+    "UserIdentityInfoOutputTypeDef",
+    {
+        "FirstName": str,
+        "LastName": str,
+        "Email": str,
+        "SecondaryEmail": str,
+        "Mobile": str,
+    },
+)
+
 UserIdentityInfoTypeDef = TypedDict(
     "UserIdentityInfoTypeDef",
     {
         "FirstName": str,
         "LastName": str,
         "Email": str,
         "SecondaryEmail": str,
         "Mobile": str,
     },
     total=False,
 )
 
+UserOutputTypeDef = TypedDict(
+    "UserOutputTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Username": str,
+        "IdentityInfo": "UserIdentityInfoOutputTypeDef",
+        "PhoneConfig": "UserPhoneConfigOutputTypeDef",
+        "DirectoryUserId": str,
+        "SecurityProfileIds": List[str],
+        "RoutingProfileId": str,
+        "HierarchyGroupId": str,
+        "Tags": Dict[str, str],
+    },
+)
+
+UserPhoneConfigOutputTypeDef = TypedDict(
+    "UserPhoneConfigOutputTypeDef",
+    {
+        "PhoneType": PhoneTypeType,
+        "AutoAccept": bool,
+        "AfterContactWorkTimeLimit": int,
+        "DeskPhoneNumber": str,
+    },
+)
+
 _RequiredUserPhoneConfigTypeDef = TypedDict(
     "_RequiredUserPhoneConfigTypeDef",
     {
         "PhoneType": PhoneTypeType,
     },
 )
 _OptionalUserPhoneConfigTypeDef = TypedDict(
@@ -7901,29 +8155,35 @@
         "AutoAccept": bool,
         "AfterContactWorkTimeLimit": int,
         "DeskPhoneNumber": str,
     },
     total=False,
 )
 
-
 class UserPhoneConfigTypeDef(_RequiredUserPhoneConfigTypeDef, _OptionalUserPhoneConfigTypeDef):
     pass
 
+UserQuickConnectConfigOutputTypeDef = TypedDict(
+    "UserQuickConnectConfigOutputTypeDef",
+    {
+        "UserId": str,
+        "ContactFlowId": str,
+    },
+)
 
 UserQuickConnectConfigTypeDef = TypedDict(
     "UserQuickConnectConfigTypeDef",
     {
         "UserId": str,
         "ContactFlowId": str,
     },
 )
 
-UserReferenceTypeDef = TypedDict(
-    "UserReferenceTypeDef",
+UserReferenceOutputTypeDef = TypedDict(
+    "UserReferenceOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 UserSearchCriteriaTypeDef = TypedDict(
@@ -7941,90 +8201,74 @@
     "UserSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-UserSearchSummaryTypeDef = TypedDict(
-    "UserSearchSummaryTypeDef",
+UserSearchSummaryOutputTypeDef = TypedDict(
+    "UserSearchSummaryOutputTypeDef",
     {
         "Arn": str,
         "DirectoryUserId": str,
         "HierarchyGroupId": str,
         "Id": str,
-        "IdentityInfo": "UserIdentityInfoLiteTypeDef",
-        "PhoneConfig": "UserPhoneConfigTypeDef",
+        "IdentityInfo": "UserIdentityInfoLiteOutputTypeDef",
+        "PhoneConfig": "UserPhoneConfigOutputTypeDef",
         "RoutingProfileId": str,
         "SecurityProfileIds": List[str],
         "Tags": Dict[str, str],
         "Username": str,
     },
 )
 
-UserSummaryTypeDef = TypedDict(
-    "UserSummaryTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Username": str,
-    },
-)
-
-UserTypeDef = TypedDict(
-    "UserTypeDef",
+UserSummaryOutputTypeDef = TypedDict(
+    "UserSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Username": str,
-        "IdentityInfo": "UserIdentityInfoTypeDef",
-        "PhoneConfig": "UserPhoneConfigTypeDef",
-        "DirectoryUserId": str,
-        "SecurityProfileIds": List[str],
-        "RoutingProfileId": str,
-        "HierarchyGroupId": str,
-        "Tags": Dict[str, str],
     },
 )
 
-VocabularySummaryTypeDef = TypedDict(
-    "VocabularySummaryTypeDef",
+VocabularyOutputTypeDef = TypedDict(
+    "VocabularyOutputTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
         "FailureReason": str,
+        "Content": str,
+        "Tags": Dict[str, str],
     },
 )
 
-VocabularyTypeDef = TypedDict(
-    "VocabularyTypeDef",
+VocabularySummaryOutputTypeDef = TypedDict(
+    "VocabularySummaryOutputTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
         "FailureReason": str,
-        "Content": str,
-        "Tags": Dict[str, str],
     },
 )
 
 VoiceRecordingConfigurationTypeDef = TypedDict(
     "VoiceRecordingConfigurationTypeDef",
     {
         "VoiceRecordingTrack": VoiceRecordingTrackType,
     },
     total=False,
 )
 
-WisdomInfoTypeDef = TypedDict(
-    "WisdomInfoTypeDef",
+WisdomInfoOutputTypeDef = TypedDict(
+    "WisdomInfoOutputTypeDef",
     {
         "SessionArn": str,
     },
 )
```

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect/type_defs.pyi` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for connect service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_connect.type_defs import ActionSummaryTypeDef
+    from mypy_boto3_connect.type_defs import ActionSummaryOutputTypeDef
 
-    data: ActionSummaryTypeDef = {...}
+    data: ActionSummaryOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -83,102 +83,105 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "ActionSummaryTypeDef",
+    "ActionSummaryOutputTypeDef",
     "ActivateEvaluationFormRequestRequestTypeDef",
-    "ActivateEvaluationFormResponseTypeDef",
-    "AgentContactReferenceTypeDef",
-    "AgentInfoTypeDef",
-    "AgentStatusReferenceTypeDef",
-    "AgentStatusSummaryTypeDef",
-    "AgentStatusTypeDef",
+    "ActivateEvaluationFormResponseOutputTypeDef",
+    "AgentContactReferenceOutputTypeDef",
+    "AgentInfoOutputTypeDef",
+    "AgentStatusOutputTypeDef",
+    "AgentStatusReferenceOutputTypeDef",
+    "AgentStatusSummaryOutputTypeDef",
     "AnswerMachineDetectionConfigTypeDef",
     "AssociateApprovedOriginRequestRequestTypeDef",
     "AssociateBotRequestRequestTypeDef",
     "AssociateDefaultVocabularyRequestRequestTypeDef",
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
-    "AssociateInstanceStorageConfigResponseTypeDef",
+    "AssociateInstanceStorageConfigResponseOutputTypeDef",
     "AssociateLambdaFunctionRequestRequestTypeDef",
     "AssociateLexBotRequestRequestTypeDef",
     "AssociatePhoneNumberContactFlowRequestRequestTypeDef",
     "AssociateQueueQuickConnectsRequestRequestTypeDef",
     "AssociateRoutingProfileQueuesRequestRequestTypeDef",
     "AssociateSecurityKeyRequestRequestTypeDef",
-    "AssociateSecurityKeyResponseTypeDef",
-    "AttachmentReferenceTypeDef",
-    "AttributeTypeDef",
-    "AvailableNumberSummaryTypeDef",
+    "AssociateSecurityKeyResponseOutputTypeDef",
+    "AttachmentReferenceOutputTypeDef",
+    "AttributeOutputTypeDef",
+    "AvailableNumberSummaryOutputTypeDef",
     "ChatMessageTypeDef",
     "ChatParticipantRoleConfigTypeDef",
     "ChatStreamingConfigurationTypeDef",
     "ClaimPhoneNumberRequestRequestTypeDef",
-    "ClaimPhoneNumberResponseTypeDef",
-    "ClaimedPhoneNumberSummaryTypeDef",
+    "ClaimPhoneNumberResponseOutputTypeDef",
+    "ClaimedPhoneNumberSummaryOutputTypeDef",
     "ContactFilterTypeDef",
-    "ContactFlowModuleSummaryTypeDef",
-    "ContactFlowModuleTypeDef",
-    "ContactFlowSummaryTypeDef",
-    "ContactFlowTypeDef",
-    "ContactTypeDef",
+    "ContactFlowModuleOutputTypeDef",
+    "ContactFlowModuleSummaryOutputTypeDef",
+    "ContactFlowOutputTypeDef",
+    "ContactFlowSummaryOutputTypeDef",
+    "ContactOutputTypeDef",
     "ControlPlaneTagFilterTypeDef",
     "CreateAgentStatusRequestRequestTypeDef",
-    "CreateAgentStatusResponseTypeDef",
+    "CreateAgentStatusResponseOutputTypeDef",
     "CreateContactFlowModuleRequestRequestTypeDef",
-    "CreateContactFlowModuleResponseTypeDef",
+    "CreateContactFlowModuleResponseOutputTypeDef",
     "CreateContactFlowRequestRequestTypeDef",
-    "CreateContactFlowResponseTypeDef",
+    "CreateContactFlowResponseOutputTypeDef",
     "CreateEvaluationFormRequestRequestTypeDef",
-    "CreateEvaluationFormResponseTypeDef",
+    "CreateEvaluationFormResponseOutputTypeDef",
     "CreateHoursOfOperationRequestRequestTypeDef",
-    "CreateHoursOfOperationResponseTypeDef",
+    "CreateHoursOfOperationResponseOutputTypeDef",
     "CreateInstanceRequestRequestTypeDef",
-    "CreateInstanceResponseTypeDef",
+    "CreateInstanceResponseOutputTypeDef",
     "CreateIntegrationAssociationRequestRequestTypeDef",
-    "CreateIntegrationAssociationResponseTypeDef",
+    "CreateIntegrationAssociationResponseOutputTypeDef",
     "CreateParticipantRequestRequestTypeDef",
-    "CreateParticipantResponseTypeDef",
+    "CreateParticipantResponseOutputTypeDef",
     "CreatePromptRequestRequestTypeDef",
-    "CreatePromptResponseTypeDef",
+    "CreatePromptResponseOutputTypeDef",
     "CreateQueueRequestRequestTypeDef",
-    "CreateQueueResponseTypeDef",
+    "CreateQueueResponseOutputTypeDef",
     "CreateQuickConnectRequestRequestTypeDef",
-    "CreateQuickConnectResponseTypeDef",
+    "CreateQuickConnectResponseOutputTypeDef",
     "CreateRoutingProfileRequestRequestTypeDef",
-    "CreateRoutingProfileResponseTypeDef",
+    "CreateRoutingProfileResponseOutputTypeDef",
     "CreateRuleRequestRequestTypeDef",
-    "CreateRuleResponseTypeDef",
+    "CreateRuleResponseOutputTypeDef",
     "CreateSecurityProfileRequestRequestTypeDef",
-    "CreateSecurityProfileResponseTypeDef",
+    "CreateSecurityProfileResponseOutputTypeDef",
     "CreateTaskTemplateRequestRequestTypeDef",
-    "CreateTaskTemplateResponseTypeDef",
+    "CreateTaskTemplateResponseOutputTypeDef",
     "CreateTrafficDistributionGroupRequestRequestTypeDef",
-    "CreateTrafficDistributionGroupResponseTypeDef",
+    "CreateTrafficDistributionGroupResponseOutputTypeDef",
     "CreateUseCaseRequestRequestTypeDef",
-    "CreateUseCaseResponseTypeDef",
+    "CreateUseCaseResponseOutputTypeDef",
     "CreateUserHierarchyGroupRequestRequestTypeDef",
-    "CreateUserHierarchyGroupResponseTypeDef",
+    "CreateUserHierarchyGroupResponseOutputTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "CreateUserResponseTypeDef",
+    "CreateUserResponseOutputTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
-    "CreateVocabularyResponseTypeDef",
-    "CredentialsTypeDef",
+    "CreateVocabularyResponseOutputTypeDef",
+    "CredentialsOutputTypeDef",
+    "CrossChannelBehaviorOutputTypeDef",
     "CrossChannelBehaviorTypeDef",
-    "CurrentMetricDataTypeDef",
-    "CurrentMetricResultTypeDef",
+    "CurrentMetricDataOutputTypeDef",
+    "CurrentMetricOutputTypeDef",
+    "CurrentMetricResultOutputTypeDef",
     "CurrentMetricSortCriteriaTypeDef",
     "CurrentMetricTypeDef",
-    "DateReferenceTypeDef",
+    "DateReferenceOutputTypeDef",
     "DeactivateEvaluationFormRequestRequestTypeDef",
-    "DeactivateEvaluationFormResponseTypeDef",
-    "DefaultVocabularyTypeDef",
+    "DeactivateEvaluationFormResponseOutputTypeDef",
+    "DefaultVocabularyOutputTypeDef",
     "DeleteContactEvaluationRequestRequestTypeDef",
     "DeleteContactFlowModuleRequestRequestTypeDef",
     "DeleteContactFlowRequestRequestTypeDef",
     "DeleteEvaluationFormRequestRequestTypeDef",
     "DeleteHoursOfOperationRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteIntegrationAssociationRequestRequestTypeDef",
@@ -190,538 +193,594 @@
     "DeleteSecurityProfileRequestRequestTypeDef",
     "DeleteTaskTemplateRequestRequestTypeDef",
     "DeleteTrafficDistributionGroupRequestRequestTypeDef",
     "DeleteUseCaseRequestRequestTypeDef",
     "DeleteUserHierarchyGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteVocabularyRequestRequestTypeDef",
-    "DeleteVocabularyResponseTypeDef",
+    "DeleteVocabularyResponseOutputTypeDef",
     "DescribeAgentStatusRequestRequestTypeDef",
-    "DescribeAgentStatusResponseTypeDef",
+    "DescribeAgentStatusResponseOutputTypeDef",
     "DescribeContactEvaluationRequestRequestTypeDef",
-    "DescribeContactEvaluationResponseTypeDef",
+    "DescribeContactEvaluationResponseOutputTypeDef",
     "DescribeContactFlowModuleRequestRequestTypeDef",
-    "DescribeContactFlowModuleResponseTypeDef",
+    "DescribeContactFlowModuleResponseOutputTypeDef",
     "DescribeContactFlowRequestRequestTypeDef",
-    "DescribeContactFlowResponseTypeDef",
+    "DescribeContactFlowResponseOutputTypeDef",
     "DescribeContactRequestRequestTypeDef",
-    "DescribeContactResponseTypeDef",
+    "DescribeContactResponseOutputTypeDef",
     "DescribeEvaluationFormRequestRequestTypeDef",
-    "DescribeEvaluationFormResponseTypeDef",
+    "DescribeEvaluationFormResponseOutputTypeDef",
     "DescribeHoursOfOperationRequestRequestTypeDef",
-    "DescribeHoursOfOperationResponseTypeDef",
+    "DescribeHoursOfOperationResponseOutputTypeDef",
     "DescribeInstanceAttributeRequestRequestTypeDef",
-    "DescribeInstanceAttributeResponseTypeDef",
+    "DescribeInstanceAttributeResponseOutputTypeDef",
     "DescribeInstanceRequestRequestTypeDef",
-    "DescribeInstanceResponseTypeDef",
+    "DescribeInstanceResponseOutputTypeDef",
     "DescribeInstanceStorageConfigRequestRequestTypeDef",
-    "DescribeInstanceStorageConfigResponseTypeDef",
+    "DescribeInstanceStorageConfigResponseOutputTypeDef",
     "DescribePhoneNumberRequestRequestTypeDef",
-    "DescribePhoneNumberResponseTypeDef",
+    "DescribePhoneNumberResponseOutputTypeDef",
     "DescribePromptRequestRequestTypeDef",
-    "DescribePromptResponseTypeDef",
+    "DescribePromptResponseOutputTypeDef",
     "DescribeQueueRequestRequestTypeDef",
-    "DescribeQueueResponseTypeDef",
+    "DescribeQueueResponseOutputTypeDef",
     "DescribeQuickConnectRequestRequestTypeDef",
-    "DescribeQuickConnectResponseTypeDef",
+    "DescribeQuickConnectResponseOutputTypeDef",
     "DescribeRoutingProfileRequestRequestTypeDef",
-    "DescribeRoutingProfileResponseTypeDef",
+    "DescribeRoutingProfileResponseOutputTypeDef",
     "DescribeRuleRequestRequestTypeDef",
-    "DescribeRuleResponseTypeDef",
+    "DescribeRuleResponseOutputTypeDef",
     "DescribeSecurityProfileRequestRequestTypeDef",
-    "DescribeSecurityProfileResponseTypeDef",
+    "DescribeSecurityProfileResponseOutputTypeDef",
     "DescribeTrafficDistributionGroupRequestRequestTypeDef",
-    "DescribeTrafficDistributionGroupResponseTypeDef",
+    "DescribeTrafficDistributionGroupResponseOutputTypeDef",
     "DescribeUserHierarchyGroupRequestRequestTypeDef",
-    "DescribeUserHierarchyGroupResponseTypeDef",
+    "DescribeUserHierarchyGroupResponseOutputTypeDef",
     "DescribeUserHierarchyStructureRequestRequestTypeDef",
-    "DescribeUserHierarchyStructureResponseTypeDef",
+    "DescribeUserHierarchyStructureResponseOutputTypeDef",
     "DescribeUserRequestRequestTypeDef",
-    "DescribeUserResponseTypeDef",
+    "DescribeUserResponseOutputTypeDef",
     "DescribeVocabularyRequestRequestTypeDef",
-    "DescribeVocabularyResponseTypeDef",
-    "DimensionsTypeDef",
+    "DescribeVocabularyResponseOutputTypeDef",
+    "DimensionsOutputTypeDef",
     "DisassociateApprovedOriginRequestRequestTypeDef",
     "DisassociateBotRequestRequestTypeDef",
     "DisassociateInstanceStorageConfigRequestRequestTypeDef",
     "DisassociateLambdaFunctionRequestRequestTypeDef",
     "DisassociateLexBotRequestRequestTypeDef",
     "DisassociatePhoneNumberContactFlowRequestRequestTypeDef",
     "DisassociateQueueQuickConnectsRequestRequestTypeDef",
     "DisassociateRoutingProfileQueuesRequestRequestTypeDef",
     "DisassociateSecurityKeyRequestRequestTypeDef",
     "DismissUserContactRequestRequestTypeDef",
+    "DistributionOutputTypeDef",
     "DistributionTypeDef",
-    "EmailReferenceTypeDef",
+    "EmailReferenceOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
+    "EvaluationAnswerDataOutputTypeDef",
     "EvaluationAnswerDataTypeDef",
     "EvaluationAnswerInputTypeDef",
-    "EvaluationAnswerOutputTypeDef",
-    "EvaluationFormContentTypeDef",
+    "EvaluationAnswerOutputOutputTypeDef",
+    "EvaluationFormContentOutputTypeDef",
+    "EvaluationFormItemOutputTypeDef",
     "EvaluationFormItemTypeDef",
+    "EvaluationFormNumericQuestionAutomationOutputTypeDef",
     "EvaluationFormNumericQuestionAutomationTypeDef",
+    "EvaluationFormNumericQuestionOptionOutputTypeDef",
     "EvaluationFormNumericQuestionOptionTypeDef",
+    "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
     "EvaluationFormNumericQuestionPropertiesTypeDef",
+    "EvaluationFormOutputTypeDef",
+    "EvaluationFormQuestionOutputTypeDef",
     "EvaluationFormQuestionTypeDef",
+    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
     "EvaluationFormQuestionTypePropertiesTypeDef",
+    "EvaluationFormScoringStrategyOutputTypeDef",
     "EvaluationFormScoringStrategyTypeDef",
+    "EvaluationFormSectionOutputTypeDef",
     "EvaluationFormSectionTypeDef",
+    "EvaluationFormSingleSelectQuestionAutomationOptionOutputTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationOptionTypeDef",
+    "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationTypeDef",
+    "EvaluationFormSingleSelectQuestionOptionOutputTypeDef",
     "EvaluationFormSingleSelectQuestionOptionTypeDef",
+    "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
     "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
-    "EvaluationFormSummaryTypeDef",
-    "EvaluationFormTypeDef",
-    "EvaluationFormVersionSummaryTypeDef",
-    "EvaluationMetadataTypeDef",
+    "EvaluationFormSummaryOutputTypeDef",
+    "EvaluationFormVersionSummaryOutputTypeDef",
+    "EvaluationMetadataOutputTypeDef",
+    "EvaluationNoteOutputTypeDef",
     "EvaluationNoteTypeDef",
-    "EvaluationScoreTypeDef",
-    "EvaluationSummaryTypeDef",
-    "EvaluationTypeDef",
+    "EvaluationOutputTypeDef",
+    "EvaluationScoreOutputTypeDef",
+    "EvaluationSummaryOutputTypeDef",
+    "EventBridgeActionDefinitionOutputTypeDef",
     "EventBridgeActionDefinitionTypeDef",
     "FilterV2TypeDef",
     "FiltersTypeDef",
     "GetContactAttributesRequestRequestTypeDef",
-    "GetContactAttributesResponseTypeDef",
+    "GetContactAttributesResponseOutputTypeDef",
     "GetCurrentMetricDataRequestRequestTypeDef",
-    "GetCurrentMetricDataResponseTypeDef",
+    "GetCurrentMetricDataResponseOutputTypeDef",
     "GetCurrentUserDataRequestRequestTypeDef",
-    "GetCurrentUserDataResponseTypeDef",
+    "GetCurrentUserDataResponseOutputTypeDef",
     "GetFederationTokenRequestRequestTypeDef",
-    "GetFederationTokenResponseTypeDef",
+    "GetFederationTokenResponseOutputTypeDef",
     "GetMetricDataRequestGetMetricDataPaginateTypeDef",
     "GetMetricDataRequestRequestTypeDef",
-    "GetMetricDataResponseTypeDef",
+    "GetMetricDataResponseOutputTypeDef",
     "GetMetricDataV2RequestRequestTypeDef",
-    "GetMetricDataV2ResponseTypeDef",
+    "GetMetricDataV2ResponseOutputTypeDef",
     "GetPromptFileRequestRequestTypeDef",
-    "GetPromptFileResponseTypeDef",
+    "GetPromptFileResponseOutputTypeDef",
     "GetTaskTemplateRequestRequestTypeDef",
-    "GetTaskTemplateResponseTypeDef",
+    "GetTaskTemplateResponseOutputTypeDef",
     "GetTrafficDistributionRequestRequestTypeDef",
-    "GetTrafficDistributionResponseTypeDef",
+    "GetTrafficDistributionResponseOutputTypeDef",
     "HierarchyGroupConditionTypeDef",
-    "HierarchyGroupSummaryReferenceTypeDef",
-    "HierarchyGroupSummaryTypeDef",
-    "HierarchyGroupTypeDef",
-    "HierarchyLevelTypeDef",
+    "HierarchyGroupOutputTypeDef",
+    "HierarchyGroupSummaryOutputTypeDef",
+    "HierarchyGroupSummaryReferenceOutputTypeDef",
+    "HierarchyLevelOutputTypeDef",
     "HierarchyLevelUpdateTypeDef",
-    "HierarchyPathReferenceTypeDef",
-    "HierarchyPathTypeDef",
-    "HierarchyStructureTypeDef",
+    "HierarchyPathOutputTypeDef",
+    "HierarchyPathReferenceOutputTypeDef",
+    "HierarchyStructureOutputTypeDef",
     "HierarchyStructureUpdateTypeDef",
-    "HistoricalMetricDataTypeDef",
-    "HistoricalMetricResultTypeDef",
+    "HistoricalMetricDataOutputTypeDef",
+    "HistoricalMetricOutputTypeDef",
+    "HistoricalMetricResultOutputTypeDef",
     "HistoricalMetricTypeDef",
+    "HoursOfOperationConfigOutputTypeDef",
     "HoursOfOperationConfigTypeDef",
+    "HoursOfOperationOutputTypeDef",
     "HoursOfOperationSearchCriteriaTypeDef",
     "HoursOfOperationSearchFilterTypeDef",
-    "HoursOfOperationSummaryTypeDef",
+    "HoursOfOperationSummaryOutputTypeDef",
+    "HoursOfOperationTimeSliceOutputTypeDef",
     "HoursOfOperationTimeSliceTypeDef",
-    "HoursOfOperationTypeDef",
-    "InstanceStatusReasonTypeDef",
+    "InstanceOutputTypeDef",
+    "InstanceStatusReasonOutputTypeDef",
+    "InstanceStorageConfigOutputTypeDef",
     "InstanceStorageConfigTypeDef",
-    "InstanceSummaryTypeDef",
-    "InstanceTypeDef",
-    "IntegrationAssociationSummaryTypeDef",
+    "InstanceSummaryOutputTypeDef",
+    "IntegrationAssociationSummaryOutputTypeDef",
+    "InvisibleFieldInfoOutputTypeDef",
     "InvisibleFieldInfoTypeDef",
+    "KinesisFirehoseConfigOutputTypeDef",
     "KinesisFirehoseConfigTypeDef",
+    "KinesisStreamConfigOutputTypeDef",
     "KinesisStreamConfigTypeDef",
+    "KinesisVideoStreamConfigOutputTypeDef",
     "KinesisVideoStreamConfigTypeDef",
-    "LexBotConfigTypeDef",
+    "LexBotConfigOutputTypeDef",
+    "LexBotOutputTypeDef",
     "LexBotTypeDef",
+    "LexV2BotOutputTypeDef",
     "LexV2BotTypeDef",
     "ListAgentStatusRequestListAgentStatusesPaginateTypeDef",
     "ListAgentStatusRequestRequestTypeDef",
-    "ListAgentStatusResponseTypeDef",
+    "ListAgentStatusResponseOutputTypeDef",
     "ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     "ListApprovedOriginsRequestRequestTypeDef",
-    "ListApprovedOriginsResponseTypeDef",
+    "ListApprovedOriginsResponseOutputTypeDef",
     "ListBotsRequestListBotsPaginateTypeDef",
     "ListBotsRequestRequestTypeDef",
-    "ListBotsResponseTypeDef",
+    "ListBotsResponseOutputTypeDef",
     "ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     "ListContactEvaluationsRequestRequestTypeDef",
-    "ListContactEvaluationsResponseTypeDef",
+    "ListContactEvaluationsResponseOutputTypeDef",
     "ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
     "ListContactFlowModulesRequestRequestTypeDef",
-    "ListContactFlowModulesResponseTypeDef",
+    "ListContactFlowModulesResponseOutputTypeDef",
     "ListContactFlowsRequestListContactFlowsPaginateTypeDef",
     "ListContactFlowsRequestRequestTypeDef",
-    "ListContactFlowsResponseTypeDef",
+    "ListContactFlowsResponseOutputTypeDef",
     "ListContactReferencesRequestListContactReferencesPaginateTypeDef",
     "ListContactReferencesRequestRequestTypeDef",
-    "ListContactReferencesResponseTypeDef",
+    "ListContactReferencesResponseOutputTypeDef",
     "ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef",
     "ListDefaultVocabulariesRequestRequestTypeDef",
-    "ListDefaultVocabulariesResponseTypeDef",
+    "ListDefaultVocabulariesResponseOutputTypeDef",
     "ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
     "ListEvaluationFormVersionsRequestRequestTypeDef",
-    "ListEvaluationFormVersionsResponseTypeDef",
+    "ListEvaluationFormVersionsResponseOutputTypeDef",
     "ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
     "ListEvaluationFormsRequestRequestTypeDef",
-    "ListEvaluationFormsResponseTypeDef",
+    "ListEvaluationFormsResponseOutputTypeDef",
     "ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
     "ListHoursOfOperationsRequestRequestTypeDef",
-    "ListHoursOfOperationsResponseTypeDef",
+    "ListHoursOfOperationsResponseOutputTypeDef",
     "ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
     "ListInstanceAttributesRequestRequestTypeDef",
-    "ListInstanceAttributesResponseTypeDef",
+    "ListInstanceAttributesResponseOutputTypeDef",
     "ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
     "ListInstanceStorageConfigsRequestRequestTypeDef",
-    "ListInstanceStorageConfigsResponseTypeDef",
+    "ListInstanceStorageConfigsResponseOutputTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
-    "ListInstancesResponseTypeDef",
+    "ListInstancesResponseOutputTypeDef",
     "ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef",
     "ListIntegrationAssociationsRequestRequestTypeDef",
-    "ListIntegrationAssociationsResponseTypeDef",
+    "ListIntegrationAssociationsResponseOutputTypeDef",
     "ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
     "ListLambdaFunctionsRequestRequestTypeDef",
-    "ListLambdaFunctionsResponseTypeDef",
+    "ListLambdaFunctionsResponseOutputTypeDef",
     "ListLexBotsRequestListLexBotsPaginateTypeDef",
     "ListLexBotsRequestRequestTypeDef",
-    "ListLexBotsResponseTypeDef",
+    "ListLexBotsResponseOutputTypeDef",
     "ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
-    "ListPhoneNumbersResponseTypeDef",
-    "ListPhoneNumbersSummaryTypeDef",
+    "ListPhoneNumbersResponseOutputTypeDef",
+    "ListPhoneNumbersSummaryOutputTypeDef",
     "ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef",
     "ListPhoneNumbersV2RequestRequestTypeDef",
-    "ListPhoneNumbersV2ResponseTypeDef",
+    "ListPhoneNumbersV2ResponseOutputTypeDef",
     "ListPromptsRequestListPromptsPaginateTypeDef",
     "ListPromptsRequestRequestTypeDef",
-    "ListPromptsResponseTypeDef",
+    "ListPromptsResponseOutputTypeDef",
     "ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
     "ListQueueQuickConnectsRequestRequestTypeDef",
-    "ListQueueQuickConnectsResponseTypeDef",
+    "ListQueueQuickConnectsResponseOutputTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "ListQueuesResponseTypeDef",
+    "ListQueuesResponseOutputTypeDef",
     "ListQuickConnectsRequestListQuickConnectsPaginateTypeDef",
     "ListQuickConnectsRequestRequestTypeDef",
-    "ListQuickConnectsResponseTypeDef",
+    "ListQuickConnectsResponseOutputTypeDef",
     "ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
     "ListRoutingProfileQueuesRequestRequestTypeDef",
-    "ListRoutingProfileQueuesResponseTypeDef",
+    "ListRoutingProfileQueuesResponseOutputTypeDef",
     "ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     "ListRoutingProfilesRequestRequestTypeDef",
-    "ListRoutingProfilesResponseTypeDef",
+    "ListRoutingProfilesResponseOutputTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
-    "ListRulesResponseTypeDef",
+    "ListRulesResponseOutputTypeDef",
     "ListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
     "ListSecurityKeysRequestRequestTypeDef",
-    "ListSecurityKeysResponseTypeDef",
+    "ListSecurityKeysResponseOutputTypeDef",
     "ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
     "ListSecurityProfilePermissionsRequestRequestTypeDef",
-    "ListSecurityProfilePermissionsResponseTypeDef",
+    "ListSecurityProfilePermissionsResponseOutputTypeDef",
     "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     "ListSecurityProfilesRequestRequestTypeDef",
-    "ListSecurityProfilesResponseTypeDef",
+    "ListSecurityProfilesResponseOutputTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
     "ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef",
     "ListTaskTemplatesRequestRequestTypeDef",
-    "ListTaskTemplatesResponseTypeDef",
+    "ListTaskTemplatesResponseOutputTypeDef",
     "ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef",
     "ListTrafficDistributionGroupsRequestRequestTypeDef",
-    "ListTrafficDistributionGroupsResponseTypeDef",
+    "ListTrafficDistributionGroupsResponseOutputTypeDef",
     "ListUseCasesRequestListUseCasesPaginateTypeDef",
     "ListUseCasesRequestRequestTypeDef",
-    "ListUseCasesResponseTypeDef",
+    "ListUseCasesResponseOutputTypeDef",
     "ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
     "ListUserHierarchyGroupsRequestRequestTypeDef",
-    "ListUserHierarchyGroupsResponseTypeDef",
+    "ListUserHierarchyGroupsResponseOutputTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
-    "ListUsersResponseTypeDef",
+    "ListUsersResponseOutputTypeDef",
+    "MediaConcurrencyOutputTypeDef",
     "MediaConcurrencyTypeDef",
-    "MetricDataV2TypeDef",
+    "MetricDataV2OutputTypeDef",
+    "MetricFilterV2OutputTypeDef",
     "MetricFilterV2TypeDef",
-    "MetricResultV2TypeDef",
+    "MetricResultV2OutputTypeDef",
+    "MetricV2OutputTypeDef",
     "MetricV2TypeDef",
     "MonitorContactRequestRequestTypeDef",
-    "MonitorContactResponseTypeDef",
+    "MonitorContactResponseOutputTypeDef",
+    "NotificationRecipientTypeOutputTypeDef",
     "NotificationRecipientTypeTypeDef",
-    "NumberReferenceTypeDef",
+    "NumberReferenceOutputTypeDef",
+    "NumericQuestionPropertyValueAutomationOutputTypeDef",
     "NumericQuestionPropertyValueAutomationTypeDef",
+    "OutboundCallerConfigOutputTypeDef",
     "OutboundCallerConfigTypeDef",
     "PaginatorConfigTypeDef",
     "ParticipantDetailsToAddTypeDef",
     "ParticipantDetailsTypeDef",
     "ParticipantTimerConfigurationTypeDef",
     "ParticipantTimerValueTypeDef",
-    "ParticipantTokenCredentialsTypeDef",
+    "ParticipantTokenCredentialsOutputTypeDef",
     "PersistentChatTypeDef",
+    "PhoneNumberQuickConnectConfigOutputTypeDef",
     "PhoneNumberQuickConnectConfigTypeDef",
-    "PhoneNumberStatusTypeDef",
-    "PhoneNumberSummaryTypeDef",
+    "PhoneNumberStatusOutputTypeDef",
+    "PhoneNumberSummaryOutputTypeDef",
+    "PromptOutputTypeDef",
     "PromptSearchCriteriaTypeDef",
     "PromptSearchFilterTypeDef",
-    "PromptSummaryTypeDef",
-    "PromptTypeDef",
+    "PromptSummaryOutputTypeDef",
     "PutUserStatusRequestRequestTypeDef",
-    "QueueInfoTypeDef",
+    "QueueInfoOutputTypeDef",
+    "QueueOutputTypeDef",
+    "QueueQuickConnectConfigOutputTypeDef",
     "QueueQuickConnectConfigTypeDef",
-    "QueueReferenceTypeDef",
+    "QueueReferenceOutputTypeDef",
     "QueueSearchCriteriaTypeDef",
     "QueueSearchFilterTypeDef",
-    "QueueSummaryTypeDef",
-    "QueueTypeDef",
+    "QueueSummaryOutputTypeDef",
+    "QuickConnectConfigOutputTypeDef",
     "QuickConnectConfigTypeDef",
+    "QuickConnectOutputTypeDef",
     "QuickConnectSearchCriteriaTypeDef",
     "QuickConnectSearchFilterTypeDef",
-    "QuickConnectSummaryTypeDef",
-    "QuickConnectTypeDef",
+    "QuickConnectSummaryOutputTypeDef",
+    "ReadOnlyFieldInfoOutputTypeDef",
     "ReadOnlyFieldInfoTypeDef",
-    "ReferenceSummaryTypeDef",
+    "ReferenceOutputTypeDef",
+    "ReferenceSummaryOutputTypeDef",
     "ReferenceTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
     "ReplicateInstanceRequestRequestTypeDef",
-    "ReplicateInstanceResponseTypeDef",
+    "ReplicateInstanceResponseOutputTypeDef",
+    "RequiredFieldInfoOutputTypeDef",
     "RequiredFieldInfoTypeDef",
     "ResourceTagsSearchCriteriaTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeContactRecordingRequestRequestTypeDef",
-    "RoutingProfileQueueConfigSummaryTypeDef",
+    "RoutingProfileOutputTypeDef",
+    "RoutingProfileQueueConfigSummaryOutputTypeDef",
     "RoutingProfileQueueConfigTypeDef",
     "RoutingProfileQueueReferenceTypeDef",
-    "RoutingProfileReferenceTypeDef",
+    "RoutingProfileReferenceOutputTypeDef",
     "RoutingProfileSearchCriteriaTypeDef",
     "RoutingProfileSearchFilterTypeDef",
-    "RoutingProfileSummaryTypeDef",
-    "RoutingProfileTypeDef",
+    "RoutingProfileSummaryOutputTypeDef",
+    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
-    "RuleSummaryTypeDef",
+    "RuleOutputTypeDef",
+    "RuleSummaryOutputTypeDef",
+    "RuleTriggerEventSourceOutputTypeDef",
     "RuleTriggerEventSourceTypeDef",
-    "RuleTypeDef",
+    "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
+    "SearchAvailablePhoneNumbersResponseOutputTypeDef",
     "SearchHoursOfOperationsRequestRequestTypeDef",
     "SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef",
-    "SearchHoursOfOperationsResponseTypeDef",
+    "SearchHoursOfOperationsResponseOutputTypeDef",
     "SearchPromptsRequestRequestTypeDef",
     "SearchPromptsRequestSearchPromptsPaginateTypeDef",
-    "SearchPromptsResponseTypeDef",
+    "SearchPromptsResponseOutputTypeDef",
     "SearchQueuesRequestRequestTypeDef",
     "SearchQueuesRequestSearchQueuesPaginateTypeDef",
-    "SearchQueuesResponseTypeDef",
+    "SearchQueuesResponseOutputTypeDef",
     "SearchQuickConnectsRequestRequestTypeDef",
     "SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef",
-    "SearchQuickConnectsResponseTypeDef",
+    "SearchQuickConnectsResponseOutputTypeDef",
     "SearchResourceTagsRequestRequestTypeDef",
     "SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
-    "SearchResourceTagsResponseTypeDef",
+    "SearchResourceTagsResponseOutputTypeDef",
     "SearchRoutingProfilesRequestRequestTypeDef",
     "SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef",
-    "SearchRoutingProfilesResponseTypeDef",
+    "SearchRoutingProfilesResponseOutputTypeDef",
     "SearchSecurityProfilesRequestRequestTypeDef",
     "SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef",
-    "SearchSecurityProfilesResponseTypeDef",
+    "SearchSecurityProfilesResponseOutputTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchUsersRequestSearchUsersPaginateTypeDef",
-    "SearchUsersResponseTypeDef",
+    "SearchUsersResponseOutputTypeDef",
     "SearchVocabulariesRequestRequestTypeDef",
     "SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef",
-    "SearchVocabulariesResponseTypeDef",
-    "SecurityKeyTypeDef",
+    "SearchVocabulariesResponseOutputTypeDef",
+    "SecurityKeyOutputTypeDef",
+    "SecurityProfileOutputTypeDef",
     "SecurityProfileSearchCriteriaTypeDef",
-    "SecurityProfileSearchSummaryTypeDef",
-    "SecurityProfileSummaryTypeDef",
-    "SecurityProfileTypeDef",
+    "SecurityProfileSearchSummaryOutputTypeDef",
+    "SecurityProfileSummaryOutputTypeDef",
     "SecurityProfilesSearchFilterTypeDef",
+    "SendNotificationActionDefinitionOutputTypeDef",
     "SendNotificationActionDefinitionTypeDef",
+    "SingleSelectQuestionRuleCategoryAutomationOutputTypeDef",
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     "StartChatContactRequestRequestTypeDef",
-    "StartChatContactResponseTypeDef",
+    "StartChatContactResponseOutputTypeDef",
     "StartContactEvaluationRequestRequestTypeDef",
-    "StartContactEvaluationResponseTypeDef",
+    "StartContactEvaluationResponseOutputTypeDef",
     "StartContactRecordingRequestRequestTypeDef",
     "StartContactStreamingRequestRequestTypeDef",
-    "StartContactStreamingResponseTypeDef",
+    "StartContactStreamingResponseOutputTypeDef",
     "StartOutboundVoiceContactRequestRequestTypeDef",
-    "StartOutboundVoiceContactResponseTypeDef",
+    "StartOutboundVoiceContactResponseOutputTypeDef",
     "StartTaskContactRequestRequestTypeDef",
-    "StartTaskContactResponseTypeDef",
+    "StartTaskContactResponseOutputTypeDef",
     "StopContactRecordingRequestRequestTypeDef",
     "StopContactRequestRequestTypeDef",
     "StopContactStreamingRequestRequestTypeDef",
     "StringConditionTypeDef",
-    "StringReferenceTypeDef",
+    "StringReferenceOutputTypeDef",
     "SubmitContactEvaluationRequestRequestTypeDef",
-    "SubmitContactEvaluationResponseTypeDef",
+    "SubmitContactEvaluationResponseOutputTypeDef",
     "SuspendContactRecordingRequestRequestTypeDef",
     "TagConditionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TagSearchConditionTypeDef",
-    "TagSetTypeDef",
+    "TagSetOutputTypeDef",
+    "TaskActionDefinitionOutputTypeDef",
     "TaskActionDefinitionTypeDef",
+    "TaskTemplateConstraintsOutputTypeDef",
     "TaskTemplateConstraintsTypeDef",
+    "TaskTemplateDefaultFieldValueOutputTypeDef",
     "TaskTemplateDefaultFieldValueTypeDef",
+    "TaskTemplateDefaultsOutputTypeDef",
     "TaskTemplateDefaultsTypeDef",
+    "TaskTemplateFieldIdentifierOutputTypeDef",
     "TaskTemplateFieldIdentifierTypeDef",
+    "TaskTemplateFieldOutputTypeDef",
     "TaskTemplateFieldTypeDef",
-    "TaskTemplateMetadataTypeDef",
+    "TaskTemplateMetadataOutputTypeDef",
+    "TelephonyConfigOutputTypeDef",
     "TelephonyConfigTypeDef",
+    "ThresholdOutputTypeDef",
     "ThresholdTypeDef",
+    "ThresholdV2OutputTypeDef",
     "ThresholdV2TypeDef",
-    "TrafficDistributionGroupSummaryTypeDef",
-    "TrafficDistributionGroupTypeDef",
+    "TrafficDistributionGroupOutputTypeDef",
+    "TrafficDistributionGroupSummaryOutputTypeDef",
     "TransferContactRequestRequestTypeDef",
-    "TransferContactResponseTypeDef",
+    "TransferContactResponseOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
     "UpdateContactAttributesRequestRequestTypeDef",
     "UpdateContactEvaluationRequestRequestTypeDef",
-    "UpdateContactEvaluationResponseTypeDef",
+    "UpdateContactEvaluationResponseOutputTypeDef",
     "UpdateContactFlowContentRequestRequestTypeDef",
     "UpdateContactFlowMetadataRequestRequestTypeDef",
     "UpdateContactFlowModuleContentRequestRequestTypeDef",
     "UpdateContactFlowModuleMetadataRequestRequestTypeDef",
     "UpdateContactFlowNameRequestRequestTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "UpdateContactScheduleRequestRequestTypeDef",
     "UpdateEvaluationFormRequestRequestTypeDef",
-    "UpdateEvaluationFormResponseTypeDef",
+    "UpdateEvaluationFormResponseOutputTypeDef",
     "UpdateHoursOfOperationRequestRequestTypeDef",
     "UpdateInstanceAttributeRequestRequestTypeDef",
     "UpdateInstanceStorageConfigRequestRequestTypeDef",
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
-    "UpdatePhoneNumberResponseTypeDef",
+    "UpdatePhoneNumberResponseOutputTypeDef",
     "UpdatePromptRequestRequestTypeDef",
-    "UpdatePromptResponseTypeDef",
+    "UpdatePromptResponseOutputTypeDef",
     "UpdateQueueHoursOfOperationRequestRequestTypeDef",
     "UpdateQueueMaxContactsRequestRequestTypeDef",
     "UpdateQueueNameRequestRequestTypeDef",
     "UpdateQueueOutboundCallerConfigRequestRequestTypeDef",
     "UpdateQueueStatusRequestRequestTypeDef",
     "UpdateQuickConnectConfigRequestRequestTypeDef",
     "UpdateQuickConnectNameRequestRequestTypeDef",
     "UpdateRoutingProfileConcurrencyRequestRequestTypeDef",
     "UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef",
     "UpdateRoutingProfileNameRequestRequestTypeDef",
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "UpdateSecurityProfileRequestRequestTypeDef",
     "UpdateTaskTemplateRequestRequestTypeDef",
-    "UpdateTaskTemplateResponseTypeDef",
+    "UpdateTaskTemplateResponseOutputTypeDef",
     "UpdateTrafficDistributionRequestRequestTypeDef",
     "UpdateUserHierarchyGroupNameRequestRequestTypeDef",
     "UpdateUserHierarchyRequestRequestTypeDef",
     "UpdateUserHierarchyStructureRequestRequestTypeDef",
     "UpdateUserIdentityInfoRequestRequestTypeDef",
     "UpdateUserPhoneConfigRequestRequestTypeDef",
     "UpdateUserRoutingProfileRequestRequestTypeDef",
     "UpdateUserSecurityProfilesRequestRequestTypeDef",
-    "UrlReferenceTypeDef",
-    "UseCaseTypeDef",
+    "UrlReferenceOutputTypeDef",
+    "UseCaseOutputTypeDef",
     "UserDataFiltersTypeDef",
-    "UserDataTypeDef",
-    "UserIdentityInfoLiteTypeDef",
+    "UserDataOutputTypeDef",
+    "UserIdentityInfoLiteOutputTypeDef",
+    "UserIdentityInfoOutputTypeDef",
     "UserIdentityInfoTypeDef",
+    "UserOutputTypeDef",
+    "UserPhoneConfigOutputTypeDef",
     "UserPhoneConfigTypeDef",
+    "UserQuickConnectConfigOutputTypeDef",
     "UserQuickConnectConfigTypeDef",
-    "UserReferenceTypeDef",
+    "UserReferenceOutputTypeDef",
     "UserSearchCriteriaTypeDef",
     "UserSearchFilterTypeDef",
-    "UserSearchSummaryTypeDef",
-    "UserSummaryTypeDef",
-    "UserTypeDef",
-    "VocabularySummaryTypeDef",
-    "VocabularyTypeDef",
+    "UserSearchSummaryOutputTypeDef",
+    "UserSummaryOutputTypeDef",
+    "VocabularyOutputTypeDef",
+    "VocabularySummaryOutputTypeDef",
     "VoiceRecordingConfigurationTypeDef",
-    "WisdomInfoTypeDef",
+    "WisdomInfoOutputTypeDef",
 )
 
-ActionSummaryTypeDef = TypedDict(
-    "ActionSummaryTypeDef",
+ActionSummaryOutputTypeDef = TypedDict(
+    "ActionSummaryOutputTypeDef",
     {
         "ActionType": ActionTypeType,
     },
 )
 
 ActivateEvaluationFormRequestRequestTypeDef = TypedDict(
     "ActivateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
     },
 )
 
-ActivateEvaluationFormResponseTypeDef = TypedDict(
-    "ActivateEvaluationFormResponseTypeDef",
+ActivateEvaluationFormResponseOutputTypeDef = TypedDict(
+    "ActivateEvaluationFormResponseOutputTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AgentContactReferenceTypeDef = TypedDict(
-    "AgentContactReferenceTypeDef",
+AgentContactReferenceOutputTypeDef = TypedDict(
+    "AgentContactReferenceOutputTypeDef",
     {
         "ContactId": str,
         "Channel": ChannelType,
         "InitiationMethod": ContactInitiationMethodType,
         "AgentContactState": ContactStateType,
         "StateStartTimestamp": datetime,
         "ConnectedToAgentTimestamp": datetime,
-        "Queue": "QueueReferenceTypeDef",
+        "Queue": "QueueReferenceOutputTypeDef",
     },
 )
 
-AgentInfoTypeDef = TypedDict(
-    "AgentInfoTypeDef",
+AgentInfoOutputTypeDef = TypedDict(
+    "AgentInfoOutputTypeDef",
     {
         "Id": str,
         "ConnectedToAgentTimestamp": datetime,
     },
 )
 
-AgentStatusReferenceTypeDef = TypedDict(
-    "AgentStatusReferenceTypeDef",
+AgentStatusOutputTypeDef = TypedDict(
+    "AgentStatusOutputTypeDef",
+    {
+        "AgentStatusARN": str,
+        "AgentStatusId": str,
+        "Name": str,
+        "Description": str,
+        "Type": AgentStatusTypeType,
+        "DisplayOrder": int,
+        "State": AgentStatusStateType,
+        "Tags": Dict[str, str],
+    },
+)
+
+AgentStatusReferenceOutputTypeDef = TypedDict(
+    "AgentStatusReferenceOutputTypeDef",
     {
         "StatusStartTimestamp": datetime,
         "StatusArn": str,
         "StatusName": str,
     },
 )
 
-AgentStatusSummaryTypeDef = TypedDict(
-    "AgentStatusSummaryTypeDef",
+AgentStatusSummaryOutputTypeDef = TypedDict(
+    "AgentStatusSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": AgentStatusTypeType,
     },
 )
 
-AgentStatusTypeDef = TypedDict(
-    "AgentStatusTypeDef",
-    {
-        "AgentStatusARN": str,
-        "AgentStatusId": str,
-        "Name": str,
-        "Description": str,
-        "Type": AgentStatusTypeType,
-        "DisplayOrder": int,
-        "State": AgentStatusStateType,
-        "Tags": Dict[str, str],
-    },
-)
-
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "EnableAnswerMachineDetection": bool,
         "AwaitAnswerMachinePrompt": bool,
     },
     total=False,
@@ -746,19 +805,21 @@
     {
         "LexBot": "LexBotTypeDef",
         "LexV2Bot": "LexV2BotTypeDef",
     },
     total=False,
 )
 
+
 class AssociateBotRequestRequestTypeDef(
     _RequiredAssociateBotRequestRequestTypeDef, _OptionalAssociateBotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAssociateDefaultVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateDefaultVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LanguageCode": VocabularyLanguageCodeType,
     },
 )
@@ -766,31 +827,33 @@
     "_OptionalAssociateDefaultVocabularyRequestRequestTypeDef",
     {
         "VocabularyId": str,
     },
     total=False,
 )
 
+
 class AssociateDefaultVocabularyRequestRequestTypeDef(
     _RequiredAssociateDefaultVocabularyRequestRequestTypeDef,
     _OptionalAssociateDefaultVocabularyRequestRequestTypeDef,
 ):
     pass
 
+
 AssociateInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
         "StorageConfig": "InstanceStorageConfigTypeDef",
     },
 )
 
-AssociateInstanceStorageConfigResponseTypeDef = TypedDict(
-    "AssociateInstanceStorageConfigResponseTypeDef",
+AssociateInstanceStorageConfigResponseOutputTypeDef = TypedDict(
+    "AssociateInstanceStorageConfigResponseOutputTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateLambdaFunctionRequestRequestTypeDef = TypedDict(
@@ -840,41 +903,41 @@
     "AssociateSecurityKeyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Key": str,
     },
 )
 
-AssociateSecurityKeyResponseTypeDef = TypedDict(
-    "AssociateSecurityKeyResponseTypeDef",
+AssociateSecurityKeyResponseOutputTypeDef = TypedDict(
+    "AssociateSecurityKeyResponseOutputTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachmentReferenceTypeDef = TypedDict(
-    "AttachmentReferenceTypeDef",
+AttachmentReferenceOutputTypeDef = TypedDict(
+    "AttachmentReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
         "Status": ReferenceStatusType,
     },
 )
 
-AttributeTypeDef = TypedDict(
-    "AttributeTypeDef",
+AttributeOutputTypeDef = TypedDict(
+    "AttributeOutputTypeDef",
     {
         "AttributeType": InstanceAttributeTypeType,
         "Value": str,
     },
 )
 
-AvailableNumberSummaryTypeDef = TypedDict(
-    "AvailableNumberSummaryTypeDef",
+AvailableNumberSummaryOutputTypeDef = TypedDict(
+    "AvailableNumberSummaryOutputTypeDef",
     {
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
 )
 
@@ -913,119 +976,121 @@
         "PhoneNumberDescription": str,
         "Tags": Mapping[str, str],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class ClaimPhoneNumberRequestRequestTypeDef(
     _RequiredClaimPhoneNumberRequestRequestTypeDef, _OptionalClaimPhoneNumberRequestRequestTypeDef
 ):
     pass
 
-ClaimPhoneNumberResponseTypeDef = TypedDict(
-    "ClaimPhoneNumberResponseTypeDef",
+
+ClaimPhoneNumberResponseOutputTypeDef = TypedDict(
+    "ClaimPhoneNumberResponseOutputTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ClaimedPhoneNumberSummaryTypeDef = TypedDict(
-    "ClaimedPhoneNumberSummaryTypeDef",
+ClaimedPhoneNumberSummaryOutputTypeDef = TypedDict(
+    "ClaimedPhoneNumberSummaryOutputTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberDescription": str,
         "TargetArn": str,
         "Tags": Dict[str, str],
-        "PhoneNumberStatus": "PhoneNumberStatusTypeDef",
+        "PhoneNumberStatus": "PhoneNumberStatusOutputTypeDef",
     },
 )
 
 ContactFilterTypeDef = TypedDict(
     "ContactFilterTypeDef",
     {
         "ContactStates": Sequence[ContactStateType],
     },
     total=False,
 )
 
-ContactFlowModuleSummaryTypeDef = TypedDict(
-    "ContactFlowModuleSummaryTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "State": ContactFlowModuleStateType,
-    },
-)
-
-ContactFlowModuleTypeDef = TypedDict(
-    "ContactFlowModuleTypeDef",
+ContactFlowModuleOutputTypeDef = TypedDict(
+    "ContactFlowModuleOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Content": str,
         "Description": str,
         "State": ContactFlowModuleStateType,
         "Status": ContactFlowModuleStatusType,
         "Tags": Dict[str, str],
     },
 )
 
-ContactFlowSummaryTypeDef = TypedDict(
-    "ContactFlowSummaryTypeDef",
+ContactFlowModuleSummaryOutputTypeDef = TypedDict(
+    "ContactFlowModuleSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
-        "ContactFlowType": ContactFlowTypeType,
-        "ContactFlowState": ContactFlowStateType,
+        "State": ContactFlowModuleStateType,
     },
 )
 
-ContactFlowTypeDef = TypedDict(
-    "ContactFlowTypeDef",
+ContactFlowOutputTypeDef = TypedDict(
+    "ContactFlowOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Type": ContactFlowTypeType,
         "State": ContactFlowStateType,
         "Description": str,
         "Content": str,
         "Tags": Dict[str, str],
     },
 )
 
-ContactTypeDef = TypedDict(
-    "ContactTypeDef",
+ContactFlowSummaryOutputTypeDef = TypedDict(
+    "ContactFlowSummaryOutputTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "ContactFlowType": ContactFlowTypeType,
+        "ContactFlowState": ContactFlowStateType,
+    },
+)
+
+ContactOutputTypeDef = TypedDict(
+    "ContactOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "InitialContactId": str,
         "PreviousContactId": str,
         "InitiationMethod": ContactInitiationMethodType,
         "Name": str,
         "Description": str,
         "Channel": ChannelType,
-        "QueueInfo": "QueueInfoTypeDef",
-        "AgentInfo": "AgentInfoTypeDef",
+        "QueueInfo": "QueueInfoOutputTypeDef",
+        "AgentInfo": "AgentInfoOutputTypeDef",
         "InitiationTimestamp": datetime,
         "DisconnectTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "ScheduledTimestamp": datetime,
         "RelatedContactId": str,
-        "WisdomInfo": "WisdomInfoTypeDef",
+        "WisdomInfo": "WisdomInfoOutputTypeDef",
     },
 )
 
 ControlPlaneTagFilterTypeDef = TypedDict(
     "ControlPlaneTagFilterTypeDef",
     {
         "OrConditions": Sequence[Sequence["TagConditionTypeDef"]],
@@ -1049,21 +1114,23 @@
         "Description": str,
         "DisplayOrder": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAgentStatusRequestRequestTypeDef(
     _RequiredCreateAgentStatusRequestRequestTypeDef, _OptionalCreateAgentStatusRequestRequestTypeDef
 ):
     pass
 
-CreateAgentStatusResponseTypeDef = TypedDict(
-    "CreateAgentStatusResponseTypeDef",
+
+CreateAgentStatusResponseOutputTypeDef = TypedDict(
+    "CreateAgentStatusResponseOutputTypeDef",
     {
         "AgentStatusARN": str,
         "AgentStatusId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1081,22 +1148,24 @@
         "Description": str,
         "Tags": Mapping[str, str],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateContactFlowModuleRequestRequestTypeDef(
     _RequiredCreateContactFlowModuleRequestRequestTypeDef,
     _OptionalCreateContactFlowModuleRequestRequestTypeDef,
 ):
     pass
 
-CreateContactFlowModuleResponseTypeDef = TypedDict(
-    "CreateContactFlowModuleResponseTypeDef",
+
+CreateContactFlowModuleResponseOutputTypeDef = TypedDict(
+    "CreateContactFlowModuleResponseOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1114,21 +1183,23 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateContactFlowRequestRequestTypeDef(
     _RequiredCreateContactFlowRequestRequestTypeDef, _OptionalCreateContactFlowRequestRequestTypeDef
 ):
     pass
 
-CreateContactFlowResponseTypeDef = TypedDict(
-    "CreateContactFlowResponseTypeDef",
+
+CreateContactFlowResponseOutputTypeDef = TypedDict(
+    "CreateContactFlowResponseOutputTypeDef",
     {
         "ContactFlowId": str,
         "ContactFlowArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1146,22 +1217,24 @@
         "Description": str,
         "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateEvaluationFormRequestRequestTypeDef(
     _RequiredCreateEvaluationFormRequestRequestTypeDef,
     _OptionalCreateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-CreateEvaluationFormResponseTypeDef = TypedDict(
-    "CreateEvaluationFormResponseTypeDef",
+
+CreateEvaluationFormResponseOutputTypeDef = TypedDict(
+    "CreateEvaluationFormResponseOutputTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1179,22 +1252,24 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateHoursOfOperationRequestRequestTypeDef(
     _RequiredCreateHoursOfOperationRequestRequestTypeDef,
     _OptionalCreateHoursOfOperationRequestRequestTypeDef,
 ):
     pass
 
-CreateHoursOfOperationResponseTypeDef = TypedDict(
-    "CreateHoursOfOperationResponseTypeDef",
+
+CreateHoursOfOperationResponseOutputTypeDef = TypedDict(
+    "CreateHoursOfOperationResponseOutputTypeDef",
     {
         "HoursOfOperationId": str,
         "HoursOfOperationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1212,21 +1287,23 @@
         "ClientToken": str,
         "InstanceAlias": str,
         "DirectoryId": str,
     },
     total=False,
 )
 
+
 class CreateInstanceRequestRequestTypeDef(
     _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
 ):
     pass
 
-CreateInstanceResponseTypeDef = TypedDict(
-    "CreateInstanceResponseTypeDef",
+
+CreateInstanceResponseOutputTypeDef = TypedDict(
+    "CreateInstanceResponseOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1245,22 +1322,24 @@
         "SourceApplicationName": str,
         "SourceType": SourceTypeType,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateIntegrationAssociationRequestRequestTypeDef(
     _RequiredCreateIntegrationAssociationRequestRequestTypeDef,
     _OptionalCreateIntegrationAssociationRequestRequestTypeDef,
 ):
     pass
 
-CreateIntegrationAssociationResponseTypeDef = TypedDict(
-    "CreateIntegrationAssociationResponseTypeDef",
+
+CreateIntegrationAssociationResponseOutputTypeDef = TypedDict(
+    "CreateIntegrationAssociationResponseOutputTypeDef",
     {
         "IntegrationAssociationId": str,
         "IntegrationAssociationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1276,23 +1355,25 @@
     "_OptionalCreateParticipantRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateParticipantRequestRequestTypeDef(
     _RequiredCreateParticipantRequestRequestTypeDef, _OptionalCreateParticipantRequestRequestTypeDef
 ):
     pass
 
-CreateParticipantResponseTypeDef = TypedDict(
-    "CreateParticipantResponseTypeDef",
+
+CreateParticipantResponseOutputTypeDef = TypedDict(
+    "CreateParticipantResponseOutputTypeDef",
     {
-        "ParticipantCredentials": "ParticipantTokenCredentialsTypeDef",
+        "ParticipantCredentials": "ParticipantTokenCredentialsOutputTypeDef",
         "ParticipantId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePromptRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePromptRequestRequestTypeDef",
@@ -1307,21 +1388,23 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreatePromptRequestRequestTypeDef(
     _RequiredCreatePromptRequestRequestTypeDef, _OptionalCreatePromptRequestRequestTypeDef
 ):
     pass
 
-CreatePromptResponseTypeDef = TypedDict(
-    "CreatePromptResponseTypeDef",
+
+CreatePromptResponseOutputTypeDef = TypedDict(
+    "CreatePromptResponseOutputTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1341,21 +1424,23 @@
         "MaxContacts": int,
         "QuickConnectIds": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateQueueRequestRequestTypeDef(
     _RequiredCreateQueueRequestRequestTypeDef, _OptionalCreateQueueRequestRequestTypeDef
 ):
     pass
 
-CreateQueueResponseTypeDef = TypedDict(
-    "CreateQueueResponseTypeDef",
+
+CreateQueueResponseOutputTypeDef = TypedDict(
+    "CreateQueueResponseOutputTypeDef",
     {
         "QueueArn": str,
         "QueueId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1372,22 +1457,24 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateQuickConnectRequestRequestTypeDef(
     _RequiredCreateQuickConnectRequestRequestTypeDef,
     _OptionalCreateQuickConnectRequestRequestTypeDef,
 ):
     pass
 
-CreateQuickConnectResponseTypeDef = TypedDict(
-    "CreateQuickConnectResponseTypeDef",
+
+CreateQuickConnectResponseOutputTypeDef = TypedDict(
+    "CreateQuickConnectResponseOutputTypeDef",
     {
         "QuickConnectARN": str,
         "QuickConnectId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1406,22 +1493,24 @@
     {
         "QueueConfigs": Sequence["RoutingProfileQueueConfigTypeDef"],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateRoutingProfileRequestRequestTypeDef(
     _RequiredCreateRoutingProfileRequestRequestTypeDef,
     _OptionalCreateRoutingProfileRequestRequestTypeDef,
 ):
     pass
 
-CreateRoutingProfileResponseTypeDef = TypedDict(
-    "CreateRoutingProfileResponseTypeDef",
+
+CreateRoutingProfileResponseOutputTypeDef = TypedDict(
+    "CreateRoutingProfileResponseOutputTypeDef",
     {
         "RoutingProfileArn": str,
         "RoutingProfileId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1440,21 +1529,23 @@
     "_OptionalCreateRuleRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateRuleRequestRequestTypeDef(
     _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
 ):
     pass
 
-CreateRuleResponseTypeDef = TypedDict(
-    "CreateRuleResponseTypeDef",
+
+CreateRuleResponseOutputTypeDef = TypedDict(
+    "CreateRuleResponseOutputTypeDef",
     {
         "RuleArn": str,
         "RuleId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1473,22 +1564,24 @@
         "Tags": Mapping[str, str],
         "AllowedAccessControlTags": Mapping[str, str],
         "TagRestrictedResources": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateSecurityProfileRequestRequestTypeDef(
     _RequiredCreateSecurityProfileRequestRequestTypeDef,
     _OptionalCreateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
-CreateSecurityProfileResponseTypeDef = TypedDict(
-    "CreateSecurityProfileResponseTypeDef",
+
+CreateSecurityProfileResponseOutputTypeDef = TypedDict(
+    "CreateSecurityProfileResponseOutputTypeDef",
     {
         "SecurityProfileId": str,
         "SecurityProfileArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1509,22 +1602,24 @@
         "Defaults": "TaskTemplateDefaultsTypeDef",
         "Status": TaskTemplateStatusType,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateTaskTemplateRequestRequestTypeDef(
     _RequiredCreateTaskTemplateRequestRequestTypeDef,
     _OptionalCreateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
-CreateTaskTemplateResponseTypeDef = TypedDict(
-    "CreateTaskTemplateResponseTypeDef",
+
+CreateTaskTemplateResponseOutputTypeDef = TypedDict(
+    "CreateTaskTemplateResponseOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1541,22 +1636,24 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateTrafficDistributionGroupRequestRequestTypeDef(
     _RequiredCreateTrafficDistributionGroupRequestRequestTypeDef,
     _OptionalCreateTrafficDistributionGroupRequestRequestTypeDef,
 ):
     pass
 
-CreateTrafficDistributionGroupResponseTypeDef = TypedDict(
-    "CreateTrafficDistributionGroupResponseTypeDef",
+
+CreateTrafficDistributionGroupResponseOutputTypeDef = TypedDict(
+    "CreateTrafficDistributionGroupResponseOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1572,21 +1669,23 @@
     "_OptionalCreateUseCaseRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateUseCaseRequestRequestTypeDef(
     _RequiredCreateUseCaseRequestRequestTypeDef, _OptionalCreateUseCaseRequestRequestTypeDef
 ):
     pass
 
-CreateUseCaseResponseTypeDef = TypedDict(
-    "CreateUseCaseResponseTypeDef",
+
+CreateUseCaseResponseOutputTypeDef = TypedDict(
+    "CreateUseCaseResponseOutputTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1602,22 +1701,24 @@
     {
         "ParentGroupId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateUserHierarchyGroupRequestRequestTypeDef(
     _RequiredCreateUserHierarchyGroupRequestRequestTypeDef,
     _OptionalCreateUserHierarchyGroupRequestRequestTypeDef,
 ):
     pass
 
-CreateUserHierarchyGroupResponseTypeDef = TypedDict(
-    "CreateUserHierarchyGroupResponseTypeDef",
+
+CreateUserHierarchyGroupResponseOutputTypeDef = TypedDict(
+    "CreateUserHierarchyGroupResponseOutputTypeDef",
     {
         "HierarchyGroupId": str,
         "HierarchyGroupArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1639,21 +1740,23 @@
         "DirectoryUserId": str,
         "HierarchyGroupId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
+
+CreateUserResponseOutputTypeDef = TypedDict(
+    "CreateUserResponseOutputTypeDef",
     {
         "UserId": str,
         "UserArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1671,59 +1774,76 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
-CreateVocabularyResponseTypeDef = TypedDict(
-    "CreateVocabularyResponseTypeDef",
+
+CreateVocabularyResponseOutputTypeDef = TypedDict(
+    "CreateVocabularyResponseOutputTypeDef",
     {
         "VocabularyArn": str,
         "VocabularyId": str,
         "State": VocabularyStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CredentialsTypeDef = TypedDict(
-    "CredentialsTypeDef",
+CredentialsOutputTypeDef = TypedDict(
+    "CredentialsOutputTypeDef",
     {
         "AccessToken": str,
         "AccessTokenExpiration": datetime,
         "RefreshToken": str,
         "RefreshTokenExpiration": datetime,
     },
 )
 
+CrossChannelBehaviorOutputTypeDef = TypedDict(
+    "CrossChannelBehaviorOutputTypeDef",
+    {
+        "BehaviorType": BehaviorTypeType,
+    },
+)
+
 CrossChannelBehaviorTypeDef = TypedDict(
     "CrossChannelBehaviorTypeDef",
     {
         "BehaviorType": BehaviorTypeType,
     },
 )
 
-CurrentMetricDataTypeDef = TypedDict(
-    "CurrentMetricDataTypeDef",
+CurrentMetricDataOutputTypeDef = TypedDict(
+    "CurrentMetricDataOutputTypeDef",
     {
-        "Metric": "CurrentMetricTypeDef",
+        "Metric": "CurrentMetricOutputTypeDef",
         "Value": float,
     },
 )
 
-CurrentMetricResultTypeDef = TypedDict(
-    "CurrentMetricResultTypeDef",
+CurrentMetricOutputTypeDef = TypedDict(
+    "CurrentMetricOutputTypeDef",
     {
-        "Dimensions": "DimensionsTypeDef",
-        "Collections": List["CurrentMetricDataTypeDef"],
+        "Name": CurrentMetricNameType,
+        "Unit": UnitType,
+    },
+)
+
+CurrentMetricResultOutputTypeDef = TypedDict(
+    "CurrentMetricResultOutputTypeDef",
+    {
+        "Dimensions": "DimensionsOutputTypeDef",
+        "Collections": List["CurrentMetricDataOutputTypeDef"],
     },
 )
 
 CurrentMetricSortCriteriaTypeDef = TypedDict(
     "CurrentMetricSortCriteriaTypeDef",
     {
         "SortByMetric": CurrentMetricNameType,
@@ -1737,16 +1857,16 @@
     {
         "Name": CurrentMetricNameType,
         "Unit": UnitType,
     },
     total=False,
 )
 
-DateReferenceTypeDef = TypedDict(
-    "DateReferenceTypeDef",
+DateReferenceOutputTypeDef = TypedDict(
+    "DateReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 DeactivateEvaluationFormRequestRequestTypeDef = TypedDict(
@@ -1754,26 +1874,26 @@
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
     },
 )
 
-DeactivateEvaluationFormResponseTypeDef = TypedDict(
-    "DeactivateEvaluationFormResponseTypeDef",
+DeactivateEvaluationFormResponseOutputTypeDef = TypedDict(
+    "DeactivateEvaluationFormResponseOutputTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DefaultVocabularyTypeDef = TypedDict(
-    "DefaultVocabularyTypeDef",
+DefaultVocabularyOutputTypeDef = TypedDict(
+    "DefaultVocabularyOutputTypeDef",
     {
         "InstanceId": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "VocabularyId": str,
         "VocabularyName": str,
     },
 )
@@ -1813,20 +1933,22 @@
     "_OptionalDeleteEvaluationFormRequestRequestTypeDef",
     {
         "EvaluationFormVersion": int,
     },
     total=False,
 )
 
+
 class DeleteEvaluationFormRequestRequestTypeDef(
     _RequiredDeleteEvaluationFormRequestRequestTypeDef,
     _OptionalDeleteEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteHoursOfOperationRequestRequestTypeDef = TypedDict(
     "DeleteHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "HoursOfOperationId": str,
     },
 )
@@ -1938,16 +2060,16 @@
     "DeleteVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "VocabularyId": str,
     },
 )
 
-DeleteVocabularyResponseTypeDef = TypedDict(
-    "DeleteVocabularyResponseTypeDef",
+DeleteVocabularyResponseOutputTypeDef = TypedDict(
+    "DeleteVocabularyResponseOutputTypeDef",
     {
         "VocabularyArn": str,
         "VocabularyId": str,
         "State": VocabularyStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1956,83 +2078,83 @@
     "DescribeAgentStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AgentStatusId": str,
     },
 )
 
-DescribeAgentStatusResponseTypeDef = TypedDict(
-    "DescribeAgentStatusResponseTypeDef",
+DescribeAgentStatusResponseOutputTypeDef = TypedDict(
+    "DescribeAgentStatusResponseOutputTypeDef",
     {
-        "AgentStatus": "AgentStatusTypeDef",
+        "AgentStatus": "AgentStatusOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactEvaluationRequestRequestTypeDef = TypedDict(
     "DescribeContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
     },
 )
 
-DescribeContactEvaluationResponseTypeDef = TypedDict(
-    "DescribeContactEvaluationResponseTypeDef",
+DescribeContactEvaluationResponseOutputTypeDef = TypedDict(
+    "DescribeContactEvaluationResponseOutputTypeDef",
     {
-        "Evaluation": "EvaluationTypeDef",
-        "EvaluationForm": "EvaluationFormContentTypeDef",
+        "Evaluation": "EvaluationOutputTypeDef",
+        "EvaluationForm": "EvaluationFormContentOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactFlowModuleRequestRequestTypeDef = TypedDict(
     "DescribeContactFlowModuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowModuleId": str,
     },
 )
 
-DescribeContactFlowModuleResponseTypeDef = TypedDict(
-    "DescribeContactFlowModuleResponseTypeDef",
+DescribeContactFlowModuleResponseOutputTypeDef = TypedDict(
+    "DescribeContactFlowModuleResponseOutputTypeDef",
     {
-        "ContactFlowModule": "ContactFlowModuleTypeDef",
+        "ContactFlowModule": "ContactFlowModuleOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactFlowRequestRequestTypeDef = TypedDict(
     "DescribeContactFlowRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowId": str,
     },
 )
 
-DescribeContactFlowResponseTypeDef = TypedDict(
-    "DescribeContactFlowResponseTypeDef",
+DescribeContactFlowResponseOutputTypeDef = TypedDict(
+    "DescribeContactFlowResponseOutputTypeDef",
     {
-        "ContactFlow": "ContactFlowTypeDef",
+        "ContactFlow": "ContactFlowOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactRequestRequestTypeDef = TypedDict(
     "DescribeContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
 
-DescribeContactResponseTypeDef = TypedDict(
-    "DescribeContactResponseTypeDef",
+DescribeContactResponseOutputTypeDef = TypedDict(
+    "DescribeContactResponseOutputTypeDef",
     {
-        "Contact": "ContactTypeDef",
+        "Contact": "ContactOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeEvaluationFormRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEvaluationFormRequestRequestTypeDef",
     {
@@ -2044,287 +2166,289 @@
     "_OptionalDescribeEvaluationFormRequestRequestTypeDef",
     {
         "EvaluationFormVersion": int,
     },
     total=False,
 )
 
+
 class DescribeEvaluationFormRequestRequestTypeDef(
     _RequiredDescribeEvaluationFormRequestRequestTypeDef,
     _OptionalDescribeEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-DescribeEvaluationFormResponseTypeDef = TypedDict(
-    "DescribeEvaluationFormResponseTypeDef",
+
+DescribeEvaluationFormResponseOutputTypeDef = TypedDict(
+    "DescribeEvaluationFormResponseOutputTypeDef",
     {
-        "EvaluationForm": "EvaluationFormTypeDef",
+        "EvaluationForm": "EvaluationFormOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeHoursOfOperationRequestRequestTypeDef = TypedDict(
     "DescribeHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "HoursOfOperationId": str,
     },
 )
 
-DescribeHoursOfOperationResponseTypeDef = TypedDict(
-    "DescribeHoursOfOperationResponseTypeDef",
+DescribeHoursOfOperationResponseOutputTypeDef = TypedDict(
+    "DescribeHoursOfOperationResponseOutputTypeDef",
     {
-        "HoursOfOperation": "HoursOfOperationTypeDef",
+        "HoursOfOperation": "HoursOfOperationOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceAttributeRequestRequestTypeDef = TypedDict(
     "DescribeInstanceAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AttributeType": InstanceAttributeTypeType,
     },
 )
 
-DescribeInstanceAttributeResponseTypeDef = TypedDict(
-    "DescribeInstanceAttributeResponseTypeDef",
+DescribeInstanceAttributeResponseOutputTypeDef = TypedDict(
+    "DescribeInstanceAttributeResponseOutputTypeDef",
     {
-        "Attribute": "AttributeTypeDef",
+        "Attribute": "AttributeOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceRequestRequestTypeDef = TypedDict(
     "DescribeInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-DescribeInstanceResponseTypeDef = TypedDict(
-    "DescribeInstanceResponseTypeDef",
+DescribeInstanceResponseOutputTypeDef = TypedDict(
+    "DescribeInstanceResponseOutputTypeDef",
     {
-        "Instance": "InstanceTypeDef",
+        "Instance": "InstanceOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "DescribeInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AssociationId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
 )
 
-DescribeInstanceStorageConfigResponseTypeDef = TypedDict(
-    "DescribeInstanceStorageConfigResponseTypeDef",
+DescribeInstanceStorageConfigResponseOutputTypeDef = TypedDict(
+    "DescribeInstanceStorageConfigResponseOutputTypeDef",
     {
-        "StorageConfig": "InstanceStorageConfigTypeDef",
+        "StorageConfig": "InstanceStorageConfigOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePhoneNumberRequestRequestTypeDef = TypedDict(
     "DescribePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-DescribePhoneNumberResponseTypeDef = TypedDict(
-    "DescribePhoneNumberResponseTypeDef",
+DescribePhoneNumberResponseOutputTypeDef = TypedDict(
+    "DescribePhoneNumberResponseOutputTypeDef",
     {
-        "ClaimedPhoneNumberSummary": "ClaimedPhoneNumberSummaryTypeDef",
+        "ClaimedPhoneNumberSummary": "ClaimedPhoneNumberSummaryOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePromptRequestRequestTypeDef = TypedDict(
     "DescribePromptRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
-DescribePromptResponseTypeDef = TypedDict(
-    "DescribePromptResponseTypeDef",
+DescribePromptResponseOutputTypeDef = TypedDict(
+    "DescribePromptResponseOutputTypeDef",
     {
-        "Prompt": "PromptTypeDef",
+        "Prompt": "PromptOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueueRequestRequestTypeDef = TypedDict(
     "DescribeQueueRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
 
-DescribeQueueResponseTypeDef = TypedDict(
-    "DescribeQueueResponseTypeDef",
+DescribeQueueResponseOutputTypeDef = TypedDict(
+    "DescribeQueueResponseOutputTypeDef",
     {
-        "Queue": "QueueTypeDef",
+        "Queue": "QueueOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQuickConnectRequestRequestTypeDef = TypedDict(
     "DescribeQuickConnectRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QuickConnectId": str,
     },
 )
 
-DescribeQuickConnectResponseTypeDef = TypedDict(
-    "DescribeQuickConnectResponseTypeDef",
+DescribeQuickConnectResponseOutputTypeDef = TypedDict(
+    "DescribeQuickConnectResponseOutputTypeDef",
     {
-        "QuickConnect": "QuickConnectTypeDef",
+        "QuickConnect": "QuickConnectOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRoutingProfileRequestRequestTypeDef = TypedDict(
     "DescribeRoutingProfileRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
     },
 )
 
-DescribeRoutingProfileResponseTypeDef = TypedDict(
-    "DescribeRoutingProfileResponseTypeDef",
+DescribeRoutingProfileResponseOutputTypeDef = TypedDict(
+    "DescribeRoutingProfileResponseOutputTypeDef",
     {
-        "RoutingProfile": "RoutingProfileTypeDef",
+        "RoutingProfile": "RoutingProfileOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRuleRequestRequestTypeDef = TypedDict(
     "DescribeRuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RuleId": str,
     },
 )
 
-DescribeRuleResponseTypeDef = TypedDict(
-    "DescribeRuleResponseTypeDef",
+DescribeRuleResponseOutputTypeDef = TypedDict(
+    "DescribeRuleResponseOutputTypeDef",
     {
-        "Rule": "RuleTypeDef",
+        "Rule": "RuleOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSecurityProfileRequestRequestTypeDef = TypedDict(
     "DescribeSecurityProfileRequestRequestTypeDef",
     {
         "SecurityProfileId": str,
         "InstanceId": str,
     },
 )
 
-DescribeSecurityProfileResponseTypeDef = TypedDict(
-    "DescribeSecurityProfileResponseTypeDef",
+DescribeSecurityProfileResponseOutputTypeDef = TypedDict(
+    "DescribeSecurityProfileResponseOutputTypeDef",
     {
-        "SecurityProfile": "SecurityProfileTypeDef",
+        "SecurityProfile": "SecurityProfileOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrafficDistributionGroupRequestRequestTypeDef = TypedDict(
     "DescribeTrafficDistributionGroupRequestRequestTypeDef",
     {
         "TrafficDistributionGroupId": str,
     },
 )
 
-DescribeTrafficDistributionGroupResponseTypeDef = TypedDict(
-    "DescribeTrafficDistributionGroupResponseTypeDef",
+DescribeTrafficDistributionGroupResponseOutputTypeDef = TypedDict(
+    "DescribeTrafficDistributionGroupResponseOutputTypeDef",
     {
-        "TrafficDistributionGroup": "TrafficDistributionGroupTypeDef",
+        "TrafficDistributionGroup": "TrafficDistributionGroupOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserHierarchyGroupRequestRequestTypeDef = TypedDict(
     "DescribeUserHierarchyGroupRequestRequestTypeDef",
     {
         "HierarchyGroupId": str,
         "InstanceId": str,
     },
 )
 
-DescribeUserHierarchyGroupResponseTypeDef = TypedDict(
-    "DescribeUserHierarchyGroupResponseTypeDef",
+DescribeUserHierarchyGroupResponseOutputTypeDef = TypedDict(
+    "DescribeUserHierarchyGroupResponseOutputTypeDef",
     {
-        "HierarchyGroup": "HierarchyGroupTypeDef",
+        "HierarchyGroup": "HierarchyGroupOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserHierarchyStructureRequestRequestTypeDef = TypedDict(
     "DescribeUserHierarchyStructureRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-DescribeUserHierarchyStructureResponseTypeDef = TypedDict(
-    "DescribeUserHierarchyStructureResponseTypeDef",
+DescribeUserHierarchyStructureResponseOutputTypeDef = TypedDict(
+    "DescribeUserHierarchyStructureResponseOutputTypeDef",
     {
-        "HierarchyStructure": "HierarchyStructureTypeDef",
+        "HierarchyStructure": "HierarchyStructureOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
     },
 )
 
-DescribeUserResponseTypeDef = TypedDict(
-    "DescribeUserResponseTypeDef",
+DescribeUserResponseOutputTypeDef = TypedDict(
+    "DescribeUserResponseOutputTypeDef",
     {
-        "User": "UserTypeDef",
+        "User": "UserOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVocabularyRequestRequestTypeDef = TypedDict(
     "DescribeVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "VocabularyId": str,
     },
 )
 
-DescribeVocabularyResponseTypeDef = TypedDict(
-    "DescribeVocabularyResponseTypeDef",
+DescribeVocabularyResponseOutputTypeDef = TypedDict(
+    "DescribeVocabularyResponseOutputTypeDef",
     {
-        "Vocabulary": "VocabularyTypeDef",
+        "Vocabulary": "VocabularyOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DimensionsTypeDef = TypedDict(
-    "DimensionsTypeDef",
+DimensionsOutputTypeDef = TypedDict(
+    "DimensionsOutputTypeDef",
     {
-        "Queue": "QueueReferenceTypeDef",
+        "Queue": "QueueReferenceOutputTypeDef",
         "Channel": ChannelType,
-        "RoutingProfile": "RoutingProfileReferenceTypeDef",
+        "RoutingProfile": "RoutingProfileReferenceOutputTypeDef",
     },
 )
 
 DisassociateApprovedOriginRequestRequestTypeDef = TypedDict(
     "DisassociateApprovedOriginRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -2343,19 +2467,21 @@
     {
         "LexBot": "LexBotTypeDef",
         "LexV2Bot": "LexV2BotTypeDef",
     },
     total=False,
 )
 
+
 class DisassociateBotRequestRequestTypeDef(
     _RequiredDisassociateBotRequestRequestTypeDef, _OptionalDisassociateBotRequestRequestTypeDef
 ):
     pass
 
+
 DisassociateInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "DisassociateInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AssociationId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
@@ -2417,100 +2543,151 @@
     {
         "UserId": str,
         "InstanceId": str,
         "ContactId": str,
     },
 )
 
+DistributionOutputTypeDef = TypedDict(
+    "DistributionOutputTypeDef",
+    {
+        "Region": str,
+        "Percentage": int,
+    },
+)
+
 DistributionTypeDef = TypedDict(
     "DistributionTypeDef",
     {
         "Region": str,
         "Percentage": int,
     },
 )
 
-EmailReferenceTypeDef = TypedDict(
-    "EmailReferenceTypeDef",
+EmailReferenceOutputTypeDef = TypedDict(
+    "EmailReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
+    {
+        "EncryptionType": Literal["KMS"],
+        "KeyId": str,
+    },
+)
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "EncryptionType": Literal["KMS"],
         "KeyId": str,
     },
 )
 
+EvaluationAnswerDataOutputTypeDef = TypedDict(
+    "EvaluationAnswerDataOutputTypeDef",
+    {
+        "StringValue": str,
+        "NumericValue": float,
+        "NotApplicable": bool,
+    },
+)
+
 EvaluationAnswerDataTypeDef = TypedDict(
     "EvaluationAnswerDataTypeDef",
     {
         "StringValue": str,
         "NumericValue": float,
         "NotApplicable": bool,
     },
+    total=False,
 )
 
 EvaluationAnswerInputTypeDef = TypedDict(
     "EvaluationAnswerInputTypeDef",
     {
         "Value": "EvaluationAnswerDataTypeDef",
     },
     total=False,
 )
 
-EvaluationAnswerOutputTypeDef = TypedDict(
-    "EvaluationAnswerOutputTypeDef",
+EvaluationAnswerOutputOutputTypeDef = TypedDict(
+    "EvaluationAnswerOutputOutputTypeDef",
     {
-        "Value": "EvaluationAnswerDataTypeDef",
-        "SystemSuggestedValue": "EvaluationAnswerDataTypeDef",
+        "Value": "EvaluationAnswerDataOutputTypeDef",
+        "SystemSuggestedValue": "EvaluationAnswerDataOutputTypeDef",
     },
 )
 
-EvaluationFormContentTypeDef = TypedDict(
-    "EvaluationFormContentTypeDef",
+EvaluationFormContentOutputTypeDef = TypedDict(
+    "EvaluationFormContentOutputTypeDef",
     {
         "EvaluationFormVersion": int,
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "Description": str,
-        "Items": List["EvaluationFormItemTypeDef"],
-        "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
+        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "ScoringStrategy": "EvaluationFormScoringStrategyOutputTypeDef",
+    },
+)
+
+EvaluationFormItemOutputTypeDef = TypedDict(
+    "EvaluationFormItemOutputTypeDef",
+    {
+        "Section": Dict[str, Any],
+        "Question": "EvaluationFormQuestionOutputTypeDef",
     },
 )
 
 EvaluationFormItemTypeDef = TypedDict(
     "EvaluationFormItemTypeDef",
     {
         "Section": Dict[str, Any],
         "Question": "EvaluationFormQuestionTypeDef",
     },
     total=False,
 )
 
+EvaluationFormNumericQuestionAutomationOutputTypeDef = TypedDict(
+    "EvaluationFormNumericQuestionAutomationOutputTypeDef",
+    {
+        "PropertyValue": "NumericQuestionPropertyValueAutomationOutputTypeDef",
+    },
+)
+
 EvaluationFormNumericQuestionAutomationTypeDef = TypedDict(
     "EvaluationFormNumericQuestionAutomationTypeDef",
     {
         "PropertyValue": "NumericQuestionPropertyValueAutomationTypeDef",
     },
     total=False,
 )
 
+EvaluationFormNumericQuestionOptionOutputTypeDef = TypedDict(
+    "EvaluationFormNumericQuestionOptionOutputTypeDef",
+    {
+        "MinValue": int,
+        "MaxValue": int,
+        "Score": int,
+        "AutomaticFail": bool,
+    },
+)
+
 _RequiredEvaluationFormNumericQuestionOptionTypeDef = TypedDict(
     "_RequiredEvaluationFormNumericQuestionOptionTypeDef",
     {
         "MinValue": int,
         "MaxValue": int,
     },
 )
@@ -2519,20 +2696,32 @@
     {
         "Score": int,
         "AutomaticFail": bool,
     },
     total=False,
 )
 
+
 class EvaluationFormNumericQuestionOptionTypeDef(
     _RequiredEvaluationFormNumericQuestionOptionTypeDef,
     _OptionalEvaluationFormNumericQuestionOptionTypeDef,
 ):
     pass
 
+
+EvaluationFormNumericQuestionPropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
+    {
+        "MinValue": int,
+        "MaxValue": int,
+        "Options": List["EvaluationFormNumericQuestionOptionOutputTypeDef"],
+        "Automation": "EvaluationFormNumericQuestionAutomationOutputTypeDef",
+    },
+)
+
 _RequiredEvaluationFormNumericQuestionPropertiesTypeDef = TypedDict(
     "_RequiredEvaluationFormNumericQuestionPropertiesTypeDef",
     {
         "MinValue": int,
         "MaxValue": int,
     },
 )
@@ -2541,20 +2730,55 @@
     {
         "Options": Sequence["EvaluationFormNumericQuestionOptionTypeDef"],
         "Automation": "EvaluationFormNumericQuestionAutomationTypeDef",
     },
     total=False,
 )
 
+
 class EvaluationFormNumericQuestionPropertiesTypeDef(
     _RequiredEvaluationFormNumericQuestionPropertiesTypeDef,
     _OptionalEvaluationFormNumericQuestionPropertiesTypeDef,
 ):
     pass
 
+
+EvaluationFormOutputTypeDef = TypedDict(
+    "EvaluationFormOutputTypeDef",
+    {
+        "EvaluationFormId": str,
+        "EvaluationFormVersion": int,
+        "Locked": bool,
+        "EvaluationFormArn": str,
+        "Title": str,
+        "Description": str,
+        "Status": EvaluationFormVersionStatusType,
+        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "ScoringStrategy": "EvaluationFormScoringStrategyOutputTypeDef",
+        "CreatedTime": datetime,
+        "CreatedBy": str,
+        "LastModifiedTime": datetime,
+        "LastModifiedBy": str,
+        "Tags": Dict[str, str],
+    },
+)
+
+EvaluationFormQuestionOutputTypeDef = TypedDict(
+    "EvaluationFormQuestionOutputTypeDef",
+    {
+        "Title": str,
+        "Instructions": str,
+        "RefId": str,
+        "NotApplicableEnabled": bool,
+        "QuestionType": EvaluationFormQuestionTypeType,
+        "QuestionTypeProperties": "EvaluationFormQuestionTypePropertiesOutputTypeDef",
+        "Weight": float,
+    },
+)
+
 _RequiredEvaluationFormQuestionTypeDef = TypedDict(
     "_RequiredEvaluationFormQuestionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "QuestionType": EvaluationFormQuestionTypeType,
     },
@@ -2566,36 +2790,65 @@
         "NotApplicableEnabled": bool,
         "QuestionTypeProperties": "EvaluationFormQuestionTypePropertiesTypeDef",
         "Weight": float,
     },
     total=False,
 )
 
+
 class EvaluationFormQuestionTypeDef(
     _RequiredEvaluationFormQuestionTypeDef, _OptionalEvaluationFormQuestionTypeDef
 ):
     pass
 
+
+EvaluationFormQuestionTypePropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
+    {
+        "Numeric": "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
+        "SingleSelect": "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
+    },
+)
+
 EvaluationFormQuestionTypePropertiesTypeDef = TypedDict(
     "EvaluationFormQuestionTypePropertiesTypeDef",
     {
         "Numeric": "EvaluationFormNumericQuestionPropertiesTypeDef",
         "SingleSelect": "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
     },
     total=False,
 )
 
+EvaluationFormScoringStrategyOutputTypeDef = TypedDict(
+    "EvaluationFormScoringStrategyOutputTypeDef",
+    {
+        "Mode": EvaluationFormScoringModeType,
+        "Status": EvaluationFormScoringStatusType,
+    },
+)
+
 EvaluationFormScoringStrategyTypeDef = TypedDict(
     "EvaluationFormScoringStrategyTypeDef",
     {
         "Mode": EvaluationFormScoringModeType,
         "Status": EvaluationFormScoringStatusType,
     },
 )
 
+EvaluationFormSectionOutputTypeDef = TypedDict(
+    "EvaluationFormSectionOutputTypeDef",
+    {
+        "Title": str,
+        "RefId": str,
+        "Instructions": str,
+        "Items": List[Dict[str, Any]],
+        "Weight": float,
+    },
+)
+
 _RequiredEvaluationFormSectionTypeDef = TypedDict(
     "_RequiredEvaluationFormSectionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "Items": Sequence[Dict[str, Any]],
     },
@@ -2605,47 +2858,76 @@
     {
         "Instructions": str,
         "Weight": float,
     },
     total=False,
 )
 
+
 class EvaluationFormSectionTypeDef(
     _RequiredEvaluationFormSectionTypeDef, _OptionalEvaluationFormSectionTypeDef
 ):
     pass
 
+
+EvaluationFormSingleSelectQuestionAutomationOptionOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionAutomationOptionOutputTypeDef",
+    {
+        "RuleCategory": "SingleSelectQuestionRuleCategoryAutomationOutputTypeDef",
+    },
+)
+
 EvaluationFormSingleSelectQuestionAutomationOptionTypeDef = TypedDict(
     "EvaluationFormSingleSelectQuestionAutomationOptionTypeDef",
     {
         "RuleCategory": "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     },
     total=False,
 )
 
+EvaluationFormSingleSelectQuestionAutomationOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
+    {
+        "Options": List["EvaluationFormSingleSelectQuestionAutomationOptionOutputTypeDef"],
+        "DefaultOptionRefId": str,
+    },
+)
+
 _RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef = TypedDict(
     "_RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef",
     {
         "Options": Sequence["EvaluationFormSingleSelectQuestionAutomationOptionTypeDef"],
     },
 )
 _OptionalEvaluationFormSingleSelectQuestionAutomationTypeDef = TypedDict(
     "_OptionalEvaluationFormSingleSelectQuestionAutomationTypeDef",
     {
         "DefaultOptionRefId": str,
     },
     total=False,
 )
 
+
 class EvaluationFormSingleSelectQuestionAutomationTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionAutomationTypeDef,
 ):
     pass
 
+
+EvaluationFormSingleSelectQuestionOptionOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionOptionOutputTypeDef",
+    {
+        "RefId": str,
+        "Text": str,
+        "Score": int,
+        "AutomaticFail": bool,
+    },
+)
+
 _RequiredEvaluationFormSingleSelectQuestionOptionTypeDef = TypedDict(
     "_RequiredEvaluationFormSingleSelectQuestionOptionTypeDef",
     {
         "RefId": str,
         "Text": str,
     },
 )
@@ -2654,20 +2936,31 @@
     {
         "Score": int,
         "AutomaticFail": bool,
     },
     total=False,
 )
 
+
 class EvaluationFormSingleSelectQuestionOptionTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionOptionTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionOptionTypeDef,
 ):
     pass
 
+
+EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef = TypedDict(
+    "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
+    {
+        "Options": List["EvaluationFormSingleSelectQuestionOptionOutputTypeDef"],
+        "DisplayAs": EvaluationFormSingleSelectQuestionDisplayModeType,
+        "Automation": "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
+    },
+)
+
 _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef = TypedDict(
     "_RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef",
     {
         "Options": Sequence["EvaluationFormSingleSelectQuestionOptionTypeDef"],
     },
 )
 _OptionalEvaluationFormSingleSelectQuestionPropertiesTypeDef = TypedDict(
@@ -2675,22 +2968,24 @@
     {
         "DisplayAs": EvaluationFormSingleSelectQuestionDisplayModeType,
         "Automation": "EvaluationFormSingleSelectQuestionAutomationTypeDef",
     },
     total=False,
 )
 
+
 class EvaluationFormSingleSelectQuestionPropertiesTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionPropertiesTypeDef,
 ):
     pass
 
-EvaluationFormSummaryTypeDef = TypedDict(
-    "EvaluationFormSummaryTypeDef",
+
+EvaluationFormSummaryOutputTypeDef = TypedDict(
+    "EvaluationFormSummaryOutputTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
@@ -2698,103 +2993,98 @@
         "LastActivatedTime": datetime,
         "LastActivatedBy": str,
         "LatestVersion": int,
         "ActiveVersion": int,
     },
 )
 
-EvaluationFormTypeDef = TypedDict(
-    "EvaluationFormTypeDef",
-    {
-        "EvaluationFormId": str,
-        "EvaluationFormVersion": int,
-        "Locked": bool,
-        "EvaluationFormArn": str,
-        "Title": str,
-        "Description": str,
-        "Status": EvaluationFormVersionStatusType,
-        "Items": List["EvaluationFormItemTypeDef"],
-        "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
-        "CreatedTime": datetime,
-        "CreatedBy": str,
-        "LastModifiedTime": datetime,
-        "LastModifiedBy": str,
-        "Tags": Dict[str, str],
-    },
-)
-
-EvaluationFormVersionSummaryTypeDef = TypedDict(
-    "EvaluationFormVersionSummaryTypeDef",
+EvaluationFormVersionSummaryOutputTypeDef = TypedDict(
+    "EvaluationFormVersionSummaryOutputTypeDef",
     {
         "EvaluationFormArn": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
         "Status": EvaluationFormVersionStatusType,
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
     },
 )
 
-EvaluationMetadataTypeDef = TypedDict(
-    "EvaluationMetadataTypeDef",
+EvaluationMetadataOutputTypeDef = TypedDict(
+    "EvaluationMetadataOutputTypeDef",
     {
         "ContactId": str,
         "EvaluatorArn": str,
         "ContactAgentId": str,
-        "Score": "EvaluationScoreTypeDef",
+        "Score": "EvaluationScoreOutputTypeDef",
+    },
+)
+
+EvaluationNoteOutputTypeDef = TypedDict(
+    "EvaluationNoteOutputTypeDef",
+    {
+        "Value": str,
     },
 )
 
 EvaluationNoteTypeDef = TypedDict(
     "EvaluationNoteTypeDef",
     {
         "Value": str,
     },
+    total=False,
 )
 
-EvaluationScoreTypeDef = TypedDict(
-    "EvaluationScoreTypeDef",
+EvaluationOutputTypeDef = TypedDict(
+    "EvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "EvaluationArn": str,
+        "Metadata": "EvaluationMetadataOutputTypeDef",
+        "Answers": Dict[str, "EvaluationAnswerOutputOutputTypeDef"],
+        "Notes": Dict[str, "EvaluationNoteOutputTypeDef"],
+        "Status": EvaluationStatusType,
+        "Scores": Dict[str, "EvaluationScoreOutputTypeDef"],
+        "CreatedTime": datetime,
+        "LastModifiedTime": datetime,
+        "Tags": Dict[str, str],
+    },
+)
+
+EvaluationScoreOutputTypeDef = TypedDict(
+    "EvaluationScoreOutputTypeDef",
     {
         "Percentage": float,
         "NotApplicable": bool,
         "AutomaticFail": bool,
     },
 )
 
-EvaluationSummaryTypeDef = TypedDict(
-    "EvaluationSummaryTypeDef",
+EvaluationSummaryOutputTypeDef = TypedDict(
+    "EvaluationSummaryOutputTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "EvaluationFormTitle": str,
         "EvaluationFormId": str,
         "Status": EvaluationStatusType,
         "EvaluatorArn": str,
-        "Score": "EvaluationScoreTypeDef",
+        "Score": "EvaluationScoreOutputTypeDef",
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
     },
 )
 
-EvaluationTypeDef = TypedDict(
-    "EvaluationTypeDef",
+EventBridgeActionDefinitionOutputTypeDef = TypedDict(
+    "EventBridgeActionDefinitionOutputTypeDef",
     {
-        "EvaluationId": str,
-        "EvaluationArn": str,
-        "Metadata": "EvaluationMetadataTypeDef",
-        "Answers": Dict[str, "EvaluationAnswerOutputTypeDef"],
-        "Notes": Dict[str, "EvaluationNoteTypeDef"],
-        "Status": EvaluationStatusType,
-        "Scores": Dict[str, "EvaluationScoreTypeDef"],
-        "CreatedTime": datetime,
-        "LastModifiedTime": datetime,
-        "Tags": Dict[str, str],
+        "Name": str,
     },
 )
 
 EventBridgeActionDefinitionTypeDef = TypedDict(
     "EventBridgeActionDefinitionTypeDef",
     {
         "Name": str,
@@ -2824,16 +3114,16 @@
     "GetContactAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "InitialContactId": str,
     },
 )
 
-GetContactAttributesResponseTypeDef = TypedDict(
-    "GetContactAttributesResponseTypeDef",
+GetContactAttributesResponseOutputTypeDef = TypedDict(
+    "GetContactAttributesResponseOutputTypeDef",
     {
         "Attributes": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetCurrentMetricDataRequestRequestTypeDef = TypedDict(
@@ -2851,25 +3141,27 @@
         "NextToken": str,
         "MaxResults": int,
         "SortCriteria": Sequence["CurrentMetricSortCriteriaTypeDef"],
     },
     total=False,
 )
 
+
 class GetCurrentMetricDataRequestRequestTypeDef(
     _RequiredGetCurrentMetricDataRequestRequestTypeDef,
     _OptionalGetCurrentMetricDataRequestRequestTypeDef,
 ):
     pass
 
-GetCurrentMetricDataResponseTypeDef = TypedDict(
-    "GetCurrentMetricDataResponseTypeDef",
+
+GetCurrentMetricDataResponseOutputTypeDef = TypedDict(
+    "GetCurrentMetricDataResponseOutputTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["CurrentMetricResultTypeDef"],
+        "MetricResults": List["CurrentMetricResultOutputTypeDef"],
         "DataSnapshotTime": datetime,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetCurrentUserDataRequestRequestTypeDef = TypedDict(
@@ -2884,41 +3176,43 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetCurrentUserDataRequestRequestTypeDef(
     _RequiredGetCurrentUserDataRequestRequestTypeDef,
     _OptionalGetCurrentUserDataRequestRequestTypeDef,
 ):
     pass
 
-GetCurrentUserDataResponseTypeDef = TypedDict(
-    "GetCurrentUserDataResponseTypeDef",
+
+GetCurrentUserDataResponseOutputTypeDef = TypedDict(
+    "GetCurrentUserDataResponseOutputTypeDef",
     {
         "NextToken": str,
-        "UserDataList": List["UserDataTypeDef"],
+        "UserDataList": List["UserDataOutputTypeDef"],
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFederationTokenRequestRequestTypeDef = TypedDict(
     "GetFederationTokenRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-GetFederationTokenResponseTypeDef = TypedDict(
-    "GetFederationTokenResponseTypeDef",
+GetFederationTokenResponseOutputTypeDef = TypedDict(
+    "GetFederationTokenResponseOutputTypeDef",
     {
-        "Credentials": "CredentialsTypeDef",
+        "Credentials": "CredentialsOutputTypeDef",
         "SignInUrl": str,
         "UserArn": str,
         "UserId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2937,20 +3231,22 @@
     {
         "Groupings": Sequence[GroupingType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetMetricDataRequestGetMetricDataPaginateTypeDef(
     _RequiredGetMetricDataRequestGetMetricDataPaginateTypeDef,
     _OptionalGetMetricDataRequestGetMetricDataPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetMetricDataRequestRequestTypeDef = TypedDict(
     "_RequiredGetMetricDataRequestRequestTypeDef",
     {
         "InstanceId": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Filters": "FiltersTypeDef",
@@ -2963,24 +3259,26 @@
         "Groupings": Sequence[GroupingType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetMetricDataRequestRequestTypeDef(
     _RequiredGetMetricDataRequestRequestTypeDef, _OptionalGetMetricDataRequestRequestTypeDef
 ):
     pass
 
-GetMetricDataResponseTypeDef = TypedDict(
-    "GetMetricDataResponseTypeDef",
+
+GetMetricDataResponseOutputTypeDef = TypedDict(
+    "GetMetricDataResponseOutputTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["HistoricalMetricResultTypeDef"],
+        "MetricResults": List["HistoricalMetricResultOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetMetricDataV2RequestRequestTypeDef = TypedDict(
     "_RequiredGetMetricDataV2RequestRequestTypeDef",
     {
@@ -2997,38 +3295,40 @@
         "Groupings": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetMetricDataV2RequestRequestTypeDef(
     _RequiredGetMetricDataV2RequestRequestTypeDef, _OptionalGetMetricDataV2RequestRequestTypeDef
 ):
     pass
 
-GetMetricDataV2ResponseTypeDef = TypedDict(
-    "GetMetricDataV2ResponseTypeDef",
+
+GetMetricDataV2ResponseOutputTypeDef = TypedDict(
+    "GetMetricDataV2ResponseOutputTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["MetricResultV2TypeDef"],
+        "MetricResults": List["MetricResultV2OutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPromptFileRequestRequestTypeDef = TypedDict(
     "GetPromptFileRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
-GetPromptFileResponseTypeDef = TypedDict(
-    "GetPromptFileResponseTypeDef",
+GetPromptFileResponseOutputTypeDef = TypedDict(
+    "GetPromptFileResponseOutputTypeDef",
     {
         "PromptPresignedUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTaskTemplateRequestRequestTypeDef = TypedDict(
@@ -3042,31 +3342,33 @@
     "_OptionalGetTaskTemplateRequestRequestTypeDef",
     {
         "SnapshotVersion": str,
     },
     total=False,
 )
 
+
 class GetTaskTemplateRequestRequestTypeDef(
     _RequiredGetTaskTemplateRequestRequestTypeDef, _OptionalGetTaskTemplateRequestRequestTypeDef
 ):
     pass
 
-GetTaskTemplateResponseTypeDef = TypedDict(
-    "GetTaskTemplateResponseTypeDef",
+
+GetTaskTemplateResponseOutputTypeDef = TypedDict(
+    "GetTaskTemplateResponseOutputTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
-        "Constraints": "TaskTemplateConstraintsTypeDef",
-        "Defaults": "TaskTemplateDefaultsTypeDef",
-        "Fields": List["TaskTemplateFieldTypeDef"],
+        "Constraints": "TaskTemplateConstraintsOutputTypeDef",
+        "Defaults": "TaskTemplateDefaultsOutputTypeDef",
+        "Fields": List["TaskTemplateFieldOutputTypeDef"],
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3074,18 +3376,18 @@
 GetTrafficDistributionRequestRequestTypeDef = TypedDict(
     "GetTrafficDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetTrafficDistributionResponseTypeDef = TypedDict(
-    "GetTrafficDistributionResponseTypeDef",
+GetTrafficDistributionResponseOutputTypeDef = TypedDict(
+    "GetTrafficDistributionResponseOutputTypeDef",
     {
-        "TelephonyConfig": "TelephonyConfigTypeDef",
+        "TelephonyConfig": "TelephonyConfigOutputTypeDef",
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HierarchyGroupConditionTypeDef = TypedDict(
@@ -3093,89 +3395,89 @@
     {
         "Value": str,
         "HierarchyGroupMatchType": HierarchyGroupMatchTypeType,
     },
     total=False,
 )
 
-HierarchyGroupSummaryReferenceTypeDef = TypedDict(
-    "HierarchyGroupSummaryReferenceTypeDef",
+HierarchyGroupOutputTypeDef = TypedDict(
+    "HierarchyGroupOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
+        "Name": str,
+        "LevelId": str,
+        "HierarchyPath": "HierarchyPathOutputTypeDef",
+        "Tags": Dict[str, str],
     },
 )
 
-HierarchyGroupSummaryTypeDef = TypedDict(
-    "HierarchyGroupSummaryTypeDef",
+HierarchyGroupSummaryOutputTypeDef = TypedDict(
+    "HierarchyGroupSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
-HierarchyGroupTypeDef = TypedDict(
-    "HierarchyGroupTypeDef",
+HierarchyGroupSummaryReferenceOutputTypeDef = TypedDict(
+    "HierarchyGroupSummaryReferenceOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
-        "Name": str,
-        "LevelId": str,
-        "HierarchyPath": "HierarchyPathTypeDef",
-        "Tags": Dict[str, str],
     },
 )
 
-HierarchyLevelTypeDef = TypedDict(
-    "HierarchyLevelTypeDef",
+HierarchyLevelOutputTypeDef = TypedDict(
+    "HierarchyLevelOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
 HierarchyLevelUpdateTypeDef = TypedDict(
     "HierarchyLevelUpdateTypeDef",
     {
         "Name": str,
     },
 )
 
-HierarchyPathReferenceTypeDef = TypedDict(
-    "HierarchyPathReferenceTypeDef",
+HierarchyPathOutputTypeDef = TypedDict(
+    "HierarchyPathOutputTypeDef",
     {
-        "LevelOne": "HierarchyGroupSummaryReferenceTypeDef",
-        "LevelTwo": "HierarchyGroupSummaryReferenceTypeDef",
-        "LevelThree": "HierarchyGroupSummaryReferenceTypeDef",
-        "LevelFour": "HierarchyGroupSummaryReferenceTypeDef",
-        "LevelFive": "HierarchyGroupSummaryReferenceTypeDef",
+        "LevelOne": "HierarchyGroupSummaryOutputTypeDef",
+        "LevelTwo": "HierarchyGroupSummaryOutputTypeDef",
+        "LevelThree": "HierarchyGroupSummaryOutputTypeDef",
+        "LevelFour": "HierarchyGroupSummaryOutputTypeDef",
+        "LevelFive": "HierarchyGroupSummaryOutputTypeDef",
     },
 )
 
-HierarchyPathTypeDef = TypedDict(
-    "HierarchyPathTypeDef",
+HierarchyPathReferenceOutputTypeDef = TypedDict(
+    "HierarchyPathReferenceOutputTypeDef",
     {
-        "LevelOne": "HierarchyGroupSummaryTypeDef",
-        "LevelTwo": "HierarchyGroupSummaryTypeDef",
-        "LevelThree": "HierarchyGroupSummaryTypeDef",
-        "LevelFour": "HierarchyGroupSummaryTypeDef",
-        "LevelFive": "HierarchyGroupSummaryTypeDef",
+        "LevelOne": "HierarchyGroupSummaryReferenceOutputTypeDef",
+        "LevelTwo": "HierarchyGroupSummaryReferenceOutputTypeDef",
+        "LevelThree": "HierarchyGroupSummaryReferenceOutputTypeDef",
+        "LevelFour": "HierarchyGroupSummaryReferenceOutputTypeDef",
+        "LevelFive": "HierarchyGroupSummaryReferenceOutputTypeDef",
     },
 )
 
-HierarchyStructureTypeDef = TypedDict(
-    "HierarchyStructureTypeDef",
+HierarchyStructureOutputTypeDef = TypedDict(
+    "HierarchyStructureOutputTypeDef",
     {
-        "LevelOne": "HierarchyLevelTypeDef",
-        "LevelTwo": "HierarchyLevelTypeDef",
-        "LevelThree": "HierarchyLevelTypeDef",
-        "LevelFour": "HierarchyLevelTypeDef",
-        "LevelFive": "HierarchyLevelTypeDef",
+        "LevelOne": "HierarchyLevelOutputTypeDef",
+        "LevelTwo": "HierarchyLevelOutputTypeDef",
+        "LevelThree": "HierarchyLevelOutputTypeDef",
+        "LevelFour": "HierarchyLevelOutputTypeDef",
+        "LevelFive": "HierarchyLevelOutputTypeDef",
     },
 )
 
 HierarchyStructureUpdateTypeDef = TypedDict(
     "HierarchyStructureUpdateTypeDef",
     {
         "LevelOne": "HierarchyLevelUpdateTypeDef",
@@ -3183,50 +3485,82 @@
         "LevelThree": "HierarchyLevelUpdateTypeDef",
         "LevelFour": "HierarchyLevelUpdateTypeDef",
         "LevelFive": "HierarchyLevelUpdateTypeDef",
     },
     total=False,
 )
 
-HistoricalMetricDataTypeDef = TypedDict(
-    "HistoricalMetricDataTypeDef",
+HistoricalMetricDataOutputTypeDef = TypedDict(
+    "HistoricalMetricDataOutputTypeDef",
     {
-        "Metric": "HistoricalMetricTypeDef",
+        "Metric": "HistoricalMetricOutputTypeDef",
         "Value": float,
     },
 )
 
-HistoricalMetricResultTypeDef = TypedDict(
-    "HistoricalMetricResultTypeDef",
+HistoricalMetricOutputTypeDef = TypedDict(
+    "HistoricalMetricOutputTypeDef",
     {
-        "Dimensions": "DimensionsTypeDef",
-        "Collections": List["HistoricalMetricDataTypeDef"],
+        "Name": HistoricalMetricNameType,
+        "Threshold": "ThresholdOutputTypeDef",
+        "Statistic": StatisticType,
+        "Unit": UnitType,
+    },
+)
+
+HistoricalMetricResultOutputTypeDef = TypedDict(
+    "HistoricalMetricResultOutputTypeDef",
+    {
+        "Dimensions": "DimensionsOutputTypeDef",
+        "Collections": List["HistoricalMetricDataOutputTypeDef"],
     },
 )
 
 HistoricalMetricTypeDef = TypedDict(
     "HistoricalMetricTypeDef",
     {
         "Name": HistoricalMetricNameType,
         "Threshold": "ThresholdTypeDef",
         "Statistic": StatisticType,
         "Unit": UnitType,
     },
     total=False,
 )
 
+HoursOfOperationConfigOutputTypeDef = TypedDict(
+    "HoursOfOperationConfigOutputTypeDef",
+    {
+        "Day": HoursOfOperationDaysType,
+        "StartTime": "HoursOfOperationTimeSliceOutputTypeDef",
+        "EndTime": "HoursOfOperationTimeSliceOutputTypeDef",
+    },
+)
+
 HoursOfOperationConfigTypeDef = TypedDict(
     "HoursOfOperationConfigTypeDef",
     {
         "Day": HoursOfOperationDaysType,
         "StartTime": "HoursOfOperationTimeSliceTypeDef",
         "EndTime": "HoursOfOperationTimeSliceTypeDef",
     },
 )
 
+HoursOfOperationOutputTypeDef = TypedDict(
+    "HoursOfOperationOutputTypeDef",
+    {
+        "HoursOfOperationId": str,
+        "HoursOfOperationArn": str,
+        "Name": str,
+        "Description": str,
+        "TimeZone": str,
+        "Config": List["HoursOfOperationConfigOutputTypeDef"],
+        "Tags": Dict[str, str],
+    },
+)
+
 HoursOfOperationSearchCriteriaTypeDef = TypedDict(
     "HoursOfOperationSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
@@ -3237,51 +3571,75 @@
     "HoursOfOperationSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-HoursOfOperationSummaryTypeDef = TypedDict(
-    "HoursOfOperationSummaryTypeDef",
+HoursOfOperationSummaryOutputTypeDef = TypedDict(
+    "HoursOfOperationSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
+HoursOfOperationTimeSliceOutputTypeDef = TypedDict(
+    "HoursOfOperationTimeSliceOutputTypeDef",
+    {
+        "Hours": int,
+        "Minutes": int,
+    },
+)
+
 HoursOfOperationTimeSliceTypeDef = TypedDict(
     "HoursOfOperationTimeSliceTypeDef",
     {
         "Hours": int,
         "Minutes": int,
     },
 )
 
-HoursOfOperationTypeDef = TypedDict(
-    "HoursOfOperationTypeDef",
+InstanceOutputTypeDef = TypedDict(
+    "InstanceOutputTypeDef",
     {
-        "HoursOfOperationId": str,
-        "HoursOfOperationArn": str,
-        "Name": str,
-        "Description": str,
-        "TimeZone": str,
-        "Config": List["HoursOfOperationConfigTypeDef"],
-        "Tags": Dict[str, str],
+        "Id": str,
+        "Arn": str,
+        "IdentityManagementType": DirectoryTypeType,
+        "InstanceAlias": str,
+        "CreatedTime": datetime,
+        "ServiceRole": str,
+        "InstanceStatus": InstanceStatusType,
+        "StatusReason": "InstanceStatusReasonOutputTypeDef",
+        "InboundCallsEnabled": bool,
+        "OutboundCallsEnabled": bool,
+        "InstanceAccessUrl": str,
     },
 )
 
-InstanceStatusReasonTypeDef = TypedDict(
-    "InstanceStatusReasonTypeDef",
+InstanceStatusReasonOutputTypeDef = TypedDict(
+    "InstanceStatusReasonOutputTypeDef",
     {
         "Message": str,
     },
 )
 
+InstanceStorageConfigOutputTypeDef = TypedDict(
+    "InstanceStorageConfigOutputTypeDef",
+    {
+        "AssociationId": str,
+        "StorageType": StorageTypeType,
+        "S3Config": "S3ConfigOutputTypeDef",
+        "KinesisVideoStreamConfig": "KinesisVideoStreamConfigOutputTypeDef",
+        "KinesisStreamConfig": "KinesisStreamConfigOutputTypeDef",
+        "KinesisFirehoseConfig": "KinesisFirehoseConfigOutputTypeDef",
+    },
+)
+
 _RequiredInstanceStorageConfigTypeDef = TypedDict(
     "_RequiredInstanceStorageConfigTypeDef",
     {
         "StorageType": StorageTypeType,
     },
 )
 _OptionalInstanceStorageConfigTypeDef = TypedDict(
@@ -3292,113 +3650,143 @@
         "KinesisVideoStreamConfig": "KinesisVideoStreamConfigTypeDef",
         "KinesisStreamConfig": "KinesisStreamConfigTypeDef",
         "KinesisFirehoseConfig": "KinesisFirehoseConfigTypeDef",
     },
     total=False,
 )
 
+
 class InstanceStorageConfigTypeDef(
     _RequiredInstanceStorageConfigTypeDef, _OptionalInstanceStorageConfigTypeDef
 ):
     pass
 
-InstanceSummaryTypeDef = TypedDict(
-    "InstanceSummaryTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "IdentityManagementType": DirectoryTypeType,
-        "InstanceAlias": str,
-        "CreatedTime": datetime,
-        "ServiceRole": str,
-        "InstanceStatus": InstanceStatusType,
-        "InboundCallsEnabled": bool,
-        "OutboundCallsEnabled": bool,
-        "InstanceAccessUrl": str,
-    },
-)
 
-InstanceTypeDef = TypedDict(
-    "InstanceTypeDef",
+InstanceSummaryOutputTypeDef = TypedDict(
+    "InstanceSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "IdentityManagementType": DirectoryTypeType,
         "InstanceAlias": str,
         "CreatedTime": datetime,
         "ServiceRole": str,
         "InstanceStatus": InstanceStatusType,
-        "StatusReason": "InstanceStatusReasonTypeDef",
         "InboundCallsEnabled": bool,
         "OutboundCallsEnabled": bool,
         "InstanceAccessUrl": str,
     },
 )
 
-IntegrationAssociationSummaryTypeDef = TypedDict(
-    "IntegrationAssociationSummaryTypeDef",
+IntegrationAssociationSummaryOutputTypeDef = TypedDict(
+    "IntegrationAssociationSummaryOutputTypeDef",
     {
         "IntegrationAssociationId": str,
         "IntegrationAssociationArn": str,
         "InstanceId": str,
         "IntegrationType": IntegrationTypeType,
         "IntegrationArn": str,
         "SourceApplicationUrl": str,
         "SourceApplicationName": str,
         "SourceType": SourceTypeType,
     },
 )
 
+InvisibleFieldInfoOutputTypeDef = TypedDict(
+    "InvisibleFieldInfoOutputTypeDef",
+    {
+        "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
+    },
+)
+
 InvisibleFieldInfoTypeDef = TypedDict(
     "InvisibleFieldInfoTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
     total=False,
 )
 
+KinesisFirehoseConfigOutputTypeDef = TypedDict(
+    "KinesisFirehoseConfigOutputTypeDef",
+    {
+        "FirehoseArn": str,
+    },
+)
+
 KinesisFirehoseConfigTypeDef = TypedDict(
     "KinesisFirehoseConfigTypeDef",
     {
         "FirehoseArn": str,
     },
 )
 
+KinesisStreamConfigOutputTypeDef = TypedDict(
+    "KinesisStreamConfigOutputTypeDef",
+    {
+        "StreamArn": str,
+    },
+)
+
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "StreamArn": str,
     },
 )
 
+KinesisVideoStreamConfigOutputTypeDef = TypedDict(
+    "KinesisVideoStreamConfigOutputTypeDef",
+    {
+        "Prefix": str,
+        "RetentionPeriodHours": int,
+        "EncryptionConfig": "EncryptionConfigOutputTypeDef",
+    },
+)
+
 KinesisVideoStreamConfigTypeDef = TypedDict(
     "KinesisVideoStreamConfigTypeDef",
     {
         "Prefix": str,
         "RetentionPeriodHours": int,
         "EncryptionConfig": "EncryptionConfigTypeDef",
     },
 )
 
-LexBotConfigTypeDef = TypedDict(
-    "LexBotConfigTypeDef",
+LexBotConfigOutputTypeDef = TypedDict(
+    "LexBotConfigOutputTypeDef",
     {
-        "LexBot": "LexBotTypeDef",
-        "LexV2Bot": "LexV2BotTypeDef",
+        "LexBot": "LexBotOutputTypeDef",
+        "LexV2Bot": "LexV2BotOutputTypeDef",
+    },
+)
+
+LexBotOutputTypeDef = TypedDict(
+    "LexBotOutputTypeDef",
+    {
+        "Name": str,
+        "LexRegion": str,
     },
 )
 
 LexBotTypeDef = TypedDict(
     "LexBotTypeDef",
     {
         "Name": str,
         "LexRegion": str,
     },
 )
 
+LexV2BotOutputTypeDef = TypedDict(
+    "LexV2BotOutputTypeDef",
+    {
+        "AliasArn": str,
+    },
+)
+
 LexV2BotTypeDef = TypedDict(
     "LexV2BotTypeDef",
     {
         "AliasArn": str,
     },
     total=False,
 )
@@ -3414,20 +3802,22 @@
     {
         "AgentStatusTypes": Sequence[AgentStatusTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListAgentStatusRequestListAgentStatusesPaginateTypeDef(
     _RequiredListAgentStatusRequestListAgentStatusesPaginateTypeDef,
     _OptionalListAgentStatusRequestListAgentStatusesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAgentStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListAgentStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListAgentStatusRequestRequestTypeDef = TypedDict(
@@ -3436,24 +3826,26 @@
         "NextToken": str,
         "MaxResults": int,
         "AgentStatusTypes": Sequence[AgentStatusTypeType],
     },
     total=False,
 )
 
+
 class ListAgentStatusRequestRequestTypeDef(
     _RequiredListAgentStatusRequestRequestTypeDef, _OptionalListAgentStatusRequestRequestTypeDef
 ):
     pass
 
-ListAgentStatusResponseTypeDef = TypedDict(
-    "ListAgentStatusResponseTypeDef",
+
+ListAgentStatusResponseOutputTypeDef = TypedDict(
+    "ListAgentStatusResponseOutputTypeDef",
     {
         "NextToken": str,
-        "AgentStatusSummaryList": List["AgentStatusSummaryTypeDef"],
+        "AgentStatusSummaryList": List["AgentStatusSummaryOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef = TypedDict(
     "_RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     {
@@ -3464,20 +3856,22 @@
     "_OptionalListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef(
     _RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
     _OptionalListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListApprovedOriginsRequestRequestTypeDef = TypedDict(
     "_RequiredListApprovedOriginsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListApprovedOriginsRequestRequestTypeDef = TypedDict(
@@ -3485,22 +3879,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListApprovedOriginsRequestRequestTypeDef(
     _RequiredListApprovedOriginsRequestRequestTypeDef,
     _OptionalListApprovedOriginsRequestRequestTypeDef,
 ):
     pass
 
-ListApprovedOriginsResponseTypeDef = TypedDict(
-    "ListApprovedOriginsResponseTypeDef",
+
+ListApprovedOriginsResponseOutputTypeDef = TypedDict(
+    "ListApprovedOriginsResponseOutputTypeDef",
     {
         "Origins": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -3515,19 +3911,21 @@
     "_OptionalListBotsRequestListBotsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListBotsRequestListBotsPaginateTypeDef(
     _RequiredListBotsRequestListBotsPaginateTypeDef, _OptionalListBotsRequestListBotsPaginateTypeDef
 ):
     pass
 
+
 _RequiredListBotsRequestRequestTypeDef = TypedDict(
     "_RequiredListBotsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LexVersion": LexVersionType,
     },
 )
@@ -3536,23 +3934,25 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListBotsRequestRequestTypeDef(
     _RequiredListBotsRequestRequestTypeDef, _OptionalListBotsRequestRequestTypeDef
 ):
     pass
 
-ListBotsResponseTypeDef = TypedDict(
-    "ListBotsResponseTypeDef",
+
+ListBotsResponseOutputTypeDef = TypedDict(
+    "ListBotsResponseOutputTypeDef",
     {
-        "LexBots": List["LexBotConfigTypeDef"],
+        "LexBots": List["LexBotConfigOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef = TypedDict(
     "_RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
@@ -3565,20 +3965,22 @@
     "_OptionalListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef(
     _RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
     _OptionalListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListContactEvaluationsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactEvaluationsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
@@ -3586,24 +3988,26 @@
     "_OptionalListContactEvaluationsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListContactEvaluationsRequestRequestTypeDef(
     _RequiredListContactEvaluationsRequestRequestTypeDef,
     _OptionalListContactEvaluationsRequestRequestTypeDef,
 ):
     pass
 
-ListContactEvaluationsResponseTypeDef = TypedDict(
-    "ListContactEvaluationsResponseTypeDef",
+
+ListContactEvaluationsResponseOutputTypeDef = TypedDict(
+    "ListContactEvaluationsResponseOutputTypeDef",
     {
-        "EvaluationSummaryList": List["EvaluationSummaryTypeDef"],
+        "EvaluationSummaryList": List["EvaluationSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
@@ -3616,20 +4020,22 @@
     {
         "ContactFlowModuleState": ContactFlowModuleStateType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef(
     _RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
     _OptionalListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListContactFlowModulesRequestRequestTypeDef = TypedDict(
     "_RequiredListContactFlowModulesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowModulesRequestRequestTypeDef = TypedDict(
@@ -3638,24 +4044,26 @@
         "NextToken": str,
         "MaxResults": int,
         "ContactFlowModuleState": ContactFlowModuleStateType,
     },
     total=False,
 )
 
+
 class ListContactFlowModulesRequestRequestTypeDef(
     _RequiredListContactFlowModulesRequestRequestTypeDef,
     _OptionalListContactFlowModulesRequestRequestTypeDef,
 ):
     pass
 
-ListContactFlowModulesResponseTypeDef = TypedDict(
-    "ListContactFlowModulesResponseTypeDef",
+
+ListContactFlowModulesResponseOutputTypeDef = TypedDict(
+    "ListContactFlowModulesResponseOutputTypeDef",
     {
-        "ContactFlowModulesSummaryList": List["ContactFlowModuleSummaryTypeDef"],
+        "ContactFlowModulesSummaryList": List["ContactFlowModuleSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef",
@@ -3668,20 +4076,22 @@
     {
         "ContactFlowTypes": Sequence[ContactFlowTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListContactFlowsRequestListContactFlowsPaginateTypeDef(
     _RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef,
     _OptionalListContactFlowsRequestListContactFlowsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListContactFlowsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactFlowsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowsRequestRequestTypeDef = TypedDict(
@@ -3690,23 +4100,25 @@
         "ContactFlowTypes": Sequence[ContactFlowTypeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListContactFlowsRequestRequestTypeDef(
     _RequiredListContactFlowsRequestRequestTypeDef, _OptionalListContactFlowsRequestRequestTypeDef
 ):
     pass
 
-ListContactFlowsResponseTypeDef = TypedDict(
-    "ListContactFlowsResponseTypeDef",
+
+ListContactFlowsResponseOutputTypeDef = TypedDict(
+    "ListContactFlowsResponseOutputTypeDef",
     {
-        "ContactFlowSummaryList": List["ContactFlowSummaryTypeDef"],
+        "ContactFlowSummaryList": List["ContactFlowSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef = TypedDict(
     "_RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef",
@@ -3720,20 +4132,22 @@
     "_OptionalListContactReferencesRequestListContactReferencesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListContactReferencesRequestListContactReferencesPaginateTypeDef(
     _RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef,
     _OptionalListContactReferencesRequestListContactReferencesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListContactReferencesRequestRequestTypeDef = TypedDict(
     "_RequiredListContactReferencesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ReferenceTypes": Sequence[ReferenceTypeType],
     },
@@ -3742,24 +4156,26 @@
     "_OptionalListContactReferencesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListContactReferencesRequestRequestTypeDef(
     _RequiredListContactReferencesRequestRequestTypeDef,
     _OptionalListContactReferencesRequestRequestTypeDef,
 ):
     pass
 
-ListContactReferencesResponseTypeDef = TypedDict(
-    "ListContactReferencesResponseTypeDef",
+
+ListContactReferencesResponseOutputTypeDef = TypedDict(
+    "ListContactReferencesResponseOutputTypeDef",
     {
-        "ReferenceSummaryList": List["ReferenceSummaryTypeDef"],
+        "ReferenceSummaryList": List["ReferenceSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef = TypedDict(
     "_RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef",
@@ -3772,20 +4188,22 @@
     {
         "LanguageCode": VocabularyLanguageCodeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef(
     _RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
     _OptionalListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDefaultVocabulariesRequestRequestTypeDef = TypedDict(
     "_RequiredListDefaultVocabulariesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListDefaultVocabulariesRequestRequestTypeDef = TypedDict(
@@ -3794,24 +4212,26 @@
         "LanguageCode": VocabularyLanguageCodeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDefaultVocabulariesRequestRequestTypeDef(
     _RequiredListDefaultVocabulariesRequestRequestTypeDef,
     _OptionalListDefaultVocabulariesRequestRequestTypeDef,
 ):
     pass
 
-ListDefaultVocabulariesResponseTypeDef = TypedDict(
-    "ListDefaultVocabulariesResponseTypeDef",
+
+ListDefaultVocabulariesResponseOutputTypeDef = TypedDict(
+    "ListDefaultVocabulariesResponseOutputTypeDef",
     {
-        "DefaultVocabularyList": List["DefaultVocabularyTypeDef"],
+        "DefaultVocabularyList": List["DefaultVocabularyOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
@@ -3824,20 +4244,22 @@
     "_OptionalListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef(
     _RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
     _OptionalListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListEvaluationFormVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListEvaluationFormVersionsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
     },
 )
@@ -3846,24 +4268,26 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListEvaluationFormVersionsRequestRequestTypeDef(
     _RequiredListEvaluationFormVersionsRequestRequestTypeDef,
     _OptionalListEvaluationFormVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListEvaluationFormVersionsResponseTypeDef = TypedDict(
-    "ListEvaluationFormVersionsResponseTypeDef",
+
+ListEvaluationFormVersionsResponseOutputTypeDef = TypedDict(
+    "ListEvaluationFormVersionsResponseOutputTypeDef",
     {
-        "EvaluationFormVersionSummaryList": List["EvaluationFormVersionSummaryTypeDef"],
+        "EvaluationFormVersionSummaryList": List["EvaluationFormVersionSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
@@ -3875,20 +4299,22 @@
     "_OptionalListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef(
     _RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
     _OptionalListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListEvaluationFormsRequestRequestTypeDef = TypedDict(
     "_RequiredListEvaluationFormsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListEvaluationFormsRequestRequestTypeDef = TypedDict(
@@ -3896,24 +4322,26 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListEvaluationFormsRequestRequestTypeDef(
     _RequiredListEvaluationFormsRequestRequestTypeDef,
     _OptionalListEvaluationFormsRequestRequestTypeDef,
 ):
     pass
 
-ListEvaluationFormsResponseTypeDef = TypedDict(
-    "ListEvaluationFormsResponseTypeDef",
+
+ListEvaluationFormsResponseOutputTypeDef = TypedDict(
+    "ListEvaluationFormsResponseOutputTypeDef",
     {
-        "EvaluationFormSummaryList": List["EvaluationFormSummaryTypeDef"],
+        "EvaluationFormSummaryList": List["EvaluationFormSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef = TypedDict(
     "_RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
@@ -3925,20 +4353,22 @@
     "_OptionalListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef(
     _RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
     _OptionalListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListHoursOfOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListHoursOfOperationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListHoursOfOperationsRequestRequestTypeDef = TypedDict(
@@ -3946,24 +4376,26 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListHoursOfOperationsRequestRequestTypeDef(
     _RequiredListHoursOfOperationsRequestRequestTypeDef,
     _OptionalListHoursOfOperationsRequestRequestTypeDef,
 ):
     pass
 
-ListHoursOfOperationsResponseTypeDef = TypedDict(
-    "ListHoursOfOperationsResponseTypeDef",
+
+ListHoursOfOperationsResponseOutputTypeDef = TypedDict(
+    "ListHoursOfOperationsResponseOutputTypeDef",
     {
-        "HoursOfOperationSummaryList": List["HoursOfOperationSummaryTypeDef"],
+        "HoursOfOperationSummaryList": List["HoursOfOperationSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef = TypedDict(
     "_RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
@@ -3975,20 +4407,22 @@
     "_OptionalListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef(
     _RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
     _OptionalListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInstanceAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListInstanceAttributesRequestRequestTypeDef = TypedDict(
@@ -3996,24 +4430,26 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListInstanceAttributesRequestRequestTypeDef(
     _RequiredListInstanceAttributesRequestRequestTypeDef,
     _OptionalListInstanceAttributesRequestRequestTypeDef,
 ):
     pass
 
-ListInstanceAttributesResponseTypeDef = TypedDict(
-    "ListInstanceAttributesResponseTypeDef",
+
+ListInstanceAttributesResponseOutputTypeDef = TypedDict(
+    "ListInstanceAttributesResponseOutputTypeDef",
     {
-        "Attributes": List["AttributeTypeDef"],
+        "Attributes": List["AttributeOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef = TypedDict(
     "_RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
@@ -4026,20 +4462,22 @@
     "_OptionalListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef(
     _RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
     _OptionalListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInstanceStorageConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceStorageConfigsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
 )
@@ -4048,24 +4486,26 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListInstanceStorageConfigsRequestRequestTypeDef(
     _RequiredListInstanceStorageConfigsRequestRequestTypeDef,
     _OptionalListInstanceStorageConfigsRequestRequestTypeDef,
 ):
     pass
 
-ListInstanceStorageConfigsResponseTypeDef = TypedDict(
-    "ListInstanceStorageConfigsResponseTypeDef",
+
+ListInstanceStorageConfigsResponseOutputTypeDef = TypedDict(
+    "ListInstanceStorageConfigsResponseOutputTypeDef",
     {
-        "StorageConfigs": List["InstanceStorageConfigTypeDef"],
+        "StorageConfigs": List["InstanceStorageConfigOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
     "ListInstancesRequestListInstancesPaginateTypeDef",
@@ -4080,18 +4520,18 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListInstancesResponseTypeDef = TypedDict(
-    "ListInstancesResponseTypeDef",
+ListInstancesResponseOutputTypeDef = TypedDict(
+    "ListInstancesResponseOutputTypeDef",
     {
-        "InstanceSummaryList": List["InstanceSummaryTypeDef"],
+        "InstanceSummaryList": List["InstanceSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef = TypedDict(
     "_RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef",
@@ -4104,20 +4544,22 @@
     {
         "IntegrationType": IntegrationTypeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef(
     _RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
     _OptionalListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListIntegrationAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListIntegrationAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListIntegrationAssociationsRequestRequestTypeDef = TypedDict(
@@ -4126,24 +4568,26 @@
         "IntegrationType": IntegrationTypeType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-ListIntegrationAssociationsResponseTypeDef = TypedDict(
-    "ListIntegrationAssociationsResponseTypeDef",
+
+ListIntegrationAssociationsResponseOutputTypeDef = TypedDict(
+    "ListIntegrationAssociationsResponseOutputTypeDef",
     {
-        "IntegrationAssociationSummaryList": List["IntegrationAssociationSummaryTypeDef"],
+        "IntegrationAssociationSummaryList": List["IntegrationAssociationSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef = TypedDict(
     "_RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
@@ -4155,20 +4599,22 @@
     "_OptionalListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef(
     _RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
     _OptionalListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListLambdaFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLambdaFunctionsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLambdaFunctionsRequestRequestTypeDef = TypedDict(
@@ -4176,22 +4622,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListLambdaFunctionsRequestRequestTypeDef(
     _RequiredListLambdaFunctionsRequestRequestTypeDef,
     _OptionalListLambdaFunctionsRequestRequestTypeDef,
 ):
     pass
 
-ListLambdaFunctionsResponseTypeDef = TypedDict(
-    "ListLambdaFunctionsResponseTypeDef",
+
+ListLambdaFunctionsResponseOutputTypeDef = TypedDict(
+    "ListLambdaFunctionsResponseOutputTypeDef",
     {
         "LambdaFunctions": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4205,20 +4653,22 @@
     "_OptionalListLexBotsRequestListLexBotsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListLexBotsRequestListLexBotsPaginateTypeDef(
     _RequiredListLexBotsRequestListLexBotsPaginateTypeDef,
     _OptionalListLexBotsRequestListLexBotsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListLexBotsRequestRequestTypeDef = TypedDict(
     "_RequiredListLexBotsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLexBotsRequestRequestTypeDef = TypedDict(
@@ -4226,23 +4676,25 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListLexBotsRequestRequestTypeDef(
     _RequiredListLexBotsRequestRequestTypeDef, _OptionalListLexBotsRequestRequestTypeDef
 ):
     pass
 
-ListLexBotsResponseTypeDef = TypedDict(
-    "ListLexBotsResponseTypeDef",
+
+ListLexBotsResponseOutputTypeDef = TypedDict(
+    "ListLexBotsResponseOutputTypeDef",
     {
-        "LexBots": List["LexBotTypeDef"],
+        "LexBots": List["LexBotOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef = TypedDict(
     "_RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef",
@@ -4256,20 +4708,22 @@
         "PhoneNumberTypes": Sequence[PhoneNumberTypeType],
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef(
     _RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
     _OptionalListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListPhoneNumbersRequestRequestTypeDef = TypedDict(
     "_RequiredListPhoneNumbersRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListPhoneNumbersRequestRequestTypeDef = TypedDict(
@@ -4279,30 +4733,32 @@
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListPhoneNumbersRequestRequestTypeDef(
     _RequiredListPhoneNumbersRequestRequestTypeDef, _OptionalListPhoneNumbersRequestRequestTypeDef
 ):
     pass
 
-ListPhoneNumbersResponseTypeDef = TypedDict(
-    "ListPhoneNumbersResponseTypeDef",
+
+ListPhoneNumbersResponseOutputTypeDef = TypedDict(
+    "ListPhoneNumbersResponseOutputTypeDef",
     {
-        "PhoneNumberSummaryList": List["PhoneNumberSummaryTypeDef"],
+        "PhoneNumberSummaryList": List["PhoneNumberSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPhoneNumbersSummaryTypeDef = TypedDict(
-    "ListPhoneNumbersSummaryTypeDef",
+ListPhoneNumbersSummaryOutputTypeDef = TypedDict(
+    "ListPhoneNumbersSummaryOutputTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "TargetArn": str,
@@ -4330,19 +4786,19 @@
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "PhoneNumberTypes": Sequence[PhoneNumberTypeType],
         "PhoneNumberPrefix": str,
     },
     total=False,
 )
 
-ListPhoneNumbersV2ResponseTypeDef = TypedDict(
-    "ListPhoneNumbersV2ResponseTypeDef",
+ListPhoneNumbersV2ResponseOutputTypeDef = TypedDict(
+    "ListPhoneNumbersV2ResponseOutputTypeDef",
     {
         "NextToken": str,
-        "ListPhoneNumbersSummaryList": List["ListPhoneNumbersSummaryTypeDef"],
+        "ListPhoneNumbersSummaryList": List["ListPhoneNumbersSummaryOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListPromptsRequestListPromptsPaginateTypeDef = TypedDict(
     "_RequiredListPromptsRequestListPromptsPaginateTypeDef",
     {
@@ -4353,20 +4809,22 @@
     "_OptionalListPromptsRequestListPromptsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListPromptsRequestListPromptsPaginateTypeDef(
     _RequiredListPromptsRequestListPromptsPaginateTypeDef,
     _OptionalListPromptsRequestListPromptsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListPromptsRequestRequestTypeDef = TypedDict(
     "_RequiredListPromptsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListPromptsRequestRequestTypeDef = TypedDict(
@@ -4374,23 +4832,25 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListPromptsRequestRequestTypeDef(
     _RequiredListPromptsRequestRequestTypeDef, _OptionalListPromptsRequestRequestTypeDef
 ):
     pass
 
-ListPromptsResponseTypeDef = TypedDict(
-    "ListPromptsResponseTypeDef",
+
+ListPromptsResponseOutputTypeDef = TypedDict(
+    "ListPromptsResponseOutputTypeDef",
     {
-        "PromptSummaryList": List["PromptSummaryTypeDef"],
+        "PromptSummaryList": List["PromptSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
@@ -4403,20 +4863,22 @@
     "_OptionalListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef(
     _RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
     _OptionalListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListQueueQuickConnectsRequestRequestTypeDef = TypedDict(
     "_RequiredListQueueQuickConnectsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
@@ -4425,25 +4887,27 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListQueueQuickConnectsRequestRequestTypeDef(
     _RequiredListQueueQuickConnectsRequestRequestTypeDef,
     _OptionalListQueueQuickConnectsRequestRequestTypeDef,
 ):
     pass
 
-ListQueueQuickConnectsResponseTypeDef = TypedDict(
-    "ListQueueQuickConnectsResponseTypeDef",
+
+ListQueueQuickConnectsResponseOutputTypeDef = TypedDict(
+    "ListQueueQuickConnectsResponseOutputTypeDef",
     {
         "NextToken": str,
-        "QuickConnectSummaryList": List["QuickConnectSummaryTypeDef"],
+        "QuickConnectSummaryList": List["QuickConnectSummaryOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
     "_RequiredListQueuesRequestListQueuesPaginateTypeDef",
     {
@@ -4455,20 +4919,22 @@
     {
         "QueueTypes": Sequence[QueueTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListQueuesRequestListQueuesPaginateTypeDef(
     _RequiredListQueuesRequestListQueuesPaginateTypeDef,
     _OptionalListQueuesRequestListQueuesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListQueuesRequestRequestTypeDef = TypedDict(
@@ -4477,23 +4943,25 @@
         "QueueTypes": Sequence[QueueTypeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListQueuesRequestRequestTypeDef(
     _RequiredListQueuesRequestRequestTypeDef, _OptionalListQueuesRequestRequestTypeDef
 ):
     pass
 
-ListQueuesResponseTypeDef = TypedDict(
-    "ListQueuesResponseTypeDef",
+
+ListQueuesResponseOutputTypeDef = TypedDict(
+    "ListQueuesResponseOutputTypeDef",
     {
-        "QueueSummaryList": List["QueueSummaryTypeDef"],
+        "QueueSummaryList": List["QueueSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef",
@@ -4506,20 +4974,22 @@
     {
         "QuickConnectTypes": Sequence[QuickConnectTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListQuickConnectsRequestListQuickConnectsPaginateTypeDef(
     _RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
     _OptionalListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListQuickConnectsRequestRequestTypeDef = TypedDict(
     "_RequiredListQuickConnectsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListQuickConnectsRequestRequestTypeDef = TypedDict(
@@ -4528,23 +4998,25 @@
         "NextToken": str,
         "MaxResults": int,
         "QuickConnectTypes": Sequence[QuickConnectTypeType],
     },
     total=False,
 )
 
+
 class ListQuickConnectsRequestRequestTypeDef(
     _RequiredListQuickConnectsRequestRequestTypeDef, _OptionalListQuickConnectsRequestRequestTypeDef
 ):
     pass
 
-ListQuickConnectsResponseTypeDef = TypedDict(
-    "ListQuickConnectsResponseTypeDef",
+
+ListQuickConnectsResponseOutputTypeDef = TypedDict(
+    "ListQuickConnectsResponseOutputTypeDef",
     {
-        "QuickConnectSummaryList": List["QuickConnectSummaryTypeDef"],
+        "QuickConnectSummaryList": List["QuickConnectSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
@@ -4557,20 +5029,22 @@
     "_OptionalListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef(
     _RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
     _OptionalListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListRoutingProfileQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutingProfileQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
     },
 )
@@ -4579,25 +5053,29 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListRoutingProfileQueuesRequestRequestTypeDef(
     _RequiredListRoutingProfileQueuesRequestRequestTypeDef,
     _OptionalListRoutingProfileQueuesRequestRequestTypeDef,
 ):
     pass
 
-ListRoutingProfileQueuesResponseTypeDef = TypedDict(
-    "ListRoutingProfileQueuesResponseTypeDef",
+
+ListRoutingProfileQueuesResponseOutputTypeDef = TypedDict(
+    "ListRoutingProfileQueuesResponseOutputTypeDef",
     {
         "NextToken": str,
-        "RoutingProfileQueueConfigSummaryList": List["RoutingProfileQueueConfigSummaryTypeDef"],
+        "RoutingProfileQueueConfigSummaryList": List[
+            "RoutingProfileQueueConfigSummaryOutputTypeDef"
+        ],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     {
@@ -4608,20 +5086,22 @@
     "_OptionalListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef(
     _RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
     _OptionalListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListRoutingProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutingProfilesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListRoutingProfilesRequestRequestTypeDef = TypedDict(
@@ -4629,24 +5109,26 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListRoutingProfilesRequestRequestTypeDef(
     _RequiredListRoutingProfilesRequestRequestTypeDef,
     _OptionalListRoutingProfilesRequestRequestTypeDef,
 ):
     pass
 
-ListRoutingProfilesResponseTypeDef = TypedDict(
-    "ListRoutingProfilesResponseTypeDef",
+
+ListRoutingProfilesResponseOutputTypeDef = TypedDict(
+    "ListRoutingProfilesResponseOutputTypeDef",
     {
-        "RoutingProfileSummaryList": List["RoutingProfileSummaryTypeDef"],
+        "RoutingProfileSummaryList": List["RoutingProfileSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
     "_RequiredListRulesRequestListRulesPaginateTypeDef",
@@ -4660,20 +5142,22 @@
         "PublishStatus": RulePublishStatusType,
         "EventSourceName": EventSourceNameType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListRulesRequestListRulesPaginateTypeDef(
     _RequiredListRulesRequestListRulesPaginateTypeDef,
     _OptionalListRulesRequestListRulesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListRulesRequestRequestTypeDef = TypedDict(
@@ -4683,23 +5167,25 @@
         "EventSourceName": EventSourceNameType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListRulesRequestRequestTypeDef(
     _RequiredListRulesRequestRequestTypeDef, _OptionalListRulesRequestRequestTypeDef
 ):
     pass
 
-ListRulesResponseTypeDef = TypedDict(
-    "ListRulesResponseTypeDef",
+
+ListRulesResponseOutputTypeDef = TypedDict(
+    "ListRulesResponseOutputTypeDef",
     {
-        "RuleSummaryList": List["RuleSummaryTypeDef"],
+        "RuleSummaryList": List["RuleSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef = TypedDict(
     "_RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
@@ -4711,20 +5197,22 @@
     "_OptionalListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListSecurityKeysRequestListSecurityKeysPaginateTypeDef(
     _RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
     _OptionalListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListSecurityKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityKeysRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityKeysRequestRequestTypeDef = TypedDict(
@@ -4732,23 +5220,25 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListSecurityKeysRequestRequestTypeDef(
     _RequiredListSecurityKeysRequestRequestTypeDef, _OptionalListSecurityKeysRequestRequestTypeDef
 ):
     pass
 
-ListSecurityKeysResponseTypeDef = TypedDict(
-    "ListSecurityKeysResponseTypeDef",
+
+ListSecurityKeysResponseOutputTypeDef = TypedDict(
+    "ListSecurityKeysResponseOutputTypeDef",
     {
-        "SecurityKeys": List["SecurityKeyTypeDef"],
+        "SecurityKeys": List["SecurityKeyOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef = TypedDict(
     "_RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
@@ -4761,20 +5251,22 @@
     "_OptionalListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef(
     _RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
     _OptionalListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListSecurityProfilePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityProfilePermissionsRequestRequestTypeDef",
     {
         "SecurityProfileId": str,
         "InstanceId": str,
     },
 )
@@ -4783,22 +5275,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListSecurityProfilePermissionsRequestRequestTypeDef(
     _RequiredListSecurityProfilePermissionsRequestRequestTypeDef,
     _OptionalListSecurityProfilePermissionsRequestRequestTypeDef,
 ):
     pass
 
-ListSecurityProfilePermissionsResponseTypeDef = TypedDict(
-    "ListSecurityProfilePermissionsResponseTypeDef",
+
+ListSecurityProfilePermissionsResponseOutputTypeDef = TypedDict(
+    "ListSecurityProfilePermissionsResponseOutputTypeDef",
     {
         "Permissions": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4812,20 +5306,22 @@
     "_OptionalListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef(
     _RequiredListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     _OptionalListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListSecurityProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityProfilesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityProfilesRequestRequestTypeDef = TypedDict(
@@ -4833,38 +5329,40 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListSecurityProfilesRequestRequestTypeDef(
     _RequiredListSecurityProfilesRequestRequestTypeDef,
     _OptionalListSecurityProfilesRequestRequestTypeDef,
 ):
     pass
 
-ListSecurityProfilesResponseTypeDef = TypedDict(
-    "ListSecurityProfilesResponseTypeDef",
+
+ListSecurityProfilesResponseOutputTypeDef = TypedDict(
+    "ListSecurityProfilesResponseOutputTypeDef",
     {
-        "SecurityProfileSummaryList": List["SecurityProfileSummaryTypeDef"],
+        "SecurityProfileSummaryList": List["SecurityProfileSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef = TypedDict(
@@ -4879,20 +5377,22 @@
         "Status": TaskTemplateStatusType,
         "Name": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef(
     _RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
     _OptionalListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTaskTemplatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTaskTemplatesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListTaskTemplatesRequestRequestTypeDef = TypedDict(
@@ -4902,23 +5402,25 @@
         "MaxResults": int,
         "Status": TaskTemplateStatusType,
         "Name": str,
     },
     total=False,
 )
 
+
 class ListTaskTemplatesRequestRequestTypeDef(
     _RequiredListTaskTemplatesRequestRequestTypeDef, _OptionalListTaskTemplatesRequestRequestTypeDef
 ):
     pass
 
-ListTaskTemplatesResponseTypeDef = TypedDict(
-    "ListTaskTemplatesResponseTypeDef",
+
+ListTaskTemplatesResponseOutputTypeDef = TypedDict(
+    "ListTaskTemplatesResponseOutputTypeDef",
     {
-        "TaskTemplates": List["TaskTemplateMetadataTypeDef"],
+        "TaskTemplates": List["TaskTemplateMetadataOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef = TypedDict(
     "ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef",
@@ -4935,19 +5437,19 @@
         "MaxResults": int,
         "NextToken": str,
         "InstanceId": str,
     },
     total=False,
 )
 
-ListTrafficDistributionGroupsResponseTypeDef = TypedDict(
-    "ListTrafficDistributionGroupsResponseTypeDef",
+ListTrafficDistributionGroupsResponseOutputTypeDef = TypedDict(
+    "ListTrafficDistributionGroupsResponseOutputTypeDef",
     {
         "NextToken": str,
-        "TrafficDistributionGroupSummaryList": List["TrafficDistributionGroupSummaryTypeDef"],
+        "TrafficDistributionGroupSummaryList": List["TrafficDistributionGroupSummaryOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUseCasesRequestListUseCasesPaginateTypeDef = TypedDict(
     "_RequiredListUseCasesRequestListUseCasesPaginateTypeDef",
     {
@@ -4959,20 +5461,22 @@
     "_OptionalListUseCasesRequestListUseCasesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListUseCasesRequestListUseCasesPaginateTypeDef(
     _RequiredListUseCasesRequestListUseCasesPaginateTypeDef,
     _OptionalListUseCasesRequestListUseCasesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListUseCasesRequestRequestTypeDef = TypedDict(
     "_RequiredListUseCasesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IntegrationAssociationId": str,
     },
 )
@@ -4981,23 +5485,25 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListUseCasesRequestRequestTypeDef(
     _RequiredListUseCasesRequestRequestTypeDef, _OptionalListUseCasesRequestRequestTypeDef
 ):
     pass
 
-ListUseCasesResponseTypeDef = TypedDict(
-    "ListUseCasesResponseTypeDef",
+
+ListUseCasesResponseOutputTypeDef = TypedDict(
+    "ListUseCasesResponseOutputTypeDef",
     {
-        "UseCaseSummaryList": List["UseCaseTypeDef"],
+        "UseCaseSummaryList": List["UseCaseOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef = TypedDict(
     "_RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
@@ -5009,20 +5515,22 @@
     "_OptionalListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef(
     _RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
     _OptionalListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListUserHierarchyGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserHierarchyGroupsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListUserHierarchyGroupsRequestRequestTypeDef = TypedDict(
@@ -5030,24 +5538,26 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListUserHierarchyGroupsRequestRequestTypeDef(
     _RequiredListUserHierarchyGroupsRequestRequestTypeDef,
     _OptionalListUserHierarchyGroupsRequestRequestTypeDef,
 ):
     pass
 
-ListUserHierarchyGroupsResponseTypeDef = TypedDict(
-    "ListUserHierarchyGroupsResponseTypeDef",
+
+ListUserHierarchyGroupsResponseOutputTypeDef = TypedDict(
+    "ListUserHierarchyGroupsResponseOutputTypeDef",
     {
-        "UserHierarchyGroupSummaryList": List["HierarchyGroupSummaryTypeDef"],
+        "UserHierarchyGroupSummaryList": List["HierarchyGroupSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
@@ -5059,20 +5569,22 @@
     "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -5080,28 +5592,39 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-ListUsersResponseTypeDef = TypedDict(
-    "ListUsersResponseTypeDef",
+
+ListUsersResponseOutputTypeDef = TypedDict(
+    "ListUsersResponseOutputTypeDef",
     {
-        "UserSummaryList": List["UserSummaryTypeDef"],
+        "UserSummaryList": List["UserSummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MediaConcurrencyOutputTypeDef = TypedDict(
+    "MediaConcurrencyOutputTypeDef",
+    {
+        "Channel": ChannelType,
+        "Concurrency": int,
+        "CrossChannelBehavior": "CrossChannelBehaviorOutputTypeDef",
+    },
+)
+
 _RequiredMediaConcurrencyTypeDef = TypedDict(
     "_RequiredMediaConcurrencyTypeDef",
     {
         "Channel": ChannelType,
         "Concurrency": int,
     },
 )
@@ -5109,39 +5632,58 @@
     "_OptionalMediaConcurrencyTypeDef",
     {
         "CrossChannelBehavior": "CrossChannelBehaviorTypeDef",
     },
     total=False,
 )
 
+
 class MediaConcurrencyTypeDef(_RequiredMediaConcurrencyTypeDef, _OptionalMediaConcurrencyTypeDef):
     pass
 
-MetricDataV2TypeDef = TypedDict(
-    "MetricDataV2TypeDef",
+
+MetricDataV2OutputTypeDef = TypedDict(
+    "MetricDataV2OutputTypeDef",
     {
-        "Metric": "MetricV2TypeDef",
+        "Metric": "MetricV2OutputTypeDef",
         "Value": float,
     },
 )
 
+MetricFilterV2OutputTypeDef = TypedDict(
+    "MetricFilterV2OutputTypeDef",
+    {
+        "MetricFilterKey": str,
+        "MetricFilterValues": List[str],
+    },
+)
+
 MetricFilterV2TypeDef = TypedDict(
     "MetricFilterV2TypeDef",
     {
         "MetricFilterKey": str,
         "MetricFilterValues": Sequence[str],
     },
     total=False,
 )
 
-MetricResultV2TypeDef = TypedDict(
-    "MetricResultV2TypeDef",
+MetricResultV2OutputTypeDef = TypedDict(
+    "MetricResultV2OutputTypeDef",
     {
         "Dimensions": Dict[str, str],
-        "Collections": List["MetricDataV2TypeDef"],
+        "Collections": List["MetricDataV2OutputTypeDef"],
+    },
+)
+
+MetricV2OutputTypeDef = TypedDict(
+    "MetricV2OutputTypeDef",
+    {
+        "Name": str,
+        "Threshold": List["ThresholdV2OutputTypeDef"],
+        "MetricFilters": List["MetricFilterV2OutputTypeDef"],
     },
 )
 
 MetricV2TypeDef = TypedDict(
     "MetricV2TypeDef",
     {
         "Name": str,
@@ -5164,52 +5706,78 @@
     {
         "AllowedMonitorCapabilities": Sequence[MonitorCapabilityType],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class MonitorContactRequestRequestTypeDef(
     _RequiredMonitorContactRequestRequestTypeDef, _OptionalMonitorContactRequestRequestTypeDef
 ):
     pass
 
-MonitorContactResponseTypeDef = TypedDict(
-    "MonitorContactResponseTypeDef",
+
+MonitorContactResponseOutputTypeDef = TypedDict(
+    "MonitorContactResponseOutputTypeDef",
     {
         "ContactId": str,
         "ContactArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+NotificationRecipientTypeOutputTypeDef = TypedDict(
+    "NotificationRecipientTypeOutputTypeDef",
+    {
+        "UserTags": Dict[str, str],
+        "UserIds": List[str],
+    },
+)
+
 NotificationRecipientTypeTypeDef = TypedDict(
     "NotificationRecipientTypeTypeDef",
     {
         "UserTags": Mapping[str, str],
         "UserIds": Sequence[str],
     },
     total=False,
 )
 
-NumberReferenceTypeDef = TypedDict(
-    "NumberReferenceTypeDef",
+NumberReferenceOutputTypeDef = TypedDict(
+    "NumberReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+NumericQuestionPropertyValueAutomationOutputTypeDef = TypedDict(
+    "NumericQuestionPropertyValueAutomationOutputTypeDef",
+    {
+        "Label": NumericQuestionPropertyAutomationLabelType,
+    },
+)
+
 NumericQuestionPropertyValueAutomationTypeDef = TypedDict(
     "NumericQuestionPropertyValueAutomationTypeDef",
     {
         "Label": NumericQuestionPropertyAutomationLabelType,
     },
 )
 
+OutboundCallerConfigOutputTypeDef = TypedDict(
+    "OutboundCallerConfigOutputTypeDef",
+    {
+        "OutboundCallerIdName": str,
+        "OutboundCallerIdNumberId": str,
+        "OutboundFlowId": str,
+    },
+)
+
 OutboundCallerConfigTypeDef = TypedDict(
     "OutboundCallerConfigTypeDef",
     {
         "OutboundCallerIdName": str,
         "OutboundCallerIdNumberId": str,
         "OutboundFlowId": str,
     },
@@ -5256,16 +5824,16 @@
     {
         "ParticipantTimerAction": Literal["Unset"],
         "ParticipantTimerDurationInMinutes": int,
     },
     total=False,
 )
 
-ParticipantTokenCredentialsTypeDef = TypedDict(
-    "ParticipantTokenCredentialsTypeDef",
+ParticipantTokenCredentialsOutputTypeDef = TypedDict(
+    "ParticipantTokenCredentialsOutputTypeDef",
     {
         "ParticipantToken": str,
         "Expiry": str,
     },
 )
 
 PersistentChatTypeDef = TypedDict(
@@ -5273,40 +5841,58 @@
     {
         "RehydrationType": RehydrationTypeType,
         "SourceContactId": str,
     },
     total=False,
 )
 
+PhoneNumberQuickConnectConfigOutputTypeDef = TypedDict(
+    "PhoneNumberQuickConnectConfigOutputTypeDef",
+    {
+        "PhoneNumber": str,
+    },
+)
+
 PhoneNumberQuickConnectConfigTypeDef = TypedDict(
     "PhoneNumberQuickConnectConfigTypeDef",
     {
         "PhoneNumber": str,
     },
 )
 
-PhoneNumberStatusTypeDef = TypedDict(
-    "PhoneNumberStatusTypeDef",
+PhoneNumberStatusOutputTypeDef = TypedDict(
+    "PhoneNumberStatusOutputTypeDef",
     {
         "Status": PhoneNumberWorkflowStatusType,
         "Message": str,
     },
 )
 
-PhoneNumberSummaryTypeDef = TypedDict(
-    "PhoneNumberSummaryTypeDef",
+PhoneNumberSummaryOutputTypeDef = TypedDict(
+    "PhoneNumberSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PhoneNumber": str,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
     },
 )
 
+PromptOutputTypeDef = TypedDict(
+    "PromptOutputTypeDef",
+    {
+        "PromptARN": str,
+        "PromptId": str,
+        "Name": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+    },
+)
+
 PromptSearchCriteriaTypeDef = TypedDict(
     "PromptSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
@@ -5317,61 +5903,73 @@
     "PromptSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-PromptSummaryTypeDef = TypedDict(
-    "PromptSummaryTypeDef",
+PromptSummaryOutputTypeDef = TypedDict(
+    "PromptSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
-PromptTypeDef = TypedDict(
-    "PromptTypeDef",
-    {
-        "PromptARN": str,
-        "PromptId": str,
-        "Name": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-    },
-)
-
 PutUserStatusRequestRequestTypeDef = TypedDict(
     "PutUserStatusRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
         "AgentStatusId": str,
     },
 )
 
-QueueInfoTypeDef = TypedDict(
-    "QueueInfoTypeDef",
+QueueInfoOutputTypeDef = TypedDict(
+    "QueueInfoOutputTypeDef",
     {
         "Id": str,
         "EnqueueTimestamp": datetime,
     },
 )
 
+QueueOutputTypeDef = TypedDict(
+    "QueueOutputTypeDef",
+    {
+        "Name": str,
+        "QueueArn": str,
+        "QueueId": str,
+        "Description": str,
+        "OutboundCallerConfig": "OutboundCallerConfigOutputTypeDef",
+        "HoursOfOperationId": str,
+        "MaxContacts": int,
+        "Status": QueueStatusType,
+        "Tags": Dict[str, str],
+    },
+)
+
+QueueQuickConnectConfigOutputTypeDef = TypedDict(
+    "QueueQuickConnectConfigOutputTypeDef",
+    {
+        "QueueId": str,
+        "ContactFlowId": str,
+    },
+)
+
 QueueQuickConnectConfigTypeDef = TypedDict(
     "QueueQuickConnectConfigTypeDef",
     {
         "QueueId": str,
         "ContactFlowId": str,
     },
 )
 
-QueueReferenceTypeDef = TypedDict(
-    "QueueReferenceTypeDef",
+QueueReferenceOutputTypeDef = TypedDict(
+    "QueueReferenceOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 QueueSearchCriteriaTypeDef = TypedDict(
@@ -5389,36 +5987,31 @@
     "QueueSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-QueueSummaryTypeDef = TypedDict(
-    "QueueSummaryTypeDef",
+QueueSummaryOutputTypeDef = TypedDict(
+    "QueueSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QueueType": QueueTypeType,
     },
 )
 
-QueueTypeDef = TypedDict(
-    "QueueTypeDef",
+QuickConnectConfigOutputTypeDef = TypedDict(
+    "QuickConnectConfigOutputTypeDef",
     {
-        "Name": str,
-        "QueueArn": str,
-        "QueueId": str,
-        "Description": str,
-        "OutboundCallerConfig": "OutboundCallerConfigTypeDef",
-        "HoursOfOperationId": str,
-        "MaxContacts": int,
-        "Status": QueueStatusType,
-        "Tags": Dict[str, str],
+        "QuickConnectType": QuickConnectTypeType,
+        "UserConfig": "UserQuickConnectConfigOutputTypeDef",
+        "QueueConfig": "QueueQuickConnectConfigOutputTypeDef",
+        "PhoneConfig": "PhoneNumberQuickConnectConfigOutputTypeDef",
     },
 )
 
 _RequiredQuickConnectConfigTypeDef = TypedDict(
     "_RequiredQuickConnectConfigTypeDef",
     {
         "QuickConnectType": QuickConnectTypeType,
@@ -5430,19 +6023,33 @@
         "UserConfig": "UserQuickConnectConfigTypeDef",
         "QueueConfig": "QueueQuickConnectConfigTypeDef",
         "PhoneConfig": "PhoneNumberQuickConnectConfigTypeDef",
     },
     total=False,
 )
 
+
 class QuickConnectConfigTypeDef(
     _RequiredQuickConnectConfigTypeDef, _OptionalQuickConnectConfigTypeDef
 ):
     pass
 
+
+QuickConnectOutputTypeDef = TypedDict(
+    "QuickConnectOutputTypeDef",
+    {
+        "QuickConnectARN": str,
+        "QuickConnectId": str,
+        "Name": str,
+        "Description": str,
+        "QuickConnectConfig": "QuickConnectConfigOutputTypeDef",
+        "Tags": Dict[str, str],
+    },
+)
+
 QuickConnectSearchCriteriaTypeDef = TypedDict(
     "QuickConnectSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
@@ -5453,53 +6060,56 @@
     "QuickConnectSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-QuickConnectSummaryTypeDef = TypedDict(
-    "QuickConnectSummaryTypeDef",
+QuickConnectSummaryOutputTypeDef = TypedDict(
+    "QuickConnectSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QuickConnectType": QuickConnectTypeType,
     },
 )
 
-QuickConnectTypeDef = TypedDict(
-    "QuickConnectTypeDef",
+ReadOnlyFieldInfoOutputTypeDef = TypedDict(
+    "ReadOnlyFieldInfoOutputTypeDef",
     {
-        "QuickConnectARN": str,
-        "QuickConnectId": str,
-        "Name": str,
-        "Description": str,
-        "QuickConnectConfig": "QuickConnectConfigTypeDef",
-        "Tags": Dict[str, str],
+        "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
     },
 )
 
 ReadOnlyFieldInfoTypeDef = TypedDict(
     "ReadOnlyFieldInfoTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
     total=False,
 )
 
-ReferenceSummaryTypeDef = TypedDict(
-    "ReferenceSummaryTypeDef",
+ReferenceOutputTypeDef = TypedDict(
+    "ReferenceOutputTypeDef",
     {
-        "Url": "UrlReferenceTypeDef",
-        "Attachment": "AttachmentReferenceTypeDef",
-        "String": "StringReferenceTypeDef",
-        "Number": "NumberReferenceTypeDef",
-        "Date": "DateReferenceTypeDef",
-        "Email": "EmailReferenceTypeDef",
+        "Value": str,
+        "Type": ReferenceTypeType,
+    },
+)
+
+ReferenceSummaryOutputTypeDef = TypedDict(
+    "ReferenceSummaryOutputTypeDef",
+    {
+        "Url": "UrlReferenceOutputTypeDef",
+        "Attachment": "AttachmentReferenceOutputTypeDef",
+        "String": "StringReferenceOutputTypeDef",
+        "Number": "NumberReferenceOutputTypeDef",
+        "Date": "DateReferenceOutputTypeDef",
+        "Email": "EmailReferenceOutputTypeDef",
     },
 )
 
 ReferenceTypeDef = TypedDict(
     "ReferenceTypeDef",
     {
         "Value": str,
@@ -5517,20 +6127,22 @@
     "_OptionalReleasePhoneNumberRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class ReleasePhoneNumberRequestRequestTypeDef(
     _RequiredReleasePhoneNumberRequestRequestTypeDef,
     _OptionalReleasePhoneNumberRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredReplicateInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ReplicaRegion": str,
         "ReplicaAlias": str,
     },
@@ -5539,28 +6151,37 @@
     "_OptionalReplicateInstanceRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class ReplicateInstanceRequestRequestTypeDef(
     _RequiredReplicateInstanceRequestRequestTypeDef, _OptionalReplicateInstanceRequestRequestTypeDef
 ):
     pass
 
-ReplicateInstanceResponseTypeDef = TypedDict(
-    "ReplicateInstanceResponseTypeDef",
+
+ReplicateInstanceResponseOutputTypeDef = TypedDict(
+    "ReplicateInstanceResponseOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RequiredFieldInfoOutputTypeDef = TypedDict(
+    "RequiredFieldInfoOutputTypeDef",
+    {
+        "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
+    },
+)
+
 RequiredFieldInfoTypeDef = TypedDict(
     "RequiredFieldInfoTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
     total=False,
 )
@@ -5589,16 +6210,32 @@
     {
         "InstanceId": str,
         "ContactId": str,
         "InitialContactId": str,
     },
 )
 
-RoutingProfileQueueConfigSummaryTypeDef = TypedDict(
-    "RoutingProfileQueueConfigSummaryTypeDef",
+RoutingProfileOutputTypeDef = TypedDict(
+    "RoutingProfileOutputTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "RoutingProfileArn": str,
+        "RoutingProfileId": str,
+        "Description": str,
+        "MediaConcurrencies": List["MediaConcurrencyOutputTypeDef"],
+        "DefaultOutboundQueueId": str,
+        "Tags": Dict[str, str],
+        "NumberOfAssociatedQueues": int,
+        "NumberOfAssociatedUsers": int,
+    },
+)
+
+RoutingProfileQueueConfigSummaryOutputTypeDef = TypedDict(
+    "RoutingProfileQueueConfigSummaryOutputTypeDef",
     {
         "QueueId": str,
         "QueueArn": str,
         "QueueName": str,
         "Priority": int,
         "Delay": int,
         "Channel": ChannelType,
@@ -5618,16 +6255,16 @@
     "RoutingProfileQueueReferenceTypeDef",
     {
         "QueueId": str,
         "Channel": ChannelType,
     },
 )
 
-RoutingProfileReferenceTypeDef = TypedDict(
-    "RoutingProfileReferenceTypeDef",
+RoutingProfileReferenceOutputTypeDef = TypedDict(
+    "RoutingProfileReferenceOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 RoutingProfileSearchCriteriaTypeDef = TypedDict(
@@ -5644,36 +6281,31 @@
     "RoutingProfileSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-RoutingProfileSummaryTypeDef = TypedDict(
-    "RoutingProfileSummaryTypeDef",
+RoutingProfileSummaryOutputTypeDef = TypedDict(
+    "RoutingProfileSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
-RoutingProfileTypeDef = TypedDict(
-    "RoutingProfileTypeDef",
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
     {
-        "InstanceId": str,
-        "Name": str,
-        "RoutingProfileArn": str,
-        "RoutingProfileId": str,
-        "Description": str,
-        "MediaConcurrencies": List["MediaConcurrencyTypeDef"],
-        "DefaultOutboundQueueId": str,
-        "Tags": Dict[str, str],
-        "NumberOfAssociatedQueues": int,
-        "NumberOfAssociatedUsers": int,
+        "ActionType": ActionTypeType,
+        "TaskAction": "TaskActionDefinitionOutputTypeDef",
+        "EventBridgeAction": "EventBridgeActionDefinitionOutputTypeDef",
+        "AssignContactCategoryAction": Dict[str, Any],
+        "SendNotificationAction": "SendNotificationActionDefinitionOutputTypeDef",
     },
 )
 
 _RequiredRuleActionTypeDef = TypedDict(
     "_RequiredRuleActionTypeDef",
     {
         "ActionType": ActionTypeType,
@@ -5686,64 +6318,85 @@
         "EventBridgeAction": "EventBridgeActionDefinitionTypeDef",
         "AssignContactCategoryAction": Mapping[str, Any],
         "SendNotificationAction": "SendNotificationActionDefinitionTypeDef",
     },
     total=False,
 )
 
+
 class RuleActionTypeDef(_RequiredRuleActionTypeDef, _OptionalRuleActionTypeDef):
     pass
 
-RuleSummaryTypeDef = TypedDict(
-    "RuleSummaryTypeDef",
+
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "Name": str,
+        "RuleId": str,
+        "RuleArn": str,
+        "TriggerEventSource": "RuleTriggerEventSourceOutputTypeDef",
+        "Function": str,
+        "Actions": List["RuleActionOutputTypeDef"],
+        "PublishStatus": RulePublishStatusType,
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "LastUpdatedBy": str,
+        "Tags": Dict[str, str],
+    },
+)
+
+RuleSummaryOutputTypeDef = TypedDict(
+    "RuleSummaryOutputTypeDef",
     {
         "Name": str,
         "RuleId": str,
         "RuleArn": str,
         "EventSourceName": EventSourceNameType,
         "PublishStatus": RulePublishStatusType,
-        "ActionSummaries": List["ActionSummaryTypeDef"],
+        "ActionSummaries": List["ActionSummaryOutputTypeDef"],
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
     },
 )
 
+RuleTriggerEventSourceOutputTypeDef = TypedDict(
+    "RuleTriggerEventSourceOutputTypeDef",
+    {
+        "EventSourceName": EventSourceNameType,
+        "IntegrationAssociationId": str,
+    },
+)
+
 _RequiredRuleTriggerEventSourceTypeDef = TypedDict(
     "_RequiredRuleTriggerEventSourceTypeDef",
     {
         "EventSourceName": EventSourceNameType,
     },
 )
 _OptionalRuleTriggerEventSourceTypeDef = TypedDict(
     "_OptionalRuleTriggerEventSourceTypeDef",
     {
         "IntegrationAssociationId": str,
     },
     total=False,
 )
 
+
 class RuleTriggerEventSourceTypeDef(
     _RequiredRuleTriggerEventSourceTypeDef, _OptionalRuleTriggerEventSourceTypeDef
 ):
     pass
 
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
+
+S3ConfigOutputTypeDef = TypedDict(
+    "S3ConfigOutputTypeDef",
     {
-        "Name": str,
-        "RuleId": str,
-        "RuleArn": str,
-        "TriggerEventSource": "RuleTriggerEventSourceTypeDef",
-        "Function": str,
-        "Actions": List["RuleActionTypeDef"],
-        "PublishStatus": RulePublishStatusType,
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "LastUpdatedBy": str,
-        "Tags": Dict[str, str],
+        "BucketName": str,
+        "BucketPrefix": str,
+        "EncryptionConfig": "EncryptionConfigOutputTypeDef",
     },
 )
 
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "BucketName": str,
@@ -5754,17 +6407,19 @@
     "_OptionalS3ConfigTypeDef",
     {
         "EncryptionConfig": "EncryptionConfigTypeDef",
     },
     total=False,
 )
 
+
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
+
 _RequiredSearchAvailablePhoneNumbersRequestRequestTypeDef = TypedDict(
     "_RequiredSearchAvailablePhoneNumbersRequestRequestTypeDef",
     {
         "TargetArn": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
@@ -5775,20 +6430,22 @@
         "PhoneNumberPrefix": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SearchAvailablePhoneNumbersRequestRequestTypeDef(
     _RequiredSearchAvailablePhoneNumbersRequestRequestTypeDef,
     _OptionalSearchAvailablePhoneNumbersRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef = TypedDict(
     "_RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef",
     {
         "TargetArn": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
@@ -5798,25 +6455,27 @@
     {
         "PhoneNumberPrefix": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef(
     _RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
     _OptionalSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
 ):
     pass
 
-SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseTypeDef",
+
+SearchAvailablePhoneNumbersResponseOutputTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseOutputTypeDef",
     {
         "NextToken": str,
-        "AvailableNumbersList": List["AvailableNumberSummaryTypeDef"],
+        "AvailableNumbersList": List["AvailableNumberSummaryOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchHoursOfOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchHoursOfOperationsRequestRequestTypeDef",
     {
@@ -5830,20 +6489,22 @@
         "MaxResults": int,
         "SearchFilter": "HoursOfOperationSearchFilterTypeDef",
         "SearchCriteria": "HoursOfOperationSearchCriteriaTypeDef",
     },
     total=False,
 )
 
+
 class SearchHoursOfOperationsRequestRequestTypeDef(
     _RequiredSearchHoursOfOperationsRequestRequestTypeDef,
     _OptionalSearchHoursOfOperationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef = TypedDict(
     "_RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef = TypedDict(
@@ -5852,24 +6513,26 @@
         "SearchFilter": "HoursOfOperationSearchFilterTypeDef",
         "SearchCriteria": "HoursOfOperationSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef(
     _RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
     _OptionalSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
 ):
     pass
 
-SearchHoursOfOperationsResponseTypeDef = TypedDict(
-    "SearchHoursOfOperationsResponseTypeDef",
+
+SearchHoursOfOperationsResponseOutputTypeDef = TypedDict(
+    "SearchHoursOfOperationsResponseOutputTypeDef",
     {
-        "HoursOfOperations": List["HoursOfOperationTypeDef"],
+        "HoursOfOperations": List["HoursOfOperationOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchPromptsRequestRequestTypeDef = TypedDict(
@@ -5885,19 +6548,21 @@
         "MaxResults": int,
         "SearchFilter": "PromptSearchFilterTypeDef",
         "SearchCriteria": "PromptSearchCriteriaTypeDef",
     },
     total=False,
 )
 
+
 class SearchPromptsRequestRequestTypeDef(
     _RequiredSearchPromptsRequestRequestTypeDef, _OptionalSearchPromptsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef = TypedDict(
     "_RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchPromptsRequestSearchPromptsPaginateTypeDef = TypedDict(
@@ -5906,24 +6571,26 @@
         "SearchFilter": "PromptSearchFilterTypeDef",
         "SearchCriteria": "PromptSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchPromptsRequestSearchPromptsPaginateTypeDef(
     _RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef,
     _OptionalSearchPromptsRequestSearchPromptsPaginateTypeDef,
 ):
     pass
 
-SearchPromptsResponseTypeDef = TypedDict(
-    "SearchPromptsResponseTypeDef",
+
+SearchPromptsResponseOutputTypeDef = TypedDict(
+    "SearchPromptsResponseOutputTypeDef",
     {
-        "Prompts": List["PromptTypeDef"],
+        "Prompts": List["PromptOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchQueuesRequestRequestTypeDef = TypedDict(
@@ -5939,19 +6606,21 @@
         "MaxResults": int,
         "SearchFilter": "QueueSearchFilterTypeDef",
         "SearchCriteria": "QueueSearchCriteriaTypeDef",
     },
     total=False,
 )
 
+
 class SearchQueuesRequestRequestTypeDef(
     _RequiredSearchQueuesRequestRequestTypeDef, _OptionalSearchQueuesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef = TypedDict(
     "_RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQueuesRequestSearchQueuesPaginateTypeDef = TypedDict(
@@ -5960,24 +6629,26 @@
         "SearchFilter": "QueueSearchFilterTypeDef",
         "SearchCriteria": "QueueSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchQueuesRequestSearchQueuesPaginateTypeDef(
     _RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef,
     _OptionalSearchQueuesRequestSearchQueuesPaginateTypeDef,
 ):
     pass
 
-SearchQueuesResponseTypeDef = TypedDict(
-    "SearchQueuesResponseTypeDef",
+
+SearchQueuesResponseOutputTypeDef = TypedDict(
+    "SearchQueuesResponseOutputTypeDef",
     {
-        "Queues": List["QueueTypeDef"],
+        "Queues": List["QueueOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchQuickConnectsRequestRequestTypeDef = TypedDict(
@@ -5993,20 +6664,22 @@
         "MaxResults": int,
         "SearchFilter": "QuickConnectSearchFilterTypeDef",
         "SearchCriteria": "QuickConnectSearchCriteriaTypeDef",
     },
     total=False,
 )
 
+
 class SearchQuickConnectsRequestRequestTypeDef(
     _RequiredSearchQuickConnectsRequestRequestTypeDef,
     _OptionalSearchQuickConnectsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef = TypedDict(
@@ -6015,24 +6688,26 @@
         "SearchFilter": "QuickConnectSearchFilterTypeDef",
         "SearchCriteria": "QuickConnectSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef(
     _RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
     _OptionalSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
 ):
     pass
 
-SearchQuickConnectsResponseTypeDef = TypedDict(
-    "SearchQuickConnectsResponseTypeDef",
+
+SearchQuickConnectsResponseOutputTypeDef = TypedDict(
+    "SearchQuickConnectsResponseOutputTypeDef",
     {
-        "QuickConnects": List["QuickConnectTypeDef"],
+        "QuickConnects": List["QuickConnectOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchResourceTagsRequestRequestTypeDef = TypedDict(
@@ -6048,20 +6723,22 @@
         "NextToken": str,
         "MaxResults": int,
         "SearchCriteria": "ResourceTagsSearchCriteriaTypeDef",
     },
     total=False,
 )
 
+
 class SearchResourceTagsRequestRequestTypeDef(
     _RequiredSearchResourceTagsRequestRequestTypeDef,
     _OptionalSearchResourceTagsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef = TypedDict(
     "_RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef = TypedDict(
@@ -6070,24 +6747,26 @@
         "ResourceTypes": Sequence[str],
         "SearchCriteria": "ResourceTagsSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef(
     _RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
     _OptionalSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
 ):
     pass
 
-SearchResourceTagsResponseTypeDef = TypedDict(
-    "SearchResourceTagsResponseTypeDef",
+
+SearchResourceTagsResponseOutputTypeDef = TypedDict(
+    "SearchResourceTagsResponseOutputTypeDef",
     {
-        "Tags": List["TagSetTypeDef"],
+        "Tags": List["TagSetOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchRoutingProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRoutingProfilesRequestRequestTypeDef",
@@ -6102,20 +6781,22 @@
         "MaxResults": int,
         "SearchFilter": "RoutingProfileSearchFilterTypeDef",
         "SearchCriteria": "RoutingProfileSearchCriteriaTypeDef",
     },
     total=False,
 )
 
+
 class SearchRoutingProfilesRequestRequestTypeDef(
     _RequiredSearchRoutingProfilesRequestRequestTypeDef,
     _OptionalSearchRoutingProfilesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef = TypedDict(
     "_RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef = TypedDict(
@@ -6124,24 +6805,26 @@
         "SearchFilter": "RoutingProfileSearchFilterTypeDef",
         "SearchCriteria": "RoutingProfileSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef(
     _RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
     _OptionalSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
 ):
     pass
 
-SearchRoutingProfilesResponseTypeDef = TypedDict(
-    "SearchRoutingProfilesResponseTypeDef",
+
+SearchRoutingProfilesResponseOutputTypeDef = TypedDict(
+    "SearchRoutingProfilesResponseOutputTypeDef",
     {
-        "RoutingProfiles": List["RoutingProfileTypeDef"],
+        "RoutingProfiles": List["RoutingProfileOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchSecurityProfilesRequestRequestTypeDef = TypedDict(
@@ -6157,20 +6840,22 @@
         "MaxResults": int,
         "SearchCriteria": "SecurityProfileSearchCriteriaTypeDef",
         "SearchFilter": "SecurityProfilesSearchFilterTypeDef",
     },
     total=False,
 )
 
+
 class SearchSecurityProfilesRequestRequestTypeDef(
     _RequiredSearchSecurityProfilesRequestRequestTypeDef,
     _OptionalSearchSecurityProfilesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef = TypedDict(
     "_RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef = TypedDict(
@@ -6179,24 +6864,26 @@
         "SearchCriteria": "SecurityProfileSearchCriteriaTypeDef",
         "SearchFilter": "SecurityProfilesSearchFilterTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef(
     _RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
     _OptionalSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
 ):
     pass
 
-SearchSecurityProfilesResponseTypeDef = TypedDict(
-    "SearchSecurityProfilesResponseTypeDef",
+
+SearchSecurityProfilesResponseOutputTypeDef = TypedDict(
+    "SearchSecurityProfilesResponseOutputTypeDef",
     {
-        "SecurityProfiles": List["SecurityProfileSearchSummaryTypeDef"],
+        "SecurityProfiles": List["SecurityProfileSearchSummaryOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchUsersRequestRequestTypeDef = TypedDict(
@@ -6218,18 +6905,18 @@
         "SearchFilter": "UserSearchFilterTypeDef",
         "SearchCriteria": "UserSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-SearchUsersResponseTypeDef = TypedDict(
-    "SearchUsersResponseTypeDef",
+SearchUsersResponseOutputTypeDef = TypedDict(
+    "SearchUsersResponseOutputTypeDef",
     {
-        "Users": List["UserSearchSummaryTypeDef"],
+        "Users": List["UserSearchSummaryOutputTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchVocabulariesRequestRequestTypeDef = TypedDict(
@@ -6246,20 +6933,22 @@
         "State": VocabularyStateType,
         "NameStartsWith": str,
         "LanguageCode": VocabularyLanguageCodeType,
     },
     total=False,
 )
 
+
 class SearchVocabulariesRequestRequestTypeDef(
     _RequiredSearchVocabulariesRequestRequestTypeDef,
     _OptionalSearchVocabulariesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef = TypedDict(
     "_RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef = TypedDict(
@@ -6269,91 +6958,104 @@
         "NameStartsWith": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef(
     _RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
     _OptionalSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
 ):
     pass
 
-SearchVocabulariesResponseTypeDef = TypedDict(
-    "SearchVocabulariesResponseTypeDef",
+
+SearchVocabulariesResponseOutputTypeDef = TypedDict(
+    "SearchVocabulariesResponseOutputTypeDef",
     {
-        "VocabularySummaryList": List["VocabularySummaryTypeDef"],
+        "VocabularySummaryList": List["VocabularySummaryOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SecurityKeyTypeDef = TypedDict(
-    "SecurityKeyTypeDef",
+SecurityKeyOutputTypeDef = TypedDict(
+    "SecurityKeyOutputTypeDef",
     {
         "AssociationId": str,
         "Key": str,
         "CreationTime": datetime,
     },
 )
 
+SecurityProfileOutputTypeDef = TypedDict(
+    "SecurityProfileOutputTypeDef",
+    {
+        "Id": str,
+        "OrganizationResourceId": str,
+        "Arn": str,
+        "SecurityProfileName": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "AllowedAccessControlTags": Dict[str, str],
+        "TagRestrictedResources": List[str],
+    },
+)
+
 SecurityProfileSearchCriteriaTypeDef = TypedDict(
     "SecurityProfileSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
     total=False,
 )
 
-SecurityProfileSearchSummaryTypeDef = TypedDict(
-    "SecurityProfileSearchSummaryTypeDef",
+SecurityProfileSearchSummaryOutputTypeDef = TypedDict(
+    "SecurityProfileSearchSummaryOutputTypeDef",
     {
         "Id": str,
         "OrganizationResourceId": str,
         "Arn": str,
         "SecurityProfileName": str,
         "Description": str,
         "Tags": Dict[str, str],
     },
 )
 
-SecurityProfileSummaryTypeDef = TypedDict(
-    "SecurityProfileSummaryTypeDef",
+SecurityProfileSummaryOutputTypeDef = TypedDict(
+    "SecurityProfileSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
-SecurityProfileTypeDef = TypedDict(
-    "SecurityProfileTypeDef",
-    {
-        "Id": str,
-        "OrganizationResourceId": str,
-        "Arn": str,
-        "SecurityProfileName": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "AllowedAccessControlTags": Dict[str, str],
-        "TagRestrictedResources": List[str],
-    },
-)
-
 SecurityProfilesSearchFilterTypeDef = TypedDict(
     "SecurityProfilesSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
+SendNotificationActionDefinitionOutputTypeDef = TypedDict(
+    "SendNotificationActionDefinitionOutputTypeDef",
+    {
+        "DeliveryMethod": Literal["EMAIL"],
+        "Subject": str,
+        "Content": str,
+        "ContentType": Literal["PLAIN_TEXT"],
+        "Recipient": "NotificationRecipientTypeOutputTypeDef",
+    },
+)
+
 _RequiredSendNotificationActionDefinitionTypeDef = TypedDict(
     "_RequiredSendNotificationActionDefinitionTypeDef",
     {
         "DeliveryMethod": Literal["EMAIL"],
         "Content": str,
         "ContentType": Literal["PLAIN_TEXT"],
         "Recipient": "NotificationRecipientTypeTypeDef",
@@ -6363,20 +7065,31 @@
     "_OptionalSendNotificationActionDefinitionTypeDef",
     {
         "Subject": str,
     },
     total=False,
 )
 
+
 class SendNotificationActionDefinitionTypeDef(
     _RequiredSendNotificationActionDefinitionTypeDef,
     _OptionalSendNotificationActionDefinitionTypeDef,
 ):
     pass
 
+
+SingleSelectQuestionRuleCategoryAutomationOutputTypeDef = TypedDict(
+    "SingleSelectQuestionRuleCategoryAutomationOutputTypeDef",
+    {
+        "Category": str,
+        "Condition": SingleSelectQuestionRuleCategoryAutomationConditionType,
+        "OptionRefId": str,
+    },
+)
+
 SingleSelectQuestionRuleCategoryAutomationTypeDef = TypedDict(
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     {
         "Category": str,
         "Condition": SingleSelectQuestionRuleCategoryAutomationConditionType,
         "OptionRefId": str,
     },
@@ -6400,21 +7113,23 @@
         "SupportedMessagingContentTypes": Sequence[str],
         "PersistentChat": "PersistentChatTypeDef",
         "RelatedContactId": str,
     },
     total=False,
 )
 
+
 class StartChatContactRequestRequestTypeDef(
     _RequiredStartChatContactRequestRequestTypeDef, _OptionalStartChatContactRequestRequestTypeDef
 ):
     pass
 
-StartChatContactResponseTypeDef = TypedDict(
-    "StartChatContactResponseTypeDef",
+
+StartChatContactResponseOutputTypeDef = TypedDict(
+    "StartChatContactResponseOutputTypeDef",
     {
         "ContactId": str,
         "ParticipantId": str,
         "ParticipantToken": str,
         "ContinuedFromContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -6432,22 +7147,24 @@
     "_OptionalStartContactEvaluationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartContactEvaluationRequestRequestTypeDef(
     _RequiredStartContactEvaluationRequestRequestTypeDef,
     _OptionalStartContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-StartContactEvaluationResponseTypeDef = TypedDict(
-    "StartContactEvaluationResponseTypeDef",
+
+StartContactEvaluationResponseOutputTypeDef = TypedDict(
+    "StartContactEvaluationResponseOutputTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -6467,16 +7184,16 @@
         "InstanceId": str,
         "ContactId": str,
         "ChatStreamingConfiguration": "ChatStreamingConfigurationTypeDef",
         "ClientToken": str,
     },
 )
 
-StartContactStreamingResponseTypeDef = TypedDict(
-    "StartContactStreamingResponseTypeDef",
+StartContactStreamingResponseOutputTypeDef = TypedDict(
+    "StartContactStreamingResponseOutputTypeDef",
     {
         "StreamingId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartOutboundVoiceContactRequestRequestTypeDef = TypedDict(
@@ -6497,22 +7214,24 @@
         "AnswerMachineDetectionConfig": "AnswerMachineDetectionConfigTypeDef",
         "CampaignId": str,
         "TrafficType": TrafficTypeType,
     },
     total=False,
 )
 
+
 class StartOutboundVoiceContactRequestRequestTypeDef(
     _RequiredStartOutboundVoiceContactRequestRequestTypeDef,
     _OptionalStartOutboundVoiceContactRequestRequestTypeDef,
 ):
     pass
 
-StartOutboundVoiceContactResponseTypeDef = TypedDict(
-    "StartOutboundVoiceContactResponseTypeDef",
+
+StartOutboundVoiceContactResponseOutputTypeDef = TypedDict(
+    "StartOutboundVoiceContactResponseOutputTypeDef",
     {
         "ContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTaskContactRequestRequestTypeDef = TypedDict(
@@ -6535,21 +7254,23 @@
         "TaskTemplateId": str,
         "QuickConnectId": str,
         "RelatedContactId": str,
     },
     total=False,
 )
 
+
 class StartTaskContactRequestRequestTypeDef(
     _RequiredStartTaskContactRequestRequestTypeDef, _OptionalStartTaskContactRequestRequestTypeDef
 ):
     pass
 
-StartTaskContactResponseTypeDef = TypedDict(
-    "StartTaskContactResponseTypeDef",
+
+StartTaskContactResponseOutputTypeDef = TypedDict(
+    "StartTaskContactResponseOutputTypeDef",
     {
         "ContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopContactRecordingRequestRequestTypeDef = TypedDict(
@@ -6584,16 +7305,16 @@
         "FieldName": str,
         "Value": str,
         "ComparisonType": StringComparisonTypeType,
     },
     total=False,
 )
 
-StringReferenceTypeDef = TypedDict(
-    "StringReferenceTypeDef",
+StringReferenceOutputTypeDef = TypedDict(
+    "StringReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 _RequiredSubmitContactEvaluationRequestRequestTypeDef = TypedDict(
@@ -6608,22 +7329,24 @@
     {
         "Answers": Mapping[str, "EvaluationAnswerInputTypeDef"],
         "Notes": Mapping[str, "EvaluationNoteTypeDef"],
     },
     total=False,
 )
 
+
 class SubmitContactEvaluationRequestRequestTypeDef(
     _RequiredSubmitContactEvaluationRequestRequestTypeDef,
     _OptionalSubmitContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-SubmitContactEvaluationResponseTypeDef = TypedDict(
-    "SubmitContactEvaluationResponseTypeDef",
+
+SubmitContactEvaluationResponseOutputTypeDef = TypedDict(
+    "SubmitContactEvaluationResponseOutputTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -6660,22 +7383,32 @@
         "tagValue": str,
         "tagKeyComparisonType": StringComparisonTypeType,
         "tagValueComparisonType": StringComparisonTypeType,
     },
     total=False,
 )
 
-TagSetTypeDef = TypedDict(
-    "TagSetTypeDef",
+TagSetOutputTypeDef = TypedDict(
+    "TagSetOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+TaskActionDefinitionOutputTypeDef = TypedDict(
+    "TaskActionDefinitionOutputTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "ContactFlowId": str,
+        "References": Dict[str, "ReferenceOutputTypeDef"],
+    },
+)
+
 _RequiredTaskActionDefinitionTypeDef = TypedDict(
     "_RequiredTaskActionDefinitionTypeDef",
     {
         "Name": str,
         "ContactFlowId": str,
     },
 )
@@ -6684,54 +7417,97 @@
     {
         "Description": str,
         "References": Mapping[str, "ReferenceTypeDef"],
     },
     total=False,
 )
 
+
 class TaskActionDefinitionTypeDef(
     _RequiredTaskActionDefinitionTypeDef, _OptionalTaskActionDefinitionTypeDef
 ):
     pass
 
+
+TaskTemplateConstraintsOutputTypeDef = TypedDict(
+    "TaskTemplateConstraintsOutputTypeDef",
+    {
+        "RequiredFields": List["RequiredFieldInfoOutputTypeDef"],
+        "ReadOnlyFields": List["ReadOnlyFieldInfoOutputTypeDef"],
+        "InvisibleFields": List["InvisibleFieldInfoOutputTypeDef"],
+    },
+)
+
 TaskTemplateConstraintsTypeDef = TypedDict(
     "TaskTemplateConstraintsTypeDef",
     {
         "RequiredFields": Sequence["RequiredFieldInfoTypeDef"],
         "ReadOnlyFields": Sequence["ReadOnlyFieldInfoTypeDef"],
         "InvisibleFields": Sequence["InvisibleFieldInfoTypeDef"],
     },
     total=False,
 )
 
+TaskTemplateDefaultFieldValueOutputTypeDef = TypedDict(
+    "TaskTemplateDefaultFieldValueOutputTypeDef",
+    {
+        "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
+        "DefaultValue": str,
+    },
+)
+
 TaskTemplateDefaultFieldValueTypeDef = TypedDict(
     "TaskTemplateDefaultFieldValueTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
         "DefaultValue": str,
     },
     total=False,
 )
 
+TaskTemplateDefaultsOutputTypeDef = TypedDict(
+    "TaskTemplateDefaultsOutputTypeDef",
+    {
+        "DefaultFieldValues": List["TaskTemplateDefaultFieldValueOutputTypeDef"],
+    },
+)
+
 TaskTemplateDefaultsTypeDef = TypedDict(
     "TaskTemplateDefaultsTypeDef",
     {
         "DefaultFieldValues": Sequence["TaskTemplateDefaultFieldValueTypeDef"],
     },
     total=False,
 )
 
+TaskTemplateFieldIdentifierOutputTypeDef = TypedDict(
+    "TaskTemplateFieldIdentifierOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 TaskTemplateFieldIdentifierTypeDef = TypedDict(
     "TaskTemplateFieldIdentifierTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+TaskTemplateFieldOutputTypeDef = TypedDict(
+    "TaskTemplateFieldOutputTypeDef",
+    {
+        "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
+        "Description": str,
+        "Type": TaskTemplateFieldTypeType,
+        "SingleSelectOptions": List[str],
+    },
+)
+
 _RequiredTaskTemplateFieldTypeDef = TypedDict(
     "_RequiredTaskTemplateFieldTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
 )
 _OptionalTaskTemplateFieldTypeDef = TypedDict(
@@ -6740,78 +7516,103 @@
         "Description": str,
         "Type": TaskTemplateFieldTypeType,
         "SingleSelectOptions": Sequence[str],
     },
     total=False,
 )
 
+
 class TaskTemplateFieldTypeDef(
     _RequiredTaskTemplateFieldTypeDef, _OptionalTaskTemplateFieldTypeDef
 ):
     pass
 
-TaskTemplateMetadataTypeDef = TypedDict(
-    "TaskTemplateMetadataTypeDef",
+
+TaskTemplateMetadataOutputTypeDef = TypedDict(
+    "TaskTemplateMetadataOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
     },
 )
 
+TelephonyConfigOutputTypeDef = TypedDict(
+    "TelephonyConfigOutputTypeDef",
+    {
+        "Distributions": List["DistributionOutputTypeDef"],
+    },
+)
+
 TelephonyConfigTypeDef = TypedDict(
     "TelephonyConfigTypeDef",
     {
-        "Distributions": List["DistributionTypeDef"],
+        "Distributions": Sequence["DistributionTypeDef"],
+    },
+)
+
+ThresholdOutputTypeDef = TypedDict(
+    "ThresholdOutputTypeDef",
+    {
+        "Comparison": Literal["LT"],
+        "ThresholdValue": float,
     },
 )
 
 ThresholdTypeDef = TypedDict(
     "ThresholdTypeDef",
     {
         "Comparison": Literal["LT"],
         "ThresholdValue": float,
     },
     total=False,
 )
 
+ThresholdV2OutputTypeDef = TypedDict(
+    "ThresholdV2OutputTypeDef",
+    {
+        "Comparison": str,
+        "ThresholdValue": float,
+    },
+)
+
 ThresholdV2TypeDef = TypedDict(
     "ThresholdV2TypeDef",
     {
         "Comparison": str,
         "ThresholdValue": float,
     },
     total=False,
 )
 
-TrafficDistributionGroupSummaryTypeDef = TypedDict(
-    "TrafficDistributionGroupSummaryTypeDef",
+TrafficDistributionGroupOutputTypeDef = TypedDict(
+    "TrafficDistributionGroupOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
+        "Description": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
+        "Tags": Dict[str, str],
     },
 )
 
-TrafficDistributionGroupTypeDef = TypedDict(
-    "TrafficDistributionGroupTypeDef",
+TrafficDistributionGroupSummaryOutputTypeDef = TypedDict(
+    "TrafficDistributionGroupSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
-        "Description": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
-        "Tags": Dict[str, str],
     },
 )
 
 _RequiredTransferContactRequestRequestTypeDef = TypedDict(
     "_RequiredTransferContactRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -6825,21 +7626,23 @@
         "QueueId": str,
         "UserId": str,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class TransferContactRequestRequestTypeDef(
     _RequiredTransferContactRequestRequestTypeDef, _OptionalTransferContactRequestRequestTypeDef
 ):
     pass
 
-TransferContactResponseTypeDef = TypedDict(
-    "TransferContactResponseTypeDef",
+
+TransferContactResponseOutputTypeDef = TypedDict(
+    "TransferContactResponseOutputTypeDef",
     {
         "ContactId": str,
         "ContactArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -6866,19 +7669,21 @@
         "State": AgentStatusStateType,
         "DisplayOrder": int,
         "ResetOrderNumber": bool,
     },
     total=False,
 )
 
+
 class UpdateAgentStatusRequestRequestTypeDef(
     _RequiredUpdateAgentStatusRequestRequestTypeDef, _OptionalUpdateAgentStatusRequestRequestTypeDef
 ):
     pass
 
+
 UpdateContactAttributesRequestRequestTypeDef = TypedDict(
     "UpdateContactAttributesRequestRequestTypeDef",
     {
         "InitialContactId": str,
         "InstanceId": str,
         "Attributes": Mapping[str, str],
     },
@@ -6896,22 +7701,24 @@
     {
         "Answers": Mapping[str, "EvaluationAnswerInputTypeDef"],
         "Notes": Mapping[str, "EvaluationNoteTypeDef"],
     },
     total=False,
 )
 
+
 class UpdateContactEvaluationRequestRequestTypeDef(
     _RequiredUpdateContactEvaluationRequestRequestTypeDef,
     _OptionalUpdateContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-UpdateContactEvaluationResponseTypeDef = TypedDict(
-    "UpdateContactEvaluationResponseTypeDef",
+
+UpdateContactEvaluationResponseOutputTypeDef = TypedDict(
+    "UpdateContactEvaluationResponseOutputTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -6937,20 +7744,22 @@
         "Name": str,
         "Description": str,
         "ContactFlowState": ContactFlowStateType,
     },
     total=False,
 )
 
+
 class UpdateContactFlowMetadataRequestRequestTypeDef(
     _RequiredUpdateContactFlowMetadataRequestRequestTypeDef,
     _OptionalUpdateContactFlowMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateContactFlowModuleContentRequestRequestTypeDef = TypedDict(
     "UpdateContactFlowModuleContentRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowModuleId": str,
         "Content": str,
     },
@@ -6969,20 +7778,22 @@
         "Name": str,
         "Description": str,
         "State": ContactFlowModuleStateType,
     },
     total=False,
 )
 
+
 class UpdateContactFlowModuleMetadataRequestRequestTypeDef(
     _RequiredUpdateContactFlowModuleMetadataRequestRequestTypeDef,
     _OptionalUpdateContactFlowModuleMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateContactFlowNameRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactFlowNameRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowId": str,
     },
 )
@@ -6991,20 +7802,22 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateContactFlowNameRequestRequestTypeDef(
     _RequiredUpdateContactFlowNameRequestRequestTypeDef,
     _OptionalUpdateContactFlowNameRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
@@ -7014,19 +7827,21 @@
         "Name": str,
         "Description": str,
         "References": Mapping[str, "ReferenceTypeDef"],
     },
     total=False,
 )
 
+
 class UpdateContactRequestRequestTypeDef(
     _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
 ):
     pass
 
+
 UpdateContactScheduleRequestRequestTypeDef = TypedDict(
     "UpdateContactScheduleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ScheduledTime": Union[datetime, str],
     },
@@ -7049,22 +7864,24 @@
         "Description": str,
         "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class UpdateEvaluationFormRequestRequestTypeDef(
     _RequiredUpdateEvaluationFormRequestRequestTypeDef,
     _OptionalUpdateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-UpdateEvaluationFormResponseTypeDef = TypedDict(
-    "UpdateEvaluationFormResponseTypeDef",
+
+UpdateEvaluationFormResponseOutputTypeDef = TypedDict(
+    "UpdateEvaluationFormResponseOutputTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -7083,20 +7900,22 @@
         "Description": str,
         "TimeZone": str,
         "Config": Sequence["HoursOfOperationConfigTypeDef"],
     },
     total=False,
 )
 
+
 class UpdateHoursOfOperationRequestRequestTypeDef(
     _RequiredUpdateHoursOfOperationRequestRequestTypeDef,
     _OptionalUpdateHoursOfOperationRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateInstanceAttributeRequestRequestTypeDef = TypedDict(
     "UpdateInstanceAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AttributeType": InstanceAttributeTypeType,
         "Value": str,
     },
@@ -7140,21 +7959,23 @@
     "_OptionalUpdatePhoneNumberRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
-UpdatePhoneNumberResponseTypeDef = TypedDict(
-    "UpdatePhoneNumberResponseTypeDef",
+
+UpdatePhoneNumberResponseOutputTypeDef = TypedDict(
+    "UpdatePhoneNumberResponseOutputTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7171,21 +7992,23 @@
         "Name": str,
         "Description": str,
         "S3Uri": str,
     },
     total=False,
 )
 
+
 class UpdatePromptRequestRequestTypeDef(
     _RequiredUpdatePromptRequestRequestTypeDef, _OptionalUpdatePromptRequestRequestTypeDef
 ):
     pass
 
-UpdatePromptResponseTypeDef = TypedDict(
-    "UpdatePromptResponseTypeDef",
+
+UpdatePromptResponseOutputTypeDef = TypedDict(
+    "UpdatePromptResponseOutputTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7209,20 +8032,22 @@
     "_OptionalUpdateQueueMaxContactsRequestRequestTypeDef",
     {
         "MaxContacts": int,
     },
     total=False,
 )
 
+
 class UpdateQueueMaxContactsRequestRequestTypeDef(
     _RequiredUpdateQueueMaxContactsRequestRequestTypeDef,
     _OptionalUpdateQueueMaxContactsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateQueueNameRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateQueueNameRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
@@ -7231,19 +8056,21 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateQueueNameRequestRequestTypeDef(
     _RequiredUpdateQueueNameRequestRequestTypeDef, _OptionalUpdateQueueNameRequestRequestTypeDef
 ):
     pass
 
+
 UpdateQueueOutboundCallerConfigRequestRequestTypeDef = TypedDict(
     "UpdateQueueOutboundCallerConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
         "OutboundCallerConfig": "OutboundCallerConfigTypeDef",
     },
@@ -7279,20 +8106,22 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateQuickConnectNameRequestRequestTypeDef(
     _RequiredUpdateQuickConnectNameRequestRequestTypeDef,
     _OptionalUpdateQuickConnectNameRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateRoutingProfileConcurrencyRequestRequestTypeDef = TypedDict(
     "UpdateRoutingProfileConcurrencyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
         "MediaConcurrencies": Sequence["MediaConcurrencyTypeDef"],
     },
@@ -7319,20 +8148,22 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateRoutingProfileNameRequestRequestTypeDef(
     _RequiredUpdateRoutingProfileNameRequestRequestTypeDef,
     _OptionalUpdateRoutingProfileNameRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateRoutingProfileQueuesRequestRequestTypeDef = TypedDict(
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
         "QueueConfigs": Sequence["RoutingProfileQueueConfigTypeDef"],
     },
@@ -7364,20 +8195,22 @@
         "Permissions": Sequence[str],
         "AllowedAccessControlTags": Mapping[str, str],
         "TagRestrictedResources": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateSecurityProfileRequestRequestTypeDef(
     _RequiredUpdateSecurityProfileRequestRequestTypeDef,
     _OptionalUpdateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateTaskTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTaskTemplateRequestRequestTypeDef",
     {
         "TaskTemplateId": str,
         "InstanceId": str,
     },
 )
@@ -7391,32 +8224,34 @@
         "Defaults": "TaskTemplateDefaultsTypeDef",
         "Status": TaskTemplateStatusType,
         "Fields": Sequence["TaskTemplateFieldTypeDef"],
     },
     total=False,
 )
 
+
 class UpdateTaskTemplateRequestRequestTypeDef(
     _RequiredUpdateTaskTemplateRequestRequestTypeDef,
     _OptionalUpdateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
-UpdateTaskTemplateResponseTypeDef = TypedDict(
-    "UpdateTaskTemplateResponseTypeDef",
+
+UpdateTaskTemplateResponseOutputTypeDef = TypedDict(
+    "UpdateTaskTemplateResponseOutputTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
-        "Constraints": "TaskTemplateConstraintsTypeDef",
-        "Defaults": "TaskTemplateDefaultsTypeDef",
-        "Fields": List["TaskTemplateFieldTypeDef"],
+        "Constraints": "TaskTemplateConstraintsOutputTypeDef",
+        "Defaults": "TaskTemplateDefaultsOutputTypeDef",
+        "Fields": List["TaskTemplateFieldOutputTypeDef"],
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7430,20 +8265,22 @@
     "_OptionalUpdateTrafficDistributionRequestRequestTypeDef",
     {
         "TelephonyConfig": "TelephonyConfigTypeDef",
     },
     total=False,
 )
 
+
 class UpdateTrafficDistributionRequestRequestTypeDef(
     _RequiredUpdateTrafficDistributionRequestRequestTypeDef,
     _OptionalUpdateTrafficDistributionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateUserHierarchyGroupNameRequestRequestTypeDef = TypedDict(
     "UpdateUserHierarchyGroupNameRequestRequestTypeDef",
     {
         "Name": str,
         "HierarchyGroupId": str,
         "InstanceId": str,
     },
@@ -7460,20 +8297,22 @@
     "_OptionalUpdateUserHierarchyRequestRequestTypeDef",
     {
         "HierarchyGroupId": str,
     },
     total=False,
 )
 
+
 class UpdateUserHierarchyRequestRequestTypeDef(
     _RequiredUpdateUserHierarchyRequestRequestTypeDef,
     _OptionalUpdateUserHierarchyRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateUserHierarchyStructureRequestRequestTypeDef = TypedDict(
     "UpdateUserHierarchyStructureRequestRequestTypeDef",
     {
         "HierarchyStructure": "HierarchyStructureUpdateTypeDef",
         "InstanceId": str,
     },
 )
@@ -7510,24 +8349,24 @@
     {
         "SecurityProfileIds": Sequence[str],
         "UserId": str,
         "InstanceId": str,
     },
 )
 
-UrlReferenceTypeDef = TypedDict(
-    "UrlReferenceTypeDef",
+UrlReferenceOutputTypeDef = TypedDict(
+    "UrlReferenceOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-UseCaseTypeDef = TypedDict(
-    "UseCaseTypeDef",
+UseCaseOutputTypeDef = TypedDict(
+    "UseCaseOutputTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "UseCaseType": UseCaseTypeType,
     },
 )
 
@@ -7539,49 +8378,86 @@
         "RoutingProfiles": Sequence[str],
         "Agents": Sequence[str],
         "UserHierarchyGroups": Sequence[str],
     },
     total=False,
 )
 
-UserDataTypeDef = TypedDict(
-    "UserDataTypeDef",
+UserDataOutputTypeDef = TypedDict(
+    "UserDataOutputTypeDef",
     {
-        "User": "UserReferenceTypeDef",
-        "RoutingProfile": "RoutingProfileReferenceTypeDef",
-        "HierarchyPath": "HierarchyPathReferenceTypeDef",
-        "Status": "AgentStatusReferenceTypeDef",
+        "User": "UserReferenceOutputTypeDef",
+        "RoutingProfile": "RoutingProfileReferenceOutputTypeDef",
+        "HierarchyPath": "HierarchyPathReferenceOutputTypeDef",
+        "Status": "AgentStatusReferenceOutputTypeDef",
         "AvailableSlotsByChannel": Dict[ChannelType, int],
         "MaxSlotsByChannel": Dict[ChannelType, int],
         "ActiveSlotsByChannel": Dict[ChannelType, int],
-        "Contacts": List["AgentContactReferenceTypeDef"],
+        "Contacts": List["AgentContactReferenceOutputTypeDef"],
         "NextStatus": str,
     },
 )
 
-UserIdentityInfoLiteTypeDef = TypedDict(
-    "UserIdentityInfoLiteTypeDef",
+UserIdentityInfoLiteOutputTypeDef = TypedDict(
+    "UserIdentityInfoLiteOutputTypeDef",
     {
         "FirstName": str,
         "LastName": str,
     },
 )
 
+UserIdentityInfoOutputTypeDef = TypedDict(
+    "UserIdentityInfoOutputTypeDef",
+    {
+        "FirstName": str,
+        "LastName": str,
+        "Email": str,
+        "SecondaryEmail": str,
+        "Mobile": str,
+    },
+)
+
 UserIdentityInfoTypeDef = TypedDict(
     "UserIdentityInfoTypeDef",
     {
         "FirstName": str,
         "LastName": str,
         "Email": str,
         "SecondaryEmail": str,
         "Mobile": str,
     },
     total=False,
 )
 
+UserOutputTypeDef = TypedDict(
+    "UserOutputTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Username": str,
+        "IdentityInfo": "UserIdentityInfoOutputTypeDef",
+        "PhoneConfig": "UserPhoneConfigOutputTypeDef",
+        "DirectoryUserId": str,
+        "SecurityProfileIds": List[str],
+        "RoutingProfileId": str,
+        "HierarchyGroupId": str,
+        "Tags": Dict[str, str],
+    },
+)
+
+UserPhoneConfigOutputTypeDef = TypedDict(
+    "UserPhoneConfigOutputTypeDef",
+    {
+        "PhoneType": PhoneTypeType,
+        "AutoAccept": bool,
+        "AfterContactWorkTimeLimit": int,
+        "DeskPhoneNumber": str,
+    },
+)
+
 _RequiredUserPhoneConfigTypeDef = TypedDict(
     "_RequiredUserPhoneConfigTypeDef",
     {
         "PhoneType": PhoneTypeType,
     },
 )
 _OptionalUserPhoneConfigTypeDef = TypedDict(
@@ -7590,27 +8466,37 @@
         "AutoAccept": bool,
         "AfterContactWorkTimeLimit": int,
         "DeskPhoneNumber": str,
     },
     total=False,
 )
 
+
 class UserPhoneConfigTypeDef(_RequiredUserPhoneConfigTypeDef, _OptionalUserPhoneConfigTypeDef):
     pass
 
+
+UserQuickConnectConfigOutputTypeDef = TypedDict(
+    "UserQuickConnectConfigOutputTypeDef",
+    {
+        "UserId": str,
+        "ContactFlowId": str,
+    },
+)
+
 UserQuickConnectConfigTypeDef = TypedDict(
     "UserQuickConnectConfigTypeDef",
     {
         "UserId": str,
         "ContactFlowId": str,
     },
 )
 
-UserReferenceTypeDef = TypedDict(
-    "UserReferenceTypeDef",
+UserReferenceOutputTypeDef = TypedDict(
+    "UserReferenceOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 UserSearchCriteriaTypeDef = TypedDict(
@@ -7628,90 +8514,74 @@
     "UserSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-UserSearchSummaryTypeDef = TypedDict(
-    "UserSearchSummaryTypeDef",
+UserSearchSummaryOutputTypeDef = TypedDict(
+    "UserSearchSummaryOutputTypeDef",
     {
         "Arn": str,
         "DirectoryUserId": str,
         "HierarchyGroupId": str,
         "Id": str,
-        "IdentityInfo": "UserIdentityInfoLiteTypeDef",
-        "PhoneConfig": "UserPhoneConfigTypeDef",
+        "IdentityInfo": "UserIdentityInfoLiteOutputTypeDef",
+        "PhoneConfig": "UserPhoneConfigOutputTypeDef",
         "RoutingProfileId": str,
         "SecurityProfileIds": List[str],
         "Tags": Dict[str, str],
         "Username": str,
     },
 )
 
-UserSummaryTypeDef = TypedDict(
-    "UserSummaryTypeDef",
+UserSummaryOutputTypeDef = TypedDict(
+    "UserSummaryOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Username": str,
     },
 )
 
-UserTypeDef = TypedDict(
-    "UserTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Username": str,
-        "IdentityInfo": "UserIdentityInfoTypeDef",
-        "PhoneConfig": "UserPhoneConfigTypeDef",
-        "DirectoryUserId": str,
-        "SecurityProfileIds": List[str],
-        "RoutingProfileId": str,
-        "HierarchyGroupId": str,
-        "Tags": Dict[str, str],
-    },
-)
-
-VocabularySummaryTypeDef = TypedDict(
-    "VocabularySummaryTypeDef",
+VocabularyOutputTypeDef = TypedDict(
+    "VocabularyOutputTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
         "FailureReason": str,
+        "Content": str,
+        "Tags": Dict[str, str],
     },
 )
 
-VocabularyTypeDef = TypedDict(
-    "VocabularyTypeDef",
+VocabularySummaryOutputTypeDef = TypedDict(
+    "VocabularySummaryOutputTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
         "FailureReason": str,
-        "Content": str,
-        "Tags": Dict[str, str],
     },
 )
 
 VoiceRecordingConfigurationTypeDef = TypedDict(
     "VoiceRecordingConfigurationTypeDef",
     {
         "VoiceRecordingTrack": VoiceRecordingTrackType,
     },
     total=False,
 )
 
-WisdomInfoTypeDef = TypedDict(
-    "WisdomInfoTypeDef",
+WisdomInfoOutputTypeDef = TypedDict(
+    "WisdomInfoOutputTypeDef",
     {
         "SessionArn": str,
     },
 )
```

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/PKG-INFO` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.28.3
-Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
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
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -578,101 +578,103 @@
 ### Typed dictionaries
 
 `mypy_boto3_connect.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connect.type_defs import (
-    ActionSummaryTypeDef,
+    ActionSummaryOutputTypeDef,
     ActivateEvaluationFormRequestRequestTypeDef,
-    ActivateEvaluationFormResponseTypeDef,
-    AgentContactReferenceTypeDef,
-    AgentInfoTypeDef,
-    AgentStatusReferenceTypeDef,
-    AgentStatusSummaryTypeDef,
-    AgentStatusTypeDef,
+    ActivateEvaluationFormResponseOutputTypeDef,
+    AgentContactReferenceOutputTypeDef,
+    AgentInfoOutputTypeDef,
+    AgentStatusOutputTypeDef,
+    AgentStatusReferenceOutputTypeDef,
+    AgentStatusSummaryOutputTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     AssociateApprovedOriginRequestRequestTypeDef,
     AssociateBotRequestRequestTypeDef,
     AssociateDefaultVocabularyRequestRequestTypeDef,
     AssociateInstanceStorageConfigRequestRequestTypeDef,
-    AssociateInstanceStorageConfigResponseTypeDef,
+    AssociateInstanceStorageConfigResponseOutputTypeDef,
     AssociateLambdaFunctionRequestRequestTypeDef,
     AssociateLexBotRequestRequestTypeDef,
     AssociatePhoneNumberContactFlowRequestRequestTypeDef,
     AssociateQueueQuickConnectsRequestRequestTypeDef,
     AssociateRoutingProfileQueuesRequestRequestTypeDef,
     AssociateSecurityKeyRequestRequestTypeDef,
-    AssociateSecurityKeyResponseTypeDef,
-    AttachmentReferenceTypeDef,
-    AttributeTypeDef,
-    AvailableNumberSummaryTypeDef,
+    AssociateSecurityKeyResponseOutputTypeDef,
+    AttachmentReferenceOutputTypeDef,
+    AttributeOutputTypeDef,
+    AvailableNumberSummaryOutputTypeDef,
     ChatMessageTypeDef,
     ChatParticipantRoleConfigTypeDef,
     ChatStreamingConfigurationTypeDef,
     ClaimPhoneNumberRequestRequestTypeDef,
-    ClaimPhoneNumberResponseTypeDef,
-    ClaimedPhoneNumberSummaryTypeDef,
+    ClaimPhoneNumberResponseOutputTypeDef,
+    ClaimedPhoneNumberSummaryOutputTypeDef,
     ContactFilterTypeDef,
-    ContactFlowModuleSummaryTypeDef,
-    ContactFlowModuleTypeDef,
-    ContactFlowSummaryTypeDef,
-    ContactFlowTypeDef,
-    ContactTypeDef,
+    ContactFlowModuleOutputTypeDef,
+    ContactFlowModuleSummaryOutputTypeDef,
+    ContactFlowOutputTypeDef,
+    ContactFlowSummaryOutputTypeDef,
+    ContactOutputTypeDef,
     ControlPlaneTagFilterTypeDef,
     CreateAgentStatusRequestRequestTypeDef,
-    CreateAgentStatusResponseTypeDef,
+    CreateAgentStatusResponseOutputTypeDef,
     CreateContactFlowModuleRequestRequestTypeDef,
-    CreateContactFlowModuleResponseTypeDef,
+    CreateContactFlowModuleResponseOutputTypeDef,
     CreateContactFlowRequestRequestTypeDef,
-    CreateContactFlowResponseTypeDef,
+    CreateContactFlowResponseOutputTypeDef,
     CreateEvaluationFormRequestRequestTypeDef,
-    CreateEvaluationFormResponseTypeDef,
+    CreateEvaluationFormResponseOutputTypeDef,
     CreateHoursOfOperationRequestRequestTypeDef,
-    CreateHoursOfOperationResponseTypeDef,
+    CreateHoursOfOperationResponseOutputTypeDef,
     CreateInstanceRequestRequestTypeDef,
-    CreateInstanceResponseTypeDef,
+    CreateInstanceResponseOutputTypeDef,
     CreateIntegrationAssociationRequestRequestTypeDef,
-    CreateIntegrationAssociationResponseTypeDef,
+    CreateIntegrationAssociationResponseOutputTypeDef,
     CreateParticipantRequestRequestTypeDef,
-    CreateParticipantResponseTypeDef,
+    CreateParticipantResponseOutputTypeDef,
     CreatePromptRequestRequestTypeDef,
-    CreatePromptResponseTypeDef,
+    CreatePromptResponseOutputTypeDef,
     CreateQueueRequestRequestTypeDef,
-    CreateQueueResponseTypeDef,
+    CreateQueueResponseOutputTypeDef,
     CreateQuickConnectRequestRequestTypeDef,
-    CreateQuickConnectResponseTypeDef,
+    CreateQuickConnectResponseOutputTypeDef,
     CreateRoutingProfileRequestRequestTypeDef,
-    CreateRoutingProfileResponseTypeDef,
+    CreateRoutingProfileResponseOutputTypeDef,
     CreateRuleRequestRequestTypeDef,
-    CreateRuleResponseTypeDef,
+    CreateRuleResponseOutputTypeDef,
     CreateSecurityProfileRequestRequestTypeDef,
-    CreateSecurityProfileResponseTypeDef,
+    CreateSecurityProfileResponseOutputTypeDef,
     CreateTaskTemplateRequestRequestTypeDef,
-    CreateTaskTemplateResponseTypeDef,
+    CreateTaskTemplateResponseOutputTypeDef,
     CreateTrafficDistributionGroupRequestRequestTypeDef,
-    CreateTrafficDistributionGroupResponseTypeDef,
+    CreateTrafficDistributionGroupResponseOutputTypeDef,
     CreateUseCaseRequestRequestTypeDef,
-    CreateUseCaseResponseTypeDef,
+    CreateUseCaseResponseOutputTypeDef,
     CreateUserHierarchyGroupRequestRequestTypeDef,
-    CreateUserHierarchyGroupResponseTypeDef,
+    CreateUserHierarchyGroupResponseOutputTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseTypeDef,
+    CreateUserResponseOutputTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    CreateVocabularyResponseTypeDef,
-    CredentialsTypeDef,
+    CreateVocabularyResponseOutputTypeDef,
+    CredentialsOutputTypeDef,
+    CrossChannelBehaviorOutputTypeDef,
     CrossChannelBehaviorTypeDef,
-    CurrentMetricDataTypeDef,
-    CurrentMetricResultTypeDef,
+    CurrentMetricDataOutputTypeDef,
+    CurrentMetricOutputTypeDef,
+    CurrentMetricResultOutputTypeDef,
     CurrentMetricSortCriteriaTypeDef,
     CurrentMetricTypeDef,
-    DateReferenceTypeDef,
+    DateReferenceOutputTypeDef,
     DeactivateEvaluationFormRequestRequestTypeDef,
-    DeactivateEvaluationFormResponseTypeDef,
-    DefaultVocabularyTypeDef,
+    DeactivateEvaluationFormResponseOutputTypeDef,
+    DefaultVocabularyOutputTypeDef,
     DeleteContactEvaluationRequestRequestTypeDef,
     DeleteContactFlowModuleRequestRequestTypeDef,
     DeleteContactFlowRequestRequestTypeDef,
     DeleteEvaluationFormRequestRequestTypeDef,
     DeleteHoursOfOperationRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteIntegrationAssociationRequestRequestTypeDef,
@@ -684,460 +686,516 @@
     DeleteSecurityProfileRequestRequestTypeDef,
     DeleteTaskTemplateRequestRequestTypeDef,
     DeleteTrafficDistributionGroupRequestRequestTypeDef,
     DeleteUseCaseRequestRequestTypeDef,
     DeleteUserHierarchyGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
-    DeleteVocabularyResponseTypeDef,
+    DeleteVocabularyResponseOutputTypeDef,
     DescribeAgentStatusRequestRequestTypeDef,
-    DescribeAgentStatusResponseTypeDef,
+    DescribeAgentStatusResponseOutputTypeDef,
     DescribeContactEvaluationRequestRequestTypeDef,
-    DescribeContactEvaluationResponseTypeDef,
+    DescribeContactEvaluationResponseOutputTypeDef,
     DescribeContactFlowModuleRequestRequestTypeDef,
-    DescribeContactFlowModuleResponseTypeDef,
+    DescribeContactFlowModuleResponseOutputTypeDef,
     DescribeContactFlowRequestRequestTypeDef,
-    DescribeContactFlowResponseTypeDef,
+    DescribeContactFlowResponseOutputTypeDef,
     DescribeContactRequestRequestTypeDef,
-    DescribeContactResponseTypeDef,
+    DescribeContactResponseOutputTypeDef,
     DescribeEvaluationFormRequestRequestTypeDef,
-    DescribeEvaluationFormResponseTypeDef,
+    DescribeEvaluationFormResponseOutputTypeDef,
     DescribeHoursOfOperationRequestRequestTypeDef,
-    DescribeHoursOfOperationResponseTypeDef,
+    DescribeHoursOfOperationResponseOutputTypeDef,
     DescribeInstanceAttributeRequestRequestTypeDef,
-    DescribeInstanceAttributeResponseTypeDef,
+    DescribeInstanceAttributeResponseOutputTypeDef,
     DescribeInstanceRequestRequestTypeDef,
-    DescribeInstanceResponseTypeDef,
+    DescribeInstanceResponseOutputTypeDef,
     DescribeInstanceStorageConfigRequestRequestTypeDef,
-    DescribeInstanceStorageConfigResponseTypeDef,
+    DescribeInstanceStorageConfigResponseOutputTypeDef,
     DescribePhoneNumberRequestRequestTypeDef,
-    DescribePhoneNumberResponseTypeDef,
+    DescribePhoneNumberResponseOutputTypeDef,
     DescribePromptRequestRequestTypeDef,
-    DescribePromptResponseTypeDef,
+    DescribePromptResponseOutputTypeDef,
     DescribeQueueRequestRequestTypeDef,
-    DescribeQueueResponseTypeDef,
+    DescribeQueueResponseOutputTypeDef,
     DescribeQuickConnectRequestRequestTypeDef,
-    DescribeQuickConnectResponseTypeDef,
+    DescribeQuickConnectResponseOutputTypeDef,
     DescribeRoutingProfileRequestRequestTypeDef,
-    DescribeRoutingProfileResponseTypeDef,
+    DescribeRoutingProfileResponseOutputTypeDef,
     DescribeRuleRequestRequestTypeDef,
-    DescribeRuleResponseTypeDef,
+    DescribeRuleResponseOutputTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
-    DescribeSecurityProfileResponseTypeDef,
+    DescribeSecurityProfileResponseOutputTypeDef,
     DescribeTrafficDistributionGroupRequestRequestTypeDef,
-    DescribeTrafficDistributionGroupResponseTypeDef,
+    DescribeTrafficDistributionGroupResponseOutputTypeDef,
     DescribeUserHierarchyGroupRequestRequestTypeDef,
-    DescribeUserHierarchyGroupResponseTypeDef,
+    DescribeUserHierarchyGroupResponseOutputTypeDef,
     DescribeUserHierarchyStructureRequestRequestTypeDef,
-    DescribeUserHierarchyStructureResponseTypeDef,
+    DescribeUserHierarchyStructureResponseOutputTypeDef,
     DescribeUserRequestRequestTypeDef,
-    DescribeUserResponseTypeDef,
+    DescribeUserResponseOutputTypeDef,
     DescribeVocabularyRequestRequestTypeDef,
-    DescribeVocabularyResponseTypeDef,
-    DimensionsTypeDef,
+    DescribeVocabularyResponseOutputTypeDef,
+    DimensionsOutputTypeDef,
     DisassociateApprovedOriginRequestRequestTypeDef,
     DisassociateBotRequestRequestTypeDef,
     DisassociateInstanceStorageConfigRequestRequestTypeDef,
     DisassociateLambdaFunctionRequestRequestTypeDef,
     DisassociateLexBotRequestRequestTypeDef,
     DisassociatePhoneNumberContactFlowRequestRequestTypeDef,
     DisassociateQueueQuickConnectsRequestRequestTypeDef,
     DisassociateRoutingProfileQueuesRequestRequestTypeDef,
     DisassociateSecurityKeyRequestRequestTypeDef,
     DismissUserContactRequestRequestTypeDef,
+    DistributionOutputTypeDef,
     DistributionTypeDef,
-    EmailReferenceTypeDef,
+    EmailReferenceOutputTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    EvaluationAnswerDataOutputTypeDef,
     EvaluationAnswerDataTypeDef,
     EvaluationAnswerInputTypeDef,
-    EvaluationAnswerOutputTypeDef,
-    EvaluationFormContentTypeDef,
+    EvaluationAnswerOutputOutputTypeDef,
+    EvaluationFormContentOutputTypeDef,
+    EvaluationFormItemOutputTypeDef,
     EvaluationFormItemTypeDef,
+    EvaluationFormNumericQuestionAutomationOutputTypeDef,
     EvaluationFormNumericQuestionAutomationTypeDef,
+    EvaluationFormNumericQuestionOptionOutputTypeDef,
     EvaluationFormNumericQuestionOptionTypeDef,
+    EvaluationFormNumericQuestionPropertiesOutputTypeDef,
     EvaluationFormNumericQuestionPropertiesTypeDef,
+    EvaluationFormOutputTypeDef,
+    EvaluationFormQuestionOutputTypeDef,
     EvaluationFormQuestionTypeDef,
+    EvaluationFormQuestionTypePropertiesOutputTypeDef,
     EvaluationFormQuestionTypePropertiesTypeDef,
+    EvaluationFormScoringStrategyOutputTypeDef,
     EvaluationFormScoringStrategyTypeDef,
+    EvaluationFormSectionOutputTypeDef,
     EvaluationFormSectionTypeDef,
+    EvaluationFormSingleSelectQuestionAutomationOptionOutputTypeDef,
     EvaluationFormSingleSelectQuestionAutomationOptionTypeDef,
+    EvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
     EvaluationFormSingleSelectQuestionAutomationTypeDef,
+    EvaluationFormSingleSelectQuestionOptionOutputTypeDef,
     EvaluationFormSingleSelectQuestionOptionTypeDef,
+    EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
     EvaluationFormSingleSelectQuestionPropertiesTypeDef,
-    EvaluationFormSummaryTypeDef,
-    EvaluationFormTypeDef,
-    EvaluationFormVersionSummaryTypeDef,
-    EvaluationMetadataTypeDef,
+    EvaluationFormSummaryOutputTypeDef,
+    EvaluationFormVersionSummaryOutputTypeDef,
+    EvaluationMetadataOutputTypeDef,
+    EvaluationNoteOutputTypeDef,
     EvaluationNoteTypeDef,
-    EvaluationScoreTypeDef,
-    EvaluationSummaryTypeDef,
-    EvaluationTypeDef,
+    EvaluationOutputTypeDef,
+    EvaluationScoreOutputTypeDef,
+    EvaluationSummaryOutputTypeDef,
+    EventBridgeActionDefinitionOutputTypeDef,
     EventBridgeActionDefinitionTypeDef,
     FilterV2TypeDef,
     FiltersTypeDef,
     GetContactAttributesRequestRequestTypeDef,
-    GetContactAttributesResponseTypeDef,
+    GetContactAttributesResponseOutputTypeDef,
     GetCurrentMetricDataRequestRequestTypeDef,
-    GetCurrentMetricDataResponseTypeDef,
+    GetCurrentMetricDataResponseOutputTypeDef,
     GetCurrentUserDataRequestRequestTypeDef,
-    GetCurrentUserDataResponseTypeDef,
+    GetCurrentUserDataResponseOutputTypeDef,
     GetFederationTokenRequestRequestTypeDef,
-    GetFederationTokenResponseTypeDef,
+    GetFederationTokenResponseOutputTypeDef,
     GetMetricDataRequestGetMetricDataPaginateTypeDef,
     GetMetricDataRequestRequestTypeDef,
-    GetMetricDataResponseTypeDef,
+    GetMetricDataResponseOutputTypeDef,
     GetMetricDataV2RequestRequestTypeDef,
-    GetMetricDataV2ResponseTypeDef,
+    GetMetricDataV2ResponseOutputTypeDef,
     GetPromptFileRequestRequestTypeDef,
-    GetPromptFileResponseTypeDef,
+    GetPromptFileResponseOutputTypeDef,
     GetTaskTemplateRequestRequestTypeDef,
-    GetTaskTemplateResponseTypeDef,
+    GetTaskTemplateResponseOutputTypeDef,
     GetTrafficDistributionRequestRequestTypeDef,
-    GetTrafficDistributionResponseTypeDef,
+    GetTrafficDistributionResponseOutputTypeDef,
     HierarchyGroupConditionTypeDef,
-    HierarchyGroupSummaryReferenceTypeDef,
-    HierarchyGroupSummaryTypeDef,
-    HierarchyGroupTypeDef,
-    HierarchyLevelTypeDef,
+    HierarchyGroupOutputTypeDef,
+    HierarchyGroupSummaryOutputTypeDef,
+    HierarchyGroupSummaryReferenceOutputTypeDef,
+    HierarchyLevelOutputTypeDef,
     HierarchyLevelUpdateTypeDef,
-    HierarchyPathReferenceTypeDef,
-    HierarchyPathTypeDef,
-    HierarchyStructureTypeDef,
+    HierarchyPathOutputTypeDef,
+    HierarchyPathReferenceOutputTypeDef,
+    HierarchyStructureOutputTypeDef,
     HierarchyStructureUpdateTypeDef,
-    HistoricalMetricDataTypeDef,
-    HistoricalMetricResultTypeDef,
+    HistoricalMetricDataOutputTypeDef,
+    HistoricalMetricOutputTypeDef,
+    HistoricalMetricResultOutputTypeDef,
     HistoricalMetricTypeDef,
+    HoursOfOperationConfigOutputTypeDef,
     HoursOfOperationConfigTypeDef,
+    HoursOfOperationOutputTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
-    HoursOfOperationSummaryTypeDef,
+    HoursOfOperationSummaryOutputTypeDef,
+    HoursOfOperationTimeSliceOutputTypeDef,
     HoursOfOperationTimeSliceTypeDef,
-    HoursOfOperationTypeDef,
-    InstanceStatusReasonTypeDef,
+    InstanceOutputTypeDef,
+    InstanceStatusReasonOutputTypeDef,
+    InstanceStorageConfigOutputTypeDef,
     InstanceStorageConfigTypeDef,
-    InstanceSummaryTypeDef,
-    InstanceTypeDef,
-    IntegrationAssociationSummaryTypeDef,
+    InstanceSummaryOutputTypeDef,
+    IntegrationAssociationSummaryOutputTypeDef,
+    InvisibleFieldInfoOutputTypeDef,
     InvisibleFieldInfoTypeDef,
+    KinesisFirehoseConfigOutputTypeDef,
     KinesisFirehoseConfigTypeDef,
+    KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
+    KinesisVideoStreamConfigOutputTypeDef,
     KinesisVideoStreamConfigTypeDef,
-    LexBotConfigTypeDef,
+    LexBotConfigOutputTypeDef,
+    LexBotOutputTypeDef,
     LexBotTypeDef,
+    LexV2BotOutputTypeDef,
     LexV2BotTypeDef,
     ListAgentStatusRequestListAgentStatusesPaginateTypeDef,
     ListAgentStatusRequestRequestTypeDef,
-    ListAgentStatusResponseTypeDef,
+    ListAgentStatusResponseOutputTypeDef,
     ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
     ListApprovedOriginsRequestRequestTypeDef,
-    ListApprovedOriginsResponseTypeDef,
+    ListApprovedOriginsResponseOutputTypeDef,
     ListBotsRequestListBotsPaginateTypeDef,
     ListBotsRequestRequestTypeDef,
-    ListBotsResponseTypeDef,
+    ListBotsResponseOutputTypeDef,
     ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
     ListContactEvaluationsRequestRequestTypeDef,
-    ListContactEvaluationsResponseTypeDef,
+    ListContactEvaluationsResponseOutputTypeDef,
     ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
     ListContactFlowModulesRequestRequestTypeDef,
-    ListContactFlowModulesResponseTypeDef,
+    ListContactFlowModulesResponseOutputTypeDef,
     ListContactFlowsRequestListContactFlowsPaginateTypeDef,
     ListContactFlowsRequestRequestTypeDef,
-    ListContactFlowsResponseTypeDef,
+    ListContactFlowsResponseOutputTypeDef,
     ListContactReferencesRequestListContactReferencesPaginateTypeDef,
     ListContactReferencesRequestRequestTypeDef,
-    ListContactReferencesResponseTypeDef,
+    ListContactReferencesResponseOutputTypeDef,
     ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
     ListDefaultVocabulariesRequestRequestTypeDef,
-    ListDefaultVocabulariesResponseTypeDef,
+    ListDefaultVocabulariesResponseOutputTypeDef,
     ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
     ListEvaluationFormVersionsRequestRequestTypeDef,
-    ListEvaluationFormVersionsResponseTypeDef,
+    ListEvaluationFormVersionsResponseOutputTypeDef,
     ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
     ListEvaluationFormsRequestRequestTypeDef,
-    ListEvaluationFormsResponseTypeDef,
+    ListEvaluationFormsResponseOutputTypeDef,
     ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
     ListHoursOfOperationsRequestRequestTypeDef,
-    ListHoursOfOperationsResponseTypeDef,
+    ListHoursOfOperationsResponseOutputTypeDef,
     ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
     ListInstanceAttributesRequestRequestTypeDef,
-    ListInstanceAttributesResponseTypeDef,
+    ListInstanceAttributesResponseOutputTypeDef,
     ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
     ListInstanceStorageConfigsRequestRequestTypeDef,
-    ListInstanceStorageConfigsResponseTypeDef,
+    ListInstanceStorageConfigsResponseOutputTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
-    ListInstancesResponseTypeDef,
+    ListInstancesResponseOutputTypeDef,
     ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
     ListIntegrationAssociationsRequestRequestTypeDef,
-    ListIntegrationAssociationsResponseTypeDef,
+    ListIntegrationAssociationsResponseOutputTypeDef,
     ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
     ListLambdaFunctionsRequestRequestTypeDef,
-    ListLambdaFunctionsResponseTypeDef,
+    ListLambdaFunctionsResponseOutputTypeDef,
     ListLexBotsRequestListLexBotsPaginateTypeDef,
     ListLexBotsRequestRequestTypeDef,
-    ListLexBotsResponseTypeDef,
+    ListLexBotsResponseOutputTypeDef,
     ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
-    ListPhoneNumbersResponseTypeDef,
-    ListPhoneNumbersSummaryTypeDef,
+    ListPhoneNumbersResponseOutputTypeDef,
+    ListPhoneNumbersSummaryOutputTypeDef,
     ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef,
     ListPhoneNumbersV2RequestRequestTypeDef,
-    ListPhoneNumbersV2ResponseTypeDef,
+    ListPhoneNumbersV2ResponseOutputTypeDef,
     ListPromptsRequestListPromptsPaginateTypeDef,
     ListPromptsRequestRequestTypeDef,
-    ListPromptsResponseTypeDef,
+    ListPromptsResponseOutputTypeDef,
     ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
     ListQueueQuickConnectsRequestRequestTypeDef,
-    ListQueueQuickConnectsResponseTypeDef,
+    ListQueueQuickConnectsResponseOutputTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResponseTypeDef,
+    ListQueuesResponseOutputTypeDef,
     ListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
     ListQuickConnectsRequestRequestTypeDef,
-    ListQuickConnectsResponseTypeDef,
+    ListQuickConnectsResponseOutputTypeDef,
     ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
     ListRoutingProfileQueuesRequestRequestTypeDef,
-    ListRoutingProfileQueuesResponseTypeDef,
+    ListRoutingProfileQueuesResponseOutputTypeDef,
     ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
     ListRoutingProfilesRequestRequestTypeDef,
-    ListRoutingProfilesResponseTypeDef,
+    ListRoutingProfilesResponseOutputTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListRulesResponseTypeDef,
+    ListRulesResponseOutputTypeDef,
     ListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
     ListSecurityKeysRequestRequestTypeDef,
-    ListSecurityKeysResponseTypeDef,
+    ListSecurityKeysResponseOutputTypeDef,
     ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
     ListSecurityProfilePermissionsRequestRequestTypeDef,
-    ListSecurityProfilePermissionsResponseTypeDef,
+    ListSecurityProfilePermissionsResponseOutputTypeDef,
     ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
-    ListSecurityProfilesResponseTypeDef,
+    ListSecurityProfilesResponseOutputTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
     ListTaskTemplatesRequestRequestTypeDef,
-    ListTaskTemplatesResponseTypeDef,
+    ListTaskTemplatesResponseOutputTypeDef,
     ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef,
     ListTrafficDistributionGroupsRequestRequestTypeDef,
-    ListTrafficDistributionGroupsResponseTypeDef,
+    ListTrafficDistributionGroupsResponseOutputTypeDef,
     ListUseCasesRequestListUseCasesPaginateTypeDef,
     ListUseCasesRequestRequestTypeDef,
-    ListUseCasesResponseTypeDef,
+    ListUseCasesResponseOutputTypeDef,
     ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
     ListUserHierarchyGroupsRequestRequestTypeDef,
-    ListUserHierarchyGroupsResponseTypeDef,
+    ListUserHierarchyGroupsResponseOutputTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListUsersResponseTypeDef,
+    ListUsersResponseOutputTypeDef,
+    MediaConcurrencyOutputTypeDef,
     MediaConcurrencyTypeDef,
-    MetricDataV2TypeDef,
+    MetricDataV2OutputTypeDef,
+    MetricFilterV2OutputTypeDef,
     MetricFilterV2TypeDef,
-    MetricResultV2TypeDef,
+    MetricResultV2OutputTypeDef,
+    MetricV2OutputTypeDef,
     MetricV2TypeDef,
     MonitorContactRequestRequestTypeDef,
-    MonitorContactResponseTypeDef,
+    MonitorContactResponseOutputTypeDef,
+    NotificationRecipientTypeOutputTypeDef,
     NotificationRecipientTypeTypeDef,
-    NumberReferenceTypeDef,
+    NumberReferenceOutputTypeDef,
+    NumericQuestionPropertyValueAutomationOutputTypeDef,
     NumericQuestionPropertyValueAutomationTypeDef,
+    OutboundCallerConfigOutputTypeDef,
     OutboundCallerConfigTypeDef,
     PaginatorConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     ParticipantTimerConfigurationTypeDef,
     ParticipantTimerValueTypeDef,
-    ParticipantTokenCredentialsTypeDef,
+    ParticipantTokenCredentialsOutputTypeDef,
     PersistentChatTypeDef,
+    PhoneNumberQuickConnectConfigOutputTypeDef,
     PhoneNumberQuickConnectConfigTypeDef,
-    PhoneNumberStatusTypeDef,
-    PhoneNumberSummaryTypeDef,
+    PhoneNumberStatusOutputTypeDef,
+    PhoneNumberSummaryOutputTypeDef,
+    PromptOutputTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
-    PromptSummaryTypeDef,
-    PromptTypeDef,
+    PromptSummaryOutputTypeDef,
     PutUserStatusRequestRequestTypeDef,
-    QueueInfoTypeDef,
+    QueueInfoOutputTypeDef,
+    QueueOutputTypeDef,
+    QueueQuickConnectConfigOutputTypeDef,
     QueueQuickConnectConfigTypeDef,
-    QueueReferenceTypeDef,
+    QueueReferenceOutputTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
-    QueueSummaryTypeDef,
-    QueueTypeDef,
+    QueueSummaryOutputTypeDef,
+    QuickConnectConfigOutputTypeDef,
     QuickConnectConfigTypeDef,
+    QuickConnectOutputTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
-    QuickConnectSummaryTypeDef,
-    QuickConnectTypeDef,
+    QuickConnectSummaryOutputTypeDef,
+    ReadOnlyFieldInfoOutputTypeDef,
     ReadOnlyFieldInfoTypeDef,
-    ReferenceSummaryTypeDef,
+    ReferenceOutputTypeDef,
+    ReferenceSummaryOutputTypeDef,
     ReferenceTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
     ReplicateInstanceRequestRequestTypeDef,
-    ReplicateInstanceResponseTypeDef,
+    ReplicateInstanceResponseOutputTypeDef,
+    RequiredFieldInfoOutputTypeDef,
     RequiredFieldInfoTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     ResponseMetadataTypeDef,
     ResumeContactRecordingRequestRequestTypeDef,
-    RoutingProfileQueueConfigSummaryTypeDef,
+    RoutingProfileOutputTypeDef,
+    RoutingProfileQueueConfigSummaryOutputTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
-    RoutingProfileReferenceTypeDef,
+    RoutingProfileReferenceOutputTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    RoutingProfileSummaryTypeDef,
-    RoutingProfileTypeDef,
+    RoutingProfileSummaryOutputTypeDef,
+    RuleActionOutputTypeDef,
     RuleActionTypeDef,
-    RuleSummaryTypeDef,
+    RuleOutputTypeDef,
+    RuleSummaryOutputTypeDef,
+    RuleTriggerEventSourceOutputTypeDef,
     RuleTriggerEventSourceTypeDef,
-    RuleTypeDef,
+    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseOutputTypeDef,
     SearchHoursOfOperationsRequestRequestTypeDef,
     SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
-    SearchHoursOfOperationsResponseTypeDef,
+    SearchHoursOfOperationsResponseOutputTypeDef,
     SearchPromptsRequestRequestTypeDef,
     SearchPromptsRequestSearchPromptsPaginateTypeDef,
-    SearchPromptsResponseTypeDef,
+    SearchPromptsResponseOutputTypeDef,
     SearchQueuesRequestRequestTypeDef,
     SearchQueuesRequestSearchQueuesPaginateTypeDef,
-    SearchQueuesResponseTypeDef,
+    SearchQueuesResponseOutputTypeDef,
     SearchQuickConnectsRequestRequestTypeDef,
     SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
-    SearchQuickConnectsResponseTypeDef,
+    SearchQuickConnectsResponseOutputTypeDef,
     SearchResourceTagsRequestRequestTypeDef,
     SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
-    SearchResourceTagsResponseTypeDef,
+    SearchResourceTagsResponseOutputTypeDef,
     SearchRoutingProfilesRequestRequestTypeDef,
     SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
-    SearchRoutingProfilesResponseTypeDef,
+    SearchRoutingProfilesResponseOutputTypeDef,
     SearchSecurityProfilesRequestRequestTypeDef,
     SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
-    SearchSecurityProfilesResponseTypeDef,
+    SearchSecurityProfilesResponseOutputTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchUsersRequestSearchUsersPaginateTypeDef,
-    SearchUsersResponseTypeDef,
+    SearchUsersResponseOutputTypeDef,
     SearchVocabulariesRequestRequestTypeDef,
     SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
-    SearchVocabulariesResponseTypeDef,
-    SecurityKeyTypeDef,
+    SearchVocabulariesResponseOutputTypeDef,
+    SecurityKeyOutputTypeDef,
+    SecurityProfileOutputTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
-    SecurityProfileSearchSummaryTypeDef,
-    SecurityProfileSummaryTypeDef,
-    SecurityProfileTypeDef,
+    SecurityProfileSearchSummaryOutputTypeDef,
+    SecurityProfileSummaryOutputTypeDef,
     SecurityProfilesSearchFilterTypeDef,
+    SendNotificationActionDefinitionOutputTypeDef,
     SendNotificationActionDefinitionTypeDef,
+    SingleSelectQuestionRuleCategoryAutomationOutputTypeDef,
     SingleSelectQuestionRuleCategoryAutomationTypeDef,
     StartChatContactRequestRequestTypeDef,
-    StartChatContactResponseTypeDef,
+    StartChatContactResponseOutputTypeDef,
     StartContactEvaluationRequestRequestTypeDef,
-    StartContactEvaluationResponseTypeDef,
+    StartContactEvaluationResponseOutputTypeDef,
     StartContactRecordingRequestRequestTypeDef,
     StartContactStreamingRequestRequestTypeDef,
-    StartContactStreamingResponseTypeDef,
+    StartContactStreamingResponseOutputTypeDef,
     StartOutboundVoiceContactRequestRequestTypeDef,
-    StartOutboundVoiceContactResponseTypeDef,
+    StartOutboundVoiceContactResponseOutputTypeDef,
     StartTaskContactRequestRequestTypeDef,
-    StartTaskContactResponseTypeDef,
+    StartTaskContactResponseOutputTypeDef,
     StopContactRecordingRequestRequestTypeDef,
     StopContactRequestRequestTypeDef,
     StopContactStreamingRequestRequestTypeDef,
     StringConditionTypeDef,
-    StringReferenceTypeDef,
+    StringReferenceOutputTypeDef,
     SubmitContactEvaluationRequestRequestTypeDef,
-    SubmitContactEvaluationResponseTypeDef,
+    SubmitContactEvaluationResponseOutputTypeDef,
     SuspendContactRecordingRequestRequestTypeDef,
     TagConditionTypeDef,
     TagResourceRequestRequestTypeDef,
     TagSearchConditionTypeDef,
-    TagSetTypeDef,
+    TagSetOutputTypeDef,
+    TaskActionDefinitionOutputTypeDef,
     TaskActionDefinitionTypeDef,
+    TaskTemplateConstraintsOutputTypeDef,
     TaskTemplateConstraintsTypeDef,
+    TaskTemplateDefaultFieldValueOutputTypeDef,
     TaskTemplateDefaultFieldValueTypeDef,
+    TaskTemplateDefaultsOutputTypeDef,
     TaskTemplateDefaultsTypeDef,
+    TaskTemplateFieldIdentifierOutputTypeDef,
     TaskTemplateFieldIdentifierTypeDef,
+    TaskTemplateFieldOutputTypeDef,
     TaskTemplateFieldTypeDef,
-    TaskTemplateMetadataTypeDef,
+    TaskTemplateMetadataOutputTypeDef,
+    TelephonyConfigOutputTypeDef,
     TelephonyConfigTypeDef,
+    ThresholdOutputTypeDef,
     ThresholdTypeDef,
+    ThresholdV2OutputTypeDef,
     ThresholdV2TypeDef,
-    TrafficDistributionGroupSummaryTypeDef,
-    TrafficDistributionGroupTypeDef,
+    TrafficDistributionGroupOutputTypeDef,
+    TrafficDistributionGroupSummaryOutputTypeDef,
     TransferContactRequestRequestTypeDef,
-    TransferContactResponseTypeDef,
+    TransferContactResponseOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     UpdateContactAttributesRequestRequestTypeDef,
     UpdateContactEvaluationRequestRequestTypeDef,
-    UpdateContactEvaluationResponseTypeDef,
+    UpdateContactEvaluationResponseOutputTypeDef,
     UpdateContactFlowContentRequestRequestTypeDef,
     UpdateContactFlowMetadataRequestRequestTypeDef,
     UpdateContactFlowModuleContentRequestRequestTypeDef,
     UpdateContactFlowModuleMetadataRequestRequestTypeDef,
     UpdateContactFlowNameRequestRequestTypeDef,
     UpdateContactRequestRequestTypeDef,
     UpdateContactScheduleRequestRequestTypeDef,
     UpdateEvaluationFormRequestRequestTypeDef,
-    UpdateEvaluationFormResponseTypeDef,
+    UpdateEvaluationFormResponseOutputTypeDef,
     UpdateHoursOfOperationRequestRequestTypeDef,
     UpdateInstanceAttributeRequestRequestTypeDef,
     UpdateInstanceStorageConfigRequestRequestTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     UpdateParticipantRoleConfigRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
-    UpdatePhoneNumberResponseTypeDef,
+    UpdatePhoneNumberResponseOutputTypeDef,
     UpdatePromptRequestRequestTypeDef,
-    UpdatePromptResponseTypeDef,
+    UpdatePromptResponseOutputTypeDef,
     UpdateQueueHoursOfOperationRequestRequestTypeDef,
     UpdateQueueMaxContactsRequestRequestTypeDef,
     UpdateQueueNameRequestRequestTypeDef,
     UpdateQueueOutboundCallerConfigRequestRequestTypeDef,
     UpdateQueueStatusRequestRequestTypeDef,
     UpdateQuickConnectConfigRequestRequestTypeDef,
     UpdateQuickConnectNameRequestRequestTypeDef,
     UpdateRoutingProfileConcurrencyRequestRequestTypeDef,
     UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef,
     UpdateRoutingProfileNameRequestRequestTypeDef,
     UpdateRoutingProfileQueuesRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
     UpdateSecurityProfileRequestRequestTypeDef,
     UpdateTaskTemplateRequestRequestTypeDef,
-    UpdateTaskTemplateResponseTypeDef,
+    UpdateTaskTemplateResponseOutputTypeDef,
     UpdateTrafficDistributionRequestRequestTypeDef,
     UpdateUserHierarchyGroupNameRequestRequestTypeDef,
     UpdateUserHierarchyRequestRequestTypeDef,
     UpdateUserHierarchyStructureRequestRequestTypeDef,
     UpdateUserIdentityInfoRequestRequestTypeDef,
     UpdateUserPhoneConfigRequestRequestTypeDef,
     UpdateUserRoutingProfileRequestRequestTypeDef,
     UpdateUserSecurityProfilesRequestRequestTypeDef,
-    UrlReferenceTypeDef,
-    UseCaseTypeDef,
+    UrlReferenceOutputTypeDef,
+    UseCaseOutputTypeDef,
     UserDataFiltersTypeDef,
-    UserDataTypeDef,
-    UserIdentityInfoLiteTypeDef,
+    UserDataOutputTypeDef,
+    UserIdentityInfoLiteOutputTypeDef,
+    UserIdentityInfoOutputTypeDef,
     UserIdentityInfoTypeDef,
+    UserOutputTypeDef,
+    UserPhoneConfigOutputTypeDef,
     UserPhoneConfigTypeDef,
+    UserQuickConnectConfigOutputTypeDef,
     UserQuickConnectConfigTypeDef,
-    UserReferenceTypeDef,
+    UserReferenceOutputTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
-    UserSearchSummaryTypeDef,
-    UserSummaryTypeDef,
-    UserTypeDef,
-    VocabularySummaryTypeDef,
-    VocabularyTypeDef,
+    UserSearchSummaryOutputTypeDef,
+    UserSummaryOutputTypeDef,
+    VocabularyOutputTypeDef,
+    VocabularySummaryOutputTypeDef,
     VoiceRecordingConfigurationTypeDef,
-    WisdomInfoTypeDef,
+    WisdomInfoOutputTypeDef,
 )
 
 
-def get_structure() -> ActionSummaryTypeDef:
+def get_structure() -> ActionSummaryOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/SOURCES.txt` & `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3/setup.py` & `mypy-boto3-connect-1.28.3.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connect",
-    version="1.28.3",
+    version="1.28.3.post1",
     packages=["mypy_boto3_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.6"
+        "Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.7"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

