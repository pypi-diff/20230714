# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551.tar", last modified: Fri Jul 14 13:46:53 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037.tar", last modified: Fri Jul 14 15:41:38 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:46:53.827149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 13:46:53.827149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 13:46:53.827149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-14 13:46:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:46:53.823149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:46:53.827149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15645 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-14 13:45:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:46:53.827149 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 13:46:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-14 13:46:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 13:46:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-14 13:46:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 13:46:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-14 15:41:34.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15645 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3520 2023-07-14 15:40:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 15:41:38.650597 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 15:41:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-14 15:41:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 15:41:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-14 15:41:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 15:41:38.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230714134551
+Version: 1.0.0.dev20230714154037
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230714134551",
+  version="1.0.0.dev20230714154037",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 from .s3_operations import S3Operations
 from .dynamo_operations import DynamoOperations
 
 
 input_bucket = os.environ['INPUT_BUCKET']
 output_bucket = os.environ['OUTPUT_BUCKET']
 table_name = os.environ['TABLE_NAME']
+output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
+output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
 
 executor = LambdaExecutor(
     s3_operations=S3Operations(),
     dynamo_operations=DynamoOperations(),
     input_bucket=input_bucket,
     output_bucket=output_bucket,
     table_name=table_name,
-    output_bucket_access_key=os.getenv('OUTPUT_BUCKET_ACCESS_KEY'),
-    output_bucket_secret_access_key=os.getenv('OUTPUT_BUCKET_SECRET_ACCESS_KEY')
+    output_bucket_access_key=output_bucket_access_key,
+    output_bucket_secret_access_key=output_bucket_secret_access_key
 )
 
 def handler(sns_event, context):
     print(f"table name: {os.environ['TABLE_NAME']}")
     print(f"input bucket: {os.environ['INPUT_BUCKET']}")
     print(f"output bucket: {os.environ['OUTPUT_BUCKET']}")
     if 'OUTPUT_BUCKET_ACCESS_KEY' in os.environ:
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230714134551
+Version: 1.0.0.dev20230714154037
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714134551/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714154037/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

