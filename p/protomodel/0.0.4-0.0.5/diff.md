# Comparing `tmp/protomodel-0.0.4.tar.gz` & `tmp/protomodel-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protomodel-0.0.4.tar", max compression
+gzip compressed data, was "protomodel-0.0.5.tar", max compression
```

## Comparing `protomodel-0.0.4.tar` & `protomodel-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0       84 2023-07-04 20:52:27.187402 protomodel-0.0.4/README.md
--rw-r--r--   0        0        0      107 2023-07-09 03:57:46.521399 protomodel-0.0.4/protomodel/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 04:40:34.047386 protomodel-0.0.4/protomodel/example/__init__.py
--rw-r--r--   0        0        0     2122 2023-07-14 18:08:55.612902 protomodel-0.0.4/protomodel/example/__pycache__/data.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-07-14 18:08:51.822900 protomodel-0.0.4/protomodel/example/data.py
--rw-r--r--   0        0        0      772 2023-07-14 15:57:15.072882 protomodel-0.0.4/protomodel/example/run.py
--rw-r--r--   0        0        0     1306 2023-07-14 18:03:37.762886 protomodel-0.0.4/protomodel/message.py
--rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.4/protomodel/protomodel/__init__.py
--rw-r--r--   0        0        0      174 2023-07-09 01:27:44.218963 protomodel-0.0.4/protomodel/protomodel/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      377 2023-07-04 21:40:33.867408 protomodel-0.0.4/protomodel/protomodel/__pycache__/grpc.cpython-311.pyc
--rw-r--r--   0        0        0     2361 2023-07-05 03:00:39.517398 protomodel-0.0.4/protomodel/protomodel/__pycache__/message.cpython-311.pyc
--rw-r--r--   0        0        0      384 2023-07-04 21:40:33.867408 protomodel-0.0.4/protomodel/protomodel/__pycache__/service.cpython-311.pyc
--rw-r--r--   0        0        0      402 2023-07-14 18:20:12.842905 protomodel-0.0.4/protomodel/rpc.py
--rw-r--r--   0        0        0     2019 2023-07-14 18:18:47.892907 protomodel-0.0.4/protomodel/service.py
--rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.4/protomodel/types/__init__.py
--rw-r--r--   0        0        0      218 2023-07-05 00:34:59.067411 protomodel-0.0.4/protomodel/types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      457 2023-07-05 18:44:19.157132 protomodel-0.0.4/protomodel/types/__pycache__/get_types.cpython-311.pyc
--rw-r--r--   0        0        0      247 2023-07-05 18:43:19.587132 protomodel-0.0.4/protomodel/types/get_types.py
--rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.4/protomodel/utils/__init__.py
--rw-r--r--   0        0        0      387 2023-07-14 18:21:56.762907 protomodel-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 protomodel-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       84 2023-07-04 20:52:27.187402 protomodel-0.0.5/README.md
+-rw-r--r--   0        0        0      107 2023-07-09 03:57:46.521399 protomodel-0.0.5/protomodel/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-14 18:51:06.762905 protomodel-0.0.5/protomodel/cli.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:40:34.047386 protomodel-0.0.5/protomodel/example/__init__.py
+-rw-r--r--   0        0        0     2122 2023-07-14 18:08:55.612902 protomodel-0.0.5/protomodel/example/__pycache__/data.cpython-311.pyc
+-rw-r--r--   0        0        0     1282 2023-07-14 18:39:14.212894 protomodel-0.0.5/protomodel/example/__pycache__/hello.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-07-14 18:08:51.822900 protomodel-0.0.5/protomodel/example/data.py
+-rw-r--r--   0        0        0      243 2023-07-14 18:33:34.502888 protomodel-0.0.5/protomodel/example/hello.py
+-rw-r--r--   0        0        0      862 2023-07-14 18:44:40.902897 protomodel-0.0.5/protomodel/example/run.py
+-rw-r--r--   0        0        0     1306 2023-07-14 18:03:37.762886 protomodel-0.0.5/protomodel/message.py
+-rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.5/protomodel/protomodel/__init__.py
+-rw-r--r--   0        0        0      174 2023-07-09 01:27:44.218963 protomodel-0.0.5/protomodel/protomodel/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      377 2023-07-04 21:40:33.867408 protomodel-0.0.5/protomodel/protomodel/__pycache__/grpc.cpython-311.pyc
+-rw-r--r--   0        0        0     2361 2023-07-05 03:00:39.517398 protomodel-0.0.5/protomodel/protomodel/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0        0        0      384 2023-07-04 21:40:33.867408 protomodel-0.0.5/protomodel/protomodel/__pycache__/service.cpython-311.pyc
+-rw-r--r--   0        0        0      402 2023-07-14 18:20:12.842905 protomodel-0.0.5/protomodel/rpc.py
+-rw-r--r--   0        0        0     2019 2023-07-14 18:18:47.892907 protomodel-0.0.5/protomodel/service.py
+-rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.5/protomodel/types/__init__.py
+-rw-r--r--   0        0        0      218 2023-07-05 00:34:59.067411 protomodel-0.0.5/protomodel/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      457 2023-07-05 18:44:19.157132 protomodel-0.0.5/protomodel/types/__pycache__/get_types.cpython-311.pyc
+-rw-r--r--   0        0        0      247 2023-07-05 18:43:19.587132 protomodel-0.0.5/protomodel/types/get_types.py
+-rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.5/protomodel/utils/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-14 18:57:56.192904 protomodel-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 protomodel-0.0.5/PKG-INFO
```

### Comparing `protomodel-0.0.4/protomodel/example/__pycache__/data.cpython-311.pyc` & `protomodel-0.0.5/protomodel/example/__pycache__/data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `protomodel-0.0.4/protomodel/message.py` & `protomodel-0.0.5/protomodel/message.py`

 * *Files identical despite different names*

### Comparing `protomodel-0.0.4/protomodel/protomodel/__pycache__/message.cpython-311.pyc` & `protomodel-0.0.5/protomodel/protomodel/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `protomodel-0.0.4/protomodel/service.py` & `protomodel-0.0.5/protomodel/service.py`

 * *Files identical despite different names*

