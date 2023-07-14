# Comparing `tmp/vap-1.0.1.tar.gz` & `tmp/vap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vap-1.0.1.tar", last modified: Tue Jun  6 14:24:26 2023, max compression
+gzip compressed data, was "vap-1.1.0.tar", last modified: Fri Jul 14 06:13:27 2023, max compression
```

## Comparing `vap-1.0.1.tar` & `vap-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:24:26.608179 vap-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 14:24:15.000000 vap-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-06 14:24:26.608179 vap-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-06 14:24:15.000000 vap-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:24:26.608179 vap-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-06 14:24:15.000000 vap-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:24:26.604179 vap-1.0.1/vap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:24:15.000000 vap-1.0.1/vap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-06 14:24:15.000000 vap-1.0.1/vap/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 14:24:15.000000 vap-1.0.1/vap/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-06 14:24:15.000000 vap-1.0.1/vap/verifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:24:26.608179 vap-1.0.1/vap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 14:24:26.000000 vap-1.0.1/vap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:13:27.924090 vap-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 06:13:19.000000 vap-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-14 06:13:27.924090 vap-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-14 06:13:19.000000 vap-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:13:27.924090 vap-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-14 06:13:19.000000 vap-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:13:27.924090 vap-1.1.0/vap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:13:19.000000 vap-1.1.0/vap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-14 06:13:19.000000 vap-1.1.0/vap/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-14 06:13:19.000000 vap-1.1.0/vap/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-14 06:13:19.000000 vap-1.1.0/vap/verifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:13:27.924090 vap-1.1.0/vap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-14 06:13:27.000000 vap-1.1.0/vap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-14 06:13:27.000000 vap-1.1.0/vap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:13:27.000000 vap-1.1.0/vap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-14 06:13:27.000000 vap-1.1.0/vap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 06:13:27.000000 vap-1.1.0/vap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-14 06:13:27.000000 vap-1.1.0/vap.egg-info/top_level.txt
```

### Comparing `vap-1.0.1/LICENSE` & `vap-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vap-1.0.1/PKG-INFO` & `vap-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vap
-Version: 1.0.1
+Version: 1.1.0
 Summary: Apple postback verifier
 Home-page: https://github.com/d-ganchar/vas
 Author: Danila Ganchar
 Author-email: danila.ganchar@gmail.com
 License: MIT
 Keywords: verify apple signature postback
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vap-1.0.1/setup.py` & `vap-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 .. _readme: https://github.com/d-ganchar/vap
 """
 
 
 setup(
     name='vap',
-    version='1.0.1',
+    version='1.1.0',
     description='Apple postback verifier',
     long_description=long_description,
     url='https://github.com/d-ganchar/vas',
     author='Danila Ganchar',
     author_email='danila.ganchar@gmail.com',
     license='MIT',
     keywords='verify apple signature postback',
```

### Comparing `vap-1.0.1/vap/cli.py` & `vap-1.1.0/vap/cli.py`

 * *Files identical despite different names*

### Comparing `vap-1.0.1/vap/verifier.py` & `vap-1.1.0/vap/verifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,48 +110,50 @@
 
 _ecdsa_wrapper = _EcdsaWrapper(_APPLE_PUB_KEY)
 
 
 def verify_postback(postback: dict) -> bool:
     version = postback['version']
     float_version = float(version)
-    if float_version < 2.1:
+    if float_version < 2.1 or float_version >= 5:
         return False
 
-    did_win = str(postback['did-win']).lower() if postback.get('did-win') is not None else ''
-    campaign_id = str(postback['campaign-id']) if postback.get('campaign-id') is not None else ''
-    fidelity_type = str(postback['fidelity-type']) if postback.get('fidelity-type') is not None else ''
-    source_identifier = postback['source-identifier'] if postback.get('source-identifier') is not None else ''
-    source_app_id = str(postback['source-app-id']) if postback.get('source-app-id') is not None else ''
-    re_download = str(postback['redownload']).lower()
+    campaign_id = str(postback.get('campaign-id'))
     app_id = str(postback['app-id'])
+    redownload = str(postback.get('redownload')).lower()
     ad_network_id = postback['ad-network-id']
     transaction_id = postback['transaction-id']
-    message_items = []
-
-    if float_version >= 4:
-        if postback.get('postback-sequence-index') is None:
-            return False
+    source_identifier = postback.get('source-identifier') or ''
+    fidelity_type = str(postback.get('fidelity-type'))
+    did_win = str(postback.get('did-win')).lower()
+    source_domain = postback.get('source-domain') or ''
+    postback_sequence_index = str(postback.get('postback-sequence-index'))
+    source_app_id = postback.get('source-app-id')
+
+    if source_app_id is not None:
+        if float_version < 3:
+            source_app_id = str(source_app_id) if isinstance(source_app_id, int) else ''
+        else:
+            source_app_id = str(postback['source-app-id']) if postback['source-app-id'] > 0 else ''
 
-        seq_index = str(postback['postback-sequence-index'])
-        source_domain = postback.get('source-domain')
+    if 4 <= float_version < 5:
         if source_app_id:
-            message_items = [version, ad_network_id, source_identifier, app_id, transaction_id, re_download,
-                             source_app_id, fidelity_type, did_win, seq_index]
+            message_items = [version, ad_network_id, source_identifier, app_id, transaction_id, redownload,
+                             source_app_id, fidelity_type, did_win, postback_sequence_index]
         elif source_domain:
-            message_items = [version, ad_network_id, source_identifier, app_id, transaction_id, re_download,
-                             str(source_domain), fidelity_type, did_win, seq_index]
-    elif float_version >= 3:
+            message_items = [version, ad_network_id, source_identifier, app_id, transaction_id, redownload,
+                             source_domain, fidelity_type, did_win, postback_sequence_index]
+        else:
+            message_items = [version, ad_network_id, source_identifier, app_id, transaction_id, redownload,
+                             fidelity_type, did_win, postback_sequence_index]
+    elif 3 <= float_version < 4:
         if source_app_id:
-            message_items = [version, ad_network_id, campaign_id, app_id, transaction_id, re_download, source_app_id,
+            message_items = [version, ad_network_id, campaign_id, app_id, transaction_id, redownload, source_app_id,
                              fidelity_type, did_win]
         else:
-            message_items = [version, ad_network_id, campaign_id, app_id, transaction_id, re_download, fidelity_type,
+            message_items = [version, ad_network_id, campaign_id, app_id, transaction_id, redownload, fidelity_type,
                              did_win]
     else:
-        message_items = [version, ad_network_id, campaign_id, app_id, transaction_id, re_download, source_app_id]
-
-    if not message_items:
-        return False
+        message_items = [version, ad_network_id, campaign_id, app_id, transaction_id, redownload, source_app_id]
 
     message = u'\u2063'.join(message_items)
     return _ecdsa_wrapper.verify(message, postback['attribution-signature'])
```

### Comparing `vap-1.0.1/vap.egg-info/PKG-INFO` & `vap-1.1.0/vap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vap
-Version: 1.0.1
+Version: 1.1.0
 Summary: Apple postback verifier
 Home-page: https://github.com/d-ganchar/vas
 Author: Danila Ganchar
 Author-email: danila.ganchar@gmail.com
 License: MIT
 Keywords: verify apple signature postback
 Classifier: Development Status :: 5 - Production/Stable
```

