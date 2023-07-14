# Comparing `tmp/onqlave-python-sdk-pilot-0.0.2.tar.gz` & `tmp/onqlave-python-sdk-pilot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onqlave-python-sdk-pilot-0.0.2.tar", last modified: Fri Jul 14 01:38:51 2023, max compression
+gzip compressed data, was "onqlave-python-sdk-pilot-0.0.3.tar", last modified: Fri Jul 14 02:03:19 2023, max compression
```

## Comparing `onqlave-python-sdk-pilot-0.0.2.tar` & `onqlave-python-sdk-pilot-0.0.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-02 14:43:10.000000 onqlave-python-sdk-pilot-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 03:10:41.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/connection/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3647 2023-07-13 20:52:36.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/connection/client.py
--rw-r--r--   0 root         (0) root         (0)     3606 2023-07-12 16:08:18.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/connection/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-12 16:35:27.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/contracts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/requests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      724 2023-07-12 16:34:50.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/requests/requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/responses/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/responses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/responses/responses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/credentials/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 16:39:18.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/credentials/credentials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:40:25.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2517 2023-07-11 14:45:55.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/encrypted_stream_processor.py
--rw-r--r--   0 root         (0) root         (0)    10851 2023-07-14 01:32:47.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/encryption.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-12 16:42:49.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/options.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-07-11 14:48:04.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/plain_stream_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)      809 2023-07-02 17:31:24.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/id_service.py
--rw-r--r--   0 root         (0) root         (0)     7120 2023-07-13 13:08:03.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/key_manager_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1179 2023-07-12 17:37:23.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/aes_gcm.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-07-12 17:36:47.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/xchacha_20_poly_1350.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/onqlave_types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/onqlave_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6737 2023-07-11 15:21:03.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/onqlave_types/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 06:40:20.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-06 10:14:04.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/aes_128_gcm_operation.py
--rw-r--r--   0 root         (0) root         (0)      492 2023-06-19 06:42:16.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/aes_256_gcm_operation.py
--rw-r--r--   0 root         (0) root         (0)      798 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
--rw-r--r--   0 root         (0) root         (0)      818 2023-07-12 17:32:48.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-07-05 15:30:04.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/aes_gcm_aead.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-07-12 15:06:19.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-07-06 16:20:02.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
--rw-r--r--   0 root         (0) root         (0)     1039 2023-07-02 17:34:23.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/random_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/logger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-13 19:20:14.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:31:41.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-06-26 16:09:49.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/test/hasher_test.py
--rw-r--r--   0 root         (0) root         (0)     3616 2023-07-13 19:20:03.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/test/master_test.py
--rw-r--r--   0 root         (0) root         (0)     3613 2023-07-02 17:49:47.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/test/test_pem_decrypt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 01:38:51.000000 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1830 2023-07-14 01:38:51.000000 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 01:38:51.000000 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-14 01:38:51.000000 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-14 01:38:51.000000 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      931 2023-07-14 01:38:35.000000 onqlave-python-sdk-pilot-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.734202 onqlave-python-sdk-pilot-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:03:19.734202 onqlave-python-sdk-pilot-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-02 14:43:10.000000 onqlave-python-sdk-pilot-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 03:10:41.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/connection/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/connection/client.py
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-07-14 01:57:58.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/connection/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-12 16:35:27.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-14 01:58:58.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/requests/requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/responses/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/responses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-07-14 01:56:52.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/responses/responses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 16:39:18.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/credentials/credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:40:25.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/encrypted_stream_processor.py
+-rw-r--r--   0 root         (0) root         (0)    10873 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/encryption.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-12 16:42:49.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/options.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/plain_stream_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/id_service.py
+-rw-r--r--   0 root         (0) root         (0)     7177 2023-07-14 01:58:27.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/key_manager_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/aes_gcm.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/xchacha_20_poly_1350.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/onqlave_types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/onqlave_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6737 2023-07-11 15:21:03.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/onqlave_types/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 06:40:20.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      720 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/aes_128_gcm_operation.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/aes_256_gcm_operation.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
+-rw-r--r--   0 root         (0) root         (0)      834 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3870 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/aes_gcm_aead.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-07-02 17:34:23.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/random_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.724202 onqlave-python-sdk-pilot-0.0.3/onqlave/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-13 19:20:14.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.734202 onqlave-python-sdk-pilot-0.0.3/onqlave/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:31:41.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-06-26 16:09:49.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/test/hasher_test.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-07-13 19:20:03.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/test/master_test.py
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-07-02 17:49:47.000000 onqlave-python-sdk-pilot-0.0.3/onqlave/test/test_pem_decrypt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:03:19.734202 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:03:19.000000 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-07-14 02:03:19.000000 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 02:03:19.000000 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-14 02:03:19.000000 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-14 02:03:19.000000 onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 02:03:19.734202 onqlave-python-sdk-pilot-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      931 2023-07-14 02:02:43.000000 onqlave-python-sdk-pilot-0.0.3/setup.py
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/PKG-INFO` & `onqlave-python-sdk-pilot-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python-sdk-pilot
-Version: 0.0.2
+Version: 0.0.3
 Summary: A SDK to use the encryption service provided by The Onqlave Platform
 Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
 Author: Onqlave Pty
 Author-email: dc@onqlave.com
 Keywords: encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/connection/client.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/connection/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import requests
 import time 
 import urllib.request
 import json
 
 from datetime import datetime
 
-from contracts.requests.requests import OnqlaveRequest
-from logger.logger import OnqlaveLogger
+from onqlave.contracts.requests.requests import OnqlaveRequest
+from onqlave.logger.logger import OnqlaveLogger
 
-from messages import messages
+from onqlave.messages import messages
 class RetrySettings:
     """A class for initializing the retry setting, default value is:
     - count = 3
     - wait_time = 400ms
     - max_wait_time = 2000ms
     """
     def __init__(
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/connection/connection.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/connection/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import calendar
 from datetime import datetime
 
-from credentials.credentials import Credential
-from connection.client import RetrySettings,Client
-from contracts.requests.requests import OnqlaveRequest
-from logger.logger import OnqlaveLogger
-from messages import messages
-from utils.hasher import Hasher
+from onqlave.credentials.credentials import Credential
+from onqlave.connection.client import RetrySettings,Client
+from onqlave.contracts.requests.requests import OnqlaveRequest
+from onqlave.logger.logger import OnqlaveLogger
+from onqlave.messages import messages
+from onqlave.utils.hasher import Hasher
 
 # A list of header constants
 OnqlaveAPIKey         = "ONQLAVE-API-KEY"
 OnqlaveContent        = "Content-Type"
 OnqlaveHost           = "ONQLAVE-HOST"
 OnqlaveVersion        = "ONQLAVE-VERSION"
 OnqlaveSignature      = "ONQLAVE-SIGNATURE"
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/requests/requests.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/requests/requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import json
 
-from requests import Request
-
 class OnqlaveRequest():
     def __init__(self,body_data: dict):
         self._json = body_data
     
     def get_content(self): # return []byte, error
         """convert to JSON encoding"""
         return json.dumps(self._json)
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/responses/responses.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/contracts/responses/responses.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ctypes import c_uint
 
-from contracts.contracts import WrappingKey,EncryptionSecurityModel,DataDecryptionKey,DataEncryptionKey
+from onqlave.contracts.contracts import WrappingKey,EncryptionSecurityModel,DataDecryptionKey,DataEncryptionKey
 
 class BaseErrorResponse:
     def __init__(self) -> None:
         self._error = "error"
 
 class Error:
     def __init__(
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/credentials/credentials.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/encrypted_stream_processor.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/encrypted_stream_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 
-from keymanager.onqlave_types.types import AlgorithmDeserialiser
+from onqlave.keymanager.onqlave_types.types import AlgorithmDeserialiser
 
 class EncryptedStreamProcessor:
     """A stream processor for the encrypted stream in the decryption process
     with two functions including reading the header and reading the packet.    
     """
     def __init__(self, cipher_stream: io.BytesIO) -> None:
         """Init an EncryptedStreamProcessor object which takes the cipher
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/encryption.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/encryption.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import logging
 import io
 from datetime import datetime
-# from logger.logger import OnqlaveLogging
+
 from onqlave.keymanager.random_service import CSPRNG
 from onqlave.keymanager.id_service import IDService
 from onqlave.keymanager.key_manager_client import KeyManager
-from connection.connection import Configuration
-from encryption.options import DebugOption,ArxOption
-from connection.client import RetrySettings
-from credentials.credentials import Credential
+from onqlave.connection.connection import Configuration
+from onqlave.encryption.options import DebugOption,ArxOption
+from onqlave.connection.client import RetrySettings
+from onqlave.credentials.credentials import Credential
 
-from encryption.plain_stream_processor import PlainStreamProcessor
-from encryption.encrypted_stream_processor import EncryptedStreamProcessor
+from onqlave.encryption.plain_stream_processor import PlainStreamProcessor
+from onqlave.encryption.encrypted_stream_processor import EncryptedStreamProcessor
 
-from logger.logger import OnqlaveLogger
+from onqlave.logger.logger import OnqlaveLogger
 
 from onqlave.keymanager.onqlave_types.types import Aesgcm128,Aesgcm256,XChacha20poly1305
 from onqlave.keymanager.onqlave_types.types import AlgorithmSerialiser, AlgorithmDeserialiser
 from onqlave.keymanager.factories.aes_gcm_factory import AEADGCMKeyFactory
 from onqlave.keymanager.factories.xchacha20_poly1305_factory import XChaCha20Poly1305KeyFactory
 from onqlave.keymanager.operations.aes_128_gcm_operation import AesGcmKeyOperation
 from onqlave.keymanager.operations.aes_256_gcm_operation import Aes256GcmKeyOperation
 from onqlave.keymanager.operations.xchacha20_poly1305_operation import XChaCha20Poly1305KeyOperation
 
-from messages import messages
+from onqlave.messages import messages
 
 
 class Encryption:
     """A class that models the encryption services with 2 main groups of features:
     - Encrypt/Decrypt data blocks
     - Encrypt/Decrypt data streams
     Before actually begin the encrypt/decrypt, it requires an inititalisation step for these operations
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/options.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/options.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/plain_stream_processor.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/encryption/plain_stream_processor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 import struct
 
-from keymanager.onqlave_types.types import AlgorithmSerialiser
+from onqlave.keymanager.onqlave_types.types import AlgorithmSerialiser
 class PlainStreamProcessor:
     """A stream processor for the plain stream in the encryption process
     with two function including writing the header and writing the packet.
     """
     def __init__(self,cipher_stream: io.BytesIO) -> None:
         """Init an PlainStreamProcessor object which takes the cipher stream
         in the encryption process as its main attribute
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/id_service.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/id_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ctypes import c_uint32
 
-from keymanager.onqlave_types.types import KeyID
-from keymanager.random_service import CSPRNG
+from onqlave.keymanager.onqlave_types.types import KeyID
+from onqlave.keymanager.random_service import CSPRNG
 class IDService:
     """A class defining the ID generation service
     """
     def __init__(self, random_service: CSPRNG) -> None:
         """Init the ID service by feeding a random service into it
 
         Args:
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/key_manager_client.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/key_manager_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import logging
 import base64
 from datetime import datetime
 
-# from credentials.credentials import Credential
-# from connection.client import RetrySettings
-from utils.hasher import Hasher
-from logger.logger import OnqlaveLogger
-from contracts.requests.requests import EncryptionOpenRequest, DecryptionOpenRequest
-from connection.connection import Connection,Configuration
-from encryption.options import DebugOption
-from keymanager.factories.rsa_ssa_pkcs1_sha_factory import RSASSAPKCS1SHAKeyFactory
-from keymanager.random_service import CSPRNG
-from keymanager.onqlave_types.types import RsaSsapkcs12048sha256f4
-from keymanager.operations.rsa_ssa_pkcs1_sha_operation import RsaSsaPkcs1Sha2562048KeyOperation
-from messages import messages
-from errors.errors import OnqlaveError
+# from onqlave.credentials.credentials import Credential
+# from onqlave.connection.client import RetrySettings
+from onqlave.utils.hasher import Hasher
+from onqlave.logger.logger import OnqlaveLogger
+from onqlave.contracts.requests.requests import EncryptionOpenRequest, DecryptionOpenRequest
+from onqlave.connection.connection import Connection,Configuration
+from onqlave.encryption.options import DebugOption
+from onqlave.keymanager.factories.rsa_ssa_pkcs1_sha_factory import RSASSAPKCS1SHAKeyFactory
+from onqlave.keymanager.random_service import CSPRNG
+from onqlave.keymanager.onqlave_types.types import RsaSsapkcs12048sha256f4
+from onqlave.keymanager.operations.rsa_ssa_pkcs1_sha_operation import RsaSsaPkcs1Sha2562048KeyOperation
+from onqlave.messages import messages
 
 
 ENCRYPT_RESOURCE_URL  = "oe2/keymanager/encrypt"
 DECRYPT_RESOURCE_URL  = "oe2/keymanager/decrypt"
 
 # class Configuration:
 #     def __init__(
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/aes_gcm.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/aes_gcm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from keymanager.onqlave_types.types import Key, KeyOperation, KeyMaterialType, KeyID, KeyData
+from onqlave.keymanager.onqlave_types.types import Key, KeyOperation, KeyMaterialType, KeyID, KeyData
 
 
 class AesGcmKeyData(KeyData):
     """A class defines the blueprint for the AES (GCM mode) key data
     """
     def __init__(
             self,
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/xchacha_20_poly_1350.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/keys/xchacha_20_poly_1350.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from keymanager.onqlave_types.types import KeyMaterialType, KeyID, KeyOperation, Key, KeyData
+from onqlave.keymanager.onqlave_types.types import KeyMaterialType, KeyID, KeyOperation, Key, KeyData
 class XChaCha20Poly1305KeyData(KeyData):
     """A class define the blueprint of XChaCha20Poly1305 key data
     """
     def __init__(
             self,
             value: bytearray,
             key_material_type: KeyMaterialType,
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/onqlave_types/types.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/onqlave_types/types.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/aes_128_gcm_operation.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/aes_128_gcm_operation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ctypes import c_uint32
-from keymanager.onqlave_types.types import KeyFactory,KeyFormat
+from onqlave.keymanager.onqlave_types.types import KeyFactory,KeyFormat
 
 AESGCMKeyVersion = 0
 
 class AesGcmKeyFormat:
     def __init__(self, key_size: c_uint32, version: c_uint32) -> None:
         self._key_size = key_size
         self._key_version = version
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ctypes import c_uint32
-from keymanager.onqlave_types.types import HashType,HashTypeSHA256,KeyOperation, KeyFactory, KeyFormat
+from onqlave.keymanager.onqlave_types.types import HashType,HashTypeSHA256,KeyOperation, KeyFactory, KeyFormat
 class RsaSsaPkcs1KeyFormat(KeyFormat):
     def __init__(self, version: c_uint32, hash: HashType) -> None:
         self._version = version
         self._hash = hash
 
     def get_hash(self):
         return self._hash
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/xchacha20_poly1305_operation.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/operations/xchacha20_poly1305_operation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ctypes import c_uint32
-from keymanager.onqlave_types.types import KeyFactory,KeyFormat, KeyOperation
-# from keymanager.factories.xchacha20_poly1305_factory import XChaCha20Poly1305KeyFactory
+from onqlave.keymanager.onqlave_types.types import KeyFactory,KeyFormat, KeyOperation
+# from onqlave.keymanager.factories.xchacha20_poly1305_factory import XChaCha20Poly1305KeyFactory
 XchaCha20Poly1305KeyVersion = 0
 
 class XChaChaKeyFormat(KeyFormat):
     def __init__(self,key_size: c_uint32, version: c_uint32) -> None:
         self._key_size = key_size
         self._version = version
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/aes_gcm_aead.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/aes_gcm_aead.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import io
 
 from Crypto.Cipher import AES
 
-from keymanager.onqlave_types.types import Key
-from keymanager.random_service import CSPRNG
+from onqlave.keymanager.onqlave_types.types import Key
+from onqlave.keymanager.random_service import CSPRNG
 
 AESGCMIVSize = 12 # aes-gcm init vector size
 AESGCMTagSize = 16 
 AESGCMMaxPlaintextSize = (1 << 36) - 31
 MAX_INT = sys.maxsize
 MaxIntPlainTextSize = MAX_INT - AESGCMIVSize - AESGCMTagSize
 MinNoIVCiphertextSize = AESGCMTagSize
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from Crypto.IO import PEM 
 from Crypto.PublicKey import RSA
 from Crypto.Cipher import PKCS1_OAEP
 
 from cryptography.hazmat.primitives.serialization import load_pem_private_key
 from cryptography.hazmat.primitives.asymmetric import rsa,padding
 from cryptography.hazmat.backends import default_backend
-from keymanager.random_service import CSPRNG
+from onqlave.keymanager.random_service import CSPRNG
 class RSASSAPKCS1SHA:
     def __init__(
         self, 
         hash_function: any,
         hash_id,
         random_service: CSPRNG,
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 from Crypto.Cipher import ChaCha20_Poly1305
-from keymanager.random_service import CSPRNG
-from keymanager.onqlave_types.types import Key, AEAD
+from onqlave.keymanager.random_service import CSPRNG
+from onqlave.keymanager.onqlave_types.types import Key, AEAD
 
 Poly1305TagSize = 16
 MAX_INT = sys.maxsize
 
 
 class XChaCha20Poly1305AEAD(AEAD):
     def __init__(self, key: Key, random_service: CSPRNG) -> None:
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/random_service.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/keymanager/random_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/test/hasher_test.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/test/hasher_test.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/test/master_test.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/test/master_test.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave/test/test_pem_decrypt.py` & `onqlave-python-sdk-pilot-0.0.3/onqlave/test/test_pem_decrypt.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/PKG-INFO` & `onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python-sdk-pilot
-Version: 0.0.2
+Version: 0.0.3
 Summary: A SDK to use the encryption service provided by The Onqlave Platform
 Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
 Author: Onqlave Pty
 Author-email: dc@onqlave.com
 Keywords: encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/SOURCES.txt` & `onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/requires.txt` & `onqlave-python-sdk-pilot-0.0.3/onqlave_python_sdk_pilot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.2/setup.py` & `onqlave-python-sdk-pilot-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='onqlave-python-sdk-pilot',
-    version='0.0.2',
+    version='0.0.3',
     author='Onqlave Pty',
     author_email='dc@onqlave.com',
     description='A SDK to use the encryption service provided by The Onqlave Platform',
     long_description='',
     long_description_content_type='text/markdown',
     url='https://github.com/onqlavelabs/onqlave-python/tree/dev',  # Replace with your package URL
     packages=find_packages(),
```

