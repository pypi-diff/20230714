# Comparing `tmp/bittensor-wallet-0.0.4.tar.gz` & `tmp/bittensor-wallet-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-wallet-0.0.4.tar", last modified: Thu Jul 13 20:19:06 2023, max compression
+gzip compressed data, was "bittensor-wallet-0.0.5.tar", last modified: Fri Jul 14 21:02:23 2023, max compression
```

## Comparing `bittensor-wallet-0.0.4.tar` & `bittensor-wallet-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.834747 bittensor-wallet-0.0.4/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1085 2023-06-27 17:13:40.000000 bittensor-wallet-0.0.4/LICENSE
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-07-13 20:19:06.834590 bittensor-wallet-0.0.4/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      711 2023-07-11 22:18:27.000000 bittensor-wallet-0.0.4/README.md
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.831829 bittensor-wallet-0.0.4/bittensor_wallet/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5677 2023-07-11 22:18:41.000000 bittensor-wallet-0.0.4/bittensor_wallet/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.832842 bittensor-wallet-0.0.4/bittensor_wallet/_keyfile/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1796 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/bittensor_wallet/_keyfile/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    20057 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.4/bittensor_wallet/_keyfile/keyfile_impl.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1204 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.4/bittensor_wallet/keypair_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.833492 bittensor-wallet-0.0.4/bittensor_wallet/mock/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1226 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3235 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/keyfile_mock.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.833923 bittensor-wallet-0.0.4/bittensor_wallet/mock/utils/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1211 2023-07-11 21:42:39.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/utils/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1669 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/utils/utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      658 2023-07-11 04:46:12.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3468 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/wallet_mock.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3781 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.4/bittensor_wallet/utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    24066 2023-06-26 22:09:07.000000 bittensor-wallet-0.0.4/bittensor_wallet/wallet_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.832561 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-07-13 20:19:06.000000 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      678 2023-07-13 20:19:06.000000 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/SOURCES.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-07-13 20:19:06.000000 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/dependency_links.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      165 2023-07-13 20:19:06.000000 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/requires.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       17 2023-07-13 20:19:06.000000 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/top_level.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-07-13 20:19:06.834797 bittensor-wallet-0.0.4/setup.cfg
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3635 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/setup.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.834319 bittensor-wallet-0.0.4/tests/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    12379 2023-07-11 22:16:48.000000 bittensor-wallet-0.0.4/tests/test.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     9441 2023-06-26 22:03:51.000000 bittensor-wallet-0.0.4/tests/test_keypair.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-14 21:02:23.226190 bittensor-wallet-0.0.5/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1085 2023-06-27 17:13:40.000000 bittensor-wallet-0.0.5/LICENSE
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-07-14 21:02:23.225979 bittensor-wallet-0.0.5/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      711 2023-07-14 17:08:20.000000 bittensor-wallet-0.0.5/README.md
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-14 21:02:23.223290 bittensor-wallet-0.0.5/bittensor_wallet/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5677 2023-07-14 17:08:11.000000 bittensor-wallet-0.0.5/bittensor_wallet/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-14 21:02:23.224314 bittensor-wallet-0.0.5/bittensor_wallet/_keyfile/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1796 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.5/bittensor_wallet/_keyfile/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    20057 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.5/bittensor_wallet/_keyfile/keyfile_impl.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1204 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.5/bittensor_wallet/keypair_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-14 21:02:23.224920 bittensor-wallet-0.0.5/bittensor_wallet/mock/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1226 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.5/bittensor_wallet/mock/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3235 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.5/bittensor_wallet/mock/keyfile_mock.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-14 21:02:23.225202 bittensor-wallet-0.0.5/bittensor_wallet/mock/utils/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1211 2023-07-13 20:19:40.000000 bittensor-wallet-0.0.5/bittensor_wallet/mock/utils/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1669 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.5/bittensor_wallet/mock/utils/utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      658 2023-07-11 04:46:12.000000 bittensor-wallet-0.0.5/bittensor_wallet/mock/utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3414 2023-07-14 17:07:42.000000 bittensor-wallet-0.0.5/bittensor_wallet/mock/wallet_mock.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3781 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.5/bittensor_wallet/utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    24066 2023-06-26 22:09:07.000000 bittensor-wallet-0.0.5/bittensor_wallet/wallet_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-14 21:02:23.224026 bittensor-wallet-0.0.5/bittensor_wallet.egg-info/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-07-14 21:02:23.000000 bittensor-wallet-0.0.5/bittensor_wallet.egg-info/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      678 2023-07-14 21:02:23.000000 bittensor-wallet-0.0.5/bittensor_wallet.egg-info/SOURCES.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-07-14 21:02:23.000000 bittensor-wallet-0.0.5/bittensor_wallet.egg-info/dependency_links.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      172 2023-07-14 21:02:23.000000 bittensor-wallet-0.0.5/bittensor_wallet.egg-info/requires.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       17 2023-07-14 21:02:23.000000 bittensor-wallet-0.0.5/bittensor_wallet.egg-info/top_level.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-07-14 21:02:23.226259 bittensor-wallet-0.0.5/setup.cfg
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3635 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.5/setup.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-14 21:02:23.225729 bittensor-wallet-0.0.5/tests/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    12379 2023-07-13 20:19:40.000000 bittensor-wallet-0.0.5/tests/test.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     9441 2023-06-26 22:03:51.000000 bittensor-wallet-0.0.5/tests/test_keypair.py
```

### Comparing `bittensor-wallet-0.0.4/LICENSE` & `bittensor-wallet-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/PKG-INFO` & `bittensor-wallet-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor-wallet
-Version: 0.0.4
+Version: 0.0.5
 Summary: BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the Bittensor API.
 Home-page: https://github.com/opentensor/bittensor-wallet
 Author: opentensor.ai
 Author-email: hello@opentensor.dev
 Maintainer: 
 Maintainer-email: 
 License: MIT
@@ -22,24 +22,24 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# BittensorWallet - v0.0.4
+# BittensorWallet - v0.0.5
 
 BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the [Bittensor Python API](https://github.com/opentensor/bittensor).  
 
 The purpose of this repo is to separate the concern of keyfile management from the https://github.com/opentensor/bittensor repo, to decrease the attack surface of Bittensor related to local keys and wallet functionality.  
 
 # Installation
 This package can be installed from [PyPi.org](https://pypi.org/project/bittensor-wallet/):
 ```bash
-pip install bittensor-wallet==0.0.4
+pip install bittensor-wallet==0.0.5
 ```
 or via this repo (using [gh-cli](https://cli.github.com/)):  
 ```bash
 gh repo clone opentensor/bittensor-wallet
 cd bittensor-wallet
 pip install -e .
 ```
```

### Comparing `bittensor-wallet-0.0.4/README.md` & `bittensor-wallet-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# BittensorWallet - v0.0.4
+# BittensorWallet - v0.0.5
 
 BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the [Bittensor Python API](https://github.com/opentensor/bittensor).  
 
 The purpose of this repo is to separate the concern of keyfile management from the https://github.com/opentensor/bittensor repo, to decrease the attack surface of Bittensor related to local keys and wallet functionality.  
 
 # Installation
 This package can be installed from [PyPi.org](https://pypi.org/project/bittensor-wallet/):
 ```bash
-pip install bittensor-wallet==0.0.4
+pip install bittensor-wallet==0.0.5
 ```
 or via this repo (using [gh-cli](https://cli.github.com/)):  
 ```bash
 gh repo clone opentensor/bittensor-wallet
 cd bittensor-wallet
 pip install -e .
 ```
```

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/__init__.py` & `bittensor-wallet-0.0.5/bittensor_wallet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __ss58_format__ = 42 # Bittensor ss58 format
 
 import argparse
 import copy
 import os
 from typing import Optional
```

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/_keyfile/__init__.py` & `bittensor-wallet-0.0.5/bittensor_wallet/_keyfile/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/_keyfile/keyfile_impl.py` & `bittensor-wallet-0.0.5/bittensor_wallet/_keyfile/keyfile_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/keypair_impl.py` & `bittensor-wallet-0.0.5/bittensor_wallet/keypair_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/mock/__init__.py` & `bittensor-wallet-0.0.5/bittensor_wallet/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/mock/keyfile_mock.py` & `bittensor-wallet-0.0.5/bittensor_wallet/mock/keyfile_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/mock/utils/__init__.py` & `bittensor-wallet-0.0.5/bittensor_wallet/mock/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/mock/utils/utils.py` & `bittensor-wallet-0.0.5/bittensor_wallet/mock/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/mock/utils.py` & `bittensor-wallet-0.0.5/bittensor_wallet/mock/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/mock/wallet_mock.py` & `bittensor-wallet-0.0.5/bittensor_wallet/mock/wallet_mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,16 +39,14 @@
         """
         super().__init__(**kwargs)
         # For mocking.
         self._is_mock = True
         self._mocked_coldkey_keyfile = None
         self._mocked_hotkey_keyfile = None
 
-        print("---- MOCKED WALLET INITIALIZED- ---")
-
     @property
     def hotkey_file(self) -> 'bittensor_wallet.Keyfile':
         if self._is_mock:
             if self._mocked_hotkey_keyfile == None:
                 self._mocked_hotkey_keyfile = MockKeyfile(path='MockedHotkey')
             return self._mocked_hotkey_keyfile
         else:
```

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/utils.py` & `bittensor-wallet-0.0.5/bittensor_wallet/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet/wallet_impl.py` & `bittensor-wallet-0.0.5/bittensor_wallet/wallet_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet.egg-info/PKG-INFO` & `bittensor-wallet-0.0.5/bittensor_wallet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor-wallet
-Version: 0.0.4
+Version: 0.0.5
 Summary: BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the Bittensor API.
 Home-page: https://github.com/opentensor/bittensor-wallet
 Author: opentensor.ai
 Author-email: hello@opentensor.dev
 Maintainer: 
 Maintainer-email: 
 License: MIT
@@ -22,24 +22,24 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# BittensorWallet - v0.0.4
+# BittensorWallet - v0.0.5
 
 BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the [Bittensor Python API](https://github.com/opentensor/bittensor).  
 
 The purpose of this repo is to separate the concern of keyfile management from the https://github.com/opentensor/bittensor repo, to decrease the attack surface of Bittensor related to local keys and wallet functionality.  
 
 # Installation
 This package can be installed from [PyPi.org](https://pypi.org/project/bittensor-wallet/):
 ```bash
-pip install bittensor-wallet==0.0.4
+pip install bittensor-wallet==0.0.5
 ```
 or via this repo (using [gh-cli](https://cli.github.com/)):  
 ```bash
 gh repo clone opentensor/bittensor-wallet
 cd bittensor-wallet
 pip install -e .
 ```
```

### Comparing `bittensor-wallet-0.0.4/bittensor_wallet.egg-info/SOURCES.txt` & `bittensor-wallet-0.0.5/bittensor_wallet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/setup.py` & `bittensor-wallet-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/tests/test.py` & `bittensor-wallet-0.0.5/tests/test.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.4/tests/test_keypair.py` & `bittensor-wallet-0.0.5/tests/test_keypair.py`

 * *Files identical despite different names*

