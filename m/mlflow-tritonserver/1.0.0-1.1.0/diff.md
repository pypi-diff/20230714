# Comparing `tmp/mlflow-tritonserver-1.0.0.tar.gz` & `tmp/mlflow-tritonserver-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-tritonserver-1.0.0.tar", last modified: Fri Jul 14 07:00:19 2023, max compression
+gzip compressed data, was "mlflow-tritonserver-1.1.0.tar", last modified: Fri Jul 14 11:07:21 2023, max compression
```

## Comparing `mlflow-tritonserver-1.0.0.tar` & `mlflow-tritonserver-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:19.665919 mlflow-tritonserver-1.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:19.661919 mlflow-tritonserver-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:19.665919 mlflow-tritonserver-1.0.0/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)    10141 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-14 07:00:19.665919 mlflow-tritonserver-1.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7244 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:19.661919 mlflow-tritonserver-1.0.0/deploy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:19.665919 mlflow-tritonserver-1.0.0/deploy/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/deploy/docker/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:19.661919 mlflow-tritonserver-1.0.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:19.665919 mlflow-tritonserver-1.0.0/examples/deploy_with_docker/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/examples/deploy_with_docker/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/examples/deploy_with_docker/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:19.665919 mlflow-tritonserver-1.0.0/examples/deploy_with_docker/onnx_float32_int32_int32/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:19.665919 mlflow-tritonserver-1.0.0/examples/deploy_with_docker/onnx_float32_int32_int32/1/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/examples/deploy_with_docker/onnx_float32_int32_int32/1/model.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/examples/deploy_with_docker/onnx_float32_int32_int32/config.pbtxt
--rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/examples/deploy_with_docker/onnx_float32_int32_int32/expected_output.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      526 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/examples/deploy_with_docker/onnx_float32_int32_int32/input.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:19.665919 mlflow-tritonserver-1.0.0/mlflow_tritonserver/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22220 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver/deployments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1986 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver/mlflow_tritonserver_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2903 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver/triton_flavor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:00:19.665919 mlflow-tritonserver-1.0.0/mlflow_tritonserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-14 07:00:19.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-14 07:00:19.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:00:19.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-14 07:00:19.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-14 07:00:19.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 07:00:19.000000 mlflow-tritonserver-1.0.0/mlflow_tritonserver.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2593 2023-07-14 07:00:07.000000 mlflow-tritonserver-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 07:00:19.665919 mlflow-tritonserver-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:21.928125 mlflow-tritonserver-1.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-07-14 11:07:07.000000 mlflow-tritonserver-1.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:21.916124 mlflow-tritonserver-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:21.920124 mlflow-tritonserver-1.1.0/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-07-14 11:07:07.000000 mlflow-tritonserver-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-14 11:07:07.000000 mlflow-tritonserver-1.1.0/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10141 2023-07-14 11:07:07.000000 mlflow-tritonserver-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-14 11:07:21.928125 mlflow-tritonserver-1.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7244 2023-07-14 11:07:07.000000 mlflow-tritonserver-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:21.916124 mlflow-tritonserver-1.1.0/deploy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:21.920124 mlflow-tritonserver-1.1.0/deploy/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-14 11:07:07.000000 mlflow-tritonserver-1.1.0/deploy/docker/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:21.916124 mlflow-tritonserver-1.1.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:21.920124 mlflow-tritonserver-1.1.0/examples/deploy_with_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-14 11:07:07.000000 mlflow-tritonserver-1.1.0/examples/deploy_with_docker/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:21.924124 mlflow-tritonserver-1.1.0/examples/deploy_with_docker/onnx_float32_int32_int32/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 11:07:07.000000 mlflow-tritonserver-1.1.0/examples/deploy_with_docker/onnx_float32_int32_int32/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:21.924124 mlflow-tritonserver-1.1.0/examples/deploy_with_docker/onnx_float32_int32_int32/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 11:07:08.000000 mlflow-tritonserver-1.1.0/examples/deploy_with_docker/onnx_float32_int32_int32/1/model.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-14 11:07:08.000000 mlflow-tritonserver-1.1.0/examples/deploy_with_docker/onnx_float32_int32_int32/config.pbtxt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-07-14 11:07:08.000000 mlflow-tritonserver-1.1.0/examples/deploy_with_docker/onnx_float32_int32_int32/expected_output.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      526 2023-07-14 11:07:08.000000 mlflow-tritonserver-1.1.0/examples/deploy_with_docker/onnx_float32_int32_int32/input.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:21.928125 mlflow-tritonserver-1.1.0/mlflow_tritonserver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:08.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-07-14 11:07:08.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-14 11:07:08.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22220 2023-07-14 11:07:08.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver/deployments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2090 2023-07-14 11:07:08.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver/mlflow_tritonserver_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2903 2023-07-14 11:07:08.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver/triton_flavor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:21.928125 mlflow-tritonserver-1.1.0/mlflow_tritonserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-14 11:07:21.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-14 11:07:21.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:07:21.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-14 11:07:21.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-14 11:07:21.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 11:07:21.000000 mlflow-tritonserver-1.1.0/mlflow_tritonserver.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2593 2023-07-14 11:07:08.000000 mlflow-tritonserver-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:07:21.928125 mlflow-tritonserver-1.1.0/setup.cfg
```

### Comparing `mlflow-tritonserver-1.0.0/.gitattributes` & `mlflow-tritonserver-1.1.0/.gitattributes`

 * *Files identical despite different names*

### Comparing `mlflow-tritonserver-1.0.0/.github/workflows/python-publish.yml` & `mlflow-tritonserver-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mlflow-tritonserver-1.0.0/.gitignore` & `mlflow-tritonserver-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mlflow-tritonserver-1.0.0/LICENSE` & `mlflow-tritonserver-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlflow-tritonserver-1.0.0/PKG-INFO` & `mlflow-tritonserver-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-tritonserver
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tritonserver Mlflow Deployment
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/msclock/mlflow-tritonserver.git
 Project-URL: Source, https://github.com/msclock/mlflow-tritonserver.git
 Project-URL: Tracker, https://github.com/msclock/mlflow-tritonserver/issues
 Keywords: machine-learning,deep-learning,inference,tritonserver,mlflow
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mlflow-tritonserver-1.0.0/README.md` & `mlflow-tritonserver-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mlflow-tritonserver-1.0.0/deploy/docker/docker-compose.yml` & `mlflow-tritonserver-1.1.0/deploy/docker/docker-compose.yml`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     healthcheck:
       test: [ "CMD-SHELL", "pg_isready -U ${POSTGRES_USER:-postgres}" ]
       interval: 30s
       timeout: 10s
       retries: 3
 
   mlflow_tracking_server:
-    image: ubuntu/mlflow:2.1.1_1.0-22.04
+    image: ghcr.io/mlflow/mlflow:v2.4.2
     depends_on:
       postgres:
         condition: service_healthy
       triton_servering:
         condition: service_healthy
       minio_mlflow_bucket:
         condition: service_completed_successfully
```

### Comparing `mlflow-tritonserver-1.0.0/examples/deploy_with_docker/README.md` & `mlflow-tritonserver-1.1.0/examples/deploy_with_docker/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 ## Deploy
 
 ### mlflow integration
 
 The following demonstrates how to deploy a machine learning model using MLflow and Triton server. It first installs the necessary dependencies and configures the MLflow tracking and Triton server endpoint. Then it launches Triton server using Docker and registers the model to the MLflow tracking. Finally, it deploys the MLflow model to the Triton server.  
 
+### Deploy with docker
+
+#### Deploy using docker commands
 
 This example presents a local path as remote model repository of tritonserver can be served, and deploying models by mlflow-tritonserver.
+
+Step 1, launch mlflow server locally.
 ```bash
 # Install mlflow-tritonserver
 pip install mlflow-tritonserver
 
 # Configure mlflow tracing
 mlflow server
+```
 
+Step 2, launch tritonserver locally
+```bash
 # Configure remote model store
 export TRITON_MODEL_REPO=/tmp/model_repository
 
 # Prepare local model repository as remote model store for tritonserver
 mkdir $TRITON_MODEL_REPO
 
 # Launch tritonserver with docker
@@ -27,27 +35,34 @@
     -v $TRITON_MODEL_REPO:/tmp/model_repository \
     -v $(pwd):/workspace -w /workspace \
     nvcr.io/nvidia/tritonserver:22.12-py3 \
     bash -c 'tritonserver --model-repository=/tmp/model_repository --model-control-mode=explicit --log-verbose=1'
 
 # Check health
 curl -v localhost:8000/v2/health/ready
+```
 
+Step 3, register model.
+```bash
 # Configure mlflow tracking uri for registering models using mlflow_tritonserver
 export MLFLOW_TRACKING_URI=http://localhost:5000
 
 # Register model to mlflow tracking
 mlflow_tritonserver_cli publish \
     --model_name onnx_float32_int32_int32 \
     --model_directory examples/onnx_float32_int32_int32 \
     --flavor triton
+```
 
+Step 4, deploy the model to tritonserver.
+```bash
+# Tacking uri is still required for deployment from now
+export MLFLOW_TRACKING_URI=http://localhost:5000
 # Configure a local path as remote model store
 export TRITON_MODEL_REPO=/tmp/model_repository
-
 # Configure tritonserver endpoint for deploying models using mlflow deployments
 export TRITON_URL=http://localhost:8000
 
 # Deploy mlflow model to tritonserver
 # For delete and update operations, refer to mlflow-tritonserver/README.md
 mlflow deployments create \
     -t triton \
@@ -57,29 +72,40 @@
 
 # Check model config
 curl localhost:8000/v2/models/onnx_float32_int32_int32/config | jq
 # Check model status
 curl -X POST localhost:8000/v2/repository/index | jq
 ```
 
+#### Deploy using docker-compose
 
 The following example presents a s3 url from minio as remote model repository of tritonserver can be served, and deploying models by mlflow-tritonserver.
+
+Step 1, launch backend services including tritonserver, minio, mlflow, postgres.
 ```bash
 # Start docker-compose
 docker-compose -f deploy/docker/docker-compose.yml up -V --remove-orphans
+```
 
+Step 2, register model.
+```bash
 # Configure mlflow tracking uri for registering models using mlflow_tritonserver
 export MLFLOW_TRACKING_URI=http://localhost:5000
 
 # Register model to mlflow tracking
 mlflow_tritonserver_cli publish \
     --model_name onnx_float32_int32_int32 \
     --model_directory examples/onnx_float32_int32_int32 \
     --flavor triton
+```
 
+Step 3, deploy the model to tritonserver.
+```bash
+# Tacking uri is still required for deployment from now
+export MLFLOW_TRACKING_URI=http://localhost:5000
 # Configure a s3 url from minio as remote model store
 export TRITON_MODEL_REPO=s3://http://localhost:9000/models
 # Set AWS access key ID for MinIO
 export AWS_ACCESS_KEY_ID=minio
 # Set AWS secret access key for MinIO
 export AWS_SECRET_ACCESS_KEY=minio123
 # Configure tritonserver endpoint for deploying models using mlflow deployments
@@ -88,9 +114,8 @@
 # Deploy mlflow model to tritonserver
 # For unload and update operations, refer to mlflow-tritonserver/README.md
 mlflow deployments create \
     -t triton \
     --flavor triton \
     --name onnx_float32_int32_int32 \
     -m models:/onnx_float32_int32_int32/1
-
 ```
```

### Comparing `mlflow-tritonserver-1.0.0/examples/deploy_with_docker/onnx_float32_int32_int32/config.pbtxt` & `mlflow-tritonserver-1.1.0/examples/deploy_with_docker/onnx_float32_int32_int32/config.pbtxt`

 * *Files identical despite different names*

### Comparing `mlflow-tritonserver-1.0.0/examples/deploy_with_docker/onnx_float32_int32_int32/input.json` & `mlflow-tritonserver-1.1.0/examples/deploy_with_docker/onnx_float32_int32_int32/input.json`

 * *Files identical despite different names*

### Comparing `mlflow-tritonserver-1.0.0/mlflow_tritonserver/config.py` & `mlflow-tritonserver-1.1.0/mlflow_tritonserver/config.py`

 * *Files identical despite different names*

### Comparing `mlflow-tritonserver-1.0.0/mlflow_tritonserver/deployments.py` & `mlflow-tritonserver-1.1.0/mlflow_tritonserver/deployments.py`

 * *Files identical despite different names*

### Comparing `mlflow-tritonserver-1.0.0/mlflow_tritonserver/mlflow_tritonserver_cli.py` & `mlflow-tritonserver-1.1.0/mlflow_tritonserver/mlflow_tritonserver_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,20 +39,21 @@
 
     Raises:
         Exception: If the flavor is not supported.
     """
     # Get MLflow tracking URI from environment variable
     mlflow_tracking_uri = os.environ["MLFLOW_TRACKING_URI"]
     artifact_path = "triton"
+    run_name = os.environ.get("MLFLOW_REGISTER_TRITON_MODEL", "register-triton-model")
 
     # Set the tracking URI for MLflow
     mlflow.set_tracking_uri(uri=mlflow_tracking_uri)
 
     # Start a new MLflow run
-    with mlflow.start_run() as run:
+    with mlflow.start_run(run_name=run_name) as run:
         # If the flavor is Triton, log the model
         if flavor == "triton":
             triton_flavor.log_model(
                 triton_model_path=model_directory,
                 artifact_path=artifact_path,
                 registered_model_name=model_name,
             )
```

### Comparing `mlflow-tritonserver-1.0.0/mlflow_tritonserver/triton_flavor.py` & `mlflow-tritonserver-1.1.0/mlflow_tritonserver/triton_flavor.py`

 * *Files identical despite different names*

### Comparing `mlflow-tritonserver-1.0.0/mlflow_tritonserver.egg-info/PKG-INFO` & `mlflow-tritonserver-1.1.0/mlflow_tritonserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-tritonserver
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tritonserver Mlflow Deployment
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/msclock/mlflow-tritonserver.git
 Project-URL: Source, https://github.com/msclock/mlflow-tritonserver.git
 Project-URL: Tracker, https://github.com/msclock/mlflow-tritonserver/issues
 Keywords: machine-learning,deep-learning,inference,tritonserver,mlflow
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mlflow-tritonserver-1.0.0/mlflow_tritonserver.egg-info/SOURCES.txt` & `mlflow-tritonserver-1.1.0/mlflow_tritonserver.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 .gitattributes
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/python-publish.yml
 deploy/docker/docker-compose.yml
-examples/deploy_with_docker/.gitignore
 examples/deploy_with_docker/README.md
+examples/deploy_with_docker/onnx_float32_int32_int32/.gitignore
 examples/deploy_with_docker/onnx_float32_int32_int32/config.pbtxt
 examples/deploy_with_docker/onnx_float32_int32_int32/expected_output.json
 examples/deploy_with_docker/onnx_float32_int32_int32/input.json
 examples/deploy_with_docker/onnx_float32_int32_int32/1/model.onnx
 mlflow_tritonserver/__init__.py
 mlflow_tritonserver/__version__.py
 mlflow_tritonserver/config.py
```

### Comparing `mlflow-tritonserver-1.0.0/pyproject.toml` & `mlflow-tritonserver-1.1.0/pyproject.toml`

 * *Files identical despite different names*

