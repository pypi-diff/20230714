# Comparing `tmp/prefect-aws-0.3.4.tar.gz` & `tmp/prefect-aws-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-8kaz6hzb/prefect-aws-0.3.4.tar", last modified: Thu Jun 15 14:30:23 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-dykgbcpt/prefect-aws-0.3.5.tar", last modified: Fri Jul 14 19:13:13 2023, max compression
```

## Comparing `prefect-aws-0.3.4.tar` & `prefect-aws-0.3.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws/deployments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    57782 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35068 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/secrets_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56907 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/workers/ecs_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57782 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/secrets_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56988 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/workers/ecs_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27593 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/versioneer.py
```

### Comparing `prefect-aws-0.3.4/LICENSE` & `prefect-aws-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/PKG-INFO` & `prefect-aws-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.4
+Version: 0.3.5
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.4 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.5 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.3.4/README.md` & `prefect-aws-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/prefect_aws/__init__.py` & `prefect-aws-0.3.5/prefect_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/prefect_aws/batch.py` & `prefect-aws-0.3.5/prefect_aws/batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/prefect_aws/client_parameters.py` & `prefect-aws-0.3.5/prefect_aws/client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/prefect_aws/client_waiter.py` & `prefect-aws-0.3.5/prefect_aws/client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/prefect_aws/credentials.py` & `prefect-aws-0.3.5/prefect_aws/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/prefect_aws/deployments/steps.py` & `prefect-aws-0.3.5/prefect_aws/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/prefect_aws/ecs.py` & `prefect-aws-0.3.5/prefect_aws/ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/prefect_aws/s3.py` & `prefect-aws-0.3.5/prefect_aws/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -824,15 +824,15 @@
             ```
 
         """
         if to_path is None:
             to_path = Path(from_path).name
 
         # Get the source object's StreamingBody
-        from_path: str = self._join_bucket_folder(from_path)
+        from_path: str = bucket._join_bucket_folder(from_path)
         from_client = bucket.credentials.get_s3_client()
         obj = await run_sync_in_worker_thread(
             from_client.get_object, Bucket=bucket.bucket_name, Key=from_path
         )
         body: StreamingBody = obj["Body"]
 
         # Upload the StreamingBody to this bucket
```

### Comparing `prefect-aws-0.3.4/prefect_aws/secrets_manager.py` & `prefect-aws-0.3.5/prefect_aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/prefect_aws/workers/ecs_worker.py` & `prefect-aws-0.3.5/prefect_aws/workers/ecs_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,16 +503,16 @@
     A Prefect worker to run flow runs as ECS tasks.
     """
 
     type = "ecs"
     job_configuration = ECSJobConfiguration
     job_configuration_variables = ECSVariables
     _description = (
-        "Execute flow runs within containers on AWS ECS. Works with existing ECS "
-        "clusters and serverless execution via AWS Fargate. Requires an AWS account."
+        "Execute flow runs within containers on AWS ECS. Works with EC2 "
+        "and Fargate clusters. Requires an AWS account."
     )
     _display_name = "AWS Elastic Container Service"
     _documentation_url = "https://prefecthq.github.io/prefect-aws/ecs_worker/"
     _is_beta = True
     _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/1jbV4lceHOjGgunX15lUwT/db88e184d727f721575aeb054a37e277/aws.png?h=250"  # noqa
 
     async def run(
@@ -671,26 +671,30 @@
 
         # Update the cached task definition ARN to avoid re-registering the task
         # definition on this worker unless necessary; registration is agressively
         # rate limited by AWS
         _TASK_DEFINITION_CACHE[flow_run.deployment_id] = task_definition_arn
 
         logger.info(f"Using ECS task definition {task_definition_arn!r}...")
-        logger.debug(f"Task definition {json.dumps(task_definition, indent=2)}")
+        logger.debug(
+            f"Task definition {json.dumps(task_definition, indent=2, default=str)}"
+        )
 
         # Prepare the task run request
         task_run_request = self._prepare_task_run_request(
             boto_session,
             configuration,
             task_definition,
             task_definition_arn,
         )
 
         logger.info("Creating ECS task run...")
-        logger.debug(f"Task run request {json.dumps(task_run_request, indent=2)}")
+        logger.debug(
+            f"Task run request {json.dumps(task_run_request, indent=2, default=str)}"
+        )
         try:
             task = self._create_task_run(ecs_client, task_run_request)
             task_arn = task["taskArn"]
             cluster_arn = task["clusterArn"]
         except Exception as exc:
             self._report_task_run_creation_failure(configuration, task_run_request, exc)
             raise
@@ -857,15 +861,18 @@
     ) -> str:
         """
         Register a new task definition with AWS.
 
         Returns the ARN.
         """
         logger.info("Registering ECS task definition...")
-        logger.debug(f"Task definition request {json.dumps(task_definition, indent=2)}")
+        logger.debug(
+            "Task definition request"
+            f"{json.dumps(task_definition, indent=2, default=str)}"
+        )
         response = ecs_client.register_task_definition(**task_definition)
         return response["taskDefinition"]["taskDefinitionArn"]
 
     def _retrieve_task_definition(
         self,
         logger: logging.Logger,
         ecs_client: _ECSClient,
```

### Comparing `prefect-aws-0.3.4/prefect_aws.egg-info/PKG-INFO` & `prefect-aws-0.3.5/prefect_aws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.4
+Version: 0.3.5
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.4 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.5 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.3.4/prefect_aws.egg-info/SOURCES.txt` & `prefect-aws-0.3.5/prefect_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/setup.cfg` & `prefect-aws-0.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/setup.py` & `prefect-aws-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/tests/test_batch.py` & `prefect-aws-0.3.5/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/tests/test_block_standards.py` & `prefect-aws-0.3.5/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/tests/test_client_parameters.py` & `prefect-aws-0.3.5/tests/test_client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/tests/test_client_waiter.py` & `prefect-aws-0.3.5/tests/test_client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/tests/test_credentials.py` & `prefect-aws-0.3.5/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/tests/test_ecs.py` & `prefect-aws-0.3.5/tests/test_ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/tests/test_s3.py` & `prefect-aws-0.3.5/tests/test_s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -619,19 +619,34 @@
 
     @pytest.fixture
     def s3_bucket_empty(self, credentials, bucket):
         _s3_bucket = S3Bucket(bucket_name="bucket", credentials=credentials)
         return _s3_bucket
 
     @pytest.fixture
+    def s3_bucket_2_empty(self, credentials, bucket):
+        _s3_bucket = S3Bucket(
+            bucket_name="bucket",
+            credentials=credentials,
+            bucket_folder="subfolder",
+        )
+        return _s3_bucket
+
+    @pytest.fixture
     def s3_bucket_with_object(self, s3_bucket_empty, object):
         _s3_bucket_with_object = s3_bucket_empty  # object will be added
         return _s3_bucket_with_object
 
     @pytest.fixture
+    def s3_bucket_2_with_object(self, s3_bucket_2_empty):
+        _s3_bucket_with_object = s3_bucket_2_empty
+        s3_bucket_2_empty.write_path("object", content=b"TEST")
+        return _s3_bucket_with_object
+
+    @pytest.fixture
     def s3_bucket_with_objects(self, s3_bucket_with_object, object_in_folder):
         _s3_bucket_with_objects = (
             s3_bucket_with_object  # object in folder will be added
         )
         return _s3_bucket_with_objects
 
     @pytest.fixture
@@ -715,20 +730,20 @@
         to_path = Path(to_path)
         assert (to_path / "object").read_text() == "TEST OBJECT IN FOLDER"
 
     @pytest.mark.parametrize("to_path", ["to_path", None])
     @pytest.mark.parametrize("client_parameters", aws_clients[-1:], indirect=True)
     def test_stream_from(
         self,
-        s3_bucket_with_object: S3Bucket,
+        s3_bucket_2_with_object: S3Bucket,
         s3_bucket_empty: S3Bucket,
         client_parameters,
         to_path,
     ):
-        path = s3_bucket_empty.stream_from(s3_bucket_with_object, "object", to_path)
+        path = s3_bucket_empty.stream_from(s3_bucket_2_with_object, "object", to_path)
         data: bytes = s3_bucket_empty.read_path(path)
         assert data == b"TEST"
 
     @pytest.mark.parametrize("to_path", ["new_object", None])
     @pytest.mark.parametrize("client_parameters", aws_clients[-1:], indirect=True)
     def test_upload_from_path(
         self, s3_bucket_empty: S3Bucket, client_parameters, tmp_path, to_path
```

### Comparing `prefect-aws-0.3.4/tests/test_secrets_manager.py` & `prefect-aws-0.3.5/tests/test_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.4/versioneer.py` & `prefect-aws-0.3.5/versioneer.py`

 * *Files identical despite different names*

