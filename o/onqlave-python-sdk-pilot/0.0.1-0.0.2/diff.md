# Comparing `tmp/onqlave-python-sdk-pilot-0.0.1.tar.gz` & `tmp/onqlave-python-sdk-pilot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onqlave-python-sdk-pilot-0.0.1.tar", last modified: Fri Jul 14 01:28:17 2023, max compression
+gzip compressed data, was "onqlave-python-sdk-pilot-0.0.2.tar", last modified: Fri Jul 14 01:38:51 2023, max compression
```

## Comparing `onqlave-python-sdk-pilot-0.0.1.tar` & `onqlave-python-sdk-pilot-0.0.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-02 14:43:10.000000 onqlave-python-sdk-pilot-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.714365 onqlave-python-sdk-pilot-0.0.1/onqlave/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 03:10:41.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/connection/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3647 2023-07-13 20:52:36.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/connection/client.py
--rw-r--r--   0 root         (0) root         (0)     3606 2023-07-12 16:08:18.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/connection/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/contracts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-12 16:35:27.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/contracts/contracts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/contracts/requests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/contracts/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      724 2023-07-12 16:34:50.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/contracts/requests/requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/contracts/responses/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/contracts/responses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/contracts/responses/responses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/credentials/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 16:39:18.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/credentials/credentials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/encryption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:40:25.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2517 2023-07-11 14:45:55.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/encryption/encrypted_stream_processor.py
--rw-r--r--   0 root         (0) root         (0)    10771 2023-07-12 16:17:53.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/encryption/encryption.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-12 16:42:49.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/encryption/options.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-07-11 14:48:04.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/encryption/plain_stream_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)      809 2023-07-02 17:31:24.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/id_service.py
--rw-r--r--   0 root         (0) root         (0)     7120 2023-07-13 13:08:03.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/key_manager_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/keys/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/keys/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1179 2023-07-12 17:37:23.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/keys/aes_gcm.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-07-12 17:36:47.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/keys/xchacha_20_poly_1350.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/onqlave_types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/onqlave_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6737 2023-07-11 15:21:03.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/onqlave_types/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/operations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 06:40:20.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-06 10:14:04.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/operations/aes_128_gcm_operation.py
--rw-r--r--   0 root         (0) root         (0)      492 2023-06-19 06:42:16.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/operations/aes_256_gcm_operation.py
--rw-r--r--   0 root         (0) root         (0)      798 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
--rw-r--r--   0 root         (0) root         (0)      818 2023-07-12 17:32:48.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/primitives/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-07-05 15:30:04.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/primitives/aes_gcm_aead.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-07-12 15:06:19.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-07-06 16:20:02.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
--rw-r--r--   0 root         (0) root         (0)     1039 2023-07-02 17:34:23.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/random_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/logger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-13 19:20:14.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:31:41.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-06-26 16:09:49.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/test/hasher_test.py
--rw-r--r--   0 root         (0) root         (0)     3616 2023-07-13 19:20:03.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/test/master_test.py
--rw-r--r--   0 root         (0) root         (0)     3613 2023-07-02 17:49:47.000000 onqlave-python-sdk-pilot-0.0.1/onqlave/test/test_pem_decrypt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/onqlave_python_sdk_pilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 01:28:17.000000 onqlave-python-sdk-pilot-0.0.1/onqlave_python_sdk_pilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1830 2023-07-14 01:28:17.000000 onqlave-python-sdk-pilot-0.0.1/onqlave_python_sdk_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 01:28:17.000000 onqlave-python-sdk-pilot-0.0.1/onqlave_python_sdk_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-14 01:28:17.000000 onqlave-python-sdk-pilot-0.0.1/onqlave_python_sdk_pilot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-14 01:28:17.000000 onqlave-python-sdk-pilot-0.0.1/onqlave_python_sdk_pilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 01:28:17.724365 onqlave-python-sdk-pilot-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      931 2023-07-14 01:24:28.000000 onqlave-python-sdk-pilot-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-02 14:43:10.000000 onqlave-python-sdk-pilot-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 03:10:41.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/connection/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2023-07-13 20:52:36.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/connection/client.py
+-rw-r--r--   0 root         (0) root         (0)     3606 2023-07-12 16:08:18.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/connection/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-12 16:35:27.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      724 2023-07-12 16:34:50.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/requests/requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/responses/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/responses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/responses/responses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 16:39:18.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/credentials/credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:40:25.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2023-07-11 14:45:55.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/encrypted_stream_processor.py
+-rw-r--r--   0 root         (0) root         (0)    10851 2023-07-14 01:32:47.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/encryption.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-12 16:42:49.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/options.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-07-11 14:48:04.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/plain_stream_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      809 2023-07-02 17:31:24.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/id_service.py
+-rw-r--r--   0 root         (0) root         (0)     7120 2023-07-13 13:08:03.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/key_manager_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2023-07-12 17:37:23.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/aes_gcm.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-07-12 17:36:47.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/xchacha_20_poly_1350.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/onqlave_types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/onqlave_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6737 2023-07-11 15:21:03.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/onqlave_types/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 06:40:20.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-06 10:14:04.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/aes_128_gcm_operation.py
+-rw-r--r--   0 root         (0) root         (0)      492 2023-06-19 06:42:16.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/aes_256_gcm_operation.py
+-rw-r--r--   0 root         (0) root         (0)      798 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-12 17:32:48.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-07-05 15:30:04.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/aes_gcm_aead.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-07-12 15:06:19.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-06 16:20:02.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-07-02 17:34:23.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/random_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-13 19:20:14.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:31:41.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-06-26 16:09:49.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/test/hasher_test.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-07-13 19:20:03.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/test/master_test.py
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-07-02 17:49:47.000000 onqlave-python-sdk-pilot-0.0.2/onqlave/test/test_pem_decrypt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 01:38:51.000000 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-07-14 01:38:51.000000 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 01:38:51.000000 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-14 01:38:51.000000 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-14 01:38:51.000000 onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 01:38:51.234320 onqlave-python-sdk-pilot-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      931 2023-07-14 01:38:35.000000 onqlave-python-sdk-pilot-0.0.2/setup.py
```

### Comparing `onqlave-python-sdk-pilot-0.0.1/PKG-INFO` & `onqlave-python-sdk-pilot-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python-sdk-pilot
-Version: 0.0.1
+Version: 0.0.2
 Summary: A SDK to use the encryption service provided by The Onqlave Platform
 Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
 Author: Onqlave Pty
 Author-email: dc@onqlave.com
 Keywords: encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/connection/client.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/connection/client.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/connection/connection.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/connection/connection.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/contracts/requests/requests.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/requests/requests.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/contracts/responses/responses.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/contracts/responses/responses.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/credentials/credentials.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/encryption/encrypted_stream_processor.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/encrypted_stream_processor.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/encryption/encryption.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/encryption.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import logging
 import io
 from datetime import datetime
 # from logger.logger import OnqlaveLogging
-from keymanager.random_service import CSPRNG
-from keymanager.id_service import IDService
-from keymanager.key_manager_client import KeyManager
+from onqlave.keymanager.random_service import CSPRNG
+from onqlave.keymanager.id_service import IDService
+from onqlave.keymanager.key_manager_client import KeyManager
 from connection.connection import Configuration
 from encryption.options import DebugOption,ArxOption
 from connection.client import RetrySettings
 from credentials.credentials import Credential
 
 from encryption.plain_stream_processor import PlainStreamProcessor
 from encryption.encrypted_stream_processor import EncryptedStreamProcessor
 
 from logger.logger import OnqlaveLogger
 
-from keymanager.onqlave_types.types import Aesgcm128,Aesgcm256,XChacha20poly1305
-from keymanager.onqlave_types.types import AlgorithmSerialiser, AlgorithmDeserialiser
-from keymanager.factories.aes_gcm_factory import AEADGCMKeyFactory
-from keymanager.factories.xchacha20_poly1305_factory import XChaCha20Poly1305KeyFactory
-from keymanager.operations.aes_128_gcm_operation import AesGcmKeyOperation
-from keymanager.operations.aes_256_gcm_operation import Aes256GcmKeyOperation
-from keymanager.operations.xchacha20_poly1305_operation import XChaCha20Poly1305KeyOperation
+from onqlave.keymanager.onqlave_types.types import Aesgcm128,Aesgcm256,XChacha20poly1305
+from onqlave.keymanager.onqlave_types.types import AlgorithmSerialiser, AlgorithmDeserialiser
+from onqlave.keymanager.factories.aes_gcm_factory import AEADGCMKeyFactory
+from onqlave.keymanager.factories.xchacha20_poly1305_factory import XChaCha20Poly1305KeyFactory
+from onqlave.keymanager.operations.aes_128_gcm_operation import AesGcmKeyOperation
+from onqlave.keymanager.operations.aes_256_gcm_operation import Aes256GcmKeyOperation
+from onqlave.keymanager.operations.xchacha20_poly1305_operation import XChaCha20Poly1305KeyOperation
 
 from messages import messages
 
 
 class Encryption:
     """A class that models the encryption services with 2 main groups of features:
     - Encrypt/Decrypt data blocks
```

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/encryption/options.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/options.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/encryption/plain_stream_processor.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/encryption/plain_stream_processor.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/id_service.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/id_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/key_manager_client.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/key_manager_client.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/keys/aes_gcm.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/keys/xchacha_20_poly_1350.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/keys/xchacha_20_poly_1350.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/onqlave_types/types.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/onqlave_types/types.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/operations/aes_128_gcm_operation.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/aes_128_gcm_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/operations/xchacha20_poly1305_operation.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/operations/xchacha20_poly1305_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/primitives/aes_gcm_aead.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/aes_gcm_aead.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/keymanager/random_service.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/keymanager/random_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/test/hasher_test.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/test/hasher_test.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/test/master_test.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/test/master_test.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave/test/test_pem_decrypt.py` & `onqlave-python-sdk-pilot-0.0.2/onqlave/test/test_pem_decrypt.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave_python_sdk_pilot.egg-info/PKG-INFO` & `onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python-sdk-pilot
-Version: 0.0.1
+Version: 0.0.2
 Summary: A SDK to use the encryption service provided by The Onqlave Platform
 Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
 Author: Onqlave Pty
 Author-email: dc@onqlave.com
 Keywords: encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave_python_sdk_pilot.egg-info/SOURCES.txt` & `onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/onqlave_python_sdk_pilot.egg-info/requires.txt` & `onqlave-python-sdk-pilot-0.0.2/onqlave_python_sdk_pilot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.1/setup.py` & `onqlave-python-sdk-pilot-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='onqlave-python-sdk-pilot',
-    version='0.0.1',
+    version='0.0.2',
     author='Onqlave Pty',
     author_email='dc@onqlave.com',
     description='A SDK to use the encryption service provided by The Onqlave Platform',
     long_description='',
     long_description_content_type='text/markdown',
     url='https://github.com/onqlavelabs/onqlave-python/tree/dev',  # Replace with your package URL
     packages=find_packages(),
```

