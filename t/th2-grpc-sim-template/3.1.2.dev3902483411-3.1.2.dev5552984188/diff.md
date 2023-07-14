# Comparing `tmp/th2_grpc_sim_template-3.1.2.dev3902483411.tar.gz` & `tmp/th2_grpc_sim_template-3.1.2.dev5552984188.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_sim_template-3.1.2.dev3902483411.tar", last modified: Thu Jan 12 13:02:28 2023, max compression
+gzip compressed data, was "dist/th2_grpc_sim_template-3.1.2.dev5552984188.tar", last modified: Fri Jul 14 10:13:20 2023, max compression
```

## Comparing `th2_grpc_sim_template-3.1.2.dev3902483411.tar` & `th2_grpc_sim_template-3.1.2.dev5552984188.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-12 13:02:28.000000 th2_grpc_sim_template-3.1.2.dev3902483411/
--rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-01-12 13:02:28.000000 th2_grpc_sim_template-3.1.2.dev3902483411/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-01-12 13:01:45.000000 th2_grpc_sim_template-3.1.2.dev3902483411/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-01-12 13:01:45.000000 th2_grpc_sim_template-3.1.2.dev3902483411/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-12 13:02:28.000000 th2_grpc_sim_template-3.1.2.dev3902483411/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4376 2023-01-12 13:01:45.000000 th2_grpc_sim_template-3.1.2.dev3902483411/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-12 13:02:28.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-12 13:02:27.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-01-12 13:01:45.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template/sim_template.proto
--rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-01-12 13:02:27.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template/sim_template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     6063 2023-01-12 13:02:27.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template/sim_template_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-01-12 13:02:10.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template/sim_template_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-12 13:02:28.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-01-12 13:02:27.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-01-12 13:02:27.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-12 13:02:27.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-01-12 13:02:27.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-01-12 13:02:27.000000 th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/
+-rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-07-14 10:12:33.000000 th2_grpc_sim_template-3.1.2.dev5552984188/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-14 10:12:34.000000 th2_grpc_sim_template-3.1.2.dev5552984188/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4376 2023-07-14 10:12:33.000000 th2_grpc_sim_template-3.1.2.dev5552984188/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-14 10:12:33.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6063 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-07-14 10:12:58.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/top_level.txt
```

### Comparing `th2_grpc_sim_template-3.1.2.dev3902483411/PKG-INFO` & `th2_grpc_sim_template-3.1.2.dev5552984188/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_sim_template
-Version: 3.1.2.dev3902483411
+Version: 3.1.2.dev5552984188
 Summary: th2_grpc_sim_template
 Home-page: https://github.com/th2-net/th2-grpc-sim-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim template library
```

### Comparing `th2_grpc_sim_template-3.1.2.dev3902483411/README.md` & `th2_grpc_sim_template-3.1.2.dev5552984188/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.1.2.dev3902483411/setup.py` & `th2_grpc_sim_template-3.1.2.dev5552984188/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template/sim_template.proto` & `th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template/sim_template_pb2.py` & `th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template/sim_template_pb2_grpc.py` & `th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template/sim_template_service.py` & `th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.1.2.dev3902483411/th2_grpc_sim_template.egg-info/PKG-INFO` & `th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-sim-template
-Version: 3.1.2.dev3902483411
+Version: 3.1.2.dev5552984188
 Summary: th2_grpc_sim_template
 Home-page: https://github.com/th2-net/th2-grpc-sim-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim template library
```

