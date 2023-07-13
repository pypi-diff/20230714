# Comparing `tmp/threemystic_cloud_client-0.1.29.tar.gz` & `tmp/threemystic_cloud_client-0.1.30.tar.gz`

## Comparing `threemystic_cloud_client-0.1.29.tar` & `threemystic_cloud_client-0.1.30.tar`

### file list

```diff
@@ -1,42 +1,45 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/action_token/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12138 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    22252 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
--rw-r--r--   0        0        0    16112 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    17146 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/hatch.toml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/pyproject.toml
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cli/actions/action_generate/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cli/actions/action_token/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12138 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    23229 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
+-rw-r--r--   0        0        0    16112 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    17146 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/hatch.toml
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/pyproject.toml
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.30/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,21 @@
         "--token": {
             "default": None, 
             "const": "token",
             "dest": "client_action",
             "help": "Action: This is so that you can generate the required token.",
             "action": 'store_const'
         },
+        "--generate,-g": {
+            "default": None, 
+            "const": "generate",
+            "dest": "client_action",
+            "help": "Action: For providers like aws it is easier to have a profile when interacting with the accounts. This will help generate the various profiles.",
+            "action": 'store_const'
+        },
         "--provider,-p": {
             "default": None, 
             "type": str,
             "choices": self._cloud_client.get_supported_providers(),
             "dest": "client_provider",
             "help": "Provider: This is to set the provider that should be used",
             "action": 'store'
@@ -94,14 +101,19 @@
       return
 
     if force_action == "token":
       from threemystic_cloud_client.cli.actions.action_token import cloud_client_token as user_action
       user_action(cloud_client= self._cloud_client).main(provider= self.__get_client_provider())
       return
 
+    if force_action == "generate":
+      from threemystic_cloud_client.cli.actions.action_generate import cloud_client_generate as user_action
+      user_action(cloud_client= self._cloud_client).main(provider= self.__get_client_provider())
+      return
+
     return
 
   def version_dispaly(self, *args, **kwargs): 
     print(f"You currenly have installed")
     print(f"3mystic_cloud_client: v{self._cloud_client.version()}")
     print(f"3mystic_common: v{self._cloud_client.get_common().version()}")
     print()
```

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/action_token/__init__.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cli/actions/action_token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,33 @@
   
   def action_test(self, *args, **kwargs):
     if not self.is_provider_config_completed():
       print("Provider must be configured first")
       self._setup_another_config()
       return
     from threemystic_cloud_client.cloud_providers.aws.action_test.step_1 import cloud_client_aws_test_step_1 as test
-    next_step = test(common= self.get_common(), logger= self.get_logger(), *args, **kwargs)
+    next_step = test(common= self.get_common(), logger= self.get_common().get_logger(), *args, **kwargs)
     
     next_step.step()
 
   def action_config(self, *args, **kwargs):     
     from threemystic_cloud_client.cloud_providers.aws.config.step_1 import cloud_client_aws_config_step_1 as step
-    next_step = step(common= self.get_common(), logger= self.get_logger())
+    next_step = step(common= self.get_common(), logger= self.get_common().get_logger())
     
     next_step.step()
 
   def action_token(self, *args, **kwargs):     
     from threemystic_cloud_client.cloud_providers.aws.action_token.step_1 import cloud_client_aws_token_step_1 as step
-    next_step = step(common= self.get_common(), logger= self.get_logger())
+    next_step = step(common= self.get_common(), logger= self.get_common().get_logger())
+    
+    next_step.step()
+
+  def action_generate(self, *args, **kwargs):     
+    from threemystic_cloud_client.cloud_providers.aws.action_generate.step_1 import cloud_client_aws_generate_step_1 as step
+    next_step = step(common= self.get_common(), logger= self.get_common().get_logger())
     
     next_step.step()
```

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     
 
   def step(self, profile_name, *args, **kwargs):
     if not super().step(*args, **kwargs):
       return
     
     from threemystic_cloud_client.cloud_client import cloud_client
-    aws_client = cloud_client(logger= self.get_logger(), common=self.get_common()).client(
+    aws_client = cloud_client(logger= self.get_common().get_logger(), common=self.get_common()).client(
       provider= "aws",
       profile_name= profile_name
     )
 
     
     print(f"Connected to Account ID: {aws_client.get_main_account_id()}")
     print(f"Org Account ID: {aws_client.get_organization_account_id()}")
```

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -384,29 +384,54 @@
   def _auto_parse_aws_expiration(self, expiration, *argv, **kwargs):
     if self.get_common().helper_type().general().is_type(obj= expiration, type_check= int):
       return self.get_common().helper_type().datetime().get_from_timestamp(time_delta=expiration)
     
     if self.get_common().helper_type().general().is_type(obj= expiration, type_check= str):
       return self.get_common().helper_type().datetime().parse_iso(iso_datetime_str=expiration)
     
+
+  def convert_assume_role_credentials_export(self, credentials):
+    
+    outputData = f"\nexport AWS_ACCESS_KEY_ID=\"{credentials['AccessKeyId']}\"\n"
+    outputData += f"export AWS_SECRET_ACCESS_KEY=\"{credentials['SecretAccessKey']}\"\n"
+    outputData += f"export AWS_SESSION_TOKEN=\"{credentials['SessionToken']}\"\n"
+    outputData += f"export AWS_DEFAULT_REGION=\"{self.get_default_region()}\"\n"
+
+    return outputData
+  
+  def convert_assume_role_credentials_cli(self, credentials):
+    # https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-sourcing-external.html
+    expiration = self._auto_parse_aws_expiration(
+      expiration= credentials["expiration"]
+    )
+
+    return {
+      "Version": 1,
+      "AccessKeyId": credentials["accessKeyId"],
+      "SecretAccessKey": credentials["secretAccessKey"],
+      "SessionToken": credentials["sessionToken"],
+      "Expiration": self.get_common().helper_type().datetime().get_iso_datetime(
+        dt= expiration
+      )
+    }
         
-  def _convert_assume_role_credentials_boto_session(self, credentials):
+  def convert_assume_role_credentials_boto_session(self, credentials):
     expiration = self._auto_parse_aws_expiration(
       expiration= credentials["expiration"]
     )
     
 
     return {
-        "access_key": credentials["accessKeyId"],
-        "secret_key": credentials["secretAccessKey"],
-        "token": credentials["sessionToken"],
-        "expiry_time": self.get_common().helper_type().datetime().get_iso_datetime(
-          dt= expiration
-        )
-      }
+      "access_key": credentials["accessKeyId"],
+      "secret_key": credentials["secretAccessKey"],
+      "token": credentials["sessionToken"],
+      "expiry_time": self.get_common().helper_type().datetime().get_iso_datetime(
+        dt= expiration
+      )
+    }
 
 
   def __get_boto_session(self, role = None, region = None, profile = None, **kwargs):
     if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile):
       return boto_session(profile_name= profile) if self.get_common().helper_type().string().is_null_or_whitespace(string_value= region) else boto_session(profile_name= profile, region_name= region)
 
     return botocore_session.get_session()
@@ -427,16 +452,16 @@
       return self._get_created_boto_sessions().get(cache_key)
 
     session = self.__get_boto_session(
       account=account, role = role, region = region, profile = profile
     )     
 
     credentials = botocore_credentials.RefreshableCredentials.create_from_metadata(
-      metadata=self._convert_assume_role_credentials_boto_session(self.assume_role(account=account, role=role)),
-      refresh_using=lambda: self._convert_assume_role_credentials_boto_session(self.assume_role(account=account, role=role, refresh= True)),
+      metadata=self.convert_assume_role_credentials_boto_session(self.assume_role(account=account, role=role)),
+      refresh_using=lambda: self.convert_assume_role_credentials_boto_session(self.assume_role(account=account, role=role, refresh= True)),
       method="sts-assume-role",
     )
 
     session._credentials = credentials 
     session.set_config_variable("region", region)
       
     self._get_created_boto_sessions()[cache_key] = boto_session(botocore_session= session)
```

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,27 @@
   def action_test(self, *args, **kwargs):    
     if not self.is_provider_config_completed():
       print("Provider must be configured first")
       self._setup_another_config()
       return
     
     from threemystic_cloud_client.cloud_providers.azure.action_test.step_1 import cloud_client_azure_test_step_1 as test
-    next_step = test(common= self.get_common(), logger= self.get_logger(), *args, **kwargs)
+    next_step = test(common= self.get_common(), logger= self.get_common().get_logger(), *args, **kwargs)
     
     next_step.step()
   
   def action_config(self, *args, **kwargs):     
     from threemystic_cloud_client.cloud_providers.azure.config.step_1 import cloud_client_azure_config_step_1 as step
-    next_step = step(common= self.get_common(), logger= self.get_logger())
+    next_step = step(common= self.get_common(), logger= self.get_common().get_logger())
     
     next_step.step()
   
   def action_token(self, *args, **kwargs):     
     from threemystic_cloud_client.cloud_providers.azure.action_token.step_1 import cloud_client_azure_token_step_1 as step
-    next_step = step(common= self.get_common(), logger= self.get_logger())
+    next_step = step(common= self.get_common(), logger= self.get_common().get_logger())
     
     next_step.step()
```

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     
 
   def step(self, *args, **kwargs):
     if not super().step( *args, **kwargs):
       return
     
     from threemystic_cloud_client.cloud_client import cloud_client
-    azure_client = cloud_client(logger= self.get_logger(), common=self.get_common()).client(
+    azure_client = cloud_client(logger= self.get_common().get_logger(), common=self.get_common()).client(
       provider= "azure"
     )
     
     print(f"You have the following tenants:")
     for tenant in azure_client.get_tenants():
       print(f"{azure_client.get_tenant_id(tenant= tenant)}")
```

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     
     if (self.get_common().helper_type().string().is_null_or_whitespace(string_value= self._processed_arg_info.get("token_tenant")) or (self.get_common().helper_type().string().is_null_or_whitespace(string_value= self._processed_arg_info.get("token_resource")) and 
       self.get_common().helper_type().string().is_null_or_whitespace(string_value= self._processed_arg_info.get("token_resource_type")))):
       self._arg_parser.print_help()
       return
 
     from threemystic_cloud_client.cloud_client import cloud_client
-    azure_client = cloud_client(logger= self.get_logger(), common=self.get_common()).client(
+    azure_client = cloud_client(logger= self.get_common().get_logger(), common=self.get_common()).client(
       provider= "azure"
     )
     
     tenant_credential = azure_client.get_tenant_credential(
       tenant= self._processed_arg_info.get("token_tenant")
     )
```

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.30/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,12 +194,15 @@
   
   def action_test(self, *args, **kwargs):
     print("Provider test config not configured")
   
   def action_token(self, *args, **kwargs):
     print("Provider token config not configured")
 
+  def action_generate(self, *args, **kwargs):     
+    print("Provider generate config not configured/not needed")
+
```

### Comparing `threemystic_cloud_client-0.1.29/.gitignore` & `threemystic_cloud_client-0.1.30/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/LICENSE` & `threemystic_cloud_client-0.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/README.md` & `threemystic_cloud_client-0.1.30/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/hatch.toml` & `threemystic_cloud_client-0.1.30/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.29/pyproject.toml` & `threemystic_cloud_client-0.1.30/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.10",
+  "threemystic-common >= 0.1.11",
   "polling2 >= 0.5.0",
   "typing-extensions >= 4.4.0",
   "pyopenssl >= 22.1.0",
   "PyJWT >= 2.7.0",
   "cryptography >= 41.0.1",
   "boto3 >= 1.26.151",
   "botocore >= 1.29.151",
```

### Comparing `threemystic_cloud_client-0.1.29/PKG-INFO` & `threemystic_cloud_client-0.1.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.29
+Version: 0.1.30
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 Requires-Dist: boto3>=1.26.151
 Requires-Dist: botocore>=1.29.151
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: cryptography>=41.0.1
 Requires-Dist: polling2>=0.5.0
 Requires-Dist: pyjwt>=2.7.0
 Requires-Dist: pyopenssl>=22.1.0
-Requires-Dist: threemystic-common>=0.1.10
+Requires-Dist: threemystic-common>=0.1.11
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_client
 A tool to help uniform the connection to the cloud providers.
 Currently supports AWS/Azure
```

