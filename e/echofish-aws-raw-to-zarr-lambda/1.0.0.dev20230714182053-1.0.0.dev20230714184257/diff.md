# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053.tar", last modified: Fri Jul 14 18:21:55 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257.tar", last modified: Fri Jul 14 18:44:04 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:21:55.138934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 18:21:55.138934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 18:21:55.138934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-14 18:21:51.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:21:55.134934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:21:55.134934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15566 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3398 2023-07-14 18:20:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:21:55.138934 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 18:21:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-14 18:21:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 18:21:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-14 18:21:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 18:21:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:44:04.391390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 18:44:04.391390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 18:44:04.391390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-14 18:43:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:44:04.387390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:44:04.387390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3398 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:44:04.391390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 18:44:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-14 18:44:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 18:44:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-14 18:44:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 18:44:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230714182053
+Version: 1.0.0.dev20230714184257
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230714182053",
+  version="1.0.0.dev20230714184257",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,16 +380,14 @@
         self.__create_local_zarr_store(
             raw_file_name=input_file_name,
             cruise_name=cruise_name,
             sensor_name=sensor_name,
             output_zarr_prefix=output_zarr_prefix,
             store_name=store_name
         )
-        # TODO: problem here, this is the first use of the NOAA-NODD credentials and for some reason
-        # those credentials can write but cannot delete???
         self.__remove_existing_s3_objects(
             prefix=os.path.join(output_zarr_prefix, store_name)
         )
         self.__upload_files(store_name, output_zarr_prefix)
         self.__update_processing_status(
             cruise_name=cruise_name,
             file_name=input_file_name,
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230714182053
+Version: 1.0.0.dev20230714184257
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714182053/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

