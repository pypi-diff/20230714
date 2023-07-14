# Comparing `tmp/symbol-lightapi-0.0.3.tar.gz` & `tmp/symbol-lightapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol-lightapi-0.0.3.tar", last modified: Fri Jul 14 15:05:34 2023, max compression
+gzip compressed data, was "symbol-lightapi-0.0.4.tar", last modified: Fri Jul 14 15:47:35 2023, max compression
```

## Comparing `symbol-lightapi-0.0.3.tar` & `symbol-lightapi-0.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/
--rw-rw-r--   0 wayon     (1000) wayon     (1000)      559 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/PKG-INFO
--rw-rw-r--   0 wayon     (1000) wayon     (1000)      192 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/README.md
-drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/cffi_src/
--rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/cffi_src/__init__.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     4151 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/cffi_src/openssl_build.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)      116 2023-07-14 13:36:29.000000 symbol-lightapi-0.0.3/pyproject.toml
--rw-rw-r--   0 wayon     (1000) wayon     (1000)      516 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/setup.cfg
--rw-rw-r--   0 wayon     (1000) wayon     (1000)      754 2023-07-14 13:36:29.000000 symbol-lightapi-0.0.3/setup.py
-drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/symbol_lightapi.egg-info/
--rw-rw-r--   0 wayon     (1000) wayon     (1000)      559 2023-07-14 15:05:34.000000 symbol-lightapi-0.0.3/symbol_lightapi.egg-info/PKG-INFO
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     1341 2023-07-14 15:05:34.000000 symbol-lightapi-0.0.3/symbol_lightapi.egg-info/SOURCES.txt
--rw-rw-r--   0 wayon     (1000) wayon     (1000)        1 2023-07-14 15:05:34.000000 symbol-lightapi-0.0.3/symbol_lightapi.egg-info/dependency_links.txt
--rw-rw-r--   0 wayon     (1000) wayon     (1000)        1 2023-07-14 15:05:34.000000 symbol-lightapi-0.0.3/symbol_lightapi.egg-info/not-zip-safe
--rw-rw-r--   0 wayon     (1000) wayon     (1000)       46 2023-07-14 15:05:34.000000 symbol-lightapi-0.0.3/symbol_lightapi.egg-info/top_level.txt
-drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/symbollightapi/
--rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/__init__.py
-drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/symbollightapi/bindings/
--rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/bindings/__init__.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)      241 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/bindings/openssl.py
-drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/symbollightapi/connector/
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     1913 2023-07-12 01:51:37.000000 symbol-lightapi-0.0.3/symbollightapi/connector/BasicConnector.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     2413 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/connector/CatapultCertificateProcessor.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     2026 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/connector/CertificateUtils.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     2883 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/connector/NemConnector.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     6169 2023-07-12 01:51:37.000000 symbol-lightapi-0.0.3/symbollightapi/connector/SymbolConnector.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     5770 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/connector/SymbolPeerConnector.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/connector/__init__.py
-drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/symbollightapi/model/
--rw-rw-r--   0 wayon     (1000) wayon     (1000)      563 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/model/Endpoint.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)      218 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/model/Exceptions.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     2036 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/model/NodeInfo.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     1556 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/model/PacketHeader.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/symbollightapi/model/__init__.py
-drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/tests/
--rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/__init__.py
-drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/tests/connector/
--rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/connector/__init__.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     7734 2023-07-12 01:51:37.000000 symbol-lightapi-0.0.3/tests/connector/test_BasicConnector.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)    10465 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/connector/test_CatapultCertificateProcessor.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     5723 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/connector/test_CertificateUtils.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)    10527 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/connector/test_NemConnector.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)    18413 2023-07-12 01:51:37.000000 symbol-lightapi-0.0.3/tests/connector/test_SymbolConnector.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     9201 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/connector/test_SymbolPeerConnector.py
-drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/tests/model/
--rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/model/__init__.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     1607 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/model/test_Endpoint.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     5953 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/model/test_NodeInfo.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     1199 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/model/test_PacketHeader.py
-drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:05:34.216488 symbol-lightapi-0.0.3/tests/test/
--rw-rw-r--   0 wayon     (1000) wayon     (1000)     3956 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/test/CertificateTestUtils.py
--rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.3/tests/test/__init__.py
+drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:47:35.005674 symbol-lightapi-0.0.4/
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)      559 2023-07-14 15:47:35.005674 symbol-lightapi-0.0.4/PKG-INFO
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)      192 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/README.md
+drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:47:35.001675 symbol-lightapi-0.0.4/cffi_src/
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/cffi_src/__init__.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     4151 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/cffi_src/openssl_build.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)      116 2023-07-14 13:36:29.000000 symbol-lightapi-0.0.4/pyproject.toml
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)      516 2023-07-14 15:47:35.005674 symbol-lightapi-0.0.4/setup.cfg
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)      746 2023-07-14 15:44:30.000000 symbol-lightapi-0.0.4/setup.py
+drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:47:35.001675 symbol-lightapi-0.0.4/symbol_lightapi.egg-info/
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)      559 2023-07-14 15:47:34.000000 symbol-lightapi-0.0.4/symbol_lightapi.egg-info/PKG-INFO
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     1341 2023-07-14 15:47:35.000000 symbol-lightapi-0.0.4/symbol_lightapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)        1 2023-07-14 15:47:34.000000 symbol-lightapi-0.0.4/symbol_lightapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)        1 2023-07-14 15:47:34.000000 symbol-lightapi-0.0.4/symbol_lightapi.egg-info/not-zip-safe
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)       46 2023-07-14 15:47:34.000000 symbol-lightapi-0.0.4/symbol_lightapi.egg-info/top_level.txt
+drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:47:35.001675 symbol-lightapi-0.0.4/symbollightapi/
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/__init__.py
+drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:47:35.001675 symbol-lightapi-0.0.4/symbollightapi/bindings/
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/bindings/__init__.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)      241 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/bindings/openssl.py
+drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:47:35.005674 symbol-lightapi-0.0.4/symbollightapi/connector/
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     1913 2023-07-12 01:51:37.000000 symbol-lightapi-0.0.4/symbollightapi/connector/BasicConnector.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     2413 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/connector/CatapultCertificateProcessor.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     2026 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/connector/CertificateUtils.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     2883 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/connector/NemConnector.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     6169 2023-07-12 01:51:37.000000 symbol-lightapi-0.0.4/symbollightapi/connector/SymbolConnector.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     5770 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/connector/SymbolPeerConnector.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/connector/__init__.py
+drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:47:35.005674 symbol-lightapi-0.0.4/symbollightapi/model/
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)      563 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/model/Endpoint.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)      218 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/model/Exceptions.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     2036 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/model/NodeInfo.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     1556 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/model/PacketHeader.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/symbollightapi/model/__init__.py
+drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:47:35.005674 symbol-lightapi-0.0.4/tests/
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/__init__.py
+drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:47:35.005674 symbol-lightapi-0.0.4/tests/connector/
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/connector/__init__.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     7734 2023-07-12 01:51:37.000000 symbol-lightapi-0.0.4/tests/connector/test_BasicConnector.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)    10465 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/connector/test_CatapultCertificateProcessor.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     5723 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/connector/test_CertificateUtils.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)    10527 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/connector/test_NemConnector.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)    18413 2023-07-12 01:51:37.000000 symbol-lightapi-0.0.4/tests/connector/test_SymbolConnector.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     9201 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/connector/test_SymbolPeerConnector.py
+drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:47:35.005674 symbol-lightapi-0.0.4/tests/model/
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/model/__init__.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     1607 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/model/test_Endpoint.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     5953 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/model/test_NodeInfo.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     1199 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/model/test_PacketHeader.py
+drwxrwxr-x   0 wayon     (1000) wayon     (1000)        0 2023-07-14 15:47:35.005674 symbol-lightapi-0.0.4/tests/test/
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)     3956 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/test/CertificateTestUtils.py
+-rw-rw-r--   0 wayon     (1000) wayon     (1000)        0 2023-06-15 01:55:07.000000 symbol-lightapi-0.0.4/tests/test/__init__.py
```

### Comparing `symbol-lightapi-0.0.3/PKG-INFO` & `symbol-lightapi-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbol-lightapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Symbol Light API
 Home-page: https://github.com/symbol/product/tree/main/python/lightapi
 Author: Symbol Contributors
 Author-email: contributors@symbol.dev
 License: MIT
 Keywords: symbol,symbollightapi,lightapi,Symbol Light API
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `symbol-lightapi-0.0.3/cffi_src/openssl_build.py` & `symbol-lightapi-0.0.4/cffi_src/openssl_build.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/setup.cfg` & `symbol-lightapi-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = symbol-lightapi
-version = 0.0.3
+version = 0.0.4
 author = Symbol Contributors
 author_email = contributors@symbol.dev
 description = Symbol Light API
 long_description = file: README.md
 keywords = symbol, symbollightapi, lightapi, Symbol Light API
 license = MIT
 classifiers =
```

### Comparing `symbol-lightapi-0.0.3/setup.py` & `symbol-lightapi-0.0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,10 +25,10 @@
 
 if '__main__' == __name__:
 	setup(
 		# Ensure limited API is set on CPython
 		cmdclass=cmdclass,
 		# CFFI
 		zip_safe=False,
-		ext_package='_lightapi_openssl_cffi_bindings',
+		ext_package='symbollightapi/bindings',
 		cffi_modules=['cffi_src/openssl_build.py:ffi_builder'],
 	)
```

### Comparing `symbol-lightapi-0.0.3/symbol_lightapi.egg-info/PKG-INFO` & `symbol-lightapi-0.0.4/symbol_lightapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbol-lightapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Symbol Light API
 Home-page: https://github.com/symbol/product/tree/main/python/lightapi
 Author: Symbol Contributors
 Author-email: contributors@symbol.dev
 License: MIT
 Keywords: symbol,symbollightapi,lightapi,Symbol Light API
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `symbol-lightapi-0.0.3/symbol_lightapi.egg-info/SOURCES.txt` & `symbol-lightapi-0.0.4/symbol_lightapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/symbollightapi/connector/BasicConnector.py` & `symbol-lightapi-0.0.4/symbollightapi/connector/BasicConnector.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/symbollightapi/connector/CatapultCertificateProcessor.py` & `symbol-lightapi-0.0.4/symbollightapi/connector/CatapultCertificateProcessor.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/symbollightapi/connector/CertificateUtils.py` & `symbol-lightapi-0.0.4/symbollightapi/connector/CertificateUtils.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/symbollightapi/connector/NemConnector.py` & `symbol-lightapi-0.0.4/symbollightapi/connector/NemConnector.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/symbollightapi/connector/SymbolConnector.py` & `symbol-lightapi-0.0.4/symbollightapi/connector/SymbolConnector.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/symbollightapi/connector/SymbolPeerConnector.py` & `symbol-lightapi-0.0.4/symbollightapi/connector/SymbolPeerConnector.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/symbollightapi/model/Endpoint.py` & `symbol-lightapi-0.0.4/symbollightapi/model/Endpoint.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/symbollightapi/model/NodeInfo.py` & `symbol-lightapi-0.0.4/symbollightapi/model/NodeInfo.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/symbollightapi/model/PacketHeader.py` & `symbol-lightapi-0.0.4/symbollightapi/model/PacketHeader.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/tests/connector/test_BasicConnector.py` & `symbol-lightapi-0.0.4/tests/connector/test_BasicConnector.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/tests/connector/test_CatapultCertificateProcessor.py` & `symbol-lightapi-0.0.4/tests/connector/test_CatapultCertificateProcessor.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/tests/connector/test_CertificateUtils.py` & `symbol-lightapi-0.0.4/tests/connector/test_CertificateUtils.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/tests/connector/test_NemConnector.py` & `symbol-lightapi-0.0.4/tests/connector/test_NemConnector.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/tests/connector/test_SymbolConnector.py` & `symbol-lightapi-0.0.4/tests/connector/test_SymbolConnector.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/tests/connector/test_SymbolPeerConnector.py` & `symbol-lightapi-0.0.4/tests/connector/test_SymbolPeerConnector.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/tests/model/test_Endpoint.py` & `symbol-lightapi-0.0.4/tests/model/test_Endpoint.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/tests/model/test_NodeInfo.py` & `symbol-lightapi-0.0.4/tests/model/test_NodeInfo.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/tests/model/test_PacketHeader.py` & `symbol-lightapi-0.0.4/tests/model/test_PacketHeader.py`

 * *Files identical despite different names*

### Comparing `symbol-lightapi-0.0.3/tests/test/CertificateTestUtils.py` & `symbol-lightapi-0.0.4/tests/test/CertificateTestUtils.py`

 * *Files identical despite different names*

