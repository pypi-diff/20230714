# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818.tar", last modified: Wed Jul 12 08:29:19 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551.tar", last modified: Fri Jul 14 13:46:53 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:29:19.294409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-12 08:29:19.294409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 08:29:19.294409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-12 08:29:14.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:29:19.290409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:29:19.290409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15654 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-12 08:28:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 08:29:19.294409 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-12 08:29:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-12 08:29:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 08:29:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-12 08:29:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-12 08:29:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:46:53.827149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 13:46:53.827149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 13:46:53.827149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-14 13:46:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:46:53.823149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:46:53.827149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15645 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3520 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:46:53.827149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 13:46:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-14 13:46:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 13:46:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-14 13:46:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 13:46:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230712082818
-Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # echofish-aws-raw-to-zarr-lambda
 
 ## Setting up the Python Environment
 
 # MacOS
   1. Install pyenv (https://github.com/pyenv/pyenv#set-up-your-shell-environment-for-pyenv)
      1. ```brew update```
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: echofish-aws-raw-to-zarr-lambda
+Version: 1.0.0.dev20230714134551
+Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # echofish-aws-raw-to-zarr-lambda
 
 ## Setting up the Python Environment
 
 # MacOS
   1. Install pyenv (https://github.com/pyenv/pyenv#set-up-your-shell-environment-for-pyenv)
      1. ```brew update```
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230712082818",
+  version="1.0.0.dev20230714134551",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,18 +346,19 @@
                     access_key_id=self.__output_bucket_access_key,
                     secret_access_key=self.__output_bucket_secret_access_key
                 )
         # print('Done uploading files')
 
     ############################################################################
     def execute(self, message):
-        ship_name = message['ship_name']
-        cruise_name = message['cruise_name']
-        sensor_name = message['sensor_name']
-        input_file_name = message['input_file_name']
+        ship_name = message['shipName']
+        cruise_name = message['cruiseName']
+        sensor_name = message['sensorName']
+        input_file_name = message['fileName']
+
         #
         store_name = f"{os.path.splitext(input_file_name)[0]}.zarr"
         print(store_name)
         output_zarr_prefix = f"level_1/{ship_name}/{cruise_name}/{sensor_name}"
         bucket_key = f"data/raw/{ship_name}/{cruise_name}/{sensor_name}/{input_file_name}"
         print(bucket_key)
         #
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230712082818
+Version: 1.0.0.dev20230714134551
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230712082818/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

