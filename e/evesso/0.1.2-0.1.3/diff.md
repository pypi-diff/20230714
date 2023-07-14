# Comparing `tmp/evesso-0.1.2.tar.gz` & `tmp/evesso-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Dev\evesso\dist\tmpq0_70mh2\evesso-0.1.2.tar", last modified: Sun Mar 13 17:37:15 2022, max compression
+gzip compressed data, was "evesso-0.1.3.tar", last modified: Fri Jul 14 18:02:49 2023, max compression
```

## Comparing `evesso-0.1.2.tar` & `evesso-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-03-13 17:37:15.631861 evesso-0.1.2/
--rw-rw-rw-   0        0        0     1084 2022-02-14 18:09:51.000000 evesso-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2388 2022-03-13 17:37:15.631861 evesso-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1923 2022-03-13 16:03:40.000000 evesso-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2022-03-13 17:37:15.599861 evesso-0.1.2/evesso/
--rw-rw-rw-   0        0        0       22 2022-03-13 15:44:25.000000 evesso-0.1.2/evesso/__init__.py
--rw-rw-rw-   0        0        0     4505 2022-03-13 16:03:40.000000 evesso-0.1.2/evesso/authorize.py
--rw-rw-rw-   0        0        0      667 2022-03-13 15:44:25.000000 evesso-0.1.2/evesso/cache.py
-drwxrwxrwx   0        0        0        0 2022-03-13 17:37:15.629859 evesso-0.1.2/evesso/callback/
--rw-rw-rw-   0        0        0       41 2022-03-13 15:44:25.000000 evesso-0.1.2/evesso/callback/__init__.py
--rw-rw-rw-   0        0        0      605 2022-03-13 15:44:25.000000 evesso-0.1.2/evesso/callback/index.html
--rw-rw-rw-   0        0        0     2248 2022-03-13 15:44:25.000000 evesso-0.1.2/evesso/callback/server.py
--rw-rw-rw-   0        0        0      304 2022-03-13 15:44:25.000000 evesso-0.1.2/evesso/const.py
--rw-rw-rw-   0        0        0      978 2022-03-13 15:44:25.000000 evesso-0.1.2/evesso/refresh.py
--rw-rw-rw-   0        0        0     5132 2022-03-13 16:03:40.000000 evesso-0.1.2/evesso/sso.py
-drwxrwxrwx   0        0        0        0 2022-03-13 17:37:15.625862 evesso-0.1.2/evesso.egg-info/
--rw-rw-rw-   0        0        0     2388 2022-03-13 17:37:15.000000 evesso-0.1.2/evesso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2022-03-13 17:37:15.000000 evesso-0.1.2/evesso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-13 17:37:15.000000 evesso-0.1.2/evesso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-03-13 17:37:15.000000 evesso-0.1.2/evesso.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-03-13 17:37:15.000000 evesso-0.1.2/evesso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-02-14 18:13:29.000000 evesso-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      575 2022-03-13 17:37:15.633860 evesso-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 18:02:49.306225 evesso-0.1.3/
+-rw-rw-rw-   0        0        0     1084 2023-04-17 09:07:04.000000 evesso-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2380 2023-07-14 18:02:49.306225 evesso-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1950 2023-07-14 16:14:13.000000 evesso-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 18:02:49.282225 evesso-0.1.3/evesso/
+-rw-rw-rw-   0        0        0       22 2023-04-17 09:07:04.000000 evesso-0.1.3/evesso/__init__.py
+-rw-rw-rw-   0        0        0     4505 2023-04-17 09:07:04.000000 evesso-0.1.3/evesso/authorize.py
+-rw-rw-rw-   0        0        0      667 2023-04-17 09:07:04.000000 evesso-0.1.3/evesso/cache.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:02:49.298225 evesso-0.1.3/evesso/callback/
+-rw-rw-rw-   0        0        0       41 2023-04-17 09:07:04.000000 evesso-0.1.3/evesso/callback/__init__.py
+-rw-rw-rw-   0        0        0      605 2023-07-14 15:59:27.000000 evesso-0.1.3/evesso/callback/index.html
+-rw-rw-rw-   0        0        0     2248 2023-04-17 09:07:04.000000 evesso-0.1.3/evesso/callback/server.py
+-rw-rw-rw-   0        0        0      304 2023-04-17 09:07:04.000000 evesso-0.1.3/evesso/const.py
+-rw-rw-rw-   0        0        0      978 2023-04-17 09:07:04.000000 evesso-0.1.3/evesso/refresh.py
+-rw-rw-rw-   0        0        0     5132 2023-04-17 09:07:04.000000 evesso-0.1.3/evesso/sso.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:02:49.292225 evesso-0.1.3/evesso.egg-info/
+-rw-rw-rw-   0        0        0     2380 2023-07-14 18:02:49.000000 evesso-0.1.3/evesso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-07-14 18:02:49.000000 evesso-0.1.3/evesso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 18:02:49.000000 evesso-0.1.3/evesso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 18:02:49.000000 evesso-0.1.3/evesso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-14 18:02:49.000000 evesso-0.1.3/evesso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-04-17 09:07:04.000000 evesso-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      581 2023-07-14 18:02:49.308225 evesso-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 18:02:49.303225 evesso-0.1.3/tests/
+-rw-rw-rw-   0        0        0     1542 2023-04-17 09:07:04.000000 evesso-0.1.3/tests/test_authorize.py
+-rw-rw-rw-   0        0        0      589 2023-04-17 09:07:04.000000 evesso-0.1.3/tests/test_cache.py
+-rw-rw-rw-   0        0        0     1352 2023-04-17 09:07:04.000000 evesso-0.1.3/tests/test_sso.py
```

### Comparing `evesso-0.1.2/LICENSE` & `evesso-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evesso-0.1.2/PKG-INFO` & `evesso-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: evesso
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python SSO Authorization for Eve Online API applications
-Home-page: https://github.com/mobiusxs/evesso
-Author: MobiusXS
-License: UNKNOWN
-Platform: UNKNOWN
+Home-page: https://github.com/harrelchris/evesso
+Author: harrelchris
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -19,21 +17,21 @@
 
 ## About
 
 This library implements the native SSO authorization flow as described [here](https://docs.esi.evetech.net/docs/sso/native_sso_flow.html). EveSSO will perform the authorization process as needed, store your access and refresh tokens, and refresh your access token as needed. It will then provide the required header for your requests.
 
 ## Installation
 
-```
+```shell
 pip install evesso
 ```
 
 ## Quickstart
 
-```
+```python
 from evesso import SSO
 import requests
 
 sso = SSO(
     client_id='1234567890asdfghjklqwertyuiop',
     callback_url='http://localhost/',
     scope='esi-characters.some_scope.v1 esi-characters.some_scope.v1'
@@ -44,23 +42,23 @@
 )
 response.raise_for_status()
 print(response.json())
 ```
 
 ### Using .env file
 
-```
-CLIENT_ID = 1234567890asdfghjklqwertyuiop
-CALLBACK_URL = http://localhost/
-SCOPE = esi-characters.some_scope.v1 esi-characters.some_scope.v1
+```dotenv
+CLIENT_ID=1234567890asdfghjklqwertyuiop
+CALLBACK_URL=http://localhost/
+SCOPE="esi-characters.some_scope.v1 esi-characters.some_scope.v1"
 ```
 
 Esi will check environment variables for credentials if not parameterized.
 
-```
+```python
 from evesso import SSO
 from dotenv import load_dotenv
 import requests
 
 load_dotenv()
 
 sso = SSO()
@@ -76,14 +74,13 @@
 
 1. Set the `cli` parameter to `True`.
 2. The auth url will be printed to the command line.
 3. Open the auth url in a browser and complete the auth process
 4. The SSO server will make a get request to the machine where you opened the auth url
 5. Copy the callback url and paste it into the command line so evesso can parse it
 
-```
+```python
 from evesso import SSO
 
 sso = SSO(cli=True)
 ...
 ```
-
```

### Comparing `evesso-0.1.2/README.md` & `evesso-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 ## About
 
 This library implements the native SSO authorization flow as described [here](https://docs.esi.evetech.net/docs/sso/native_sso_flow.html). EveSSO will perform the authorization process as needed, store your access and refresh tokens, and refresh your access token as needed. It will then provide the required header for your requests.
 
 ## Installation
 
-```
+```shell
 pip install evesso
 ```
 
 ## Quickstart
 
-```
+```python
 from evesso import SSO
 import requests
 
 sso = SSO(
     client_id='1234567890asdfghjklqwertyuiop',
     callback_url='http://localhost/',
     scope='esi-characters.some_scope.v1 esi-characters.some_scope.v1'
@@ -29,23 +29,23 @@
 )
 response.raise_for_status()
 print(response.json())
 ```
 
 ### Using .env file
 
-```
-CLIENT_ID = 1234567890asdfghjklqwertyuiop
-CALLBACK_URL = http://localhost/
-SCOPE = esi-characters.some_scope.v1 esi-characters.some_scope.v1
+```dotenv
+CLIENT_ID=1234567890asdfghjklqwertyuiop
+CALLBACK_URL=http://localhost/
+SCOPE="esi-characters.some_scope.v1 esi-characters.some_scope.v1"
 ```
 
 Esi will check environment variables for credentials if not parameterized.
 
-```
+```python
 from evesso import SSO
 from dotenv import load_dotenv
 import requests
 
 load_dotenv()
 
 sso = SSO()
@@ -61,13 +61,13 @@
 
 1. Set the `cli` parameter to `True`.
 2. The auth url will be printed to the command line.
 3. Open the auth url in a browser and complete the auth process
 4. The SSO server will make a get request to the machine where you opened the auth url
 5. Copy the callback url and paste it into the command line so evesso can parse it
 
-```
+```python
 from evesso import SSO
 
 sso = SSO(cli=True)
 ...
-```
+```
```

### Comparing `evesso-0.1.2/evesso/authorize.py` & `evesso-0.1.3/evesso/authorize.py`

 * *Files identical despite different names*

### Comparing `evesso-0.1.2/evesso/cache.py` & `evesso-0.1.3/evesso/cache.py`

 * *Files identical despite different names*

### Comparing `evesso-0.1.2/evesso/callback/server.py` & `evesso-0.1.3/evesso/callback/server.py`

 * *Files identical despite different names*

### Comparing `evesso-0.1.2/evesso/refresh.py` & `evesso-0.1.3/evesso/refresh.py`

 * *Files identical despite different names*

### Comparing `evesso-0.1.2/evesso/sso.py` & `evesso-0.1.3/evesso/sso.py`

 * *Files identical despite different names*

### Comparing `evesso-0.1.2/evesso.egg-info/PKG-INFO` & `evesso-0.1.3/evesso.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: evesso
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python SSO Authorization for Eve Online API applications
-Home-page: https://github.com/mobiusxs/evesso
-Author: MobiusXS
-License: UNKNOWN
-Platform: UNKNOWN
+Home-page: https://github.com/harrelchris/evesso
+Author: harrelchris
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -19,21 +17,21 @@
 
 ## About
 
 This library implements the native SSO authorization flow as described [here](https://docs.esi.evetech.net/docs/sso/native_sso_flow.html). EveSSO will perform the authorization process as needed, store your access and refresh tokens, and refresh your access token as needed. It will then provide the required header for your requests.
 
 ## Installation
 
-```
+```shell
 pip install evesso
 ```
 
 ## Quickstart
 
-```
+```python
 from evesso import SSO
 import requests
 
 sso = SSO(
     client_id='1234567890asdfghjklqwertyuiop',
     callback_url='http://localhost/',
     scope='esi-characters.some_scope.v1 esi-characters.some_scope.v1'
@@ -44,23 +42,23 @@
 )
 response.raise_for_status()
 print(response.json())
 ```
 
 ### Using .env file
 
-```
-CLIENT_ID = 1234567890asdfghjklqwertyuiop
-CALLBACK_URL = http://localhost/
-SCOPE = esi-characters.some_scope.v1 esi-characters.some_scope.v1
+```dotenv
+CLIENT_ID=1234567890asdfghjklqwertyuiop
+CALLBACK_URL=http://localhost/
+SCOPE="esi-characters.some_scope.v1 esi-characters.some_scope.v1"
 ```
 
 Esi will check environment variables for credentials if not parameterized.
 
-```
+```python
 from evesso import SSO
 from dotenv import load_dotenv
 import requests
 
 load_dotenv()
 
 sso = SSO()
@@ -76,14 +74,13 @@
 
 1. Set the `cli` parameter to `True`.
 2. The auth url will be printed to the command line.
 3. Open the auth url in a browser and complete the auth process
 4. The SSO server will make a get request to the machine where you opened the auth url
 5. Copy the callback url and paste it into the command line so evesso can parse it
 
-```
+```python
 from evesso import SSO
 
 sso = SSO(cli=True)
 ...
 ```
-
```

### Comparing `evesso-0.1.2/setup.cfg` & `evesso-0.1.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7665 7373 6f0d 0a76 6572 7369   = evesso..versi
-00000020: 6f6e 203d 2030 2e31 2e32 0d0a 6175 7468  on = 0.1.2..auth
-00000030: 6f72 203d 204d 6f62 6975 7358 530d 0a64  or = MobiusXS..d
-00000040: 6573 6372 6970 7469 6f6e 203d 2050 7974  escription = Pyt
-00000050: 686f 6e20 5353 4f20 4175 7468 6f72 697a  hon SSO Authoriz
-00000060: 6174 696f 6e20 666f 7220 4576 6520 4f6e  ation for Eve On
-00000070: 6c69 6e65 2041 5049 2061 7070 6c69 6361  line API applica
-00000080: 7469 6f6e 730d 0a6c 6f6e 675f 6465 7363  tions..long_desc
-00000090: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-000000a0: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
-000000b0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-000000c0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-000000d0: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
-000000e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000000f0: 6f6d 2f6d 6f62 6975 7378 732f 6576 6573  om/mobiusxs/eves
-00000100: 736f 0d0a 636c 6173 7369 6669 6572 7320  so..classifiers 
-00000110: 3d20 0d0a 0950 726f 6772 616d 6d69 6e67  = ...Programming
-00000120: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000130: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
-00000140: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000150: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-00000160: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
-00000170: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00000180: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
-00000190: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
-000001a0: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-000001b0: 7175 6972 6573 203d 203e 3d33 2e36 0d0a  quires = >=3.6..
-000001c0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-000001d0: 203d 200d 0a09 7265 7175 6573 7473 0d0a   = ...requests..
-000001e0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000001f0: 6765 5f64 6174 615d 0d0a 2a20 3d20 6361  ge_data]..* = ca
-00000200: 6c6c 6261 636b 2f69 6e64 6578 2e68 746d  llback/index.htm
-00000210: 6c0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  l....[egg_info].
-00000220: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000230: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000020: 6f6e 203d 2030 2e31 2e33 0d0a 6175 7468  on = 0.1.3..auth
+00000030: 6f72 203d 2068 6172 7265 6c63 6872 6973  or = harrelchris
+00000040: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
+00000050: 5079 7468 6f6e 2053 534f 2041 7574 686f  Python SSO Autho
+00000060: 7269 7a61 7469 6f6e 2066 6f72 2045 7665  rization for Eve
+00000070: 204f 6e6c 696e 6520 4150 4920 6170 706c   Online API appl
+00000080: 6963 6174 696f 6e73 0d0a 6c6f 6e67 5f64  ications..long_d
+00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+000000a0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
+000000b0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+000000c0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+000000d0: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
+000000e0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+000000f0: 622e 636f 6d2f 6861 7272 656c 6368 7269  b.com/harrelchri
+00000100: 732f 6576 6573 736f 0d0a 636c 6173 7369  s/evesso..classi
+00000110: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
+00000120: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000130: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
+00000140: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
+00000150: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000160: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+00000170: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000180: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
+00000190: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
+000001a0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+000001b0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+000001c0: 3d33 2e36 0d0a 696e 7374 616c 6c5f 7265  =3.6..install_re
+000001d0: 7175 6972 6573 203d 200d 0a09 7265 7175  quires = ...requ
+000001e0: 6573 7473 0d0a 0d0a 5b6f 7074 696f 6e73  ests....[options
+000001f0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
+00000200: 2a20 3d20 6361 6c6c 6261 636b 2f69 6e64  * = callback/ind
+00000210: 6578 2e68 746d 6c0d 0a0d 0a5b 6567 675f  ex.html....[egg_
+00000220: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000230: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000240: 300d 0a0d 0a                             0....
```

