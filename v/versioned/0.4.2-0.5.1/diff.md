# Comparing `tmp/versioned-0.4.2.tar.gz` & `tmp/versioned-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versioned-0.4.2.tar", last modified: Fri Jul  7 18:17:27 2023, max compression
+gzip compressed data, was "versioned-0.5.1.tar", last modified: Fri Jul 14 20:42:02 2023, max compression
```

## Comparing `versioned-0.4.2.tar` & `versioned-0.5.1.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.539202 versioned-0.4.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.4.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.4.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.4.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-07 18:17:27.539063 versioned-0.4.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.4.2/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     4015 2023-07-07 18:16:47.000000 versioned-0.4.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.4.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.4.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.4.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.4.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.4.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-07 18:17:27.539247 versioned-0.4.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.4.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.536214 versioned-0.4.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1091 2023-07-07 14:48:52.000000 versioned-0.4.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     9626 2023-07-07 14:49:13.000000 versioned-0.4.2/tests/test_core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.537205 versioned-0.4.2/versioned/
--rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.4.2/versioned/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-07 18:16:04.000000 versioned-0.4.2/versioned/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-07-06 16:22:35.000000 versioned-0.4.2/versioned/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1959 2023-07-07 14:49:41.000000 versioned-0.4.2/versioned/bootstrap.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      181 2023-07-06 16:33:04.000000 versioned-0.4.2/versioned/constants.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    16648 2023-07-07 18:15:44.000000 versioned-0.4.2/versioned/core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.537866 versioned-0.4.2/versioned/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.4.2/versioned/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.4.2/versioned/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.538277 versioned-0.4.2/versioned/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.4.2/versioned/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.538877 versioned-0.4.2/versioned/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.4.2/versioned/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.537762 versioned-0.4.2/versioned.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-07 18:17:27.000000 versioned-0.4.2/versioned.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-07 18:17:27.000000 versioned-0.4.2/versioned.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-07 18:17:27.000000 versioned-0.4.2/versioned.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-07 18:17:27.000000 versioned-0.4.2/versioned.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-07 18:17:27.000000 versioned-0.4.2/versioned.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.960472 versioned-0.5.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.5.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.5.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.5.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3963 2023-07-14 20:42:02.960337 versioned-0.5.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2828 2023-07-13 01:42:39.000000 versioned-0.5.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4587 2023-07-14 20:41:46.000000 versioned-0.5.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.5.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.5.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.5.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.5.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      159 2023-07-14 20:41:46.000000 versioned-0.5.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-14 20:42:02.960519 versioned-0.5.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.5.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.957006 versioned-0.5.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1154 2023-07-14 20:41:46.000000 versioned-0.5.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-07-14 20:41:46.000000 versioned-0.5.1/tests/test_dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10411 2023-07-14 20:41:46.000000 versioned-0.5.1/tests/test_s3_and_dynamodb_backend.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    15087 2023-07-14 20:41:46.000000 versioned-0.5.1/tests/test_s3_only_backend.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.958465 versioned-0.5.1/versioned/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.5.1/versioned/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      472 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1959 2023-07-07 14:49:41.000000 versioned-0.5.1/versioned/bootstrap.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      383 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/compat.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      230 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/constants.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.959243 versioned-0.5.1/versioned/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4518 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.5.1/versioned/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17619 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/s3_and_dynamodb_backend.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    23254 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/s3_only_backend.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.959675 versioned-0.5.1/versioned/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.5.1/versioned/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.960152 versioned-0.5.1/versioned/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7573 2023-07-14 20:41:46.000000 versioned-0.5.1/versioned/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.5.1/versioned/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:42:02.959127 versioned-0.5.1/versioned.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3963 2023-07-14 20:42:02.000000 versioned-0.5.1/versioned.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      911 2023-07-14 20:42:02.000000 versioned-0.5.1/versioned.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-14 20:42:02.000000 versioned-0.5.1/versioned.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      281 2023-07-14 20:42:02.000000 versioned-0.5.1/versioned.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-14 20:42:02.000000 versioned-0.5.1/versioned.egg-info/top_level.txt
```

### Comparing `versioned-0.4.2/AUTHORS.rst` & `versioned-0.5.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.4.2/LICENSE.txt` & `versioned-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.4.2/PKG-INFO` & `versioned-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.4.2
+Version: 0.5.1
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.4.2#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.5.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -84,14 +84,18 @@
 ==============================================================================
 The version and alias best practice for immutable artifacts and deployment.
 
 Tutorial:
 
 - `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
 
+Learn why Blue / Green, Canary deployment and Rollback made easy with versioning and alias management.
+
+.. image:: https://github.com/MacHu-GWU/versioned-project/assets/6800411/57f7970e-3821-45a0-9deb-64890e04c129
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``versioned`` is released on PyPI, so all you need is to:
```

### Comparing `versioned-0.4.2/README.rst` & `versioned-0.5.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,18 @@
 ==============================================================================
 The version and alias best practice for immutable artifacts and deployment.
 
 Tutorial:
 
 - `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
 
+Learn why Blue / Green, Canary deployment and Rollback made easy with versioning and alias management.
+
+.. image:: https://github.com/MacHu-GWU/versioned-project/assets/6800411/57f7970e-3821-45a0-9deb-64890e04c129
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``versioned`` is released on PyPI, so all you need is to:
```

### Comparing `versioned-0.4.2/release-history.rst` & `versioned-0.5.1/release-history.rst`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,27 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.5.1 (2023-07-14)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add S3 only backend in ``s3_only_backend.py`` module. It doesn't require DynamoDB table.
+- the old ``core.py`` module is renamed to ``s3_and_dynamodb_backend.py`` module. The public API is not changed.
+- suggest to use ``from versioned import api as versioned``, then use ``versioned.s3_and_dynamodb_backend`` or ``versioned.s3_only_backend`` to access the backend.
+
+**Minor Improvements**
+
+- improve test for ``s3_and_dynamodb_backend``.
+
+
 0.4.2 (2023-07-07)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a bug that the ``purge_all`` method cannot delete DynamoDB items correctly when S3 doesn't have the artifacts.
```

### Comparing `versioned-0.4.2/requirements-doc.txt` & `versioned-0.5.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.4.2/setup.py` & `versioned-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.2/tests/test_api.py` & `versioned-0.5.1/tests/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 def test():
     _ = api
     _ = api.exc
     _ = api.DYNAMODB_TABLE_NAME
     _ = api.S3_PREFIX
     _ = api.LATEST_VERSION
     _ = api.VERSION_ZFILL
+    _ = api.METADATA_KEY_ARTIFACT_SHA256
     _ = api.Artifact
     _ = api.Alias
     _ = api.Repository
-    _ = api.Repository.get_artifact_s3path
     _ = api.Repository.put_artifact
     _ = api.Repository.get_artifact_version
     _ = api.Repository.list_artifact_versions
     _ = api.Repository.publish_artifact_version
     _ = api.Repository.delete_artifact_version
     _ = api.Repository.put_alias
     _ = api.Repository.get_alias
@@ -27,12 +27,15 @@
     _ = api.Repository.purge_all
     _ = api.Artifact.s3path
     _ = api.Artifact.get_content
     _ = api.Alias.s3path_version
     _ = api.Alias.get_version_content
     _ = api.Alias.s3path_secondary_version
     _ = api.Alias.get_secondary_version_content
+    _ = api.s3_and_dynamodb_backend
+    _ = api.s3_only_backend
+
 
 if __name__ == "__main__":
     from versioned.tests import run_cov_test
 
     run_cov_test(__file__, "versioned.api", preview=False)
```

### Comparing `versioned-0.4.2/tests/test_core.py` & `versioned-0.5.1/tests/test_s3_and_dynamodb_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,132 +3,74 @@
 import moto
 import pytest
 
 from s3pathlib import S3Path, context
 
 from versioned import exc
 from versioned import constants
-from versioned.dynamodb import encode_version
+from versioned.dynamodb import encode_version_sk
 from versioned.tests.mock_aws import BaseMockTest
-from versioned.core import Repository
+from versioned.s3_and_dynamodb_backend import Repository
 
 from rich import print as rprint
 
 
 class Test(BaseMockTest):
     use_mock = True
 
     mock_list = [
         moto.mock_sts,
         moto.mock_s3,
         moto.mock_dynamodb,
     ]
 
+    _mock_list = []
+
     repo: Repository = None
 
     @classmethod
     def setup_class_post_hook(cls):
         context.attach_boto_session(cls.bsm.boto_ses)
         cls.repo = Repository(
             aws_region=cls.bsm.aws_region,
             s3_bucket=f"{cls.bsm.aws_account_id}-{cls.bsm.aws_region}-artifacts",
             suffix=".txt",
         )
         cls.repo.bootstrap(cls.bsm)
 
-    def _test(self):
+    def _test_error(self):
         name = "deploy"
-        alias = "LIVE"
 
         self.repo.purge_all()
 
-        # ======================================================================
-        # Artifact
-        # ======================================================================
-        # --- test ArtifactNotFoundError ---
+        # --- test Artifact error ---
         # at this moment, no artifact exists
         with pytest.raises(exc.ArtifactNotFoundError):
             self.repo.publish_artifact_version(name=name)
 
         with pytest.raises(exc.ArtifactNotFoundError):
             self.repo.get_artifact_version(name=name)
 
         artifact_list = self.repo.list_artifact_versions(name=name)
         assert len(artifact_list) == 0
 
-        # put artifact
-        artifact = self.repo.put_artifact(
-            name=name,
-            content=b"v1",
-            content_type="text/plain",
-            metadata={"foo": "bar"},
-        )
-        # rprint(artifact)
-        # put artifact with the same content, S3 and Dynamodb should not changed
-        artifact = self.repo.put_artifact(name=name, content=b"v1")
-
-        def _assert_artifact(artifact):
-            assert artifact.name == name
-            assert artifact.version == constants.LATEST_VERSION
-            assert artifact.s3uri.endswith(constants.LATEST_VERSION + ".txt")
-            assert artifact.get_content(bsm=self.bsm) == b"v1"
-
-        _assert_artifact(artifact)
-
-        artifact = self.repo.get_artifact_version(name=name)
-        # rprint(artifact)
-        _assert_artifact(artifact)
-
-        artifact_list = self.repo.list_artifact_versions(name=name)
-        # rprint(artifact_list)
-        assert len(artifact_list) == 1
-        _assert_artifact(artifact_list[0])
-
-        artifact = self.repo.publish_artifact_version(name=name)
-        # rprint(artifact)
-        assert artifact.version == "1"
-        assert artifact.s3uri.endswith("1".zfill(constants.VERSION_ZFILL) + ".txt")
-        assert (
-            artifact.s3path.basename == str("1").zfill(constants.VERSION_ZFILL) + ".txt"
-        )
-        assert artifact.s3path.metadata["foo"] == "bar"
-        assert artifact.get_content(bsm=self.bsm) == b"v1"
-
-        # put artifact again
-        artifact = self.repo.put_artifact(name=name, content=b"v2")
-        # rprint(artifact)
-        assert artifact.version == constants.LATEST_VERSION
-        assert S3Path(artifact.s3uri).read_text(bsm=self.bsm) == "v2"
-
-        artifact = self.repo.publish_artifact_version(name=name)
-        # rprint(artifact)
-        assert artifact.version == "2"
-        s3path = S3Path(artifact.s3uri)
-        assert artifact.s3uri.endswith("2".zfill(constants.VERSION_ZFILL) + ".txt")
-        assert (
-            artifact.s3path.basename == str("2").zfill(constants.VERSION_ZFILL) + ".txt"
-        )
-        assert artifact.get_content(bsm=self.bsm) == b"v2"
+        # delete an non existing artifact version should always success for idempotency
+        self.repo.delete_artifact_version(name=name)
+        self.repo.delete_artifact_version(name=name, version=1)
 
-        artifact_list = self.repo.list_artifact_versions(name=name)
-        assert len(artifact_list) == 3
+        # --- test Alias error ---
+        alias = "LIVE"
 
-        # ======================================================================
-        # Artifact
-        # ======================================================================
-        # --- test raises error ---
         # try to put alias on non-exist artifact
         with pytest.raises(exc.ArtifactNotFoundError):
             self.repo.put_alias(name=name, alias=alias, version=999)
 
         # secondary_version_weight type is wrong
         with pytest.raises(TypeError):
-            self.repo.put_alias(
-                name=name, alias=alias, secondary_version=999
-            )
+            self.repo.put_alias(name=name, alias=alias, secondary_version=999)
 
         # secondary_version_weight type is wrong
         with pytest.raises(TypeError):
             self.repo.put_alias(
                 name=name,
                 alias=alias,
                 secondary_version=999,
@@ -172,21 +114,99 @@
                 secondary_version_weight=20,
             )
 
         # alias not exists
         with pytest.raises(exc.AliasNotFoundError):
             self.repo.get_alias(name=name, alias="Invalid")
 
+        alias_list = self.repo.list_aliases(name=name)
+        assert len(alias_list) == 0
+
+    def _test_artifact_and_alias(self):
+        name = "deploy"
+        alias = "LIVE"
+
+        self.repo.purge_all()
+
+        # ======================================================================
+        # Artifact
+        # ======================================================================
+        # put artifact
+        artifact = self.repo.put_artifact(
+            name=name,
+            content=b"v1",
+            content_type="text/plain",
+            metadata={"foo": "bar"},
+        )
+        # rprint(artifact)
+        expected_update_at = artifact.update_at
+
+        # put artifact with the same content, S3 and Dynamodb should not changed
+        artifact = self.repo.put_artifact(name=name, content=b"v1")
+        # rprint(artifact)
+
+        def _assert_artifact(artifact):
+            assert artifact.name == name
+            assert artifact.version == constants.LATEST_VERSION
+            assert artifact.update_at == expected_update_at
+            assert artifact.s3uri.endswith(constants.LATEST_VERSION + ".txt")
+            assert artifact.get_content(bsm=self.bsm) == b"v1"
+
+        _assert_artifact(artifact)
+
+        artifact = self.repo.get_artifact_version(name=name)
+        # rprint(artifact)
+        _assert_artifact(artifact)
+
+        artifact_list = self.repo.list_artifact_versions(name=name)
+        # rprint(artifact_list)
+        assert len(artifact_list) == 1
+        _assert_artifact(artifact_list[0])
+
+        artifact = self.repo.publish_artifact_version(name=name)
+        # rprint(artifact)
+        assert artifact.version == "1"
+        assert artifact.s3uri.endswith("1".zfill(constants.VERSION_ZFILL) + ".txt")
+        assert (
+            artifact.s3path.basename == str("1").zfill(constants.VERSION_ZFILL) + ".txt"
+        )
+        assert artifact.s3path.metadata["foo"] == "bar"
+        assert artifact.get_content(bsm=self.bsm) == b"v1"
+
+        # put artifact again
+        artifact = self.repo.put_artifact(name=name, content=b"v2")
+        # rprint(artifact)
+        assert artifact.version == constants.LATEST_VERSION
+        assert S3Path(artifact.s3uri).read_text(bsm=self.bsm) == "v2"
+
+        artifact = self.repo.publish_artifact_version(name=name)
+        # rprint(artifact)
+        assert artifact.version == "2"
+        s3path = S3Path(artifact.s3uri)
+        assert artifact.s3uri.endswith("2".zfill(constants.VERSION_ZFILL) + ".txt")
+        assert (
+            artifact.s3path.basename == str("2").zfill(constants.VERSION_ZFILL) + ".txt"
+        )
+        assert artifact.get_content(bsm=self.bsm) == b"v2"
+
+        artifact_list = self.repo.list_artifact_versions(name=name)
+        assert len(artifact_list) == 3
+
+        # ======================================================================
+        # Alias
+        # ======================================================================
         # put alias
         ali = self.repo.put_alias(name=name, alias=alias)
         # rprint(ali)
+        expected_update_at = ali.update_at
 
         def _assert_alias(ali):
             assert ali.name == name
             assert ali.alias == alias
+            assert ali.update_at == expected_update_at
             assert ali.version == constants.LATEST_VERSION
             assert ali.secondary_version is None
             assert ali.secondary_version_weight is None
             assert ali.version_s3uri.endswith(constants.LATEST_VERSION + ".txt")
             assert ali.secondary_version_s3uri is None
             assert ali.get_version_content(bsm=self.bsm) == b"v2"
 
@@ -209,19 +229,20 @@
             secondary_version_weight=20,
         )
         # rprint(ali)
 
         def _assert_alias(ali):
             assert ali.name == name
             assert ali.alias == alias
+            assert ali.update_at > expected_update_at
             assert ali.version == "1"
             assert ali.secondary_version == "2"
             assert ali.secondary_version_weight == 20
-            assert ali.version_s3uri.endswith(encode_version(1) + ".txt")
-            assert ali.secondary_version_s3uri.endswith(encode_version(2) + ".txt")
+            assert ali.version_s3uri.endswith(encode_version_sk(1) + ".txt")
+            assert ali.secondary_version_s3uri.endswith(encode_version_sk(2) + ".txt")
             assert ali.get_version_content(bsm=self.bsm) == b"v1"
             assert ali.get_secondary_version_content(bsm=self.bsm) == b"v2"
 
         _assert_alias(ali)
 
         ali = self.repo.get_alias(name=name, alias=alias)
         # rprint(ali)
@@ -266,14 +287,15 @@
         artifact_list = self.repo.list_artifact_versions(name=name)
         assert len(artifact_list) == 0
         ali_list = self.repo.list_aliases(name=name)
         assert len(ali_list) == 0
 
     def test(self):
         self.repo.connect_boto_session(self.bsm)
-        self._test()
+        self._test_error()
+        self._test_artifact_and_alias()
 
 
 if __name__ == "__main__":
     from versioned.tests import run_cov_test
 
-    run_cov_test(__file__, "versioned.core", preview=False)
+    run_cov_test(__file__, "versioned.s3_and_dynamodb_backend", preview=False)
```

### Comparing `versioned-0.4.2/versioned/bootstrap.py` & `versioned-0.5.1/versioned/bootstrap.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.2/versioned/core.py` & `versioned-0.5.1/versioned/s3_and_dynamodb_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,23 +60,25 @@
     Data class for alias.
 
     It is not the same as the underlying DynamodbItem, it is a public facing
     API data class.
 
     :param name: artifact name.
     :param alias: alias name. alias name cannot have hyphen
+    :param update_at: an utc datetime object when this artifact was updated
     :param version: artifact version. If ``None``, the latest version is used.
     :param secondary_version: see above.
     :param secondary_version_weight: an integer between 0 ~ 100.
     :param version_s3uri: s3uri of the primary artifact version of this alias.
     :param secondary_version_s3uri: s3uri of the secondary artifact version of this alias.
     """
 
     name: str
     alias: str
+    update_at: datetime
     version: str
     secondary_version: T.Optional[str]
     secondary_version_weight: T.Optional[int]
     version_s3uri: str
     secondary_version_s3uri: T.Optional[str]
 
     @property
@@ -105,14 +107,16 @@
         """
         return self.s3path_secondary_version.read_bytes(bsm=bsm)
 
 
 @dataclasses.dataclass
 class Repository:
     """
+    Repository class for artifact store.
+
     :param aws_region: the aws region of where the artifact store is.
     :param s3_bucket: the s3 bucket name of the artifact store.
     :param s3_prefix: the s3 prefix (folder path) of the artifact store.
     :param dynamodb_table_name: the dynamodb table name of the artifact metadata store.
     :param suffix: the file extension suffix of the artifact binary.
     """
 
@@ -125,26 +129,29 @@
     @property
     def s3dir_artifact_store(self) -> S3Path:
         """
         Return the s3dir of the artifact store folder.
         """
         return S3Path(self.s3_bucket).joinpath(self.s3_prefix).to_dir()
 
-    def get_artifact_s3path(self, name: str, version: str) -> S3Path:
+    def _get_artifact_s3path(self, name: str, version: str) -> S3Path:
         return self.s3dir_artifact_store.joinpath(
             name,
-            f"{dynamodb.encode_version(version)}{self.suffix}",
+            f"{dynamodb.encode_version_sk(version)}{self.suffix}",
         )
 
     def bootstrap(
         self,
         bsm: BotoSesManager,
         dynamodb_write_capacity_units: T.Optional[int] = None,
         dynamodb_read_capacity_units: T.Optional[int] = None,
     ):
+        """
+        Create necessary backend resources for the artifact store.
+        """
         bootstrap(
             bsm=bsm,
             aws_region=self.aws_region,
             bucket_name=self.s3_bucket,
             dynamodb_table_name=self.dynamodb_table_name,
             dynamodb_write_capacity_units=dynamodb_write_capacity_units,
             dynamodb_read_capacity_units=dynamodb_read_capacity_units,
@@ -169,33 +176,33 @@
         return Alias
 
     def _get_artifact_object(
         self,
         artifact: dynamodb.Artifact,
     ) -> Artifact:
         dct = artifact.to_dict()
-        dct["s3uri"] = self.get_artifact_s3path(
+        dct["s3uri"] = self._get_artifact_s3path(
             name=artifact.name,
             version=artifact.version,
         ).uri
         return Artifact(**dct)
 
     def _get_alias_object(
         self,
         alias: dynamodb.Alias,
     ) -> Alias:
         dct = alias.to_dict()
-        dct["version_s3uri"] = self.get_artifact_s3path(
+        dct["version_s3uri"] = self._get_artifact_s3path(
             name=alias.name,
             version=alias.version,
         ).uri
         if alias.secondary_version is None:
             dct["secondary_version_s3uri"] = None
         else:
-            dct["secondary_version_s3uri"] = self.get_artifact_s3path(
+            dct["secondary_version_s3uri"] = self._get_artifact_s3path(
                 name=alias.name,
                 version=alias.secondary_version,
             ).uri
         return Alias(**dct)
 
     def connect_boto_session(self, bsm: BotoSesManager):
         """
@@ -225,46 +232,49 @@
         :param content: binary artifact content.
         :param metadata: optional metadata of the s3 object.
         :param tags: optional tags of the s3 object.
         """
         artifact = self._artifact_class.new(name=name)
         artifact_sha256 = hashes.of_bytes(content)
         artifact.sha256 = artifact_sha256
-        s3path = self.get_artifact_s3path(name=name, version=constants.LATEST_VERSION)
+        s3path = self._get_artifact_s3path(name=name, version=constants.LATEST_VERSION)
 
         # do nothing if the content is not changed
         if s3path.exists():
             if s3path.metadata["artifact_sha256"] == artifact_sha256:
+                artifact.update_at = s3path.last_modified_at
                 return self._get_artifact_object(artifact=artifact)
 
         final_metadata = dict(
             artifact_name=name,
             artifact_sha256=artifact_sha256,
         )
         if metadata is not NOTHING:
             final_metadata.update(metadata)
         s3path.write_bytes(
             content,
             metadata=final_metadata,
             content_type=content_type,
             tags=tags,
         )
+        s3path.head_object()
+        artifact.update_at = s3path.last_modified_at
         artifact.save()
         return self._get_artifact_object(artifact=artifact)
 
     def _get_artifact_dynamodb_item(
         self,
         artifact_class: T.Type[dynamodb.Artifact],
         name: str,
         version: T.Union[int, str],
     ) -> dynamodb.Artifact:
         try:
             artifact = artifact_class.get(
                 hash_key=name,
-                range_key=dynamodb.encode_version(version),
+                range_key=dynamodb.encode_version_sk(version),
             )
             if artifact.is_deleted:
                 raise exc.ArtifactNotFoundError(
                     f"name = {name!r}, version = {version!r}"
                 )
             return artifact
         except artifact_class.DoesNotExist:
@@ -323,26 +333,32 @@
         Artifact = self._artifact_class
         artifacts = list(
             Artifact.query(hash_key=name, scan_index_forward=False, limit=2)
         )
         if len(artifacts) == 0:
             raise exc.ArtifactNotFoundError(f"name = {name!r}")
         elif len(artifacts) == 1:
-            new_version = "1"
+            new_version = dynamodb.encode_version(1)
         else:
             new_version = str(int(artifacts[1].version) + 1)
-        artifact = Artifact.new(name=name, version=new_version)
-        artifact.sha256 = artifacts[0].sha256
-        artifact.save()
-        s3path_old = self.get_artifact_s3path(
+
+        # copy artifact from latest to the new version
+        s3path_old = self._get_artifact_s3path(
             name=name,
             version=constants.LATEST_VERSION,
         )
-        s3path_new = self.get_artifact_s3path(name=name, version=new_version)
+        s3path_new = self._get_artifact_s3path(name=name, version=new_version)
         s3path_old.copy_to(s3path_new)
+        s3path_new.head_object()
+
+        # create artifact object
+        artifact = Artifact.new(name=name, version=new_version)
+        artifact.sha256 = artifacts[0].sha256
+        artifact.update_at = s3path_new.last_modified_at
+        artifact.save()
         return self._get_artifact_object(artifact=artifact)
 
     def delete_artifact_version(
         self,
         name: str,
         version: T.Optional[T.Union[int, str]] = None,
     ):
@@ -387,28 +403,39 @@
         :param name: artifact name.
         :param alias: alias name. alias name cannot have hyphen
         :param version: artifact version. If ``None``, the latest version is used.
         :param secondary_version: see above.
         :param secondary_version_weight: an integer between 0 ~ 100.
         """
         # validate argument
+        # todo: add more alias naming convention rules
         if "-" in alias:  # pragma: no cover
             raise ValueError("alias cannot have hyphen")
 
+        version = dynamodb.encode_version(version)
+
         if secondary_version is not None:
+            secondary_version = dynamodb.encode_version(secondary_version)
             if not isinstance(secondary_version_weight, int):
                 raise TypeError("secondary_version_weight must be int")
             if not (0 <= secondary_version_weight < 100):
                 raise ValueError("secondary_version_weight must be 0 <= x < 100")
+            if version == secondary_version:
+                raise ValueError(
+                    f"version {version!r} and secondary_version {secondary_version!r} "
+                    f"cannot be the same!"
+                )
 
         # ensure the artifact exists
         Artifact = self._artifact_class
-        if version is None:
-            version = constants.LATEST_VERSION
-        self._get_artifact_dynamodb_item(Artifact, name=name, version=version)
+        self._get_artifact_dynamodb_item(
+            Artifact,
+            name=name,
+            version=version,
+        )
         if secondary_version is not None:
             self._get_artifact_dynamodb_item(
                 Artifact,
                 name=name,
                 version=secondary_version,
             )
 
@@ -416,15 +443,14 @@
         alias = Alias.new(
             name=name,
             alias=alias,
             version=version,
             secondary_version=secondary_version,
             secondary_version_weight=secondary_version_weight,
         )
-
         alias.save()
         return self._get_alias_object(alias=alias)
 
     def get_alias(
         self,
         name: str,
         alias: str,
@@ -435,15 +461,15 @@
         :param name: artifact name.
         :param alias: alias name. alias name cannot have hyphen
         """
         Alias = self._alias_class
         try:
             return self._get_alias_object(
                 alias=Alias.get(
-                    hash_key=dynamodb.encode_alias_key(name),
+                    hash_key=dynamodb.encode_alias_pk(name),
                     range_key=alias,
                 ),
             )
         except Alias.DoesNotExist:
             raise exc.AliasNotFoundError(f"name = {name!r}, alias = {alias!r}")
 
     def list_aliases(
@@ -454,15 +480,15 @@
         Returns a list of aliases for an artifact.
 
         :param name: artifact name.
         """
         Alias = self._alias_class
         return [
             self._get_alias_object(alias=alias)
-            for alias in Alias.query(hash_key=dynamodb.encode_alias_key(name))
+            for alias in Alias.query(hash_key=dynamodb.encode_alias_pk(name))
         ]
 
     def delete_alias(
         self,
         name: str,
         alias: str,
     ):
@@ -479,25 +505,25 @@
         """
         Completely delete all artifacts and aliases of the given artifact name.
         This operation is irreversible. It will remove all related S3 artifacts
         and DynamoDB items.
 
         :param name: artifact name.
         """
-        s3path = self.get_artifact_s3path(name=name, version=constants.LATEST_VERSION)
+        s3path = self._get_artifact_s3path(name=name, version=constants.LATEST_VERSION)
         s3dir = s3path.parent
         s3dir.delete()
 
         Artifact = self._artifact_class
         Alias = self._alias_class
         with Artifact.batch_write() as batch:
             for artifact in Artifact.query(hash_key=name):
                 batch.delete(artifact)
         with Alias.batch_write() as batch:
-            for alias in Alias.query(hash_key=dynamodb.encode_alias_key(name)):
+            for alias in Alias.query(hash_key=dynamodb.encode_alias_pk(name)):
                 batch.delete(alias)
 
     def purge_all(self):
         """
         Completely delete all artifacts and aliases in this Repository
         This operation is irreversible. It will remove all related S3 artifacts
         and DynamoDB items.
```

### Comparing `versioned-0.4.2/versioned/dynamodb.py` & `versioned-0.5.1/versioned/dynamodb.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,25 +9,63 @@
 
 from pynamodb.models import Model
 from pynamodb.attributes import UnicodeAttribute
 from pynamodb.attributes import NumberAttribute
 from pynamodb.attributes import BooleanAttribute
 from pynamodb.attributes import UTCDateTimeAttribute
 
-from .constants import LATEST_VERSION, VERSION_ZFILL
+from .constants import (
+    LATEST_VERSION,
+    VERSION_ZFILL,
+)
 
 
 def get_utc_now() -> datetime:
     return datetime.utcnow().replace(tzinfo=timezone.utc)
 
 
-def encode_version(version: T.Union[int, str]) -> str:
-    return str(version).zfill(VERSION_ZFILL)
+def encode_version(version: T.Optional[T.Union[int, str]]) -> str:
+    """
+    Encode human readable "version" into the data class field "version".
+
+    Example::
+
+        None    -> LATEST
+        LATEST  -> LATEST
+        1       -> 1
+        000001  -> 1
+    """
+    if version is None:
+        return LATEST_VERSION
+    else:
+        return str(version).lstrip("0")
+
+
+def encode_version_sk(version: T.Optional[T.Union[int, str]]) -> str:
+    """
+    Get the Dynamodb sort key of a version.
+
+    Example::
+
+        None    -> LATEST
+        LATEST  -> LATEST
+        999999  -> 999999
+        ...
+        2       -> 000002
+        1       -> 000001
+    """
+    return encode_version(version).zfill(VERSION_ZFILL)
+
 
-def encode_alias_key(name: str) -> str:
+def encode_alias_pk(name: str) -> str:
+    """
+    Get the Dynamodb partition key of an alias.
+
+    :param name: artifact name
+    """
     return f"__{name}-alias"
 
 
 class Base(Model):
     pk: T.Union[str, UnicodeAttribute] = UnicodeAttribute(hash_key=True)
     sk: T.Union[str, UnicodeAttribute] = UnicodeAttribute(
         range_key=True,
@@ -35,32 +73,31 @@
     )
 
 
 class Artifact(Base):
     """
     Todo: docstring
     """
-    update_at: T.Union[datetime, UTCDateTimeAttribute] = UTCDateTimeAttribute(
-        default=get_utc_now,
-    )
+
+    update_at: T.Union[datetime, UTCDateTimeAttribute] = UTCDateTimeAttribute()
     is_deleted: T.Union[bool, BooleanAttribute] = BooleanAttribute(
         default=False,
     )
     sha256: T.Union[str, UnicodeAttribute] = UnicodeAttribute()
 
     @classmethod
     def new(
         cls,
         name: str,
         version: T.Optional[T.Union[int, str]] = None,
     ) -> "Artifact":
         if version is None:
             return cls(pk=name)
         else:
-            return cls(pk=name, sk=encode_version(version))
+            return cls(pk=name, sk=encode_version_sk(version))
 
     @property
     def name(self) -> str:
         return self.pk
 
     @property
     def version(self) -> str:
@@ -75,14 +112,17 @@
         }
 
 
 class Alias(Base):
     """
     Todo: docstring
     """
+    update_at: T.Union[datetime, UTCDateTimeAttribute] = UTCDateTimeAttribute(
+        default=get_utc_now,
+    )
     version: T.Union[str, UnicodeAttribute] = UnicodeAttribute()
     secondary_version: T.Optional[T.Union[str, UnicodeAttribute]] = UnicodeAttribute(
         null=True,
     )
     secondary_version_weight: T.Optional[
         T.Union[int, NumberAttribute]
     ] = NumberAttribute(
@@ -96,22 +136,21 @@
         alias: str,
         version: T.Optional[T.Union[int, str]] = None,
         secondary_version: T.Optional[T.Union[int, str]] = None,
         secondary_version_weight: T.Optional[int] = None,
     ):
         if version is None:
             version = LATEST_VERSION
-        version = encode_version(version)
+        version = encode_version_sk(version)
         if secondary_version is not None:
-            secondary_version = encode_version(secondary_version)
+            secondary_version = encode_version_sk(secondary_version)
             if version == secondary_version:
                 raise ValueError
-
         return cls(
-            pk=encode_alias_key(name),
+            pk=encode_alias_pk(name),
             sk=alias,
             version=version,
             secondary_version=secondary_version,
             secondary_version_weight=secondary_version_weight,
         )
 
     @property
@@ -126,11 +165,12 @@
         if self.secondary_version is None:
             secondary_version = None
         else:
             secondary_version = self.secondary_version.lstrip("0")
         return {
             "name": self.name,
             "alias": self.alias,
+            "update_at": self.update_at,
             "version": self.version.lstrip("0"),
             "secondary_version": secondary_version,
             "secondary_version_weight": self.secondary_version_weight,
         }
```

### Comparing `versioned-0.4.2/versioned/paths.py` & `versioned-0.5.1/versioned/paths.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.2/versioned/tests/mock_aws.py` & `versioned-0.5.1/versioned/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.2/versioned/vendor/hashes.py` & `versioned-0.5.1/versioned/vendor/hashes.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,7 +268,8 @@
             s="".join(hashes),
             algo=algo,
             hexdigest=hexdigest,
         )
 
 
 hashes = Hashes()
+hashes.use_sha256()
```

### Comparing `versioned-0.4.2/versioned/vendor/pytest_cov_helper.py` & `versioned-0.5.1/versioned/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.2/versioned.egg-info/PKG-INFO` & `versioned-0.5.1/versioned.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.4.2
+Version: 0.5.1
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.4.2#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.5.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -84,14 +84,18 @@
 ==============================================================================
 The version and alias best practice for immutable artifacts and deployment.
 
 Tutorial:
 
 - `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
 
+Learn why Blue / Green, Canary deployment and Rollback made easy with versioning and alias management.
+
+.. image:: https://github.com/MacHu-GWU/versioned-project/assets/6800411/57f7970e-3821-45a0-9deb-64890e04c129
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``versioned`` is released on PyPI, so all you need is to:
```

### Comparing `versioned-0.4.2/versioned.egg-info/SOURCES.txt` & `versioned-0.5.1/versioned.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 requirements-automation.txt
 requirements-dev.txt
 requirements-doc.txt
 requirements-test.txt
 requirements.txt
 setup.py
 tests/test_api.py
-tests/test_core.py
+tests/test_dynamodb.py
+tests/test_s3_and_dynamodb_backend.py
+tests/test_s3_only_backend.py
 versioned/__init__.py
 versioned/_version.py
 versioned/api.py
 versioned/bootstrap.py
+versioned/compat.py
 versioned/constants.py
-versioned/core.py
 versioned/dynamodb.py
 versioned/exc.py
 versioned/paths.py
+versioned/s3_and_dynamodb_backend.py
+versioned/s3_only_backend.py
 versioned.egg-info/PKG-INFO
 versioned.egg-info/SOURCES.txt
 versioned.egg-info/dependency_links.txt
 versioned.egg-info/requires.txt
 versioned.egg-info/top_level.txt
 versioned/docs/__init__.py
 versioned/tests/__init__.py
```

