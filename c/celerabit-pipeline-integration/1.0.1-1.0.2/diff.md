# Comparing `tmp/celerabit-pipeline-integration-1.0.1.tar.gz` & `tmp/celerabit-pipeline-integration-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celerabit-pipeline-integration-1.0.1.tar", last modified: Thu Jul 13 17:48:25 2023, max compression
+gzip compressed data, was "celerabit-pipeline-integration-1.0.2.tar", last modified: Fri Jul 14 12:01:37 2023, max compression
```

## Comparing `celerabit-pipeline-integration-1.0.1.tar` & `celerabit-pipeline-integration-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-07-13 17:48:25.441534 celerabit-pipeline-integration-1.0.1/
--rw-r--r--   0 raul.devilla   (501) staff       (20)      553 2023-07-10 22:13:20.000000 celerabit-pipeline-integration-1.0.1/LICENCE
--rw-r--r--   0 raul.devilla   (501) staff       (20)     6145 2023-07-13 17:48:25.441383 celerabit-pipeline-integration-1.0.1/PKG-INFO
--rw-r--r--   0 raul.devilla   (501) staff       (20)     5661 2023-07-10 19:56:31.000000 celerabit-pipeline-integration-1.0.1/README.md
-drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-07-13 17:48:25.441198 celerabit-pipeline-integration-1.0.1/celerabit_pipeline_integration.egg-info/
--rw-r--r--   0 raul.devilla   (501) staff       (20)     6145 2023-07-13 17:48:25.000000 celerabit-pipeline-integration-1.0.1/celerabit_pipeline_integration.egg-info/PKG-INFO
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1001 2023-07-13 17:48:25.000000 celerabit-pipeline-integration-1.0.1/celerabit_pipeline_integration.egg-info/SOURCES.txt
--rw-r--r--   0 raul.devilla   (501) staff       (20)        1 2023-07-13 17:48:25.000000 celerabit-pipeline-integration-1.0.1/celerabit_pipeline_integration.egg-info/dependency_links.txt
--rw-r--r--   0 raul.devilla   (501) staff       (20)       17 2023-07-13 17:48:25.000000 celerabit-pipeline-integration-1.0.1/celerabit_pipeline_integration.egg-info/requires.txt
--rw-r--r--   0 raul.devilla   (501) staff       (20)       29 2023-07-13 17:48:25.000000 celerabit-pipeline-integration-1.0.1/celerabit_pipeline_integration.egg-info/top_level.txt
-drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-07-13 17:48:25.440404 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/
--rw-r--r--   0 raul.devilla   (501) staff       (20)      789 2023-07-10 19:55:45.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/__init__.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      187 2023-07-10 19:55:37.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/__main__.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     6989 2023-07-10 19:55:39.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/int_main_module.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      174 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/model_credentials.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     2365 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/model_execution_params.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)       69 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/model_job.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1471 2023-07-10 19:58:17.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/uc_authenticator.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     3867 2023-07-10 19:59:44.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/uc_scenario_runner.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1536 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/util_compliance_evaluator.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1509 2023-07-10 20:07:23.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/util_configuration.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      397 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/util_http.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1143 2023-07-10 20:07:46.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/util_http_client.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      134 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/util_json.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)     1232 2023-07-10 19:56:04.000000 celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/util_logger.py
--rw-r--r--   0 raul.devilla   (501) staff       (20)      153 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.1/pyproject.toml
--rw-r--r--   0 raul.devilla   (501) staff       (20)       38 2023-07-13 17:48:25.441573 celerabit-pipeline-integration-1.0.1/setup.cfg
--rw-r--r--   0 raul.devilla   (501) staff       (20)      852 2023-07-10 19:55:48.000000 celerabit-pipeline-integration-1.0.1/setup.py
+drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-07-14 12:01:37.414410 celerabit-pipeline-integration-1.0.2/
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      553 2023-07-10 22:13:20.000000 celerabit-pipeline-integration-1.0.2/LICENCE
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     6145 2023-07-14 12:01:37.414206 celerabit-pipeline-integration-1.0.2/PKG-INFO
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     5661 2023-07-10 19:56:31.000000 celerabit-pipeline-integration-1.0.2/README.md
+drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-07-14 12:01:37.414003 celerabit-pipeline-integration-1.0.2/celerabit_pipeline_integration.egg-info/
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     6145 2023-07-14 12:01:37.000000 celerabit-pipeline-integration-1.0.2/celerabit_pipeline_integration.egg-info/PKG-INFO
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1001 2023-07-14 12:01:37.000000 celerabit-pipeline-integration-1.0.2/celerabit_pipeline_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 raul.devilla   (501) staff       (20)        1 2023-07-14 12:01:37.000000 celerabit-pipeline-integration-1.0.2/celerabit_pipeline_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 raul.devilla   (501) staff       (20)       17 2023-07-14 12:01:37.000000 celerabit-pipeline-integration-1.0.2/celerabit_pipeline_integration.egg-info/requires.txt
+-rw-r--r--   0 raul.devilla   (501) staff       (20)       29 2023-07-14 12:01:37.000000 celerabit-pipeline-integration-1.0.2/celerabit_pipeline_integration.egg-info/top_level.txt
+drwxr-xr-x   0 raul.devilla   (501) staff       (20)        0 2023-07-14 12:01:37.413261 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      789 2023-07-10 19:55:45.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/__init__.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      187 2023-07-10 19:55:37.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/__main__.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     6989 2023-07-10 19:55:39.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/int_main_module.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      174 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/model_credentials.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     2365 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/model_execution_params.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)       69 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/model_job.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1471 2023-07-10 19:58:17.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/uc_authenticator.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     3867 2023-07-10 19:59:44.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/uc_scenario_runner.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1536 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/util_compliance_evaluator.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1509 2023-07-14 12:00:30.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/util_configuration.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      397 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/util_http.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1143 2023-07-10 20:07:46.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/util_http_client.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      134 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/util_json.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)     1232 2023-07-10 19:56:04.000000 celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/util_logger.py
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      153 2023-07-10 19:40:07.000000 celerabit-pipeline-integration-1.0.2/pyproject.toml
+-rw-r--r--   0 raul.devilla   (501) staff       (20)       38 2023-07-14 12:01:37.414460 celerabit-pipeline-integration-1.0.2/setup.cfg
+-rw-r--r--   0 raul.devilla   (501) staff       (20)      852 2023-07-14 12:01:34.000000 celerabit-pipeline-integration-1.0.2/setup.py
```

### Comparing `celerabit-pipeline-integration-1.0.1/LICENCE` & `celerabit-pipeline-integration-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `celerabit-pipeline-integration-1.0.1/PKG-INFO` & `celerabit-pipeline-integration-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celerabit-pipeline-integration
-Version: 1.0.1
+Version: 1.0.2
 Summary: Celerabit tools to integrate with pipelines
 Home-page: https://git-codecommit.zone.amazonaws.com/v1/repos/celerabit-pipeline-integration-py-package
 Author: Raul A. de Villa C.
 Author-email: raul.devilla@techandsolve.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `celerabit-pipeline-integration-1.0.1/README.md` & `celerabit-pipeline-integration-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `celerabit-pipeline-integration-1.0.1/celerabit_pipeline_integration.egg-info/PKG-INFO` & `celerabit-pipeline-integration-1.0.2/celerabit_pipeline_integration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celerabit-pipeline-integration
-Version: 1.0.1
+Version: 1.0.2
 Summary: Celerabit tools to integrate with pipelines
 Home-page: https://git-codecommit.zone.amazonaws.com/v1/repos/celerabit-pipeline-integration-py-package
 Author: Raul A. de Villa C.
 Author-email: raul.devilla@techandsolve.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `celerabit-pipeline-integration-1.0.1/celerabit_pipeline_integration.egg-info/SOURCES.txt` & `celerabit-pipeline-integration-1.0.2/celerabit_pipeline_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/__init__.py` & `celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/__init__.py`

 * *Files identical despite different names*

### Comparing `celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/int_main_module.py` & `celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/int_main_module.py`

 * *Files identical despite different names*

### Comparing `celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/model_execution_params.py` & `celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/model_execution_params.py`

 * *Files identical despite different names*

### Comparing `celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/uc_authenticator.py` & `celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/uc_authenticator.py`

 * *Files identical despite different names*

### Comparing `celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/uc_scenario_runner.py` & `celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/uc_scenario_runner.py`

 * *Files identical despite different names*

### Comparing `celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/util_compliance_evaluator.py` & `celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/util_compliance_evaluator.py`

 * *Files identical despite different names*

### Comparing `celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/util_configuration.py` & `celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/util_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 class Configuration:
 
     __instance__ = None
     
     sections:any = {
         'CELERABIT-ENDPOINTS': {
-            'authenticate': 'https://sec-api.celerabit.com/authenticate',
-            'run': 'https://app-api.celerabit.com/named/client/{client}/target/{application}/scenario/{scenario}/run',
-            'get-job': 'https://app-api.celerabit.com/named/client/{client}/target/{application}/scenario/{scenario}/job/{job}'
+            'authenticate': 'https://sec-api.runfalcon.com/authenticate',
+            'run': 'https://app-api.runfalcon.com/named/client/{client}/target/{application}/scenario/{scenario}/run',
+            'get-job': 'https://app-api.runfalcon.com/named/client/{client}/target/{application}/scenario/{scenario}/job/{job}'
         },
         'INVOKER': {
             'id': 'celerabitpipelineintegration',
             'wait-to-get-status': 10,
             'default-run-timeout-seconds': 300
         },
         'LOGGER': {
```

### Comparing `celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/util_http_client.py` & `celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/util_http_client.py`

 * *Files identical despite different names*

### Comparing `celerabit-pipeline-integration-1.0.1/celerabitpipelineintegration/util_logger.py` & `celerabit-pipeline-integration-1.0.2/celerabitpipelineintegration/util_logger.py`

 * *Files identical despite different names*

### Comparing `celerabit-pipeline-integration-1.0.1/setup.py` & `celerabit-pipeline-integration-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 long_description:str = open('README.md').read()
 
 setuptools.setup (
     include_package_data=True,
     name='celerabit-pipeline-integration',
-    version='1.0.1',
+    version='1.0.2',
     description='Celerabit tools to integrate with pipelines',
     long_description = long_description,
     long_description_content_type='text/markdown',
     url='https://git-codecommit.zone.amazonaws.com/v1/repos/celerabit-pipeline-integration-py-package',
     author='Raul A. de Villa C.',
     author_email='raul.devilla@techandsolve.com',
     python_requires='>=3.6',
```

