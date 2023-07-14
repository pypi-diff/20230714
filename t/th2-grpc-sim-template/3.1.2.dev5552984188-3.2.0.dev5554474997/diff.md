# Comparing `tmp/th2_grpc_sim_template-3.1.2.dev5552984188.tar.gz` & `tmp/th2_grpc_sim_template-3.2.0.dev5554474997.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_sim_template-3.1.2.dev5552984188.tar", last modified: Fri Jul 14 10:13:20 2023, max compression
+gzip compressed data, was "dist/th2_grpc_sim_template-3.2.0.dev5554474997.tar", last modified: Fri Jul 14 13:13:24 2023, max compression
```

## Comparing `th2_grpc_sim_template-3.1.2.dev5552984188.tar` & `th2_grpc_sim_template-3.2.0.dev5554474997.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/
--rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-07-14 10:12:33.000000 th2_grpc_sim_template-3.1.2.dev5552984188/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-14 10:12:34.000000 th2_grpc_sim_template-3.1.2.dev5552984188/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4376 2023-07-14 10:12:33.000000 th2_grpc_sim_template-3.1.2.dev5552984188/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-14 10:12:33.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template.proto
--rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     6063 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-07-14 10:12:58.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-14 10:13:20.000000 th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/
+-rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-07-14 13:12:26.000000 th2_grpc_sim_template-3.2.0.dev5554474997/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-14 13:12:26.000000 th2_grpc_sim_template-3.2.0.dev5554474997/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4600 2023-07-14 13:12:26.000000 th2_grpc_sim_template-3.2.0.dev5554474997/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-14 13:12:26.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2295 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     6063 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-14 13:13:03.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/top_level.txt
```

### Comparing `th2_grpc_sim_template-3.1.2.dev5552984188/PKG-INFO` & `th2_grpc_sim_template-3.2.0.dev5554474997/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_sim_template
-Version: 3.1.2.dev5552984188
+Version: 3.2.0.dev5554474997
 Summary: th2_grpc_sim_template
 Home-page: https://github.com/th2-net/th2-grpc-sim-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim template library
         
@@ -42,12 +42,21 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 3.2.0
+        
+        + Update to `th2-bom` version `4.4.0`
+        + Update to `grpc-sim` version `5.1.0`
+        + Update to `grpc-common` version `4.3.0`
+        + Update to `th2-grpc-service-genrator` version `3.4.0`
+        + Update to `grpcio-tools` version `1.56.0`
+        
         ### 3.1.2
+        
         + Update libraries versions.
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `th2_grpc_sim_template-3.1.2.dev5552984188/README.md` & `th2_grpc_sim_template-3.2.0.dev5554474997/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,9 +34,18 @@
     python setup.py sdist
     twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
     ```
    `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
 
 ## Release notes
 
+### 3.2.0
+
++ Update to `th2-bom` version `4.4.0`
++ Update to `grpc-sim` version `5.1.0`
++ Update to `grpc-common` version `4.3.0`
++ Update to `th2-grpc-service-genrator` version `3.4.0`
++ Update to `grpcio-tools` version `1.56.0`
+
 ### 3.1.2
+
 + Update libraries versions.
```

### Comparing `th2_grpc_sim_template-3.1.2.dev5552984188/setup.py` & `th2_grpc_sim_template-3.2.0.dev5554474997/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright 2020-2021 Exactpro (Exactpro Systems Limited)
+#   Copyright 2020-2023 Exactpro (Exactpro Systems Limited)
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -34,15 +34,15 @@
         self.strict_mode = False
 
     def finalize_options(self):
         pass
 
     def run(self):
         proto_path = os.path.abspath('src/main/proto')
-        gen_path = os.path.abspath('src/gen/main/python')
+        gen_path = os.path.abspath('build/generated/source/proto/main/services/python')
 
         if not os.path.exists(gen_path):
             os.makedirs(gen_path)
 
         proto_files = []
         for root, _, files in os.walk(proto_path):
             for filename in files:
@@ -54,42 +54,44 @@
                          [f'--proto_path={resource_filename(x[0], x[1])}' for x in protos] + \
                          [f'--proto_path={get_python_lib()}']
 
         from grpc_tools import protoc
         for proto_file in proto_files:
             command = ['grpc_tools.protoc'] + \
                       protos_include + \
-                      ['--python_out={}'.format(gen_path), '--grpc_python_out={}'.format(gen_path)] + \
+                      [f'--python_out={gen_path}', f'--grpc_python_out={gen_path}'] + \
+                      [f'--mypy_out={gen_path}'] + \
                       [proto_file]
 
             if protoc.main(command) != 0:
                 if self.strict_mode:
                     raise Exception(f'error: {command} failed')
 
 
 class CustomDist(sdist):
 
     def run(self):
         copy_tree(f'src/main/proto/{package_name}', package_name)
 
-        copy_tree(f'src/gen/main/python/{package_name}', package_name)
-        copy_tree(f'src/gen/main/services/python/{package_name}', package_name)
+        copy_tree(f'build/generated/source/proto/main/services/python/{package_name}', package_name)
         Path(f'{package_name}/__init__.py').touch()
+        Path(f'{package_name}/py.typed').touch()
 
         def make_packages(root_dir):
             for path in Path(root_dir).iterdir():
                 if path.is_dir():
                     path.joinpath('__init__.py').touch()
                     make_packages(path)
 
         make_packages(package_name)
 
         self.distribution.packages = [''] + find_packages(include=[package_name, f'{package_name}.*'])
         self.distribution.package_data = {'': ['package_info.json'],
-                                          **dict.fromkeys(self.distribution.packages[1:], ['*.proto'])}
+                                          **dict.fromkeys(self.distribution.packages[1:],
+                                                          ['*.proto', 'py.typed', '*.pyi'])}
 
         sdist.run(self)
 
         rmtree(package_name, ignore_errors=True)
 
 
 with open('package_info.json', 'r') as file:
@@ -98,31 +100,33 @@
 package_name = package_info['package_name'].replace('-', '_')
 package_version = package_info['package_version']
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 packages = [''] + find_packages(include=[package_name, f'{package_name}.*'])
-package_data = {'': ['package_info.json'], **dict.fromkeys(packages[1:], ['*.proto'])}
+package_data = {'': ['package_info.json'],
+                **dict.fromkeys(packages[1:], ['*.proto', 'py.typed', '*.pyi'])}
 
 
 setup(
     name=package_name,
     version=package_version,
     description=package_name,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='TH2-devs',
     author_email='th2-devs@exactprosystems.com',
     url='https://github.com/th2-net/th2-grpc-sim-template',
     license='Apache License 2.0',
     python_requires='>=3.7',
     install_requires=[
-        'th2-grpc-sim~=3.1.3',
-        'grpcio-tools==1.38.1'
+        'th2-grpc-sim~=5.1.0.dev',
+        'th2-grpc-common~=4.3.0.dev',
+        'grpcio-tools==1.56.0'
     ],
     packages=packages,
     package_data=package_data,
     cmdclass={
         'generate': ProtoGenerator,
         'sdist': CustomDist
     }
```

### Comparing `th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template.proto` & `th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template_pb2_grpc.py` & `th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template/sim_template_service.py` & `th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from . import sim_template_pb2_grpc as importStub
 
 class SimTemplateService(object):
 
     def __init__(self, router):
         self.connector = router.get_connection(SimTemplateService, importStub.SimTemplateStub)
 
-    def createRuleFixSecurity(self, request, timeout=None):
-        return self.connector.create_request('createRuleFixSecurity', request, timeout)
+    def createRuleFixSecurity(self, request, timeout=None, properties=None):
+        return self.connector.create_request('createRuleFixSecurity', request, timeout, properties)
 
-    def createDemoRule(self, request, timeout=None):
-        return self.connector.create_request('createDemoRule', request, timeout)
+    def createDemoRule(self, request, timeout=None, properties=None):
+        return self.connector.create_request('createDemoRule', request, timeout, properties)
 
-    def createRuleFix(self, request, timeout=None):
-        return self.connector.create_request('createRuleFix', request, timeout)
+    def createRuleFix(self, request, timeout=None, properties=None):
+        return self.connector.create_request('createRuleFix', request, timeout, properties)
```

### Comparing `th2_grpc_sim_template-3.1.2.dev5552984188/th2_grpc_sim_template.egg-info/PKG-INFO` & `th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-sim-template
-Version: 3.1.2.dev5552984188
+Version: 3.2.0.dev5554474997
 Summary: th2_grpc_sim_template
 Home-page: https://github.com/th2-net/th2-grpc-sim-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim template library
         
@@ -42,12 +42,21 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 3.2.0
+        
+        + Update to `th2-bom` version `4.4.0`
+        + Update to `grpc-sim` version `5.1.0`
+        + Update to `grpc-common` version `4.3.0`
+        + Update to `th2-grpc-service-genrator` version `3.4.0`
+        + Update to `grpcio-tools` version `1.56.0`
+        
         ### 3.1.2
+        
         + Update libraries versions.
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

