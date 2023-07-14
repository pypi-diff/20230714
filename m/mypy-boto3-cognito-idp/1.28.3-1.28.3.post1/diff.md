# Comparing `tmp/mypy-boto3-cognito-idp-1.28.3.tar.gz` & `tmp/mypy-boto3-cognito-idp-1.28.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-idp-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
+gzip compressed data, was "mypy-boto3-cognito-idp-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
```

## Comparing `mypy-boto3-cognito-idp-1.28.3.tar` & `mypy-boto3-cognito-idp-1.28.3.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.673227 mypy-boto3-cognito-idp-1.28.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-13 19:49:12.665227 mypy-boto3-cognito-idp-1.28.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.657227 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78755 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    78638 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-13 19:46:56.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-13 19:46:56.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    95323 2023-07-13 19:46:58.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    95194 2023-07-13 19:46:57.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.665227 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.673227 mypy-boto3-cognito-idp-1.28.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 19:46:54.000000 mypy-boto3-cognito-idp-1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.903361 mypy-boto3-cognito-idp-1.28.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27194 2023-07-14 16:17:59.899361 mypy-boto3-cognito-idp-1.28.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25675 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79559 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79442 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-14 16:15:17.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-14 16:15:17.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   108255 2023-07-14 16:15:20.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108118 2023-07-14 16:15:18.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.899361 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27194 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.903361 mypy-boto3-cognito-idp-1.28.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-14 16:15:15.000000 mypy-boto3-cognito-idp-1.28.3.post1/setup.py
```

### Comparing `mypy-boto3-cognito-idp-1.28.3/LICENSE` & `mypy-boto3-cognito-idp-1.28.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3/PKG-INFO` & `mypy-boto3-cognito-idp-1.28.3.post1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.28.3
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -394,73 +394,83 @@
 ### Typed dictionaries
 
 `mypy_boto3_cognito_idp.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_idp.type_defs import (
+    RecoveryOptionTypeOutputTypeDef,
     RecoveryOptionTypeTypeDef,
+    AccountTakeoverActionTypeOutputTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
+    MessageTemplateTypeOutputTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
     ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
-    MFAOptionTypeTypeDef,
+    AttributeTypeOutputTypeDef,
+    MFAOptionTypeOutputTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
-    GroupTypeTypeDef,
+    GroupTypeOutputTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
+    MFAOptionTypeTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
+    AnalyticsConfigurationTypeOutputTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    ChallengeResponseTypeTypeDef,
-    EventContextDataTypeTypeDef,
-    EventFeedbackTypeTypeDef,
-    EventRiskTypeTypeDef,
-    NewDeviceMetadataTypeTypeDef,
+    ChallengeResponseTypeOutputTypeDef,
+    EventContextDataTypeOutputTypeDef,
+    EventFeedbackTypeOutputTypeDef,
+    EventRiskTypeOutputTypeDef,
+    NewDeviceMetadataTypeOutputTypeDef,
     ChangePasswordRequestRequestTypeDef,
-    CodeDeliveryDetailsTypeTypeDef,
+    CodeDeliveryDetailsTypeOutputTypeDef,
+    CompromisedCredentialsActionsTypeOutputTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    IdentityProviderTypeTypeDef,
+    IdentityProviderTypeOutputTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
-    UserImportJobTypeTypeDef,
+    UserImportJobTypeOutputTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
+    CustomDomainConfigTypeOutputTypeDef,
+    CustomEmailLambdaVersionConfigTypeOutputTypeDef,
     CustomEmailLambdaVersionConfigTypeTypeDef,
+    CustomSMSLambdaVersionConfigTypeOutputTypeDef,
     CustomSMSLambdaVersionConfigTypeTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
     DeleteResourceServerRequestRequestTypeDef,
     DeleteUserAttributesRequestRequestTypeDef,
     DeleteUserPoolClientRequestRequestTypeDef,
     DeleteUserPoolDomainRequestRequestTypeDef,
@@ -469,181 +479,206 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
+    DeviceConfigurationTypeOutputTypeDef,
+    EmailConfigurationTypeOutputTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
     GetUICustomizationRequestRequestTypeDef,
-    UICustomizationTypeTypeDef,
+    UICustomizationTypeOutputTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
-    SoftwareTokenMfaConfigTypeTypeDef,
+    SoftwareTokenMfaConfigTypeOutputTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
-    ProviderDescriptionTypeDef,
+    ProviderDescriptionOutputTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
-    UserPoolClientDescriptionTypeDef,
+    UserPoolClientDescriptionOutputTypeDef,
     ListUserPoolsRequestRequestTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
+    NotifyEmailTypeOutputTypeDef,
     NotifyEmailTypeTypeDef,
+    NumberAttributeConstraintsTypeOutputTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
+    PasswordPolicyTypeOutputTypeDef,
     PasswordPolicyTypeTypeDef,
+    ResourceServerScopeTypeOutputTypeDef,
     RevokeTokenRequestRequestTypeDef,
+    RiskExceptionConfigurationTypeOutputTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
+    StringAttributeConstraintsTypeOutputTypeDef,
     StringAttributeConstraintsTypeTypeDef,
     SetUICustomizationRequestRequestTypeDef,
+    SoftwareTokenMfaConfigTypeTypeDef,
+    SmsConfigurationTypeOutputTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    TokenValidityUnitsTypeOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
+    UserAttributeUpdateSettingsTypeOutputTypeDef,
+    UserPoolAddOnsTypeOutputTypeDef,
+    UsernameConfigurationTypeOutputTypeDef,
+    VerificationMessageTemplateTypeOutputTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
+    AccountRecoverySettingTypeOutputTypeDef,
     AccountRecoverySettingTypeTypeDef,
+    AccountTakeoverActionsTypeOutputTypeDef,
     AccountTakeoverActionsTypeTypeDef,
+    AdminCreateUserConfigTypeOutputTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
-    DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
-    ConfirmDeviceResponseTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
+    AssociateSoftwareTokenResponseOutputTypeDef,
+    ConfirmDeviceResponseOutputTypeDef,
+    CreateUserPoolDomainResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetCSVHeaderResponseTypeDef,
-    GetSigningCertificateResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
+    GetCSVHeaderResponseOutputTypeDef,
+    GetSigningCertificateResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    UpdateUserPoolDomainResponseOutputTypeDef,
+    VerifySoftwareTokenResponseOutputTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
-    AdminGetUserResponseTypeDef,
-    AdminSetUserSettingsRequestRequestTypeDef,
-    GetUserResponseTypeDef,
-    SetUserSettingsRequestRequestTypeDef,
-    UserTypeTypeDef,
+    DeviceTypeOutputTypeDef,
+    AdminGetUserResponseOutputTypeDef,
+    GetUserResponseOutputTypeDef,
+    UserTypeOutputTypeDef,
     AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
     AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
-    AdminListGroupsForUserResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    GetGroupResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    UpdateGroupResponseTypeDef,
+    AdminListGroupsForUserResponseOutputTypeDef,
+    CreateGroupResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
+    UpdateGroupResponseOutputTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
-    AuthEventTypeTypeDef,
-    AuthenticationResultTypeTypeDef,
-    ForgotPasswordResponseTypeDef,
-    GetUserAttributeVerificationCodeResponseTypeDef,
-    ResendConfirmationCodeResponseTypeDef,
-    SignUpResponseTypeDef,
-    UpdateUserAttributesResponseTypeDef,
+    AdminSetUserSettingsRequestRequestTypeDef,
+    SetUserSettingsRequestRequestTypeDef,
+    AuthEventTypeOutputTypeDef,
+    AuthenticationResultTypeOutputTypeDef,
+    ForgotPasswordResponseOutputTypeDef,
+    GetUserAttributeVerificationCodeResponseOutputTypeDef,
+    ResendConfirmationCodeResponseOutputTypeDef,
+    SignUpResponseOutputTypeDef,
+    UpdateUserAttributesResponseOutputTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
     ConfirmDeviceRequestRequestTypeDef,
     ConfirmForgotPasswordRequestRequestTypeDef,
     ConfirmSignUpRequestRequestTypeDef,
     ForgotPasswordRequestRequestTypeDef,
     InitiateAuthRequestRequestTypeDef,
     ResendConfirmationCodeRequestRequestTypeDef,
     RespondToAuthChallengeRequestRequestTypeDef,
     SignUpRequestRequestTypeDef,
     ContextDataTypeTypeDef,
-    CreateIdentityProviderResponseTypeDef,
-    DescribeIdentityProviderResponseTypeDef,
-    GetIdentityProviderByIdentifierResponseTypeDef,
-    UpdateIdentityProviderResponseTypeDef,
+    CreateIdentityProviderResponseOutputTypeDef,
+    DescribeIdentityProviderResponseOutputTypeDef,
+    GetIdentityProviderByIdentifierResponseOutputTypeDef,
+    UpdateIdentityProviderResponseOutputTypeDef,
     CreateResourceServerRequestRequestTypeDef,
-    ResourceServerTypeTypeDef,
     UpdateResourceServerRequestRequestTypeDef,
-    CreateUserImportJobResponseTypeDef,
-    DescribeUserImportJobResponseTypeDef,
-    ListUserImportJobsResponseTypeDef,
-    StartUserImportJobResponseTypeDef,
-    StopUserImportJobResponseTypeDef,
+    CreateUserImportJobResponseOutputTypeDef,
+    DescribeUserImportJobResponseOutputTypeDef,
+    ListUserImportJobsResponseOutputTypeDef,
+    StartUserImportJobResponseOutputTypeDef,
+    StopUserImportJobResponseOutputTypeDef,
     CreateUserPoolClientRequestRequestTypeDef,
     UpdateUserPoolClientRequestRequestTypeDef,
-    UserPoolClientTypeTypeDef,
     CreateUserPoolDomainRequestRequestTypeDef,
-    DomainDescriptionTypeTypeDef,
     UpdateUserPoolDomainRequestRequestTypeDef,
     SmsMfaConfigTypeTypeDef,
+    DomainDescriptionTypeOutputTypeDef,
+    LambdaConfigTypeOutputTypeDef,
     LambdaConfigTypeTypeDef,
-    GetUICustomizationResponseTypeDef,
-    SetUICustomizationResponseTypeDef,
-    ListIdentityProvidersResponseTypeDef,
-    ListUserPoolClientsResponseTypeDef,
+    GetUICustomizationResponseOutputTypeDef,
+    SetUICustomizationResponseOutputTypeDef,
+    ListIdentityProvidersResponseOutputTypeDef,
+    ListUserPoolClientsResponseOutputTypeDef,
+    NotifyConfigurationTypeOutputTypeDef,
     NotifyConfigurationTypeTypeDef,
+    UserPoolPolicyTypeOutputTypeDef,
     UserPoolPolicyTypeTypeDef,
+    ResourceServerTypeOutputTypeDef,
+    SchemaAttributeTypeOutputTypeDef,
     SchemaAttributeTypeTypeDef,
-    AdminGetDeviceResponseTypeDef,
-    AdminListDevicesResponseTypeDef,
-    GetDeviceResponseTypeDef,
-    ListDevicesResponseTypeDef,
-    AdminCreateUserResponseTypeDef,
-    ListUsersInGroupResponseTypeDef,
-    ListUsersResponseTypeDef,
-    AdminListUserAuthEventsResponseTypeDef,
-    AdminInitiateAuthResponseTypeDef,
-    AdminRespondToAuthChallengeResponseTypeDef,
-    InitiateAuthResponseTypeDef,
-    RespondToAuthChallengeResponseTypeDef,
+    SmsMfaConfigTypeOutputTypeDef,
+    UserPoolClientTypeOutputTypeDef,
+    AdminGetDeviceResponseOutputTypeDef,
+    AdminListDevicesResponseOutputTypeDef,
+    GetDeviceResponseOutputTypeDef,
+    ListDevicesResponseOutputTypeDef,
+    AdminCreateUserResponseOutputTypeDef,
+    ListUsersInGroupResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
+    AdminListUserAuthEventsResponseOutputTypeDef,
+    AdminInitiateAuthResponseOutputTypeDef,
+    AdminRespondToAuthChallengeResponseOutputTypeDef,
+    InitiateAuthResponseOutputTypeDef,
+    RespondToAuthChallengeResponseOutputTypeDef,
     AdminInitiateAuthRequestRequestTypeDef,
     AdminRespondToAuthChallengeRequestRequestTypeDef,
-    CreateResourceServerResponseTypeDef,
-    DescribeResourceServerResponseTypeDef,
-    ListResourceServersResponseTypeDef,
-    UpdateResourceServerResponseTypeDef,
-    CreateUserPoolClientResponseTypeDef,
-    DescribeUserPoolClientResponseTypeDef,
-    UpdateUserPoolClientResponseTypeDef,
-    DescribeUserPoolDomainResponseTypeDef,
-    GetUserPoolMfaConfigResponseTypeDef,
     SetUserPoolMfaConfigRequestRequestTypeDef,
-    SetUserPoolMfaConfigResponseTypeDef,
-    UserPoolDescriptionTypeTypeDef,
+    DescribeUserPoolDomainResponseOutputTypeDef,
+    UserPoolDescriptionTypeOutputTypeDef,
+    AccountTakeoverRiskConfigurationTypeOutputTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     UpdateUserPoolRequestRequestTypeDef,
+    CreateResourceServerResponseOutputTypeDef,
+    DescribeResourceServerResponseOutputTypeDef,
+    ListResourceServersResponseOutputTypeDef,
+    UpdateResourceServerResponseOutputTypeDef,
+    UserPoolTypeOutputTypeDef,
     AddCustomAttributesRequestRequestTypeDef,
     CreateUserPoolRequestRequestTypeDef,
-    UserPoolTypeTypeDef,
-    ListUserPoolsResponseTypeDef,
-    RiskConfigurationTypeTypeDef,
+    GetUserPoolMfaConfigResponseOutputTypeDef,
+    SetUserPoolMfaConfigResponseOutputTypeDef,
+    CreateUserPoolClientResponseOutputTypeDef,
+    DescribeUserPoolClientResponseOutputTypeDef,
+    UpdateUserPoolClientResponseOutputTypeDef,
+    ListUserPoolsResponseOutputTypeDef,
+    RiskConfigurationTypeOutputTypeDef,
     SetRiskConfigurationRequestRequestTypeDef,
-    CreateUserPoolResponseTypeDef,
-    DescribeUserPoolResponseTypeDef,
-    DescribeRiskConfigurationResponseTypeDef,
-    SetRiskConfigurationResponseTypeDef,
+    CreateUserPoolResponseOutputTypeDef,
+    DescribeUserPoolResponseOutputTypeDef,
+    DescribeRiskConfigurationResponseOutputTypeDef,
+    SetRiskConfigurationResponseOutputTypeDef,
 )
 
 
-def get_structure() -> RecoveryOptionTypeTypeDef:
+def get_structure() -> RecoveryOptionTypeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-idp-1.28.3/README.md` & `mypy-boto3-cognito-idp-1.28.3.post1/README.md`

 * *Files 16% similar despite different names*

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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,73 +362,83 @@
 ### Typed dictionaries
 
 `mypy_boto3_cognito_idp.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_idp.type_defs import (
+    RecoveryOptionTypeOutputTypeDef,
     RecoveryOptionTypeTypeDef,
+    AccountTakeoverActionTypeOutputTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
+    MessageTemplateTypeOutputTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
     ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
-    MFAOptionTypeTypeDef,
+    AttributeTypeOutputTypeDef,
+    MFAOptionTypeOutputTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
-    GroupTypeTypeDef,
+    GroupTypeOutputTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
+    MFAOptionTypeTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
+    AnalyticsConfigurationTypeOutputTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    ChallengeResponseTypeTypeDef,
-    EventContextDataTypeTypeDef,
-    EventFeedbackTypeTypeDef,
-    EventRiskTypeTypeDef,
-    NewDeviceMetadataTypeTypeDef,
+    ChallengeResponseTypeOutputTypeDef,
+    EventContextDataTypeOutputTypeDef,
+    EventFeedbackTypeOutputTypeDef,
+    EventRiskTypeOutputTypeDef,
+    NewDeviceMetadataTypeOutputTypeDef,
     ChangePasswordRequestRequestTypeDef,
-    CodeDeliveryDetailsTypeTypeDef,
+    CodeDeliveryDetailsTypeOutputTypeDef,
+    CompromisedCredentialsActionsTypeOutputTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    IdentityProviderTypeTypeDef,
+    IdentityProviderTypeOutputTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
-    UserImportJobTypeTypeDef,
+    UserImportJobTypeOutputTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
+    CustomDomainConfigTypeOutputTypeDef,
+    CustomEmailLambdaVersionConfigTypeOutputTypeDef,
     CustomEmailLambdaVersionConfigTypeTypeDef,
+    CustomSMSLambdaVersionConfigTypeOutputTypeDef,
     CustomSMSLambdaVersionConfigTypeTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
     DeleteResourceServerRequestRequestTypeDef,
     DeleteUserAttributesRequestRequestTypeDef,
     DeleteUserPoolClientRequestRequestTypeDef,
     DeleteUserPoolDomainRequestRequestTypeDef,
@@ -437,181 +447,206 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
+    DeviceConfigurationTypeOutputTypeDef,
+    EmailConfigurationTypeOutputTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
     GetUICustomizationRequestRequestTypeDef,
-    UICustomizationTypeTypeDef,
+    UICustomizationTypeOutputTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
-    SoftwareTokenMfaConfigTypeTypeDef,
+    SoftwareTokenMfaConfigTypeOutputTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
-    ProviderDescriptionTypeDef,
+    ProviderDescriptionOutputTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
-    UserPoolClientDescriptionTypeDef,
+    UserPoolClientDescriptionOutputTypeDef,
     ListUserPoolsRequestRequestTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
+    NotifyEmailTypeOutputTypeDef,
     NotifyEmailTypeTypeDef,
+    NumberAttributeConstraintsTypeOutputTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
+    PasswordPolicyTypeOutputTypeDef,
     PasswordPolicyTypeTypeDef,
+    ResourceServerScopeTypeOutputTypeDef,
     RevokeTokenRequestRequestTypeDef,
+    RiskExceptionConfigurationTypeOutputTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
+    StringAttributeConstraintsTypeOutputTypeDef,
     StringAttributeConstraintsTypeTypeDef,
     SetUICustomizationRequestRequestTypeDef,
+    SoftwareTokenMfaConfigTypeTypeDef,
+    SmsConfigurationTypeOutputTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    TokenValidityUnitsTypeOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
+    UserAttributeUpdateSettingsTypeOutputTypeDef,
+    UserPoolAddOnsTypeOutputTypeDef,
+    UsernameConfigurationTypeOutputTypeDef,
+    VerificationMessageTemplateTypeOutputTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
+    AccountRecoverySettingTypeOutputTypeDef,
     AccountRecoverySettingTypeTypeDef,
+    AccountTakeoverActionsTypeOutputTypeDef,
     AccountTakeoverActionsTypeTypeDef,
+    AdminCreateUserConfigTypeOutputTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
-    DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
-    ConfirmDeviceResponseTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
+    AssociateSoftwareTokenResponseOutputTypeDef,
+    ConfirmDeviceResponseOutputTypeDef,
+    CreateUserPoolDomainResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetCSVHeaderResponseTypeDef,
-    GetSigningCertificateResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
+    GetCSVHeaderResponseOutputTypeDef,
+    GetSigningCertificateResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    UpdateUserPoolDomainResponseOutputTypeDef,
+    VerifySoftwareTokenResponseOutputTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
-    AdminGetUserResponseTypeDef,
-    AdminSetUserSettingsRequestRequestTypeDef,
-    GetUserResponseTypeDef,
-    SetUserSettingsRequestRequestTypeDef,
-    UserTypeTypeDef,
+    DeviceTypeOutputTypeDef,
+    AdminGetUserResponseOutputTypeDef,
+    GetUserResponseOutputTypeDef,
+    UserTypeOutputTypeDef,
     AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
     AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
-    AdminListGroupsForUserResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    GetGroupResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    UpdateGroupResponseTypeDef,
+    AdminListGroupsForUserResponseOutputTypeDef,
+    CreateGroupResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
+    UpdateGroupResponseOutputTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
-    AuthEventTypeTypeDef,
-    AuthenticationResultTypeTypeDef,
-    ForgotPasswordResponseTypeDef,
-    GetUserAttributeVerificationCodeResponseTypeDef,
-    ResendConfirmationCodeResponseTypeDef,
-    SignUpResponseTypeDef,
-    UpdateUserAttributesResponseTypeDef,
+    AdminSetUserSettingsRequestRequestTypeDef,
+    SetUserSettingsRequestRequestTypeDef,
+    AuthEventTypeOutputTypeDef,
+    AuthenticationResultTypeOutputTypeDef,
+    ForgotPasswordResponseOutputTypeDef,
+    GetUserAttributeVerificationCodeResponseOutputTypeDef,
+    ResendConfirmationCodeResponseOutputTypeDef,
+    SignUpResponseOutputTypeDef,
+    UpdateUserAttributesResponseOutputTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
     ConfirmDeviceRequestRequestTypeDef,
     ConfirmForgotPasswordRequestRequestTypeDef,
     ConfirmSignUpRequestRequestTypeDef,
     ForgotPasswordRequestRequestTypeDef,
     InitiateAuthRequestRequestTypeDef,
     ResendConfirmationCodeRequestRequestTypeDef,
     RespondToAuthChallengeRequestRequestTypeDef,
     SignUpRequestRequestTypeDef,
     ContextDataTypeTypeDef,
-    CreateIdentityProviderResponseTypeDef,
-    DescribeIdentityProviderResponseTypeDef,
-    GetIdentityProviderByIdentifierResponseTypeDef,
-    UpdateIdentityProviderResponseTypeDef,
+    CreateIdentityProviderResponseOutputTypeDef,
+    DescribeIdentityProviderResponseOutputTypeDef,
+    GetIdentityProviderByIdentifierResponseOutputTypeDef,
+    UpdateIdentityProviderResponseOutputTypeDef,
     CreateResourceServerRequestRequestTypeDef,
-    ResourceServerTypeTypeDef,
     UpdateResourceServerRequestRequestTypeDef,
-    CreateUserImportJobResponseTypeDef,
-    DescribeUserImportJobResponseTypeDef,
-    ListUserImportJobsResponseTypeDef,
-    StartUserImportJobResponseTypeDef,
-    StopUserImportJobResponseTypeDef,
+    CreateUserImportJobResponseOutputTypeDef,
+    DescribeUserImportJobResponseOutputTypeDef,
+    ListUserImportJobsResponseOutputTypeDef,
+    StartUserImportJobResponseOutputTypeDef,
+    StopUserImportJobResponseOutputTypeDef,
     CreateUserPoolClientRequestRequestTypeDef,
     UpdateUserPoolClientRequestRequestTypeDef,
-    UserPoolClientTypeTypeDef,
     CreateUserPoolDomainRequestRequestTypeDef,
-    DomainDescriptionTypeTypeDef,
     UpdateUserPoolDomainRequestRequestTypeDef,
     SmsMfaConfigTypeTypeDef,
+    DomainDescriptionTypeOutputTypeDef,
+    LambdaConfigTypeOutputTypeDef,
     LambdaConfigTypeTypeDef,
-    GetUICustomizationResponseTypeDef,
-    SetUICustomizationResponseTypeDef,
-    ListIdentityProvidersResponseTypeDef,
-    ListUserPoolClientsResponseTypeDef,
+    GetUICustomizationResponseOutputTypeDef,
+    SetUICustomizationResponseOutputTypeDef,
+    ListIdentityProvidersResponseOutputTypeDef,
+    ListUserPoolClientsResponseOutputTypeDef,
+    NotifyConfigurationTypeOutputTypeDef,
     NotifyConfigurationTypeTypeDef,
+    UserPoolPolicyTypeOutputTypeDef,
     UserPoolPolicyTypeTypeDef,
+    ResourceServerTypeOutputTypeDef,
+    SchemaAttributeTypeOutputTypeDef,
     SchemaAttributeTypeTypeDef,
-    AdminGetDeviceResponseTypeDef,
-    AdminListDevicesResponseTypeDef,
-    GetDeviceResponseTypeDef,
-    ListDevicesResponseTypeDef,
-    AdminCreateUserResponseTypeDef,
-    ListUsersInGroupResponseTypeDef,
-    ListUsersResponseTypeDef,
-    AdminListUserAuthEventsResponseTypeDef,
-    AdminInitiateAuthResponseTypeDef,
-    AdminRespondToAuthChallengeResponseTypeDef,
-    InitiateAuthResponseTypeDef,
-    RespondToAuthChallengeResponseTypeDef,
+    SmsMfaConfigTypeOutputTypeDef,
+    UserPoolClientTypeOutputTypeDef,
+    AdminGetDeviceResponseOutputTypeDef,
+    AdminListDevicesResponseOutputTypeDef,
+    GetDeviceResponseOutputTypeDef,
+    ListDevicesResponseOutputTypeDef,
+    AdminCreateUserResponseOutputTypeDef,
+    ListUsersInGroupResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
+    AdminListUserAuthEventsResponseOutputTypeDef,
+    AdminInitiateAuthResponseOutputTypeDef,
+    AdminRespondToAuthChallengeResponseOutputTypeDef,
+    InitiateAuthResponseOutputTypeDef,
+    RespondToAuthChallengeResponseOutputTypeDef,
     AdminInitiateAuthRequestRequestTypeDef,
     AdminRespondToAuthChallengeRequestRequestTypeDef,
-    CreateResourceServerResponseTypeDef,
-    DescribeResourceServerResponseTypeDef,
-    ListResourceServersResponseTypeDef,
-    UpdateResourceServerResponseTypeDef,
-    CreateUserPoolClientResponseTypeDef,
-    DescribeUserPoolClientResponseTypeDef,
-    UpdateUserPoolClientResponseTypeDef,
-    DescribeUserPoolDomainResponseTypeDef,
-    GetUserPoolMfaConfigResponseTypeDef,
     SetUserPoolMfaConfigRequestRequestTypeDef,
-    SetUserPoolMfaConfigResponseTypeDef,
-    UserPoolDescriptionTypeTypeDef,
+    DescribeUserPoolDomainResponseOutputTypeDef,
+    UserPoolDescriptionTypeOutputTypeDef,
+    AccountTakeoverRiskConfigurationTypeOutputTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     UpdateUserPoolRequestRequestTypeDef,
+    CreateResourceServerResponseOutputTypeDef,
+    DescribeResourceServerResponseOutputTypeDef,
+    ListResourceServersResponseOutputTypeDef,
+    UpdateResourceServerResponseOutputTypeDef,
+    UserPoolTypeOutputTypeDef,
     AddCustomAttributesRequestRequestTypeDef,
     CreateUserPoolRequestRequestTypeDef,
-    UserPoolTypeTypeDef,
-    ListUserPoolsResponseTypeDef,
-    RiskConfigurationTypeTypeDef,
+    GetUserPoolMfaConfigResponseOutputTypeDef,
+    SetUserPoolMfaConfigResponseOutputTypeDef,
+    CreateUserPoolClientResponseOutputTypeDef,
+    DescribeUserPoolClientResponseOutputTypeDef,
+    UpdateUserPoolClientResponseOutputTypeDef,
+    ListUserPoolsResponseOutputTypeDef,
+    RiskConfigurationTypeOutputTypeDef,
     SetRiskConfigurationRequestRequestTypeDef,
-    CreateUserPoolResponseTypeDef,
-    DescribeUserPoolResponseTypeDef,
-    DescribeRiskConfigurationResponseTypeDef,
-    SetRiskConfigurationResponseTypeDef,
+    CreateUserPoolResponseOutputTypeDef,
+    DescribeUserPoolResponseOutputTypeDef,
+    DescribeRiskConfigurationResponseOutputTypeDef,
+    SetRiskConfigurationResponseOutputTypeDef,
 )
 
 
-def get_structure() -> RecoveryOptionTypeTypeDef:
+def get_structure() -> RecoveryOptionTypeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__init__.py` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__init__.pyi` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__main__.py` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.CognitoIdentityProvider 1.28.3\nVersion:        "
-        " 1.28.3\nBuilder version: 7.14.6\nDocs:           "
+        " 1.28.3.post1\nBuilder version: 7.14.7\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider\nOther"
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

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/client.py` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,102 +47,102 @@
     ListUsersInGroupPaginator,
     ListUsersPaginator,
 )
 from .type_defs import (
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
-    AdminCreateUserResponseTypeDef,
-    AdminGetDeviceResponseTypeDef,
-    AdminGetUserResponseTypeDef,
-    AdminInitiateAuthResponseTypeDef,
-    AdminListDevicesResponseTypeDef,
-    AdminListGroupsForUserResponseTypeDef,
-    AdminListUserAuthEventsResponseTypeDef,
-    AdminRespondToAuthChallengeResponseTypeDef,
+    AdminCreateUserResponseOutputTypeDef,
+    AdminGetDeviceResponseOutputTypeDef,
+    AdminGetUserResponseOutputTypeDef,
+    AdminInitiateAuthResponseOutputTypeDef,
+    AdminListDevicesResponseOutputTypeDef,
+    AdminListGroupsForUserResponseOutputTypeDef,
+    AdminListUserAuthEventsResponseOutputTypeDef,
+    AdminRespondToAuthChallengeResponseOutputTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
+    AssociateSoftwareTokenResponseOutputTypeDef,
     AttributeTypeTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
-    ConfirmDeviceResponseTypeDef,
+    ConfirmDeviceResponseOutputTypeDef,
     ContextDataTypeTypeDef,
-    CreateGroupResponseTypeDef,
-    CreateIdentityProviderResponseTypeDef,
-    CreateResourceServerResponseTypeDef,
-    CreateUserImportJobResponseTypeDef,
-    CreateUserPoolClientResponseTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
-    CreateUserPoolResponseTypeDef,
+    CreateGroupResponseOutputTypeDef,
+    CreateIdentityProviderResponseOutputTypeDef,
+    CreateResourceServerResponseOutputTypeDef,
+    CreateUserImportJobResponseOutputTypeDef,
+    CreateUserPoolClientResponseOutputTypeDef,
+    CreateUserPoolDomainResponseOutputTypeDef,
+    CreateUserPoolResponseOutputTypeDef,
     CustomDomainConfigTypeTypeDef,
-    DescribeIdentityProviderResponseTypeDef,
-    DescribeResourceServerResponseTypeDef,
-    DescribeRiskConfigurationResponseTypeDef,
-    DescribeUserImportJobResponseTypeDef,
-    DescribeUserPoolClientResponseTypeDef,
-    DescribeUserPoolDomainResponseTypeDef,
-    DescribeUserPoolResponseTypeDef,
+    DescribeIdentityProviderResponseOutputTypeDef,
+    DescribeResourceServerResponseOutputTypeDef,
+    DescribeRiskConfigurationResponseOutputTypeDef,
+    DescribeUserImportJobResponseOutputTypeDef,
+    DescribeUserPoolClientResponseOutputTypeDef,
+    DescribeUserPoolDomainResponseOutputTypeDef,
+    DescribeUserPoolResponseOutputTypeDef,
     DeviceConfigurationTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     EmptyResponseMetadataTypeDef,
-    ForgotPasswordResponseTypeDef,
-    GetCSVHeaderResponseTypeDef,
-    GetDeviceResponseTypeDef,
-    GetGroupResponseTypeDef,
-    GetIdentityProviderByIdentifierResponseTypeDef,
-    GetSigningCertificateResponseTypeDef,
-    GetUICustomizationResponseTypeDef,
-    GetUserAttributeVerificationCodeResponseTypeDef,
-    GetUserPoolMfaConfigResponseTypeDef,
-    GetUserResponseTypeDef,
-    InitiateAuthResponseTypeDef,
+    ForgotPasswordResponseOutputTypeDef,
+    GetCSVHeaderResponseOutputTypeDef,
+    GetDeviceResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    GetIdentityProviderByIdentifierResponseOutputTypeDef,
+    GetSigningCertificateResponseOutputTypeDef,
+    GetUICustomizationResponseOutputTypeDef,
+    GetUserAttributeVerificationCodeResponseOutputTypeDef,
+    GetUserPoolMfaConfigResponseOutputTypeDef,
+    GetUserResponseOutputTypeDef,
+    InitiateAuthResponseOutputTypeDef,
     LambdaConfigTypeTypeDef,
-    ListDevicesResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    ListIdentityProvidersResponseTypeDef,
-    ListResourceServersResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUserImportJobsResponseTypeDef,
-    ListUserPoolClientsResponseTypeDef,
-    ListUserPoolsResponseTypeDef,
-    ListUsersInGroupResponseTypeDef,
-    ListUsersResponseTypeDef,
+    ListDevicesResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
+    ListIdentityProvidersResponseOutputTypeDef,
+    ListResourceServersResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListUserImportJobsResponseOutputTypeDef,
+    ListUserPoolClientsResponseOutputTypeDef,
+    ListUserPoolsResponseOutputTypeDef,
+    ListUsersInGroupResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
     MFAOptionTypeTypeDef,
     ProviderUserIdentifierTypeTypeDef,
-    ResendConfirmationCodeResponseTypeDef,
+    ResendConfirmationCodeResponseOutputTypeDef,
     ResourceServerScopeTypeTypeDef,
-    RespondToAuthChallengeResponseTypeDef,
+    RespondToAuthChallengeResponseOutputTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     SchemaAttributeTypeTypeDef,
-    SetRiskConfigurationResponseTypeDef,
-    SetUICustomizationResponseTypeDef,
-    SetUserPoolMfaConfigResponseTypeDef,
-    SignUpResponseTypeDef,
+    SetRiskConfigurationResponseOutputTypeDef,
+    SetUICustomizationResponseOutputTypeDef,
+    SetUserPoolMfaConfigResponseOutputTypeDef,
+    SignUpResponseOutputTypeDef,
     SmsConfigurationTypeTypeDef,
     SmsMfaConfigTypeTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
-    StartUserImportJobResponseTypeDef,
-    StopUserImportJobResponseTypeDef,
+    StartUserImportJobResponseOutputTypeDef,
+    StopUserImportJobResponseOutputTypeDef,
     TokenValidityUnitsTypeTypeDef,
-    UpdateGroupResponseTypeDef,
-    UpdateIdentityProviderResponseTypeDef,
-    UpdateResourceServerResponseTypeDef,
-    UpdateUserAttributesResponseTypeDef,
-    UpdateUserPoolClientResponseTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
+    UpdateGroupResponseOutputTypeDef,
+    UpdateIdentityProviderResponseOutputTypeDef,
+    UpdateResourceServerResponseOutputTypeDef,
+    UpdateUserAttributesResponseOutputTypeDef,
+    UpdateUserPoolClientResponseOutputTypeDef,
+    UpdateUserPoolDomainResponseOutputTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserContextDataTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
+    VerifySoftwareTokenResponseOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -258,15 +258,15 @@
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         TemporaryPassword: str = ...,
         ForceAliasCreation: bool = ...,
         MessageAction: MessageActionTypeType = ...,
         DesiredDeliveryMediums: Sequence[DeliveryMediumTypeType] = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> AdminCreateUserResponseTypeDef:
+    ) -> AdminCreateUserResponseOutputTypeDef:
         """
         Creates a new user in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_create_user)
         """
 
@@ -323,23 +323,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_forget_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_forget_device)
         """
 
     def admin_get_device(
         self, *, DeviceKey: str, UserPoolId: str, Username: str
-    ) -> AdminGetDeviceResponseTypeDef:
+    ) -> AdminGetDeviceResponseOutputTypeDef:
         """
         Gets the device, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_get_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_get_device)
         """
 
-    def admin_get_user(self, *, UserPoolId: str, Username: str) -> AdminGetUserResponseTypeDef:
+    def admin_get_user(
+        self, *, UserPoolId: str, Username: str
+    ) -> AdminGetUserResponseOutputTypeDef:
         """
         Gets the specified user by user name in a user pool as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_get_user)
         """
 
@@ -349,15 +351,15 @@
         UserPoolId: str,
         ClientId: str,
         AuthFlow: AuthFlowTypeType,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ContextData: ContextDataTypeTypeDef = ...
-    ) -> AdminInitiateAuthResponseTypeDef:
+    ) -> AdminInitiateAuthResponseOutputTypeDef:
         """
         Initiates the authentication flow, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_initiate_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_initiate_auth)
         """
 
@@ -375,35 +377,35 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_link_provider_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_link_provider_for_user)
         """
 
     def admin_list_devices(
         self, *, UserPoolId: str, Username: str, Limit: int = ..., PaginationToken: str = ...
-    ) -> AdminListDevicesResponseTypeDef:
+    ) -> AdminListDevicesResponseOutputTypeDef:
         """
         Lists devices, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_devices)
         """
 
     def admin_list_groups_for_user(
         self, *, Username: str, UserPoolId: str, Limit: int = ..., NextToken: str = ...
-    ) -> AdminListGroupsForUserResponseTypeDef:
+    ) -> AdminListGroupsForUserResponseOutputTypeDef:
         """
         Lists the groups that the user belongs to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_groups_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_groups_for_user)
         """
 
     def admin_list_user_auth_events(
         self, *, UserPoolId: str, Username: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> AdminListUserAuthEventsResponseTypeDef:
+    ) -> AdminListUserAuthEventsResponseOutputTypeDef:
         """
         A history of user activity and any risks detected as part of Amazon Cognito
         advanced security.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_user_auth_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_user_auth_events)
         """
@@ -435,15 +437,15 @@
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         ChallengeResponses: Mapping[str, str] = ...,
         Session: str = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ContextData: ContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> AdminRespondToAuthChallengeResponseTypeDef:
+    ) -> AdminRespondToAuthChallengeResponseOutputTypeDef:
         """
         Responds to an authentication challenge, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_respond_to_auth_challenge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_respond_to_auth_challenge)
         """
 
@@ -531,15 +533,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_user_global_sign_out)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_user_global_sign_out)
         """
 
     def associate_software_token(
         self, *, AccessToken: str = ..., Session: str = ...
-    ) -> AssociateSoftwareTokenResponseTypeDef:
+    ) -> AssociateSoftwareTokenResponseOutputTypeDef:
         """
         Begins setup of time-based one-time password (TOTP) multi-factor authentication
         (MFA) for a user, with a unique private key that Amazon Cognito generates and
         returns in the API response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.associate_software_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#associate_software_token)
@@ -574,15 +576,15 @@
     def confirm_device(
         self,
         *,
         AccessToken: str,
         DeviceKey: str,
         DeviceSecretVerifierConfig: DeviceSecretVerifierConfigTypeTypeDef = ...,
         DeviceName: str = ...
-    ) -> ConfirmDeviceResponseTypeDef:
+    ) -> ConfirmDeviceResponseOutputTypeDef:
         """
         Confirms tracking of the device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#confirm_device)
         """
 
@@ -628,15 +630,15 @@
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
         Precedence: int = ...
-    ) -> CreateGroupResponseTypeDef:
+    ) -> CreateGroupResponseOutputTypeDef:
         """
         Creates a new group in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_group)
         """
 
@@ -645,40 +647,40 @@
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderType: IdentityProviderTypeTypeType,
         ProviderDetails: Mapping[str, str],
         AttributeMapping: Mapping[str, str] = ...,
         IdpIdentifiers: Sequence[str] = ...
-    ) -> CreateIdentityProviderResponseTypeDef:
+    ) -> CreateIdentityProviderResponseOutputTypeDef:
         """
         Creates an IdP for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_identity_provider)
         """
 
     def create_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
         Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
-    ) -> CreateResourceServerResponseTypeDef:
+    ) -> CreateResourceServerResponseOutputTypeDef:
         """
         Creates a new OAuth2.0 resource server and defines custom scopes within it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_resource_server)
         """
 
     def create_user_import_job(
         self, *, JobName: str, UserPoolId: str, CloudWatchLogsRoleArn: str
-    ) -> CreateUserImportJobResponseTypeDef:
+    ) -> CreateUserImportJobResponseOutputTypeDef:
         """
         Creates the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_import_job)
         """
 
@@ -704,15 +706,15 @@
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
         AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
-    ) -> CreateUserPoolResponseTypeDef:
+    ) -> CreateUserPoolResponseOutputTypeDef:
         """
         Creates a new Amazon Cognito user pool and sets the password policy for the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool)
         """
@@ -738,29 +740,29 @@
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
         AuthSessionValidity: int = ...
-    ) -> CreateUserPoolClientResponseTypeDef:
+    ) -> CreateUserPoolClientResponseOutputTypeDef:
         """
         Creates the user pool client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool_client)
         """
 
     def create_user_pool_domain(
         self,
         *,
         Domain: str,
         UserPoolId: str,
         CustomDomainConfig: CustomDomainConfigTypeTypeDef = ...
-    ) -> CreateUserPoolDomainResponseTypeDef:
+    ) -> CreateUserPoolDomainResponseOutputTypeDef:
         """
         Creates a new domain for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool_domain)
         """
 
@@ -834,72 +836,74 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#delete_user_pool_domain)
         """
 
     def describe_identity_provider(
         self, *, UserPoolId: str, ProviderName: str
-    ) -> DescribeIdentityProviderResponseTypeDef:
+    ) -> DescribeIdentityProviderResponseOutputTypeDef:
         """
         Gets information about a specific IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_identity_provider)
         """
 
     def describe_resource_server(
         self, *, UserPoolId: str, Identifier: str
-    ) -> DescribeResourceServerResponseTypeDef:
+    ) -> DescribeResourceServerResponseOutputTypeDef:
         """
         Describes a resource server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_resource_server)
         """
 
     def describe_risk_configuration(
         self, *, UserPoolId: str, ClientId: str = ...
-    ) -> DescribeRiskConfigurationResponseTypeDef:
+    ) -> DescribeRiskConfigurationResponseOutputTypeDef:
         """
         Describes the risk configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_risk_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_risk_configuration)
         """
 
     def describe_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> DescribeUserImportJobResponseTypeDef:
+    ) -> DescribeUserImportJobResponseOutputTypeDef:
         """
         Describes the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_import_job)
         """
 
-    def describe_user_pool(self, *, UserPoolId: str) -> DescribeUserPoolResponseTypeDef:
+    def describe_user_pool(self, *, UserPoolId: str) -> DescribeUserPoolResponseOutputTypeDef:
         """
         Returns the configuration information and metadata of the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool)
         """
 
     def describe_user_pool_client(
         self, *, UserPoolId: str, ClientId: str
-    ) -> DescribeUserPoolClientResponseTypeDef:
+    ) -> DescribeUserPoolClientResponseOutputTypeDef:
         """
         Client method for returning the configuration information and metadata of the
         specified user pool app client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool_client)
         """
 
-    def describe_user_pool_domain(self, *, Domain: str) -> DescribeUserPoolDomainResponseTypeDef:
+    def describe_user_pool_domain(
+        self, *, Domain: str
+    ) -> DescribeUserPoolDomainResponseOutputTypeDef:
         """
         Gets information about a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool_domain)
         """
 
@@ -918,15 +922,15 @@
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> ForgotPasswordResponseTypeDef:
+    ) -> ForgotPasswordResponseOutputTypeDef:
         """
         Calling this API causes a message to be sent to the end user with a confirmation
         code that is required to change the user's password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.forgot_password)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#forgot_password)
         """
@@ -941,87 +945,93 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#generate_presigned_url)
         """
 
-    def get_csv_header(self, *, UserPoolId: str) -> GetCSVHeaderResponseTypeDef:
+    def get_csv_header(self, *, UserPoolId: str) -> GetCSVHeaderResponseOutputTypeDef:
         """
         Gets the header information for the comma-separated value (CSV) file to be used
         as input for the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_csv_header)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_csv_header)
         """
 
-    def get_device(self, *, DeviceKey: str, AccessToken: str = ...) -> GetDeviceResponseTypeDef:
+    def get_device(
+        self, *, DeviceKey: str, AccessToken: str = ...
+    ) -> GetDeviceResponseOutputTypeDef:
         """
         Gets the device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_device)
         """
 
-    def get_group(self, *, GroupName: str, UserPoolId: str) -> GetGroupResponseTypeDef:
+    def get_group(self, *, GroupName: str, UserPoolId: str) -> GetGroupResponseOutputTypeDef:
         """
         Gets a group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_group)
         """
 
     def get_identity_provider_by_identifier(
         self, *, UserPoolId: str, IdpIdentifier: str
-    ) -> GetIdentityProviderByIdentifierResponseTypeDef:
+    ) -> GetIdentityProviderByIdentifierResponseOutputTypeDef:
         """
         Gets the specified IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_identity_provider_by_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_identity_provider_by_identifier)
         """
 
-    def get_signing_certificate(self, *, UserPoolId: str) -> GetSigningCertificateResponseTypeDef:
+    def get_signing_certificate(
+        self, *, UserPoolId: str
+    ) -> GetSigningCertificateResponseOutputTypeDef:
         """
         This method takes a user pool ID, and returns the signing certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_signing_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_signing_certificate)
         """
 
     def get_ui_customization(
         self, *, UserPoolId: str, ClientId: str = ...
-    ) -> GetUICustomizationResponseTypeDef:
+    ) -> GetUICustomizationResponseOutputTypeDef:
         """
         Gets the user interface (UI) Customization information for a particular app
         client's app UI, if any such information exists for the client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_ui_customization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_ui_customization)
         """
 
-    def get_user(self, *, AccessToken: str) -> GetUserResponseTypeDef:
+    def get_user(self, *, AccessToken: str) -> GetUserResponseOutputTypeDef:
         """
         Gets the user attributes and metadata for a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user)
         """
 
     def get_user_attribute_verification_code(
         self, *, AccessToken: str, AttributeName: str, ClientMetadata: Mapping[str, str] = ...
-    ) -> GetUserAttributeVerificationCodeResponseTypeDef:
+    ) -> GetUserAttributeVerificationCodeResponseOutputTypeDef:
         """
         Generates a user attribute verification code for the specified attribute name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user_attribute_verification_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user_attribute_verification_code)
         """
 
-    def get_user_pool_mfa_config(self, *, UserPoolId: str) -> GetUserPoolMfaConfigResponseTypeDef:
+    def get_user_pool_mfa_config(
+        self, *, UserPoolId: str
+    ) -> GetUserPoolMfaConfigResponseOutputTypeDef:
         """
         Gets the user pool multi-factor authentication (MFA) configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user_pool_mfa_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user_pool_mfa_config)
         """
 
@@ -1038,94 +1048,96 @@
         *,
         AuthFlow: AuthFlowTypeType,
         ClientId: str,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...
-    ) -> InitiateAuthResponseTypeDef:
+    ) -> InitiateAuthResponseOutputTypeDef:
         """
         Initiates sign-in for a user in the Amazon Cognito user directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.initiate_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#initiate_auth)
         """
 
     def list_devices(
         self, *, AccessToken: str, Limit: int = ..., PaginationToken: str = ...
-    ) -> ListDevicesResponseTypeDef:
+    ) -> ListDevicesResponseOutputTypeDef:
         """
         Lists the sign-in devices that Amazon Cognito has registered to the current
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_devices)
         """
 
     def list_groups(
         self, *, UserPoolId: str, Limit: int = ..., NextToken: str = ...
-    ) -> ListGroupsResponseTypeDef:
+    ) -> ListGroupsResponseOutputTypeDef:
         """
         Lists the groups associated with a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_groups)
         """
 
     def list_identity_providers(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListIdentityProvidersResponseTypeDef:
+    ) -> ListIdentityProvidersResponseOutputTypeDef:
         """
         Lists information about all IdPs for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_identity_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_identity_providers)
         """
 
     def list_resource_servers(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListResourceServersResponseTypeDef:
+    ) -> ListResourceServersResponseOutputTypeDef:
         """
         Lists the resource servers for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_resource_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_resource_servers)
         """
 
-    def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
+    def list_tags_for_resource(
+        self, *, ResourceArn: str
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Lists the tags that are assigned to an Amazon Cognito user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_tags_for_resource)
         """
 
     def list_user_import_jobs(
         self, *, UserPoolId: str, MaxResults: int, PaginationToken: str = ...
-    ) -> ListUserImportJobsResponseTypeDef:
+    ) -> ListUserImportJobsResponseOutputTypeDef:
         """
         Lists the user import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_import_jobs)
         """
 
     def list_user_pool_clients(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListUserPoolClientsResponseTypeDef:
+    ) -> ListUserPoolClientsResponseOutputTypeDef:
         """
         Lists the clients that have been created for the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_pool_clients)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_pool_clients)
         """
 
     def list_user_pools(
         self, *, MaxResults: int, NextToken: str = ...
-    ) -> ListUserPoolsResponseTypeDef:
+    ) -> ListUserPoolsResponseOutputTypeDef:
         """
         Lists the user pools associated with an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_pools)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_pools)
         """
 
@@ -1133,25 +1145,25 @@
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         PaginationToken: str = ...,
         Filter: str = ...
-    ) -> ListUsersResponseTypeDef:
+    ) -> ListUsersResponseOutputTypeDef:
         """
         Lists the users in the Amazon Cognito user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_users)
         """
 
     def list_users_in_group(
         self, *, UserPoolId: str, GroupName: str, Limit: int = ..., NextToken: str = ...
-    ) -> ListUsersInGroupResponseTypeDef:
+    ) -> ListUsersInGroupResponseOutputTypeDef:
         """
         Lists the users in the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users_in_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_users_in_group)
         """
 
@@ -1160,15 +1172,15 @@
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> ResendConfirmationCodeResponseTypeDef:
+    ) -> ResendConfirmationCodeResponseOutputTypeDef:
         """
         Resends the confirmation (for confirmation of registration) to a specific user
         in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.resend_confirmation_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#resend_confirmation_code)
         """
@@ -1179,15 +1191,15 @@
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         Session: str = ...,
         ChallengeResponses: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> RespondToAuthChallengeResponseTypeDef:
+    ) -> RespondToAuthChallengeResponseOutputTypeDef:
         """
         Responds to the authentication challenge.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.respond_to_auth_challenge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#respond_to_auth_challenge)
         """
 
@@ -1204,30 +1216,30 @@
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
         CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
         RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...
-    ) -> SetRiskConfigurationResponseTypeDef:
+    ) -> SetRiskConfigurationResponseOutputTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_risk_configuration)
         """
 
     def set_ui_customization(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
         CSS: str = ...,
         ImageFile: Union[str, bytes, IO[Any], StreamingBody] = ...
-    ) -> SetUICustomizationResponseTypeDef:
+    ) -> SetUICustomizationResponseOutputTypeDef:
         """
         Sets the user interface (UI) customization information for a user pool's built-
         in app UI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_ui_customization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_ui_customization)
         """
@@ -1250,15 +1262,15 @@
     def set_user_pool_mfa_config(
         self,
         *,
         UserPoolId: str,
         SmsMfaConfiguration: SmsMfaConfigTypeTypeDef = ...,
         SoftwareTokenMfaConfiguration: SoftwareTokenMfaConfigTypeTypeDef = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...
-    ) -> SetUserPoolMfaConfigResponseTypeDef:
+    ) -> SetUserPoolMfaConfigResponseOutputTypeDef:
         """
         Sets the user pool multi-factor authentication (MFA) configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_user_pool_mfa_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_user_pool_mfa_config)
         """
 
@@ -1280,36 +1292,36 @@
         Password: str,
         SecretHash: str = ...,
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> SignUpResponseTypeDef:
+    ) -> SignUpResponseOutputTypeDef:
         """
         Registers the user in the specified user pool and creates a user name, password,
         and user attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.sign_up)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#sign_up)
         """
 
     def start_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> StartUserImportJobResponseTypeDef:
+    ) -> StartUserImportJobResponseOutputTypeDef:
         """
         Starts the user import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.start_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#start_user_import_job)
         """
 
     def stop_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> StopUserImportJobResponseTypeDef:
+    ) -> StopUserImportJobResponseOutputTypeDef:
         """
         Stops the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.stop_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#stop_user_import_job)
         """
 
@@ -1364,15 +1376,15 @@
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
         Precedence: int = ...
-    ) -> UpdateGroupResponseTypeDef:
+    ) -> UpdateGroupResponseOutputTypeDef:
         """
         Updates the specified group with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_group)
         """
 
@@ -1380,44 +1392,44 @@
         self,
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderDetails: Mapping[str, str] = ...,
         AttributeMapping: Mapping[str, str] = ...,
         IdpIdentifiers: Sequence[str] = ...
-    ) -> UpdateIdentityProviderResponseTypeDef:
+    ) -> UpdateIdentityProviderResponseOutputTypeDef:
         """
         Updates IdP information for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_identity_provider)
         """
 
     def update_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
         Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
-    ) -> UpdateResourceServerResponseTypeDef:
+    ) -> UpdateResourceServerResponseOutputTypeDef:
         """
         Updates the name and scopes of resource server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_resource_server)
         """
 
     def update_user_attributes(
         self,
         *,
         UserAttributes: Sequence[AttributeTypeTypeDef],
         AccessToken: str,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> UpdateUserAttributesResponseTypeDef:
+    ) -> UpdateUserAttributesResponseOutputTypeDef:
         """
         Allows a user to update a specific attribute (one at a time).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_attributes)
         """
 
@@ -1472,25 +1484,25 @@
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
         AuthSessionValidity: int = ...
-    ) -> UpdateUserPoolClientResponseTypeDef:
+    ) -> UpdateUserPoolClientResponseOutputTypeDef:
         """
         Updates the specified user pool app client with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_pool_client)
         """
 
     def update_user_pool_domain(
         self, *, Domain: str, UserPoolId: str, CustomDomainConfig: CustomDomainConfigTypeTypeDef
-    ) -> UpdateUserPoolDomainResponseTypeDef:
+    ) -> UpdateUserPoolDomainResponseOutputTypeDef:
         """
         Updates the Secure Sockets Layer (SSL) certificate for the custom domain for
         your user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_pool_domain)
         """
@@ -1498,15 +1510,15 @@
     def verify_software_token(
         self,
         *,
         UserCode: str,
         AccessToken: str = ...,
         Session: str = ...,
         FriendlyDeviceName: str = ...
-    ) -> VerifySoftwareTokenResponseTypeDef:
+    ) -> VerifySoftwareTokenResponseOutputTypeDef:
         """
         Use this API to register a user's entered time-based one-time password (TOTP)
         code and mark the user's software token MFA status as "verified" if successful.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.verify_software_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#verify_software_token)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/client.pyi` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -47,102 +47,102 @@
     ListUsersInGroupPaginator,
     ListUsersPaginator,
 )
 from .type_defs import (
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
-    AdminCreateUserResponseTypeDef,
-    AdminGetDeviceResponseTypeDef,
-    AdminGetUserResponseTypeDef,
-    AdminInitiateAuthResponseTypeDef,
-    AdminListDevicesResponseTypeDef,
-    AdminListGroupsForUserResponseTypeDef,
-    AdminListUserAuthEventsResponseTypeDef,
-    AdminRespondToAuthChallengeResponseTypeDef,
+    AdminCreateUserResponseOutputTypeDef,
+    AdminGetDeviceResponseOutputTypeDef,
+    AdminGetUserResponseOutputTypeDef,
+    AdminInitiateAuthResponseOutputTypeDef,
+    AdminListDevicesResponseOutputTypeDef,
+    AdminListGroupsForUserResponseOutputTypeDef,
+    AdminListUserAuthEventsResponseOutputTypeDef,
+    AdminRespondToAuthChallengeResponseOutputTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
+    AssociateSoftwareTokenResponseOutputTypeDef,
     AttributeTypeTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
-    ConfirmDeviceResponseTypeDef,
+    ConfirmDeviceResponseOutputTypeDef,
     ContextDataTypeTypeDef,
-    CreateGroupResponseTypeDef,
-    CreateIdentityProviderResponseTypeDef,
-    CreateResourceServerResponseTypeDef,
-    CreateUserImportJobResponseTypeDef,
-    CreateUserPoolClientResponseTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
-    CreateUserPoolResponseTypeDef,
+    CreateGroupResponseOutputTypeDef,
+    CreateIdentityProviderResponseOutputTypeDef,
+    CreateResourceServerResponseOutputTypeDef,
+    CreateUserImportJobResponseOutputTypeDef,
+    CreateUserPoolClientResponseOutputTypeDef,
+    CreateUserPoolDomainResponseOutputTypeDef,
+    CreateUserPoolResponseOutputTypeDef,
     CustomDomainConfigTypeTypeDef,
-    DescribeIdentityProviderResponseTypeDef,
-    DescribeResourceServerResponseTypeDef,
-    DescribeRiskConfigurationResponseTypeDef,
-    DescribeUserImportJobResponseTypeDef,
-    DescribeUserPoolClientResponseTypeDef,
-    DescribeUserPoolDomainResponseTypeDef,
-    DescribeUserPoolResponseTypeDef,
+    DescribeIdentityProviderResponseOutputTypeDef,
+    DescribeResourceServerResponseOutputTypeDef,
+    DescribeRiskConfigurationResponseOutputTypeDef,
+    DescribeUserImportJobResponseOutputTypeDef,
+    DescribeUserPoolClientResponseOutputTypeDef,
+    DescribeUserPoolDomainResponseOutputTypeDef,
+    DescribeUserPoolResponseOutputTypeDef,
     DeviceConfigurationTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     EmptyResponseMetadataTypeDef,
-    ForgotPasswordResponseTypeDef,
-    GetCSVHeaderResponseTypeDef,
-    GetDeviceResponseTypeDef,
-    GetGroupResponseTypeDef,
-    GetIdentityProviderByIdentifierResponseTypeDef,
-    GetSigningCertificateResponseTypeDef,
-    GetUICustomizationResponseTypeDef,
-    GetUserAttributeVerificationCodeResponseTypeDef,
-    GetUserPoolMfaConfigResponseTypeDef,
-    GetUserResponseTypeDef,
-    InitiateAuthResponseTypeDef,
+    ForgotPasswordResponseOutputTypeDef,
+    GetCSVHeaderResponseOutputTypeDef,
+    GetDeviceResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    GetIdentityProviderByIdentifierResponseOutputTypeDef,
+    GetSigningCertificateResponseOutputTypeDef,
+    GetUICustomizationResponseOutputTypeDef,
+    GetUserAttributeVerificationCodeResponseOutputTypeDef,
+    GetUserPoolMfaConfigResponseOutputTypeDef,
+    GetUserResponseOutputTypeDef,
+    InitiateAuthResponseOutputTypeDef,
     LambdaConfigTypeTypeDef,
-    ListDevicesResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    ListIdentityProvidersResponseTypeDef,
-    ListResourceServersResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUserImportJobsResponseTypeDef,
-    ListUserPoolClientsResponseTypeDef,
-    ListUserPoolsResponseTypeDef,
-    ListUsersInGroupResponseTypeDef,
-    ListUsersResponseTypeDef,
+    ListDevicesResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
+    ListIdentityProvidersResponseOutputTypeDef,
+    ListResourceServersResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListUserImportJobsResponseOutputTypeDef,
+    ListUserPoolClientsResponseOutputTypeDef,
+    ListUserPoolsResponseOutputTypeDef,
+    ListUsersInGroupResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
     MFAOptionTypeTypeDef,
     ProviderUserIdentifierTypeTypeDef,
-    ResendConfirmationCodeResponseTypeDef,
+    ResendConfirmationCodeResponseOutputTypeDef,
     ResourceServerScopeTypeTypeDef,
-    RespondToAuthChallengeResponseTypeDef,
+    RespondToAuthChallengeResponseOutputTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     SchemaAttributeTypeTypeDef,
-    SetRiskConfigurationResponseTypeDef,
-    SetUICustomizationResponseTypeDef,
-    SetUserPoolMfaConfigResponseTypeDef,
-    SignUpResponseTypeDef,
+    SetRiskConfigurationResponseOutputTypeDef,
+    SetUICustomizationResponseOutputTypeDef,
+    SetUserPoolMfaConfigResponseOutputTypeDef,
+    SignUpResponseOutputTypeDef,
     SmsConfigurationTypeTypeDef,
     SmsMfaConfigTypeTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
-    StartUserImportJobResponseTypeDef,
-    StopUserImportJobResponseTypeDef,
+    StartUserImportJobResponseOutputTypeDef,
+    StopUserImportJobResponseOutputTypeDef,
     TokenValidityUnitsTypeTypeDef,
-    UpdateGroupResponseTypeDef,
-    UpdateIdentityProviderResponseTypeDef,
-    UpdateResourceServerResponseTypeDef,
-    UpdateUserAttributesResponseTypeDef,
-    UpdateUserPoolClientResponseTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
+    UpdateGroupResponseOutputTypeDef,
+    UpdateIdentityProviderResponseOutputTypeDef,
+    UpdateResourceServerResponseOutputTypeDef,
+    UpdateUserAttributesResponseOutputTypeDef,
+    UpdateUserPoolClientResponseOutputTypeDef,
+    UpdateUserPoolDomainResponseOutputTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserContextDataTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
+    VerifySoftwareTokenResponseOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -250,15 +250,15 @@
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         TemporaryPassword: str = ...,
         ForceAliasCreation: bool = ...,
         MessageAction: MessageActionTypeType = ...,
         DesiredDeliveryMediums: Sequence[DeliveryMediumTypeType] = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> AdminCreateUserResponseTypeDef:
+    ) -> AdminCreateUserResponseOutputTypeDef:
         """
         Creates a new user in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_create_user)
         """
     def admin_delete_user(self, *, UserPoolId: str, Username: str) -> EmptyResponseMetadataTypeDef:
@@ -308,22 +308,24 @@
         Forgets the device, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_forget_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_forget_device)
         """
     def admin_get_device(
         self, *, DeviceKey: str, UserPoolId: str, Username: str
-    ) -> AdminGetDeviceResponseTypeDef:
+    ) -> AdminGetDeviceResponseOutputTypeDef:
         """
         Gets the device, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_get_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_get_device)
         """
-    def admin_get_user(self, *, UserPoolId: str, Username: str) -> AdminGetUserResponseTypeDef:
+    def admin_get_user(
+        self, *, UserPoolId: str, Username: str
+    ) -> AdminGetUserResponseOutputTypeDef:
         """
         Gets the specified user by user name in a user pool as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_get_user)
         """
     def admin_initiate_auth(
@@ -332,15 +334,15 @@
         UserPoolId: str,
         ClientId: str,
         AuthFlow: AuthFlowTypeType,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ContextData: ContextDataTypeTypeDef = ...
-    ) -> AdminInitiateAuthResponseTypeDef:
+    ) -> AdminInitiateAuthResponseOutputTypeDef:
         """
         Initiates the authentication flow, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_initiate_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_initiate_auth)
         """
     def admin_link_provider_for_user(
@@ -356,33 +358,33 @@
         name and value from the external IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_link_provider_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_link_provider_for_user)
         """
     def admin_list_devices(
         self, *, UserPoolId: str, Username: str, Limit: int = ..., PaginationToken: str = ...
-    ) -> AdminListDevicesResponseTypeDef:
+    ) -> AdminListDevicesResponseOutputTypeDef:
         """
         Lists devices, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_devices)
         """
     def admin_list_groups_for_user(
         self, *, Username: str, UserPoolId: str, Limit: int = ..., NextToken: str = ...
-    ) -> AdminListGroupsForUserResponseTypeDef:
+    ) -> AdminListGroupsForUserResponseOutputTypeDef:
         """
         Lists the groups that the user belongs to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_groups_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_groups_for_user)
         """
     def admin_list_user_auth_events(
         self, *, UserPoolId: str, Username: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> AdminListUserAuthEventsResponseTypeDef:
+    ) -> AdminListUserAuthEventsResponseOutputTypeDef:
         """
         A history of user activity and any risks detected as part of Amazon Cognito
         advanced security.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_user_auth_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_user_auth_events)
         """
@@ -411,15 +413,15 @@
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         ChallengeResponses: Mapping[str, str] = ...,
         Session: str = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ContextData: ContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> AdminRespondToAuthChallengeResponseTypeDef:
+    ) -> AdminRespondToAuthChallengeResponseOutputTypeDef:
         """
         Responds to an authentication challenge, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_respond_to_auth_challenge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_respond_to_auth_challenge)
         """
     def admin_set_user_mfa_preference(
@@ -499,15 +501,15 @@
         Signs out a user from all devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_user_global_sign_out)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_user_global_sign_out)
         """
     def associate_software_token(
         self, *, AccessToken: str = ..., Session: str = ...
-    ) -> AssociateSoftwareTokenResponseTypeDef:
+    ) -> AssociateSoftwareTokenResponseOutputTypeDef:
         """
         Begins setup of time-based one-time password (TOTP) multi-factor authentication
         (MFA) for a user, with a unique private key that Amazon Cognito generates and
         returns in the API response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.associate_software_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#associate_software_token)
@@ -538,15 +540,15 @@
     def confirm_device(
         self,
         *,
         AccessToken: str,
         DeviceKey: str,
         DeviceSecretVerifierConfig: DeviceSecretVerifierConfigTypeTypeDef = ...,
         DeviceName: str = ...
-    ) -> ConfirmDeviceResponseTypeDef:
+    ) -> ConfirmDeviceResponseOutputTypeDef:
         """
         Confirms tracking of the device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#confirm_device)
         """
     def confirm_forgot_password(
@@ -589,15 +591,15 @@
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
         Precedence: int = ...
-    ) -> CreateGroupResponseTypeDef:
+    ) -> CreateGroupResponseOutputTypeDef:
         """
         Creates a new group in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_group)
         """
     def create_identity_provider(
@@ -605,38 +607,38 @@
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderType: IdentityProviderTypeTypeType,
         ProviderDetails: Mapping[str, str],
         AttributeMapping: Mapping[str, str] = ...,
         IdpIdentifiers: Sequence[str] = ...
-    ) -> CreateIdentityProviderResponseTypeDef:
+    ) -> CreateIdentityProviderResponseOutputTypeDef:
         """
         Creates an IdP for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_identity_provider)
         """
     def create_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
         Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
-    ) -> CreateResourceServerResponseTypeDef:
+    ) -> CreateResourceServerResponseOutputTypeDef:
         """
         Creates a new OAuth2.0 resource server and defines custom scopes within it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_resource_server)
         """
     def create_user_import_job(
         self, *, JobName: str, UserPoolId: str, CloudWatchLogsRoleArn: str
-    ) -> CreateUserImportJobResponseTypeDef:
+    ) -> CreateUserImportJobResponseOutputTypeDef:
         """
         Creates the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_import_job)
         """
     def create_user_pool(
@@ -661,15 +663,15 @@
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
         AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
-    ) -> CreateUserPoolResponseTypeDef:
+    ) -> CreateUserPoolResponseOutputTypeDef:
         """
         Creates a new Amazon Cognito user pool and sets the password policy for the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool)
         """
@@ -694,28 +696,28 @@
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
         AuthSessionValidity: int = ...
-    ) -> CreateUserPoolClientResponseTypeDef:
+    ) -> CreateUserPoolClientResponseOutputTypeDef:
         """
         Creates the user pool client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool_client)
         """
     def create_user_pool_domain(
         self,
         *,
         Domain: str,
         UserPoolId: str,
         CustomDomainConfig: CustomDomainConfigTypeTypeDef = ...
-    ) -> CreateUserPoolDomainResponseTypeDef:
+    ) -> CreateUserPoolDomainResponseOutputTypeDef:
         """
         Creates a new domain for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool_domain)
         """
     def delete_group(self, *, GroupName: str, UserPoolId: str) -> EmptyResponseMetadataTypeDef:
@@ -780,66 +782,68 @@
         Deletes a domain for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#delete_user_pool_domain)
         """
     def describe_identity_provider(
         self, *, UserPoolId: str, ProviderName: str
-    ) -> DescribeIdentityProviderResponseTypeDef:
+    ) -> DescribeIdentityProviderResponseOutputTypeDef:
         """
         Gets information about a specific IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_identity_provider)
         """
     def describe_resource_server(
         self, *, UserPoolId: str, Identifier: str
-    ) -> DescribeResourceServerResponseTypeDef:
+    ) -> DescribeResourceServerResponseOutputTypeDef:
         """
         Describes a resource server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_resource_server)
         """
     def describe_risk_configuration(
         self, *, UserPoolId: str, ClientId: str = ...
-    ) -> DescribeRiskConfigurationResponseTypeDef:
+    ) -> DescribeRiskConfigurationResponseOutputTypeDef:
         """
         Describes the risk configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_risk_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_risk_configuration)
         """
     def describe_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> DescribeUserImportJobResponseTypeDef:
+    ) -> DescribeUserImportJobResponseOutputTypeDef:
         """
         Describes the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_import_job)
         """
-    def describe_user_pool(self, *, UserPoolId: str) -> DescribeUserPoolResponseTypeDef:
+    def describe_user_pool(self, *, UserPoolId: str) -> DescribeUserPoolResponseOutputTypeDef:
         """
         Returns the configuration information and metadata of the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool)
         """
     def describe_user_pool_client(
         self, *, UserPoolId: str, ClientId: str
-    ) -> DescribeUserPoolClientResponseTypeDef:
+    ) -> DescribeUserPoolClientResponseOutputTypeDef:
         """
         Client method for returning the configuration information and metadata of the
         specified user pool app client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool_client)
         """
-    def describe_user_pool_domain(self, *, Domain: str) -> DescribeUserPoolDomainResponseTypeDef:
+    def describe_user_pool_domain(
+        self, *, Domain: str
+    ) -> DescribeUserPoolDomainResponseOutputTypeDef:
         """
         Gets information about a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool_domain)
         """
     def forget_device(
@@ -856,15 +860,15 @@
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> ForgotPasswordResponseTypeDef:
+    ) -> ForgotPasswordResponseOutputTypeDef:
         """
         Calling this API causes a message to be sent to the end user with a confirmation
         code that is required to change the user's password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.forgot_password)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#forgot_password)
         """
@@ -877,79 +881,85 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#generate_presigned_url)
         """
-    def get_csv_header(self, *, UserPoolId: str) -> GetCSVHeaderResponseTypeDef:
+    def get_csv_header(self, *, UserPoolId: str) -> GetCSVHeaderResponseOutputTypeDef:
         """
         Gets the header information for the comma-separated value (CSV) file to be used
         as input for the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_csv_header)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_csv_header)
         """
-    def get_device(self, *, DeviceKey: str, AccessToken: str = ...) -> GetDeviceResponseTypeDef:
+    def get_device(
+        self, *, DeviceKey: str, AccessToken: str = ...
+    ) -> GetDeviceResponseOutputTypeDef:
         """
         Gets the device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_device)
         """
-    def get_group(self, *, GroupName: str, UserPoolId: str) -> GetGroupResponseTypeDef:
+    def get_group(self, *, GroupName: str, UserPoolId: str) -> GetGroupResponseOutputTypeDef:
         """
         Gets a group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_group)
         """
     def get_identity_provider_by_identifier(
         self, *, UserPoolId: str, IdpIdentifier: str
-    ) -> GetIdentityProviderByIdentifierResponseTypeDef:
+    ) -> GetIdentityProviderByIdentifierResponseOutputTypeDef:
         """
         Gets the specified IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_identity_provider_by_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_identity_provider_by_identifier)
         """
-    def get_signing_certificate(self, *, UserPoolId: str) -> GetSigningCertificateResponseTypeDef:
+    def get_signing_certificate(
+        self, *, UserPoolId: str
+    ) -> GetSigningCertificateResponseOutputTypeDef:
         """
         This method takes a user pool ID, and returns the signing certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_signing_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_signing_certificate)
         """
     def get_ui_customization(
         self, *, UserPoolId: str, ClientId: str = ...
-    ) -> GetUICustomizationResponseTypeDef:
+    ) -> GetUICustomizationResponseOutputTypeDef:
         """
         Gets the user interface (UI) Customization information for a particular app
         client's app UI, if any such information exists for the client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_ui_customization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_ui_customization)
         """
-    def get_user(self, *, AccessToken: str) -> GetUserResponseTypeDef:
+    def get_user(self, *, AccessToken: str) -> GetUserResponseOutputTypeDef:
         """
         Gets the user attributes and metadata for a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user)
         """
     def get_user_attribute_verification_code(
         self, *, AccessToken: str, AttributeName: str, ClientMetadata: Mapping[str, str] = ...
-    ) -> GetUserAttributeVerificationCodeResponseTypeDef:
+    ) -> GetUserAttributeVerificationCodeResponseOutputTypeDef:
         """
         Generates a user attribute verification code for the specified attribute name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user_attribute_verification_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user_attribute_verification_code)
         """
-    def get_user_pool_mfa_config(self, *, UserPoolId: str) -> GetUserPoolMfaConfigResponseTypeDef:
+    def get_user_pool_mfa_config(
+        self, *, UserPoolId: str
+    ) -> GetUserPoolMfaConfigResponseOutputTypeDef:
         """
         Gets the user pool multi-factor authentication (MFA) configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user_pool_mfa_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user_pool_mfa_config)
         """
     def global_sign_out(self, *, AccessToken: str) -> Dict[str, Any]:
@@ -964,110 +974,112 @@
         *,
         AuthFlow: AuthFlowTypeType,
         ClientId: str,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...
-    ) -> InitiateAuthResponseTypeDef:
+    ) -> InitiateAuthResponseOutputTypeDef:
         """
         Initiates sign-in for a user in the Amazon Cognito user directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.initiate_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#initiate_auth)
         """
     def list_devices(
         self, *, AccessToken: str, Limit: int = ..., PaginationToken: str = ...
-    ) -> ListDevicesResponseTypeDef:
+    ) -> ListDevicesResponseOutputTypeDef:
         """
         Lists the sign-in devices that Amazon Cognito has registered to the current
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_devices)
         """
     def list_groups(
         self, *, UserPoolId: str, Limit: int = ..., NextToken: str = ...
-    ) -> ListGroupsResponseTypeDef:
+    ) -> ListGroupsResponseOutputTypeDef:
         """
         Lists the groups associated with a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_groups)
         """
     def list_identity_providers(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListIdentityProvidersResponseTypeDef:
+    ) -> ListIdentityProvidersResponseOutputTypeDef:
         """
         Lists information about all IdPs for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_identity_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_identity_providers)
         """
     def list_resource_servers(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListResourceServersResponseTypeDef:
+    ) -> ListResourceServersResponseOutputTypeDef:
         """
         Lists the resource servers for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_resource_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_resource_servers)
         """
-    def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
+    def list_tags_for_resource(
+        self, *, ResourceArn: str
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Lists the tags that are assigned to an Amazon Cognito user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_tags_for_resource)
         """
     def list_user_import_jobs(
         self, *, UserPoolId: str, MaxResults: int, PaginationToken: str = ...
-    ) -> ListUserImportJobsResponseTypeDef:
+    ) -> ListUserImportJobsResponseOutputTypeDef:
         """
         Lists the user import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_import_jobs)
         """
     def list_user_pool_clients(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListUserPoolClientsResponseTypeDef:
+    ) -> ListUserPoolClientsResponseOutputTypeDef:
         """
         Lists the clients that have been created for the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_pool_clients)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_pool_clients)
         """
     def list_user_pools(
         self, *, MaxResults: int, NextToken: str = ...
-    ) -> ListUserPoolsResponseTypeDef:
+    ) -> ListUserPoolsResponseOutputTypeDef:
         """
         Lists the user pools associated with an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_pools)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_pools)
         """
     def list_users(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         PaginationToken: str = ...,
         Filter: str = ...
-    ) -> ListUsersResponseTypeDef:
+    ) -> ListUsersResponseOutputTypeDef:
         """
         Lists the users in the Amazon Cognito user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_users)
         """
     def list_users_in_group(
         self, *, UserPoolId: str, GroupName: str, Limit: int = ..., NextToken: str = ...
-    ) -> ListUsersInGroupResponseTypeDef:
+    ) -> ListUsersInGroupResponseOutputTypeDef:
         """
         Lists the users in the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users_in_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_users_in_group)
         """
     def resend_confirmation_code(
@@ -1075,15 +1087,15 @@
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> ResendConfirmationCodeResponseTypeDef:
+    ) -> ResendConfirmationCodeResponseOutputTypeDef:
         """
         Resends the confirmation (for confirmation of registration) to a specific user
         in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.resend_confirmation_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#resend_confirmation_code)
         """
@@ -1093,15 +1105,15 @@
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         Session: str = ...,
         ChallengeResponses: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> RespondToAuthChallengeResponseTypeDef:
+    ) -> RespondToAuthChallengeResponseOutputTypeDef:
         """
         Responds to the authentication challenge.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.respond_to_auth_challenge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#respond_to_auth_challenge)
         """
     def revoke_token(self, *, Token: str, ClientId: str, ClientSecret: str = ...) -> Dict[str, Any]:
@@ -1116,29 +1128,29 @@
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
         CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
         RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...
-    ) -> SetRiskConfigurationResponseTypeDef:
+    ) -> SetRiskConfigurationResponseOutputTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_risk_configuration)
         """
     def set_ui_customization(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
         CSS: str = ...,
         ImageFile: Union[str, bytes, IO[Any], StreamingBody] = ...
-    ) -> SetUICustomizationResponseTypeDef:
+    ) -> SetUICustomizationResponseOutputTypeDef:
         """
         Sets the user interface (UI) customization information for a user pool's built-
         in app UI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_ui_customization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_ui_customization)
         """
@@ -1159,15 +1171,15 @@
     def set_user_pool_mfa_config(
         self,
         *,
         UserPoolId: str,
         SmsMfaConfiguration: SmsMfaConfigTypeTypeDef = ...,
         SoftwareTokenMfaConfiguration: SoftwareTokenMfaConfigTypeTypeDef = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...
-    ) -> SetUserPoolMfaConfigResponseTypeDef:
+    ) -> SetUserPoolMfaConfigResponseOutputTypeDef:
         """
         Sets the user pool multi-factor authentication (MFA) configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_user_pool_mfa_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_user_pool_mfa_config)
         """
     def set_user_settings(
@@ -1187,34 +1199,34 @@
         Password: str,
         SecretHash: str = ...,
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> SignUpResponseTypeDef:
+    ) -> SignUpResponseOutputTypeDef:
         """
         Registers the user in the specified user pool and creates a user name, password,
         and user attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.sign_up)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#sign_up)
         """
     def start_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> StartUserImportJobResponseTypeDef:
+    ) -> StartUserImportJobResponseOutputTypeDef:
         """
         Starts the user import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.start_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#start_user_import_job)
         """
     def stop_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> StopUserImportJobResponseTypeDef:
+    ) -> StopUserImportJobResponseOutputTypeDef:
         """
         Stops the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.stop_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#stop_user_import_job)
         """
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
@@ -1264,57 +1276,57 @@
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
         Precedence: int = ...
-    ) -> UpdateGroupResponseTypeDef:
+    ) -> UpdateGroupResponseOutputTypeDef:
         """
         Updates the specified group with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_group)
         """
     def update_identity_provider(
         self,
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderDetails: Mapping[str, str] = ...,
         AttributeMapping: Mapping[str, str] = ...,
         IdpIdentifiers: Sequence[str] = ...
-    ) -> UpdateIdentityProviderResponseTypeDef:
+    ) -> UpdateIdentityProviderResponseOutputTypeDef:
         """
         Updates IdP information for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_identity_provider)
         """
     def update_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
         Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
-    ) -> UpdateResourceServerResponseTypeDef:
+    ) -> UpdateResourceServerResponseOutputTypeDef:
         """
         Updates the name and scopes of resource server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_resource_server)
         """
     def update_user_attributes(
         self,
         *,
         UserAttributes: Sequence[AttributeTypeTypeDef],
         AccessToken: str,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> UpdateUserAttributesResponseTypeDef:
+    ) -> UpdateUserAttributesResponseOutputTypeDef:
         """
         Allows a user to update a specific attribute (one at a time).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_attributes)
         """
     def update_user_pool(
@@ -1367,39 +1379,39 @@
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
         AuthSessionValidity: int = ...
-    ) -> UpdateUserPoolClientResponseTypeDef:
+    ) -> UpdateUserPoolClientResponseOutputTypeDef:
         """
         Updates the specified user pool app client with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_pool_client)
         """
     def update_user_pool_domain(
         self, *, Domain: str, UserPoolId: str, CustomDomainConfig: CustomDomainConfigTypeTypeDef
-    ) -> UpdateUserPoolDomainResponseTypeDef:
+    ) -> UpdateUserPoolDomainResponseOutputTypeDef:
         """
         Updates the Secure Sockets Layer (SSL) certificate for the custom domain for
         your user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_pool_domain)
         """
     def verify_software_token(
         self,
         *,
         UserCode: str,
         AccessToken: str = ...,
         Session: str = ...,
         FriendlyDeviceName: str = ...
-    ) -> VerifySoftwareTokenResponseTypeDef:
+    ) -> VerifySoftwareTokenResponseOutputTypeDef:
         """
         Use this API to register a user's entered time-based one-time password (TOTP)
         code and mark the user's software token MFA status as "verified" if successful.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.verify_software_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#verify_software_token)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/literals.py` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/literals.pyi` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/paginator.py` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,23 +36,23 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    AdminListGroupsForUserResponseTypeDef,
-    AdminListUserAuthEventsResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    ListIdentityProvidersResponseTypeDef,
-    ListResourceServersResponseTypeDef,
-    ListUserPoolClientsResponseTypeDef,
-    ListUserPoolsResponseTypeDef,
-    ListUsersInGroupResponseTypeDef,
-    ListUsersResponseTypeDef,
+    AdminListGroupsForUserResponseOutputTypeDef,
+    AdminListUserAuthEventsResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
+    ListIdentityProvidersResponseOutputTypeDef,
+    ListResourceServersResponseOutputTypeDef,
+    ListUserPoolClientsResponseOutputTypeDef,
+    ListUserPoolsResponseOutputTypeDef,
+    ListUsersInGroupResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "AdminListGroupsForUserPaginator",
     "AdminListUserAuthEventsPaginator",
     "ListGroupsPaginator",
@@ -79,105 +79,105 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
     """
 
     def paginate(
         self, *, Username: str, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[AdminListGroupsForUserResponseTypeDef]:
+    ) -> _PageIterator[AdminListGroupsForUserResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
         """
 
 
 class AdminListUserAuthEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, Username: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[AdminListUserAuthEventsResponseTypeDef]:
+    ) -> _PageIterator[AdminListUserAuthEventsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
         """
 
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListGroupsResponseTypeDef]:
+    ) -> _PageIterator[ListGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
         """
 
 
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
+    ) -> _PageIterator[ListIdentityProvidersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
         """
 
 
 class ListResourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListResourceServersResponseTypeDef]:
+    ) -> _PageIterator[ListResourceServersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
         """
 
 
 class ListUserPoolClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUserPoolClientsResponseTypeDef]:
+    ) -> _PageIterator[ListUserPoolClientsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
         """
 
 
 class ListUserPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUserPoolsResponseTypeDef]:
+    ) -> _PageIterator[ListUserPoolsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
         """
 
 
 class ListUsersPaginator(Paginator):
@@ -189,27 +189,27 @@
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUsersResponseTypeDef]:
+    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserspaginator)
         """
 
 
 class ListUsersInGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUsersInGroupResponseTypeDef]:
+    ) -> _PageIterator[ListUsersInGroupResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/paginator.pyi` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/paginator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -36,23 +36,23 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    AdminListGroupsForUserResponseTypeDef,
-    AdminListUserAuthEventsResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    ListIdentityProvidersResponseTypeDef,
-    ListResourceServersResponseTypeDef,
-    ListUserPoolClientsResponseTypeDef,
-    ListUserPoolsResponseTypeDef,
-    ListUsersInGroupResponseTypeDef,
-    ListUsersResponseTypeDef,
+    AdminListGroupsForUserResponseOutputTypeDef,
+    AdminListUserAuthEventsResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
+    ListIdentityProvidersResponseOutputTypeDef,
+    ListResourceServersResponseOutputTypeDef,
+    ListUserPoolClientsResponseOutputTypeDef,
+    ListUserPoolsResponseOutputTypeDef,
+    ListUsersInGroupResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "AdminListGroupsForUserPaginator",
     "AdminListUserAuthEventsPaginator",
     "ListGroupsPaginator",
@@ -76,99 +76,99 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
     """
 
     def paginate(
         self, *, Username: str, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[AdminListGroupsForUserResponseTypeDef]:
+    ) -> _PageIterator[AdminListGroupsForUserResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
         """
 
 class AdminListUserAuthEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, Username: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[AdminListUserAuthEventsResponseTypeDef]:
+    ) -> _PageIterator[AdminListUserAuthEventsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
         """
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListGroupsResponseTypeDef]:
+    ) -> _PageIterator[ListGroupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
         """
 
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
+    ) -> _PageIterator[ListIdentityProvidersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
         """
 
 class ListResourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListResourceServersResponseTypeDef]:
+    ) -> _PageIterator[ListResourceServersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
         """
 
 class ListUserPoolClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUserPoolClientsResponseTypeDef]:
+    ) -> _PageIterator[ListUserPoolClientsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
         """
 
 class ListUserPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUserPoolsResponseTypeDef]:
+    ) -> _PageIterator[ListUserPoolsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
         """
 
 class ListUsersPaginator(Paginator):
     """
@@ -179,26 +179,26 @@
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUsersResponseTypeDef]:
+    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserspaginator)
         """
 
 class ListUsersInGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUsersInGroupResponseTypeDef]:
+    ) -> _PageIterator[ListUsersInGroupResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/type_defs.py` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/type_defs.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cognito-idp service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cognito_idp.type_defs import RecoveryOptionTypeTypeDef
+    from mypy_boto3_cognito_idp.type_defs import RecoveryOptionTypeOutputTypeDef
 
-    data: RecoveryOptionTypeTypeDef = {...}
+    data: RecoveryOptionTypeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -62,73 +62,83 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "RecoveryOptionTypeOutputTypeDef",
     "RecoveryOptionTypeTypeDef",
+    "AccountTakeoverActionTypeOutputTypeDef",
     "AccountTakeoverActionTypeTypeDef",
     "AdminAddUserToGroupRequestRequestTypeDef",
     "AdminConfirmSignUpRequestRequestTypeDef",
+    "MessageTemplateTypeOutputTypeDef",
     "MessageTemplateTypeTypeDef",
     "AttributeTypeTypeDef",
     "ResponseMetadataTypeDef",
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     "AdminDeleteUserRequestRequestTypeDef",
     "ProviderUserIdentifierTypeTypeDef",
     "AdminDisableUserRequestRequestTypeDef",
     "AdminEnableUserRequestRequestTypeDef",
     "AdminForgetDeviceRequestRequestTypeDef",
     "AdminGetDeviceRequestRequestTypeDef",
     "AdminGetUserRequestRequestTypeDef",
-    "MFAOptionTypeTypeDef",
+    "AttributeTypeOutputTypeDef",
+    "MFAOptionTypeOutputTypeDef",
     "AnalyticsMetadataTypeTypeDef",
     "AdminListDevicesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "AdminListGroupsForUserRequestRequestTypeDef",
-    "GroupTypeTypeDef",
+    "GroupTypeOutputTypeDef",
     "AdminListUserAuthEventsRequestRequestTypeDef",
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     "AdminResetUserPasswordRequestRequestTypeDef",
     "SMSMfaSettingsTypeTypeDef",
     "SoftwareTokenMfaSettingsTypeTypeDef",
     "AdminSetUserPasswordRequestRequestTypeDef",
+    "MFAOptionTypeTypeDef",
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     "AdminUpdateDeviceStatusRequestRequestTypeDef",
     "AdminUserGlobalSignOutRequestRequestTypeDef",
+    "AnalyticsConfigurationTypeOutputTypeDef",
     "AnalyticsConfigurationTypeTypeDef",
     "AssociateSoftwareTokenRequestRequestTypeDef",
-    "ChallengeResponseTypeTypeDef",
-    "EventContextDataTypeTypeDef",
-    "EventFeedbackTypeTypeDef",
-    "EventRiskTypeTypeDef",
-    "NewDeviceMetadataTypeTypeDef",
+    "ChallengeResponseTypeOutputTypeDef",
+    "EventContextDataTypeOutputTypeDef",
+    "EventFeedbackTypeOutputTypeDef",
+    "EventRiskTypeOutputTypeDef",
+    "NewDeviceMetadataTypeOutputTypeDef",
     "ChangePasswordRequestRequestTypeDef",
-    "CodeDeliveryDetailsTypeTypeDef",
+    "CodeDeliveryDetailsTypeOutputTypeDef",
+    "CompromisedCredentialsActionsTypeOutputTypeDef",
     "CompromisedCredentialsActionsTypeTypeDef",
     "DeviceSecretVerifierConfigTypeTypeDef",
     "UserContextDataTypeTypeDef",
     "HttpHeaderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
-    "IdentityProviderTypeTypeDef",
+    "IdentityProviderTypeOutputTypeDef",
     "ResourceServerScopeTypeTypeDef",
     "CreateUserImportJobRequestRequestTypeDef",
-    "UserImportJobTypeTypeDef",
+    "UserImportJobTypeOutputTypeDef",
     "TokenValidityUnitsTypeTypeDef",
     "CustomDomainConfigTypeTypeDef",
     "DeviceConfigurationTypeTypeDef",
     "EmailConfigurationTypeTypeDef",
     "SmsConfigurationTypeTypeDef",
     "UserAttributeUpdateSettingsTypeTypeDef",
     "UserPoolAddOnsTypeTypeDef",
     "UsernameConfigurationTypeTypeDef",
     "VerificationMessageTemplateTypeTypeDef",
+    "CustomDomainConfigTypeOutputTypeDef",
+    "CustomEmailLambdaVersionConfigTypeOutputTypeDef",
     "CustomEmailLambdaVersionConfigTypeTypeDef",
+    "CustomSMSLambdaVersionConfigTypeOutputTypeDef",
     "CustomSMSLambdaVersionConfigTypeTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteIdentityProviderRequestRequestTypeDef",
     "DeleteResourceServerRequestRequestTypeDef",
     "DeleteUserAttributesRequestRequestTypeDef",
     "DeleteUserPoolClientRequestRequestTypeDef",
     "DeleteUserPoolDomainRequestRequestTypeDef",
@@ -137,187 +147,228 @@
     "DescribeIdentityProviderRequestRequestTypeDef",
     "DescribeResourceServerRequestRequestTypeDef",
     "DescribeRiskConfigurationRequestRequestTypeDef",
     "DescribeUserImportJobRequestRequestTypeDef",
     "DescribeUserPoolClientRequestRequestTypeDef",
     "DescribeUserPoolDomainRequestRequestTypeDef",
     "DescribeUserPoolRequestRequestTypeDef",
+    "DeviceConfigurationTypeOutputTypeDef",
+    "EmailConfigurationTypeOutputTypeDef",
     "ForgetDeviceRequestRequestTypeDef",
     "GetCSVHeaderRequestRequestTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIdentityProviderByIdentifierRequestRequestTypeDef",
     "GetSigningCertificateRequestRequestTypeDef",
     "GetUICustomizationRequestRequestTypeDef",
-    "UICustomizationTypeTypeDef",
+    "UICustomizationTypeOutputTypeDef",
     "GetUserAttributeVerificationCodeRequestRequestTypeDef",
     "GetUserPoolMfaConfigRequestRequestTypeDef",
-    "SoftwareTokenMfaConfigTypeTypeDef",
+    "SoftwareTokenMfaConfigTypeOutputTypeDef",
     "GetUserRequestRequestTypeDef",
     "GlobalSignOutRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
-    "ProviderDescriptionTypeDef",
+    "ProviderDescriptionOutputTypeDef",
     "ListResourceServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUserImportJobsRequestRequestTypeDef",
     "ListUserPoolClientsRequestRequestTypeDef",
-    "UserPoolClientDescriptionTypeDef",
+    "UserPoolClientDescriptionOutputTypeDef",
     "ListUserPoolsRequestRequestTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
+    "NotifyEmailTypeOutputTypeDef",
     "NotifyEmailTypeTypeDef",
+    "NumberAttributeConstraintsTypeOutputTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
+    "PasswordPolicyTypeOutputTypeDef",
     "PasswordPolicyTypeTypeDef",
+    "ResourceServerScopeTypeOutputTypeDef",
     "RevokeTokenRequestRequestTypeDef",
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
+    "StringAttributeConstraintsTypeOutputTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
     "SetUICustomizationRequestRequestTypeDef",
+    "SoftwareTokenMfaConfigTypeTypeDef",
+    "SmsConfigurationTypeOutputTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TokenValidityUnitsTypeOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
+    "UserPoolAddOnsTypeOutputTypeDef",
+    "UsernameConfigurationTypeOutputTypeDef",
+    "VerificationMessageTemplateTypeOutputTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
+    "AccountRecoverySettingTypeOutputTypeDef",
     "AccountRecoverySettingTypeTypeDef",
+    "AccountTakeoverActionsTypeOutputTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
+    "AdminCreateUserConfigTypeOutputTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
-    "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
-    "AssociateSoftwareTokenResponseTypeDef",
-    "ConfirmDeviceResponseTypeDef",
-    "CreateUserPoolDomainResponseTypeDef",
+    "AssociateSoftwareTokenResponseOutputTypeDef",
+    "ConfirmDeviceResponseOutputTypeDef",
+    "CreateUserPoolDomainResponseOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "GetCSVHeaderResponseTypeDef",
-    "GetSigningCertificateResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateUserPoolDomainResponseTypeDef",
-    "VerifySoftwareTokenResponseTypeDef",
+    "GetCSVHeaderResponseOutputTypeDef",
+    "GetSigningCertificateResponseOutputTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
+    "UpdateUserPoolDomainResponseOutputTypeDef",
+    "VerifySoftwareTokenResponseOutputTypeDef",
     "AdminDisableProviderForUserRequestRequestTypeDef",
     "AdminLinkProviderForUserRequestRequestTypeDef",
-    "AdminGetUserResponseTypeDef",
-    "AdminSetUserSettingsRequestRequestTypeDef",
-    "GetUserResponseTypeDef",
-    "SetUserSettingsRequestRequestTypeDef",
-    "UserTypeTypeDef",
+    "DeviceTypeOutputTypeDef",
+    "AdminGetUserResponseOutputTypeDef",
+    "GetUserResponseOutputTypeDef",
+    "UserTypeOutputTypeDef",
     "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListResourceServersRequestListResourceServersPaginateTypeDef",
     "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
     "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
     "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
-    "AdminListGroupsForUserResponseTypeDef",
-    "CreateGroupResponseTypeDef",
-    "GetGroupResponseTypeDef",
-    "ListGroupsResponseTypeDef",
-    "UpdateGroupResponseTypeDef",
+    "AdminListGroupsForUserResponseOutputTypeDef",
+    "CreateGroupResponseOutputTypeDef",
+    "GetGroupResponseOutputTypeDef",
+    "ListGroupsResponseOutputTypeDef",
+    "UpdateGroupResponseOutputTypeDef",
     "AdminSetUserMFAPreferenceRequestRequestTypeDef",
     "SetUserMFAPreferenceRequestRequestTypeDef",
-    "AuthEventTypeTypeDef",
-    "AuthenticationResultTypeTypeDef",
-    "ForgotPasswordResponseTypeDef",
-    "GetUserAttributeVerificationCodeResponseTypeDef",
-    "ResendConfirmationCodeResponseTypeDef",
-    "SignUpResponseTypeDef",
-    "UpdateUserAttributesResponseTypeDef",
+    "AdminSetUserSettingsRequestRequestTypeDef",
+    "SetUserSettingsRequestRequestTypeDef",
+    "AuthEventTypeOutputTypeDef",
+    "AuthenticationResultTypeOutputTypeDef",
+    "ForgotPasswordResponseOutputTypeDef",
+    "GetUserAttributeVerificationCodeResponseOutputTypeDef",
+    "ResendConfirmationCodeResponseOutputTypeDef",
+    "SignUpResponseOutputTypeDef",
+    "UpdateUserAttributesResponseOutputTypeDef",
+    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     "ConfirmDeviceRequestRequestTypeDef",
     "ConfirmForgotPasswordRequestRequestTypeDef",
     "ConfirmSignUpRequestRequestTypeDef",
     "ForgotPasswordRequestRequestTypeDef",
     "InitiateAuthRequestRequestTypeDef",
     "ResendConfirmationCodeRequestRequestTypeDef",
     "RespondToAuthChallengeRequestRequestTypeDef",
     "SignUpRequestRequestTypeDef",
     "ContextDataTypeTypeDef",
-    "CreateIdentityProviderResponseTypeDef",
-    "DescribeIdentityProviderResponseTypeDef",
-    "GetIdentityProviderByIdentifierResponseTypeDef",
-    "UpdateIdentityProviderResponseTypeDef",
+    "CreateIdentityProviderResponseOutputTypeDef",
+    "DescribeIdentityProviderResponseOutputTypeDef",
+    "GetIdentityProviderByIdentifierResponseOutputTypeDef",
+    "UpdateIdentityProviderResponseOutputTypeDef",
     "CreateResourceServerRequestRequestTypeDef",
-    "ResourceServerTypeTypeDef",
     "UpdateResourceServerRequestRequestTypeDef",
-    "CreateUserImportJobResponseTypeDef",
-    "DescribeUserImportJobResponseTypeDef",
-    "ListUserImportJobsResponseTypeDef",
-    "StartUserImportJobResponseTypeDef",
-    "StopUserImportJobResponseTypeDef",
+    "CreateUserImportJobResponseOutputTypeDef",
+    "DescribeUserImportJobResponseOutputTypeDef",
+    "ListUserImportJobsResponseOutputTypeDef",
+    "StartUserImportJobResponseOutputTypeDef",
+    "StopUserImportJobResponseOutputTypeDef",
     "CreateUserPoolClientRequestRequestTypeDef",
     "UpdateUserPoolClientRequestRequestTypeDef",
-    "UserPoolClientTypeTypeDef",
     "CreateUserPoolDomainRequestRequestTypeDef",
-    "DomainDescriptionTypeTypeDef",
     "UpdateUserPoolDomainRequestRequestTypeDef",
     "SmsMfaConfigTypeTypeDef",
+    "DomainDescriptionTypeOutputTypeDef",
+    "LambdaConfigTypeOutputTypeDef",
     "LambdaConfigTypeTypeDef",
-    "GetUICustomizationResponseTypeDef",
-    "SetUICustomizationResponseTypeDef",
-    "ListIdentityProvidersResponseTypeDef",
-    "ListUserPoolClientsResponseTypeDef",
+    "GetUICustomizationResponseOutputTypeDef",
+    "SetUICustomizationResponseOutputTypeDef",
+    "ListIdentityProvidersResponseOutputTypeDef",
+    "ListUserPoolClientsResponseOutputTypeDef",
+    "NotifyConfigurationTypeOutputTypeDef",
     "NotifyConfigurationTypeTypeDef",
+    "UserPoolPolicyTypeOutputTypeDef",
     "UserPoolPolicyTypeTypeDef",
+    "ResourceServerTypeOutputTypeDef",
+    "SchemaAttributeTypeOutputTypeDef",
     "SchemaAttributeTypeTypeDef",
-    "AdminGetDeviceResponseTypeDef",
-    "AdminListDevicesResponseTypeDef",
-    "GetDeviceResponseTypeDef",
-    "ListDevicesResponseTypeDef",
-    "AdminCreateUserResponseTypeDef",
-    "ListUsersInGroupResponseTypeDef",
-    "ListUsersResponseTypeDef",
-    "AdminListUserAuthEventsResponseTypeDef",
-    "AdminInitiateAuthResponseTypeDef",
-    "AdminRespondToAuthChallengeResponseTypeDef",
-    "InitiateAuthResponseTypeDef",
-    "RespondToAuthChallengeResponseTypeDef",
+    "SmsMfaConfigTypeOutputTypeDef",
+    "UserPoolClientTypeOutputTypeDef",
+    "AdminGetDeviceResponseOutputTypeDef",
+    "AdminListDevicesResponseOutputTypeDef",
+    "GetDeviceResponseOutputTypeDef",
+    "ListDevicesResponseOutputTypeDef",
+    "AdminCreateUserResponseOutputTypeDef",
+    "ListUsersInGroupResponseOutputTypeDef",
+    "ListUsersResponseOutputTypeDef",
+    "AdminListUserAuthEventsResponseOutputTypeDef",
+    "AdminInitiateAuthResponseOutputTypeDef",
+    "AdminRespondToAuthChallengeResponseOutputTypeDef",
+    "InitiateAuthResponseOutputTypeDef",
+    "RespondToAuthChallengeResponseOutputTypeDef",
     "AdminInitiateAuthRequestRequestTypeDef",
     "AdminRespondToAuthChallengeRequestRequestTypeDef",
-    "CreateResourceServerResponseTypeDef",
-    "DescribeResourceServerResponseTypeDef",
-    "ListResourceServersResponseTypeDef",
-    "UpdateResourceServerResponseTypeDef",
-    "CreateUserPoolClientResponseTypeDef",
-    "DescribeUserPoolClientResponseTypeDef",
-    "UpdateUserPoolClientResponseTypeDef",
-    "DescribeUserPoolDomainResponseTypeDef",
-    "GetUserPoolMfaConfigResponseTypeDef",
     "SetUserPoolMfaConfigRequestRequestTypeDef",
-    "SetUserPoolMfaConfigResponseTypeDef",
-    "UserPoolDescriptionTypeTypeDef",
+    "DescribeUserPoolDomainResponseOutputTypeDef",
+    "UserPoolDescriptionTypeOutputTypeDef",
+    "AccountTakeoverRiskConfigurationTypeOutputTypeDef",
     "AccountTakeoverRiskConfigurationTypeTypeDef",
     "UpdateUserPoolRequestRequestTypeDef",
+    "CreateResourceServerResponseOutputTypeDef",
+    "DescribeResourceServerResponseOutputTypeDef",
+    "ListResourceServersResponseOutputTypeDef",
+    "UpdateResourceServerResponseOutputTypeDef",
+    "UserPoolTypeOutputTypeDef",
     "AddCustomAttributesRequestRequestTypeDef",
     "CreateUserPoolRequestRequestTypeDef",
-    "UserPoolTypeTypeDef",
-    "ListUserPoolsResponseTypeDef",
-    "RiskConfigurationTypeTypeDef",
+    "GetUserPoolMfaConfigResponseOutputTypeDef",
+    "SetUserPoolMfaConfigResponseOutputTypeDef",
+    "CreateUserPoolClientResponseOutputTypeDef",
+    "DescribeUserPoolClientResponseOutputTypeDef",
+    "UpdateUserPoolClientResponseOutputTypeDef",
+    "ListUserPoolsResponseOutputTypeDef",
+    "RiskConfigurationTypeOutputTypeDef",
     "SetRiskConfigurationRequestRequestTypeDef",
-    "CreateUserPoolResponseTypeDef",
-    "DescribeUserPoolResponseTypeDef",
-    "DescribeRiskConfigurationResponseTypeDef",
-    "SetRiskConfigurationResponseTypeDef",
+    "CreateUserPoolResponseOutputTypeDef",
+    "DescribeUserPoolResponseOutputTypeDef",
+    "DescribeRiskConfigurationResponseOutputTypeDef",
+    "SetRiskConfigurationResponseOutputTypeDef",
+)
+
+RecoveryOptionTypeOutputTypeDef = TypedDict(
+    "RecoveryOptionTypeOutputTypeDef",
+    {
+        "Priority": int,
+        "Name": RecoveryOptionNameTypeType,
+    },
 )
 
 RecoveryOptionTypeTypeDef = TypedDict(
     "RecoveryOptionTypeTypeDef",
     {
         "Priority": int,
         "Name": RecoveryOptionNameTypeType,
     },
 )
 
+AccountTakeoverActionTypeOutputTypeDef = TypedDict(
+    "AccountTakeoverActionTypeOutputTypeDef",
+    {
+        "Notify": bool,
+        "EventAction": AccountTakeoverEventActionTypeType,
+    },
+)
+
 AccountTakeoverActionTypeTypeDef = TypedDict(
     "AccountTakeoverActionTypeTypeDef",
     {
         "Notify": bool,
         "EventAction": AccountTakeoverEventActionTypeType,
     },
 )
@@ -350,14 +401,23 @@
 class AdminConfirmSignUpRequestRequestTypeDef(
     _RequiredAdminConfirmSignUpRequestRequestTypeDef,
     _OptionalAdminConfirmSignUpRequestRequestTypeDef,
 ):
     pass
 
 
+MessageTemplateTypeOutputTypeDef = TypedDict(
+    "MessageTemplateTypeOutputTypeDef",
+    {
+        "SMSMessage": str,
+        "EmailMessage": str,
+        "EmailSubject": str,
+    },
+)
+
 MessageTemplateTypeTypeDef = TypedDict(
     "MessageTemplateTypeTypeDef",
     {
         "SMSMessage": str,
         "EmailMessage": str,
         "EmailSubject": str,
     },
@@ -459,16 +519,24 @@
     "AdminGetUserRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
 
-MFAOptionTypeTypeDef = TypedDict(
-    "MFAOptionTypeTypeDef",
+AttributeTypeOutputTypeDef = TypedDict(
+    "AttributeTypeOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
+MFAOptionTypeOutputTypeDef = TypedDict(
+    "MFAOptionTypeOutputTypeDef",
     {
         "DeliveryMedium": DeliveryMediumTypeType,
         "AttributeName": str,
     },
 )
 
 AnalyticsMetadataTypeTypeDef = TypedDict(
@@ -532,16 +600,16 @@
 class AdminListGroupsForUserRequestRequestTypeDef(
     _RequiredAdminListGroupsForUserRequestRequestTypeDef,
     _OptionalAdminListGroupsForUserRequestRequestTypeDef,
 ):
     pass
 
 
-GroupTypeTypeDef = TypedDict(
-    "GroupTypeTypeDef",
+GroupTypeOutputTypeDef = TypedDict(
+    "GroupTypeOutputTypeDef",
     {
         "GroupName": str,
         "UserPoolId": str,
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
         "LastModifiedDate": datetime,
@@ -643,14 +711,23 @@
 class AdminSetUserPasswordRequestRequestTypeDef(
     _RequiredAdminSetUserPasswordRequestRequestTypeDef,
     _OptionalAdminSetUserPasswordRequestRequestTypeDef,
 ):
     pass
 
 
+MFAOptionTypeTypeDef = TypedDict(
+    "MFAOptionTypeTypeDef",
+    {
+        "DeliveryMedium": DeliveryMediumTypeType,
+        "AttributeName": str,
+    },
+    total=False,
+)
+
 AdminUpdateAuthEventFeedbackRequestRequestTypeDef = TypedDict(
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "EventId": str,
         "FeedbackValue": FeedbackValueTypeType,
@@ -685,14 +762,25 @@
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
 
+AnalyticsConfigurationTypeOutputTypeDef = TypedDict(
+    "AnalyticsConfigurationTypeOutputTypeDef",
+    {
+        "ApplicationId": str,
+        "ApplicationArn": str,
+        "RoleArn": str,
+        "ExternalId": str,
+        "UserDataShared": bool,
+    },
+)
+
 AnalyticsConfigurationTypeTypeDef = TypedDict(
     "AnalyticsConfigurationTypeTypeDef",
     {
         "ApplicationId": str,
         "ApplicationArn": str,
         "RoleArn": str,
         "ExternalId": str,
@@ -706,53 +794,53 @@
     {
         "AccessToken": str,
         "Session": str,
     },
     total=False,
 )
 
-ChallengeResponseTypeTypeDef = TypedDict(
-    "ChallengeResponseTypeTypeDef",
+ChallengeResponseTypeOutputTypeDef = TypedDict(
+    "ChallengeResponseTypeOutputTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
 )
 
-EventContextDataTypeTypeDef = TypedDict(
-    "EventContextDataTypeTypeDef",
+EventContextDataTypeOutputTypeDef = TypedDict(
+    "EventContextDataTypeOutputTypeDef",
     {
         "IpAddress": str,
         "DeviceName": str,
         "Timezone": str,
         "City": str,
         "Country": str,
     },
 )
 
-EventFeedbackTypeTypeDef = TypedDict(
-    "EventFeedbackTypeTypeDef",
+EventFeedbackTypeOutputTypeDef = TypedDict(
+    "EventFeedbackTypeOutputTypeDef",
     {
         "FeedbackValue": FeedbackValueTypeType,
         "Provider": str,
         "FeedbackDate": datetime,
     },
 )
 
-EventRiskTypeTypeDef = TypedDict(
-    "EventRiskTypeTypeDef",
+EventRiskTypeOutputTypeDef = TypedDict(
+    "EventRiskTypeOutputTypeDef",
     {
         "RiskDecision": RiskDecisionTypeType,
         "RiskLevel": RiskLevelTypeType,
         "CompromisedCredentialsDetected": bool,
     },
 )
 
-NewDeviceMetadataTypeTypeDef = TypedDict(
-    "NewDeviceMetadataTypeTypeDef",
+NewDeviceMetadataTypeOutputTypeDef = TypedDict(
+    "NewDeviceMetadataTypeOutputTypeDef",
     {
         "DeviceKey": str,
         "DeviceGroupKey": str,
     },
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
@@ -760,23 +848,30 @@
     {
         "PreviousPassword": str,
         "ProposedPassword": str,
         "AccessToken": str,
     },
 )
 
-CodeDeliveryDetailsTypeTypeDef = TypedDict(
-    "CodeDeliveryDetailsTypeTypeDef",
+CodeDeliveryDetailsTypeOutputTypeDef = TypedDict(
+    "CodeDeliveryDetailsTypeOutputTypeDef",
     {
         "Destination": str,
         "DeliveryMedium": DeliveryMediumTypeType,
         "AttributeName": str,
     },
 )
 
+CompromisedCredentialsActionsTypeOutputTypeDef = TypedDict(
+    "CompromisedCredentialsActionsTypeOutputTypeDef",
+    {
+        "EventAction": CompromisedCredentialsEventActionTypeType,
+    },
+)
+
 CompromisedCredentialsActionsTypeTypeDef = TypedDict(
     "CompromisedCredentialsActionsTypeTypeDef",
     {
         "EventAction": CompromisedCredentialsEventActionTypeType,
     },
 )
 
@@ -853,16 +948,16 @@
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
 
-IdentityProviderTypeTypeDef = TypedDict(
-    "IdentityProviderTypeTypeDef",
+IdentityProviderTypeOutputTypeDef = TypedDict(
+    "IdentityProviderTypeOutputTypeDef",
     {
         "UserPoolId": str,
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "ProviderDetails": Dict[str, str],
         "AttributeMapping": Dict[str, str],
         "IdpIdentifiers": List[str],
@@ -884,16 +979,16 @@
     {
         "JobName": str,
         "UserPoolId": str,
         "CloudWatchLogsRoleArn": str,
     },
 )
 
-UserImportJobTypeTypeDef = TypedDict(
-    "UserImportJobTypeTypeDef",
+UserImportJobTypeOutputTypeDef = TypedDict(
+    "UserImportJobTypeOutputTypeDef",
     {
         "JobName": str,
         "JobId": str,
         "UserPoolId": str,
         "PreSignedUrl": str,
         "CreationDate": datetime,
         "StartDate": datetime,
@@ -998,22 +1093,45 @@
         "EmailMessageByLink": str,
         "EmailSubjectByLink": str,
         "DefaultEmailOption": DefaultEmailOptionTypeType,
     },
     total=False,
 )
 
+CustomDomainConfigTypeOutputTypeDef = TypedDict(
+    "CustomDomainConfigTypeOutputTypeDef",
+    {
+        "CertificateArn": str,
+    },
+)
+
+CustomEmailLambdaVersionConfigTypeOutputTypeDef = TypedDict(
+    "CustomEmailLambdaVersionConfigTypeOutputTypeDef",
+    {
+        "LambdaVersion": Literal["V1_0"],
+        "LambdaArn": str,
+    },
+)
+
 CustomEmailLambdaVersionConfigTypeTypeDef = TypedDict(
     "CustomEmailLambdaVersionConfigTypeTypeDef",
     {
         "LambdaVersion": Literal["V1_0"],
         "LambdaArn": str,
     },
 )
 
+CustomSMSLambdaVersionConfigTypeOutputTypeDef = TypedDict(
+    "CustomSMSLambdaVersionConfigTypeOutputTypeDef",
+    {
+        "LambdaVersion": Literal["V1_0"],
+        "LambdaArn": str,
+    },
+)
+
 CustomSMSLambdaVersionConfigTypeTypeDef = TypedDict(
     "CustomSMSLambdaVersionConfigTypeTypeDef",
     {
         "LambdaVersion": Literal["V1_0"],
         "LambdaArn": str,
     },
 )
@@ -1144,14 +1262,33 @@
 DescribeUserPoolRequestRequestTypeDef = TypedDict(
     "DescribeUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
+DeviceConfigurationTypeOutputTypeDef = TypedDict(
+    "DeviceConfigurationTypeOutputTypeDef",
+    {
+        "ChallengeRequiredOnNewDevice": bool,
+        "DeviceOnlyRememberedOnUserPrompt": bool,
+    },
+)
+
+EmailConfigurationTypeOutputTypeDef = TypedDict(
+    "EmailConfigurationTypeOutputTypeDef",
+    {
+        "SourceArn": str,
+        "ReplyToEmailAddress": str,
+        "EmailSendingAccount": EmailSendingAccountTypeType,
+        "From": str,
+        "ConfigurationSet": str,
+    },
+)
+
 _RequiredForgetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredForgetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalForgetDeviceRequestRequestTypeDef = TypedDict(
@@ -1238,16 +1375,16 @@
 class GetUICustomizationRequestRequestTypeDef(
     _RequiredGetUICustomizationRequestRequestTypeDef,
     _OptionalGetUICustomizationRequestRequestTypeDef,
 ):
     pass
 
 
-UICustomizationTypeTypeDef = TypedDict(
-    "UICustomizationTypeTypeDef",
+UICustomizationTypeOutputTypeDef = TypedDict(
+    "UICustomizationTypeOutputTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "ImageUrl": str,
         "CSS": str,
         "CSSVersion": str,
         "LastModifiedDate": datetime,
@@ -1281,16 +1418,16 @@
 GetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-SoftwareTokenMfaConfigTypeTypeDef = TypedDict(
-    "SoftwareTokenMfaConfigTypeTypeDef",
+SoftwareTokenMfaConfigTypeOutputTypeDef = TypedDict(
+    "SoftwareTokenMfaConfigTypeOutputTypeDef",
     {
         "Enabled": bool,
     },
 )
 
 GetUserRequestRequestTypeDef = TypedDict(
     "GetUserRequestRequestTypeDef",
@@ -1369,16 +1506,16 @@
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
 
-ProviderDescriptionTypeDef = TypedDict(
-    "ProviderDescriptionTypeDef",
+ProviderDescriptionOutputTypeDef = TypedDict(
+    "ProviderDescriptionOutputTypeDef",
     {
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
 )
@@ -1455,16 +1592,16 @@
 class ListUserPoolClientsRequestRequestTypeDef(
     _RequiredListUserPoolClientsRequestRequestTypeDef,
     _OptionalListUserPoolClientsRequestRequestTypeDef,
 ):
     pass
 
 
-UserPoolClientDescriptionTypeDef = TypedDict(
-    "UserPoolClientDescriptionTypeDef",
+UserPoolClientDescriptionOutputTypeDef = TypedDict(
+    "UserPoolClientDescriptionOutputTypeDef",
     {
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
 )
 
@@ -1532,45 +1669,93 @@
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
 
-NotifyEmailTypeTypeDef = TypedDict(
-    "NotifyEmailTypeTypeDef",
+NotifyEmailTypeOutputTypeDef = TypedDict(
+    "NotifyEmailTypeOutputTypeDef",
     {
         "Subject": str,
         "HtmlBody": str,
         "TextBody": str,
     },
 )
 
+_RequiredNotifyEmailTypeTypeDef = TypedDict(
+    "_RequiredNotifyEmailTypeTypeDef",
+    {
+        "Subject": str,
+    },
+)
+_OptionalNotifyEmailTypeTypeDef = TypedDict(
+    "_OptionalNotifyEmailTypeTypeDef",
+    {
+        "HtmlBody": str,
+        "TextBody": str,
+    },
+    total=False,
+)
+
+
+class NotifyEmailTypeTypeDef(_RequiredNotifyEmailTypeTypeDef, _OptionalNotifyEmailTypeTypeDef):
+    pass
+
+
+NumberAttributeConstraintsTypeOutputTypeDef = TypedDict(
+    "NumberAttributeConstraintsTypeOutputTypeDef",
+    {
+        "MinValue": str,
+        "MaxValue": str,
+    },
+)
+
 NumberAttributeConstraintsTypeTypeDef = TypedDict(
     "NumberAttributeConstraintsTypeTypeDef",
     {
         "MinValue": str,
         "MaxValue": str,
     },
     total=False,
 )
 
+PasswordPolicyTypeOutputTypeDef = TypedDict(
+    "PasswordPolicyTypeOutputTypeDef",
+    {
+        "MinimumLength": int,
+        "RequireUppercase": bool,
+        "RequireLowercase": bool,
+        "RequireNumbers": bool,
+        "RequireSymbols": bool,
+        "TemporaryPasswordValidityDays": int,
+    },
+)
+
 PasswordPolicyTypeTypeDef = TypedDict(
     "PasswordPolicyTypeTypeDef",
     {
         "MinimumLength": int,
         "RequireUppercase": bool,
         "RequireLowercase": bool,
         "RequireNumbers": bool,
         "RequireSymbols": bool,
         "TemporaryPasswordValidityDays": int,
     },
     total=False,
 )
 
+ResourceServerScopeTypeOutputTypeDef = TypedDict(
+    "ResourceServerScopeTypeOutputTypeDef",
+    {
+        "ScopeName": str,
+        "ScopeDescription": str,
+    },
+)
+
 _RequiredRevokeTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeTokenRequestRequestTypeDef",
     {
         "Token": str,
         "ClientId": str,
     },
 )
@@ -1585,22 +1770,39 @@
 
 class RevokeTokenRequestRequestTypeDef(
     _RequiredRevokeTokenRequestRequestTypeDef, _OptionalRevokeTokenRequestRequestTypeDef
 ):
     pass
 
 
-RiskExceptionConfigurationTypeTypeDef = TypedDict(
-    "RiskExceptionConfigurationTypeTypeDef",
+RiskExceptionConfigurationTypeOutputTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     {
         "BlockedIPRangeList": List[str],
         "SkippedIPRangeList": List[str],
     },
 )
 
+RiskExceptionConfigurationTypeTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeTypeDef",
+    {
+        "BlockedIPRangeList": Sequence[str],
+        "SkippedIPRangeList": Sequence[str],
+    },
+    total=False,
+)
+
+StringAttributeConstraintsTypeOutputTypeDef = TypedDict(
+    "StringAttributeConstraintsTypeOutputTypeDef",
+    {
+        "MinLength": str,
+        "MaxLength": str,
+    },
+)
+
 StringAttributeConstraintsTypeTypeDef = TypedDict(
     "StringAttributeConstraintsTypeTypeDef",
     {
         "MinLength": str,
         "MaxLength": str,
     },
     total=False,
@@ -1626,14 +1828,31 @@
 class SetUICustomizationRequestRequestTypeDef(
     _RequiredSetUICustomizationRequestRequestTypeDef,
     _OptionalSetUICustomizationRequestRequestTypeDef,
 ):
     pass
 
 
+SoftwareTokenMfaConfigTypeTypeDef = TypedDict(
+    "SoftwareTokenMfaConfigTypeTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+SmsConfigurationTypeOutputTypeDef = TypedDict(
+    "SmsConfigurationTypeOutputTypeDef",
+    {
+        "SnsCallerArn": str,
+        "ExternalId": str,
+        "SnsRegion": str,
+    },
+)
+
 StartUserImportJobRequestRequestTypeDef = TypedDict(
     "StartUserImportJobRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "JobId": str,
     },
 )
@@ -1650,14 +1869,23 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TokenValidityUnitsTypeOutputTypeDef = TypedDict(
+    "TokenValidityUnitsTypeOutputTypeDef",
+    {
+        "AccessToken": TimeUnitsTypeType,
+        "IdToken": TimeUnitsTypeType,
+        "RefreshToken": TimeUnitsTypeType,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1741,14 +1969,47 @@
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
 
+UserAttributeUpdateSettingsTypeOutputTypeDef = TypedDict(
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
+    {
+        "AttributesRequireVerificationBeforeUpdate": List[VerifiedAttributeTypeType],
+    },
+)
+
+UserPoolAddOnsTypeOutputTypeDef = TypedDict(
+    "UserPoolAddOnsTypeOutputTypeDef",
+    {
+        "AdvancedSecurityMode": AdvancedSecurityModeTypeType,
+    },
+)
+
+UsernameConfigurationTypeOutputTypeDef = TypedDict(
+    "UsernameConfigurationTypeOutputTypeDef",
+    {
+        "CaseSensitive": bool,
+    },
+)
+
+VerificationMessageTemplateTypeOutputTypeDef = TypedDict(
+    "VerificationMessageTemplateTypeOutputTypeDef",
+    {
+        "SmsMessage": str,
+        "EmailMessage": str,
+        "EmailSubject": str,
+        "EmailMessageByLink": str,
+        "EmailSubjectByLink": str,
+        "DefaultEmailOption": DefaultEmailOptionTypeType,
+    },
+)
+
 _RequiredVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "_RequiredVerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
     },
 )
 _OptionalVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
@@ -1774,29 +2035,55 @@
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
     },
 )
 
+AccountRecoverySettingTypeOutputTypeDef = TypedDict(
+    "AccountRecoverySettingTypeOutputTypeDef",
+    {
+        "RecoveryMechanisms": List[RecoveryOptionTypeOutputTypeDef],
+    },
+)
+
 AccountRecoverySettingTypeTypeDef = TypedDict(
     "AccountRecoverySettingTypeTypeDef",
     {
         "RecoveryMechanisms": Sequence[RecoveryOptionTypeTypeDef],
     },
     total=False,
 )
 
+AccountTakeoverActionsTypeOutputTypeDef = TypedDict(
+    "AccountTakeoverActionsTypeOutputTypeDef",
+    {
+        "LowAction": AccountTakeoverActionTypeOutputTypeDef,
+        "MediumAction": AccountTakeoverActionTypeOutputTypeDef,
+        "HighAction": AccountTakeoverActionTypeOutputTypeDef,
+    },
+)
+
 AccountTakeoverActionsTypeTypeDef = TypedDict(
     "AccountTakeoverActionsTypeTypeDef",
     {
         "LowAction": AccountTakeoverActionTypeTypeDef,
         "MediumAction": AccountTakeoverActionTypeTypeDef,
         "HighAction": AccountTakeoverActionTypeTypeDef,
     },
+    total=False,
+)
+
+AdminCreateUserConfigTypeOutputTypeDef = TypedDict(
+    "AdminCreateUserConfigTypeOutputTypeDef",
+    {
+        "AllowAdminCreateUserOnly": bool,
+        "UnusedAccountValidityDays": int,
+        "InviteMessageTemplate": MessageTemplateTypeOutputTypeDef,
+    },
 )
 
 AdminCreateUserConfigTypeTypeDef = TypedDict(
     "AdminCreateUserConfigTypeTypeDef",
     {
         "AllowAdminCreateUserOnly": bool,
         "UnusedAccountValidityDays": int,
@@ -1853,25 +2140,14 @@
 class AdminUpdateUserAttributesRequestRequestTypeDef(
     _RequiredAdminUpdateUserAttributesRequestRequestTypeDef,
     _OptionalAdminUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-DeviceTypeTypeDef = TypedDict(
-    "DeviceTypeTypeDef",
-    {
-        "DeviceKey": str,
-        "DeviceAttributes": List[AttributeTypeTypeDef],
-        "DeviceCreateDate": datetime,
-        "DeviceLastModifiedDate": datetime,
-        "DeviceLastAuthenticatedDate": datetime,
-    },
-)
-
 _RequiredUpdateUserAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAttributesRequestRequestTypeDef",
     {
         "UserAttributes": Sequence[AttributeTypeTypeDef],
         "AccessToken": str,
     },
 )
@@ -1887,81 +2163,81 @@
 class UpdateUserAttributesRequestRequestTypeDef(
     _RequiredUpdateUserAttributesRequestRequestTypeDef,
     _OptionalUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateSoftwareTokenResponseTypeDef = TypedDict(
-    "AssociateSoftwareTokenResponseTypeDef",
+AssociateSoftwareTokenResponseOutputTypeDef = TypedDict(
+    "AssociateSoftwareTokenResponseOutputTypeDef",
     {
         "SecretCode": str,
         "Session": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfirmDeviceResponseTypeDef = TypedDict(
-    "ConfirmDeviceResponseTypeDef",
+ConfirmDeviceResponseOutputTypeDef = TypedDict(
+    "ConfirmDeviceResponseOutputTypeDef",
     {
         "UserConfirmationNecessary": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateUserPoolDomainResponseTypeDef = TypedDict(
-    "CreateUserPoolDomainResponseTypeDef",
+CreateUserPoolDomainResponseOutputTypeDef = TypedDict(
+    "CreateUserPoolDomainResponseOutputTypeDef",
     {
         "CloudFrontDomain": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCSVHeaderResponseTypeDef = TypedDict(
-    "GetCSVHeaderResponseTypeDef",
+GetCSVHeaderResponseOutputTypeDef = TypedDict(
+    "GetCSVHeaderResponseOutputTypeDef",
     {
         "UserPoolId": str,
         "CSVHeader": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetSigningCertificateResponseTypeDef = TypedDict(
-    "GetSigningCertificateResponseTypeDef",
+GetSigningCertificateResponseOutputTypeDef = TypedDict(
+    "GetSigningCertificateResponseOutputTypeDef",
     {
         "Certificate": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateUserPoolDomainResponseTypeDef = TypedDict(
-    "UpdateUserPoolDomainResponseTypeDef",
+UpdateUserPoolDomainResponseOutputTypeDef = TypedDict(
+    "UpdateUserPoolDomainResponseOutputTypeDef",
     {
         "CloudFrontDomain": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VerifySoftwareTokenResponseTypeDef = TypedDict(
-    "VerifySoftwareTokenResponseTypeDef",
+VerifySoftwareTokenResponseOutputTypeDef = TypedDict(
+    "VerifySoftwareTokenResponseOutputTypeDef",
     {
         "Status": VerifySoftwareTokenResponseTypeType,
         "Session": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1978,69 +2254,63 @@
     {
         "UserPoolId": str,
         "DestinationUser": ProviderUserIdentifierTypeTypeDef,
         "SourceUser": ProviderUserIdentifierTypeTypeDef,
     },
 )
 
-AdminGetUserResponseTypeDef = TypedDict(
-    "AdminGetUserResponseTypeDef",
+DeviceTypeOutputTypeDef = TypedDict(
+    "DeviceTypeOutputTypeDef",
+    {
+        "DeviceKey": str,
+        "DeviceAttributes": List[AttributeTypeOutputTypeDef],
+        "DeviceCreateDate": datetime,
+        "DeviceLastModifiedDate": datetime,
+        "DeviceLastAuthenticatedDate": datetime,
+    },
+)
+
+AdminGetUserResponseOutputTypeDef = TypedDict(
+    "AdminGetUserResponseOutputTypeDef",
     {
         "Username": str,
-        "UserAttributes": List[AttributeTypeTypeDef],
+        "UserAttributes": List[AttributeTypeOutputTypeDef],
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
-        "MFAOptions": List[MFAOptionTypeTypeDef],
+        "MFAOptions": List[MFAOptionTypeOutputTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminSetUserSettingsRequestRequestTypeDef = TypedDict(
-    "AdminSetUserSettingsRequestRequestTypeDef",
+GetUserResponseOutputTypeDef = TypedDict(
+    "GetUserResponseOutputTypeDef",
     {
-        "UserPoolId": str,
         "Username": str,
-        "MFAOptions": Sequence[MFAOptionTypeTypeDef],
-    },
-)
-
-GetUserResponseTypeDef = TypedDict(
-    "GetUserResponseTypeDef",
-    {
-        "Username": str,
-        "UserAttributes": List[AttributeTypeTypeDef],
-        "MFAOptions": List[MFAOptionTypeTypeDef],
+        "UserAttributes": List[AttributeTypeOutputTypeDef],
+        "MFAOptions": List[MFAOptionTypeOutputTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetUserSettingsRequestRequestTypeDef = TypedDict(
-    "SetUserSettingsRequestRequestTypeDef",
-    {
-        "AccessToken": str,
-        "MFAOptions": Sequence[MFAOptionTypeTypeDef],
-    },
-)
-
-UserTypeTypeDef = TypedDict(
-    "UserTypeTypeDef",
+UserTypeOutputTypeDef = TypedDict(
+    "UserTypeOutputTypeDef",
     {
         "Username": str,
-        "Attributes": List[AttributeTypeTypeDef],
+        "Attributes": List[AttributeTypeOutputTypeDef],
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
-        "MFAOptions": List[MFAOptionTypeTypeDef],
+        "MFAOptions": List[MFAOptionTypeOutputTypeDef],
     },
 )
 
 _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
     "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     {
         "Username": str,
@@ -2225,52 +2495,52 @@
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
 
-AdminListGroupsForUserResponseTypeDef = TypedDict(
-    "AdminListGroupsForUserResponseTypeDef",
+AdminListGroupsForUserResponseOutputTypeDef = TypedDict(
+    "AdminListGroupsForUserResponseOutputTypeDef",
     {
-        "Groups": List[GroupTypeTypeDef],
+        "Groups": List[GroupTypeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
+CreateGroupResponseOutputTypeDef = TypedDict(
+    "CreateGroupResponseOutputTypeDef",
     {
-        "Group": GroupTypeTypeDef,
+        "Group": GroupTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
+GetGroupResponseOutputTypeDef = TypedDict(
+    "GetGroupResponseOutputTypeDef",
     {
-        "Group": GroupTypeTypeDef,
+        "Group": GroupTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListGroupsResponseTypeDef = TypedDict(
-    "ListGroupsResponseTypeDef",
+ListGroupsResponseOutputTypeDef = TypedDict(
+    "ListGroupsResponseOutputTypeDef",
     {
-        "Groups": List[GroupTypeTypeDef],
+        "Groups": List[GroupTypeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateGroupResponseTypeDef = TypedDict(
-    "UpdateGroupResponseTypeDef",
+UpdateGroupResponseOutputTypeDef = TypedDict(
+    "UpdateGroupResponseOutputTypeDef",
     {
-        "Group": GroupTypeTypeDef,
+        "Group": GroupTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef",
     {
@@ -2314,89 +2584,128 @@
 class SetUserMFAPreferenceRequestRequestTypeDef(
     _RequiredSetUserMFAPreferenceRequestRequestTypeDef,
     _OptionalSetUserMFAPreferenceRequestRequestTypeDef,
 ):
     pass
 
 
-AuthEventTypeTypeDef = TypedDict(
-    "AuthEventTypeTypeDef",
+AdminSetUserSettingsRequestRequestTypeDef = TypedDict(
+    "AdminSetUserSettingsRequestRequestTypeDef",
+    {
+        "UserPoolId": str,
+        "Username": str,
+        "MFAOptions": Sequence[MFAOptionTypeTypeDef],
+    },
+)
+
+SetUserSettingsRequestRequestTypeDef = TypedDict(
+    "SetUserSettingsRequestRequestTypeDef",
+    {
+        "AccessToken": str,
+        "MFAOptions": Sequence[MFAOptionTypeTypeDef],
+    },
+)
+
+AuthEventTypeOutputTypeDef = TypedDict(
+    "AuthEventTypeOutputTypeDef",
     {
         "EventId": str,
         "EventType": EventTypeType,
         "CreationDate": datetime,
         "EventResponse": EventResponseTypeType,
-        "EventRisk": EventRiskTypeTypeDef,
-        "ChallengeResponses": List[ChallengeResponseTypeTypeDef],
-        "EventContextData": EventContextDataTypeTypeDef,
-        "EventFeedback": EventFeedbackTypeTypeDef,
+        "EventRisk": EventRiskTypeOutputTypeDef,
+        "ChallengeResponses": List[ChallengeResponseTypeOutputTypeDef],
+        "EventContextData": EventContextDataTypeOutputTypeDef,
+        "EventFeedback": EventFeedbackTypeOutputTypeDef,
     },
 )
 
-AuthenticationResultTypeTypeDef = TypedDict(
-    "AuthenticationResultTypeTypeDef",
+AuthenticationResultTypeOutputTypeDef = TypedDict(
+    "AuthenticationResultTypeOutputTypeDef",
     {
         "AccessToken": str,
         "ExpiresIn": int,
         "TokenType": str,
         "RefreshToken": str,
         "IdToken": str,
-        "NewDeviceMetadata": NewDeviceMetadataTypeTypeDef,
+        "NewDeviceMetadata": NewDeviceMetadataTypeOutputTypeDef,
     },
 )
 
-ForgotPasswordResponseTypeDef = TypedDict(
-    "ForgotPasswordResponseTypeDef",
+ForgotPasswordResponseOutputTypeDef = TypedDict(
+    "ForgotPasswordResponseOutputTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetUserAttributeVerificationCodeResponseTypeDef = TypedDict(
-    "GetUserAttributeVerificationCodeResponseTypeDef",
+GetUserAttributeVerificationCodeResponseOutputTypeDef = TypedDict(
+    "GetUserAttributeVerificationCodeResponseOutputTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResendConfirmationCodeResponseTypeDef = TypedDict(
-    "ResendConfirmationCodeResponseTypeDef",
+ResendConfirmationCodeResponseOutputTypeDef = TypedDict(
+    "ResendConfirmationCodeResponseOutputTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SignUpResponseTypeDef = TypedDict(
-    "SignUpResponseTypeDef",
+SignUpResponseOutputTypeDef = TypedDict(
+    "SignUpResponseOutputTypeDef",
     {
         "UserConfirmed": bool,
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
         "UserSub": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateUserAttributesResponseTypeDef = TypedDict(
-    "UpdateUserAttributesResponseTypeDef",
+UpdateUserAttributesResponseOutputTypeDef = TypedDict(
+    "UpdateUserAttributesResponseOutputTypeDef",
     {
-        "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
+        "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
-    "CompromisedCredentialsRiskConfigurationTypeTypeDef",
+CompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
+    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     {
         "EventFilter": List[EventFilterTypeType],
+        "Actions": CompromisedCredentialsActionsTypeOutputTypeDef,
+    },
+)
+
+_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
+    "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
+    {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
     },
 )
+_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
+    "_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef",
+    {
+        "EventFilter": Sequence[EventFilterTypeType],
+    },
+    total=False,
+)
+
+
+class CompromisedCredentialsRiskConfigurationTypeTypeDef(
+    _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef,
+    _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef,
+):
+    pass
+
 
 _RequiredConfirmDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
         "DeviceKey": str,
     },
@@ -2621,42 +2930,42 @@
 )
 
 
 class ContextDataTypeTypeDef(_RequiredContextDataTypeTypeDef, _OptionalContextDataTypeTypeDef):
     pass
 
 
-CreateIdentityProviderResponseTypeDef = TypedDict(
-    "CreateIdentityProviderResponseTypeDef",
+CreateIdentityProviderResponseOutputTypeDef = TypedDict(
+    "CreateIdentityProviderResponseOutputTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeTypeDef,
+        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeIdentityProviderResponseTypeDef = TypedDict(
-    "DescribeIdentityProviderResponseTypeDef",
+DescribeIdentityProviderResponseOutputTypeDef = TypedDict(
+    "DescribeIdentityProviderResponseOutputTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeTypeDef,
+        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetIdentityProviderByIdentifierResponseTypeDef = TypedDict(
-    "GetIdentityProviderByIdentifierResponseTypeDef",
+GetIdentityProviderByIdentifierResponseOutputTypeDef = TypedDict(
+    "GetIdentityProviderByIdentifierResponseOutputTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeTypeDef,
+        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateIdentityProviderResponseTypeDef = TypedDict(
-    "UpdateIdentityProviderResponseTypeDef",
+UpdateIdentityProviderResponseOutputTypeDef = TypedDict(
+    "UpdateIdentityProviderResponseOutputTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeTypeDef,
+        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceServerRequestRequestTypeDef",
     {
@@ -2677,24 +2986,14 @@
 class CreateResourceServerRequestRequestTypeDef(
     _RequiredCreateResourceServerRequestRequestTypeDef,
     _OptionalCreateResourceServerRequestRequestTypeDef,
 ):
     pass
 
 
-ResourceServerTypeTypeDef = TypedDict(
-    "ResourceServerTypeTypeDef",
-    {
-        "UserPoolId": str,
-        "Identifier": str,
-        "Name": str,
-        "Scopes": List[ResourceServerScopeTypeTypeDef],
-    },
-)
-
 _RequiredUpdateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceServerRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Identifier": str,
         "Name": str,
     },
@@ -2711,51 +3010,51 @@
 class UpdateResourceServerRequestRequestTypeDef(
     _RequiredUpdateResourceServerRequestRequestTypeDef,
     _OptionalUpdateResourceServerRequestRequestTypeDef,
 ):
     pass
 
 
-CreateUserImportJobResponseTypeDef = TypedDict(
-    "CreateUserImportJobResponseTypeDef",
+CreateUserImportJobResponseOutputTypeDef = TypedDict(
+    "CreateUserImportJobResponseOutputTypeDef",
     {
-        "UserImportJob": UserImportJobTypeTypeDef,
+        "UserImportJob": UserImportJobTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeUserImportJobResponseTypeDef = TypedDict(
-    "DescribeUserImportJobResponseTypeDef",
+DescribeUserImportJobResponseOutputTypeDef = TypedDict(
+    "DescribeUserImportJobResponseOutputTypeDef",
     {
-        "UserImportJob": UserImportJobTypeTypeDef,
+        "UserImportJob": UserImportJobTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserImportJobsResponseTypeDef = TypedDict(
-    "ListUserImportJobsResponseTypeDef",
+ListUserImportJobsResponseOutputTypeDef = TypedDict(
+    "ListUserImportJobsResponseOutputTypeDef",
     {
-        "UserImportJobs": List[UserImportJobTypeTypeDef],
+        "UserImportJobs": List[UserImportJobTypeOutputTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartUserImportJobResponseTypeDef = TypedDict(
-    "StartUserImportJobResponseTypeDef",
+StartUserImportJobResponseOutputTypeDef = TypedDict(
+    "StartUserImportJobResponseOutputTypeDef",
     {
-        "UserImportJob": UserImportJobTypeTypeDef,
+        "UserImportJob": UserImportJobTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopUserImportJobResponseTypeDef = TypedDict(
-    "StopUserImportJobResponseTypeDef",
+StopUserImportJobResponseOutputTypeDef = TypedDict(
+    "StopUserImportJobResponseOutputTypeDef",
     {
-        "UserImportJob": UserImportJobTypeTypeDef,
+        "UserImportJob": UserImportJobTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolClientRequestRequestTypeDef",
     {
@@ -2836,45 +3135,14 @@
 class UpdateUserPoolClientRequestRequestTypeDef(
     _RequiredUpdateUserPoolClientRequestRequestTypeDef,
     _OptionalUpdateUserPoolClientRequestRequestTypeDef,
 ):
     pass
 
 
-UserPoolClientTypeTypeDef = TypedDict(
-    "UserPoolClientTypeTypeDef",
-    {
-        "UserPoolId": str,
-        "ClientName": str,
-        "ClientId": str,
-        "ClientSecret": str,
-        "LastModifiedDate": datetime,
-        "CreationDate": datetime,
-        "RefreshTokenValidity": int,
-        "AccessTokenValidity": int,
-        "IdTokenValidity": int,
-        "TokenValidityUnits": TokenValidityUnitsTypeTypeDef,
-        "ReadAttributes": List[str],
-        "WriteAttributes": List[str],
-        "ExplicitAuthFlows": List[ExplicitAuthFlowsTypeType],
-        "SupportedIdentityProviders": List[str],
-        "CallbackURLs": List[str],
-        "LogoutURLs": List[str],
-        "DefaultRedirectURI": str,
-        "AllowedOAuthFlows": List[OAuthFlowTypeType],
-        "AllowedOAuthScopes": List[str],
-        "AllowedOAuthFlowsUserPoolClient": bool,
-        "AnalyticsConfiguration": AnalyticsConfigurationTypeTypeDef,
-        "PreventUserExistenceErrors": PreventUserExistenceErrorTypesType,
-        "EnableTokenRevocation": bool,
-        "EnablePropagateAdditionalUserContextData": bool,
-        "AuthSessionValidity": int,
-    },
-)
-
 _RequiredCreateUserPoolDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolDomainRequestRequestTypeDef",
     {
         "Domain": str,
         "UserPoolId": str,
     },
 )
@@ -2890,28 +3158,14 @@
 class CreateUserPoolDomainRequestRequestTypeDef(
     _RequiredCreateUserPoolDomainRequestRequestTypeDef,
     _OptionalCreateUserPoolDomainRequestRequestTypeDef,
 ):
     pass
 
 
-DomainDescriptionTypeTypeDef = TypedDict(
-    "DomainDescriptionTypeTypeDef",
-    {
-        "UserPoolId": str,
-        "AWSAccountId": str,
-        "Domain": str,
-        "S3Bucket": str,
-        "CloudFrontDistribution": str,
-        "Version": str,
-        "Status": DomainStatusTypeType,
-        "CustomDomainConfig": CustomDomainConfigTypeTypeDef,
-    },
-)
-
 UpdateUserPoolDomainRequestRequestTypeDef = TypedDict(
     "UpdateUserPoolDomainRequestRequestTypeDef",
     {
         "Domain": str,
         "UserPoolId": str,
         "CustomDomainConfig": CustomDomainConfigTypeTypeDef,
     },
@@ -2919,14 +3173,48 @@
 
 SmsMfaConfigTypeTypeDef = TypedDict(
     "SmsMfaConfigTypeTypeDef",
     {
         "SmsAuthenticationMessage": str,
         "SmsConfiguration": SmsConfigurationTypeTypeDef,
     },
+    total=False,
+)
+
+DomainDescriptionTypeOutputTypeDef = TypedDict(
+    "DomainDescriptionTypeOutputTypeDef",
+    {
+        "UserPoolId": str,
+        "AWSAccountId": str,
+        "Domain": str,
+        "S3Bucket": str,
+        "CloudFrontDistribution": str,
+        "Version": str,
+        "Status": DomainStatusTypeType,
+        "CustomDomainConfig": CustomDomainConfigTypeOutputTypeDef,
+    },
+)
+
+LambdaConfigTypeOutputTypeDef = TypedDict(
+    "LambdaConfigTypeOutputTypeDef",
+    {
+        "PreSignUp": str,
+        "CustomMessage": str,
+        "PostConfirmation": str,
+        "PreAuthentication": str,
+        "PostAuthentication": str,
+        "DefineAuthChallenge": str,
+        "CreateAuthChallenge": str,
+        "VerifyAuthChallengeResponse": str,
+        "PreTokenGeneration": str,
+        "UserMigration": str,
+        "CustomSMSSender": CustomSMSLambdaVersionConfigTypeOutputTypeDef,
+        "CustomEmailSender": CustomEmailLambdaVersionConfigTypeOutputTypeDef,
+        "KMSKeyID": str,
+    },
 )
 
 LambdaConfigTypeTypeDef = TypedDict(
     "LambdaConfigTypeTypeDef",
     {
         "PreSignUp": str,
         "CustomMessage": str,
@@ -2941,191 +3229,285 @@
         "CustomSMSSender": CustomSMSLambdaVersionConfigTypeTypeDef,
         "CustomEmailSender": CustomEmailLambdaVersionConfigTypeTypeDef,
         "KMSKeyID": str,
     },
     total=False,
 )
 
-GetUICustomizationResponseTypeDef = TypedDict(
-    "GetUICustomizationResponseTypeDef",
+GetUICustomizationResponseOutputTypeDef = TypedDict(
+    "GetUICustomizationResponseOutputTypeDef",
     {
-        "UICustomization": UICustomizationTypeTypeDef,
+        "UICustomization": UICustomizationTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetUICustomizationResponseTypeDef = TypedDict(
-    "SetUICustomizationResponseTypeDef",
+SetUICustomizationResponseOutputTypeDef = TypedDict(
+    "SetUICustomizationResponseOutputTypeDef",
     {
-        "UICustomization": UICustomizationTypeTypeDef,
+        "UICustomization": UICustomizationTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListIdentityProvidersResponseTypeDef = TypedDict(
-    "ListIdentityProvidersResponseTypeDef",
+ListIdentityProvidersResponseOutputTypeDef = TypedDict(
+    "ListIdentityProvidersResponseOutputTypeDef",
     {
-        "Providers": List[ProviderDescriptionTypeDef],
+        "Providers": List[ProviderDescriptionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserPoolClientsResponseTypeDef = TypedDict(
-    "ListUserPoolClientsResponseTypeDef",
+ListUserPoolClientsResponseOutputTypeDef = TypedDict(
+    "ListUserPoolClientsResponseOutputTypeDef",
     {
-        "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
+        "UserPoolClients": List[UserPoolClientDescriptionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NotifyConfigurationTypeTypeDef = TypedDict(
-    "NotifyConfigurationTypeTypeDef",
+NotifyConfigurationTypeOutputTypeDef = TypedDict(
+    "NotifyConfigurationTypeOutputTypeDef",
     {
         "From": str,
         "ReplyTo": str,
         "SourceArn": str,
+        "BlockEmail": NotifyEmailTypeOutputTypeDef,
+        "NoActionEmail": NotifyEmailTypeOutputTypeDef,
+        "MfaEmail": NotifyEmailTypeOutputTypeDef,
+    },
+)
+
+_RequiredNotifyConfigurationTypeTypeDef = TypedDict(
+    "_RequiredNotifyConfigurationTypeTypeDef",
+    {
+        "SourceArn": str,
+    },
+)
+_OptionalNotifyConfigurationTypeTypeDef = TypedDict(
+    "_OptionalNotifyConfigurationTypeTypeDef",
+    {
+        "From": str,
+        "ReplyTo": str,
         "BlockEmail": NotifyEmailTypeTypeDef,
         "NoActionEmail": NotifyEmailTypeTypeDef,
         "MfaEmail": NotifyEmailTypeTypeDef,
     },
+    total=False,
+)
+
+
+class NotifyConfigurationTypeTypeDef(
+    _RequiredNotifyConfigurationTypeTypeDef, _OptionalNotifyConfigurationTypeTypeDef
+):
+    pass
+
+
+UserPoolPolicyTypeOutputTypeDef = TypedDict(
+    "UserPoolPolicyTypeOutputTypeDef",
+    {
+        "PasswordPolicy": PasswordPolicyTypeOutputTypeDef,
+    },
 )
 
 UserPoolPolicyTypeTypeDef = TypedDict(
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
 
+ResourceServerTypeOutputTypeDef = TypedDict(
+    "ResourceServerTypeOutputTypeDef",
+    {
+        "UserPoolId": str,
+        "Identifier": str,
+        "Name": str,
+        "Scopes": List[ResourceServerScopeTypeOutputTypeDef],
+    },
+)
+
+SchemaAttributeTypeOutputTypeDef = TypedDict(
+    "SchemaAttributeTypeOutputTypeDef",
+    {
+        "Name": str,
+        "AttributeDataType": AttributeDataTypeType,
+        "DeveloperOnlyAttribute": bool,
+        "Mutable": bool,
+        "Required": bool,
+        "NumberAttributeConstraints": NumberAttributeConstraintsTypeOutputTypeDef,
+        "StringAttributeConstraints": StringAttributeConstraintsTypeOutputTypeDef,
+    },
+)
+
 SchemaAttributeTypeTypeDef = TypedDict(
     "SchemaAttributeTypeTypeDef",
     {
         "Name": str,
         "AttributeDataType": AttributeDataTypeType,
         "DeveloperOnlyAttribute": bool,
         "Mutable": bool,
         "Required": bool,
         "NumberAttributeConstraints": NumberAttributeConstraintsTypeTypeDef,
         "StringAttributeConstraints": StringAttributeConstraintsTypeTypeDef,
     },
     total=False,
 )
 
-AdminGetDeviceResponseTypeDef = TypedDict(
-    "AdminGetDeviceResponseTypeDef",
+SmsMfaConfigTypeOutputTypeDef = TypedDict(
+    "SmsMfaConfigTypeOutputTypeDef",
     {
-        "Device": DeviceTypeTypeDef,
+        "SmsAuthenticationMessage": str,
+        "SmsConfiguration": SmsConfigurationTypeOutputTypeDef,
+    },
+)
+
+UserPoolClientTypeOutputTypeDef = TypedDict(
+    "UserPoolClientTypeOutputTypeDef",
+    {
+        "UserPoolId": str,
+        "ClientName": str,
+        "ClientId": str,
+        "ClientSecret": str,
+        "LastModifiedDate": datetime,
+        "CreationDate": datetime,
+        "RefreshTokenValidity": int,
+        "AccessTokenValidity": int,
+        "IdTokenValidity": int,
+        "TokenValidityUnits": TokenValidityUnitsTypeOutputTypeDef,
+        "ReadAttributes": List[str],
+        "WriteAttributes": List[str],
+        "ExplicitAuthFlows": List[ExplicitAuthFlowsTypeType],
+        "SupportedIdentityProviders": List[str],
+        "CallbackURLs": List[str],
+        "LogoutURLs": List[str],
+        "DefaultRedirectURI": str,
+        "AllowedOAuthFlows": List[OAuthFlowTypeType],
+        "AllowedOAuthScopes": List[str],
+        "AllowedOAuthFlowsUserPoolClient": bool,
+        "AnalyticsConfiguration": AnalyticsConfigurationTypeOutputTypeDef,
+        "PreventUserExistenceErrors": PreventUserExistenceErrorTypesType,
+        "EnableTokenRevocation": bool,
+        "EnablePropagateAdditionalUserContextData": bool,
+        "AuthSessionValidity": int,
+    },
+)
+
+AdminGetDeviceResponseOutputTypeDef = TypedDict(
+    "AdminGetDeviceResponseOutputTypeDef",
+    {
+        "Device": DeviceTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminListDevicesResponseTypeDef = TypedDict(
-    "AdminListDevicesResponseTypeDef",
+AdminListDevicesResponseOutputTypeDef = TypedDict(
+    "AdminListDevicesResponseOutputTypeDef",
     {
-        "Devices": List[DeviceTypeTypeDef],
+        "Devices": List[DeviceTypeOutputTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetDeviceResponseTypeDef = TypedDict(
-    "GetDeviceResponseTypeDef",
+GetDeviceResponseOutputTypeDef = TypedDict(
+    "GetDeviceResponseOutputTypeDef",
     {
-        "Device": DeviceTypeTypeDef,
+        "Device": DeviceTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDevicesResponseTypeDef = TypedDict(
-    "ListDevicesResponseTypeDef",
+ListDevicesResponseOutputTypeDef = TypedDict(
+    "ListDevicesResponseOutputTypeDef",
     {
-        "Devices": List[DeviceTypeTypeDef],
+        "Devices": List[DeviceTypeOutputTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminCreateUserResponseTypeDef = TypedDict(
-    "AdminCreateUserResponseTypeDef",
+AdminCreateUserResponseOutputTypeDef = TypedDict(
+    "AdminCreateUserResponseOutputTypeDef",
     {
-        "User": UserTypeTypeDef,
+        "User": UserTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUsersInGroupResponseTypeDef = TypedDict(
-    "ListUsersInGroupResponseTypeDef",
+ListUsersInGroupResponseOutputTypeDef = TypedDict(
+    "ListUsersInGroupResponseOutputTypeDef",
     {
-        "Users": List[UserTypeTypeDef],
+        "Users": List[UserTypeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUsersResponseTypeDef = TypedDict(
-    "ListUsersResponseTypeDef",
+ListUsersResponseOutputTypeDef = TypedDict(
+    "ListUsersResponseOutputTypeDef",
     {
-        "Users": List[UserTypeTypeDef],
+        "Users": List[UserTypeOutputTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminListUserAuthEventsResponseTypeDef = TypedDict(
-    "AdminListUserAuthEventsResponseTypeDef",
+AdminListUserAuthEventsResponseOutputTypeDef = TypedDict(
+    "AdminListUserAuthEventsResponseOutputTypeDef",
     {
-        "AuthEvents": List[AuthEventTypeTypeDef],
+        "AuthEvents": List[AuthEventTypeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminInitiateAuthResponseTypeDef = TypedDict(
-    "AdminInitiateAuthResponseTypeDef",
+AdminInitiateAuthResponseOutputTypeDef = TypedDict(
+    "AdminInitiateAuthResponseOutputTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminRespondToAuthChallengeResponseTypeDef = TypedDict(
-    "AdminRespondToAuthChallengeResponseTypeDef",
+AdminRespondToAuthChallengeResponseOutputTypeDef = TypedDict(
+    "AdminRespondToAuthChallengeResponseOutputTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InitiateAuthResponseTypeDef = TypedDict(
-    "InitiateAuthResponseTypeDef",
+InitiateAuthResponseOutputTypeDef = TypedDict(
+    "InitiateAuthResponseOutputTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RespondToAuthChallengeResponseTypeDef = TypedDict(
-    "RespondToAuthChallengeResponseTypeDef",
+RespondToAuthChallengeResponseOutputTypeDef = TypedDict(
+    "RespondToAuthChallengeResponseOutputTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
@@ -3176,89 +3558,14 @@
 class AdminRespondToAuthChallengeRequestRequestTypeDef(
     _RequiredAdminRespondToAuthChallengeRequestRequestTypeDef,
     _OptionalAdminRespondToAuthChallengeRequestRequestTypeDef,
 ):
     pass
 
 
-CreateResourceServerResponseTypeDef = TypedDict(
-    "CreateResourceServerResponseTypeDef",
-    {
-        "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeResourceServerResponseTypeDef = TypedDict(
-    "DescribeResourceServerResponseTypeDef",
-    {
-        "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListResourceServersResponseTypeDef = TypedDict(
-    "ListResourceServersResponseTypeDef",
-    {
-        "ResourceServers": List[ResourceServerTypeTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateResourceServerResponseTypeDef = TypedDict(
-    "UpdateResourceServerResponseTypeDef",
-    {
-        "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserPoolClientResponseTypeDef = TypedDict(
-    "CreateUserPoolClientResponseTypeDef",
-    {
-        "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeUserPoolClientResponseTypeDef = TypedDict(
-    "DescribeUserPoolClientResponseTypeDef",
-    {
-        "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateUserPoolClientResponseTypeDef = TypedDict(
-    "UpdateUserPoolClientResponseTypeDef",
-    {
-        "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeUserPoolDomainResponseTypeDef = TypedDict(
-    "DescribeUserPoolDomainResponseTypeDef",
-    {
-        "DomainDescription": DomainDescriptionTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUserPoolMfaConfigResponseTypeDef = TypedDict(
-    "GetUserPoolMfaConfigResponseTypeDef",
-    {
-        "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
-        "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
-        "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredSetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalSetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
@@ -3275,43 +3582,63 @@
 class SetUserPoolMfaConfigRequestRequestTypeDef(
     _RequiredSetUserPoolMfaConfigRequestRequestTypeDef,
     _OptionalSetUserPoolMfaConfigRequestRequestTypeDef,
 ):
     pass
 
 
-SetUserPoolMfaConfigResponseTypeDef = TypedDict(
-    "SetUserPoolMfaConfigResponseTypeDef",
+DescribeUserPoolDomainResponseOutputTypeDef = TypedDict(
+    "DescribeUserPoolDomainResponseOutputTypeDef",
     {
-        "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
-        "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
-        "MfaConfiguration": UserPoolMfaTypeType,
+        "DomainDescription": DomainDescriptionTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserPoolDescriptionTypeTypeDef = TypedDict(
-    "UserPoolDescriptionTypeTypeDef",
+UserPoolDescriptionTypeOutputTypeDef = TypedDict(
+    "UserPoolDescriptionTypeOutputTypeDef",
     {
         "Id": str,
         "Name": str,
-        "LambdaConfig": LambdaConfigTypeTypeDef,
+        "LambdaConfig": LambdaConfigTypeOutputTypeDef,
         "Status": StatusTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
 )
 
-AccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
-    "AccountTakeoverRiskConfigurationTypeTypeDef",
+AccountTakeoverRiskConfigurationTypeOutputTypeDef = TypedDict(
+    "AccountTakeoverRiskConfigurationTypeOutputTypeDef",
+    {
+        "NotifyConfiguration": NotifyConfigurationTypeOutputTypeDef,
+        "Actions": AccountTakeoverActionsTypeOutputTypeDef,
+    },
+)
+
+_RequiredAccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
+    "_RequiredAccountTakeoverRiskConfigurationTypeTypeDef",
     {
-        "NotifyConfiguration": NotifyConfigurationTypeTypeDef,
         "Actions": AccountTakeoverActionsTypeTypeDef,
     },
 )
+_OptionalAccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
+    "_OptionalAccountTakeoverRiskConfigurationTypeTypeDef",
+    {
+        "NotifyConfiguration": NotifyConfigurationTypeTypeDef,
+    },
+    total=False,
+)
+
+
+class AccountTakeoverRiskConfigurationTypeTypeDef(
+    _RequiredAccountTakeoverRiskConfigurationTypeTypeDef,
+    _OptionalAccountTakeoverRiskConfigurationTypeTypeDef,
+):
+    pass
+
 
 _RequiredUpdateUserPoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
@@ -3343,14 +3670,86 @@
 
 class UpdateUserPoolRequestRequestTypeDef(
     _RequiredUpdateUserPoolRequestRequestTypeDef, _OptionalUpdateUserPoolRequestRequestTypeDef
 ):
     pass
 
 
+CreateResourceServerResponseOutputTypeDef = TypedDict(
+    "CreateResourceServerResponseOutputTypeDef",
+    {
+        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeResourceServerResponseOutputTypeDef = TypedDict(
+    "DescribeResourceServerResponseOutputTypeDef",
+    {
+        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourceServersResponseOutputTypeDef = TypedDict(
+    "ListResourceServersResponseOutputTypeDef",
+    {
+        "ResourceServers": List[ResourceServerTypeOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateResourceServerResponseOutputTypeDef = TypedDict(
+    "UpdateResourceServerResponseOutputTypeDef",
+    {
+        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UserPoolTypeOutputTypeDef = TypedDict(
+    "UserPoolTypeOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Policies": UserPoolPolicyTypeOutputTypeDef,
+        "DeletionProtection": DeletionProtectionTypeType,
+        "LambdaConfig": LambdaConfigTypeOutputTypeDef,
+        "Status": StatusTypeType,
+        "LastModifiedDate": datetime,
+        "CreationDate": datetime,
+        "SchemaAttributes": List[SchemaAttributeTypeOutputTypeDef],
+        "AutoVerifiedAttributes": List[VerifiedAttributeTypeType],
+        "AliasAttributes": List[AliasAttributeTypeType],
+        "UsernameAttributes": List[UsernameAttributeTypeType],
+        "SmsVerificationMessage": str,
+        "EmailVerificationMessage": str,
+        "EmailVerificationSubject": str,
+        "VerificationMessageTemplate": VerificationMessageTemplateTypeOutputTypeDef,
+        "SmsAuthenticationMessage": str,
+        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeOutputTypeDef,
+        "MfaConfiguration": UserPoolMfaTypeType,
+        "DeviceConfiguration": DeviceConfigurationTypeOutputTypeDef,
+        "EstimatedNumberOfUsers": int,
+        "EmailConfiguration": EmailConfigurationTypeOutputTypeDef,
+        "SmsConfiguration": SmsConfigurationTypeOutputTypeDef,
+        "UserPoolTags": Dict[str, str],
+        "SmsConfigurationFailure": str,
+        "EmailConfigurationFailure": str,
+        "Domain": str,
+        "CustomDomain": str,
+        "AdminCreateUserConfig": AdminCreateUserConfigTypeOutputTypeDef,
+        "UserPoolAddOns": UserPoolAddOnsTypeOutputTypeDef,
+        "UsernameConfiguration": UsernameConfigurationTypeOutputTypeDef,
+        "Arn": str,
+        "AccountRecoverySetting": AccountRecoverySettingTypeOutputTypeDef,
+    },
+)
+
 AddCustomAttributesRequestRequestTypeDef = TypedDict(
     "AddCustomAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "CustomAttributes": Sequence[SchemaAttributeTypeTypeDef],
     },
 )
@@ -3393,72 +3792,77 @@
 
 class CreateUserPoolRequestRequestTypeDef(
     _RequiredCreateUserPoolRequestRequestTypeDef, _OptionalCreateUserPoolRequestRequestTypeDef
 ):
     pass
 
 
-UserPoolTypeTypeDef = TypedDict(
-    "UserPoolTypeTypeDef",
+GetUserPoolMfaConfigResponseOutputTypeDef = TypedDict(
+    "GetUserPoolMfaConfigResponseOutputTypeDef",
     {
-        "Id": str,
-        "Name": str,
-        "Policies": UserPoolPolicyTypeTypeDef,
-        "DeletionProtection": DeletionProtectionTypeType,
-        "LambdaConfig": LambdaConfigTypeTypeDef,
-        "Status": StatusTypeType,
-        "LastModifiedDate": datetime,
-        "CreationDate": datetime,
-        "SchemaAttributes": List[SchemaAttributeTypeTypeDef],
-        "AutoVerifiedAttributes": List[VerifiedAttributeTypeType],
-        "AliasAttributes": List[AliasAttributeTypeType],
-        "UsernameAttributes": List[UsernameAttributeTypeType],
-        "SmsVerificationMessage": str,
-        "EmailVerificationMessage": str,
-        "EmailVerificationSubject": str,
-        "VerificationMessageTemplate": VerificationMessageTemplateTypeTypeDef,
-        "SmsAuthenticationMessage": str,
-        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeTypeDef,
+        "SmsMfaConfiguration": SmsMfaConfigTypeOutputTypeDef,
+        "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeOutputTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "DeviceConfiguration": DeviceConfigurationTypeTypeDef,
-        "EstimatedNumberOfUsers": int,
-        "EmailConfiguration": EmailConfigurationTypeTypeDef,
-        "SmsConfiguration": SmsConfigurationTypeTypeDef,
-        "UserPoolTags": Dict[str, str],
-        "SmsConfigurationFailure": str,
-        "EmailConfigurationFailure": str,
-        "Domain": str,
-        "CustomDomain": str,
-        "AdminCreateUserConfig": AdminCreateUserConfigTypeTypeDef,
-        "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
-        "UsernameConfiguration": UsernameConfigurationTypeTypeDef,
-        "Arn": str,
-        "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetUserPoolMfaConfigResponseOutputTypeDef = TypedDict(
+    "SetUserPoolMfaConfigResponseOutputTypeDef",
+    {
+        "SmsMfaConfiguration": SmsMfaConfigTypeOutputTypeDef,
+        "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeOutputTypeDef,
+        "MfaConfiguration": UserPoolMfaTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserPoolsResponseTypeDef = TypedDict(
-    "ListUserPoolsResponseTypeDef",
+CreateUserPoolClientResponseOutputTypeDef = TypedDict(
+    "CreateUserPoolClientResponseOutputTypeDef",
     {
-        "UserPools": List[UserPoolDescriptionTypeTypeDef],
+        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUserPoolClientResponseOutputTypeDef = TypedDict(
+    "DescribeUserPoolClientResponseOutputTypeDef",
+    {
+        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateUserPoolClientResponseOutputTypeDef = TypedDict(
+    "UpdateUserPoolClientResponseOutputTypeDef",
+    {
+        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListUserPoolsResponseOutputTypeDef = TypedDict(
+    "ListUserPoolsResponseOutputTypeDef",
+    {
+        "UserPools": List[UserPoolDescriptionTypeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RiskConfigurationTypeTypeDef = TypedDict(
-    "RiskConfigurationTypeTypeDef",
+RiskConfigurationTypeOutputTypeDef = TypedDict(
+    "RiskConfigurationTypeOutputTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "CompromisedCredentialsRiskConfiguration": (
-            CompromisedCredentialsRiskConfigurationTypeTypeDef
+            CompromisedCredentialsRiskConfigurationTypeOutputTypeDef
         ),
-        "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
-        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
+        "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeOutputTypeDef,
+        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeOutputTypeDef,
         "LastModifiedDate": datetime,
     },
 )
 
 _RequiredSetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetRiskConfigurationRequestRequestTypeDef",
     {
@@ -3482,38 +3886,38 @@
 class SetRiskConfigurationRequestRequestTypeDef(
     _RequiredSetRiskConfigurationRequestRequestTypeDef,
     _OptionalSetRiskConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-CreateUserPoolResponseTypeDef = TypedDict(
-    "CreateUserPoolResponseTypeDef",
+CreateUserPoolResponseOutputTypeDef = TypedDict(
+    "CreateUserPoolResponseOutputTypeDef",
     {
-        "UserPool": UserPoolTypeTypeDef,
+        "UserPool": UserPoolTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeUserPoolResponseTypeDef = TypedDict(
-    "DescribeUserPoolResponseTypeDef",
+DescribeUserPoolResponseOutputTypeDef = TypedDict(
+    "DescribeUserPoolResponseOutputTypeDef",
     {
-        "UserPool": UserPoolTypeTypeDef,
+        "UserPool": UserPoolTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeRiskConfigurationResponseTypeDef = TypedDict(
-    "DescribeRiskConfigurationResponseTypeDef",
+DescribeRiskConfigurationResponseOutputTypeDef = TypedDict(
+    "DescribeRiskConfigurationResponseOutputTypeDef",
     {
-        "RiskConfiguration": RiskConfigurationTypeTypeDef,
+        "RiskConfiguration": RiskConfigurationTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetRiskConfigurationResponseTypeDef = TypedDict(
-    "SetRiskConfigurationResponseTypeDef",
+SetRiskConfigurationResponseOutputTypeDef = TypedDict(
+    "SetRiskConfigurationResponseOutputTypeDef",
     {
-        "RiskConfiguration": RiskConfigurationTypeTypeDef,
+        "RiskConfiguration": RiskConfigurationTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/type_defs.pyi` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cognito-idp service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cognito_idp.type_defs import RecoveryOptionTypeTypeDef
+    from mypy_boto3_cognito_idp.type_defs import RecoveryOptionTypeOutputTypeDef
 
-    data: RecoveryOptionTypeTypeDef = {...}
+    data: RecoveryOptionTypeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -61,73 +61,83 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "RecoveryOptionTypeOutputTypeDef",
     "RecoveryOptionTypeTypeDef",
+    "AccountTakeoverActionTypeOutputTypeDef",
     "AccountTakeoverActionTypeTypeDef",
     "AdminAddUserToGroupRequestRequestTypeDef",
     "AdminConfirmSignUpRequestRequestTypeDef",
+    "MessageTemplateTypeOutputTypeDef",
     "MessageTemplateTypeTypeDef",
     "AttributeTypeTypeDef",
     "ResponseMetadataTypeDef",
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     "AdminDeleteUserRequestRequestTypeDef",
     "ProviderUserIdentifierTypeTypeDef",
     "AdminDisableUserRequestRequestTypeDef",
     "AdminEnableUserRequestRequestTypeDef",
     "AdminForgetDeviceRequestRequestTypeDef",
     "AdminGetDeviceRequestRequestTypeDef",
     "AdminGetUserRequestRequestTypeDef",
-    "MFAOptionTypeTypeDef",
+    "AttributeTypeOutputTypeDef",
+    "MFAOptionTypeOutputTypeDef",
     "AnalyticsMetadataTypeTypeDef",
     "AdminListDevicesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "AdminListGroupsForUserRequestRequestTypeDef",
-    "GroupTypeTypeDef",
+    "GroupTypeOutputTypeDef",
     "AdminListUserAuthEventsRequestRequestTypeDef",
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     "AdminResetUserPasswordRequestRequestTypeDef",
     "SMSMfaSettingsTypeTypeDef",
     "SoftwareTokenMfaSettingsTypeTypeDef",
     "AdminSetUserPasswordRequestRequestTypeDef",
+    "MFAOptionTypeTypeDef",
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     "AdminUpdateDeviceStatusRequestRequestTypeDef",
     "AdminUserGlobalSignOutRequestRequestTypeDef",
+    "AnalyticsConfigurationTypeOutputTypeDef",
     "AnalyticsConfigurationTypeTypeDef",
     "AssociateSoftwareTokenRequestRequestTypeDef",
-    "ChallengeResponseTypeTypeDef",
-    "EventContextDataTypeTypeDef",
-    "EventFeedbackTypeTypeDef",
-    "EventRiskTypeTypeDef",
-    "NewDeviceMetadataTypeTypeDef",
+    "ChallengeResponseTypeOutputTypeDef",
+    "EventContextDataTypeOutputTypeDef",
+    "EventFeedbackTypeOutputTypeDef",
+    "EventRiskTypeOutputTypeDef",
+    "NewDeviceMetadataTypeOutputTypeDef",
     "ChangePasswordRequestRequestTypeDef",
-    "CodeDeliveryDetailsTypeTypeDef",
+    "CodeDeliveryDetailsTypeOutputTypeDef",
+    "CompromisedCredentialsActionsTypeOutputTypeDef",
     "CompromisedCredentialsActionsTypeTypeDef",
     "DeviceSecretVerifierConfigTypeTypeDef",
     "UserContextDataTypeTypeDef",
     "HttpHeaderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
-    "IdentityProviderTypeTypeDef",
+    "IdentityProviderTypeOutputTypeDef",
     "ResourceServerScopeTypeTypeDef",
     "CreateUserImportJobRequestRequestTypeDef",
-    "UserImportJobTypeTypeDef",
+    "UserImportJobTypeOutputTypeDef",
     "TokenValidityUnitsTypeTypeDef",
     "CustomDomainConfigTypeTypeDef",
     "DeviceConfigurationTypeTypeDef",
     "EmailConfigurationTypeTypeDef",
     "SmsConfigurationTypeTypeDef",
     "UserAttributeUpdateSettingsTypeTypeDef",
     "UserPoolAddOnsTypeTypeDef",
     "UsernameConfigurationTypeTypeDef",
     "VerificationMessageTemplateTypeTypeDef",
+    "CustomDomainConfigTypeOutputTypeDef",
+    "CustomEmailLambdaVersionConfigTypeOutputTypeDef",
     "CustomEmailLambdaVersionConfigTypeTypeDef",
+    "CustomSMSLambdaVersionConfigTypeOutputTypeDef",
     "CustomSMSLambdaVersionConfigTypeTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteIdentityProviderRequestRequestTypeDef",
     "DeleteResourceServerRequestRequestTypeDef",
     "DeleteUserAttributesRequestRequestTypeDef",
     "DeleteUserPoolClientRequestRequestTypeDef",
     "DeleteUserPoolDomainRequestRequestTypeDef",
@@ -136,187 +146,228 @@
     "DescribeIdentityProviderRequestRequestTypeDef",
     "DescribeResourceServerRequestRequestTypeDef",
     "DescribeRiskConfigurationRequestRequestTypeDef",
     "DescribeUserImportJobRequestRequestTypeDef",
     "DescribeUserPoolClientRequestRequestTypeDef",
     "DescribeUserPoolDomainRequestRequestTypeDef",
     "DescribeUserPoolRequestRequestTypeDef",
+    "DeviceConfigurationTypeOutputTypeDef",
+    "EmailConfigurationTypeOutputTypeDef",
     "ForgetDeviceRequestRequestTypeDef",
     "GetCSVHeaderRequestRequestTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIdentityProviderByIdentifierRequestRequestTypeDef",
     "GetSigningCertificateRequestRequestTypeDef",
     "GetUICustomizationRequestRequestTypeDef",
-    "UICustomizationTypeTypeDef",
+    "UICustomizationTypeOutputTypeDef",
     "GetUserAttributeVerificationCodeRequestRequestTypeDef",
     "GetUserPoolMfaConfigRequestRequestTypeDef",
-    "SoftwareTokenMfaConfigTypeTypeDef",
+    "SoftwareTokenMfaConfigTypeOutputTypeDef",
     "GetUserRequestRequestTypeDef",
     "GlobalSignOutRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
-    "ProviderDescriptionTypeDef",
+    "ProviderDescriptionOutputTypeDef",
     "ListResourceServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUserImportJobsRequestRequestTypeDef",
     "ListUserPoolClientsRequestRequestTypeDef",
-    "UserPoolClientDescriptionTypeDef",
+    "UserPoolClientDescriptionOutputTypeDef",
     "ListUserPoolsRequestRequestTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
+    "NotifyEmailTypeOutputTypeDef",
     "NotifyEmailTypeTypeDef",
+    "NumberAttributeConstraintsTypeOutputTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
+    "PasswordPolicyTypeOutputTypeDef",
     "PasswordPolicyTypeTypeDef",
+    "ResourceServerScopeTypeOutputTypeDef",
     "RevokeTokenRequestRequestTypeDef",
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
+    "StringAttributeConstraintsTypeOutputTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
     "SetUICustomizationRequestRequestTypeDef",
+    "SoftwareTokenMfaConfigTypeTypeDef",
+    "SmsConfigurationTypeOutputTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TokenValidityUnitsTypeOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
+    "UserPoolAddOnsTypeOutputTypeDef",
+    "UsernameConfigurationTypeOutputTypeDef",
+    "VerificationMessageTemplateTypeOutputTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
+    "AccountRecoverySettingTypeOutputTypeDef",
     "AccountRecoverySettingTypeTypeDef",
+    "AccountTakeoverActionsTypeOutputTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
+    "AdminCreateUserConfigTypeOutputTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
-    "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
-    "AssociateSoftwareTokenResponseTypeDef",
-    "ConfirmDeviceResponseTypeDef",
-    "CreateUserPoolDomainResponseTypeDef",
+    "AssociateSoftwareTokenResponseOutputTypeDef",
+    "ConfirmDeviceResponseOutputTypeDef",
+    "CreateUserPoolDomainResponseOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "GetCSVHeaderResponseTypeDef",
-    "GetSigningCertificateResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateUserPoolDomainResponseTypeDef",
-    "VerifySoftwareTokenResponseTypeDef",
+    "GetCSVHeaderResponseOutputTypeDef",
+    "GetSigningCertificateResponseOutputTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
+    "UpdateUserPoolDomainResponseOutputTypeDef",
+    "VerifySoftwareTokenResponseOutputTypeDef",
     "AdminDisableProviderForUserRequestRequestTypeDef",
     "AdminLinkProviderForUserRequestRequestTypeDef",
-    "AdminGetUserResponseTypeDef",
-    "AdminSetUserSettingsRequestRequestTypeDef",
-    "GetUserResponseTypeDef",
-    "SetUserSettingsRequestRequestTypeDef",
-    "UserTypeTypeDef",
+    "DeviceTypeOutputTypeDef",
+    "AdminGetUserResponseOutputTypeDef",
+    "GetUserResponseOutputTypeDef",
+    "UserTypeOutputTypeDef",
     "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListResourceServersRequestListResourceServersPaginateTypeDef",
     "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
     "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
     "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
-    "AdminListGroupsForUserResponseTypeDef",
-    "CreateGroupResponseTypeDef",
-    "GetGroupResponseTypeDef",
-    "ListGroupsResponseTypeDef",
-    "UpdateGroupResponseTypeDef",
+    "AdminListGroupsForUserResponseOutputTypeDef",
+    "CreateGroupResponseOutputTypeDef",
+    "GetGroupResponseOutputTypeDef",
+    "ListGroupsResponseOutputTypeDef",
+    "UpdateGroupResponseOutputTypeDef",
     "AdminSetUserMFAPreferenceRequestRequestTypeDef",
     "SetUserMFAPreferenceRequestRequestTypeDef",
-    "AuthEventTypeTypeDef",
-    "AuthenticationResultTypeTypeDef",
-    "ForgotPasswordResponseTypeDef",
-    "GetUserAttributeVerificationCodeResponseTypeDef",
-    "ResendConfirmationCodeResponseTypeDef",
-    "SignUpResponseTypeDef",
-    "UpdateUserAttributesResponseTypeDef",
+    "AdminSetUserSettingsRequestRequestTypeDef",
+    "SetUserSettingsRequestRequestTypeDef",
+    "AuthEventTypeOutputTypeDef",
+    "AuthenticationResultTypeOutputTypeDef",
+    "ForgotPasswordResponseOutputTypeDef",
+    "GetUserAttributeVerificationCodeResponseOutputTypeDef",
+    "ResendConfirmationCodeResponseOutputTypeDef",
+    "SignUpResponseOutputTypeDef",
+    "UpdateUserAttributesResponseOutputTypeDef",
+    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     "ConfirmDeviceRequestRequestTypeDef",
     "ConfirmForgotPasswordRequestRequestTypeDef",
     "ConfirmSignUpRequestRequestTypeDef",
     "ForgotPasswordRequestRequestTypeDef",
     "InitiateAuthRequestRequestTypeDef",
     "ResendConfirmationCodeRequestRequestTypeDef",
     "RespondToAuthChallengeRequestRequestTypeDef",
     "SignUpRequestRequestTypeDef",
     "ContextDataTypeTypeDef",
-    "CreateIdentityProviderResponseTypeDef",
-    "DescribeIdentityProviderResponseTypeDef",
-    "GetIdentityProviderByIdentifierResponseTypeDef",
-    "UpdateIdentityProviderResponseTypeDef",
+    "CreateIdentityProviderResponseOutputTypeDef",
+    "DescribeIdentityProviderResponseOutputTypeDef",
+    "GetIdentityProviderByIdentifierResponseOutputTypeDef",
+    "UpdateIdentityProviderResponseOutputTypeDef",
     "CreateResourceServerRequestRequestTypeDef",
-    "ResourceServerTypeTypeDef",
     "UpdateResourceServerRequestRequestTypeDef",
-    "CreateUserImportJobResponseTypeDef",
-    "DescribeUserImportJobResponseTypeDef",
-    "ListUserImportJobsResponseTypeDef",
-    "StartUserImportJobResponseTypeDef",
-    "StopUserImportJobResponseTypeDef",
+    "CreateUserImportJobResponseOutputTypeDef",
+    "DescribeUserImportJobResponseOutputTypeDef",
+    "ListUserImportJobsResponseOutputTypeDef",
+    "StartUserImportJobResponseOutputTypeDef",
+    "StopUserImportJobResponseOutputTypeDef",
     "CreateUserPoolClientRequestRequestTypeDef",
     "UpdateUserPoolClientRequestRequestTypeDef",
-    "UserPoolClientTypeTypeDef",
     "CreateUserPoolDomainRequestRequestTypeDef",
-    "DomainDescriptionTypeTypeDef",
     "UpdateUserPoolDomainRequestRequestTypeDef",
     "SmsMfaConfigTypeTypeDef",
+    "DomainDescriptionTypeOutputTypeDef",
+    "LambdaConfigTypeOutputTypeDef",
     "LambdaConfigTypeTypeDef",
-    "GetUICustomizationResponseTypeDef",
-    "SetUICustomizationResponseTypeDef",
-    "ListIdentityProvidersResponseTypeDef",
-    "ListUserPoolClientsResponseTypeDef",
+    "GetUICustomizationResponseOutputTypeDef",
+    "SetUICustomizationResponseOutputTypeDef",
+    "ListIdentityProvidersResponseOutputTypeDef",
+    "ListUserPoolClientsResponseOutputTypeDef",
+    "NotifyConfigurationTypeOutputTypeDef",
     "NotifyConfigurationTypeTypeDef",
+    "UserPoolPolicyTypeOutputTypeDef",
     "UserPoolPolicyTypeTypeDef",
+    "ResourceServerTypeOutputTypeDef",
+    "SchemaAttributeTypeOutputTypeDef",
     "SchemaAttributeTypeTypeDef",
-    "AdminGetDeviceResponseTypeDef",
-    "AdminListDevicesResponseTypeDef",
-    "GetDeviceResponseTypeDef",
-    "ListDevicesResponseTypeDef",
-    "AdminCreateUserResponseTypeDef",
-    "ListUsersInGroupResponseTypeDef",
-    "ListUsersResponseTypeDef",
-    "AdminListUserAuthEventsResponseTypeDef",
-    "AdminInitiateAuthResponseTypeDef",
-    "AdminRespondToAuthChallengeResponseTypeDef",
-    "InitiateAuthResponseTypeDef",
-    "RespondToAuthChallengeResponseTypeDef",
+    "SmsMfaConfigTypeOutputTypeDef",
+    "UserPoolClientTypeOutputTypeDef",
+    "AdminGetDeviceResponseOutputTypeDef",
+    "AdminListDevicesResponseOutputTypeDef",
+    "GetDeviceResponseOutputTypeDef",
+    "ListDevicesResponseOutputTypeDef",
+    "AdminCreateUserResponseOutputTypeDef",
+    "ListUsersInGroupResponseOutputTypeDef",
+    "ListUsersResponseOutputTypeDef",
+    "AdminListUserAuthEventsResponseOutputTypeDef",
+    "AdminInitiateAuthResponseOutputTypeDef",
+    "AdminRespondToAuthChallengeResponseOutputTypeDef",
+    "InitiateAuthResponseOutputTypeDef",
+    "RespondToAuthChallengeResponseOutputTypeDef",
     "AdminInitiateAuthRequestRequestTypeDef",
     "AdminRespondToAuthChallengeRequestRequestTypeDef",
-    "CreateResourceServerResponseTypeDef",
-    "DescribeResourceServerResponseTypeDef",
-    "ListResourceServersResponseTypeDef",
-    "UpdateResourceServerResponseTypeDef",
-    "CreateUserPoolClientResponseTypeDef",
-    "DescribeUserPoolClientResponseTypeDef",
-    "UpdateUserPoolClientResponseTypeDef",
-    "DescribeUserPoolDomainResponseTypeDef",
-    "GetUserPoolMfaConfigResponseTypeDef",
     "SetUserPoolMfaConfigRequestRequestTypeDef",
-    "SetUserPoolMfaConfigResponseTypeDef",
-    "UserPoolDescriptionTypeTypeDef",
+    "DescribeUserPoolDomainResponseOutputTypeDef",
+    "UserPoolDescriptionTypeOutputTypeDef",
+    "AccountTakeoverRiskConfigurationTypeOutputTypeDef",
     "AccountTakeoverRiskConfigurationTypeTypeDef",
     "UpdateUserPoolRequestRequestTypeDef",
+    "CreateResourceServerResponseOutputTypeDef",
+    "DescribeResourceServerResponseOutputTypeDef",
+    "ListResourceServersResponseOutputTypeDef",
+    "UpdateResourceServerResponseOutputTypeDef",
+    "UserPoolTypeOutputTypeDef",
     "AddCustomAttributesRequestRequestTypeDef",
     "CreateUserPoolRequestRequestTypeDef",
-    "UserPoolTypeTypeDef",
-    "ListUserPoolsResponseTypeDef",
-    "RiskConfigurationTypeTypeDef",
+    "GetUserPoolMfaConfigResponseOutputTypeDef",
+    "SetUserPoolMfaConfigResponseOutputTypeDef",
+    "CreateUserPoolClientResponseOutputTypeDef",
+    "DescribeUserPoolClientResponseOutputTypeDef",
+    "UpdateUserPoolClientResponseOutputTypeDef",
+    "ListUserPoolsResponseOutputTypeDef",
+    "RiskConfigurationTypeOutputTypeDef",
     "SetRiskConfigurationRequestRequestTypeDef",
-    "CreateUserPoolResponseTypeDef",
-    "DescribeUserPoolResponseTypeDef",
-    "DescribeRiskConfigurationResponseTypeDef",
-    "SetRiskConfigurationResponseTypeDef",
+    "CreateUserPoolResponseOutputTypeDef",
+    "DescribeUserPoolResponseOutputTypeDef",
+    "DescribeRiskConfigurationResponseOutputTypeDef",
+    "SetRiskConfigurationResponseOutputTypeDef",
+)
+
+RecoveryOptionTypeOutputTypeDef = TypedDict(
+    "RecoveryOptionTypeOutputTypeDef",
+    {
+        "Priority": int,
+        "Name": RecoveryOptionNameTypeType,
+    },
 )
 
 RecoveryOptionTypeTypeDef = TypedDict(
     "RecoveryOptionTypeTypeDef",
     {
         "Priority": int,
         "Name": RecoveryOptionNameTypeType,
     },
 )
 
+AccountTakeoverActionTypeOutputTypeDef = TypedDict(
+    "AccountTakeoverActionTypeOutputTypeDef",
+    {
+        "Notify": bool,
+        "EventAction": AccountTakeoverEventActionTypeType,
+    },
+)
+
 AccountTakeoverActionTypeTypeDef = TypedDict(
     "AccountTakeoverActionTypeTypeDef",
     {
         "Notify": bool,
         "EventAction": AccountTakeoverEventActionTypeType,
     },
 )
@@ -347,14 +398,23 @@
 
 class AdminConfirmSignUpRequestRequestTypeDef(
     _RequiredAdminConfirmSignUpRequestRequestTypeDef,
     _OptionalAdminConfirmSignUpRequestRequestTypeDef,
 ):
     pass
 
+MessageTemplateTypeOutputTypeDef = TypedDict(
+    "MessageTemplateTypeOutputTypeDef",
+    {
+        "SMSMessage": str,
+        "EmailMessage": str,
+        "EmailSubject": str,
+    },
+)
+
 MessageTemplateTypeTypeDef = TypedDict(
     "MessageTemplateTypeTypeDef",
     {
         "SMSMessage": str,
         "EmailMessage": str,
         "EmailSubject": str,
     },
@@ -454,16 +514,24 @@
     "AdminGetUserRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
 
-MFAOptionTypeTypeDef = TypedDict(
-    "MFAOptionTypeTypeDef",
+AttributeTypeOutputTypeDef = TypedDict(
+    "AttributeTypeOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
+MFAOptionTypeOutputTypeDef = TypedDict(
+    "MFAOptionTypeOutputTypeDef",
     {
         "DeliveryMedium": DeliveryMediumTypeType,
         "AttributeName": str,
     },
 )
 
 AnalyticsMetadataTypeTypeDef = TypedDict(
@@ -523,16 +591,16 @@
 
 class AdminListGroupsForUserRequestRequestTypeDef(
     _RequiredAdminListGroupsForUserRequestRequestTypeDef,
     _OptionalAdminListGroupsForUserRequestRequestTypeDef,
 ):
     pass
 
-GroupTypeTypeDef = TypedDict(
-    "GroupTypeTypeDef",
+GroupTypeOutputTypeDef = TypedDict(
+    "GroupTypeOutputTypeDef",
     {
         "GroupName": str,
         "UserPoolId": str,
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
         "LastModifiedDate": datetime,
@@ -628,14 +696,23 @@
 
 class AdminSetUserPasswordRequestRequestTypeDef(
     _RequiredAdminSetUserPasswordRequestRequestTypeDef,
     _OptionalAdminSetUserPasswordRequestRequestTypeDef,
 ):
     pass
 
+MFAOptionTypeTypeDef = TypedDict(
+    "MFAOptionTypeTypeDef",
+    {
+        "DeliveryMedium": DeliveryMediumTypeType,
+        "AttributeName": str,
+    },
+    total=False,
+)
+
 AdminUpdateAuthEventFeedbackRequestRequestTypeDef = TypedDict(
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "EventId": str,
         "FeedbackValue": FeedbackValueTypeType,
@@ -668,14 +745,25 @@
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
 
+AnalyticsConfigurationTypeOutputTypeDef = TypedDict(
+    "AnalyticsConfigurationTypeOutputTypeDef",
+    {
+        "ApplicationId": str,
+        "ApplicationArn": str,
+        "RoleArn": str,
+        "ExternalId": str,
+        "UserDataShared": bool,
+    },
+)
+
 AnalyticsConfigurationTypeTypeDef = TypedDict(
     "AnalyticsConfigurationTypeTypeDef",
     {
         "ApplicationId": str,
         "ApplicationArn": str,
         "RoleArn": str,
         "ExternalId": str,
@@ -689,53 +777,53 @@
     {
         "AccessToken": str,
         "Session": str,
     },
     total=False,
 )
 
-ChallengeResponseTypeTypeDef = TypedDict(
-    "ChallengeResponseTypeTypeDef",
+ChallengeResponseTypeOutputTypeDef = TypedDict(
+    "ChallengeResponseTypeOutputTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
 )
 
-EventContextDataTypeTypeDef = TypedDict(
-    "EventContextDataTypeTypeDef",
+EventContextDataTypeOutputTypeDef = TypedDict(
+    "EventContextDataTypeOutputTypeDef",
     {
         "IpAddress": str,
         "DeviceName": str,
         "Timezone": str,
         "City": str,
         "Country": str,
     },
 )
 
-EventFeedbackTypeTypeDef = TypedDict(
-    "EventFeedbackTypeTypeDef",
+EventFeedbackTypeOutputTypeDef = TypedDict(
+    "EventFeedbackTypeOutputTypeDef",
     {
         "FeedbackValue": FeedbackValueTypeType,
         "Provider": str,
         "FeedbackDate": datetime,
     },
 )
 
-EventRiskTypeTypeDef = TypedDict(
-    "EventRiskTypeTypeDef",
+EventRiskTypeOutputTypeDef = TypedDict(
+    "EventRiskTypeOutputTypeDef",
     {
         "RiskDecision": RiskDecisionTypeType,
         "RiskLevel": RiskLevelTypeType,
         "CompromisedCredentialsDetected": bool,
     },
 )
 
-NewDeviceMetadataTypeTypeDef = TypedDict(
-    "NewDeviceMetadataTypeTypeDef",
+NewDeviceMetadataTypeOutputTypeDef = TypedDict(
+    "NewDeviceMetadataTypeOutputTypeDef",
     {
         "DeviceKey": str,
         "DeviceGroupKey": str,
     },
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
@@ -743,23 +831,30 @@
     {
         "PreviousPassword": str,
         "ProposedPassword": str,
         "AccessToken": str,
     },
 )
 
-CodeDeliveryDetailsTypeTypeDef = TypedDict(
-    "CodeDeliveryDetailsTypeTypeDef",
+CodeDeliveryDetailsTypeOutputTypeDef = TypedDict(
+    "CodeDeliveryDetailsTypeOutputTypeDef",
     {
         "Destination": str,
         "DeliveryMedium": DeliveryMediumTypeType,
         "AttributeName": str,
     },
 )
 
+CompromisedCredentialsActionsTypeOutputTypeDef = TypedDict(
+    "CompromisedCredentialsActionsTypeOutputTypeDef",
+    {
+        "EventAction": CompromisedCredentialsEventActionTypeType,
+    },
+)
+
 CompromisedCredentialsActionsTypeTypeDef = TypedDict(
     "CompromisedCredentialsActionsTypeTypeDef",
     {
         "EventAction": CompromisedCredentialsEventActionTypeType,
     },
 )
 
@@ -832,16 +927,16 @@
 
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-IdentityProviderTypeTypeDef = TypedDict(
-    "IdentityProviderTypeTypeDef",
+IdentityProviderTypeOutputTypeDef = TypedDict(
+    "IdentityProviderTypeOutputTypeDef",
     {
         "UserPoolId": str,
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "ProviderDetails": Dict[str, str],
         "AttributeMapping": Dict[str, str],
         "IdpIdentifiers": List[str],
@@ -863,16 +958,16 @@
     {
         "JobName": str,
         "UserPoolId": str,
         "CloudWatchLogsRoleArn": str,
     },
 )
 
-UserImportJobTypeTypeDef = TypedDict(
-    "UserImportJobTypeTypeDef",
+UserImportJobTypeOutputTypeDef = TypedDict(
+    "UserImportJobTypeOutputTypeDef",
     {
         "JobName": str,
         "JobId": str,
         "UserPoolId": str,
         "PreSignedUrl": str,
         "CreationDate": datetime,
         "StartDate": datetime,
@@ -975,22 +1070,45 @@
         "EmailMessageByLink": str,
         "EmailSubjectByLink": str,
         "DefaultEmailOption": DefaultEmailOptionTypeType,
     },
     total=False,
 )
 
+CustomDomainConfigTypeOutputTypeDef = TypedDict(
+    "CustomDomainConfigTypeOutputTypeDef",
+    {
+        "CertificateArn": str,
+    },
+)
+
+CustomEmailLambdaVersionConfigTypeOutputTypeDef = TypedDict(
+    "CustomEmailLambdaVersionConfigTypeOutputTypeDef",
+    {
+        "LambdaVersion": Literal["V1_0"],
+        "LambdaArn": str,
+    },
+)
+
 CustomEmailLambdaVersionConfigTypeTypeDef = TypedDict(
     "CustomEmailLambdaVersionConfigTypeTypeDef",
     {
         "LambdaVersion": Literal["V1_0"],
         "LambdaArn": str,
     },
 )
 
+CustomSMSLambdaVersionConfigTypeOutputTypeDef = TypedDict(
+    "CustomSMSLambdaVersionConfigTypeOutputTypeDef",
+    {
+        "LambdaVersion": Literal["V1_0"],
+        "LambdaArn": str,
+    },
+)
+
 CustomSMSLambdaVersionConfigTypeTypeDef = TypedDict(
     "CustomSMSLambdaVersionConfigTypeTypeDef",
     {
         "LambdaVersion": Literal["V1_0"],
         "LambdaArn": str,
     },
 )
@@ -1119,14 +1237,33 @@
 DescribeUserPoolRequestRequestTypeDef = TypedDict(
     "DescribeUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
+DeviceConfigurationTypeOutputTypeDef = TypedDict(
+    "DeviceConfigurationTypeOutputTypeDef",
+    {
+        "ChallengeRequiredOnNewDevice": bool,
+        "DeviceOnlyRememberedOnUserPrompt": bool,
+    },
+)
+
+EmailConfigurationTypeOutputTypeDef = TypedDict(
+    "EmailConfigurationTypeOutputTypeDef",
+    {
+        "SourceArn": str,
+        "ReplyToEmailAddress": str,
+        "EmailSendingAccount": EmailSendingAccountTypeType,
+        "From": str,
+        "ConfigurationSet": str,
+    },
+)
+
 _RequiredForgetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredForgetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalForgetDeviceRequestRequestTypeDef = TypedDict(
@@ -1207,16 +1344,16 @@
 
 class GetUICustomizationRequestRequestTypeDef(
     _RequiredGetUICustomizationRequestRequestTypeDef,
     _OptionalGetUICustomizationRequestRequestTypeDef,
 ):
     pass
 
-UICustomizationTypeTypeDef = TypedDict(
-    "UICustomizationTypeTypeDef",
+UICustomizationTypeOutputTypeDef = TypedDict(
+    "UICustomizationTypeOutputTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "ImageUrl": str,
         "CSS": str,
         "CSSVersion": str,
         "LastModifiedDate": datetime,
@@ -1248,16 +1385,16 @@
 GetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-SoftwareTokenMfaConfigTypeTypeDef = TypedDict(
-    "SoftwareTokenMfaConfigTypeTypeDef",
+SoftwareTokenMfaConfigTypeOutputTypeDef = TypedDict(
+    "SoftwareTokenMfaConfigTypeOutputTypeDef",
     {
         "Enabled": bool,
     },
 )
 
 GetUserRequestRequestTypeDef = TypedDict(
     "GetUserRequestRequestTypeDef",
@@ -1330,16 +1467,16 @@
 
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
-ProviderDescriptionTypeDef = TypedDict(
-    "ProviderDescriptionTypeDef",
+ProviderDescriptionOutputTypeDef = TypedDict(
+    "ProviderDescriptionOutputTypeDef",
     {
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
 )
@@ -1410,16 +1547,16 @@
 
 class ListUserPoolClientsRequestRequestTypeDef(
     _RequiredListUserPoolClientsRequestRequestTypeDef,
     _OptionalListUserPoolClientsRequestRequestTypeDef,
 ):
     pass
 
-UserPoolClientDescriptionTypeDef = TypedDict(
-    "UserPoolClientDescriptionTypeDef",
+UserPoolClientDescriptionOutputTypeDef = TypedDict(
+    "UserPoolClientDescriptionOutputTypeDef",
     {
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
 )
 
@@ -1481,45 +1618,91 @@
 )
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-NotifyEmailTypeTypeDef = TypedDict(
-    "NotifyEmailTypeTypeDef",
+NotifyEmailTypeOutputTypeDef = TypedDict(
+    "NotifyEmailTypeOutputTypeDef",
+    {
+        "Subject": str,
+        "HtmlBody": str,
+        "TextBody": str,
+    },
+)
+
+_RequiredNotifyEmailTypeTypeDef = TypedDict(
+    "_RequiredNotifyEmailTypeTypeDef",
     {
         "Subject": str,
+    },
+)
+_OptionalNotifyEmailTypeTypeDef = TypedDict(
+    "_OptionalNotifyEmailTypeTypeDef",
+    {
         "HtmlBody": str,
         "TextBody": str,
     },
+    total=False,
+)
+
+class NotifyEmailTypeTypeDef(_RequiredNotifyEmailTypeTypeDef, _OptionalNotifyEmailTypeTypeDef):
+    pass
+
+NumberAttributeConstraintsTypeOutputTypeDef = TypedDict(
+    "NumberAttributeConstraintsTypeOutputTypeDef",
+    {
+        "MinValue": str,
+        "MaxValue": str,
+    },
 )
 
 NumberAttributeConstraintsTypeTypeDef = TypedDict(
     "NumberAttributeConstraintsTypeTypeDef",
     {
         "MinValue": str,
         "MaxValue": str,
     },
     total=False,
 )
 
+PasswordPolicyTypeOutputTypeDef = TypedDict(
+    "PasswordPolicyTypeOutputTypeDef",
+    {
+        "MinimumLength": int,
+        "RequireUppercase": bool,
+        "RequireLowercase": bool,
+        "RequireNumbers": bool,
+        "RequireSymbols": bool,
+        "TemporaryPasswordValidityDays": int,
+    },
+)
+
 PasswordPolicyTypeTypeDef = TypedDict(
     "PasswordPolicyTypeTypeDef",
     {
         "MinimumLength": int,
         "RequireUppercase": bool,
         "RequireLowercase": bool,
         "RequireNumbers": bool,
         "RequireSymbols": bool,
         "TemporaryPasswordValidityDays": int,
     },
     total=False,
 )
 
+ResourceServerScopeTypeOutputTypeDef = TypedDict(
+    "ResourceServerScopeTypeOutputTypeDef",
+    {
+        "ScopeName": str,
+        "ScopeDescription": str,
+    },
+)
+
 _RequiredRevokeTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeTokenRequestRequestTypeDef",
     {
         "Token": str,
         "ClientId": str,
     },
 )
@@ -1532,22 +1715,39 @@
 )
 
 class RevokeTokenRequestRequestTypeDef(
     _RequiredRevokeTokenRequestRequestTypeDef, _OptionalRevokeTokenRequestRequestTypeDef
 ):
     pass
 
-RiskExceptionConfigurationTypeTypeDef = TypedDict(
-    "RiskExceptionConfigurationTypeTypeDef",
+RiskExceptionConfigurationTypeOutputTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     {
         "BlockedIPRangeList": List[str],
         "SkippedIPRangeList": List[str],
     },
 )
 
+RiskExceptionConfigurationTypeTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeTypeDef",
+    {
+        "BlockedIPRangeList": Sequence[str],
+        "SkippedIPRangeList": Sequence[str],
+    },
+    total=False,
+)
+
+StringAttributeConstraintsTypeOutputTypeDef = TypedDict(
+    "StringAttributeConstraintsTypeOutputTypeDef",
+    {
+        "MinLength": str,
+        "MaxLength": str,
+    },
+)
+
 StringAttributeConstraintsTypeTypeDef = TypedDict(
     "StringAttributeConstraintsTypeTypeDef",
     {
         "MinLength": str,
         "MaxLength": str,
     },
     total=False,
@@ -1571,14 +1771,31 @@
 
 class SetUICustomizationRequestRequestTypeDef(
     _RequiredSetUICustomizationRequestRequestTypeDef,
     _OptionalSetUICustomizationRequestRequestTypeDef,
 ):
     pass
 
+SoftwareTokenMfaConfigTypeTypeDef = TypedDict(
+    "SoftwareTokenMfaConfigTypeTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+SmsConfigurationTypeOutputTypeDef = TypedDict(
+    "SmsConfigurationTypeOutputTypeDef",
+    {
+        "SnsCallerArn": str,
+        "ExternalId": str,
+        "SnsRegion": str,
+    },
+)
+
 StartUserImportJobRequestRequestTypeDef = TypedDict(
     "StartUserImportJobRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "JobId": str,
     },
 )
@@ -1595,14 +1812,23 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TokenValidityUnitsTypeOutputTypeDef = TypedDict(
+    "TokenValidityUnitsTypeOutputTypeDef",
+    {
+        "AccessToken": TimeUnitsTypeType,
+        "IdToken": TimeUnitsTypeType,
+        "RefreshToken": TimeUnitsTypeType,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1680,14 +1906,47 @@
 
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
+UserAttributeUpdateSettingsTypeOutputTypeDef = TypedDict(
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
+    {
+        "AttributesRequireVerificationBeforeUpdate": List[VerifiedAttributeTypeType],
+    },
+)
+
+UserPoolAddOnsTypeOutputTypeDef = TypedDict(
+    "UserPoolAddOnsTypeOutputTypeDef",
+    {
+        "AdvancedSecurityMode": AdvancedSecurityModeTypeType,
+    },
+)
+
+UsernameConfigurationTypeOutputTypeDef = TypedDict(
+    "UsernameConfigurationTypeOutputTypeDef",
+    {
+        "CaseSensitive": bool,
+    },
+)
+
+VerificationMessageTemplateTypeOutputTypeDef = TypedDict(
+    "VerificationMessageTemplateTypeOutputTypeDef",
+    {
+        "SmsMessage": str,
+        "EmailMessage": str,
+        "EmailSubject": str,
+        "EmailMessageByLink": str,
+        "EmailSubjectByLink": str,
+        "DefaultEmailOption": DefaultEmailOptionTypeType,
+    },
+)
+
 _RequiredVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "_RequiredVerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
     },
 )
 _OptionalVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
@@ -1711,29 +1970,55 @@
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
     },
 )
 
+AccountRecoverySettingTypeOutputTypeDef = TypedDict(
+    "AccountRecoverySettingTypeOutputTypeDef",
+    {
+        "RecoveryMechanisms": List[RecoveryOptionTypeOutputTypeDef],
+    },
+)
+
 AccountRecoverySettingTypeTypeDef = TypedDict(
     "AccountRecoverySettingTypeTypeDef",
     {
         "RecoveryMechanisms": Sequence[RecoveryOptionTypeTypeDef],
     },
     total=False,
 )
 
+AccountTakeoverActionsTypeOutputTypeDef = TypedDict(
+    "AccountTakeoverActionsTypeOutputTypeDef",
+    {
+        "LowAction": AccountTakeoverActionTypeOutputTypeDef,
+        "MediumAction": AccountTakeoverActionTypeOutputTypeDef,
+        "HighAction": AccountTakeoverActionTypeOutputTypeDef,
+    },
+)
+
 AccountTakeoverActionsTypeTypeDef = TypedDict(
     "AccountTakeoverActionsTypeTypeDef",
     {
         "LowAction": AccountTakeoverActionTypeTypeDef,
         "MediumAction": AccountTakeoverActionTypeTypeDef,
         "HighAction": AccountTakeoverActionTypeTypeDef,
     },
+    total=False,
+)
+
+AdminCreateUserConfigTypeOutputTypeDef = TypedDict(
+    "AdminCreateUserConfigTypeOutputTypeDef",
+    {
+        "AllowAdminCreateUserOnly": bool,
+        "UnusedAccountValidityDays": int,
+        "InviteMessageTemplate": MessageTemplateTypeOutputTypeDef,
+    },
 )
 
 AdminCreateUserConfigTypeTypeDef = TypedDict(
     "AdminCreateUserConfigTypeTypeDef",
     {
         "AllowAdminCreateUserOnly": bool,
         "UnusedAccountValidityDays": int,
@@ -1786,25 +2071,14 @@
 
 class AdminUpdateUserAttributesRequestRequestTypeDef(
     _RequiredAdminUpdateUserAttributesRequestRequestTypeDef,
     _OptionalAdminUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
-DeviceTypeTypeDef = TypedDict(
-    "DeviceTypeTypeDef",
-    {
-        "DeviceKey": str,
-        "DeviceAttributes": List[AttributeTypeTypeDef],
-        "DeviceCreateDate": datetime,
-        "DeviceLastModifiedDate": datetime,
-        "DeviceLastAuthenticatedDate": datetime,
-    },
-)
-
 _RequiredUpdateUserAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAttributesRequestRequestTypeDef",
     {
         "UserAttributes": Sequence[AttributeTypeTypeDef],
         "AccessToken": str,
     },
 )
@@ -1818,81 +2092,81 @@
 
 class UpdateUserAttributesRequestRequestTypeDef(
     _RequiredUpdateUserAttributesRequestRequestTypeDef,
     _OptionalUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
-AssociateSoftwareTokenResponseTypeDef = TypedDict(
-    "AssociateSoftwareTokenResponseTypeDef",
+AssociateSoftwareTokenResponseOutputTypeDef = TypedDict(
+    "AssociateSoftwareTokenResponseOutputTypeDef",
     {
         "SecretCode": str,
         "Session": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfirmDeviceResponseTypeDef = TypedDict(
-    "ConfirmDeviceResponseTypeDef",
+ConfirmDeviceResponseOutputTypeDef = TypedDict(
+    "ConfirmDeviceResponseOutputTypeDef",
     {
         "UserConfirmationNecessary": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateUserPoolDomainResponseTypeDef = TypedDict(
-    "CreateUserPoolDomainResponseTypeDef",
+CreateUserPoolDomainResponseOutputTypeDef = TypedDict(
+    "CreateUserPoolDomainResponseOutputTypeDef",
     {
         "CloudFrontDomain": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCSVHeaderResponseTypeDef = TypedDict(
-    "GetCSVHeaderResponseTypeDef",
+GetCSVHeaderResponseOutputTypeDef = TypedDict(
+    "GetCSVHeaderResponseOutputTypeDef",
     {
         "UserPoolId": str,
         "CSVHeader": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetSigningCertificateResponseTypeDef = TypedDict(
-    "GetSigningCertificateResponseTypeDef",
+GetSigningCertificateResponseOutputTypeDef = TypedDict(
+    "GetSigningCertificateResponseOutputTypeDef",
     {
         "Certificate": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateUserPoolDomainResponseTypeDef = TypedDict(
-    "UpdateUserPoolDomainResponseTypeDef",
+UpdateUserPoolDomainResponseOutputTypeDef = TypedDict(
+    "UpdateUserPoolDomainResponseOutputTypeDef",
     {
         "CloudFrontDomain": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VerifySoftwareTokenResponseTypeDef = TypedDict(
-    "VerifySoftwareTokenResponseTypeDef",
+VerifySoftwareTokenResponseOutputTypeDef = TypedDict(
+    "VerifySoftwareTokenResponseOutputTypeDef",
     {
         "Status": VerifySoftwareTokenResponseTypeType,
         "Session": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1909,69 +2183,63 @@
     {
         "UserPoolId": str,
         "DestinationUser": ProviderUserIdentifierTypeTypeDef,
         "SourceUser": ProviderUserIdentifierTypeTypeDef,
     },
 )
 
-AdminGetUserResponseTypeDef = TypedDict(
-    "AdminGetUserResponseTypeDef",
+DeviceTypeOutputTypeDef = TypedDict(
+    "DeviceTypeOutputTypeDef",
+    {
+        "DeviceKey": str,
+        "DeviceAttributes": List[AttributeTypeOutputTypeDef],
+        "DeviceCreateDate": datetime,
+        "DeviceLastModifiedDate": datetime,
+        "DeviceLastAuthenticatedDate": datetime,
+    },
+)
+
+AdminGetUserResponseOutputTypeDef = TypedDict(
+    "AdminGetUserResponseOutputTypeDef",
     {
         "Username": str,
-        "UserAttributes": List[AttributeTypeTypeDef],
+        "UserAttributes": List[AttributeTypeOutputTypeDef],
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
-        "MFAOptions": List[MFAOptionTypeTypeDef],
+        "MFAOptions": List[MFAOptionTypeOutputTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminSetUserSettingsRequestRequestTypeDef = TypedDict(
-    "AdminSetUserSettingsRequestRequestTypeDef",
-    {
-        "UserPoolId": str,
-        "Username": str,
-        "MFAOptions": Sequence[MFAOptionTypeTypeDef],
-    },
-)
-
-GetUserResponseTypeDef = TypedDict(
-    "GetUserResponseTypeDef",
+GetUserResponseOutputTypeDef = TypedDict(
+    "GetUserResponseOutputTypeDef",
     {
         "Username": str,
-        "UserAttributes": List[AttributeTypeTypeDef],
-        "MFAOptions": List[MFAOptionTypeTypeDef],
+        "UserAttributes": List[AttributeTypeOutputTypeDef],
+        "MFAOptions": List[MFAOptionTypeOutputTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetUserSettingsRequestRequestTypeDef = TypedDict(
-    "SetUserSettingsRequestRequestTypeDef",
-    {
-        "AccessToken": str,
-        "MFAOptions": Sequence[MFAOptionTypeTypeDef],
-    },
-)
-
-UserTypeTypeDef = TypedDict(
-    "UserTypeTypeDef",
+UserTypeOutputTypeDef = TypedDict(
+    "UserTypeOutputTypeDef",
     {
         "Username": str,
-        "Attributes": List[AttributeTypeTypeDef],
+        "Attributes": List[AttributeTypeOutputTypeDef],
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
-        "MFAOptions": List[MFAOptionTypeTypeDef],
+        "MFAOptions": List[MFAOptionTypeOutputTypeDef],
     },
 )
 
 _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
     "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     {
         "Username": str,
@@ -2140,52 +2408,52 @@
 
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
-AdminListGroupsForUserResponseTypeDef = TypedDict(
-    "AdminListGroupsForUserResponseTypeDef",
+AdminListGroupsForUserResponseOutputTypeDef = TypedDict(
+    "AdminListGroupsForUserResponseOutputTypeDef",
     {
-        "Groups": List[GroupTypeTypeDef],
+        "Groups": List[GroupTypeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
+CreateGroupResponseOutputTypeDef = TypedDict(
+    "CreateGroupResponseOutputTypeDef",
     {
-        "Group": GroupTypeTypeDef,
+        "Group": GroupTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
+GetGroupResponseOutputTypeDef = TypedDict(
+    "GetGroupResponseOutputTypeDef",
     {
-        "Group": GroupTypeTypeDef,
+        "Group": GroupTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListGroupsResponseTypeDef = TypedDict(
-    "ListGroupsResponseTypeDef",
+ListGroupsResponseOutputTypeDef = TypedDict(
+    "ListGroupsResponseOutputTypeDef",
     {
-        "Groups": List[GroupTypeTypeDef],
+        "Groups": List[GroupTypeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateGroupResponseTypeDef = TypedDict(
-    "UpdateGroupResponseTypeDef",
+UpdateGroupResponseOutputTypeDef = TypedDict(
+    "UpdateGroupResponseOutputTypeDef",
     {
-        "Group": GroupTypeTypeDef,
+        "Group": GroupTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef",
     {
@@ -2225,89 +2493,126 @@
 
 class SetUserMFAPreferenceRequestRequestTypeDef(
     _RequiredSetUserMFAPreferenceRequestRequestTypeDef,
     _OptionalSetUserMFAPreferenceRequestRequestTypeDef,
 ):
     pass
 
-AuthEventTypeTypeDef = TypedDict(
-    "AuthEventTypeTypeDef",
+AdminSetUserSettingsRequestRequestTypeDef = TypedDict(
+    "AdminSetUserSettingsRequestRequestTypeDef",
+    {
+        "UserPoolId": str,
+        "Username": str,
+        "MFAOptions": Sequence[MFAOptionTypeTypeDef],
+    },
+)
+
+SetUserSettingsRequestRequestTypeDef = TypedDict(
+    "SetUserSettingsRequestRequestTypeDef",
+    {
+        "AccessToken": str,
+        "MFAOptions": Sequence[MFAOptionTypeTypeDef],
+    },
+)
+
+AuthEventTypeOutputTypeDef = TypedDict(
+    "AuthEventTypeOutputTypeDef",
     {
         "EventId": str,
         "EventType": EventTypeType,
         "CreationDate": datetime,
         "EventResponse": EventResponseTypeType,
-        "EventRisk": EventRiskTypeTypeDef,
-        "ChallengeResponses": List[ChallengeResponseTypeTypeDef],
-        "EventContextData": EventContextDataTypeTypeDef,
-        "EventFeedback": EventFeedbackTypeTypeDef,
+        "EventRisk": EventRiskTypeOutputTypeDef,
+        "ChallengeResponses": List[ChallengeResponseTypeOutputTypeDef],
+        "EventContextData": EventContextDataTypeOutputTypeDef,
+        "EventFeedback": EventFeedbackTypeOutputTypeDef,
     },
 )
 
-AuthenticationResultTypeTypeDef = TypedDict(
-    "AuthenticationResultTypeTypeDef",
+AuthenticationResultTypeOutputTypeDef = TypedDict(
+    "AuthenticationResultTypeOutputTypeDef",
     {
         "AccessToken": str,
         "ExpiresIn": int,
         "TokenType": str,
         "RefreshToken": str,
         "IdToken": str,
-        "NewDeviceMetadata": NewDeviceMetadataTypeTypeDef,
+        "NewDeviceMetadata": NewDeviceMetadataTypeOutputTypeDef,
     },
 )
 
-ForgotPasswordResponseTypeDef = TypedDict(
-    "ForgotPasswordResponseTypeDef",
+ForgotPasswordResponseOutputTypeDef = TypedDict(
+    "ForgotPasswordResponseOutputTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetUserAttributeVerificationCodeResponseTypeDef = TypedDict(
-    "GetUserAttributeVerificationCodeResponseTypeDef",
+GetUserAttributeVerificationCodeResponseOutputTypeDef = TypedDict(
+    "GetUserAttributeVerificationCodeResponseOutputTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResendConfirmationCodeResponseTypeDef = TypedDict(
-    "ResendConfirmationCodeResponseTypeDef",
+ResendConfirmationCodeResponseOutputTypeDef = TypedDict(
+    "ResendConfirmationCodeResponseOutputTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SignUpResponseTypeDef = TypedDict(
-    "SignUpResponseTypeDef",
+SignUpResponseOutputTypeDef = TypedDict(
+    "SignUpResponseOutputTypeDef",
     {
         "UserConfirmed": bool,
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
         "UserSub": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateUserAttributesResponseTypeDef = TypedDict(
-    "UpdateUserAttributesResponseTypeDef",
+UpdateUserAttributesResponseOutputTypeDef = TypedDict(
+    "UpdateUserAttributesResponseOutputTypeDef",
     {
-        "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
+        "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
-    "CompromisedCredentialsRiskConfigurationTypeTypeDef",
+CompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
+    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     {
         "EventFilter": List[EventFilterTypeType],
+        "Actions": CompromisedCredentialsActionsTypeOutputTypeDef,
+    },
+)
+
+_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
+    "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
+    {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
     },
 )
+_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
+    "_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef",
+    {
+        "EventFilter": Sequence[EventFilterTypeType],
+    },
+    total=False,
+)
+
+class CompromisedCredentialsRiskConfigurationTypeTypeDef(
+    _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef,
+    _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef,
+):
+    pass
 
 _RequiredConfirmDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
         "DeviceKey": str,
     },
@@ -2514,42 +2819,42 @@
     },
     total=False,
 )
 
 class ContextDataTypeTypeDef(_RequiredContextDataTypeTypeDef, _OptionalContextDataTypeTypeDef):
     pass
 
-CreateIdentityProviderResponseTypeDef = TypedDict(
-    "CreateIdentityProviderResponseTypeDef",
+CreateIdentityProviderResponseOutputTypeDef = TypedDict(
+    "CreateIdentityProviderResponseOutputTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeTypeDef,
+        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeIdentityProviderResponseTypeDef = TypedDict(
-    "DescribeIdentityProviderResponseTypeDef",
+DescribeIdentityProviderResponseOutputTypeDef = TypedDict(
+    "DescribeIdentityProviderResponseOutputTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeTypeDef,
+        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetIdentityProviderByIdentifierResponseTypeDef = TypedDict(
-    "GetIdentityProviderByIdentifierResponseTypeDef",
+GetIdentityProviderByIdentifierResponseOutputTypeDef = TypedDict(
+    "GetIdentityProviderByIdentifierResponseOutputTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeTypeDef,
+        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateIdentityProviderResponseTypeDef = TypedDict(
-    "UpdateIdentityProviderResponseTypeDef",
+UpdateIdentityProviderResponseOutputTypeDef = TypedDict(
+    "UpdateIdentityProviderResponseOutputTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeTypeDef,
+        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceServerRequestRequestTypeDef",
     {
@@ -2568,24 +2873,14 @@
 
 class CreateResourceServerRequestRequestTypeDef(
     _RequiredCreateResourceServerRequestRequestTypeDef,
     _OptionalCreateResourceServerRequestRequestTypeDef,
 ):
     pass
 
-ResourceServerTypeTypeDef = TypedDict(
-    "ResourceServerTypeTypeDef",
-    {
-        "UserPoolId": str,
-        "Identifier": str,
-        "Name": str,
-        "Scopes": List[ResourceServerScopeTypeTypeDef],
-    },
-)
-
 _RequiredUpdateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceServerRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Identifier": str,
         "Name": str,
     },
@@ -2600,51 +2895,51 @@
 
 class UpdateResourceServerRequestRequestTypeDef(
     _RequiredUpdateResourceServerRequestRequestTypeDef,
     _OptionalUpdateResourceServerRequestRequestTypeDef,
 ):
     pass
 
-CreateUserImportJobResponseTypeDef = TypedDict(
-    "CreateUserImportJobResponseTypeDef",
+CreateUserImportJobResponseOutputTypeDef = TypedDict(
+    "CreateUserImportJobResponseOutputTypeDef",
     {
-        "UserImportJob": UserImportJobTypeTypeDef,
+        "UserImportJob": UserImportJobTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeUserImportJobResponseTypeDef = TypedDict(
-    "DescribeUserImportJobResponseTypeDef",
+DescribeUserImportJobResponseOutputTypeDef = TypedDict(
+    "DescribeUserImportJobResponseOutputTypeDef",
     {
-        "UserImportJob": UserImportJobTypeTypeDef,
+        "UserImportJob": UserImportJobTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserImportJobsResponseTypeDef = TypedDict(
-    "ListUserImportJobsResponseTypeDef",
+ListUserImportJobsResponseOutputTypeDef = TypedDict(
+    "ListUserImportJobsResponseOutputTypeDef",
     {
-        "UserImportJobs": List[UserImportJobTypeTypeDef],
+        "UserImportJobs": List[UserImportJobTypeOutputTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartUserImportJobResponseTypeDef = TypedDict(
-    "StartUserImportJobResponseTypeDef",
+StartUserImportJobResponseOutputTypeDef = TypedDict(
+    "StartUserImportJobResponseOutputTypeDef",
     {
-        "UserImportJob": UserImportJobTypeTypeDef,
+        "UserImportJob": UserImportJobTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopUserImportJobResponseTypeDef = TypedDict(
-    "StopUserImportJobResponseTypeDef",
+StopUserImportJobResponseOutputTypeDef = TypedDict(
+    "StopUserImportJobResponseOutputTypeDef",
     {
-        "UserImportJob": UserImportJobTypeTypeDef,
+        "UserImportJob": UserImportJobTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolClientRequestRequestTypeDef",
     {
@@ -2721,45 +3016,14 @@
 
 class UpdateUserPoolClientRequestRequestTypeDef(
     _RequiredUpdateUserPoolClientRequestRequestTypeDef,
     _OptionalUpdateUserPoolClientRequestRequestTypeDef,
 ):
     pass
 
-UserPoolClientTypeTypeDef = TypedDict(
-    "UserPoolClientTypeTypeDef",
-    {
-        "UserPoolId": str,
-        "ClientName": str,
-        "ClientId": str,
-        "ClientSecret": str,
-        "LastModifiedDate": datetime,
-        "CreationDate": datetime,
-        "RefreshTokenValidity": int,
-        "AccessTokenValidity": int,
-        "IdTokenValidity": int,
-        "TokenValidityUnits": TokenValidityUnitsTypeTypeDef,
-        "ReadAttributes": List[str],
-        "WriteAttributes": List[str],
-        "ExplicitAuthFlows": List[ExplicitAuthFlowsTypeType],
-        "SupportedIdentityProviders": List[str],
-        "CallbackURLs": List[str],
-        "LogoutURLs": List[str],
-        "DefaultRedirectURI": str,
-        "AllowedOAuthFlows": List[OAuthFlowTypeType],
-        "AllowedOAuthScopes": List[str],
-        "AllowedOAuthFlowsUserPoolClient": bool,
-        "AnalyticsConfiguration": AnalyticsConfigurationTypeTypeDef,
-        "PreventUserExistenceErrors": PreventUserExistenceErrorTypesType,
-        "EnableTokenRevocation": bool,
-        "EnablePropagateAdditionalUserContextData": bool,
-        "AuthSessionValidity": int,
-    },
-)
-
 _RequiredCreateUserPoolDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolDomainRequestRequestTypeDef",
     {
         "Domain": str,
         "UserPoolId": str,
     },
 )
@@ -2773,28 +3037,14 @@
 
 class CreateUserPoolDomainRequestRequestTypeDef(
     _RequiredCreateUserPoolDomainRequestRequestTypeDef,
     _OptionalCreateUserPoolDomainRequestRequestTypeDef,
 ):
     pass
 
-DomainDescriptionTypeTypeDef = TypedDict(
-    "DomainDescriptionTypeTypeDef",
-    {
-        "UserPoolId": str,
-        "AWSAccountId": str,
-        "Domain": str,
-        "S3Bucket": str,
-        "CloudFrontDistribution": str,
-        "Version": str,
-        "Status": DomainStatusTypeType,
-        "CustomDomainConfig": CustomDomainConfigTypeTypeDef,
-    },
-)
-
 UpdateUserPoolDomainRequestRequestTypeDef = TypedDict(
     "UpdateUserPoolDomainRequestRequestTypeDef",
     {
         "Domain": str,
         "UserPoolId": str,
         "CustomDomainConfig": CustomDomainConfigTypeTypeDef,
     },
@@ -2802,14 +3052,48 @@
 
 SmsMfaConfigTypeTypeDef = TypedDict(
     "SmsMfaConfigTypeTypeDef",
     {
         "SmsAuthenticationMessage": str,
         "SmsConfiguration": SmsConfigurationTypeTypeDef,
     },
+    total=False,
+)
+
+DomainDescriptionTypeOutputTypeDef = TypedDict(
+    "DomainDescriptionTypeOutputTypeDef",
+    {
+        "UserPoolId": str,
+        "AWSAccountId": str,
+        "Domain": str,
+        "S3Bucket": str,
+        "CloudFrontDistribution": str,
+        "Version": str,
+        "Status": DomainStatusTypeType,
+        "CustomDomainConfig": CustomDomainConfigTypeOutputTypeDef,
+    },
+)
+
+LambdaConfigTypeOutputTypeDef = TypedDict(
+    "LambdaConfigTypeOutputTypeDef",
+    {
+        "PreSignUp": str,
+        "CustomMessage": str,
+        "PostConfirmation": str,
+        "PreAuthentication": str,
+        "PostAuthentication": str,
+        "DefineAuthChallenge": str,
+        "CreateAuthChallenge": str,
+        "VerifyAuthChallengeResponse": str,
+        "PreTokenGeneration": str,
+        "UserMigration": str,
+        "CustomSMSSender": CustomSMSLambdaVersionConfigTypeOutputTypeDef,
+        "CustomEmailSender": CustomEmailLambdaVersionConfigTypeOutputTypeDef,
+        "KMSKeyID": str,
+    },
 )
 
 LambdaConfigTypeTypeDef = TypedDict(
     "LambdaConfigTypeTypeDef",
     {
         "PreSignUp": str,
         "CustomMessage": str,
@@ -2824,191 +3108,283 @@
         "CustomSMSSender": CustomSMSLambdaVersionConfigTypeTypeDef,
         "CustomEmailSender": CustomEmailLambdaVersionConfigTypeTypeDef,
         "KMSKeyID": str,
     },
     total=False,
 )
 
-GetUICustomizationResponseTypeDef = TypedDict(
-    "GetUICustomizationResponseTypeDef",
+GetUICustomizationResponseOutputTypeDef = TypedDict(
+    "GetUICustomizationResponseOutputTypeDef",
     {
-        "UICustomization": UICustomizationTypeTypeDef,
+        "UICustomization": UICustomizationTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetUICustomizationResponseTypeDef = TypedDict(
-    "SetUICustomizationResponseTypeDef",
+SetUICustomizationResponseOutputTypeDef = TypedDict(
+    "SetUICustomizationResponseOutputTypeDef",
     {
-        "UICustomization": UICustomizationTypeTypeDef,
+        "UICustomization": UICustomizationTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListIdentityProvidersResponseTypeDef = TypedDict(
-    "ListIdentityProvidersResponseTypeDef",
+ListIdentityProvidersResponseOutputTypeDef = TypedDict(
+    "ListIdentityProvidersResponseOutputTypeDef",
     {
-        "Providers": List[ProviderDescriptionTypeDef],
+        "Providers": List[ProviderDescriptionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserPoolClientsResponseTypeDef = TypedDict(
-    "ListUserPoolClientsResponseTypeDef",
+ListUserPoolClientsResponseOutputTypeDef = TypedDict(
+    "ListUserPoolClientsResponseOutputTypeDef",
     {
-        "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
+        "UserPoolClients": List[UserPoolClientDescriptionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NotifyConfigurationTypeTypeDef = TypedDict(
-    "NotifyConfigurationTypeTypeDef",
+NotifyConfigurationTypeOutputTypeDef = TypedDict(
+    "NotifyConfigurationTypeOutputTypeDef",
     {
         "From": str,
         "ReplyTo": str,
         "SourceArn": str,
+        "BlockEmail": NotifyEmailTypeOutputTypeDef,
+        "NoActionEmail": NotifyEmailTypeOutputTypeDef,
+        "MfaEmail": NotifyEmailTypeOutputTypeDef,
+    },
+)
+
+_RequiredNotifyConfigurationTypeTypeDef = TypedDict(
+    "_RequiredNotifyConfigurationTypeTypeDef",
+    {
+        "SourceArn": str,
+    },
+)
+_OptionalNotifyConfigurationTypeTypeDef = TypedDict(
+    "_OptionalNotifyConfigurationTypeTypeDef",
+    {
+        "From": str,
+        "ReplyTo": str,
         "BlockEmail": NotifyEmailTypeTypeDef,
         "NoActionEmail": NotifyEmailTypeTypeDef,
         "MfaEmail": NotifyEmailTypeTypeDef,
     },
+    total=False,
+)
+
+class NotifyConfigurationTypeTypeDef(
+    _RequiredNotifyConfigurationTypeTypeDef, _OptionalNotifyConfigurationTypeTypeDef
+):
+    pass
+
+UserPoolPolicyTypeOutputTypeDef = TypedDict(
+    "UserPoolPolicyTypeOutputTypeDef",
+    {
+        "PasswordPolicy": PasswordPolicyTypeOutputTypeDef,
+    },
 )
 
 UserPoolPolicyTypeTypeDef = TypedDict(
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
 
+ResourceServerTypeOutputTypeDef = TypedDict(
+    "ResourceServerTypeOutputTypeDef",
+    {
+        "UserPoolId": str,
+        "Identifier": str,
+        "Name": str,
+        "Scopes": List[ResourceServerScopeTypeOutputTypeDef],
+    },
+)
+
+SchemaAttributeTypeOutputTypeDef = TypedDict(
+    "SchemaAttributeTypeOutputTypeDef",
+    {
+        "Name": str,
+        "AttributeDataType": AttributeDataTypeType,
+        "DeveloperOnlyAttribute": bool,
+        "Mutable": bool,
+        "Required": bool,
+        "NumberAttributeConstraints": NumberAttributeConstraintsTypeOutputTypeDef,
+        "StringAttributeConstraints": StringAttributeConstraintsTypeOutputTypeDef,
+    },
+)
+
 SchemaAttributeTypeTypeDef = TypedDict(
     "SchemaAttributeTypeTypeDef",
     {
         "Name": str,
         "AttributeDataType": AttributeDataTypeType,
         "DeveloperOnlyAttribute": bool,
         "Mutable": bool,
         "Required": bool,
         "NumberAttributeConstraints": NumberAttributeConstraintsTypeTypeDef,
         "StringAttributeConstraints": StringAttributeConstraintsTypeTypeDef,
     },
     total=False,
 )
 
-AdminGetDeviceResponseTypeDef = TypedDict(
-    "AdminGetDeviceResponseTypeDef",
+SmsMfaConfigTypeOutputTypeDef = TypedDict(
+    "SmsMfaConfigTypeOutputTypeDef",
+    {
+        "SmsAuthenticationMessage": str,
+        "SmsConfiguration": SmsConfigurationTypeOutputTypeDef,
+    },
+)
+
+UserPoolClientTypeOutputTypeDef = TypedDict(
+    "UserPoolClientTypeOutputTypeDef",
+    {
+        "UserPoolId": str,
+        "ClientName": str,
+        "ClientId": str,
+        "ClientSecret": str,
+        "LastModifiedDate": datetime,
+        "CreationDate": datetime,
+        "RefreshTokenValidity": int,
+        "AccessTokenValidity": int,
+        "IdTokenValidity": int,
+        "TokenValidityUnits": TokenValidityUnitsTypeOutputTypeDef,
+        "ReadAttributes": List[str],
+        "WriteAttributes": List[str],
+        "ExplicitAuthFlows": List[ExplicitAuthFlowsTypeType],
+        "SupportedIdentityProviders": List[str],
+        "CallbackURLs": List[str],
+        "LogoutURLs": List[str],
+        "DefaultRedirectURI": str,
+        "AllowedOAuthFlows": List[OAuthFlowTypeType],
+        "AllowedOAuthScopes": List[str],
+        "AllowedOAuthFlowsUserPoolClient": bool,
+        "AnalyticsConfiguration": AnalyticsConfigurationTypeOutputTypeDef,
+        "PreventUserExistenceErrors": PreventUserExistenceErrorTypesType,
+        "EnableTokenRevocation": bool,
+        "EnablePropagateAdditionalUserContextData": bool,
+        "AuthSessionValidity": int,
+    },
+)
+
+AdminGetDeviceResponseOutputTypeDef = TypedDict(
+    "AdminGetDeviceResponseOutputTypeDef",
     {
-        "Device": DeviceTypeTypeDef,
+        "Device": DeviceTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminListDevicesResponseTypeDef = TypedDict(
-    "AdminListDevicesResponseTypeDef",
+AdminListDevicesResponseOutputTypeDef = TypedDict(
+    "AdminListDevicesResponseOutputTypeDef",
     {
-        "Devices": List[DeviceTypeTypeDef],
+        "Devices": List[DeviceTypeOutputTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetDeviceResponseTypeDef = TypedDict(
-    "GetDeviceResponseTypeDef",
+GetDeviceResponseOutputTypeDef = TypedDict(
+    "GetDeviceResponseOutputTypeDef",
     {
-        "Device": DeviceTypeTypeDef,
+        "Device": DeviceTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDevicesResponseTypeDef = TypedDict(
-    "ListDevicesResponseTypeDef",
+ListDevicesResponseOutputTypeDef = TypedDict(
+    "ListDevicesResponseOutputTypeDef",
     {
-        "Devices": List[DeviceTypeTypeDef],
+        "Devices": List[DeviceTypeOutputTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminCreateUserResponseTypeDef = TypedDict(
-    "AdminCreateUserResponseTypeDef",
+AdminCreateUserResponseOutputTypeDef = TypedDict(
+    "AdminCreateUserResponseOutputTypeDef",
     {
-        "User": UserTypeTypeDef,
+        "User": UserTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUsersInGroupResponseTypeDef = TypedDict(
-    "ListUsersInGroupResponseTypeDef",
+ListUsersInGroupResponseOutputTypeDef = TypedDict(
+    "ListUsersInGroupResponseOutputTypeDef",
     {
-        "Users": List[UserTypeTypeDef],
+        "Users": List[UserTypeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUsersResponseTypeDef = TypedDict(
-    "ListUsersResponseTypeDef",
+ListUsersResponseOutputTypeDef = TypedDict(
+    "ListUsersResponseOutputTypeDef",
     {
-        "Users": List[UserTypeTypeDef],
+        "Users": List[UserTypeOutputTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminListUserAuthEventsResponseTypeDef = TypedDict(
-    "AdminListUserAuthEventsResponseTypeDef",
+AdminListUserAuthEventsResponseOutputTypeDef = TypedDict(
+    "AdminListUserAuthEventsResponseOutputTypeDef",
     {
-        "AuthEvents": List[AuthEventTypeTypeDef],
+        "AuthEvents": List[AuthEventTypeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminInitiateAuthResponseTypeDef = TypedDict(
-    "AdminInitiateAuthResponseTypeDef",
+AdminInitiateAuthResponseOutputTypeDef = TypedDict(
+    "AdminInitiateAuthResponseOutputTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminRespondToAuthChallengeResponseTypeDef = TypedDict(
-    "AdminRespondToAuthChallengeResponseTypeDef",
+AdminRespondToAuthChallengeResponseOutputTypeDef = TypedDict(
+    "AdminRespondToAuthChallengeResponseOutputTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InitiateAuthResponseTypeDef = TypedDict(
-    "InitiateAuthResponseTypeDef",
+InitiateAuthResponseOutputTypeDef = TypedDict(
+    "InitiateAuthResponseOutputTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RespondToAuthChallengeResponseTypeDef = TypedDict(
-    "RespondToAuthChallengeResponseTypeDef",
+RespondToAuthChallengeResponseOutputTypeDef = TypedDict(
+    "RespondToAuthChallengeResponseOutputTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
@@ -3055,89 +3431,14 @@
 
 class AdminRespondToAuthChallengeRequestRequestTypeDef(
     _RequiredAdminRespondToAuthChallengeRequestRequestTypeDef,
     _OptionalAdminRespondToAuthChallengeRequestRequestTypeDef,
 ):
     pass
 
-CreateResourceServerResponseTypeDef = TypedDict(
-    "CreateResourceServerResponseTypeDef",
-    {
-        "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeResourceServerResponseTypeDef = TypedDict(
-    "DescribeResourceServerResponseTypeDef",
-    {
-        "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListResourceServersResponseTypeDef = TypedDict(
-    "ListResourceServersResponseTypeDef",
-    {
-        "ResourceServers": List[ResourceServerTypeTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateResourceServerResponseTypeDef = TypedDict(
-    "UpdateResourceServerResponseTypeDef",
-    {
-        "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserPoolClientResponseTypeDef = TypedDict(
-    "CreateUserPoolClientResponseTypeDef",
-    {
-        "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeUserPoolClientResponseTypeDef = TypedDict(
-    "DescribeUserPoolClientResponseTypeDef",
-    {
-        "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateUserPoolClientResponseTypeDef = TypedDict(
-    "UpdateUserPoolClientResponseTypeDef",
-    {
-        "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeUserPoolDomainResponseTypeDef = TypedDict(
-    "DescribeUserPoolDomainResponseTypeDef",
-    {
-        "DomainDescription": DomainDescriptionTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUserPoolMfaConfigResponseTypeDef = TypedDict(
-    "GetUserPoolMfaConfigResponseTypeDef",
-    {
-        "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
-        "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
-        "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredSetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalSetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
@@ -3152,43 +3453,61 @@
 
 class SetUserPoolMfaConfigRequestRequestTypeDef(
     _RequiredSetUserPoolMfaConfigRequestRequestTypeDef,
     _OptionalSetUserPoolMfaConfigRequestRequestTypeDef,
 ):
     pass
 
-SetUserPoolMfaConfigResponseTypeDef = TypedDict(
-    "SetUserPoolMfaConfigResponseTypeDef",
+DescribeUserPoolDomainResponseOutputTypeDef = TypedDict(
+    "DescribeUserPoolDomainResponseOutputTypeDef",
     {
-        "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
-        "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
-        "MfaConfiguration": UserPoolMfaTypeType,
+        "DomainDescription": DomainDescriptionTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserPoolDescriptionTypeTypeDef = TypedDict(
-    "UserPoolDescriptionTypeTypeDef",
+UserPoolDescriptionTypeOutputTypeDef = TypedDict(
+    "UserPoolDescriptionTypeOutputTypeDef",
     {
         "Id": str,
         "Name": str,
-        "LambdaConfig": LambdaConfigTypeTypeDef,
+        "LambdaConfig": LambdaConfigTypeOutputTypeDef,
         "Status": StatusTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
 )
 
-AccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
-    "AccountTakeoverRiskConfigurationTypeTypeDef",
+AccountTakeoverRiskConfigurationTypeOutputTypeDef = TypedDict(
+    "AccountTakeoverRiskConfigurationTypeOutputTypeDef",
+    {
+        "NotifyConfiguration": NotifyConfigurationTypeOutputTypeDef,
+        "Actions": AccountTakeoverActionsTypeOutputTypeDef,
+    },
+)
+
+_RequiredAccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
+    "_RequiredAccountTakeoverRiskConfigurationTypeTypeDef",
     {
-        "NotifyConfiguration": NotifyConfigurationTypeTypeDef,
         "Actions": AccountTakeoverActionsTypeTypeDef,
     },
 )
+_OptionalAccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
+    "_OptionalAccountTakeoverRiskConfigurationTypeTypeDef",
+    {
+        "NotifyConfiguration": NotifyConfigurationTypeTypeDef,
+    },
+    total=False,
+)
+
+class AccountTakeoverRiskConfigurationTypeTypeDef(
+    _RequiredAccountTakeoverRiskConfigurationTypeTypeDef,
+    _OptionalAccountTakeoverRiskConfigurationTypeTypeDef,
+):
+    pass
 
 _RequiredUpdateUserPoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
@@ -3218,14 +3537,86 @@
 )
 
 class UpdateUserPoolRequestRequestTypeDef(
     _RequiredUpdateUserPoolRequestRequestTypeDef, _OptionalUpdateUserPoolRequestRequestTypeDef
 ):
     pass
 
+CreateResourceServerResponseOutputTypeDef = TypedDict(
+    "CreateResourceServerResponseOutputTypeDef",
+    {
+        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeResourceServerResponseOutputTypeDef = TypedDict(
+    "DescribeResourceServerResponseOutputTypeDef",
+    {
+        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourceServersResponseOutputTypeDef = TypedDict(
+    "ListResourceServersResponseOutputTypeDef",
+    {
+        "ResourceServers": List[ResourceServerTypeOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateResourceServerResponseOutputTypeDef = TypedDict(
+    "UpdateResourceServerResponseOutputTypeDef",
+    {
+        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UserPoolTypeOutputTypeDef = TypedDict(
+    "UserPoolTypeOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Policies": UserPoolPolicyTypeOutputTypeDef,
+        "DeletionProtection": DeletionProtectionTypeType,
+        "LambdaConfig": LambdaConfigTypeOutputTypeDef,
+        "Status": StatusTypeType,
+        "LastModifiedDate": datetime,
+        "CreationDate": datetime,
+        "SchemaAttributes": List[SchemaAttributeTypeOutputTypeDef],
+        "AutoVerifiedAttributes": List[VerifiedAttributeTypeType],
+        "AliasAttributes": List[AliasAttributeTypeType],
+        "UsernameAttributes": List[UsernameAttributeTypeType],
+        "SmsVerificationMessage": str,
+        "EmailVerificationMessage": str,
+        "EmailVerificationSubject": str,
+        "VerificationMessageTemplate": VerificationMessageTemplateTypeOutputTypeDef,
+        "SmsAuthenticationMessage": str,
+        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeOutputTypeDef,
+        "MfaConfiguration": UserPoolMfaTypeType,
+        "DeviceConfiguration": DeviceConfigurationTypeOutputTypeDef,
+        "EstimatedNumberOfUsers": int,
+        "EmailConfiguration": EmailConfigurationTypeOutputTypeDef,
+        "SmsConfiguration": SmsConfigurationTypeOutputTypeDef,
+        "UserPoolTags": Dict[str, str],
+        "SmsConfigurationFailure": str,
+        "EmailConfigurationFailure": str,
+        "Domain": str,
+        "CustomDomain": str,
+        "AdminCreateUserConfig": AdminCreateUserConfigTypeOutputTypeDef,
+        "UserPoolAddOns": UserPoolAddOnsTypeOutputTypeDef,
+        "UsernameConfiguration": UsernameConfigurationTypeOutputTypeDef,
+        "Arn": str,
+        "AccountRecoverySetting": AccountRecoverySettingTypeOutputTypeDef,
+    },
+)
+
 AddCustomAttributesRequestRequestTypeDef = TypedDict(
     "AddCustomAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "CustomAttributes": Sequence[SchemaAttributeTypeTypeDef],
     },
 )
@@ -3266,72 +3657,77 @@
 )
 
 class CreateUserPoolRequestRequestTypeDef(
     _RequiredCreateUserPoolRequestRequestTypeDef, _OptionalCreateUserPoolRequestRequestTypeDef
 ):
     pass
 
-UserPoolTypeTypeDef = TypedDict(
-    "UserPoolTypeTypeDef",
+GetUserPoolMfaConfigResponseOutputTypeDef = TypedDict(
+    "GetUserPoolMfaConfigResponseOutputTypeDef",
     {
-        "Id": str,
-        "Name": str,
-        "Policies": UserPoolPolicyTypeTypeDef,
-        "DeletionProtection": DeletionProtectionTypeType,
-        "LambdaConfig": LambdaConfigTypeTypeDef,
-        "Status": StatusTypeType,
-        "LastModifiedDate": datetime,
-        "CreationDate": datetime,
-        "SchemaAttributes": List[SchemaAttributeTypeTypeDef],
-        "AutoVerifiedAttributes": List[VerifiedAttributeTypeType],
-        "AliasAttributes": List[AliasAttributeTypeType],
-        "UsernameAttributes": List[UsernameAttributeTypeType],
-        "SmsVerificationMessage": str,
-        "EmailVerificationMessage": str,
-        "EmailVerificationSubject": str,
-        "VerificationMessageTemplate": VerificationMessageTemplateTypeTypeDef,
-        "SmsAuthenticationMessage": str,
-        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeTypeDef,
+        "SmsMfaConfiguration": SmsMfaConfigTypeOutputTypeDef,
+        "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeOutputTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "DeviceConfiguration": DeviceConfigurationTypeTypeDef,
-        "EstimatedNumberOfUsers": int,
-        "EmailConfiguration": EmailConfigurationTypeTypeDef,
-        "SmsConfiguration": SmsConfigurationTypeTypeDef,
-        "UserPoolTags": Dict[str, str],
-        "SmsConfigurationFailure": str,
-        "EmailConfigurationFailure": str,
-        "Domain": str,
-        "CustomDomain": str,
-        "AdminCreateUserConfig": AdminCreateUserConfigTypeTypeDef,
-        "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
-        "UsernameConfiguration": UsernameConfigurationTypeTypeDef,
-        "Arn": str,
-        "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetUserPoolMfaConfigResponseOutputTypeDef = TypedDict(
+    "SetUserPoolMfaConfigResponseOutputTypeDef",
+    {
+        "SmsMfaConfiguration": SmsMfaConfigTypeOutputTypeDef,
+        "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeOutputTypeDef,
+        "MfaConfiguration": UserPoolMfaTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserPoolsResponseTypeDef = TypedDict(
-    "ListUserPoolsResponseTypeDef",
+CreateUserPoolClientResponseOutputTypeDef = TypedDict(
+    "CreateUserPoolClientResponseOutputTypeDef",
     {
-        "UserPools": List[UserPoolDescriptionTypeTypeDef],
+        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUserPoolClientResponseOutputTypeDef = TypedDict(
+    "DescribeUserPoolClientResponseOutputTypeDef",
+    {
+        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateUserPoolClientResponseOutputTypeDef = TypedDict(
+    "UpdateUserPoolClientResponseOutputTypeDef",
+    {
+        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListUserPoolsResponseOutputTypeDef = TypedDict(
+    "ListUserPoolsResponseOutputTypeDef",
+    {
+        "UserPools": List[UserPoolDescriptionTypeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RiskConfigurationTypeTypeDef = TypedDict(
-    "RiskConfigurationTypeTypeDef",
+RiskConfigurationTypeOutputTypeDef = TypedDict(
+    "RiskConfigurationTypeOutputTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "CompromisedCredentialsRiskConfiguration": (
-            CompromisedCredentialsRiskConfigurationTypeTypeDef
+            CompromisedCredentialsRiskConfigurationTypeOutputTypeDef
         ),
-        "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
-        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
+        "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeOutputTypeDef,
+        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeOutputTypeDef,
         "LastModifiedDate": datetime,
     },
 )
 
 _RequiredSetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetRiskConfigurationRequestRequestTypeDef",
     {
@@ -3353,38 +3749,38 @@
 
 class SetRiskConfigurationRequestRequestTypeDef(
     _RequiredSetRiskConfigurationRequestRequestTypeDef,
     _OptionalSetRiskConfigurationRequestRequestTypeDef,
 ):
     pass
 
-CreateUserPoolResponseTypeDef = TypedDict(
-    "CreateUserPoolResponseTypeDef",
+CreateUserPoolResponseOutputTypeDef = TypedDict(
+    "CreateUserPoolResponseOutputTypeDef",
     {
-        "UserPool": UserPoolTypeTypeDef,
+        "UserPool": UserPoolTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeUserPoolResponseTypeDef = TypedDict(
-    "DescribeUserPoolResponseTypeDef",
+DescribeUserPoolResponseOutputTypeDef = TypedDict(
+    "DescribeUserPoolResponseOutputTypeDef",
     {
-        "UserPool": UserPoolTypeTypeDef,
+        "UserPool": UserPoolTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeRiskConfigurationResponseTypeDef = TypedDict(
-    "DescribeRiskConfigurationResponseTypeDef",
+DescribeRiskConfigurationResponseOutputTypeDef = TypedDict(
+    "DescribeRiskConfigurationResponseOutputTypeDef",
     {
-        "RiskConfiguration": RiskConfigurationTypeTypeDef,
+        "RiskConfiguration": RiskConfigurationTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetRiskConfigurationResponseTypeDef = TypedDict(
-    "SetRiskConfigurationResponseTypeDef",
+SetRiskConfigurationResponseOutputTypeDef = TypedDict(
+    "SetRiskConfigurationResponseOutputTypeDef",
     {
-        "RiskConfiguration": RiskConfigurationTypeTypeDef,
+        "RiskConfiguration": RiskConfigurationTypeOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/PKG-INFO` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.28.3
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -394,73 +394,83 @@
 ### Typed dictionaries
 
 `mypy_boto3_cognito_idp.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_idp.type_defs import (
+    RecoveryOptionTypeOutputTypeDef,
     RecoveryOptionTypeTypeDef,
+    AccountTakeoverActionTypeOutputTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
+    MessageTemplateTypeOutputTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
     ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
-    MFAOptionTypeTypeDef,
+    AttributeTypeOutputTypeDef,
+    MFAOptionTypeOutputTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
-    GroupTypeTypeDef,
+    GroupTypeOutputTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
+    MFAOptionTypeTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
+    AnalyticsConfigurationTypeOutputTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    ChallengeResponseTypeTypeDef,
-    EventContextDataTypeTypeDef,
-    EventFeedbackTypeTypeDef,
-    EventRiskTypeTypeDef,
-    NewDeviceMetadataTypeTypeDef,
+    ChallengeResponseTypeOutputTypeDef,
+    EventContextDataTypeOutputTypeDef,
+    EventFeedbackTypeOutputTypeDef,
+    EventRiskTypeOutputTypeDef,
+    NewDeviceMetadataTypeOutputTypeDef,
     ChangePasswordRequestRequestTypeDef,
-    CodeDeliveryDetailsTypeTypeDef,
+    CodeDeliveryDetailsTypeOutputTypeDef,
+    CompromisedCredentialsActionsTypeOutputTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    IdentityProviderTypeTypeDef,
+    IdentityProviderTypeOutputTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
-    UserImportJobTypeTypeDef,
+    UserImportJobTypeOutputTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
+    CustomDomainConfigTypeOutputTypeDef,
+    CustomEmailLambdaVersionConfigTypeOutputTypeDef,
     CustomEmailLambdaVersionConfigTypeTypeDef,
+    CustomSMSLambdaVersionConfigTypeOutputTypeDef,
     CustomSMSLambdaVersionConfigTypeTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
     DeleteResourceServerRequestRequestTypeDef,
     DeleteUserAttributesRequestRequestTypeDef,
     DeleteUserPoolClientRequestRequestTypeDef,
     DeleteUserPoolDomainRequestRequestTypeDef,
@@ -469,181 +479,206 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
+    DeviceConfigurationTypeOutputTypeDef,
+    EmailConfigurationTypeOutputTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
     GetUICustomizationRequestRequestTypeDef,
-    UICustomizationTypeTypeDef,
+    UICustomizationTypeOutputTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
-    SoftwareTokenMfaConfigTypeTypeDef,
+    SoftwareTokenMfaConfigTypeOutputTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
-    ProviderDescriptionTypeDef,
+    ProviderDescriptionOutputTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
-    UserPoolClientDescriptionTypeDef,
+    UserPoolClientDescriptionOutputTypeDef,
     ListUserPoolsRequestRequestTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
+    NotifyEmailTypeOutputTypeDef,
     NotifyEmailTypeTypeDef,
+    NumberAttributeConstraintsTypeOutputTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
+    PasswordPolicyTypeOutputTypeDef,
     PasswordPolicyTypeTypeDef,
+    ResourceServerScopeTypeOutputTypeDef,
     RevokeTokenRequestRequestTypeDef,
+    RiskExceptionConfigurationTypeOutputTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
+    StringAttributeConstraintsTypeOutputTypeDef,
     StringAttributeConstraintsTypeTypeDef,
     SetUICustomizationRequestRequestTypeDef,
+    SoftwareTokenMfaConfigTypeTypeDef,
+    SmsConfigurationTypeOutputTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    TokenValidityUnitsTypeOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
+    UserAttributeUpdateSettingsTypeOutputTypeDef,
+    UserPoolAddOnsTypeOutputTypeDef,
+    UsernameConfigurationTypeOutputTypeDef,
+    VerificationMessageTemplateTypeOutputTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
+    AccountRecoverySettingTypeOutputTypeDef,
     AccountRecoverySettingTypeTypeDef,
+    AccountTakeoverActionsTypeOutputTypeDef,
     AccountTakeoverActionsTypeTypeDef,
+    AdminCreateUserConfigTypeOutputTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
-    DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
-    ConfirmDeviceResponseTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
+    AssociateSoftwareTokenResponseOutputTypeDef,
+    ConfirmDeviceResponseOutputTypeDef,
+    CreateUserPoolDomainResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetCSVHeaderResponseTypeDef,
-    GetSigningCertificateResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
+    GetCSVHeaderResponseOutputTypeDef,
+    GetSigningCertificateResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    UpdateUserPoolDomainResponseOutputTypeDef,
+    VerifySoftwareTokenResponseOutputTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
-    AdminGetUserResponseTypeDef,
-    AdminSetUserSettingsRequestRequestTypeDef,
-    GetUserResponseTypeDef,
-    SetUserSettingsRequestRequestTypeDef,
-    UserTypeTypeDef,
+    DeviceTypeOutputTypeDef,
+    AdminGetUserResponseOutputTypeDef,
+    GetUserResponseOutputTypeDef,
+    UserTypeOutputTypeDef,
     AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
     AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
-    AdminListGroupsForUserResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    GetGroupResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    UpdateGroupResponseTypeDef,
+    AdminListGroupsForUserResponseOutputTypeDef,
+    CreateGroupResponseOutputTypeDef,
+    GetGroupResponseOutputTypeDef,
+    ListGroupsResponseOutputTypeDef,
+    UpdateGroupResponseOutputTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
-    AuthEventTypeTypeDef,
-    AuthenticationResultTypeTypeDef,
-    ForgotPasswordResponseTypeDef,
-    GetUserAttributeVerificationCodeResponseTypeDef,
-    ResendConfirmationCodeResponseTypeDef,
-    SignUpResponseTypeDef,
-    UpdateUserAttributesResponseTypeDef,
+    AdminSetUserSettingsRequestRequestTypeDef,
+    SetUserSettingsRequestRequestTypeDef,
+    AuthEventTypeOutputTypeDef,
+    AuthenticationResultTypeOutputTypeDef,
+    ForgotPasswordResponseOutputTypeDef,
+    GetUserAttributeVerificationCodeResponseOutputTypeDef,
+    ResendConfirmationCodeResponseOutputTypeDef,
+    SignUpResponseOutputTypeDef,
+    UpdateUserAttributesResponseOutputTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
     ConfirmDeviceRequestRequestTypeDef,
     ConfirmForgotPasswordRequestRequestTypeDef,
     ConfirmSignUpRequestRequestTypeDef,
     ForgotPasswordRequestRequestTypeDef,
     InitiateAuthRequestRequestTypeDef,
     ResendConfirmationCodeRequestRequestTypeDef,
     RespondToAuthChallengeRequestRequestTypeDef,
     SignUpRequestRequestTypeDef,
     ContextDataTypeTypeDef,
-    CreateIdentityProviderResponseTypeDef,
-    DescribeIdentityProviderResponseTypeDef,
-    GetIdentityProviderByIdentifierResponseTypeDef,
-    UpdateIdentityProviderResponseTypeDef,
+    CreateIdentityProviderResponseOutputTypeDef,
+    DescribeIdentityProviderResponseOutputTypeDef,
+    GetIdentityProviderByIdentifierResponseOutputTypeDef,
+    UpdateIdentityProviderResponseOutputTypeDef,
     CreateResourceServerRequestRequestTypeDef,
-    ResourceServerTypeTypeDef,
     UpdateResourceServerRequestRequestTypeDef,
-    CreateUserImportJobResponseTypeDef,
-    DescribeUserImportJobResponseTypeDef,
-    ListUserImportJobsResponseTypeDef,
-    StartUserImportJobResponseTypeDef,
-    StopUserImportJobResponseTypeDef,
+    CreateUserImportJobResponseOutputTypeDef,
+    DescribeUserImportJobResponseOutputTypeDef,
+    ListUserImportJobsResponseOutputTypeDef,
+    StartUserImportJobResponseOutputTypeDef,
+    StopUserImportJobResponseOutputTypeDef,
     CreateUserPoolClientRequestRequestTypeDef,
     UpdateUserPoolClientRequestRequestTypeDef,
-    UserPoolClientTypeTypeDef,
     CreateUserPoolDomainRequestRequestTypeDef,
-    DomainDescriptionTypeTypeDef,
     UpdateUserPoolDomainRequestRequestTypeDef,
     SmsMfaConfigTypeTypeDef,
+    DomainDescriptionTypeOutputTypeDef,
+    LambdaConfigTypeOutputTypeDef,
     LambdaConfigTypeTypeDef,
-    GetUICustomizationResponseTypeDef,
-    SetUICustomizationResponseTypeDef,
-    ListIdentityProvidersResponseTypeDef,
-    ListUserPoolClientsResponseTypeDef,
+    GetUICustomizationResponseOutputTypeDef,
+    SetUICustomizationResponseOutputTypeDef,
+    ListIdentityProvidersResponseOutputTypeDef,
+    ListUserPoolClientsResponseOutputTypeDef,
+    NotifyConfigurationTypeOutputTypeDef,
     NotifyConfigurationTypeTypeDef,
+    UserPoolPolicyTypeOutputTypeDef,
     UserPoolPolicyTypeTypeDef,
+    ResourceServerTypeOutputTypeDef,
+    SchemaAttributeTypeOutputTypeDef,
     SchemaAttributeTypeTypeDef,
-    AdminGetDeviceResponseTypeDef,
-    AdminListDevicesResponseTypeDef,
-    GetDeviceResponseTypeDef,
-    ListDevicesResponseTypeDef,
-    AdminCreateUserResponseTypeDef,
-    ListUsersInGroupResponseTypeDef,
-    ListUsersResponseTypeDef,
-    AdminListUserAuthEventsResponseTypeDef,
-    AdminInitiateAuthResponseTypeDef,
-    AdminRespondToAuthChallengeResponseTypeDef,
-    InitiateAuthResponseTypeDef,
-    RespondToAuthChallengeResponseTypeDef,
+    SmsMfaConfigTypeOutputTypeDef,
+    UserPoolClientTypeOutputTypeDef,
+    AdminGetDeviceResponseOutputTypeDef,
+    AdminListDevicesResponseOutputTypeDef,
+    GetDeviceResponseOutputTypeDef,
+    ListDevicesResponseOutputTypeDef,
+    AdminCreateUserResponseOutputTypeDef,
+    ListUsersInGroupResponseOutputTypeDef,
+    ListUsersResponseOutputTypeDef,
+    AdminListUserAuthEventsResponseOutputTypeDef,
+    AdminInitiateAuthResponseOutputTypeDef,
+    AdminRespondToAuthChallengeResponseOutputTypeDef,
+    InitiateAuthResponseOutputTypeDef,
+    RespondToAuthChallengeResponseOutputTypeDef,
     AdminInitiateAuthRequestRequestTypeDef,
     AdminRespondToAuthChallengeRequestRequestTypeDef,
-    CreateResourceServerResponseTypeDef,
-    DescribeResourceServerResponseTypeDef,
-    ListResourceServersResponseTypeDef,
-    UpdateResourceServerResponseTypeDef,
-    CreateUserPoolClientResponseTypeDef,
-    DescribeUserPoolClientResponseTypeDef,
-    UpdateUserPoolClientResponseTypeDef,
-    DescribeUserPoolDomainResponseTypeDef,
-    GetUserPoolMfaConfigResponseTypeDef,
     SetUserPoolMfaConfigRequestRequestTypeDef,
-    SetUserPoolMfaConfigResponseTypeDef,
-    UserPoolDescriptionTypeTypeDef,
+    DescribeUserPoolDomainResponseOutputTypeDef,
+    UserPoolDescriptionTypeOutputTypeDef,
+    AccountTakeoverRiskConfigurationTypeOutputTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     UpdateUserPoolRequestRequestTypeDef,
+    CreateResourceServerResponseOutputTypeDef,
+    DescribeResourceServerResponseOutputTypeDef,
+    ListResourceServersResponseOutputTypeDef,
+    UpdateResourceServerResponseOutputTypeDef,
+    UserPoolTypeOutputTypeDef,
     AddCustomAttributesRequestRequestTypeDef,
     CreateUserPoolRequestRequestTypeDef,
-    UserPoolTypeTypeDef,
-    ListUserPoolsResponseTypeDef,
-    RiskConfigurationTypeTypeDef,
+    GetUserPoolMfaConfigResponseOutputTypeDef,
+    SetUserPoolMfaConfigResponseOutputTypeDef,
+    CreateUserPoolClientResponseOutputTypeDef,
+    DescribeUserPoolClientResponseOutputTypeDef,
+    UpdateUserPoolClientResponseOutputTypeDef,
+    ListUserPoolsResponseOutputTypeDef,
+    RiskConfigurationTypeOutputTypeDef,
     SetRiskConfigurationRequestRequestTypeDef,
-    CreateUserPoolResponseTypeDef,
-    DescribeUserPoolResponseTypeDef,
-    DescribeRiskConfigurationResponseTypeDef,
-    SetRiskConfigurationResponseTypeDef,
+    CreateUserPoolResponseOutputTypeDef,
+    DescribeUserPoolResponseOutputTypeDef,
+    DescribeRiskConfigurationResponseOutputTypeDef,
+    SetRiskConfigurationResponseOutputTypeDef,
 )
 
 
-def get_structure() -> RecoveryOptionTypeTypeDef:
+def get_structure() -> RecoveryOptionTypeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/SOURCES.txt` & `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3/setup.py` & `mypy-boto3-cognito-idp-1.28.3.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-idp",
-    version="1.28.3",
+    version="1.28.3.post1",
     packages=["mypy_boto3_cognito_idp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with"
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

