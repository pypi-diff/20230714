# Comparing `tmp/ievv_auth-3.0.0.tar.gz` & `tmp/ievv_auth-3.1.0.tar.gz`

## Comparing `ievv_auth-3.0.0.tar` & `ievv_auth-3.1.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/__init__.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/version.json
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/README.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/__init__.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/admin.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/apps.py
--rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/models.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/management/commands/__init__.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/migrations/0002_auto_20201119_1956.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/tests/__init__.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_api_key/tests/test_models.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/README.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/admin.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/apps.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/exceptions.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/models.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/settings.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/__init__.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/authentication.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/serializers/__init__.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/serializers/api_key_serializers.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/views/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/views/api_key_views.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/views/base_view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/__init__.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/api_key_backend.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/backend_registry.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/base_backend.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/__init__.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_api/__init__.py
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_api/api_test_mixin.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_api/test_api_key_views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/__init__.py
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_api_key_backend.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_backend_registry.py
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_base_backend.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/utils/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/utils/deep_merge.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/ievv_jwt/utils/load_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/settingsproxy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/default/__init__.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/default/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/develop/__init__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/develop/common_settings.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/develop/develop_settings.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/ievv_auth/project/develop/test_settings.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/.gitignore
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/LICENSE
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/README.md
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 ievv_auth-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/__init__.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/version.json
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/README.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/__init__.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/admin.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/apps.py
+-rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/models.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/management/commands/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/migrations/0002_auto_20201119_1956.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/tests/__init__.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_api_key/tests/test_models.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/admin.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/apps.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/exceptions.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/models.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/settings.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/api/__init__.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/api/authentication.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/api/serializers/__init__.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/api/serializers/api_key_serializers.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/api/views/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/api/views/api_key_views.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/api/views/base_view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/backends/__init__.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/backends/api_key_backend.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/backends/backend_registry.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/backends/base_backend.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/__init__.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_api/__init__.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_api/api_test_mixin.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_api/test_api_key_views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_backends/__init__.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_backends/test_api_key_backend.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_backends/test_backend_registry.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_backends/test_base_backend.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/utils/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/utils/deep_merge.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/ievv_jwt/utils/load_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/project/__init__.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/project/settingsproxy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/project/default/__init__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/project/default/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/project/develop/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/project/develop/common_settings.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/project/develop/develop_settings.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/ievv_auth/project/develop/test_settings.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/.gitignore
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/LICENSE
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/README.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 ievv_auth-3.1.0/PKG-INFO
```

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_api_key/README.md` & `ievv_auth-3.1.0/ievv_auth/ievv_api_key/README.md`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_api_key/admin.py` & `ievv_auth-3.1.0/ievv_auth/ievv_api_key/admin.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_api_key/models.py` & `ievv_auth-3.1.0/ievv_auth/ievv_api_key/models.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_api_key/migrations/0001_initial.py` & `ievv_auth-3.1.0/ievv_auth/ievv_api_key/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_api_key/migrations/0002_auto_20201119_1956.py` & `ievv_auth-3.1.0/ievv_auth/ievv_api_key/migrations/0002_auto_20201119_1956.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_api_key/tests/test_models.py` & `ievv_auth-3.1.0/ievv_auth/ievv_api_key/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/README.md` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/README.md`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/settings.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/settings.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/authentication.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/api/authentication.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/serializers/api_key_serializers.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/api/serializers/api_key_serializers.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/api/views/base_view.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/api/views/base_view.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/backend_registry.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/backends/backend_registry.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/backends/base_backend.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/backends/base_backend.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_utils.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_api/api_test_mixin.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_api/api_test_mixin.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_api/test_api_key_views.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_api/test_api_key_views.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_api_key_backend.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_backends/test_api_key_backend.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_backend_registry.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_backends/test_backend_registry.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/tests/test_backends/test_base_backend.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/tests/test_backends/test_base_backend.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/utils/deep_merge.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/utils/deep_merge.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/ievv_jwt/utils/load_settings.py` & `ievv_auth-3.1.0/ievv_auth/ievv_jwt/utils/load_settings.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/project/settingsproxy.py` & `ievv_auth-3.1.0/ievv_auth/project/settingsproxy.py`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/ievv_auth/project/default/settings.py` & `ievv_auth-3.1.0/ievv_auth/project/default/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 SECRET_KEY = 'gxha11rjtb_7l6^(mzx-q%=+5qeldh&p$jig0x!*&q&5lq$1j6'
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
 ALLOWED_HOSTS = []
 
-DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
+DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
 
 # Application definition
 
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
```

### Comparing `ievv_auth-3.0.0/LICENSE` & `ievv_auth-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ievv_auth-3.0.0/README.md` & `ievv_auth-3.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,34 @@
 ### Upgrade your local packages
 This will upgrade all local packages according to the constraints
 set in pyproject.toml:
 ```bash
 pip install --upgrade --upgrade-strategy=eager ".[dev,test]"
 ```
 
+### Docker compose and runserver
+Start
+```bash
+docker-compose up
+python manage.py runserver
+```
+
+Stop
+```bash
+docker-compose down
+```
+
+To wipe out the database, run:
+```bash
+docker-compose down -v
+docker-compose up
+python manage.py migrate
+python manage.py runserver
+```
+
 ### Run tests
 ```bash
 source .venv/bin/activate   # enable virtualenv
 pytest ievv_opensource
 ```
```

### Comparing `ievv_auth-3.0.0/pyproject.toml` & `ievv_auth-3.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,15 @@
     "ievv_opensource>=9.2.2,<10.0.0",
     "psycopg2",
     "PyJWT==1.7.1",
     "python-dateutil",
 ]
 
 [project.optional-dependencies]
-dev = [
-    'django-dbdev',
-]
+dev = []
 
 test = [
     'model-bakery',
     "pytest",
     "pytest-django",
     "pytest-env",
 ]
@@ -54,13 +52,13 @@
 packages = [
     "/ievv_auth",
 ]
 exclude = []
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.0.0"
+version = "3.1.0"
 version_files = [
     "ievv_auth/__init__.py:__version__"
 ]
 tag_format = "$version"
 update_changelog_on_bump = true
```

### Comparing `ievv_auth-3.0.0/PKG-INFO` & `ievv_auth-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ievv-auth
-Version: 3.0.0
+Version: 3.1.0
 Summary: Authentication modules for the Django framework.
 Project-URL: Homepage, https://github.com/appressoas/ievv_auth
 Author-email: Appresso developers <post@appresso.no>
 License: Copyright (c) 2020, Appresso AS
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -43,15 +43,14 @@
 Requires-Dist: django<5.0.0,>=4.0.0
 Requires-Dist: djangorestframework
 Requires-Dist: ievv-opensource<10.0.0,>=9.2.2
 Requires-Dist: psycopg2
 Requires-Dist: pyjwt==1.7.1
 Requires-Dist: python-dateutil
 Provides-Extra: dev
-Requires-Dist: django-dbdev; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: model-bakery; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-django; extra == 'test'
 Requires-Dist: pytest-env; extra == 'test'
 Description-Content-Type: text/markdown
 
@@ -124,14 +123,34 @@
 ### Upgrade your local packages
 This will upgrade all local packages according to the constraints
 set in pyproject.toml:
 ```bash
 pip install --upgrade --upgrade-strategy=eager ".[dev,test]"
 ```
 
+### Docker compose and runserver
+Start
+```bash
+docker-compose up
+python manage.py runserver
+```
+
+Stop
+```bash
+docker-compose down
+```
+
+To wipe out the database, run:
+```bash
+docker-compose down -v
+docker-compose up
+python manage.py migrate
+python manage.py runserver
+```
+
 ### Run tests
 ```bash
 source .venv/bin/activate   # enable virtualenv
 pytest ievv_opensource
 ```
```

