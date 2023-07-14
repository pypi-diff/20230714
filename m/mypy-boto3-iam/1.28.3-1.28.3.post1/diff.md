# Comparing `tmp/mypy-boto3-iam-1.28.3.tar.gz` & `tmp/mypy-boto3-iam-1.28.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iam-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
+gzip compressed data, was "mypy-boto3-iam-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
```

## Comparing `mypy-boto3-iam-1.28.3.tar` & `mypy-boto3-iam-1.28.3.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.685228 mypy-boto3-iam-1.28.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-13 19:49:12.677227 mypy-boto3-iam-1.28.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40459 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.677227 mypy-boto3-iam-1.28.3/mypy_boto3_iam/
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113198 2023-07-13 19:48:11.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   112994 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-13 19:48:13.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-07-13 19:48:13.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    38502 2023-07-13 19:48:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    38466 2023-07-13 19:48:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   141689 2023-07-13 19:48:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   141336 2023-07-13 19:48:11.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   141573 2023-07-13 19:48:16.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   141392 2023-07-13 19:48:15.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-13 19:48:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-13 19:48:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.677227 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.685228 mypy-boto3-iam-1.28.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.907362 mypy-boto3-iam-1.28.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42754 2023-07-14 16:17:59.903361 mypy-boto3-iam-1.28.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    41279 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114262 2023-07-14 16:16:43.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114058 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-14 16:16:45.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-07-14 16:16:45.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38904 2023-07-14 16:16:45.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38868 2023-07-14 16:16:44.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   141783 2023-07-14 16:16:44.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141430 2023-07-14 16:16:44.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   144793 2023-07-14 16:16:49.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144612 2023-07-14 16:16:47.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-14 16:16:45.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-14 16:16:45.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.903361 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42754 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.907362 mypy-boto3-iam-1.28.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-14 16:16:41.000000 mypy-boto3-iam-1.28.3.post1/setup.py
```

### Comparing `mypy-boto3-iam-1.28.3/LICENSE` & `mypy-boto3-iam-1.28.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3/PKG-INFO` & `mypy-boto3-iam-1.28.3.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iam
-Version: 1.28.3
-Summary: Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/
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
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -639,18 +639,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_iam.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iam.type_defs import (
-    AccessDetailTypeDef,
-    AccessKeyLastUsedTypeDef,
-    AccessKeyMetadataTypeDef,
-    AccessKeyTypeDef,
+    AccessDetailOutputTypeDef,
+    AccessKeyLastUsedOutputTypeDef,
+    AccessKeyMetadataOutputTypeDef,
+    AccessKeyOutputTypeDef,
     AddClientIDToOpenIDConnectProviderRequestRequestTypeDef,
     AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef,
     AddRoleToInstanceProfileRequestRequestTypeDef,
     AddUserToGroupRequestGroupAddUserTypeDef,
     AddUserToGroupRequestRequestTypeDef,
     AddUserToGroupRequestUserAddGroupTypeDef,
     AttachGroupPolicyRequestGroupAttachPolicyTypeDef,
@@ -658,38 +658,39 @@
     AttachGroupPolicyRequestRequestTypeDef,
     AttachRolePolicyRequestPolicyAttachRoleTypeDef,
     AttachRolePolicyRequestRequestTypeDef,
     AttachRolePolicyRequestRoleAttachPolicyTypeDef,
     AttachUserPolicyRequestPolicyAttachUserTypeDef,
     AttachUserPolicyRequestRequestTypeDef,
     AttachUserPolicyRequestUserAttachPolicyTypeDef,
+    AttachedPermissionsBoundaryOutputTypeDef,
     AttachedPermissionsBoundaryResponseMetadataTypeDef,
-    AttachedPermissionsBoundaryTypeDef,
-    AttachedPolicyTypeDef,
+    AttachedPolicyOutputTypeDef,
     ChangePasswordRequestRequestTypeDef,
     ChangePasswordRequestServiceResourceChangePasswordTypeDef,
     ContextEntryTypeDef,
     CreateAccessKeyRequestRequestTypeDef,
     CreateAccountAliasRequestRequestTypeDef,
     CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef,
     CreateGroupRequestGroupCreateTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateGroupRequestServiceResourceCreateGroupTypeDef,
-    GroupTypeDef,
+    GroupOutputTypeDef,
     TagTypeDef,
     CreateLoginProfileRequestLoginProfileCreateTypeDef,
     CreateLoginProfileRequestRequestTypeDef,
     CreateLoginProfileRequestUserCreateLoginProfileTypeDef,
-    LoginProfileTypeDef,
+    LoginProfileOutputTypeDef,
+    TagOutputTypeDef,
     CreatePolicyVersionRequestPolicyCreateVersionTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    PolicyVersionTypeDef,
+    PolicyVersionOutputTypeDef,
     CreateServiceLinkedRoleRequestRequestTypeDef,
     CreateServiceSpecificCredentialRequestRequestTypeDef,
-    ServiceSpecificCredentialTypeDef,
+    ServiceSpecificCredentialOutputTypeDef,
     DeactivateMFADeviceRequestRequestTypeDef,
     DeleteAccessKeyRequestRequestTypeDef,
     DeleteAccountAliasRequestRequestTypeDef,
     DeleteGroupPolicyRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
     DeleteLoginProfileRequestRequestTypeDef,
@@ -699,159 +700,159 @@
     DeleteRolePermissionsBoundaryRequestRequestTypeDef,
     DeleteRolePolicyRequestRequestTypeDef,
     DeleteRoleRequestRequestTypeDef,
     DeleteSAMLProviderRequestRequestTypeDef,
     DeleteSSHPublicKeyRequestRequestTypeDef,
     DeleteServerCertificateRequestRequestTypeDef,
     DeleteServiceLinkedRoleRequestRequestTypeDef,
-    DeleteServiceLinkedRoleResponseTypeDef,
+    DeleteServiceLinkedRoleResponseOutputTypeDef,
     DeleteServiceSpecificCredentialRequestRequestTypeDef,
     DeleteSigningCertificateRequestRequestTypeDef,
     DeleteUserPermissionsBoundaryRequestRequestTypeDef,
     DeleteUserPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVirtualMFADeviceRequestRequestTypeDef,
-    RoleUsageTypeTypeDef,
+    RoleUsageTypeOutputTypeDef,
     DetachGroupPolicyRequestGroupDetachPolicyTypeDef,
     DetachGroupPolicyRequestPolicyDetachGroupTypeDef,
     DetachGroupPolicyRequestRequestTypeDef,
     DetachRolePolicyRequestPolicyDetachRoleTypeDef,
     DetachRolePolicyRequestRequestTypeDef,
     DetachRolePolicyRequestRoleDetachPolicyTypeDef,
     DetachUserPolicyRequestPolicyDetachUserTypeDef,
     DetachUserPolicyRequestRequestTypeDef,
     DetachUserPolicyRequestUserDetachPolicyTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableMFADeviceRequestMfaDeviceAssociateTypeDef,
     EnableMFADeviceRequestRequestTypeDef,
     EnableMFADeviceRequestUserEnableMfaTypeDef,
-    EntityInfoTypeDef,
-    ErrorDetailsTypeDef,
-    OrganizationsDecisionDetailTypeDef,
-    PermissionsBoundaryDecisionDetailTypeDef,
-    GenerateCredentialReportResponseTypeDef,
+    EntityInfoOutputTypeDef,
+    ErrorDetailsOutputTypeDef,
+    OrganizationsDecisionDetailOutputTypeDef,
+    PermissionsBoundaryDecisionDetailOutputTypeDef,
+    GenerateCredentialReportResponseOutputTypeDef,
     GenerateOrganizationsAccessReportRequestRequestTypeDef,
-    GenerateOrganizationsAccessReportResponseTypeDef,
+    GenerateOrganizationsAccessReportResponseOutputTypeDef,
     GenerateServiceLastAccessedDetailsRequestRequestTypeDef,
-    GenerateServiceLastAccessedDetailsResponseTypeDef,
+    GenerateServiceLastAccessedDetailsResponseOutputTypeDef,
     GetAccessKeyLastUsedRequestRequestTypeDef,
     GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
     GetAccountAuthorizationDetailsRequestRequestTypeDef,
-    PasswordPolicyTypeDef,
-    GetAccountSummaryResponseTypeDef,
+    PasswordPolicyOutputTypeDef,
+    GetAccountSummaryResponseOutputTypeDef,
     GetContextKeysForCustomPolicyRequestRequestTypeDef,
-    GetContextKeysForPolicyResponseTypeDef,
+    GetContextKeysForPolicyResponseOutputTypeDef,
     GetContextKeysForPrincipalPolicyRequestRequestTypeDef,
-    GetCredentialReportResponseTypeDef,
+    GetCredentialReportResponseOutputTypeDef,
     GetGroupPolicyRequestRequestTypeDef,
-    GetGroupPolicyResponseTypeDef,
+    GetGroupPolicyResponseOutputTypeDef,
     GetGroupRequestGetGroupPaginateTypeDef,
     GetGroupRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetLoginProfileRequestRequestTypeDef,
     GetMFADeviceRequestRequestTypeDef,
-    GetMFADeviceResponseTypeDef,
+    GetMFADeviceResponseOutputTypeDef,
     GetOpenIDConnectProviderRequestRequestTypeDef,
     GetOrganizationsAccessReportRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
     GetRolePolicyRequestRequestTypeDef,
-    GetRolePolicyResponseTypeDef,
+    GetRolePolicyResponseOutputTypeDef,
     GetRoleRequestRequestTypeDef,
     GetSAMLProviderRequestRequestTypeDef,
     GetSSHPublicKeyRequestRequestTypeDef,
-    SSHPublicKeyTypeDef,
+    SSHPublicKeyOutputTypeDef,
     GetServerCertificateRequestRequestTypeDef,
     GetServiceLastAccessedDetailsRequestRequestTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
     GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef,
     GetUserPolicyRequestRequestTypeDef,
-    GetUserPolicyResponseTypeDef,
+    GetUserPolicyResponseOutputTypeDef,
     GetUserRequestRequestTypeDef,
-    PolicyDetailTypeDef,
+    PolicyDetailOutputTypeDef,
     ListAccessKeysRequestListAccessKeysPaginateTypeDef,
     ListAccessKeysRequestRequestTypeDef,
     ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
     ListAccountAliasesRequestRequestTypeDef,
-    ListAccountAliasesResponseTypeDef,
+    ListAccountAliasesResponseOutputTypeDef,
     ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
     ListAttachedGroupPoliciesRequestRequestTypeDef,
     ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
     ListAttachedRolePoliciesRequestRequestTypeDef,
     ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
     ListAttachedUserPoliciesRequestRequestTypeDef,
     ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
     ListEntitiesForPolicyRequestRequestTypeDef,
-    PolicyGroupTypeDef,
-    PolicyRoleTypeDef,
-    PolicyUserTypeDef,
+    PolicyGroupOutputTypeDef,
+    PolicyRoleOutputTypeDef,
+    PolicyUserOutputTypeDef,
     ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
     ListGroupPoliciesRequestRequestTypeDef,
-    ListGroupPoliciesResponseTypeDef,
+    ListGroupPoliciesResponseOutputTypeDef,
     ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
     ListGroupsForUserRequestRequestTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
     ListInstanceProfileTagsRequestRequestTypeDef,
     ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
     ListInstanceProfilesForRoleRequestRequestTypeDef,
     ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
     ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
     ListMFADeviceTagsRequestRequestTypeDef,
     ListMFADevicesRequestListMFADevicesPaginateTypeDef,
     ListMFADevicesRequestRequestTypeDef,
-    MFADeviceTypeDef,
+    MFADeviceOutputTypeDef,
     ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
     ListOpenIDConnectProviderTagsRequestRequestTypeDef,
-    OpenIDConnectProviderListEntryTypeDef,
-    PolicyGrantingServiceAccessTypeDef,
+    OpenIDConnectProviderListEntryOutputTypeDef,
+    PolicyGrantingServiceAccessOutputTypeDef,
     ListPoliciesGrantingServiceAccessRequestRequestTypeDef,
     ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
     ListPolicyTagsRequestRequestTypeDef,
     ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
     ListRolePoliciesRequestRequestTypeDef,
-    ListRolePoliciesResponseTypeDef,
+    ListRolePoliciesResponseOutputTypeDef,
     ListRoleTagsRequestListRoleTagsPaginateTypeDef,
     ListRoleTagsRequestRequestTypeDef,
     ListRolesRequestListRolesPaginateTypeDef,
     ListRolesRequestRequestTypeDef,
     ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
     ListSAMLProviderTagsRequestRequestTypeDef,
-    SAMLProviderListEntryTypeDef,
+    SAMLProviderListEntryOutputTypeDef,
     ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
     ListSSHPublicKeysRequestRequestTypeDef,
-    SSHPublicKeyMetadataTypeDef,
+    SSHPublicKeyMetadataOutputTypeDef,
     ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
     ListServerCertificateTagsRequestRequestTypeDef,
     ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
     ListServerCertificatesRequestRequestTypeDef,
-    ServerCertificateMetadataTypeDef,
+    ServerCertificateMetadataOutputTypeDef,
     ListServiceSpecificCredentialsRequestRequestTypeDef,
-    ServiceSpecificCredentialMetadataTypeDef,
+    ServiceSpecificCredentialMetadataOutputTypeDef,
     ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
     ListSigningCertificatesRequestRequestTypeDef,
-    SigningCertificateTypeDef,
+    SigningCertificateOutputTypeDef,
     ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
     ListUserPoliciesRequestRequestTypeDef,
-    ListUserPoliciesResponseTypeDef,
+    ListUserPoliciesResponseOutputTypeDef,
     ListUserTagsRequestListUserTagsPaginateTypeDef,
     ListUserTagsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
     ListVirtualMFADevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    PositionTypeDef,
+    PositionOutputTypeDef,
     PutGroupPolicyRequestGroupCreatePolicyTypeDef,
     PutGroupPolicyRequestGroupPolicyPutTypeDef,
     PutGroupPolicyRequestRequestTypeDef,
     PutRolePermissionsBoundaryRequestRequestTypeDef,
     PutRolePolicyRequestRequestTypeDef,
     PutRolePolicyRequestRolePolicyPutTypeDef,
     PutUserPermissionsBoundaryRequestRequestTypeDef,
@@ -864,18 +865,18 @@
     RemoveUserFromGroupRequestGroupRemoveUserTypeDef,
     RemoveUserFromGroupRequestRequestTypeDef,
     RemoveUserFromGroupRequestUserRemoveGroupTypeDef,
     ResetServiceSpecificCredentialRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ResyncMFADeviceRequestMfaDeviceResyncTypeDef,
     ResyncMFADeviceRequestRequestTypeDef,
-    RoleLastUsedTypeDef,
+    RoleLastUsedOutputTypeDef,
     RoleLastUsedResponseMetadataTypeDef,
     ServerCertificateMetadataResponseMetadataTypeDef,
-    TrackedActionLastAccessedTypeDef,
+    TrackedActionLastAccessedOutputTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetSecurityTokenServicePreferencesRequestRequestTypeDef,
     UntagInstanceProfileRequestRequestTypeDef,
     UntagMFADeviceRequestRequestTypeDef,
     UntagOpenIDConnectProviderRequestRequestTypeDef,
     UntagPolicyRequestRequestTypeDef,
     UntagRoleRequestRequestTypeDef,
@@ -897,148 +898,148 @@
     UpdateLoginProfileRequestLoginProfileUpdateTypeDef,
     UpdateLoginProfileRequestRequestTypeDef,
     UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef,
     UpdateRoleDescriptionRequestRequestTypeDef,
     UpdateRoleRequestRequestTypeDef,
     UpdateSAMLProviderRequestRequestTypeDef,
     UpdateSAMLProviderRequestSamlProviderUpdateTypeDef,
-    UpdateSAMLProviderResponseTypeDef,
+    UpdateSAMLProviderResponseOutputTypeDef,
     UpdateSSHPublicKeyRequestRequestTypeDef,
     UpdateServerCertificateRequestRequestTypeDef,
     UpdateServerCertificateRequestServerCertificateUpdateTypeDef,
     UpdateServiceSpecificCredentialRequestRequestTypeDef,
     UpdateSigningCertificateRequestRequestTypeDef,
     UpdateSigningCertificateRequestSigningCertificateActivateTypeDef,
     UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserRequestUserUpdateTypeDef,
     UploadSSHPublicKeyRequestRequestTypeDef,
     UploadSigningCertificateRequestRequestTypeDef,
     UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
-    GetAccessKeyLastUsedResponseTypeDef,
-    ListAccessKeysResponseTypeDef,
-    CreateAccessKeyResponseTypeDef,
-    ListAttachedGroupPoliciesResponseTypeDef,
-    ListAttachedRolePoliciesResponseTypeDef,
-    ListAttachedUserPoliciesResponseTypeDef,
+    GetAccessKeyLastUsedResponseOutputTypeDef,
+    ListAccessKeysResponseOutputTypeDef,
+    CreateAccessKeyResponseOutputTypeDef,
+    ListAttachedGroupPoliciesResponseOutputTypeDef,
+    ListAttachedRolePoliciesResponseOutputTypeDef,
+    ListAttachedUserPoliciesResponseOutputTypeDef,
     SimulateCustomPolicyRequestRequestTypeDef,
     SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
     SimulatePrincipalPolicyRequestRequestTypeDef,
     SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
-    CreateGroupResponseTypeDef,
-    ListGroupsForUserResponseTypeDef,
-    ListGroupsResponseTypeDef,
+    CreateGroupResponseOutputTypeDef,
+    ListGroupsForUserResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
     CreateOpenIDConnectProviderRequestRequestTypeDef,
-    CreateOpenIDConnectProviderResponseTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreatePolicyRequestServiceResourceCreatePolicyTypeDef,
     CreateRoleRequestRequestTypeDef,
     CreateRoleRequestServiceResourceCreateRoleTypeDef,
     CreateSAMLProviderRequestRequestTypeDef,
     CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef,
-    CreateSAMLProviderResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     CreateUserRequestServiceResourceCreateUserTypeDef,
     CreateUserRequestUserCreateTypeDef,
     CreateVirtualMFADeviceRequestRequestTypeDef,
     CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef,
-    GetOpenIDConnectProviderResponseTypeDef,
-    GetSAMLProviderResponseTypeDef,
-    ListInstanceProfileTagsResponseTypeDef,
-    ListMFADeviceTagsResponseTypeDef,
-    ListOpenIDConnectProviderTagsResponseTypeDef,
-    ListPolicyTagsResponseTypeDef,
-    ListRoleTagsResponseTypeDef,
-    ListSAMLProviderTagsResponseTypeDef,
-    ListServerCertificateTagsResponseTypeDef,
-    ListUserTagsResponseTypeDef,
-    PolicyTypeDef,
     TagInstanceProfileRequestRequestTypeDef,
     TagMFADeviceRequestRequestTypeDef,
     TagOpenIDConnectProviderRequestRequestTypeDef,
     TagPolicyRequestRequestTypeDef,
     TagRoleRequestRequestTypeDef,
     TagSAMLProviderRequestRequestTypeDef,
     TagServerCertificateRequestRequestTypeDef,
     TagUserRequestRequestTypeDef,
     UploadServerCertificateRequestRequestTypeDef,
     UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
+    CreateLoginProfileResponseOutputTypeDef,
+    GetLoginProfileResponseOutputTypeDef,
+    CreateOpenIDConnectProviderResponseOutputTypeDef,
+    CreateSAMLProviderResponseOutputTypeDef,
+    GetOpenIDConnectProviderResponseOutputTypeDef,
+    GetSAMLProviderResponseOutputTypeDef,
+    ListInstanceProfileTagsResponseOutputTypeDef,
+    ListMFADeviceTagsResponseOutputTypeDef,
+    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
+    ListPolicyTagsResponseOutputTypeDef,
+    ListRoleTagsResponseOutputTypeDef,
+    ListSAMLProviderTagsResponseOutputTypeDef,
+    ListServerCertificateTagsResponseOutputTypeDef,
+    ListUserTagsResponseOutputTypeDef,
+    PolicyOutputTypeDef,
+    UserOutputTypeDef,
     UserResponseMetadataTypeDef,
-    UserTypeDef,
-    CreateLoginProfileResponseTypeDef,
-    GetLoginProfileResponseTypeDef,
-    CreatePolicyVersionResponseTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    ListPolicyVersionsResponseTypeDef,
-    ManagedPolicyDetailTypeDef,
-    CreateServiceSpecificCredentialResponseTypeDef,
-    ResetServiceSpecificCredentialResponseTypeDef,
-    DeletionTaskFailureReasonTypeTypeDef,
-    EntityDetailsTypeDef,
-    GetOrganizationsAccessReportResponseTypeDef,
-    GetAccountPasswordPolicyResponseTypeDef,
+    CreatePolicyVersionResponseOutputTypeDef,
+    GetPolicyVersionResponseOutputTypeDef,
+    ListPolicyVersionsResponseOutputTypeDef,
+    ManagedPolicyDetailOutputTypeDef,
+    CreateServiceSpecificCredentialResponseOutputTypeDef,
+    ResetServiceSpecificCredentialResponseOutputTypeDef,
+    DeletionTaskFailureReasonTypeOutputTypeDef,
+    EntityDetailsOutputTypeDef,
+    GetOrganizationsAccessReportResponseOutputTypeDef,
+    GetAccountPasswordPolicyResponseOutputTypeDef,
     GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
     GetPolicyRequestPolicyExistsWaitTypeDef,
     GetRoleRequestRoleExistsWaitTypeDef,
     GetUserRequestUserExistsWaitTypeDef,
-    GetSSHPublicKeyResponseTypeDef,
-    UploadSSHPublicKeyResponseTypeDef,
-    GroupDetailTypeDef,
-    UserDetailTypeDef,
-    ListEntitiesForPolicyResponseTypeDef,
-    ListMFADevicesResponseTypeDef,
-    ListOpenIDConnectProvidersResponseTypeDef,
-    ListPoliciesGrantingServiceAccessEntryTypeDef,
-    ListSAMLProvidersResponseTypeDef,
-    ListSSHPublicKeysResponseTypeDef,
-    ListServerCertificatesResponseTypeDef,
-    ServerCertificateTypeDef,
-    UploadServerCertificateResponseTypeDef,
-    ListServiceSpecificCredentialsResponseTypeDef,
-    ListSigningCertificatesResponseTypeDef,
-    UploadSigningCertificateResponseTypeDef,
-    StatementTypeDef,
-    RoleTypeDef,
-    ServiceLastAccessedTypeDef,
-    CreatePolicyResponseTypeDef,
-    GetPolicyResponseTypeDef,
-    ListPoliciesResponseTypeDef,
-    CreateUserResponseTypeDef,
-    GetGroupResponseTypeDef,
-    GetUserResponseTypeDef,
-    ListUsersResponseTypeDef,
-    VirtualMFADeviceTypeDef,
-    GetServiceLinkedRoleDeletionStatusResponseTypeDef,
-    GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
-    ListPoliciesGrantingServiceAccessResponseTypeDef,
-    GetServerCertificateResponseTypeDef,
-    ResourceSpecificResultTypeDef,
-    CreateRoleResponseTypeDef,
-    CreateServiceLinkedRoleResponseTypeDef,
-    GetRoleResponseTypeDef,
-    InstanceProfileTypeDef,
-    ListRolesResponseTypeDef,
-    UpdateRoleDescriptionResponseTypeDef,
-    GetServiceLastAccessedDetailsResponseTypeDef,
-    CreateVirtualMFADeviceResponseTypeDef,
-    ListVirtualMFADevicesResponseTypeDef,
-    EvaluationResultTypeDef,
-    CreateInstanceProfileResponseTypeDef,
-    GetInstanceProfileResponseTypeDef,
-    ListInstanceProfilesForRoleResponseTypeDef,
-    ListInstanceProfilesResponseTypeDef,
-    RoleDetailTypeDef,
-    SimulatePolicyResponseTypeDef,
-    GetAccountAuthorizationDetailsResponseTypeDef,
+    GetSSHPublicKeyResponseOutputTypeDef,
+    UploadSSHPublicKeyResponseOutputTypeDef,
+    GroupDetailOutputTypeDef,
+    UserDetailOutputTypeDef,
+    ListEntitiesForPolicyResponseOutputTypeDef,
+    ListMFADevicesResponseOutputTypeDef,
+    ListOpenIDConnectProvidersResponseOutputTypeDef,
+    ListPoliciesGrantingServiceAccessEntryOutputTypeDef,
+    ListSAMLProvidersResponseOutputTypeDef,
+    ListSSHPublicKeysResponseOutputTypeDef,
+    ListServerCertificatesResponseOutputTypeDef,
+    ServerCertificateOutputTypeDef,
+    UploadServerCertificateResponseOutputTypeDef,
+    ListServiceSpecificCredentialsResponseOutputTypeDef,
+    ListSigningCertificatesResponseOutputTypeDef,
+    UploadSigningCertificateResponseOutputTypeDef,
+    StatementOutputTypeDef,
+    RoleOutputTypeDef,
+    ServiceLastAccessedOutputTypeDef,
+    CreatePolicyResponseOutputTypeDef,
+    GetPolicyResponseOutputTypeDef,
+    ListPoliciesResponseOutputTypeDef,
+    CreateUserResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    GetUserResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
+    VirtualMFADeviceOutputTypeDef,
+    GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef,
+    GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef,
+    ListPoliciesGrantingServiceAccessResponseOutputTypeDef,
+    GetServerCertificateResponseOutputTypeDef,
+    ResourceSpecificResultOutputTypeDef,
+    CreateRoleResponseOutputTypeDef,
+    CreateServiceLinkedRoleResponseOutputTypeDef,
+    GetRoleResponseOutputTypeDef,
+    InstanceProfileOutputTypeDef,
+    ListRolesResponseOutputTypeDef,
+    UpdateRoleDescriptionResponseOutputTypeDef,
+    GetServiceLastAccessedDetailsResponseOutputTypeDef,
+    CreateVirtualMFADeviceResponseOutputTypeDef,
+    ListVirtualMFADevicesResponseOutputTypeDef,
+    EvaluationResultOutputTypeDef,
+    CreateInstanceProfileResponseOutputTypeDef,
+    GetInstanceProfileResponseOutputTypeDef,
+    ListInstanceProfilesForRoleResponseOutputTypeDef,
+    ListInstanceProfilesResponseOutputTypeDef,
+    RoleDetailOutputTypeDef,
+    SimulatePolicyResponseOutputTypeDef,
+    GetAccountAuthorizationDetailsResponseOutputTypeDef,
 )
 
 
-def get_structure() -> AccessDetailTypeDef:
+def get_structure() -> AccessDetailOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iam-1.28.3/README.md` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-iam
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 iam type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iam"></a>
 
 # mypy-boto3-iam
 
 [![PyPI - mypy-boto3-iam](https://img.shields.io/pypi/v/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/)
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
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -607,18 +639,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_iam.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iam.type_defs import (
-    AccessDetailTypeDef,
-    AccessKeyLastUsedTypeDef,
-    AccessKeyMetadataTypeDef,
-    AccessKeyTypeDef,
+    AccessDetailOutputTypeDef,
+    AccessKeyLastUsedOutputTypeDef,
+    AccessKeyMetadataOutputTypeDef,
+    AccessKeyOutputTypeDef,
     AddClientIDToOpenIDConnectProviderRequestRequestTypeDef,
     AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef,
     AddRoleToInstanceProfileRequestRequestTypeDef,
     AddUserToGroupRequestGroupAddUserTypeDef,
     AddUserToGroupRequestRequestTypeDef,
     AddUserToGroupRequestUserAddGroupTypeDef,
     AttachGroupPolicyRequestGroupAttachPolicyTypeDef,
@@ -626,38 +658,39 @@
     AttachGroupPolicyRequestRequestTypeDef,
     AttachRolePolicyRequestPolicyAttachRoleTypeDef,
     AttachRolePolicyRequestRequestTypeDef,
     AttachRolePolicyRequestRoleAttachPolicyTypeDef,
     AttachUserPolicyRequestPolicyAttachUserTypeDef,
     AttachUserPolicyRequestRequestTypeDef,
     AttachUserPolicyRequestUserAttachPolicyTypeDef,
+    AttachedPermissionsBoundaryOutputTypeDef,
     AttachedPermissionsBoundaryResponseMetadataTypeDef,
-    AttachedPermissionsBoundaryTypeDef,
-    AttachedPolicyTypeDef,
+    AttachedPolicyOutputTypeDef,
     ChangePasswordRequestRequestTypeDef,
     ChangePasswordRequestServiceResourceChangePasswordTypeDef,
     ContextEntryTypeDef,
     CreateAccessKeyRequestRequestTypeDef,
     CreateAccountAliasRequestRequestTypeDef,
     CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef,
     CreateGroupRequestGroupCreateTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateGroupRequestServiceResourceCreateGroupTypeDef,
-    GroupTypeDef,
+    GroupOutputTypeDef,
     TagTypeDef,
     CreateLoginProfileRequestLoginProfileCreateTypeDef,
     CreateLoginProfileRequestRequestTypeDef,
     CreateLoginProfileRequestUserCreateLoginProfileTypeDef,
-    LoginProfileTypeDef,
+    LoginProfileOutputTypeDef,
+    TagOutputTypeDef,
     CreatePolicyVersionRequestPolicyCreateVersionTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    PolicyVersionTypeDef,
+    PolicyVersionOutputTypeDef,
     CreateServiceLinkedRoleRequestRequestTypeDef,
     CreateServiceSpecificCredentialRequestRequestTypeDef,
-    ServiceSpecificCredentialTypeDef,
+    ServiceSpecificCredentialOutputTypeDef,
     DeactivateMFADeviceRequestRequestTypeDef,
     DeleteAccessKeyRequestRequestTypeDef,
     DeleteAccountAliasRequestRequestTypeDef,
     DeleteGroupPolicyRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
     DeleteLoginProfileRequestRequestTypeDef,
@@ -667,159 +700,159 @@
     DeleteRolePermissionsBoundaryRequestRequestTypeDef,
     DeleteRolePolicyRequestRequestTypeDef,
     DeleteRoleRequestRequestTypeDef,
     DeleteSAMLProviderRequestRequestTypeDef,
     DeleteSSHPublicKeyRequestRequestTypeDef,
     DeleteServerCertificateRequestRequestTypeDef,
     DeleteServiceLinkedRoleRequestRequestTypeDef,
-    DeleteServiceLinkedRoleResponseTypeDef,
+    DeleteServiceLinkedRoleResponseOutputTypeDef,
     DeleteServiceSpecificCredentialRequestRequestTypeDef,
     DeleteSigningCertificateRequestRequestTypeDef,
     DeleteUserPermissionsBoundaryRequestRequestTypeDef,
     DeleteUserPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVirtualMFADeviceRequestRequestTypeDef,
-    RoleUsageTypeTypeDef,
+    RoleUsageTypeOutputTypeDef,
     DetachGroupPolicyRequestGroupDetachPolicyTypeDef,
     DetachGroupPolicyRequestPolicyDetachGroupTypeDef,
     DetachGroupPolicyRequestRequestTypeDef,
     DetachRolePolicyRequestPolicyDetachRoleTypeDef,
     DetachRolePolicyRequestRequestTypeDef,
     DetachRolePolicyRequestRoleDetachPolicyTypeDef,
     DetachUserPolicyRequestPolicyDetachUserTypeDef,
     DetachUserPolicyRequestRequestTypeDef,
     DetachUserPolicyRequestUserDetachPolicyTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableMFADeviceRequestMfaDeviceAssociateTypeDef,
     EnableMFADeviceRequestRequestTypeDef,
     EnableMFADeviceRequestUserEnableMfaTypeDef,
-    EntityInfoTypeDef,
-    ErrorDetailsTypeDef,
-    OrganizationsDecisionDetailTypeDef,
-    PermissionsBoundaryDecisionDetailTypeDef,
-    GenerateCredentialReportResponseTypeDef,
+    EntityInfoOutputTypeDef,
+    ErrorDetailsOutputTypeDef,
+    OrganizationsDecisionDetailOutputTypeDef,
+    PermissionsBoundaryDecisionDetailOutputTypeDef,
+    GenerateCredentialReportResponseOutputTypeDef,
     GenerateOrganizationsAccessReportRequestRequestTypeDef,
-    GenerateOrganizationsAccessReportResponseTypeDef,
+    GenerateOrganizationsAccessReportResponseOutputTypeDef,
     GenerateServiceLastAccessedDetailsRequestRequestTypeDef,
-    GenerateServiceLastAccessedDetailsResponseTypeDef,
+    GenerateServiceLastAccessedDetailsResponseOutputTypeDef,
     GetAccessKeyLastUsedRequestRequestTypeDef,
     GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
     GetAccountAuthorizationDetailsRequestRequestTypeDef,
-    PasswordPolicyTypeDef,
-    GetAccountSummaryResponseTypeDef,
+    PasswordPolicyOutputTypeDef,
+    GetAccountSummaryResponseOutputTypeDef,
     GetContextKeysForCustomPolicyRequestRequestTypeDef,
-    GetContextKeysForPolicyResponseTypeDef,
+    GetContextKeysForPolicyResponseOutputTypeDef,
     GetContextKeysForPrincipalPolicyRequestRequestTypeDef,
-    GetCredentialReportResponseTypeDef,
+    GetCredentialReportResponseOutputTypeDef,
     GetGroupPolicyRequestRequestTypeDef,
-    GetGroupPolicyResponseTypeDef,
+    GetGroupPolicyResponseOutputTypeDef,
     GetGroupRequestGetGroupPaginateTypeDef,
     GetGroupRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetLoginProfileRequestRequestTypeDef,
     GetMFADeviceRequestRequestTypeDef,
-    GetMFADeviceResponseTypeDef,
+    GetMFADeviceResponseOutputTypeDef,
     GetOpenIDConnectProviderRequestRequestTypeDef,
     GetOrganizationsAccessReportRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
     GetRolePolicyRequestRequestTypeDef,
-    GetRolePolicyResponseTypeDef,
+    GetRolePolicyResponseOutputTypeDef,
     GetRoleRequestRequestTypeDef,
     GetSAMLProviderRequestRequestTypeDef,
     GetSSHPublicKeyRequestRequestTypeDef,
-    SSHPublicKeyTypeDef,
+    SSHPublicKeyOutputTypeDef,
     GetServerCertificateRequestRequestTypeDef,
     GetServiceLastAccessedDetailsRequestRequestTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
     GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef,
     GetUserPolicyRequestRequestTypeDef,
-    GetUserPolicyResponseTypeDef,
+    GetUserPolicyResponseOutputTypeDef,
     GetUserRequestRequestTypeDef,
-    PolicyDetailTypeDef,
+    PolicyDetailOutputTypeDef,
     ListAccessKeysRequestListAccessKeysPaginateTypeDef,
     ListAccessKeysRequestRequestTypeDef,
     ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
     ListAccountAliasesRequestRequestTypeDef,
-    ListAccountAliasesResponseTypeDef,
+    ListAccountAliasesResponseOutputTypeDef,
     ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
     ListAttachedGroupPoliciesRequestRequestTypeDef,
     ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
     ListAttachedRolePoliciesRequestRequestTypeDef,
     ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
     ListAttachedUserPoliciesRequestRequestTypeDef,
     ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
     ListEntitiesForPolicyRequestRequestTypeDef,
-    PolicyGroupTypeDef,
-    PolicyRoleTypeDef,
-    PolicyUserTypeDef,
+    PolicyGroupOutputTypeDef,
+    PolicyRoleOutputTypeDef,
+    PolicyUserOutputTypeDef,
     ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
     ListGroupPoliciesRequestRequestTypeDef,
-    ListGroupPoliciesResponseTypeDef,
+    ListGroupPoliciesResponseOutputTypeDef,
     ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
     ListGroupsForUserRequestRequestTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
     ListInstanceProfileTagsRequestRequestTypeDef,
     ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
     ListInstanceProfilesForRoleRequestRequestTypeDef,
     ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
     ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
     ListMFADeviceTagsRequestRequestTypeDef,
     ListMFADevicesRequestListMFADevicesPaginateTypeDef,
     ListMFADevicesRequestRequestTypeDef,
-    MFADeviceTypeDef,
+    MFADeviceOutputTypeDef,
     ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
     ListOpenIDConnectProviderTagsRequestRequestTypeDef,
-    OpenIDConnectProviderListEntryTypeDef,
-    PolicyGrantingServiceAccessTypeDef,
+    OpenIDConnectProviderListEntryOutputTypeDef,
+    PolicyGrantingServiceAccessOutputTypeDef,
     ListPoliciesGrantingServiceAccessRequestRequestTypeDef,
     ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
     ListPolicyTagsRequestRequestTypeDef,
     ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
     ListRolePoliciesRequestRequestTypeDef,
-    ListRolePoliciesResponseTypeDef,
+    ListRolePoliciesResponseOutputTypeDef,
     ListRoleTagsRequestListRoleTagsPaginateTypeDef,
     ListRoleTagsRequestRequestTypeDef,
     ListRolesRequestListRolesPaginateTypeDef,
     ListRolesRequestRequestTypeDef,
     ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
     ListSAMLProviderTagsRequestRequestTypeDef,
-    SAMLProviderListEntryTypeDef,
+    SAMLProviderListEntryOutputTypeDef,
     ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
     ListSSHPublicKeysRequestRequestTypeDef,
-    SSHPublicKeyMetadataTypeDef,
+    SSHPublicKeyMetadataOutputTypeDef,
     ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
     ListServerCertificateTagsRequestRequestTypeDef,
     ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
     ListServerCertificatesRequestRequestTypeDef,
-    ServerCertificateMetadataTypeDef,
+    ServerCertificateMetadataOutputTypeDef,
     ListServiceSpecificCredentialsRequestRequestTypeDef,
-    ServiceSpecificCredentialMetadataTypeDef,
+    ServiceSpecificCredentialMetadataOutputTypeDef,
     ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
     ListSigningCertificatesRequestRequestTypeDef,
-    SigningCertificateTypeDef,
+    SigningCertificateOutputTypeDef,
     ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
     ListUserPoliciesRequestRequestTypeDef,
-    ListUserPoliciesResponseTypeDef,
+    ListUserPoliciesResponseOutputTypeDef,
     ListUserTagsRequestListUserTagsPaginateTypeDef,
     ListUserTagsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
     ListVirtualMFADevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    PositionTypeDef,
+    PositionOutputTypeDef,
     PutGroupPolicyRequestGroupCreatePolicyTypeDef,
     PutGroupPolicyRequestGroupPolicyPutTypeDef,
     PutGroupPolicyRequestRequestTypeDef,
     PutRolePermissionsBoundaryRequestRequestTypeDef,
     PutRolePolicyRequestRequestTypeDef,
     PutRolePolicyRequestRolePolicyPutTypeDef,
     PutUserPermissionsBoundaryRequestRequestTypeDef,
@@ -832,18 +865,18 @@
     RemoveUserFromGroupRequestGroupRemoveUserTypeDef,
     RemoveUserFromGroupRequestRequestTypeDef,
     RemoveUserFromGroupRequestUserRemoveGroupTypeDef,
     ResetServiceSpecificCredentialRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ResyncMFADeviceRequestMfaDeviceResyncTypeDef,
     ResyncMFADeviceRequestRequestTypeDef,
-    RoleLastUsedTypeDef,
+    RoleLastUsedOutputTypeDef,
     RoleLastUsedResponseMetadataTypeDef,
     ServerCertificateMetadataResponseMetadataTypeDef,
-    TrackedActionLastAccessedTypeDef,
+    TrackedActionLastAccessedOutputTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetSecurityTokenServicePreferencesRequestRequestTypeDef,
     UntagInstanceProfileRequestRequestTypeDef,
     UntagMFADeviceRequestRequestTypeDef,
     UntagOpenIDConnectProviderRequestRequestTypeDef,
     UntagPolicyRequestRequestTypeDef,
     UntagRoleRequestRequestTypeDef,
@@ -865,148 +898,148 @@
     UpdateLoginProfileRequestLoginProfileUpdateTypeDef,
     UpdateLoginProfileRequestRequestTypeDef,
     UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef,
     UpdateRoleDescriptionRequestRequestTypeDef,
     UpdateRoleRequestRequestTypeDef,
     UpdateSAMLProviderRequestRequestTypeDef,
     UpdateSAMLProviderRequestSamlProviderUpdateTypeDef,
-    UpdateSAMLProviderResponseTypeDef,
+    UpdateSAMLProviderResponseOutputTypeDef,
     UpdateSSHPublicKeyRequestRequestTypeDef,
     UpdateServerCertificateRequestRequestTypeDef,
     UpdateServerCertificateRequestServerCertificateUpdateTypeDef,
     UpdateServiceSpecificCredentialRequestRequestTypeDef,
     UpdateSigningCertificateRequestRequestTypeDef,
     UpdateSigningCertificateRequestSigningCertificateActivateTypeDef,
     UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserRequestUserUpdateTypeDef,
     UploadSSHPublicKeyRequestRequestTypeDef,
     UploadSigningCertificateRequestRequestTypeDef,
     UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
-    GetAccessKeyLastUsedResponseTypeDef,
-    ListAccessKeysResponseTypeDef,
-    CreateAccessKeyResponseTypeDef,
-    ListAttachedGroupPoliciesResponseTypeDef,
-    ListAttachedRolePoliciesResponseTypeDef,
-    ListAttachedUserPoliciesResponseTypeDef,
+    GetAccessKeyLastUsedResponseOutputTypeDef,
+    ListAccessKeysResponseOutputTypeDef,
+    CreateAccessKeyResponseOutputTypeDef,
+    ListAttachedGroupPoliciesResponseOutputTypeDef,
+    ListAttachedRolePoliciesResponseOutputTypeDef,
+    ListAttachedUserPoliciesResponseOutputTypeDef,
     SimulateCustomPolicyRequestRequestTypeDef,
     SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
     SimulatePrincipalPolicyRequestRequestTypeDef,
     SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
-    CreateGroupResponseTypeDef,
-    ListGroupsForUserResponseTypeDef,
-    ListGroupsResponseTypeDef,
+    CreateGroupResponseOutputTypeDef,
+    ListGroupsForUserResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
     CreateOpenIDConnectProviderRequestRequestTypeDef,
-    CreateOpenIDConnectProviderResponseTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreatePolicyRequestServiceResourceCreatePolicyTypeDef,
     CreateRoleRequestRequestTypeDef,
     CreateRoleRequestServiceResourceCreateRoleTypeDef,
     CreateSAMLProviderRequestRequestTypeDef,
     CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef,
-    CreateSAMLProviderResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     CreateUserRequestServiceResourceCreateUserTypeDef,
     CreateUserRequestUserCreateTypeDef,
     CreateVirtualMFADeviceRequestRequestTypeDef,
     CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef,
-    GetOpenIDConnectProviderResponseTypeDef,
-    GetSAMLProviderResponseTypeDef,
-    ListInstanceProfileTagsResponseTypeDef,
-    ListMFADeviceTagsResponseTypeDef,
-    ListOpenIDConnectProviderTagsResponseTypeDef,
-    ListPolicyTagsResponseTypeDef,
-    ListRoleTagsResponseTypeDef,
-    ListSAMLProviderTagsResponseTypeDef,
-    ListServerCertificateTagsResponseTypeDef,
-    ListUserTagsResponseTypeDef,
-    PolicyTypeDef,
     TagInstanceProfileRequestRequestTypeDef,
     TagMFADeviceRequestRequestTypeDef,
     TagOpenIDConnectProviderRequestRequestTypeDef,
     TagPolicyRequestRequestTypeDef,
     TagRoleRequestRequestTypeDef,
     TagSAMLProviderRequestRequestTypeDef,
     TagServerCertificateRequestRequestTypeDef,
     TagUserRequestRequestTypeDef,
     UploadServerCertificateRequestRequestTypeDef,
     UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
+    CreateLoginProfileResponseOutputTypeDef,
+    GetLoginProfileResponseOutputTypeDef,
+    CreateOpenIDConnectProviderResponseOutputTypeDef,
+    CreateSAMLProviderResponseOutputTypeDef,
+    GetOpenIDConnectProviderResponseOutputTypeDef,
+    GetSAMLProviderResponseOutputTypeDef,
+    ListInstanceProfileTagsResponseOutputTypeDef,
+    ListMFADeviceTagsResponseOutputTypeDef,
+    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
+    ListPolicyTagsResponseOutputTypeDef,
+    ListRoleTagsResponseOutputTypeDef,
+    ListSAMLProviderTagsResponseOutputTypeDef,
+    ListServerCertificateTagsResponseOutputTypeDef,
+    ListUserTagsResponseOutputTypeDef,
+    PolicyOutputTypeDef,
+    UserOutputTypeDef,
     UserResponseMetadataTypeDef,
-    UserTypeDef,
-    CreateLoginProfileResponseTypeDef,
-    GetLoginProfileResponseTypeDef,
-    CreatePolicyVersionResponseTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    ListPolicyVersionsResponseTypeDef,
-    ManagedPolicyDetailTypeDef,
-    CreateServiceSpecificCredentialResponseTypeDef,
-    ResetServiceSpecificCredentialResponseTypeDef,
-    DeletionTaskFailureReasonTypeTypeDef,
-    EntityDetailsTypeDef,
-    GetOrganizationsAccessReportResponseTypeDef,
-    GetAccountPasswordPolicyResponseTypeDef,
+    CreatePolicyVersionResponseOutputTypeDef,
+    GetPolicyVersionResponseOutputTypeDef,
+    ListPolicyVersionsResponseOutputTypeDef,
+    ManagedPolicyDetailOutputTypeDef,
+    CreateServiceSpecificCredentialResponseOutputTypeDef,
+    ResetServiceSpecificCredentialResponseOutputTypeDef,
+    DeletionTaskFailureReasonTypeOutputTypeDef,
+    EntityDetailsOutputTypeDef,
+    GetOrganizationsAccessReportResponseOutputTypeDef,
+    GetAccountPasswordPolicyResponseOutputTypeDef,
     GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
     GetPolicyRequestPolicyExistsWaitTypeDef,
     GetRoleRequestRoleExistsWaitTypeDef,
     GetUserRequestUserExistsWaitTypeDef,
-    GetSSHPublicKeyResponseTypeDef,
-    UploadSSHPublicKeyResponseTypeDef,
-    GroupDetailTypeDef,
-    UserDetailTypeDef,
-    ListEntitiesForPolicyResponseTypeDef,
-    ListMFADevicesResponseTypeDef,
-    ListOpenIDConnectProvidersResponseTypeDef,
-    ListPoliciesGrantingServiceAccessEntryTypeDef,
-    ListSAMLProvidersResponseTypeDef,
-    ListSSHPublicKeysResponseTypeDef,
-    ListServerCertificatesResponseTypeDef,
-    ServerCertificateTypeDef,
-    UploadServerCertificateResponseTypeDef,
-    ListServiceSpecificCredentialsResponseTypeDef,
-    ListSigningCertificatesResponseTypeDef,
-    UploadSigningCertificateResponseTypeDef,
-    StatementTypeDef,
-    RoleTypeDef,
-    ServiceLastAccessedTypeDef,
-    CreatePolicyResponseTypeDef,
-    GetPolicyResponseTypeDef,
-    ListPoliciesResponseTypeDef,
-    CreateUserResponseTypeDef,
-    GetGroupResponseTypeDef,
-    GetUserResponseTypeDef,
-    ListUsersResponseTypeDef,
-    VirtualMFADeviceTypeDef,
-    GetServiceLinkedRoleDeletionStatusResponseTypeDef,
-    GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
-    ListPoliciesGrantingServiceAccessResponseTypeDef,
-    GetServerCertificateResponseTypeDef,
-    ResourceSpecificResultTypeDef,
-    CreateRoleResponseTypeDef,
-    CreateServiceLinkedRoleResponseTypeDef,
-    GetRoleResponseTypeDef,
-    InstanceProfileTypeDef,
-    ListRolesResponseTypeDef,
-    UpdateRoleDescriptionResponseTypeDef,
-    GetServiceLastAccessedDetailsResponseTypeDef,
-    CreateVirtualMFADeviceResponseTypeDef,
-    ListVirtualMFADevicesResponseTypeDef,
-    EvaluationResultTypeDef,
-    CreateInstanceProfileResponseTypeDef,
-    GetInstanceProfileResponseTypeDef,
-    ListInstanceProfilesForRoleResponseTypeDef,
-    ListInstanceProfilesResponseTypeDef,
-    RoleDetailTypeDef,
-    SimulatePolicyResponseTypeDef,
-    GetAccountAuthorizationDetailsResponseTypeDef,
+    GetSSHPublicKeyResponseOutputTypeDef,
+    UploadSSHPublicKeyResponseOutputTypeDef,
+    GroupDetailOutputTypeDef,
+    UserDetailOutputTypeDef,
+    ListEntitiesForPolicyResponseOutputTypeDef,
+    ListMFADevicesResponseOutputTypeDef,
+    ListOpenIDConnectProvidersResponseOutputTypeDef,
+    ListPoliciesGrantingServiceAccessEntryOutputTypeDef,
+    ListSAMLProvidersResponseOutputTypeDef,
+    ListSSHPublicKeysResponseOutputTypeDef,
+    ListServerCertificatesResponseOutputTypeDef,
+    ServerCertificateOutputTypeDef,
+    UploadServerCertificateResponseOutputTypeDef,
+    ListServiceSpecificCredentialsResponseOutputTypeDef,
+    ListSigningCertificatesResponseOutputTypeDef,
+    UploadSigningCertificateResponseOutputTypeDef,
+    StatementOutputTypeDef,
+    RoleOutputTypeDef,
+    ServiceLastAccessedOutputTypeDef,
+    CreatePolicyResponseOutputTypeDef,
+    GetPolicyResponseOutputTypeDef,
+    ListPoliciesResponseOutputTypeDef,
+    CreateUserResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    GetUserResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
+    VirtualMFADeviceOutputTypeDef,
+    GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef,
+    GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef,
+    ListPoliciesGrantingServiceAccessResponseOutputTypeDef,
+    GetServerCertificateResponseOutputTypeDef,
+    ResourceSpecificResultOutputTypeDef,
+    CreateRoleResponseOutputTypeDef,
+    CreateServiceLinkedRoleResponseOutputTypeDef,
+    GetRoleResponseOutputTypeDef,
+    InstanceProfileOutputTypeDef,
+    ListRolesResponseOutputTypeDef,
+    UpdateRoleDescriptionResponseOutputTypeDef,
+    GetServiceLastAccessedDetailsResponseOutputTypeDef,
+    CreateVirtualMFADeviceResponseOutputTypeDef,
+    ListVirtualMFADevicesResponseOutputTypeDef,
+    EvaluationResultOutputTypeDef,
+    CreateInstanceProfileResponseOutputTypeDef,
+    GetInstanceProfileResponseOutputTypeDef,
+    ListInstanceProfilesForRoleResponseOutputTypeDef,
+    ListInstanceProfilesResponseOutputTypeDef,
+    RoleDetailOutputTypeDef,
+    SimulatePolicyResponseOutputTypeDef,
+    GetAccountAuthorizationDetailsResponseOutputTypeDef,
 )
 
 
-def get_structure() -> AccessDetailTypeDef:
+def get_structure() -> AccessDetailOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/__init__.py` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/__init__.pyi` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/__main__.py` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAM 1.28.3\nVersion:         1.28.3\nBuilder version:"
-        " 7.14.6\nDocs:           "
+        "Type annotations for boto3.IAM 1.28.3\nVersion:         1.28.3.post1\nBuilder version:"
+        " 7.14.7\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM\nOther"
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

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/client.py` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,99 +63,99 @@
     ListUserTagsPaginator,
     ListVirtualMFADevicesPaginator,
     SimulateCustomPolicyPaginator,
     SimulatePrincipalPolicyPaginator,
 )
 from .type_defs import (
     ContextEntryTypeDef,
-    CreateAccessKeyResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    CreateInstanceProfileResponseTypeDef,
-    CreateLoginProfileResponseTypeDef,
-    CreateOpenIDConnectProviderResponseTypeDef,
-    CreatePolicyResponseTypeDef,
-    CreatePolicyVersionResponseTypeDef,
-    CreateRoleResponseTypeDef,
-    CreateSAMLProviderResponseTypeDef,
-    CreateServiceLinkedRoleResponseTypeDef,
-    CreateServiceSpecificCredentialResponseTypeDef,
-    CreateUserResponseTypeDef,
-    CreateVirtualMFADeviceResponseTypeDef,
-    DeleteServiceLinkedRoleResponseTypeDef,
+    CreateAccessKeyResponseOutputTypeDef,
+    CreateGroupResponseOutputTypeDef,
+    CreateInstanceProfileResponseOutputTypeDef,
+    CreateLoginProfileResponseOutputTypeDef,
+    CreateOpenIDConnectProviderResponseOutputTypeDef,
+    CreatePolicyResponseOutputTypeDef,
+    CreatePolicyVersionResponseOutputTypeDef,
+    CreateRoleResponseOutputTypeDef,
+    CreateSAMLProviderResponseOutputTypeDef,
+    CreateServiceLinkedRoleResponseOutputTypeDef,
+    CreateServiceSpecificCredentialResponseOutputTypeDef,
+    CreateUserResponseOutputTypeDef,
+    CreateVirtualMFADeviceResponseOutputTypeDef,
+    DeleteServiceLinkedRoleResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
-    GenerateCredentialReportResponseTypeDef,
-    GenerateOrganizationsAccessReportResponseTypeDef,
-    GenerateServiceLastAccessedDetailsResponseTypeDef,
-    GetAccessKeyLastUsedResponseTypeDef,
-    GetAccountAuthorizationDetailsResponseTypeDef,
-    GetAccountPasswordPolicyResponseTypeDef,
-    GetAccountSummaryResponseTypeDef,
-    GetContextKeysForPolicyResponseTypeDef,
-    GetCredentialReportResponseTypeDef,
-    GetGroupPolicyResponseTypeDef,
-    GetGroupResponseTypeDef,
-    GetInstanceProfileResponseTypeDef,
-    GetLoginProfileResponseTypeDef,
-    GetMFADeviceResponseTypeDef,
-    GetOpenIDConnectProviderResponseTypeDef,
-    GetOrganizationsAccessReportResponseTypeDef,
-    GetPolicyResponseTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    GetRolePolicyResponseTypeDef,
-    GetRoleResponseTypeDef,
-    GetSAMLProviderResponseTypeDef,
-    GetServerCertificateResponseTypeDef,
-    GetServiceLastAccessedDetailsResponseTypeDef,
-    GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
-    GetServiceLinkedRoleDeletionStatusResponseTypeDef,
-    GetSSHPublicKeyResponseTypeDef,
-    GetUserPolicyResponseTypeDef,
-    GetUserResponseTypeDef,
-    ListAccessKeysResponseTypeDef,
-    ListAccountAliasesResponseTypeDef,
-    ListAttachedGroupPoliciesResponseTypeDef,
-    ListAttachedRolePoliciesResponseTypeDef,
-    ListAttachedUserPoliciesResponseTypeDef,
-    ListEntitiesForPolicyResponseTypeDef,
-    ListGroupPoliciesResponseTypeDef,
-    ListGroupsForUserResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    ListInstanceProfilesForRoleResponseTypeDef,
-    ListInstanceProfilesResponseTypeDef,
-    ListInstanceProfileTagsResponseTypeDef,
-    ListMFADevicesResponseTypeDef,
-    ListMFADeviceTagsResponseTypeDef,
-    ListOpenIDConnectProvidersResponseTypeDef,
-    ListOpenIDConnectProviderTagsResponseTypeDef,
-    ListPoliciesGrantingServiceAccessResponseTypeDef,
-    ListPoliciesResponseTypeDef,
-    ListPolicyTagsResponseTypeDef,
-    ListPolicyVersionsResponseTypeDef,
-    ListRolePoliciesResponseTypeDef,
-    ListRolesResponseTypeDef,
-    ListRoleTagsResponseTypeDef,
-    ListSAMLProvidersResponseTypeDef,
-    ListSAMLProviderTagsResponseTypeDef,
-    ListServerCertificatesResponseTypeDef,
-    ListServerCertificateTagsResponseTypeDef,
-    ListServiceSpecificCredentialsResponseTypeDef,
-    ListSigningCertificatesResponseTypeDef,
-    ListSSHPublicKeysResponseTypeDef,
-    ListUserPoliciesResponseTypeDef,
-    ListUsersResponseTypeDef,
-    ListUserTagsResponseTypeDef,
-    ListVirtualMFADevicesResponseTypeDef,
-    ResetServiceSpecificCredentialResponseTypeDef,
-    SimulatePolicyResponseTypeDef,
+    GenerateCredentialReportResponseOutputTypeDef,
+    GenerateOrganizationsAccessReportResponseOutputTypeDef,
+    GenerateServiceLastAccessedDetailsResponseOutputTypeDef,
+    GetAccessKeyLastUsedResponseOutputTypeDef,
+    GetAccountAuthorizationDetailsResponseOutputTypeDef,
+    GetAccountPasswordPolicyResponseOutputTypeDef,
+    GetAccountSummaryResponseOutputTypeDef,
+    GetContextKeysForPolicyResponseOutputTypeDef,
+    GetCredentialReportResponseOutputTypeDef,
+    GetGroupPolicyResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    GetInstanceProfileResponseOutputTypeDef,
+    GetLoginProfileResponseOutputTypeDef,
+    GetMFADeviceResponseOutputTypeDef,
+    GetOpenIDConnectProviderResponseOutputTypeDef,
+    GetOrganizationsAccessReportResponseOutputTypeDef,
+    GetPolicyResponseOutputTypeDef,
+    GetPolicyVersionResponseOutputTypeDef,
+    GetRolePolicyResponseOutputTypeDef,
+    GetRoleResponseOutputTypeDef,
+    GetSAMLProviderResponseOutputTypeDef,
+    GetServerCertificateResponseOutputTypeDef,
+    GetServiceLastAccessedDetailsResponseOutputTypeDef,
+    GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef,
+    GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef,
+    GetSSHPublicKeyResponseOutputTypeDef,
+    GetUserPolicyResponseOutputTypeDef,
+    GetUserResponseOutputTypeDef,
+    ListAccessKeysResponseOutputTypeDef,
+    ListAccountAliasesResponseOutputTypeDef,
+    ListAttachedGroupPoliciesResponseOutputTypeDef,
+    ListAttachedRolePoliciesResponseOutputTypeDef,
+    ListAttachedUserPoliciesResponseOutputTypeDef,
+    ListEntitiesForPolicyResponseOutputTypeDef,
+    ListGroupPoliciesResponseOutputTypeDef,
+    ListGroupsForUserResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
+    ListInstanceProfilesForRoleResponseOutputTypeDef,
+    ListInstanceProfilesResponseOutputTypeDef,
+    ListInstanceProfileTagsResponseOutputTypeDef,
+    ListMFADevicesResponseOutputTypeDef,
+    ListMFADeviceTagsResponseOutputTypeDef,
+    ListOpenIDConnectProvidersResponseOutputTypeDef,
+    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
+    ListPoliciesGrantingServiceAccessResponseOutputTypeDef,
+    ListPoliciesResponseOutputTypeDef,
+    ListPolicyTagsResponseOutputTypeDef,
+    ListPolicyVersionsResponseOutputTypeDef,
+    ListRolePoliciesResponseOutputTypeDef,
+    ListRolesResponseOutputTypeDef,
+    ListRoleTagsResponseOutputTypeDef,
+    ListSAMLProvidersResponseOutputTypeDef,
+    ListSAMLProviderTagsResponseOutputTypeDef,
+    ListServerCertificatesResponseOutputTypeDef,
+    ListServerCertificateTagsResponseOutputTypeDef,
+    ListServiceSpecificCredentialsResponseOutputTypeDef,
+    ListSigningCertificatesResponseOutputTypeDef,
+    ListSSHPublicKeysResponseOutputTypeDef,
+    ListUserPoliciesResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
+    ListUserTagsResponseOutputTypeDef,
+    ListVirtualMFADevicesResponseOutputTypeDef,
+    ResetServiceSpecificCredentialResponseOutputTypeDef,
+    SimulatePolicyResponseOutputTypeDef,
     TagTypeDef,
-    UpdateRoleDescriptionResponseTypeDef,
-    UpdateSAMLProviderResponseTypeDef,
-    UploadServerCertificateResponseTypeDef,
-    UploadSigningCertificateResponseTypeDef,
-    UploadSSHPublicKeyResponseTypeDef,
+    UpdateRoleDescriptionResponseOutputTypeDef,
+    UpdateSAMLProviderResponseOutputTypeDef,
+    UploadServerCertificateResponseOutputTypeDef,
+    UploadSigningCertificateResponseOutputTypeDef,
+    UploadSSHPublicKeyResponseOutputTypeDef,
 )
 from .waiter import (
     InstanceProfileExistsWaiter,
     PolicyExistsWaiter,
     RoleExistsWaiter,
     UserExistsWaiter,
 )
@@ -302,15 +302,15 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#close)
         """
 
-    def create_access_key(self, *, UserName: str = ...) -> CreateAccessKeyResponseTypeDef:
+    def create_access_key(self, *, UserName: str = ...) -> CreateAccessKeyResponseOutputTypeDef:
         """
         Creates a new Amazon Web Services secret access key and corresponding Amazon Web
         Services access key ID for the specified user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_access_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_access_key)
         """
@@ -319,50 +319,50 @@
         """
         Creates an alias for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_account_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_account_alias)
         """
 
-    def create_group(self, *, GroupName: str, Path: str = ...) -> CreateGroupResponseTypeDef:
+    def create_group(self, *, GroupName: str, Path: str = ...) -> CreateGroupResponseOutputTypeDef:
         """
         Creates a new group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_group)
         """
 
     def create_instance_profile(
         self, *, InstanceProfileName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateInstanceProfileResponseTypeDef:
+    ) -> CreateInstanceProfileResponseOutputTypeDef:
         """
         Creates a new instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_instance_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_instance_profile)
         """
 
     def create_login_profile(
         self, *, UserName: str, Password: str, PasswordResetRequired: bool = ...
-    ) -> CreateLoginProfileResponseTypeDef:
+    ) -> CreateLoginProfileResponseOutputTypeDef:
         """
         Creates a password for the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_login_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_login_profile)
         """
 
     def create_open_id_connect_provider(
         self,
         *,
         Url: str,
         ThumbprintList: Sequence[str],
         ClientIDList: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateOpenIDConnectProviderResponseTypeDef:
+    ) -> CreateOpenIDConnectProviderResponseOutputTypeDef:
         """
         Creates an IAM entity to describe an identity provider (IdP) that supports
         `OpenID Connect (OIDC) <http://openid.net/connect/>`__.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_open_id_connect_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_open_id_connect_provider)
         """
@@ -371,25 +371,25 @@
         self,
         *,
         PolicyName: str,
         PolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreatePolicyResponseTypeDef:
+    ) -> CreatePolicyResponseOutputTypeDef:
         """
         Creates a new managed policy for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_policy)
         """
 
     def create_policy_version(
         self, *, PolicyArn: str, PolicyDocument: str, SetAsDefault: bool = ...
-    ) -> CreatePolicyVersionResponseTypeDef:
+    ) -> CreatePolicyVersionResponseOutputTypeDef:
         """
         Creates a new version of the specified managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_policy_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_policy_version)
         """
 
@@ -399,46 +399,46 @@
         RoleName: str,
         AssumeRolePolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         MaxSessionDuration: int = ...,
         PermissionsBoundary: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRoleResponseTypeDef:
+    ) -> CreateRoleResponseOutputTypeDef:
         """
         Creates a new role for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_role)
         """
 
     def create_saml_provider(
         self, *, SAMLMetadataDocument: str, Name: str, Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSAMLProviderResponseTypeDef:
+    ) -> CreateSAMLProviderResponseOutputTypeDef:
         """
         Creates an IAM resource that describes an identity provider (IdP) that supports
         SAML 2.0.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_saml_provider)
         """
 
     def create_service_linked_role(
         self, *, AWSServiceName: str, Description: str = ..., CustomSuffix: str = ...
-    ) -> CreateServiceLinkedRoleResponseTypeDef:
+    ) -> CreateServiceLinkedRoleResponseOutputTypeDef:
         """
         Creates an IAM role that is linked to a specific Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_service_linked_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_service_linked_role)
         """
 
     def create_service_specific_credential(
         self, *, UserName: str, ServiceName: str
-    ) -> CreateServiceSpecificCredentialResponseTypeDef:
+    ) -> CreateServiceSpecificCredentialResponseOutputTypeDef:
         """
         Generates a set of credentials consisting of a user name and password that can
         be used to access the service specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_service_specific_credential)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_service_specific_credential)
         """
@@ -446,25 +446,25 @@
     def create_user(
         self,
         *,
         UserName: str,
         Path: str = ...,
         PermissionsBoundary: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateUserResponseTypeDef:
+    ) -> CreateUserResponseOutputTypeDef:
         """
         Creates a new IAM user for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_user)
         """
 
     def create_virtual_mfa_device(
         self, *, VirtualMFADeviceName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateVirtualMFADeviceResponseTypeDef:
+    ) -> CreateVirtualMFADeviceResponseOutputTypeDef:
         """
         Creates a new virtual MFA device for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_virtual_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_virtual_mfa_device)
         """
 
@@ -610,15 +610,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.delete_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#delete_server_certificate)
         """
 
     def delete_service_linked_role(
         self, *, RoleName: str
-    ) -> DeleteServiceLinkedRoleResponseTypeDef:
+    ) -> DeleteServiceLinkedRoleResponseOutputTypeDef:
         """
         Submits a service-linked role deletion request and returns a `DeletionTaskId`,
         which you can use to check the status of the deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.delete_service_linked_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#delete_service_linked_role)
         """
@@ -722,25 +722,25 @@
         """
         Enables the specified MFA device and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.enable_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#enable_mfa_device)
         """
 
-    def generate_credential_report(self) -> GenerateCredentialReportResponseTypeDef:
+    def generate_credential_report(self) -> GenerateCredentialReportResponseOutputTypeDef:
         """
         Generates a credential report for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_credential_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_credential_report)
         """
 
     def generate_organizations_access_report(
         self, *, EntityPath: str, OrganizationsPolicyId: str = ...
-    ) -> GenerateOrganizationsAccessReportResponseTypeDef:
+    ) -> GenerateOrganizationsAccessReportResponseOutputTypeDef:
         """
         Generates a report for service last accessed data for Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_organizations_access_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_organizations_access_report)
         """
 
@@ -756,323 +756,331 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_presigned_url)
         """
 
     def generate_service_last_accessed_details(
         self, *, Arn: str, Granularity: AccessAdvisorUsageGranularityTypeType = ...
-    ) -> GenerateServiceLastAccessedDetailsResponseTypeDef:
+    ) -> GenerateServiceLastAccessedDetailsResponseOutputTypeDef:
         """
         Generates a report that includes details about when an IAM resource (user,
         group, role, or policy) was last used in an attempt to access Amazon Web
         Services services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_service_last_accessed_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_service_last_accessed_details)
         """
 
-    def get_access_key_last_used(self, *, AccessKeyId: str) -> GetAccessKeyLastUsedResponseTypeDef:
+    def get_access_key_last_used(
+        self, *, AccessKeyId: str
+    ) -> GetAccessKeyLastUsedResponseOutputTypeDef:
         """
         Retrieves information about when the specified access key was last used.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_access_key_last_used)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_access_key_last_used)
         """
 
     def get_account_authorization_details(
         self, *, Filter: Sequence[EntityTypeType] = ..., MaxItems: int = ..., Marker: str = ...
-    ) -> GetAccountAuthorizationDetailsResponseTypeDef:
+    ) -> GetAccountAuthorizationDetailsResponseOutputTypeDef:
         """
         Retrieves information about all IAM users, groups, roles, and policies in your
         Amazon Web Services account, including their relationships to one another.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_authorization_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_authorization_details)
         """
 
-    def get_account_password_policy(self) -> GetAccountPasswordPolicyResponseTypeDef:
+    def get_account_password_policy(self) -> GetAccountPasswordPolicyResponseOutputTypeDef:
         """
         Retrieves the password policy for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_password_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_password_policy)
         """
 
-    def get_account_summary(self) -> GetAccountSummaryResponseTypeDef:
+    def get_account_summary(self) -> GetAccountSummaryResponseOutputTypeDef:
         """
         Retrieves information about IAM entity usage and IAM quotas in the Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_summary)
         """
 
     def get_context_keys_for_custom_policy(
         self, *, PolicyInputList: Sequence[str]
-    ) -> GetContextKeysForPolicyResponseTypeDef:
+    ) -> GetContextKeysForPolicyResponseOutputTypeDef:
         """
         Gets a list of all of the context keys referenced in the input policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_context_keys_for_custom_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_context_keys_for_custom_policy)
         """
 
     def get_context_keys_for_principal_policy(
         self, *, PolicySourceArn: str, PolicyInputList: Sequence[str] = ...
-    ) -> GetContextKeysForPolicyResponseTypeDef:
+    ) -> GetContextKeysForPolicyResponseOutputTypeDef:
         """
         Gets a list of all of the context keys referenced in all the IAM policies that
         are attached to the specified IAM entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_context_keys_for_principal_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_context_keys_for_principal_policy)
         """
 
-    def get_credential_report(self) -> GetCredentialReportResponseTypeDef:
+    def get_credential_report(self) -> GetCredentialReportResponseOutputTypeDef:
         """
         Retrieves a credential report for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_credential_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_credential_report)
         """
 
     def get_group(
         self, *, GroupName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> GetGroupResponseTypeDef:
+    ) -> GetGroupResponseOutputTypeDef:
         """
         Returns a list of IAM users that are in the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_group)
         """
 
-    def get_group_policy(self, *, GroupName: str, PolicyName: str) -> GetGroupPolicyResponseTypeDef:
+    def get_group_policy(
+        self, *, GroupName: str, PolicyName: str
+    ) -> GetGroupPolicyResponseOutputTypeDef:
         """
         Retrieves the specified inline policy document that is embedded in the specified
         IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_group_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_group_policy)
         """
 
     def get_instance_profile(
         self, *, InstanceProfileName: str
-    ) -> GetInstanceProfileResponseTypeDef:
+    ) -> GetInstanceProfileResponseOutputTypeDef:
         """
         Retrieves information about the specified instance profile, including the
         instance profile's path, GUID, ARN, and role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_instance_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_instance_profile)
         """
 
-    def get_login_profile(self, *, UserName: str) -> GetLoginProfileResponseTypeDef:
+    def get_login_profile(self, *, UserName: str) -> GetLoginProfileResponseOutputTypeDef:
         """
         Retrieves the user name for the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_login_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_login_profile)
         """
 
     def get_mfa_device(
         self, *, SerialNumber: str, UserName: str = ...
-    ) -> GetMFADeviceResponseTypeDef:
+    ) -> GetMFADeviceResponseOutputTypeDef:
         """
         Retrieves information about an MFA device for a specified user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_mfa_device)
         """
 
     def get_open_id_connect_provider(
         self, *, OpenIDConnectProviderArn: str
-    ) -> GetOpenIDConnectProviderResponseTypeDef:
+    ) -> GetOpenIDConnectProviderResponseOutputTypeDef:
         """
         Returns information about the specified OpenID Connect (OIDC) provider resource
         object in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_open_id_connect_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_open_id_connect_provider)
         """
 
     def get_organizations_access_report(
         self, *, JobId: str, MaxItems: int = ..., Marker: str = ..., SortKey: sortKeyTypeType = ...
-    ) -> GetOrganizationsAccessReportResponseTypeDef:
+    ) -> GetOrganizationsAccessReportResponseOutputTypeDef:
         """
         Retrieves the service last accessed data report for Organizations that was
         previously generated using the `GenerateOrganizationsAccessReport` operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_organizations_access_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_organizations_access_report)
         """
 
-    def get_policy(self, *, PolicyArn: str) -> GetPolicyResponseTypeDef:
+    def get_policy(self, *, PolicyArn: str) -> GetPolicyResponseOutputTypeDef:
         """
         Retrieves information about the specified managed policy, including the policy's
         default version and the total number of IAM users, groups, and roles to which
         the policy is attached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_policy)
         """
 
     def get_policy_version(
         self, *, PolicyArn: str, VersionId: str
-    ) -> GetPolicyVersionResponseTypeDef:
+    ) -> GetPolicyVersionResponseOutputTypeDef:
         """
         Retrieves information about the specified version of the specified managed
         policy, including the policy document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_policy_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_policy_version)
         """
 
-    def get_role(self, *, RoleName: str) -> GetRoleResponseTypeDef:
+    def get_role(self, *, RoleName: str) -> GetRoleResponseOutputTypeDef:
         """
         Retrieves information about the specified role, including the role's path, GUID,
         ARN, and the role's trust policy that grants permission to assume the role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_role)
         """
 
-    def get_role_policy(self, *, RoleName: str, PolicyName: str) -> GetRolePolicyResponseTypeDef:
+    def get_role_policy(
+        self, *, RoleName: str, PolicyName: str
+    ) -> GetRolePolicyResponseOutputTypeDef:
         """
         Retrieves the specified inline policy document that is embedded with the
         specified IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_role_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_role_policy)
         """
 
-    def get_saml_provider(self, *, SAMLProviderArn: str) -> GetSAMLProviderResponseTypeDef:
+    def get_saml_provider(self, *, SAMLProviderArn: str) -> GetSAMLProviderResponseOutputTypeDef:
         """
         Returns the SAML provider metadocument that was uploaded when the IAM SAML
         provider resource object was created or updated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_saml_provider)
         """
 
     def get_server_certificate(
         self, *, ServerCertificateName: str
-    ) -> GetServerCertificateResponseTypeDef:
+    ) -> GetServerCertificateResponseOutputTypeDef:
         """
         Retrieves information about the specified server certificate stored in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_server_certificate)
         """
 
     def get_service_last_accessed_details(
         self, *, JobId: str, MaxItems: int = ..., Marker: str = ...
-    ) -> GetServiceLastAccessedDetailsResponseTypeDef:
+    ) -> GetServiceLastAccessedDetailsResponseOutputTypeDef:
         """
         Retrieves a service last accessed report that was created using the
         `GenerateServiceLastAccessedDetails` operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_last_accessed_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_last_accessed_details)
         """
 
     def get_service_last_accessed_details_with_entities(
         self, *, JobId: str, ServiceNamespace: str, MaxItems: int = ..., Marker: str = ...
-    ) -> GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef:
+    ) -> GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef:
         """
         After you generate a group or policy report using the
         `GenerateServiceLastAccessedDetails` operation, you can use the `JobId`
         parameter in `GetServiceLastAccessedDetailsWithEntities`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_last_accessed_details_with_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_last_accessed_details_with_entities)
         """
 
     def get_service_linked_role_deletion_status(
         self, *, DeletionTaskId: str
-    ) -> GetServiceLinkedRoleDeletionStatusResponseTypeDef:
+    ) -> GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef:
         """
         Retrieves the status of your service-linked role deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_linked_role_deletion_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_linked_role_deletion_status)
         """
 
     def get_ssh_public_key(
         self, *, UserName: str, SSHPublicKeyId: str, Encoding: encodingTypeType
-    ) -> GetSSHPublicKeyResponseTypeDef:
+    ) -> GetSSHPublicKeyResponseOutputTypeDef:
         """
         Retrieves the specified SSH public key, including metadata about the key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_ssh_public_key)
         """
 
-    def get_user(self, *, UserName: str = ...) -> GetUserResponseTypeDef:
+    def get_user(self, *, UserName: str = ...) -> GetUserResponseOutputTypeDef:
         """
         Retrieves information about the specified IAM user, including the user's
         creation date, path, unique ID, and ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_user)
         """
 
-    def get_user_policy(self, *, UserName: str, PolicyName: str) -> GetUserPolicyResponseTypeDef:
+    def get_user_policy(
+        self, *, UserName: str, PolicyName: str
+    ) -> GetUserPolicyResponseOutputTypeDef:
         """
         Retrieves the specified inline policy document that is embedded in the specified
         IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_user_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_user_policy)
         """
 
     def list_access_keys(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAccessKeysResponseTypeDef:
+    ) -> ListAccessKeysResponseOutputTypeDef:
         """
         Returns information about the access key IDs associated with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_access_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_access_keys)
         """
 
     def list_account_aliases(
         self, *, Marker: str = ..., MaxItems: int = ...
-    ) -> ListAccountAliasesResponseTypeDef:
+    ) -> ListAccountAliasesResponseOutputTypeDef:
         """
         Lists the account alias associated with the Amazon Web Services account (Note:
         you can have only one).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_account_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_account_aliases)
         """
 
     def list_attached_group_policies(
         self, *, GroupName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedGroupPoliciesResponseTypeDef:
+    ) -> ListAttachedGroupPoliciesResponseOutputTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_group_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_group_policies)
         """
 
     def list_attached_role_policies(
         self, *, RoleName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedRolePoliciesResponseTypeDef:
+    ) -> ListAttachedRolePoliciesResponseOutputTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_role_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_role_policies)
         """
 
     def list_attached_user_policies(
         self, *, UserName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedUserPoliciesResponseTypeDef:
+    ) -> ListAttachedUserPoliciesResponseOutputTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_user_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_user_policies)
         """
 
@@ -1081,117 +1089,117 @@
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListEntitiesForPolicyResponseTypeDef:
+    ) -> ListEntitiesForPolicyResponseOutputTypeDef:
         """
         Lists all IAM users, groups, and roles that the specified managed policy is
         attached to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_entities_for_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_entities_for_policy)
         """
 
     def list_group_policies(
         self, *, GroupName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupPoliciesResponseTypeDef:
+    ) -> ListGroupPoliciesResponseOutputTypeDef:
         """
         Lists the names of the inline policies that are embedded in the specified IAM
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_group_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_group_policies)
         """
 
     def list_groups(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupsResponseTypeDef:
+    ) -> ListGroupsResponseOutputTypeDef:
         """
         Lists the IAM groups that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_groups)
         """
 
     def list_groups_for_user(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupsForUserResponseTypeDef:
+    ) -> ListGroupsForUserResponseOutputTypeDef:
         """
         Lists the IAM groups that the specified IAM user belongs to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_groups_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_groups_for_user)
         """
 
     def list_instance_profile_tags(
         self, *, InstanceProfileName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfileTagsResponseTypeDef:
+    ) -> ListInstanceProfileTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified IAM instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profile_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profile_tags)
         """
 
     def list_instance_profiles(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfilesResponseTypeDef:
+    ) -> ListInstanceProfilesResponseOutputTypeDef:
         """
         Lists the instance profiles that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profiles)
         """
 
     def list_instance_profiles_for_role(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfilesForRoleResponseTypeDef:
+    ) -> ListInstanceProfilesForRoleResponseOutputTypeDef:
         """
         Lists the instance profiles that have the specified associated IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profiles_for_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profiles_for_role)
         """
 
     def list_mfa_device_tags(
         self, *, SerialNumber: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListMFADeviceTagsResponseTypeDef:
+    ) -> ListMFADeviceTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified IAM virtual multi-factor
         authentication (MFA) device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_mfa_device_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_mfa_device_tags)
         """
 
     def list_mfa_devices(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListMFADevicesResponseTypeDef:
+    ) -> ListMFADevicesResponseOutputTypeDef:
         """
         Lists the MFA devices for an IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_mfa_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_mfa_devices)
         """
 
     def list_open_id_connect_provider_tags(
         self, *, OpenIDConnectProviderArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListOpenIDConnectProviderTagsResponseTypeDef:
+    ) -> ListOpenIDConnectProviderTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified OpenID Connect
         (OIDC)-compatible identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_open_id_connect_provider_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_open_id_connect_provider_tags)
         """
 
-    def list_open_id_connect_providers(self) -> ListOpenIDConnectProvidersResponseTypeDef:
+    def list_open_id_connect_providers(self) -> ListOpenIDConnectProvidersResponseOutputTypeDef:
         """
         Lists information about the IAM OpenID Connect (OIDC) provider resource objects
         defined in the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_open_id_connect_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_open_id_connect_providers)
         """
@@ -1201,196 +1209,196 @@
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListPoliciesResponseTypeDef:
+    ) -> ListPoliciesResponseOutputTypeDef:
         """
         Lists all the managed policies that are available in your Amazon Web Services
         account, including your own customer-defined managed policies and all Amazon Web
         Services managed policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policies)
         """
 
     def list_policies_granting_service_access(
         self, *, Arn: str, ServiceNamespaces: Sequence[str], Marker: str = ...
-    ) -> ListPoliciesGrantingServiceAccessResponseTypeDef:
+    ) -> ListPoliciesGrantingServiceAccessResponseOutputTypeDef:
         """
         Retrieves a list of policies that the IAM identity (user, group, or role) can
         use to access each specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policies_granting_service_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policies_granting_service_access)
         """
 
     def list_policy_tags(
         self, *, PolicyArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListPolicyTagsResponseTypeDef:
+    ) -> ListPolicyTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified IAM customer managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policy_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policy_tags)
         """
 
     def list_policy_versions(
         self, *, PolicyArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListPolicyVersionsResponseTypeDef:
+    ) -> ListPolicyVersionsResponseOutputTypeDef:
         """
         Lists information about the versions of the specified managed policy, including
         the version that is currently set as the policy's default version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policy_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policy_versions)
         """
 
     def list_role_policies(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListRolePoliciesResponseTypeDef:
+    ) -> ListRolePoliciesResponseOutputTypeDef:
         """
         Lists the names of the inline policies that are embedded in the specified IAM
         role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_role_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_role_policies)
         """
 
     def list_role_tags(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListRoleTagsResponseTypeDef:
+    ) -> ListRoleTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_role_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_role_tags)
         """
 
     def list_roles(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListRolesResponseTypeDef:
+    ) -> ListRolesResponseOutputTypeDef:
         """
         Lists the IAM roles that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_roles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_roles)
         """
 
     def list_saml_provider_tags(
         self, *, SAMLProviderArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListSAMLProviderTagsResponseTypeDef:
+    ) -> ListSAMLProviderTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified Security Assertion Markup
         Language (SAML) identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_saml_provider_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_saml_provider_tags)
         """
 
-    def list_saml_providers(self) -> ListSAMLProvidersResponseTypeDef:
+    def list_saml_providers(self) -> ListSAMLProvidersResponseOutputTypeDef:
         """
         Lists the SAML provider resource objects defined in IAM in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_saml_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_saml_providers)
         """
 
     def list_server_certificate_tags(
         self, *, ServerCertificateName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListServerCertificateTagsResponseTypeDef:
+    ) -> ListServerCertificateTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified IAM server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_server_certificate_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_server_certificate_tags)
         """
 
     def list_server_certificates(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListServerCertificatesResponseTypeDef:
+    ) -> ListServerCertificatesResponseOutputTypeDef:
         """
         Lists the server certificates stored in IAM that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_server_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_server_certificates)
         """
 
     def list_service_specific_credentials(
         self, *, UserName: str = ..., ServiceName: str = ...
-    ) -> ListServiceSpecificCredentialsResponseTypeDef:
+    ) -> ListServiceSpecificCredentialsResponseOutputTypeDef:
         """
         Returns information about the service-specific credentials associated with the
         specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_service_specific_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_service_specific_credentials)
         """
 
     def list_signing_certificates(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListSigningCertificatesResponseTypeDef:
+    ) -> ListSigningCertificatesResponseOutputTypeDef:
         """
         Returns information about the signing certificates associated with the specified
         IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_signing_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_signing_certificates)
         """
 
     def list_ssh_public_keys(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListSSHPublicKeysResponseTypeDef:
+    ) -> ListSSHPublicKeysResponseOutputTypeDef:
         """
         Returns information about the SSH public keys associated with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_ssh_public_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_ssh_public_keys)
         """
 
     def list_user_policies(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListUserPoliciesResponseTypeDef:
+    ) -> ListUserPoliciesResponseOutputTypeDef:
         """
         Lists the names of the inline policies embedded in the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_user_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_user_policies)
         """
 
     def list_user_tags(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListUserTagsResponseTypeDef:
+    ) -> ListUserTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_user_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_user_tags)
         """
 
     def list_users(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListUsersResponseTypeDef:
+    ) -> ListUsersResponseOutputTypeDef:
         """
         Lists the IAM users that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_users)
         """
 
     def list_virtual_mfa_devices(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListVirtualMFADevicesResponseTypeDef:
+    ) -> ListVirtualMFADevicesResponseOutputTypeDef:
         """
         Lists the virtual MFA devices defined in the Amazon Web Services account by
         assignment status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_virtual_mfa_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_virtual_mfa_devices)
         """
@@ -1480,15 +1488,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.remove_user_from_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#remove_user_from_group)
         """
 
     def reset_service_specific_credential(
         self, *, ServiceSpecificCredentialId: str, UserName: str = ...
-    ) -> ResetServiceSpecificCredentialResponseTypeDef:
+    ) -> ResetServiceSpecificCredentialResponseOutputTypeDef:
         """
         Resets the password for a service-specific credential.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.reset_service_specific_credential)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#reset_service_specific_credential)
         """
 
@@ -1540,15 +1548,15 @@
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
         Marker: str = ...
-    ) -> SimulatePolicyResponseTypeDef:
+    ) -> SimulatePolicyResponseOutputTypeDef:
         """
         Simulate how a set of IAM policies and optionally a resource-based policy works
         with a list of API operations and Amazon Web Services resources to determine the
         policies' effective permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.simulate_custom_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#simulate_custom_policy)
@@ -1565,15 +1573,15 @@
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
         Marker: str = ...
-    ) -> SimulatePolicyResponseTypeDef:
+    ) -> SimulatePolicyResponseOutputTypeDef:
         """
         Simulate how a set of IAM policies attached to an IAM entity works with a list
         of API operations and Amazon Web Services resources to determine the policies'
         effective permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.simulate_principal_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#simulate_principal_policy)
@@ -1820,25 +1828,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_role)
         """
 
     def update_role_description(
         self, *, RoleName: str, Description: str
-    ) -> UpdateRoleDescriptionResponseTypeDef:
+    ) -> UpdateRoleDescriptionResponseOutputTypeDef:
         """
         Use  UpdateRole instead.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_role_description)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_role_description)
         """
 
     def update_saml_provider(
         self, *, SAMLMetadataDocument: str, SAMLProviderArn: str
-    ) -> UpdateSAMLProviderResponseTypeDef:
+    ) -> UpdateSAMLProviderResponseOutputTypeDef:
         """
         Updates the metadata document for an existing SAML provider resource object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_saml_provider)
         """
 
@@ -1899,36 +1907,36 @@
         *,
         ServerCertificateName: str,
         CertificateBody: str,
         PrivateKey: str,
         Path: str = ...,
         CertificateChain: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UploadServerCertificateResponseTypeDef:
+    ) -> UploadServerCertificateResponseOutputTypeDef:
         """
         Uploads a server certificate entity for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_server_certificate)
         """
 
     def upload_signing_certificate(
         self, *, CertificateBody: str, UserName: str = ...
-    ) -> UploadSigningCertificateResponseTypeDef:
+    ) -> UploadSigningCertificateResponseOutputTypeDef:
         """
         Uploads an X.509 signing certificate and associates it with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_signing_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_signing_certificate)
         """
 
     def upload_ssh_public_key(
         self, *, UserName: str, SSHPublicKeyBody: str
-    ) -> UploadSSHPublicKeyResponseTypeDef:
+    ) -> UploadSSHPublicKeyResponseOutputTypeDef:
         """
         Uploads an SSH public key and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_ssh_public_key)
         """
```

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/client.pyi` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -63,99 +63,99 @@
     ListUserTagsPaginator,
     ListVirtualMFADevicesPaginator,
     SimulateCustomPolicyPaginator,
     SimulatePrincipalPolicyPaginator,
 )
 from .type_defs import (
     ContextEntryTypeDef,
-    CreateAccessKeyResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    CreateInstanceProfileResponseTypeDef,
-    CreateLoginProfileResponseTypeDef,
-    CreateOpenIDConnectProviderResponseTypeDef,
-    CreatePolicyResponseTypeDef,
-    CreatePolicyVersionResponseTypeDef,
-    CreateRoleResponseTypeDef,
-    CreateSAMLProviderResponseTypeDef,
-    CreateServiceLinkedRoleResponseTypeDef,
-    CreateServiceSpecificCredentialResponseTypeDef,
-    CreateUserResponseTypeDef,
-    CreateVirtualMFADeviceResponseTypeDef,
-    DeleteServiceLinkedRoleResponseTypeDef,
+    CreateAccessKeyResponseOutputTypeDef,
+    CreateGroupResponseOutputTypeDef,
+    CreateInstanceProfileResponseOutputTypeDef,
+    CreateLoginProfileResponseOutputTypeDef,
+    CreateOpenIDConnectProviderResponseOutputTypeDef,
+    CreatePolicyResponseOutputTypeDef,
+    CreatePolicyVersionResponseOutputTypeDef,
+    CreateRoleResponseOutputTypeDef,
+    CreateSAMLProviderResponseOutputTypeDef,
+    CreateServiceLinkedRoleResponseOutputTypeDef,
+    CreateServiceSpecificCredentialResponseOutputTypeDef,
+    CreateUserResponseOutputTypeDef,
+    CreateVirtualMFADeviceResponseOutputTypeDef,
+    DeleteServiceLinkedRoleResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
-    GenerateCredentialReportResponseTypeDef,
-    GenerateOrganizationsAccessReportResponseTypeDef,
-    GenerateServiceLastAccessedDetailsResponseTypeDef,
-    GetAccessKeyLastUsedResponseTypeDef,
-    GetAccountAuthorizationDetailsResponseTypeDef,
-    GetAccountPasswordPolicyResponseTypeDef,
-    GetAccountSummaryResponseTypeDef,
-    GetContextKeysForPolicyResponseTypeDef,
-    GetCredentialReportResponseTypeDef,
-    GetGroupPolicyResponseTypeDef,
-    GetGroupResponseTypeDef,
-    GetInstanceProfileResponseTypeDef,
-    GetLoginProfileResponseTypeDef,
-    GetMFADeviceResponseTypeDef,
-    GetOpenIDConnectProviderResponseTypeDef,
-    GetOrganizationsAccessReportResponseTypeDef,
-    GetPolicyResponseTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    GetRolePolicyResponseTypeDef,
-    GetRoleResponseTypeDef,
-    GetSAMLProviderResponseTypeDef,
-    GetServerCertificateResponseTypeDef,
-    GetServiceLastAccessedDetailsResponseTypeDef,
-    GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
-    GetServiceLinkedRoleDeletionStatusResponseTypeDef,
-    GetSSHPublicKeyResponseTypeDef,
-    GetUserPolicyResponseTypeDef,
-    GetUserResponseTypeDef,
-    ListAccessKeysResponseTypeDef,
-    ListAccountAliasesResponseTypeDef,
-    ListAttachedGroupPoliciesResponseTypeDef,
-    ListAttachedRolePoliciesResponseTypeDef,
-    ListAttachedUserPoliciesResponseTypeDef,
-    ListEntitiesForPolicyResponseTypeDef,
-    ListGroupPoliciesResponseTypeDef,
-    ListGroupsForUserResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    ListInstanceProfilesForRoleResponseTypeDef,
-    ListInstanceProfilesResponseTypeDef,
-    ListInstanceProfileTagsResponseTypeDef,
-    ListMFADevicesResponseTypeDef,
-    ListMFADeviceTagsResponseTypeDef,
-    ListOpenIDConnectProvidersResponseTypeDef,
-    ListOpenIDConnectProviderTagsResponseTypeDef,
-    ListPoliciesGrantingServiceAccessResponseTypeDef,
-    ListPoliciesResponseTypeDef,
-    ListPolicyTagsResponseTypeDef,
-    ListPolicyVersionsResponseTypeDef,
-    ListRolePoliciesResponseTypeDef,
-    ListRolesResponseTypeDef,
-    ListRoleTagsResponseTypeDef,
-    ListSAMLProvidersResponseTypeDef,
-    ListSAMLProviderTagsResponseTypeDef,
-    ListServerCertificatesResponseTypeDef,
-    ListServerCertificateTagsResponseTypeDef,
-    ListServiceSpecificCredentialsResponseTypeDef,
-    ListSigningCertificatesResponseTypeDef,
-    ListSSHPublicKeysResponseTypeDef,
-    ListUserPoliciesResponseTypeDef,
-    ListUsersResponseTypeDef,
-    ListUserTagsResponseTypeDef,
-    ListVirtualMFADevicesResponseTypeDef,
-    ResetServiceSpecificCredentialResponseTypeDef,
-    SimulatePolicyResponseTypeDef,
+    GenerateCredentialReportResponseOutputTypeDef,
+    GenerateOrganizationsAccessReportResponseOutputTypeDef,
+    GenerateServiceLastAccessedDetailsResponseOutputTypeDef,
+    GetAccessKeyLastUsedResponseOutputTypeDef,
+    GetAccountAuthorizationDetailsResponseOutputTypeDef,
+    GetAccountPasswordPolicyResponseOutputTypeDef,
+    GetAccountSummaryResponseOutputTypeDef,
+    GetContextKeysForPolicyResponseOutputTypeDef,
+    GetCredentialReportResponseOutputTypeDef,
+    GetGroupPolicyResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    GetInstanceProfileResponseOutputTypeDef,
+    GetLoginProfileResponseOutputTypeDef,
+    GetMFADeviceResponseOutputTypeDef,
+    GetOpenIDConnectProviderResponseOutputTypeDef,
+    GetOrganizationsAccessReportResponseOutputTypeDef,
+    GetPolicyResponseOutputTypeDef,
+    GetPolicyVersionResponseOutputTypeDef,
+    GetRolePolicyResponseOutputTypeDef,
+    GetRoleResponseOutputTypeDef,
+    GetSAMLProviderResponseOutputTypeDef,
+    GetServerCertificateResponseOutputTypeDef,
+    GetServiceLastAccessedDetailsResponseOutputTypeDef,
+    GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef,
+    GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef,
+    GetSSHPublicKeyResponseOutputTypeDef,
+    GetUserPolicyResponseOutputTypeDef,
+    GetUserResponseOutputTypeDef,
+    ListAccessKeysResponseOutputTypeDef,
+    ListAccountAliasesResponseOutputTypeDef,
+    ListAttachedGroupPoliciesResponseOutputTypeDef,
+    ListAttachedRolePoliciesResponseOutputTypeDef,
+    ListAttachedUserPoliciesResponseOutputTypeDef,
+    ListEntitiesForPolicyResponseOutputTypeDef,
+    ListGroupPoliciesResponseOutputTypeDef,
+    ListGroupsForUserResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
+    ListInstanceProfilesForRoleResponseOutputTypeDef,
+    ListInstanceProfilesResponseOutputTypeDef,
+    ListInstanceProfileTagsResponseOutputTypeDef,
+    ListMFADevicesResponseOutputTypeDef,
+    ListMFADeviceTagsResponseOutputTypeDef,
+    ListOpenIDConnectProvidersResponseOutputTypeDef,
+    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
+    ListPoliciesGrantingServiceAccessResponseOutputTypeDef,
+    ListPoliciesResponseOutputTypeDef,
+    ListPolicyTagsResponseOutputTypeDef,
+    ListPolicyVersionsResponseOutputTypeDef,
+    ListRolePoliciesResponseOutputTypeDef,
+    ListRolesResponseOutputTypeDef,
+    ListRoleTagsResponseOutputTypeDef,
+    ListSAMLProvidersResponseOutputTypeDef,
+    ListSAMLProviderTagsResponseOutputTypeDef,
+    ListServerCertificatesResponseOutputTypeDef,
+    ListServerCertificateTagsResponseOutputTypeDef,
+    ListServiceSpecificCredentialsResponseOutputTypeDef,
+    ListSigningCertificatesResponseOutputTypeDef,
+    ListSSHPublicKeysResponseOutputTypeDef,
+    ListUserPoliciesResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
+    ListUserTagsResponseOutputTypeDef,
+    ListVirtualMFADevicesResponseOutputTypeDef,
+    ResetServiceSpecificCredentialResponseOutputTypeDef,
+    SimulatePolicyResponseOutputTypeDef,
     TagTypeDef,
-    UpdateRoleDescriptionResponseTypeDef,
-    UpdateSAMLProviderResponseTypeDef,
-    UploadServerCertificateResponseTypeDef,
-    UploadSigningCertificateResponseTypeDef,
-    UploadSSHPublicKeyResponseTypeDef,
+    UpdateRoleDescriptionResponseOutputTypeDef,
+    UpdateSAMLProviderResponseOutputTypeDef,
+    UploadServerCertificateResponseOutputTypeDef,
+    UploadSigningCertificateResponseOutputTypeDef,
+    UploadSSHPublicKeyResponseOutputTypeDef,
 )
 from .waiter import (
     InstanceProfileExistsWaiter,
     PolicyExistsWaiter,
     RoleExistsWaiter,
     UserExistsWaiter,
 )
@@ -288,62 +288,62 @@
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#close)
         """
-    def create_access_key(self, *, UserName: str = ...) -> CreateAccessKeyResponseTypeDef:
+    def create_access_key(self, *, UserName: str = ...) -> CreateAccessKeyResponseOutputTypeDef:
         """
         Creates a new Amazon Web Services secret access key and corresponding Amazon Web
         Services access key ID for the specified user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_access_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_access_key)
         """
     def create_account_alias(self, *, AccountAlias: str) -> EmptyResponseMetadataTypeDef:
         """
         Creates an alias for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_account_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_account_alias)
         """
-    def create_group(self, *, GroupName: str, Path: str = ...) -> CreateGroupResponseTypeDef:
+    def create_group(self, *, GroupName: str, Path: str = ...) -> CreateGroupResponseOutputTypeDef:
         """
         Creates a new group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_group)
         """
     def create_instance_profile(
         self, *, InstanceProfileName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateInstanceProfileResponseTypeDef:
+    ) -> CreateInstanceProfileResponseOutputTypeDef:
         """
         Creates a new instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_instance_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_instance_profile)
         """
     def create_login_profile(
         self, *, UserName: str, Password: str, PasswordResetRequired: bool = ...
-    ) -> CreateLoginProfileResponseTypeDef:
+    ) -> CreateLoginProfileResponseOutputTypeDef:
         """
         Creates a password for the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_login_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_login_profile)
         """
     def create_open_id_connect_provider(
         self,
         *,
         Url: str,
         ThumbprintList: Sequence[str],
         ClientIDList: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateOpenIDConnectProviderResponseTypeDef:
+    ) -> CreateOpenIDConnectProviderResponseOutputTypeDef:
         """
         Creates an IAM entity to describe an identity provider (IdP) that supports
         `OpenID Connect (OIDC) <http://openid.net/connect/>`__.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_open_id_connect_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_open_id_connect_provider)
         """
@@ -351,24 +351,24 @@
         self,
         *,
         PolicyName: str,
         PolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreatePolicyResponseTypeDef:
+    ) -> CreatePolicyResponseOutputTypeDef:
         """
         Creates a new managed policy for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_policy)
         """
     def create_policy_version(
         self, *, PolicyArn: str, PolicyDocument: str, SetAsDefault: bool = ...
-    ) -> CreatePolicyVersionResponseTypeDef:
+    ) -> CreatePolicyVersionResponseOutputTypeDef:
         """
         Creates a new version of the specified managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_policy_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_policy_version)
         """
     def create_role(
@@ -377,67 +377,67 @@
         RoleName: str,
         AssumeRolePolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         MaxSessionDuration: int = ...,
         PermissionsBoundary: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRoleResponseTypeDef:
+    ) -> CreateRoleResponseOutputTypeDef:
         """
         Creates a new role for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_role)
         """
     def create_saml_provider(
         self, *, SAMLMetadataDocument: str, Name: str, Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSAMLProviderResponseTypeDef:
+    ) -> CreateSAMLProviderResponseOutputTypeDef:
         """
         Creates an IAM resource that describes an identity provider (IdP) that supports
         SAML 2.0.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_saml_provider)
         """
     def create_service_linked_role(
         self, *, AWSServiceName: str, Description: str = ..., CustomSuffix: str = ...
-    ) -> CreateServiceLinkedRoleResponseTypeDef:
+    ) -> CreateServiceLinkedRoleResponseOutputTypeDef:
         """
         Creates an IAM role that is linked to a specific Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_service_linked_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_service_linked_role)
         """
     def create_service_specific_credential(
         self, *, UserName: str, ServiceName: str
-    ) -> CreateServiceSpecificCredentialResponseTypeDef:
+    ) -> CreateServiceSpecificCredentialResponseOutputTypeDef:
         """
         Generates a set of credentials consisting of a user name and password that can
         be used to access the service specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_service_specific_credential)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_service_specific_credential)
         """
     def create_user(
         self,
         *,
         UserName: str,
         Path: str = ...,
         PermissionsBoundary: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateUserResponseTypeDef:
+    ) -> CreateUserResponseOutputTypeDef:
         """
         Creates a new IAM user for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_user)
         """
     def create_virtual_mfa_device(
         self, *, VirtualMFADeviceName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateVirtualMFADeviceResponseTypeDef:
+    ) -> CreateVirtualMFADeviceResponseOutputTypeDef:
         """
         Creates a new virtual MFA device for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_virtual_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_virtual_mfa_device)
         """
     def deactivate_mfa_device(
@@ -566,15 +566,15 @@
         Deletes the specified server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.delete_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#delete_server_certificate)
         """
     def delete_service_linked_role(
         self, *, RoleName: str
-    ) -> DeleteServiceLinkedRoleResponseTypeDef:
+    ) -> DeleteServiceLinkedRoleResponseOutputTypeDef:
         """
         Submits a service-linked role deletion request and returns a `DeletionTaskId`,
         which you can use to check the status of the deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.delete_service_linked_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#delete_service_linked_role)
         """
@@ -666,24 +666,24 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables the specified MFA device and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.enable_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#enable_mfa_device)
         """
-    def generate_credential_report(self) -> GenerateCredentialReportResponseTypeDef:
+    def generate_credential_report(self) -> GenerateCredentialReportResponseOutputTypeDef:
         """
         Generates a credential report for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_credential_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_credential_report)
         """
     def generate_organizations_access_report(
         self, *, EntityPath: str, OrganizationsPolicyId: str = ...
-    ) -> GenerateOrganizationsAccessReportResponseTypeDef:
+    ) -> GenerateOrganizationsAccessReportResponseOutputTypeDef:
         """
         Generates a report for service last accessed data for Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_organizations_access_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_organizations_access_report)
         """
     def generate_presigned_url(
@@ -697,292 +697,300 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_presigned_url)
         """
     def generate_service_last_accessed_details(
         self, *, Arn: str, Granularity: AccessAdvisorUsageGranularityTypeType = ...
-    ) -> GenerateServiceLastAccessedDetailsResponseTypeDef:
+    ) -> GenerateServiceLastAccessedDetailsResponseOutputTypeDef:
         """
         Generates a report that includes details about when an IAM resource (user,
         group, role, or policy) was last used in an attempt to access Amazon Web
         Services services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_service_last_accessed_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_service_last_accessed_details)
         """
-    def get_access_key_last_used(self, *, AccessKeyId: str) -> GetAccessKeyLastUsedResponseTypeDef:
+    def get_access_key_last_used(
+        self, *, AccessKeyId: str
+    ) -> GetAccessKeyLastUsedResponseOutputTypeDef:
         """
         Retrieves information about when the specified access key was last used.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_access_key_last_used)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_access_key_last_used)
         """
     def get_account_authorization_details(
         self, *, Filter: Sequence[EntityTypeType] = ..., MaxItems: int = ..., Marker: str = ...
-    ) -> GetAccountAuthorizationDetailsResponseTypeDef:
+    ) -> GetAccountAuthorizationDetailsResponseOutputTypeDef:
         """
         Retrieves information about all IAM users, groups, roles, and policies in your
         Amazon Web Services account, including their relationships to one another.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_authorization_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_authorization_details)
         """
-    def get_account_password_policy(self) -> GetAccountPasswordPolicyResponseTypeDef:
+    def get_account_password_policy(self) -> GetAccountPasswordPolicyResponseOutputTypeDef:
         """
         Retrieves the password policy for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_password_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_password_policy)
         """
-    def get_account_summary(self) -> GetAccountSummaryResponseTypeDef:
+    def get_account_summary(self) -> GetAccountSummaryResponseOutputTypeDef:
         """
         Retrieves information about IAM entity usage and IAM quotas in the Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_summary)
         """
     def get_context_keys_for_custom_policy(
         self, *, PolicyInputList: Sequence[str]
-    ) -> GetContextKeysForPolicyResponseTypeDef:
+    ) -> GetContextKeysForPolicyResponseOutputTypeDef:
         """
         Gets a list of all of the context keys referenced in the input policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_context_keys_for_custom_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_context_keys_for_custom_policy)
         """
     def get_context_keys_for_principal_policy(
         self, *, PolicySourceArn: str, PolicyInputList: Sequence[str] = ...
-    ) -> GetContextKeysForPolicyResponseTypeDef:
+    ) -> GetContextKeysForPolicyResponseOutputTypeDef:
         """
         Gets a list of all of the context keys referenced in all the IAM policies that
         are attached to the specified IAM entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_context_keys_for_principal_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_context_keys_for_principal_policy)
         """
-    def get_credential_report(self) -> GetCredentialReportResponseTypeDef:
+    def get_credential_report(self) -> GetCredentialReportResponseOutputTypeDef:
         """
         Retrieves a credential report for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_credential_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_credential_report)
         """
     def get_group(
         self, *, GroupName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> GetGroupResponseTypeDef:
+    ) -> GetGroupResponseOutputTypeDef:
         """
         Returns a list of IAM users that are in the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_group)
         """
-    def get_group_policy(self, *, GroupName: str, PolicyName: str) -> GetGroupPolicyResponseTypeDef:
+    def get_group_policy(
+        self, *, GroupName: str, PolicyName: str
+    ) -> GetGroupPolicyResponseOutputTypeDef:
         """
         Retrieves the specified inline policy document that is embedded in the specified
         IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_group_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_group_policy)
         """
     def get_instance_profile(
         self, *, InstanceProfileName: str
-    ) -> GetInstanceProfileResponseTypeDef:
+    ) -> GetInstanceProfileResponseOutputTypeDef:
         """
         Retrieves information about the specified instance profile, including the
         instance profile's path, GUID, ARN, and role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_instance_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_instance_profile)
         """
-    def get_login_profile(self, *, UserName: str) -> GetLoginProfileResponseTypeDef:
+    def get_login_profile(self, *, UserName: str) -> GetLoginProfileResponseOutputTypeDef:
         """
         Retrieves the user name for the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_login_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_login_profile)
         """
     def get_mfa_device(
         self, *, SerialNumber: str, UserName: str = ...
-    ) -> GetMFADeviceResponseTypeDef:
+    ) -> GetMFADeviceResponseOutputTypeDef:
         """
         Retrieves information about an MFA device for a specified user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_mfa_device)
         """
     def get_open_id_connect_provider(
         self, *, OpenIDConnectProviderArn: str
-    ) -> GetOpenIDConnectProviderResponseTypeDef:
+    ) -> GetOpenIDConnectProviderResponseOutputTypeDef:
         """
         Returns information about the specified OpenID Connect (OIDC) provider resource
         object in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_open_id_connect_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_open_id_connect_provider)
         """
     def get_organizations_access_report(
         self, *, JobId: str, MaxItems: int = ..., Marker: str = ..., SortKey: sortKeyTypeType = ...
-    ) -> GetOrganizationsAccessReportResponseTypeDef:
+    ) -> GetOrganizationsAccessReportResponseOutputTypeDef:
         """
         Retrieves the service last accessed data report for Organizations that was
         previously generated using the `GenerateOrganizationsAccessReport` operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_organizations_access_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_organizations_access_report)
         """
-    def get_policy(self, *, PolicyArn: str) -> GetPolicyResponseTypeDef:
+    def get_policy(self, *, PolicyArn: str) -> GetPolicyResponseOutputTypeDef:
         """
         Retrieves information about the specified managed policy, including the policy's
         default version and the total number of IAM users, groups, and roles to which
         the policy is attached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_policy)
         """
     def get_policy_version(
         self, *, PolicyArn: str, VersionId: str
-    ) -> GetPolicyVersionResponseTypeDef:
+    ) -> GetPolicyVersionResponseOutputTypeDef:
         """
         Retrieves information about the specified version of the specified managed
         policy, including the policy document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_policy_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_policy_version)
         """
-    def get_role(self, *, RoleName: str) -> GetRoleResponseTypeDef:
+    def get_role(self, *, RoleName: str) -> GetRoleResponseOutputTypeDef:
         """
         Retrieves information about the specified role, including the role's path, GUID,
         ARN, and the role's trust policy that grants permission to assume the role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_role)
         """
-    def get_role_policy(self, *, RoleName: str, PolicyName: str) -> GetRolePolicyResponseTypeDef:
+    def get_role_policy(
+        self, *, RoleName: str, PolicyName: str
+    ) -> GetRolePolicyResponseOutputTypeDef:
         """
         Retrieves the specified inline policy document that is embedded with the
         specified IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_role_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_role_policy)
         """
-    def get_saml_provider(self, *, SAMLProviderArn: str) -> GetSAMLProviderResponseTypeDef:
+    def get_saml_provider(self, *, SAMLProviderArn: str) -> GetSAMLProviderResponseOutputTypeDef:
         """
         Returns the SAML provider metadocument that was uploaded when the IAM SAML
         provider resource object was created or updated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_saml_provider)
         """
     def get_server_certificate(
         self, *, ServerCertificateName: str
-    ) -> GetServerCertificateResponseTypeDef:
+    ) -> GetServerCertificateResponseOutputTypeDef:
         """
         Retrieves information about the specified server certificate stored in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_server_certificate)
         """
     def get_service_last_accessed_details(
         self, *, JobId: str, MaxItems: int = ..., Marker: str = ...
-    ) -> GetServiceLastAccessedDetailsResponseTypeDef:
+    ) -> GetServiceLastAccessedDetailsResponseOutputTypeDef:
         """
         Retrieves a service last accessed report that was created using the
         `GenerateServiceLastAccessedDetails` operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_last_accessed_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_last_accessed_details)
         """
     def get_service_last_accessed_details_with_entities(
         self, *, JobId: str, ServiceNamespace: str, MaxItems: int = ..., Marker: str = ...
-    ) -> GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef:
+    ) -> GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef:
         """
         After you generate a group or policy report using the
         `GenerateServiceLastAccessedDetails` operation, you can use the `JobId`
         parameter in `GetServiceLastAccessedDetailsWithEntities`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_last_accessed_details_with_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_last_accessed_details_with_entities)
         """
     def get_service_linked_role_deletion_status(
         self, *, DeletionTaskId: str
-    ) -> GetServiceLinkedRoleDeletionStatusResponseTypeDef:
+    ) -> GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef:
         """
         Retrieves the status of your service-linked role deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_linked_role_deletion_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_linked_role_deletion_status)
         """
     def get_ssh_public_key(
         self, *, UserName: str, SSHPublicKeyId: str, Encoding: encodingTypeType
-    ) -> GetSSHPublicKeyResponseTypeDef:
+    ) -> GetSSHPublicKeyResponseOutputTypeDef:
         """
         Retrieves the specified SSH public key, including metadata about the key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_ssh_public_key)
         """
-    def get_user(self, *, UserName: str = ...) -> GetUserResponseTypeDef:
+    def get_user(self, *, UserName: str = ...) -> GetUserResponseOutputTypeDef:
         """
         Retrieves information about the specified IAM user, including the user's
         creation date, path, unique ID, and ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_user)
         """
-    def get_user_policy(self, *, UserName: str, PolicyName: str) -> GetUserPolicyResponseTypeDef:
+    def get_user_policy(
+        self, *, UserName: str, PolicyName: str
+    ) -> GetUserPolicyResponseOutputTypeDef:
         """
         Retrieves the specified inline policy document that is embedded in the specified
         IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_user_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_user_policy)
         """
     def list_access_keys(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAccessKeysResponseTypeDef:
+    ) -> ListAccessKeysResponseOutputTypeDef:
         """
         Returns information about the access key IDs associated with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_access_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_access_keys)
         """
     def list_account_aliases(
         self, *, Marker: str = ..., MaxItems: int = ...
-    ) -> ListAccountAliasesResponseTypeDef:
+    ) -> ListAccountAliasesResponseOutputTypeDef:
         """
         Lists the account alias associated with the Amazon Web Services account (Note:
         you can have only one).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_account_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_account_aliases)
         """
     def list_attached_group_policies(
         self, *, GroupName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedGroupPoliciesResponseTypeDef:
+    ) -> ListAttachedGroupPoliciesResponseOutputTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_group_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_group_policies)
         """
     def list_attached_role_policies(
         self, *, RoleName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedRolePoliciesResponseTypeDef:
+    ) -> ListAttachedRolePoliciesResponseOutputTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_role_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_role_policies)
         """
     def list_attached_user_policies(
         self, *, UserName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedUserPoliciesResponseTypeDef:
+    ) -> ListAttachedUserPoliciesResponseOutputTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_user_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_user_policies)
         """
     def list_entities_for_policy(
@@ -990,107 +998,107 @@
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListEntitiesForPolicyResponseTypeDef:
+    ) -> ListEntitiesForPolicyResponseOutputTypeDef:
         """
         Lists all IAM users, groups, and roles that the specified managed policy is
         attached to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_entities_for_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_entities_for_policy)
         """
     def list_group_policies(
         self, *, GroupName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupPoliciesResponseTypeDef:
+    ) -> ListGroupPoliciesResponseOutputTypeDef:
         """
         Lists the names of the inline policies that are embedded in the specified IAM
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_group_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_group_policies)
         """
     def list_groups(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupsResponseTypeDef:
+    ) -> ListGroupsResponseOutputTypeDef:
         """
         Lists the IAM groups that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_groups)
         """
     def list_groups_for_user(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupsForUserResponseTypeDef:
+    ) -> ListGroupsForUserResponseOutputTypeDef:
         """
         Lists the IAM groups that the specified IAM user belongs to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_groups_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_groups_for_user)
         """
     def list_instance_profile_tags(
         self, *, InstanceProfileName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfileTagsResponseTypeDef:
+    ) -> ListInstanceProfileTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified IAM instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profile_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profile_tags)
         """
     def list_instance_profiles(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfilesResponseTypeDef:
+    ) -> ListInstanceProfilesResponseOutputTypeDef:
         """
         Lists the instance profiles that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profiles)
         """
     def list_instance_profiles_for_role(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfilesForRoleResponseTypeDef:
+    ) -> ListInstanceProfilesForRoleResponseOutputTypeDef:
         """
         Lists the instance profiles that have the specified associated IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profiles_for_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profiles_for_role)
         """
     def list_mfa_device_tags(
         self, *, SerialNumber: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListMFADeviceTagsResponseTypeDef:
+    ) -> ListMFADeviceTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified IAM virtual multi-factor
         authentication (MFA) device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_mfa_device_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_mfa_device_tags)
         """
     def list_mfa_devices(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListMFADevicesResponseTypeDef:
+    ) -> ListMFADevicesResponseOutputTypeDef:
         """
         Lists the MFA devices for an IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_mfa_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_mfa_devices)
         """
     def list_open_id_connect_provider_tags(
         self, *, OpenIDConnectProviderArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListOpenIDConnectProviderTagsResponseTypeDef:
+    ) -> ListOpenIDConnectProviderTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified OpenID Connect
         (OIDC)-compatible identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_open_id_connect_provider_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_open_id_connect_provider_tags)
         """
-    def list_open_id_connect_providers(self) -> ListOpenIDConnectProvidersResponseTypeDef:
+    def list_open_id_connect_providers(self) -> ListOpenIDConnectProvidersResponseOutputTypeDef:
         """
         Lists information about the IAM OpenID Connect (OIDC) provider resource objects
         defined in the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_open_id_connect_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_open_id_connect_providers)
         """
@@ -1099,179 +1107,179 @@
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListPoliciesResponseTypeDef:
+    ) -> ListPoliciesResponseOutputTypeDef:
         """
         Lists all the managed policies that are available in your Amazon Web Services
         account, including your own customer-defined managed policies and all Amazon Web
         Services managed policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policies)
         """
     def list_policies_granting_service_access(
         self, *, Arn: str, ServiceNamespaces: Sequence[str], Marker: str = ...
-    ) -> ListPoliciesGrantingServiceAccessResponseTypeDef:
+    ) -> ListPoliciesGrantingServiceAccessResponseOutputTypeDef:
         """
         Retrieves a list of policies that the IAM identity (user, group, or role) can
         use to access each specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policies_granting_service_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policies_granting_service_access)
         """
     def list_policy_tags(
         self, *, PolicyArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListPolicyTagsResponseTypeDef:
+    ) -> ListPolicyTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified IAM customer managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policy_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policy_tags)
         """
     def list_policy_versions(
         self, *, PolicyArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListPolicyVersionsResponseTypeDef:
+    ) -> ListPolicyVersionsResponseOutputTypeDef:
         """
         Lists information about the versions of the specified managed policy, including
         the version that is currently set as the policy's default version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policy_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policy_versions)
         """
     def list_role_policies(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListRolePoliciesResponseTypeDef:
+    ) -> ListRolePoliciesResponseOutputTypeDef:
         """
         Lists the names of the inline policies that are embedded in the specified IAM
         role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_role_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_role_policies)
         """
     def list_role_tags(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListRoleTagsResponseTypeDef:
+    ) -> ListRoleTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_role_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_role_tags)
         """
     def list_roles(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListRolesResponseTypeDef:
+    ) -> ListRolesResponseOutputTypeDef:
         """
         Lists the IAM roles that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_roles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_roles)
         """
     def list_saml_provider_tags(
         self, *, SAMLProviderArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListSAMLProviderTagsResponseTypeDef:
+    ) -> ListSAMLProviderTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified Security Assertion Markup
         Language (SAML) identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_saml_provider_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_saml_provider_tags)
         """
-    def list_saml_providers(self) -> ListSAMLProvidersResponseTypeDef:
+    def list_saml_providers(self) -> ListSAMLProvidersResponseOutputTypeDef:
         """
         Lists the SAML provider resource objects defined in IAM in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_saml_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_saml_providers)
         """
     def list_server_certificate_tags(
         self, *, ServerCertificateName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListServerCertificateTagsResponseTypeDef:
+    ) -> ListServerCertificateTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified IAM server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_server_certificate_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_server_certificate_tags)
         """
     def list_server_certificates(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListServerCertificatesResponseTypeDef:
+    ) -> ListServerCertificatesResponseOutputTypeDef:
         """
         Lists the server certificates stored in IAM that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_server_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_server_certificates)
         """
     def list_service_specific_credentials(
         self, *, UserName: str = ..., ServiceName: str = ...
-    ) -> ListServiceSpecificCredentialsResponseTypeDef:
+    ) -> ListServiceSpecificCredentialsResponseOutputTypeDef:
         """
         Returns information about the service-specific credentials associated with the
         specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_service_specific_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_service_specific_credentials)
         """
     def list_signing_certificates(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListSigningCertificatesResponseTypeDef:
+    ) -> ListSigningCertificatesResponseOutputTypeDef:
         """
         Returns information about the signing certificates associated with the specified
         IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_signing_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_signing_certificates)
         """
     def list_ssh_public_keys(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListSSHPublicKeysResponseTypeDef:
+    ) -> ListSSHPublicKeysResponseOutputTypeDef:
         """
         Returns information about the SSH public keys associated with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_ssh_public_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_ssh_public_keys)
         """
     def list_user_policies(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListUserPoliciesResponseTypeDef:
+    ) -> ListUserPoliciesResponseOutputTypeDef:
         """
         Lists the names of the inline policies embedded in the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_user_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_user_policies)
         """
     def list_user_tags(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListUserTagsResponseTypeDef:
+    ) -> ListUserTagsResponseOutputTypeDef:
         """
         Lists the tags that are attached to the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_user_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_user_tags)
         """
     def list_users(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListUsersResponseTypeDef:
+    ) -> ListUsersResponseOutputTypeDef:
         """
         Lists the IAM users that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_users)
         """
     def list_virtual_mfa_devices(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListVirtualMFADevicesResponseTypeDef:
+    ) -> ListVirtualMFADevicesResponseOutputTypeDef:
         """
         Lists the virtual MFA devices defined in the Amazon Web Services account by
         assignment status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_virtual_mfa_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_virtual_mfa_devices)
         """
@@ -1352,15 +1360,15 @@
         Removes the specified user from the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.remove_user_from_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#remove_user_from_group)
         """
     def reset_service_specific_credential(
         self, *, ServiceSpecificCredentialId: str, UserName: str = ...
-    ) -> ResetServiceSpecificCredentialResponseTypeDef:
+    ) -> ResetServiceSpecificCredentialResponseOutputTypeDef:
         """
         Resets the password for a service-specific credential.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.reset_service_specific_credential)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#reset_service_specific_credential)
         """
     def resync_mfa_device(
@@ -1408,15 +1416,15 @@
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
         Marker: str = ...
-    ) -> SimulatePolicyResponseTypeDef:
+    ) -> SimulatePolicyResponseOutputTypeDef:
         """
         Simulate how a set of IAM policies and optionally a resource-based policy works
         with a list of API operations and Amazon Web Services resources to determine the
         policies' effective permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.simulate_custom_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#simulate_custom_policy)
@@ -1432,15 +1440,15 @@
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
         Marker: str = ...
-    ) -> SimulatePolicyResponseTypeDef:
+    ) -> SimulatePolicyResponseOutputTypeDef:
         """
         Simulate how a set of IAM policies attached to an IAM entity works with a list
         of API operations and Amazon Web Services resources to determine the policies'
         effective permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.simulate_principal_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#simulate_principal_policy)
@@ -1663,24 +1671,24 @@
         Updates the description or maximum session duration setting of a role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_role)
         """
     def update_role_description(
         self, *, RoleName: str, Description: str
-    ) -> UpdateRoleDescriptionResponseTypeDef:
+    ) -> UpdateRoleDescriptionResponseOutputTypeDef:
         """
         Use  UpdateRole instead.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_role_description)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_role_description)
         """
     def update_saml_provider(
         self, *, SAMLMetadataDocument: str, SAMLProviderArn: str
-    ) -> UpdateSAMLProviderResponseTypeDef:
+    ) -> UpdateSAMLProviderResponseOutputTypeDef:
         """
         Updates the metadata document for an existing SAML provider resource object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_saml_provider)
         """
     def update_server_certificate(
@@ -1735,34 +1743,34 @@
         *,
         ServerCertificateName: str,
         CertificateBody: str,
         PrivateKey: str,
         Path: str = ...,
         CertificateChain: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UploadServerCertificateResponseTypeDef:
+    ) -> UploadServerCertificateResponseOutputTypeDef:
         """
         Uploads a server certificate entity for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_server_certificate)
         """
     def upload_signing_certificate(
         self, *, CertificateBody: str, UserName: str = ...
-    ) -> UploadSigningCertificateResponseTypeDef:
+    ) -> UploadSigningCertificateResponseOutputTypeDef:
         """
         Uploads an X.509 signing certificate and associates it with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_signing_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_signing_certificate)
         """
     def upload_ssh_public_key(
         self, *, UserName: str, SSHPublicKeyBody: str
-    ) -> UploadSSHPublicKeyResponseTypeDef:
+    ) -> UploadSSHPublicKeyResponseOutputTypeDef:
         """
         Uploads an SSH public key and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_ssh_public_key)
         """
     @overload
```

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/literals.py` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/literals.pyi` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/paginator.py` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,48 +93,48 @@
     EntityTypeType,
     PolicyUsageTypeType,
     assignmentStatusTypeType,
     policyScopeTypeType,
 )
 from .type_defs import (
     ContextEntryTypeDef,
-    GetAccountAuthorizationDetailsResponseTypeDef,
-    GetGroupResponseTypeDef,
-    ListAccessKeysResponseTypeDef,
-    ListAccountAliasesResponseTypeDef,
-    ListAttachedGroupPoliciesResponseTypeDef,
-    ListAttachedRolePoliciesResponseTypeDef,
-    ListAttachedUserPoliciesResponseTypeDef,
-    ListEntitiesForPolicyResponseTypeDef,
-    ListGroupPoliciesResponseTypeDef,
-    ListGroupsForUserResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    ListInstanceProfilesForRoleResponseTypeDef,
-    ListInstanceProfilesResponseTypeDef,
-    ListInstanceProfileTagsResponseTypeDef,
-    ListMFADevicesResponseTypeDef,
-    ListMFADeviceTagsResponseTypeDef,
-    ListOpenIDConnectProviderTagsResponseTypeDef,
-    ListPoliciesResponseTypeDef,
-    ListPolicyTagsResponseTypeDef,
-    ListPolicyVersionsResponseTypeDef,
-    ListRolePoliciesResponseTypeDef,
-    ListRolesResponseTypeDef,
-    ListRoleTagsResponseTypeDef,
-    ListSAMLProviderTagsResponseTypeDef,
-    ListServerCertificatesResponseTypeDef,
-    ListServerCertificateTagsResponseTypeDef,
-    ListSigningCertificatesResponseTypeDef,
-    ListSSHPublicKeysResponseTypeDef,
-    ListUserPoliciesResponseTypeDef,
-    ListUsersResponseTypeDef,
-    ListUserTagsResponseTypeDef,
-    ListVirtualMFADevicesResponseTypeDef,
+    GetAccountAuthorizationDetailsResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    ListAccessKeysResponseOutputTypeDef,
+    ListAccountAliasesResponseOutputTypeDef,
+    ListAttachedGroupPoliciesResponseOutputTypeDef,
+    ListAttachedRolePoliciesResponseOutputTypeDef,
+    ListAttachedUserPoliciesResponseOutputTypeDef,
+    ListEntitiesForPolicyResponseOutputTypeDef,
+    ListGroupPoliciesResponseOutputTypeDef,
+    ListGroupsForUserResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
+    ListInstanceProfilesForRoleResponseOutputTypeDef,
+    ListInstanceProfilesResponseOutputTypeDef,
+    ListInstanceProfileTagsResponseOutputTypeDef,
+    ListMFADevicesResponseOutputTypeDef,
+    ListMFADeviceTagsResponseOutputTypeDef,
+    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
+    ListPoliciesResponseOutputTypeDef,
+    ListPolicyTagsResponseOutputTypeDef,
+    ListPolicyVersionsResponseOutputTypeDef,
+    ListRolePoliciesResponseOutputTypeDef,
+    ListRolesResponseOutputTypeDef,
+    ListRoleTagsResponseOutputTypeDef,
+    ListSAMLProviderTagsResponseOutputTypeDef,
+    ListServerCertificatesResponseOutputTypeDef,
+    ListServerCertificateTagsResponseOutputTypeDef,
+    ListSigningCertificatesResponseOutputTypeDef,
+    ListSSHPublicKeysResponseOutputTypeDef,
+    ListUserPoliciesResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
+    ListUserTagsResponseOutputTypeDef,
+    ListVirtualMFADevicesResponseOutputTypeDef,
     PaginatorConfigTypeDef,
-    SimulatePolicyResponseTypeDef,
+    SimulatePolicyResponseOutputTypeDef,
 )
 
 __all__ = (
     "GetAccountAuthorizationDetailsPaginator",
     "GetGroupPaginator",
     "ListAccessKeysPaginator",
     "ListAccountAliasesPaginator",
@@ -188,60 +188,60 @@
     """
 
     def paginate(
         self,
         *,
         Filter: Sequence[EntityTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetAccountAuthorizationDetailsResponseTypeDef]:
+    ) -> _PageIterator[GetAccountAuthorizationDetailsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetAccountAuthorizationDetails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getaccountauthorizationdetailspaginator)
         """
 
 
 class GetGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getgrouppaginator)
     """
 
     def paginate(
         self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetGroupResponseTypeDef]:
+    ) -> _PageIterator[GetGroupResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getgrouppaginator)
         """
 
 
 class ListAccessKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccesskeyspaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAccessKeysResponseTypeDef]:
+    ) -> _PageIterator[ListAccessKeysResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccesskeyspaginator)
         """
 
 
 class ListAccountAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccountaliasespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAccountAliasesResponseTypeDef]:
+    ) -> _PageIterator[ListAccountAliasesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccountaliasespaginator)
         """
 
 
 class ListAttachedGroupPoliciesPaginator(Paginator):
@@ -252,15 +252,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedGroupPoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListAttachedGroupPoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedGroupPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattachedgrouppoliciespaginator)
         """
 
 
 class ListAttachedRolePoliciesPaginator(Paginator):
@@ -271,15 +271,15 @@
 
     def paginate(
         self,
         *,
         RoleName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedRolePoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListAttachedRolePoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedRolePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattachedrolepoliciespaginator)
         """
 
 
 class ListAttachedUserPoliciesPaginator(Paginator):
@@ -290,15 +290,15 @@
 
     def paginate(
         self,
         *,
         UserName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedUserPoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListAttachedUserPoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedUserPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattacheduserpoliciespaginator)
         """
 
 
 class ListEntitiesForPolicyPaginator(Paginator):
@@ -311,150 +311,150 @@
         self,
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEntitiesForPolicyResponseTypeDef]:
+    ) -> _PageIterator[ListEntitiesForPolicyResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListEntitiesForPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listentitiesforpolicypaginator)
         """
 
 
 class ListGroupPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgrouppoliciespaginator)
     """
 
     def paginate(
         self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupPoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListGroupPoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgrouppoliciespaginator)
         """
 
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupsResponseTypeDef]:
+    ) -> _PageIterator[ListGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupspaginator)
         """
 
 
 class ListGroupsForUserPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupsforuserpaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupsForUserResponseTypeDef]:
+    ) -> _PageIterator[ListGroupsForUserResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupsforuserpaginator)
         """
 
 
 class ListInstanceProfileTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofiletagspaginator)
     """
 
     def paginate(
         self, *, InstanceProfileName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfileTagsResponseTypeDef]:
+    ) -> _PageIterator[ListInstanceProfileTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofiletagspaginator)
         """
 
 
 class ListInstanceProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfilesResponseTypeDef]:
+    ) -> _PageIterator[ListInstanceProfilesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilespaginator)
         """
 
 
 class ListInstanceProfilesForRolePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilesforrolepaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfilesForRoleResponseTypeDef]:
+    ) -> _PageIterator[ListInstanceProfilesForRoleResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilesforrolepaginator)
         """
 
 
 class ListMFADeviceTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicetagspaginator)
     """
 
     def paginate(
         self, *, SerialNumber: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMFADeviceTagsResponseTypeDef]:
+    ) -> _PageIterator[ListMFADeviceTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicetagspaginator)
         """
 
 
 class ListMFADevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicespaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMFADevicesResponseTypeDef]:
+    ) -> _PageIterator[ListMFADevicesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicespaginator)
         """
 
 
 class ListOpenIDConnectProviderTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listopenidconnectprovidertagspaginator)
     """
 
     def paginate(
         self, *, OpenIDConnectProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListOpenIDConnectProviderTagsResponseTypeDef]:
+    ) -> _PageIterator[ListOpenIDConnectProviderTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listopenidconnectprovidertagspaginator)
         """
 
 
 class ListPoliciesPaginator(Paginator):
@@ -467,210 +467,210 @@
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListPoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpoliciespaginator)
         """
 
 
 class ListPolicyTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicytagspaginator)
     """
 
     def paginate(
         self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPolicyTagsResponseTypeDef]:
+    ) -> _PageIterator[ListPolicyTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicytagspaginator)
         """
 
 
 class ListPolicyVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicyversionspaginator)
     """
 
     def paginate(
         self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPolicyVersionsResponseTypeDef]:
+    ) -> _PageIterator[ListPolicyVersionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicyversionspaginator)
         """
 
 
 class ListRolePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolepoliciespaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRolePoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListRolePoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolepoliciespaginator)
         """
 
 
 class ListRoleTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listroletagspaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoleTagsResponseTypeDef]:
+    ) -> _PageIterator[ListRoleTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listroletagspaginator)
         """
 
 
 class ListRolesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRolesResponseTypeDef]:
+    ) -> _PageIterator[ListRolesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolespaginator)
         """
 
 
 class ListSAMLProviderTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsamlprovidertagspaginator)
     """
 
     def paginate(
         self, *, SAMLProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSAMLProviderTagsResponseTypeDef]:
+    ) -> _PageIterator[ListSAMLProviderTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsamlprovidertagspaginator)
         """
 
 
 class ListSSHPublicKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsshpublickeyspaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSSHPublicKeysResponseTypeDef]:
+    ) -> _PageIterator[ListSSHPublicKeysResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsshpublickeyspaginator)
         """
 
 
 class ListServerCertificateTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatetagspaginator)
     """
 
     def paginate(
         self, *, ServerCertificateName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServerCertificateTagsResponseTypeDef]:
+    ) -> _PageIterator[ListServerCertificateTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatetagspaginator)
         """
 
 
 class ListServerCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServerCertificatesResponseTypeDef]:
+    ) -> _PageIterator[ListServerCertificatesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatespaginator)
         """
 
 
 class ListSigningCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsigningcertificatespaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSigningCertificatesResponseTypeDef]:
+    ) -> _PageIterator[ListSigningCertificatesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsigningcertificatespaginator)
         """
 
 
 class ListUserPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserpoliciespaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserPoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListUserPoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserpoliciespaginator)
         """
 
 
 class ListUserTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listusertagspaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserTagsResponseTypeDef]:
+    ) -> _PageIterator[ListUserTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listusertagspaginator)
         """
 
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserspaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUsersResponseTypeDef]:
+    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserspaginator)
         """
 
 
 class ListVirtualMFADevicesPaginator(Paginator):
@@ -680,15 +680,15 @@
     """
 
     def paginate(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListVirtualMFADevicesResponseTypeDef]:
+    ) -> _PageIterator[ListVirtualMFADevicesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListVirtualMFADevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listvirtualmfadevicespaginator)
         """
 
 
 class SimulateCustomPolicyPaginator(Paginator):
@@ -706,15 +706,15 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SimulatePolicyResponseTypeDef]:
+    ) -> _PageIterator[SimulatePolicyResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulateCustomPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#simulatecustompolicypaginator)
         """
 
 
 class SimulatePrincipalPolicyPaginator(Paginator):
@@ -733,12 +733,12 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SimulatePolicyResponseTypeDef]:
+    ) -> _PageIterator[SimulatePolicyResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulatePrincipalPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#simulateprincipalpolicypaginator)
         """
```

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/paginator.pyi` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -93,48 +93,48 @@
     EntityTypeType,
     PolicyUsageTypeType,
     assignmentStatusTypeType,
     policyScopeTypeType,
 )
 from .type_defs import (
     ContextEntryTypeDef,
-    GetAccountAuthorizationDetailsResponseTypeDef,
-    GetGroupResponseTypeDef,
-    ListAccessKeysResponseTypeDef,
-    ListAccountAliasesResponseTypeDef,
-    ListAttachedGroupPoliciesResponseTypeDef,
-    ListAttachedRolePoliciesResponseTypeDef,
-    ListAttachedUserPoliciesResponseTypeDef,
-    ListEntitiesForPolicyResponseTypeDef,
-    ListGroupPoliciesResponseTypeDef,
-    ListGroupsForUserResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    ListInstanceProfilesForRoleResponseTypeDef,
-    ListInstanceProfilesResponseTypeDef,
-    ListInstanceProfileTagsResponseTypeDef,
-    ListMFADevicesResponseTypeDef,
-    ListMFADeviceTagsResponseTypeDef,
-    ListOpenIDConnectProviderTagsResponseTypeDef,
-    ListPoliciesResponseTypeDef,
-    ListPolicyTagsResponseTypeDef,
-    ListPolicyVersionsResponseTypeDef,
-    ListRolePoliciesResponseTypeDef,
-    ListRolesResponseTypeDef,
-    ListRoleTagsResponseTypeDef,
-    ListSAMLProviderTagsResponseTypeDef,
-    ListServerCertificatesResponseTypeDef,
-    ListServerCertificateTagsResponseTypeDef,
-    ListSigningCertificatesResponseTypeDef,
-    ListSSHPublicKeysResponseTypeDef,
-    ListUserPoliciesResponseTypeDef,
-    ListUsersResponseTypeDef,
-    ListUserTagsResponseTypeDef,
-    ListVirtualMFADevicesResponseTypeDef,
+    GetAccountAuthorizationDetailsResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    ListAccessKeysResponseOutputTypeDef,
+    ListAccountAliasesResponseOutputTypeDef,
+    ListAttachedGroupPoliciesResponseOutputTypeDef,
+    ListAttachedRolePoliciesResponseOutputTypeDef,
+    ListAttachedUserPoliciesResponseOutputTypeDef,
+    ListEntitiesForPolicyResponseOutputTypeDef,
+    ListGroupPoliciesResponseOutputTypeDef,
+    ListGroupsForUserResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
+    ListInstanceProfilesForRoleResponseOutputTypeDef,
+    ListInstanceProfilesResponseOutputTypeDef,
+    ListInstanceProfileTagsResponseOutputTypeDef,
+    ListMFADevicesResponseOutputTypeDef,
+    ListMFADeviceTagsResponseOutputTypeDef,
+    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
+    ListPoliciesResponseOutputTypeDef,
+    ListPolicyTagsResponseOutputTypeDef,
+    ListPolicyVersionsResponseOutputTypeDef,
+    ListRolePoliciesResponseOutputTypeDef,
+    ListRolesResponseOutputTypeDef,
+    ListRoleTagsResponseOutputTypeDef,
+    ListSAMLProviderTagsResponseOutputTypeDef,
+    ListServerCertificatesResponseOutputTypeDef,
+    ListServerCertificateTagsResponseOutputTypeDef,
+    ListSigningCertificatesResponseOutputTypeDef,
+    ListSSHPublicKeysResponseOutputTypeDef,
+    ListUserPoliciesResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
+    ListUserTagsResponseOutputTypeDef,
+    ListVirtualMFADevicesResponseOutputTypeDef,
     PaginatorConfigTypeDef,
-    SimulatePolicyResponseTypeDef,
+    SimulatePolicyResponseOutputTypeDef,
 )
 
 __all__ = (
     "GetAccountAuthorizationDetailsPaginator",
     "GetGroupPaginator",
     "ListAccessKeysPaginator",
     "ListAccountAliasesPaginator",
@@ -185,57 +185,57 @@
     """
 
     def paginate(
         self,
         *,
         Filter: Sequence[EntityTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetAccountAuthorizationDetailsResponseTypeDef]:
+    ) -> _PageIterator[GetAccountAuthorizationDetailsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetAccountAuthorizationDetails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getaccountauthorizationdetailspaginator)
         """
 
 class GetGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getgrouppaginator)
     """
 
     def paginate(
         self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetGroupResponseTypeDef]:
+    ) -> _PageIterator[GetGroupResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getgrouppaginator)
         """
 
 class ListAccessKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccesskeyspaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAccessKeysResponseTypeDef]:
+    ) -> _PageIterator[ListAccessKeysResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccesskeyspaginator)
         """
 
 class ListAccountAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccountaliasespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAccountAliasesResponseTypeDef]:
+    ) -> _PageIterator[ListAccountAliasesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccountaliasespaginator)
         """
 
 class ListAttachedGroupPoliciesPaginator(Paginator):
     """
@@ -245,15 +245,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedGroupPoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListAttachedGroupPoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedGroupPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattachedgrouppoliciespaginator)
         """
 
 class ListAttachedRolePoliciesPaginator(Paginator):
     """
@@ -263,15 +263,15 @@
 
     def paginate(
         self,
         *,
         RoleName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedRolePoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListAttachedRolePoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedRolePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattachedrolepoliciespaginator)
         """
 
 class ListAttachedUserPoliciesPaginator(Paginator):
     """
@@ -281,15 +281,15 @@
 
     def paginate(
         self,
         *,
         UserName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedUserPoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListAttachedUserPoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedUserPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattacheduserpoliciespaginator)
         """
 
 class ListEntitiesForPolicyPaginator(Paginator):
     """
@@ -301,141 +301,141 @@
         self,
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEntitiesForPolicyResponseTypeDef]:
+    ) -> _PageIterator[ListEntitiesForPolicyResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListEntitiesForPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listentitiesforpolicypaginator)
         """
 
 class ListGroupPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgrouppoliciespaginator)
     """
 
     def paginate(
         self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupPoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListGroupPoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgrouppoliciespaginator)
         """
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupsResponseTypeDef]:
+    ) -> _PageIterator[ListGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupspaginator)
         """
 
 class ListGroupsForUserPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupsforuserpaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupsForUserResponseTypeDef]:
+    ) -> _PageIterator[ListGroupsForUserResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupsforuserpaginator)
         """
 
 class ListInstanceProfileTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofiletagspaginator)
     """
 
     def paginate(
         self, *, InstanceProfileName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfileTagsResponseTypeDef]:
+    ) -> _PageIterator[ListInstanceProfileTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofiletagspaginator)
         """
 
 class ListInstanceProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfilesResponseTypeDef]:
+    ) -> _PageIterator[ListInstanceProfilesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilespaginator)
         """
 
 class ListInstanceProfilesForRolePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilesforrolepaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfilesForRoleResponseTypeDef]:
+    ) -> _PageIterator[ListInstanceProfilesForRoleResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilesforrolepaginator)
         """
 
 class ListMFADeviceTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicetagspaginator)
     """
 
     def paginate(
         self, *, SerialNumber: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMFADeviceTagsResponseTypeDef]:
+    ) -> _PageIterator[ListMFADeviceTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicetagspaginator)
         """
 
 class ListMFADevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicespaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMFADevicesResponseTypeDef]:
+    ) -> _PageIterator[ListMFADevicesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicespaginator)
         """
 
 class ListOpenIDConnectProviderTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listopenidconnectprovidertagspaginator)
     """
 
     def paginate(
         self, *, OpenIDConnectProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListOpenIDConnectProviderTagsResponseTypeDef]:
+    ) -> _PageIterator[ListOpenIDConnectProviderTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listopenidconnectprovidertagspaginator)
         """
 
 class ListPoliciesPaginator(Paginator):
     """
@@ -447,197 +447,197 @@
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListPoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpoliciespaginator)
         """
 
 class ListPolicyTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicytagspaginator)
     """
 
     def paginate(
         self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPolicyTagsResponseTypeDef]:
+    ) -> _PageIterator[ListPolicyTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicytagspaginator)
         """
 
 class ListPolicyVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicyversionspaginator)
     """
 
     def paginate(
         self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPolicyVersionsResponseTypeDef]:
+    ) -> _PageIterator[ListPolicyVersionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicyversionspaginator)
         """
 
 class ListRolePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolepoliciespaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRolePoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListRolePoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolepoliciespaginator)
         """
 
 class ListRoleTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listroletagspaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoleTagsResponseTypeDef]:
+    ) -> _PageIterator[ListRoleTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listroletagspaginator)
         """
 
 class ListRolesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRolesResponseTypeDef]:
+    ) -> _PageIterator[ListRolesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolespaginator)
         """
 
 class ListSAMLProviderTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsamlprovidertagspaginator)
     """
 
     def paginate(
         self, *, SAMLProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSAMLProviderTagsResponseTypeDef]:
+    ) -> _PageIterator[ListSAMLProviderTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsamlprovidertagspaginator)
         """
 
 class ListSSHPublicKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsshpublickeyspaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSSHPublicKeysResponseTypeDef]:
+    ) -> _PageIterator[ListSSHPublicKeysResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsshpublickeyspaginator)
         """
 
 class ListServerCertificateTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatetagspaginator)
     """
 
     def paginate(
         self, *, ServerCertificateName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServerCertificateTagsResponseTypeDef]:
+    ) -> _PageIterator[ListServerCertificateTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatetagspaginator)
         """
 
 class ListServerCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServerCertificatesResponseTypeDef]:
+    ) -> _PageIterator[ListServerCertificatesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatespaginator)
         """
 
 class ListSigningCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsigningcertificatespaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSigningCertificatesResponseTypeDef]:
+    ) -> _PageIterator[ListSigningCertificatesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsigningcertificatespaginator)
         """
 
 class ListUserPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserpoliciespaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserPoliciesResponseTypeDef]:
+    ) -> _PageIterator[ListUserPoliciesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserpoliciespaginator)
         """
 
 class ListUserTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listusertagspaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserTagsResponseTypeDef]:
+    ) -> _PageIterator[ListUserTagsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listusertagspaginator)
         """
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserspaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUsersResponseTypeDef]:
+    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserspaginator)
         """
 
 class ListVirtualMFADevicesPaginator(Paginator):
     """
@@ -646,15 +646,15 @@
     """
 
     def paginate(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListVirtualMFADevicesResponseTypeDef]:
+    ) -> _PageIterator[ListVirtualMFADevicesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListVirtualMFADevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listvirtualmfadevicespaginator)
         """
 
 class SimulateCustomPolicyPaginator(Paginator):
     """
@@ -671,15 +671,15 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SimulatePolicyResponseTypeDef]:
+    ) -> _PageIterator[SimulatePolicyResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulateCustomPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#simulatecustompolicypaginator)
         """
 
 class SimulatePrincipalPolicyPaginator(Paginator):
     """
@@ -697,12 +697,12 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SimulatePolicyResponseTypeDef]:
+    ) -> _PageIterator[SimulatePolicyResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulatePrincipalPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#simulateprincipalpolicypaginator)
         """
```

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/service_resource.py` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,18 +51,19 @@
     policyScopeTypeType,
     statusTypeType,
     summaryKeyTypeType,
 )
 from .type_defs import (
     AttachedPermissionsBoundaryResponseMetadataTypeDef,
     RoleLastUsedResponseMetadataTypeDef,
-    RoleTypeDef,
+    RoleOutputTypeDef,
     ServerCertificateMetadataResponseMetadataTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
-    UpdateSAMLProviderResponseTypeDef,
+    UpdateSAMLProviderResponseOutputTypeDef,
     UserResponseMetadataTypeDef,
 )
 
 __all__ = (
     "IAMServiceResource",
     "AccessKey",
     "AccessKeyPair",
@@ -1418,15 +1419,15 @@
     path: str
     user_name: str
     user_id: str
     arn: str
     create_date: datetime
     password_last_used: datetime
     permissions_boundary: AttachedPermissionsBoundaryResponseMetadataTypeDef
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     user: "User"
     access_keys: CurrentUserAccessKeysCollection
     mfa_devices: CurrentUserMfaDevicesCollection
     signing_certificates: CurrentUserSigningCertificatesCollection
 
     def get_available_subresources(self) -> Sequence[str]:
         """
@@ -1465,16 +1466,16 @@
     """
 
     path: str
     instance_profile_name: str
     instance_profile_id: str
     arn: str
     create_date: datetime
-    roles_attribute: List[RoleTypeDef]
-    tags: List[TagTypeDef]
+    roles_attribute: List[RoleOutputTypeDef]
+    tags: List[TagOutputTypeDef]
     name: str
     roles: List["Role"]
 
     def add_role(self, *, RoleName: str) -> None:
         """
         Adds the specified IAM role to the specified instance profile.
 
@@ -1592,15 +1593,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.SamlProvider)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlprovider)
     """
 
     saml_metadata_document: str
     create_date: datetime
     valid_until: datetime
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     arn: str
 
     def delete(self) -> None:
         """
         Deletes a SAML provider resource in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.delete)
@@ -1629,15 +1630,15 @@
         Calls :py:meth:`IAM.Client.get_saml_provider` to update the attributes of the
         SamlProvider resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.reload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlproviderreload-method)
         """
 
-    def update(self, *, SAMLMetadataDocument: str) -> UpdateSAMLProviderResponseTypeDef:
+    def update(self, *, SAMLMetadataDocument: str) -> UpdateSAMLProviderResponseOutputTypeDef:
         """
         Updates the metadata document for an existing SAML provider resource object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlproviderupdate-method)
         """
 
@@ -1651,15 +1652,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#virtualmfadevice)
     """
 
     base32_string_seed: bytes
     qr_code_png: bytes
     user_attribute: UserResponseMetadataTypeDef
     enable_date: datetime
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     serial_number: str
     user: "User"
 
     def delete(self) -> None:
         """
         Deletes a virtual MFA device.
 
@@ -1907,15 +1908,15 @@
     default_version_id: str
     attachment_count: int
     permissions_boundary_usage_count: int
     is_attachable: bool
     description: str
     create_date: datetime
     update_date: datetime
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     arn: str
     default_version: "PolicyVersion"
     attached_groups: PolicyAttachedGroupsCollection
     attached_roles: PolicyAttachedRolesCollection
     attached_users: PolicyAttachedUsersCollection
     versions: PolicyVersionsCollection
 
@@ -2084,15 +2085,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.ServerCertificate)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#servercertificate)
     """
 
     server_certificate_metadata: ServerCertificateMetadataResponseMetadataTypeDef
     certificate_body: str
     certificate_chain: str
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     name: str
 
     def delete(self) -> None:
         """
         Deletes the specified server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServerCertificate.delete)
@@ -2351,15 +2352,15 @@
     role_id: str
     arn: str
     create_date: datetime
     assume_role_policy_document: str
     description: str
     max_session_duration: int
     permissions_boundary: AttachedPermissionsBoundaryResponseMetadataTypeDef
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     role_last_used: RoleLastUsedResponseMetadataTypeDef
     name: str
     attached_policies: RoleAttachedPoliciesCollection
     instance_profiles: RoleInstanceProfilesCollection
     policies: RolePoliciesCollection
 
     def AssumeRolePolicy(self) -> _AssumeRolePolicy:
@@ -2560,15 +2561,15 @@
     path: str
     user_name: str
     user_id: str
     arn: str
     create_date: datetime
     password_last_used: datetime
     permissions_boundary: AttachedPermissionsBoundaryResponseMetadataTypeDef
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     name: str
     access_keys: UserAccessKeysCollection
     attached_policies: UserAttachedPoliciesCollection
     groups: UserGroupsCollection
     mfa_devices: UserMfaDevicesCollection
     policies: UserPoliciesCollection
     signing_certificates: UserSigningCertificatesCollection
```

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/service_resource.pyi` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -51,18 +51,19 @@
     policyScopeTypeType,
     statusTypeType,
     summaryKeyTypeType,
 )
 from .type_defs import (
     AttachedPermissionsBoundaryResponseMetadataTypeDef,
     RoleLastUsedResponseMetadataTypeDef,
-    RoleTypeDef,
+    RoleOutputTypeDef,
     ServerCertificateMetadataResponseMetadataTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
-    UpdateSAMLProviderResponseTypeDef,
+    UpdateSAMLProviderResponseOutputTypeDef,
     UserResponseMetadataTypeDef,
 )
 
 __all__ = (
     "IAMServiceResource",
     "AccessKey",
     "AccessKeyPair",
@@ -1240,15 +1241,15 @@
     path: str
     user_name: str
     user_id: str
     arn: str
     create_date: datetime
     password_last_used: datetime
     permissions_boundary: AttachedPermissionsBoundaryResponseMetadataTypeDef
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     user: "User"
     access_keys: CurrentUserAccessKeysCollection
     mfa_devices: CurrentUserMfaDevicesCollection
     signing_certificates: CurrentUserSigningCertificatesCollection
 
     def get_available_subresources(self) -> Sequence[str]:
         """
@@ -1283,16 +1284,16 @@
     """
 
     path: str
     instance_profile_name: str
     instance_profile_id: str
     arn: str
     create_date: datetime
-    roles_attribute: List[RoleTypeDef]
-    tags: List[TagTypeDef]
+    roles_attribute: List[RoleOutputTypeDef]
+    tags: List[TagOutputTypeDef]
     name: str
     roles: List["Role"]
 
     def add_role(self, *, RoleName: str) -> None:
         """
         Adds the specified IAM role to the specified instance profile.
 
@@ -1397,15 +1398,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.SamlProvider)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlprovider)
     """
 
     saml_metadata_document: str
     create_date: datetime
     valid_until: datetime
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     arn: str
 
     def delete(self) -> None:
         """
         Deletes a SAML provider resource in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.delete)
@@ -1430,15 +1431,15 @@
         """
         Calls :py:meth:`IAM.Client.get_saml_provider` to update the attributes of the
         SamlProvider resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.reload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlproviderreload-method)
         """
-    def update(self, *, SAMLMetadataDocument: str) -> UpdateSAMLProviderResponseTypeDef:
+    def update(self, *, SAMLMetadataDocument: str) -> UpdateSAMLProviderResponseOutputTypeDef:
         """
         Updates the metadata document for an existing SAML provider resource object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlproviderupdate-method)
         """
 
@@ -1450,15 +1451,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#virtualmfadevice)
     """
 
     base32_string_seed: bytes
     qr_code_png: bytes
     user_attribute: UserResponseMetadataTypeDef
     enable_date: datetime
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     serial_number: str
     user: "User"
 
     def delete(self) -> None:
         """
         Deletes a virtual MFA device.
 
@@ -1680,15 +1681,15 @@
     default_version_id: str
     attachment_count: int
     permissions_boundary_usage_count: int
     is_attachable: bool
     description: str
     create_date: datetime
     update_date: datetime
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     arn: str
     default_version: "PolicyVersion"
     attached_groups: PolicyAttachedGroupsCollection
     attached_roles: PolicyAttachedRolesCollection
     attached_users: PolicyAttachedUsersCollection
     versions: PolicyVersionsCollection
 
@@ -1838,15 +1839,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.ServerCertificate)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#servercertificate)
     """
 
     server_certificate_metadata: ServerCertificateMetadataResponseMetadataTypeDef
     certificate_body: str
     certificate_chain: str
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     name: str
 
     def delete(self) -> None:
         """
         Deletes the specified server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServerCertificate.delete)
@@ -2184,15 +2185,15 @@
     role_id: str
     arn: str
     create_date: datetime
     assume_role_policy_document: str
     description: str
     max_session_duration: int
     permissions_boundary: AttachedPermissionsBoundaryResponseMetadataTypeDef
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     role_last_used: RoleLastUsedResponseMetadataTypeDef
     name: str
     attached_policies: RoleAttachedPoliciesCollection
     instance_profiles: RoleInstanceProfilesCollection
     policies: RolePoliciesCollection
 
     def AssumeRolePolicy(self) -> _AssumeRolePolicy:
@@ -2265,15 +2266,15 @@
     path: str
     user_name: str
     user_id: str
     arn: str
     create_date: datetime
     password_last_used: datetime
     permissions_boundary: AttachedPermissionsBoundaryResponseMetadataTypeDef
-    tags: List[TagTypeDef]
+    tags: List[TagOutputTypeDef]
     name: str
     access_keys: UserAccessKeysCollection
     attached_policies: UserAttachedPoliciesCollection
     groups: UserGroupsCollection
     mfa_devices: UserMfaDevicesCollection
     policies: UserPoliciesCollection
     signing_certificates: UserSigningCertificatesCollection
```

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/type_defs.py` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iam service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iam.type_defs import AccessDetailTypeDef
+    from mypy_boto3_iam.type_defs import AccessDetailOutputTypeDef
 
-    data: AccessDetailTypeDef = {...}
+    data: AccessDetailOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -43,18 +43,18 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AccessDetailTypeDef",
-    "AccessKeyLastUsedTypeDef",
-    "AccessKeyMetadataTypeDef",
-    "AccessKeyTypeDef",
+    "AccessDetailOutputTypeDef",
+    "AccessKeyLastUsedOutputTypeDef",
+    "AccessKeyMetadataOutputTypeDef",
+    "AccessKeyOutputTypeDef",
     "AddClientIDToOpenIDConnectProviderRequestRequestTypeDef",
     "AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef",
     "AddRoleToInstanceProfileRequestRequestTypeDef",
     "AddUserToGroupRequestGroupAddUserTypeDef",
     "AddUserToGroupRequestRequestTypeDef",
     "AddUserToGroupRequestUserAddGroupTypeDef",
     "AttachGroupPolicyRequestGroupAttachPolicyTypeDef",
@@ -62,38 +62,39 @@
     "AttachGroupPolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestPolicyAttachRoleTypeDef",
     "AttachRolePolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestRoleAttachPolicyTypeDef",
     "AttachUserPolicyRequestPolicyAttachUserTypeDef",
     "AttachUserPolicyRequestRequestTypeDef",
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
+    "AttachedPermissionsBoundaryOutputTypeDef",
     "AttachedPermissionsBoundaryResponseMetadataTypeDef",
-    "AttachedPermissionsBoundaryTypeDef",
-    "AttachedPolicyTypeDef",
+    "AttachedPolicyOutputTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "ChangePasswordRequestServiceResourceChangePasswordTypeDef",
     "ContextEntryTypeDef",
     "CreateAccessKeyRequestRequestTypeDef",
     "CreateAccountAliasRequestRequestTypeDef",
     "CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef",
     "CreateGroupRequestGroupCreateTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateGroupRequestServiceResourceCreateGroupTypeDef",
-    "GroupTypeDef",
+    "GroupOutputTypeDef",
     "TagTypeDef",
     "CreateLoginProfileRequestLoginProfileCreateTypeDef",
     "CreateLoginProfileRequestRequestTypeDef",
     "CreateLoginProfileRequestUserCreateLoginProfileTypeDef",
-    "LoginProfileTypeDef",
+    "LoginProfileOutputTypeDef",
+    "TagOutputTypeDef",
     "CreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
-    "PolicyVersionTypeDef",
+    "PolicyVersionOutputTypeDef",
     "CreateServiceLinkedRoleRequestRequestTypeDef",
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
-    "ServiceSpecificCredentialTypeDef",
+    "ServiceSpecificCredentialOutputTypeDef",
     "DeactivateMFADeviceRequestRequestTypeDef",
     "DeleteAccessKeyRequestRequestTypeDef",
     "DeleteAccountAliasRequestRequestTypeDef",
     "DeleteGroupPolicyRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteInstanceProfileRequestRequestTypeDef",
     "DeleteLoginProfileRequestRequestTypeDef",
@@ -103,159 +104,159 @@
     "DeleteRolePermissionsBoundaryRequestRequestTypeDef",
     "DeleteRolePolicyRequestRequestTypeDef",
     "DeleteRoleRequestRequestTypeDef",
     "DeleteSAMLProviderRequestRequestTypeDef",
     "DeleteSSHPublicKeyRequestRequestTypeDef",
     "DeleteServerCertificateRequestRequestTypeDef",
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
-    "DeleteServiceLinkedRoleResponseTypeDef",
+    "DeleteServiceLinkedRoleResponseOutputTypeDef",
     "DeleteServiceSpecificCredentialRequestRequestTypeDef",
     "DeleteSigningCertificateRequestRequestTypeDef",
     "DeleteUserPermissionsBoundaryRequestRequestTypeDef",
     "DeleteUserPolicyRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteVirtualMFADeviceRequestRequestTypeDef",
-    "RoleUsageTypeTypeDef",
+    "RoleUsageTypeOutputTypeDef",
     "DetachGroupPolicyRequestGroupDetachPolicyTypeDef",
     "DetachGroupPolicyRequestPolicyDetachGroupTypeDef",
     "DetachGroupPolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestPolicyDetachRoleTypeDef",
     "DetachRolePolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestRoleDetachPolicyTypeDef",
     "DetachUserPolicyRequestPolicyDetachUserTypeDef",
     "DetachUserPolicyRequestRequestTypeDef",
     "DetachUserPolicyRequestUserDetachPolicyTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableMFADeviceRequestMfaDeviceAssociateTypeDef",
     "EnableMFADeviceRequestRequestTypeDef",
     "EnableMFADeviceRequestUserEnableMfaTypeDef",
-    "EntityInfoTypeDef",
-    "ErrorDetailsTypeDef",
-    "OrganizationsDecisionDetailTypeDef",
-    "PermissionsBoundaryDecisionDetailTypeDef",
-    "GenerateCredentialReportResponseTypeDef",
+    "EntityInfoOutputTypeDef",
+    "ErrorDetailsOutputTypeDef",
+    "OrganizationsDecisionDetailOutputTypeDef",
+    "PermissionsBoundaryDecisionDetailOutputTypeDef",
+    "GenerateCredentialReportResponseOutputTypeDef",
     "GenerateOrganizationsAccessReportRequestRequestTypeDef",
-    "GenerateOrganizationsAccessReportResponseTypeDef",
+    "GenerateOrganizationsAccessReportResponseOutputTypeDef",
     "GenerateServiceLastAccessedDetailsRequestRequestTypeDef",
-    "GenerateServiceLastAccessedDetailsResponseTypeDef",
+    "GenerateServiceLastAccessedDetailsResponseOutputTypeDef",
     "GetAccessKeyLastUsedRequestRequestTypeDef",
     "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
     "GetAccountAuthorizationDetailsRequestRequestTypeDef",
-    "PasswordPolicyTypeDef",
-    "GetAccountSummaryResponseTypeDef",
+    "PasswordPolicyOutputTypeDef",
+    "GetAccountSummaryResponseOutputTypeDef",
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
-    "GetContextKeysForPolicyResponseTypeDef",
+    "GetContextKeysForPolicyResponseOutputTypeDef",
     "GetContextKeysForPrincipalPolicyRequestRequestTypeDef",
-    "GetCredentialReportResponseTypeDef",
+    "GetCredentialReportResponseOutputTypeDef",
     "GetGroupPolicyRequestRequestTypeDef",
-    "GetGroupPolicyResponseTypeDef",
+    "GetGroupPolicyResponseOutputTypeDef",
     "GetGroupRequestGetGroupPaginateTypeDef",
     "GetGroupRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
     "GetLoginProfileRequestRequestTypeDef",
     "GetMFADeviceRequestRequestTypeDef",
-    "GetMFADeviceResponseTypeDef",
+    "GetMFADeviceResponseOutputTypeDef",
     "GetOpenIDConnectProviderRequestRequestTypeDef",
     "GetOrganizationsAccessReportRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetPolicyVersionRequestRequestTypeDef",
     "GetRolePolicyRequestRequestTypeDef",
-    "GetRolePolicyResponseTypeDef",
+    "GetRolePolicyResponseOutputTypeDef",
     "GetRoleRequestRequestTypeDef",
     "GetSAMLProviderRequestRequestTypeDef",
     "GetSSHPublicKeyRequestRequestTypeDef",
-    "SSHPublicKeyTypeDef",
+    "SSHPublicKeyOutputTypeDef",
     "GetServerCertificateRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef",
     "GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef",
     "GetUserPolicyRequestRequestTypeDef",
-    "GetUserPolicyResponseTypeDef",
+    "GetUserPolicyResponseOutputTypeDef",
     "GetUserRequestRequestTypeDef",
-    "PolicyDetailTypeDef",
+    "PolicyDetailOutputTypeDef",
     "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
     "ListAccessKeysRequestRequestTypeDef",
     "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
     "ListAccountAliasesRequestRequestTypeDef",
-    "ListAccountAliasesResponseTypeDef",
+    "ListAccountAliasesResponseOutputTypeDef",
     "ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
     "ListAttachedGroupPoliciesRequestRequestTypeDef",
     "ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
     "ListAttachedRolePoliciesRequestRequestTypeDef",
     "ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
     "ListAttachedUserPoliciesRequestRequestTypeDef",
     "ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
     "ListEntitiesForPolicyRequestRequestTypeDef",
-    "PolicyGroupTypeDef",
-    "PolicyRoleTypeDef",
-    "PolicyUserTypeDef",
+    "PolicyGroupOutputTypeDef",
+    "PolicyRoleOutputTypeDef",
+    "PolicyUserOutputTypeDef",
     "ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
     "ListGroupPoliciesRequestRequestTypeDef",
-    "ListGroupPoliciesResponseTypeDef",
+    "ListGroupPoliciesResponseOutputTypeDef",
     "ListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
     "ListGroupsForUserRequestRequestTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
     "ListInstanceProfileTagsRequestRequestTypeDef",
     "ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
     "ListInstanceProfilesForRoleRequestRequestTypeDef",
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListInstanceProfilesRequestRequestTypeDef",
     "ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
     "ListMFADeviceTagsRequestRequestTypeDef",
     "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
     "ListMFADevicesRequestRequestTypeDef",
-    "MFADeviceTypeDef",
+    "MFADeviceOutputTypeDef",
     "ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
     "ListOpenIDConnectProviderTagsRequestRequestTypeDef",
-    "OpenIDConnectProviderListEntryTypeDef",
-    "PolicyGrantingServiceAccessTypeDef",
+    "OpenIDConnectProviderListEntryOutputTypeDef",
+    "PolicyGrantingServiceAccessOutputTypeDef",
     "ListPoliciesGrantingServiceAccessRequestRequestTypeDef",
     "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "ListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
     "ListPolicyTagsRequestRequestTypeDef",
     "ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
     "ListPolicyVersionsRequestRequestTypeDef",
     "ListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
     "ListRolePoliciesRequestRequestTypeDef",
-    "ListRolePoliciesResponseTypeDef",
+    "ListRolePoliciesResponseOutputTypeDef",
     "ListRoleTagsRequestListRoleTagsPaginateTypeDef",
     "ListRoleTagsRequestRequestTypeDef",
     "ListRolesRequestListRolesPaginateTypeDef",
     "ListRolesRequestRequestTypeDef",
     "ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
     "ListSAMLProviderTagsRequestRequestTypeDef",
-    "SAMLProviderListEntryTypeDef",
+    "SAMLProviderListEntryOutputTypeDef",
     "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
     "ListSSHPublicKeysRequestRequestTypeDef",
-    "SSHPublicKeyMetadataTypeDef",
+    "SSHPublicKeyMetadataOutputTypeDef",
     "ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
     "ListServerCertificateTagsRequestRequestTypeDef",
     "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
     "ListServerCertificatesRequestRequestTypeDef",
-    "ServerCertificateMetadataTypeDef",
+    "ServerCertificateMetadataOutputTypeDef",
     "ListServiceSpecificCredentialsRequestRequestTypeDef",
-    "ServiceSpecificCredentialMetadataTypeDef",
+    "ServiceSpecificCredentialMetadataOutputTypeDef",
     "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
     "ListSigningCertificatesRequestRequestTypeDef",
-    "SigningCertificateTypeDef",
+    "SigningCertificateOutputTypeDef",
     "ListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
     "ListUserPoliciesRequestRequestTypeDef",
-    "ListUserPoliciesResponseTypeDef",
+    "ListUserPoliciesResponseOutputTypeDef",
     "ListUserTagsRequestListUserTagsPaginateTypeDef",
     "ListUserTagsRequestRequestTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
     "ListVirtualMFADevicesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "PositionTypeDef",
+    "PositionOutputTypeDef",
     "PutGroupPolicyRequestGroupCreatePolicyTypeDef",
     "PutGroupPolicyRequestGroupPolicyPutTypeDef",
     "PutGroupPolicyRequestRequestTypeDef",
     "PutRolePermissionsBoundaryRequestRequestTypeDef",
     "PutRolePolicyRequestRequestTypeDef",
     "PutRolePolicyRequestRolePolicyPutTypeDef",
     "PutUserPermissionsBoundaryRequestRequestTypeDef",
@@ -268,18 +269,18 @@
     "RemoveUserFromGroupRequestGroupRemoveUserTypeDef",
     "RemoveUserFromGroupRequestRequestTypeDef",
     "RemoveUserFromGroupRequestUserRemoveGroupTypeDef",
     "ResetServiceSpecificCredentialRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ResyncMFADeviceRequestMfaDeviceResyncTypeDef",
     "ResyncMFADeviceRequestRequestTypeDef",
-    "RoleLastUsedTypeDef",
+    "RoleLastUsedOutputTypeDef",
     "RoleLastUsedResponseMetadataTypeDef",
     "ServerCertificateMetadataResponseMetadataTypeDef",
-    "TrackedActionLastAccessedTypeDef",
+    "TrackedActionLastAccessedOutputTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetSecurityTokenServicePreferencesRequestRequestTypeDef",
     "UntagInstanceProfileRequestRequestTypeDef",
     "UntagMFADeviceRequestRequestTypeDef",
     "UntagOpenIDConnectProviderRequestRequestTypeDef",
     "UntagPolicyRequestRequestTypeDef",
     "UntagRoleRequestRequestTypeDef",
@@ -301,179 +302,179 @@
     "UpdateLoginProfileRequestLoginProfileUpdateTypeDef",
     "UpdateLoginProfileRequestRequestTypeDef",
     "UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef",
     "UpdateRoleDescriptionRequestRequestTypeDef",
     "UpdateRoleRequestRequestTypeDef",
     "UpdateSAMLProviderRequestRequestTypeDef",
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
-    "UpdateSAMLProviderResponseTypeDef",
+    "UpdateSAMLProviderResponseOutputTypeDef",
     "UpdateSSHPublicKeyRequestRequestTypeDef",
     "UpdateServerCertificateRequestRequestTypeDef",
     "UpdateServerCertificateRequestServerCertificateUpdateTypeDef",
     "UpdateServiceSpecificCredentialRequestRequestTypeDef",
     "UpdateSigningCertificateRequestRequestTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateActivateTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserRequestUserUpdateTypeDef",
     "UploadSSHPublicKeyRequestRequestTypeDef",
     "UploadSigningCertificateRequestRequestTypeDef",
     "UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
-    "GetAccessKeyLastUsedResponseTypeDef",
-    "ListAccessKeysResponseTypeDef",
-    "CreateAccessKeyResponseTypeDef",
-    "ListAttachedGroupPoliciesResponseTypeDef",
-    "ListAttachedRolePoliciesResponseTypeDef",
-    "ListAttachedUserPoliciesResponseTypeDef",
+    "GetAccessKeyLastUsedResponseOutputTypeDef",
+    "ListAccessKeysResponseOutputTypeDef",
+    "CreateAccessKeyResponseOutputTypeDef",
+    "ListAttachedGroupPoliciesResponseOutputTypeDef",
+    "ListAttachedRolePoliciesResponseOutputTypeDef",
+    "ListAttachedUserPoliciesResponseOutputTypeDef",
     "SimulateCustomPolicyRequestRequestTypeDef",
     "SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
     "SimulatePrincipalPolicyRequestRequestTypeDef",
     "SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
-    "CreateGroupResponseTypeDef",
-    "ListGroupsForUserResponseTypeDef",
-    "ListGroupsResponseTypeDef",
+    "CreateGroupResponseOutputTypeDef",
+    "ListGroupsForUserResponseOutputTypeDef",
+    "ListGroupsResponseOutputTypeDef",
     "CreateInstanceProfileRequestRequestTypeDef",
     "CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef",
     "CreateOpenIDConnectProviderRequestRequestTypeDef",
-    "CreateOpenIDConnectProviderResponseTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreatePolicyRequestServiceResourceCreatePolicyTypeDef",
     "CreateRoleRequestRequestTypeDef",
     "CreateRoleRequestServiceResourceCreateRoleTypeDef",
     "CreateSAMLProviderRequestRequestTypeDef",
     "CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef",
-    "CreateSAMLProviderResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "CreateUserRequestServiceResourceCreateUserTypeDef",
     "CreateUserRequestUserCreateTypeDef",
     "CreateVirtualMFADeviceRequestRequestTypeDef",
     "CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef",
-    "GetOpenIDConnectProviderResponseTypeDef",
-    "GetSAMLProviderResponseTypeDef",
-    "ListInstanceProfileTagsResponseTypeDef",
-    "ListMFADeviceTagsResponseTypeDef",
-    "ListOpenIDConnectProviderTagsResponseTypeDef",
-    "ListPolicyTagsResponseTypeDef",
-    "ListRoleTagsResponseTypeDef",
-    "ListSAMLProviderTagsResponseTypeDef",
-    "ListServerCertificateTagsResponseTypeDef",
-    "ListUserTagsResponseTypeDef",
-    "PolicyTypeDef",
     "TagInstanceProfileRequestRequestTypeDef",
     "TagMFADeviceRequestRequestTypeDef",
     "TagOpenIDConnectProviderRequestRequestTypeDef",
     "TagPolicyRequestRequestTypeDef",
     "TagRoleRequestRequestTypeDef",
     "TagSAMLProviderRequestRequestTypeDef",
     "TagServerCertificateRequestRequestTypeDef",
     "TagUserRequestRequestTypeDef",
     "UploadServerCertificateRequestRequestTypeDef",
     "UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
+    "CreateLoginProfileResponseOutputTypeDef",
+    "GetLoginProfileResponseOutputTypeDef",
+    "CreateOpenIDConnectProviderResponseOutputTypeDef",
+    "CreateSAMLProviderResponseOutputTypeDef",
+    "GetOpenIDConnectProviderResponseOutputTypeDef",
+    "GetSAMLProviderResponseOutputTypeDef",
+    "ListInstanceProfileTagsResponseOutputTypeDef",
+    "ListMFADeviceTagsResponseOutputTypeDef",
+    "ListOpenIDConnectProviderTagsResponseOutputTypeDef",
+    "ListPolicyTagsResponseOutputTypeDef",
+    "ListRoleTagsResponseOutputTypeDef",
+    "ListSAMLProviderTagsResponseOutputTypeDef",
+    "ListServerCertificateTagsResponseOutputTypeDef",
+    "ListUserTagsResponseOutputTypeDef",
+    "PolicyOutputTypeDef",
+    "UserOutputTypeDef",
     "UserResponseMetadataTypeDef",
-    "UserTypeDef",
-    "CreateLoginProfileResponseTypeDef",
-    "GetLoginProfileResponseTypeDef",
-    "CreatePolicyVersionResponseTypeDef",
-    "GetPolicyVersionResponseTypeDef",
-    "ListPolicyVersionsResponseTypeDef",
-    "ManagedPolicyDetailTypeDef",
-    "CreateServiceSpecificCredentialResponseTypeDef",
-    "ResetServiceSpecificCredentialResponseTypeDef",
-    "DeletionTaskFailureReasonTypeTypeDef",
-    "EntityDetailsTypeDef",
-    "GetOrganizationsAccessReportResponseTypeDef",
-    "GetAccountPasswordPolicyResponseTypeDef",
+    "CreatePolicyVersionResponseOutputTypeDef",
+    "GetPolicyVersionResponseOutputTypeDef",
+    "ListPolicyVersionsResponseOutputTypeDef",
+    "ManagedPolicyDetailOutputTypeDef",
+    "CreateServiceSpecificCredentialResponseOutputTypeDef",
+    "ResetServiceSpecificCredentialResponseOutputTypeDef",
+    "DeletionTaskFailureReasonTypeOutputTypeDef",
+    "EntityDetailsOutputTypeDef",
+    "GetOrganizationsAccessReportResponseOutputTypeDef",
+    "GetAccountPasswordPolicyResponseOutputTypeDef",
     "GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     "GetPolicyRequestPolicyExistsWaitTypeDef",
     "GetRoleRequestRoleExistsWaitTypeDef",
     "GetUserRequestUserExistsWaitTypeDef",
-    "GetSSHPublicKeyResponseTypeDef",
-    "UploadSSHPublicKeyResponseTypeDef",
-    "GroupDetailTypeDef",
-    "UserDetailTypeDef",
-    "ListEntitiesForPolicyResponseTypeDef",
-    "ListMFADevicesResponseTypeDef",
-    "ListOpenIDConnectProvidersResponseTypeDef",
-    "ListPoliciesGrantingServiceAccessEntryTypeDef",
-    "ListSAMLProvidersResponseTypeDef",
-    "ListSSHPublicKeysResponseTypeDef",
-    "ListServerCertificatesResponseTypeDef",
-    "ServerCertificateTypeDef",
-    "UploadServerCertificateResponseTypeDef",
-    "ListServiceSpecificCredentialsResponseTypeDef",
-    "ListSigningCertificatesResponseTypeDef",
-    "UploadSigningCertificateResponseTypeDef",
-    "StatementTypeDef",
-    "RoleTypeDef",
-    "ServiceLastAccessedTypeDef",
-    "CreatePolicyResponseTypeDef",
-    "GetPolicyResponseTypeDef",
-    "ListPoliciesResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "GetGroupResponseTypeDef",
-    "GetUserResponseTypeDef",
-    "ListUsersResponseTypeDef",
-    "VirtualMFADeviceTypeDef",
-    "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
-    "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
-    "ListPoliciesGrantingServiceAccessResponseTypeDef",
-    "GetServerCertificateResponseTypeDef",
-    "ResourceSpecificResultTypeDef",
-    "CreateRoleResponseTypeDef",
-    "CreateServiceLinkedRoleResponseTypeDef",
-    "GetRoleResponseTypeDef",
-    "InstanceProfileTypeDef",
-    "ListRolesResponseTypeDef",
-    "UpdateRoleDescriptionResponseTypeDef",
-    "GetServiceLastAccessedDetailsResponseTypeDef",
-    "CreateVirtualMFADeviceResponseTypeDef",
-    "ListVirtualMFADevicesResponseTypeDef",
-    "EvaluationResultTypeDef",
-    "CreateInstanceProfileResponseTypeDef",
-    "GetInstanceProfileResponseTypeDef",
-    "ListInstanceProfilesForRoleResponseTypeDef",
-    "ListInstanceProfilesResponseTypeDef",
-    "RoleDetailTypeDef",
-    "SimulatePolicyResponseTypeDef",
-    "GetAccountAuthorizationDetailsResponseTypeDef",
+    "GetSSHPublicKeyResponseOutputTypeDef",
+    "UploadSSHPublicKeyResponseOutputTypeDef",
+    "GroupDetailOutputTypeDef",
+    "UserDetailOutputTypeDef",
+    "ListEntitiesForPolicyResponseOutputTypeDef",
+    "ListMFADevicesResponseOutputTypeDef",
+    "ListOpenIDConnectProvidersResponseOutputTypeDef",
+    "ListPoliciesGrantingServiceAccessEntryOutputTypeDef",
+    "ListSAMLProvidersResponseOutputTypeDef",
+    "ListSSHPublicKeysResponseOutputTypeDef",
+    "ListServerCertificatesResponseOutputTypeDef",
+    "ServerCertificateOutputTypeDef",
+    "UploadServerCertificateResponseOutputTypeDef",
+    "ListServiceSpecificCredentialsResponseOutputTypeDef",
+    "ListSigningCertificatesResponseOutputTypeDef",
+    "UploadSigningCertificateResponseOutputTypeDef",
+    "StatementOutputTypeDef",
+    "RoleOutputTypeDef",
+    "ServiceLastAccessedOutputTypeDef",
+    "CreatePolicyResponseOutputTypeDef",
+    "GetPolicyResponseOutputTypeDef",
+    "ListPoliciesResponseOutputTypeDef",
+    "CreateUserResponseOutputTypeDef",
+    "GetGroupResponseOutputTypeDef",
+    "GetUserResponseOutputTypeDef",
+    "ListUsersResponseOutputTypeDef",
+    "VirtualMFADeviceOutputTypeDef",
+    "GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef",
+    "GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef",
+    "ListPoliciesGrantingServiceAccessResponseOutputTypeDef",
+    "GetServerCertificateResponseOutputTypeDef",
+    "ResourceSpecificResultOutputTypeDef",
+    "CreateRoleResponseOutputTypeDef",
+    "CreateServiceLinkedRoleResponseOutputTypeDef",
+    "GetRoleResponseOutputTypeDef",
+    "InstanceProfileOutputTypeDef",
+    "ListRolesResponseOutputTypeDef",
+    "UpdateRoleDescriptionResponseOutputTypeDef",
+    "GetServiceLastAccessedDetailsResponseOutputTypeDef",
+    "CreateVirtualMFADeviceResponseOutputTypeDef",
+    "ListVirtualMFADevicesResponseOutputTypeDef",
+    "EvaluationResultOutputTypeDef",
+    "CreateInstanceProfileResponseOutputTypeDef",
+    "GetInstanceProfileResponseOutputTypeDef",
+    "ListInstanceProfilesForRoleResponseOutputTypeDef",
+    "ListInstanceProfilesResponseOutputTypeDef",
+    "RoleDetailOutputTypeDef",
+    "SimulatePolicyResponseOutputTypeDef",
+    "GetAccountAuthorizationDetailsResponseOutputTypeDef",
 )
 
-AccessDetailTypeDef = TypedDict(
-    "AccessDetailTypeDef",
+AccessDetailOutputTypeDef = TypedDict(
+    "AccessDetailOutputTypeDef",
     {
         "ServiceName": str,
         "ServiceNamespace": str,
         "Region": str,
         "EntityPath": str,
         "LastAuthenticatedTime": datetime,
         "TotalAuthenticatedEntities": int,
     },
 )
 
-AccessKeyLastUsedTypeDef = TypedDict(
-    "AccessKeyLastUsedTypeDef",
+AccessKeyLastUsedOutputTypeDef = TypedDict(
+    "AccessKeyLastUsedOutputTypeDef",
     {
         "LastUsedDate": datetime,
         "ServiceName": str,
         "Region": str,
     },
 )
 
-AccessKeyMetadataTypeDef = TypedDict(
-    "AccessKeyMetadataTypeDef",
+AccessKeyMetadataOutputTypeDef = TypedDict(
+    "AccessKeyMetadataOutputTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "CreateDate": datetime,
     },
 )
 
-AccessKeyTypeDef = TypedDict(
-    "AccessKeyTypeDef",
+AccessKeyOutputTypeDef = TypedDict(
+    "AccessKeyOutputTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "SecretAccessKey": str,
         "CreateDate": datetime,
     },
@@ -586,33 +587,33 @@
 AttachUserPolicyRequestUserAttachPolicyTypeDef = TypedDict(
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
     {
         "PolicyArn": str,
     },
 )
 
-AttachedPermissionsBoundaryResponseMetadataTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
+AttachedPermissionsBoundaryOutputTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryOutputTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachedPermissionsBoundaryTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryTypeDef",
+AttachedPermissionsBoundaryResponseMetadataTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachedPolicyTypeDef = TypedDict(
-    "AttachedPolicyTypeDef",
+AttachedPolicyOutputTypeDef = TypedDict(
+    "AttachedPolicyOutputTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
@@ -710,16 +711,16 @@
 class CreateGroupRequestServiceResourceCreateGroupTypeDef(
     _RequiredCreateGroupRequestServiceResourceCreateGroupTypeDef,
     _OptionalCreateGroupRequestServiceResourceCreateGroupTypeDef,
 ):
     pass
 
 
-GroupTypeDef = TypedDict(
-    "GroupTypeDef",
+GroupOutputTypeDef = TypedDict(
+    "GroupOutputTypeDef",
     {
         "Path": str,
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
         "CreateDate": datetime,
     },
@@ -796,23 +797,31 @@
 class CreateLoginProfileRequestUserCreateLoginProfileTypeDef(
     _RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
     _OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
 ):
     pass
 
 
-LoginProfileTypeDef = TypedDict(
-    "LoginProfileTypeDef",
+LoginProfileOutputTypeDef = TypedDict(
+    "LoginProfileOutputTypeDef",
     {
         "UserName": str,
         "CreateDate": datetime,
         "PasswordResetRequired": bool,
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
 _RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     {
         "PolicyDocument": str,
     },
 )
 _OptionalCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
@@ -850,16 +859,16 @@
 class CreatePolicyVersionRequestRequestTypeDef(
     _RequiredCreatePolicyVersionRequestRequestTypeDef,
     _OptionalCreatePolicyVersionRequestRequestTypeDef,
 ):
     pass
 
 
-PolicyVersionTypeDef = TypedDict(
-    "PolicyVersionTypeDef",
+PolicyVersionOutputTypeDef = TypedDict(
+    "PolicyVersionOutputTypeDef",
     {
         "Document": str,
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": datetime,
     },
 )
@@ -891,16 +900,16 @@
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
         "ServiceName": str,
     },
 )
 
-ServiceSpecificCredentialTypeDef = TypedDict(
-    "ServiceSpecificCredentialTypeDef",
+ServiceSpecificCredentialOutputTypeDef = TypedDict(
+    "ServiceSpecificCredentialOutputTypeDef",
     {
         "CreateDate": datetime,
         "ServiceName": str,
         "ServiceUserName": str,
         "ServicePassword": str,
         "ServiceSpecificCredentialId": str,
         "UserName": str,
@@ -1042,16 +1051,16 @@
 DeleteServiceLinkedRoleRequestRequestTypeDef = TypedDict(
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 
-DeleteServiceLinkedRoleResponseTypeDef = TypedDict(
-    "DeleteServiceLinkedRoleResponseTypeDef",
+DeleteServiceLinkedRoleResponseOutputTypeDef = TypedDict(
+    "DeleteServiceLinkedRoleResponseOutputTypeDef",
     {
         "DeletionTaskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteServiceSpecificCredentialRequestRequestTypeDef = TypedDict(
@@ -1123,16 +1132,16 @@
 DeleteVirtualMFADeviceRequestRequestTypeDef = TypedDict(
     "DeleteVirtualMFADeviceRequestRequestTypeDef",
     {
         "SerialNumber": str,
     },
 )
 
-RoleUsageTypeTypeDef = TypedDict(
-    "RoleUsageTypeTypeDef",
+RoleUsageTypeOutputTypeDef = TypedDict(
+    "RoleUsageTypeOutputTypeDef",
     {
         "Region": str,
         "Resources": List[str],
     },
 )
 
 DetachGroupPolicyRequestGroupDetachPolicyTypeDef = TypedDict(
@@ -1231,49 +1240,49 @@
     {
         "SerialNumber": str,
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
 
-EntityInfoTypeDef = TypedDict(
-    "EntityInfoTypeDef",
+EntityInfoOutputTypeDef = TypedDict(
+    "EntityInfoOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": policyOwnerEntityTypeType,
         "Id": str,
         "Path": str,
     },
 )
 
-ErrorDetailsTypeDef = TypedDict(
-    "ErrorDetailsTypeDef",
+ErrorDetailsOutputTypeDef = TypedDict(
+    "ErrorDetailsOutputTypeDef",
     {
         "Message": str,
         "Code": str,
     },
 )
 
-OrganizationsDecisionDetailTypeDef = TypedDict(
-    "OrganizationsDecisionDetailTypeDef",
+OrganizationsDecisionDetailOutputTypeDef = TypedDict(
+    "OrganizationsDecisionDetailOutputTypeDef",
     {
         "AllowedByOrganizations": bool,
     },
 )
 
-PermissionsBoundaryDecisionDetailTypeDef = TypedDict(
-    "PermissionsBoundaryDecisionDetailTypeDef",
+PermissionsBoundaryDecisionDetailOutputTypeDef = TypedDict(
+    "PermissionsBoundaryDecisionDetailOutputTypeDef",
     {
         "AllowedByPermissionsBoundary": bool,
     },
 )
 
-GenerateCredentialReportResponseTypeDef = TypedDict(
-    "GenerateCredentialReportResponseTypeDef",
+GenerateCredentialReportResponseOutputTypeDef = TypedDict(
+    "GenerateCredentialReportResponseOutputTypeDef",
     {
         "State": ReportStateTypeType,
         "Description": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1295,16 +1304,16 @@
 class GenerateOrganizationsAccessReportRequestRequestTypeDef(
     _RequiredGenerateOrganizationsAccessReportRequestRequestTypeDef,
     _OptionalGenerateOrganizationsAccessReportRequestRequestTypeDef,
 ):
     pass
 
 
-GenerateOrganizationsAccessReportResponseTypeDef = TypedDict(
-    "GenerateOrganizationsAccessReportResponseTypeDef",
+GenerateOrganizationsAccessReportResponseOutputTypeDef = TypedDict(
+    "GenerateOrganizationsAccessReportResponseOutputTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef = TypedDict(
@@ -1325,16 +1334,16 @@
 class GenerateServiceLastAccessedDetailsRequestRequestTypeDef(
     _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
     _OptionalGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
 ):
     pass
 
 
-GenerateServiceLastAccessedDetailsResponseTypeDef = TypedDict(
-    "GenerateServiceLastAccessedDetailsResponseTypeDef",
+GenerateServiceLastAccessedDetailsResponseOutputTypeDef = TypedDict(
+    "GenerateServiceLastAccessedDetailsResponseOutputTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccessKeyLastUsedRequestRequestTypeDef = TypedDict(
@@ -1359,47 +1368,47 @@
         "Filter": Sequence[EntityTypeType],
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
-PasswordPolicyTypeDef = TypedDict(
-    "PasswordPolicyTypeDef",
+PasswordPolicyOutputTypeDef = TypedDict(
+    "PasswordPolicyOutputTypeDef",
     {
         "MinimumPasswordLength": int,
         "RequireSymbols": bool,
         "RequireNumbers": bool,
         "RequireUppercaseCharacters": bool,
         "RequireLowercaseCharacters": bool,
         "AllowUsersToChangePassword": bool,
         "ExpirePasswords": bool,
         "MaxPasswordAge": int,
         "PasswordReusePrevention": int,
         "HardExpiry": bool,
     },
 )
 
-GetAccountSummaryResponseTypeDef = TypedDict(
-    "GetAccountSummaryResponseTypeDef",
+GetAccountSummaryResponseOutputTypeDef = TypedDict(
+    "GetAccountSummaryResponseOutputTypeDef",
     {
         "SummaryMap": Dict[summaryKeyTypeType, int],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContextKeysForCustomPolicyRequestRequestTypeDef = TypedDict(
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
     {
         "PolicyInputList": Sequence[str],
     },
 )
 
-GetContextKeysForPolicyResponseTypeDef = TypedDict(
-    "GetContextKeysForPolicyResponseTypeDef",
+GetContextKeysForPolicyResponseOutputTypeDef = TypedDict(
+    "GetContextKeysForPolicyResponseOutputTypeDef",
     {
         "ContextKeyNames": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef = TypedDict(
@@ -1420,16 +1429,16 @@
 class GetContextKeysForPrincipalPolicyRequestRequestTypeDef(
     _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
     _OptionalGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-GetCredentialReportResponseTypeDef = TypedDict(
-    "GetCredentialReportResponseTypeDef",
+GetCredentialReportResponseOutputTypeDef = TypedDict(
+    "GetCredentialReportResponseOutputTypeDef",
     {
         "Content": bytes,
         "ReportFormat": Literal["text/csv"],
         "GeneratedTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1438,16 +1447,16 @@
     "GetGroupPolicyRequestRequestTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
     },
 )
 
-GetGroupPolicyResponseTypeDef = TypedDict(
-    "GetGroupPolicyResponseTypeDef",
+GetGroupPolicyResponseOutputTypeDef = TypedDict(
+    "GetGroupPolicyResponseOutputTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1535,16 +1544,16 @@
 
 class GetMFADeviceRequestRequestTypeDef(
     _RequiredGetMFADeviceRequestRequestTypeDef, _OptionalGetMFADeviceRequestRequestTypeDef
 ):
     pass
 
 
-GetMFADeviceResponseTypeDef = TypedDict(
-    "GetMFADeviceResponseTypeDef",
+GetMFADeviceResponseOutputTypeDef = TypedDict(
+    "GetMFADeviceResponseOutputTypeDef",
     {
         "UserName": str,
         "SerialNumber": str,
         "EnableDate": datetime,
         "Certifications": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1600,16 +1609,16 @@
     "GetRolePolicyRequestRequestTypeDef",
     {
         "RoleName": str,
         "PolicyName": str,
     },
 )
 
-GetRolePolicyResponseTypeDef = TypedDict(
-    "GetRolePolicyResponseTypeDef",
+GetRolePolicyResponseOutputTypeDef = TypedDict(
+    "GetRolePolicyResponseOutputTypeDef",
     {
         "RoleName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1633,16 +1642,16 @@
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Encoding": encodingTypeType,
     },
 )
 
-SSHPublicKeyTypeDef = TypedDict(
-    "SSHPublicKeyTypeDef",
+SSHPublicKeyOutputTypeDef = TypedDict(
+    "SSHPublicKeyOutputTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Fingerprint": str,
         "SSHPublicKeyBody": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
@@ -1714,16 +1723,16 @@
     "GetUserPolicyRequestRequestTypeDef",
     {
         "UserName": str,
         "PolicyName": str,
     },
 )
 
-GetUserPolicyResponseTypeDef = TypedDict(
-    "GetUserPolicyResponseTypeDef",
+GetUserPolicyResponseOutputTypeDef = TypedDict(
+    "GetUserPolicyResponseOutputTypeDef",
     {
         "UserName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1732,16 +1741,16 @@
     "GetUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-PolicyDetailTypeDef = TypedDict(
-    "PolicyDetailTypeDef",
+PolicyDetailOutputTypeDef = TypedDict(
+    "PolicyDetailOutputTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
 
 ListAccessKeysRequestListAccessKeysPaginateTypeDef = TypedDict(
@@ -1776,16 +1785,16 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListAccountAliasesResponseTypeDef = TypedDict(
-    "ListAccountAliasesResponseTypeDef",
+ListAccountAliasesResponseOutputTypeDef = TypedDict(
+    "ListAccountAliasesResponseOutputTypeDef",
     {
         "AccountAliases": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1978,32 +1987,32 @@
 class ListEntitiesForPolicyRequestRequestTypeDef(
     _RequiredListEntitiesForPolicyRequestRequestTypeDef,
     _OptionalListEntitiesForPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-PolicyGroupTypeDef = TypedDict(
-    "PolicyGroupTypeDef",
+PolicyGroupOutputTypeDef = TypedDict(
+    "PolicyGroupOutputTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
 )
 
-PolicyRoleTypeDef = TypedDict(
-    "PolicyRoleTypeDef",
+PolicyRoleOutputTypeDef = TypedDict(
+    "PolicyRoleOutputTypeDef",
     {
         "RoleName": str,
         "RoleId": str,
     },
 )
 
-PolicyUserTypeDef = TypedDict(
-    "PolicyUserTypeDef",
+PolicyUserOutputTypeDef = TypedDict(
+    "PolicyUserOutputTypeDef",
     {
         "UserName": str,
         "UserId": str,
     },
 )
 
 _RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
@@ -2046,16 +2055,16 @@
 
 class ListGroupPoliciesRequestRequestTypeDef(
     _RequiredListGroupPoliciesRequestRequestTypeDef, _OptionalListGroupPoliciesRequestRequestTypeDef
 ):
     pass
 
 
-ListGroupPoliciesResponseTypeDef = TypedDict(
-    "ListGroupPoliciesResponseTypeDef",
+ListGroupPoliciesResponseOutputTypeDef = TypedDict(
+    "ListGroupPoliciesResponseOutputTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2291,16 +2300,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-MFADeviceTypeDef = TypedDict(
-    "MFADeviceTypeDef",
+MFADeviceOutputTypeDef = TypedDict(
+    "MFADeviceOutputTypeDef",
     {
         "UserName": str,
         "SerialNumber": str,
         "EnableDate": datetime,
     },
 )
 
@@ -2349,23 +2358,23 @@
 class ListOpenIDConnectProviderTagsRequestRequestTypeDef(
     _RequiredListOpenIDConnectProviderTagsRequestRequestTypeDef,
     _OptionalListOpenIDConnectProviderTagsRequestRequestTypeDef,
 ):
     pass
 
 
-OpenIDConnectProviderListEntryTypeDef = TypedDict(
-    "OpenIDConnectProviderListEntryTypeDef",
+OpenIDConnectProviderListEntryOutputTypeDef = TypedDict(
+    "OpenIDConnectProviderListEntryOutputTypeDef",
     {
         "Arn": str,
     },
 )
 
-PolicyGrantingServiceAccessTypeDef = TypedDict(
-    "PolicyGrantingServiceAccessTypeDef",
+PolicyGrantingServiceAccessOutputTypeDef = TypedDict(
+    "PolicyGrantingServiceAccessOutputTypeDef",
     {
         "PolicyName": str,
         "PolicyType": policyTypeType,
         "PolicyArn": str,
         "EntityType": policyOwnerEntityTypeType,
         "EntityName": str,
     },
@@ -2548,16 +2557,16 @@
 
 class ListRolePoliciesRequestRequestTypeDef(
     _RequiredListRolePoliciesRequestRequestTypeDef, _OptionalListRolePoliciesRequestRequestTypeDef
 ):
     pass
 
 
-ListRolePoliciesResponseTypeDef = TypedDict(
-    "ListRolePoliciesResponseTypeDef",
+ListRolePoliciesResponseOutputTypeDef = TypedDict(
+    "ListRolePoliciesResponseOutputTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2666,16 +2675,16 @@
 class ListSAMLProviderTagsRequestRequestTypeDef(
     _RequiredListSAMLProviderTagsRequestRequestTypeDef,
     _OptionalListSAMLProviderTagsRequestRequestTypeDef,
 ):
     pass
 
 
-SAMLProviderListEntryTypeDef = TypedDict(
-    "SAMLProviderListEntryTypeDef",
+SAMLProviderListEntryOutputTypeDef = TypedDict(
+    "SAMLProviderListEntryOutputTypeDef",
     {
         "Arn": str,
         "ValidUntil": datetime,
         "CreateDate": datetime,
     },
 )
 
@@ -2694,16 +2703,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-SSHPublicKeyMetadataTypeDef = TypedDict(
-    "SSHPublicKeyMetadataTypeDef",
+SSHPublicKeyMetadataOutputTypeDef = TypedDict(
+    "SSHPublicKeyMetadataOutputTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
     },
 )
@@ -2768,16 +2777,16 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ServerCertificateMetadataTypeDef = TypedDict(
-    "ServerCertificateMetadataTypeDef",
+ServerCertificateMetadataOutputTypeDef = TypedDict(
+    "ServerCertificateMetadataOutputTypeDef",
     {
         "Path": str,
         "ServerCertificateName": str,
         "ServerCertificateId": str,
         "Arn": str,
         "UploadDate": datetime,
         "Expiration": datetime,
@@ -2789,16 +2798,16 @@
     {
         "UserName": str,
         "ServiceName": str,
     },
     total=False,
 )
 
-ServiceSpecificCredentialMetadataTypeDef = TypedDict(
-    "ServiceSpecificCredentialMetadataTypeDef",
+ServiceSpecificCredentialMetadataOutputTypeDef = TypedDict(
+    "ServiceSpecificCredentialMetadataOutputTypeDef",
     {
         "UserName": str,
         "Status": statusTypeType,
         "ServiceUserName": str,
         "CreateDate": datetime,
         "ServiceSpecificCredentialId": str,
         "ServiceName": str,
@@ -2820,16 +2829,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-SigningCertificateTypeDef = TypedDict(
-    "SigningCertificateTypeDef",
+SigningCertificateOutputTypeDef = TypedDict(
+    "SigningCertificateOutputTypeDef",
     {
         "UserName": str,
         "CertificateId": str,
         "CertificateBody": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
     },
@@ -2875,16 +2884,16 @@
 
 class ListUserPoliciesRequestRequestTypeDef(
     _RequiredListUserPoliciesRequestRequestTypeDef, _OptionalListUserPoliciesRequestRequestTypeDef
 ):
     pass
 
 
-ListUserPoliciesResponseTypeDef = TypedDict(
-    "ListUserPoliciesResponseTypeDef",
+ListUserPoliciesResponseOutputTypeDef = TypedDict(
+    "ListUserPoliciesResponseOutputTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2977,16 +2986,16 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-PositionTypeDef = TypedDict(
-    "PositionTypeDef",
+PositionOutputTypeDef = TypedDict(
+    "PositionOutputTypeDef",
     {
         "Line": int,
         "Column": int,
     },
 )
 
 PutGroupPolicyRequestGroupCreatePolicyTypeDef = TypedDict(
@@ -3161,16 +3170,16 @@
         "UserName": str,
         "SerialNumber": str,
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
 
-RoleLastUsedTypeDef = TypedDict(
-    "RoleLastUsedTypeDef",
+RoleLastUsedOutputTypeDef = TypedDict(
+    "RoleLastUsedOutputTypeDef",
     {
         "LastUsedDate": datetime,
         "Region": str,
     },
 )
 
 RoleLastUsedResponseMetadataTypeDef = TypedDict(
@@ -3191,16 +3200,16 @@
         "Arn": str,
         "UploadDate": datetime,
         "Expiration": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TrackedActionLastAccessedTypeDef = TypedDict(
-    "TrackedActionLastAccessedTypeDef",
+TrackedActionLastAccessedOutputTypeDef = TypedDict(
+    "TrackedActionLastAccessedOutputTypeDef",
     {
         "ActionName": str,
         "LastAccessedEntity": str,
         "LastAccessedTime": datetime,
         "LastAccessedRegion": str,
     },
 )
@@ -3513,16 +3522,16 @@
 UpdateSAMLProviderRequestSamlProviderUpdateTypeDef = TypedDict(
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
     {
         "SAMLMetadataDocument": str,
     },
 )
 
-UpdateSAMLProviderResponseTypeDef = TypedDict(
-    "UpdateSAMLProviderResponseTypeDef",
+UpdateSAMLProviderResponseOutputTypeDef = TypedDict(
+    "UpdateSAMLProviderResponseOutputTypeDef",
     {
         "SAMLProviderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSSHPublicKeyRequestRequestTypeDef = TypedDict(
@@ -3707,65 +3716,65 @@
 class UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef(
     _RequiredUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
     _OptionalUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
 ):
     pass
 
 
-GetAccessKeyLastUsedResponseTypeDef = TypedDict(
-    "GetAccessKeyLastUsedResponseTypeDef",
+GetAccessKeyLastUsedResponseOutputTypeDef = TypedDict(
+    "GetAccessKeyLastUsedResponseOutputTypeDef",
     {
         "UserName": str,
-        "AccessKeyLastUsed": AccessKeyLastUsedTypeDef,
+        "AccessKeyLastUsed": AccessKeyLastUsedOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAccessKeysResponseTypeDef = TypedDict(
-    "ListAccessKeysResponseTypeDef",
+ListAccessKeysResponseOutputTypeDef = TypedDict(
+    "ListAccessKeysResponseOutputTypeDef",
     {
-        "AccessKeyMetadata": List[AccessKeyMetadataTypeDef],
+        "AccessKeyMetadata": List[AccessKeyMetadataOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateAccessKeyResponseTypeDef = TypedDict(
-    "CreateAccessKeyResponseTypeDef",
+CreateAccessKeyResponseOutputTypeDef = TypedDict(
+    "CreateAccessKeyResponseOutputTypeDef",
     {
-        "AccessKey": AccessKeyTypeDef,
+        "AccessKey": AccessKeyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedGroupPoliciesResponseTypeDef = TypedDict(
-    "ListAttachedGroupPoliciesResponseTypeDef",
+ListAttachedGroupPoliciesResponseOutputTypeDef = TypedDict(
+    "ListAttachedGroupPoliciesResponseOutputTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyTypeDef],
+        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedRolePoliciesResponseTypeDef = TypedDict(
-    "ListAttachedRolePoliciesResponseTypeDef",
+ListAttachedRolePoliciesResponseOutputTypeDef = TypedDict(
+    "ListAttachedRolePoliciesResponseOutputTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyTypeDef],
+        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedUserPoliciesResponseTypeDef = TypedDict(
-    "ListAttachedUserPoliciesResponseTypeDef",
+ListAttachedUserPoliciesResponseOutputTypeDef = TypedDict(
+    "ListAttachedUserPoliciesResponseOutputTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyTypeDef],
+        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSimulateCustomPolicyRequestRequestTypeDef = TypedDict(
@@ -3888,36 +3897,36 @@
 class SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef(
     _RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
     _OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
 ):
     pass
 
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
+CreateGroupResponseOutputTypeDef = TypedDict(
+    "CreateGroupResponseOutputTypeDef",
     {
-        "Group": GroupTypeDef,
+        "Group": GroupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGroupsForUserResponseTypeDef = TypedDict(
-    "ListGroupsForUserResponseTypeDef",
+ListGroupsForUserResponseOutputTypeDef = TypedDict(
+    "ListGroupsForUserResponseOutputTypeDef",
     {
-        "Groups": List[GroupTypeDef],
+        "Groups": List[GroupOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGroupsResponseTypeDef = TypedDict(
-    "ListGroupsResponseTypeDef",
+ListGroupsResponseOutputTypeDef = TypedDict(
+    "ListGroupsResponseOutputTypeDef",
     {
-        "Groups": List[GroupTypeDef],
+        "Groups": List[GroupOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateInstanceProfileRequestRequestTypeDef = TypedDict(
@@ -3986,23 +3995,14 @@
 class CreateOpenIDConnectProviderRequestRequestTypeDef(
     _RequiredCreateOpenIDConnectProviderRequestRequestTypeDef,
     _OptionalCreateOpenIDConnectProviderRequestRequestTypeDef,
 ):
     pass
 
 
-CreateOpenIDConnectProviderResponseTypeDef = TypedDict(
-    "CreateOpenIDConnectProviderResponseTypeDef",
-    {
-        "OpenIDConnectProviderArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
@@ -4143,23 +4143,14 @@
 class CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef(
     _RequiredCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef,
     _OptionalCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef,
 ):
     pass
 
 
-CreateSAMLProviderResponseTypeDef = TypedDict(
-    "CreateSAMLProviderResponseTypeDef",
-    {
-        "SAMLProviderArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
 _OptionalCreateUserRequestRequestTypeDef = TypedDict(
@@ -4255,135 +4246,14 @@
 class CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef(
     _RequiredCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef,
     _OptionalCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef,
 ):
     pass
 
 
-GetOpenIDConnectProviderResponseTypeDef = TypedDict(
-    "GetOpenIDConnectProviderResponseTypeDef",
-    {
-        "Url": str,
-        "ClientIDList": List[str],
-        "ThumbprintList": List[str],
-        "CreateDate": datetime,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSAMLProviderResponseTypeDef = TypedDict(
-    "GetSAMLProviderResponseTypeDef",
-    {
-        "SAMLMetadataDocument": str,
-        "CreateDate": datetime,
-        "ValidUntil": datetime,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListInstanceProfileTagsResponseTypeDef = TypedDict(
-    "ListInstanceProfileTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListMFADeviceTagsResponseTypeDef = TypedDict(
-    "ListMFADeviceTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListOpenIDConnectProviderTagsResponseTypeDef = TypedDict(
-    "ListOpenIDConnectProviderTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPolicyTagsResponseTypeDef = TypedDict(
-    "ListPolicyTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRoleTagsResponseTypeDef = TypedDict(
-    "ListRoleTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSAMLProviderTagsResponseTypeDef = TypedDict(
-    "ListSAMLProviderTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListServerCertificateTagsResponseTypeDef = TypedDict(
-    "ListServerCertificateTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListUserTagsResponseTypeDef = TypedDict(
-    "ListUserTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PolicyTypeDef = TypedDict(
-    "PolicyTypeDef",
-    {
-        "PolicyName": str,
-        "PolicyId": str,
-        "Arn": str,
-        "Path": str,
-        "DefaultVersionId": str,
-        "AttachmentCount": int,
-        "PermissionsBoundaryUsageCount": int,
-        "IsAttachable": bool,
-        "Description": str,
-        "CreateDate": datetime,
-        "UpdateDate": datetime,
-        "Tags": List[TagTypeDef],
-    },
-)
-
 TagInstanceProfileRequestRequestTypeDef = TypedDict(
     "TagInstanceProfileRequestRequestTypeDef",
     {
         "InstanceProfileName": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -4492,155 +4362,294 @@
 class UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef(
     _RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
     _OptionalUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
 ):
     pass
 
 
-UserResponseMetadataTypeDef = TypedDict(
-    "UserResponseMetadataTypeDef",
+CreateLoginProfileResponseOutputTypeDef = TypedDict(
+    "CreateLoginProfileResponseOutputTypeDef",
     {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
+        "LoginProfile": LoginProfileOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetLoginProfileResponseOutputTypeDef = TypedDict(
+    "GetLoginProfileResponseOutputTypeDef",
+    {
+        "LoginProfile": LoginProfileOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateOpenIDConnectProviderResponseOutputTypeDef = TypedDict(
+    "CreateOpenIDConnectProviderResponseOutputTypeDef",
+    {
+        "OpenIDConnectProviderArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSAMLProviderResponseOutputTypeDef = TypedDict(
+    "CreateSAMLProviderResponseOutputTypeDef",
+    {
+        "SAMLProviderArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetOpenIDConnectProviderResponseOutputTypeDef = TypedDict(
+    "GetOpenIDConnectProviderResponseOutputTypeDef",
+    {
+        "Url": str,
+        "ClientIDList": List[str],
+        "ThumbprintList": List[str],
         "CreateDate": datetime,
-        "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UserTypeDef = TypedDict(
-    "UserTypeDef",
+GetSAMLProviderResponseOutputTypeDef = TypedDict(
+    "GetSAMLProviderResponseOutputTypeDef",
     {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
+        "SAMLMetadataDocument": str,
         "CreateDate": datetime,
-        "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
+        "ValidUntil": datetime,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListInstanceProfileTagsResponseOutputTypeDef = TypedDict(
+    "ListInstanceProfileTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListMFADeviceTagsResponseOutputTypeDef = TypedDict(
+    "ListMFADeviceTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListOpenIDConnectProviderTagsResponseOutputTypeDef = TypedDict(
+    "ListOpenIDConnectProviderTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPolicyTagsResponseOutputTypeDef = TypedDict(
+    "ListPolicyTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListRoleTagsResponseOutputTypeDef = TypedDict(
+    "ListRoleTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSAMLProviderTagsResponseOutputTypeDef = TypedDict(
+    "ListSAMLProviderTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLoginProfileResponseTypeDef = TypedDict(
-    "CreateLoginProfileResponseTypeDef",
+ListServerCertificateTagsResponseOutputTypeDef = TypedDict(
+    "ListServerCertificateTagsResponseOutputTypeDef",
     {
-        "LoginProfile": LoginProfileTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetLoginProfileResponseTypeDef = TypedDict(
-    "GetLoginProfileResponseTypeDef",
+ListUserTagsResponseOutputTypeDef = TypedDict(
+    "ListUserTagsResponseOutputTypeDef",
     {
-        "LoginProfile": LoginProfileTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PolicyOutputTypeDef = TypedDict(
+    "PolicyOutputTypeDef",
+    {
+        "PolicyName": str,
+        "PolicyId": str,
+        "Arn": str,
+        "Path": str,
+        "DefaultVersionId": str,
+        "AttachmentCount": int,
+        "PermissionsBoundaryUsageCount": int,
+        "IsAttachable": bool,
+        "Description": str,
+        "CreateDate": datetime,
+        "UpdateDate": datetime,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+UserOutputTypeDef = TypedDict(
+    "UserOutputTypeDef",
+    {
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "PasswordLastUsed": datetime,
+        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+UserResponseMetadataTypeDef = TypedDict(
+    "UserResponseMetadataTypeDef",
+    {
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "PasswordLastUsed": datetime,
+        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreatePolicyVersionResponseTypeDef = TypedDict(
-    "CreatePolicyVersionResponseTypeDef",
+CreatePolicyVersionResponseOutputTypeDef = TypedDict(
+    "CreatePolicyVersionResponseOutputTypeDef",
     {
-        "PolicyVersion": PolicyVersionTypeDef,
+        "PolicyVersion": PolicyVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPolicyVersionResponseTypeDef = TypedDict(
-    "GetPolicyVersionResponseTypeDef",
+GetPolicyVersionResponseOutputTypeDef = TypedDict(
+    "GetPolicyVersionResponseOutputTypeDef",
     {
-        "PolicyVersion": PolicyVersionTypeDef,
+        "PolicyVersion": PolicyVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPolicyVersionsResponseTypeDef = TypedDict(
-    "ListPolicyVersionsResponseTypeDef",
+ListPolicyVersionsResponseOutputTypeDef = TypedDict(
+    "ListPolicyVersionsResponseOutputTypeDef",
     {
-        "Versions": List[PolicyVersionTypeDef],
+        "Versions": List[PolicyVersionOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ManagedPolicyDetailTypeDef = TypedDict(
-    "ManagedPolicyDetailTypeDef",
+ManagedPolicyDetailOutputTypeDef = TypedDict(
+    "ManagedPolicyDetailOutputTypeDef",
     {
         "PolicyName": str,
         "PolicyId": str,
         "Arn": str,
         "Path": str,
         "DefaultVersionId": str,
         "AttachmentCount": int,
         "PermissionsBoundaryUsageCount": int,
         "IsAttachable": bool,
         "Description": str,
         "CreateDate": datetime,
         "UpdateDate": datetime,
-        "PolicyVersionList": List[PolicyVersionTypeDef],
+        "PolicyVersionList": List[PolicyVersionOutputTypeDef],
     },
 )
 
-CreateServiceSpecificCredentialResponseTypeDef = TypedDict(
-    "CreateServiceSpecificCredentialResponseTypeDef",
+CreateServiceSpecificCredentialResponseOutputTypeDef = TypedDict(
+    "CreateServiceSpecificCredentialResponseOutputTypeDef",
     {
-        "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
+        "ServiceSpecificCredential": ServiceSpecificCredentialOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResetServiceSpecificCredentialResponseTypeDef = TypedDict(
-    "ResetServiceSpecificCredentialResponseTypeDef",
+ResetServiceSpecificCredentialResponseOutputTypeDef = TypedDict(
+    "ResetServiceSpecificCredentialResponseOutputTypeDef",
     {
-        "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
+        "ServiceSpecificCredential": ServiceSpecificCredentialOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeletionTaskFailureReasonTypeTypeDef = TypedDict(
-    "DeletionTaskFailureReasonTypeTypeDef",
+DeletionTaskFailureReasonTypeOutputTypeDef = TypedDict(
+    "DeletionTaskFailureReasonTypeOutputTypeDef",
     {
         "Reason": str,
-        "RoleUsageList": List[RoleUsageTypeTypeDef],
+        "RoleUsageList": List[RoleUsageTypeOutputTypeDef],
     },
 )
 
-EntityDetailsTypeDef = TypedDict(
-    "EntityDetailsTypeDef",
+EntityDetailsOutputTypeDef = TypedDict(
+    "EntityDetailsOutputTypeDef",
     {
-        "EntityInfo": EntityInfoTypeDef,
+        "EntityInfo": EntityInfoOutputTypeDef,
         "LastAuthenticated": datetime,
     },
 )
 
-GetOrganizationsAccessReportResponseTypeDef = TypedDict(
-    "GetOrganizationsAccessReportResponseTypeDef",
+GetOrganizationsAccessReportResponseOutputTypeDef = TypedDict(
+    "GetOrganizationsAccessReportResponseOutputTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
         "NumberOfServicesAccessible": int,
         "NumberOfServicesNotAccessed": int,
-        "AccessDetails": List[AccessDetailTypeDef],
+        "AccessDetails": List[AccessDetailOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ErrorDetails": ErrorDetailsTypeDef,
+        "ErrorDetails": ErrorDetailsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccountPasswordPolicyResponseTypeDef = TypedDict(
-    "GetAccountPasswordPolicyResponseTypeDef",
+GetAccountPasswordPolicyResponseOutputTypeDef = TypedDict(
+    "GetAccountPasswordPolicyResponseOutputTypeDef",
     {
-        "PasswordPolicy": PasswordPolicyTypeDef,
+        "PasswordPolicy": PasswordPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef = TypedDict(
     "_RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     {
@@ -4711,510 +4720,510 @@
     {
         "UserName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-GetSSHPublicKeyResponseTypeDef = TypedDict(
-    "GetSSHPublicKeyResponseTypeDef",
+GetSSHPublicKeyResponseOutputTypeDef = TypedDict(
+    "GetSSHPublicKeyResponseOutputTypeDef",
     {
-        "SSHPublicKey": SSHPublicKeyTypeDef,
+        "SSHPublicKey": SSHPublicKeyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadSSHPublicKeyResponseTypeDef = TypedDict(
-    "UploadSSHPublicKeyResponseTypeDef",
+UploadSSHPublicKeyResponseOutputTypeDef = TypedDict(
+    "UploadSSHPublicKeyResponseOutputTypeDef",
     {
-        "SSHPublicKey": SSHPublicKeyTypeDef,
+        "SSHPublicKey": SSHPublicKeyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GroupDetailTypeDef = TypedDict(
-    "GroupDetailTypeDef",
+GroupDetailOutputTypeDef = TypedDict(
+    "GroupDetailOutputTypeDef",
     {
         "Path": str,
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "GroupPolicyList": List[PolicyDetailTypeDef],
-        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
+        "GroupPolicyList": List[PolicyDetailOutputTypeDef],
+        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
     },
 )
 
-UserDetailTypeDef = TypedDict(
-    "UserDetailTypeDef",
+UserDetailOutputTypeDef = TypedDict(
+    "UserDetailOutputTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "UserPolicyList": List[PolicyDetailTypeDef],
+        "UserPolicyList": List[PolicyDetailOutputTypeDef],
         "GroupList": List[str],
-        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
+        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
+        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
-ListEntitiesForPolicyResponseTypeDef = TypedDict(
-    "ListEntitiesForPolicyResponseTypeDef",
+ListEntitiesForPolicyResponseOutputTypeDef = TypedDict(
+    "ListEntitiesForPolicyResponseOutputTypeDef",
     {
-        "PolicyGroups": List[PolicyGroupTypeDef],
-        "PolicyUsers": List[PolicyUserTypeDef],
-        "PolicyRoles": List[PolicyRoleTypeDef],
+        "PolicyGroups": List[PolicyGroupOutputTypeDef],
+        "PolicyUsers": List[PolicyUserOutputTypeDef],
+        "PolicyRoles": List[PolicyRoleOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListMFADevicesResponseTypeDef = TypedDict(
-    "ListMFADevicesResponseTypeDef",
+ListMFADevicesResponseOutputTypeDef = TypedDict(
+    "ListMFADevicesResponseOutputTypeDef",
     {
-        "MFADevices": List[MFADeviceTypeDef],
+        "MFADevices": List[MFADeviceOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListOpenIDConnectProvidersResponseTypeDef = TypedDict(
-    "ListOpenIDConnectProvidersResponseTypeDef",
+ListOpenIDConnectProvidersResponseOutputTypeDef = TypedDict(
+    "ListOpenIDConnectProvidersResponseOutputTypeDef",
     {
-        "OpenIDConnectProviderList": List[OpenIDConnectProviderListEntryTypeDef],
+        "OpenIDConnectProviderList": List[OpenIDConnectProviderListEntryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesGrantingServiceAccessEntryTypeDef = TypedDict(
-    "ListPoliciesGrantingServiceAccessEntryTypeDef",
+ListPoliciesGrantingServiceAccessEntryOutputTypeDef = TypedDict(
+    "ListPoliciesGrantingServiceAccessEntryOutputTypeDef",
     {
         "ServiceNamespace": str,
-        "Policies": List[PolicyGrantingServiceAccessTypeDef],
+        "Policies": List[PolicyGrantingServiceAccessOutputTypeDef],
     },
 )
 
-ListSAMLProvidersResponseTypeDef = TypedDict(
-    "ListSAMLProvidersResponseTypeDef",
+ListSAMLProvidersResponseOutputTypeDef = TypedDict(
+    "ListSAMLProvidersResponseOutputTypeDef",
     {
-        "SAMLProviderList": List[SAMLProviderListEntryTypeDef],
+        "SAMLProviderList": List[SAMLProviderListEntryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSSHPublicKeysResponseTypeDef = TypedDict(
-    "ListSSHPublicKeysResponseTypeDef",
+ListSSHPublicKeysResponseOutputTypeDef = TypedDict(
+    "ListSSHPublicKeysResponseOutputTypeDef",
     {
-        "SSHPublicKeys": List[SSHPublicKeyMetadataTypeDef],
+        "SSHPublicKeys": List[SSHPublicKeyMetadataOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServerCertificatesResponseTypeDef = TypedDict(
-    "ListServerCertificatesResponseTypeDef",
+ListServerCertificatesResponseOutputTypeDef = TypedDict(
+    "ListServerCertificatesResponseOutputTypeDef",
     {
-        "ServerCertificateMetadataList": List[ServerCertificateMetadataTypeDef],
+        "ServerCertificateMetadataList": List[ServerCertificateMetadataOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ServerCertificateTypeDef = TypedDict(
-    "ServerCertificateTypeDef",
+ServerCertificateOutputTypeDef = TypedDict(
+    "ServerCertificateOutputTypeDef",
     {
-        "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
+        "ServerCertificateMetadata": ServerCertificateMetadataOutputTypeDef,
         "CertificateBody": str,
         "CertificateChain": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
-UploadServerCertificateResponseTypeDef = TypedDict(
-    "UploadServerCertificateResponseTypeDef",
+UploadServerCertificateResponseOutputTypeDef = TypedDict(
+    "UploadServerCertificateResponseOutputTypeDef",
     {
-        "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
-        "Tags": List[TagTypeDef],
+        "ServerCertificateMetadata": ServerCertificateMetadataOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceSpecificCredentialsResponseTypeDef = TypedDict(
-    "ListServiceSpecificCredentialsResponseTypeDef",
+ListServiceSpecificCredentialsResponseOutputTypeDef = TypedDict(
+    "ListServiceSpecificCredentialsResponseOutputTypeDef",
     {
-        "ServiceSpecificCredentials": List[ServiceSpecificCredentialMetadataTypeDef],
+        "ServiceSpecificCredentials": List[ServiceSpecificCredentialMetadataOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSigningCertificatesResponseTypeDef = TypedDict(
-    "ListSigningCertificatesResponseTypeDef",
+ListSigningCertificatesResponseOutputTypeDef = TypedDict(
+    "ListSigningCertificatesResponseOutputTypeDef",
     {
-        "Certificates": List[SigningCertificateTypeDef],
+        "Certificates": List[SigningCertificateOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadSigningCertificateResponseTypeDef = TypedDict(
-    "UploadSigningCertificateResponseTypeDef",
+UploadSigningCertificateResponseOutputTypeDef = TypedDict(
+    "UploadSigningCertificateResponseOutputTypeDef",
     {
-        "Certificate": SigningCertificateTypeDef,
+        "Certificate": SigningCertificateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StatementTypeDef = TypedDict(
-    "StatementTypeDef",
+StatementOutputTypeDef = TypedDict(
+    "StatementOutputTypeDef",
     {
         "SourcePolicyId": str,
         "SourcePolicyType": PolicySourceTypeType,
-        "StartPosition": PositionTypeDef,
-        "EndPosition": PositionTypeDef,
+        "StartPosition": PositionOutputTypeDef,
+        "EndPosition": PositionOutputTypeDef,
     },
 )
 
-RoleTypeDef = TypedDict(
-    "RoleTypeDef",
+RoleOutputTypeDef = TypedDict(
+    "RoleOutputTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
         "CreateDate": datetime,
         "AssumeRolePolicyDocument": str,
         "Description": str,
         "MaxSessionDuration": int,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-        "RoleLastUsed": RoleLastUsedTypeDef,
+        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "RoleLastUsed": RoleLastUsedOutputTypeDef,
     },
 )
 
-ServiceLastAccessedTypeDef = TypedDict(
-    "ServiceLastAccessedTypeDef",
+ServiceLastAccessedOutputTypeDef = TypedDict(
+    "ServiceLastAccessedOutputTypeDef",
     {
         "ServiceName": str,
         "LastAuthenticated": datetime,
         "ServiceNamespace": str,
         "LastAuthenticatedEntity": str,
         "LastAuthenticatedRegion": str,
         "TotalAuthenticatedEntities": int,
-        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
+        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedOutputTypeDef],
     },
 )
 
-CreatePolicyResponseTypeDef = TypedDict(
-    "CreatePolicyResponseTypeDef",
+CreatePolicyResponseOutputTypeDef = TypedDict(
+    "CreatePolicyResponseOutputTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
+GetPolicyResponseOutputTypeDef = TypedDict(
+    "GetPolicyResponseOutputTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesResponseTypeDef = TypedDict(
-    "ListPoliciesResponseTypeDef",
+ListPoliciesResponseOutputTypeDef = TypedDict(
+    "ListPoliciesResponseOutputTypeDef",
     {
-        "Policies": List[PolicyTypeDef],
+        "Policies": List[PolicyOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
+CreateUserResponseOutputTypeDef = TypedDict(
+    "CreateUserResponseOutputTypeDef",
     {
-        "User": UserTypeDef,
+        "User": UserOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
+GetGroupResponseOutputTypeDef = TypedDict(
+    "GetGroupResponseOutputTypeDef",
     {
-        "Group": GroupTypeDef,
-        "Users": List[UserTypeDef],
+        "Group": GroupOutputTypeDef,
+        "Users": List[UserOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetUserResponseTypeDef = TypedDict(
-    "GetUserResponseTypeDef",
+GetUserResponseOutputTypeDef = TypedDict(
+    "GetUserResponseOutputTypeDef",
     {
-        "User": UserTypeDef,
+        "User": UserOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListUsersResponseTypeDef = TypedDict(
-    "ListUsersResponseTypeDef",
+ListUsersResponseOutputTypeDef = TypedDict(
+    "ListUsersResponseOutputTypeDef",
     {
-        "Users": List[UserTypeDef],
+        "Users": List[UserOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VirtualMFADeviceTypeDef = TypedDict(
-    "VirtualMFADeviceTypeDef",
+VirtualMFADeviceOutputTypeDef = TypedDict(
+    "VirtualMFADeviceOutputTypeDef",
     {
         "SerialNumber": str,
         "Base32StringSeed": bytes,
         "QRCodePNG": bytes,
-        "User": UserTypeDef,
+        "User": UserOutputTypeDef,
         "EnableDate": datetime,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
-GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
-    "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
+GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef = TypedDict(
+    "GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
-        "Reason": DeletionTaskFailureReasonTypeTypeDef,
+        "Reason": DeletionTaskFailureReasonTypeOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef = TypedDict(
-    "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
+GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef = TypedDict(
+    "GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
-        "EntityDetailsList": List[EntityDetailsTypeDef],
+        "EntityDetailsList": List[EntityDetailsOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "Error": ErrorDetailsTypeDef,
+        "Error": ErrorDetailsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesGrantingServiceAccessResponseTypeDef = TypedDict(
-    "ListPoliciesGrantingServiceAccessResponseTypeDef",
+ListPoliciesGrantingServiceAccessResponseOutputTypeDef = TypedDict(
+    "ListPoliciesGrantingServiceAccessResponseOutputTypeDef",
     {
-        "PoliciesGrantingServiceAccess": List[ListPoliciesGrantingServiceAccessEntryTypeDef],
+        "PoliciesGrantingServiceAccess": List[ListPoliciesGrantingServiceAccessEntryOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServerCertificateResponseTypeDef = TypedDict(
-    "GetServerCertificateResponseTypeDef",
+GetServerCertificateResponseOutputTypeDef = TypedDict(
+    "GetServerCertificateResponseOutputTypeDef",
     {
-        "ServerCertificate": ServerCertificateTypeDef,
+        "ServerCertificate": ServerCertificateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResourceSpecificResultTypeDef = TypedDict(
-    "ResourceSpecificResultTypeDef",
+ResourceSpecificResultOutputTypeDef = TypedDict(
+    "ResourceSpecificResultOutputTypeDef",
     {
         "EvalResourceName": str,
         "EvalResourceDecision": PolicyEvaluationDecisionTypeType,
-        "MatchedStatements": List[StatementTypeDef],
+        "MatchedStatements": List[StatementOutputTypeDef],
         "MissingContextValues": List[str],
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
-        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
+        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailOutputTypeDef,
     },
 )
 
-CreateRoleResponseTypeDef = TypedDict(
-    "CreateRoleResponseTypeDef",
+CreateRoleResponseOutputTypeDef = TypedDict(
+    "CreateRoleResponseOutputTypeDef",
     {
-        "Role": RoleTypeDef,
+        "Role": RoleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceLinkedRoleResponseTypeDef = TypedDict(
-    "CreateServiceLinkedRoleResponseTypeDef",
+CreateServiceLinkedRoleResponseOutputTypeDef = TypedDict(
+    "CreateServiceLinkedRoleResponseOutputTypeDef",
     {
-        "Role": RoleTypeDef,
+        "Role": RoleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetRoleResponseTypeDef = TypedDict(
-    "GetRoleResponseTypeDef",
+GetRoleResponseOutputTypeDef = TypedDict(
+    "GetRoleResponseOutputTypeDef",
     {
-        "Role": RoleTypeDef,
+        "Role": RoleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InstanceProfileTypeDef = TypedDict(
-    "InstanceProfileTypeDef",
+InstanceProfileOutputTypeDef = TypedDict(
+    "InstanceProfileOutputTypeDef",
     {
         "Path": str,
         "InstanceProfileName": str,
         "InstanceProfileId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "Roles": List[RoleTypeDef],
-        "Tags": List[TagTypeDef],
+        "Roles": List[RoleOutputTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
-ListRolesResponseTypeDef = TypedDict(
-    "ListRolesResponseTypeDef",
+ListRolesResponseOutputTypeDef = TypedDict(
+    "ListRolesResponseOutputTypeDef",
     {
-        "Roles": List[RoleTypeDef],
+        "Roles": List[RoleOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRoleDescriptionResponseTypeDef = TypedDict(
-    "UpdateRoleDescriptionResponseTypeDef",
+UpdateRoleDescriptionResponseOutputTypeDef = TypedDict(
+    "UpdateRoleDescriptionResponseOutputTypeDef",
     {
-        "Role": RoleTypeDef,
+        "Role": RoleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceLastAccessedDetailsResponseTypeDef = TypedDict(
-    "GetServiceLastAccessedDetailsResponseTypeDef",
+GetServiceLastAccessedDetailsResponseOutputTypeDef = TypedDict(
+    "GetServiceLastAccessedDetailsResponseOutputTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobType": AccessAdvisorUsageGranularityTypeType,
         "JobCreationDate": datetime,
-        "ServicesLastAccessed": List[ServiceLastAccessedTypeDef],
+        "ServicesLastAccessed": List[ServiceLastAccessedOutputTypeDef],
         "JobCompletionDate": datetime,
         "IsTruncated": bool,
         "Marker": str,
-        "Error": ErrorDetailsTypeDef,
+        "Error": ErrorDetailsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVirtualMFADeviceResponseTypeDef = TypedDict(
-    "CreateVirtualMFADeviceResponseTypeDef",
+CreateVirtualMFADeviceResponseOutputTypeDef = TypedDict(
+    "CreateVirtualMFADeviceResponseOutputTypeDef",
     {
-        "VirtualMFADevice": VirtualMFADeviceTypeDef,
+        "VirtualMFADevice": VirtualMFADeviceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListVirtualMFADevicesResponseTypeDef = TypedDict(
-    "ListVirtualMFADevicesResponseTypeDef",
+ListVirtualMFADevicesResponseOutputTypeDef = TypedDict(
+    "ListVirtualMFADevicesResponseOutputTypeDef",
     {
-        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
+        "VirtualMFADevices": List[VirtualMFADeviceOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EvaluationResultTypeDef = TypedDict(
-    "EvaluationResultTypeDef",
+EvaluationResultOutputTypeDef = TypedDict(
+    "EvaluationResultOutputTypeDef",
     {
         "EvalActionName": str,
         "EvalResourceName": str,
         "EvalDecision": PolicyEvaluationDecisionTypeType,
-        "MatchedStatements": List[StatementTypeDef],
+        "MatchedStatements": List[StatementOutputTypeDef],
         "MissingContextValues": List[str],
-        "OrganizationsDecisionDetail": OrganizationsDecisionDetailTypeDef,
-        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
+        "OrganizationsDecisionDetail": OrganizationsDecisionDetailOutputTypeDef,
+        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailOutputTypeDef,
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
-        "ResourceSpecificResults": List[ResourceSpecificResultTypeDef],
+        "ResourceSpecificResults": List[ResourceSpecificResultOutputTypeDef],
     },
 )
 
-CreateInstanceProfileResponseTypeDef = TypedDict(
-    "CreateInstanceProfileResponseTypeDef",
+CreateInstanceProfileResponseOutputTypeDef = TypedDict(
+    "CreateInstanceProfileResponseOutputTypeDef",
     {
-        "InstanceProfile": InstanceProfileTypeDef,
+        "InstanceProfile": InstanceProfileOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetInstanceProfileResponseTypeDef = TypedDict(
-    "GetInstanceProfileResponseTypeDef",
+GetInstanceProfileResponseOutputTypeDef = TypedDict(
+    "GetInstanceProfileResponseOutputTypeDef",
     {
-        "InstanceProfile": InstanceProfileTypeDef,
+        "InstanceProfile": InstanceProfileOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListInstanceProfilesForRoleResponseTypeDef = TypedDict(
-    "ListInstanceProfilesForRoleResponseTypeDef",
+ListInstanceProfilesForRoleResponseOutputTypeDef = TypedDict(
+    "ListInstanceProfilesForRoleResponseOutputTypeDef",
     {
-        "InstanceProfiles": List[InstanceProfileTypeDef],
+        "InstanceProfiles": List[InstanceProfileOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListInstanceProfilesResponseTypeDef = TypedDict(
-    "ListInstanceProfilesResponseTypeDef",
+ListInstanceProfilesResponseOutputTypeDef = TypedDict(
+    "ListInstanceProfilesResponseOutputTypeDef",
     {
-        "InstanceProfiles": List[InstanceProfileTypeDef],
+        "InstanceProfiles": List[InstanceProfileOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RoleDetailTypeDef = TypedDict(
-    "RoleDetailTypeDef",
+RoleDetailOutputTypeDef = TypedDict(
+    "RoleDetailOutputTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
         "CreateDate": datetime,
         "AssumeRolePolicyDocument": str,
-        "InstanceProfileList": List[InstanceProfileTypeDef],
-        "RolePolicyList": List[PolicyDetailTypeDef],
-        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-        "RoleLastUsed": RoleLastUsedTypeDef,
+        "InstanceProfileList": List[InstanceProfileOutputTypeDef],
+        "RolePolicyList": List[PolicyDetailOutputTypeDef],
+        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
+        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "RoleLastUsed": RoleLastUsedOutputTypeDef,
     },
 )
 
-SimulatePolicyResponseTypeDef = TypedDict(
-    "SimulatePolicyResponseTypeDef",
+SimulatePolicyResponseOutputTypeDef = TypedDict(
+    "SimulatePolicyResponseOutputTypeDef",
     {
-        "EvaluationResults": List[EvaluationResultTypeDef],
+        "EvaluationResults": List[EvaluationResultOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccountAuthorizationDetailsResponseTypeDef = TypedDict(
-    "GetAccountAuthorizationDetailsResponseTypeDef",
+GetAccountAuthorizationDetailsResponseOutputTypeDef = TypedDict(
+    "GetAccountAuthorizationDetailsResponseOutputTypeDef",
     {
-        "UserDetailList": List[UserDetailTypeDef],
-        "GroupDetailList": List[GroupDetailTypeDef],
-        "RoleDetailList": List[RoleDetailTypeDef],
-        "Policies": List[ManagedPolicyDetailTypeDef],
+        "UserDetailList": List[UserDetailOutputTypeDef],
+        "GroupDetailList": List[GroupDetailOutputTypeDef],
+        "RoleDetailList": List[RoleDetailOutputTypeDef],
+        "Policies": List[ManagedPolicyDetailOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/type_defs.pyi` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/type_defs.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iam service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iam.type_defs import AccessDetailTypeDef
+    from mypy_boto3_iam.type_defs import AccessDetailOutputTypeDef
 
-    data: AccessDetailTypeDef = {...}
+    data: AccessDetailOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -42,18 +42,18 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AccessDetailTypeDef",
-    "AccessKeyLastUsedTypeDef",
-    "AccessKeyMetadataTypeDef",
-    "AccessKeyTypeDef",
+    "AccessDetailOutputTypeDef",
+    "AccessKeyLastUsedOutputTypeDef",
+    "AccessKeyMetadataOutputTypeDef",
+    "AccessKeyOutputTypeDef",
     "AddClientIDToOpenIDConnectProviderRequestRequestTypeDef",
     "AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef",
     "AddRoleToInstanceProfileRequestRequestTypeDef",
     "AddUserToGroupRequestGroupAddUserTypeDef",
     "AddUserToGroupRequestRequestTypeDef",
     "AddUserToGroupRequestUserAddGroupTypeDef",
     "AttachGroupPolicyRequestGroupAttachPolicyTypeDef",
@@ -61,38 +61,39 @@
     "AttachGroupPolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestPolicyAttachRoleTypeDef",
     "AttachRolePolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestRoleAttachPolicyTypeDef",
     "AttachUserPolicyRequestPolicyAttachUserTypeDef",
     "AttachUserPolicyRequestRequestTypeDef",
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
+    "AttachedPermissionsBoundaryOutputTypeDef",
     "AttachedPermissionsBoundaryResponseMetadataTypeDef",
-    "AttachedPermissionsBoundaryTypeDef",
-    "AttachedPolicyTypeDef",
+    "AttachedPolicyOutputTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "ChangePasswordRequestServiceResourceChangePasswordTypeDef",
     "ContextEntryTypeDef",
     "CreateAccessKeyRequestRequestTypeDef",
     "CreateAccountAliasRequestRequestTypeDef",
     "CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef",
     "CreateGroupRequestGroupCreateTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateGroupRequestServiceResourceCreateGroupTypeDef",
-    "GroupTypeDef",
+    "GroupOutputTypeDef",
     "TagTypeDef",
     "CreateLoginProfileRequestLoginProfileCreateTypeDef",
     "CreateLoginProfileRequestRequestTypeDef",
     "CreateLoginProfileRequestUserCreateLoginProfileTypeDef",
-    "LoginProfileTypeDef",
+    "LoginProfileOutputTypeDef",
+    "TagOutputTypeDef",
     "CreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
-    "PolicyVersionTypeDef",
+    "PolicyVersionOutputTypeDef",
     "CreateServiceLinkedRoleRequestRequestTypeDef",
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
-    "ServiceSpecificCredentialTypeDef",
+    "ServiceSpecificCredentialOutputTypeDef",
     "DeactivateMFADeviceRequestRequestTypeDef",
     "DeleteAccessKeyRequestRequestTypeDef",
     "DeleteAccountAliasRequestRequestTypeDef",
     "DeleteGroupPolicyRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteInstanceProfileRequestRequestTypeDef",
     "DeleteLoginProfileRequestRequestTypeDef",
@@ -102,159 +103,159 @@
     "DeleteRolePermissionsBoundaryRequestRequestTypeDef",
     "DeleteRolePolicyRequestRequestTypeDef",
     "DeleteRoleRequestRequestTypeDef",
     "DeleteSAMLProviderRequestRequestTypeDef",
     "DeleteSSHPublicKeyRequestRequestTypeDef",
     "DeleteServerCertificateRequestRequestTypeDef",
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
-    "DeleteServiceLinkedRoleResponseTypeDef",
+    "DeleteServiceLinkedRoleResponseOutputTypeDef",
     "DeleteServiceSpecificCredentialRequestRequestTypeDef",
     "DeleteSigningCertificateRequestRequestTypeDef",
     "DeleteUserPermissionsBoundaryRequestRequestTypeDef",
     "DeleteUserPolicyRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteVirtualMFADeviceRequestRequestTypeDef",
-    "RoleUsageTypeTypeDef",
+    "RoleUsageTypeOutputTypeDef",
     "DetachGroupPolicyRequestGroupDetachPolicyTypeDef",
     "DetachGroupPolicyRequestPolicyDetachGroupTypeDef",
     "DetachGroupPolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestPolicyDetachRoleTypeDef",
     "DetachRolePolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestRoleDetachPolicyTypeDef",
     "DetachUserPolicyRequestPolicyDetachUserTypeDef",
     "DetachUserPolicyRequestRequestTypeDef",
     "DetachUserPolicyRequestUserDetachPolicyTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableMFADeviceRequestMfaDeviceAssociateTypeDef",
     "EnableMFADeviceRequestRequestTypeDef",
     "EnableMFADeviceRequestUserEnableMfaTypeDef",
-    "EntityInfoTypeDef",
-    "ErrorDetailsTypeDef",
-    "OrganizationsDecisionDetailTypeDef",
-    "PermissionsBoundaryDecisionDetailTypeDef",
-    "GenerateCredentialReportResponseTypeDef",
+    "EntityInfoOutputTypeDef",
+    "ErrorDetailsOutputTypeDef",
+    "OrganizationsDecisionDetailOutputTypeDef",
+    "PermissionsBoundaryDecisionDetailOutputTypeDef",
+    "GenerateCredentialReportResponseOutputTypeDef",
     "GenerateOrganizationsAccessReportRequestRequestTypeDef",
-    "GenerateOrganizationsAccessReportResponseTypeDef",
+    "GenerateOrganizationsAccessReportResponseOutputTypeDef",
     "GenerateServiceLastAccessedDetailsRequestRequestTypeDef",
-    "GenerateServiceLastAccessedDetailsResponseTypeDef",
+    "GenerateServiceLastAccessedDetailsResponseOutputTypeDef",
     "GetAccessKeyLastUsedRequestRequestTypeDef",
     "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
     "GetAccountAuthorizationDetailsRequestRequestTypeDef",
-    "PasswordPolicyTypeDef",
-    "GetAccountSummaryResponseTypeDef",
+    "PasswordPolicyOutputTypeDef",
+    "GetAccountSummaryResponseOutputTypeDef",
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
-    "GetContextKeysForPolicyResponseTypeDef",
+    "GetContextKeysForPolicyResponseOutputTypeDef",
     "GetContextKeysForPrincipalPolicyRequestRequestTypeDef",
-    "GetCredentialReportResponseTypeDef",
+    "GetCredentialReportResponseOutputTypeDef",
     "GetGroupPolicyRequestRequestTypeDef",
-    "GetGroupPolicyResponseTypeDef",
+    "GetGroupPolicyResponseOutputTypeDef",
     "GetGroupRequestGetGroupPaginateTypeDef",
     "GetGroupRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
     "GetLoginProfileRequestRequestTypeDef",
     "GetMFADeviceRequestRequestTypeDef",
-    "GetMFADeviceResponseTypeDef",
+    "GetMFADeviceResponseOutputTypeDef",
     "GetOpenIDConnectProviderRequestRequestTypeDef",
     "GetOrganizationsAccessReportRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetPolicyVersionRequestRequestTypeDef",
     "GetRolePolicyRequestRequestTypeDef",
-    "GetRolePolicyResponseTypeDef",
+    "GetRolePolicyResponseOutputTypeDef",
     "GetRoleRequestRequestTypeDef",
     "GetSAMLProviderRequestRequestTypeDef",
     "GetSSHPublicKeyRequestRequestTypeDef",
-    "SSHPublicKeyTypeDef",
+    "SSHPublicKeyOutputTypeDef",
     "GetServerCertificateRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef",
     "GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef",
     "GetUserPolicyRequestRequestTypeDef",
-    "GetUserPolicyResponseTypeDef",
+    "GetUserPolicyResponseOutputTypeDef",
     "GetUserRequestRequestTypeDef",
-    "PolicyDetailTypeDef",
+    "PolicyDetailOutputTypeDef",
     "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
     "ListAccessKeysRequestRequestTypeDef",
     "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
     "ListAccountAliasesRequestRequestTypeDef",
-    "ListAccountAliasesResponseTypeDef",
+    "ListAccountAliasesResponseOutputTypeDef",
     "ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
     "ListAttachedGroupPoliciesRequestRequestTypeDef",
     "ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
     "ListAttachedRolePoliciesRequestRequestTypeDef",
     "ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
     "ListAttachedUserPoliciesRequestRequestTypeDef",
     "ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
     "ListEntitiesForPolicyRequestRequestTypeDef",
-    "PolicyGroupTypeDef",
-    "PolicyRoleTypeDef",
-    "PolicyUserTypeDef",
+    "PolicyGroupOutputTypeDef",
+    "PolicyRoleOutputTypeDef",
+    "PolicyUserOutputTypeDef",
     "ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
     "ListGroupPoliciesRequestRequestTypeDef",
-    "ListGroupPoliciesResponseTypeDef",
+    "ListGroupPoliciesResponseOutputTypeDef",
     "ListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
     "ListGroupsForUserRequestRequestTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
     "ListInstanceProfileTagsRequestRequestTypeDef",
     "ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
     "ListInstanceProfilesForRoleRequestRequestTypeDef",
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListInstanceProfilesRequestRequestTypeDef",
     "ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
     "ListMFADeviceTagsRequestRequestTypeDef",
     "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
     "ListMFADevicesRequestRequestTypeDef",
-    "MFADeviceTypeDef",
+    "MFADeviceOutputTypeDef",
     "ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
     "ListOpenIDConnectProviderTagsRequestRequestTypeDef",
-    "OpenIDConnectProviderListEntryTypeDef",
-    "PolicyGrantingServiceAccessTypeDef",
+    "OpenIDConnectProviderListEntryOutputTypeDef",
+    "PolicyGrantingServiceAccessOutputTypeDef",
     "ListPoliciesGrantingServiceAccessRequestRequestTypeDef",
     "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "ListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
     "ListPolicyTagsRequestRequestTypeDef",
     "ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
     "ListPolicyVersionsRequestRequestTypeDef",
     "ListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
     "ListRolePoliciesRequestRequestTypeDef",
-    "ListRolePoliciesResponseTypeDef",
+    "ListRolePoliciesResponseOutputTypeDef",
     "ListRoleTagsRequestListRoleTagsPaginateTypeDef",
     "ListRoleTagsRequestRequestTypeDef",
     "ListRolesRequestListRolesPaginateTypeDef",
     "ListRolesRequestRequestTypeDef",
     "ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
     "ListSAMLProviderTagsRequestRequestTypeDef",
-    "SAMLProviderListEntryTypeDef",
+    "SAMLProviderListEntryOutputTypeDef",
     "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
     "ListSSHPublicKeysRequestRequestTypeDef",
-    "SSHPublicKeyMetadataTypeDef",
+    "SSHPublicKeyMetadataOutputTypeDef",
     "ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
     "ListServerCertificateTagsRequestRequestTypeDef",
     "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
     "ListServerCertificatesRequestRequestTypeDef",
-    "ServerCertificateMetadataTypeDef",
+    "ServerCertificateMetadataOutputTypeDef",
     "ListServiceSpecificCredentialsRequestRequestTypeDef",
-    "ServiceSpecificCredentialMetadataTypeDef",
+    "ServiceSpecificCredentialMetadataOutputTypeDef",
     "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
     "ListSigningCertificatesRequestRequestTypeDef",
-    "SigningCertificateTypeDef",
+    "SigningCertificateOutputTypeDef",
     "ListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
     "ListUserPoliciesRequestRequestTypeDef",
-    "ListUserPoliciesResponseTypeDef",
+    "ListUserPoliciesResponseOutputTypeDef",
     "ListUserTagsRequestListUserTagsPaginateTypeDef",
     "ListUserTagsRequestRequestTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
     "ListVirtualMFADevicesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "PositionTypeDef",
+    "PositionOutputTypeDef",
     "PutGroupPolicyRequestGroupCreatePolicyTypeDef",
     "PutGroupPolicyRequestGroupPolicyPutTypeDef",
     "PutGroupPolicyRequestRequestTypeDef",
     "PutRolePermissionsBoundaryRequestRequestTypeDef",
     "PutRolePolicyRequestRequestTypeDef",
     "PutRolePolicyRequestRolePolicyPutTypeDef",
     "PutUserPermissionsBoundaryRequestRequestTypeDef",
@@ -267,18 +268,18 @@
     "RemoveUserFromGroupRequestGroupRemoveUserTypeDef",
     "RemoveUserFromGroupRequestRequestTypeDef",
     "RemoveUserFromGroupRequestUserRemoveGroupTypeDef",
     "ResetServiceSpecificCredentialRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ResyncMFADeviceRequestMfaDeviceResyncTypeDef",
     "ResyncMFADeviceRequestRequestTypeDef",
-    "RoleLastUsedTypeDef",
+    "RoleLastUsedOutputTypeDef",
     "RoleLastUsedResponseMetadataTypeDef",
     "ServerCertificateMetadataResponseMetadataTypeDef",
-    "TrackedActionLastAccessedTypeDef",
+    "TrackedActionLastAccessedOutputTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetSecurityTokenServicePreferencesRequestRequestTypeDef",
     "UntagInstanceProfileRequestRequestTypeDef",
     "UntagMFADeviceRequestRequestTypeDef",
     "UntagOpenIDConnectProviderRequestRequestTypeDef",
     "UntagPolicyRequestRequestTypeDef",
     "UntagRoleRequestRequestTypeDef",
@@ -300,179 +301,179 @@
     "UpdateLoginProfileRequestLoginProfileUpdateTypeDef",
     "UpdateLoginProfileRequestRequestTypeDef",
     "UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef",
     "UpdateRoleDescriptionRequestRequestTypeDef",
     "UpdateRoleRequestRequestTypeDef",
     "UpdateSAMLProviderRequestRequestTypeDef",
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
-    "UpdateSAMLProviderResponseTypeDef",
+    "UpdateSAMLProviderResponseOutputTypeDef",
     "UpdateSSHPublicKeyRequestRequestTypeDef",
     "UpdateServerCertificateRequestRequestTypeDef",
     "UpdateServerCertificateRequestServerCertificateUpdateTypeDef",
     "UpdateServiceSpecificCredentialRequestRequestTypeDef",
     "UpdateSigningCertificateRequestRequestTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateActivateTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserRequestUserUpdateTypeDef",
     "UploadSSHPublicKeyRequestRequestTypeDef",
     "UploadSigningCertificateRequestRequestTypeDef",
     "UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
-    "GetAccessKeyLastUsedResponseTypeDef",
-    "ListAccessKeysResponseTypeDef",
-    "CreateAccessKeyResponseTypeDef",
-    "ListAttachedGroupPoliciesResponseTypeDef",
-    "ListAttachedRolePoliciesResponseTypeDef",
-    "ListAttachedUserPoliciesResponseTypeDef",
+    "GetAccessKeyLastUsedResponseOutputTypeDef",
+    "ListAccessKeysResponseOutputTypeDef",
+    "CreateAccessKeyResponseOutputTypeDef",
+    "ListAttachedGroupPoliciesResponseOutputTypeDef",
+    "ListAttachedRolePoliciesResponseOutputTypeDef",
+    "ListAttachedUserPoliciesResponseOutputTypeDef",
     "SimulateCustomPolicyRequestRequestTypeDef",
     "SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
     "SimulatePrincipalPolicyRequestRequestTypeDef",
     "SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
-    "CreateGroupResponseTypeDef",
-    "ListGroupsForUserResponseTypeDef",
-    "ListGroupsResponseTypeDef",
+    "CreateGroupResponseOutputTypeDef",
+    "ListGroupsForUserResponseOutputTypeDef",
+    "ListGroupsResponseOutputTypeDef",
     "CreateInstanceProfileRequestRequestTypeDef",
     "CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef",
     "CreateOpenIDConnectProviderRequestRequestTypeDef",
-    "CreateOpenIDConnectProviderResponseTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreatePolicyRequestServiceResourceCreatePolicyTypeDef",
     "CreateRoleRequestRequestTypeDef",
     "CreateRoleRequestServiceResourceCreateRoleTypeDef",
     "CreateSAMLProviderRequestRequestTypeDef",
     "CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef",
-    "CreateSAMLProviderResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "CreateUserRequestServiceResourceCreateUserTypeDef",
     "CreateUserRequestUserCreateTypeDef",
     "CreateVirtualMFADeviceRequestRequestTypeDef",
     "CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef",
-    "GetOpenIDConnectProviderResponseTypeDef",
-    "GetSAMLProviderResponseTypeDef",
-    "ListInstanceProfileTagsResponseTypeDef",
-    "ListMFADeviceTagsResponseTypeDef",
-    "ListOpenIDConnectProviderTagsResponseTypeDef",
-    "ListPolicyTagsResponseTypeDef",
-    "ListRoleTagsResponseTypeDef",
-    "ListSAMLProviderTagsResponseTypeDef",
-    "ListServerCertificateTagsResponseTypeDef",
-    "ListUserTagsResponseTypeDef",
-    "PolicyTypeDef",
     "TagInstanceProfileRequestRequestTypeDef",
     "TagMFADeviceRequestRequestTypeDef",
     "TagOpenIDConnectProviderRequestRequestTypeDef",
     "TagPolicyRequestRequestTypeDef",
     "TagRoleRequestRequestTypeDef",
     "TagSAMLProviderRequestRequestTypeDef",
     "TagServerCertificateRequestRequestTypeDef",
     "TagUserRequestRequestTypeDef",
     "UploadServerCertificateRequestRequestTypeDef",
     "UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
+    "CreateLoginProfileResponseOutputTypeDef",
+    "GetLoginProfileResponseOutputTypeDef",
+    "CreateOpenIDConnectProviderResponseOutputTypeDef",
+    "CreateSAMLProviderResponseOutputTypeDef",
+    "GetOpenIDConnectProviderResponseOutputTypeDef",
+    "GetSAMLProviderResponseOutputTypeDef",
+    "ListInstanceProfileTagsResponseOutputTypeDef",
+    "ListMFADeviceTagsResponseOutputTypeDef",
+    "ListOpenIDConnectProviderTagsResponseOutputTypeDef",
+    "ListPolicyTagsResponseOutputTypeDef",
+    "ListRoleTagsResponseOutputTypeDef",
+    "ListSAMLProviderTagsResponseOutputTypeDef",
+    "ListServerCertificateTagsResponseOutputTypeDef",
+    "ListUserTagsResponseOutputTypeDef",
+    "PolicyOutputTypeDef",
+    "UserOutputTypeDef",
     "UserResponseMetadataTypeDef",
-    "UserTypeDef",
-    "CreateLoginProfileResponseTypeDef",
-    "GetLoginProfileResponseTypeDef",
-    "CreatePolicyVersionResponseTypeDef",
-    "GetPolicyVersionResponseTypeDef",
-    "ListPolicyVersionsResponseTypeDef",
-    "ManagedPolicyDetailTypeDef",
-    "CreateServiceSpecificCredentialResponseTypeDef",
-    "ResetServiceSpecificCredentialResponseTypeDef",
-    "DeletionTaskFailureReasonTypeTypeDef",
-    "EntityDetailsTypeDef",
-    "GetOrganizationsAccessReportResponseTypeDef",
-    "GetAccountPasswordPolicyResponseTypeDef",
+    "CreatePolicyVersionResponseOutputTypeDef",
+    "GetPolicyVersionResponseOutputTypeDef",
+    "ListPolicyVersionsResponseOutputTypeDef",
+    "ManagedPolicyDetailOutputTypeDef",
+    "CreateServiceSpecificCredentialResponseOutputTypeDef",
+    "ResetServiceSpecificCredentialResponseOutputTypeDef",
+    "DeletionTaskFailureReasonTypeOutputTypeDef",
+    "EntityDetailsOutputTypeDef",
+    "GetOrganizationsAccessReportResponseOutputTypeDef",
+    "GetAccountPasswordPolicyResponseOutputTypeDef",
     "GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     "GetPolicyRequestPolicyExistsWaitTypeDef",
     "GetRoleRequestRoleExistsWaitTypeDef",
     "GetUserRequestUserExistsWaitTypeDef",
-    "GetSSHPublicKeyResponseTypeDef",
-    "UploadSSHPublicKeyResponseTypeDef",
-    "GroupDetailTypeDef",
-    "UserDetailTypeDef",
-    "ListEntitiesForPolicyResponseTypeDef",
-    "ListMFADevicesResponseTypeDef",
-    "ListOpenIDConnectProvidersResponseTypeDef",
-    "ListPoliciesGrantingServiceAccessEntryTypeDef",
-    "ListSAMLProvidersResponseTypeDef",
-    "ListSSHPublicKeysResponseTypeDef",
-    "ListServerCertificatesResponseTypeDef",
-    "ServerCertificateTypeDef",
-    "UploadServerCertificateResponseTypeDef",
-    "ListServiceSpecificCredentialsResponseTypeDef",
-    "ListSigningCertificatesResponseTypeDef",
-    "UploadSigningCertificateResponseTypeDef",
-    "StatementTypeDef",
-    "RoleTypeDef",
-    "ServiceLastAccessedTypeDef",
-    "CreatePolicyResponseTypeDef",
-    "GetPolicyResponseTypeDef",
-    "ListPoliciesResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "GetGroupResponseTypeDef",
-    "GetUserResponseTypeDef",
-    "ListUsersResponseTypeDef",
-    "VirtualMFADeviceTypeDef",
-    "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
-    "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
-    "ListPoliciesGrantingServiceAccessResponseTypeDef",
-    "GetServerCertificateResponseTypeDef",
-    "ResourceSpecificResultTypeDef",
-    "CreateRoleResponseTypeDef",
-    "CreateServiceLinkedRoleResponseTypeDef",
-    "GetRoleResponseTypeDef",
-    "InstanceProfileTypeDef",
-    "ListRolesResponseTypeDef",
-    "UpdateRoleDescriptionResponseTypeDef",
-    "GetServiceLastAccessedDetailsResponseTypeDef",
-    "CreateVirtualMFADeviceResponseTypeDef",
-    "ListVirtualMFADevicesResponseTypeDef",
-    "EvaluationResultTypeDef",
-    "CreateInstanceProfileResponseTypeDef",
-    "GetInstanceProfileResponseTypeDef",
-    "ListInstanceProfilesForRoleResponseTypeDef",
-    "ListInstanceProfilesResponseTypeDef",
-    "RoleDetailTypeDef",
-    "SimulatePolicyResponseTypeDef",
-    "GetAccountAuthorizationDetailsResponseTypeDef",
+    "GetSSHPublicKeyResponseOutputTypeDef",
+    "UploadSSHPublicKeyResponseOutputTypeDef",
+    "GroupDetailOutputTypeDef",
+    "UserDetailOutputTypeDef",
+    "ListEntitiesForPolicyResponseOutputTypeDef",
+    "ListMFADevicesResponseOutputTypeDef",
+    "ListOpenIDConnectProvidersResponseOutputTypeDef",
+    "ListPoliciesGrantingServiceAccessEntryOutputTypeDef",
+    "ListSAMLProvidersResponseOutputTypeDef",
+    "ListSSHPublicKeysResponseOutputTypeDef",
+    "ListServerCertificatesResponseOutputTypeDef",
+    "ServerCertificateOutputTypeDef",
+    "UploadServerCertificateResponseOutputTypeDef",
+    "ListServiceSpecificCredentialsResponseOutputTypeDef",
+    "ListSigningCertificatesResponseOutputTypeDef",
+    "UploadSigningCertificateResponseOutputTypeDef",
+    "StatementOutputTypeDef",
+    "RoleOutputTypeDef",
+    "ServiceLastAccessedOutputTypeDef",
+    "CreatePolicyResponseOutputTypeDef",
+    "GetPolicyResponseOutputTypeDef",
+    "ListPoliciesResponseOutputTypeDef",
+    "CreateUserResponseOutputTypeDef",
+    "GetGroupResponseOutputTypeDef",
+    "GetUserResponseOutputTypeDef",
+    "ListUsersResponseOutputTypeDef",
+    "VirtualMFADeviceOutputTypeDef",
+    "GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef",
+    "GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef",
+    "ListPoliciesGrantingServiceAccessResponseOutputTypeDef",
+    "GetServerCertificateResponseOutputTypeDef",
+    "ResourceSpecificResultOutputTypeDef",
+    "CreateRoleResponseOutputTypeDef",
+    "CreateServiceLinkedRoleResponseOutputTypeDef",
+    "GetRoleResponseOutputTypeDef",
+    "InstanceProfileOutputTypeDef",
+    "ListRolesResponseOutputTypeDef",
+    "UpdateRoleDescriptionResponseOutputTypeDef",
+    "GetServiceLastAccessedDetailsResponseOutputTypeDef",
+    "CreateVirtualMFADeviceResponseOutputTypeDef",
+    "ListVirtualMFADevicesResponseOutputTypeDef",
+    "EvaluationResultOutputTypeDef",
+    "CreateInstanceProfileResponseOutputTypeDef",
+    "GetInstanceProfileResponseOutputTypeDef",
+    "ListInstanceProfilesForRoleResponseOutputTypeDef",
+    "ListInstanceProfilesResponseOutputTypeDef",
+    "RoleDetailOutputTypeDef",
+    "SimulatePolicyResponseOutputTypeDef",
+    "GetAccountAuthorizationDetailsResponseOutputTypeDef",
 )
 
-AccessDetailTypeDef = TypedDict(
-    "AccessDetailTypeDef",
+AccessDetailOutputTypeDef = TypedDict(
+    "AccessDetailOutputTypeDef",
     {
         "ServiceName": str,
         "ServiceNamespace": str,
         "Region": str,
         "EntityPath": str,
         "LastAuthenticatedTime": datetime,
         "TotalAuthenticatedEntities": int,
     },
 )
 
-AccessKeyLastUsedTypeDef = TypedDict(
-    "AccessKeyLastUsedTypeDef",
+AccessKeyLastUsedOutputTypeDef = TypedDict(
+    "AccessKeyLastUsedOutputTypeDef",
     {
         "LastUsedDate": datetime,
         "ServiceName": str,
         "Region": str,
     },
 )
 
-AccessKeyMetadataTypeDef = TypedDict(
-    "AccessKeyMetadataTypeDef",
+AccessKeyMetadataOutputTypeDef = TypedDict(
+    "AccessKeyMetadataOutputTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "CreateDate": datetime,
     },
 )
 
-AccessKeyTypeDef = TypedDict(
-    "AccessKeyTypeDef",
+AccessKeyOutputTypeDef = TypedDict(
+    "AccessKeyOutputTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "SecretAccessKey": str,
         "CreateDate": datetime,
     },
@@ -585,33 +586,33 @@
 AttachUserPolicyRequestUserAttachPolicyTypeDef = TypedDict(
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
     {
         "PolicyArn": str,
     },
 )
 
-AttachedPermissionsBoundaryResponseMetadataTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
+AttachedPermissionsBoundaryOutputTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryOutputTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachedPermissionsBoundaryTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryTypeDef",
+AttachedPermissionsBoundaryResponseMetadataTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachedPolicyTypeDef = TypedDict(
-    "AttachedPolicyTypeDef",
+AttachedPolicyOutputTypeDef = TypedDict(
+    "AttachedPolicyOutputTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
@@ -705,16 +706,16 @@
 
 class CreateGroupRequestServiceResourceCreateGroupTypeDef(
     _RequiredCreateGroupRequestServiceResourceCreateGroupTypeDef,
     _OptionalCreateGroupRequestServiceResourceCreateGroupTypeDef,
 ):
     pass
 
-GroupTypeDef = TypedDict(
-    "GroupTypeDef",
+GroupOutputTypeDef = TypedDict(
+    "GroupOutputTypeDef",
     {
         "Path": str,
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
         "CreateDate": datetime,
     },
@@ -785,23 +786,31 @@
 
 class CreateLoginProfileRequestUserCreateLoginProfileTypeDef(
     _RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
     _OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
 ):
     pass
 
-LoginProfileTypeDef = TypedDict(
-    "LoginProfileTypeDef",
+LoginProfileOutputTypeDef = TypedDict(
+    "LoginProfileOutputTypeDef",
     {
         "UserName": str,
         "CreateDate": datetime,
         "PasswordResetRequired": bool,
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
 _RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     {
         "PolicyDocument": str,
     },
 )
 _OptionalCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
@@ -835,16 +844,16 @@
 
 class CreatePolicyVersionRequestRequestTypeDef(
     _RequiredCreatePolicyVersionRequestRequestTypeDef,
     _OptionalCreatePolicyVersionRequestRequestTypeDef,
 ):
     pass
 
-PolicyVersionTypeDef = TypedDict(
-    "PolicyVersionTypeDef",
+PolicyVersionOutputTypeDef = TypedDict(
+    "PolicyVersionOutputTypeDef",
     {
         "Document": str,
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": datetime,
     },
 )
@@ -874,16 +883,16 @@
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
         "ServiceName": str,
     },
 )
 
-ServiceSpecificCredentialTypeDef = TypedDict(
-    "ServiceSpecificCredentialTypeDef",
+ServiceSpecificCredentialOutputTypeDef = TypedDict(
+    "ServiceSpecificCredentialOutputTypeDef",
     {
         "CreateDate": datetime,
         "ServiceName": str,
         "ServiceUserName": str,
         "ServicePassword": str,
         "ServiceSpecificCredentialId": str,
         "UserName": str,
@@ -1023,16 +1032,16 @@
 DeleteServiceLinkedRoleRequestRequestTypeDef = TypedDict(
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 
-DeleteServiceLinkedRoleResponseTypeDef = TypedDict(
-    "DeleteServiceLinkedRoleResponseTypeDef",
+DeleteServiceLinkedRoleResponseOutputTypeDef = TypedDict(
+    "DeleteServiceLinkedRoleResponseOutputTypeDef",
     {
         "DeletionTaskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteServiceSpecificCredentialRequestRequestTypeDef = TypedDict(
@@ -1100,16 +1109,16 @@
 DeleteVirtualMFADeviceRequestRequestTypeDef = TypedDict(
     "DeleteVirtualMFADeviceRequestRequestTypeDef",
     {
         "SerialNumber": str,
     },
 )
 
-RoleUsageTypeTypeDef = TypedDict(
-    "RoleUsageTypeTypeDef",
+RoleUsageTypeOutputTypeDef = TypedDict(
+    "RoleUsageTypeOutputTypeDef",
     {
         "Region": str,
         "Resources": List[str],
     },
 )
 
 DetachGroupPolicyRequestGroupDetachPolicyTypeDef = TypedDict(
@@ -1208,49 +1217,49 @@
     {
         "SerialNumber": str,
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
 
-EntityInfoTypeDef = TypedDict(
-    "EntityInfoTypeDef",
+EntityInfoOutputTypeDef = TypedDict(
+    "EntityInfoOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": policyOwnerEntityTypeType,
         "Id": str,
         "Path": str,
     },
 )
 
-ErrorDetailsTypeDef = TypedDict(
-    "ErrorDetailsTypeDef",
+ErrorDetailsOutputTypeDef = TypedDict(
+    "ErrorDetailsOutputTypeDef",
     {
         "Message": str,
         "Code": str,
     },
 )
 
-OrganizationsDecisionDetailTypeDef = TypedDict(
-    "OrganizationsDecisionDetailTypeDef",
+OrganizationsDecisionDetailOutputTypeDef = TypedDict(
+    "OrganizationsDecisionDetailOutputTypeDef",
     {
         "AllowedByOrganizations": bool,
     },
 )
 
-PermissionsBoundaryDecisionDetailTypeDef = TypedDict(
-    "PermissionsBoundaryDecisionDetailTypeDef",
+PermissionsBoundaryDecisionDetailOutputTypeDef = TypedDict(
+    "PermissionsBoundaryDecisionDetailOutputTypeDef",
     {
         "AllowedByPermissionsBoundary": bool,
     },
 )
 
-GenerateCredentialReportResponseTypeDef = TypedDict(
-    "GenerateCredentialReportResponseTypeDef",
+GenerateCredentialReportResponseOutputTypeDef = TypedDict(
+    "GenerateCredentialReportResponseOutputTypeDef",
     {
         "State": ReportStateTypeType,
         "Description": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1270,16 +1279,16 @@
 
 class GenerateOrganizationsAccessReportRequestRequestTypeDef(
     _RequiredGenerateOrganizationsAccessReportRequestRequestTypeDef,
     _OptionalGenerateOrganizationsAccessReportRequestRequestTypeDef,
 ):
     pass
 
-GenerateOrganizationsAccessReportResponseTypeDef = TypedDict(
-    "GenerateOrganizationsAccessReportResponseTypeDef",
+GenerateOrganizationsAccessReportResponseOutputTypeDef = TypedDict(
+    "GenerateOrganizationsAccessReportResponseOutputTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef = TypedDict(
@@ -1298,16 +1307,16 @@
 
 class GenerateServiceLastAccessedDetailsRequestRequestTypeDef(
     _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
     _OptionalGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
 ):
     pass
 
-GenerateServiceLastAccessedDetailsResponseTypeDef = TypedDict(
-    "GenerateServiceLastAccessedDetailsResponseTypeDef",
+GenerateServiceLastAccessedDetailsResponseOutputTypeDef = TypedDict(
+    "GenerateServiceLastAccessedDetailsResponseOutputTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccessKeyLastUsedRequestRequestTypeDef = TypedDict(
@@ -1332,47 +1341,47 @@
         "Filter": Sequence[EntityTypeType],
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
-PasswordPolicyTypeDef = TypedDict(
-    "PasswordPolicyTypeDef",
+PasswordPolicyOutputTypeDef = TypedDict(
+    "PasswordPolicyOutputTypeDef",
     {
         "MinimumPasswordLength": int,
         "RequireSymbols": bool,
         "RequireNumbers": bool,
         "RequireUppercaseCharacters": bool,
         "RequireLowercaseCharacters": bool,
         "AllowUsersToChangePassword": bool,
         "ExpirePasswords": bool,
         "MaxPasswordAge": int,
         "PasswordReusePrevention": int,
         "HardExpiry": bool,
     },
 )
 
-GetAccountSummaryResponseTypeDef = TypedDict(
-    "GetAccountSummaryResponseTypeDef",
+GetAccountSummaryResponseOutputTypeDef = TypedDict(
+    "GetAccountSummaryResponseOutputTypeDef",
     {
         "SummaryMap": Dict[summaryKeyTypeType, int],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContextKeysForCustomPolicyRequestRequestTypeDef = TypedDict(
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
     {
         "PolicyInputList": Sequence[str],
     },
 )
 
-GetContextKeysForPolicyResponseTypeDef = TypedDict(
-    "GetContextKeysForPolicyResponseTypeDef",
+GetContextKeysForPolicyResponseOutputTypeDef = TypedDict(
+    "GetContextKeysForPolicyResponseOutputTypeDef",
     {
         "ContextKeyNames": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef = TypedDict(
@@ -1391,16 +1400,16 @@
 
 class GetContextKeysForPrincipalPolicyRequestRequestTypeDef(
     _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
     _OptionalGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
 ):
     pass
 
-GetCredentialReportResponseTypeDef = TypedDict(
-    "GetCredentialReportResponseTypeDef",
+GetCredentialReportResponseOutputTypeDef = TypedDict(
+    "GetCredentialReportResponseOutputTypeDef",
     {
         "Content": bytes,
         "ReportFormat": Literal["text/csv"],
         "GeneratedTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1409,16 +1418,16 @@
     "GetGroupPolicyRequestRequestTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
     },
 )
 
-GetGroupPolicyResponseTypeDef = TypedDict(
-    "GetGroupPolicyResponseTypeDef",
+GetGroupPolicyResponseOutputTypeDef = TypedDict(
+    "GetGroupPolicyResponseOutputTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1500,16 +1509,16 @@
 )
 
 class GetMFADeviceRequestRequestTypeDef(
     _RequiredGetMFADeviceRequestRequestTypeDef, _OptionalGetMFADeviceRequestRequestTypeDef
 ):
     pass
 
-GetMFADeviceResponseTypeDef = TypedDict(
-    "GetMFADeviceResponseTypeDef",
+GetMFADeviceResponseOutputTypeDef = TypedDict(
+    "GetMFADeviceResponseOutputTypeDef",
     {
         "UserName": str,
         "SerialNumber": str,
         "EnableDate": datetime,
         "Certifications": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1563,16 +1572,16 @@
     "GetRolePolicyRequestRequestTypeDef",
     {
         "RoleName": str,
         "PolicyName": str,
     },
 )
 
-GetRolePolicyResponseTypeDef = TypedDict(
-    "GetRolePolicyResponseTypeDef",
+GetRolePolicyResponseOutputTypeDef = TypedDict(
+    "GetRolePolicyResponseOutputTypeDef",
     {
         "RoleName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1596,16 +1605,16 @@
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Encoding": encodingTypeType,
     },
 )
 
-SSHPublicKeyTypeDef = TypedDict(
-    "SSHPublicKeyTypeDef",
+SSHPublicKeyOutputTypeDef = TypedDict(
+    "SSHPublicKeyOutputTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Fingerprint": str,
         "SSHPublicKeyBody": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
@@ -1673,16 +1682,16 @@
     "GetUserPolicyRequestRequestTypeDef",
     {
         "UserName": str,
         "PolicyName": str,
     },
 )
 
-GetUserPolicyResponseTypeDef = TypedDict(
-    "GetUserPolicyResponseTypeDef",
+GetUserPolicyResponseOutputTypeDef = TypedDict(
+    "GetUserPolicyResponseOutputTypeDef",
     {
         "UserName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1691,16 +1700,16 @@
     "GetUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-PolicyDetailTypeDef = TypedDict(
-    "PolicyDetailTypeDef",
+PolicyDetailOutputTypeDef = TypedDict(
+    "PolicyDetailOutputTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
 
 ListAccessKeysRequestListAccessKeysPaginateTypeDef = TypedDict(
@@ -1735,16 +1744,16 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListAccountAliasesResponseTypeDef = TypedDict(
-    "ListAccountAliasesResponseTypeDef",
+ListAccountAliasesResponseOutputTypeDef = TypedDict(
+    "ListAccountAliasesResponseOutputTypeDef",
     {
         "AccountAliases": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1921,32 +1930,32 @@
 
 class ListEntitiesForPolicyRequestRequestTypeDef(
     _RequiredListEntitiesForPolicyRequestRequestTypeDef,
     _OptionalListEntitiesForPolicyRequestRequestTypeDef,
 ):
     pass
 
-PolicyGroupTypeDef = TypedDict(
-    "PolicyGroupTypeDef",
+PolicyGroupOutputTypeDef = TypedDict(
+    "PolicyGroupOutputTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
 )
 
-PolicyRoleTypeDef = TypedDict(
-    "PolicyRoleTypeDef",
+PolicyRoleOutputTypeDef = TypedDict(
+    "PolicyRoleOutputTypeDef",
     {
         "RoleName": str,
         "RoleId": str,
     },
 )
 
-PolicyUserTypeDef = TypedDict(
-    "PolicyUserTypeDef",
+PolicyUserOutputTypeDef = TypedDict(
+    "PolicyUserOutputTypeDef",
     {
         "UserName": str,
         "UserId": str,
     },
 )
 
 _RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
@@ -1985,16 +1994,16 @@
 )
 
 class ListGroupPoliciesRequestRequestTypeDef(
     _RequiredListGroupPoliciesRequestRequestTypeDef, _OptionalListGroupPoliciesRequestRequestTypeDef
 ):
     pass
 
-ListGroupPoliciesResponseTypeDef = TypedDict(
-    "ListGroupPoliciesResponseTypeDef",
+ListGroupPoliciesResponseOutputTypeDef = TypedDict(
+    "ListGroupPoliciesResponseOutputTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2214,16 +2223,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-MFADeviceTypeDef = TypedDict(
-    "MFADeviceTypeDef",
+MFADeviceOutputTypeDef = TypedDict(
+    "MFADeviceOutputTypeDef",
     {
         "UserName": str,
         "SerialNumber": str,
         "EnableDate": datetime,
     },
 )
 
@@ -2268,23 +2277,23 @@
 
 class ListOpenIDConnectProviderTagsRequestRequestTypeDef(
     _RequiredListOpenIDConnectProviderTagsRequestRequestTypeDef,
     _OptionalListOpenIDConnectProviderTagsRequestRequestTypeDef,
 ):
     pass
 
-OpenIDConnectProviderListEntryTypeDef = TypedDict(
-    "OpenIDConnectProviderListEntryTypeDef",
+OpenIDConnectProviderListEntryOutputTypeDef = TypedDict(
+    "OpenIDConnectProviderListEntryOutputTypeDef",
     {
         "Arn": str,
     },
 )
 
-PolicyGrantingServiceAccessTypeDef = TypedDict(
-    "PolicyGrantingServiceAccessTypeDef",
+PolicyGrantingServiceAccessOutputTypeDef = TypedDict(
+    "PolicyGrantingServiceAccessOutputTypeDef",
     {
         "PolicyName": str,
         "PolicyType": policyTypeType,
         "PolicyArn": str,
         "EntityType": policyOwnerEntityTypeType,
         "EntityName": str,
     },
@@ -2453,16 +2462,16 @@
 )
 
 class ListRolePoliciesRequestRequestTypeDef(
     _RequiredListRolePoliciesRequestRequestTypeDef, _OptionalListRolePoliciesRequestRequestTypeDef
 ):
     pass
 
-ListRolePoliciesResponseTypeDef = TypedDict(
-    "ListRolePoliciesResponseTypeDef",
+ListRolePoliciesResponseOutputTypeDef = TypedDict(
+    "ListRolePoliciesResponseOutputTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2563,16 +2572,16 @@
 
 class ListSAMLProviderTagsRequestRequestTypeDef(
     _RequiredListSAMLProviderTagsRequestRequestTypeDef,
     _OptionalListSAMLProviderTagsRequestRequestTypeDef,
 ):
     pass
 
-SAMLProviderListEntryTypeDef = TypedDict(
-    "SAMLProviderListEntryTypeDef",
+SAMLProviderListEntryOutputTypeDef = TypedDict(
+    "SAMLProviderListEntryOutputTypeDef",
     {
         "Arn": str,
         "ValidUntil": datetime,
         "CreateDate": datetime,
     },
 )
 
@@ -2591,16 +2600,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-SSHPublicKeyMetadataTypeDef = TypedDict(
-    "SSHPublicKeyMetadataTypeDef",
+SSHPublicKeyMetadataOutputTypeDef = TypedDict(
+    "SSHPublicKeyMetadataOutputTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
     },
 )
@@ -2661,16 +2670,16 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ServerCertificateMetadataTypeDef = TypedDict(
-    "ServerCertificateMetadataTypeDef",
+ServerCertificateMetadataOutputTypeDef = TypedDict(
+    "ServerCertificateMetadataOutputTypeDef",
     {
         "Path": str,
         "ServerCertificateName": str,
         "ServerCertificateId": str,
         "Arn": str,
         "UploadDate": datetime,
         "Expiration": datetime,
@@ -2682,16 +2691,16 @@
     {
         "UserName": str,
         "ServiceName": str,
     },
     total=False,
 )
 
-ServiceSpecificCredentialMetadataTypeDef = TypedDict(
-    "ServiceSpecificCredentialMetadataTypeDef",
+ServiceSpecificCredentialMetadataOutputTypeDef = TypedDict(
+    "ServiceSpecificCredentialMetadataOutputTypeDef",
     {
         "UserName": str,
         "Status": statusTypeType,
         "ServiceUserName": str,
         "CreateDate": datetime,
         "ServiceSpecificCredentialId": str,
         "ServiceName": str,
@@ -2713,16 +2722,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-SigningCertificateTypeDef = TypedDict(
-    "SigningCertificateTypeDef",
+SigningCertificateOutputTypeDef = TypedDict(
+    "SigningCertificateOutputTypeDef",
     {
         "UserName": str,
         "CertificateId": str,
         "CertificateBody": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
     },
@@ -2764,16 +2773,16 @@
 )
 
 class ListUserPoliciesRequestRequestTypeDef(
     _RequiredListUserPoliciesRequestRequestTypeDef, _OptionalListUserPoliciesRequestRequestTypeDef
 ):
     pass
 
-ListUserPoliciesResponseTypeDef = TypedDict(
-    "ListUserPoliciesResponseTypeDef",
+ListUserPoliciesResponseOutputTypeDef = TypedDict(
+    "ListUserPoliciesResponseOutputTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2862,16 +2871,16 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-PositionTypeDef = TypedDict(
-    "PositionTypeDef",
+PositionOutputTypeDef = TypedDict(
+    "PositionOutputTypeDef",
     {
         "Line": int,
         "Column": int,
     },
 )
 
 PutGroupPolicyRequestGroupCreatePolicyTypeDef = TypedDict(
@@ -3044,16 +3053,16 @@
         "UserName": str,
         "SerialNumber": str,
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
 
-RoleLastUsedTypeDef = TypedDict(
-    "RoleLastUsedTypeDef",
+RoleLastUsedOutputTypeDef = TypedDict(
+    "RoleLastUsedOutputTypeDef",
     {
         "LastUsedDate": datetime,
         "Region": str,
     },
 )
 
 RoleLastUsedResponseMetadataTypeDef = TypedDict(
@@ -3074,16 +3083,16 @@
         "Arn": str,
         "UploadDate": datetime,
         "Expiration": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TrackedActionLastAccessedTypeDef = TypedDict(
-    "TrackedActionLastAccessedTypeDef",
+TrackedActionLastAccessedOutputTypeDef = TypedDict(
+    "TrackedActionLastAccessedOutputTypeDef",
     {
         "ActionName": str,
         "LastAccessedEntity": str,
         "LastAccessedTime": datetime,
         "LastAccessedRegion": str,
     },
 )
@@ -3388,16 +3397,16 @@
 UpdateSAMLProviderRequestSamlProviderUpdateTypeDef = TypedDict(
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
     {
         "SAMLMetadataDocument": str,
     },
 )
 
-UpdateSAMLProviderResponseTypeDef = TypedDict(
-    "UpdateSAMLProviderResponseTypeDef",
+UpdateSAMLProviderResponseOutputTypeDef = TypedDict(
+    "UpdateSAMLProviderResponseOutputTypeDef",
     {
         "SAMLProviderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSSHPublicKeyRequestRequestTypeDef = TypedDict(
@@ -3570,65 +3579,65 @@
 
 class UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef(
     _RequiredUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
     _OptionalUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
 ):
     pass
 
-GetAccessKeyLastUsedResponseTypeDef = TypedDict(
-    "GetAccessKeyLastUsedResponseTypeDef",
+GetAccessKeyLastUsedResponseOutputTypeDef = TypedDict(
+    "GetAccessKeyLastUsedResponseOutputTypeDef",
     {
         "UserName": str,
-        "AccessKeyLastUsed": AccessKeyLastUsedTypeDef,
+        "AccessKeyLastUsed": AccessKeyLastUsedOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAccessKeysResponseTypeDef = TypedDict(
-    "ListAccessKeysResponseTypeDef",
+ListAccessKeysResponseOutputTypeDef = TypedDict(
+    "ListAccessKeysResponseOutputTypeDef",
     {
-        "AccessKeyMetadata": List[AccessKeyMetadataTypeDef],
+        "AccessKeyMetadata": List[AccessKeyMetadataOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateAccessKeyResponseTypeDef = TypedDict(
-    "CreateAccessKeyResponseTypeDef",
+CreateAccessKeyResponseOutputTypeDef = TypedDict(
+    "CreateAccessKeyResponseOutputTypeDef",
     {
-        "AccessKey": AccessKeyTypeDef,
+        "AccessKey": AccessKeyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedGroupPoliciesResponseTypeDef = TypedDict(
-    "ListAttachedGroupPoliciesResponseTypeDef",
+ListAttachedGroupPoliciesResponseOutputTypeDef = TypedDict(
+    "ListAttachedGroupPoliciesResponseOutputTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyTypeDef],
+        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedRolePoliciesResponseTypeDef = TypedDict(
-    "ListAttachedRolePoliciesResponseTypeDef",
+ListAttachedRolePoliciesResponseOutputTypeDef = TypedDict(
+    "ListAttachedRolePoliciesResponseOutputTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyTypeDef],
+        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedUserPoliciesResponseTypeDef = TypedDict(
-    "ListAttachedUserPoliciesResponseTypeDef",
+ListAttachedUserPoliciesResponseOutputTypeDef = TypedDict(
+    "ListAttachedUserPoliciesResponseOutputTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyTypeDef],
+        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSimulateCustomPolicyRequestRequestTypeDef = TypedDict(
@@ -3743,36 +3752,36 @@
 
 class SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef(
     _RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
     _OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
 ):
     pass
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
+CreateGroupResponseOutputTypeDef = TypedDict(
+    "CreateGroupResponseOutputTypeDef",
     {
-        "Group": GroupTypeDef,
+        "Group": GroupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGroupsForUserResponseTypeDef = TypedDict(
-    "ListGroupsForUserResponseTypeDef",
+ListGroupsForUserResponseOutputTypeDef = TypedDict(
+    "ListGroupsForUserResponseOutputTypeDef",
     {
-        "Groups": List[GroupTypeDef],
+        "Groups": List[GroupOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGroupsResponseTypeDef = TypedDict(
-    "ListGroupsResponseTypeDef",
+ListGroupsResponseOutputTypeDef = TypedDict(
+    "ListGroupsResponseOutputTypeDef",
     {
-        "Groups": List[GroupTypeDef],
+        "Groups": List[GroupOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateInstanceProfileRequestRequestTypeDef = TypedDict(
@@ -3835,23 +3844,14 @@
 
 class CreateOpenIDConnectProviderRequestRequestTypeDef(
     _RequiredCreateOpenIDConnectProviderRequestRequestTypeDef,
     _OptionalCreateOpenIDConnectProviderRequestRequestTypeDef,
 ):
     pass
 
-CreateOpenIDConnectProviderResponseTypeDef = TypedDict(
-    "CreateOpenIDConnectProviderResponseTypeDef",
-    {
-        "OpenIDConnectProviderArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
@@ -3980,23 +3980,14 @@
 
 class CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef(
     _RequiredCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef,
     _OptionalCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef,
 ):
     pass
 
-CreateSAMLProviderResponseTypeDef = TypedDict(
-    "CreateSAMLProviderResponseTypeDef",
-    {
-        "SAMLProviderArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
 _OptionalCreateUserRequestRequestTypeDef = TypedDict(
@@ -4084,135 +4075,14 @@
 
 class CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef(
     _RequiredCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef,
     _OptionalCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef,
 ):
     pass
 
-GetOpenIDConnectProviderResponseTypeDef = TypedDict(
-    "GetOpenIDConnectProviderResponseTypeDef",
-    {
-        "Url": str,
-        "ClientIDList": List[str],
-        "ThumbprintList": List[str],
-        "CreateDate": datetime,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSAMLProviderResponseTypeDef = TypedDict(
-    "GetSAMLProviderResponseTypeDef",
-    {
-        "SAMLMetadataDocument": str,
-        "CreateDate": datetime,
-        "ValidUntil": datetime,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListInstanceProfileTagsResponseTypeDef = TypedDict(
-    "ListInstanceProfileTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListMFADeviceTagsResponseTypeDef = TypedDict(
-    "ListMFADeviceTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListOpenIDConnectProviderTagsResponseTypeDef = TypedDict(
-    "ListOpenIDConnectProviderTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPolicyTagsResponseTypeDef = TypedDict(
-    "ListPolicyTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRoleTagsResponseTypeDef = TypedDict(
-    "ListRoleTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSAMLProviderTagsResponseTypeDef = TypedDict(
-    "ListSAMLProviderTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListServerCertificateTagsResponseTypeDef = TypedDict(
-    "ListServerCertificateTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListUserTagsResponseTypeDef = TypedDict(
-    "ListUserTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PolicyTypeDef = TypedDict(
-    "PolicyTypeDef",
-    {
-        "PolicyName": str,
-        "PolicyId": str,
-        "Arn": str,
-        "Path": str,
-        "DefaultVersionId": str,
-        "AttachmentCount": int,
-        "PermissionsBoundaryUsageCount": int,
-        "IsAttachable": bool,
-        "Description": str,
-        "CreateDate": datetime,
-        "UpdateDate": datetime,
-        "Tags": List[TagTypeDef],
-    },
-)
-
 TagInstanceProfileRequestRequestTypeDef = TypedDict(
     "TagInstanceProfileRequestRequestTypeDef",
     {
         "InstanceProfileName": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -4317,155 +4187,294 @@
 
 class UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef(
     _RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
     _OptionalUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
 ):
     pass
 
-UserResponseMetadataTypeDef = TypedDict(
-    "UserResponseMetadataTypeDef",
+CreateLoginProfileResponseOutputTypeDef = TypedDict(
+    "CreateLoginProfileResponseOutputTypeDef",
     {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
+        "LoginProfile": LoginProfileOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetLoginProfileResponseOutputTypeDef = TypedDict(
+    "GetLoginProfileResponseOutputTypeDef",
+    {
+        "LoginProfile": LoginProfileOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateOpenIDConnectProviderResponseOutputTypeDef = TypedDict(
+    "CreateOpenIDConnectProviderResponseOutputTypeDef",
+    {
+        "OpenIDConnectProviderArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSAMLProviderResponseOutputTypeDef = TypedDict(
+    "CreateSAMLProviderResponseOutputTypeDef",
+    {
+        "SAMLProviderArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetOpenIDConnectProviderResponseOutputTypeDef = TypedDict(
+    "GetOpenIDConnectProviderResponseOutputTypeDef",
+    {
+        "Url": str,
+        "ClientIDList": List[str],
+        "ThumbprintList": List[str],
         "CreateDate": datetime,
-        "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UserTypeDef = TypedDict(
-    "UserTypeDef",
+GetSAMLProviderResponseOutputTypeDef = TypedDict(
+    "GetSAMLProviderResponseOutputTypeDef",
     {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
+        "SAMLMetadataDocument": str,
         "CreateDate": datetime,
-        "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
+        "ValidUntil": datetime,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListInstanceProfileTagsResponseOutputTypeDef = TypedDict(
+    "ListInstanceProfileTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListMFADeviceTagsResponseOutputTypeDef = TypedDict(
+    "ListMFADeviceTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListOpenIDConnectProviderTagsResponseOutputTypeDef = TypedDict(
+    "ListOpenIDConnectProviderTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPolicyTagsResponseOutputTypeDef = TypedDict(
+    "ListPolicyTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListRoleTagsResponseOutputTypeDef = TypedDict(
+    "ListRoleTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSAMLProviderTagsResponseOutputTypeDef = TypedDict(
+    "ListSAMLProviderTagsResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLoginProfileResponseTypeDef = TypedDict(
-    "CreateLoginProfileResponseTypeDef",
+ListServerCertificateTagsResponseOutputTypeDef = TypedDict(
+    "ListServerCertificateTagsResponseOutputTypeDef",
     {
-        "LoginProfile": LoginProfileTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetLoginProfileResponseTypeDef = TypedDict(
-    "GetLoginProfileResponseTypeDef",
+ListUserTagsResponseOutputTypeDef = TypedDict(
+    "ListUserTagsResponseOutputTypeDef",
     {
-        "LoginProfile": LoginProfileTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PolicyOutputTypeDef = TypedDict(
+    "PolicyOutputTypeDef",
+    {
+        "PolicyName": str,
+        "PolicyId": str,
+        "Arn": str,
+        "Path": str,
+        "DefaultVersionId": str,
+        "AttachmentCount": int,
+        "PermissionsBoundaryUsageCount": int,
+        "IsAttachable": bool,
+        "Description": str,
+        "CreateDate": datetime,
+        "UpdateDate": datetime,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+UserOutputTypeDef = TypedDict(
+    "UserOutputTypeDef",
+    {
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "PasswordLastUsed": datetime,
+        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+UserResponseMetadataTypeDef = TypedDict(
+    "UserResponseMetadataTypeDef",
+    {
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "PasswordLastUsed": datetime,
+        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreatePolicyVersionResponseTypeDef = TypedDict(
-    "CreatePolicyVersionResponseTypeDef",
+CreatePolicyVersionResponseOutputTypeDef = TypedDict(
+    "CreatePolicyVersionResponseOutputTypeDef",
     {
-        "PolicyVersion": PolicyVersionTypeDef,
+        "PolicyVersion": PolicyVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPolicyVersionResponseTypeDef = TypedDict(
-    "GetPolicyVersionResponseTypeDef",
+GetPolicyVersionResponseOutputTypeDef = TypedDict(
+    "GetPolicyVersionResponseOutputTypeDef",
     {
-        "PolicyVersion": PolicyVersionTypeDef,
+        "PolicyVersion": PolicyVersionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPolicyVersionsResponseTypeDef = TypedDict(
-    "ListPolicyVersionsResponseTypeDef",
+ListPolicyVersionsResponseOutputTypeDef = TypedDict(
+    "ListPolicyVersionsResponseOutputTypeDef",
     {
-        "Versions": List[PolicyVersionTypeDef],
+        "Versions": List[PolicyVersionOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ManagedPolicyDetailTypeDef = TypedDict(
-    "ManagedPolicyDetailTypeDef",
+ManagedPolicyDetailOutputTypeDef = TypedDict(
+    "ManagedPolicyDetailOutputTypeDef",
     {
         "PolicyName": str,
         "PolicyId": str,
         "Arn": str,
         "Path": str,
         "DefaultVersionId": str,
         "AttachmentCount": int,
         "PermissionsBoundaryUsageCount": int,
         "IsAttachable": bool,
         "Description": str,
         "CreateDate": datetime,
         "UpdateDate": datetime,
-        "PolicyVersionList": List[PolicyVersionTypeDef],
+        "PolicyVersionList": List[PolicyVersionOutputTypeDef],
     },
 )
 
-CreateServiceSpecificCredentialResponseTypeDef = TypedDict(
-    "CreateServiceSpecificCredentialResponseTypeDef",
+CreateServiceSpecificCredentialResponseOutputTypeDef = TypedDict(
+    "CreateServiceSpecificCredentialResponseOutputTypeDef",
     {
-        "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
+        "ServiceSpecificCredential": ServiceSpecificCredentialOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResetServiceSpecificCredentialResponseTypeDef = TypedDict(
-    "ResetServiceSpecificCredentialResponseTypeDef",
+ResetServiceSpecificCredentialResponseOutputTypeDef = TypedDict(
+    "ResetServiceSpecificCredentialResponseOutputTypeDef",
     {
-        "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
+        "ServiceSpecificCredential": ServiceSpecificCredentialOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeletionTaskFailureReasonTypeTypeDef = TypedDict(
-    "DeletionTaskFailureReasonTypeTypeDef",
+DeletionTaskFailureReasonTypeOutputTypeDef = TypedDict(
+    "DeletionTaskFailureReasonTypeOutputTypeDef",
     {
         "Reason": str,
-        "RoleUsageList": List[RoleUsageTypeTypeDef],
+        "RoleUsageList": List[RoleUsageTypeOutputTypeDef],
     },
 )
 
-EntityDetailsTypeDef = TypedDict(
-    "EntityDetailsTypeDef",
+EntityDetailsOutputTypeDef = TypedDict(
+    "EntityDetailsOutputTypeDef",
     {
-        "EntityInfo": EntityInfoTypeDef,
+        "EntityInfo": EntityInfoOutputTypeDef,
         "LastAuthenticated": datetime,
     },
 )
 
-GetOrganizationsAccessReportResponseTypeDef = TypedDict(
-    "GetOrganizationsAccessReportResponseTypeDef",
+GetOrganizationsAccessReportResponseOutputTypeDef = TypedDict(
+    "GetOrganizationsAccessReportResponseOutputTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
         "NumberOfServicesAccessible": int,
         "NumberOfServicesNotAccessed": int,
-        "AccessDetails": List[AccessDetailTypeDef],
+        "AccessDetails": List[AccessDetailOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ErrorDetails": ErrorDetailsTypeDef,
+        "ErrorDetails": ErrorDetailsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccountPasswordPolicyResponseTypeDef = TypedDict(
-    "GetAccountPasswordPolicyResponseTypeDef",
+GetAccountPasswordPolicyResponseOutputTypeDef = TypedDict(
+    "GetAccountPasswordPolicyResponseOutputTypeDef",
     {
-        "PasswordPolicy": PasswordPolicyTypeDef,
+        "PasswordPolicy": PasswordPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef = TypedDict(
     "_RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     {
@@ -4530,510 +4539,510 @@
     {
         "UserName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-GetSSHPublicKeyResponseTypeDef = TypedDict(
-    "GetSSHPublicKeyResponseTypeDef",
+GetSSHPublicKeyResponseOutputTypeDef = TypedDict(
+    "GetSSHPublicKeyResponseOutputTypeDef",
     {
-        "SSHPublicKey": SSHPublicKeyTypeDef,
+        "SSHPublicKey": SSHPublicKeyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadSSHPublicKeyResponseTypeDef = TypedDict(
-    "UploadSSHPublicKeyResponseTypeDef",
+UploadSSHPublicKeyResponseOutputTypeDef = TypedDict(
+    "UploadSSHPublicKeyResponseOutputTypeDef",
     {
-        "SSHPublicKey": SSHPublicKeyTypeDef,
+        "SSHPublicKey": SSHPublicKeyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GroupDetailTypeDef = TypedDict(
-    "GroupDetailTypeDef",
+GroupDetailOutputTypeDef = TypedDict(
+    "GroupDetailOutputTypeDef",
     {
         "Path": str,
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "GroupPolicyList": List[PolicyDetailTypeDef],
-        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
+        "GroupPolicyList": List[PolicyDetailOutputTypeDef],
+        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
     },
 )
 
-UserDetailTypeDef = TypedDict(
-    "UserDetailTypeDef",
+UserDetailOutputTypeDef = TypedDict(
+    "UserDetailOutputTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "UserPolicyList": List[PolicyDetailTypeDef],
+        "UserPolicyList": List[PolicyDetailOutputTypeDef],
         "GroupList": List[str],
-        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
+        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
+        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
-ListEntitiesForPolicyResponseTypeDef = TypedDict(
-    "ListEntitiesForPolicyResponseTypeDef",
+ListEntitiesForPolicyResponseOutputTypeDef = TypedDict(
+    "ListEntitiesForPolicyResponseOutputTypeDef",
     {
-        "PolicyGroups": List[PolicyGroupTypeDef],
-        "PolicyUsers": List[PolicyUserTypeDef],
-        "PolicyRoles": List[PolicyRoleTypeDef],
+        "PolicyGroups": List[PolicyGroupOutputTypeDef],
+        "PolicyUsers": List[PolicyUserOutputTypeDef],
+        "PolicyRoles": List[PolicyRoleOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListMFADevicesResponseTypeDef = TypedDict(
-    "ListMFADevicesResponseTypeDef",
+ListMFADevicesResponseOutputTypeDef = TypedDict(
+    "ListMFADevicesResponseOutputTypeDef",
     {
-        "MFADevices": List[MFADeviceTypeDef],
+        "MFADevices": List[MFADeviceOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListOpenIDConnectProvidersResponseTypeDef = TypedDict(
-    "ListOpenIDConnectProvidersResponseTypeDef",
+ListOpenIDConnectProvidersResponseOutputTypeDef = TypedDict(
+    "ListOpenIDConnectProvidersResponseOutputTypeDef",
     {
-        "OpenIDConnectProviderList": List[OpenIDConnectProviderListEntryTypeDef],
+        "OpenIDConnectProviderList": List[OpenIDConnectProviderListEntryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesGrantingServiceAccessEntryTypeDef = TypedDict(
-    "ListPoliciesGrantingServiceAccessEntryTypeDef",
+ListPoliciesGrantingServiceAccessEntryOutputTypeDef = TypedDict(
+    "ListPoliciesGrantingServiceAccessEntryOutputTypeDef",
     {
         "ServiceNamespace": str,
-        "Policies": List[PolicyGrantingServiceAccessTypeDef],
+        "Policies": List[PolicyGrantingServiceAccessOutputTypeDef],
     },
 )
 
-ListSAMLProvidersResponseTypeDef = TypedDict(
-    "ListSAMLProvidersResponseTypeDef",
+ListSAMLProvidersResponseOutputTypeDef = TypedDict(
+    "ListSAMLProvidersResponseOutputTypeDef",
     {
-        "SAMLProviderList": List[SAMLProviderListEntryTypeDef],
+        "SAMLProviderList": List[SAMLProviderListEntryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSSHPublicKeysResponseTypeDef = TypedDict(
-    "ListSSHPublicKeysResponseTypeDef",
+ListSSHPublicKeysResponseOutputTypeDef = TypedDict(
+    "ListSSHPublicKeysResponseOutputTypeDef",
     {
-        "SSHPublicKeys": List[SSHPublicKeyMetadataTypeDef],
+        "SSHPublicKeys": List[SSHPublicKeyMetadataOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServerCertificatesResponseTypeDef = TypedDict(
-    "ListServerCertificatesResponseTypeDef",
+ListServerCertificatesResponseOutputTypeDef = TypedDict(
+    "ListServerCertificatesResponseOutputTypeDef",
     {
-        "ServerCertificateMetadataList": List[ServerCertificateMetadataTypeDef],
+        "ServerCertificateMetadataList": List[ServerCertificateMetadataOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ServerCertificateTypeDef = TypedDict(
-    "ServerCertificateTypeDef",
+ServerCertificateOutputTypeDef = TypedDict(
+    "ServerCertificateOutputTypeDef",
     {
-        "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
+        "ServerCertificateMetadata": ServerCertificateMetadataOutputTypeDef,
         "CertificateBody": str,
         "CertificateChain": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
-UploadServerCertificateResponseTypeDef = TypedDict(
-    "UploadServerCertificateResponseTypeDef",
+UploadServerCertificateResponseOutputTypeDef = TypedDict(
+    "UploadServerCertificateResponseOutputTypeDef",
     {
-        "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
-        "Tags": List[TagTypeDef],
+        "ServerCertificateMetadata": ServerCertificateMetadataOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceSpecificCredentialsResponseTypeDef = TypedDict(
-    "ListServiceSpecificCredentialsResponseTypeDef",
+ListServiceSpecificCredentialsResponseOutputTypeDef = TypedDict(
+    "ListServiceSpecificCredentialsResponseOutputTypeDef",
     {
-        "ServiceSpecificCredentials": List[ServiceSpecificCredentialMetadataTypeDef],
+        "ServiceSpecificCredentials": List[ServiceSpecificCredentialMetadataOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSigningCertificatesResponseTypeDef = TypedDict(
-    "ListSigningCertificatesResponseTypeDef",
+ListSigningCertificatesResponseOutputTypeDef = TypedDict(
+    "ListSigningCertificatesResponseOutputTypeDef",
     {
-        "Certificates": List[SigningCertificateTypeDef],
+        "Certificates": List[SigningCertificateOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadSigningCertificateResponseTypeDef = TypedDict(
-    "UploadSigningCertificateResponseTypeDef",
+UploadSigningCertificateResponseOutputTypeDef = TypedDict(
+    "UploadSigningCertificateResponseOutputTypeDef",
     {
-        "Certificate": SigningCertificateTypeDef,
+        "Certificate": SigningCertificateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StatementTypeDef = TypedDict(
-    "StatementTypeDef",
+StatementOutputTypeDef = TypedDict(
+    "StatementOutputTypeDef",
     {
         "SourcePolicyId": str,
         "SourcePolicyType": PolicySourceTypeType,
-        "StartPosition": PositionTypeDef,
-        "EndPosition": PositionTypeDef,
+        "StartPosition": PositionOutputTypeDef,
+        "EndPosition": PositionOutputTypeDef,
     },
 )
 
-RoleTypeDef = TypedDict(
-    "RoleTypeDef",
+RoleOutputTypeDef = TypedDict(
+    "RoleOutputTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
         "CreateDate": datetime,
         "AssumeRolePolicyDocument": str,
         "Description": str,
         "MaxSessionDuration": int,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-        "RoleLastUsed": RoleLastUsedTypeDef,
+        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "RoleLastUsed": RoleLastUsedOutputTypeDef,
     },
 )
 
-ServiceLastAccessedTypeDef = TypedDict(
-    "ServiceLastAccessedTypeDef",
+ServiceLastAccessedOutputTypeDef = TypedDict(
+    "ServiceLastAccessedOutputTypeDef",
     {
         "ServiceName": str,
         "LastAuthenticated": datetime,
         "ServiceNamespace": str,
         "LastAuthenticatedEntity": str,
         "LastAuthenticatedRegion": str,
         "TotalAuthenticatedEntities": int,
-        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
+        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedOutputTypeDef],
     },
 )
 
-CreatePolicyResponseTypeDef = TypedDict(
-    "CreatePolicyResponseTypeDef",
+CreatePolicyResponseOutputTypeDef = TypedDict(
+    "CreatePolicyResponseOutputTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
+GetPolicyResponseOutputTypeDef = TypedDict(
+    "GetPolicyResponseOutputTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesResponseTypeDef = TypedDict(
-    "ListPoliciesResponseTypeDef",
+ListPoliciesResponseOutputTypeDef = TypedDict(
+    "ListPoliciesResponseOutputTypeDef",
     {
-        "Policies": List[PolicyTypeDef],
+        "Policies": List[PolicyOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
+CreateUserResponseOutputTypeDef = TypedDict(
+    "CreateUserResponseOutputTypeDef",
     {
-        "User": UserTypeDef,
+        "User": UserOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
+GetGroupResponseOutputTypeDef = TypedDict(
+    "GetGroupResponseOutputTypeDef",
     {
-        "Group": GroupTypeDef,
-        "Users": List[UserTypeDef],
+        "Group": GroupOutputTypeDef,
+        "Users": List[UserOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetUserResponseTypeDef = TypedDict(
-    "GetUserResponseTypeDef",
+GetUserResponseOutputTypeDef = TypedDict(
+    "GetUserResponseOutputTypeDef",
     {
-        "User": UserTypeDef,
+        "User": UserOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListUsersResponseTypeDef = TypedDict(
-    "ListUsersResponseTypeDef",
+ListUsersResponseOutputTypeDef = TypedDict(
+    "ListUsersResponseOutputTypeDef",
     {
-        "Users": List[UserTypeDef],
+        "Users": List[UserOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VirtualMFADeviceTypeDef = TypedDict(
-    "VirtualMFADeviceTypeDef",
+VirtualMFADeviceOutputTypeDef = TypedDict(
+    "VirtualMFADeviceOutputTypeDef",
     {
         "SerialNumber": str,
         "Base32StringSeed": bytes,
         "QRCodePNG": bytes,
-        "User": UserTypeDef,
+        "User": UserOutputTypeDef,
         "EnableDate": datetime,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
-GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
-    "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
+GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef = TypedDict(
+    "GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
-        "Reason": DeletionTaskFailureReasonTypeTypeDef,
+        "Reason": DeletionTaskFailureReasonTypeOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef = TypedDict(
-    "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
+GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef = TypedDict(
+    "GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
-        "EntityDetailsList": List[EntityDetailsTypeDef],
+        "EntityDetailsList": List[EntityDetailsOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "Error": ErrorDetailsTypeDef,
+        "Error": ErrorDetailsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesGrantingServiceAccessResponseTypeDef = TypedDict(
-    "ListPoliciesGrantingServiceAccessResponseTypeDef",
+ListPoliciesGrantingServiceAccessResponseOutputTypeDef = TypedDict(
+    "ListPoliciesGrantingServiceAccessResponseOutputTypeDef",
     {
-        "PoliciesGrantingServiceAccess": List[ListPoliciesGrantingServiceAccessEntryTypeDef],
+        "PoliciesGrantingServiceAccess": List[ListPoliciesGrantingServiceAccessEntryOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServerCertificateResponseTypeDef = TypedDict(
-    "GetServerCertificateResponseTypeDef",
+GetServerCertificateResponseOutputTypeDef = TypedDict(
+    "GetServerCertificateResponseOutputTypeDef",
     {
-        "ServerCertificate": ServerCertificateTypeDef,
+        "ServerCertificate": ServerCertificateOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResourceSpecificResultTypeDef = TypedDict(
-    "ResourceSpecificResultTypeDef",
+ResourceSpecificResultOutputTypeDef = TypedDict(
+    "ResourceSpecificResultOutputTypeDef",
     {
         "EvalResourceName": str,
         "EvalResourceDecision": PolicyEvaluationDecisionTypeType,
-        "MatchedStatements": List[StatementTypeDef],
+        "MatchedStatements": List[StatementOutputTypeDef],
         "MissingContextValues": List[str],
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
-        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
+        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailOutputTypeDef,
     },
 )
 
-CreateRoleResponseTypeDef = TypedDict(
-    "CreateRoleResponseTypeDef",
+CreateRoleResponseOutputTypeDef = TypedDict(
+    "CreateRoleResponseOutputTypeDef",
     {
-        "Role": RoleTypeDef,
+        "Role": RoleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceLinkedRoleResponseTypeDef = TypedDict(
-    "CreateServiceLinkedRoleResponseTypeDef",
+CreateServiceLinkedRoleResponseOutputTypeDef = TypedDict(
+    "CreateServiceLinkedRoleResponseOutputTypeDef",
     {
-        "Role": RoleTypeDef,
+        "Role": RoleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetRoleResponseTypeDef = TypedDict(
-    "GetRoleResponseTypeDef",
+GetRoleResponseOutputTypeDef = TypedDict(
+    "GetRoleResponseOutputTypeDef",
     {
-        "Role": RoleTypeDef,
+        "Role": RoleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InstanceProfileTypeDef = TypedDict(
-    "InstanceProfileTypeDef",
+InstanceProfileOutputTypeDef = TypedDict(
+    "InstanceProfileOutputTypeDef",
     {
         "Path": str,
         "InstanceProfileName": str,
         "InstanceProfileId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "Roles": List[RoleTypeDef],
-        "Tags": List[TagTypeDef],
+        "Roles": List[RoleOutputTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
-ListRolesResponseTypeDef = TypedDict(
-    "ListRolesResponseTypeDef",
+ListRolesResponseOutputTypeDef = TypedDict(
+    "ListRolesResponseOutputTypeDef",
     {
-        "Roles": List[RoleTypeDef],
+        "Roles": List[RoleOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRoleDescriptionResponseTypeDef = TypedDict(
-    "UpdateRoleDescriptionResponseTypeDef",
+UpdateRoleDescriptionResponseOutputTypeDef = TypedDict(
+    "UpdateRoleDescriptionResponseOutputTypeDef",
     {
-        "Role": RoleTypeDef,
+        "Role": RoleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceLastAccessedDetailsResponseTypeDef = TypedDict(
-    "GetServiceLastAccessedDetailsResponseTypeDef",
+GetServiceLastAccessedDetailsResponseOutputTypeDef = TypedDict(
+    "GetServiceLastAccessedDetailsResponseOutputTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobType": AccessAdvisorUsageGranularityTypeType,
         "JobCreationDate": datetime,
-        "ServicesLastAccessed": List[ServiceLastAccessedTypeDef],
+        "ServicesLastAccessed": List[ServiceLastAccessedOutputTypeDef],
         "JobCompletionDate": datetime,
         "IsTruncated": bool,
         "Marker": str,
-        "Error": ErrorDetailsTypeDef,
+        "Error": ErrorDetailsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVirtualMFADeviceResponseTypeDef = TypedDict(
-    "CreateVirtualMFADeviceResponseTypeDef",
+CreateVirtualMFADeviceResponseOutputTypeDef = TypedDict(
+    "CreateVirtualMFADeviceResponseOutputTypeDef",
     {
-        "VirtualMFADevice": VirtualMFADeviceTypeDef,
+        "VirtualMFADevice": VirtualMFADeviceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListVirtualMFADevicesResponseTypeDef = TypedDict(
-    "ListVirtualMFADevicesResponseTypeDef",
+ListVirtualMFADevicesResponseOutputTypeDef = TypedDict(
+    "ListVirtualMFADevicesResponseOutputTypeDef",
     {
-        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
+        "VirtualMFADevices": List[VirtualMFADeviceOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EvaluationResultTypeDef = TypedDict(
-    "EvaluationResultTypeDef",
+EvaluationResultOutputTypeDef = TypedDict(
+    "EvaluationResultOutputTypeDef",
     {
         "EvalActionName": str,
         "EvalResourceName": str,
         "EvalDecision": PolicyEvaluationDecisionTypeType,
-        "MatchedStatements": List[StatementTypeDef],
+        "MatchedStatements": List[StatementOutputTypeDef],
         "MissingContextValues": List[str],
-        "OrganizationsDecisionDetail": OrganizationsDecisionDetailTypeDef,
-        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
+        "OrganizationsDecisionDetail": OrganizationsDecisionDetailOutputTypeDef,
+        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailOutputTypeDef,
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
-        "ResourceSpecificResults": List[ResourceSpecificResultTypeDef],
+        "ResourceSpecificResults": List[ResourceSpecificResultOutputTypeDef],
     },
 )
 
-CreateInstanceProfileResponseTypeDef = TypedDict(
-    "CreateInstanceProfileResponseTypeDef",
+CreateInstanceProfileResponseOutputTypeDef = TypedDict(
+    "CreateInstanceProfileResponseOutputTypeDef",
     {
-        "InstanceProfile": InstanceProfileTypeDef,
+        "InstanceProfile": InstanceProfileOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetInstanceProfileResponseTypeDef = TypedDict(
-    "GetInstanceProfileResponseTypeDef",
+GetInstanceProfileResponseOutputTypeDef = TypedDict(
+    "GetInstanceProfileResponseOutputTypeDef",
     {
-        "InstanceProfile": InstanceProfileTypeDef,
+        "InstanceProfile": InstanceProfileOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListInstanceProfilesForRoleResponseTypeDef = TypedDict(
-    "ListInstanceProfilesForRoleResponseTypeDef",
+ListInstanceProfilesForRoleResponseOutputTypeDef = TypedDict(
+    "ListInstanceProfilesForRoleResponseOutputTypeDef",
     {
-        "InstanceProfiles": List[InstanceProfileTypeDef],
+        "InstanceProfiles": List[InstanceProfileOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListInstanceProfilesResponseTypeDef = TypedDict(
-    "ListInstanceProfilesResponseTypeDef",
+ListInstanceProfilesResponseOutputTypeDef = TypedDict(
+    "ListInstanceProfilesResponseOutputTypeDef",
     {
-        "InstanceProfiles": List[InstanceProfileTypeDef],
+        "InstanceProfiles": List[InstanceProfileOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RoleDetailTypeDef = TypedDict(
-    "RoleDetailTypeDef",
+RoleDetailOutputTypeDef = TypedDict(
+    "RoleDetailOutputTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
         "CreateDate": datetime,
         "AssumeRolePolicyDocument": str,
-        "InstanceProfileList": List[InstanceProfileTypeDef],
-        "RolePolicyList": List[PolicyDetailTypeDef],
-        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-        "RoleLastUsed": RoleLastUsedTypeDef,
+        "InstanceProfileList": List[InstanceProfileOutputTypeDef],
+        "RolePolicyList": List[PolicyDetailOutputTypeDef],
+        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
+        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "RoleLastUsed": RoleLastUsedOutputTypeDef,
     },
 )
 
-SimulatePolicyResponseTypeDef = TypedDict(
-    "SimulatePolicyResponseTypeDef",
+SimulatePolicyResponseOutputTypeDef = TypedDict(
+    "SimulatePolicyResponseOutputTypeDef",
     {
-        "EvaluationResults": List[EvaluationResultTypeDef],
+        "EvaluationResults": List[EvaluationResultOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccountAuthorizationDetailsResponseTypeDef = TypedDict(
-    "GetAccountAuthorizationDetailsResponseTypeDef",
+GetAccountAuthorizationDetailsResponseOutputTypeDef = TypedDict(
+    "GetAccountAuthorizationDetailsResponseOutputTypeDef",
     {
-        "UserDetailList": List[UserDetailTypeDef],
-        "GroupDetailList": List[GroupDetailTypeDef],
-        "RoleDetailList": List[RoleDetailTypeDef],
-        "Policies": List[ManagedPolicyDetailTypeDef],
+        "UserDetailList": List[UserDetailOutputTypeDef],
+        "GroupDetailList": List[GroupDetailOutputTypeDef],
+        "RoleDetailList": List[RoleDetailOutputTypeDef],
+        "Policies": List[ManagedPolicyDetailOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/waiter.py` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam/waiter.pyi` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/PKG-INFO` & `mypy-boto3-iam-1.28.3.post1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-iam
-Version: 1.28.3
-Summary: Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.6
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iam type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iam"></a>
 
 # mypy-boto3-iam
 
 [![PyPI - mypy-boto3-iam](https://img.shields.io/pypi/v/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/)
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
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -639,18 +607,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_iam.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iam.type_defs import (
-    AccessDetailTypeDef,
-    AccessKeyLastUsedTypeDef,
-    AccessKeyMetadataTypeDef,
-    AccessKeyTypeDef,
+    AccessDetailOutputTypeDef,
+    AccessKeyLastUsedOutputTypeDef,
+    AccessKeyMetadataOutputTypeDef,
+    AccessKeyOutputTypeDef,
     AddClientIDToOpenIDConnectProviderRequestRequestTypeDef,
     AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef,
     AddRoleToInstanceProfileRequestRequestTypeDef,
     AddUserToGroupRequestGroupAddUserTypeDef,
     AddUserToGroupRequestRequestTypeDef,
     AddUserToGroupRequestUserAddGroupTypeDef,
     AttachGroupPolicyRequestGroupAttachPolicyTypeDef,
@@ -658,38 +626,39 @@
     AttachGroupPolicyRequestRequestTypeDef,
     AttachRolePolicyRequestPolicyAttachRoleTypeDef,
     AttachRolePolicyRequestRequestTypeDef,
     AttachRolePolicyRequestRoleAttachPolicyTypeDef,
     AttachUserPolicyRequestPolicyAttachUserTypeDef,
     AttachUserPolicyRequestRequestTypeDef,
     AttachUserPolicyRequestUserAttachPolicyTypeDef,
+    AttachedPermissionsBoundaryOutputTypeDef,
     AttachedPermissionsBoundaryResponseMetadataTypeDef,
-    AttachedPermissionsBoundaryTypeDef,
-    AttachedPolicyTypeDef,
+    AttachedPolicyOutputTypeDef,
     ChangePasswordRequestRequestTypeDef,
     ChangePasswordRequestServiceResourceChangePasswordTypeDef,
     ContextEntryTypeDef,
     CreateAccessKeyRequestRequestTypeDef,
     CreateAccountAliasRequestRequestTypeDef,
     CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef,
     CreateGroupRequestGroupCreateTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateGroupRequestServiceResourceCreateGroupTypeDef,
-    GroupTypeDef,
+    GroupOutputTypeDef,
     TagTypeDef,
     CreateLoginProfileRequestLoginProfileCreateTypeDef,
     CreateLoginProfileRequestRequestTypeDef,
     CreateLoginProfileRequestUserCreateLoginProfileTypeDef,
-    LoginProfileTypeDef,
+    LoginProfileOutputTypeDef,
+    TagOutputTypeDef,
     CreatePolicyVersionRequestPolicyCreateVersionTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    PolicyVersionTypeDef,
+    PolicyVersionOutputTypeDef,
     CreateServiceLinkedRoleRequestRequestTypeDef,
     CreateServiceSpecificCredentialRequestRequestTypeDef,
-    ServiceSpecificCredentialTypeDef,
+    ServiceSpecificCredentialOutputTypeDef,
     DeactivateMFADeviceRequestRequestTypeDef,
     DeleteAccessKeyRequestRequestTypeDef,
     DeleteAccountAliasRequestRequestTypeDef,
     DeleteGroupPolicyRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
     DeleteLoginProfileRequestRequestTypeDef,
@@ -699,159 +668,159 @@
     DeleteRolePermissionsBoundaryRequestRequestTypeDef,
     DeleteRolePolicyRequestRequestTypeDef,
     DeleteRoleRequestRequestTypeDef,
     DeleteSAMLProviderRequestRequestTypeDef,
     DeleteSSHPublicKeyRequestRequestTypeDef,
     DeleteServerCertificateRequestRequestTypeDef,
     DeleteServiceLinkedRoleRequestRequestTypeDef,
-    DeleteServiceLinkedRoleResponseTypeDef,
+    DeleteServiceLinkedRoleResponseOutputTypeDef,
     DeleteServiceSpecificCredentialRequestRequestTypeDef,
     DeleteSigningCertificateRequestRequestTypeDef,
     DeleteUserPermissionsBoundaryRequestRequestTypeDef,
     DeleteUserPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVirtualMFADeviceRequestRequestTypeDef,
-    RoleUsageTypeTypeDef,
+    RoleUsageTypeOutputTypeDef,
     DetachGroupPolicyRequestGroupDetachPolicyTypeDef,
     DetachGroupPolicyRequestPolicyDetachGroupTypeDef,
     DetachGroupPolicyRequestRequestTypeDef,
     DetachRolePolicyRequestPolicyDetachRoleTypeDef,
     DetachRolePolicyRequestRequestTypeDef,
     DetachRolePolicyRequestRoleDetachPolicyTypeDef,
     DetachUserPolicyRequestPolicyDetachUserTypeDef,
     DetachUserPolicyRequestRequestTypeDef,
     DetachUserPolicyRequestUserDetachPolicyTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableMFADeviceRequestMfaDeviceAssociateTypeDef,
     EnableMFADeviceRequestRequestTypeDef,
     EnableMFADeviceRequestUserEnableMfaTypeDef,
-    EntityInfoTypeDef,
-    ErrorDetailsTypeDef,
-    OrganizationsDecisionDetailTypeDef,
-    PermissionsBoundaryDecisionDetailTypeDef,
-    GenerateCredentialReportResponseTypeDef,
+    EntityInfoOutputTypeDef,
+    ErrorDetailsOutputTypeDef,
+    OrganizationsDecisionDetailOutputTypeDef,
+    PermissionsBoundaryDecisionDetailOutputTypeDef,
+    GenerateCredentialReportResponseOutputTypeDef,
     GenerateOrganizationsAccessReportRequestRequestTypeDef,
-    GenerateOrganizationsAccessReportResponseTypeDef,
+    GenerateOrganizationsAccessReportResponseOutputTypeDef,
     GenerateServiceLastAccessedDetailsRequestRequestTypeDef,
-    GenerateServiceLastAccessedDetailsResponseTypeDef,
+    GenerateServiceLastAccessedDetailsResponseOutputTypeDef,
     GetAccessKeyLastUsedRequestRequestTypeDef,
     GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
     GetAccountAuthorizationDetailsRequestRequestTypeDef,
-    PasswordPolicyTypeDef,
-    GetAccountSummaryResponseTypeDef,
+    PasswordPolicyOutputTypeDef,
+    GetAccountSummaryResponseOutputTypeDef,
     GetContextKeysForCustomPolicyRequestRequestTypeDef,
-    GetContextKeysForPolicyResponseTypeDef,
+    GetContextKeysForPolicyResponseOutputTypeDef,
     GetContextKeysForPrincipalPolicyRequestRequestTypeDef,
-    GetCredentialReportResponseTypeDef,
+    GetCredentialReportResponseOutputTypeDef,
     GetGroupPolicyRequestRequestTypeDef,
-    GetGroupPolicyResponseTypeDef,
+    GetGroupPolicyResponseOutputTypeDef,
     GetGroupRequestGetGroupPaginateTypeDef,
     GetGroupRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetLoginProfileRequestRequestTypeDef,
     GetMFADeviceRequestRequestTypeDef,
-    GetMFADeviceResponseTypeDef,
+    GetMFADeviceResponseOutputTypeDef,
     GetOpenIDConnectProviderRequestRequestTypeDef,
     GetOrganizationsAccessReportRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
     GetRolePolicyRequestRequestTypeDef,
-    GetRolePolicyResponseTypeDef,
+    GetRolePolicyResponseOutputTypeDef,
     GetRoleRequestRequestTypeDef,
     GetSAMLProviderRequestRequestTypeDef,
     GetSSHPublicKeyRequestRequestTypeDef,
-    SSHPublicKeyTypeDef,
+    SSHPublicKeyOutputTypeDef,
     GetServerCertificateRequestRequestTypeDef,
     GetServiceLastAccessedDetailsRequestRequestTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
     GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef,
     GetUserPolicyRequestRequestTypeDef,
-    GetUserPolicyResponseTypeDef,
+    GetUserPolicyResponseOutputTypeDef,
     GetUserRequestRequestTypeDef,
-    PolicyDetailTypeDef,
+    PolicyDetailOutputTypeDef,
     ListAccessKeysRequestListAccessKeysPaginateTypeDef,
     ListAccessKeysRequestRequestTypeDef,
     ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
     ListAccountAliasesRequestRequestTypeDef,
-    ListAccountAliasesResponseTypeDef,
+    ListAccountAliasesResponseOutputTypeDef,
     ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
     ListAttachedGroupPoliciesRequestRequestTypeDef,
     ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
     ListAttachedRolePoliciesRequestRequestTypeDef,
     ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
     ListAttachedUserPoliciesRequestRequestTypeDef,
     ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
     ListEntitiesForPolicyRequestRequestTypeDef,
-    PolicyGroupTypeDef,
-    PolicyRoleTypeDef,
-    PolicyUserTypeDef,
+    PolicyGroupOutputTypeDef,
+    PolicyRoleOutputTypeDef,
+    PolicyUserOutputTypeDef,
     ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
     ListGroupPoliciesRequestRequestTypeDef,
-    ListGroupPoliciesResponseTypeDef,
+    ListGroupPoliciesResponseOutputTypeDef,
     ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
     ListGroupsForUserRequestRequestTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
     ListInstanceProfileTagsRequestRequestTypeDef,
     ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
     ListInstanceProfilesForRoleRequestRequestTypeDef,
     ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
     ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
     ListMFADeviceTagsRequestRequestTypeDef,
     ListMFADevicesRequestListMFADevicesPaginateTypeDef,
     ListMFADevicesRequestRequestTypeDef,
-    MFADeviceTypeDef,
+    MFADeviceOutputTypeDef,
     ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
     ListOpenIDConnectProviderTagsRequestRequestTypeDef,
-    OpenIDConnectProviderListEntryTypeDef,
-    PolicyGrantingServiceAccessTypeDef,
+    OpenIDConnectProviderListEntryOutputTypeDef,
+    PolicyGrantingServiceAccessOutputTypeDef,
     ListPoliciesGrantingServiceAccessRequestRequestTypeDef,
     ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
     ListPolicyTagsRequestRequestTypeDef,
     ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
     ListRolePoliciesRequestRequestTypeDef,
-    ListRolePoliciesResponseTypeDef,
+    ListRolePoliciesResponseOutputTypeDef,
     ListRoleTagsRequestListRoleTagsPaginateTypeDef,
     ListRoleTagsRequestRequestTypeDef,
     ListRolesRequestListRolesPaginateTypeDef,
     ListRolesRequestRequestTypeDef,
     ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
     ListSAMLProviderTagsRequestRequestTypeDef,
-    SAMLProviderListEntryTypeDef,
+    SAMLProviderListEntryOutputTypeDef,
     ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
     ListSSHPublicKeysRequestRequestTypeDef,
-    SSHPublicKeyMetadataTypeDef,
+    SSHPublicKeyMetadataOutputTypeDef,
     ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
     ListServerCertificateTagsRequestRequestTypeDef,
     ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
     ListServerCertificatesRequestRequestTypeDef,
-    ServerCertificateMetadataTypeDef,
+    ServerCertificateMetadataOutputTypeDef,
     ListServiceSpecificCredentialsRequestRequestTypeDef,
-    ServiceSpecificCredentialMetadataTypeDef,
+    ServiceSpecificCredentialMetadataOutputTypeDef,
     ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
     ListSigningCertificatesRequestRequestTypeDef,
-    SigningCertificateTypeDef,
+    SigningCertificateOutputTypeDef,
     ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
     ListUserPoliciesRequestRequestTypeDef,
-    ListUserPoliciesResponseTypeDef,
+    ListUserPoliciesResponseOutputTypeDef,
     ListUserTagsRequestListUserTagsPaginateTypeDef,
     ListUserTagsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
     ListVirtualMFADevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    PositionTypeDef,
+    PositionOutputTypeDef,
     PutGroupPolicyRequestGroupCreatePolicyTypeDef,
     PutGroupPolicyRequestGroupPolicyPutTypeDef,
     PutGroupPolicyRequestRequestTypeDef,
     PutRolePermissionsBoundaryRequestRequestTypeDef,
     PutRolePolicyRequestRequestTypeDef,
     PutRolePolicyRequestRolePolicyPutTypeDef,
     PutUserPermissionsBoundaryRequestRequestTypeDef,
@@ -864,18 +833,18 @@
     RemoveUserFromGroupRequestGroupRemoveUserTypeDef,
     RemoveUserFromGroupRequestRequestTypeDef,
     RemoveUserFromGroupRequestUserRemoveGroupTypeDef,
     ResetServiceSpecificCredentialRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ResyncMFADeviceRequestMfaDeviceResyncTypeDef,
     ResyncMFADeviceRequestRequestTypeDef,
-    RoleLastUsedTypeDef,
+    RoleLastUsedOutputTypeDef,
     RoleLastUsedResponseMetadataTypeDef,
     ServerCertificateMetadataResponseMetadataTypeDef,
-    TrackedActionLastAccessedTypeDef,
+    TrackedActionLastAccessedOutputTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetSecurityTokenServicePreferencesRequestRequestTypeDef,
     UntagInstanceProfileRequestRequestTypeDef,
     UntagMFADeviceRequestRequestTypeDef,
     UntagOpenIDConnectProviderRequestRequestTypeDef,
     UntagPolicyRequestRequestTypeDef,
     UntagRoleRequestRequestTypeDef,
@@ -897,148 +866,148 @@
     UpdateLoginProfileRequestLoginProfileUpdateTypeDef,
     UpdateLoginProfileRequestRequestTypeDef,
     UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef,
     UpdateRoleDescriptionRequestRequestTypeDef,
     UpdateRoleRequestRequestTypeDef,
     UpdateSAMLProviderRequestRequestTypeDef,
     UpdateSAMLProviderRequestSamlProviderUpdateTypeDef,
-    UpdateSAMLProviderResponseTypeDef,
+    UpdateSAMLProviderResponseOutputTypeDef,
     UpdateSSHPublicKeyRequestRequestTypeDef,
     UpdateServerCertificateRequestRequestTypeDef,
     UpdateServerCertificateRequestServerCertificateUpdateTypeDef,
     UpdateServiceSpecificCredentialRequestRequestTypeDef,
     UpdateSigningCertificateRequestRequestTypeDef,
     UpdateSigningCertificateRequestSigningCertificateActivateTypeDef,
     UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserRequestUserUpdateTypeDef,
     UploadSSHPublicKeyRequestRequestTypeDef,
     UploadSigningCertificateRequestRequestTypeDef,
     UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
-    GetAccessKeyLastUsedResponseTypeDef,
-    ListAccessKeysResponseTypeDef,
-    CreateAccessKeyResponseTypeDef,
-    ListAttachedGroupPoliciesResponseTypeDef,
-    ListAttachedRolePoliciesResponseTypeDef,
-    ListAttachedUserPoliciesResponseTypeDef,
+    GetAccessKeyLastUsedResponseOutputTypeDef,
+    ListAccessKeysResponseOutputTypeDef,
+    CreateAccessKeyResponseOutputTypeDef,
+    ListAttachedGroupPoliciesResponseOutputTypeDef,
+    ListAttachedRolePoliciesResponseOutputTypeDef,
+    ListAttachedUserPoliciesResponseOutputTypeDef,
     SimulateCustomPolicyRequestRequestTypeDef,
     SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
     SimulatePrincipalPolicyRequestRequestTypeDef,
     SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
-    CreateGroupResponseTypeDef,
-    ListGroupsForUserResponseTypeDef,
-    ListGroupsResponseTypeDef,
+    CreateGroupResponseOutputTypeDef,
+    ListGroupsForUserResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
     CreateOpenIDConnectProviderRequestRequestTypeDef,
-    CreateOpenIDConnectProviderResponseTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreatePolicyRequestServiceResourceCreatePolicyTypeDef,
     CreateRoleRequestRequestTypeDef,
     CreateRoleRequestServiceResourceCreateRoleTypeDef,
     CreateSAMLProviderRequestRequestTypeDef,
     CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef,
-    CreateSAMLProviderResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     CreateUserRequestServiceResourceCreateUserTypeDef,
     CreateUserRequestUserCreateTypeDef,
     CreateVirtualMFADeviceRequestRequestTypeDef,
     CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef,
-    GetOpenIDConnectProviderResponseTypeDef,
-    GetSAMLProviderResponseTypeDef,
-    ListInstanceProfileTagsResponseTypeDef,
-    ListMFADeviceTagsResponseTypeDef,
-    ListOpenIDConnectProviderTagsResponseTypeDef,
-    ListPolicyTagsResponseTypeDef,
-    ListRoleTagsResponseTypeDef,
-    ListSAMLProviderTagsResponseTypeDef,
-    ListServerCertificateTagsResponseTypeDef,
-    ListUserTagsResponseTypeDef,
-    PolicyTypeDef,
     TagInstanceProfileRequestRequestTypeDef,
     TagMFADeviceRequestRequestTypeDef,
     TagOpenIDConnectProviderRequestRequestTypeDef,
     TagPolicyRequestRequestTypeDef,
     TagRoleRequestRequestTypeDef,
     TagSAMLProviderRequestRequestTypeDef,
     TagServerCertificateRequestRequestTypeDef,
     TagUserRequestRequestTypeDef,
     UploadServerCertificateRequestRequestTypeDef,
     UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
+    CreateLoginProfileResponseOutputTypeDef,
+    GetLoginProfileResponseOutputTypeDef,
+    CreateOpenIDConnectProviderResponseOutputTypeDef,
+    CreateSAMLProviderResponseOutputTypeDef,
+    GetOpenIDConnectProviderResponseOutputTypeDef,
+    GetSAMLProviderResponseOutputTypeDef,
+    ListInstanceProfileTagsResponseOutputTypeDef,
+    ListMFADeviceTagsResponseOutputTypeDef,
+    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
+    ListPolicyTagsResponseOutputTypeDef,
+    ListRoleTagsResponseOutputTypeDef,
+    ListSAMLProviderTagsResponseOutputTypeDef,
+    ListServerCertificateTagsResponseOutputTypeDef,
+    ListUserTagsResponseOutputTypeDef,
+    PolicyOutputTypeDef,
+    UserOutputTypeDef,
     UserResponseMetadataTypeDef,
-    UserTypeDef,
-    CreateLoginProfileResponseTypeDef,
-    GetLoginProfileResponseTypeDef,
-    CreatePolicyVersionResponseTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    ListPolicyVersionsResponseTypeDef,
-    ManagedPolicyDetailTypeDef,
-    CreateServiceSpecificCredentialResponseTypeDef,
-    ResetServiceSpecificCredentialResponseTypeDef,
-    DeletionTaskFailureReasonTypeTypeDef,
-    EntityDetailsTypeDef,
-    GetOrganizationsAccessReportResponseTypeDef,
-    GetAccountPasswordPolicyResponseTypeDef,
+    CreatePolicyVersionResponseOutputTypeDef,
+    GetPolicyVersionResponseOutputTypeDef,
+    ListPolicyVersionsResponseOutputTypeDef,
+    ManagedPolicyDetailOutputTypeDef,
+    CreateServiceSpecificCredentialResponseOutputTypeDef,
+    ResetServiceSpecificCredentialResponseOutputTypeDef,
+    DeletionTaskFailureReasonTypeOutputTypeDef,
+    EntityDetailsOutputTypeDef,
+    GetOrganizationsAccessReportResponseOutputTypeDef,
+    GetAccountPasswordPolicyResponseOutputTypeDef,
     GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
     GetPolicyRequestPolicyExistsWaitTypeDef,
     GetRoleRequestRoleExistsWaitTypeDef,
     GetUserRequestUserExistsWaitTypeDef,
-    GetSSHPublicKeyResponseTypeDef,
-    UploadSSHPublicKeyResponseTypeDef,
-    GroupDetailTypeDef,
-    UserDetailTypeDef,
-    ListEntitiesForPolicyResponseTypeDef,
-    ListMFADevicesResponseTypeDef,
-    ListOpenIDConnectProvidersResponseTypeDef,
-    ListPoliciesGrantingServiceAccessEntryTypeDef,
-    ListSAMLProvidersResponseTypeDef,
-    ListSSHPublicKeysResponseTypeDef,
-    ListServerCertificatesResponseTypeDef,
-    ServerCertificateTypeDef,
-    UploadServerCertificateResponseTypeDef,
-    ListServiceSpecificCredentialsResponseTypeDef,
-    ListSigningCertificatesResponseTypeDef,
-    UploadSigningCertificateResponseTypeDef,
-    StatementTypeDef,
-    RoleTypeDef,
-    ServiceLastAccessedTypeDef,
-    CreatePolicyResponseTypeDef,
-    GetPolicyResponseTypeDef,
-    ListPoliciesResponseTypeDef,
-    CreateUserResponseTypeDef,
-    GetGroupResponseTypeDef,
-    GetUserResponseTypeDef,
-    ListUsersResponseTypeDef,
-    VirtualMFADeviceTypeDef,
-    GetServiceLinkedRoleDeletionStatusResponseTypeDef,
-    GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
-    ListPoliciesGrantingServiceAccessResponseTypeDef,
-    GetServerCertificateResponseTypeDef,
-    ResourceSpecificResultTypeDef,
-    CreateRoleResponseTypeDef,
-    CreateServiceLinkedRoleResponseTypeDef,
-    GetRoleResponseTypeDef,
-    InstanceProfileTypeDef,
-    ListRolesResponseTypeDef,
-    UpdateRoleDescriptionResponseTypeDef,
-    GetServiceLastAccessedDetailsResponseTypeDef,
-    CreateVirtualMFADeviceResponseTypeDef,
-    ListVirtualMFADevicesResponseTypeDef,
-    EvaluationResultTypeDef,
-    CreateInstanceProfileResponseTypeDef,
-    GetInstanceProfileResponseTypeDef,
-    ListInstanceProfilesForRoleResponseTypeDef,
-    ListInstanceProfilesResponseTypeDef,
-    RoleDetailTypeDef,
-    SimulatePolicyResponseTypeDef,
-    GetAccountAuthorizationDetailsResponseTypeDef,
+    GetSSHPublicKeyResponseOutputTypeDef,
+    UploadSSHPublicKeyResponseOutputTypeDef,
+    GroupDetailOutputTypeDef,
+    UserDetailOutputTypeDef,
+    ListEntitiesForPolicyResponseOutputTypeDef,
+    ListMFADevicesResponseOutputTypeDef,
+    ListOpenIDConnectProvidersResponseOutputTypeDef,
+    ListPoliciesGrantingServiceAccessEntryOutputTypeDef,
+    ListSAMLProvidersResponseOutputTypeDef,
+    ListSSHPublicKeysResponseOutputTypeDef,
+    ListServerCertificatesResponseOutputTypeDef,
+    ServerCertificateOutputTypeDef,
+    UploadServerCertificateResponseOutputTypeDef,
+    ListServiceSpecificCredentialsResponseOutputTypeDef,
+    ListSigningCertificatesResponseOutputTypeDef,
+    UploadSigningCertificateResponseOutputTypeDef,
+    StatementOutputTypeDef,
+    RoleOutputTypeDef,
+    ServiceLastAccessedOutputTypeDef,
+    CreatePolicyResponseOutputTypeDef,
+    GetPolicyResponseOutputTypeDef,
+    ListPoliciesResponseOutputTypeDef,
+    CreateUserResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    GetUserResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
+    VirtualMFADeviceOutputTypeDef,
+    GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef,
+    GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef,
+    ListPoliciesGrantingServiceAccessResponseOutputTypeDef,
+    GetServerCertificateResponseOutputTypeDef,
+    ResourceSpecificResultOutputTypeDef,
+    CreateRoleResponseOutputTypeDef,
+    CreateServiceLinkedRoleResponseOutputTypeDef,
+    GetRoleResponseOutputTypeDef,
+    InstanceProfileOutputTypeDef,
+    ListRolesResponseOutputTypeDef,
+    UpdateRoleDescriptionResponseOutputTypeDef,
+    GetServiceLastAccessedDetailsResponseOutputTypeDef,
+    CreateVirtualMFADeviceResponseOutputTypeDef,
+    ListVirtualMFADevicesResponseOutputTypeDef,
+    EvaluationResultOutputTypeDef,
+    CreateInstanceProfileResponseOutputTypeDef,
+    GetInstanceProfileResponseOutputTypeDef,
+    ListInstanceProfilesForRoleResponseOutputTypeDef,
+    ListInstanceProfilesResponseOutputTypeDef,
+    RoleDetailOutputTypeDef,
+    SimulatePolicyResponseOutputTypeDef,
+    GetAccountAuthorizationDetailsResponseOutputTypeDef,
 )
 
 
-def get_structure() -> AccessDetailTypeDef:
+def get_structure() -> AccessDetailOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/SOURCES.txt` & `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3/setup.py` & `mypy-boto3-iam-1.28.3.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iam",
-    version="1.28.3",
+    version="1.28.3.post1",
     packages=["mypy_boto3_iam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.6"
+        "Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.7"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

