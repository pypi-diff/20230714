# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037.tar", last modified: Fri Jul 14 15:41:38 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053.tar", last modified: Fri Jul 14 18:21:55 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-14 15:41:34.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15645 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 15:41:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-14 15:41:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 15:41:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-14 15:41:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 15:41:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:21:55.138934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 18:21:55.138934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 18:21:55.138934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-14 18:21:51.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:21:55.134934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:21:55.134934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15566 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3398 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:21:55.138934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 18:21:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-14 18:21:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 18:21:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-14 18:21:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 18:21:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230714154037
+Version: 1.0.0.dev20230714182053
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230714154037",
+  version="1.0.0.dev20230714182053",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,21 +353,18 @@
         ship_name = message['shipName']
         cruise_name = message['cruiseName']
         sensor_name = message['sensorName']
         input_file_name = message['fileName']
 
         #
         store_name = f"{os.path.splitext(input_file_name)[0]}.zarr"
-        print(store_name)
         output_zarr_prefix = f"level_1/{ship_name}/{cruise_name}/{sensor_name}"
         bucket_key = f"data/raw/{ship_name}/{cruise_name}/{sensor_name}/{input_file_name}"
-        print(bucket_key)
         #
         os.chdir(TEMPDIR)
-        print(os.getcwd())
         #
         self.__set_processing_status(
             ship_name=ship_name,
             cruise_name=cruise_name,
             sensor_name=sensor_name,
             file_name=input_file_name,
             new_status="PROCESSING"
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,22 +19,14 @@
     output_bucket=output_bucket,
     table_name=table_name,
     output_bucket_access_key=output_bucket_access_key,
     output_bucket_secret_access_key=output_bucket_secret_access_key
 )
 
 def handler(sns_event, context):
-    print(f"table name: {os.environ['TABLE_NAME']}")
-    print(f"input bucket: {os.environ['INPUT_BUCKET']}")
-    print(f"output bucket: {os.environ['OUTPUT_BUCKET']}")
-    if 'OUTPUT_BUCKET_ACCESS_KEY' in os.environ:
-        print(os.environ['OUTPUT_BUCKET_ACCESS_KEY'])
-    if 'OUTPUT_BUCKET_SECRET_ACCESS_KEY' in os.environ:
-        print(os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY'])
-    #
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
     for record in sns_event['Records']:
         message = json.loads(record['Sns']['Message'])
         print("Start Message : " + str(message))
         executor.execute(message)
         print("Done Message : " + str(message))
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         session = boto3.Session()
         if access_key_id:
             s3_client = session.client(
                 service_name='s3',
                 aws_access_key_id=access_key_id,
                 aws_secret_access_key=secret_access_key
             )
-            print('NODD Authenticated')
         else:
             s3_client = session.client(service_name='s3')
         return s3_client
 
     #####################################################################
     def __chunked(
             self,
@@ -55,15 +54,14 @@
         # Returns a list of key strings for each object in bucket defined by prefix
         s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
         keys = []
         for page in s3_client.get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
             if 'Contents' in page.keys():
                 # keys.extend(page['Contents'])
                 keys.extend([k['Key'] for k in page['Contents']])
-        print(f'Found {len(keys)} items')
         return keys
 
     #####################################################################
     def download_file(
             self,
             bucket_name,
             key,
@@ -78,16 +76,14 @@
     def delete_object(
             self,
             bucket_name,
             key,
             access_key_id=None,
             secret_access_key=None
     ):
-        print('key')
-        print(key)
         s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
         print(f"Deleting item: Bucket={bucket_name}, Key={key}")
         s3_client.delete_object(Bucket=bucket_name, Key=key)
 
     #####################################################################
     def upload_file(
             self,
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230714154037
+Version: 1.0.0.dev20230714182053
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

