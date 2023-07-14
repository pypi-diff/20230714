# Comparing `tmp/msal_requests_auth-0.7.0.tar.gz` & `tmp/msal_requests_auth-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msal_requests_auth-0.7.0.tar", last modified: Fri Apr 28 19:32:48 2023, max compression
+gzip compressed data, was "msal_requests_auth-0.7.1.tar", last modified: Fri Jul 14 14:46:49 2023, max compression
```

## Comparing `msal_requests_auth-0.7.0.tar` & `msal_requests_auth-0.7.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/msal_requests_auth/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/msal_requests_auth/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/auth/base_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/auth/client_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/auth/device_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/test/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/test/test_client_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/test/test_devide_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/msal_requests_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/msal_requests_auth/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/auth/base_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/auth/client_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/auth/device_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/test/test_client_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/test/test_devide_code.py
```

### Comparing `msal_requests_auth-0.7.0/AUTHORS.rst` & `msal_requests_auth-0.7.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.0/CODE_OF_CONDUCT.rst` & `msal_requests_auth-0.7.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.0/CONTRIBUTING.rst` & `msal_requests_auth-0.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.0/LICENSE` & `msal_requests_auth-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.0/PKG-INFO` & `msal_requests_auth-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal_requests_auth
-Version: 0.7.0
+Version: 0.7.1
 Summary: Authentication using python requests and MSAL
 Home-page: https://github.com/corteva/msal-requests-auth
 Download-URL: http://python.org/pypi/msal-requests-auth
 Author: msal_requests_auth Contributors
 Author-email: alansnow21@gmail.com
 License: BSD License
 Keywords: msal,requests
```

### Comparing `msal_requests_auth-0.7.0/README.rst` & `msal_requests_auth-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.0/msal_requests_auth/auth/base_auth_client.py` & `msal_requests_auth-0.7.1/msal_requests_auth/auth/base_auth_client.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.0/msal_requests_auth/auth/client_credential.py` & `msal_requests_auth-0.7.1/msal_requests_auth/auth/client_credential.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.0/msal_requests_auth/auth/device_code.py` & `msal_requests_auth-0.7.1/msal_requests_auth/auth/device_code.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.0/msal_requests_auth.egg-info/PKG-INFO` & `msal_requests_auth-0.7.1/msal_requests_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal-requests-auth
-Version: 0.7.0
+Version: 0.7.1
 Summary: Authentication using python requests and MSAL
 Home-page: https://github.com/corteva/msal-requests-auth
 Download-URL: http://python.org/pypi/msal-requests-auth
 Author: msal_requests_auth Contributors
 Author-email: alansnow21@gmail.com
 License: BSD License
 Keywords: msal,requests
```

### Comparing `msal_requests_auth-0.7.0/msal_requests_auth.egg-info/SOURCES.txt` & `msal_requests_auth-0.7.1/msal_requests_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.0/setup.cfg` & `msal_requests_auth-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.0/test/test_cache.py` & `msal_requests_auth-0.7.1/test/test_cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from unittest.mock import patch
 
+import pytest
+
 from msal_requests_auth.cache import KeyringTokenCache, SimpleTokenCache
 
 
 @patch("msal_requests_auth.cache.user_cache_dir")
 @patch("msal_requests_auth.cache.SimpleTokenCache.serialize")
 def test_simple_token_cache(serialize_mock, user_cache_dir_mock, tmp_path):
     serialize_mock.return_value = "TEST"
@@ -85,7 +87,54 @@
 
 @patch("msal_requests_auth.cache._import_keyring")
 @patch("msal_requests_auth.cache.KeyringTokenCache.deserialize")
 def test_keyring_token_cache__deserialize(deserialize_mock, keyring_mock):
     keyring_mock.return_value.get_password.return_value = "TEST"
     KeyringTokenCache()
     deserialize_mock.assert_called_with("TEST")
+
+
+@patch("msal_requests_auth.cache._import_keyring")
+@patch("msal_requests_auth.cache.KeyringTokenCache.serialize")
+def test_keyring_token_cache__write_cache__windows_error(serialize_mock, keyring_mock):
+    class MyException(Exception):
+        def __init__(self, *args, **kwargs) -> None:
+            self.winerror = 1783
+            super().__init__(*args, **kwargs)
+
+    keyring_mock.return_value.set_password.side_effect = MyException
+
+    serialize_mock.return_value = "TEST"
+    keyring_mock.return_value.get_password.return_value = None
+    with KeyringTokenCache() as cache:
+        pass
+    keyring_mock.return_value.get_password.assert_called_with(
+        "__msal_requests_auth__", "token"
+    )
+    keyring_mock.return_value.set_password.assert_not_called()
+    cache.has_state_changed = True
+    with pytest.warns(match="Token cache skipped due to error writing to keyring"):
+        with KeyringTokenCache() as cache:
+            cache.has_state_changed = True
+    keyring_mock.return_value.set_password.assert_called_with(
+        "__msal_requests_auth__", "token", "TEST"
+    )
+
+
+@patch("msal_requests_auth.cache._import_keyring")
+@patch("msal_requests_auth.cache.KeyringTokenCache.serialize")
+def test_keyring_token_cache__write_cache__error(serialize_mock, keyring_mock):
+    keyring_mock.return_value.set_password.side_effect = RuntimeError
+    serialize_mock.return_value = "TEST"
+    keyring_mock.return_value.get_password.return_value = None
+    with KeyringTokenCache() as cache:
+        pass
+    keyring_mock.return_value.get_password.assert_called_with(
+        "__msal_requests_auth__", "token"
+    )
+    keyring_mock.return_value.set_password.assert_not_called()
+    with pytest.raises(RuntimeError):
+        with KeyringTokenCache() as cache:
+            cache.has_state_changed = True
+    keyring_mock.return_value.set_password.assert_called_with(
+        "__msal_requests_auth__", "token", "TEST"
+    )
```

### Comparing `msal_requests_auth-0.7.0/test/test_client_credential.py` & `msal_requests_auth-0.7.1/test/test_client_credential.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.0/test/test_devide_code.py` & `msal_requests_auth-0.7.1/test/test_devide_code.py`

 * *Files identical despite different names*

