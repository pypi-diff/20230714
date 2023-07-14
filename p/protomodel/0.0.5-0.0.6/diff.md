# Comparing `tmp/protomodel-0.0.5.tar.gz` & `tmp/protomodel-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protomodel-0.0.5.tar", max compression
+gzip compressed data, was "protomodel-0.0.6.tar", max compression
```

## Comparing `protomodel-0.0.5.tar` & `protomodel-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,16 @@
--rw-r--r--   0        0        0       84 2023-07-04 20:52:27.187402 protomodel-0.0.5/README.md
--rw-r--r--   0        0        0      107 2023-07-09 03:57:46.521399 protomodel-0.0.5/protomodel/__init__.py
--rw-r--r--   0        0        0      155 2023-07-14 18:51:06.762905 protomodel-0.0.5/protomodel/cli.py
--rw-r--r--   0        0        0        0 2023-07-05 04:40:34.047386 protomodel-0.0.5/protomodel/example/__init__.py
--rw-r--r--   0        0        0     2122 2023-07-14 18:08:55.612902 protomodel-0.0.5/protomodel/example/__pycache__/data.cpython-311.pyc
--rw-r--r--   0        0        0     1282 2023-07-14 18:39:14.212894 protomodel-0.0.5/protomodel/example/__pycache__/hello.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-07-14 18:08:51.822900 protomodel-0.0.5/protomodel/example/data.py
--rw-r--r--   0        0        0      243 2023-07-14 18:33:34.502888 protomodel-0.0.5/protomodel/example/hello.py
--rw-r--r--   0        0        0      862 2023-07-14 18:44:40.902897 protomodel-0.0.5/protomodel/example/run.py
--rw-r--r--   0        0        0     1306 2023-07-14 18:03:37.762886 protomodel-0.0.5/protomodel/message.py
--rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.5/protomodel/protomodel/__init__.py
--rw-r--r--   0        0        0      174 2023-07-09 01:27:44.218963 protomodel-0.0.5/protomodel/protomodel/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      377 2023-07-04 21:40:33.867408 protomodel-0.0.5/protomodel/protomodel/__pycache__/grpc.cpython-311.pyc
--rw-r--r--   0        0        0     2361 2023-07-05 03:00:39.517398 protomodel-0.0.5/protomodel/protomodel/__pycache__/message.cpython-311.pyc
--rw-r--r--   0        0        0      384 2023-07-04 21:40:33.867408 protomodel-0.0.5/protomodel/protomodel/__pycache__/service.cpython-311.pyc
--rw-r--r--   0        0        0      402 2023-07-14 18:20:12.842905 protomodel-0.0.5/protomodel/rpc.py
--rw-r--r--   0        0        0     2019 2023-07-14 18:18:47.892907 protomodel-0.0.5/protomodel/service.py
--rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.5/protomodel/types/__init__.py
--rw-r--r--   0        0        0      218 2023-07-05 00:34:59.067411 protomodel-0.0.5/protomodel/types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      457 2023-07-05 18:44:19.157132 protomodel-0.0.5/protomodel/types/__pycache__/get_types.cpython-311.pyc
--rw-r--r--   0        0        0      247 2023-07-05 18:43:19.587132 protomodel-0.0.5/protomodel/types/get_types.py
--rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.5/protomodel/utils/__init__.py
--rw-r--r--   0        0        0      460 2023-07-14 18:57:56.192904 protomodel-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 protomodel-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      843 2023-07-14 19:45:21.892900 protomodel-0.0.6/README.md
+-rw-r--r--   0        0        0      107 2023-07-09 03:57:46.521399 protomodel-0.0.6/protomodel/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-14 19:30:08.222905 protomodel-0.0.6/protomodel/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:40:34.047386 protomodel-0.0.6/protomodel/example/__init__.py
+-rw-r--r--   0        0        0      504 2023-07-14 18:08:51.822900 protomodel-0.0.6/protomodel/example/data.py
+-rw-r--r--   0        0        0      243 2023-07-14 19:31:05.512889 protomodel-0.0.6/protomodel/hello.py
+-rw-r--r--   0        0        0     1306 2023-07-14 18:03:37.762886 protomodel-0.0.6/protomodel/message.py
+-rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.6/protomodel/protomodel-cli/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-14 18:51:06.762905 protomodel-0.0.6/protomodel/protomodel-cli/cli.py
+-rw-r--r--   0        0        0      402 2023-07-14 18:20:12.842905 protomodel-0.0.6/protomodel/rpc.py
+-rw-r--r--   0        0        0     2019 2023-07-14 18:18:47.892907 protomodel-0.0.6/protomodel/service.py
+-rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.6/protomodel/types/__init__.py
+-rw-r--r--   0        0        0      247 2023-07-05 18:43:19.587132 protomodel-0.0.6/protomodel/types/get_types.py
+-rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.6/protomodel/utils/__init__.py
+-rw-r--r--   0        0        0      475 2023-07-14 19:44:37.422895 protomodel-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1249 1970-01-01 00:00:00.000000 protomodel-0.0.6/PKG-INFO
```

### Comparing `protomodel-0.0.5/protomodel/example/run.py` & `protomodel-0.0.6/protomodel/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,39 @@
-import importlib.util
-from protomodel import message, service
-from typing import TextIO, List
+import click
+import  importlib.util
 
-input_filename = "hello.py"
-output_filename = "data.proto"
-package_name = "app.proto"
+@click.group()
+def cli():
+    pass
 
-data_spec = importlib.util.spec_from_file_location(input_filename.split(".")[0], input_filename)
-data_module = importlib.util.module_from_spec(data_spec)
-data_spec.loader.exec_module(data_module)
+@cli.command()
+@click.option('--python_file', help='Python file name with directory.')
+@click.option('--proto_name', help='Proto buffer file name with directory.')
+def generate(python_file, proto_name):
+    from protomodel import message, service
+    from typing import TextIO, List
 
-proto_file: TextIO = open(f"./{output_filename}", "w")
-proto_file.write(f'syntax = "proto3";\n\npackage {package_name};\n\n')
+    input_filename = python_file
+    output_filename = proto_name
+    package_name = "app.proto"
 
-messages: List[message] = [cls for cls in data_module.__dict__.values() if isinstance(cls, message)]
-services: List[service] = [cls for cls in data_module.__dict__.values() if isinstance(cls, service)]
+    data_spec = importlib.util.spec_from_file_location(input_filename.split(".")[0], input_filename)
+    data_module = importlib.util.module_from_spec(data_spec)
+    data_spec.loader.exec_module(data_module)
 
-for msg in messages:
-    msg.add_field(proto_file)
+    proto_file: TextIO = open(f"{output_filename}", "w")
+    proto_file.write(f'syntax = "proto3";\n\npackage {package_name};\n\n')
 
-for service in services:
-    service.add_field(proto_file)
+    messages: List[message] = [cls for cls in data_module.__dict__.values() if isinstance(cls, message)]
+    services: List[service] = [cls for cls in data_module.__dict__.values() if isinstance(cls, service)]
 
-print('file created.')
-proto_file.close()
+    for msg in messages:
+        msg.add_field(proto_file)
+
+    for service in services:
+        service.add_field(proto_file)
+
+    print('file created.')
+    proto_file.close()
+
+if __name__ == "__main__":
+    cli()
```

### Comparing `protomodel-0.0.5/protomodel/message.py` & `protomodel-0.0.6/protomodel/message.py`

 * *Files identical despite different names*

### Comparing `protomodel-0.0.5/protomodel/service.py` & `protomodel-0.0.6/protomodel/service.py`

 * *Files identical despite different names*

