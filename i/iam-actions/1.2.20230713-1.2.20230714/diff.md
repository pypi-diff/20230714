# Comparing `tmp/iam_actions-1.2.20230713.tar.gz` & `tmp/iam_actions-1.2.20230714.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230713.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230714.tar", max compression
```

## Comparing `iam_actions-1.2.20230713.tar` & `iam_actions-1.2.20230714.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-13 02:54:45.938350 iam_actions-1.2.20230713/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-13 02:54:45.938350 iam_actions-1.2.20230713/README.md
--rw-r--r--   0        0        0      228 2023-07-13 02:54:45.938350 iam_actions-1.2.20230713/iam_actions/__init__.py
--rw-r--r--   0        0        0  4363235 2023-07-13 02:56:32.886715 iam_actions-1.2.20230713/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-13 02:54:45.938350 iam_actions-1.2.20230713/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-13 02:54:45.938350 iam_actions-1.2.20230713/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-13 02:54:45.938350 iam_actions-1.2.20230713/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-13 02:54:45.938350 iam_actions-1.2.20230713/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-13 02:54:45.938350 iam_actions-1.2.20230713/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-13 02:54:45.938350 iam_actions-1.2.20230713/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-13 02:54:45.938350 iam_actions-1.2.20230713/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-13 02:54:45.938350 iam_actions-1.2.20230713/iam_actions/generate/services.py
--rw-r--r--   0        0        0   560950 2023-07-13 02:56:32.886715 iam_actions-1.2.20230713/iam_actions/policies.json
--rw-r--r--   0        0        0   197380 2023-07-13 02:56:32.886715 iam_actions-1.2.20230713/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   544067 2023-07-13 02:56:32.886715 iam_actions-1.2.20230713/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-13 02:56:33.898718 iam_actions-1.2.20230713/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230713/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230713/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/README.md
+-rw-r--r--   0        0        0      228 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4364411 2023-07-14 02:55:21.750086 iam_actions-1.2.20230714/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   561038 2023-07-14 02:55:21.750086 iam_actions-1.2.20230714/iam_actions/policies.json
+-rw-r--r--   0        0        0   197380 2023-07-14 02:55:21.750086 iam_actions-1.2.20230714/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   544152 2023-07-14 02:55:21.750086 iam_actions-1.2.20230714/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-14 02:55:22.510083 iam_actions-1.2.20230714/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230714/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230714/PKG-INFO
```

### Comparing `iam_actions-1.2.20230713/LICENSE` & `iam_actions-1.2.20230714/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230713/README.md` & `iam_actions-1.2.20230714/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230713/iam_actions/actions.json` & `iam_actions-1.2.20230714/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999952359796487%*

 * *Differences: {"'apigateway'": "{'DELETE': {'resources': {insert: [(15, 'VpcLink')]}}, 'GET': {'resources': "*

 * *                 "{insert: [(27, 'VpcLink'), (28, 'VpcLinks')]}}, 'PATCH': {'resources': {insert: "*

 * *                 "[(11, 'VpcLink')]}}, 'POST': {'resources': {insert: [(10, 'VpcLinks')]}}}",*

 * * "'connect'": "{'DeleteQueue': OrderedDict([('access_level', 'Write'), ('action', 'DeleteQueue'), "*

 * *              "('condition_keys', ['aws:ResourceTag/${TagKey}', 'connect:InstanceId']), "*

 * *              "('description', ' […]*

```diff
@@ -3242,15 +3242,16 @@
                 "Integration",
                 "IntegrationResponse",
                 "Model",
                 "Route",
                 "RouteRequestParameter",
                 "RouteResponse",
                 "RouteSettings",
-                "Stage"
+                "Stage",
+                "VpcLink"
             ]
         },
         "GET": {
             "access_level": "Read",
             "action": "GET",
             "condition_keys": [],
             "description": "Grants permission to read a particular resource",
@@ -3278,15 +3279,17 @@
                 "Route",
                 "RouteRequestParameter",
                 "RouteResponse",
                 "RouteResponses",
                 "RouteSettings",
                 "Routes",
                 "Stage",
-                "Stages"
+                "Stages",
+                "VpcLink",
+                "VpcLinks"
             ]
         },
         "PATCH": {
             "access_level": "Write",
             "action": "PATCH",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
@@ -3301,15 +3304,16 @@
                 "Deployment",
                 "Integration",
                 "IntegrationResponse",
                 "Model",
                 "Route",
                 "RouteRequestParameter",
                 "RouteResponse",
-                "Stage"
+                "Stage",
+                "VpcLink"
             ]
         },
         "POST": {
             "access_level": "Write",
             "action": "POST",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
@@ -3323,15 +3327,16 @@
                 "Authorizers",
                 "Deployments",
                 "IntegrationResponses",
                 "Integrations",
                 "Models",
                 "RouteResponses",
                 "Routes",
-                "Stages"
+                "Stages",
+                "VpcLinks"
             ]
         },
         "PUT": {
             "access_level": "Write",
             "action": "PUT",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
@@ -30761,27 +30766,53 @@
             ],
             "description": "Grants permission to delete a prompt in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "prompt"
             ]
         },
+        "DeleteQueue": {
+            "access_level": "Write",
+            "action": "DeleteQueue",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to delete a queue in an Amazon Connect instance",
+            "orphan": false,
+            "resources": [
+                "queue"
+            ]
+        },
         "DeleteQuickConnect": {
             "access_level": "Write",
             "action": "DeleteQuickConnect",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
             "description": "Grants permission to delete a quick connect in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "quick-connect"
             ]
         },
+        "DeleteRoutingProfile": {
+            "access_level": "Write",
+            "action": "DeleteRoutingProfile",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to delete routing profiles in an Amazon Connect instance",
+            "orphan": false,
+            "resources": [
+                "routing-profile"
+            ]
+        },
         "DeleteRule": {
             "access_level": "Write",
             "action": "DeleteRule",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
@@ -44019,15 +44050,14 @@
                 "fpga-image"
             ]
         },
         "CopyImage": {
             "access_level": "Write",
             "action": "CopyImage",
             "condition_keys": [
-                "ec2:ImageID",
                 "ec2:Owner",
                 "ec2:Region"
             ],
             "description": "Grants permission to copy an Amazon Machine Image (AMI) from a source Region to the current Region. Resource-level permissions specified for this action apply to the new AMI only. They do not apply to the source AMI",
             "orphan": false,
             "resources": [
                 "image"
@@ -63974,14 +64004,24 @@
             "condition_keys": [],
             "description": "Grants permission to associate DNS aliases with an Amazon FSx for Windows File Server file system",
             "orphan": false,
             "resources": [
                 "file-system"
             ]
         },
+        "BypassSnaplockEnterpriseRetention": {
+            "access_level": "Permissions management",
+            "action": "BypassSnaplockEnterpriseRetention",
+            "condition_keys": [],
+            "description": "Grants permission to allow deletion of an FSx for ONTAP SnapLock Enterprise volume that contains WORM (write once, read many) files with active retention periods",
+            "orphan": false,
+            "resources": [
+                "volume"
+            ]
+        },
         "CancelDataRepositoryTask": {
             "access_level": "Write",
             "action": "CancelDataRepositoryTask",
             "condition_keys": [],
             "description": "Grants permission to cancel a data repository task",
             "orphan": false,
             "resources": [
@@ -121952,14 +121992,15 @@
         "CreateFirewallRule": {
             "access_level": "Write",
             "action": "CreateFirewallRule",
             "condition_keys": [],
             "description": "Grants permission to create a Firewall rule within a Firewall rule group",
             "orphan": false,
             "resources": [
+                "firewall-domain-list",
                 "firewall-rule-group"
             ]
         },
         "CreateFirewallRuleGroup": {
             "access_level": "Write",
             "action": "CreateFirewallRuleGroup",
             "condition_keys": [
@@ -122022,14 +122063,15 @@
         "DeleteFirewallRule": {
             "access_level": "Write",
             "action": "DeleteFirewallRule",
             "condition_keys": [],
             "description": "Grants permission to delete a Firewall rule within a Firewall rule group",
             "orphan": false,
             "resources": [
+                "firewall-domain-list",
                 "firewall-rule-group"
             ]
         },
         "DeleteFirewallRuleGroup": {
             "access_level": "Write",
             "action": "DeleteFirewallRuleGroup",
             "condition_keys": [],
@@ -122259,17 +122301,15 @@
         },
         "ListFirewallConfigs": {
             "access_level": "List",
             "action": "ListFirewallConfigs",
             "condition_keys": [],
             "description": "Grants permission to list all the Firewall config that current AWS account is able to check",
             "orphan": false,
-            "resources": [
-                "firewall-config"
-            ]
+            "resources": []
         },
         "ListFirewallDomainLists": {
             "access_level": "List",
             "action": "ListFirewallDomainLists",
             "condition_keys": [],
             "description": "Grants permission to list all the Firewall domain list that current AWS account is able to use",
             "orphan": false,
@@ -122488,14 +122528,15 @@
         "UpdateFirewallRule": {
             "access_level": "Write",
             "action": "UpdateFirewallRule",
             "condition_keys": [],
             "description": "Grants permission to update selected settings for an Firewall rule in a Firewall rule group",
             "orphan": false,
             "resources": [
+                "firewall-domain-list",
                 "firewall-rule-group"
             ]
         },
         "UpdateFirewallRuleGroupAssociation": {
             "access_level": "Write",
             "action": "UpdateFirewallRuleGroupAssociation",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230713/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230714/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230713/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230714/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230713/iam_actions/generate/generate.py` & `iam_actions-1.2.20230714/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230713/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230714/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230713/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230714/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230713/iam_actions/generate/services.py` & `iam_actions-1.2.20230714/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230713/iam_actions/policies.json` & `iam_actions-1.2.20230714/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999996546575878%*

 * *Differences: {"'serviceMap'": "{'Amazon Connect': {'Actions': {insert: [(44, 'DeleteQueue'), (46, "*

 * *                 "'DeleteRoutingProfile')]}}, 'Amazon FSx': {'Actions': {insert: [(2, "*

 * *                 "'BypassSnaplockEnterpriseRetention')]}}}"}*

```diff
@@ -11647,15 +11647,17 @@
                 "DeleteContactFlow",
                 "DeleteContactFlowModule",
                 "DeleteEvaluationForm",
                 "DeleteHoursOfOperation",
                 "DeleteInstance",
                 "DeleteIntegrationAssociation",
                 "DeletePrompt",
+                "DeleteQueue",
                 "DeleteQuickConnect",
+                "DeleteRoutingProfile",
                 "DeleteRule",
                 "DeleteSecurityProfile",
                 "DeleteTaskTemplate",
                 "DeleteTrafficDistributionGroup",
                 "DeleteUseCase",
                 "DeleteUser",
                 "DeleteUserHierarchyGroup",
@@ -14010,14 +14012,15 @@
         },
         "Amazon FSx": {
             "ARNFormat": "arn:aws:fsx:${Region}:${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:fsx:.+",
             "Actions": [
                 "AssociateFileGateway",
                 "AssociateFileSystemAliases",
+                "BypassSnaplockEnterpriseRetention",
                 "CancelDataRepositoryTask",
                 "CopyBackup",
                 "CreateBackup",
                 "CreateDataRepositoryAssociation",
                 "CreateDataRepositoryTask",
                 "CreateFileCache",
                 "CreateFileSystem",
```

### Comparing `iam_actions-1.2.20230713/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230714/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -278,14 +278,22 @@
             "arn_pattern": "arn:*:apigateway:*::/apis/*/stages/*",
             "condition_keys": "apigateway:Request/AccessLoggingDestination"
         },
         "Stages": {
             "arn_pattern": "arn:*:apigateway:*::/apis/*/stages",
             "condition_keys": "apigateway:Request/AccessLoggingDestination"
         },
+        "VpcLink": {
+            "arn_pattern": "arn:*:apigateway:*::/vpclinks/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "VpcLinks": {
+            "arn_pattern": "arn:*:apigateway:*::/vpclinks",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "Account": {
             "arn_pattern": "arn:*:apigateway:*::/account",
             "condition_keys": null
         },
         "ApiKey": {
             "arn_pattern": "arn:*:apigateway:*::/apikeys/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
@@ -394,22 +402,14 @@
             "arn_pattern": "arn:*:apigateway:*::/usageplans/*/keys/*",
             "condition_keys": null
         },
         "UsagePlanKeys": {
             "arn_pattern": "arn:*:apigateway:*::/usageplans/*/keys",
             "condition_keys": null
         },
-        "VpcLink": {
-            "arn_pattern": "arn:*:apigateway:*::/vpclinks/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "VpcLinks": {
-            "arn_pattern": "arn:*:apigateway:*::/vpclinks",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
         "Tags": {
             "arn_pattern": "arn:*:apigateway:*::/tags/*",
             "condition_keys": null
         }
     },
     "app-integrations": {
         "event-integration": {
```

### Comparing `iam_actions-1.2.20230713/iam_actions/services.json` & `iam_actions-1.2.20230714/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999963848452714%*

 * *Differences: {"'connect'": "{'Actions': {insert: [(44, 'DeleteQueue'), (46, 'DeleteRoutingProfile')]}}",*

 * * "'fsx'": "{'Actions': {insert: [(2, 'BypassSnaplockEnterpriseRetention')]}}"}*

```diff
@@ -4660,15 +4660,17 @@
             "DeleteContactFlow",
             "DeleteContactFlowModule",
             "DeleteEvaluationForm",
             "DeleteHoursOfOperation",
             "DeleteInstance",
             "DeleteIntegrationAssociation",
             "DeletePrompt",
+            "DeleteQueue",
             "DeleteQuickConnect",
+            "DeleteRoutingProfile",
             "DeleteRule",
             "DeleteSecurityProfile",
             "DeleteTaskTemplate",
             "DeleteTrafficDistributionGroup",
             "DeleteUseCase",
             "DeleteUser",
             "DeleteUserHierarchyGroup",
@@ -8783,14 +8785,15 @@
         ],
         "ARNRegexes": [
             "^arn:aws:fsx:.+"
         ],
         "Actions": [
             "AssociateFileGateway",
             "AssociateFileSystemAliases",
+            "BypassSnaplockEnterpriseRetention",
             "CancelDataRepositoryTask",
             "CopyBackup",
             "CreateBackup",
             "CreateDataRepositoryAssociation",
             "CreateDataRepositoryTask",
             "CreateFileCache",
             "CreateFileSystem",
```

### Comparing `iam_actions-1.2.20230713/pyproject.toml` & `iam_actions-1.2.20230714/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230713"
+version = "1.2.20230714"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230713/setup.py` & `iam_actions-1.2.20230714/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230713',
+    'version': '1.2.20230714',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230713/PKG-INFO` & `iam_actions-1.2.20230714/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230713
+Version: 1.2.20230714
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

