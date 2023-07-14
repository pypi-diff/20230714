# Comparing `tmp/mypy-boto3-secretsmanager-1.28.3.tar.gz` & `tmp/mypy-boto3-secretsmanager-1.28.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-secretsmanager-1.28.3.tar", last modified: Thu Jul 13 19:49:15 2023, max compression
+gzip compressed data, was "mypy-boto3-secretsmanager-1.28.3.post1.tar", last modified: Fri Jul 14 16:18:03 2023, max compression
```

## Comparing `mypy-boto3-secretsmanager-1.28.3.tar` & `mypy-boto3-secretsmanager-1.28.3.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.173303 mypy-boto3-secretsmanager-1.28.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-07-13 19:49:15.169303 mypy-boto3-secretsmanager-1.28.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.165303 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19556 2023-07-13 19:49:01.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-07-13 19:49:01.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.169303 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:15.173303 mypy-boto3-secretsmanager-1.28.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.095742 mypy-boto3-secretsmanager-1.28.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15245 2023-07-14 16:18:03.091741 mypy-boto3-secretsmanager-1.28.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.091741 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-07-14 16:17:44.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.091741 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15245 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:18:03.095742 mypy-boto3-secretsmanager-1.28.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/setup.py
```

### Comparing `mypy-boto3-secretsmanager-1.28.3/LICENSE` & `mypy-boto3-secretsmanager-1.28.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3/PKG-INFO` & `mypy-boto3-secretsmanager-1.28.3.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-secretsmanager
-Version: 1.28.3
-Summary: Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/
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
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,67 +324,69 @@
 
 `mypy_boto3_secretsmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_secretsmanager.type_defs import (
     CancelRotateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseTypeDef,
+    CancelRotateSecretResponseOutputTypeDef,
     ReplicaRegionTypeTypeDef,
     TagTypeDef,
-    ReplicationStatusTypeTypeDef,
+    ReplicationStatusTypeOutputTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
+    DeleteResourcePolicyResponseOutputTypeDef,
     DeleteSecretRequestRequestTypeDef,
-    DeleteSecretResponseTypeDef,
+    DeleteSecretResponseOutputTypeDef,
     DescribeSecretRequestRequestTypeDef,
-    RotationRulesTypeTypeDef,
+    RotationRulesTypeOutputTypeDef,
+    TagOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GetRandomPasswordRequestRequestTypeDef,
-    GetRandomPasswordResponseTypeDef,
+    GetRandomPasswordResponseOutputTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
+    GetResourcePolicyResponseOutputTypeDef,
     GetSecretValueRequestRequestTypeDef,
-    GetSecretValueResponseTypeDef,
+    GetSecretValueResponseOutputTypeDef,
     ListSecretVersionIdsRequestRequestTypeDef,
-    SecretVersionsListEntryTypeDef,
+    SecretVersionsListEntryOutputTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
+    PutResourcePolicyResponseOutputTypeDef,
     PutSecretValueRequestRequestTypeDef,
-    PutSecretValueResponseTypeDef,
+    PutSecretValueResponseOutputTypeDef,
     RemoveRegionsFromReplicationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     RestoreSecretRequestRequestTypeDef,
-    RestoreSecretResponseTypeDef,
-    RotateSecretResponseTypeDef,
+    RestoreSecretResponseOutputTypeDef,
+    RotationRulesTypeTypeDef,
+    RotateSecretResponseOutputTypeDef,
     StopReplicationToReplicaRequestRequestTypeDef,
-    StopReplicationToReplicaResponseTypeDef,
+    StopReplicationToReplicaResponseOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSecretRequestRequestTypeDef,
-    UpdateSecretResponseTypeDef,
+    UpdateSecretResponseOutputTypeDef,
     UpdateSecretVersionStageRequestRequestTypeDef,
-    UpdateSecretVersionStageResponseTypeDef,
+    UpdateSecretVersionStageResponseOutputTypeDef,
     ValidateResourcePolicyRequestRequestTypeDef,
-    ValidationErrorsEntryTypeDef,
+    ValidationErrorsEntryOutputTypeDef,
     ReplicateSecretToRegionsRequestRequestTypeDef,
     CreateSecretRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateSecretResponseTypeDef,
-    RemoveRegionsFromReplicationResponseTypeDef,
-    ReplicateSecretToRegionsResponseTypeDef,
-    DescribeSecretResponseTypeDef,
-    RotateSecretRequestRequestTypeDef,
-    SecretListEntryTypeDef,
+    CreateSecretResponseOutputTypeDef,
+    RemoveRegionsFromReplicationResponseOutputTypeDef,
+    ReplicateSecretToRegionsResponseOutputTypeDef,
+    DescribeSecretResponseOutputTypeDef,
+    SecretListEntryOutputTypeDef,
     ListSecretsRequestListSecretsPaginateTypeDef,
     ListSecretsRequestRequestTypeDef,
-    ListSecretVersionIdsResponseTypeDef,
-    ValidateResourcePolicyResponseTypeDef,
-    ListSecretsResponseTypeDef,
+    ListSecretVersionIdsResponseOutputTypeDef,
+    RotateSecretRequestRequestTypeDef,
+    ValidateResourcePolicyResponseOutputTypeDef,
+    ListSecretsResponseOutputTypeDef,
 )
 
 
 def get_structure() -> CancelRotateSecretRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-secretsmanager-1.28.3/README.md` & `mypy-boto3-secretsmanager-1.28.3.post1/README.md`

 * *Files 5% similar despite different names*

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
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,67 +292,69 @@
 
 `mypy_boto3_secretsmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_secretsmanager.type_defs import (
     CancelRotateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseTypeDef,
+    CancelRotateSecretResponseOutputTypeDef,
     ReplicaRegionTypeTypeDef,
     TagTypeDef,
-    ReplicationStatusTypeTypeDef,
+    ReplicationStatusTypeOutputTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
+    DeleteResourcePolicyResponseOutputTypeDef,
     DeleteSecretRequestRequestTypeDef,
-    DeleteSecretResponseTypeDef,
+    DeleteSecretResponseOutputTypeDef,
     DescribeSecretRequestRequestTypeDef,
-    RotationRulesTypeTypeDef,
+    RotationRulesTypeOutputTypeDef,
+    TagOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GetRandomPasswordRequestRequestTypeDef,
-    GetRandomPasswordResponseTypeDef,
+    GetRandomPasswordResponseOutputTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
+    GetResourcePolicyResponseOutputTypeDef,
     GetSecretValueRequestRequestTypeDef,
-    GetSecretValueResponseTypeDef,
+    GetSecretValueResponseOutputTypeDef,
     ListSecretVersionIdsRequestRequestTypeDef,
-    SecretVersionsListEntryTypeDef,
+    SecretVersionsListEntryOutputTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
+    PutResourcePolicyResponseOutputTypeDef,
     PutSecretValueRequestRequestTypeDef,
-    PutSecretValueResponseTypeDef,
+    PutSecretValueResponseOutputTypeDef,
     RemoveRegionsFromReplicationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     RestoreSecretRequestRequestTypeDef,
-    RestoreSecretResponseTypeDef,
-    RotateSecretResponseTypeDef,
+    RestoreSecretResponseOutputTypeDef,
+    RotationRulesTypeTypeDef,
+    RotateSecretResponseOutputTypeDef,
     StopReplicationToReplicaRequestRequestTypeDef,
-    StopReplicationToReplicaResponseTypeDef,
+    StopReplicationToReplicaResponseOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSecretRequestRequestTypeDef,
-    UpdateSecretResponseTypeDef,
+    UpdateSecretResponseOutputTypeDef,
     UpdateSecretVersionStageRequestRequestTypeDef,
-    UpdateSecretVersionStageResponseTypeDef,
+    UpdateSecretVersionStageResponseOutputTypeDef,
     ValidateResourcePolicyRequestRequestTypeDef,
-    ValidationErrorsEntryTypeDef,
+    ValidationErrorsEntryOutputTypeDef,
     ReplicateSecretToRegionsRequestRequestTypeDef,
     CreateSecretRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateSecretResponseTypeDef,
-    RemoveRegionsFromReplicationResponseTypeDef,
-    ReplicateSecretToRegionsResponseTypeDef,
-    DescribeSecretResponseTypeDef,
-    RotateSecretRequestRequestTypeDef,
-    SecretListEntryTypeDef,
+    CreateSecretResponseOutputTypeDef,
+    RemoveRegionsFromReplicationResponseOutputTypeDef,
+    ReplicateSecretToRegionsResponseOutputTypeDef,
+    DescribeSecretResponseOutputTypeDef,
+    SecretListEntryOutputTypeDef,
     ListSecretsRequestListSecretsPaginateTypeDef,
     ListSecretsRequestRequestTypeDef,
-    ListSecretVersionIdsResponseTypeDef,
-    ValidateResourcePolicyResponseTypeDef,
-    ListSecretsResponseTypeDef,
+    ListSecretVersionIdsResponseOutputTypeDef,
+    RotateSecretRequestRequestTypeDef,
+    ValidateResourcePolicyResponseOutputTypeDef,
+    ListSecretsResponseOutputTypeDef,
 )
 
 
 def get_structure() -> CancelRotateSecretRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__init__.py` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__init__.pyi` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__main__.py` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecretsManager 1.28.3\nVersion:         1.28.3\nBuilder"
-        " version: 7.14.6\nDocs:           "
+        "Type annotations for boto3.SecretsManager 1.28.3\nVersion:         1.28.3.post1\nBuilder"
+        " version: 7.14.7\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager\nOther"
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

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/client.py` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,39 +18,39 @@
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import SortOrderTypeType
 from .paginator import ListSecretsPaginator
 from .type_defs import (
-    CancelRotateSecretResponseTypeDef,
-    CreateSecretResponseTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
-    DeleteSecretResponseTypeDef,
-    DescribeSecretResponseTypeDef,
+    CancelRotateSecretResponseOutputTypeDef,
+    CreateSecretResponseOutputTypeDef,
+    DeleteResourcePolicyResponseOutputTypeDef,
+    DeleteSecretResponseOutputTypeDef,
+    DescribeSecretResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
-    GetRandomPasswordResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetSecretValueResponseTypeDef,
-    ListSecretsResponseTypeDef,
-    ListSecretVersionIdsResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    PutSecretValueResponseTypeDef,
-    RemoveRegionsFromReplicationResponseTypeDef,
+    GetRandomPasswordResponseOutputTypeDef,
+    GetResourcePolicyResponseOutputTypeDef,
+    GetSecretValueResponseOutputTypeDef,
+    ListSecretsResponseOutputTypeDef,
+    ListSecretVersionIdsResponseOutputTypeDef,
+    PutResourcePolicyResponseOutputTypeDef,
+    PutSecretValueResponseOutputTypeDef,
+    RemoveRegionsFromReplicationResponseOutputTypeDef,
     ReplicaRegionTypeTypeDef,
-    ReplicateSecretToRegionsResponseTypeDef,
-    RestoreSecretResponseTypeDef,
-    RotateSecretResponseTypeDef,
+    ReplicateSecretToRegionsResponseOutputTypeDef,
+    RestoreSecretResponseOutputTypeDef,
+    RotateSecretResponseOutputTypeDef,
     RotationRulesTypeTypeDef,
-    StopReplicationToReplicaResponseTypeDef,
+    StopReplicationToReplicaResponseOutputTypeDef,
     TagTypeDef,
-    UpdateSecretResponseTypeDef,
-    UpdateSecretVersionStageResponseTypeDef,
-    ValidateResourcePolicyResponseTypeDef,
+    UpdateSecretResponseOutputTypeDef,
+    UpdateSecretVersionStageResponseOutputTypeDef,
+    ValidateResourcePolicyResponseOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -103,15 +103,15 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#can_paginate)
         """
 
-    def cancel_rotate_secret(self, *, SecretId: str) -> CancelRotateSecretResponseTypeDef:
+    def cancel_rotate_secret(self, *, SecretId: str) -> CancelRotateSecretResponseOutputTypeDef:
         """
         Turns off automatic rotation, and if a rotation is currently in progress,
         cancels the rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.cancel_rotate_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#cancel_rotate_secret)
         """
@@ -132,45 +132,45 @@
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef] = ...,
         ForceOverwriteReplicaSecret: bool = ...
-    ) -> CreateSecretResponseTypeDef:
+    ) -> CreateSecretResponseOutputTypeDef:
         """
         Creates a new secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.create_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#create_secret)
         """
 
-    def delete_resource_policy(self, *, SecretId: str) -> DeleteResourcePolicyResponseTypeDef:
+    def delete_resource_policy(self, *, SecretId: str) -> DeleteResourcePolicyResponseOutputTypeDef:
         """
         Deletes the resource-based permission policy attached to the secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#delete_resource_policy)
         """
 
     def delete_secret(
         self,
         *,
         SecretId: str,
         RecoveryWindowInDays: int = ...,
         ForceDeleteWithoutRecovery: bool = ...
-    ) -> DeleteSecretResponseTypeDef:
+    ) -> DeleteSecretResponseOutputTypeDef:
         """
         Deletes a secret and all of its versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.delete_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#delete_secret)
         """
 
-    def describe_secret(self, *, SecretId: str) -> DescribeSecretResponseTypeDef:
+    def describe_secret(self, *, SecretId: str) -> DescribeSecretResponseOutputTypeDef:
         """
         Retrieves the details of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.describe_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#describe_secret)
         """
 
@@ -195,34 +195,34 @@
         ExcludeCharacters: str = ...,
         ExcludeNumbers: bool = ...,
         ExcludePunctuation: bool = ...,
         ExcludeUppercase: bool = ...,
         ExcludeLowercase: bool = ...,
         IncludeSpace: bool = ...,
         RequireEachIncludedType: bool = ...
-    ) -> GetRandomPasswordResponseTypeDef:
+    ) -> GetRandomPasswordResponseOutputTypeDef:
         """
         Generates a random password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_random_password)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_random_password)
         """
 
-    def get_resource_policy(self, *, SecretId: str) -> GetResourcePolicyResponseTypeDef:
+    def get_resource_policy(self, *, SecretId: str) -> GetResourcePolicyResponseOutputTypeDef:
         """
         Retrieves the JSON text of the resource-based policy document attached to the
         secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_resource_policy)
         """
 
     def get_secret_value(
         self, *, SecretId: str, VersionId: str = ..., VersionStage: str = ...
-    ) -> GetSecretValueResponseTypeDef:
+    ) -> GetSecretValueResponseOutputTypeDef:
         """
         Retrieves the contents of the encrypted fields `SecretString` or `SecretBinary`
         from the specified version of a secret, whichever contains content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_secret_value)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_secret_value)
         """
@@ -230,15 +230,15 @@
     def list_secret_version_ids(
         self,
         *,
         SecretId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         IncludeDeprecated: bool = ...
-    ) -> ListSecretVersionIdsResponseTypeDef:
+    ) -> ListSecretVersionIdsResponseOutputTypeDef:
         """
         Lists the versions of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secret_version_ids)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#list_secret_version_ids)
         """
 
@@ -246,26 +246,26 @@
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...
-    ) -> ListSecretsResponseTypeDef:
+    ) -> ListSecretsResponseOutputTypeDef:
         """
         Lists the secrets that are stored by Secrets Manager in the Amazon Web Services
         account, not including secrets that are marked for deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secrets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#list_secrets)
         """
 
     def put_resource_policy(
         self, *, SecretId: str, ResourcePolicy: str, BlockPublicPolicy: bool = ...
-    ) -> PutResourcePolicyResponseTypeDef:
+    ) -> PutResourcePolicyResponseOutputTypeDef:
         """
         Attaches a resource-based permission policy to a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#put_resource_policy)
         """
 
@@ -273,49 +273,49 @@
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...,
         VersionStages: Sequence[str] = ...
-    ) -> PutSecretValueResponseTypeDef:
+    ) -> PutSecretValueResponseOutputTypeDef:
         """
         Creates a new version with a new encrypted secret value and attaches it to the
         secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.put_secret_value)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#put_secret_value)
         """
 
     def remove_regions_from_replication(
         self, *, SecretId: str, RemoveReplicaRegions: Sequence[str]
-    ) -> RemoveRegionsFromReplicationResponseTypeDef:
+    ) -> RemoveRegionsFromReplicationResponseOutputTypeDef:
         """
         For a secret that is replicated to other Regions, deletes the secret replicas
         from the Regions you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.remove_regions_from_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#remove_regions_from_replication)
         """
 
     def replicate_secret_to_regions(
         self,
         *,
         SecretId: str,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef],
         ForceOverwriteReplicaSecret: bool = ...
-    ) -> ReplicateSecretToRegionsResponseTypeDef:
+    ) -> ReplicateSecretToRegionsResponseOutputTypeDef:
         """
         Replicates the secret to a new Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.replicate_secret_to_regions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#replicate_secret_to_regions)
         """
 
-    def restore_secret(self, *, SecretId: str) -> RestoreSecretResponseTypeDef:
+    def restore_secret(self, *, SecretId: str) -> RestoreSecretResponseOutputTypeDef:
         """
         Cancels the scheduled deletion of a secret by removing the `DeletedDate` time
         stamp.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.restore_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#restore_secret)
         """
@@ -324,25 +324,25 @@
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         RotationLambdaARN: str = ...,
         RotationRules: RotationRulesTypeTypeDef = ...,
         RotateImmediately: bool = ...
-    ) -> RotateSecretResponseTypeDef:
+    ) -> RotateSecretResponseOutputTypeDef:
         """
         Configures and starts the asynchronous process of rotating the secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.rotate_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#rotate_secret)
         """
 
     def stop_replication_to_replica(
         self, *, SecretId: str
-    ) -> StopReplicationToReplicaResponseTypeDef:
+    ) -> StopReplicationToReplicaResponseOutputTypeDef:
         """
         Removes the link between the replica secret and the primary secret and promotes
         the replica to a primary secret in the replica Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.stop_replication_to_replica)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#stop_replication_to_replica)
         """
@@ -372,40 +372,40 @@
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...
-    ) -> UpdateSecretResponseTypeDef:
+    ) -> UpdateSecretResponseOutputTypeDef:
         """
         Modifies the details of a secret, including metadata and the secret value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#update_secret)
         """
 
     def update_secret_version_stage(
         self,
         *,
         SecretId: str,
         VersionStage: str,
         RemoveFromVersionId: str = ...,
         MoveToVersionId: str = ...
-    ) -> UpdateSecretVersionStageResponseTypeDef:
+    ) -> UpdateSecretVersionStageResponseOutputTypeDef:
         """
         Modifies the staging labels attached to a version of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret_version_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#update_secret_version_stage)
         """
 
     def validate_resource_policy(
         self, *, ResourcePolicy: str, SecretId: str = ...
-    ) -> ValidateResourcePolicyResponseTypeDef:
+    ) -> ValidateResourcePolicyResponseOutputTypeDef:
         """
         Validates that a resource policy does not grant a wide range of principals
         access to your secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.validate_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#validate_resource_policy)
         """
```

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/client.pyi` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/client.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -18,39 +18,39 @@
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import SortOrderTypeType
 from .paginator import ListSecretsPaginator
 from .type_defs import (
-    CancelRotateSecretResponseTypeDef,
-    CreateSecretResponseTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
-    DeleteSecretResponseTypeDef,
-    DescribeSecretResponseTypeDef,
+    CancelRotateSecretResponseOutputTypeDef,
+    CreateSecretResponseOutputTypeDef,
+    DeleteResourcePolicyResponseOutputTypeDef,
+    DeleteSecretResponseOutputTypeDef,
+    DescribeSecretResponseOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
-    GetRandomPasswordResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetSecretValueResponseTypeDef,
-    ListSecretsResponseTypeDef,
-    ListSecretVersionIdsResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    PutSecretValueResponseTypeDef,
-    RemoveRegionsFromReplicationResponseTypeDef,
+    GetRandomPasswordResponseOutputTypeDef,
+    GetResourcePolicyResponseOutputTypeDef,
+    GetSecretValueResponseOutputTypeDef,
+    ListSecretsResponseOutputTypeDef,
+    ListSecretVersionIdsResponseOutputTypeDef,
+    PutResourcePolicyResponseOutputTypeDef,
+    PutSecretValueResponseOutputTypeDef,
+    RemoveRegionsFromReplicationResponseOutputTypeDef,
     ReplicaRegionTypeTypeDef,
-    ReplicateSecretToRegionsResponseTypeDef,
-    RestoreSecretResponseTypeDef,
-    RotateSecretResponseTypeDef,
+    ReplicateSecretToRegionsResponseOutputTypeDef,
+    RestoreSecretResponseOutputTypeDef,
+    RotateSecretResponseOutputTypeDef,
     RotationRulesTypeTypeDef,
-    StopReplicationToReplicaResponseTypeDef,
+    StopReplicationToReplicaResponseOutputTypeDef,
     TagTypeDef,
-    UpdateSecretResponseTypeDef,
-    UpdateSecretVersionStageResponseTypeDef,
-    ValidateResourcePolicyResponseTypeDef,
+    UpdateSecretResponseOutputTypeDef,
+    UpdateSecretVersionStageResponseOutputTypeDef,
+    ValidateResourcePolicyResponseOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -97,15 +97,15 @@
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#can_paginate)
         """
-    def cancel_rotate_secret(self, *, SecretId: str) -> CancelRotateSecretResponseTypeDef:
+    def cancel_rotate_secret(self, *, SecretId: str) -> CancelRotateSecretResponseOutputTypeDef:
         """
         Turns off automatic rotation, and if a rotation is currently in progress,
         cancels the rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.cancel_rotate_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#cancel_rotate_secret)
         """
@@ -124,42 +124,42 @@
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef] = ...,
         ForceOverwriteReplicaSecret: bool = ...
-    ) -> CreateSecretResponseTypeDef:
+    ) -> CreateSecretResponseOutputTypeDef:
         """
         Creates a new secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.create_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#create_secret)
         """
-    def delete_resource_policy(self, *, SecretId: str) -> DeleteResourcePolicyResponseTypeDef:
+    def delete_resource_policy(self, *, SecretId: str) -> DeleteResourcePolicyResponseOutputTypeDef:
         """
         Deletes the resource-based permission policy attached to the secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#delete_resource_policy)
         """
     def delete_secret(
         self,
         *,
         SecretId: str,
         RecoveryWindowInDays: int = ...,
         ForceDeleteWithoutRecovery: bool = ...
-    ) -> DeleteSecretResponseTypeDef:
+    ) -> DeleteSecretResponseOutputTypeDef:
         """
         Deletes a secret and all of its versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.delete_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#delete_secret)
         """
-    def describe_secret(self, *, SecretId: str) -> DescribeSecretResponseTypeDef:
+    def describe_secret(self, *, SecretId: str) -> DescribeSecretResponseOutputTypeDef:
         """
         Retrieves the details of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.describe_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#describe_secret)
         """
     def generate_presigned_url(
@@ -182,118 +182,118 @@
         ExcludeCharacters: str = ...,
         ExcludeNumbers: bool = ...,
         ExcludePunctuation: bool = ...,
         ExcludeUppercase: bool = ...,
         ExcludeLowercase: bool = ...,
         IncludeSpace: bool = ...,
         RequireEachIncludedType: bool = ...
-    ) -> GetRandomPasswordResponseTypeDef:
+    ) -> GetRandomPasswordResponseOutputTypeDef:
         """
         Generates a random password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_random_password)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_random_password)
         """
-    def get_resource_policy(self, *, SecretId: str) -> GetResourcePolicyResponseTypeDef:
+    def get_resource_policy(self, *, SecretId: str) -> GetResourcePolicyResponseOutputTypeDef:
         """
         Retrieves the JSON text of the resource-based policy document attached to the
         secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_resource_policy)
         """
     def get_secret_value(
         self, *, SecretId: str, VersionId: str = ..., VersionStage: str = ...
-    ) -> GetSecretValueResponseTypeDef:
+    ) -> GetSecretValueResponseOutputTypeDef:
         """
         Retrieves the contents of the encrypted fields `SecretString` or `SecretBinary`
         from the specified version of a secret, whichever contains content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_secret_value)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_secret_value)
         """
     def list_secret_version_ids(
         self,
         *,
         SecretId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         IncludeDeprecated: bool = ...
-    ) -> ListSecretVersionIdsResponseTypeDef:
+    ) -> ListSecretVersionIdsResponseOutputTypeDef:
         """
         Lists the versions of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secret_version_ids)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#list_secret_version_ids)
         """
     def list_secrets(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...
-    ) -> ListSecretsResponseTypeDef:
+    ) -> ListSecretsResponseOutputTypeDef:
         """
         Lists the secrets that are stored by Secrets Manager in the Amazon Web Services
         account, not including secrets that are marked for deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secrets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#list_secrets)
         """
     def put_resource_policy(
         self, *, SecretId: str, ResourcePolicy: str, BlockPublicPolicy: bool = ...
-    ) -> PutResourcePolicyResponseTypeDef:
+    ) -> PutResourcePolicyResponseOutputTypeDef:
         """
         Attaches a resource-based permission policy to a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#put_resource_policy)
         """
     def put_secret_value(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...,
         VersionStages: Sequence[str] = ...
-    ) -> PutSecretValueResponseTypeDef:
+    ) -> PutSecretValueResponseOutputTypeDef:
         """
         Creates a new version with a new encrypted secret value and attaches it to the
         secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.put_secret_value)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#put_secret_value)
         """
     def remove_regions_from_replication(
         self, *, SecretId: str, RemoveReplicaRegions: Sequence[str]
-    ) -> RemoveRegionsFromReplicationResponseTypeDef:
+    ) -> RemoveRegionsFromReplicationResponseOutputTypeDef:
         """
         For a secret that is replicated to other Regions, deletes the secret replicas
         from the Regions you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.remove_regions_from_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#remove_regions_from_replication)
         """
     def replicate_secret_to_regions(
         self,
         *,
         SecretId: str,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef],
         ForceOverwriteReplicaSecret: bool = ...
-    ) -> ReplicateSecretToRegionsResponseTypeDef:
+    ) -> ReplicateSecretToRegionsResponseOutputTypeDef:
         """
         Replicates the secret to a new Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.replicate_secret_to_regions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#replicate_secret_to_regions)
         """
-    def restore_secret(self, *, SecretId: str) -> RestoreSecretResponseTypeDef:
+    def restore_secret(self, *, SecretId: str) -> RestoreSecretResponseOutputTypeDef:
         """
         Cancels the scheduled deletion of a secret by removing the `DeletedDate` time
         stamp.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.restore_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#restore_secret)
         """
@@ -301,24 +301,24 @@
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         RotationLambdaARN: str = ...,
         RotationRules: RotationRulesTypeTypeDef = ...,
         RotateImmediately: bool = ...
-    ) -> RotateSecretResponseTypeDef:
+    ) -> RotateSecretResponseOutputTypeDef:
         """
         Configures and starts the asynchronous process of rotating the secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.rotate_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#rotate_secret)
         """
     def stop_replication_to_replica(
         self, *, SecretId: str
-    ) -> StopReplicationToReplicaResponseTypeDef:
+    ) -> StopReplicationToReplicaResponseOutputTypeDef:
         """
         Removes the link between the replica secret and the primary secret and promotes
         the replica to a primary secret in the replica Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.stop_replication_to_replica)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#stop_replication_to_replica)
         """
@@ -345,38 +345,38 @@
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...
-    ) -> UpdateSecretResponseTypeDef:
+    ) -> UpdateSecretResponseOutputTypeDef:
         """
         Modifies the details of a secret, including metadata and the secret value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#update_secret)
         """
     def update_secret_version_stage(
         self,
         *,
         SecretId: str,
         VersionStage: str,
         RemoveFromVersionId: str = ...,
         MoveToVersionId: str = ...
-    ) -> UpdateSecretVersionStageResponseTypeDef:
+    ) -> UpdateSecretVersionStageResponseOutputTypeDef:
         """
         Modifies the staging labels attached to a version of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret_version_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#update_secret_version_stage)
         """
     def validate_resource_policy(
         self, *, ResourcePolicy: str, SecretId: str = ...
-    ) -> ValidateResourcePolicyResponseTypeDef:
+    ) -> ValidateResourcePolicyResponseOutputTypeDef:
         """
         Validates that a resource policy does not grant a wide range of principals
         access to your secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.validate_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#validate_resource_policy)
         """
```

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/literals.py` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/literals.pyi` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/paginator.py` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SortOrderTypeType
-from .type_defs import FilterTypeDef, ListSecretsResponseTypeDef, PaginatorConfigTypeDef
+from .type_defs import FilterTypeDef, ListSecretsResponseOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListSecretsPaginator",)
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
@@ -48,12 +48,12 @@
     def paginate(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecretsResponseTypeDef]:
+    ) -> _PageIterator[ListSecretsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Paginator.ListSecrets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/paginators/#listsecretspaginator)
         """
```

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/paginator.pyi` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SortOrderTypeType
-from .type_defs import FilterTypeDef, ListSecretsResponseTypeDef, PaginatorConfigTypeDef
+from .type_defs import FilterTypeDef, ListSecretsResponseOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListSecretsPaginator",)
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
@@ -45,12 +45,12 @@
     def paginate(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecretsResponseTypeDef]:
+    ) -> _PageIterator[ListSecretsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Paginator.ListSecrets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/paginators/#listsecretspaginator)
         """
```

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/type_defs.py` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,78 +23,80 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelRotateSecretRequestRequestTypeDef",
-    "CancelRotateSecretResponseTypeDef",
+    "CancelRotateSecretResponseOutputTypeDef",
     "ReplicaRegionTypeTypeDef",
     "TagTypeDef",
-    "ReplicationStatusTypeTypeDef",
+    "ReplicationStatusTypeOutputTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
-    "DeleteResourcePolicyResponseTypeDef",
+    "DeleteResourcePolicyResponseOutputTypeDef",
     "DeleteSecretRequestRequestTypeDef",
-    "DeleteSecretResponseTypeDef",
+    "DeleteSecretResponseOutputTypeDef",
     "DescribeSecretRequestRequestTypeDef",
-    "RotationRulesTypeTypeDef",
+    "RotationRulesTypeOutputTypeDef",
+    "TagOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "FilterTypeDef",
     "GetRandomPasswordRequestRequestTypeDef",
-    "GetRandomPasswordResponseTypeDef",
+    "GetRandomPasswordResponseOutputTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
+    "GetResourcePolicyResponseOutputTypeDef",
     "GetSecretValueRequestRequestTypeDef",
-    "GetSecretValueResponseTypeDef",
+    "GetSecretValueResponseOutputTypeDef",
     "ListSecretVersionIdsRequestRequestTypeDef",
-    "SecretVersionsListEntryTypeDef",
+    "SecretVersionsListEntryOutputTypeDef",
     "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
+    "PutResourcePolicyResponseOutputTypeDef",
     "PutSecretValueRequestRequestTypeDef",
-    "PutSecretValueResponseTypeDef",
+    "PutSecretValueResponseOutputTypeDef",
     "RemoveRegionsFromReplicationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreSecretRequestRequestTypeDef",
-    "RestoreSecretResponseTypeDef",
-    "RotateSecretResponseTypeDef",
+    "RestoreSecretResponseOutputTypeDef",
+    "RotationRulesTypeTypeDef",
+    "RotateSecretResponseOutputTypeDef",
     "StopReplicationToReplicaRequestRequestTypeDef",
-    "StopReplicationToReplicaResponseTypeDef",
+    "StopReplicationToReplicaResponseOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateSecretRequestRequestTypeDef",
-    "UpdateSecretResponseTypeDef",
+    "UpdateSecretResponseOutputTypeDef",
     "UpdateSecretVersionStageRequestRequestTypeDef",
-    "UpdateSecretVersionStageResponseTypeDef",
+    "UpdateSecretVersionStageResponseOutputTypeDef",
     "ValidateResourcePolicyRequestRequestTypeDef",
-    "ValidationErrorsEntryTypeDef",
+    "ValidationErrorsEntryOutputTypeDef",
     "ReplicateSecretToRegionsRequestRequestTypeDef",
     "CreateSecretRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateSecretResponseTypeDef",
-    "RemoveRegionsFromReplicationResponseTypeDef",
-    "ReplicateSecretToRegionsResponseTypeDef",
-    "DescribeSecretResponseTypeDef",
-    "RotateSecretRequestRequestTypeDef",
-    "SecretListEntryTypeDef",
+    "CreateSecretResponseOutputTypeDef",
+    "RemoveRegionsFromReplicationResponseOutputTypeDef",
+    "ReplicateSecretToRegionsResponseOutputTypeDef",
+    "DescribeSecretResponseOutputTypeDef",
+    "SecretListEntryOutputTypeDef",
     "ListSecretsRequestListSecretsPaginateTypeDef",
     "ListSecretsRequestRequestTypeDef",
-    "ListSecretVersionIdsResponseTypeDef",
-    "ValidateResourcePolicyResponseTypeDef",
-    "ListSecretsResponseTypeDef",
+    "ListSecretVersionIdsResponseOutputTypeDef",
+    "RotateSecretRequestRequestTypeDef",
+    "ValidateResourcePolicyResponseOutputTypeDef",
+    "ListSecretsResponseOutputTypeDef",
 )
 
 CancelRotateSecretRequestRequestTypeDef = TypedDict(
     "CancelRotateSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-CancelRotateSecretResponseTypeDef = TypedDict(
-    "CancelRotateSecretResponseTypeDef",
+CancelRotateSecretResponseOutputTypeDef = TypedDict(
+    "CancelRotateSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -113,16 +115,16 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ReplicationStatusTypeTypeDef = TypedDict(
-    "ReplicationStatusTypeTypeDef",
+ReplicationStatusTypeOutputTypeDef = TypedDict(
+    "ReplicationStatusTypeOutputTypeDef",
     {
         "Region": str,
         "KmsKeyId": str,
         "Status": StatusTypeType,
         "StatusMessage": str,
         "LastAccessedDate": datetime,
     },
@@ -131,16 +133,16 @@
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-DeleteResourcePolicyResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyResponseTypeDef",
+DeleteResourcePolicyResponseOutputTypeDef = TypedDict(
+    "DeleteResourcePolicyResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -162,16 +164,16 @@
 
 class DeleteSecretRequestRequestTypeDef(
     _RequiredDeleteSecretRequestRequestTypeDef, _OptionalDeleteSecretRequestRequestTypeDef
 ):
     pass
 
 
-DeleteSecretResponseTypeDef = TypedDict(
-    "DeleteSecretResponseTypeDef",
+DeleteSecretResponseOutputTypeDef = TypedDict(
+    "DeleteSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "DeletionDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -179,23 +181,31 @@
 DescribeSecretRequestRequestTypeDef = TypedDict(
     "DescribeSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-RotationRulesTypeTypeDef = TypedDict(
-    "RotationRulesTypeTypeDef",
+RotationRulesTypeOutputTypeDef = TypedDict(
+    "RotationRulesTypeOutputTypeDef",
     {
         "AutomaticallyAfterDays": int,
         "Duration": str,
         "ScheduleExpression": str,
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
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -219,31 +229,31 @@
         "ExcludeLowercase": bool,
         "IncludeSpace": bool,
         "RequireEachIncludedType": bool,
     },
     total=False,
 )
 
-GetRandomPasswordResponseTypeDef = TypedDict(
-    "GetRandomPasswordResponseTypeDef",
+GetRandomPasswordResponseOutputTypeDef = TypedDict(
+    "GetRandomPasswordResponseOutputTypeDef",
     {
         "RandomPassword": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
+GetResourcePolicyResponseOutputTypeDef = TypedDict(
+    "GetResourcePolicyResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResourcePolicy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -266,16 +276,16 @@
 
 class GetSecretValueRequestRequestTypeDef(
     _RequiredGetSecretValueRequestRequestTypeDef, _OptionalGetSecretValueRequestRequestTypeDef
 ):
     pass
 
 
-GetSecretValueResponseTypeDef = TypedDict(
-    "GetSecretValueResponseTypeDef",
+GetSecretValueResponseOutputTypeDef = TypedDict(
+    "GetSecretValueResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "SecretBinary": bytes,
         "SecretString": str,
         "VersionStages": List[str],
@@ -304,16 +314,16 @@
 class ListSecretVersionIdsRequestRequestTypeDef(
     _RequiredListSecretVersionIdsRequestRequestTypeDef,
     _OptionalListSecretVersionIdsRequestRequestTypeDef,
 ):
     pass
 
 
-SecretVersionsListEntryTypeDef = TypedDict(
-    "SecretVersionsListEntryTypeDef",
+SecretVersionsListEntryOutputTypeDef = TypedDict(
+    "SecretVersionsListEntryOutputTypeDef",
     {
         "VersionId": str,
         "VersionStages": List[str],
         "LastAccessedDate": datetime,
         "CreatedDate": datetime,
         "KmsKeyIds": List[str],
     },
@@ -347,16 +357,16 @@
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
+PutResourcePolicyResponseOutputTypeDef = TypedDict(
+    "PutResourcePolicyResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -380,16 +390,16 @@
 
 class PutSecretValueRequestRequestTypeDef(
     _RequiredPutSecretValueRequestRequestTypeDef, _OptionalPutSecretValueRequestRequestTypeDef
 ):
     pass
 
 
-PutSecretValueResponseTypeDef = TypedDict(
-    "PutSecretValueResponseTypeDef",
+PutSecretValueResponseOutputTypeDef = TypedDict(
+    "PutSecretValueResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "VersionStages": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -417,25 +427,35 @@
 RestoreSecretRequestRequestTypeDef = TypedDict(
     "RestoreSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-RestoreSecretResponseTypeDef = TypedDict(
-    "RestoreSecretResponseTypeDef",
+RestoreSecretResponseOutputTypeDef = TypedDict(
+    "RestoreSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RotateSecretResponseTypeDef = TypedDict(
-    "RotateSecretResponseTypeDef",
+RotationRulesTypeTypeDef = TypedDict(
+    "RotationRulesTypeTypeDef",
+    {
+        "AutomaticallyAfterDays": int,
+        "Duration": str,
+        "ScheduleExpression": str,
+    },
+    total=False,
+)
+
+RotateSecretResponseOutputTypeDef = TypedDict(
+    "RotateSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -443,16 +463,16 @@
 StopReplicationToReplicaRequestRequestTypeDef = TypedDict(
     "StopReplicationToReplicaRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-StopReplicationToReplicaResponseTypeDef = TypedDict(
-    "StopReplicationToReplicaResponseTypeDef",
+StopReplicationToReplicaResponseOutputTypeDef = TypedDict(
+    "StopReplicationToReplicaResponseOutputTypeDef",
     {
         "ARN": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
@@ -484,16 +504,16 @@
 
 class UpdateSecretRequestRequestTypeDef(
     _RequiredUpdateSecretRequestRequestTypeDef, _OptionalUpdateSecretRequestRequestTypeDef
 ):
     pass
 
 
-UpdateSecretResponseTypeDef = TypedDict(
-    "UpdateSecretResponseTypeDef",
+UpdateSecretResponseOutputTypeDef = TypedDict(
+    "UpdateSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -518,16 +538,16 @@
 class UpdateSecretVersionStageRequestRequestTypeDef(
     _RequiredUpdateSecretVersionStageRequestRequestTypeDef,
     _OptionalUpdateSecretVersionStageRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateSecretVersionStageResponseTypeDef = TypedDict(
-    "UpdateSecretVersionStageResponseTypeDef",
+UpdateSecretVersionStageResponseOutputTypeDef = TypedDict(
+    "UpdateSecretVersionStageResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -549,16 +569,16 @@
 class ValidateResourcePolicyRequestRequestTypeDef(
     _RequiredValidateResourcePolicyRequestRequestTypeDef,
     _OptionalValidateResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
 
-ValidationErrorsEntryTypeDef = TypedDict(
-    "ValidationErrorsEntryTypeDef",
+ValidationErrorsEntryOutputTypeDef = TypedDict(
+    "ValidationErrorsEntryOutputTypeDef",
     {
         "CheckName": str,
         "ErrorMessage": str,
     },
 )
 
 _RequiredReplicateSecretToRegionsRequestRequestTypeDef = TypedDict(
@@ -616,108 +636,84 @@
     "TagResourceRequestRequestTypeDef",
     {
         "SecretId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateSecretResponseTypeDef = TypedDict(
-    "CreateSecretResponseTypeDef",
+CreateSecretResponseOutputTypeDef = TypedDict(
+    "CreateSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
-        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RemoveRegionsFromReplicationResponseTypeDef = TypedDict(
-    "RemoveRegionsFromReplicationResponseTypeDef",
+RemoveRegionsFromReplicationResponseOutputTypeDef = TypedDict(
+    "RemoveRegionsFromReplicationResponseOutputTypeDef",
     {
         "ARN": str,
-        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReplicateSecretToRegionsResponseTypeDef = TypedDict(
-    "ReplicateSecretToRegionsResponseTypeDef",
+ReplicateSecretToRegionsResponseOutputTypeDef = TypedDict(
+    "ReplicateSecretToRegionsResponseOutputTypeDef",
     {
         "ARN": str,
-        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSecretResponseTypeDef = TypedDict(
-    "DescribeSecretResponseTypeDef",
+DescribeSecretResponseOutputTypeDef = TypedDict(
+    "DescribeSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "Description": str,
         "KmsKeyId": str,
         "RotationEnabled": bool,
         "RotationLambdaARN": str,
-        "RotationRules": RotationRulesTypeTypeDef,
+        "RotationRules": RotationRulesTypeOutputTypeDef,
         "LastRotatedDate": datetime,
         "LastChangedDate": datetime,
         "LastAccessedDate": datetime,
         "DeletedDate": datetime,
         "NextRotationDate": datetime,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "VersionIdsToStages": Dict[str, List[str]],
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
-        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRotateSecretRequestRequestTypeDef = TypedDict(
-    "_RequiredRotateSecretRequestRequestTypeDef",
-    {
-        "SecretId": str,
-    },
-)
-_OptionalRotateSecretRequestRequestTypeDef = TypedDict(
-    "_OptionalRotateSecretRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "RotationLambdaARN": str,
-        "RotationRules": RotationRulesTypeTypeDef,
-        "RotateImmediately": bool,
-    },
-    total=False,
-)
-
-
-class RotateSecretRequestRequestTypeDef(
-    _RequiredRotateSecretRequestRequestTypeDef, _OptionalRotateSecretRequestRequestTypeDef
-):
-    pass
-
-
-SecretListEntryTypeDef = TypedDict(
-    "SecretListEntryTypeDef",
+SecretListEntryOutputTypeDef = TypedDict(
+    "SecretListEntryOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "Description": str,
         "KmsKeyId": str,
         "RotationEnabled": bool,
         "RotationLambdaARN": str,
-        "RotationRules": RotationRulesTypeTypeDef,
+        "RotationRules": RotationRulesTypeOutputTypeDef,
         "LastRotatedDate": datetime,
         "LastChangedDate": datetime,
         "LastAccessedDate": datetime,
         "DeletedDate": datetime,
         "NextRotationDate": datetime,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "SecretVersionsToStages": Dict[str, List[str]],
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
     },
 )
 
@@ -740,35 +736,59 @@
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortOrder": SortOrderTypeType,
     },
     total=False,
 )
 
-ListSecretVersionIdsResponseTypeDef = TypedDict(
-    "ListSecretVersionIdsResponseTypeDef",
+ListSecretVersionIdsResponseOutputTypeDef = TypedDict(
+    "ListSecretVersionIdsResponseOutputTypeDef",
     {
-        "Versions": List[SecretVersionsListEntryTypeDef],
+        "Versions": List[SecretVersionsListEntryOutputTypeDef],
         "NextToken": str,
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ValidateResourcePolicyResponseTypeDef = TypedDict(
-    "ValidateResourcePolicyResponseTypeDef",
+_RequiredRotateSecretRequestRequestTypeDef = TypedDict(
+    "_RequiredRotateSecretRequestRequestTypeDef",
+    {
+        "SecretId": str,
+    },
+)
+_OptionalRotateSecretRequestRequestTypeDef = TypedDict(
+    "_OptionalRotateSecretRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "RotationLambdaARN": str,
+        "RotationRules": RotationRulesTypeTypeDef,
+        "RotateImmediately": bool,
+    },
+    total=False,
+)
+
+
+class RotateSecretRequestRequestTypeDef(
+    _RequiredRotateSecretRequestRequestTypeDef, _OptionalRotateSecretRequestRequestTypeDef
+):
+    pass
+
+
+ValidateResourcePolicyResponseOutputTypeDef = TypedDict(
+    "ValidateResourcePolicyResponseOutputTypeDef",
     {
         "PolicyValidationPassed": bool,
-        "ValidationErrors": List[ValidationErrorsEntryTypeDef],
+        "ValidationErrors": List[ValidationErrorsEntryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSecretsResponseTypeDef = TypedDict(
-    "ListSecretsResponseTypeDef",
+ListSecretsResponseOutputTypeDef = TypedDict(
+    "ListSecretsResponseOutputTypeDef",
     {
-        "SecretList": List[SecretListEntryTypeDef],
+        "SecretList": List[SecretListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/type_defs.pyi` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -22,78 +22,80 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelRotateSecretRequestRequestTypeDef",
-    "CancelRotateSecretResponseTypeDef",
+    "CancelRotateSecretResponseOutputTypeDef",
     "ReplicaRegionTypeTypeDef",
     "TagTypeDef",
-    "ReplicationStatusTypeTypeDef",
+    "ReplicationStatusTypeOutputTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
-    "DeleteResourcePolicyResponseTypeDef",
+    "DeleteResourcePolicyResponseOutputTypeDef",
     "DeleteSecretRequestRequestTypeDef",
-    "DeleteSecretResponseTypeDef",
+    "DeleteSecretResponseOutputTypeDef",
     "DescribeSecretRequestRequestTypeDef",
-    "RotationRulesTypeTypeDef",
+    "RotationRulesTypeOutputTypeDef",
+    "TagOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "FilterTypeDef",
     "GetRandomPasswordRequestRequestTypeDef",
-    "GetRandomPasswordResponseTypeDef",
+    "GetRandomPasswordResponseOutputTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
+    "GetResourcePolicyResponseOutputTypeDef",
     "GetSecretValueRequestRequestTypeDef",
-    "GetSecretValueResponseTypeDef",
+    "GetSecretValueResponseOutputTypeDef",
     "ListSecretVersionIdsRequestRequestTypeDef",
-    "SecretVersionsListEntryTypeDef",
+    "SecretVersionsListEntryOutputTypeDef",
     "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
+    "PutResourcePolicyResponseOutputTypeDef",
     "PutSecretValueRequestRequestTypeDef",
-    "PutSecretValueResponseTypeDef",
+    "PutSecretValueResponseOutputTypeDef",
     "RemoveRegionsFromReplicationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreSecretRequestRequestTypeDef",
-    "RestoreSecretResponseTypeDef",
-    "RotateSecretResponseTypeDef",
+    "RestoreSecretResponseOutputTypeDef",
+    "RotationRulesTypeTypeDef",
+    "RotateSecretResponseOutputTypeDef",
     "StopReplicationToReplicaRequestRequestTypeDef",
-    "StopReplicationToReplicaResponseTypeDef",
+    "StopReplicationToReplicaResponseOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateSecretRequestRequestTypeDef",
-    "UpdateSecretResponseTypeDef",
+    "UpdateSecretResponseOutputTypeDef",
     "UpdateSecretVersionStageRequestRequestTypeDef",
-    "UpdateSecretVersionStageResponseTypeDef",
+    "UpdateSecretVersionStageResponseOutputTypeDef",
     "ValidateResourcePolicyRequestRequestTypeDef",
-    "ValidationErrorsEntryTypeDef",
+    "ValidationErrorsEntryOutputTypeDef",
     "ReplicateSecretToRegionsRequestRequestTypeDef",
     "CreateSecretRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateSecretResponseTypeDef",
-    "RemoveRegionsFromReplicationResponseTypeDef",
-    "ReplicateSecretToRegionsResponseTypeDef",
-    "DescribeSecretResponseTypeDef",
-    "RotateSecretRequestRequestTypeDef",
-    "SecretListEntryTypeDef",
+    "CreateSecretResponseOutputTypeDef",
+    "RemoveRegionsFromReplicationResponseOutputTypeDef",
+    "ReplicateSecretToRegionsResponseOutputTypeDef",
+    "DescribeSecretResponseOutputTypeDef",
+    "SecretListEntryOutputTypeDef",
     "ListSecretsRequestListSecretsPaginateTypeDef",
     "ListSecretsRequestRequestTypeDef",
-    "ListSecretVersionIdsResponseTypeDef",
-    "ValidateResourcePolicyResponseTypeDef",
-    "ListSecretsResponseTypeDef",
+    "ListSecretVersionIdsResponseOutputTypeDef",
+    "RotateSecretRequestRequestTypeDef",
+    "ValidateResourcePolicyResponseOutputTypeDef",
+    "ListSecretsResponseOutputTypeDef",
 )
 
 CancelRotateSecretRequestRequestTypeDef = TypedDict(
     "CancelRotateSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-CancelRotateSecretResponseTypeDef = TypedDict(
-    "CancelRotateSecretResponseTypeDef",
+CancelRotateSecretResponseOutputTypeDef = TypedDict(
+    "CancelRotateSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -112,16 +114,16 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ReplicationStatusTypeTypeDef = TypedDict(
-    "ReplicationStatusTypeTypeDef",
+ReplicationStatusTypeOutputTypeDef = TypedDict(
+    "ReplicationStatusTypeOutputTypeDef",
     {
         "Region": str,
         "KmsKeyId": str,
         "Status": StatusTypeType,
         "StatusMessage": str,
         "LastAccessedDate": datetime,
     },
@@ -130,16 +132,16 @@
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-DeleteResourcePolicyResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyResponseTypeDef",
+DeleteResourcePolicyResponseOutputTypeDef = TypedDict(
+    "DeleteResourcePolicyResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -159,16 +161,16 @@
 )
 
 class DeleteSecretRequestRequestTypeDef(
     _RequiredDeleteSecretRequestRequestTypeDef, _OptionalDeleteSecretRequestRequestTypeDef
 ):
     pass
 
-DeleteSecretResponseTypeDef = TypedDict(
-    "DeleteSecretResponseTypeDef",
+DeleteSecretResponseOutputTypeDef = TypedDict(
+    "DeleteSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "DeletionDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -176,23 +178,31 @@
 DescribeSecretRequestRequestTypeDef = TypedDict(
     "DescribeSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-RotationRulesTypeTypeDef = TypedDict(
-    "RotationRulesTypeTypeDef",
+RotationRulesTypeOutputTypeDef = TypedDict(
+    "RotationRulesTypeOutputTypeDef",
     {
         "AutomaticallyAfterDays": int,
         "Duration": str,
         "ScheduleExpression": str,
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
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -216,31 +226,31 @@
         "ExcludeLowercase": bool,
         "IncludeSpace": bool,
         "RequireEachIncludedType": bool,
     },
     total=False,
 )
 
-GetRandomPasswordResponseTypeDef = TypedDict(
-    "GetRandomPasswordResponseTypeDef",
+GetRandomPasswordResponseOutputTypeDef = TypedDict(
+    "GetRandomPasswordResponseOutputTypeDef",
     {
         "RandomPassword": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
+GetResourcePolicyResponseOutputTypeDef = TypedDict(
+    "GetResourcePolicyResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResourcePolicy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -261,16 +271,16 @@
 )
 
 class GetSecretValueRequestRequestTypeDef(
     _RequiredGetSecretValueRequestRequestTypeDef, _OptionalGetSecretValueRequestRequestTypeDef
 ):
     pass
 
-GetSecretValueResponseTypeDef = TypedDict(
-    "GetSecretValueResponseTypeDef",
+GetSecretValueResponseOutputTypeDef = TypedDict(
+    "GetSecretValueResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "SecretBinary": bytes,
         "SecretString": str,
         "VersionStages": List[str],
@@ -297,16 +307,16 @@
 
 class ListSecretVersionIdsRequestRequestTypeDef(
     _RequiredListSecretVersionIdsRequestRequestTypeDef,
     _OptionalListSecretVersionIdsRequestRequestTypeDef,
 ):
     pass
 
-SecretVersionsListEntryTypeDef = TypedDict(
-    "SecretVersionsListEntryTypeDef",
+SecretVersionsListEntryOutputTypeDef = TypedDict(
+    "SecretVersionsListEntryOutputTypeDef",
     {
         "VersionId": str,
         "VersionStages": List[str],
         "LastAccessedDate": datetime,
         "CreatedDate": datetime,
         "KmsKeyIds": List[str],
     },
@@ -338,16 +348,16 @@
 )
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
+PutResourcePolicyResponseOutputTypeDef = TypedDict(
+    "PutResourcePolicyResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -369,16 +379,16 @@
 )
 
 class PutSecretValueRequestRequestTypeDef(
     _RequiredPutSecretValueRequestRequestTypeDef, _OptionalPutSecretValueRequestRequestTypeDef
 ):
     pass
 
-PutSecretValueResponseTypeDef = TypedDict(
-    "PutSecretValueResponseTypeDef",
+PutSecretValueResponseOutputTypeDef = TypedDict(
+    "PutSecretValueResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "VersionStages": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -406,25 +416,35 @@
 RestoreSecretRequestRequestTypeDef = TypedDict(
     "RestoreSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-RestoreSecretResponseTypeDef = TypedDict(
-    "RestoreSecretResponseTypeDef",
+RestoreSecretResponseOutputTypeDef = TypedDict(
+    "RestoreSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RotateSecretResponseTypeDef = TypedDict(
-    "RotateSecretResponseTypeDef",
+RotationRulesTypeTypeDef = TypedDict(
+    "RotationRulesTypeTypeDef",
+    {
+        "AutomaticallyAfterDays": int,
+        "Duration": str,
+        "ScheduleExpression": str,
+    },
+    total=False,
+)
+
+RotateSecretResponseOutputTypeDef = TypedDict(
+    "RotateSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -432,16 +452,16 @@
 StopReplicationToReplicaRequestRequestTypeDef = TypedDict(
     "StopReplicationToReplicaRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-StopReplicationToReplicaResponseTypeDef = TypedDict(
-    "StopReplicationToReplicaResponseTypeDef",
+StopReplicationToReplicaResponseOutputTypeDef = TypedDict(
+    "StopReplicationToReplicaResponseOutputTypeDef",
     {
         "ARN": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
@@ -471,16 +491,16 @@
 )
 
 class UpdateSecretRequestRequestTypeDef(
     _RequiredUpdateSecretRequestRequestTypeDef, _OptionalUpdateSecretRequestRequestTypeDef
 ):
     pass
 
-UpdateSecretResponseTypeDef = TypedDict(
-    "UpdateSecretResponseTypeDef",
+UpdateSecretResponseOutputTypeDef = TypedDict(
+    "UpdateSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -503,16 +523,16 @@
 
 class UpdateSecretVersionStageRequestRequestTypeDef(
     _RequiredUpdateSecretVersionStageRequestRequestTypeDef,
     _OptionalUpdateSecretVersionStageRequestRequestTypeDef,
 ):
     pass
 
-UpdateSecretVersionStageResponseTypeDef = TypedDict(
-    "UpdateSecretVersionStageResponseTypeDef",
+UpdateSecretVersionStageResponseOutputTypeDef = TypedDict(
+    "UpdateSecretVersionStageResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -532,16 +552,16 @@
 
 class ValidateResourcePolicyRequestRequestTypeDef(
     _RequiredValidateResourcePolicyRequestRequestTypeDef,
     _OptionalValidateResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-ValidationErrorsEntryTypeDef = TypedDict(
-    "ValidationErrorsEntryTypeDef",
+ValidationErrorsEntryOutputTypeDef = TypedDict(
+    "ValidationErrorsEntryOutputTypeDef",
     {
         "CheckName": str,
         "ErrorMessage": str,
     },
 )
 
 _RequiredReplicateSecretToRegionsRequestRequestTypeDef = TypedDict(
@@ -595,106 +615,84 @@
     "TagResourceRequestRequestTypeDef",
     {
         "SecretId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateSecretResponseTypeDef = TypedDict(
-    "CreateSecretResponseTypeDef",
+CreateSecretResponseOutputTypeDef = TypedDict(
+    "CreateSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
-        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RemoveRegionsFromReplicationResponseTypeDef = TypedDict(
-    "RemoveRegionsFromReplicationResponseTypeDef",
+RemoveRegionsFromReplicationResponseOutputTypeDef = TypedDict(
+    "RemoveRegionsFromReplicationResponseOutputTypeDef",
     {
         "ARN": str,
-        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReplicateSecretToRegionsResponseTypeDef = TypedDict(
-    "ReplicateSecretToRegionsResponseTypeDef",
+ReplicateSecretToRegionsResponseOutputTypeDef = TypedDict(
+    "ReplicateSecretToRegionsResponseOutputTypeDef",
     {
         "ARN": str,
-        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSecretResponseTypeDef = TypedDict(
-    "DescribeSecretResponseTypeDef",
+DescribeSecretResponseOutputTypeDef = TypedDict(
+    "DescribeSecretResponseOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "Description": str,
         "KmsKeyId": str,
         "RotationEnabled": bool,
         "RotationLambdaARN": str,
-        "RotationRules": RotationRulesTypeTypeDef,
+        "RotationRules": RotationRulesTypeOutputTypeDef,
         "LastRotatedDate": datetime,
         "LastChangedDate": datetime,
         "LastAccessedDate": datetime,
         "DeletedDate": datetime,
         "NextRotationDate": datetime,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "VersionIdsToStages": Dict[str, List[str]],
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
-        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRotateSecretRequestRequestTypeDef = TypedDict(
-    "_RequiredRotateSecretRequestRequestTypeDef",
-    {
-        "SecretId": str,
-    },
-)
-_OptionalRotateSecretRequestRequestTypeDef = TypedDict(
-    "_OptionalRotateSecretRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "RotationLambdaARN": str,
-        "RotationRules": RotationRulesTypeTypeDef,
-        "RotateImmediately": bool,
-    },
-    total=False,
-)
-
-class RotateSecretRequestRequestTypeDef(
-    _RequiredRotateSecretRequestRequestTypeDef, _OptionalRotateSecretRequestRequestTypeDef
-):
-    pass
-
-SecretListEntryTypeDef = TypedDict(
-    "SecretListEntryTypeDef",
+SecretListEntryOutputTypeDef = TypedDict(
+    "SecretListEntryOutputTypeDef",
     {
         "ARN": str,
         "Name": str,
         "Description": str,
         "KmsKeyId": str,
         "RotationEnabled": bool,
         "RotationLambdaARN": str,
-        "RotationRules": RotationRulesTypeTypeDef,
+        "RotationRules": RotationRulesTypeOutputTypeDef,
         "LastRotatedDate": datetime,
         "LastChangedDate": datetime,
         "LastAccessedDate": datetime,
         "DeletedDate": datetime,
         "NextRotationDate": datetime,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "SecretVersionsToStages": Dict[str, List[str]],
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
     },
 )
 
@@ -717,35 +715,57 @@
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortOrder": SortOrderTypeType,
     },
     total=False,
 )
 
-ListSecretVersionIdsResponseTypeDef = TypedDict(
-    "ListSecretVersionIdsResponseTypeDef",
+ListSecretVersionIdsResponseOutputTypeDef = TypedDict(
+    "ListSecretVersionIdsResponseOutputTypeDef",
     {
-        "Versions": List[SecretVersionsListEntryTypeDef],
+        "Versions": List[SecretVersionsListEntryOutputTypeDef],
         "NextToken": str,
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ValidateResourcePolicyResponseTypeDef = TypedDict(
-    "ValidateResourcePolicyResponseTypeDef",
+_RequiredRotateSecretRequestRequestTypeDef = TypedDict(
+    "_RequiredRotateSecretRequestRequestTypeDef",
+    {
+        "SecretId": str,
+    },
+)
+_OptionalRotateSecretRequestRequestTypeDef = TypedDict(
+    "_OptionalRotateSecretRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "RotationLambdaARN": str,
+        "RotationRules": RotationRulesTypeTypeDef,
+        "RotateImmediately": bool,
+    },
+    total=False,
+)
+
+class RotateSecretRequestRequestTypeDef(
+    _RequiredRotateSecretRequestRequestTypeDef, _OptionalRotateSecretRequestRequestTypeDef
+):
+    pass
+
+ValidateResourcePolicyResponseOutputTypeDef = TypedDict(
+    "ValidateResourcePolicyResponseOutputTypeDef",
     {
         "PolicyValidationPassed": bool,
-        "ValidationErrors": List[ValidationErrorsEntryTypeDef],
+        "ValidationErrors": List[ValidationErrorsEntryOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSecretsResponseTypeDef = TypedDict(
-    "ListSecretsResponseTypeDef",
+ListSecretsResponseOutputTypeDef = TypedDict(
+    "ListSecretsResponseOutputTypeDef",
     {
-        "SecretList": List[SecretListEntryTypeDef],
+        "SecretList": List[SecretListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/PKG-INFO` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-secretsmanager
-Version: 1.28.3
-Summary: Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/
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
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,67 +324,69 @@
 
 `mypy_boto3_secretsmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_secretsmanager.type_defs import (
     CancelRotateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseTypeDef,
+    CancelRotateSecretResponseOutputTypeDef,
     ReplicaRegionTypeTypeDef,
     TagTypeDef,
-    ReplicationStatusTypeTypeDef,
+    ReplicationStatusTypeOutputTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
+    DeleteResourcePolicyResponseOutputTypeDef,
     DeleteSecretRequestRequestTypeDef,
-    DeleteSecretResponseTypeDef,
+    DeleteSecretResponseOutputTypeDef,
     DescribeSecretRequestRequestTypeDef,
-    RotationRulesTypeTypeDef,
+    RotationRulesTypeOutputTypeDef,
+    TagOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GetRandomPasswordRequestRequestTypeDef,
-    GetRandomPasswordResponseTypeDef,
+    GetRandomPasswordResponseOutputTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
+    GetResourcePolicyResponseOutputTypeDef,
     GetSecretValueRequestRequestTypeDef,
-    GetSecretValueResponseTypeDef,
+    GetSecretValueResponseOutputTypeDef,
     ListSecretVersionIdsRequestRequestTypeDef,
-    SecretVersionsListEntryTypeDef,
+    SecretVersionsListEntryOutputTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
+    PutResourcePolicyResponseOutputTypeDef,
     PutSecretValueRequestRequestTypeDef,
-    PutSecretValueResponseTypeDef,
+    PutSecretValueResponseOutputTypeDef,
     RemoveRegionsFromReplicationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     RestoreSecretRequestRequestTypeDef,
-    RestoreSecretResponseTypeDef,
-    RotateSecretResponseTypeDef,
+    RestoreSecretResponseOutputTypeDef,
+    RotationRulesTypeTypeDef,
+    RotateSecretResponseOutputTypeDef,
     StopReplicationToReplicaRequestRequestTypeDef,
-    StopReplicationToReplicaResponseTypeDef,
+    StopReplicationToReplicaResponseOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSecretRequestRequestTypeDef,
-    UpdateSecretResponseTypeDef,
+    UpdateSecretResponseOutputTypeDef,
     UpdateSecretVersionStageRequestRequestTypeDef,
-    UpdateSecretVersionStageResponseTypeDef,
+    UpdateSecretVersionStageResponseOutputTypeDef,
     ValidateResourcePolicyRequestRequestTypeDef,
-    ValidationErrorsEntryTypeDef,
+    ValidationErrorsEntryOutputTypeDef,
     ReplicateSecretToRegionsRequestRequestTypeDef,
     CreateSecretRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateSecretResponseTypeDef,
-    RemoveRegionsFromReplicationResponseTypeDef,
-    ReplicateSecretToRegionsResponseTypeDef,
-    DescribeSecretResponseTypeDef,
-    RotateSecretRequestRequestTypeDef,
-    SecretListEntryTypeDef,
+    CreateSecretResponseOutputTypeDef,
+    RemoveRegionsFromReplicationResponseOutputTypeDef,
+    ReplicateSecretToRegionsResponseOutputTypeDef,
+    DescribeSecretResponseOutputTypeDef,
+    SecretListEntryOutputTypeDef,
     ListSecretsRequestListSecretsPaginateTypeDef,
     ListSecretsRequestRequestTypeDef,
-    ListSecretVersionIdsResponseTypeDef,
-    ValidateResourcePolicyResponseTypeDef,
-    ListSecretsResponseTypeDef,
+    ListSecretVersionIdsResponseOutputTypeDef,
+    RotateSecretRequestRequestTypeDef,
+    ValidateResourcePolicyResponseOutputTypeDef,
+    ListSecretsResponseOutputTypeDef,
 )
 
 
 def get_structure() -> CancelRotateSecretRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/SOURCES.txt` & `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3/setup.py` & `mypy-boto3-secretsmanager-1.28.3.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-secretsmanager",
-    version="1.28.3",
+    version="1.28.3.post1",
     packages=["mypy_boto3_secretsmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder"
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

