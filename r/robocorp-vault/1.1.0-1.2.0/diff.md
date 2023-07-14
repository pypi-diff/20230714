# Comparing `tmp/robocorp_vault-1.1.0.tar.gz` & `tmp/robocorp_vault-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_vault-1.1.0.tar", max compression
+gzip compressed data, was "robocorp_vault-1.2.0.tar", max compression
```

## Comparing `robocorp_vault-1.1.0.tar` & `robocorp_vault-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1193 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/README.md
--rw-r--r--   0        0        0      802 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5350 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/__init__.py
--rw-r--r--   0        0        0    12926 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_adapters.py
--rw-r--r--   0        0        0      112 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_errors.py
--rw-r--r--   0        0        0     6335 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_requests.py
--rw-r--r--   0        0        0     1587 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_secrets.py
--rw-r--r--   0        0        0     1858 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_utils.py
--rw-r--r--   0        0        0     3080 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/_vault.py
--rw-r--r--   0        0        0        0 2023-07-12 14:21:40.506984 robocorp_vault-1.1.0/src/robocorp/vault/py.typed
--rw-r--r--   0        0        0     1980 1970-01-01 00:00:00.000000 robocorp_vault-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3912 2023-07-14 16:06:45.087694 robocorp_vault-1.2.0/README.md
+-rw-r--r--   0        0        0      802 2023-07-14 16:06:45.087694 robocorp_vault-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4051 2023-07-14 16:06:45.087694 robocorp_vault-1.2.0/src/robocorp/vault/__init__.py
+-rw-r--r--   0        0        0    12926 2023-07-14 16:06:45.087694 robocorp_vault-1.2.0/src/robocorp/vault/_adapters.py
+-rw-r--r--   0        0        0      112 2023-07-14 16:06:45.087694 robocorp_vault-1.2.0/src/robocorp/vault/_errors.py
+-rw-r--r--   0        0        0     6335 2023-07-14 16:06:45.087694 robocorp_vault-1.2.0/src/robocorp/vault/_requests.py
+-rw-r--r--   0        0        0     1587 2023-07-14 16:06:45.087694 robocorp_vault-1.2.0/src/robocorp/vault/_secrets.py
+-rw-r--r--   0        0        0     1858 2023-07-14 16:06:45.087694 robocorp_vault-1.2.0/src/robocorp/vault/_utils.py
+-rw-r--r--   0        0        0     2945 2023-07-14 16:06:45.087694 robocorp_vault-1.2.0/src/robocorp/vault/_vault.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:06:45.087694 robocorp_vault-1.2.0/src/robocorp/vault/py.typed
+-rw-r--r--   0        0        0     4699 1970-01-01 00:00:00.000000 robocorp_vault-1.2.0/PKG-INFO
```

### Comparing `robocorp_vault-1.1.0/pyproject.toml` & `robocorp_vault-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-vault"
-version = "1.1.0"
+version = "1.2.0"
 description = "Robocorp Control Room Vault API integration library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
```

### Comparing `robocorp_vault-1.1.0/src/robocorp/vault/_adapters.py` & `robocorp_vault-1.2.0/src/robocorp/vault/_adapters.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-1.1.0/src/robocorp/vault/_requests.py` & `robocorp_vault-1.2.0/src/robocorp/vault/_requests.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-1.1.0/src/robocorp/vault/_secrets.py` & `robocorp_vault-1.2.0/src/robocorp/vault/_secrets.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-1.1.0/src/robocorp/vault/_utils.py` & `robocorp_vault-1.2.0/src/robocorp/vault/_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-1.1.0/src/robocorp/vault/_vault.py` & `robocorp_vault-1.2.0/src/robocorp/vault/_vault.py`

 * *Files 18% similar despite different names*

```diff
@@ -74,17 +74,13 @@
 
         Returns:
             `SecretContainer` object.
         """
         return self.adapter.get_secret(secret_name)
 
     def set_secret(self, secret: SecretContainer) -> None:
-        """Overwrite an existing secret with new values.
-
-        Note:
-            Only allows modifying existing secrets, and replaces
-              all values contained within it.
+        """Create secret or overwrite existing.
 
         Args:
             secret: `SecretContainer` object, from e.g. `get_secret`.
         """
         self.adapter.set_secret(secret)
```

