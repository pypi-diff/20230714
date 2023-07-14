# Comparing `tmp/onqlave-python-sdk-pilot-0.0.6.tar.gz` & `tmp/onqlave-python-sdk-pilot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onqlave-python-sdk-pilot-0.0.6.tar", last modified: Fri Jul 14 02:15:39 2023, max compression
+gzip compressed data, was "onqlave-python-sdk-pilot-0.0.7.tar", last modified: Fri Jul 14 02:16:55 2023, max compression
```

## Comparing `onqlave-python-sdk-pilot-0.0.6.tar` & `onqlave-python-sdk-pilot-0.0.7.tar`

### file list

```diff
@@ -1,75 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-02 14:43:10.000000 onqlave-python-sdk-pilot-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.354147 onqlave-python-sdk-pilot-0.0.6/onqlave/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 03:10:41.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.354147 onqlave-python-sdk-pilot-0.0.6/onqlave/connection/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3671 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/connection/client.py
--rw-r--r--   0 root         (0) root         (0)     3654 2023-07-14 01:57:58.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/connection/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.354147 onqlave-python-sdk-pilot-0.0.6/onqlave/contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/contracts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-12 16:35:27.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/contracts/contracts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.354147 onqlave-python-sdk-pilot-0.0.6/onqlave/contracts/requests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/contracts/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-14 01:58:58.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/contracts/requests/requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.354147 onqlave-python-sdk-pilot-0.0.6/onqlave/contracts/responses/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/contracts/responses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-07-14 01:56:52.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/contracts/responses/responses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.354147 onqlave-python-sdk-pilot-0.0.6/onqlave/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/credentials/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 16:39:18.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/credentials/credentials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave/encryption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:40:25.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2525 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/encryption/encrypted_stream_processor.py
--rw-r--r--   0 root         (0) root         (0)    10873 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/encryption/encryption.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-12 16:42:49.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/encryption/options.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/encryption/plain_stream_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave/errors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:13:49.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)      608 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/errors/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)      825 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/id_service.py
--rw-r--r--   0 root         (0) root         (0)     7177 2023-07-14 01:58:27.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/key_manager_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/keys/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/keys/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1187 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/keys/aes_gcm.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/keys/xchacha_20_poly_1350.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/onqlave_types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/onqlave_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6737 2023-07-11 15:21:03.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/onqlave_types/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/operations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 06:40:20.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      720 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/operations/aes_128_gcm_operation.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/operations/aes_256_gcm_operation.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
--rw-r--r--   0 root         (0) root         (0)      834 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/primitives/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3870 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/primitives/aes_gcm_aead.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
--rw-r--r--   0 root         (0) root         (0)     1039 2023-07-02 17:34:23.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/random_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave/logger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-13 19:20:14.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave/messages/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:10:53.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/messages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-07-12 17:40:52.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/messages/messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:31:41.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-06-26 16:09:49.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/test/hasher_test.py
--rw-r--r--   0 root         (0) root         (0)     3616 2023-07-13 19:20:03.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/test/master_test.py
--rw-r--r--   0 root         (0) root         (0)     3613 2023-07-02 17:49:47.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/test/test_pem_decrypt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:10:47.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-07-14 01:56:52.000000 onqlave-python-sdk-pilot-0.0.6/onqlave/utils/hasher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/onqlave_python_sdk_pilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:15:39.000000 onqlave-python-sdk-pilot-0.0.6/onqlave_python_sdk_pilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1990 2023-07-14 02:15:39.000000 onqlave-python-sdk-pilot-0.0.6/onqlave_python_sdk_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 02:15:39.000000 onqlave-python-sdk-pilot-0.0.6/onqlave_python_sdk_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-14 02:15:39.000000 onqlave-python-sdk-pilot-0.0.6/onqlave_python_sdk_pilot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-14 02:15:39.000000 onqlave-python-sdk-pilot-0.0.6/onqlave_python_sdk_pilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 02:15:39.364147 onqlave-python-sdk-pilot-0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      931 2023-07-14 02:15:24.000000 onqlave-python-sdk-pilot-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.184142 onqlave-python-sdk-pilot-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:16:55.184142 onqlave-python-sdk-pilot-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-02 14:43:10.000000 onqlave-python-sdk-pilot-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.164142 onqlave-python-sdk-pilot-0.0.7/onqlave/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 03:10:41.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/connection/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/connection/client.py
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-07-14 01:57:58.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/connection/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-12 16:35:27.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-14 01:58:58.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/requests/requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/responses/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/responses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-07-14 01:56:52.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/responses/responses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 16:39:18.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/credentials/credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:40:25.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/encrypted_stream_processor.py
+-rw-r--r--   0 root         (0) root         (0)    10873 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/encryption.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-12 16:42:49.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/options.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/plain_stream_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/errors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:13:49.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      608 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/errors/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:16:29.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/aes_gcm_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/xchacha20_poly1305_factory.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/id_service.py
+-rw-r--r--   0 root         (0) root         (0)     7177 2023-07-14 01:58:27.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/key_manager_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/aes_gcm.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/xchacha_20_poly_1350.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/onqlave_types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/onqlave_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6737 2023-07-11 15:21:03.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/onqlave_types/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 06:40:20.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      720 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/aes_128_gcm_operation.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/aes_256_gcm_operation.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
+-rw-r--r--   0 root         (0) root         (0)      834 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3870 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/aes_gcm_aead.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-07-02 17:34:23.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/random_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-13 19:20:14.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/messages/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:10:53.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-07-12 17:40:52.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/messages/messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:31:41.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-06-26 16:09:49.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/test/hasher_test.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-07-13 19:20:03.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/test/master_test.py
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-07-02 17:49:47.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/test/test_pem_decrypt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.184142 onqlave-python-sdk-pilot-0.0.7/onqlave/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:10:47.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-07-14 01:56:52.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/utils/hasher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.184142 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:16:55.000000 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-07-14 02:16:55.000000 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 02:16:55.000000 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-14 02:16:55.000000 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-14 02:16:55.000000 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 02:16:55.184142 onqlave-python-sdk-pilot-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      931 2023-07-14 02:16:50.000000 onqlave-python-sdk-pilot-0.0.7/setup.py
```

### Comparing `onqlave-python-sdk-pilot-0.0.6/PKG-INFO` & `onqlave-python-sdk-pilot-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python-sdk-pilot
-Version: 0.0.6
+Version: 0.0.7
 Summary: A SDK to use the encryption service provided by The Onqlave Platform
 Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
 Author: Onqlave Pty
 Author-email: dc@onqlave.com
 Keywords: encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/connection/client.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/connection/client.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/connection/connection.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/connection/connection.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/contracts/requests/requests.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/requests/requests.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/contracts/responses/responses.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/responses/responses.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/credentials/credentials.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/encryption/encrypted_stream_processor.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/encrypted_stream_processor.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/encryption/encryption.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/encryption/options.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/options.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/encryption/plain_stream_processor.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/plain_stream_processor.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/errors/errors.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/errors/errors.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/id_service.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/id_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/key_manager_client.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/key_manager_client.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/keys/aes_gcm.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/keys/xchacha_20_poly_1350.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/xchacha_20_poly_1350.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/onqlave_types/types.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/onqlave_types/types.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/operations/aes_128_gcm_operation.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/aes_128_gcm_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/operations/xchacha20_poly1305_operation.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/xchacha20_poly1305_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/primitives/aes_gcm_aead.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/aes_gcm_aead.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/keymanager/random_service.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/random_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/messages/messages.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/messages/messages.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/test/hasher_test.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/test/hasher_test.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/test/master_test.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/test/master_test.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/test/test_pem_decrypt.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/test/test_pem_decrypt.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave/utils/hasher.py` & `onqlave-python-sdk-pilot-0.0.7/onqlave/utils/hasher.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave_python_sdk_pilot.egg-info/PKG-INFO` & `onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python-sdk-pilot
-Version: 0.0.6
+Version: 0.0.7
 Summary: A SDK to use the encryption service provided by The Onqlave Platform
 Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
 Author: Onqlave Pty
 Author-email: dc@onqlave.com
 Keywords: encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave_python_sdk_pilot.egg-info/SOURCES.txt` & `onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 onqlave/encryption/plain_stream_processor.py
 onqlave/errors/__init__.py
 onqlave/errors/errors.py
 onqlave/keymanager/__init__.py
 onqlave/keymanager/id_service.py
 onqlave/keymanager/key_manager_client.py
 onqlave/keymanager/random_service.py
+onqlave/keymanager/factories/__init__.py
+onqlave/keymanager/factories/aes_gcm_factory.py
+onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py
+onqlave/keymanager/factories/xchacha20_poly1305_factory.py
 onqlave/keymanager/keys/__init__.py
 onqlave/keymanager/keys/aes_gcm.py
 onqlave/keymanager/keys/xchacha_20_poly_1350.py
 onqlave/keymanager/onqlave_types/__init__.py
 onqlave/keymanager/onqlave_types/types.py
 onqlave/keymanager/operations/__init__.py
 onqlave/keymanager/operations/aes_128_gcm_operation.py
```

### Comparing `onqlave-python-sdk-pilot-0.0.6/onqlave_python_sdk_pilot.egg-info/requires.txt` & `onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.6/setup.py` & `onqlave-python-sdk-pilot-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='onqlave-python-sdk-pilot',
-    version='0.0.6',
+    version='0.0.7',
     author='Onqlave Pty',
     author_email='dc@onqlave.com',
     description='A SDK to use the encryption service provided by The Onqlave Platform',
     long_description='',
     long_description_content_type='text/markdown',
     url='https://github.com/onqlavelabs/onqlave-python/tree/dev',  # Replace with your package URL
     packages=find_packages(),
```

