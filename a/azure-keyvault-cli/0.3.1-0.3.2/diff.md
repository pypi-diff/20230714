# Comparing `tmp/azure_keyvault_cli-0.3.1.tar.gz` & `tmp/azure_keyvault_cli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_keyvault_cli-0.3.1.tar", max compression
+gzip compressed data, was "azure_keyvault_cli-0.3.2.tar", max compression
```

## Comparing `azure_keyvault_cli-0.3.1.tar` & `azure_keyvault_cli-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0     3920 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/__init__.py
--rw-r--r--   0        0        0      388 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/azkv.py
--rw-r--r--   0        0        0        0 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/client/__init__.py
--rw-r--r--   0        0        0     3826 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/client/keyvault_client.py
--rw-r--r--   0        0        0     2845 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/client/keyvault_clients.py
--rw-r--r--   0        0        0      748 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/client/keyvault_secret.py
--rw-r--r--   0        0        0        0 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/commands/__init__.py
--rw-r--r--   0        0        0     1245 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/commands/check.py
--rw-r--r--   0        0        0     3032 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/commands/common.py
--rw-r--r--   0        0        0     1790 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/commands/edit.py
--rw-r--r--   0        0        0     1951 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/commands/show.py
--rw-r--r--   0        0        0        0 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/commands/vaults/__init__.py
--rw-r--r--   0        0        0      713 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/commands/vaults/add.py
--rw-r--r--   0        0        0      585 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/commands/vaults/login.py
--rw-r--r--   0        0        0     1402 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/commands/vaults/main.py
--rw-r--r--   0        0        0      728 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/commands/vaults/remove.py
--rw-r--r--   0        0        0      464 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/commands/vaults/select.py
--rw-r--r--   0        0        0      482 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/decorators.py
--rw-r--r--   0        0        0     2322 2023-06-29 17:28:05.358646 azure_keyvault_cli-0.3.1/cli/main.py
--rw-r--r--   0        0        0     1019 2023-06-29 17:28:05.362646 azure_keyvault_cli-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4948 1970-01-01 00:00:00.000000 azure_keyvault_cli-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     3920 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/__init__.py
+-rw-r--r--   0        0        0      388 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/azkv.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/client/__init__.py
+-rw-r--r--   0        0        0     3826 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/client/keyvault_client.py
+-rw-r--r--   0        0        0     2868 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/client/keyvault_clients.py
+-rw-r--r--   0        0        0      748 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/client/keyvault_secret.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1245 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/commands/check.py
+-rw-r--r--   0        0        0     3032 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/commands/common.py
+-rw-r--r--   0        0        0     1790 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/commands/edit.py
+-rw-r--r--   0        0        0     1951 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/commands/show.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/commands/vaults/__init__.py
+-rw-r--r--   0        0        0      797 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/commands/vaults/add.py
+-rw-r--r--   0        0        0      688 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/commands/vaults/login.py
+-rw-r--r--   0        0        0     2087 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/commands/vaults/main.py
+-rw-r--r--   0        0        0      833 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/commands/vaults/remove.py
+-rw-r--r--   0        0        0      451 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/commands/vaults/select.py
+-rw-r--r--   0        0        0      482 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/decorators.py
+-rw-r--r--   0        0        0     2322 2023-07-14 10:51:38.045276 azure_keyvault_cli-0.3.2/cli/main.py
+-rw-r--r--   0        0        0     1019 2023-07-14 10:51:38.049276 azure_keyvault_cli-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4948 1970-01-01 00:00:00.000000 azure_keyvault_cli-0.3.2/PKG-INFO
```

### Comparing `azure_keyvault_cli-0.3.1/LICENSE.txt` & `azure_keyvault_cli-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `azure_keyvault_cli-0.3.1/README.md` & `azure_keyvault_cli-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `azure_keyvault_cli-0.3.1/cli/client/keyvault_client.py` & `azure_keyvault_cli-0.3.2/cli/client/keyvault_client.py`

 * *Files identical despite different names*

### Comparing `azure_keyvault_cli-0.3.1/cli/client/keyvault_clients.py` & `azure_keyvault_cli-0.3.2/cli/client/keyvault_clients.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,20 @@
     @property
     def location(self):
         return self._location
 
     def add_client(self, client: KeyVaultClient):
         if client.vault_url in self.clients:
             raise ValueError("Client already exists")
-        self.clients[client.vault_url] = client
+        self.clients[client.vault_url] = client  # type: ignore
         self.save()
 
     def remove_client(self, client: KeyVaultClient):
         try:
-            del self.clients[client.settings.vault_url]
+            del self.clients[client.vault_url]  # type: ignore
         except KeyError:
             pass
         self.save()
 
     def login(self):
         for client in self.clients.values():
             if not self._is_valid():
```

### Comparing `azure_keyvault_cli-0.3.1/cli/client/keyvault_secret.py` & `azure_keyvault_cli-0.3.2/cli/client/keyvault_secret.py`

 * *Files identical despite different names*

### Comparing `azure_keyvault_cli-0.3.1/cli/commands/check.py` & `azure_keyvault_cli-0.3.2/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `azure_keyvault_cli-0.3.1/cli/commands/common.py` & `azure_keyvault_cli-0.3.2/cli/commands/common.py`

 * *Files identical despite different names*

### Comparing `azure_keyvault_cli-0.3.1/cli/commands/edit.py` & `azure_keyvault_cli-0.3.2/cli/commands/edit.py`

 * *Files identical despite different names*

### Comparing `azure_keyvault_cli-0.3.1/cli/commands/show.py` & `azure_keyvault_cli-0.3.2/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `azure_keyvault_cli-0.3.1/cli/commands/vaults/add.py` & `azure_keyvault_cli-0.3.2/cli/commands/vaults/add.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,11 +17,13 @@
     kv.login()
     clients.add_client(kv)
 
 
 def is_valid_url(url):
     try:
         url = url.strip('"').strip("'").strip()
+        if not url.startswith(("http://", "https://")):
+            raise Exception
         result = urlparse(url)
         return all([result.scheme, result.netloc])
     except Exception:
         return False
```

### Comparing `azure_keyvault_cli-0.3.1/cli/commands/vaults/login.py` & `azure_keyvault_cli-0.3.2/cli/commands/vaults/login.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 from InquirerPy.base.control import Choice
 
 
 def login(clients, vault_url=None):
     if not vault_url:
         choices = []
         for client in clients.clients.values():
-            choices.append(Choice(value=client.settings.vault_url, enabled=True))
-        vault_url = inquirer.list(
+            choices.append(Choice(value=client.vault_url, enabled=True))
+        vault_url = inquirer.select(
             message="Select vault to login:",
             choices=choices,
             validate=lambda v: len(v) >= 1,
             invalid_message="At least one vault must be selected",
         ).execute()
-    clients.clients[vault_url].login()
-    clients.save()
+    try:
+        clients.clients[vault_url].login(force_reauth=True)
+        clients.save()
+    except KeyError:
+        raise KeyError(f"Vault {vault_url} not found")
```

### Comparing `azure_keyvault_cli-0.3.1/cli/commands/vaults/remove.py` & `azure_keyvault_cli-0.3.2/cli/commands/vaults/remove.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 from InquirerPy.base.control import Choice
 
 
 def remove(clients, vault_url=None):
     if not vault_url:
         choices = []
         for client in clients.clients.values():
-            choices.append(Choice(value=client.settings.vault_url, enabled=True))
+            choices.append(Choice(value=client.vault_url, enabled=True))
         vault_url = inquirer.select(
             message="Select vault to remove:",
             choices=choices,
             validate=lambda v: len(v) >= 1,
             invalid_message="You must select a vault to remove",
         ).execute()
+    else:
+        if vault_url not in clients.clients:
+            raise KeyError(f"Vault {vault_url} not found")
     proceed = inquirer.confirm(
         message="Are you sure you want to remove this vault?", default=False
     ).execute()
     if proceed:
         clients.remove_client(clients.clients[vault_url])
```

### Comparing `azure_keyvault_cli-0.3.1/cli/main.py` & `azure_keyvault_cli-0.3.2/cli/main.py`

 * *Files identical despite different names*

### Comparing `azure_keyvault_cli-0.3.1/pyproject.toml` & `azure_keyvault_cli-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "azure-keyvault-cli"
-version = "0.3.1"
+version = "0.3.2"
 description = "This is a CLI to show and check secrets from an Azure KeyVault"
 authors = ["mkah91 <marius_knepper@web.de>"]
 repository = "https://github.com/mkah91/azure-keyvault-cli"
 keywords = ["azure", "keyvault", "cli", "secrets"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cli"}]
```

### Comparing `azure_keyvault_cli-0.3.1/PKG-INFO` & `azure_keyvault_cli-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-keyvault-cli
-Version: 0.3.1
+Version: 0.3.2
 Summary: This is a CLI to show and check secrets from an Azure KeyVault
 Home-page: https://github.com/mkah91/azure-keyvault-cli
 License: MIT
 Keywords: azure,keyvault,cli,secrets
 Author: mkah91
 Author-email: marius_knepper@web.de
 Requires-Python: >=3.9,<4.0
```

