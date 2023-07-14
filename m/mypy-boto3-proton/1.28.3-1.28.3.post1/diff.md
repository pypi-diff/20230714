# Comparing `tmp/mypy-boto3-proton-1.28.3.tar.gz` & `tmp/mypy-boto3-proton-1.28.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-proton-1.28.3.tar", last modified: Thu Jul 13 19:49:15 2023, max compression
+gzip compressed data, was "mypy-boto3-proton-1.28.3.post1.tar", last modified: Fri Jul 14 16:18:03 2023, max compression
```

## Comparing `mypy-boto3-proton-1.28.3.tar` & `mypy-boto3-proton-1.28.3.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.197303 mypy-boto3-proton-1.28.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-07-13 19:49:15.197303 mypy-boto3-proton-1.28.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29826 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.197303 mypy-boto3-proton-1.28.3/mypy_boto3_proton/
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    74390 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    74265 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15855 2023-07-13 19:48:25.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-07-13 19:48:24.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-07-13 19:48:24.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   104634 2023-07-13 19:48:26.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   104511 2023-07-13 19:48:26.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-13 19:48:24.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-07-13 19:48:24.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.197303 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:15.197303 mypy-boto3-proton-1.28.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.031734 mypy-boto3-proton-1.28.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32134 2023-07-14 16:18:03.031734 mypy-boto3-proton-1.28.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30647 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.023733 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75426 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75301 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15855 2023-07-14 16:16:59.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26772 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26749 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   107926 2023-07-14 16:17:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107803 2023-07-14 16:17:00.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.031734 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32134 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:18:03.031734 mypy-boto3-proton-1.28.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/setup.py
```

### Comparing `mypy-boto3-proton-1.28.3/LICENSE` & `mypy-boto3-proton-1.28.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3/README.md` & `mypy-boto3-proton-1.28.3.post1/README.md`

 * *Files 19% similar despite different names*

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
 [mypy-boto3-proton docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/).
 
 See how it helps to find and fix potential bugs:
 
@@ -462,84 +462,84 @@
 
 `mypy_boto3_proton.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_proton.type_defs import (
     AcceptEnvironmentAccountConnectionInputRequestTypeDef,
-    EnvironmentAccountConnectionTypeDef,
-    RepositoryBranchTypeDef,
+    EnvironmentAccountConnectionOutputTypeDef,
+    RepositoryBranchOutputTypeDef,
     CancelComponentDeploymentInputRequestTypeDef,
-    ComponentTypeDef,
+    ComponentOutputTypeDef,
     CancelEnvironmentDeploymentInputRequestTypeDef,
     CancelServiceInstanceDeploymentInputRequestTypeDef,
-    ServiceInstanceTypeDef,
+    ServiceInstanceOutputTypeDef,
     CancelServicePipelineDeploymentInputRequestTypeDef,
-    ServicePipelineTypeDef,
+    ServicePipelineOutputTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
-    CompatibleEnvironmentTemplateTypeDef,
-    ComponentStateTypeDef,
-    ComponentSummaryTypeDef,
-    ResourceCountsSummaryTypeDef,
+    CompatibleEnvironmentTemplateOutputTypeDef,
+    ComponentStateOutputTypeDef,
+    ComponentSummaryOutputTypeDef,
+    ResourceCountsSummaryOutputTypeDef,
     TagTypeDef,
     RepositoryBranchInputTypeDef,
-    EnvironmentTemplateTypeDef,
-    EnvironmentTemplateVersionTypeDef,
-    RepositoryTypeDef,
+    EnvironmentTemplateOutputTypeDef,
+    EnvironmentTemplateVersionOutputTypeDef,
+    RepositoryOutputTypeDef,
     CreateServiceSyncConfigInputRequestTypeDef,
-    ServiceSyncConfigTypeDef,
-    ServiceTemplateTypeDef,
+    ServiceSyncConfigOutputTypeDef,
+    ServiceTemplateOutputTypeDef,
     CreateTemplateSyncConfigInputRequestTypeDef,
-    TemplateSyncConfigTypeDef,
+    TemplateSyncConfigOutputTypeDef,
     DeleteComponentInputRequestTypeDef,
     DeleteDeploymentInputRequestTypeDef,
     DeleteEnvironmentAccountConnectionInputRequestTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DeleteEnvironmentTemplateInputRequestTypeDef,
     DeleteEnvironmentTemplateVersionInputRequestTypeDef,
     DeleteRepositoryInputRequestTypeDef,
     DeleteServiceInputRequestTypeDef,
     DeleteServiceSyncConfigInputRequestTypeDef,
     DeleteServiceTemplateInputRequestTypeDef,
     DeleteServiceTemplateVersionInputRequestTypeDef,
     DeleteTemplateSyncConfigInputRequestTypeDef,
-    EnvironmentStateTypeDef,
-    ServiceInstanceStateTypeDef,
-    ServicePipelineStateTypeDef,
-    DeploymentSummaryTypeDef,
-    EnvironmentAccountConnectionSummaryTypeDef,
-    EnvironmentSummaryTypeDef,
+    EnvironmentStateOutputTypeDef,
+    ServiceInstanceStateOutputTypeDef,
+    ServicePipelineStateOutputTypeDef,
+    DeploymentSummaryOutputTypeDef,
+    EnvironmentAccountConnectionSummaryOutputTypeDef,
+    EnvironmentSummaryOutputTypeDef,
     EnvironmentTemplateFilterTypeDef,
-    EnvironmentTemplateSummaryTypeDef,
-    EnvironmentTemplateVersionSummaryTypeDef,
+    EnvironmentTemplateSummaryOutputTypeDef,
+    EnvironmentTemplateVersionSummaryOutputTypeDef,
     WaiterConfigTypeDef,
     GetComponentInputRequestTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetEnvironmentAccountConnectionInputRequestTypeDef,
     GetEnvironmentInputRequestTypeDef,
     GetEnvironmentTemplateInputRequestTypeDef,
     GetEnvironmentTemplateVersionInputRequestTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositorySyncStatusInputRequestTypeDef,
     GetServiceInputRequestTypeDef,
     GetServiceInstanceInputRequestTypeDef,
     GetServiceInstanceSyncStatusInputRequestTypeDef,
-    RevisionTypeDef,
+    RevisionOutputTypeDef,
     GetServiceSyncBlockerSummaryInputRequestTypeDef,
     GetServiceSyncConfigInputRequestTypeDef,
     GetServiceTemplateInputRequestTypeDef,
     GetServiceTemplateVersionInputRequestTypeDef,
     GetTemplateSyncConfigInputRequestTypeDef,
     GetTemplateSyncStatusInputRequestTypeDef,
     ListComponentOutputsInputListComponentOutputsPaginateTypeDef,
     ListComponentOutputsInputRequestTypeDef,
-    OutputTypeDef,
+    OutputOutputTypeDef,
     ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
     ListComponentProvisionedResourcesInputRequestTypeDef,
-    ProvisionedResourceTypeDef,
+    ProvisionedResourceOutputTypeDef,
     ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
     ListDeploymentsInputListDeploymentsPaginateTypeDef,
     ListDeploymentsInputRequestTypeDef,
     ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
     ListEnvironmentAccountConnectionsInputRequestTypeDef,
     ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
@@ -548,183 +548,185 @@
     ListEnvironmentProvisionedResourcesInputRequestTypeDef,
     ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
     ListEnvironmentTemplateVersionsInputRequestTypeDef,
     ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef,
     ListEnvironmentTemplatesInputRequestTypeDef,
     ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
-    RepositorySummaryTypeDef,
+    RepositorySummaryOutputTypeDef,
     ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
     ListRepositorySyncDefinitionsInputRequestTypeDef,
-    RepositorySyncDefinitionTypeDef,
+    RepositorySyncDefinitionOutputTypeDef,
     ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
     ListServiceInstanceOutputsInputRequestTypeDef,
     ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
     ListServiceInstanceProvisionedResourcesInputRequestTypeDef,
     ListServiceInstancesFilterTypeDef,
-    ServiceInstanceSummaryTypeDef,
+    ServiceInstanceSummaryOutputTypeDef,
     ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
     ListServicePipelineOutputsInputRequestTypeDef,
     ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
     ListServicePipelineProvisionedResourcesInputRequestTypeDef,
     ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
     ListServiceTemplateVersionsInputRequestTypeDef,
-    ServiceTemplateVersionSummaryTypeDef,
+    ServiceTemplateVersionSummaryOutputTypeDef,
     ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef,
     ListServiceTemplatesInputRequestTypeDef,
-    ServiceTemplateSummaryTypeDef,
+    ServiceTemplateSummaryOutputTypeDef,
     ListServicesInputListServicesPaginateTypeDef,
     ListServicesInputRequestTypeDef,
-    ServiceSummaryTypeDef,
+    ServiceSummaryOutputTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TagOutputTypeDef,
+    OutputTypeDef,
     PaginatorConfigTypeDef,
     RejectEnvironmentAccountConnectionInputRequestTypeDef,
-    RepositorySyncEventTypeDef,
-    ResourceSyncEventTypeDef,
+    RepositorySyncEventOutputTypeDef,
+    ResourceSyncEventOutputTypeDef,
     ResponseMetadataTypeDef,
     S3ObjectSourceTypeDef,
-    SyncBlockerContextTypeDef,
+    SyncBlockerContextOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateComponentInputRequestTypeDef,
     UpdateEnvironmentAccountConnectionInputRequestTypeDef,
     UpdateEnvironmentTemplateInputRequestTypeDef,
     UpdateEnvironmentTemplateVersionInputRequestTypeDef,
     UpdateServiceInputRequestTypeDef,
     UpdateServiceInstanceInputRequestTypeDef,
     UpdateServicePipelineInputRequestTypeDef,
     UpdateServiceSyncBlockerInputRequestTypeDef,
     UpdateServiceSyncConfigInputRequestTypeDef,
     UpdateServiceTemplateInputRequestTypeDef,
     UpdateTemplateSyncConfigInputRequestTypeDef,
-    AcceptEnvironmentAccountConnectionOutputTypeDef,
-    CreateEnvironmentAccountConnectionOutputTypeDef,
-    DeleteEnvironmentAccountConnectionOutputTypeDef,
-    GetEnvironmentAccountConnectionOutputTypeDef,
-    RejectEnvironmentAccountConnectionOutputTypeDef,
-    UpdateEnvironmentAccountConnectionOutputTypeDef,
-    AccountSettingsTypeDef,
-    EnvironmentTypeDef,
-    CancelComponentDeploymentOutputTypeDef,
-    CreateComponentOutputTypeDef,
-    DeleteComponentOutputTypeDef,
-    GetComponentOutputTypeDef,
-    UpdateComponentOutputTypeDef,
-    CancelServiceInstanceDeploymentOutputTypeDef,
-    CreateServiceInstanceOutputTypeDef,
-    GetServiceInstanceOutputTypeDef,
-    UpdateServiceInstanceOutputTypeDef,
-    CancelServicePipelineDeploymentOutputTypeDef,
-    ServiceTypeDef,
-    UpdateServicePipelineOutputTypeDef,
+    AcceptEnvironmentAccountConnectionOutputOutputTypeDef,
+    CreateEnvironmentAccountConnectionOutputOutputTypeDef,
+    DeleteEnvironmentAccountConnectionOutputOutputTypeDef,
+    GetEnvironmentAccountConnectionOutputOutputTypeDef,
+    RejectEnvironmentAccountConnectionOutputOutputTypeDef,
+    UpdateEnvironmentAccountConnectionOutputOutputTypeDef,
+    AccountSettingsOutputTypeDef,
+    EnvironmentOutputTypeDef,
+    CancelComponentDeploymentOutputOutputTypeDef,
+    CreateComponentOutputOutputTypeDef,
+    DeleteComponentOutputOutputTypeDef,
+    GetComponentOutputOutputTypeDef,
+    UpdateComponentOutputOutputTypeDef,
+    CancelServiceInstanceDeploymentOutputOutputTypeDef,
+    CreateServiceInstanceOutputOutputTypeDef,
+    GetServiceInstanceOutputOutputTypeDef,
+    UpdateServiceInstanceOutputOutputTypeDef,
+    CancelServicePipelineDeploymentOutputOutputTypeDef,
+    ServiceOutputTypeDef,
+    UpdateServicePipelineOutputOutputTypeDef,
     UpdateServiceTemplateVersionInputRequestTypeDef,
-    ServiceTemplateVersionTypeDef,
-    ListComponentsOutputTypeDef,
-    CountsSummaryTypeDef,
+    ServiceTemplateVersionOutputTypeDef,
+    ListComponentsOutputOutputTypeDef,
+    CountsSummaryOutputTypeDef,
     CreateComponentInputRequestTypeDef,
     CreateEnvironmentAccountConnectionInputRequestTypeDef,
     CreateEnvironmentTemplateInputRequestTypeDef,
     CreateRepositoryInputRequestTypeDef,
     CreateServiceInputRequestTypeDef,
     CreateServiceInstanceInputRequestTypeDef,
     CreateServiceTemplateInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
-    CreateEnvironmentTemplateOutputTypeDef,
-    DeleteEnvironmentTemplateOutputTypeDef,
-    GetEnvironmentTemplateOutputTypeDef,
-    UpdateEnvironmentTemplateOutputTypeDef,
-    CreateEnvironmentTemplateVersionOutputTypeDef,
-    DeleteEnvironmentTemplateVersionOutputTypeDef,
-    GetEnvironmentTemplateVersionOutputTypeDef,
-    UpdateEnvironmentTemplateVersionOutputTypeDef,
-    CreateRepositoryOutputTypeDef,
-    DeleteRepositoryOutputTypeDef,
-    GetRepositoryOutputTypeDef,
-    CreateServiceSyncConfigOutputTypeDef,
-    DeleteServiceSyncConfigOutputTypeDef,
-    GetServiceSyncConfigOutputTypeDef,
-    UpdateServiceSyncConfigOutputTypeDef,
-    CreateServiceTemplateOutputTypeDef,
-    DeleteServiceTemplateOutputTypeDef,
-    GetServiceTemplateOutputTypeDef,
-    UpdateServiceTemplateOutputTypeDef,
-    CreateTemplateSyncConfigOutputTypeDef,
-    DeleteTemplateSyncConfigOutputTypeDef,
-    GetTemplateSyncConfigOutputTypeDef,
-    UpdateTemplateSyncConfigOutputTypeDef,
-    DeploymentStateTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListEnvironmentAccountConnectionsOutputTypeDef,
-    ListEnvironmentsOutputTypeDef,
+    CreateEnvironmentTemplateOutputOutputTypeDef,
+    DeleteEnvironmentTemplateOutputOutputTypeDef,
+    GetEnvironmentTemplateOutputOutputTypeDef,
+    UpdateEnvironmentTemplateOutputOutputTypeDef,
+    CreateEnvironmentTemplateVersionOutputOutputTypeDef,
+    DeleteEnvironmentTemplateVersionOutputOutputTypeDef,
+    GetEnvironmentTemplateVersionOutputOutputTypeDef,
+    UpdateEnvironmentTemplateVersionOutputOutputTypeDef,
+    CreateRepositoryOutputOutputTypeDef,
+    DeleteRepositoryOutputOutputTypeDef,
+    GetRepositoryOutputOutputTypeDef,
+    CreateServiceSyncConfigOutputOutputTypeDef,
+    DeleteServiceSyncConfigOutputOutputTypeDef,
+    GetServiceSyncConfigOutputOutputTypeDef,
+    UpdateServiceSyncConfigOutputOutputTypeDef,
+    CreateServiceTemplateOutputOutputTypeDef,
+    DeleteServiceTemplateOutputOutputTypeDef,
+    GetServiceTemplateOutputOutputTypeDef,
+    UpdateServiceTemplateOutputOutputTypeDef,
+    CreateTemplateSyncConfigOutputOutputTypeDef,
+    DeleteTemplateSyncConfigOutputOutputTypeDef,
+    GetTemplateSyncConfigOutputOutputTypeDef,
+    UpdateTemplateSyncConfigOutputOutputTypeDef,
+    DeploymentStateOutputTypeDef,
+    ListDeploymentsOutputOutputTypeDef,
+    ListEnvironmentAccountConnectionsOutputOutputTypeDef,
+    ListEnvironmentsOutputOutputTypeDef,
     ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     ListEnvironmentsInputRequestTypeDef,
-    ListEnvironmentTemplatesOutputTypeDef,
-    ListEnvironmentTemplateVersionsOutputTypeDef,
+    ListEnvironmentTemplatesOutputOutputTypeDef,
+    ListEnvironmentTemplateVersionsOutputOutputTypeDef,
     GetComponentInputComponentDeletedWaitTypeDef,
     GetComponentInputComponentDeployedWaitTypeDef,
     GetEnvironmentInputEnvironmentDeployedWaitTypeDef,
     GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef,
     GetServiceInputServiceCreatedWaitTypeDef,
     GetServiceInputServiceDeletedWaitTypeDef,
     GetServiceInputServicePipelineDeployedWaitTypeDef,
     GetServiceInputServiceUpdatedWaitTypeDef,
     GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef,
     GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
-    ListComponentOutputsOutputTypeDef,
-    ListEnvironmentOutputsOutputTypeDef,
-    ListServiceInstanceOutputsOutputTypeDef,
-    ListServicePipelineOutputsOutputTypeDef,
-    NotifyResourceDeploymentStatusChangeInputRequestTypeDef,
-    ListComponentProvisionedResourcesOutputTypeDef,
-    ListEnvironmentProvisionedResourcesOutputTypeDef,
-    ListServiceInstanceProvisionedResourcesOutputTypeDef,
-    ListServicePipelineProvisionedResourcesOutputTypeDef,
-    ListRepositoriesOutputTypeDef,
-    ListRepositorySyncDefinitionsOutputTypeDef,
+    ListComponentOutputsOutputOutputTypeDef,
+    ListEnvironmentOutputsOutputOutputTypeDef,
+    ListServiceInstanceOutputsOutputOutputTypeDef,
+    ListServicePipelineOutputsOutputOutputTypeDef,
+    ListComponentProvisionedResourcesOutputOutputTypeDef,
+    ListEnvironmentProvisionedResourcesOutputOutputTypeDef,
+    ListServiceInstanceProvisionedResourcesOutputOutputTypeDef,
+    ListServicePipelineProvisionedResourcesOutputOutputTypeDef,
+    ListRepositoriesOutputOutputTypeDef,
+    ListRepositorySyncDefinitionsOutputOutputTypeDef,
     ListServiceInstancesInputListServiceInstancesPaginateTypeDef,
     ListServiceInstancesInputRequestTypeDef,
-    ListServiceInstancesOutputTypeDef,
-    ListServiceTemplateVersionsOutputTypeDef,
-    ListServiceTemplatesOutputTypeDef,
-    ListServicesOutputTypeDef,
-    RepositorySyncAttemptTypeDef,
-    ResourceSyncAttemptTypeDef,
+    ListServiceInstancesOutputOutputTypeDef,
+    ListServiceTemplateVersionsOutputOutputTypeDef,
+    ListServiceTemplatesOutputOutputTypeDef,
+    ListServicesOutputOutputTypeDef,
+    ListTagsForResourceOutputOutputTypeDef,
+    NotifyResourceDeploymentStatusChangeInputRequestTypeDef,
+    RepositorySyncAttemptOutputTypeDef,
+    ResourceSyncAttemptOutputTypeDef,
     TemplateVersionSourceInputTypeDef,
-    SyncBlockerTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
-    CancelEnvironmentDeploymentOutputTypeDef,
-    CreateEnvironmentOutputTypeDef,
-    DeleteEnvironmentOutputTypeDef,
-    GetEnvironmentOutputTypeDef,
-    UpdateEnvironmentOutputTypeDef,
-    CreateServiceOutputTypeDef,
-    DeleteServiceOutputTypeDef,
-    GetServiceOutputTypeDef,
-    UpdateServiceOutputTypeDef,
-    CreateServiceTemplateVersionOutputTypeDef,
-    DeleteServiceTemplateVersionOutputTypeDef,
-    GetServiceTemplateVersionOutputTypeDef,
-    UpdateServiceTemplateVersionOutputTypeDef,
-    GetResourcesSummaryOutputTypeDef,
-    DeploymentTypeDef,
-    GetRepositorySyncStatusOutputTypeDef,
-    GetServiceInstanceSyncStatusOutputTypeDef,
-    GetTemplateSyncStatusOutputTypeDef,
+    SyncBlockerOutputTypeDef,
+    GetAccountSettingsOutputOutputTypeDef,
+    UpdateAccountSettingsOutputOutputTypeDef,
+    CancelEnvironmentDeploymentOutputOutputTypeDef,
+    CreateEnvironmentOutputOutputTypeDef,
+    DeleteEnvironmentOutputOutputTypeDef,
+    GetEnvironmentOutputOutputTypeDef,
+    UpdateEnvironmentOutputOutputTypeDef,
+    CreateServiceOutputOutputTypeDef,
+    DeleteServiceOutputOutputTypeDef,
+    GetServiceOutputOutputTypeDef,
+    UpdateServiceOutputOutputTypeDef,
+    CreateServiceTemplateVersionOutputOutputTypeDef,
+    DeleteServiceTemplateVersionOutputOutputTypeDef,
+    GetServiceTemplateVersionOutputOutputTypeDef,
+    UpdateServiceTemplateVersionOutputOutputTypeDef,
+    GetResourcesSummaryOutputOutputTypeDef,
+    DeploymentOutputTypeDef,
+    GetRepositorySyncStatusOutputOutputTypeDef,
+    GetServiceInstanceSyncStatusOutputOutputTypeDef,
+    GetTemplateSyncStatusOutputOutputTypeDef,
     CreateEnvironmentTemplateVersionInputRequestTypeDef,
     CreateServiceTemplateVersionInputRequestTypeDef,
-    ServiceSyncBlockerSummaryTypeDef,
-    UpdateServiceSyncBlockerOutputTypeDef,
-    DeleteDeploymentOutputTypeDef,
-    GetDeploymentOutputTypeDef,
-    GetServiceSyncBlockerSummaryOutputTypeDef,
+    ServiceSyncBlockerSummaryOutputTypeDef,
+    UpdateServiceSyncBlockerOutputOutputTypeDef,
+    DeleteDeploymentOutputOutputTypeDef,
+    GetDeploymentOutputOutputTypeDef,
+    GetServiceSyncBlockerSummaryOutputOutputTypeDef,
 )
 
 
 def get_structure() -> AcceptEnvironmentAccountConnectionInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/__init__.py` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/__init__.pyi` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/__main__.py` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Proton 1.28.3\nVersion:         1.28.3\nBuilder version:"
-        " 7.14.6\nDocs:           "
+        "Type annotations for boto3.Proton 1.28.3\nVersion:         1.28.3.post1\nBuilder version:"
+        " 7.14.7\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton\nOther"
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

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/client.py` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,105 +51,105 @@
     ListServicePipelineProvisionedResourcesPaginator,
     ListServicesPaginator,
     ListServiceTemplatesPaginator,
     ListServiceTemplateVersionsPaginator,
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
-    AcceptEnvironmentAccountConnectionOutputTypeDef,
-    CancelComponentDeploymentOutputTypeDef,
-    CancelEnvironmentDeploymentOutputTypeDef,
-    CancelServiceInstanceDeploymentOutputTypeDef,
-    CancelServicePipelineDeploymentOutputTypeDef,
+    AcceptEnvironmentAccountConnectionOutputOutputTypeDef,
+    CancelComponentDeploymentOutputOutputTypeDef,
+    CancelEnvironmentDeploymentOutputOutputTypeDef,
+    CancelServiceInstanceDeploymentOutputOutputTypeDef,
+    CancelServicePipelineDeploymentOutputOutputTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
-    CreateComponentOutputTypeDef,
-    CreateEnvironmentAccountConnectionOutputTypeDef,
-    CreateEnvironmentOutputTypeDef,
-    CreateEnvironmentTemplateOutputTypeDef,
-    CreateEnvironmentTemplateVersionOutputTypeDef,
-    CreateRepositoryOutputTypeDef,
-    CreateServiceInstanceOutputTypeDef,
-    CreateServiceOutputTypeDef,
-    CreateServiceSyncConfigOutputTypeDef,
-    CreateServiceTemplateOutputTypeDef,
-    CreateServiceTemplateVersionOutputTypeDef,
-    CreateTemplateSyncConfigOutputTypeDef,
-    DeleteComponentOutputTypeDef,
-    DeleteDeploymentOutputTypeDef,
-    DeleteEnvironmentAccountConnectionOutputTypeDef,
-    DeleteEnvironmentOutputTypeDef,
-    DeleteEnvironmentTemplateOutputTypeDef,
-    DeleteEnvironmentTemplateVersionOutputTypeDef,
-    DeleteRepositoryOutputTypeDef,
-    DeleteServiceOutputTypeDef,
-    DeleteServiceSyncConfigOutputTypeDef,
-    DeleteServiceTemplateOutputTypeDef,
-    DeleteServiceTemplateVersionOutputTypeDef,
-    DeleteTemplateSyncConfigOutputTypeDef,
+    CreateComponentOutputOutputTypeDef,
+    CreateEnvironmentAccountConnectionOutputOutputTypeDef,
+    CreateEnvironmentOutputOutputTypeDef,
+    CreateEnvironmentTemplateOutputOutputTypeDef,
+    CreateEnvironmentTemplateVersionOutputOutputTypeDef,
+    CreateRepositoryOutputOutputTypeDef,
+    CreateServiceInstanceOutputOutputTypeDef,
+    CreateServiceOutputOutputTypeDef,
+    CreateServiceSyncConfigOutputOutputTypeDef,
+    CreateServiceTemplateOutputOutputTypeDef,
+    CreateServiceTemplateVersionOutputOutputTypeDef,
+    CreateTemplateSyncConfigOutputOutputTypeDef,
+    DeleteComponentOutputOutputTypeDef,
+    DeleteDeploymentOutputOutputTypeDef,
+    DeleteEnvironmentAccountConnectionOutputOutputTypeDef,
+    DeleteEnvironmentOutputOutputTypeDef,
+    DeleteEnvironmentTemplateOutputOutputTypeDef,
+    DeleteEnvironmentTemplateVersionOutputOutputTypeDef,
+    DeleteRepositoryOutputOutputTypeDef,
+    DeleteServiceOutputOutputTypeDef,
+    DeleteServiceSyncConfigOutputOutputTypeDef,
+    DeleteServiceTemplateOutputOutputTypeDef,
+    DeleteServiceTemplateVersionOutputOutputTypeDef,
+    DeleteTemplateSyncConfigOutputOutputTypeDef,
     EnvironmentTemplateFilterTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    GetComponentOutputTypeDef,
-    GetDeploymentOutputTypeDef,
-    GetEnvironmentAccountConnectionOutputTypeDef,
-    GetEnvironmentOutputTypeDef,
-    GetEnvironmentTemplateOutputTypeDef,
-    GetEnvironmentTemplateVersionOutputTypeDef,
-    GetRepositoryOutputTypeDef,
-    GetRepositorySyncStatusOutputTypeDef,
-    GetResourcesSummaryOutputTypeDef,
-    GetServiceInstanceOutputTypeDef,
-    GetServiceInstanceSyncStatusOutputTypeDef,
-    GetServiceOutputTypeDef,
-    GetServiceSyncBlockerSummaryOutputTypeDef,
-    GetServiceSyncConfigOutputTypeDef,
-    GetServiceTemplateOutputTypeDef,
-    GetServiceTemplateVersionOutputTypeDef,
-    GetTemplateSyncConfigOutputTypeDef,
-    GetTemplateSyncStatusOutputTypeDef,
-    ListComponentOutputsOutputTypeDef,
-    ListComponentProvisionedResourcesOutputTypeDef,
-    ListComponentsOutputTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListEnvironmentAccountConnectionsOutputTypeDef,
-    ListEnvironmentOutputsOutputTypeDef,
-    ListEnvironmentProvisionedResourcesOutputTypeDef,
-    ListEnvironmentsOutputTypeDef,
-    ListEnvironmentTemplatesOutputTypeDef,
-    ListEnvironmentTemplateVersionsOutputTypeDef,
-    ListRepositoriesOutputTypeDef,
-    ListRepositorySyncDefinitionsOutputTypeDef,
-    ListServiceInstanceOutputsOutputTypeDef,
-    ListServiceInstanceProvisionedResourcesOutputTypeDef,
+    GetAccountSettingsOutputOutputTypeDef,
+    GetComponentOutputOutputTypeDef,
+    GetDeploymentOutputOutputTypeDef,
+    GetEnvironmentAccountConnectionOutputOutputTypeDef,
+    GetEnvironmentOutputOutputTypeDef,
+    GetEnvironmentTemplateOutputOutputTypeDef,
+    GetEnvironmentTemplateVersionOutputOutputTypeDef,
+    GetRepositoryOutputOutputTypeDef,
+    GetRepositorySyncStatusOutputOutputTypeDef,
+    GetResourcesSummaryOutputOutputTypeDef,
+    GetServiceInstanceOutputOutputTypeDef,
+    GetServiceInstanceSyncStatusOutputOutputTypeDef,
+    GetServiceOutputOutputTypeDef,
+    GetServiceSyncBlockerSummaryOutputOutputTypeDef,
+    GetServiceSyncConfigOutputOutputTypeDef,
+    GetServiceTemplateOutputOutputTypeDef,
+    GetServiceTemplateVersionOutputOutputTypeDef,
+    GetTemplateSyncConfigOutputOutputTypeDef,
+    GetTemplateSyncStatusOutputOutputTypeDef,
+    ListComponentOutputsOutputOutputTypeDef,
+    ListComponentProvisionedResourcesOutputOutputTypeDef,
+    ListComponentsOutputOutputTypeDef,
+    ListDeploymentsOutputOutputTypeDef,
+    ListEnvironmentAccountConnectionsOutputOutputTypeDef,
+    ListEnvironmentOutputsOutputOutputTypeDef,
+    ListEnvironmentProvisionedResourcesOutputOutputTypeDef,
+    ListEnvironmentsOutputOutputTypeDef,
+    ListEnvironmentTemplatesOutputOutputTypeDef,
+    ListEnvironmentTemplateVersionsOutputOutputTypeDef,
+    ListRepositoriesOutputOutputTypeDef,
+    ListRepositorySyncDefinitionsOutputOutputTypeDef,
+    ListServiceInstanceOutputsOutputOutputTypeDef,
+    ListServiceInstanceProvisionedResourcesOutputOutputTypeDef,
     ListServiceInstancesFilterTypeDef,
-    ListServiceInstancesOutputTypeDef,
-    ListServicePipelineOutputsOutputTypeDef,
-    ListServicePipelineProvisionedResourcesOutputTypeDef,
-    ListServicesOutputTypeDef,
-    ListServiceTemplatesOutputTypeDef,
-    ListServiceTemplateVersionsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
+    ListServiceInstancesOutputOutputTypeDef,
+    ListServicePipelineOutputsOutputOutputTypeDef,
+    ListServicePipelineProvisionedResourcesOutputOutputTypeDef,
+    ListServicesOutputOutputTypeDef,
+    ListServiceTemplatesOutputOutputTypeDef,
+    ListServiceTemplateVersionsOutputOutputTypeDef,
+    ListTagsForResourceOutputOutputTypeDef,
     OutputTypeDef,
-    RejectEnvironmentAccountConnectionOutputTypeDef,
+    RejectEnvironmentAccountConnectionOutputOutputTypeDef,
     RepositoryBranchInputTypeDef,
     TagTypeDef,
     TemplateVersionSourceInputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
-    UpdateComponentOutputTypeDef,
-    UpdateEnvironmentAccountConnectionOutputTypeDef,
-    UpdateEnvironmentOutputTypeDef,
-    UpdateEnvironmentTemplateOutputTypeDef,
-    UpdateEnvironmentTemplateVersionOutputTypeDef,
-    UpdateServiceInstanceOutputTypeDef,
-    UpdateServiceOutputTypeDef,
-    UpdateServicePipelineOutputTypeDef,
-    UpdateServiceSyncBlockerOutputTypeDef,
-    UpdateServiceSyncConfigOutputTypeDef,
-    UpdateServiceTemplateOutputTypeDef,
-    UpdateServiceTemplateVersionOutputTypeDef,
-    UpdateTemplateSyncConfigOutputTypeDef,
+    UpdateAccountSettingsOutputOutputTypeDef,
+    UpdateComponentOutputOutputTypeDef,
+    UpdateEnvironmentAccountConnectionOutputOutputTypeDef,
+    UpdateEnvironmentOutputOutputTypeDef,
+    UpdateEnvironmentTemplateOutputOutputTypeDef,
+    UpdateEnvironmentTemplateVersionOutputOutputTypeDef,
+    UpdateServiceInstanceOutputOutputTypeDef,
+    UpdateServiceOutputOutputTypeDef,
+    UpdateServicePipelineOutputOutputTypeDef,
+    UpdateServiceSyncBlockerOutputOutputTypeDef,
+    UpdateServiceSyncConfigOutputOutputTypeDef,
+    UpdateServiceTemplateOutputOutputTypeDef,
+    UpdateServiceTemplateVersionOutputOutputTypeDef,
+    UpdateTemplateSyncConfigOutputOutputTypeDef,
 )
 from .waiter import (
     ComponentDeletedWaiter,
     ComponentDeployedWaiter,
     EnvironmentDeployedWaiter,
     EnvironmentTemplateVersionRegisteredWaiter,
     ServiceCreatedWaiter,
@@ -203,15 +203,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#exceptions)
         """
 
     def accept_environment_account_connection(
         self, *, id: str
-    ) -> AcceptEnvironmentAccountConnectionOutputTypeDef:
+    ) -> AcceptEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         In a management account, an environment account connection request is accepted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.accept_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#accept_environment_account_connection)
         """
 
@@ -221,48 +221,48 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#can_paginate)
         """
 
     def cancel_component_deployment(
         self, *, componentName: str
-    ) -> CancelComponentDeploymentOutputTypeDef:
+    ) -> CancelComponentDeploymentOutputOutputTypeDef:
         """
         Attempts to cancel a component deployment (for a component that is in the
         `IN_PROGRESS` deployment status).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_component_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_component_deployment)
         """
 
     def cancel_environment_deployment(
         self, *, environmentName: str
-    ) -> CancelEnvironmentDeploymentOutputTypeDef:
+    ) -> CancelEnvironmentDeploymentOutputOutputTypeDef:
         """
         Attempts to cancel an environment deployment on an  UpdateEnvironment action, if
         the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_environment_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_environment_deployment)
         """
 
     def cancel_service_instance_deployment(
         self, *, serviceInstanceName: str, serviceName: str
-    ) -> CancelServiceInstanceDeploymentOutputTypeDef:
+    ) -> CancelServiceInstanceDeploymentOutputOutputTypeDef:
         """
         Attempts to cancel a service instance deployment on an  UpdateServiceInstance
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_instance_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_instance_deployment)
         """
 
     def cancel_service_pipeline_deployment(
         self, *, serviceName: str
-    ) -> CancelServicePipelineDeploymentOutputTypeDef:
+    ) -> CancelServicePipelineDeploymentOutputOutputTypeDef:
         """
         Attempts to cancel a service pipeline deployment on an  UpdateServicePipeline
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_pipeline_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_pipeline_deployment)
         """
@@ -284,15 +284,15 @@
         clientToken: str = ...,
         description: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateComponentOutputTypeDef:
+    ) -> CreateComponentOutputOutputTypeDef:
         """
         Create an Proton component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_component)
         """
 
@@ -307,15 +307,15 @@
         componentRoleArn: str = ...,
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMinorVersion: str = ...
-    ) -> CreateEnvironmentOutputTypeDef:
+    ) -> CreateEnvironmentOutputOutputTypeDef:
         """
         Deploy a new environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment)
         """
 
@@ -325,15 +325,15 @@
         environmentName: str,
         managementAccountId: str,
         clientToken: str = ...,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentAccountConnectionOutputTypeDef:
+    ) -> CreateEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         Create an environment account connection in an environment account so that
         environment infrastructure resources can be provisioned in the environment
         account from a management account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_account_connection)
@@ -344,15 +344,15 @@
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         provisioning: Literal["CUSTOMER_MANAGED"] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentTemplateOutputTypeDef:
+    ) -> CreateEnvironmentTemplateOutputOutputTypeDef:
         """
         Create an environment template for Proton.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template)
         """
 
@@ -361,15 +361,15 @@
         *,
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentTemplateVersionOutputTypeDef:
+    ) -> CreateEnvironmentTemplateVersionOutputOutputTypeDef:
         """
         Create a new major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template_version)
         """
 
@@ -377,15 +377,15 @@
         self,
         *,
         connectionArn: str,
         name: str,
         provider: RepositoryProviderType,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRepositoryOutputTypeDef:
+    ) -> CreateRepositoryOutputOutputTypeDef:
         """
         Create and register a link to a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_repository)
         """
 
@@ -398,15 +398,15 @@
         templateName: str,
         branchName: str = ...,
         description: str = ...,
         repositoryConnectionArn: str = ...,
         repositoryId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMinorVersion: str = ...
-    ) -> CreateServiceOutputTypeDef:
+    ) -> CreateServiceOutputOutputTypeDef:
         """
         Create an Proton service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service)
         """
 
@@ -416,15 +416,15 @@
         name: str,
         serviceName: str,
         spec: str,
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> CreateServiceInstanceOutputTypeDef:
+    ) -> CreateServiceInstanceOutputOutputTypeDef:
         """
         Create a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_instance)
         """
 
@@ -432,15 +432,15 @@
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         serviceName: str
-    ) -> CreateServiceSyncConfigOutputTypeDef:
+    ) -> CreateServiceSyncConfigOutputOutputTypeDef:
         """
         Create the Proton Ops configuration file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_sync_config)
         """
 
@@ -449,15 +449,15 @@
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         pipelineProvisioning: Literal["CUSTOMER_MANAGED"] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateServiceTemplateOutputTypeDef:
+    ) -> CreateServiceTemplateOutputOutputTypeDef:
         """
         Create a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template)
         """
 
@@ -468,15 +468,15 @@
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
         supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateServiceTemplateVersionOutputTypeDef:
+    ) -> CreateServiceTemplateVersionOutputOutputTypeDef:
         """
         Create a new major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template_version)
         """
 
@@ -485,128 +485,130 @@
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
         subdirectory: str = ...
-    ) -> CreateTemplateSyncConfigOutputTypeDef:
+    ) -> CreateTemplateSyncConfigOutputOutputTypeDef:
         """
         Set up a template to create new template versions automatically by tracking a
         linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_template_sync_config)
         """
 
-    def delete_component(self, *, name: str) -> DeleteComponentOutputTypeDef:
+    def delete_component(self, *, name: str) -> DeleteComponentOutputOutputTypeDef:
         """
         Delete an Proton component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_component)
         """
 
-    def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputTypeDef:
+    def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputOutputTypeDef:
         """
         Delete the deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_deployment)
         """
 
-    def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputTypeDef:
+    def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputOutputTypeDef:
         """
         Delete an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment)
         """
 
     def delete_environment_account_connection(
         self, *, id: str
-    ) -> DeleteEnvironmentAccountConnectionOutputTypeDef:
+    ) -> DeleteEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         In an environment account, delete an environment account connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_account_connection)
         """
 
-    def delete_environment_template(self, *, name: str) -> DeleteEnvironmentTemplateOutputTypeDef:
+    def delete_environment_template(
+        self, *, name: str
+    ) -> DeleteEnvironmentTemplateOutputOutputTypeDef:
         """
         If no other major or minor versions of an environment template exist, delete the
         environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template)
         """
 
     def delete_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> DeleteEnvironmentTemplateVersionOutputTypeDef:
+    ) -> DeleteEnvironmentTemplateVersionOutputOutputTypeDef:
         """
         If no other minor versions of an environment template exist, delete a major
         version of the environment template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template_version)
         """
 
     def delete_repository(
         self, *, name: str, provider: RepositoryProviderType
-    ) -> DeleteRepositoryOutputTypeDef:
+    ) -> DeleteRepositoryOutputOutputTypeDef:
         """
         De-register and unlink your repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_repository)
         """
 
-    def delete_service(self, *, name: str) -> DeleteServiceOutputTypeDef:
+    def delete_service(self, *, name: str) -> DeleteServiceOutputOutputTypeDef:
         """
         Delete a service, with its instances and pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service)
         """
 
     def delete_service_sync_config(
         self, *, serviceName: str
-    ) -> DeleteServiceSyncConfigOutputTypeDef:
+    ) -> DeleteServiceSyncConfigOutputOutputTypeDef:
         """
         Delete the Proton Ops file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_sync_config)
         """
 
-    def delete_service_template(self, *, name: str) -> DeleteServiceTemplateOutputTypeDef:
+    def delete_service_template(self, *, name: str) -> DeleteServiceTemplateOutputOutputTypeDef:
         """
         If no other major or minor versions of the service template exist, delete the
         service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template)
         """
 
     def delete_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> DeleteServiceTemplateVersionOutputTypeDef:
+    ) -> DeleteServiceTemplateVersionOutputOutputTypeDef:
         """
         If no other minor versions of a service template exist, delete a major version
         of the service template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template_version)
         """
 
     def delete_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
-    ) -> DeleteTemplateSyncConfigOutputTypeDef:
+    ) -> DeleteTemplateSyncConfigOutputOutputTypeDef:
         """
         Delete a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_template_sync_config)
         """
 
@@ -620,23 +622,23 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#generate_presigned_url)
         """
 
-    def get_account_settings(self) -> GetAccountSettingsOutputTypeDef:
+    def get_account_settings(self) -> GetAccountSettingsOutputOutputTypeDef:
         """
         Get detail data for Proton account-wide settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_account_settings)
         """
 
-    def get_component(self, *, name: str) -> GetComponentOutputTypeDef:
+    def get_component(self, *, name: str) -> GetComponentOutputOutputTypeDef:
         """
         Get detailed data for a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_component)
         """
 
@@ -644,189 +646,191 @@
         self,
         *,
         id: str,
         componentName: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> GetDeploymentOutputTypeDef:
+    ) -> GetDeploymentOutputOutputTypeDef:
         """
         Get detailed data for a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_deployment)
         """
 
-    def get_environment(self, *, name: str) -> GetEnvironmentOutputTypeDef:
+    def get_environment(self, *, name: str) -> GetEnvironmentOutputOutputTypeDef:
         """
         Get detailed data for an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment)
         """
 
     def get_environment_account_connection(
         self, *, id: str
-    ) -> GetEnvironmentAccountConnectionOutputTypeDef:
+    ) -> GetEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         In an environment account, get the detailed data for an environment account
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_account_connection)
         """
 
-    def get_environment_template(self, *, name: str) -> GetEnvironmentTemplateOutputTypeDef:
+    def get_environment_template(self, *, name: str) -> GetEnvironmentTemplateOutputOutputTypeDef:
         """
         Get detailed data for an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template)
         """
 
     def get_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> GetEnvironmentTemplateVersionOutputTypeDef:
+    ) -> GetEnvironmentTemplateVersionOutputOutputTypeDef:
         """
         Get detailed data for a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template_version)
         """
 
     def get_repository(
         self, *, name: str, provider: RepositoryProviderType
-    ) -> GetRepositoryOutputTypeDef:
+    ) -> GetRepositoryOutputOutputTypeDef:
         """
         Get detail data for a linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository)
         """
 
     def get_repository_sync_status(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType
-    ) -> GetRepositorySyncStatusOutputTypeDef:
+    ) -> GetRepositorySyncStatusOutputOutputTypeDef:
         """
         Get the sync status of a repository used for Proton template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository_sync_status)
         """
 
-    def get_resources_summary(self) -> GetResourcesSummaryOutputTypeDef:
+    def get_resources_summary(self) -> GetResourcesSummaryOutputOutputTypeDef:
         """
         Get counts of Proton resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_resources_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_resources_summary)
         """
 
-    def get_service(self, *, name: str) -> GetServiceOutputTypeDef:
+    def get_service(self, *, name: str) -> GetServiceOutputOutputTypeDef:
         """
         Get detailed data for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service)
         """
 
     def get_service_instance(
         self, *, name: str, serviceName: str
-    ) -> GetServiceInstanceOutputTypeDef:
+    ) -> GetServiceInstanceOutputOutputTypeDef:
         """
         Get detailed data for a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance)
         """
 
     def get_service_instance_sync_status(
         self, *, serviceInstanceName: str, serviceName: str
-    ) -> GetServiceInstanceSyncStatusOutputTypeDef:
+    ) -> GetServiceInstanceSyncStatusOutputOutputTypeDef:
         """
         Get the status of the synced service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance_sync_status)
         """
 
     def get_service_sync_blocker_summary(
         self, *, serviceName: str, serviceInstanceName: str = ...
-    ) -> GetServiceSyncBlockerSummaryOutputTypeDef:
+    ) -> GetServiceSyncBlockerSummaryOutputOutputTypeDef:
         """
         Get detailed data for the service sync blocker summary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_blocker_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_blocker_summary)
         """
 
-    def get_service_sync_config(self, *, serviceName: str) -> GetServiceSyncConfigOutputTypeDef:
+    def get_service_sync_config(
+        self, *, serviceName: str
+    ) -> GetServiceSyncConfigOutputOutputTypeDef:
         """
         Get detailed information for the service sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_config)
         """
 
-    def get_service_template(self, *, name: str) -> GetServiceTemplateOutputTypeDef:
+    def get_service_template(self, *, name: str) -> GetServiceTemplateOutputOutputTypeDef:
         """
         Get detailed data for a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template)
         """
 
     def get_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> GetServiceTemplateVersionOutputTypeDef:
+    ) -> GetServiceTemplateVersionOutputOutputTypeDef:
         """
         Get detailed data for a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template_version)
         """
 
     def get_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
-    ) -> GetTemplateSyncConfigOutputTypeDef:
+    ) -> GetTemplateSyncConfigOutputOutputTypeDef:
         """
         Get detail data for a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_config)
         """
 
     def get_template_sync_status(
         self, *, templateName: str, templateType: TemplateTypeType, templateVersion: str
-    ) -> GetTemplateSyncStatusOutputTypeDef:
+    ) -> GetTemplateSyncStatusOutputOutputTypeDef:
         """
         Get the status of a template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_status)
         """
 
     def list_component_outputs(
         self, *, componentName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListComponentOutputsOutputTypeDef:
+    ) -> ListComponentOutputsOutputOutputTypeDef:
         """
         Get a list of component Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_outputs)
         """
 
     def list_component_provisioned_resources(
         self, *, componentName: str, nextToken: str = ...
-    ) -> ListComponentProvisionedResourcesOutputTypeDef:
+    ) -> ListComponentProvisionedResourcesOutputOutputTypeDef:
         """
         List provisioned resources for a component with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_provisioned_resources)
         """
 
@@ -834,15 +838,15 @@
         self,
         *,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> ListComponentsOutputTypeDef:
+    ) -> ListComponentsOutputOutputTypeDef:
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_components)
         """
 
@@ -851,15 +855,15 @@
         *,
         componentName: str = ...,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> ListDeploymentsOutputTypeDef:
+    ) -> ListDeploymentsOutputOutputTypeDef:
         """
         List deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_deployments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_deployments)
         """
 
@@ -867,124 +871,124 @@
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...
-    ) -> ListEnvironmentAccountConnectionsOutputTypeDef:
+    ) -> ListEnvironmentAccountConnectionsOutputOutputTypeDef:
         """
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_account_connections)
         """
 
     def list_environment_outputs(
         self, *, environmentName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListEnvironmentOutputsOutputTypeDef:
+    ) -> ListEnvironmentOutputsOutputOutputTypeDef:
         """
         List the infrastructure as code outputs for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_outputs)
         """
 
     def list_environment_provisioned_resources(
         self, *, environmentName: str, nextToken: str = ...
-    ) -> ListEnvironmentProvisionedResourcesOutputTypeDef:
+    ) -> ListEnvironmentProvisionedResourcesOutputOutputTypeDef:
         """
         List the provisioned resources for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_provisioned_resources)
         """
 
     def list_environment_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListEnvironmentTemplateVersionsOutputTypeDef:
+    ) -> ListEnvironmentTemplateVersionsOutputOutputTypeDef:
         """
         List major or minor versions of an environment template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_template_versions)
         """
 
     def list_environment_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListEnvironmentTemplatesOutputTypeDef:
+    ) -> ListEnvironmentTemplatesOutputOutputTypeDef:
         """
         List environment templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_templates)
         """
 
     def list_environments(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListEnvironmentsOutputTypeDef:
+    ) -> ListEnvironmentsOutputOutputTypeDef:
         """
         List environments with detail data summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environments)
         """
 
     def list_repositories(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListRepositoriesOutputTypeDef:
+    ) -> ListRepositoriesOutputOutputTypeDef:
         """
         List linked repositories with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repositories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repositories)
         """
 
     def list_repository_sync_definitions(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType,
         nextToken: str = ...
-    ) -> ListRepositorySyncDefinitionsOutputTypeDef:
+    ) -> ListRepositorySyncDefinitionsOutputOutputTypeDef:
         """
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repository_sync_definitions)
         """
 
     def list_service_instance_outputs(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         deploymentId: str = ...,
         nextToken: str = ...
-    ) -> ListServiceInstanceOutputsOutputTypeDef:
+    ) -> ListServiceInstanceOutputsOutputOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_outputs)
         """
 
     def list_service_instance_provisioned_resources(
         self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
-    ) -> ListServiceInstanceProvisionedResourcesOutputTypeDef:
+    ) -> ListServiceInstanceProvisionedResourcesOutputOutputTypeDef:
         """
         List provisioned resources for a service instance with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_provisioned_resources)
         """
 
@@ -993,80 +997,80 @@
         *,
         filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceName: str = ...,
         sortBy: ListServiceInstancesSortByType = ...,
         sortOrder: SortOrderType = ...
-    ) -> ListServiceInstancesOutputTypeDef:
+    ) -> ListServiceInstancesOutputOutputTypeDef:
         """
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instances)
         """
 
     def list_service_pipeline_outputs(
         self, *, serviceName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListServicePipelineOutputsOutputTypeDef:
+    ) -> ListServicePipelineOutputsOutputOutputTypeDef:
         """
         Get a list of service pipeline Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_outputs)
         """
 
     def list_service_pipeline_provisioned_resources(
         self, *, serviceName: str, nextToken: str = ...
-    ) -> ListServicePipelineProvisionedResourcesOutputTypeDef:
+    ) -> ListServicePipelineProvisionedResourcesOutputOutputTypeDef:
         """
         List provisioned resources for a service and pipeline with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_provisioned_resources)
         """
 
     def list_service_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListServiceTemplateVersionsOutputTypeDef:
+    ) -> ListServiceTemplateVersionsOutputOutputTypeDef:
         """
         List major or minor versions of a service template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_template_versions)
         """
 
     def list_service_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListServiceTemplatesOutputTypeDef:
+    ) -> ListServiceTemplatesOutputOutputTypeDef:
         """
         List service templates with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_templates)
         """
 
     def list_services(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListServicesOutputTypeDef:
+    ) -> ListServicesOutputOutputTypeDef:
         """
         List services with summaries of detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_services)
         """
 
     def list_tags_for_resource(
         self, *, resourceArn: str, maxResults: int = ..., nextToken: str = ...
-    ) -> ListTagsForResourceOutputTypeDef:
+    ) -> ListTagsForResourceOutputOutputTypeDef:
         """
         List tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_tags_for_resource)
         """
 
@@ -1085,15 +1089,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.notify_resource_deployment_status_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#notify_resource_deployment_status_change)
         """
 
     def reject_environment_account_connection(
         self, *, id: str
-    ) -> RejectEnvironmentAccountConnectionOutputTypeDef:
+    ) -> RejectEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         In a management account, reject an environment account connection from another
         environment account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.reject_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#reject_environment_account_connection)
         """
@@ -1117,15 +1121,15 @@
     def update_account_settings(
         self,
         *,
         deletePipelineProvisioningRepository: bool = ...,
         pipelineCodebuildRoleArn: str = ...,
         pipelineProvisioningRepository: RepositoryBranchInputTypeDef = ...,
         pipelineServiceRoleArn: str = ...
-    ) -> UpdateAccountSettingsOutputTypeDef:
+    ) -> UpdateAccountSettingsOutputOutputTypeDef:
         """
         Update Proton settings that are used for multiple services in the Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_account_settings)
         """
@@ -1137,15 +1141,15 @@
         name: str,
         clientToken: str = ...,
         description: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         templateFile: str = ...
-    ) -> UpdateComponentOutputTypeDef:
+    ) -> UpdateComponentOutputOutputTypeDef:
         """
         Update a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_component)
         """
 
@@ -1159,41 +1163,41 @@
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateEnvironmentOutputTypeDef:
+    ) -> UpdateEnvironmentOutputOutputTypeDef:
         """
         Update an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment)
         """
 
     def update_environment_account_connection(
         self,
         *,
         id: str,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...
-    ) -> UpdateEnvironmentAccountConnectionOutputTypeDef:
+    ) -> UpdateEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         In an environment account, update an environment account connection to use a new
         IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_account_connection)
         """
 
     def update_environment_template(
         self, *, name: str, description: str = ..., displayName: str = ...
-    ) -> UpdateEnvironmentTemplateOutputTypeDef:
+    ) -> UpdateEnvironmentTemplateOutputOutputTypeDef:
         """
         Update an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template)
         """
 
@@ -1201,25 +1205,25 @@
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         description: str = ...,
         status: TemplateVersionStatusType = ...
-    ) -> UpdateEnvironmentTemplateVersionOutputTypeDef:
+    ) -> UpdateEnvironmentTemplateVersionOutputOutputTypeDef:
         """
         Update a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template_version)
         """
 
     def update_service(
         self, *, name: str, description: str = ..., spec: str = ...
-    ) -> UpdateServiceOutputTypeDef:
+    ) -> UpdateServiceOutputOutputTypeDef:
         """
         Edit a service description or use a spec to add and delete service instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service)
         """
 
@@ -1229,15 +1233,15 @@
         deploymentType: DeploymentUpdateTypeType,
         name: str,
         serviceName: str,
         clientToken: str = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateServiceInstanceOutputTypeDef:
+    ) -> UpdateServiceInstanceOutputOutputTypeDef:
         """
         Update a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_instance)
         """
 
@@ -1245,25 +1249,25 @@
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         serviceName: str,
         spec: str,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateServicePipelineOutputTypeDef:
+    ) -> UpdateServicePipelineOutputOutputTypeDef:
         """
         Update the service pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_pipeline)
         """
 
     def update_service_sync_blocker(
         self, *, id: str, resolvedReason: str
-    ) -> UpdateServiceSyncBlockerOutputTypeDef:
+    ) -> UpdateServiceSyncBlockerOutputOutputTypeDef:
         """
         Update the service sync blocker by resolving it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_blocker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_blocker)
         """
 
@@ -1271,25 +1275,25 @@
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         serviceName: str
-    ) -> UpdateServiceSyncConfigOutputTypeDef:
+    ) -> UpdateServiceSyncConfigOutputOutputTypeDef:
         """
         Update the Proton Ops config file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_config)
         """
 
     def update_service_template(
         self, *, name: str, description: str = ..., displayName: str = ...
-    ) -> UpdateServiceTemplateOutputTypeDef:
+    ) -> UpdateServiceTemplateOutputOutputTypeDef:
         """
         Update a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template)
         """
 
@@ -1299,15 +1303,15 @@
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef] = ...,
         description: str = ...,
         status: TemplateVersionStatusType = ...,
         supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...
-    ) -> UpdateServiceTemplateVersionOutputTypeDef:
+    ) -> UpdateServiceTemplateVersionOutputOutputTypeDef:
         """
         Update a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template_version)
         """
 
@@ -1316,15 +1320,15 @@
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
         subdirectory: str = ...
-    ) -> UpdateTemplateSyncConfigOutputTypeDef:
+    ) -> UpdateTemplateSyncConfigOutputOutputTypeDef:
         """
         Update template sync configuration parameters, except for the `templateName` and
         `templateType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_template_sync_config)
         """
```

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/client.pyi` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -51,105 +51,105 @@
     ListServicePipelineProvisionedResourcesPaginator,
     ListServicesPaginator,
     ListServiceTemplatesPaginator,
     ListServiceTemplateVersionsPaginator,
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
-    AcceptEnvironmentAccountConnectionOutputTypeDef,
-    CancelComponentDeploymentOutputTypeDef,
-    CancelEnvironmentDeploymentOutputTypeDef,
-    CancelServiceInstanceDeploymentOutputTypeDef,
-    CancelServicePipelineDeploymentOutputTypeDef,
+    AcceptEnvironmentAccountConnectionOutputOutputTypeDef,
+    CancelComponentDeploymentOutputOutputTypeDef,
+    CancelEnvironmentDeploymentOutputOutputTypeDef,
+    CancelServiceInstanceDeploymentOutputOutputTypeDef,
+    CancelServicePipelineDeploymentOutputOutputTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
-    CreateComponentOutputTypeDef,
-    CreateEnvironmentAccountConnectionOutputTypeDef,
-    CreateEnvironmentOutputTypeDef,
-    CreateEnvironmentTemplateOutputTypeDef,
-    CreateEnvironmentTemplateVersionOutputTypeDef,
-    CreateRepositoryOutputTypeDef,
-    CreateServiceInstanceOutputTypeDef,
-    CreateServiceOutputTypeDef,
-    CreateServiceSyncConfigOutputTypeDef,
-    CreateServiceTemplateOutputTypeDef,
-    CreateServiceTemplateVersionOutputTypeDef,
-    CreateTemplateSyncConfigOutputTypeDef,
-    DeleteComponentOutputTypeDef,
-    DeleteDeploymentOutputTypeDef,
-    DeleteEnvironmentAccountConnectionOutputTypeDef,
-    DeleteEnvironmentOutputTypeDef,
-    DeleteEnvironmentTemplateOutputTypeDef,
-    DeleteEnvironmentTemplateVersionOutputTypeDef,
-    DeleteRepositoryOutputTypeDef,
-    DeleteServiceOutputTypeDef,
-    DeleteServiceSyncConfigOutputTypeDef,
-    DeleteServiceTemplateOutputTypeDef,
-    DeleteServiceTemplateVersionOutputTypeDef,
-    DeleteTemplateSyncConfigOutputTypeDef,
+    CreateComponentOutputOutputTypeDef,
+    CreateEnvironmentAccountConnectionOutputOutputTypeDef,
+    CreateEnvironmentOutputOutputTypeDef,
+    CreateEnvironmentTemplateOutputOutputTypeDef,
+    CreateEnvironmentTemplateVersionOutputOutputTypeDef,
+    CreateRepositoryOutputOutputTypeDef,
+    CreateServiceInstanceOutputOutputTypeDef,
+    CreateServiceOutputOutputTypeDef,
+    CreateServiceSyncConfigOutputOutputTypeDef,
+    CreateServiceTemplateOutputOutputTypeDef,
+    CreateServiceTemplateVersionOutputOutputTypeDef,
+    CreateTemplateSyncConfigOutputOutputTypeDef,
+    DeleteComponentOutputOutputTypeDef,
+    DeleteDeploymentOutputOutputTypeDef,
+    DeleteEnvironmentAccountConnectionOutputOutputTypeDef,
+    DeleteEnvironmentOutputOutputTypeDef,
+    DeleteEnvironmentTemplateOutputOutputTypeDef,
+    DeleteEnvironmentTemplateVersionOutputOutputTypeDef,
+    DeleteRepositoryOutputOutputTypeDef,
+    DeleteServiceOutputOutputTypeDef,
+    DeleteServiceSyncConfigOutputOutputTypeDef,
+    DeleteServiceTemplateOutputOutputTypeDef,
+    DeleteServiceTemplateVersionOutputOutputTypeDef,
+    DeleteTemplateSyncConfigOutputOutputTypeDef,
     EnvironmentTemplateFilterTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    GetComponentOutputTypeDef,
-    GetDeploymentOutputTypeDef,
-    GetEnvironmentAccountConnectionOutputTypeDef,
-    GetEnvironmentOutputTypeDef,
-    GetEnvironmentTemplateOutputTypeDef,
-    GetEnvironmentTemplateVersionOutputTypeDef,
-    GetRepositoryOutputTypeDef,
-    GetRepositorySyncStatusOutputTypeDef,
-    GetResourcesSummaryOutputTypeDef,
-    GetServiceInstanceOutputTypeDef,
-    GetServiceInstanceSyncStatusOutputTypeDef,
-    GetServiceOutputTypeDef,
-    GetServiceSyncBlockerSummaryOutputTypeDef,
-    GetServiceSyncConfigOutputTypeDef,
-    GetServiceTemplateOutputTypeDef,
-    GetServiceTemplateVersionOutputTypeDef,
-    GetTemplateSyncConfigOutputTypeDef,
-    GetTemplateSyncStatusOutputTypeDef,
-    ListComponentOutputsOutputTypeDef,
-    ListComponentProvisionedResourcesOutputTypeDef,
-    ListComponentsOutputTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListEnvironmentAccountConnectionsOutputTypeDef,
-    ListEnvironmentOutputsOutputTypeDef,
-    ListEnvironmentProvisionedResourcesOutputTypeDef,
-    ListEnvironmentsOutputTypeDef,
-    ListEnvironmentTemplatesOutputTypeDef,
-    ListEnvironmentTemplateVersionsOutputTypeDef,
-    ListRepositoriesOutputTypeDef,
-    ListRepositorySyncDefinitionsOutputTypeDef,
-    ListServiceInstanceOutputsOutputTypeDef,
-    ListServiceInstanceProvisionedResourcesOutputTypeDef,
+    GetAccountSettingsOutputOutputTypeDef,
+    GetComponentOutputOutputTypeDef,
+    GetDeploymentOutputOutputTypeDef,
+    GetEnvironmentAccountConnectionOutputOutputTypeDef,
+    GetEnvironmentOutputOutputTypeDef,
+    GetEnvironmentTemplateOutputOutputTypeDef,
+    GetEnvironmentTemplateVersionOutputOutputTypeDef,
+    GetRepositoryOutputOutputTypeDef,
+    GetRepositorySyncStatusOutputOutputTypeDef,
+    GetResourcesSummaryOutputOutputTypeDef,
+    GetServiceInstanceOutputOutputTypeDef,
+    GetServiceInstanceSyncStatusOutputOutputTypeDef,
+    GetServiceOutputOutputTypeDef,
+    GetServiceSyncBlockerSummaryOutputOutputTypeDef,
+    GetServiceSyncConfigOutputOutputTypeDef,
+    GetServiceTemplateOutputOutputTypeDef,
+    GetServiceTemplateVersionOutputOutputTypeDef,
+    GetTemplateSyncConfigOutputOutputTypeDef,
+    GetTemplateSyncStatusOutputOutputTypeDef,
+    ListComponentOutputsOutputOutputTypeDef,
+    ListComponentProvisionedResourcesOutputOutputTypeDef,
+    ListComponentsOutputOutputTypeDef,
+    ListDeploymentsOutputOutputTypeDef,
+    ListEnvironmentAccountConnectionsOutputOutputTypeDef,
+    ListEnvironmentOutputsOutputOutputTypeDef,
+    ListEnvironmentProvisionedResourcesOutputOutputTypeDef,
+    ListEnvironmentsOutputOutputTypeDef,
+    ListEnvironmentTemplatesOutputOutputTypeDef,
+    ListEnvironmentTemplateVersionsOutputOutputTypeDef,
+    ListRepositoriesOutputOutputTypeDef,
+    ListRepositorySyncDefinitionsOutputOutputTypeDef,
+    ListServiceInstanceOutputsOutputOutputTypeDef,
+    ListServiceInstanceProvisionedResourcesOutputOutputTypeDef,
     ListServiceInstancesFilterTypeDef,
-    ListServiceInstancesOutputTypeDef,
-    ListServicePipelineOutputsOutputTypeDef,
-    ListServicePipelineProvisionedResourcesOutputTypeDef,
-    ListServicesOutputTypeDef,
-    ListServiceTemplatesOutputTypeDef,
-    ListServiceTemplateVersionsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
+    ListServiceInstancesOutputOutputTypeDef,
+    ListServicePipelineOutputsOutputOutputTypeDef,
+    ListServicePipelineProvisionedResourcesOutputOutputTypeDef,
+    ListServicesOutputOutputTypeDef,
+    ListServiceTemplatesOutputOutputTypeDef,
+    ListServiceTemplateVersionsOutputOutputTypeDef,
+    ListTagsForResourceOutputOutputTypeDef,
     OutputTypeDef,
-    RejectEnvironmentAccountConnectionOutputTypeDef,
+    RejectEnvironmentAccountConnectionOutputOutputTypeDef,
     RepositoryBranchInputTypeDef,
     TagTypeDef,
     TemplateVersionSourceInputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
-    UpdateComponentOutputTypeDef,
-    UpdateEnvironmentAccountConnectionOutputTypeDef,
-    UpdateEnvironmentOutputTypeDef,
-    UpdateEnvironmentTemplateOutputTypeDef,
-    UpdateEnvironmentTemplateVersionOutputTypeDef,
-    UpdateServiceInstanceOutputTypeDef,
-    UpdateServiceOutputTypeDef,
-    UpdateServicePipelineOutputTypeDef,
-    UpdateServiceSyncBlockerOutputTypeDef,
-    UpdateServiceSyncConfigOutputTypeDef,
-    UpdateServiceTemplateOutputTypeDef,
-    UpdateServiceTemplateVersionOutputTypeDef,
-    UpdateTemplateSyncConfigOutputTypeDef,
+    UpdateAccountSettingsOutputOutputTypeDef,
+    UpdateComponentOutputOutputTypeDef,
+    UpdateEnvironmentAccountConnectionOutputOutputTypeDef,
+    UpdateEnvironmentOutputOutputTypeDef,
+    UpdateEnvironmentTemplateOutputOutputTypeDef,
+    UpdateEnvironmentTemplateVersionOutputOutputTypeDef,
+    UpdateServiceInstanceOutputOutputTypeDef,
+    UpdateServiceOutputOutputTypeDef,
+    UpdateServicePipelineOutputOutputTypeDef,
+    UpdateServiceSyncBlockerOutputOutputTypeDef,
+    UpdateServiceSyncConfigOutputOutputTypeDef,
+    UpdateServiceTemplateOutputOutputTypeDef,
+    UpdateServiceTemplateVersionOutputOutputTypeDef,
+    UpdateTemplateSyncConfigOutputOutputTypeDef,
 )
 from .waiter import (
     ComponentDeletedWaiter,
     ComponentDeployedWaiter,
     EnvironmentDeployedWaiter,
     EnvironmentTemplateVersionRegisteredWaiter,
     ServiceCreatedWaiter,
@@ -198,15 +198,15 @@
         ProtonClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#exceptions)
         """
     def accept_environment_account_connection(
         self, *, id: str
-    ) -> AcceptEnvironmentAccountConnectionOutputTypeDef:
+    ) -> AcceptEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         In a management account, an environment account connection request is accepted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.accept_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#accept_environment_account_connection)
         """
     def can_paginate(self, operation_name: str) -> bool:
@@ -214,45 +214,45 @@
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#can_paginate)
         """
     def cancel_component_deployment(
         self, *, componentName: str
-    ) -> CancelComponentDeploymentOutputTypeDef:
+    ) -> CancelComponentDeploymentOutputOutputTypeDef:
         """
         Attempts to cancel a component deployment (for a component that is in the
         `IN_PROGRESS` deployment status).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_component_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_component_deployment)
         """
     def cancel_environment_deployment(
         self, *, environmentName: str
-    ) -> CancelEnvironmentDeploymentOutputTypeDef:
+    ) -> CancelEnvironmentDeploymentOutputOutputTypeDef:
         """
         Attempts to cancel an environment deployment on an  UpdateEnvironment action, if
         the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_environment_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_environment_deployment)
         """
     def cancel_service_instance_deployment(
         self, *, serviceInstanceName: str, serviceName: str
-    ) -> CancelServiceInstanceDeploymentOutputTypeDef:
+    ) -> CancelServiceInstanceDeploymentOutputOutputTypeDef:
         """
         Attempts to cancel a service instance deployment on an  UpdateServiceInstance
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_instance_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_instance_deployment)
         """
     def cancel_service_pipeline_deployment(
         self, *, serviceName: str
-    ) -> CancelServicePipelineDeploymentOutputTypeDef:
+    ) -> CancelServicePipelineDeploymentOutputOutputTypeDef:
         """
         Attempts to cancel a service pipeline deployment on an  UpdateServicePipeline
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_pipeline_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_pipeline_deployment)
         """
@@ -272,15 +272,15 @@
         clientToken: str = ...,
         description: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateComponentOutputTypeDef:
+    ) -> CreateComponentOutputOutputTypeDef:
         """
         Create an Proton component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_component)
         """
     def create_environment(
@@ -294,15 +294,15 @@
         componentRoleArn: str = ...,
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMinorVersion: str = ...
-    ) -> CreateEnvironmentOutputTypeDef:
+    ) -> CreateEnvironmentOutputOutputTypeDef:
         """
         Deploy a new environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment)
         """
     def create_environment_account_connection(
@@ -311,15 +311,15 @@
         environmentName: str,
         managementAccountId: str,
         clientToken: str = ...,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentAccountConnectionOutputTypeDef:
+    ) -> CreateEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         Create an environment account connection in an environment account so that
         environment infrastructure resources can be provisioned in the environment
         account from a management account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_account_connection)
@@ -329,15 +329,15 @@
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         provisioning: Literal["CUSTOMER_MANAGED"] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentTemplateOutputTypeDef:
+    ) -> CreateEnvironmentTemplateOutputOutputTypeDef:
         """
         Create an environment template for Proton.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template)
         """
     def create_environment_template_version(
@@ -345,30 +345,30 @@
         *,
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentTemplateVersionOutputTypeDef:
+    ) -> CreateEnvironmentTemplateVersionOutputOutputTypeDef:
         """
         Create a new major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template_version)
         """
     def create_repository(
         self,
         *,
         connectionArn: str,
         name: str,
         provider: RepositoryProviderType,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRepositoryOutputTypeDef:
+    ) -> CreateRepositoryOutputOutputTypeDef:
         """
         Create and register a link to a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_repository)
         """
     def create_service(
@@ -380,15 +380,15 @@
         templateName: str,
         branchName: str = ...,
         description: str = ...,
         repositoryConnectionArn: str = ...,
         repositoryId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMinorVersion: str = ...
-    ) -> CreateServiceOutputTypeDef:
+    ) -> CreateServiceOutputOutputTypeDef:
         """
         Create an Proton service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service)
         """
     def create_service_instance(
@@ -397,30 +397,30 @@
         name: str,
         serviceName: str,
         spec: str,
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> CreateServiceInstanceOutputTypeDef:
+    ) -> CreateServiceInstanceOutputOutputTypeDef:
         """
         Create a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_instance)
         """
     def create_service_sync_config(
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         serviceName: str
-    ) -> CreateServiceSyncConfigOutputTypeDef:
+    ) -> CreateServiceSyncConfigOutputOutputTypeDef:
         """
         Create the Proton Ops configuration file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_sync_config)
         """
     def create_service_template(
@@ -428,15 +428,15 @@
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         pipelineProvisioning: Literal["CUSTOMER_MANAGED"] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateServiceTemplateOutputTypeDef:
+    ) -> CreateServiceTemplateOutputOutputTypeDef:
         """
         Create a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template)
         """
     def create_service_template_version(
@@ -446,15 +446,15 @@
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
         supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateServiceTemplateVersionOutputTypeDef:
+    ) -> CreateServiceTemplateVersionOutputOutputTypeDef:
         """
         Create a new major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template_version)
         """
     def create_template_sync_config(
@@ -462,116 +462,118 @@
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
         subdirectory: str = ...
-    ) -> CreateTemplateSyncConfigOutputTypeDef:
+    ) -> CreateTemplateSyncConfigOutputOutputTypeDef:
         """
         Set up a template to create new template versions automatically by tracking a
         linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_template_sync_config)
         """
-    def delete_component(self, *, name: str) -> DeleteComponentOutputTypeDef:
+    def delete_component(self, *, name: str) -> DeleteComponentOutputOutputTypeDef:
         """
         Delete an Proton component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_component)
         """
-    def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputTypeDef:
+    def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputOutputTypeDef:
         """
         Delete the deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_deployment)
         """
-    def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputTypeDef:
+    def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputOutputTypeDef:
         """
         Delete an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment)
         """
     def delete_environment_account_connection(
         self, *, id: str
-    ) -> DeleteEnvironmentAccountConnectionOutputTypeDef:
+    ) -> DeleteEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         In an environment account, delete an environment account connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_account_connection)
         """
-    def delete_environment_template(self, *, name: str) -> DeleteEnvironmentTemplateOutputTypeDef:
+    def delete_environment_template(
+        self, *, name: str
+    ) -> DeleteEnvironmentTemplateOutputOutputTypeDef:
         """
         If no other major or minor versions of an environment template exist, delete the
         environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template)
         """
     def delete_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> DeleteEnvironmentTemplateVersionOutputTypeDef:
+    ) -> DeleteEnvironmentTemplateVersionOutputOutputTypeDef:
         """
         If no other minor versions of an environment template exist, delete a major
         version of the environment template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template_version)
         """
     def delete_repository(
         self, *, name: str, provider: RepositoryProviderType
-    ) -> DeleteRepositoryOutputTypeDef:
+    ) -> DeleteRepositoryOutputOutputTypeDef:
         """
         De-register and unlink your repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_repository)
         """
-    def delete_service(self, *, name: str) -> DeleteServiceOutputTypeDef:
+    def delete_service(self, *, name: str) -> DeleteServiceOutputOutputTypeDef:
         """
         Delete a service, with its instances and pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service)
         """
     def delete_service_sync_config(
         self, *, serviceName: str
-    ) -> DeleteServiceSyncConfigOutputTypeDef:
+    ) -> DeleteServiceSyncConfigOutputOutputTypeDef:
         """
         Delete the Proton Ops file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_sync_config)
         """
-    def delete_service_template(self, *, name: str) -> DeleteServiceTemplateOutputTypeDef:
+    def delete_service_template(self, *, name: str) -> DeleteServiceTemplateOutputOutputTypeDef:
         """
         If no other major or minor versions of the service template exist, delete the
         service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template)
         """
     def delete_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> DeleteServiceTemplateVersionOutputTypeDef:
+    ) -> DeleteServiceTemplateVersionOutputOutputTypeDef:
         """
         If no other minor versions of a service template exist, delete a major version
         of the service template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template_version)
         """
     def delete_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
-    ) -> DeleteTemplateSyncConfigOutputTypeDef:
+    ) -> DeleteTemplateSyncConfigOutputOutputTypeDef:
         """
         Delete a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_template_sync_config)
         """
     def generate_presigned_url(
@@ -583,208 +585,210 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#generate_presigned_url)
         """
-    def get_account_settings(self) -> GetAccountSettingsOutputTypeDef:
+    def get_account_settings(self) -> GetAccountSettingsOutputOutputTypeDef:
         """
         Get detail data for Proton account-wide settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_account_settings)
         """
-    def get_component(self, *, name: str) -> GetComponentOutputTypeDef:
+    def get_component(self, *, name: str) -> GetComponentOutputOutputTypeDef:
         """
         Get detailed data for a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_component)
         """
     def get_deployment(
         self,
         *,
         id: str,
         componentName: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> GetDeploymentOutputTypeDef:
+    ) -> GetDeploymentOutputOutputTypeDef:
         """
         Get detailed data for a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_deployment)
         """
-    def get_environment(self, *, name: str) -> GetEnvironmentOutputTypeDef:
+    def get_environment(self, *, name: str) -> GetEnvironmentOutputOutputTypeDef:
         """
         Get detailed data for an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment)
         """
     def get_environment_account_connection(
         self, *, id: str
-    ) -> GetEnvironmentAccountConnectionOutputTypeDef:
+    ) -> GetEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         In an environment account, get the detailed data for an environment account
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_account_connection)
         """
-    def get_environment_template(self, *, name: str) -> GetEnvironmentTemplateOutputTypeDef:
+    def get_environment_template(self, *, name: str) -> GetEnvironmentTemplateOutputOutputTypeDef:
         """
         Get detailed data for an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template)
         """
     def get_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> GetEnvironmentTemplateVersionOutputTypeDef:
+    ) -> GetEnvironmentTemplateVersionOutputOutputTypeDef:
         """
         Get detailed data for a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template_version)
         """
     def get_repository(
         self, *, name: str, provider: RepositoryProviderType
-    ) -> GetRepositoryOutputTypeDef:
+    ) -> GetRepositoryOutputOutputTypeDef:
         """
         Get detail data for a linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository)
         """
     def get_repository_sync_status(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType
-    ) -> GetRepositorySyncStatusOutputTypeDef:
+    ) -> GetRepositorySyncStatusOutputOutputTypeDef:
         """
         Get the sync status of a repository used for Proton template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository_sync_status)
         """
-    def get_resources_summary(self) -> GetResourcesSummaryOutputTypeDef:
+    def get_resources_summary(self) -> GetResourcesSummaryOutputOutputTypeDef:
         """
         Get counts of Proton resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_resources_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_resources_summary)
         """
-    def get_service(self, *, name: str) -> GetServiceOutputTypeDef:
+    def get_service(self, *, name: str) -> GetServiceOutputOutputTypeDef:
         """
         Get detailed data for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service)
         """
     def get_service_instance(
         self, *, name: str, serviceName: str
-    ) -> GetServiceInstanceOutputTypeDef:
+    ) -> GetServiceInstanceOutputOutputTypeDef:
         """
         Get detailed data for a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance)
         """
     def get_service_instance_sync_status(
         self, *, serviceInstanceName: str, serviceName: str
-    ) -> GetServiceInstanceSyncStatusOutputTypeDef:
+    ) -> GetServiceInstanceSyncStatusOutputOutputTypeDef:
         """
         Get the status of the synced service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance_sync_status)
         """
     def get_service_sync_blocker_summary(
         self, *, serviceName: str, serviceInstanceName: str = ...
-    ) -> GetServiceSyncBlockerSummaryOutputTypeDef:
+    ) -> GetServiceSyncBlockerSummaryOutputOutputTypeDef:
         """
         Get detailed data for the service sync blocker summary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_blocker_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_blocker_summary)
         """
-    def get_service_sync_config(self, *, serviceName: str) -> GetServiceSyncConfigOutputTypeDef:
+    def get_service_sync_config(
+        self, *, serviceName: str
+    ) -> GetServiceSyncConfigOutputOutputTypeDef:
         """
         Get detailed information for the service sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_config)
         """
-    def get_service_template(self, *, name: str) -> GetServiceTemplateOutputTypeDef:
+    def get_service_template(self, *, name: str) -> GetServiceTemplateOutputOutputTypeDef:
         """
         Get detailed data for a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template)
         """
     def get_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> GetServiceTemplateVersionOutputTypeDef:
+    ) -> GetServiceTemplateVersionOutputOutputTypeDef:
         """
         Get detailed data for a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template_version)
         """
     def get_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
-    ) -> GetTemplateSyncConfigOutputTypeDef:
+    ) -> GetTemplateSyncConfigOutputOutputTypeDef:
         """
         Get detail data for a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_config)
         """
     def get_template_sync_status(
         self, *, templateName: str, templateType: TemplateTypeType, templateVersion: str
-    ) -> GetTemplateSyncStatusOutputTypeDef:
+    ) -> GetTemplateSyncStatusOutputOutputTypeDef:
         """
         Get the status of a template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_status)
         """
     def list_component_outputs(
         self, *, componentName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListComponentOutputsOutputTypeDef:
+    ) -> ListComponentOutputsOutputOutputTypeDef:
         """
         Get a list of component Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_outputs)
         """
     def list_component_provisioned_resources(
         self, *, componentName: str, nextToken: str = ...
-    ) -> ListComponentProvisionedResourcesOutputTypeDef:
+    ) -> ListComponentProvisionedResourcesOutputOutputTypeDef:
         """
         List provisioned resources for a component with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_provisioned_resources)
         """
     def list_components(
         self,
         *,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> ListComponentsOutputTypeDef:
+    ) -> ListComponentsOutputOutputTypeDef:
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_components)
         """
     def list_deployments(
@@ -792,130 +796,130 @@
         *,
         componentName: str = ...,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> ListDeploymentsOutputTypeDef:
+    ) -> ListDeploymentsOutputOutputTypeDef:
         """
         List deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_deployments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_deployments)
         """
     def list_environment_account_connections(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...
-    ) -> ListEnvironmentAccountConnectionsOutputTypeDef:
+    ) -> ListEnvironmentAccountConnectionsOutputOutputTypeDef:
         """
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_account_connections)
         """
     def list_environment_outputs(
         self, *, environmentName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListEnvironmentOutputsOutputTypeDef:
+    ) -> ListEnvironmentOutputsOutputOutputTypeDef:
         """
         List the infrastructure as code outputs for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_outputs)
         """
     def list_environment_provisioned_resources(
         self, *, environmentName: str, nextToken: str = ...
-    ) -> ListEnvironmentProvisionedResourcesOutputTypeDef:
+    ) -> ListEnvironmentProvisionedResourcesOutputOutputTypeDef:
         """
         List the provisioned resources for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_provisioned_resources)
         """
     def list_environment_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListEnvironmentTemplateVersionsOutputTypeDef:
+    ) -> ListEnvironmentTemplateVersionsOutputOutputTypeDef:
         """
         List major or minor versions of an environment template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_template_versions)
         """
     def list_environment_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListEnvironmentTemplatesOutputTypeDef:
+    ) -> ListEnvironmentTemplatesOutputOutputTypeDef:
         """
         List environment templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_templates)
         """
     def list_environments(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListEnvironmentsOutputTypeDef:
+    ) -> ListEnvironmentsOutputOutputTypeDef:
         """
         List environments with detail data summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environments)
         """
     def list_repositories(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListRepositoriesOutputTypeDef:
+    ) -> ListRepositoriesOutputOutputTypeDef:
         """
         List linked repositories with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repositories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repositories)
         """
     def list_repository_sync_definitions(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType,
         nextToken: str = ...
-    ) -> ListRepositorySyncDefinitionsOutputTypeDef:
+    ) -> ListRepositorySyncDefinitionsOutputOutputTypeDef:
         """
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repository_sync_definitions)
         """
     def list_service_instance_outputs(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         deploymentId: str = ...,
         nextToken: str = ...
-    ) -> ListServiceInstanceOutputsOutputTypeDef:
+    ) -> ListServiceInstanceOutputsOutputOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_outputs)
         """
     def list_service_instance_provisioned_resources(
         self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
-    ) -> ListServiceInstanceProvisionedResourcesOutputTypeDef:
+    ) -> ListServiceInstanceProvisionedResourcesOutputOutputTypeDef:
         """
         List provisioned resources for a service instance with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_provisioned_resources)
         """
     def list_service_instances(
@@ -923,74 +927,74 @@
         *,
         filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceName: str = ...,
         sortBy: ListServiceInstancesSortByType = ...,
         sortOrder: SortOrderType = ...
-    ) -> ListServiceInstancesOutputTypeDef:
+    ) -> ListServiceInstancesOutputOutputTypeDef:
         """
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instances)
         """
     def list_service_pipeline_outputs(
         self, *, serviceName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListServicePipelineOutputsOutputTypeDef:
+    ) -> ListServicePipelineOutputsOutputOutputTypeDef:
         """
         Get a list of service pipeline Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_outputs)
         """
     def list_service_pipeline_provisioned_resources(
         self, *, serviceName: str, nextToken: str = ...
-    ) -> ListServicePipelineProvisionedResourcesOutputTypeDef:
+    ) -> ListServicePipelineProvisionedResourcesOutputOutputTypeDef:
         """
         List provisioned resources for a service and pipeline with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_provisioned_resources)
         """
     def list_service_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListServiceTemplateVersionsOutputTypeDef:
+    ) -> ListServiceTemplateVersionsOutputOutputTypeDef:
         """
         List major or minor versions of a service template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_template_versions)
         """
     def list_service_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListServiceTemplatesOutputTypeDef:
+    ) -> ListServiceTemplatesOutputOutputTypeDef:
         """
         List service templates with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_templates)
         """
     def list_services(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListServicesOutputTypeDef:
+    ) -> ListServicesOutputOutputTypeDef:
         """
         List services with summaries of detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_services)
         """
     def list_tags_for_resource(
         self, *, resourceArn: str, maxResults: int = ..., nextToken: str = ...
-    ) -> ListTagsForResourceOutputTypeDef:
+    ) -> ListTagsForResourceOutputOutputTypeDef:
         """
         List tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_tags_for_resource)
         """
     def notify_resource_deployment_status_change(
@@ -1007,15 +1011,15 @@
         managed provisioning.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.notify_resource_deployment_status_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#notify_resource_deployment_status_change)
         """
     def reject_environment_account_connection(
         self, *, id: str
-    ) -> RejectEnvironmentAccountConnectionOutputTypeDef:
+    ) -> RejectEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         In a management account, reject an environment account connection from another
         environment account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.reject_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#reject_environment_account_connection)
         """
@@ -1036,15 +1040,15 @@
     def update_account_settings(
         self,
         *,
         deletePipelineProvisioningRepository: bool = ...,
         pipelineCodebuildRoleArn: str = ...,
         pipelineProvisioningRepository: RepositoryBranchInputTypeDef = ...,
         pipelineServiceRoleArn: str = ...
-    ) -> UpdateAccountSettingsOutputTypeDef:
+    ) -> UpdateAccountSettingsOutputOutputTypeDef:
         """
         Update Proton settings that are used for multiple services in the Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_account_settings)
         """
@@ -1055,15 +1059,15 @@
         name: str,
         clientToken: str = ...,
         description: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         templateFile: str = ...
-    ) -> UpdateComponentOutputTypeDef:
+    ) -> UpdateComponentOutputOutputTypeDef:
         """
         Update a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_component)
         """
     def update_environment(
@@ -1076,63 +1080,63 @@
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateEnvironmentOutputTypeDef:
+    ) -> UpdateEnvironmentOutputOutputTypeDef:
         """
         Update an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment)
         """
     def update_environment_account_connection(
         self,
         *,
         id: str,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...
-    ) -> UpdateEnvironmentAccountConnectionOutputTypeDef:
+    ) -> UpdateEnvironmentAccountConnectionOutputOutputTypeDef:
         """
         In an environment account, update an environment account connection to use a new
         IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_account_connection)
         """
     def update_environment_template(
         self, *, name: str, description: str = ..., displayName: str = ...
-    ) -> UpdateEnvironmentTemplateOutputTypeDef:
+    ) -> UpdateEnvironmentTemplateOutputOutputTypeDef:
         """
         Update an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template)
         """
     def update_environment_template_version(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         description: str = ...,
         status: TemplateVersionStatusType = ...
-    ) -> UpdateEnvironmentTemplateVersionOutputTypeDef:
+    ) -> UpdateEnvironmentTemplateVersionOutputOutputTypeDef:
         """
         Update a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template_version)
         """
     def update_service(
         self, *, name: str, description: str = ..., spec: str = ...
-    ) -> UpdateServiceOutputTypeDef:
+    ) -> UpdateServiceOutputOutputTypeDef:
         """
         Edit a service description or use a spec to add and delete service instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service)
         """
     def update_service_instance(
@@ -1141,63 +1145,63 @@
         deploymentType: DeploymentUpdateTypeType,
         name: str,
         serviceName: str,
         clientToken: str = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateServiceInstanceOutputTypeDef:
+    ) -> UpdateServiceInstanceOutputOutputTypeDef:
         """
         Update a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_instance)
         """
     def update_service_pipeline(
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         serviceName: str,
         spec: str,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateServicePipelineOutputTypeDef:
+    ) -> UpdateServicePipelineOutputOutputTypeDef:
         """
         Update the service pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_pipeline)
         """
     def update_service_sync_blocker(
         self, *, id: str, resolvedReason: str
-    ) -> UpdateServiceSyncBlockerOutputTypeDef:
+    ) -> UpdateServiceSyncBlockerOutputOutputTypeDef:
         """
         Update the service sync blocker by resolving it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_blocker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_blocker)
         """
     def update_service_sync_config(
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         serviceName: str
-    ) -> UpdateServiceSyncConfigOutputTypeDef:
+    ) -> UpdateServiceSyncConfigOutputOutputTypeDef:
         """
         Update the Proton Ops config file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_config)
         """
     def update_service_template(
         self, *, name: str, description: str = ..., displayName: str = ...
-    ) -> UpdateServiceTemplateOutputTypeDef:
+    ) -> UpdateServiceTemplateOutputOutputTypeDef:
         """
         Update a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template)
         """
     def update_service_template_version(
@@ -1206,15 +1210,15 @@
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef] = ...,
         description: str = ...,
         status: TemplateVersionStatusType = ...,
         supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...
-    ) -> UpdateServiceTemplateVersionOutputTypeDef:
+    ) -> UpdateServiceTemplateVersionOutputOutputTypeDef:
         """
         Update a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template_version)
         """
     def update_template_sync_config(
@@ -1222,15 +1226,15 @@
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
         subdirectory: str = ...
-    ) -> UpdateTemplateSyncConfigOutputTypeDef:
+    ) -> UpdateTemplateSyncConfigOutputOutputTypeDef:
         """
         Update template sync configuration parameters, except for the `templateName` and
         `templateType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_template_sync_config)
         """
```

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/literals.py` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/literals.pyi` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/paginator.py` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,36 +69,36 @@
     ListServiceInstancesSortByType,
     RepositoryProviderType,
     SortOrderType,
     SyncTypeType,
 )
 from .type_defs import (
     EnvironmentTemplateFilterTypeDef,
-    ListComponentOutputsOutputTypeDef,
-    ListComponentProvisionedResourcesOutputTypeDef,
-    ListComponentsOutputTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListEnvironmentAccountConnectionsOutputTypeDef,
-    ListEnvironmentOutputsOutputTypeDef,
-    ListEnvironmentProvisionedResourcesOutputTypeDef,
-    ListEnvironmentsOutputTypeDef,
-    ListEnvironmentTemplatesOutputTypeDef,
-    ListEnvironmentTemplateVersionsOutputTypeDef,
-    ListRepositoriesOutputTypeDef,
-    ListRepositorySyncDefinitionsOutputTypeDef,
-    ListServiceInstanceOutputsOutputTypeDef,
-    ListServiceInstanceProvisionedResourcesOutputTypeDef,
+    ListComponentOutputsOutputOutputTypeDef,
+    ListComponentProvisionedResourcesOutputOutputTypeDef,
+    ListComponentsOutputOutputTypeDef,
+    ListDeploymentsOutputOutputTypeDef,
+    ListEnvironmentAccountConnectionsOutputOutputTypeDef,
+    ListEnvironmentOutputsOutputOutputTypeDef,
+    ListEnvironmentProvisionedResourcesOutputOutputTypeDef,
+    ListEnvironmentsOutputOutputTypeDef,
+    ListEnvironmentTemplatesOutputOutputTypeDef,
+    ListEnvironmentTemplateVersionsOutputOutputTypeDef,
+    ListRepositoriesOutputOutputTypeDef,
+    ListRepositorySyncDefinitionsOutputOutputTypeDef,
+    ListServiceInstanceOutputsOutputOutputTypeDef,
+    ListServiceInstanceProvisionedResourcesOutputOutputTypeDef,
     ListServiceInstancesFilterTypeDef,
-    ListServiceInstancesOutputTypeDef,
-    ListServicePipelineOutputsOutputTypeDef,
-    ListServicePipelineProvisionedResourcesOutputTypeDef,
-    ListServicesOutputTypeDef,
-    ListServiceTemplatesOutputTypeDef,
-    ListServiceTemplateVersionsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
+    ListServiceInstancesOutputOutputTypeDef,
+    ListServicePipelineOutputsOutputOutputTypeDef,
+    ListServicePipelineProvisionedResourcesOutputOutputTypeDef,
+    ListServicesOutputOutputTypeDef,
+    ListServiceTemplatesOutputOutputTypeDef,
+    ListServiceTemplateVersionsOutputOutputTypeDef,
+    ListTagsForResourceOutputOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
@@ -141,30 +141,30 @@
 
     def paginate(
         self,
         *,
         componentName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListComponentOutputsOutputTypeDef]:
+    ) -> _PageIterator[ListComponentOutputsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
         """
 
 
 class ListComponentProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
     """
 
     def paginate(
         self, *, componentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListComponentProvisionedResourcesOutputTypeDef]:
+    ) -> _PageIterator[ListComponentProvisionedResourcesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
         """
 
 
 class ListComponentsPaginator(Paginator):
@@ -176,15 +176,15 @@
     def paginate(
         self,
         *,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListComponentsOutputTypeDef]:
+    ) -> _PageIterator[ListComponentsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
         """
 
 
 class ListDeploymentsPaginator(Paginator):
@@ -197,15 +197,15 @@
         self,
         *,
         componentName: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
+    ) -> _PageIterator[ListDeploymentsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listdeploymentspaginator)
         """
 
 
 class ListEnvironmentAccountConnectionsPaginator(Paginator):
@@ -217,15 +217,15 @@
     def paginate(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentAccountConnectionsOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentAccountConnectionsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
         """
 
 
 class ListEnvironmentOutputsPaginator(Paginator):
@@ -236,30 +236,30 @@
 
     def paginate(
         self,
         *,
         environmentName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentOutputsOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentOutputsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
         """
 
 
 class ListEnvironmentProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
     """
 
     def paginate(
         self, *, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentProvisionedResourcesOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentProvisionedResourcesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
         """
 
 
 class ListEnvironmentTemplateVersionsPaginator(Paginator):
@@ -270,30 +270,30 @@
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentTemplateVersionsOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentTemplateVersionsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplateversionspaginator)
         """
 
 
 class ListEnvironmentTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentTemplatesOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentTemplatesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
         """
 
 
 class ListEnvironmentsPaginator(Paginator):
@@ -303,30 +303,30 @@
     """
 
     def paginate(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentspaginator)
         """
 
 
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRepositoriesOutputTypeDef]:
+    ) -> _PageIterator[ListRepositoriesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
         """
 
 
 class ListRepositorySyncDefinitionsPaginator(Paginator):
@@ -338,15 +338,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRepositorySyncDefinitionsOutputTypeDef]:
+    ) -> _PageIterator[ListRepositorySyncDefinitionsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositorysyncdefinitionspaginator)
         """
 
 
 class ListServiceInstanceOutputsPaginator(Paginator):
@@ -358,15 +358,15 @@
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceInstanceOutputsOutputTypeDef]:
+    ) -> _PageIterator[ListServiceInstanceOutputsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
         """
 
 
 class ListServiceInstanceProvisionedResourcesPaginator(Paginator):
@@ -377,15 +377,15 @@
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceInstanceProvisionedResourcesOutputTypeDef]:
+    ) -> _PageIterator[ListServiceInstanceProvisionedResourcesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
         """
 
 
 class ListServiceInstancesPaginator(Paginator):
@@ -398,15 +398,15 @@
         self,
         *,
         filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
         serviceName: str = ...,
         sortBy: ListServiceInstancesSortByType = ...,
         sortOrder: SortOrderType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceInstancesOutputTypeDef]:
+    ) -> _PageIterator[ListServiceInstancesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstancespaginator)
         """
 
 
 class ListServicePipelineOutputsPaginator(Paginator):
@@ -417,30 +417,30 @@
 
     def paginate(
         self,
         *,
         serviceName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServicePipelineOutputsOutputTypeDef]:
+    ) -> _PageIterator[ListServicePipelineOutputsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
         """
 
 
 class ListServicePipelineProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
     """
 
     def paginate(
         self, *, serviceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServicePipelineProvisionedResourcesOutputTypeDef]:
+    ) -> _PageIterator[ListServicePipelineProvisionedResourcesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
         """
 
 
 class ListServiceTemplateVersionsPaginator(Paginator):
@@ -451,57 +451,57 @@
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceTemplateVersionsOutputTypeDef]:
+    ) -> _PageIterator[ListServiceTemplateVersionsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplateversionspaginator)
         """
 
 
 class ListServiceTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceTemplatesOutputTypeDef]:
+    ) -> _PageIterator[ListServiceTemplatesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
         """
 
 
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServicesOutputTypeDef]:
+    ) -> _PageIterator[ListServicesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
         self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
+    ) -> _PageIterator[ListTagsForResourceOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/paginator.pyi` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -69,36 +69,36 @@
     ListServiceInstancesSortByType,
     RepositoryProviderType,
     SortOrderType,
     SyncTypeType,
 )
 from .type_defs import (
     EnvironmentTemplateFilterTypeDef,
-    ListComponentOutputsOutputTypeDef,
-    ListComponentProvisionedResourcesOutputTypeDef,
-    ListComponentsOutputTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListEnvironmentAccountConnectionsOutputTypeDef,
-    ListEnvironmentOutputsOutputTypeDef,
-    ListEnvironmentProvisionedResourcesOutputTypeDef,
-    ListEnvironmentsOutputTypeDef,
-    ListEnvironmentTemplatesOutputTypeDef,
-    ListEnvironmentTemplateVersionsOutputTypeDef,
-    ListRepositoriesOutputTypeDef,
-    ListRepositorySyncDefinitionsOutputTypeDef,
-    ListServiceInstanceOutputsOutputTypeDef,
-    ListServiceInstanceProvisionedResourcesOutputTypeDef,
+    ListComponentOutputsOutputOutputTypeDef,
+    ListComponentProvisionedResourcesOutputOutputTypeDef,
+    ListComponentsOutputOutputTypeDef,
+    ListDeploymentsOutputOutputTypeDef,
+    ListEnvironmentAccountConnectionsOutputOutputTypeDef,
+    ListEnvironmentOutputsOutputOutputTypeDef,
+    ListEnvironmentProvisionedResourcesOutputOutputTypeDef,
+    ListEnvironmentsOutputOutputTypeDef,
+    ListEnvironmentTemplatesOutputOutputTypeDef,
+    ListEnvironmentTemplateVersionsOutputOutputTypeDef,
+    ListRepositoriesOutputOutputTypeDef,
+    ListRepositorySyncDefinitionsOutputOutputTypeDef,
+    ListServiceInstanceOutputsOutputOutputTypeDef,
+    ListServiceInstanceProvisionedResourcesOutputOutputTypeDef,
     ListServiceInstancesFilterTypeDef,
-    ListServiceInstancesOutputTypeDef,
-    ListServicePipelineOutputsOutputTypeDef,
-    ListServicePipelineProvisionedResourcesOutputTypeDef,
-    ListServicesOutputTypeDef,
-    ListServiceTemplatesOutputTypeDef,
-    ListServiceTemplateVersionsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
+    ListServiceInstancesOutputOutputTypeDef,
+    ListServicePipelineOutputsOutputOutputTypeDef,
+    ListServicePipelineProvisionedResourcesOutputOutputTypeDef,
+    ListServicesOutputOutputTypeDef,
+    ListServiceTemplatesOutputOutputTypeDef,
+    ListServiceTemplateVersionsOutputOutputTypeDef,
+    ListTagsForResourceOutputOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
@@ -138,29 +138,29 @@
 
     def paginate(
         self,
         *,
         componentName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListComponentOutputsOutputTypeDef]:
+    ) -> _PageIterator[ListComponentOutputsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
         """
 
 class ListComponentProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
     """
 
     def paginate(
         self, *, componentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListComponentProvisionedResourcesOutputTypeDef]:
+    ) -> _PageIterator[ListComponentProvisionedResourcesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
         """
 
 class ListComponentsPaginator(Paginator):
     """
@@ -171,15 +171,15 @@
     def paginate(
         self,
         *,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListComponentsOutputTypeDef]:
+    ) -> _PageIterator[ListComponentsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
         """
 
 class ListDeploymentsPaginator(Paginator):
     """
@@ -191,15 +191,15 @@
         self,
         *,
         componentName: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
+    ) -> _PageIterator[ListDeploymentsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listdeploymentspaginator)
         """
 
 class ListEnvironmentAccountConnectionsPaginator(Paginator):
     """
@@ -210,15 +210,15 @@
     def paginate(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentAccountConnectionsOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentAccountConnectionsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
         """
 
 class ListEnvironmentOutputsPaginator(Paginator):
     """
@@ -228,29 +228,29 @@
 
     def paginate(
         self,
         *,
         environmentName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentOutputsOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentOutputsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
         """
 
 class ListEnvironmentProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
     """
 
     def paginate(
         self, *, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentProvisionedResourcesOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentProvisionedResourcesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
         """
 
 class ListEnvironmentTemplateVersionsPaginator(Paginator):
     """
@@ -260,29 +260,29 @@
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentTemplateVersionsOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentTemplateVersionsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplateversionspaginator)
         """
 
 class ListEnvironmentTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentTemplatesOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentTemplatesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
         """
 
 class ListEnvironmentsPaginator(Paginator):
     """
@@ -291,29 +291,29 @@
     """
 
     def paginate(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentspaginator)
         """
 
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRepositoriesOutputTypeDef]:
+    ) -> _PageIterator[ListRepositoriesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
         """
 
 class ListRepositorySyncDefinitionsPaginator(Paginator):
     """
@@ -324,15 +324,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRepositorySyncDefinitionsOutputTypeDef]:
+    ) -> _PageIterator[ListRepositorySyncDefinitionsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositorysyncdefinitionspaginator)
         """
 
 class ListServiceInstanceOutputsPaginator(Paginator):
     """
@@ -343,15 +343,15 @@
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceInstanceOutputsOutputTypeDef]:
+    ) -> _PageIterator[ListServiceInstanceOutputsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
         """
 
 class ListServiceInstanceProvisionedResourcesPaginator(Paginator):
     """
@@ -361,15 +361,15 @@
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceInstanceProvisionedResourcesOutputTypeDef]:
+    ) -> _PageIterator[ListServiceInstanceProvisionedResourcesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
         """
 
 class ListServiceInstancesPaginator(Paginator):
     """
@@ -381,15 +381,15 @@
         self,
         *,
         filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
         serviceName: str = ...,
         sortBy: ListServiceInstancesSortByType = ...,
         sortOrder: SortOrderType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceInstancesOutputTypeDef]:
+    ) -> _PageIterator[ListServiceInstancesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstancespaginator)
         """
 
 class ListServicePipelineOutputsPaginator(Paginator):
     """
@@ -399,29 +399,29 @@
 
     def paginate(
         self,
         *,
         serviceName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServicePipelineOutputsOutputTypeDef]:
+    ) -> _PageIterator[ListServicePipelineOutputsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
         """
 
 class ListServicePipelineProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
     """
 
     def paginate(
         self, *, serviceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServicePipelineProvisionedResourcesOutputTypeDef]:
+    ) -> _PageIterator[ListServicePipelineProvisionedResourcesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
         """
 
 class ListServiceTemplateVersionsPaginator(Paginator):
     """
@@ -431,54 +431,54 @@
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceTemplateVersionsOutputTypeDef]:
+    ) -> _PageIterator[ListServiceTemplateVersionsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplateversionspaginator)
         """
 
 class ListServiceTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceTemplatesOutputTypeDef]:
+    ) -> _PageIterator[ListServiceTemplatesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
         """
 
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServicesOutputTypeDef]:
+    ) -> _PageIterator[ListServicesOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
         self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
+    ) -> _PageIterator[ListTagsForResourceOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/type_defs.py` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,84 +45,84 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
-    "EnvironmentAccountConnectionTypeDef",
-    "RepositoryBranchTypeDef",
+    "EnvironmentAccountConnectionOutputTypeDef",
+    "RepositoryBranchOutputTypeDef",
     "CancelComponentDeploymentInputRequestTypeDef",
-    "ComponentTypeDef",
+    "ComponentOutputTypeDef",
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
-    "ServiceInstanceTypeDef",
+    "ServiceInstanceOutputTypeDef",
     "CancelServicePipelineDeploymentInputRequestTypeDef",
-    "ServicePipelineTypeDef",
+    "ServicePipelineOutputTypeDef",
     "CompatibleEnvironmentTemplateInputTypeDef",
-    "CompatibleEnvironmentTemplateTypeDef",
-    "ComponentStateTypeDef",
-    "ComponentSummaryTypeDef",
-    "ResourceCountsSummaryTypeDef",
+    "CompatibleEnvironmentTemplateOutputTypeDef",
+    "ComponentStateOutputTypeDef",
+    "ComponentSummaryOutputTypeDef",
+    "ResourceCountsSummaryOutputTypeDef",
     "TagTypeDef",
     "RepositoryBranchInputTypeDef",
-    "EnvironmentTemplateTypeDef",
-    "EnvironmentTemplateVersionTypeDef",
-    "RepositoryTypeDef",
+    "EnvironmentTemplateOutputTypeDef",
+    "EnvironmentTemplateVersionOutputTypeDef",
+    "RepositoryOutputTypeDef",
     "CreateServiceSyncConfigInputRequestTypeDef",
-    "ServiceSyncConfigTypeDef",
-    "ServiceTemplateTypeDef",
+    "ServiceSyncConfigOutputTypeDef",
+    "ServiceTemplateOutputTypeDef",
     "CreateTemplateSyncConfigInputRequestTypeDef",
-    "TemplateSyncConfigTypeDef",
+    "TemplateSyncConfigOutputTypeDef",
     "DeleteComponentInputRequestTypeDef",
     "DeleteDeploymentInputRequestTypeDef",
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DeleteEnvironmentTemplateInputRequestTypeDef",
     "DeleteEnvironmentTemplateVersionInputRequestTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
     "DeleteServiceInputRequestTypeDef",
     "DeleteServiceSyncConfigInputRequestTypeDef",
     "DeleteServiceTemplateInputRequestTypeDef",
     "DeleteServiceTemplateVersionInputRequestTypeDef",
     "DeleteTemplateSyncConfigInputRequestTypeDef",
-    "EnvironmentStateTypeDef",
-    "ServiceInstanceStateTypeDef",
-    "ServicePipelineStateTypeDef",
-    "DeploymentSummaryTypeDef",
-    "EnvironmentAccountConnectionSummaryTypeDef",
-    "EnvironmentSummaryTypeDef",
+    "EnvironmentStateOutputTypeDef",
+    "ServiceInstanceStateOutputTypeDef",
+    "ServicePipelineStateOutputTypeDef",
+    "DeploymentSummaryOutputTypeDef",
+    "EnvironmentAccountConnectionSummaryOutputTypeDef",
+    "EnvironmentSummaryOutputTypeDef",
     "EnvironmentTemplateFilterTypeDef",
-    "EnvironmentTemplateSummaryTypeDef",
-    "EnvironmentTemplateVersionSummaryTypeDef",
+    "EnvironmentTemplateSummaryOutputTypeDef",
+    "EnvironmentTemplateVersionSummaryOutputTypeDef",
     "WaiterConfigTypeDef",
     "GetComponentInputRequestTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "GetEnvironmentTemplateInputRequestTypeDef",
     "GetEnvironmentTemplateVersionInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositorySyncStatusInputRequestTypeDef",
     "GetServiceInputRequestTypeDef",
     "GetServiceInstanceInputRequestTypeDef",
     "GetServiceInstanceSyncStatusInputRequestTypeDef",
-    "RevisionTypeDef",
+    "RevisionOutputTypeDef",
     "GetServiceSyncBlockerSummaryInputRequestTypeDef",
     "GetServiceSyncConfigInputRequestTypeDef",
     "GetServiceTemplateInputRequestTypeDef",
     "GetServiceTemplateVersionInputRequestTypeDef",
     "GetTemplateSyncConfigInputRequestTypeDef",
     "GetTemplateSyncStatusInputRequestTypeDef",
     "ListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     "ListComponentOutputsInputRequestTypeDef",
-    "OutputTypeDef",
+    "OutputOutputTypeDef",
     "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     "ListComponentProvisionedResourcesInputRequestTypeDef",
-    "ProvisionedResourceTypeDef",
+    "ProvisionedResourceOutputTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
     "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     "ListEnvironmentAccountConnectionsInputRequestTypeDef",
     "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
@@ -131,194 +131,196 @@
     "ListEnvironmentProvisionedResourcesInputRequestTypeDef",
     "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
     "ListEnvironmentTemplateVersionsInputRequestTypeDef",
     "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
     "ListEnvironmentTemplatesInputRequestTypeDef",
     "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
-    "RepositorySummaryTypeDef",
+    "RepositorySummaryOutputTypeDef",
     "ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
     "ListRepositorySyncDefinitionsInputRequestTypeDef",
-    "RepositorySyncDefinitionTypeDef",
+    "RepositorySyncDefinitionOutputTypeDef",
     "ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
     "ListServiceInstanceOutputsInputRequestTypeDef",
     "ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
     "ListServiceInstanceProvisionedResourcesInputRequestTypeDef",
     "ListServiceInstancesFilterTypeDef",
-    "ServiceInstanceSummaryTypeDef",
+    "ServiceInstanceSummaryOutputTypeDef",
     "ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     "ListServicePipelineOutputsInputRequestTypeDef",
     "ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
     "ListServicePipelineProvisionedResourcesInputRequestTypeDef",
     "ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
     "ListServiceTemplateVersionsInputRequestTypeDef",
-    "ServiceTemplateVersionSummaryTypeDef",
+    "ServiceTemplateVersionSummaryOutputTypeDef",
     "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
     "ListServiceTemplatesInputRequestTypeDef",
-    "ServiceTemplateSummaryTypeDef",
+    "ServiceTemplateSummaryOutputTypeDef",
     "ListServicesInputListServicesPaginateTypeDef",
     "ListServicesInputRequestTypeDef",
-    "ServiceSummaryTypeDef",
+    "ServiceSummaryOutputTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "TagOutputTypeDef",
+    "OutputTypeDef",
     "PaginatorConfigTypeDef",
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
-    "RepositorySyncEventTypeDef",
-    "ResourceSyncEventTypeDef",
+    "RepositorySyncEventOutputTypeDef",
+    "ResourceSyncEventOutputTypeDef",
     "ResponseMetadataTypeDef",
     "S3ObjectSourceTypeDef",
-    "SyncBlockerContextTypeDef",
+    "SyncBlockerContextOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateComponentInputRequestTypeDef",
     "UpdateEnvironmentAccountConnectionInputRequestTypeDef",
     "UpdateEnvironmentTemplateInputRequestTypeDef",
     "UpdateEnvironmentTemplateVersionInputRequestTypeDef",
     "UpdateServiceInputRequestTypeDef",
     "UpdateServiceInstanceInputRequestTypeDef",
     "UpdateServicePipelineInputRequestTypeDef",
     "UpdateServiceSyncBlockerInputRequestTypeDef",
     "UpdateServiceSyncConfigInputRequestTypeDef",
     "UpdateServiceTemplateInputRequestTypeDef",
     "UpdateTemplateSyncConfigInputRequestTypeDef",
-    "AcceptEnvironmentAccountConnectionOutputTypeDef",
-    "CreateEnvironmentAccountConnectionOutputTypeDef",
-    "DeleteEnvironmentAccountConnectionOutputTypeDef",
-    "GetEnvironmentAccountConnectionOutputTypeDef",
-    "RejectEnvironmentAccountConnectionOutputTypeDef",
-    "UpdateEnvironmentAccountConnectionOutputTypeDef",
-    "AccountSettingsTypeDef",
-    "EnvironmentTypeDef",
-    "CancelComponentDeploymentOutputTypeDef",
-    "CreateComponentOutputTypeDef",
-    "DeleteComponentOutputTypeDef",
-    "GetComponentOutputTypeDef",
-    "UpdateComponentOutputTypeDef",
-    "CancelServiceInstanceDeploymentOutputTypeDef",
-    "CreateServiceInstanceOutputTypeDef",
-    "GetServiceInstanceOutputTypeDef",
-    "UpdateServiceInstanceOutputTypeDef",
-    "CancelServicePipelineDeploymentOutputTypeDef",
-    "ServiceTypeDef",
-    "UpdateServicePipelineOutputTypeDef",
+    "AcceptEnvironmentAccountConnectionOutputOutputTypeDef",
+    "CreateEnvironmentAccountConnectionOutputOutputTypeDef",
+    "DeleteEnvironmentAccountConnectionOutputOutputTypeDef",
+    "GetEnvironmentAccountConnectionOutputOutputTypeDef",
+    "RejectEnvironmentAccountConnectionOutputOutputTypeDef",
+    "UpdateEnvironmentAccountConnectionOutputOutputTypeDef",
+    "AccountSettingsOutputTypeDef",
+    "EnvironmentOutputTypeDef",
+    "CancelComponentDeploymentOutputOutputTypeDef",
+    "CreateComponentOutputOutputTypeDef",
+    "DeleteComponentOutputOutputTypeDef",
+    "GetComponentOutputOutputTypeDef",
+    "UpdateComponentOutputOutputTypeDef",
+    "CancelServiceInstanceDeploymentOutputOutputTypeDef",
+    "CreateServiceInstanceOutputOutputTypeDef",
+    "GetServiceInstanceOutputOutputTypeDef",
+    "UpdateServiceInstanceOutputOutputTypeDef",
+    "CancelServicePipelineDeploymentOutputOutputTypeDef",
+    "ServiceOutputTypeDef",
+    "UpdateServicePipelineOutputOutputTypeDef",
     "UpdateServiceTemplateVersionInputRequestTypeDef",
-    "ServiceTemplateVersionTypeDef",
-    "ListComponentsOutputTypeDef",
-    "CountsSummaryTypeDef",
+    "ServiceTemplateVersionOutputTypeDef",
+    "ListComponentsOutputOutputTypeDef",
+    "CountsSummaryOutputTypeDef",
     "CreateComponentInputRequestTypeDef",
     "CreateEnvironmentAccountConnectionInputRequestTypeDef",
     "CreateEnvironmentTemplateInputRequestTypeDef",
     "CreateRepositoryInputRequestTypeDef",
     "CreateServiceInputRequestTypeDef",
     "CreateServiceInstanceInputRequestTypeDef",
     "CreateServiceTemplateInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
-    "CreateEnvironmentTemplateOutputTypeDef",
-    "DeleteEnvironmentTemplateOutputTypeDef",
-    "GetEnvironmentTemplateOutputTypeDef",
-    "UpdateEnvironmentTemplateOutputTypeDef",
-    "CreateEnvironmentTemplateVersionOutputTypeDef",
-    "DeleteEnvironmentTemplateVersionOutputTypeDef",
-    "GetEnvironmentTemplateVersionOutputTypeDef",
-    "UpdateEnvironmentTemplateVersionOutputTypeDef",
-    "CreateRepositoryOutputTypeDef",
-    "DeleteRepositoryOutputTypeDef",
-    "GetRepositoryOutputTypeDef",
-    "CreateServiceSyncConfigOutputTypeDef",
-    "DeleteServiceSyncConfigOutputTypeDef",
-    "GetServiceSyncConfigOutputTypeDef",
-    "UpdateServiceSyncConfigOutputTypeDef",
-    "CreateServiceTemplateOutputTypeDef",
-    "DeleteServiceTemplateOutputTypeDef",
-    "GetServiceTemplateOutputTypeDef",
-    "UpdateServiceTemplateOutputTypeDef",
-    "CreateTemplateSyncConfigOutputTypeDef",
-    "DeleteTemplateSyncConfigOutputTypeDef",
-    "GetTemplateSyncConfigOutputTypeDef",
-    "UpdateTemplateSyncConfigOutputTypeDef",
-    "DeploymentStateTypeDef",
-    "ListDeploymentsOutputTypeDef",
-    "ListEnvironmentAccountConnectionsOutputTypeDef",
-    "ListEnvironmentsOutputTypeDef",
+    "CreateEnvironmentTemplateOutputOutputTypeDef",
+    "DeleteEnvironmentTemplateOutputOutputTypeDef",
+    "GetEnvironmentTemplateOutputOutputTypeDef",
+    "UpdateEnvironmentTemplateOutputOutputTypeDef",
+    "CreateEnvironmentTemplateVersionOutputOutputTypeDef",
+    "DeleteEnvironmentTemplateVersionOutputOutputTypeDef",
+    "GetEnvironmentTemplateVersionOutputOutputTypeDef",
+    "UpdateEnvironmentTemplateVersionOutputOutputTypeDef",
+    "CreateRepositoryOutputOutputTypeDef",
+    "DeleteRepositoryOutputOutputTypeDef",
+    "GetRepositoryOutputOutputTypeDef",
+    "CreateServiceSyncConfigOutputOutputTypeDef",
+    "DeleteServiceSyncConfigOutputOutputTypeDef",
+    "GetServiceSyncConfigOutputOutputTypeDef",
+    "UpdateServiceSyncConfigOutputOutputTypeDef",
+    "CreateServiceTemplateOutputOutputTypeDef",
+    "DeleteServiceTemplateOutputOutputTypeDef",
+    "GetServiceTemplateOutputOutputTypeDef",
+    "UpdateServiceTemplateOutputOutputTypeDef",
+    "CreateTemplateSyncConfigOutputOutputTypeDef",
+    "DeleteTemplateSyncConfigOutputOutputTypeDef",
+    "GetTemplateSyncConfigOutputOutputTypeDef",
+    "UpdateTemplateSyncConfigOutputOutputTypeDef",
+    "DeploymentStateOutputTypeDef",
+    "ListDeploymentsOutputOutputTypeDef",
+    "ListEnvironmentAccountConnectionsOutputOutputTypeDef",
+    "ListEnvironmentsOutputOutputTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
-    "ListEnvironmentTemplatesOutputTypeDef",
-    "ListEnvironmentTemplateVersionsOutputTypeDef",
+    "ListEnvironmentTemplatesOutputOutputTypeDef",
+    "ListEnvironmentTemplateVersionsOutputOutputTypeDef",
     "GetComponentInputComponentDeletedWaitTypeDef",
     "GetComponentInputComponentDeployedWaitTypeDef",
     "GetEnvironmentInputEnvironmentDeployedWaitTypeDef",
     "GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef",
     "GetServiceInputServiceCreatedWaitTypeDef",
     "GetServiceInputServiceDeletedWaitTypeDef",
     "GetServiceInputServicePipelineDeployedWaitTypeDef",
     "GetServiceInputServiceUpdatedWaitTypeDef",
     "GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     "GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
-    "ListComponentOutputsOutputTypeDef",
-    "ListEnvironmentOutputsOutputTypeDef",
-    "ListServiceInstanceOutputsOutputTypeDef",
-    "ListServicePipelineOutputsOutputTypeDef",
-    "NotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    "ListComponentProvisionedResourcesOutputTypeDef",
-    "ListEnvironmentProvisionedResourcesOutputTypeDef",
-    "ListServiceInstanceProvisionedResourcesOutputTypeDef",
-    "ListServicePipelineProvisionedResourcesOutputTypeDef",
-    "ListRepositoriesOutputTypeDef",
-    "ListRepositorySyncDefinitionsOutputTypeDef",
+    "ListComponentOutputsOutputOutputTypeDef",
+    "ListEnvironmentOutputsOutputOutputTypeDef",
+    "ListServiceInstanceOutputsOutputOutputTypeDef",
+    "ListServicePipelineOutputsOutputOutputTypeDef",
+    "ListComponentProvisionedResourcesOutputOutputTypeDef",
+    "ListEnvironmentProvisionedResourcesOutputOutputTypeDef",
+    "ListServiceInstanceProvisionedResourcesOutputOutputTypeDef",
+    "ListServicePipelineProvisionedResourcesOutputOutputTypeDef",
+    "ListRepositoriesOutputOutputTypeDef",
+    "ListRepositorySyncDefinitionsOutputOutputTypeDef",
     "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
     "ListServiceInstancesInputRequestTypeDef",
-    "ListServiceInstancesOutputTypeDef",
-    "ListServiceTemplateVersionsOutputTypeDef",
-    "ListServiceTemplatesOutputTypeDef",
-    "ListServicesOutputTypeDef",
-    "RepositorySyncAttemptTypeDef",
-    "ResourceSyncAttemptTypeDef",
+    "ListServiceInstancesOutputOutputTypeDef",
+    "ListServiceTemplateVersionsOutputOutputTypeDef",
+    "ListServiceTemplatesOutputOutputTypeDef",
+    "ListServicesOutputOutputTypeDef",
+    "ListTagsForResourceOutputOutputTypeDef",
+    "NotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    "RepositorySyncAttemptOutputTypeDef",
+    "ResourceSyncAttemptOutputTypeDef",
     "TemplateVersionSourceInputTypeDef",
-    "SyncBlockerTypeDef",
-    "GetAccountSettingsOutputTypeDef",
-    "UpdateAccountSettingsOutputTypeDef",
-    "CancelEnvironmentDeploymentOutputTypeDef",
-    "CreateEnvironmentOutputTypeDef",
-    "DeleteEnvironmentOutputTypeDef",
-    "GetEnvironmentOutputTypeDef",
-    "UpdateEnvironmentOutputTypeDef",
-    "CreateServiceOutputTypeDef",
-    "DeleteServiceOutputTypeDef",
-    "GetServiceOutputTypeDef",
-    "UpdateServiceOutputTypeDef",
-    "CreateServiceTemplateVersionOutputTypeDef",
-    "DeleteServiceTemplateVersionOutputTypeDef",
-    "GetServiceTemplateVersionOutputTypeDef",
-    "UpdateServiceTemplateVersionOutputTypeDef",
-    "GetResourcesSummaryOutputTypeDef",
-    "DeploymentTypeDef",
-    "GetRepositorySyncStatusOutputTypeDef",
-    "GetServiceInstanceSyncStatusOutputTypeDef",
-    "GetTemplateSyncStatusOutputTypeDef",
+    "SyncBlockerOutputTypeDef",
+    "GetAccountSettingsOutputOutputTypeDef",
+    "UpdateAccountSettingsOutputOutputTypeDef",
+    "CancelEnvironmentDeploymentOutputOutputTypeDef",
+    "CreateEnvironmentOutputOutputTypeDef",
+    "DeleteEnvironmentOutputOutputTypeDef",
+    "GetEnvironmentOutputOutputTypeDef",
+    "UpdateEnvironmentOutputOutputTypeDef",
+    "CreateServiceOutputOutputTypeDef",
+    "DeleteServiceOutputOutputTypeDef",
+    "GetServiceOutputOutputTypeDef",
+    "UpdateServiceOutputOutputTypeDef",
+    "CreateServiceTemplateVersionOutputOutputTypeDef",
+    "DeleteServiceTemplateVersionOutputOutputTypeDef",
+    "GetServiceTemplateVersionOutputOutputTypeDef",
+    "UpdateServiceTemplateVersionOutputOutputTypeDef",
+    "GetResourcesSummaryOutputOutputTypeDef",
+    "DeploymentOutputTypeDef",
+    "GetRepositorySyncStatusOutputOutputTypeDef",
+    "GetServiceInstanceSyncStatusOutputOutputTypeDef",
+    "GetTemplateSyncStatusOutputOutputTypeDef",
     "CreateEnvironmentTemplateVersionInputRequestTypeDef",
     "CreateServiceTemplateVersionInputRequestTypeDef",
-    "ServiceSyncBlockerSummaryTypeDef",
-    "UpdateServiceSyncBlockerOutputTypeDef",
-    "DeleteDeploymentOutputTypeDef",
-    "GetDeploymentOutputTypeDef",
-    "GetServiceSyncBlockerSummaryOutputTypeDef",
+    "ServiceSyncBlockerSummaryOutputTypeDef",
+    "UpdateServiceSyncBlockerOutputOutputTypeDef",
+    "DeleteDeploymentOutputOutputTypeDef",
+    "GetDeploymentOutputOutputTypeDef",
+    "GetServiceSyncBlockerSummaryOutputOutputTypeDef",
 )
 
 AcceptEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-EnvironmentAccountConnectionTypeDef = TypedDict(
-    "EnvironmentAccountConnectionTypeDef",
+EnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "EnvironmentAccountConnectionOutputTypeDef",
     {
         "arn": str,
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
@@ -326,16 +328,16 @@
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
 
-RepositoryBranchTypeDef = TypedDict(
-    "RepositoryBranchTypeDef",
+RepositoryBranchOutputTypeDef = TypedDict(
+    "RepositoryBranchOutputTypeDef",
     {
         "arn": str,
         "branch": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
@@ -343,16 +345,16 @@
 CancelComponentDeploymentInputRequestTypeDef = TypedDict(
     "CancelComponentDeploymentInputRequestTypeDef",
     {
         "componentName": str,
     },
 )
 
-ComponentTypeDef = TypedDict(
-    "ComponentTypeDef",
+ComponentOutputTypeDef = TypedDict(
+    "ComponentOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentName": str,
@@ -380,16 +382,16 @@
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-ServiceInstanceTypeDef = TypedDict(
-    "ServiceInstanceTypeDef",
+ServiceInstanceOutputTypeDef = TypedDict(
+    "ServiceInstanceOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -409,16 +411,16 @@
 CancelServicePipelineDeploymentInputRequestTypeDef = TypedDict(
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
-ServicePipelineTypeDef = TypedDict(
-    "ServicePipelineTypeDef",
+ServicePipelineOutputTypeDef = TypedDict(
+    "ServicePipelineOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
@@ -435,34 +437,34 @@
     "CompatibleEnvironmentTemplateInputTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-CompatibleEnvironmentTemplateTypeDef = TypedDict(
-    "CompatibleEnvironmentTemplateTypeDef",
+CompatibleEnvironmentTemplateOutputTypeDef = TypedDict(
+    "CompatibleEnvironmentTemplateOutputTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-ComponentStateTypeDef = TypedDict(
-    "ComponentStateTypeDef",
+ComponentStateOutputTypeDef = TypedDict(
+    "ComponentStateOutputTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
         "templateFile": str,
     },
 )
 
-ComponentSummaryTypeDef = TypedDict(
-    "ComponentSummaryTypeDef",
+ComponentSummaryOutputTypeDef = TypedDict(
+    "ComponentSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -472,16 +474,16 @@
         "lastSucceededDeploymentId": str,
         "name": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-ResourceCountsSummaryTypeDef = TypedDict(
-    "ResourceCountsSummaryTypeDef",
+ResourceCountsSummaryOutputTypeDef = TypedDict(
+    "ResourceCountsSummaryOutputTypeDef",
     {
         "behindMajor": int,
         "behindMinor": int,
         "failed": int,
         "total": int,
         "upToDate": int,
     },
@@ -500,31 +502,31 @@
     {
         "branch": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
 
-EnvironmentTemplateTypeDef = TypedDict(
-    "EnvironmentTemplateTypeDef",
+EnvironmentTemplateOutputTypeDef = TypedDict(
+    "EnvironmentTemplateOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "encryptionKey": str,
         "lastModifiedAt": datetime,
         "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
 )
 
-EnvironmentTemplateVersionTypeDef = TypedDict(
-    "EnvironmentTemplateVersionTypeDef",
+EnvironmentTemplateVersionOutputTypeDef = TypedDict(
+    "EnvironmentTemplateVersionOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -532,16 +534,16 @@
         "schema": str,
         "status": TemplateVersionStatusType,
         "statusMessage": str,
         "templateName": str,
     },
 )
 
-RepositoryTypeDef = TypedDict(
-    "RepositoryTypeDef",
+RepositoryOutputTypeDef = TypedDict(
+    "RepositoryOutputTypeDef",
     {
         "arn": str,
         "connectionArn": str,
         "encryptionKey": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
@@ -554,27 +556,27 @@
         "filePath": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "serviceName": str,
     },
 )
 
-ServiceSyncConfigTypeDef = TypedDict(
-    "ServiceSyncConfigTypeDef",
+ServiceSyncConfigOutputTypeDef = TypedDict(
+    "ServiceSyncConfigOutputTypeDef",
     {
         "branch": str,
         "filePath": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "serviceName": str,
     },
 )
 
-ServiceTemplateTypeDef = TypedDict(
-    "ServiceTemplateTypeDef",
+ServiceTemplateOutputTypeDef = TypedDict(
+    "ServiceTemplateOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "encryptionKey": str,
         "lastModifiedAt": datetime,
@@ -606,16 +608,16 @@
 class CreateTemplateSyncConfigInputRequestTypeDef(
     _RequiredCreateTemplateSyncConfigInputRequestTypeDef,
     _OptionalCreateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
 
-TemplateSyncConfigTypeDef = TypedDict(
-    "TemplateSyncConfigTypeDef",
+TemplateSyncConfigOutputTypeDef = TypedDict(
+    "TemplateSyncConfigOutputTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "subdirectory": str,
         "templateName": str,
         "templateType": TemplateTypeType,
@@ -708,49 +710,49 @@
     "DeleteTemplateSyncConfigInputRequestTypeDef",
     {
         "templateName": str,
         "templateType": TemplateTypeType,
     },
 )
 
-EnvironmentStateTypeDef = TypedDict(
-    "EnvironmentStateTypeDef",
+EnvironmentStateOutputTypeDef = TypedDict(
+    "EnvironmentStateOutputTypeDef",
     {
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-ServiceInstanceStateTypeDef = TypedDict(
-    "ServiceInstanceStateTypeDef",
+ServiceInstanceStateOutputTypeDef = TypedDict(
+    "ServiceInstanceStateOutputTypeDef",
     {
         "lastSuccessfulComponentDeploymentIds": List[str],
         "lastSuccessfulEnvironmentDeploymentId": str,
         "lastSuccessfulServicePipelineDeploymentId": str,
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-ServicePipelineStateTypeDef = TypedDict(
-    "ServicePipelineStateTypeDef",
+ServicePipelineStateOutputTypeDef = TypedDict(
+    "ServicePipelineStateOutputTypeDef",
     {
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-DeploymentSummaryTypeDef = TypedDict(
-    "DeploymentSummaryTypeDef",
+DeploymentSummaryOutputTypeDef = TypedDict(
+    "DeploymentSummaryOutputTypeDef",
     {
         "arn": str,
         "completedAt": datetime,
         "componentName": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "environmentName": str,
@@ -762,32 +764,32 @@
         "serviceName": str,
         "targetArn": str,
         "targetResourceCreatedAt": datetime,
         "targetResourceType": DeploymentTargetResourceTypeType,
     },
 )
 
-EnvironmentAccountConnectionSummaryTypeDef = TypedDict(
-    "EnvironmentAccountConnectionSummaryTypeDef",
+EnvironmentAccountConnectionSummaryOutputTypeDef = TypedDict(
+    "EnvironmentAccountConnectionSummaryOutputTypeDef",
     {
         "arn": str,
         "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
         "lastModifiedAt": datetime,
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
 
-EnvironmentSummaryTypeDef = TypedDict(
-    "EnvironmentSummaryTypeDef",
+EnvironmentSummaryOutputTypeDef = TypedDict(
+    "EnvironmentSummaryOutputTypeDef",
     {
         "arn": str,
         "componentRoleArn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "description": str,
@@ -810,30 +812,30 @@
     "EnvironmentTemplateFilterTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-EnvironmentTemplateSummaryTypeDef = TypedDict(
-    "EnvironmentTemplateSummaryTypeDef",
+EnvironmentTemplateSummaryOutputTypeDef = TypedDict(
+    "EnvironmentTemplateSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "lastModifiedAt": datetime,
         "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
 )
 
-EnvironmentTemplateVersionSummaryTypeDef = TypedDict(
-    "EnvironmentTemplateVersionSummaryTypeDef",
+EnvironmentTemplateVersionSummaryOutputTypeDef = TypedDict(
+    "EnvironmentTemplateVersionSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -951,16 +953,16 @@
     "GetServiceInstanceSyncStatusInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-RevisionTypeDef = TypedDict(
-    "RevisionTypeDef",
+RevisionOutputTypeDef = TypedDict(
+    "RevisionOutputTypeDef",
     {
         "branch": str,
         "directory": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "sha": str,
     },
@@ -1070,16 +1072,16 @@
 class ListComponentOutputsInputRequestTypeDef(
     _RequiredListComponentOutputsInputRequestTypeDef,
     _OptionalListComponentOutputsInputRequestTypeDef,
 ):
     pass
 
 
-OutputTypeDef = TypedDict(
-    "OutputTypeDef",
+OutputOutputTypeDef = TypedDict(
+    "OutputOutputTypeDef",
     {
         "key": str,
         "valueString": str,
     },
 )
 
 _RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
@@ -1122,16 +1124,16 @@
 class ListComponentProvisionedResourcesInputRequestTypeDef(
     _RequiredListComponentProvisionedResourcesInputRequestTypeDef,
     _OptionalListComponentProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
 
-ProvisionedResourceTypeDef = TypedDict(
-    "ProvisionedResourceTypeDef",
+ProvisionedResourceOutputTypeDef = TypedDict(
+    "ProvisionedResourceOutputTypeDef",
     {
         "identifier": str,
         "name": str,
         "provisioningEngine": ProvisionedResourceEngineType,
     },
 )
 
@@ -1399,16 +1401,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-RepositorySummaryTypeDef = TypedDict(
-    "RepositorySummaryTypeDef",
+RepositorySummaryOutputTypeDef = TypedDict(
+    "RepositorySummaryOutputTypeDef",
     {
         "arn": str,
         "connectionArn": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
@@ -1457,16 +1459,16 @@
 class ListRepositorySyncDefinitionsInputRequestTypeDef(
     _RequiredListRepositorySyncDefinitionsInputRequestTypeDef,
     _OptionalListRepositorySyncDefinitionsInputRequestTypeDef,
 ):
     pass
 
 
-RepositorySyncDefinitionTypeDef = TypedDict(
-    "RepositorySyncDefinitionTypeDef",
+RepositorySyncDefinitionOutputTypeDef = TypedDict(
+    "RepositorySyncDefinitionOutputTypeDef",
     {
         "branch": str,
         "directory": str,
         "parent": str,
         "target": str,
     },
 )
@@ -1570,16 +1572,16 @@
     {
         "key": ListServiceInstancesFilterByType,
         "value": str,
     },
     total=False,
 )
 
-ServiceInstanceSummaryTypeDef = TypedDict(
-    "ServiceInstanceSummaryTypeDef",
+ServiceInstanceSummaryOutputTypeDef = TypedDict(
+    "ServiceInstanceSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -1727,16 +1729,16 @@
 class ListServiceTemplateVersionsInputRequestTypeDef(
     _RequiredListServiceTemplateVersionsInputRequestTypeDef,
     _OptionalListServiceTemplateVersionsInputRequestTypeDef,
 ):
     pass
 
 
-ServiceTemplateVersionSummaryTypeDef = TypedDict(
-    "ServiceTemplateVersionSummaryTypeDef",
+ServiceTemplateVersionSummaryOutputTypeDef = TypedDict(
+    "ServiceTemplateVersionSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -1760,16 +1762,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ServiceTemplateSummaryTypeDef = TypedDict(
-    "ServiceTemplateSummaryTypeDef",
+ServiceTemplateSummaryOutputTypeDef = TypedDict(
+    "ServiceTemplateSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "lastModifiedAt": datetime,
         "name": str,
@@ -1791,16 +1793,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ServiceSummaryTypeDef = TypedDict(
-    "ServiceSummaryTypeDef",
+ServiceSummaryOutputTypeDef = TypedDict(
+    "ServiceSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
@@ -1849,14 +1851,31 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+OutputTypeDef = TypedDict(
+    "OutputTypeDef",
+    {
+        "key": str,
+        "valueString": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1866,26 +1885,26 @@
 RejectEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-RepositorySyncEventTypeDef = TypedDict(
-    "RepositorySyncEventTypeDef",
+RepositorySyncEventOutputTypeDef = TypedDict(
+    "RepositorySyncEventOutputTypeDef",
     {
         "event": str,
         "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
 
-ResourceSyncEventTypeDef = TypedDict(
-    "ResourceSyncEventTypeDef",
+ResourceSyncEventOutputTypeDef = TypedDict(
+    "ResourceSyncEventOutputTypeDef",
     {
         "event": str,
         "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
@@ -1905,16 +1924,16 @@
     "S3ObjectSourceTypeDef",
     {
         "bucket": str,
         "key": str,
     },
 )
 
-SyncBlockerContextTypeDef = TypedDict(
-    "SyncBlockerContextTypeDef",
+SyncBlockerContextOutputTypeDef = TypedDict(
+    "SyncBlockerContextOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
 UntagResourceInputRequestTypeDef = TypedDict(
@@ -2162,73 +2181,73 @@
 class UpdateTemplateSyncConfigInputRequestTypeDef(
     _RequiredUpdateTemplateSyncConfigInputRequestTypeDef,
     _OptionalUpdateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
 
-AcceptEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "AcceptEnvironmentAccountConnectionOutputTypeDef",
+AcceptEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "AcceptEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "CreateEnvironmentAccountConnectionOutputTypeDef",
+CreateEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "CreateEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "DeleteEnvironmentAccountConnectionOutputTypeDef",
+DeleteEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "DeleteEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "GetEnvironmentAccountConnectionOutputTypeDef",
+GetEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "GetEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RejectEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "RejectEnvironmentAccountConnectionOutputTypeDef",
+RejectEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "RejectEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "UpdateEnvironmentAccountConnectionOutputTypeDef",
+UpdateEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "UpdateEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AccountSettingsTypeDef = TypedDict(
-    "AccountSettingsTypeDef",
+AccountSettingsOutputTypeDef = TypedDict(
+    "AccountSettingsOutputTypeDef",
     {
         "pipelineCodebuildRoleArn": str,
-        "pipelineProvisioningRepository": RepositoryBranchTypeDef,
+        "pipelineProvisioningRepository": RepositoryBranchOutputTypeDef,
         "pipelineServiceRoleArn": str,
     },
 )
 
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
+EnvironmentOutputTypeDef = TypedDict(
+    "EnvironmentOutputTypeDef",
     {
         "arn": str,
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
@@ -2238,125 +2257,125 @@
         "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
         "lastSucceededDeploymentId": str,
         "name": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
-        "provisioningRepository": RepositoryBranchTypeDef,
+        "provisioningRepository": RepositoryBranchOutputTypeDef,
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-CancelComponentDeploymentOutputTypeDef = TypedDict(
-    "CancelComponentDeploymentOutputTypeDef",
+CancelComponentDeploymentOutputOutputTypeDef = TypedDict(
+    "CancelComponentDeploymentOutputOutputTypeDef",
     {
-        "component": ComponentTypeDef,
+        "component": ComponentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateComponentOutputTypeDef = TypedDict(
-    "CreateComponentOutputTypeDef",
+CreateComponentOutputOutputTypeDef = TypedDict(
+    "CreateComponentOutputOutputTypeDef",
     {
-        "component": ComponentTypeDef,
+        "component": ComponentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteComponentOutputTypeDef = TypedDict(
-    "DeleteComponentOutputTypeDef",
+DeleteComponentOutputOutputTypeDef = TypedDict(
+    "DeleteComponentOutputOutputTypeDef",
     {
-        "component": ComponentTypeDef,
+        "component": ComponentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetComponentOutputTypeDef = TypedDict(
-    "GetComponentOutputTypeDef",
+GetComponentOutputOutputTypeDef = TypedDict(
+    "GetComponentOutputOutputTypeDef",
     {
-        "component": ComponentTypeDef,
+        "component": ComponentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateComponentOutputTypeDef = TypedDict(
-    "UpdateComponentOutputTypeDef",
+UpdateComponentOutputOutputTypeDef = TypedDict(
+    "UpdateComponentOutputOutputTypeDef",
     {
-        "component": ComponentTypeDef,
+        "component": ComponentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelServiceInstanceDeploymentOutputTypeDef = TypedDict(
-    "CancelServiceInstanceDeploymentOutputTypeDef",
+CancelServiceInstanceDeploymentOutputOutputTypeDef = TypedDict(
+    "CancelServiceInstanceDeploymentOutputOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceTypeDef,
+        "serviceInstance": ServiceInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceInstanceOutputTypeDef = TypedDict(
-    "CreateServiceInstanceOutputTypeDef",
+CreateServiceInstanceOutputOutputTypeDef = TypedDict(
+    "CreateServiceInstanceOutputOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceTypeDef,
+        "serviceInstance": ServiceInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceInstanceOutputTypeDef = TypedDict(
-    "GetServiceInstanceOutputTypeDef",
+GetServiceInstanceOutputOutputTypeDef = TypedDict(
+    "GetServiceInstanceOutputOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceTypeDef,
+        "serviceInstance": ServiceInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceInstanceOutputTypeDef = TypedDict(
-    "UpdateServiceInstanceOutputTypeDef",
+UpdateServiceInstanceOutputOutputTypeDef = TypedDict(
+    "UpdateServiceInstanceOutputOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceTypeDef,
+        "serviceInstance": ServiceInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelServicePipelineDeploymentOutputTypeDef = TypedDict(
-    "CancelServicePipelineDeploymentOutputTypeDef",
+CancelServicePipelineDeploymentOutputOutputTypeDef = TypedDict(
+    "CancelServicePipelineDeploymentOutputOutputTypeDef",
     {
-        "pipeline": ServicePipelineTypeDef,
+        "pipeline": ServicePipelineOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ServiceTypeDef = TypedDict(
-    "ServiceTypeDef",
+ServiceOutputTypeDef = TypedDict(
+    "ServiceOutputTypeDef",
     {
         "arn": str,
         "branchName": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "name": str,
-        "pipeline": ServicePipelineTypeDef,
+        "pipeline": ServicePipelineOutputTypeDef,
         "repositoryConnectionArn": str,
         "repositoryId": str,
         "spec": str,
         "status": ServiceStatusType,
         "statusMessage": str,
         "templateName": str,
     },
 )
 
-UpdateServicePipelineOutputTypeDef = TypedDict(
-    "UpdateServicePipelineOutputTypeDef",
+UpdateServicePipelineOutputOutputTypeDef = TypedDict(
+    "UpdateServicePipelineOutputOutputTypeDef",
     {
-        "pipeline": ServicePipelineTypeDef,
+        "pipeline": ServicePipelineOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateServiceTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceTemplateVersionInputRequestTypeDef",
     {
@@ -2380,52 +2399,52 @@
 class UpdateServiceTemplateVersionInputRequestTypeDef(
     _RequiredUpdateServiceTemplateVersionInputRequestTypeDef,
     _OptionalUpdateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
 
-ServiceTemplateVersionTypeDef = TypedDict(
-    "ServiceTemplateVersionTypeDef",
+ServiceTemplateVersionOutputTypeDef = TypedDict(
+    "ServiceTemplateVersionOutputTypeDef",
     {
         "arn": str,
-        "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateTypeDef],
+        "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateOutputTypeDef],
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
         "recommendedMinorVersion": str,
         "schema": str,
         "status": TemplateVersionStatusType,
         "statusMessage": str,
         "supportedComponentSources": List[Literal["DIRECTLY_DEFINED"]],
         "templateName": str,
     },
 )
 
-ListComponentsOutputTypeDef = TypedDict(
-    "ListComponentsOutputTypeDef",
+ListComponentsOutputOutputTypeDef = TypedDict(
+    "ListComponentsOutputOutputTypeDef",
     {
-        "components": List[ComponentSummaryTypeDef],
+        "components": List[ComponentSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CountsSummaryTypeDef = TypedDict(
-    "CountsSummaryTypeDef",
+CountsSummaryOutputTypeDef = TypedDict(
+    "CountsSummaryOutputTypeDef",
     {
-        "components": ResourceCountsSummaryTypeDef,
-        "environmentTemplates": ResourceCountsSummaryTypeDef,
-        "environments": ResourceCountsSummaryTypeDef,
-        "pipelines": ResourceCountsSummaryTypeDef,
-        "serviceInstances": ResourceCountsSummaryTypeDef,
-        "serviceTemplates": ResourceCountsSummaryTypeDef,
-        "services": ResourceCountsSummaryTypeDef,
+        "components": ResourceCountsSummaryOutputTypeDef,
+        "environmentTemplates": ResourceCountsSummaryOutputTypeDef,
+        "environments": ResourceCountsSummaryOutputTypeDef,
+        "pipelines": ResourceCountsSummaryOutputTypeDef,
+        "serviceInstances": ResourceCountsSummaryOutputTypeDef,
+        "serviceTemplates": ResourceCountsSummaryOutputTypeDef,
+        "services": ResourceCountsSummaryOutputTypeDef,
     },
 )
 
 _RequiredCreateComponentInputRequestTypeDef = TypedDict(
     "_RequiredCreateComponentInputRequestTypeDef",
     {
         "manifest": str,
@@ -2609,23 +2628,14 @@
 class CreateServiceTemplateInputRequestTypeDef(
     _RequiredCreateServiceTemplateInputRequestTypeDef,
     _OptionalCreateServiceTemplateInputRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "nextToken": str,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -2698,230 +2708,230 @@
 
 class UpdateEnvironmentInputRequestTypeDef(
     _RequiredUpdateEnvironmentInputRequestTypeDef, _OptionalUpdateEnvironmentInputRequestTypeDef
 ):
     pass
 
 
-CreateEnvironmentTemplateOutputTypeDef = TypedDict(
-    "CreateEnvironmentTemplateOutputTypeDef",
+CreateEnvironmentTemplateOutputOutputTypeDef = TypedDict(
+    "CreateEnvironmentTemplateOutputOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateTypeDef,
+        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentTemplateOutputTypeDef = TypedDict(
-    "DeleteEnvironmentTemplateOutputTypeDef",
+DeleteEnvironmentTemplateOutputOutputTypeDef = TypedDict(
+    "DeleteEnvironmentTemplateOutputOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateTypeDef,
+        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentTemplateOutputTypeDef = TypedDict(
-    "GetEnvironmentTemplateOutputTypeDef",
+GetEnvironmentTemplateOutputOutputTypeDef = TypedDict(
+    "GetEnvironmentTemplateOutputOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateTypeDef,
+        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentTemplateOutputTypeDef = TypedDict(
-    "UpdateEnvironmentTemplateOutputTypeDef",
+UpdateEnvironmentTemplateOutputOutputTypeDef = TypedDict(
+    "UpdateEnvironmentTemplateOutputOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateTypeDef,
+        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
-    "CreateEnvironmentTemplateVersionOutputTypeDef",
+CreateEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
+    "CreateEnvironmentTemplateVersionOutputOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentTemplateVersionOutputTypeDef = TypedDict(
-    "DeleteEnvironmentTemplateVersionOutputTypeDef",
+DeleteEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
+    "DeleteEnvironmentTemplateVersionOutputOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentTemplateVersionOutputTypeDef = TypedDict(
-    "GetEnvironmentTemplateVersionOutputTypeDef",
+GetEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
+    "GetEnvironmentTemplateVersionOutputOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
-    "UpdateEnvironmentTemplateVersionOutputTypeDef",
+UpdateEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
+    "UpdateEnvironmentTemplateVersionOutputOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRepositoryOutputTypeDef = TypedDict(
-    "CreateRepositoryOutputTypeDef",
+CreateRepositoryOutputOutputTypeDef = TypedDict(
+    "CreateRepositoryOutputOutputTypeDef",
     {
-        "repository": RepositoryTypeDef,
+        "repository": RepositoryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRepositoryOutputTypeDef = TypedDict(
-    "DeleteRepositoryOutputTypeDef",
+DeleteRepositoryOutputOutputTypeDef = TypedDict(
+    "DeleteRepositoryOutputOutputTypeDef",
     {
-        "repository": RepositoryTypeDef,
+        "repository": RepositoryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetRepositoryOutputTypeDef = TypedDict(
-    "GetRepositoryOutputTypeDef",
+GetRepositoryOutputOutputTypeDef = TypedDict(
+    "GetRepositoryOutputOutputTypeDef",
     {
-        "repository": RepositoryTypeDef,
+        "repository": RepositoryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceSyncConfigOutputTypeDef = TypedDict(
-    "CreateServiceSyncConfigOutputTypeDef",
+CreateServiceSyncConfigOutputOutputTypeDef = TypedDict(
+    "CreateServiceSyncConfigOutputOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceSyncConfigOutputTypeDef = TypedDict(
-    "DeleteServiceSyncConfigOutputTypeDef",
+DeleteServiceSyncConfigOutputOutputTypeDef = TypedDict(
+    "DeleteServiceSyncConfigOutputOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceSyncConfigOutputTypeDef = TypedDict(
-    "GetServiceSyncConfigOutputTypeDef",
+GetServiceSyncConfigOutputOutputTypeDef = TypedDict(
+    "GetServiceSyncConfigOutputOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceSyncConfigOutputTypeDef = TypedDict(
-    "UpdateServiceSyncConfigOutputTypeDef",
+UpdateServiceSyncConfigOutputOutputTypeDef = TypedDict(
+    "UpdateServiceSyncConfigOutputOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceTemplateOutputTypeDef = TypedDict(
-    "CreateServiceTemplateOutputTypeDef",
+CreateServiceTemplateOutputOutputTypeDef = TypedDict(
+    "CreateServiceTemplateOutputOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateTypeDef,
+        "serviceTemplate": ServiceTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceTemplateOutputTypeDef = TypedDict(
-    "DeleteServiceTemplateOutputTypeDef",
+DeleteServiceTemplateOutputOutputTypeDef = TypedDict(
+    "DeleteServiceTemplateOutputOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateTypeDef,
+        "serviceTemplate": ServiceTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceTemplateOutputTypeDef = TypedDict(
-    "GetServiceTemplateOutputTypeDef",
+GetServiceTemplateOutputOutputTypeDef = TypedDict(
+    "GetServiceTemplateOutputOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateTypeDef,
+        "serviceTemplate": ServiceTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceTemplateOutputTypeDef = TypedDict(
-    "UpdateServiceTemplateOutputTypeDef",
+UpdateServiceTemplateOutputOutputTypeDef = TypedDict(
+    "UpdateServiceTemplateOutputOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateTypeDef,
+        "serviceTemplate": ServiceTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateTemplateSyncConfigOutputTypeDef = TypedDict(
-    "CreateTemplateSyncConfigOutputTypeDef",
+CreateTemplateSyncConfigOutputOutputTypeDef = TypedDict(
+    "CreateTemplateSyncConfigOutputOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigTypeDef,
+        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteTemplateSyncConfigOutputTypeDef = TypedDict(
-    "DeleteTemplateSyncConfigOutputTypeDef",
+DeleteTemplateSyncConfigOutputOutputTypeDef = TypedDict(
+    "DeleteTemplateSyncConfigOutputOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigTypeDef,
+        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetTemplateSyncConfigOutputTypeDef = TypedDict(
-    "GetTemplateSyncConfigOutputTypeDef",
+GetTemplateSyncConfigOutputOutputTypeDef = TypedDict(
+    "GetTemplateSyncConfigOutputOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigTypeDef,
+        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateTemplateSyncConfigOutputTypeDef = TypedDict(
-    "UpdateTemplateSyncConfigOutputTypeDef",
+UpdateTemplateSyncConfigOutputOutputTypeDef = TypedDict(
+    "UpdateTemplateSyncConfigOutputOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigTypeDef,
+        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeploymentStateTypeDef = TypedDict(
-    "DeploymentStateTypeDef",
+DeploymentStateOutputTypeDef = TypedDict(
+    "DeploymentStateOutputTypeDef",
     {
-        "component": ComponentStateTypeDef,
-        "environment": EnvironmentStateTypeDef,
-        "serviceInstance": ServiceInstanceStateTypeDef,
-        "servicePipeline": ServicePipelineStateTypeDef,
+        "component": ComponentStateOutputTypeDef,
+        "environment": EnvironmentStateOutputTypeDef,
+        "serviceInstance": ServiceInstanceStateOutputTypeDef,
+        "servicePipeline": ServicePipelineStateOutputTypeDef,
     },
 )
 
-ListDeploymentsOutputTypeDef = TypedDict(
-    "ListDeploymentsOutputTypeDef",
+ListDeploymentsOutputOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputOutputTypeDef",
     {
-        "deployments": List[DeploymentSummaryTypeDef],
+        "deployments": List[DeploymentSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentAccountConnectionsOutputTypeDef = TypedDict(
-    "ListEnvironmentAccountConnectionsOutputTypeDef",
+ListEnvironmentAccountConnectionsOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentAccountConnectionsOutputOutputTypeDef",
     {
-        "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryTypeDef],
+        "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentsOutputTypeDef = TypedDict(
-    "ListEnvironmentsOutputTypeDef",
+ListEnvironmentsOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentsOutputOutputTypeDef",
     {
-        "environments": List[EnvironmentSummaryTypeDef],
+        "environments": List[EnvironmentSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
@@ -2938,28 +2948,28 @@
         "environmentTemplates": Sequence[EnvironmentTemplateFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListEnvironmentTemplatesOutputTypeDef = TypedDict(
-    "ListEnvironmentTemplatesOutputTypeDef",
+ListEnvironmentTemplatesOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentTemplatesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "templates": List[EnvironmentTemplateSummaryTypeDef],
+        "templates": List[EnvironmentTemplateSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentTemplateVersionsOutputTypeDef = TypedDict(
-    "ListEnvironmentTemplateVersionsOutputTypeDef",
+ListEnvironmentTemplateVersionsOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentTemplateVersionsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "templateVersions": List[EnvironmentTemplateVersionSummaryTypeDef],
+        "templateVersions": List[EnvironmentTemplateVersionSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetComponentInputComponentDeletedWaitTypeDef = TypedDict(
     "_RequiredGetComponentInputComponentDeletedWaitTypeDef",
     {
@@ -3181,125 +3191,100 @@
 class GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef(
     _RequiredGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
     _OptionalGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
 ):
     pass
 
 
-ListComponentOutputsOutputTypeDef = TypedDict(
-    "ListComponentOutputsOutputTypeDef",
+ListComponentOutputsOutputOutputTypeDef = TypedDict(
+    "ListComponentOutputsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputTypeDef],
+        "outputs": List[OutputOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentOutputsOutputTypeDef = TypedDict(
-    "ListEnvironmentOutputsOutputTypeDef",
+ListEnvironmentOutputsOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentOutputsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputTypeDef],
+        "outputs": List[OutputOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceInstanceOutputsOutputTypeDef = TypedDict(
-    "ListServiceInstanceOutputsOutputTypeDef",
+ListServiceInstanceOutputsOutputOutputTypeDef = TypedDict(
+    "ListServiceInstanceOutputsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputTypeDef],
+        "outputs": List[OutputOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicePipelineOutputsOutputTypeDef = TypedDict(
-    "ListServicePipelineOutputsOutputTypeDef",
+ListServicePipelineOutputsOutputOutputTypeDef = TypedDict(
+    "ListServicePipelineOutputsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputTypeDef],
+        "outputs": List[OutputOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
-    "_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
-    "_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    {
-        "deploymentId": str,
-        "outputs": Sequence[OutputTypeDef],
-        "status": ResourceDeploymentStatusType,
-        "statusMessage": str,
-    },
-    total=False,
-)
-
-
-class NotifyResourceDeploymentStatusChangeInputRequestTypeDef(
-    _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
-    _OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
-):
-    pass
-
-
-ListComponentProvisionedResourcesOutputTypeDef = TypedDict(
-    "ListComponentProvisionedResourcesOutputTypeDef",
+ListComponentProvisionedResourcesOutputOutputTypeDef = TypedDict(
+    "ListComponentProvisionedResourcesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceTypeDef],
+        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentProvisionedResourcesOutputTypeDef = TypedDict(
-    "ListEnvironmentProvisionedResourcesOutputTypeDef",
+ListEnvironmentProvisionedResourcesOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentProvisionedResourcesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceTypeDef],
+        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceInstanceProvisionedResourcesOutputTypeDef = TypedDict(
-    "ListServiceInstanceProvisionedResourcesOutputTypeDef",
+ListServiceInstanceProvisionedResourcesOutputOutputTypeDef = TypedDict(
+    "ListServiceInstanceProvisionedResourcesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceTypeDef],
+        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicePipelineProvisionedResourcesOutputTypeDef = TypedDict(
-    "ListServicePipelineProvisionedResourcesOutputTypeDef",
+ListServicePipelineProvisionedResourcesOutputOutputTypeDef = TypedDict(
+    "ListServicePipelineProvisionedResourcesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceTypeDef],
+        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRepositoriesOutputTypeDef = TypedDict(
-    "ListRepositoriesOutputTypeDef",
+ListRepositoriesOutputOutputTypeDef = TypedDict(
+    "ListRepositoriesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "repositories": List[RepositorySummaryTypeDef],
+        "repositories": List[RepositorySummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRepositorySyncDefinitionsOutputTypeDef = TypedDict(
-    "ListRepositorySyncDefinitionsOutputTypeDef",
+ListRepositorySyncDefinitionsOutputOutputTypeDef = TypedDict(
+    "ListRepositorySyncDefinitionsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "syncDefinitions": List[RepositorySyncDefinitionTypeDef],
+        "syncDefinitions": List[RepositorySyncDefinitionOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceInstancesInputListServiceInstancesPaginateTypeDef = TypedDict(
     "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
     {
@@ -3321,269 +3306,303 @@
         "serviceName": str,
         "sortBy": ListServiceInstancesSortByType,
         "sortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListServiceInstancesOutputTypeDef = TypedDict(
-    "ListServiceInstancesOutputTypeDef",
+ListServiceInstancesOutputOutputTypeDef = TypedDict(
+    "ListServiceInstancesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "serviceInstances": List[ServiceInstanceSummaryTypeDef],
+        "serviceInstances": List[ServiceInstanceSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceTemplateVersionsOutputTypeDef = TypedDict(
-    "ListServiceTemplateVersionsOutputTypeDef",
+ListServiceTemplateVersionsOutputOutputTypeDef = TypedDict(
+    "ListServiceTemplateVersionsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "templateVersions": List[ServiceTemplateVersionSummaryTypeDef],
+        "templateVersions": List[ServiceTemplateVersionSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceTemplatesOutputTypeDef = TypedDict(
-    "ListServiceTemplatesOutputTypeDef",
+ListServiceTemplatesOutputOutputTypeDef = TypedDict(
+    "ListServiceTemplatesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "templates": List[ServiceTemplateSummaryTypeDef],
+        "templates": List[ServiceTemplateSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicesOutputTypeDef = TypedDict(
-    "ListServicesOutputTypeDef",
+ListServicesOutputOutputTypeDef = TypedDict(
+    "ListServicesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "services": List[ServiceSummaryTypeDef],
+        "services": List[ServiceSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RepositorySyncAttemptTypeDef = TypedDict(
-    "RepositorySyncAttemptTypeDef",
+ListTagsForResourceOutputOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputOutputTypeDef",
+    {
+        "nextToken": str,
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
+    "_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
+    "_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    {
+        "deploymentId": str,
+        "outputs": Sequence[OutputTypeDef],
+        "status": ResourceDeploymentStatusType,
+        "statusMessage": str,
+    },
+    total=False,
+)
+
+
+class NotifyResourceDeploymentStatusChangeInputRequestTypeDef(
+    _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
+    _OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
+):
+    pass
+
+
+RepositorySyncAttemptOutputTypeDef = TypedDict(
+    "RepositorySyncAttemptOutputTypeDef",
     {
-        "events": List[RepositorySyncEventTypeDef],
+        "events": List[RepositorySyncEventOutputTypeDef],
         "startedAt": datetime,
         "status": RepositorySyncStatusType,
     },
 )
 
-ResourceSyncAttemptTypeDef = TypedDict(
-    "ResourceSyncAttemptTypeDef",
+ResourceSyncAttemptOutputTypeDef = TypedDict(
+    "ResourceSyncAttemptOutputTypeDef",
     {
-        "events": List[ResourceSyncEventTypeDef],
-        "initialRevision": RevisionTypeDef,
+        "events": List[ResourceSyncEventOutputTypeDef],
+        "initialRevision": RevisionOutputTypeDef,
         "startedAt": datetime,
         "status": ResourceSyncStatusType,
         "target": str,
-        "targetRevision": RevisionTypeDef,
+        "targetRevision": RevisionOutputTypeDef,
     },
 )
 
 TemplateVersionSourceInputTypeDef = TypedDict(
     "TemplateVersionSourceInputTypeDef",
     {
         "s3": S3ObjectSourceTypeDef,
     },
     total=False,
 )
 
-SyncBlockerTypeDef = TypedDict(
-    "SyncBlockerTypeDef",
+SyncBlockerOutputTypeDef = TypedDict(
+    "SyncBlockerOutputTypeDef",
     {
-        "contexts": List[SyncBlockerContextTypeDef],
+        "contexts": List[SyncBlockerContextOutputTypeDef],
         "createdAt": datetime,
         "createdReason": str,
         "id": str,
         "resolvedAt": datetime,
         "resolvedReason": str,
         "status": BlockerStatusType,
         "type": Literal["AUTOMATED"],
     },
 )
 
-GetAccountSettingsOutputTypeDef = TypedDict(
-    "GetAccountSettingsOutputTypeDef",
+GetAccountSettingsOutputOutputTypeDef = TypedDict(
+    "GetAccountSettingsOutputOutputTypeDef",
     {
-        "accountSettings": AccountSettingsTypeDef,
+        "accountSettings": AccountSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAccountSettingsOutputTypeDef = TypedDict(
-    "UpdateAccountSettingsOutputTypeDef",
+UpdateAccountSettingsOutputOutputTypeDef = TypedDict(
+    "UpdateAccountSettingsOutputOutputTypeDef",
     {
-        "accountSettings": AccountSettingsTypeDef,
+        "accountSettings": AccountSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelEnvironmentDeploymentOutputTypeDef = TypedDict(
-    "CancelEnvironmentDeploymentOutputTypeDef",
+CancelEnvironmentDeploymentOutputOutputTypeDef = TypedDict(
+    "CancelEnvironmentDeploymentOutputOutputTypeDef",
     {
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentOutputTypeDef = TypedDict(
-    "CreateEnvironmentOutputTypeDef",
+CreateEnvironmentOutputOutputTypeDef = TypedDict(
+    "CreateEnvironmentOutputOutputTypeDef",
     {
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentOutputTypeDef = TypedDict(
-    "DeleteEnvironmentOutputTypeDef",
+DeleteEnvironmentOutputOutputTypeDef = TypedDict(
+    "DeleteEnvironmentOutputOutputTypeDef",
     {
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentOutputTypeDef = TypedDict(
-    "GetEnvironmentOutputTypeDef",
+GetEnvironmentOutputOutputTypeDef = TypedDict(
+    "GetEnvironmentOutputOutputTypeDef",
     {
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentOutputTypeDef = TypedDict(
-    "UpdateEnvironmentOutputTypeDef",
+UpdateEnvironmentOutputOutputTypeDef = TypedDict(
+    "UpdateEnvironmentOutputOutputTypeDef",
     {
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceOutputTypeDef = TypedDict(
-    "CreateServiceOutputTypeDef",
+CreateServiceOutputOutputTypeDef = TypedDict(
+    "CreateServiceOutputOutputTypeDef",
     {
-        "service": ServiceTypeDef,
+        "service": ServiceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceOutputTypeDef = TypedDict(
-    "DeleteServiceOutputTypeDef",
+DeleteServiceOutputOutputTypeDef = TypedDict(
+    "DeleteServiceOutputOutputTypeDef",
     {
-        "service": ServiceTypeDef,
+        "service": ServiceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceOutputTypeDef = TypedDict(
-    "GetServiceOutputTypeDef",
+GetServiceOutputOutputTypeDef = TypedDict(
+    "GetServiceOutputOutputTypeDef",
     {
-        "service": ServiceTypeDef,
+        "service": ServiceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceOutputTypeDef = TypedDict(
-    "UpdateServiceOutputTypeDef",
+UpdateServiceOutputOutputTypeDef = TypedDict(
+    "UpdateServiceOutputOutputTypeDef",
     {
-        "service": ServiceTypeDef,
+        "service": ServiceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceTemplateVersionOutputTypeDef = TypedDict(
-    "CreateServiceTemplateVersionOutputTypeDef",
+CreateServiceTemplateVersionOutputOutputTypeDef = TypedDict(
+    "CreateServiceTemplateVersionOutputOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceTemplateVersionOutputTypeDef = TypedDict(
-    "DeleteServiceTemplateVersionOutputTypeDef",
+DeleteServiceTemplateVersionOutputOutputTypeDef = TypedDict(
+    "DeleteServiceTemplateVersionOutputOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceTemplateVersionOutputTypeDef = TypedDict(
-    "GetServiceTemplateVersionOutputTypeDef",
+GetServiceTemplateVersionOutputOutputTypeDef = TypedDict(
+    "GetServiceTemplateVersionOutputOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceTemplateVersionOutputTypeDef = TypedDict(
-    "UpdateServiceTemplateVersionOutputTypeDef",
+UpdateServiceTemplateVersionOutputOutputTypeDef = TypedDict(
+    "UpdateServiceTemplateVersionOutputOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetResourcesSummaryOutputTypeDef = TypedDict(
-    "GetResourcesSummaryOutputTypeDef",
+GetResourcesSummaryOutputOutputTypeDef = TypedDict(
+    "GetResourcesSummaryOutputOutputTypeDef",
     {
-        "counts": CountsSummaryTypeDef,
+        "counts": CountsSummaryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeploymentTypeDef = TypedDict(
-    "DeploymentTypeDef",
+DeploymentOutputTypeDef = TypedDict(
+    "DeploymentOutputTypeDef",
     {
         "arn": str,
         "completedAt": datetime,
         "componentName": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "id": str,
-        "initialState": DeploymentStateTypeDef,
+        "initialState": DeploymentStateOutputTypeDef,
         "lastAttemptedDeploymentId": str,
         "lastModifiedAt": datetime,
         "lastSucceededDeploymentId": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "targetArn": str,
         "targetResourceCreatedAt": datetime,
         "targetResourceType": DeploymentTargetResourceTypeType,
-        "targetState": DeploymentStateTypeDef,
+        "targetState": DeploymentStateOutputTypeDef,
     },
 )
 
-GetRepositorySyncStatusOutputTypeDef = TypedDict(
-    "GetRepositorySyncStatusOutputTypeDef",
+GetRepositorySyncStatusOutputOutputTypeDef = TypedDict(
+    "GetRepositorySyncStatusOutputOutputTypeDef",
     {
-        "latestSync": RepositorySyncAttemptTypeDef,
+        "latestSync": RepositorySyncAttemptOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceInstanceSyncStatusOutputTypeDef = TypedDict(
-    "GetServiceInstanceSyncStatusOutputTypeDef",
+GetServiceInstanceSyncStatusOutputOutputTypeDef = TypedDict(
+    "GetServiceInstanceSyncStatusOutputOutputTypeDef",
     {
-        "desiredState": RevisionTypeDef,
-        "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
-        "latestSync": ResourceSyncAttemptTypeDef,
+        "desiredState": RevisionOutputTypeDef,
+        "latestSuccessfulSync": ResourceSyncAttemptOutputTypeDef,
+        "latestSync": ResourceSyncAttemptOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetTemplateSyncStatusOutputTypeDef = TypedDict(
-    "GetTemplateSyncStatusOutputTypeDef",
+GetTemplateSyncStatusOutputOutputTypeDef = TypedDict(
+    "GetTemplateSyncStatusOutputOutputTypeDef",
     {
-        "desiredState": RevisionTypeDef,
-        "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
-        "latestSync": ResourceSyncAttemptTypeDef,
+        "desiredState": RevisionOutputTypeDef,
+        "latestSuccessfulSync": ResourceSyncAttemptOutputTypeDef,
+        "latestSync": ResourceSyncAttemptOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef",
     {
@@ -3634,49 +3653,49 @@
 class CreateServiceTemplateVersionInputRequestTypeDef(
     _RequiredCreateServiceTemplateVersionInputRequestTypeDef,
     _OptionalCreateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
 
-ServiceSyncBlockerSummaryTypeDef = TypedDict(
-    "ServiceSyncBlockerSummaryTypeDef",
+ServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
+    "ServiceSyncBlockerSummaryOutputTypeDef",
     {
-        "latestBlockers": List[SyncBlockerTypeDef],
+        "latestBlockers": List[SyncBlockerOutputTypeDef],
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-UpdateServiceSyncBlockerOutputTypeDef = TypedDict(
-    "UpdateServiceSyncBlockerOutputTypeDef",
+UpdateServiceSyncBlockerOutputOutputTypeDef = TypedDict(
+    "UpdateServiceSyncBlockerOutputOutputTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
-        "serviceSyncBlocker": SyncBlockerTypeDef,
+        "serviceSyncBlocker": SyncBlockerOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteDeploymentOutputTypeDef = TypedDict(
-    "DeleteDeploymentOutputTypeDef",
+DeleteDeploymentOutputOutputTypeDef = TypedDict(
+    "DeleteDeploymentOutputOutputTypeDef",
     {
-        "deployment": DeploymentTypeDef,
+        "deployment": DeploymentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetDeploymentOutputTypeDef = TypedDict(
-    "GetDeploymentOutputTypeDef",
+GetDeploymentOutputOutputTypeDef = TypedDict(
+    "GetDeploymentOutputOutputTypeDef",
     {
-        "deployment": DeploymentTypeDef,
+        "deployment": DeploymentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
-    "GetServiceSyncBlockerSummaryOutputTypeDef",
+GetServiceSyncBlockerSummaryOutputOutputTypeDef = TypedDict(
+    "GetServiceSyncBlockerSummaryOutputOutputTypeDef",
     {
-        "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryTypeDef,
+        "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/type_defs.pyi` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,84 +44,84 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
-    "EnvironmentAccountConnectionTypeDef",
-    "RepositoryBranchTypeDef",
+    "EnvironmentAccountConnectionOutputTypeDef",
+    "RepositoryBranchOutputTypeDef",
     "CancelComponentDeploymentInputRequestTypeDef",
-    "ComponentTypeDef",
+    "ComponentOutputTypeDef",
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
-    "ServiceInstanceTypeDef",
+    "ServiceInstanceOutputTypeDef",
     "CancelServicePipelineDeploymentInputRequestTypeDef",
-    "ServicePipelineTypeDef",
+    "ServicePipelineOutputTypeDef",
     "CompatibleEnvironmentTemplateInputTypeDef",
-    "CompatibleEnvironmentTemplateTypeDef",
-    "ComponentStateTypeDef",
-    "ComponentSummaryTypeDef",
-    "ResourceCountsSummaryTypeDef",
+    "CompatibleEnvironmentTemplateOutputTypeDef",
+    "ComponentStateOutputTypeDef",
+    "ComponentSummaryOutputTypeDef",
+    "ResourceCountsSummaryOutputTypeDef",
     "TagTypeDef",
     "RepositoryBranchInputTypeDef",
-    "EnvironmentTemplateTypeDef",
-    "EnvironmentTemplateVersionTypeDef",
-    "RepositoryTypeDef",
+    "EnvironmentTemplateOutputTypeDef",
+    "EnvironmentTemplateVersionOutputTypeDef",
+    "RepositoryOutputTypeDef",
     "CreateServiceSyncConfigInputRequestTypeDef",
-    "ServiceSyncConfigTypeDef",
-    "ServiceTemplateTypeDef",
+    "ServiceSyncConfigOutputTypeDef",
+    "ServiceTemplateOutputTypeDef",
     "CreateTemplateSyncConfigInputRequestTypeDef",
-    "TemplateSyncConfigTypeDef",
+    "TemplateSyncConfigOutputTypeDef",
     "DeleteComponentInputRequestTypeDef",
     "DeleteDeploymentInputRequestTypeDef",
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DeleteEnvironmentTemplateInputRequestTypeDef",
     "DeleteEnvironmentTemplateVersionInputRequestTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
     "DeleteServiceInputRequestTypeDef",
     "DeleteServiceSyncConfigInputRequestTypeDef",
     "DeleteServiceTemplateInputRequestTypeDef",
     "DeleteServiceTemplateVersionInputRequestTypeDef",
     "DeleteTemplateSyncConfigInputRequestTypeDef",
-    "EnvironmentStateTypeDef",
-    "ServiceInstanceStateTypeDef",
-    "ServicePipelineStateTypeDef",
-    "DeploymentSummaryTypeDef",
-    "EnvironmentAccountConnectionSummaryTypeDef",
-    "EnvironmentSummaryTypeDef",
+    "EnvironmentStateOutputTypeDef",
+    "ServiceInstanceStateOutputTypeDef",
+    "ServicePipelineStateOutputTypeDef",
+    "DeploymentSummaryOutputTypeDef",
+    "EnvironmentAccountConnectionSummaryOutputTypeDef",
+    "EnvironmentSummaryOutputTypeDef",
     "EnvironmentTemplateFilterTypeDef",
-    "EnvironmentTemplateSummaryTypeDef",
-    "EnvironmentTemplateVersionSummaryTypeDef",
+    "EnvironmentTemplateSummaryOutputTypeDef",
+    "EnvironmentTemplateVersionSummaryOutputTypeDef",
     "WaiterConfigTypeDef",
     "GetComponentInputRequestTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "GetEnvironmentTemplateInputRequestTypeDef",
     "GetEnvironmentTemplateVersionInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositorySyncStatusInputRequestTypeDef",
     "GetServiceInputRequestTypeDef",
     "GetServiceInstanceInputRequestTypeDef",
     "GetServiceInstanceSyncStatusInputRequestTypeDef",
-    "RevisionTypeDef",
+    "RevisionOutputTypeDef",
     "GetServiceSyncBlockerSummaryInputRequestTypeDef",
     "GetServiceSyncConfigInputRequestTypeDef",
     "GetServiceTemplateInputRequestTypeDef",
     "GetServiceTemplateVersionInputRequestTypeDef",
     "GetTemplateSyncConfigInputRequestTypeDef",
     "GetTemplateSyncStatusInputRequestTypeDef",
     "ListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     "ListComponentOutputsInputRequestTypeDef",
-    "OutputTypeDef",
+    "OutputOutputTypeDef",
     "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     "ListComponentProvisionedResourcesInputRequestTypeDef",
-    "ProvisionedResourceTypeDef",
+    "ProvisionedResourceOutputTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
     "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     "ListEnvironmentAccountConnectionsInputRequestTypeDef",
     "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
@@ -130,194 +130,196 @@
     "ListEnvironmentProvisionedResourcesInputRequestTypeDef",
     "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
     "ListEnvironmentTemplateVersionsInputRequestTypeDef",
     "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
     "ListEnvironmentTemplatesInputRequestTypeDef",
     "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
-    "RepositorySummaryTypeDef",
+    "RepositorySummaryOutputTypeDef",
     "ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
     "ListRepositorySyncDefinitionsInputRequestTypeDef",
-    "RepositorySyncDefinitionTypeDef",
+    "RepositorySyncDefinitionOutputTypeDef",
     "ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
     "ListServiceInstanceOutputsInputRequestTypeDef",
     "ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
     "ListServiceInstanceProvisionedResourcesInputRequestTypeDef",
     "ListServiceInstancesFilterTypeDef",
-    "ServiceInstanceSummaryTypeDef",
+    "ServiceInstanceSummaryOutputTypeDef",
     "ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     "ListServicePipelineOutputsInputRequestTypeDef",
     "ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
     "ListServicePipelineProvisionedResourcesInputRequestTypeDef",
     "ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
     "ListServiceTemplateVersionsInputRequestTypeDef",
-    "ServiceTemplateVersionSummaryTypeDef",
+    "ServiceTemplateVersionSummaryOutputTypeDef",
     "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
     "ListServiceTemplatesInputRequestTypeDef",
-    "ServiceTemplateSummaryTypeDef",
+    "ServiceTemplateSummaryOutputTypeDef",
     "ListServicesInputListServicesPaginateTypeDef",
     "ListServicesInputRequestTypeDef",
-    "ServiceSummaryTypeDef",
+    "ServiceSummaryOutputTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "TagOutputTypeDef",
+    "OutputTypeDef",
     "PaginatorConfigTypeDef",
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
-    "RepositorySyncEventTypeDef",
-    "ResourceSyncEventTypeDef",
+    "RepositorySyncEventOutputTypeDef",
+    "ResourceSyncEventOutputTypeDef",
     "ResponseMetadataTypeDef",
     "S3ObjectSourceTypeDef",
-    "SyncBlockerContextTypeDef",
+    "SyncBlockerContextOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateComponentInputRequestTypeDef",
     "UpdateEnvironmentAccountConnectionInputRequestTypeDef",
     "UpdateEnvironmentTemplateInputRequestTypeDef",
     "UpdateEnvironmentTemplateVersionInputRequestTypeDef",
     "UpdateServiceInputRequestTypeDef",
     "UpdateServiceInstanceInputRequestTypeDef",
     "UpdateServicePipelineInputRequestTypeDef",
     "UpdateServiceSyncBlockerInputRequestTypeDef",
     "UpdateServiceSyncConfigInputRequestTypeDef",
     "UpdateServiceTemplateInputRequestTypeDef",
     "UpdateTemplateSyncConfigInputRequestTypeDef",
-    "AcceptEnvironmentAccountConnectionOutputTypeDef",
-    "CreateEnvironmentAccountConnectionOutputTypeDef",
-    "DeleteEnvironmentAccountConnectionOutputTypeDef",
-    "GetEnvironmentAccountConnectionOutputTypeDef",
-    "RejectEnvironmentAccountConnectionOutputTypeDef",
-    "UpdateEnvironmentAccountConnectionOutputTypeDef",
-    "AccountSettingsTypeDef",
-    "EnvironmentTypeDef",
-    "CancelComponentDeploymentOutputTypeDef",
-    "CreateComponentOutputTypeDef",
-    "DeleteComponentOutputTypeDef",
-    "GetComponentOutputTypeDef",
-    "UpdateComponentOutputTypeDef",
-    "CancelServiceInstanceDeploymentOutputTypeDef",
-    "CreateServiceInstanceOutputTypeDef",
-    "GetServiceInstanceOutputTypeDef",
-    "UpdateServiceInstanceOutputTypeDef",
-    "CancelServicePipelineDeploymentOutputTypeDef",
-    "ServiceTypeDef",
-    "UpdateServicePipelineOutputTypeDef",
+    "AcceptEnvironmentAccountConnectionOutputOutputTypeDef",
+    "CreateEnvironmentAccountConnectionOutputOutputTypeDef",
+    "DeleteEnvironmentAccountConnectionOutputOutputTypeDef",
+    "GetEnvironmentAccountConnectionOutputOutputTypeDef",
+    "RejectEnvironmentAccountConnectionOutputOutputTypeDef",
+    "UpdateEnvironmentAccountConnectionOutputOutputTypeDef",
+    "AccountSettingsOutputTypeDef",
+    "EnvironmentOutputTypeDef",
+    "CancelComponentDeploymentOutputOutputTypeDef",
+    "CreateComponentOutputOutputTypeDef",
+    "DeleteComponentOutputOutputTypeDef",
+    "GetComponentOutputOutputTypeDef",
+    "UpdateComponentOutputOutputTypeDef",
+    "CancelServiceInstanceDeploymentOutputOutputTypeDef",
+    "CreateServiceInstanceOutputOutputTypeDef",
+    "GetServiceInstanceOutputOutputTypeDef",
+    "UpdateServiceInstanceOutputOutputTypeDef",
+    "CancelServicePipelineDeploymentOutputOutputTypeDef",
+    "ServiceOutputTypeDef",
+    "UpdateServicePipelineOutputOutputTypeDef",
     "UpdateServiceTemplateVersionInputRequestTypeDef",
-    "ServiceTemplateVersionTypeDef",
-    "ListComponentsOutputTypeDef",
-    "CountsSummaryTypeDef",
+    "ServiceTemplateVersionOutputTypeDef",
+    "ListComponentsOutputOutputTypeDef",
+    "CountsSummaryOutputTypeDef",
     "CreateComponentInputRequestTypeDef",
     "CreateEnvironmentAccountConnectionInputRequestTypeDef",
     "CreateEnvironmentTemplateInputRequestTypeDef",
     "CreateRepositoryInputRequestTypeDef",
     "CreateServiceInputRequestTypeDef",
     "CreateServiceInstanceInputRequestTypeDef",
     "CreateServiceTemplateInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
-    "CreateEnvironmentTemplateOutputTypeDef",
-    "DeleteEnvironmentTemplateOutputTypeDef",
-    "GetEnvironmentTemplateOutputTypeDef",
-    "UpdateEnvironmentTemplateOutputTypeDef",
-    "CreateEnvironmentTemplateVersionOutputTypeDef",
-    "DeleteEnvironmentTemplateVersionOutputTypeDef",
-    "GetEnvironmentTemplateVersionOutputTypeDef",
-    "UpdateEnvironmentTemplateVersionOutputTypeDef",
-    "CreateRepositoryOutputTypeDef",
-    "DeleteRepositoryOutputTypeDef",
-    "GetRepositoryOutputTypeDef",
-    "CreateServiceSyncConfigOutputTypeDef",
-    "DeleteServiceSyncConfigOutputTypeDef",
-    "GetServiceSyncConfigOutputTypeDef",
-    "UpdateServiceSyncConfigOutputTypeDef",
-    "CreateServiceTemplateOutputTypeDef",
-    "DeleteServiceTemplateOutputTypeDef",
-    "GetServiceTemplateOutputTypeDef",
-    "UpdateServiceTemplateOutputTypeDef",
-    "CreateTemplateSyncConfigOutputTypeDef",
-    "DeleteTemplateSyncConfigOutputTypeDef",
-    "GetTemplateSyncConfigOutputTypeDef",
-    "UpdateTemplateSyncConfigOutputTypeDef",
-    "DeploymentStateTypeDef",
-    "ListDeploymentsOutputTypeDef",
-    "ListEnvironmentAccountConnectionsOutputTypeDef",
-    "ListEnvironmentsOutputTypeDef",
+    "CreateEnvironmentTemplateOutputOutputTypeDef",
+    "DeleteEnvironmentTemplateOutputOutputTypeDef",
+    "GetEnvironmentTemplateOutputOutputTypeDef",
+    "UpdateEnvironmentTemplateOutputOutputTypeDef",
+    "CreateEnvironmentTemplateVersionOutputOutputTypeDef",
+    "DeleteEnvironmentTemplateVersionOutputOutputTypeDef",
+    "GetEnvironmentTemplateVersionOutputOutputTypeDef",
+    "UpdateEnvironmentTemplateVersionOutputOutputTypeDef",
+    "CreateRepositoryOutputOutputTypeDef",
+    "DeleteRepositoryOutputOutputTypeDef",
+    "GetRepositoryOutputOutputTypeDef",
+    "CreateServiceSyncConfigOutputOutputTypeDef",
+    "DeleteServiceSyncConfigOutputOutputTypeDef",
+    "GetServiceSyncConfigOutputOutputTypeDef",
+    "UpdateServiceSyncConfigOutputOutputTypeDef",
+    "CreateServiceTemplateOutputOutputTypeDef",
+    "DeleteServiceTemplateOutputOutputTypeDef",
+    "GetServiceTemplateOutputOutputTypeDef",
+    "UpdateServiceTemplateOutputOutputTypeDef",
+    "CreateTemplateSyncConfigOutputOutputTypeDef",
+    "DeleteTemplateSyncConfigOutputOutputTypeDef",
+    "GetTemplateSyncConfigOutputOutputTypeDef",
+    "UpdateTemplateSyncConfigOutputOutputTypeDef",
+    "DeploymentStateOutputTypeDef",
+    "ListDeploymentsOutputOutputTypeDef",
+    "ListEnvironmentAccountConnectionsOutputOutputTypeDef",
+    "ListEnvironmentsOutputOutputTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
-    "ListEnvironmentTemplatesOutputTypeDef",
-    "ListEnvironmentTemplateVersionsOutputTypeDef",
+    "ListEnvironmentTemplatesOutputOutputTypeDef",
+    "ListEnvironmentTemplateVersionsOutputOutputTypeDef",
     "GetComponentInputComponentDeletedWaitTypeDef",
     "GetComponentInputComponentDeployedWaitTypeDef",
     "GetEnvironmentInputEnvironmentDeployedWaitTypeDef",
     "GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef",
     "GetServiceInputServiceCreatedWaitTypeDef",
     "GetServiceInputServiceDeletedWaitTypeDef",
     "GetServiceInputServicePipelineDeployedWaitTypeDef",
     "GetServiceInputServiceUpdatedWaitTypeDef",
     "GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     "GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
-    "ListComponentOutputsOutputTypeDef",
-    "ListEnvironmentOutputsOutputTypeDef",
-    "ListServiceInstanceOutputsOutputTypeDef",
-    "ListServicePipelineOutputsOutputTypeDef",
-    "NotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    "ListComponentProvisionedResourcesOutputTypeDef",
-    "ListEnvironmentProvisionedResourcesOutputTypeDef",
-    "ListServiceInstanceProvisionedResourcesOutputTypeDef",
-    "ListServicePipelineProvisionedResourcesOutputTypeDef",
-    "ListRepositoriesOutputTypeDef",
-    "ListRepositorySyncDefinitionsOutputTypeDef",
+    "ListComponentOutputsOutputOutputTypeDef",
+    "ListEnvironmentOutputsOutputOutputTypeDef",
+    "ListServiceInstanceOutputsOutputOutputTypeDef",
+    "ListServicePipelineOutputsOutputOutputTypeDef",
+    "ListComponentProvisionedResourcesOutputOutputTypeDef",
+    "ListEnvironmentProvisionedResourcesOutputOutputTypeDef",
+    "ListServiceInstanceProvisionedResourcesOutputOutputTypeDef",
+    "ListServicePipelineProvisionedResourcesOutputOutputTypeDef",
+    "ListRepositoriesOutputOutputTypeDef",
+    "ListRepositorySyncDefinitionsOutputOutputTypeDef",
     "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
     "ListServiceInstancesInputRequestTypeDef",
-    "ListServiceInstancesOutputTypeDef",
-    "ListServiceTemplateVersionsOutputTypeDef",
-    "ListServiceTemplatesOutputTypeDef",
-    "ListServicesOutputTypeDef",
-    "RepositorySyncAttemptTypeDef",
-    "ResourceSyncAttemptTypeDef",
+    "ListServiceInstancesOutputOutputTypeDef",
+    "ListServiceTemplateVersionsOutputOutputTypeDef",
+    "ListServiceTemplatesOutputOutputTypeDef",
+    "ListServicesOutputOutputTypeDef",
+    "ListTagsForResourceOutputOutputTypeDef",
+    "NotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    "RepositorySyncAttemptOutputTypeDef",
+    "ResourceSyncAttemptOutputTypeDef",
     "TemplateVersionSourceInputTypeDef",
-    "SyncBlockerTypeDef",
-    "GetAccountSettingsOutputTypeDef",
-    "UpdateAccountSettingsOutputTypeDef",
-    "CancelEnvironmentDeploymentOutputTypeDef",
-    "CreateEnvironmentOutputTypeDef",
-    "DeleteEnvironmentOutputTypeDef",
-    "GetEnvironmentOutputTypeDef",
-    "UpdateEnvironmentOutputTypeDef",
-    "CreateServiceOutputTypeDef",
-    "DeleteServiceOutputTypeDef",
-    "GetServiceOutputTypeDef",
-    "UpdateServiceOutputTypeDef",
-    "CreateServiceTemplateVersionOutputTypeDef",
-    "DeleteServiceTemplateVersionOutputTypeDef",
-    "GetServiceTemplateVersionOutputTypeDef",
-    "UpdateServiceTemplateVersionOutputTypeDef",
-    "GetResourcesSummaryOutputTypeDef",
-    "DeploymentTypeDef",
-    "GetRepositorySyncStatusOutputTypeDef",
-    "GetServiceInstanceSyncStatusOutputTypeDef",
-    "GetTemplateSyncStatusOutputTypeDef",
+    "SyncBlockerOutputTypeDef",
+    "GetAccountSettingsOutputOutputTypeDef",
+    "UpdateAccountSettingsOutputOutputTypeDef",
+    "CancelEnvironmentDeploymentOutputOutputTypeDef",
+    "CreateEnvironmentOutputOutputTypeDef",
+    "DeleteEnvironmentOutputOutputTypeDef",
+    "GetEnvironmentOutputOutputTypeDef",
+    "UpdateEnvironmentOutputOutputTypeDef",
+    "CreateServiceOutputOutputTypeDef",
+    "DeleteServiceOutputOutputTypeDef",
+    "GetServiceOutputOutputTypeDef",
+    "UpdateServiceOutputOutputTypeDef",
+    "CreateServiceTemplateVersionOutputOutputTypeDef",
+    "DeleteServiceTemplateVersionOutputOutputTypeDef",
+    "GetServiceTemplateVersionOutputOutputTypeDef",
+    "UpdateServiceTemplateVersionOutputOutputTypeDef",
+    "GetResourcesSummaryOutputOutputTypeDef",
+    "DeploymentOutputTypeDef",
+    "GetRepositorySyncStatusOutputOutputTypeDef",
+    "GetServiceInstanceSyncStatusOutputOutputTypeDef",
+    "GetTemplateSyncStatusOutputOutputTypeDef",
     "CreateEnvironmentTemplateVersionInputRequestTypeDef",
     "CreateServiceTemplateVersionInputRequestTypeDef",
-    "ServiceSyncBlockerSummaryTypeDef",
-    "UpdateServiceSyncBlockerOutputTypeDef",
-    "DeleteDeploymentOutputTypeDef",
-    "GetDeploymentOutputTypeDef",
-    "GetServiceSyncBlockerSummaryOutputTypeDef",
+    "ServiceSyncBlockerSummaryOutputTypeDef",
+    "UpdateServiceSyncBlockerOutputOutputTypeDef",
+    "DeleteDeploymentOutputOutputTypeDef",
+    "GetDeploymentOutputOutputTypeDef",
+    "GetServiceSyncBlockerSummaryOutputOutputTypeDef",
 )
 
 AcceptEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-EnvironmentAccountConnectionTypeDef = TypedDict(
-    "EnvironmentAccountConnectionTypeDef",
+EnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "EnvironmentAccountConnectionOutputTypeDef",
     {
         "arn": str,
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
@@ -325,16 +327,16 @@
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
 
-RepositoryBranchTypeDef = TypedDict(
-    "RepositoryBranchTypeDef",
+RepositoryBranchOutputTypeDef = TypedDict(
+    "RepositoryBranchOutputTypeDef",
     {
         "arn": str,
         "branch": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
@@ -342,16 +344,16 @@
 CancelComponentDeploymentInputRequestTypeDef = TypedDict(
     "CancelComponentDeploymentInputRequestTypeDef",
     {
         "componentName": str,
     },
 )
 
-ComponentTypeDef = TypedDict(
-    "ComponentTypeDef",
+ComponentOutputTypeDef = TypedDict(
+    "ComponentOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentName": str,
@@ -379,16 +381,16 @@
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-ServiceInstanceTypeDef = TypedDict(
-    "ServiceInstanceTypeDef",
+ServiceInstanceOutputTypeDef = TypedDict(
+    "ServiceInstanceOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -408,16 +410,16 @@
 CancelServicePipelineDeploymentInputRequestTypeDef = TypedDict(
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
-ServicePipelineTypeDef = TypedDict(
-    "ServicePipelineTypeDef",
+ServicePipelineOutputTypeDef = TypedDict(
+    "ServicePipelineOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
@@ -434,34 +436,34 @@
     "CompatibleEnvironmentTemplateInputTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-CompatibleEnvironmentTemplateTypeDef = TypedDict(
-    "CompatibleEnvironmentTemplateTypeDef",
+CompatibleEnvironmentTemplateOutputTypeDef = TypedDict(
+    "CompatibleEnvironmentTemplateOutputTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-ComponentStateTypeDef = TypedDict(
-    "ComponentStateTypeDef",
+ComponentStateOutputTypeDef = TypedDict(
+    "ComponentStateOutputTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
         "templateFile": str,
     },
 )
 
-ComponentSummaryTypeDef = TypedDict(
-    "ComponentSummaryTypeDef",
+ComponentSummaryOutputTypeDef = TypedDict(
+    "ComponentSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -471,16 +473,16 @@
         "lastSucceededDeploymentId": str,
         "name": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-ResourceCountsSummaryTypeDef = TypedDict(
-    "ResourceCountsSummaryTypeDef",
+ResourceCountsSummaryOutputTypeDef = TypedDict(
+    "ResourceCountsSummaryOutputTypeDef",
     {
         "behindMajor": int,
         "behindMinor": int,
         "failed": int,
         "total": int,
         "upToDate": int,
     },
@@ -499,31 +501,31 @@
     {
         "branch": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
 
-EnvironmentTemplateTypeDef = TypedDict(
-    "EnvironmentTemplateTypeDef",
+EnvironmentTemplateOutputTypeDef = TypedDict(
+    "EnvironmentTemplateOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "encryptionKey": str,
         "lastModifiedAt": datetime,
         "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
 )
 
-EnvironmentTemplateVersionTypeDef = TypedDict(
-    "EnvironmentTemplateVersionTypeDef",
+EnvironmentTemplateVersionOutputTypeDef = TypedDict(
+    "EnvironmentTemplateVersionOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -531,16 +533,16 @@
         "schema": str,
         "status": TemplateVersionStatusType,
         "statusMessage": str,
         "templateName": str,
     },
 )
 
-RepositoryTypeDef = TypedDict(
-    "RepositoryTypeDef",
+RepositoryOutputTypeDef = TypedDict(
+    "RepositoryOutputTypeDef",
     {
         "arn": str,
         "connectionArn": str,
         "encryptionKey": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
@@ -553,27 +555,27 @@
         "filePath": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "serviceName": str,
     },
 )
 
-ServiceSyncConfigTypeDef = TypedDict(
-    "ServiceSyncConfigTypeDef",
+ServiceSyncConfigOutputTypeDef = TypedDict(
+    "ServiceSyncConfigOutputTypeDef",
     {
         "branch": str,
         "filePath": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "serviceName": str,
     },
 )
 
-ServiceTemplateTypeDef = TypedDict(
-    "ServiceTemplateTypeDef",
+ServiceTemplateOutputTypeDef = TypedDict(
+    "ServiceTemplateOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "encryptionKey": str,
         "lastModifiedAt": datetime,
@@ -603,16 +605,16 @@
 
 class CreateTemplateSyncConfigInputRequestTypeDef(
     _RequiredCreateTemplateSyncConfigInputRequestTypeDef,
     _OptionalCreateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
-TemplateSyncConfigTypeDef = TypedDict(
-    "TemplateSyncConfigTypeDef",
+TemplateSyncConfigOutputTypeDef = TypedDict(
+    "TemplateSyncConfigOutputTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "subdirectory": str,
         "templateName": str,
         "templateType": TemplateTypeType,
@@ -705,49 +707,49 @@
     "DeleteTemplateSyncConfigInputRequestTypeDef",
     {
         "templateName": str,
         "templateType": TemplateTypeType,
     },
 )
 
-EnvironmentStateTypeDef = TypedDict(
-    "EnvironmentStateTypeDef",
+EnvironmentStateOutputTypeDef = TypedDict(
+    "EnvironmentStateOutputTypeDef",
     {
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-ServiceInstanceStateTypeDef = TypedDict(
-    "ServiceInstanceStateTypeDef",
+ServiceInstanceStateOutputTypeDef = TypedDict(
+    "ServiceInstanceStateOutputTypeDef",
     {
         "lastSuccessfulComponentDeploymentIds": List[str],
         "lastSuccessfulEnvironmentDeploymentId": str,
         "lastSuccessfulServicePipelineDeploymentId": str,
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-ServicePipelineStateTypeDef = TypedDict(
-    "ServicePipelineStateTypeDef",
+ServicePipelineStateOutputTypeDef = TypedDict(
+    "ServicePipelineStateOutputTypeDef",
     {
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-DeploymentSummaryTypeDef = TypedDict(
-    "DeploymentSummaryTypeDef",
+DeploymentSummaryOutputTypeDef = TypedDict(
+    "DeploymentSummaryOutputTypeDef",
     {
         "arn": str,
         "completedAt": datetime,
         "componentName": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "environmentName": str,
@@ -759,32 +761,32 @@
         "serviceName": str,
         "targetArn": str,
         "targetResourceCreatedAt": datetime,
         "targetResourceType": DeploymentTargetResourceTypeType,
     },
 )
 
-EnvironmentAccountConnectionSummaryTypeDef = TypedDict(
-    "EnvironmentAccountConnectionSummaryTypeDef",
+EnvironmentAccountConnectionSummaryOutputTypeDef = TypedDict(
+    "EnvironmentAccountConnectionSummaryOutputTypeDef",
     {
         "arn": str,
         "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
         "lastModifiedAt": datetime,
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
 
-EnvironmentSummaryTypeDef = TypedDict(
-    "EnvironmentSummaryTypeDef",
+EnvironmentSummaryOutputTypeDef = TypedDict(
+    "EnvironmentSummaryOutputTypeDef",
     {
         "arn": str,
         "componentRoleArn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "description": str,
@@ -807,30 +809,30 @@
     "EnvironmentTemplateFilterTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-EnvironmentTemplateSummaryTypeDef = TypedDict(
-    "EnvironmentTemplateSummaryTypeDef",
+EnvironmentTemplateSummaryOutputTypeDef = TypedDict(
+    "EnvironmentTemplateSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "lastModifiedAt": datetime,
         "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
 )
 
-EnvironmentTemplateVersionSummaryTypeDef = TypedDict(
-    "EnvironmentTemplateVersionSummaryTypeDef",
+EnvironmentTemplateVersionSummaryOutputTypeDef = TypedDict(
+    "EnvironmentTemplateVersionSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -946,16 +948,16 @@
     "GetServiceInstanceSyncStatusInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-RevisionTypeDef = TypedDict(
-    "RevisionTypeDef",
+RevisionOutputTypeDef = TypedDict(
+    "RevisionOutputTypeDef",
     {
         "branch": str,
         "directory": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "sha": str,
     },
@@ -1059,16 +1061,16 @@
 
 class ListComponentOutputsInputRequestTypeDef(
     _RequiredListComponentOutputsInputRequestTypeDef,
     _OptionalListComponentOutputsInputRequestTypeDef,
 ):
     pass
 
-OutputTypeDef = TypedDict(
-    "OutputTypeDef",
+OutputOutputTypeDef = TypedDict(
+    "OutputOutputTypeDef",
     {
         "key": str,
         "valueString": str,
     },
 )
 
 _RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
@@ -1107,16 +1109,16 @@
 
 class ListComponentProvisionedResourcesInputRequestTypeDef(
     _RequiredListComponentProvisionedResourcesInputRequestTypeDef,
     _OptionalListComponentProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
-ProvisionedResourceTypeDef = TypedDict(
-    "ProvisionedResourceTypeDef",
+ProvisionedResourceOutputTypeDef = TypedDict(
+    "ProvisionedResourceOutputTypeDef",
     {
         "identifier": str,
         "name": str,
         "provisioningEngine": ProvisionedResourceEngineType,
     },
 )
 
@@ -1368,16 +1370,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-RepositorySummaryTypeDef = TypedDict(
-    "RepositorySummaryTypeDef",
+RepositorySummaryOutputTypeDef = TypedDict(
+    "RepositorySummaryOutputTypeDef",
     {
         "arn": str,
         "connectionArn": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
@@ -1422,16 +1424,16 @@
 
 class ListRepositorySyncDefinitionsInputRequestTypeDef(
     _RequiredListRepositorySyncDefinitionsInputRequestTypeDef,
     _OptionalListRepositorySyncDefinitionsInputRequestTypeDef,
 ):
     pass
 
-RepositorySyncDefinitionTypeDef = TypedDict(
-    "RepositorySyncDefinitionTypeDef",
+RepositorySyncDefinitionOutputTypeDef = TypedDict(
+    "RepositorySyncDefinitionOutputTypeDef",
     {
         "branch": str,
         "directory": str,
         "parent": str,
         "target": str,
     },
 )
@@ -1527,16 +1529,16 @@
     {
         "key": ListServiceInstancesFilterByType,
         "value": str,
     },
     total=False,
 )
 
-ServiceInstanceSummaryTypeDef = TypedDict(
-    "ServiceInstanceSummaryTypeDef",
+ServiceInstanceSummaryOutputTypeDef = TypedDict(
+    "ServiceInstanceSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -1672,16 +1674,16 @@
 
 class ListServiceTemplateVersionsInputRequestTypeDef(
     _RequiredListServiceTemplateVersionsInputRequestTypeDef,
     _OptionalListServiceTemplateVersionsInputRequestTypeDef,
 ):
     pass
 
-ServiceTemplateVersionSummaryTypeDef = TypedDict(
-    "ServiceTemplateVersionSummaryTypeDef",
+ServiceTemplateVersionSummaryOutputTypeDef = TypedDict(
+    "ServiceTemplateVersionSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -1705,16 +1707,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ServiceTemplateSummaryTypeDef = TypedDict(
-    "ServiceTemplateSummaryTypeDef",
+ServiceTemplateSummaryOutputTypeDef = TypedDict(
+    "ServiceTemplateSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "lastModifiedAt": datetime,
         "name": str,
@@ -1736,16 +1738,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ServiceSummaryTypeDef = TypedDict(
-    "ServiceSummaryTypeDef",
+ServiceSummaryOutputTypeDef = TypedDict(
+    "ServiceSummaryOutputTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
@@ -1790,14 +1792,31 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+OutputTypeDef = TypedDict(
+    "OutputTypeDef",
+    {
+        "key": str,
+        "valueString": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1807,26 +1826,26 @@
 RejectEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-RepositorySyncEventTypeDef = TypedDict(
-    "RepositorySyncEventTypeDef",
+RepositorySyncEventOutputTypeDef = TypedDict(
+    "RepositorySyncEventOutputTypeDef",
     {
         "event": str,
         "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
 
-ResourceSyncEventTypeDef = TypedDict(
-    "ResourceSyncEventTypeDef",
+ResourceSyncEventOutputTypeDef = TypedDict(
+    "ResourceSyncEventOutputTypeDef",
     {
         "event": str,
         "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
@@ -1846,16 +1865,16 @@
     "S3ObjectSourceTypeDef",
     {
         "bucket": str,
         "key": str,
     },
 )
 
-SyncBlockerContextTypeDef = TypedDict(
-    "SyncBlockerContextTypeDef",
+SyncBlockerContextOutputTypeDef = TypedDict(
+    "SyncBlockerContextOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
 UntagResourceInputRequestTypeDef = TypedDict(
@@ -2085,73 +2104,73 @@
 
 class UpdateTemplateSyncConfigInputRequestTypeDef(
     _RequiredUpdateTemplateSyncConfigInputRequestTypeDef,
     _OptionalUpdateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
-AcceptEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "AcceptEnvironmentAccountConnectionOutputTypeDef",
+AcceptEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "AcceptEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "CreateEnvironmentAccountConnectionOutputTypeDef",
+CreateEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "CreateEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "DeleteEnvironmentAccountConnectionOutputTypeDef",
+DeleteEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "DeleteEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "GetEnvironmentAccountConnectionOutputTypeDef",
+GetEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "GetEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RejectEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "RejectEnvironmentAccountConnectionOutputTypeDef",
+RejectEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "RejectEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "UpdateEnvironmentAccountConnectionOutputTypeDef",
+UpdateEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
+    "UpdateEnvironmentAccountConnectionOutputOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AccountSettingsTypeDef = TypedDict(
-    "AccountSettingsTypeDef",
+AccountSettingsOutputTypeDef = TypedDict(
+    "AccountSettingsOutputTypeDef",
     {
         "pipelineCodebuildRoleArn": str,
-        "pipelineProvisioningRepository": RepositoryBranchTypeDef,
+        "pipelineProvisioningRepository": RepositoryBranchOutputTypeDef,
         "pipelineServiceRoleArn": str,
     },
 )
 
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
+EnvironmentOutputTypeDef = TypedDict(
+    "EnvironmentOutputTypeDef",
     {
         "arn": str,
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
@@ -2161,125 +2180,125 @@
         "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
         "lastSucceededDeploymentId": str,
         "name": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
-        "provisioningRepository": RepositoryBranchTypeDef,
+        "provisioningRepository": RepositoryBranchOutputTypeDef,
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-CancelComponentDeploymentOutputTypeDef = TypedDict(
-    "CancelComponentDeploymentOutputTypeDef",
+CancelComponentDeploymentOutputOutputTypeDef = TypedDict(
+    "CancelComponentDeploymentOutputOutputTypeDef",
     {
-        "component": ComponentTypeDef,
+        "component": ComponentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateComponentOutputTypeDef = TypedDict(
-    "CreateComponentOutputTypeDef",
+CreateComponentOutputOutputTypeDef = TypedDict(
+    "CreateComponentOutputOutputTypeDef",
     {
-        "component": ComponentTypeDef,
+        "component": ComponentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteComponentOutputTypeDef = TypedDict(
-    "DeleteComponentOutputTypeDef",
+DeleteComponentOutputOutputTypeDef = TypedDict(
+    "DeleteComponentOutputOutputTypeDef",
     {
-        "component": ComponentTypeDef,
+        "component": ComponentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetComponentOutputTypeDef = TypedDict(
-    "GetComponentOutputTypeDef",
+GetComponentOutputOutputTypeDef = TypedDict(
+    "GetComponentOutputOutputTypeDef",
     {
-        "component": ComponentTypeDef,
+        "component": ComponentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateComponentOutputTypeDef = TypedDict(
-    "UpdateComponentOutputTypeDef",
+UpdateComponentOutputOutputTypeDef = TypedDict(
+    "UpdateComponentOutputOutputTypeDef",
     {
-        "component": ComponentTypeDef,
+        "component": ComponentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelServiceInstanceDeploymentOutputTypeDef = TypedDict(
-    "CancelServiceInstanceDeploymentOutputTypeDef",
+CancelServiceInstanceDeploymentOutputOutputTypeDef = TypedDict(
+    "CancelServiceInstanceDeploymentOutputOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceTypeDef,
+        "serviceInstance": ServiceInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceInstanceOutputTypeDef = TypedDict(
-    "CreateServiceInstanceOutputTypeDef",
+CreateServiceInstanceOutputOutputTypeDef = TypedDict(
+    "CreateServiceInstanceOutputOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceTypeDef,
+        "serviceInstance": ServiceInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceInstanceOutputTypeDef = TypedDict(
-    "GetServiceInstanceOutputTypeDef",
+GetServiceInstanceOutputOutputTypeDef = TypedDict(
+    "GetServiceInstanceOutputOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceTypeDef,
+        "serviceInstance": ServiceInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceInstanceOutputTypeDef = TypedDict(
-    "UpdateServiceInstanceOutputTypeDef",
+UpdateServiceInstanceOutputOutputTypeDef = TypedDict(
+    "UpdateServiceInstanceOutputOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceTypeDef,
+        "serviceInstance": ServiceInstanceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelServicePipelineDeploymentOutputTypeDef = TypedDict(
-    "CancelServicePipelineDeploymentOutputTypeDef",
+CancelServicePipelineDeploymentOutputOutputTypeDef = TypedDict(
+    "CancelServicePipelineDeploymentOutputOutputTypeDef",
     {
-        "pipeline": ServicePipelineTypeDef,
+        "pipeline": ServicePipelineOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ServiceTypeDef = TypedDict(
-    "ServiceTypeDef",
+ServiceOutputTypeDef = TypedDict(
+    "ServiceOutputTypeDef",
     {
         "arn": str,
         "branchName": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "name": str,
-        "pipeline": ServicePipelineTypeDef,
+        "pipeline": ServicePipelineOutputTypeDef,
         "repositoryConnectionArn": str,
         "repositoryId": str,
         "spec": str,
         "status": ServiceStatusType,
         "statusMessage": str,
         "templateName": str,
     },
 )
 
-UpdateServicePipelineOutputTypeDef = TypedDict(
-    "UpdateServicePipelineOutputTypeDef",
+UpdateServicePipelineOutputOutputTypeDef = TypedDict(
+    "UpdateServicePipelineOutputOutputTypeDef",
     {
-        "pipeline": ServicePipelineTypeDef,
+        "pipeline": ServicePipelineOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateServiceTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceTemplateVersionInputRequestTypeDef",
     {
@@ -2301,52 +2320,52 @@
 
 class UpdateServiceTemplateVersionInputRequestTypeDef(
     _RequiredUpdateServiceTemplateVersionInputRequestTypeDef,
     _OptionalUpdateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
-ServiceTemplateVersionTypeDef = TypedDict(
-    "ServiceTemplateVersionTypeDef",
+ServiceTemplateVersionOutputTypeDef = TypedDict(
+    "ServiceTemplateVersionOutputTypeDef",
     {
         "arn": str,
-        "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateTypeDef],
+        "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateOutputTypeDef],
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
         "recommendedMinorVersion": str,
         "schema": str,
         "status": TemplateVersionStatusType,
         "statusMessage": str,
         "supportedComponentSources": List[Literal["DIRECTLY_DEFINED"]],
         "templateName": str,
     },
 )
 
-ListComponentsOutputTypeDef = TypedDict(
-    "ListComponentsOutputTypeDef",
+ListComponentsOutputOutputTypeDef = TypedDict(
+    "ListComponentsOutputOutputTypeDef",
     {
-        "components": List[ComponentSummaryTypeDef],
+        "components": List[ComponentSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CountsSummaryTypeDef = TypedDict(
-    "CountsSummaryTypeDef",
+CountsSummaryOutputTypeDef = TypedDict(
+    "CountsSummaryOutputTypeDef",
     {
-        "components": ResourceCountsSummaryTypeDef,
-        "environmentTemplates": ResourceCountsSummaryTypeDef,
-        "environments": ResourceCountsSummaryTypeDef,
-        "pipelines": ResourceCountsSummaryTypeDef,
-        "serviceInstances": ResourceCountsSummaryTypeDef,
-        "serviceTemplates": ResourceCountsSummaryTypeDef,
-        "services": ResourceCountsSummaryTypeDef,
+        "components": ResourceCountsSummaryOutputTypeDef,
+        "environmentTemplates": ResourceCountsSummaryOutputTypeDef,
+        "environments": ResourceCountsSummaryOutputTypeDef,
+        "pipelines": ResourceCountsSummaryOutputTypeDef,
+        "serviceInstances": ResourceCountsSummaryOutputTypeDef,
+        "serviceTemplates": ResourceCountsSummaryOutputTypeDef,
+        "services": ResourceCountsSummaryOutputTypeDef,
     },
 )
 
 _RequiredCreateComponentInputRequestTypeDef = TypedDict(
     "_RequiredCreateComponentInputRequestTypeDef",
     {
         "manifest": str,
@@ -2516,23 +2535,14 @@
 
 class CreateServiceTemplateInputRequestTypeDef(
     _RequiredCreateServiceTemplateInputRequestTypeDef,
     _OptionalCreateServiceTemplateInputRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "nextToken": str,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -2601,230 +2611,230 @@
 )
 
 class UpdateEnvironmentInputRequestTypeDef(
     _RequiredUpdateEnvironmentInputRequestTypeDef, _OptionalUpdateEnvironmentInputRequestTypeDef
 ):
     pass
 
-CreateEnvironmentTemplateOutputTypeDef = TypedDict(
-    "CreateEnvironmentTemplateOutputTypeDef",
+CreateEnvironmentTemplateOutputOutputTypeDef = TypedDict(
+    "CreateEnvironmentTemplateOutputOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateTypeDef,
+        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentTemplateOutputTypeDef = TypedDict(
-    "DeleteEnvironmentTemplateOutputTypeDef",
+DeleteEnvironmentTemplateOutputOutputTypeDef = TypedDict(
+    "DeleteEnvironmentTemplateOutputOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateTypeDef,
+        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentTemplateOutputTypeDef = TypedDict(
-    "GetEnvironmentTemplateOutputTypeDef",
+GetEnvironmentTemplateOutputOutputTypeDef = TypedDict(
+    "GetEnvironmentTemplateOutputOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateTypeDef,
+        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentTemplateOutputTypeDef = TypedDict(
-    "UpdateEnvironmentTemplateOutputTypeDef",
+UpdateEnvironmentTemplateOutputOutputTypeDef = TypedDict(
+    "UpdateEnvironmentTemplateOutputOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateTypeDef,
+        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
-    "CreateEnvironmentTemplateVersionOutputTypeDef",
+CreateEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
+    "CreateEnvironmentTemplateVersionOutputOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentTemplateVersionOutputTypeDef = TypedDict(
-    "DeleteEnvironmentTemplateVersionOutputTypeDef",
+DeleteEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
+    "DeleteEnvironmentTemplateVersionOutputOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentTemplateVersionOutputTypeDef = TypedDict(
-    "GetEnvironmentTemplateVersionOutputTypeDef",
+GetEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
+    "GetEnvironmentTemplateVersionOutputOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
-    "UpdateEnvironmentTemplateVersionOutputTypeDef",
+UpdateEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
+    "UpdateEnvironmentTemplateVersionOutputOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRepositoryOutputTypeDef = TypedDict(
-    "CreateRepositoryOutputTypeDef",
+CreateRepositoryOutputOutputTypeDef = TypedDict(
+    "CreateRepositoryOutputOutputTypeDef",
     {
-        "repository": RepositoryTypeDef,
+        "repository": RepositoryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRepositoryOutputTypeDef = TypedDict(
-    "DeleteRepositoryOutputTypeDef",
+DeleteRepositoryOutputOutputTypeDef = TypedDict(
+    "DeleteRepositoryOutputOutputTypeDef",
     {
-        "repository": RepositoryTypeDef,
+        "repository": RepositoryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetRepositoryOutputTypeDef = TypedDict(
-    "GetRepositoryOutputTypeDef",
+GetRepositoryOutputOutputTypeDef = TypedDict(
+    "GetRepositoryOutputOutputTypeDef",
     {
-        "repository": RepositoryTypeDef,
+        "repository": RepositoryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceSyncConfigOutputTypeDef = TypedDict(
-    "CreateServiceSyncConfigOutputTypeDef",
+CreateServiceSyncConfigOutputOutputTypeDef = TypedDict(
+    "CreateServiceSyncConfigOutputOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceSyncConfigOutputTypeDef = TypedDict(
-    "DeleteServiceSyncConfigOutputTypeDef",
+DeleteServiceSyncConfigOutputOutputTypeDef = TypedDict(
+    "DeleteServiceSyncConfigOutputOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceSyncConfigOutputTypeDef = TypedDict(
-    "GetServiceSyncConfigOutputTypeDef",
+GetServiceSyncConfigOutputOutputTypeDef = TypedDict(
+    "GetServiceSyncConfigOutputOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceSyncConfigOutputTypeDef = TypedDict(
-    "UpdateServiceSyncConfigOutputTypeDef",
+UpdateServiceSyncConfigOutputOutputTypeDef = TypedDict(
+    "UpdateServiceSyncConfigOutputOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceTemplateOutputTypeDef = TypedDict(
-    "CreateServiceTemplateOutputTypeDef",
+CreateServiceTemplateOutputOutputTypeDef = TypedDict(
+    "CreateServiceTemplateOutputOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateTypeDef,
+        "serviceTemplate": ServiceTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceTemplateOutputTypeDef = TypedDict(
-    "DeleteServiceTemplateOutputTypeDef",
+DeleteServiceTemplateOutputOutputTypeDef = TypedDict(
+    "DeleteServiceTemplateOutputOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateTypeDef,
+        "serviceTemplate": ServiceTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceTemplateOutputTypeDef = TypedDict(
-    "GetServiceTemplateOutputTypeDef",
+GetServiceTemplateOutputOutputTypeDef = TypedDict(
+    "GetServiceTemplateOutputOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateTypeDef,
+        "serviceTemplate": ServiceTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceTemplateOutputTypeDef = TypedDict(
-    "UpdateServiceTemplateOutputTypeDef",
+UpdateServiceTemplateOutputOutputTypeDef = TypedDict(
+    "UpdateServiceTemplateOutputOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateTypeDef,
+        "serviceTemplate": ServiceTemplateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateTemplateSyncConfigOutputTypeDef = TypedDict(
-    "CreateTemplateSyncConfigOutputTypeDef",
+CreateTemplateSyncConfigOutputOutputTypeDef = TypedDict(
+    "CreateTemplateSyncConfigOutputOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigTypeDef,
+        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteTemplateSyncConfigOutputTypeDef = TypedDict(
-    "DeleteTemplateSyncConfigOutputTypeDef",
+DeleteTemplateSyncConfigOutputOutputTypeDef = TypedDict(
+    "DeleteTemplateSyncConfigOutputOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigTypeDef,
+        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetTemplateSyncConfigOutputTypeDef = TypedDict(
-    "GetTemplateSyncConfigOutputTypeDef",
+GetTemplateSyncConfigOutputOutputTypeDef = TypedDict(
+    "GetTemplateSyncConfigOutputOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigTypeDef,
+        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateTemplateSyncConfigOutputTypeDef = TypedDict(
-    "UpdateTemplateSyncConfigOutputTypeDef",
+UpdateTemplateSyncConfigOutputOutputTypeDef = TypedDict(
+    "UpdateTemplateSyncConfigOutputOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigTypeDef,
+        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeploymentStateTypeDef = TypedDict(
-    "DeploymentStateTypeDef",
+DeploymentStateOutputTypeDef = TypedDict(
+    "DeploymentStateOutputTypeDef",
     {
-        "component": ComponentStateTypeDef,
-        "environment": EnvironmentStateTypeDef,
-        "serviceInstance": ServiceInstanceStateTypeDef,
-        "servicePipeline": ServicePipelineStateTypeDef,
+        "component": ComponentStateOutputTypeDef,
+        "environment": EnvironmentStateOutputTypeDef,
+        "serviceInstance": ServiceInstanceStateOutputTypeDef,
+        "servicePipeline": ServicePipelineStateOutputTypeDef,
     },
 )
 
-ListDeploymentsOutputTypeDef = TypedDict(
-    "ListDeploymentsOutputTypeDef",
+ListDeploymentsOutputOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputOutputTypeDef",
     {
-        "deployments": List[DeploymentSummaryTypeDef],
+        "deployments": List[DeploymentSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentAccountConnectionsOutputTypeDef = TypedDict(
-    "ListEnvironmentAccountConnectionsOutputTypeDef",
+ListEnvironmentAccountConnectionsOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentAccountConnectionsOutputOutputTypeDef",
     {
-        "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryTypeDef],
+        "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentsOutputTypeDef = TypedDict(
-    "ListEnvironmentsOutputTypeDef",
+ListEnvironmentsOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentsOutputOutputTypeDef",
     {
-        "environments": List[EnvironmentSummaryTypeDef],
+        "environments": List[EnvironmentSummaryOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
@@ -2841,28 +2851,28 @@
         "environmentTemplates": Sequence[EnvironmentTemplateFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListEnvironmentTemplatesOutputTypeDef = TypedDict(
-    "ListEnvironmentTemplatesOutputTypeDef",
+ListEnvironmentTemplatesOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentTemplatesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "templates": List[EnvironmentTemplateSummaryTypeDef],
+        "templates": List[EnvironmentTemplateSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentTemplateVersionsOutputTypeDef = TypedDict(
-    "ListEnvironmentTemplateVersionsOutputTypeDef",
+ListEnvironmentTemplateVersionsOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentTemplateVersionsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "templateVersions": List[EnvironmentTemplateVersionSummaryTypeDef],
+        "templateVersions": List[EnvironmentTemplateVersionSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetComponentInputComponentDeletedWaitTypeDef = TypedDict(
     "_RequiredGetComponentInputComponentDeletedWaitTypeDef",
     {
@@ -3064,123 +3074,100 @@
 
 class GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef(
     _RequiredGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
     _OptionalGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
 ):
     pass
 
-ListComponentOutputsOutputTypeDef = TypedDict(
-    "ListComponentOutputsOutputTypeDef",
+ListComponentOutputsOutputOutputTypeDef = TypedDict(
+    "ListComponentOutputsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputTypeDef],
+        "outputs": List[OutputOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentOutputsOutputTypeDef = TypedDict(
-    "ListEnvironmentOutputsOutputTypeDef",
+ListEnvironmentOutputsOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentOutputsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputTypeDef],
+        "outputs": List[OutputOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceInstanceOutputsOutputTypeDef = TypedDict(
-    "ListServiceInstanceOutputsOutputTypeDef",
+ListServiceInstanceOutputsOutputOutputTypeDef = TypedDict(
+    "ListServiceInstanceOutputsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputTypeDef],
+        "outputs": List[OutputOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicePipelineOutputsOutputTypeDef = TypedDict(
-    "ListServicePipelineOutputsOutputTypeDef",
+ListServicePipelineOutputsOutputOutputTypeDef = TypedDict(
+    "ListServicePipelineOutputsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputTypeDef],
+        "outputs": List[OutputOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
-    "_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
-    "_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    {
-        "deploymentId": str,
-        "outputs": Sequence[OutputTypeDef],
-        "status": ResourceDeploymentStatusType,
-        "statusMessage": str,
-    },
-    total=False,
-)
-
-class NotifyResourceDeploymentStatusChangeInputRequestTypeDef(
-    _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
-    _OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
-):
-    pass
-
-ListComponentProvisionedResourcesOutputTypeDef = TypedDict(
-    "ListComponentProvisionedResourcesOutputTypeDef",
+ListComponentProvisionedResourcesOutputOutputTypeDef = TypedDict(
+    "ListComponentProvisionedResourcesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceTypeDef],
+        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentProvisionedResourcesOutputTypeDef = TypedDict(
-    "ListEnvironmentProvisionedResourcesOutputTypeDef",
+ListEnvironmentProvisionedResourcesOutputOutputTypeDef = TypedDict(
+    "ListEnvironmentProvisionedResourcesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceTypeDef],
+        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceInstanceProvisionedResourcesOutputTypeDef = TypedDict(
-    "ListServiceInstanceProvisionedResourcesOutputTypeDef",
+ListServiceInstanceProvisionedResourcesOutputOutputTypeDef = TypedDict(
+    "ListServiceInstanceProvisionedResourcesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceTypeDef],
+        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicePipelineProvisionedResourcesOutputTypeDef = TypedDict(
-    "ListServicePipelineProvisionedResourcesOutputTypeDef",
+ListServicePipelineProvisionedResourcesOutputOutputTypeDef = TypedDict(
+    "ListServicePipelineProvisionedResourcesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceTypeDef],
+        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRepositoriesOutputTypeDef = TypedDict(
-    "ListRepositoriesOutputTypeDef",
+ListRepositoriesOutputOutputTypeDef = TypedDict(
+    "ListRepositoriesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "repositories": List[RepositorySummaryTypeDef],
+        "repositories": List[RepositorySummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRepositorySyncDefinitionsOutputTypeDef = TypedDict(
-    "ListRepositorySyncDefinitionsOutputTypeDef",
+ListRepositorySyncDefinitionsOutputOutputTypeDef = TypedDict(
+    "ListRepositorySyncDefinitionsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "syncDefinitions": List[RepositorySyncDefinitionTypeDef],
+        "syncDefinitions": List[RepositorySyncDefinitionOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceInstancesInputListServiceInstancesPaginateTypeDef = TypedDict(
     "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
     {
@@ -3202,269 +3189,301 @@
         "serviceName": str,
         "sortBy": ListServiceInstancesSortByType,
         "sortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListServiceInstancesOutputTypeDef = TypedDict(
-    "ListServiceInstancesOutputTypeDef",
+ListServiceInstancesOutputOutputTypeDef = TypedDict(
+    "ListServiceInstancesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "serviceInstances": List[ServiceInstanceSummaryTypeDef],
+        "serviceInstances": List[ServiceInstanceSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceTemplateVersionsOutputTypeDef = TypedDict(
-    "ListServiceTemplateVersionsOutputTypeDef",
+ListServiceTemplateVersionsOutputOutputTypeDef = TypedDict(
+    "ListServiceTemplateVersionsOutputOutputTypeDef",
     {
         "nextToken": str,
-        "templateVersions": List[ServiceTemplateVersionSummaryTypeDef],
+        "templateVersions": List[ServiceTemplateVersionSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceTemplatesOutputTypeDef = TypedDict(
-    "ListServiceTemplatesOutputTypeDef",
+ListServiceTemplatesOutputOutputTypeDef = TypedDict(
+    "ListServiceTemplatesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "templates": List[ServiceTemplateSummaryTypeDef],
+        "templates": List[ServiceTemplateSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicesOutputTypeDef = TypedDict(
-    "ListServicesOutputTypeDef",
+ListServicesOutputOutputTypeDef = TypedDict(
+    "ListServicesOutputOutputTypeDef",
     {
         "nextToken": str,
-        "services": List[ServiceSummaryTypeDef],
+        "services": List[ServiceSummaryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RepositorySyncAttemptTypeDef = TypedDict(
-    "RepositorySyncAttemptTypeDef",
+ListTagsForResourceOutputOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputOutputTypeDef",
+    {
+        "nextToken": str,
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
+    "_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
+    "_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    {
+        "deploymentId": str,
+        "outputs": Sequence[OutputTypeDef],
+        "status": ResourceDeploymentStatusType,
+        "statusMessage": str,
+    },
+    total=False,
+)
+
+class NotifyResourceDeploymentStatusChangeInputRequestTypeDef(
+    _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
+    _OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
+):
+    pass
+
+RepositorySyncAttemptOutputTypeDef = TypedDict(
+    "RepositorySyncAttemptOutputTypeDef",
     {
-        "events": List[RepositorySyncEventTypeDef],
+        "events": List[RepositorySyncEventOutputTypeDef],
         "startedAt": datetime,
         "status": RepositorySyncStatusType,
     },
 )
 
-ResourceSyncAttemptTypeDef = TypedDict(
-    "ResourceSyncAttemptTypeDef",
+ResourceSyncAttemptOutputTypeDef = TypedDict(
+    "ResourceSyncAttemptOutputTypeDef",
     {
-        "events": List[ResourceSyncEventTypeDef],
-        "initialRevision": RevisionTypeDef,
+        "events": List[ResourceSyncEventOutputTypeDef],
+        "initialRevision": RevisionOutputTypeDef,
         "startedAt": datetime,
         "status": ResourceSyncStatusType,
         "target": str,
-        "targetRevision": RevisionTypeDef,
+        "targetRevision": RevisionOutputTypeDef,
     },
 )
 
 TemplateVersionSourceInputTypeDef = TypedDict(
     "TemplateVersionSourceInputTypeDef",
     {
         "s3": S3ObjectSourceTypeDef,
     },
     total=False,
 )
 
-SyncBlockerTypeDef = TypedDict(
-    "SyncBlockerTypeDef",
+SyncBlockerOutputTypeDef = TypedDict(
+    "SyncBlockerOutputTypeDef",
     {
-        "contexts": List[SyncBlockerContextTypeDef],
+        "contexts": List[SyncBlockerContextOutputTypeDef],
         "createdAt": datetime,
         "createdReason": str,
         "id": str,
         "resolvedAt": datetime,
         "resolvedReason": str,
         "status": BlockerStatusType,
         "type": Literal["AUTOMATED"],
     },
 )
 
-GetAccountSettingsOutputTypeDef = TypedDict(
-    "GetAccountSettingsOutputTypeDef",
+GetAccountSettingsOutputOutputTypeDef = TypedDict(
+    "GetAccountSettingsOutputOutputTypeDef",
     {
-        "accountSettings": AccountSettingsTypeDef,
+        "accountSettings": AccountSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAccountSettingsOutputTypeDef = TypedDict(
-    "UpdateAccountSettingsOutputTypeDef",
+UpdateAccountSettingsOutputOutputTypeDef = TypedDict(
+    "UpdateAccountSettingsOutputOutputTypeDef",
     {
-        "accountSettings": AccountSettingsTypeDef,
+        "accountSettings": AccountSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelEnvironmentDeploymentOutputTypeDef = TypedDict(
-    "CancelEnvironmentDeploymentOutputTypeDef",
+CancelEnvironmentDeploymentOutputOutputTypeDef = TypedDict(
+    "CancelEnvironmentDeploymentOutputOutputTypeDef",
     {
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentOutputTypeDef = TypedDict(
-    "CreateEnvironmentOutputTypeDef",
+CreateEnvironmentOutputOutputTypeDef = TypedDict(
+    "CreateEnvironmentOutputOutputTypeDef",
     {
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentOutputTypeDef = TypedDict(
-    "DeleteEnvironmentOutputTypeDef",
+DeleteEnvironmentOutputOutputTypeDef = TypedDict(
+    "DeleteEnvironmentOutputOutputTypeDef",
     {
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentOutputTypeDef = TypedDict(
-    "GetEnvironmentOutputTypeDef",
+GetEnvironmentOutputOutputTypeDef = TypedDict(
+    "GetEnvironmentOutputOutputTypeDef",
     {
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentOutputTypeDef = TypedDict(
-    "UpdateEnvironmentOutputTypeDef",
+UpdateEnvironmentOutputOutputTypeDef = TypedDict(
+    "UpdateEnvironmentOutputOutputTypeDef",
     {
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceOutputTypeDef = TypedDict(
-    "CreateServiceOutputTypeDef",
+CreateServiceOutputOutputTypeDef = TypedDict(
+    "CreateServiceOutputOutputTypeDef",
     {
-        "service": ServiceTypeDef,
+        "service": ServiceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceOutputTypeDef = TypedDict(
-    "DeleteServiceOutputTypeDef",
+DeleteServiceOutputOutputTypeDef = TypedDict(
+    "DeleteServiceOutputOutputTypeDef",
     {
-        "service": ServiceTypeDef,
+        "service": ServiceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceOutputTypeDef = TypedDict(
-    "GetServiceOutputTypeDef",
+GetServiceOutputOutputTypeDef = TypedDict(
+    "GetServiceOutputOutputTypeDef",
     {
-        "service": ServiceTypeDef,
+        "service": ServiceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceOutputTypeDef = TypedDict(
-    "UpdateServiceOutputTypeDef",
+UpdateServiceOutputOutputTypeDef = TypedDict(
+    "UpdateServiceOutputOutputTypeDef",
     {
-        "service": ServiceTypeDef,
+        "service": ServiceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceTemplateVersionOutputTypeDef = TypedDict(
-    "CreateServiceTemplateVersionOutputTypeDef",
+CreateServiceTemplateVersionOutputOutputTypeDef = TypedDict(
+    "CreateServiceTemplateVersionOutputOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceTemplateVersionOutputTypeDef = TypedDict(
-    "DeleteServiceTemplateVersionOutputTypeDef",
+DeleteServiceTemplateVersionOutputOutputTypeDef = TypedDict(
+    "DeleteServiceTemplateVersionOutputOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceTemplateVersionOutputTypeDef = TypedDict(
-    "GetServiceTemplateVersionOutputTypeDef",
+GetServiceTemplateVersionOutputOutputTypeDef = TypedDict(
+    "GetServiceTemplateVersionOutputOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceTemplateVersionOutputTypeDef = TypedDict(
-    "UpdateServiceTemplateVersionOutputTypeDef",
+UpdateServiceTemplateVersionOutputOutputTypeDef = TypedDict(
+    "UpdateServiceTemplateVersionOutputOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetResourcesSummaryOutputTypeDef = TypedDict(
-    "GetResourcesSummaryOutputTypeDef",
+GetResourcesSummaryOutputOutputTypeDef = TypedDict(
+    "GetResourcesSummaryOutputOutputTypeDef",
     {
-        "counts": CountsSummaryTypeDef,
+        "counts": CountsSummaryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeploymentTypeDef = TypedDict(
-    "DeploymentTypeDef",
+DeploymentOutputTypeDef = TypedDict(
+    "DeploymentOutputTypeDef",
     {
         "arn": str,
         "completedAt": datetime,
         "componentName": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "id": str,
-        "initialState": DeploymentStateTypeDef,
+        "initialState": DeploymentStateOutputTypeDef,
         "lastAttemptedDeploymentId": str,
         "lastModifiedAt": datetime,
         "lastSucceededDeploymentId": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "targetArn": str,
         "targetResourceCreatedAt": datetime,
         "targetResourceType": DeploymentTargetResourceTypeType,
-        "targetState": DeploymentStateTypeDef,
+        "targetState": DeploymentStateOutputTypeDef,
     },
 )
 
-GetRepositorySyncStatusOutputTypeDef = TypedDict(
-    "GetRepositorySyncStatusOutputTypeDef",
+GetRepositorySyncStatusOutputOutputTypeDef = TypedDict(
+    "GetRepositorySyncStatusOutputOutputTypeDef",
     {
-        "latestSync": RepositorySyncAttemptTypeDef,
+        "latestSync": RepositorySyncAttemptOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceInstanceSyncStatusOutputTypeDef = TypedDict(
-    "GetServiceInstanceSyncStatusOutputTypeDef",
+GetServiceInstanceSyncStatusOutputOutputTypeDef = TypedDict(
+    "GetServiceInstanceSyncStatusOutputOutputTypeDef",
     {
-        "desiredState": RevisionTypeDef,
-        "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
-        "latestSync": ResourceSyncAttemptTypeDef,
+        "desiredState": RevisionOutputTypeDef,
+        "latestSuccessfulSync": ResourceSyncAttemptOutputTypeDef,
+        "latestSync": ResourceSyncAttemptOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetTemplateSyncStatusOutputTypeDef = TypedDict(
-    "GetTemplateSyncStatusOutputTypeDef",
+GetTemplateSyncStatusOutputOutputTypeDef = TypedDict(
+    "GetTemplateSyncStatusOutputOutputTypeDef",
     {
-        "desiredState": RevisionTypeDef,
-        "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
-        "latestSync": ResourceSyncAttemptTypeDef,
+        "desiredState": RevisionOutputTypeDef,
+        "latestSuccessfulSync": ResourceSyncAttemptOutputTypeDef,
+        "latestSync": ResourceSyncAttemptOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef",
     {
@@ -3511,49 +3530,49 @@
 
 class CreateServiceTemplateVersionInputRequestTypeDef(
     _RequiredCreateServiceTemplateVersionInputRequestTypeDef,
     _OptionalCreateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
-ServiceSyncBlockerSummaryTypeDef = TypedDict(
-    "ServiceSyncBlockerSummaryTypeDef",
+ServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
+    "ServiceSyncBlockerSummaryOutputTypeDef",
     {
-        "latestBlockers": List[SyncBlockerTypeDef],
+        "latestBlockers": List[SyncBlockerOutputTypeDef],
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-UpdateServiceSyncBlockerOutputTypeDef = TypedDict(
-    "UpdateServiceSyncBlockerOutputTypeDef",
+UpdateServiceSyncBlockerOutputOutputTypeDef = TypedDict(
+    "UpdateServiceSyncBlockerOutputOutputTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
-        "serviceSyncBlocker": SyncBlockerTypeDef,
+        "serviceSyncBlocker": SyncBlockerOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteDeploymentOutputTypeDef = TypedDict(
-    "DeleteDeploymentOutputTypeDef",
+DeleteDeploymentOutputOutputTypeDef = TypedDict(
+    "DeleteDeploymentOutputOutputTypeDef",
     {
-        "deployment": DeploymentTypeDef,
+        "deployment": DeploymentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetDeploymentOutputTypeDef = TypedDict(
-    "GetDeploymentOutputTypeDef",
+GetDeploymentOutputOutputTypeDef = TypedDict(
+    "GetDeploymentOutputOutputTypeDef",
     {
-        "deployment": DeploymentTypeDef,
+        "deployment": DeploymentOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
-    "GetServiceSyncBlockerSummaryOutputTypeDef",
+GetServiceSyncBlockerSummaryOutputOutputTypeDef = TypedDict(
+    "GetServiceSyncBlockerSummaryOutputOutputTypeDef",
     {
-        "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryTypeDef,
+        "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/waiter.py` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton/waiter.pyi` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/SOURCES.txt` & `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3/setup.py` & `mypy-boto3-proton-1.28.3.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-proton",
-    version="1.28.3",
+    version="1.28.3.post1",
     packages=["mypy_boto3_proton"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Proton 1.28.3 service generated with mypy-boto3-builder 7.14.6"
+        "Type annotations for boto3.Proton 1.28.3 service generated with mypy-boto3-builder 7.14.7"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

