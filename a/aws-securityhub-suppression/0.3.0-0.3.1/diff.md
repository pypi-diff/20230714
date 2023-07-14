# Comparing `tmp/aws_securityhub_suppression-0.3.0.tar.gz` & `tmp/aws_securityhub_suppression-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_securityhub_suppression-0.3.0.tar", max compression
+gzip compressed data, was "aws_securityhub_suppression-0.3.1.tar", max compression
```

## Comparing `aws_securityhub_suppression-0.3.0.tar` & `aws_securityhub_suppression-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      836 2023-07-14 15:08:25.449800 aws_securityhub_suppression-0.3.0/README.md
--rw-r--r--   0        0        0     1453 2023-07-14 15:08:26.457805 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/__init__.py
--rw-r--r--   0        0        0      948 2023-07-14 15:08:25.449800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/account.py
--rw-r--r--   0        0        0      515 2023-07-14 15:08:25.449800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 15:08:25.449800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-14 15:08:25.449800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/check.py
--rw-r--r--   0        0        0      970 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/prepare.py
--rw-r--r--   0        0        0     1583 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/update.py
--rw-r--r--   0        0        0      793 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/context.py
--rw-r--r--   0        0        0      744 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/handler.py
--rw-r--r--   0        0        0     1133 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/documentation_generator.py
--rw-r--r--   0        0        0     1303 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/finding.py
--rw-r--r--   0        0        0      830 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/schemas/__init__.py
--rw-r--r--   0        0        0      793 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/schemas/environment.yaml
--rw-r--r--   0        0        0      158 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/schemas/workload.yaml
--rw-r--r--   0        0        0     1307 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/suppress_findings.py
--rw-r--r--   0        0        0      759 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/suppression.py
--rw-r--r--   0        0        0      561 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/workload.py
--rw-r--r--   0        0        0     1695 2023-07-14 15:08:25.453800 aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/workload_generator.py
--rw-r--r--   0        0        0     1220 2023-07-14 15:08:26.457805 aws_securityhub_suppression-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 aws_securityhub_suppression-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      836 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/README.md
+-rw-r--r--   0        0        0     1453 2023-07-14 18:51:48.883242 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/__init__.py
+-rw-r--r--   0        0        0      948 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/account.py
+-rw-r--r--   0        0        0      515 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/check.py
+-rw-r--r--   0        0        0      970 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/prepare.py
+-rw-r--r--   0        0        0     1583 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/update.py
+-rw-r--r--   0        0        0      793 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/context.py
+-rw-r--r--   0        0        0      744 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/handler.py
+-rw-r--r--   0        0        0     1133 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/documentation_generator.py
+-rw-r--r--   0        0        0     1303 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/finding.py
+-rw-r--r--   0        0        0      830 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/schemas/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/schemas/environment.yaml
+-rw-r--r--   0        0        0      158 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/schemas/workload.yaml
+-rw-r--r--   0        0        0     1307 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/suppress_findings.py
+-rw-r--r--   0        0        0      759 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/suppression.py
+-rw-r--r--   0        0        0      561 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/workload.py
+-rw-r--r--   0        0        0     2011 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/workload_generator.py
+-rw-r--r--   0        0        0     1220 2023-07-14 18:51:48.883242 aws_securityhub_suppression-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 aws_securityhub_suppression-0.3.1/PKG-INFO
```

### Comparing `aws_securityhub_suppression-0.3.0/README.md` & `aws_securityhub_suppression-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/__init__.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     safe_load_file,
 )
 from aws_securityhub_suppression.workload import Workload
 from aws_securityhub_suppression.suppression import Suppression
 from aws_securityhub_suppression.finding import Finding
 
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 
 def load_workloads(workload_path: str) -> List[Workload]:
     workloads = glob.glob(os.path.join(workload_path, "**/info.yaml"), recursive=True)
 
     def load_workload(file: str) -> Optional[Workload]:
         return load_workload_by_file(file)
```

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/account.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/account.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/__init__.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/check.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/prepare.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/prepare.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/commands/update.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/context.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/context.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/cli/handler.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/documentation_generator.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/finding.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/finding.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/schemas/__init__.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/schemas/environment.yaml` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/schemas/environment.yaml`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/suppress_findings.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/suppress_findings.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/suppression.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/suppression.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/workload.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/workload.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.0/aws_securityhub_suppression/workload_generator.py` & `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/workload_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,20 +17,26 @@
     def __ensure_folder(path: str) -> None:
         if not os.path.isdir(path):
             os.mkdir(path)
 
     def __resolve_workload_info(self, file: str) -> dict:
         info = {
             "Name": self.__workload.name,
+            "Environments": list(
+                map(lambda account: account.environment, self.__workload.accounts)
+            ),
         }
 
         if os.path.isfile(file):
             with open(file, "r") as fh:
                 info = yaml.safe_load(fh)
                 info["Name"] = self.__workload.name
+                info["Environments"] = list(
+                    map(lambda account: account.environment, self.__workload.accounts)
+                )
 
         return info
 
     @staticmethod
     def __resolve_account_info(account: Account) -> dict:
         return {
             "Name": account.name,
@@ -40,15 +46,15 @@
 
     def __prepare_workload_folder(self, path: str) -> None:
         self.__ensure_folder(path)
         file = os.path.join(path, "info.yaml")
         info = self.__resolve_workload_info(file)
 
         with open(file, "w") as fh:
-            yaml.dump(info, fh)
+            yaml.dump(info, fh, sort_keys=False)
 
         for account in self.__workload.accounts:
             environment_file = os.path.join(path, f"{account.environment}.yaml")
 
             if not os.path.isfile(environment_file):
                 with open(environment_file, "w") as fh:
-                    yaml.dump(self.__resolve_account_info(account), fh)
+                    yaml.dump(self.__resolve_account_info(account), fh, sort_keys=False)
```

### Comparing `aws_securityhub_suppression-0.3.0/pyproject.toml` & `aws_securityhub_suppression-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-securityhub-suppression"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_securityhub_suppression"}]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aws_securityhub_suppression-0.3.0/PKG-INFO` & `aws_securityhub_suppression-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-securityhub-suppression
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

