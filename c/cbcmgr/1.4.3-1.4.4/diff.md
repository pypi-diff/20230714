# Comparing `tmp/cbcmgr-1.4.3.tar.gz` & `tmp/cbcmgr-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.4.3.tar", last modified: Fri Jul 14 15:56:18 2023, max compression
+gzip compressed data, was "cbcmgr-1.4.4.tar", last modified: Fri Jul 14 19:29:06 2023, max compression
```

## Comparing `cbcmgr-1.4.3.tar` & `cbcmgr-1.4.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-14 15:56:18.679311 cbcmgr-1.4.3/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.4.3/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-14 15:56:18.678981 cbcmgr-1.4.3/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.4.3/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-14 15:56:18.423865 cbcmgr-1.4.3/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.4.3/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     3180 2023-07-13 22:09:16.000000 cbcmgr-1.4.3/cbcmgr/async_pool.py
--rw-r--r--   0 michael    (501) staff       (20)    10719 2023-07-12 01:28:33.000000 cbcmgr-1.4.3/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    10466 2023-07-13 01:22:43.000000 cbcmgr-1.4.3/cbcmgr/cb_connect_lite.py
--rw-r--r--   0 michael    (501) staff       (20)    11368 2023-07-13 02:29:07.000000 cbcmgr-1.4.3/cbcmgr/cb_connect_lite_a.py
--rw-r--r--   0 michael    (501) staff       (20)    27544 2023-07-12 01:28:33.000000 cbcmgr-1.4.3/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)     7487 2023-07-13 21:35:08.000000 cbcmgr-1.4.3/cbcmgr/cb_operation_a.py
--rw-r--r--   0 michael    (501) staff       (20)     7121 2023-07-12 14:35:27.000000 cbcmgr-1.4.3/cbcmgr/cb_operation_s.py
--rw-r--r--   0 michael    (501) staff       (20)     3881 2023-07-12 13:52:42.000000 cbcmgr-1.4.3/cbcmgr/cb_pathmap.py
--rw-r--r--   0 michael    (501) staff       (20)    12508 2023-07-12 14:35:27.000000 cbcmgr-1.4.3/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.4.3/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4334 2023-07-12 01:28:33.000000 cbcmgr-1.4.3/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.4.3/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)      938 2023-07-12 01:28:33.000000 cbcmgr-1.4.3/cbcmgr/id_format.py
--rw-r--r--   0 michael    (501) staff       (20)     2700 2023-07-14 15:07:19.000000 cbcmgr-1.4.3/cbcmgr/mt_pool.py
--rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-1.4.3/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.4.3/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)     1446 2023-07-12 01:28:33.000000 cbcmgr-1.4.3/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-14 15:56:18.678298 cbcmgr-1.4.3/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-14 15:56:18.000000 cbcmgr-1.4.3/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      559 2023-07-14 15:56:18.000000 cbcmgr-1.4.3/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-14 15:56:18.000000 cbcmgr-1.4.3/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       82 2023-07-14 15:56:18.000000 cbcmgr-1.4.3/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-14 15:56:18.000000 cbcmgr-1.4.3/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-14 15:56:18.679414 cbcmgr-1.4.3/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1292 2023-07-14 15:55:55.000000 cbcmgr-1.4.3/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-14 19:29:05.975137 cbcmgr-1.4.4/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.4.4/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     2451 2023-07-14 19:29:05.974810 cbcmgr-1.4.4/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1652 2023-07-14 19:16:35.000000 cbcmgr-1.4.4/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-14 19:29:05.921104 cbcmgr-1.4.4/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.4.4/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     3180 2023-07-14 15:57:41.000000 cbcmgr-1.4.4/cbcmgr/async_pool.py
+-rw-r--r--   0 michael    (501) staff       (20)    10719 2023-07-12 01:28:33.000000 cbcmgr-1.4.4/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    10466 2023-07-13 01:22:43.000000 cbcmgr-1.4.4/cbcmgr/cb_connect_lite.py
+-rw-r--r--   0 michael    (501) staff       (20)    11368 2023-07-13 02:29:07.000000 cbcmgr-1.4.4/cbcmgr/cb_connect_lite_a.py
+-rw-r--r--   0 michael    (501) staff       (20)    27544 2023-07-12 01:28:33.000000 cbcmgr-1.4.4/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)     7487 2023-07-14 15:57:41.000000 cbcmgr-1.4.4/cbcmgr/cb_operation_a.py
+-rw-r--r--   0 michael    (501) staff       (20)     7121 2023-07-12 14:35:27.000000 cbcmgr-1.4.4/cbcmgr/cb_operation_s.py
+-rw-r--r--   0 michael    (501) staff       (20)     3881 2023-07-12 13:52:42.000000 cbcmgr-1.4.4/cbcmgr/cb_pathmap.py
+-rw-r--r--   0 michael    (501) staff       (20)    12508 2023-07-12 14:35:27.000000 cbcmgr-1.4.4/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.4.4/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4334 2023-07-12 01:28:33.000000 cbcmgr-1.4.4/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.4.4/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)      938 2023-07-12 01:28:33.000000 cbcmgr-1.4.4/cbcmgr/id_format.py
+-rw-r--r--   0 michael    (501) staff       (20)     3250 2023-07-14 18:20:35.000000 cbcmgr-1.4.4/cbcmgr/mt_pool.py
+-rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-1.4.4/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.4.4/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)     1446 2023-07-12 01:28:33.000000 cbcmgr-1.4.4/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-14 19:29:05.974117 cbcmgr-1.4.4/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     2451 2023-07-14 19:29:05.000000 cbcmgr-1.4.4/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      559 2023-07-14 19:29:05.000000 cbcmgr-1.4.4/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-14 19:29:05.000000 cbcmgr-1.4.4/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       82 2023-07-14 19:29:05.000000 cbcmgr-1.4.4/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-14 19:29:05.000000 cbcmgr-1.4.4/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-14 19:29:05.975235 cbcmgr-1.4.4/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1292 2023-07-14 19:14:28.000000 cbcmgr-1.4.4/setup.py
```

### Comparing `cbcmgr-1.4.3/LICENSE.txt` & `cbcmgr-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/async_pool.py` & `cbcmgr-1.4.4/cbcmgr/async_pool.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/cb_connect.py` & `cbcmgr-1.4.4/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/cb_connect_lite.py` & `cbcmgr-1.4.4/cbcmgr/cb_connect_lite.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/cb_connect_lite_a.py` & `cbcmgr-1.4.4/cbcmgr/cb_connect_lite_a.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/cb_management.py` & `cbcmgr-1.4.4/cbcmgr/cb_management.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/cb_operation_a.py` & `cbcmgr-1.4.4/cbcmgr/cb_operation_a.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/cb_operation_s.py` & `cbcmgr-1.4.4/cbcmgr/cb_operation_s.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/cb_pathmap.py` & `cbcmgr-1.4.4/cbcmgr/cb_pathmap.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/cb_session.py` & `cbcmgr-1.4.4/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/config.py` & `cbcmgr-1.4.4/cbcmgr/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/exceptions.py` & `cbcmgr-1.4.4/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.4.4/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/id_format.py` & `cbcmgr-1.4.4/cbcmgr/id_format.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/mt_pool.py` & `cbcmgr-1.4.4/cbcmgr/mt_pool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 ##
 ##
 
 import concurrent.futures
 import logging
 import os
+import itertools
+from typing import Union
 from cbcmgr.exceptions import TaskError
 from cbcmgr.cb_session import BucketMode
 from cbcmgr.cb_operation_s import CBOperation, Operation
 
 logger = logging.getLogger('cbutil.mt.pool')
 logger.addHandler(logging.NullHandler())
 
@@ -21,18 +23,24 @@
                  ssl=False,
                  external=False,
                  kv_timeout: int = 5,
                  query_timeout: int = 60,
                  create: bool = False,
                  quota: int = 256,
                  replicas: int = 0,
-                 mode: BucketMode = BucketMode.DEFAULT):
+                 mode: BucketMode = BucketMode.DEFAULT,
+                 connections: Union[None, int] = None):
         self.keyspace = {}
         self.tasks = set()
-        self.max_threads = min(64, os.cpu_count() * 4)
+        if connections:
+            self.connections = connections
+        else:
+            self.connections = os.cpu_count()
+        self.index_cycle = itertools.cycle(range(self.connections))
+        self.max_threads = max(self.connections * 4, os.cpu_count() * 4)
         self.executor = concurrent.futures.ThreadPoolExecutor(max_workers=self.max_threads)
         self.hostname = hostname
         self.username = username
         self.password = password
         self.ssl = ssl
         self.external = external
         self.kv_timeout = kv_timeout
@@ -42,27 +50,30 @@
         self.replicas = replicas
         self.mode = mode
 
     def connect(self, keyspace):
         if keyspace in self.keyspace:
             return
         logger.debug(f"pool add: {self.hostname} {keyspace} create is {self.create}")
-        self.keyspace[keyspace] = CBOperation(self.hostname,
-                                              self.username,
-                                              self.password,
-                                              ssl=self.ssl,
-                                              kv_timeout=self.kv_timeout,
-                                              query_timeout=self.query_timeout,
-                                              quota=self.quota,
-                                              replicas=self.replicas,
-                                              mode=self.mode,
-                                              create=self.create).connect(keyspace)
+        self.keyspace[keyspace] = [None] * self.connections
+        for num in range(self.connections):
+            self.keyspace[keyspace][num] = CBOperation(self.hostname,
+                                                       self.username,
+                                                       self.password,
+                                                       ssl=self.ssl,
+                                                       kv_timeout=self.kv_timeout,
+                                                       query_timeout=self.query_timeout,
+                                                       quota=self.quota,
+                                                       replicas=self.replicas,
+                                                       mode=self.mode,
+                                                       create=self.create).connect(keyspace)
 
     def dispatch(self, keyspace: str, op: Operation, *args):
-        opm = self.keyspace[keyspace]
+        index = next(self.index_cycle)
+        opm = self.keyspace[keyspace][index]
         operator = opm.get_operator(op)
         operator.prep(*args)
         self.tasks.add(self.executor.submit(operator.execute))
 
     def join(self):
         while self.tasks:
             done, self.tasks = concurrent.futures.wait(self.tasks, return_when=concurrent.futures.FIRST_COMPLETED)
```

### Comparing `cbcmgr-1.4.3/cbcmgr/retry.py` & `cbcmgr-1.4.4/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/schema.py` & `cbcmgr-1.4.4/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr/util.py` & `cbcmgr-1.4.4/cbcmgr/util.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/cbcmgr.egg-info/SOURCES.txt` & `cbcmgr-1.4.4/cbcmgr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.3/setup.py` & `cbcmgr-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.4.3',
+    version='1.4.4',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```

