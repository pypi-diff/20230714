# Comparing `tmp/eppo-server-sdk-1.2.1.tar.gz` & `tmp/eppo-server-sdk-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eppo-server-sdk-1.2.1.tar", last modified: Thu Jul 13 23:14:58 2023, max compression
+gzip compressed data, was "eppo-server-sdk-1.2.2.tar", last modified: Fri Jul 14 17:53:10 2023, max compression
```

## Comparing `eppo-server-sdk-1.2.1.tar` & `eppo-server-sdk-1.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sven       (501) staff       (20)        0 2023-07-13 23:14:58.146839 eppo-server-sdk-1.2.1/
--rw-r--r--   0 sven       (501) staff       (20)     1071 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/LICENSE
--rw-r--r--   0 sven       (501) staff       (20)       88 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/MANIFEST.in
--rw-r--r--   0 sven       (501) staff       (20)      799 2023-07-13 23:14:58.146918 eppo-server-sdk-1.2.1/PKG-INFO
--rw-r--r--   0 sven       (501) staff       (20)      308 2023-07-13 23:14:30.000000 eppo-server-sdk-1.2.1/README.md
-drwxr-xr-x   0 sven       (501) staff       (20)        0 2023-07-13 23:14:58.145934 eppo-server-sdk-1.2.1/eppo_client/
--rw-r--r--   0 sven       (501) staff       (20)     2507 2023-07-13 23:14:30.000000 eppo-server-sdk-1.2.1/eppo_client/__init__.py
--rw-r--r--   0 sven       (501) staff       (20)      117 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/assignment_logger.py
--rw-r--r--   0 sven       (501) staff       (20)      326 2023-07-13 22:58:53.000000 eppo-server-sdk-1.2.1/eppo_client/base_model.py
--rw-r--r--   0 sven       (501) staff       (20)     4946 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/client.py
--rw-r--r--   0 sven       (501) staff       (20)      518 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/config.py
--rw-r--r--   0 sven       (501) staff       (20)     1914 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/configuration_requestor.py
--rw-r--r--   0 sven       (501) staff       (20)      868 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/configuration_store.py
--rw-r--r--   0 sven       (501) staff       (20)      249 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/constants.py
--rw-r--r--   0 sven       (501) staff       (20)     2107 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/http_client.py
--rw-r--r--   0 sven       (501) staff       (20)     1130 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/poller.py
--rw-r--r--   0 sven       (501) staff       (20)     1222 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/read_write_lock.py
--rw-r--r--   0 sven       (501) staff       (20)     2200 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/rules.py
--rw-r--r--   0 sven       (501) staff       (20)      618 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/shard.py
--rw-r--r--   0 sven       (501) staff       (20)      193 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/eppo_client/validation.py
-drwxr-xr-x   0 sven       (501) staff       (20)        0 2023-07-13 23:14:58.146708 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/
--rw-r--r--   0 sven       (501) staff       (20)      799 2023-07-13 23:14:58.000000 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sven       (501) staff       (20)      661 2023-07-13 23:14:58.000000 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sven       (501) staff       (20)        1 2023-07-13 23:14:58.000000 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sven       (501) staff       (20)       29 2023-07-13 23:14:58.000000 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/requires.txt
--rw-r--r--   0 sven       (501) staff       (20)       12 2023-07-13 23:14:58.000000 eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/top_level.txt
--rw-r--r--   0 sven       (501) staff       (20)       84 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/pyproject.toml
--rw-r--r--   0 sven       (501) staff       (20)       25 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.1/requirements-test.txt
--rw-r--r--   0 sven       (501) staff       (20)       99 2023-07-13 23:14:30.000000 eppo-server-sdk-1.2.1/requirements.txt
--rw-r--r--   0 sven       (501) staff       (20)      667 2023-07-13 23:14:58.147216 eppo-server-sdk-1.2.1/setup.cfg
+drwxr-xr-x   0 sven       (501) staff       (20)        0 2023-07-14 17:53:10.649696 eppo-server-sdk-1.2.2/
+-rw-r--r--   0 sven       (501) staff       (20)     1071 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/LICENSE
+-rw-r--r--   0 sven       (501) staff       (20)       88 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/MANIFEST.in
+-rw-r--r--   0 sven       (501) staff       (20)      799 2023-07-14 17:53:10.649786 eppo-server-sdk-1.2.2/PKG-INFO
+-rw-r--r--   0 sven       (501) staff       (20)      308 2023-07-13 23:14:30.000000 eppo-server-sdk-1.2.2/README.md
+drwxr-xr-x   0 sven       (501) staff       (20)        0 2023-07-14 17:53:10.648631 eppo-server-sdk-1.2.2/eppo_client/
+-rw-r--r--   0 sven       (501) staff       (20)     2507 2023-07-14 17:53:01.000000 eppo-server-sdk-1.2.2/eppo_client/__init__.py
+-rw-r--r--   0 sven       (501) staff       (20)      117 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/assignment_logger.py
+-rw-r--r--   0 sven       (501) staff       (20)      326 2023-07-13 22:58:53.000000 eppo-server-sdk-1.2.2/eppo_client/base_model.py
+-rw-r--r--   0 sven       (501) staff       (20)     4946 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/client.py
+-rw-r--r--   0 sven       (501) staff       (20)      518 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/config.py
+-rw-r--r--   0 sven       (501) staff       (20)     1914 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/configuration_requestor.py
+-rw-r--r--   0 sven       (501) staff       (20)      868 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/configuration_store.py
+-rw-r--r--   0 sven       (501) staff       (20)      249 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/constants.py
+-rw-r--r--   0 sven       (501) staff       (20)     2107 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/http_client.py
+-rw-r--r--   0 sven       (501) staff       (20)     1130 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/poller.py
+-rw-r--r--   0 sven       (501) staff       (20)     1222 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/read_write_lock.py
+-rw-r--r--   0 sven       (501) staff       (20)     2200 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/rules.py
+-rw-r--r--   0 sven       (501) staff       (20)      618 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/shard.py
+-rw-r--r--   0 sven       (501) staff       (20)      193 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/eppo_client/validation.py
+drwxr-xr-x   0 sven       (501) staff       (20)        0 2023-07-14 17:53:10.649559 eppo-server-sdk-1.2.2/eppo_server_sdk.egg-info/
+-rw-r--r--   0 sven       (501) staff       (20)      799 2023-07-14 17:53:10.000000 eppo-server-sdk-1.2.2/eppo_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sven       (501) staff       (20)      661 2023-07-14 17:53:10.000000 eppo-server-sdk-1.2.2/eppo_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sven       (501) staff       (20)        1 2023-07-14 17:53:10.000000 eppo-server-sdk-1.2.2/eppo_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sven       (501) staff       (20)       31 2023-07-14 17:53:10.000000 eppo-server-sdk-1.2.2/eppo_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 sven       (501) staff       (20)       12 2023-07-14 17:53:10.000000 eppo-server-sdk-1.2.2/eppo_server_sdk.egg-info/top_level.txt
+-rw-r--r--   0 sven       (501) staff       (20)       84 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/pyproject.toml
+-rw-r--r--   0 sven       (501) staff       (20)       25 2023-07-13 22:42:54.000000 eppo-server-sdk-1.2.2/requirements-test.txt
+-rw-r--r--   0 sven       (501) staff       (20)       99 2023-07-13 23:14:30.000000 eppo-server-sdk-1.2.2/requirements.txt
+-rw-r--r--   0 sven       (501) staff       (20)      669 2023-07-14 17:53:10.650125 eppo-server-sdk-1.2.2/setup.cfg
```

### Comparing `eppo-server-sdk-1.2.1/LICENSE` & `eppo-server-sdk-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.1/PKG-INFO` & `eppo-server-sdk-1.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 1.2.1
+Version: 1.2.2
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eppo-server-sdk-1.2.1/eppo_client/__init__.py` & `eppo-server-sdk-1.2.2/eppo_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ExperimentConfigurationRequestor,
 )
 from eppo_client.configuration_store import ConfigurationStore
 from eppo_client.constants import MAX_CACHE_ENTRIES
 from eppo_client.http_client import HttpClient, SdkParams
 from eppo_client.read_write_lock import ReadWriteLock
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 __client: Optional[EppoClient] = None
 __lock = ReadWriteLock()
 
 
 def init(config: Config) -> EppoClient:
     """Initializes a global Eppo client instance
```

### Comparing `eppo-server-sdk-1.2.1/eppo_client/client.py` & `eppo-server-sdk-1.2.2/eppo_client/client.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.1/eppo_client/config.py` & `eppo-server-sdk-1.2.2/eppo_client/config.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.1/eppo_client/configuration_requestor.py` & `eppo-server-sdk-1.2.2/eppo_client/configuration_requestor.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.1/eppo_client/configuration_store.py` & `eppo-server-sdk-1.2.2/eppo_client/configuration_store.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.1/eppo_client/http_client.py` & `eppo-server-sdk-1.2.2/eppo_client/http_client.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.1/eppo_client/poller.py` & `eppo-server-sdk-1.2.2/eppo_client/poller.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.1/eppo_client/read_write_lock.py` & `eppo-server-sdk-1.2.2/eppo_client/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.1/eppo_client/rules.py` & `eppo-server-sdk-1.2.2/eppo_client/rules.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.1/eppo_client/shard.py` & `eppo-server-sdk-1.2.2/eppo_client/shard.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/PKG-INFO` & `eppo-server-sdk-1.2.2/eppo_server_sdk.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 1.2.1
+Version: 1.2.2
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eppo-server-sdk-1.2.1/eppo_server_sdk.egg-info/SOURCES.txt` & `eppo-server-sdk-1.2.2/eppo_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.2.1/setup.cfg` & `eppo-server-sdk-1.2.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = eppo_client
 python_requires = >=3.6
 include_package_data = True
 install_requires = 
-	pydantic
+	pydantic<2
 	requests
 	cachetools
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

