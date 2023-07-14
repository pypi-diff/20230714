# Comparing `tmp/strangeworks_core-0.2.1.tar.gz` & `tmp/strangeworks_core-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_core-0.2.1.tar", max compression
+gzip compressed data, was "strangeworks_core-0.2.2.tar", max compression
```

## Comparing `strangeworks_core-0.2.1.tar` & `strangeworks_core-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      655 2023-06-08 19:51:40.847974 strangeworks_core-0.2.1/README.md
--rw-r--r--   0        0        0      891 2023-06-08 19:51:57.848067 strangeworks_core-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      109 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/__init__.py
--rw-r--r--   0        0        0       19 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/batch/__init__.py
--rw-r--r--   0        0        0    12246 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/batch/utils.py
--rw-r--r--   0        0        0       19 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/__init__.py
--rw-r--r--   0        0        0      647 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/base.py
--rw-r--r--   0        0        0     3340 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/config.py
--rw-r--r--   0        0        0      874 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/defaults.py
--rw-r--r--   0        0        0     1846 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/env.py
--rw-r--r--   0        0        0     6262 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/file.py
--rw-r--r--   0        0        0       19 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/errors/__init__.py
--rw-r--r--   0        0        0     2613 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/errors/error.py
--rw-r--r--   0        0        0       19 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/platform/__init__.py
--rw-r--r--   0        0        0     2457 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/platform/auth.py
--rw-r--r--   0        0        0     4880 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/platform/gql.py
--rw-r--r--   0        0        0    10844 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/platform/rest_client.py
--rw-r--r--   0        0        0     3275 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/platform/transport.py
--rw-r--r--   0        0        0       19 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/__init__.py
--rw-r--r--   0        0        0     3572 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/backend.py
--rw-r--r--   0        0        0     2024 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/file.py
--rw-r--r--   0        0        0      647 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/func.py
--rw-r--r--   0        0        0     5748 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/job.py
--rw-r--r--   0        0        0      760 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/machine.py
--rw-r--r--   0        0        0     1088 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/product.py
--rw-r--r--   0        0        0     2732 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/resource.py
--rw-r--r--   0        0        0      553 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/utils.py
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 strangeworks_core-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      655 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/README.md
+-rw-r--r--   0        0        0      914 2023-07-14 18:30:40.408649 strangeworks_core-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/batch/__init__.py
+-rw-r--r--   0        0        0    12246 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/batch/utils.py
+-rw-r--r--   0        0        0       19 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/base.py
+-rw-r--r--   0        0        0     3340 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/config.py
+-rw-r--r--   0        0        0      874 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/defaults.py
+-rw-r--r--   0        0        0     1846 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/env.py
+-rw-r--r--   0        0        0     6262 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/file.py
+-rw-r--r--   0        0        0       19 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/errors/__init__.py
+-rw-r--r--   0        0        0     2613 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/errors/error.py
+-rw-r--r--   0        0        0       19 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/platform/__init__.py
+-rw-r--r--   0        0        0     2457 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/platform/auth.py
+-rw-r--r--   0        0        0     4880 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/platform/gql.py
+-rw-r--r--   0        0        0    10844 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/platform/rest_client.py
+-rw-r--r--   0        0        0     3275 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/platform/transport.py
+-rw-r--r--   0        0        0       19 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/__init__.py
+-rw-r--r--   0        0        0     3572 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/backend.py
+-rw-r--r--   0        0        0     2024 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/file.py
+-rw-r--r--   0        0        0      647 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/func.py
+-rw-r--r--   0        0        0     6517 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/job.py
+-rw-r--r--   0        0        0      760 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/machine.py
+-rw-r--r--   0        0        0     1088 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/product.py
+-rw-r--r--   0        0        0     2732 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/resource.py
+-rw-r--r--   0        0        0      553 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/utils.py
+-rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 strangeworks_core-0.2.2/PKG-INFO
```

### Comparing `strangeworks_core-0.2.1/README.md` & `strangeworks_core-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/pyproject.toml` & `strangeworks_core-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 
 name = "strangeworks-core"
-version = "0.2.1"
+version = "0.2.2"
 
 description = "Strangeworks Core provides the infrastructure to interact with the platform."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_core"}]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.2"
 tomlkit = "^0.11.6"
 gql = "^3.4.0"
 requests-toolbelt = "^1.0.0"
 dill = "^0.3.6"
+deprecated = "^1.2.14"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 pytest-cov = "^4.0.0"
```

### Comparing `strangeworks_core-0.2.1/strangeworks_core/batch/utils.py` & `strangeworks_core-0.2.2/strangeworks_core/batch/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/config/base.py` & `strangeworks_core-0.2.2/strangeworks_core/config/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/config/config.py` & `strangeworks_core-0.2.2/strangeworks_core/config/config.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/config/defaults.py` & `strangeworks_core-0.2.2/strangeworks_core/config/defaults.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/config/env.py` & `strangeworks_core-0.2.2/strangeworks_core/config/env.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/config/file.py` & `strangeworks_core-0.2.2/strangeworks_core/config/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/errors/error.py` & `strangeworks_core-0.2.2/strangeworks_core/errors/error.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/platform/auth.py` & `strangeworks_core-0.2.2/strangeworks_core/platform/auth.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/platform/gql.py` & `strangeworks_core-0.2.2/strangeworks_core/platform/gql.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/platform/rest_client.py` & `strangeworks_core-0.2.2/strangeworks_core/platform/rest_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/platform/transport.py` & `strangeworks_core-0.2.2/strangeworks_core/platform/transport.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/types/backend.py` & `strangeworks_core-0.2.2/strangeworks_core/types/backend.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/types/file.py` & `strangeworks_core-0.2.2/strangeworks_core/types/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/types/func.py` & `strangeworks_core-0.2.2/strangeworks_core/types/func.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/types/job.py` & `strangeworks_core-0.2.2/strangeworks_core/types/job.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """jobs.py."""
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
+from deprecated import deprecated
+
 from strangeworks_core.types.file import File
 from strangeworks_core.types.resource import Resource
 from strangeworks_core.utils import str_to_datetime
 
 
 class Status(str, Enum):
     """Enumeration of possible job statuses."""
@@ -77,15 +79,15 @@
         self.slug: str = slug
         self.job_id: Optional[str] = id
         self.external_identifier: Optional[str] = externalIdentifier
 
         self.status: Optional[Status] = (
             Status(status.strip().upper()) if status else None
         )
-        self.is_terminal_state: Optional[bool] = isTerminalState
+        self._is_terminal_state: Optional[bool] = isTerminalState
         self.remote_status: Optional[str] = remoteStatus
         self.job_data_schema: Optional[str] = jobDataSchema
         self.job_data: Optional[Dict[str, Any]] = jobData
         self.date_created: Optional[datetime] = (
             str_to_datetime(dateCreated) if dateCreated else None
         )
         self.date_updated: Optional[datetime] = (
@@ -118,24 +120,45 @@
         Return
         ------
         "Job"
             a job object.
         """
         return cls(**res)
 
+    @deprecated(
+        reason=(
+            "This method is deprecated and will be removed. Use is_terminal_state instead."  # noqa E501
+        )
+    )
     def is_complete(self) -> bool:
         """Check if job is in terminal state.
 
         deprecated method, kept to limit number of changes
         required for extension SDKs
         """
-        return self.is_terminal_state
+        return self._is_terminal_state
+
+    @property
+    def is_terminal_state(self) -> bool:
+        """Return if job is in terminal state.
+
+        If _is_terminal_state was set, return that value. Otherwise, return True if
+        self.status is in [Status.CANCELLED, Status.COMPLETED, Status.FAILED],
+        otherwise False.
+        """
+        return (
+            self._is_terminal_state
+            if self._is_terminal_state is not None
+            else self.status in [Status.CANCELLED, Status.COMPLETED, Status.FAILED]
+        )
 
 
 class JobFile:
+    """Object which represents a Strangeworks platform job file entry."""
+
     def __init__(
         self,
         file: Dict[str, Any],
         sortWeight: Optional[int] = None,
         isPublic: Optional[bool] = None,
         **kwargs,
     ) -> None:
```

### Comparing `strangeworks_core-0.2.1/strangeworks_core/types/machine.py` & `strangeworks_core-0.2.2/strangeworks_core/types/machine.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/types/product.py` & `strangeworks_core-0.2.2/strangeworks_core/types/product.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/types/resource.py` & `strangeworks_core-0.2.2/strangeworks_core/types/resource.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/strangeworks_core/utils.py` & `strangeworks_core-0.2.2/strangeworks_core/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.1/PKG-INFO` & `strangeworks_core-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: strangeworks-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: Strangeworks Core provides the infrastructure to interact with the platform.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: deprecated (>=1.2.14,<2.0.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: tomlkit (>=0.11.6,<0.12.0)
 Description-Content-Type: text/markdown
```

