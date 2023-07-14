# Comparing `tmp/protomodel-0.0.3.tar.gz` & `tmp/protomodel-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protomodel-0.0.3.tar", max compression
+gzip compressed data, was "protomodel-0.0.4.tar", max compression
```

## Comparing `protomodel-0.0.3.tar` & `protomodel-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0       84 2023-07-04 20:52:27.187402 protomodel-0.0.3/README.md
--rw-r--r--   0        0        0      107 2023-07-09 03:57:46.521399 protomodel-0.0.3/protomodel/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 04:40:34.047386 protomodel-0.0.3/protomodel/example/__init__.py
--rw-r--r--   0        0        0      348 2023-07-05 18:47:04.977144 protomodel-0.0.3/protomodel/example/data.py
--rw-r--r--   0        0        0      584 2023-07-09 03:00:20.241381 protomodel-0.0.3/protomodel/example/run.py
--rw-r--r--   0        0        0     1306 2023-07-09 03:57:31.021375 protomodel-0.0.3/protomodel/message.py
--rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.3/protomodel/protomodel/__init__.py
--rw-r--r--   0        0        0       22 2023-07-09 03:57:46.521399 protomodel-0.0.3/protomodel/rpc.py
--rw-r--r--   0        0        0       25 2023-07-05 03:07:52.257387 protomodel-0.0.3/protomodel/service.py
--rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.3/protomodel/types/__init__.py
--rw-r--r--   0        0        0      247 2023-07-05 18:43:19.587132 protomodel-0.0.3/protomodel/types/get_types.py
--rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.3/protomodel/utils/__init__.py
--rw-r--r--   0        0        0      387 2023-07-09 03:58:23.321417 protomodel-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 protomodel-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       84 2023-07-04 20:52:27.187402 protomodel-0.0.4/README.md
+-rw-r--r--   0        0        0      107 2023-07-09 03:57:46.521399 protomodel-0.0.4/protomodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:40:34.047386 protomodel-0.0.4/protomodel/example/__init__.py
+-rw-r--r--   0        0        0     2122 2023-07-14 18:08:55.612902 protomodel-0.0.4/protomodel/example/__pycache__/data.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-07-14 18:08:51.822900 protomodel-0.0.4/protomodel/example/data.py
+-rw-r--r--   0        0        0      772 2023-07-14 15:57:15.072882 protomodel-0.0.4/protomodel/example/run.py
+-rw-r--r--   0        0        0     1306 2023-07-14 18:03:37.762886 protomodel-0.0.4/protomodel/message.py
+-rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.4/protomodel/protomodel/__init__.py
+-rw-r--r--   0        0        0      174 2023-07-09 01:27:44.218963 protomodel-0.0.4/protomodel/protomodel/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      377 2023-07-04 21:40:33.867408 protomodel-0.0.4/protomodel/protomodel/__pycache__/grpc.cpython-311.pyc
+-rw-r--r--   0        0        0     2361 2023-07-05 03:00:39.517398 protomodel-0.0.4/protomodel/protomodel/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0        0        0      384 2023-07-04 21:40:33.867408 protomodel-0.0.4/protomodel/protomodel/__pycache__/service.cpython-311.pyc
+-rw-r--r--   0        0        0      402 2023-07-14 18:20:12.842905 protomodel-0.0.4/protomodel/rpc.py
+-rw-r--r--   0        0        0     2019 2023-07-14 18:18:47.892907 protomodel-0.0.4/protomodel/service.py
+-rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.4/protomodel/types/__init__.py
+-rw-r--r--   0        0        0      218 2023-07-05 00:34:59.067411 protomodel-0.0.4/protomodel/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      457 2023-07-05 18:44:19.157132 protomodel-0.0.4/protomodel/types/__pycache__/get_types.cpython-311.pyc
+-rw-r--r--   0        0        0      247 2023-07-05 18:43:19.587132 protomodel-0.0.4/protomodel/types/get_types.py
+-rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.4/protomodel/utils/__init__.py
+-rw-r--r--   0        0        0      387 2023-07-14 18:21:56.762907 protomodel-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 protomodel-0.0.4/PKG-INFO
```

### Comparing `protomodel-0.0.3/protomodel/example/run.py` & `protomodel-0.0.4/protomodel/example/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import data
 from protomodel import message, service, rpc
 from typing import TextIO, List, Type, Any
 
 input_filename = "data.py"
 output_filename = "data.proto"
+package_name = "app.proto"
     
 proto_file: TextIO = open(f"./{output_filename}", "w")
-proto_file.write('syntax = "proto3";\n\npackage app.proto;\n\n')
+proto_file.write(f'syntax = "proto3";\n\npackage {package_name};\n\n')
 
 # global_symbols = globals()
 # messages = [cls for cls in global_symbols.values() if isinstance(cls, message)]
 messages: List[message] = [cls for cls in data.__dict__.values() if isinstance(cls, message)]
+services: List[service] = [cls for cls in data.__dict__.values() if isinstance(cls, service)]
+
 
 for msg in messages:
     msg.add_field(proto_file)
 
+for service in services:
+    service.add_field(proto_file)
+
 print('file created.')
 proto_file.close()
```

### Comparing `protomodel-0.0.3/protomodel/message.py` & `protomodel-0.0.4/protomodel/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def add_field(self, file: TextIO) -> None:
         file.write(f"{self.__class__.__name__.lower()} {self.message_model.__name__} {{\n")
         annotations = self.message_model.__annotations__
 
         for index, field in enumerate(annotations, 1):
             annotation: Type[Any] = annotations[field]
             field_type: str = self.__get_type_string(annotation)
-            file.write(f"\t{field_type} {field} = {index};\n")
+            file.write(f"  {field_type} {field} = {index};\n")
 
         file.write(f"}}\n\n")
 
     def __get_type_string(self, annotation: Type[Any]) -> str:
         if hasattr(annotation, "__origin__") and annotation.__origin__ in [List, list]:
             return f"{get_types(annotation.__name__)} {annotation.__args__[0].message_model.__name__}"
         try:
```

