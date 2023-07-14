# Comparing `tmp/aws-secure-log-bucket-0.8.0.tar.gz` & `tmp/aws-secure-log-bucket-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-secure-log-bucket-0.8.0.tar", last modified: Fri Jul 14 05:49:06 2023, max compression
+gzip compressed data, was "aws-secure-log-bucket-0.8.1.tar", last modified: Fri Jul 14 18:15:52 2023, max compression
```

## Comparing `aws-secure-log-bucket-0.8.0.tar` & `aws-secure-log-bucket-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:49:06.061621 aws-secure-log-bucket-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-14 05:48:52.000000 aws-secure-log-bucket-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 05:48:52.000000 aws-secure-log-bucket-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-14 05:49:06.061621 aws-secure-log-bucket-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-14 05:48:52.000000 aws-secure-log-bucket-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 05:48:52.000000 aws-secure-log-bucket-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:49:06.061621 aws-secure-log-bucket-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-14 05:48:52.000000 aws-secure-log-bucket-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:49:06.057621 aws-secure-log-bucket-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:49:06.061621 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-14 05:48:52.000000 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:49:06.061621 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-14 05:48:52.000000 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23401 2023-07-14 05:48:52.000000 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@0.8.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:48:52.000000 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:49:06.061621 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-14 05:49:06.000000 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-14 05:49:06.000000 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:49:06.000000 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 05:49:06.000000 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 05:49:06.000000 aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:15:52.915917 aws-secure-log-bucket-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-14 18:15:39.000000 aws-secure-log-bucket-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 18:15:39.000000 aws-secure-log-bucket-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-14 18:15:52.915917 aws-secure-log-bucket-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-14 18:15:39.000000 aws-secure-log-bucket-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 18:15:39.000000 aws-secure-log-bucket-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 18:15:52.915917 aws-secure-log-bucket-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-14 18:15:39.000000 aws-secure-log-bucket-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:15:52.915917 aws-secure-log-bucket-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:15:52.915917 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-14 18:15:39.000000 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:15:52.915917 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-14 18:15:39.000000 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23405 2023-07-14 18:15:39.000000 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@0.8.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:15:39.000000 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:15:52.915917 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-14 18:15:52.000000 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-14 18:15:52.000000 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:15:52.000000 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 18:15:52.000000 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 18:15:52.000000 aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket.egg-info/top_level.txt
```

### Comparing `aws-secure-log-bucket-0.8.0/LICENSE` & `aws-secure-log-bucket-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-secure-log-bucket-0.8.0/PKG-INFO` & `aws-secure-log-bucket-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-secure-log-bucket
-Version: 0.8.0
+Version: 0.8.1
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/yicr/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-secure-log-bucket-0.8.0/README.md` & `aws-secure-log-bucket-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `aws-secure-log-bucket-0.8.0/setup.py` & `aws-secure-log-bucket-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-secure-log-bucket",
-    "version": "0.8.0",
+    "version": "0.8.1",
     "description": "secure multiple transition phases in a single lifecycle policy bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-log-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_secure_log_bucket",
         "aws_secure_log_bucket._jsii"
     ],
     "package_data": {
         "aws_secure_log_bucket._jsii": [
-            "aws-secure-log-bucket@0.8.0.jsii.tgz"
+            "aws-secure-log-bucket@0.8.1.jsii.tgz"
         ],
         "aws_secure_log_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket/__init__.py` & `aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-secure-log-bucket-0.8.0/src/aws_secure_log_bucket.egg-info/PKG-INFO` & `aws-secure-log-bucket-0.8.1/src/aws_secure_log_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-secure-log-bucket
-Version: 0.8.0
+Version: 0.8.1
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/yicr/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

