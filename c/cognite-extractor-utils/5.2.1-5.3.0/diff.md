# Comparing `tmp/cognite_extractor_utils-5.2.1.tar.gz` & `tmp/cognite_extractor_utils-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_utils-5.2.1.tar", max compression
+gzip compressed data, was "cognite_extractor_utils-5.3.0.tar", max compression
```

## Comparing `cognite_extractor_utils-5.2.1.tar` & `cognite_extractor_utils-5.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    10173 2023-07-06 06:33:06.189123 cognite_extractor_utils-5.2.1/LICENSE
--rw-r--r--   0        0        0     4090 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/README.md
--rw-r--r--   0        0        0      739 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/__init__.py
--rw-r--r--   0        0        0     1558 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/_inner_util.py
--rw-r--r--   0        0        0    15974 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/base.py
--rw-r--r--   0        0        0     2861 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/__init__.py
--rw-r--r--   0        0        0     4739 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/_util.py
--rw-r--r--   0        0        0    19910 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/elements.py
--rw-r--r--   0        0        0     9545 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/loaders.py
--rw-r--r--   0        0        0     1061 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/exceptions.py
--rw-r--r--   0        0        0    14929 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/metrics.py
--rw-r--r--   0        0        0     1108 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/middleware.py
--rw-r--r--   0        0        0        0 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/py.typed
--rw-r--r--   0        0        0    17829 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/statestore.py
--rw-r--r--   0        0        0     3054 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/__init__.py
--rw-r--r--   0        0        0     4983 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/_base.py
--rw-r--r--   0        0        0     3865 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/_metrics.py
--rw-r--r--   0        0        0     6118 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/events.py
--rw-r--r--   0        0        0    11674 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/files.py
--rw-r--r--   0        0        0     7021 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/raw.py
--rw-r--r--   0        0        0    26582 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/time_series.py
--rw-r--r--   0        0        0     7476 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader_extractor.py
--rw-r--r--   0        0        0     1146 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader_types.py
--rw-r--r--   0        0        0    14284 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/util.py
--rw-r--r--   0        0        0     2066 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/pyproject.toml
--rw-r--r--   0        0        0     5406 1970-01-01 00:00:00.000000 cognite_extractor_utils-5.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/LICENSE
+-rw-r--r--   0        0        0     4090 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/README.md
+-rw-r--r--   0        0        0      739 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/cognite/extractorutils/__init__.py
+-rw-r--r--   0        0        0     1558 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/cognite/extractorutils/_inner_util.py
+-rw-r--r--   0        0        0    15974 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/cognite/extractorutils/base.py
+-rw-r--r--   0        0        0     2861 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/__init__.py
+-rw-r--r--   0        0        0     4739 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/_util.py
+-rw-r--r--   0        0        0    19910 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/elements.py
+-rw-r--r--   0        0        0     9545 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/loaders.py
+-rw-r--r--   0        0        0     1061 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/exceptions.py
+-rw-r--r--   0        0        0    14929 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/metrics.py
+-rw-r--r--   0        0        0     1108 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/middleware.py
+-rw-r--r--   0        0        0        0 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/py.typed
+-rw-r--r--   0        0        0    17829 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/statestore.py
+-rw-r--r--   0        0        0     3091 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/__init__.py
+-rw-r--r--   0        0        0     5169 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/_base.py
+-rw-r--r--   0        0        0     4300 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/_metrics.py
+-rw-r--r--   0        0        0     5814 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/assets.py
+-rw-r--r--   0        0        0     5895 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/events.py
+-rw-r--r--   0        0        0    11674 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/files.py
+-rw-r--r--   0        0        0     7021 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/raw.py
+-rw-r--r--   0        0        0    26582 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/time_series.py
+-rw-r--r--   0        0        0     7476 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader_extractor.py
+-rw-r--r--   0        0        0     1146 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader_types.py
+-rw-r--r--   0        0        0    14284 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/util.py
+-rw-r--r--   0        0        0     2067 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 cognite_extractor_utils-5.3.0/PKG-INFO
```

### Comparing `cognite_extractor_utils-5.2.1/LICENSE` & `cognite_extractor_utils-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/README.md` & `cognite_extractor_utils-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/__init__.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """
 Cognite extractor utils is a Python package that simplifies the development of new extractors.
 """
 
-__version__ = "5.2.1"
+__version__ = "5.3.0"
 from .base import Extractor
```

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/_inner_util.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/_inner_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/base.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/__init__.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/_util.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/elements.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/elements.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/loaders.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/loaders.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/exceptions.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/metrics.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/middleware.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/middleware.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/statestore.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/statestore.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/__init__.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
 This will call the ``start()`` and ``stop()`` methods automatically.
 
 You can also trigger uploads after a given amount of data is added, by using the ``max_queue_size`` keyword argument
 instead. If both are used, the condition being met first will trigger the upload.
 """
 
+from .assets import AssetUploadQueue
 from .events import EventUploadQueue
 from .files import BytesUploadQueue, FileUploadQueue
 from .raw import RawUploadQueue
 from .time_series import (
     DataPoint,
     DataPointList,
     SequenceUploadQueue,
```

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/_base.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,23 @@
             ensure_upload (bool): (Optional). Call upload one last time after shutting down thread to ensure empty
                 upload queue.
         """
         self.cancellation_token.set()
         if ensure_upload:
             self.upload()
 
+    def __len__(self) -> int:
+        """
+        The size of the upload queue
+
+        Returns:
+            Number of events in queue
+        """
+        return self.upload_queue_size
+
 
 @dataclass(frozen=True)
 class TimestampedObject:
     payload: Any
     created: Arrow
```

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/_metrics.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,7 +72,13 @@
 BYTES_UPLOADER_QUEUED = Counter("cognite_bytes_uploader_queued", "Total number of frames queued")
 BYTES_UPLOADER_WRITTEN = Counter("cognite_bytes_uploader_written", "Total number of frames written")
 BYTES_UPLOADER_QUEUE_SIZE = Gauge("cognite_bytes_uploader_queue_size", "Internal queue size")
 BYTES_UPLOADER_LATENCY = Histogram(
     "cognite_bytes_uploader_latency",
     "Distribution of times in minutes records spend in the queue",
 )
+ASSETS_UPLOADER_QUEUED = Counter("cognite_assets_uploader_queued", "Total number of assets queued")
+ASSETS_UPLOADER_WRITTEN = Counter("cognite_assets_uploader_written", "Total number of assets written")
+ASSETS_UPLOADER_QUEUE_SIZE = Gauge("cognite_assets_uploader_queue_size", "Internal queue size")
+ASSETS_UPLOADER_LATENCY = Histogram(
+    "cognite_assets_uploader_latency", "Distribution of times in minutes records spend in queue"
+)
```

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/events.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #  limitations under the License.
 
 import threading
 from types import TracebackType
 from typing import Callable, List, Optional, Type
 
 import arrow
-from requests import ConnectionError
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Event
 from cognite.client.exceptions import CogniteAPIError, CogniteDuplicatedError
 from cognite.extractorutils.uploader._base import (
     RETRIES,
     RETRY_BACKOFF_FACTOR,
@@ -168,16 +167,7 @@
 
         Args:
             exc_type: Exception type
             exc_val: Exception value
             exc_tb: Traceback
         """
         self.stop()
-
-    def __len__(self) -> int:
-        """
-        The size of the upload queue
-
-        Returns:
-            Number of events in queue
-        """
-        return self.upload_queue_size
```

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/files.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/files.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/raw.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/time_series.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader_extractor.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader_types.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader_types.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/cognite/extractorutils/util.py` & `cognite_extractor_utils-5.3.0/cognite/extractorutils/util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.1/pyproject.toml` & `cognite_extractor_utils-5.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-utils"
-version = "5.2.1"
+version = "5.3.0"
 description = "Utilities for easier development of extractors for CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/python-extractor-utils"
 
 packages = [
@@ -62,27 +62,27 @@
 pyyaml = ">=5.3.0, <7"
 dacite = "^1.6.0"
 psutil = "^5.7.0"
 decorator = "^5.1.1"
 more-itertools = "^9.0.0"
 typing-extensions = ">=3.7.4, <5"
 python-dotenv = "^1.0.0"
-jq = [{version = "^1.3.0", platform = "macos"}, {version = "^1.3.0", platform = "linux"}]
+jq = [{version = "^1.3.0", platform = "darwin"}, {version = "^1.3.0", platform = "linux"}]
 
 [tool.poetry.extras]
 experimental = ["cognite-sdk-experimental"]
 
 [tool.poetry.group.dev.dependencies]
-black = "23.3.0"
+black = "23.7.0"
 mypy = "1.4.1"
-ruff = "^0.0.277"
+ruff = "^0.0.278"
 pytest = "^7.0.0"
 pytest-cov = "^4.0.0"
 sphinx = "^6.0.0"
-sphinx-rtd-theme = "^1.0.0"
+sphinx-rtd-theme = "^1.2.2"
 pre-commit = "^3.3.0"
 SecretStorage = "^3.1.2"
 twine = "^4.0.0"
 pytest-order = "^1.0.1"
 parameterized = "*"
 
 [build-system]
```

### Comparing `cognite_extractor_utils-5.2.1/PKG-INFO` & `cognite_extractor_utils-5.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-utils
-Version: 5.2.1
+Version: 5.3.0
 Summary: Utilities for easier development of extractors for CDF
 Home-page: https://github.com/cognitedata/python-extractor-utils
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: experimental
 Requires-Dist: arrow (>=1.0.0,<2.0.0)
 Requires-Dist: cognite-sdk (>=6.0,<7)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
+Requires-Dist: jq (>=1.3.0,<2.0.0) ; sys_platform == "darwin"
 Requires-Dist: jq (>=1.3.0,<2.0.0) ; sys_platform == "linux"
-Requires-Dist: jq (>=1.3.0,<2.0.0) ; sys_platform == "macos"
 Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
 Requires-Dist: prometheus-client (>0.7.0,<=1.0.0)
 Requires-Dist: psutil (>=5.7.0,<6.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=5.3.0,<7)
 Requires-Dist: typing-extensions (>=3.7.4,<5)
 Project-URL: Repository, https://github.com/cognitedata/python-extractor-utils
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 5.2.1 Summary:
+Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 5.3.0 Summary:
 Utilities for easier development of extractors for CDF Home-page: https://
 github.com/cognitedata/python-extractor-utils License: Apache-2.0 Author:
 Mathias Lohne Author-email: mathias.lohne@cognite.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: experimental Requires-Dist: arrow
 (>=1.0.0,<2.0.0) Requires-Dist: cognite-sdk (>=6.0,<7) Requires-Dist: dacite
 (>=1.6.0,<2.0.0) Requires-Dist: decorator (>=5.1.1,<6.0.0) Requires-Dist: jq
-(>=1.3.0,<2.0.0) ; sys_platform == "linux" Requires-Dist: jq (>=1.3.0,<2.0.0) ;
-sys_platform == "macos" Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
+(>=1.3.0,<2.0.0) ; sys_platform == "darwin" Requires-Dist: jq (>=1.3.0,<2.0.0)
+; sys_platform == "linux" Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
 Requires-Dist: prometheus-client (>0.7.0,<=1.0.0) Requires-Dist: psutil
 (>=5.7.0,<6.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-Dist:
 pyyaml (>=5.3.0,<7) Requires-Dist: typing-extensions (>=3.7.4,<5) Project-URL:
 Repository, https://github.com/cognitedata/python-extractor-utils Description-
 Content-Type: text/markdown [Cognite_logo] Cognite Python `extractor-utils`
 ================================ [![Build Status](https://github.com/
 cognitedata/python-extractor-utils/workflows/release/badge.svg)](https://
```

