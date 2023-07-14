# Comparing `tmp/cbcmgr-1.4.2.tar.gz` & `tmp/cbcmgr-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.4.2.tar", last modified: Thu Jul 13 02:48:10 2023, max compression
+gzip compressed data, was "cbcmgr-1.4.3.tar", last modified: Fri Jul 14 15:56:18 2023, max compression
```

## Comparing `cbcmgr-1.4.2.tar` & `cbcmgr-1.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-13 02:48:10.111665 cbcmgr-1.4.2/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.4.2/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-13 02:48:10.111279 cbcmgr-1.4.2/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.4.2/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-13 02:48:10.097897 cbcmgr-1.4.2/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.4.2/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     2606 2023-07-13 01:40:09.000000 cbcmgr-1.4.2/cbcmgr/async_pool.py
--rw-r--r--   0 michael    (501) staff       (20)    10719 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    10466 2023-07-13 01:22:43.000000 cbcmgr-1.4.2/cbcmgr/cb_connect_lite.py
--rw-r--r--   0 michael    (501) staff       (20)    11368 2023-07-13 02:29:07.000000 cbcmgr-1.4.2/cbcmgr/cb_connect_lite_a.py
--rw-r--r--   0 michael    (501) staff       (20)    27544 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)     7658 2023-07-12 21:45:43.000000 cbcmgr-1.4.2/cbcmgr/cb_operation_a.py
--rw-r--r--   0 michael    (501) staff       (20)     7121 2023-07-12 14:35:27.000000 cbcmgr-1.4.2/cbcmgr/cb_operation_s.py
--rw-r--r--   0 michael    (501) staff       (20)     3881 2023-07-12 13:52:42.000000 cbcmgr-1.4.2/cbcmgr/cb_pathmap.py
--rw-r--r--   0 michael    (501) staff       (20)    12508 2023-07-12 14:35:27.000000 cbcmgr-1.4.2/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.4.2/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4334 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.4.2/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)      938 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/id_format.py
--rw-r--r--   0 michael    (501) staff       (20)     2373 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/mt_pool.py
--rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-1.4.2/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.4.2/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)     1446 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-13 02:48:10.110567 cbcmgr-1.4.2/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-13 02:48:09.000000 cbcmgr-1.4.2/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      559 2023-07-13 02:48:09.000000 cbcmgr-1.4.2/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-13 02:48:09.000000 cbcmgr-1.4.2/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       82 2023-07-13 02:48:09.000000 cbcmgr-1.4.2/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-13 02:48:09.000000 cbcmgr-1.4.2/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-13 02:48:10.111798 cbcmgr-1.4.2/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1292 2023-07-12 22:19:35.000000 cbcmgr-1.4.2/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-14 15:56:18.679311 cbcmgr-1.4.3/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.4.3/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-14 15:56:18.678981 cbcmgr-1.4.3/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.4.3/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-14 15:56:18.423865 cbcmgr-1.4.3/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.4.3/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     3180 2023-07-13 22:09:16.000000 cbcmgr-1.4.3/cbcmgr/async_pool.py
+-rw-r--r--   0 michael    (501) staff       (20)    10719 2023-07-12 01:28:33.000000 cbcmgr-1.4.3/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    10466 2023-07-13 01:22:43.000000 cbcmgr-1.4.3/cbcmgr/cb_connect_lite.py
+-rw-r--r--   0 michael    (501) staff       (20)    11368 2023-07-13 02:29:07.000000 cbcmgr-1.4.3/cbcmgr/cb_connect_lite_a.py
+-rw-r--r--   0 michael    (501) staff       (20)    27544 2023-07-12 01:28:33.000000 cbcmgr-1.4.3/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)     7487 2023-07-13 21:35:08.000000 cbcmgr-1.4.3/cbcmgr/cb_operation_a.py
+-rw-r--r--   0 michael    (501) staff       (20)     7121 2023-07-12 14:35:27.000000 cbcmgr-1.4.3/cbcmgr/cb_operation_s.py
+-rw-r--r--   0 michael    (501) staff       (20)     3881 2023-07-12 13:52:42.000000 cbcmgr-1.4.3/cbcmgr/cb_pathmap.py
+-rw-r--r--   0 michael    (501) staff       (20)    12508 2023-07-12 14:35:27.000000 cbcmgr-1.4.3/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.4.3/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4334 2023-07-12 01:28:33.000000 cbcmgr-1.4.3/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.4.3/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)      938 2023-07-12 01:28:33.000000 cbcmgr-1.4.3/cbcmgr/id_format.py
+-rw-r--r--   0 michael    (501) staff       (20)     2700 2023-07-14 15:07:19.000000 cbcmgr-1.4.3/cbcmgr/mt_pool.py
+-rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-1.4.3/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.4.3/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)     1446 2023-07-12 01:28:33.000000 cbcmgr-1.4.3/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-14 15:56:18.678298 cbcmgr-1.4.3/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-14 15:56:18.000000 cbcmgr-1.4.3/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      559 2023-07-14 15:56:18.000000 cbcmgr-1.4.3/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-14 15:56:18.000000 cbcmgr-1.4.3/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       82 2023-07-14 15:56:18.000000 cbcmgr-1.4.3/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-14 15:56:18.000000 cbcmgr-1.4.3/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-14 15:56:18.679414 cbcmgr-1.4.3/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1292 2023-07-14 15:55:55.000000 cbcmgr-1.4.3/setup.py
```

### Comparing `cbcmgr-1.4.2/LICENSE.txt` & `cbcmgr-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/PKG-INFO` & `cbcmgr-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.4.2
+Version: 1.4.3
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.4.2/README.md` & `cbcmgr-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/async_pool.py` & `cbcmgr-1.4.3/cbcmgr/async_pool.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,51 +21,64 @@
                  ssl=False,
                  external=False,
                  kv_timeout: int = 5,
                  query_timeout: int = 60,
                  create: bool = False,
                  quota: int = 256,
                  replicas: int = 0,
-                 mode: BucketMode = BucketMode.DEFAULT):
+                 mode: BucketMode = BucketMode.DEFAULT,
+                 throttle: bool = False):
         self.keyspace = {}
         self.tasks = set()
         self.loop = asyncio.get_event_loop()
         self.hostname = hostname
         self.username = username
         self.password = password
         self.ssl = ssl
         self.external = external
+        self.kv_timeout = kv_timeout
+        self.query_timeout = query_timeout
         self.create = create
         self.quota = quota
         self.replicas = replicas
         self.mode = mode
-        self.max_tasks = min(100, os.cpu_count() * 10)
+        self.max_tasks = max(32, os.cpu_count() * 2)
         self.factor = 0.01
+        self.throttle = throttle
+        self.retry_number = 0
 
     async def connect(self, keyspace):
         if keyspace in self.keyspace:
             return
         logger.debug(f"pool add: {self.hostname} {keyspace} create is {self.create}")
         opc = CBOperationAsync(self.hostname,
                                self.username,
                                self.password,
                                ssl=self.ssl,
+                               kv_timeout=self.kv_timeout,
+                               query_timeout=self.query_timeout,
                                quota=self.quota,
                                replicas=self.replicas,
                                mode=self.mode,
                                create=self.create)
         opm = await opc.init()
         self.keyspace[keyspace] = await opm.connect(keyspace)
 
     async def dispatch(self, keyspace: str, op: Operation, *args):
-        retry_number = 0
-        while len(asyncio.all_tasks()) > self.max_tasks:
+        if self.throttle and len(asyncio.all_tasks()) > (self.max_tasks * 1.1):
+            self.retry_number += 1
             wait = self.factor
-            wait *= (2 ** (retry_number + 1))
+            wait *= (2 ** self.retry_number)
             await asyncio.sleep(wait)
+        elif self.throttle and len(asyncio.all_tasks()) > self.max_tasks:
+            wait = self.factor
+            wait *= (2 ** self.retry_number)
+            await asyncio.sleep(wait)
+        else:
+            self.retry_number = 0
         opm = self.keyspace[keyspace]
         operator = opm.get_operator(op)
         operator.prep(*args)
         self.tasks.add(self.loop.create_task(operator.execute()))
 
     async def join(self):
         if len(self.tasks) > 0:
```

### Comparing `cbcmgr-1.4.2/cbcmgr/cb_connect.py` & `cbcmgr-1.4.3/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/cb_connect_lite.py` & `cbcmgr-1.4.3/cbcmgr/cb_connect_lite.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/cb_connect_lite_a.py` & `cbcmgr-1.4.3/cbcmgr/cb_connect_lite_a.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/cb_management.py` & `cbcmgr-1.4.3/cbcmgr/cb_management.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/cb_operation_a.py` & `cbcmgr-1.4.3/cbcmgr/cb_operation_a.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 ##
 ##
 
 from __future__ import annotations
 import logging
 from typing import Union, Dict, Any, List
-from enum import Enum
 from acouchbase.cluster import AsyncCluster
 from acouchbase.bucket import AsyncBucket
 from acouchbase.scope import AsyncScope
 from acouchbase.collection import AsyncCollection
 from couchbase.exceptions import (BucketDoesNotExistException, BucketNotFoundException, ScopeNotFoundException, CollectionNotFoundException)
 from cbcmgr.cb_session import BucketMode
 from cbcmgr.cb_connect_lite_a import CBConnectLiteAsync
-from cbcmgr.retry import retry
-from cbcmgr.exceptions import CollectionCountError
-from cbcmgr.httpsessionmgr import APISession
+from cbcmgr.cb_operation_s import Operation
 
 logger = logging.getLogger('cbutil.operation')
 logger.addHandler(logging.NullHandler())
 JSONType = Union[str, int, float, bool, None, Dict[str, Any], List[Any]]
 
 
-class Operation(Enum):
-    READ = 0
-    WRITE = 1
-    QUERY = 2
-
-
 class CBOperationAsync(CBConnectLiteAsync):
 
     def __init__(self, *args, create: bool = False, quota: int = 256, replicas: int = 0, mode: BucketMode = BucketMode.DEFAULT, **kwargs):
         super().__init__(*args, **kwargs)
         logger.debug("begin operation class")
         self._cluster: AsyncCluster
         self._bucket: AsyncBucket
```

### Comparing `cbcmgr-1.4.2/cbcmgr/cb_operation_s.py` & `cbcmgr-1.4.3/cbcmgr/cb_operation_s.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/cb_pathmap.py` & `cbcmgr-1.4.3/cbcmgr/cb_pathmap.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/cb_session.py` & `cbcmgr-1.4.3/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/config.py` & `cbcmgr-1.4.3/cbcmgr/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/exceptions.py` & `cbcmgr-1.4.3/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.4.3/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/id_format.py` & `cbcmgr-1.4.3/cbcmgr/id_format.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/mt_pool.py` & `cbcmgr-1.4.3/cbcmgr/mt_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ##
 ##
 
 import concurrent.futures
 import logging
+import os
 from cbcmgr.exceptions import TaskError
 from cbcmgr.cb_session import BucketMode
 from cbcmgr.cb_operation_s import CBOperation, Operation
 
 logger = logging.getLogger('cbutil.mt.pool')
 logger.addHandler(logging.NullHandler())
 
@@ -23,33 +24,38 @@
                  query_timeout: int = 60,
                  create: bool = False,
                  quota: int = 256,
                  replicas: int = 0,
                  mode: BucketMode = BucketMode.DEFAULT):
         self.keyspace = {}
         self.tasks = set()
-        self.executor = concurrent.futures.ThreadPoolExecutor()
+        self.max_threads = min(64, os.cpu_count() * 4)
+        self.executor = concurrent.futures.ThreadPoolExecutor(max_workers=self.max_threads)
         self.hostname = hostname
         self.username = username
         self.password = password
         self.ssl = ssl
         self.external = external
+        self.kv_timeout = kv_timeout
+        self.query_timeout = query_timeout
         self.create = create
         self.quota = quota
         self.replicas = replicas
         self.mode = mode
 
     def connect(self, keyspace):
         if keyspace in self.keyspace:
             return
         logger.debug(f"pool add: {self.hostname} {keyspace} create is {self.create}")
         self.keyspace[keyspace] = CBOperation(self.hostname,
                                               self.username,
                                               self.password,
                                               ssl=self.ssl,
+                                              kv_timeout=self.kv_timeout,
+                                              query_timeout=self.query_timeout,
                                               quota=self.quota,
                                               replicas=self.replicas,
                                               mode=self.mode,
                                               create=self.create).connect(keyspace)
 
     def dispatch(self, keyspace: str, op: Operation, *args):
         opm = self.keyspace[keyspace]
```

### Comparing `cbcmgr-1.4.2/cbcmgr/retry.py` & `cbcmgr-1.4.3/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/schema.py` & `cbcmgr-1.4.3/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr/util.py` & `cbcmgr-1.4.3/cbcmgr/util.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.4.3/cbcmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.4.2
+Version: 1.4.3
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.4.2/cbcmgr.egg-info/SOURCES.txt` & `cbcmgr-1.4.3/cbcmgr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.2/setup.py` & `cbcmgr-1.4.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.4.2',
+    version='1.4.3',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```

