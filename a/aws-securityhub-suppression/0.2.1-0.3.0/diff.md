# Comparing `tmp/aws_securityhub_suppression-0.2.1.tar.gz` & `tmp/aws_securityhub_suppression-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_securityhub_suppression-0.2.1.tar", max compression
+gzip compressed data, was "aws_securityhub_suppression-0.3.0.tar", max compression
```

## Comparing `aws_securityhub_suppression-0.2.1.tar` & `aws_securityhub_suppression-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0      820 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/README.md
--rw-r--r--   0        0        0     1236 2023-06-12 18:12:10.871699 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/__init__.py
--rw-r--r--   0        0        0     1058 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/account.py
--rw-r--r--   0        0        0      515 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/commands/__init__.py
--rw-r--r--   0        0        0      970 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/commands/prepare.py
--rw-r--r--   0        0        0     1583 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/commands/update.py
--rw-r--r--   0        0        0      793 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/context.py
--rw-r--r--   0        0        0      744 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/handler.py
--rw-r--r--   0        0        0     1133 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/documentation_generator.py
--rw-r--r--   0        0        0     1024 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/finding.py
--rw-r--r--   0        0        0     1307 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/suppress_findings.py
--rw-r--r--   0        0        0      865 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/suppression.py
--rw-r--r--   0        0        0      672 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/workload.py
--rw-r--r--   0        0        0     1695 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/workload_generator.py
--rw-r--r--   0        0        0     1197 2023-06-12 18:12:10.871699 aws_securityhub_suppression-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 aws_securityhub_suppression-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      836 2023-07-14 15:08:25.449800 aws_securityhub_suppression-0.3.0/README.md
+-rw-r--r--   0        0        0     1453 2023-07-14 15:08:26.457805 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/__init__.py
+-rw-r--r--   0        0        0      948 2023-07-14 15:08:25.449800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/account.py
+-rw-r--r--   0        0        0      515 2023-07-14 15:08:25.449800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:08:25.449800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-14 15:08:25.449800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/check.py
+-rw-r--r--   0        0        0      970 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/prepare.py
+-rw-r--r--   0        0        0     1583 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/update.py
+-rw-r--r--   0        0        0      793 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/context.py
+-rw-r--r--   0        0        0      744 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/handler.py
+-rw-r--r--   0        0        0     1133 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/documentation_generator.py
+-rw-r--r--   0        0        0     1303 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/finding.py
+-rw-r--r--   0        0        0      830 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/schemas/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/schemas/environment.yaml
+-rw-r--r--   0        0        0      158 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/schemas/workload.yaml
+-rw-r--r--   0        0        0     1307 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/suppress_findings.py
+-rw-r--r--   0        0        0      759 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/suppression.py
+-rw-r--r--   0        0        0      561 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/workload.py
+-rw-r--r--   0        0        0     1695 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/workload_generator.py
+-rw-r--r--   0        0        0     1220 2023-07-14 15:08:26.457805 aws_securityhub_suppression-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 aws_securityhub_suppression-0.3.0/PKG-INFO
```

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/__init__.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 from typing import List, Optional
 import glob
 import os
-import yaml
 from aws_securityhub_suppression.account import Account
+from aws_securityhub_suppression.schemas import (
+    WorkloadSchema,
+    EnvironmentSchema,
+    safe_load_file,
+)
 from aws_securityhub_suppression.workload import Workload
 from aws_securityhub_suppression.suppression import Suppression
+from aws_securityhub_suppression.finding import Finding
 
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 
 
 def load_workloads(workload_path: str) -> List[Workload]:
     workloads = glob.glob(os.path.join(workload_path, "**/info.yaml"), recursive=True)
 
     def load_workload(file: str) -> Optional[Workload]:
         return load_workload_by_file(file)
 
     response = list(map(load_workload, workloads))
 
     return list(filter(None, response))
 
 
-def load_accounts_by_file(path: str) -> Optional[Account]:
-    with open(path, "r") as f:
-        return Account.from_dict(yaml.safe_load(f))
+def load_environments_by_file(path: str) -> Optional[Account]:
+    data = safe_load_file(EnvironmentSchema, path)
+    return Account.from_dict(data)
 
 
 def load_workload_by_file(path: str) -> Optional[Workload]:
-    workload_base = os.path.dirname(path)
-    accounts_files = glob.glob(os.path.join(workload_base, "*.yaml"), recursive=True)
-    accounts_files = [file for file in accounts_files if not file.endswith("info.yaml")]
-    response = list(map(load_accounts_by_file, accounts_files))
+    data = safe_load_file(WorkloadSchema, path)
+
+    def convert_environments_to_file_locations(environment: str) -> str:
+        return os.path.join(os.path.dirname(path), f"{environment}.yaml")
+
+    accounts_files = list(
+        map(convert_environments_to_file_locations, data.get("Environments", []))
+    )
+    response = list(map(load_environments_by_file, accounts_files))
     accounts = list(filter(None, response))
 
-    with open(path, "r") as f:
-        return Workload.from_dict(yaml.safe_load(f), accounts)
+    return Workload.from_dict(data, accounts)
```

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/account.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/account.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Optional, List
+from typing import List
 
 import landingzone_organization
 
 from aws_securityhub_suppression.suppression import Suppression
 
 
 class Account(landingzone_organization.Account):
@@ -18,18 +18,14 @@
         return self.__suppressions
 
     def scheduled_for_suppression(self) -> List[Suppression]:
         # TODO: Do something clever here
         return self.suppressions
 
     @staticmethod
-    def from_dict(data: dict) -> Optional[Account]:
-        # TODO: Schema validation
-        if "Name" not in data:
-            return None
-
+    def from_dict(data: dict) -> Account:
         suppressions = list(Suppression.from_dict(d) for d in data["Suppressions"])
         return Account(
             name=data["Name"],
             account_id=data["AccountId"],
             suppressions=list(filter(None, suppressions)),
         )
```

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/__init__.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/commands/prepare.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/prepare.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/commands/update.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/context.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/context.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/handler.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/documentation_generator.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/finding.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/finding.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,26 @@
+from __future__ import annotations
+
+
 class Finding:
-    def __init__(self, finding_arn: str) -> None:
+    def __init__(self, name: str, finding_arn: str) -> None:
         parts = finding_arn.split(":")
+        self.__name = name
         self.__finding_arn = finding_arn
         self.__service = parts[2]
         self.__region = parts[3]
         self.__account_id = parts[4]
         self.__finding_id = parts[-1].split("/")[-1]
         self.__generator_id = "/".join(finding_arn.split("/")[1:-2])
 
     @property
+    def name(self) -> str:
+        return self.__name
+
+    @property
     def arn(self) -> str:
         return self.__finding_arn
 
     @property
     def id(self) -> str:
         return self.__finding_id
 
@@ -34,7 +42,11 @@
 
     @property
     def product_arn(self) -> str:
         return f"arn:aws:securityhub:{self.region}::product/aws/securityhub"
 
     def __str__(self) -> str:
         return self.__finding_arn
+
+    @staticmethod
+    def from_dict(data: dict) -> Finding:
+        return Finding(name=data["Name"], finding_arn=data["FindingArn"])
```

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/suppress_findings.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/suppress_findings.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/suppression.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/suppression.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Optional, List, Any
+from typing import List
 
 from aws_securityhub_suppression.finding import Finding
 
 
 class Suppression:
     def __init__(self, name: str, reason: str, findings: List[Finding]) -> None:
         self.__name = name
@@ -19,15 +19,10 @@
         return self.__reason
 
     @property
     def findings(self) -> List[Finding]:
         return self.__findings
 
     @staticmethod
-    def from_dict(data: dict) -> Optional[Suppression]:
-        # TODO: Schema validation
-        if "Name" not in data:
-            return None
-
-        findings = list(map(Finding, data["Findings"]))
-
+    def from_dict(data: dict) -> Suppression:
+        findings = list(map(Finding.from_dict, data["Findings"]))
         return Suppression(name=data["Name"], reason=data["Reason"], findings=findings)
```

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/workload.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/workload.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
-
-from typing import Optional, List
+from typing import List
 
 from aws_securityhub_suppression import Account
 
 
 class Workload:
     def __init__(self, name: str, accounts: List[Account]) -> None:
         self.__name = name
@@ -15,13 +14,9 @@
         return self.__name
 
     @property
     def accounts(self) -> List[Account]:
         return self.__accounts
 
     @staticmethod
-    def from_dict(data: dict, accounts: List[Account]) -> Optional[Workload]:
-        # TODO: Schema validation
-        if "Name" not in data:
-            return None
-
+    def from_dict(data: dict, accounts: List[Account]) -> Workload:
         return Workload(name=data["Name"], accounts=accounts)
```

### Comparing `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/workload_generator.py` & `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/workload_generator.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.1/pyproject.toml` & `aws_securityhub_suppression-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-securityhub-suppression"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_securityhub_suppression"}]
 
 [tool.poetry.group.dev.dependencies]
@@ -28,14 +28,15 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 landingzone-organization = "^0.4.0"
 click = "^8.1.3"
 pyyaml = "^6.0"
 jinja2 = "^3.1.2"
 xenon = "^0.9.0"
+jsonschema = "^4.18.3"
 
 
 [tool.poetry.scripts]
 aws-securityhub-suppression = "aws_securityhub_suppression.cli:cli"
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `aws_securityhub_suppression-0.2.1/PKG-INFO` & `aws_securityhub_suppression-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: aws-securityhub-suppression
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: jsonschema (>=4.18.3,<5.0.0)
 Requires-Dist: landingzone-organization (>=0.4.0,<0.5.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: xenon (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # AWS SecurityHub - Suppression
 
-[![Maintenance](https://img.shields.io/badge/Maintained-yes-green.svg)](https://github.com/Nr18/pull-request-codecommit/graphs/commit-activity)
-[![GitHub release](https://img.shields.io/github/release/binxio/landingzone-organization.svg)](https://github.com/binxio/landingzone-organization/releases/)
-[![Continuous Integration](https://github.com/binxio/landingzone-organization/actions/workflows/ci.yml/badge.svg)](https://github.com/binxio/landingzone-organization/actions/workflows/ci.yml)
+[![Maintenance](https://img.shields.io/badge/Maintained-yes-green.svg)](https://github.com/Nr18/aws-securityhub-suppression/graphs/commit-activity)
+[![GitHub release](https://img.shields.io/github/release/binxio/aws-securityhub-suppression.svg)](https://github.com/binxio/aws-securityhub-suppression/releases/)
+[![Continuous Integration](https://github.com/binxio/aws-securityhub-suppression/actions/workflows/ci.yml/badge.svg)](https://github.com/binxio/aws-securityhub-suppression/actions/workflows/ci.yml)
 
 This tool allows you to manage your Suppression's as Code.
 
 **Useful links:**
 - [Documentation](https://binxio.github.io/aws-securityhub-suppression/)
 - [Bug Tracker](https://github.com/binxio/aws-securityhub-suppression/issues)
 - [PyPi](https://pypi.org/project/aws-securityhub-suppression/)
```

