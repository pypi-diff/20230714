# Comparing `tmp/versioned-0.5.1.tar.gz` & `tmp/versioned-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versioned-0.5.1.tar", last modified: Fri Jul 14 20:42:02 2023, max compression
+gzip compressed data, was "versioned-0.5.2.tar", last modified: Fri Jul 14 20:47:33 2023, max compression
```

## Comparing `versioned-0.5.1.tar` & `versioned-0.5.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.960472 versioned-0.5.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.5.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.5.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.5.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3963 2023-07-14 20:42:02.960337 versioned-0.5.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2828 2023-07-13 01:42:39.000000 versioned-0.5.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     4587 2023-07-14 20:41:46.000000 versioned-0.5.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.5.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.5.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.5.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.5.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      159 2023-07-14 20:41:46.000000 versioned-0.5.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-14 20:42:02.960519 versioned-0.5.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.5.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.957006 versioned-0.5.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1154 2023-07-14 20:41:46.000000 versioned-0.5.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-07-14 20:41:46.000000 versioned-0.5.1/tests/test_dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    10411 2023-07-14 20:41:46.000000 versioned-0.5.1/tests/test_s3_and_dynamodb_backend.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    15087 2023-07-14 20:41:46.000000 versioned-0.5.1/tests/test_s3_only_backend.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.958465 versioned-0.5.1/versioned/
--rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.5.1/versioned/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      472 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1959 2023-07-07 14:49:41.000000 versioned-0.5.1/versioned/bootstrap.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      383 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/compat.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      230 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/constants.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.959243 versioned-0.5.1/versioned/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4518 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.5.1/versioned/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17619 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/s3_and_dynamodb_backend.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    23254 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/s3_only_backend.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.959675 versioned-0.5.1/versioned/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.5.1/versioned/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.960152 versioned-0.5.1/versioned/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7573 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.959127 versioned-0.5.1/versioned.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3963 2023-07-14 20:42:02.000000 versioned-0.5.1/versioned.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      911 2023-07-14 20:42:02.000000 versioned-0.5.1/versioned.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-14 20:42:02.000000 versioned-0.5.1/versioned.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      281 2023-07-14 20:42:02.000000 versioned-0.5.1/versioned.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-14 20:42:02.000000 versioned-0.5.1/versioned.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:33.001953 versioned-0.5.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.5.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.5.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.5.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4256 2023-07-14 20:47:33.001833 versioned-0.5.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3121 2023-07-14 20:43:22.000000 versioned-0.5.2/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4772 2023-07-14 20:47:04.000000 versioned-0.5.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.5.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.5.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.5.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.5.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      159 2023-07-14 20:41:46.000000 versioned-0.5.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-14 20:47:33.001993 versioned-0.5.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.5.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:32.997287 versioned-0.5.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1197 2023-07-14 20:45:40.000000 versioned-0.5.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-07-14 20:41:46.000000 versioned-0.5.2/tests/test_dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10411 2023-07-14 20:41:46.000000 versioned-0.5.2/tests/test_s3_and_dynamodb_backend.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    15087 2023-07-14 20:41:46.000000 versioned-0.5.2/tests/test_s3_only_backend.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:32.999826 versioned-0.5.2/versioned/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.5.2/versioned/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-14 20:45:16.000000 versioned-0.5.2/versioned/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      472 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1959 2023-07-07 14:49:41.000000 versioned-0.5.2/versioned/bootstrap.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      383 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/compat.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      230 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/constants.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:33.000739 versioned-0.5.2/versioned/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4518 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.5.2/versioned/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17807 2023-07-14 20:46:31.000000 versioned-0.5.2/versioned/s3_and_dynamodb_backend.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    23254 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/s3_only_backend.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:33.001160 versioned-0.5.2/versioned/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.5.2/versioned/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:33.001645 versioned-0.5.2/versioned/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7573 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:33.000632 versioned-0.5.2/versioned.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4256 2023-07-14 20:47:32.000000 versioned-0.5.2/versioned.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      911 2023-07-14 20:47:32.000000 versioned-0.5.2/versioned.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-14 20:47:32.000000 versioned-0.5.2/versioned.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      281 2023-07-14 20:47:32.000000 versioned-0.5.2/versioned.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-14 20:47:32.000000 versioned-0.5.2/versioned.egg-info/top_level.txt
```

### Comparing `versioned-0.5.1/AUTHORS.rst` & `versioned-0.5.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/LICENSE.txt` & `versioned-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/PKG-INFO` & `versioned-0.5.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.5.1
+Version: 0.5.2
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.5.1#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.5.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -88,14 +88,19 @@
 
 - `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
 
 Learn why Blue / Green, Canary deployment and Rollback made easy with versioning and alias management.
 
 .. image:: https://github.com/MacHu-GWU/versioned-project/assets/6800411/57f7970e-3821-45a0-9deb-64890e04c129
 
+Related Project:
+
+- `aws_glue_artifact <https://github.com/MacHu-GWU/aws_glue_artifact-project>`_ enables the versioned deployment for AWS Glue.
+- `airflow_dag_artifact <https://github.com/MacHu-GWU/airflow_dag_artifact-project>`_ enables the versioned deployment for Airflow DAG deployment.
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``versioned`` is released on PyPI, so all you need is to:
```

### Comparing `versioned-0.5.1/README.rst` & `versioned-0.5.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -56,14 +56,19 @@
 
 - `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
 
 Learn why Blue / Green, Canary deployment and Rollback made easy with versioning and alias management.
 
 .. image:: https://github.com/MacHu-GWU/versioned-project/assets/6800411/57f7970e-3821-45a0-9deb-64890e04c129
 
+Related Project:
+
+- `aws_glue_artifact <https://github.com/MacHu-GWU/aws_glue_artifact-project>`_ enables the versioned deployment for AWS Glue.
+- `airflow_dag_artifact <https://github.com/MacHu-GWU/airflow_dag_artifact-project>`_ enables the versioned deployment for Airflow DAG deployment.
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``versioned`` is released on PyPI, so all you need is to:
```

### Comparing `versioned-0.5.1/release-history.rst` & `versioned-0.5.2/release-history.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.5.2 (2023-07-07)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug that accidentally deleted the ``get_artifact_s3path`` API.
+
+
 0.5.1 (2023-07-14)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add S3 only backend in ``s3_only_backend.py`` module. It doesn't require DynamoDB table.
 - the old ``core.py`` module is renamed to ``s3_and_dynamodb_backend.py`` module. The public API is not changed.
 - suggest to use ``from versioned import api as versioned``, then use ``versioned.s3_and_dynamodb_backend`` or ``versioned.s3_only_backend`` to access the backend.
```

### Comparing `versioned-0.5.1/requirements-doc.txt` & `versioned-0.5.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/setup.py` & `versioned-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/tests/test_api.py` & `versioned-0.5.2/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     _ = api.S3_PREFIX
     _ = api.LATEST_VERSION
     _ = api.VERSION_ZFILL
     _ = api.METADATA_KEY_ARTIFACT_SHA256
     _ = api.Artifact
     _ = api.Alias
     _ = api.Repository
+    _ = api.Repository.get_artifact_s3path
     _ = api.Repository.put_artifact
     _ = api.Repository.get_artifact_version
     _ = api.Repository.list_artifact_versions
     _ = api.Repository.publish_artifact_version
     _ = api.Repository.delete_artifact_version
     _ = api.Repository.put_alias
     _ = api.Repository.get_alias
```

### Comparing `versioned-0.5.1/tests/test_dynamodb.py` & `versioned-0.5.2/tests/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/tests/test_s3_and_dynamodb_backend.py` & `versioned-0.5.2/tests/test_s3_and_dynamodb_backend.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/tests/test_s3_only_backend.py` & `versioned-0.5.2/tests/test_s3_only_backend.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/versioned/bootstrap.py` & `versioned-0.5.2/versioned/bootstrap.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/versioned/dynamodb.py` & `versioned-0.5.2/versioned/dynamodb.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/versioned/paths.py` & `versioned-0.5.2/versioned/paths.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/versioned/s3_and_dynamodb_backend.py` & `versioned-0.5.2/versioned/s3_and_dynamodb_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,21 @@
     @property
     def s3dir_artifact_store(self) -> S3Path:
         """
         Return the s3dir of the artifact store folder.
         """
         return S3Path(self.s3_bucket).joinpath(self.s3_prefix).to_dir()
 
-    def _get_artifact_s3path(self, name: str, version: str) -> S3Path:
+    def get_artifact_s3path(self, name: str, version: str) -> S3Path:
+        """
+        Return the s3path of the artifact s3 object.
+
+        :param name: artifact name.
+        :param version: artifact version. If ``None``, return the latest version.
+        """
         return self.s3dir_artifact_store.joinpath(
             name,
             f"{dynamodb.encode_version_sk(version)}{self.suffix}",
         )
 
     def bootstrap(
         self,
@@ -176,33 +182,33 @@
         return Alias
 
     def _get_artifact_object(
         self,
         artifact: dynamodb.Artifact,
     ) -> Artifact:
         dct = artifact.to_dict()
-        dct["s3uri"] = self._get_artifact_s3path(
+        dct["s3uri"] = self.get_artifact_s3path(
             name=artifact.name,
             version=artifact.version,
         ).uri
         return Artifact(**dct)
 
     def _get_alias_object(
         self,
         alias: dynamodb.Alias,
     ) -> Alias:
         dct = alias.to_dict()
-        dct["version_s3uri"] = self._get_artifact_s3path(
+        dct["version_s3uri"] = self.get_artifact_s3path(
             name=alias.name,
             version=alias.version,
         ).uri
         if alias.secondary_version is None:
             dct["secondary_version_s3uri"] = None
         else:
-            dct["secondary_version_s3uri"] = self._get_artifact_s3path(
+            dct["secondary_version_s3uri"] = self.get_artifact_s3path(
                 name=alias.name,
                 version=alias.secondary_version,
             ).uri
         return Alias(**dct)
 
     def connect_boto_session(self, bsm: BotoSesManager):
         """
@@ -232,15 +238,15 @@
         :param content: binary artifact content.
         :param metadata: optional metadata of the s3 object.
         :param tags: optional tags of the s3 object.
         """
         artifact = self._artifact_class.new(name=name)
         artifact_sha256 = hashes.of_bytes(content)
         artifact.sha256 = artifact_sha256
-        s3path = self._get_artifact_s3path(name=name, version=constants.LATEST_VERSION)
+        s3path = self.get_artifact_s3path(name=name, version=constants.LATEST_VERSION)
 
         # do nothing if the content is not changed
         if s3path.exists():
             if s3path.metadata["artifact_sha256"] == artifact_sha256:
                 artifact.update_at = s3path.last_modified_at
                 return self._get_artifact_object(artifact=artifact)
 
@@ -338,19 +344,19 @@
             raise exc.ArtifactNotFoundError(f"name = {name!r}")
         elif len(artifacts) == 1:
             new_version = dynamodb.encode_version(1)
         else:
             new_version = str(int(artifacts[1].version) + 1)
 
         # copy artifact from latest to the new version
-        s3path_old = self._get_artifact_s3path(
+        s3path_old = self.get_artifact_s3path(
             name=name,
             version=constants.LATEST_VERSION,
         )
-        s3path_new = self._get_artifact_s3path(name=name, version=new_version)
+        s3path_new = self.get_artifact_s3path(name=name, version=new_version)
         s3path_old.copy_to(s3path_new)
         s3path_new.head_object()
 
         # create artifact object
         artifact = Artifact.new(name=name, version=new_version)
         artifact.sha256 = artifacts[0].sha256
         artifact.update_at = s3path_new.last_modified_at
@@ -505,15 +511,15 @@
         """
         Completely delete all artifacts and aliases of the given artifact name.
         This operation is irreversible. It will remove all related S3 artifacts
         and DynamoDB items.
 
         :param name: artifact name.
         """
-        s3path = self._get_artifact_s3path(name=name, version=constants.LATEST_VERSION)
+        s3path = self.get_artifact_s3path(name=name, version=constants.LATEST_VERSION)
         s3dir = s3path.parent
         s3dir.delete()
 
         Artifact = self._artifact_class
         Alias = self._alias_class
         with Artifact.batch_write() as batch:
             for artifact in Artifact.query(hash_key=name):
```

### Comparing `versioned-0.5.1/versioned/s3_only_backend.py` & `versioned-0.5.2/versioned/s3_only_backend.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/versioned/tests/mock_aws.py` & `versioned-0.5.2/versioned/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/versioned/vendor/hashes.py` & `versioned-0.5.2/versioned/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/versioned/vendor/pytest_cov_helper.py` & `versioned-0.5.2/versioned/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.1/versioned.egg-info/PKG-INFO` & `versioned-0.5.2/versioned.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.5.1
+Version: 0.5.2
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.5.1#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.5.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -88,14 +88,19 @@
 
 - `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
 
 Learn why Blue / Green, Canary deployment and Rollback made easy with versioning and alias management.
 
 .. image:: https://github.com/MacHu-GWU/versioned-project/assets/6800411/57f7970e-3821-45a0-9deb-64890e04c129
 
+Related Project:
+
+- `aws_glue_artifact <https://github.com/MacHu-GWU/aws_glue_artifact-project>`_ enables the versioned deployment for AWS Glue.
+- `airflow_dag_artifact <https://github.com/MacHu-GWU/airflow_dag_artifact-project>`_ enables the versioned deployment for Airflow DAG deployment.
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``versioned`` is released on PyPI, so all you need is to:
```

### Comparing `versioned-0.5.1/versioned.egg-info/SOURCES.txt` & `versioned-0.5.2/versioned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

