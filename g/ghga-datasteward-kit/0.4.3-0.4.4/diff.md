# Comparing `tmp/ghga_datasteward_kit-0.4.3.tar.gz` & `tmp/ghga_datasteward_kit-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_datasteward_kit-0.4.3.tar", last modified: Thu Jul  6 11:59:00 2023, max compression
+gzip compressed data, was "ghga_datasteward_kit-0.4.4.tar", last modified: Fri Jul 14 08:29:56 2023, max compression
```

## Comparing `ghga_datasteward_kit-0.4.3.tar` & `ghga_datasteward_kit-0.4.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.508344 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6589 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/batch_s3_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/catalog_accession_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/file_ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20809 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.508344 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/fixtures/ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/fixtures/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/test_file_ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/test_s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/test_size_adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.916890 ghga_datasteward_kit-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-14 08:29:56.916890 ghga_datasteward_kit-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.912890 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6589 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/batch_s3_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/catalog_accession_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.912890 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/file_ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22083 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.912890 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-14 08:29:56.916890 ghga_datasteward_kit-0.4.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.912890 ghga_datasteward_kit-0.4.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.916890 ghga_datasteward_kit-0.4.4/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/fixtures/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/fixtures/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/test_file_ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/test_s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/test_size_adjustment.py
```

### Comparing `ghga_datasteward_kit-0.4.3/LICENSE` & `ghga_datasteward_kit-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/PKG-INFO` & `ghga_datasteward_kit-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_datasteward_kit
-Version: 0.4.3
+Version: 0.4.4
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Home-page: https://github.com/ghga-de/ghga-datasteward-kit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_datasteward_kit-0.4.3/README.md` & `ghga_datasteward_kit-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/__init__.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A utils package for GHGA data stewards."""
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
```

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/__main__.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/batch_s3_upload.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/batch_s3_upload.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/catalog_accession_generator.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/catalog_accession_generator.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/__init__.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/file.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/file.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/main.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/main.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/metadata.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/config.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/config.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/file_ingest.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/file_ingest.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/loading.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/loading.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/main.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/main.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/metadata.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/models.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/models.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/s3_upload.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/s3_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
 import asyncio
 import logging
 import math
 import os
 import subprocess  # nosec
 import sys
+from contextlib import contextmanager
 from functools import partial
 from io import BufferedReader
 from pathlib import Path
 from time import time
-from typing import Generator
+from typing import Generator, Iterator
 from uuid import uuid4
 
 import crypt4gh.header  # type: ignore
 import crypt4gh.keys  # type: ignore
 import crypt4gh.lib  # type: ignore
-from ghga_connector.core.client import HttpxClientState, httpx_client
-from ghga_connector.core.file_operations import read_file_parts
+import httpx
 from hexkit.providers.s3 import S3Config, S3ObjectStorage  # type: ignore
 from nacl.bindings import crypto_aead_chacha20poly1305_ietf_encrypt
 from pydantic import BaseSettings, Field, SecretStr, validator
 
 from ghga_datasteward_kit import models
 from ghga_datasteward_kit.utils import load_config_yaml
 
@@ -401,14 +401,62 @@
                 upload_id=self.upload_id,
                 bucket_id=self.config.bucket_id,
                 object_id=self.file_id,
             )
             raise exc
 
 
+class HttpxClientState:
+    """Helper class to make max_retries user configurable"""
+
+    max_retries: int
+
+    @classmethod
+    def configure(cls, max_retries: int):
+        """Configure client with exponential backoff retry (using httpx's 0.5 default)"""
+
+        # can't be negative - should we log this?
+        cls.max_retries = max(0, max_retries)
+
+
+@contextmanager
+def httpx_client():
+    """Yields a context manager httpx client and closes it afterward"""
+
+    transport = httpx.HTTPTransport(retries=HttpxClientState.max_retries)
+
+    with httpx.Client(transport=transport) as client:
+        yield client
+
+
+def read_file_parts(
+    file: BufferedReader, *, part_size: int, from_part: int = 1
+) -> Iterator[bytes]:
+    """
+    Returns an iterator to iterate through file parts of the given size (in bytes).
+
+    By default it start with the first part but you may also start from a specific part
+    in the middle of the file using the `from_part` argument. This might be useful to
+    resume an interrupted reading process.
+
+    Please note: opening and closing of the file MUST happen outside of this function.
+    """
+
+    initial_offset = part_size * (from_part - 1)
+    file.seek(initial_offset)
+
+    while True:
+        file_part = file.read(part_size)
+
+        if len(file_part) == 0:
+            return
+
+        yield file_part
+
+
 def objectstorage(config: Config):
     """Configure S3 and return S3 DAO"""
     s3_config = S3Config(
         s3_endpoint_url=config.s3_endpoint_url.get_secret_value(),
         s3_access_key_id=config.s3_access_key_id.get_secret_value(),
         s3_secret_access_key=config.s3_secret_access_key.get_secret_value(),
     )
```

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/utils.py` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/PKG-INFO` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-datasteward-kit
-Version: 0.4.3
+Version: 0.4.4
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Home-page: https://github.com/ghga-de/ghga-datasteward-kit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/SOURCES.txt` & `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/setup.cfg` & `ghga_datasteward_kit-0.4.4/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 	Topic :: Scientific/Engineering :: Bio-Informatics
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
+	crypt4gh==1.6
 	hexkit[mongodb,s3]==0.10.0
-	ghga-connector==0.3.5
 	ghga-transpiler==1.0.3
 	metldata==0.3.6
 python_requires = >= 3.9
 
 [options.entry_points]
 console_scripts = 
 	ghga-datasteward-kit = ghga_datasteward_kit.__main__:run
```

### Comparing `ghga_datasteward_kit-0.4.3/setup.py` & `ghga_datasteward_kit-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/tests/fixtures/__init__.py` & `ghga_datasteward_kit-0.4.4/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/tests/fixtures/config.py` & `ghga_datasteward_kit-0.4.4/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/tests/fixtures/ingest.py` & `ghga_datasteward_kit-0.4.4/tests/fixtures/ingest.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/tests/fixtures/metadata.py` & `ghga_datasteward_kit-0.4.4/tests/fixtures/metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/tests/fixtures/utils.py` & `ghga_datasteward_kit-0.4.4/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/tests/test_file_ingest.py` & `ghga_datasteward_kit-0.4.4/tests/test_file_ingest.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/tests/test_metadata.py` & `ghga_datasteward_kit-0.4.4/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/tests/test_s3_upload.py` & `ghga_datasteward_kit-0.4.4/tests/test_s3_upload.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.3/tests/test_size_adjustment.py` & `ghga_datasteward_kit-0.4.4/tests/test_size_adjustment.py`

 * *Files identical despite different names*

