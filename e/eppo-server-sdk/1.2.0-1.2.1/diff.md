# Comparing `tmp/eppo-server-sdk-1.2.0.tar.gz` & `tmp/eppo-server-sdk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eppo-server-sdk-1.2.0.tar", last modified: Mon Apr 24 21:00:48 2023, max compression
+gzip compressed data, was "eppo-server-sdk-1.2.1.tar", last modified: Thu Jul 13 23:14:58 2023, max compression
```

## Comparing `eppo-server-sdk-1.2.0.tar` & `eppo-server-sdk-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:00:48.738955 eppo-server-sdk-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     1071 2022-05-06 19:46:08.000000 eppo-server-sdk-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       88 2022-05-06 19:46:08.000000 eppo-server-sdk-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      762 2023-04-24 21:00:48.739630 eppo-server-sdk-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      271 2023-04-21 00:23:31.000000 eppo-server-sdk-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:00:48.709364 eppo-server-sdk-1.2.0/eppo_client/
--rw-r--r--   0 root         (0) root         (0)     2507 2023-04-24 20:58:09.000000 eppo-server-sdk-1.2.0/eppo_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-21 00:23:31.000000 eppo-server-sdk-1.2.0/eppo_client/assignment_logger.py
--rw-r--r--   0 root         (0) root         (0)      326 2022-05-06 19:46:08.000000 eppo-server-sdk-1.2.0/eppo_client/base_model.py
--rw-r--r--   0 root         (0) root         (0)     4946 2023-04-21 00:23:31.000000 eppo-server-sdk-1.2.0/eppo_client/client.py
--rw-r--r--   0 root         (0) root         (0)      518 2023-04-24 20:58:09.000000 eppo-server-sdk-1.2.0/eppo_client/config.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-04-24 20:58:09.000000 eppo-server-sdk-1.2.0/eppo_client/configuration_requestor.py
--rw-r--r--   0 root         (0) root         (0)      868 2022-05-06 19:46:08.000000 eppo-server-sdk-1.2.0/eppo_client/configuration_store.py
--rw-r--r--   0 root         (0) root         (0)      249 2022-05-06 19:46:08.000000 eppo-server-sdk-1.2.0/eppo_client/constants.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-04-21 00:23:31.000000 eppo-server-sdk-1.2.0/eppo_client/http_client.py
--rw-r--r--   0 root         (0) root         (0)     1130 2022-05-06 19:46:08.000000 eppo-server-sdk-1.2.0/eppo_client/poller.py
--rw-r--r--   0 root         (0) root         (0)     1222 2022-05-06 19:46:08.000000 eppo-server-sdk-1.2.0/eppo_client/read_write_lock.py
--rw-r--r--   0 root         (0) root         (0)     2200 2023-04-21 00:23:31.000000 eppo-server-sdk-1.2.0/eppo_client/rules.py
--rw-r--r--   0 root         (0) root         (0)      618 2022-05-06 19:46:08.000000 eppo-server-sdk-1.2.0/eppo_client/shard.py
--rw-r--r--   0 root         (0) root         (0)      193 2022-05-06 19:46:08.000000 eppo-server-sdk-1.2.0/eppo_client/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:00:48.735094 eppo-server-sdk-1.2.0/eppo_server_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      762 2023-04-24 21:00:48.000000 eppo-server-sdk-1.2.0/eppo_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      661 2023-04-24 21:00:48.000000 eppo-server-sdk-1.2.0/eppo_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 21:00:48.000000 eppo-server-sdk-1.2.0/eppo_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-24 21:00:48.000000 eppo-server-sdk-1.2.0/eppo_server_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-24 21:00:48.000000 eppo-server-sdk-1.2.0/eppo_server_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       84 2022-05-06 19:46:08.000000 eppo-server-sdk-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-21 00:23:31.000000 eppo-server-sdk-1.2.0/requirements-test.txt
--rw-r--r--   0 root         (0) root         (0)       61 2022-05-06 19:46:08.000000 eppo-server-sdk-1.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      667 2023-04-24 21:00:48.742196 eppo-server-sdk-1.2.0/setup.cfg
+drwxr-xr-x   0 sven       (501) staff       (20)        0 2023-07-13 23:14:58.146839 eppo-server-sdk-1.2.1/
+-rw-r--r--   0 sven       (501) staff       (20)     1071 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/LICENSE
+-rw-r--r--   0 sven       (501) staff       (20)       88 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/MANIFEST.in
+-rw-r--r--   0 sven       (501) staff       (20)      799 2023-07-13 23:14:58.146918 eppo-server-sdk-1.2.1/PKG-INFO
+-rw-r--r--   0 sven       (501) staff       (20)      308 2023-07-13 23:14:30.000000 eppo-server-sdk-1.2.1/README.md
+drwxr-xr-x   0 sven       (501) staff       (20)        0 2023-07-13 23:14:58.145934 eppo-server-sdk-1.2.1/eppo_client/
+-rw-r--r--   0 sven       (501) staff       (20)     2507 2023-07-13 23:14:30.000000 eppo-server-sdk-1.2.1/eppo_client/__init__.py
+-rw-r--r--   0 sven       (501) staff       (20)      117 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/assignment_logger.py
+-rw-r--r--   0 sven       (501) staff       (20)      326 2023-07-13 22:58:53.000000 eppo-server-sdk-1.2.1/eppo_client/base_model.py
+-rw-r--r--   0 sven       (501) staff       (20)     4946 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/client.py
+-rw-r--r--   0 sven       (501) staff       (20)      518 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/config.py
+-rw-r--r--   0 sven       (501) staff       (20)     1914 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/configuration_requestor.py
+-rw-r--r--   0 sven       (501) staff       (20)      868 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/configuration_store.py
+-rw-r--r--   0 sven       (501) staff       (20)      249 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/constants.py
+-rw-r--r--   0 sven       (501) staff       (20)     2107 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/http_client.py
+-rw-r--r--   0 sven       (501) staff       (20)     1130 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/poller.py
+-rw-r--r--   0 sven       (501) staff       (20)     1222 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/read_write_lock.py
+-rw-r--r--   0 sven       (501) staff       (20)     2200 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/rules.py
+-rw-r--r--   0 sven       (501) staff       (20)      618 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/shard.py
+-rw-r--r--   0 sven       (501) staff       (20)      193 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/validation.py
+drwxr-xr-x   0 sven       (501) staff       (20)        0 2023-07-13 23:14:58.146708 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/
+-rw-r--r--   0 sven       (501) staff       (20)      799 2023-07-13 23:14:58.000000 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sven       (501) staff       (20)      661 2023-07-13 23:14:58.000000 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sven       (501) staff       (20)        1 2023-07-13 23:14:58.000000 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sven       (501) staff       (20)       29 2023-07-13 23:14:58.000000 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 sven       (501) staff       (20)       12 2023-07-13 23:14:58.000000 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/top_level.txt
+-rw-r--r--   0 sven       (501) staff       (20)       84 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/pyproject.toml
+-rw-r--r--   0 sven       (501) staff       (20)       25 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/requirements-test.txt
+-rw-r--r--   0 sven       (501) staff       (20)       99 2023-07-13 23:14:30.000000 eppo-server-sdk-1.2.1/requirements.txt
+-rw-r--r--   0 sven       (501) staff       (20)      667 2023-07-13 23:14:58.147216 eppo-server-sdk-1.2.1/setup.cfg
```

### Comparing `eppo-server-sdk-1.2.0/LICENSE` & `eppo-server-sdk-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.0/PKG-INFO` & `eppo-server-sdk-1.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 1.2.0
+Version: 1.2.1
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,11 +13,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Eppo SDK for Python
 
 ## Getting Started
 
-Refer to our [SDK documentation](https://docs.geteppo.com/feature-flags/sdks/server-sdks/python) for how to install and use the SDK.
+Refer to our [SDK documentation](https://docs.geteppo.com/feature-flags/sdks/python) for how to install and use the SDK.
 
 ## Supported Python Versions
+
 This version of the SDK is compatible with Python 3.6 and above.
+
+## Development
+
+### Running tests
+
+`make test`
```

### Comparing `eppo-server-sdk-1.2.0/eppo_client/__init__.py` & `eppo-server-sdk-1.2.1/eppo_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ExperimentConfigurationRequestor,
 )
 from eppo_client.configuration_store import ConfigurationStore
 from eppo_client.constants import MAX_CACHE_ENTRIES
 from eppo_client.http_client import HttpClient, SdkParams
 from eppo_client.read_write_lock import ReadWriteLock
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 __client: Optional[EppoClient] = None
 __lock = ReadWriteLock()
 
 
 def init(config: Config) -> EppoClient:
     """Initializes a global Eppo client instance
```

### Comparing `eppo-server-sdk-1.2.0/eppo_client/client.py` & `eppo-server-sdk-1.2.1/eppo_client/client.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.0/eppo_client/config.py` & `eppo-server-sdk-1.2.1/eppo_client/config.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.0/eppo_client/configuration_requestor.py` & `eppo-server-sdk-1.2.1/eppo_client/configuration_requestor.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.0/eppo_client/configuration_store.py` & `eppo-server-sdk-1.2.1/eppo_client/configuration_store.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.0/eppo_client/http_client.py` & `eppo-server-sdk-1.2.1/eppo_client/http_client.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.0/eppo_client/poller.py` & `eppo-server-sdk-1.2.1/eppo_client/poller.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.0/eppo_client/read_write_lock.py` & `eppo-server-sdk-1.2.1/eppo_client/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.0/eppo_client/rules.py` & `eppo-server-sdk-1.2.1/eppo_client/rules.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.0/eppo_client/shard.py` & `eppo-server-sdk-1.2.1/eppo_client/shard.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.0/eppo_server_sdk.egg-info/PKG-INFO` & `eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 1.2.0
+Version: 1.2.1
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,11 +13,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Eppo SDK for Python
 
 ## Getting Started
 
-Refer to our [SDK documentation](https://docs.geteppo.com/feature-flags/sdks/server-sdks/python) for how to install and use the SDK.
+Refer to our [SDK documentation](https://docs.geteppo.com/feature-flags/sdks/python) for how to install and use the SDK.
 
 ## Supported Python Versions
+
 This version of the SDK is compatible with Python 3.6 and above.
+
+## Development
+
+### Running tests
+
+`make test`
```

### Comparing `eppo-server-sdk-1.2.0/eppo_server_sdk.egg-info/SOURCES.txt` & `eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.0/setup.cfg` & `eppo-server-sdk-1.2.1/setup.cfg`

 * *Files identical despite different names*

