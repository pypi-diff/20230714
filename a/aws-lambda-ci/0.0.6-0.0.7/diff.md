# Comparing `tmp/aws-lambda-ci-0.0.6.tar.gz` & `tmp/aws-lambda-ci-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-lambda-ci-0.0.6.tar", last modified: Thu Oct 28 11:39:17 2021, max compression
+gzip compressed data, was "aws-lambda-ci-0.0.7.tar", last modified: Fri Jul 14 14:08:27 2023, max compression
```

## Comparing `aws-lambda-ci-0.0.6.tar` & `aws-lambda-ci-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-28 11:39:17.770511 aws-lambda-ci-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2021-10-28 11:39:06.000000 aws-lambda-ci-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)    12605 2021-10-28 11:39:17.770511 aws-lambda-ci-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    12214 2021-10-28 11:39:06.000000 aws-lambda-ci-0.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-10-28 11:39:17.770511 aws-lambda-ci-0.0.6/aws_lambda_ci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    12605 2021-10-28 11:39:17.000000 aws-lambda-ci-0.0.6/aws_lambda_ci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      267 2021-10-28 11:39:17.000000 aws-lambda-ci-0.0.6/aws_lambda_ci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-10-28 11:39:17.000000 aws-lambda-ci-0.0.6/aws_lambda_ci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       41 2021-10-28 11:39:17.000000 aws-lambda-ci-0.0.6/aws_lambda_ci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2021-10-28 11:39:17.000000 aws-lambda-ci-0.0.6/aws_lambda_ci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        3 2021-10-28 11:39:17.000000 aws-lambda-ci-0.0.6/aws_lambda_ci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    18121 2021-10-28 11:39:06.000000 aws-lambda-ci-0.0.6/ci.py
--rw-r--r--   0 runner    (1001) docker     (116)      183 2021-10-28 11:39:17.770511 aws-lambda-ci-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      596 2021-10-28 11:39:06.000000 aws-lambda-ci-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:27.666601 aws-lambda-ci-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 14:08:16.000000 aws-lambda-ci-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-14 14:08:27.666601 aws-lambda-ci-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-07-14 14:08:16.000000 aws-lambda-ci-0.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:27.666601 aws-lambda-ci-0.0.7/aws_lambda_ci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-14 14:08:27.000000 aws-lambda-ci-0.0.7/aws_lambda_ci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-14 14:08:27.000000 aws-lambda-ci-0.0.7/aws_lambda_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:08:27.000000 aws-lambda-ci-0.0.7/aws_lambda_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 14:08:27.000000 aws-lambda-ci-0.0.7/aws_lambda_ci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 14:08:27.000000 aws-lambda-ci-0.0.7/aws_lambda_ci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-14 14:08:27.000000 aws-lambda-ci-0.0.7/aws_lambda_ci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-07-14 14:08:16.000000 aws-lambda-ci-0.0.7/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-14 14:08:27.666601 aws-lambda-ci-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-14 14:08:16.000000 aws-lambda-ci-0.0.7/setup.py
```

### Comparing `aws-lambda-ci-0.0.6/LICENSE` & `aws-lambda-ci-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-lambda-ci-0.0.6/PKG-INFO` & `aws-lambda-ci-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-lambda-ci
-Version: 0.0.6
+Version: 0.0.7
 Summary: Continuous integration pipeline for aws lambda function
 Home-page: https://github.com/kodless/aws-lambda-ci
 Author: Hamza Adami
 Author-email: me@adamihamza.com
 License: Apache License 2.0
 Keywords: aws,lambda,ci,cd,serverless
 Platform: any
@@ -217,9 +217,7 @@
 Nothing changed
 ---------------
 
 If both code and dependencies not changed, the pipeline will not publish anything.
 
 .. image:: https://github.com/obytes/aws-lambda-ci/raw/main/docs/images/demo_nothing_changed.gif
 
-
-
```

### Comparing `aws-lambda-ci-0.0.6/README.rst` & `aws-lambda-ci-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `aws-lambda-ci-0.0.6/aws_lambda_ci.egg-info/PKG-INFO` & `aws-lambda-ci-0.0.7/aws_lambda_ci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-lambda-ci
-Version: 0.0.6
+Version: 0.0.7
 Summary: Continuous integration pipeline for aws lambda function
 Home-page: https://github.com/kodless/aws-lambda-ci
 Author: Hamza Adami
 Author-email: me@adamihamza.com
 License: Apache License 2.0
 Keywords: aws,lambda,ci,cd,serverless
 Platform: any
@@ -217,9 +217,7 @@
 Nothing changed
 ---------------
 
 If both code and dependencies not changed, the pipeline will not publish anything.
 
 .. image:: https://github.com/obytes/aws-lambda-ci/raw/main/docs/images/demo_nothing_changed.gif
 
-
-
```

### Comparing `aws-lambda-ci-0.0.6/ci.py` & `aws-lambda-ci-0.0.7/ci.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,18 @@
 parser.add_argument('--source-version', dest='source_version', required=False, default=uuid.uuid4().hex.upper(),
                     help="The unique revision id (eg: github commit sha, or SemVer tag)")
 parser.add_argument('--aws-profile-name', dest='aws_profile_name', required=False,
                     help="AWS profile name (if not provided, will use default aws env variables)")
 parser.add_argument('--watch-log-stream', dest='watch_log_stream', required=False, default=False, action='store_true',
                     help="AWS profile name (if not provided, will use default aws env variables)")
 
+# To use custom lambci docker repository, eg: ECR repository.
+parser.add_argument('--build-docker-repo', dest='build_docker_repo', required=False, default="lambci/lambda",
+                    help="Use custom lambci/lambda build docker repository")
+
 args = parser.parse_args()
 
 # Validation
 # ----------
 if args.aws_profile_name:
     boto3.setup_default_session(profile_name=args.aws_profile_name)
 
@@ -133,14 +137,17 @@
 APP_CURRENT_S3_KEY = f"{APP_S3_KEY_PREFIX}/{FUNCTION_CURRENT_GIT_VERSION}/app.zip"
 DEP_CURRENT_S3_KEY = f"{APP_S3_KEY_PREFIX}/{FUNCTION_LAYER_CURRENT_GIT_VERSION}/deps.zip"
 
 # Internals
 APP_ZIP_FILENAME = f"{WORKING_DIR}/app"
 DEP_ZIP_FILENAME = f"{WORKING_DIR}/deps"
 
+# Build repo
+BUILD_DOCKER_REPO = args.build_docker_repo
+
 COL_BLU = "\033[94m"
 COL_GRN = "\033[92m"
 COL_YEL = "\033[93m"
 COL_MAG = "\033[95m"
 COL_CYN = "\033[96m"
 COL_WHT = "\033[97m"
 COL_END = "\033[0m"
@@ -336,15 +343,15 @@
     install_cmd = f"npm install"
     docker_run(install_cmd)
 
 
 def docker_run(install_cmd):
     docker_cmd = (
         "docker", "run", f'-v "{WORKING_DIR}":/var/task',
-        f"--rm lambci/lambda:build-{FUNCTION_RUNTIME}",
+        f"--rm {BUILD_DOCKER_REPO}:build-{FUNCTION_RUNTIME}",
         f'/bin/sh -c "{install_cmd}"'
     )
     try:
         with open(f"/tmp/{SOURCE_VERSION}-deps.log", 'w') as output:
             subprocess.check_call(
                 " ".join(docker_cmd),
                 shell=True,
```

### Comparing `aws-lambda-ci-0.0.6/setup.py` & `aws-lambda-ci-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="aws-lambda-ci",
-    version="0.0.6",
+    version="0.0.7",
     url="https://github.com/kodless/aws-lambda-ci",
     license="Apache License 2.0",
     author="Hamza Adami",
     author_email="me@adamihamza.com",
     description="Continuous integration pipeline for aws lambda function",
     keywords="aws,lambda,ci,cd,serverless",
     platforms='any',
```

