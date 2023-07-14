# Comparing `tmp/onqlave-python-sdk-pilot-0.0.3.tar.gz` & `tmp/onqlave-python-sdk-pilot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onqlave-python-sdk-pilot-0.0.3.tar", last modified: Fri Jul 14 02:03:19 2023, max compression
+gzip compressed data, was "onqlave-python-sdk-pilot-0.0.4.tar", last modified: Fri Jul 14 02:09:36 2023, max compression
```

## Comparing `onqlave-python-sdk-pilot-0.0.3.tar` & `onqlave-python-sdk-pilot-0.0.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.734202 onqlave-python-sdk-pilot-0.0.3/
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:03:19.734202 onqlave-python-sdk-pilot-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-02 14:43:10.000000 onqlave-python-sdk-pilot-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 03:10:41.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/connection/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3671 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/connection/client.py
--rw-r--r--   0 root         (0) root         (0)     3654 2023-07-14 01:57:58.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/connection/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-12 16:35:27.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/contracts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/requests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-14 01:58:58.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/requests/requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/responses/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/responses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-07-14 01:56:52.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/responses/responses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/credentials/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 16:39:18.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/credentials/credentials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:40:25.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2525 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/encrypted_stream_processor.py
--rw-r--r--   0 root         (0) root         (0)    10873 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/encryption.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-12 16:42:49.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/options.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/plain_stream_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)      825 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/id_service.py
--rw-r--r--   0 root         (0) root         (0)     7177 2023-07-14 01:58:27.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/key_manager_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1187 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/aes_gcm.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/xchacha_20_poly_1350.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/onqlave_types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/onqlave_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6737 2023-07-11 15:21:03.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/onqlave_types/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 06:40:20.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      720 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/aes_128_gcm_operation.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/aes_256_gcm_operation.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
--rw-r--r--   0 root         (0) root         (0)      834 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3870 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/aes_gcm_aead.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
--rw-r--r--   0 root         (0) root         (0)     1039 2023-07-02 17:34:23.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/random_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/logger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-13 19:20:14.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.734202 onqlave-python-sdk-pilot-0.0.3/onqlave/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:31:41.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-06-26 16:09:49.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/test/hasher_test.py
--rw-r--r--   0 root         (0) root         (0)     3616 2023-07-13 19:20:03.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/test/master_test.py
--rw-r--r--   0 root         (0) root         (0)     3613 2023-07-02 17:49:47.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/test/test_pem_decrypt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.734202 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:03:19.000000 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1830 2023-07-14 02:03:19.000000 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 02:03:19.000000 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-14 02:03:19.000000 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-14 02:03:19.000000 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 02:03:19.734202 onqlave-python-sdk-pilot-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      931 2023-07-14 02:02:43.000000 onqlave-python-sdk-pilot-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.954184 onqlave-python-sdk-pilot-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:09:36.954184 onqlave-python-sdk-pilot-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-02 14:43:10.000000 onqlave-python-sdk-pilot-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.944184 onqlave-python-sdk-pilot-0.0.4/onqlave/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 03:10:41.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.944184 onqlave-python-sdk-pilot-0.0.4/onqlave/connection/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/connection/client.py
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-07-14 01:57:58.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/connection/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.944184 onqlave-python-sdk-pilot-0.0.4/onqlave/contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/contracts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-12 16:35:27.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/contracts/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.944184 onqlave-python-sdk-pilot-0.0.4/onqlave/contracts/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/contracts/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-14 01:58:58.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/contracts/requests/requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.944184 onqlave-python-sdk-pilot-0.0.4/onqlave/contracts/responses/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/contracts/responses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-07-14 01:56:52.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/contracts/responses/responses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.944184 onqlave-python-sdk-pilot-0.0.4/onqlave/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 16:39:18.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/credentials/credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.944184 onqlave-python-sdk-pilot-0.0.4/onqlave/encryption/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:40:25.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/encryption/encrypted_stream_processor.py
+-rw-r--r--   0 root         (0) root         (0)    10873 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/encryption/encryption.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-12 16:42:49.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/encryption/options.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/encryption/plain_stream_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.944184 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/id_service.py
+-rw-r--r--   0 root         (0) root         (0)     7177 2023-07-14 01:58:27.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/key_manager_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.944184 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/keys/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/keys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/keys/aes_gcm.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/keys/xchacha_20_poly_1350.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.944184 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/onqlave_types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/onqlave_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6737 2023-07-11 15:21:03.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/onqlave_types/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.944184 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/operations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 06:40:20.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      720 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/operations/aes_128_gcm_operation.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/operations/aes_256_gcm_operation.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
+-rw-r--r--   0 root         (0) root         (0)      834 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.954184 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/primitives/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3870 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/primitives/aes_gcm_aead.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-07-02 17:34:23.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/random_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.954184 onqlave-python-sdk-pilot-0.0.4/onqlave/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-13 19:20:14.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.954184 onqlave-python-sdk-pilot-0.0.4/onqlave/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:31:41.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-06-26 16:09:49.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/test/hasher_test.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-07-13 19:20:03.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/test/master_test.py
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-07-02 17:49:47.000000 onqlave-python-sdk-pilot-0.0.4/onqlave/test/test_pem_decrypt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:09:36.954184 onqlave-python-sdk-pilot-0.0.4/onqlave_python_sdk_pilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:09:36.000000 onqlave-python-sdk-pilot-0.0.4/onqlave_python_sdk_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-07-14 02:09:36.000000 onqlave-python-sdk-pilot-0.0.4/onqlave_python_sdk_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 02:09:36.000000 onqlave-python-sdk-pilot-0.0.4/onqlave_python_sdk_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-14 02:09:36.000000 onqlave-python-sdk-pilot-0.0.4/onqlave_python_sdk_pilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-14 02:09:36.000000 onqlave-python-sdk-pilot-0.0.4/onqlave_python_sdk_pilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 02:09:36.954184 onqlave-python-sdk-pilot-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      931 2023-07-14 02:09:30.000000 onqlave-python-sdk-pilot-0.0.4/setup.py
```

### Comparing `onqlave-python-sdk-pilot-0.0.3/PKG-INFO` & `onqlave-python-sdk-pilot-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python-sdk-pilot
-Version: 0.0.3
+Version: 0.0.4
 Summary: A SDK to use the encryption service provided by The Onqlave Platform
 Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
 Author: Onqlave Pty
 Author-email: dc@onqlave.com
 Keywords: encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/connection/client.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/connection/client.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/connection/connection.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/connection/connection.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/requests/requests.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/contracts/requests/requests.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/responses/responses.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/contracts/responses/responses.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/credentials/credentials.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/encrypted_stream_processor.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/encryption/encrypted_stream_processor.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/encryption.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/options.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/encryption/options.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/plain_stream_processor.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/encryption/plain_stream_processor.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/id_service.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/id_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/key_manager_client.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/key_manager_client.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/aes_gcm.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/keys/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/xchacha_20_poly_1350.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/keys/xchacha_20_poly_1350.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/onqlave_types/types.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/onqlave_types/types.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/aes_128_gcm_operation.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/operations/aes_128_gcm_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/xchacha20_poly1305_operation.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/operations/xchacha20_poly1305_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/aes_gcm_aead.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/primitives/aes_gcm_aead.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/random_service.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/keymanager/random_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/test/hasher_test.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/test/hasher_test.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/test/master_test.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/test/master_test.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave/test/test_pem_decrypt.py` & `onqlave-python-sdk-pilot-0.0.4/onqlave/test/test_pem_decrypt.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/PKG-INFO` & `onqlave-python-sdk-pilot-0.0.4/onqlave_python_sdk_pilot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python-sdk-pilot
-Version: 0.0.3
+Version: 0.0.4
 Summary: A SDK to use the encryption service provided by The Onqlave Platform
 Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
 Author: Onqlave Pty
 Author-email: dc@onqlave.com
 Keywords: encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/SOURCES.txt` & `onqlave-python-sdk-pilot-0.0.4/onqlave_python_sdk_pilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/requires.txt` & `onqlave-python-sdk-pilot-0.0.4/onqlave_python_sdk_pilot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.3/setup.py` & `onqlave-python-sdk-pilot-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='onqlave-python-sdk-pilot',
-    version='0.0.3',
+    version='0.0.4',
     author='Onqlave Pty',
     author_email='dc@onqlave.com',
     description='A SDK to use the encryption service provided by The Onqlave Platform',
     long_description='',
     long_description_content_type='text/markdown',
     url='https://github.com/onqlavelabs/onqlave-python/tree/dev',  # Replace with your package URL
     packages=find_packages(),
```

