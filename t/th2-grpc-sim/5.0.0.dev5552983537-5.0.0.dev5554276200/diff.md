# Comparing `tmp/th2_grpc_sim-5.0.0.dev5552983537.tar.gz` & `tmp/th2_grpc_sim-5.0.0.dev5554276200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_sim-5.0.0.dev5552983537.tar", last modified: Fri Jul 14 10:13:26 2023, max compression
+gzip compressed data, was "dist/th2_grpc_sim-5.0.0.dev5554276200.tar", last modified: Fri Jul 14 12:52:47 2023, max compression
```

## Comparing `th2_grpc_sim-5.0.0.dev5552983537.tar` & `th2_grpc_sim-5.0.0.dev5554276200.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-07-14 10:12:29.000000 th2_grpc_sim-5.0.0.dev5552983537/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-14 10:12:30.000000 th2_grpc_sim-5.0.0.dev5552983537/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-07-14 10:12:29.000000 th2_grpc_sim-5.0.0.dev5552983537/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-07-14 10:12:29.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim/sim.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2586 2023-07-14 10:13:25.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim/sim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     4355 2023-07-14 10:13:25.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim/sim_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     7291 2023-07-14 10:13:25.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim/sim_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-07-14 10:13:06.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim/sim_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-14 10:13:26.000000 th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 12:52:47.000000 th2_grpc_sim-5.0.0.dev5554276200/
+-rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-07-14 12:52:47.000000 th2_grpc_sim-5.0.0.dev5554276200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-07-14 12:51:50.000000 th2_grpc_sim-5.0.0.dev5554276200/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-14 12:51:51.000000 th2_grpc_sim-5.0.0.dev5554276200/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 12:52:47.000000 th2_grpc_sim-5.0.0.dev5554276200/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-07-14 12:51:50.000000 th2_grpc_sim-5.0.0.dev5554276200/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 12:52:47.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 12:52:46.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 12:52:46.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-07-14 12:51:50.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim/sim.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-07-14 12:52:46.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim/sim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5241 2023-07-14 12:52:46.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim/sim_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     7291 2023-07-14 12:52:46.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim/sim_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-07-14 12:52:31.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim/sim_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 12:52:47.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-07-14 12:52:46.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-07-14 12:52:47.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 12:52:46.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-07-14 12:52:46.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-14 12:52:46.000000 th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim.egg-info/top_level.txt
```

### Comparing `th2_grpc_sim-5.0.0.dev5552983537/PKG-INFO` & `th2_grpc_sim-5.0.0.dev5554276200/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_sim
-Version: 5.0.0.dev5552983537
+Version: 5.0.0.dev5554276200
 Summary: th2_grpc_sim
 Home-page: https://github.com/th2-net/th2-grpc-sim
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim library
         
@@ -42,19 +42,28 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 5.1.0
+        
+        + Update to `th2-bom` version `4.4.0`
+        + Update to `th2-grpc-service-genrator` version `3.4.0`
+        + Update to `grpcio-tools` version `1.56.0`
+        + Update to `mypy-protobuf` version `3.4`
+        
         ### 4.2.0
+        
         + Update libraries versions.
         + Vulnerability check pipeline step.
         
         ### 4.1.0
+        
         + Add stubs for Python
         + Update `th2-grpc-common` from `3.9.0` to `3.11.1`
         + Update `th2-grpc-service-generator` from `3.1.12` to `3.2.2`
         
         ### 4.0.0 
         + New param relation
         + Added new method 'getRelatedRules'
```

### Comparing `th2_grpc_sim-5.0.0.dev5552983537/README.md` & `th2_grpc_sim-5.0.0.dev5554276200/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,19 +34,28 @@
     python setup.py sdist
     twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
     ```
    `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
 
 ## Release notes
 
+### 5.1.0
+
++ Update to `th2-bom` version `4.4.0`
++ Update to `th2-grpc-service-genrator` version `3.4.0`
++ Update to `grpcio-tools` version `1.56.0`
++ Update to `mypy-protobuf` version `3.4`
+
 ### 4.2.0
+
 + Update libraries versions.
 + Vulnerability check pipeline step.
 
 ### 4.1.0
+
 + Add stubs for Python
 + Update `th2-grpc-common` from `3.9.0` to `3.11.1`
 + Update `th2-grpc-service-generator` from `3.1.12` to `3.2.2`
 
 ### 4.0.0 
 + New param relation
 + Added new method 'getRelatedRules'
```

### Comparing `th2_grpc_sim-5.0.0.dev5552983537/setup.py` & `th2_grpc_sim-5.0.0.dev5554276200/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright 2020-2022 Exactpro (Exactpro Systems Limited)
+#   Copyright 2020-2023 Exactpro (Exactpro Systems Limited)
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -116,16 +116,16 @@
     long_description_content_type='text/markdown',
     author='TH2-devs',
     author_email='th2-devs@exactprosystems.com',
     url='https://github.com/th2-net/th2-grpc-sim',
     license='Apache License 2.0',
     python_requires='>=3.7',
     install_requires=[
-        'mypy-protobuf==3.2',
-        'grpcio-tools==1.50.0'
+        'mypy-protobuf==3.4',
+        'grpcio-tools==1.56.0'
     ],
     packages=packages,
     package_data=package_data,
     cmdclass={
         'generate': ProtoGenerator,
         'sdist': CustomDist
     }
```

### Comparing `th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim/sim.proto` & `th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim/sim.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim/sim_pb2_grpc.py` & `th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim/sim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim/sim_service.py` & `th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim/sim_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5552983537/th2_grpc_sim.egg-info/PKG-INFO` & `th2_grpc_sim-5.0.0.dev5554276200/th2_grpc_sim.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-sim
-Version: 5.0.0.dev5552983537
+Version: 5.0.0.dev5554276200
 Summary: th2_grpc_sim
 Home-page: https://github.com/th2-net/th2-grpc-sim
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim library
         
@@ -42,19 +42,28 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 5.1.0
+        
+        + Update to `th2-bom` version `4.4.0`
+        + Update to `th2-grpc-service-genrator` version `3.4.0`
+        + Update to `grpcio-tools` version `1.56.0`
+        + Update to `mypy-protobuf` version `3.4`
+        
         ### 4.2.0
+        
         + Update libraries versions.
         + Vulnerability check pipeline step.
         
         ### 4.1.0
+        
         + Add stubs for Python
         + Update `th2-grpc-common` from `3.9.0` to `3.11.1`
         + Update `th2-grpc-service-generator` from `3.1.12` to `3.2.2`
         
         ### 4.0.0 
         + New param relation
         + Added new method 'getRelatedRules'
```

