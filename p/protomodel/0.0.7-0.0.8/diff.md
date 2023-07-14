# Comparing `tmp/protomodel-0.0.7.tar.gz` & `tmp/protomodel-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protomodel-0.0.7.tar", max compression
+gzip compressed data, was "protomodel-0.0.8.tar", max compression
```

## Comparing `protomodel-0.0.7.tar` & `protomodel-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      843 2023-07-14 19:45:21.892900 protomodel-0.0.7/README.md
--rw-r--r--   0        0        0      107 2023-07-09 03:57:46.521399 protomodel-0.0.7/protomodel/__init__.py
--rw-r--r--   0        0        0     1223 2023-07-14 19:30:08.222905 protomodel-0.0.7/protomodel/__main__.py
--rw-r--r--   0        0        0        0 2023-07-05 04:40:34.047386 protomodel-0.0.7/protomodel/example/__init__.py
--rw-r--r--   0        0        0      504 2023-07-14 18:08:51.822900 protomodel-0.0.7/protomodel/example/data.py
--rw-r--r--   0        0        0      243 2023-07-14 19:31:05.512889 protomodel-0.0.7/protomodel/hello.py
--rw-r--r--   0        0        0     1306 2023-07-14 18:03:37.762886 protomodel-0.0.7/protomodel/message.py
--rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.7/protomodel/protomodel-cli/__init__.py
--rw-r--r--   0        0        0      155 2023-07-14 18:51:06.762905 protomodel-0.0.7/protomodel/protomodel-cli/cli.py
--rw-r--r--   0        0        0      402 2023-07-14 18:20:12.842905 protomodel-0.0.7/protomodel/rpc.py
--rw-r--r--   0        0        0     2019 2023-07-14 18:18:47.892907 protomodel-0.0.7/protomodel/service.py
--rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.7/protomodel/types/__init__.py
--rw-r--r--   0        0        0      247 2023-07-05 18:43:19.587132 protomodel-0.0.7/protomodel/types/get_types.py
--rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.7/protomodel/utils/__init__.py
--rw-r--r--   0        0        0      466 2023-07-14 20:08:26.402893 protomodel-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1249 1970-01-01 00:00:00.000000 protomodel-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1229 2023-07-14 21:32:02.952890 protomodel-0.0.8/README.md
+-rw-r--r--   0        0        0      107 2023-07-09 03:57:46.521399 protomodel-0.0.8/protomodel/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-14 19:30:08.222905 protomodel-0.0.8/protomodel/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:40:34.047386 protomodel-0.0.8/protomodel/example/__init__.py
+-rw-r--r--   0        0        0      504 2023-07-14 18:08:51.822900 protomodel-0.0.8/protomodel/example/data.py
+-rw-r--r--   0        0        0      243 2023-07-14 19:31:05.512889 protomodel-0.0.8/protomodel/hello.py
+-rw-r--r--   0        0        0     1306 2023-07-14 18:03:37.762886 protomodel-0.0.8/protomodel/message.py
+-rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.8/protomodel/protomodel-cli/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-14 18:51:06.762905 protomodel-0.0.8/protomodel/protomodel-cli/cli.py
+-rw-r--r--   0        0        0      402 2023-07-14 18:20:12.842905 protomodel-0.0.8/protomodel/rpc.py
+-rw-r--r--   0        0        0     2019 2023-07-14 18:18:47.892907 protomodel-0.0.8/protomodel/service.py
+-rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.8/protomodel/types/__init__.py
+-rw-r--r--   0        0        0      247 2023-07-05 18:43:19.587132 protomodel-0.0.8/protomodel/types/get_types.py
+-rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.8/protomodel/utils/__init__.py
+-rw-r--r--   0        0        0      466 2023-07-14 21:32:02.952890 protomodel-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1635 1970-01-01 00:00:00.000000 protomodel-0.0.8/PKG-INFO
```

### Comparing `protomodel-0.0.7/README.md` & `protomodel-0.0.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: protomodel
+Version: 0.0.8
+Summary: Python Library to generate protobuffers code from python using type hints
+Author: Pablo España
+Author-email: pabloespanab@outlook.com
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.5,<9.0.0)
+Description-Content-Type: text/markdown
+
 
 
 # Protomodel
 Python Library to generate proto buffer code from python using type hints
 
 ## Example
 Generate a file hello.py and add the following code:
@@ -18,15 +30,15 @@
     message: str
 
 @service
 class Greeter:
 
     @rpc
     def say_hello(hello_request: HelloRequest) -> HelloReply:
-        ...
+        pass
 
 ```
 
 ## Generate file
 
 Run the following command to generate a proto buffer file
 ```bash
@@ -47,8 +59,38 @@
 message HelloReply {
   string message = 1;
 }
 
 service Greeter {
   rpc SayHello (HelloRequest) returns (HelloReply) {}
 }
-```
+```
+
+## Adding another types
+```python
+@message
+class Item:
+    id: int
+    name: str
+    description: str
+    price: float
+    enabled: bool
+
+@message
+class ItemsList:
+    items: list[Item]
+```
+
+### Result:
+```proto
+message Item {
+  int32 id = 1;
+  string name = 2;
+  string description = 3;
+  double price = 4;
+  bool enabled = 5;
+}
+
+message ItemsList {
+  repeated Item items = 1;
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `protomodel-0.0.7/protomodel/__main__.py` & `protomodel-0.0.8/protomodel/__main__.py`

 * *Files identical despite different names*

### Comparing `protomodel-0.0.7/protomodel/message.py` & `protomodel-0.0.8/protomodel/message.py`

 * *Files identical despite different names*

### Comparing `protomodel-0.0.7/protomodel/service.py` & `protomodel-0.0.8/protomodel/service.py`

 * *Files identical despite different names*

