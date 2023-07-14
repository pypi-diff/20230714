# Comparing `tmp/spellbook_serve_client-0.0.0a0.tar.gz` & `tmp/spellbook_serve_client-0.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spellbook_serve_client-0.0.0a0.tar", max compression
+gzip compressed data, was "spellbook_serve_client-0.0.0a1.tar", max compression
```

## Comparing `spellbook_serve_client-0.0.0a0.tar` & `spellbook_serve_client-0.0.0a1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      958 2023-07-13 21:52:42.334478 spellbook_serve_client-0.0.0a0/README.md
--rw-r--r--   0        0        0      785 2023-07-13 21:52:42.335277 spellbook_serve_client-0.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     1058 2023-07-13 21:52:42.336945 spellbook_serve_client-0.0.0a0/spellbook_serve_client/__init__.py
--rw-r--r--   0        0        0     5223 2023-07-13 21:52:42.337687 spellbook_serve_client-0.0.0a0/spellbook_serve_client/api_engine.py
--rw-r--r--   0        0        0    17935 2023-07-13 20:04:00.902936 spellbook_serve_client-0.0.0a0/spellbook_serve_client/client.py
--rw-r--r--   0        0        0     6110 2023-07-13 21:52:42.338374 spellbook_serve_client-0.0.0a0/spellbook_serve_client/completion.py
--rw-r--r--   0        0        0     8036 2023-07-13 21:52:42.339007 spellbook_serve_client-0.0.0a0/spellbook_serve_client/data_types.py
--rw-r--r--   0        0        0     1533 2023-07-13 21:46:02.300116 spellbook_serve_client-0.0.0a0/spellbook_serve_client/errors.py
--rw-r--r--   0        0        0     3184 2023-07-13 21:52:42.339582 spellbook_serve_client-0.0.0a0/spellbook_serve_client/fine_tuning.py
--rw-r--r--   0        0        0     8026 2023-07-13 20:04:00.903346 spellbook_serve_client-0.0.0a0/spellbook_serve_client/types.py
--rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 spellbook_serve_client-0.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-14 08:40:45.809471 spellbook_serve_client-0.0.0a1/README.md
+-rw-r--r--   0        0        0      785 2023-07-14 08:41:35.249647 spellbook_serve_client-0.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1112 2023-07-14 08:41:35.255611 spellbook_serve_client-0.0.0a1/spellbook_serve_client/__init__.py
+-rw-r--r--   0        0        0     5588 2023-07-14 08:35:22.194557 spellbook_serve_client-0.0.0a1/spellbook_serve_client/api_engine.py
+-rw-r--r--   0        0        0    17935 2023-07-13 20:04:00.902936 spellbook_serve_client-0.0.0a1/spellbook_serve_client/client.py
+-rw-r--r--   0        0        0     6032 2023-07-14 08:35:22.195470 spellbook_serve_client-0.0.0a1/spellbook_serve_client/completion.py
+-rw-r--r--   0        0        0     8036 2023-07-13 21:52:42.339007 spellbook_serve_client-0.0.0a1/spellbook_serve_client/data_types.py
+-rw-r--r--   0        0        0     1533 2023-07-13 21:46:02.300116 spellbook_serve_client-0.0.0a1/spellbook_serve_client/errors.py
+-rw-r--r--   0        0        0     3179 2023-07-14 08:35:22.196251 spellbook_serve_client-0.0.0a1/spellbook_serve_client/fine_tuning.py
+-rw-r--r--   0        0        0     2168 2023-07-14 08:35:22.196784 spellbook_serve_client-0.0.0a1/spellbook_serve_client/model.py
+-rw-r--r--   0        0        0     8026 2023-07-13 20:04:00.903346 spellbook_serve_client-0.0.0a1/spellbook_serve_client/types.py
+-rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 spellbook_serve_client-0.0.0a1/PKG-INFO
```

### Comparing `spellbook_serve_client-0.0.0a0/README.md` & `spellbook_serve_client-0.0.0a1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Spellbook Serve
 
 The Spellbook Serve Python library provides a convenient way of interfacing with a
 `spellbook-serve` endpoint running on
-[Scale Spellbook Serve](https://spellbook.readme.io/docs/) or on your own infrastructure.
+[Scale Spellbook Serve](https://scaleapi.github.io/spellbook-serve/) or on your own infrastructure.
 
 ## Get Started
 
 ### Install
 
 ```shell
 pip install spellbook-serve-client
@@ -22,14 +22,19 @@
 `SPELLBOOK_SERVE_BASE_PATH` environment variable to the base URL of your
 self-hosted `spellbook-serve` endpoint.
 
 ```python
 from spellbook_serve_client import Completion
 
 response = Completion.create(
-    model_name="llama-7b-text-generation-inference",
+    model_name="llama-7b",
     prompt="Hello, my name is",
     max_new_tokens=10,
     temperature=0.2,
 )
 print(response.outputs[0].text)
 ```
+
+## Documentation
+
+Documentation is available at
+[https://scaleapi.github.io/spellbook-serve/](https://scaleapi.github.io/spellbook-serve/).
```

### Comparing `spellbook_serve_client-0.0.0a0/pyproject.toml` & `spellbook_serve_client-0.0.0a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "spellbook-serve-client"
-version = "0.0.0.alpha0"
+version = "0.0.0.alpha1"
 description = "Spellbok Serve Python Client"
 license = "Apache-2.0"
 authors = ["Phil Chen <phil.chen@scale.com>"]
 maintainers = ["Phil Chen <phil.chen@scale.com>"]
 readme = "README.md"
-homepage = "https://github.com/scaleapi/spellbook-serve"
+homepage = "https://scaleapi.github.io/spellbook-serve/"
 repository = "https://github.com/scaleapi/spellbook-serve"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = "^1.10"
 aiohttp = "^3.8"
```

### Comparing `spellbook_serve_client-0.0.0a0/spellbook_serve_client/__init__.py` & `spellbook_serve_client-0.0.0a1/spellbook_serve_client/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.0"
+__version__ = "0.0.0.alpha1"
 
 from spellbook_serve_client.completion import Completion
 from spellbook_serve_client.data_types import (
     CancelFineTuneJobResponse,
     CompletionOutput,
     CompletionStreamOutput,
     CompletionStreamV1Response,
@@ -24,7 +24,8 @@
     CreateFineTuneJobRequest,
     CreateFineTuneJobResponse,
     GetFineTuneJobResponse,
     ListFineTuneJobResponse,
     TaskStatus,
 )
 from spellbook_serve_client.fine_tuning import FineTune
+from spellbook_serve_client.model import Model
```

### Comparing `spellbook_serve_client-0.0.0a0/spellbook_serve_client/api_engine.py` & `spellbook_serve_client-0.0.0a1/spellbook_serve_client/api_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 import json
 import os
+from functools import wraps
 from typing import Any, AsyncIterable, Dict, Iterator, Optional
 
 import requests
 from aiohttp import BasicAuth, ClientSession, ClientTimeout
 from spellbook_serve_client.errors import parse_error
 
 SCALE_API_KEY = os.getenv("SCALE_API_KEY")
 SPELLBOOK_API_URL = "https://api.spellbook.scale.com"
 SPELLBOOK_SERVE_BASE_PATH = os.getenv("SPELLBOOK_SERVE_BASE_PATH", SPELLBOOK_API_URL)
+DEFAULT_TIMEOUT: int = 10
 
 
 def get_api_key() -> str:
     return SCALE_API_KEY or "root"
 
 
+def assert_self_hosted(func):
+    @wraps(func)
+    def inner(*args, **kwargs):
+        if SPELLBOOK_API_URL == SPELLBOOK_SERVE_BASE_PATH:
+            raise ValueError(
+                "This feature is only available for self-hosted users."
+            )
+        return func(*args, **kwargs)
+
+    return inner
+
+
 class APIEngine:
     @classmethod
     def validate_api_key(cls):
         if SPELLBOOK_API_URL == SPELLBOOK_SERVE_BASE_PATH and not SCALE_API_KEY:
             raise ValueError(
                 "You must set SCALE_API_KEY in your environment to to use the Spellbook Serve API."
             )
```

### Comparing `spellbook_serve_client-0.0.0a0/spellbook_serve_client/client.py` & `spellbook_serve_client-0.0.0a1/spellbook_serve_client/client.py`

 * *Files identical despite different names*

### Comparing `spellbook_serve_client-0.0.0a0/spellbook_serve_client/completion.py` & `spellbook_serve_client-0.0.0a1/spellbook_serve_client/completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,28 @@
     Completion API. This API is used to generate text completions.
 
     Example:
         ```python
         from spellbook_serve_client import Completion
 
         response = Completion.create(
-            model_name="llama-7b-text-generation-inference",
+            model_name="llama-7b",
             prompt="Hello, my name is",
             max_new_tokens=10,
             temperature=0.2,
         )
         print(response.outputs[0].text)
         ```
 
     Example:
         ```python
         from spellbook_serve_client import Completion
 
         response_stream = Completion.create(
-            model_name="llama-7b-text-generation-inference",
+            model_name="llama-7b",
             prompt="Hello, my name is",
             max_new_tokens=10,
             temperature=0.2,
             stream=True,
         )
         for response in response_stream:
             print(response.output.text)
@@ -43,15 +43,15 @@
 
     Example:
         ```python
         from spellbook_serve_client import Completion
 
         async def main():
             response_stream = await Completion.acreate(
-                model_name="llama-7b-text-generation-inference",
+                model_name="llama-7b",
                 prompt="Hello, my name is",
                 max_new_tokens=10,
                 temperature=0.2,
                 stream=True,
             )
             async for response in response_stream:
                 print(response.output.text)
```

### Comparing `spellbook_serve_client-0.0.0a0/spellbook_serve_client/data_types.py` & `spellbook_serve_client-0.0.0a1/spellbook_serve_client/data_types.py`

 * *Files identical despite different names*

### Comparing `spellbook_serve_client-0.0.0a0/spellbook_serve_client/errors.py` & `spellbook_serve_client-0.0.0a1/spellbook_serve_client/errors.py`

 * *Files identical despite different names*

### Comparing `spellbook_serve_client-0.0.0a0/spellbook_serve_client/fine_tuning.py` & `spellbook_serve_client-0.0.0a1/spellbook_serve_client/fine_tuning.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from typing import Dict
 
-from spellbook_serve_client.api_engine import APIEngine
+from spellbook_serve_client.api_engine import APIEngine, DEFAULT_TIMEOUT
 from spellbook_serve_client.data_types import (
     CancelFineTuneJobResponse,
     CreateFineTuneJobRequest,
     CreateFineTuneJobResponse,
     GetFineTuneJobResponse,
     ListFineTuneJobResponse,
 )
 
-DEFAULT_TIMEOUT = 10
-
 
 class FineTune(APIEngine):
     """
     FineTune API. This API is used to fine-tune models.
     """
 
     @classmethod
```

### Comparing `spellbook_serve_client-0.0.0a0/spellbook_serve_client/types.py` & `spellbook_serve_client-0.0.0a1/spellbook_serve_client/types.py`

 * *Files identical despite different names*

### Comparing `spellbook_serve_client-0.0.0a0/PKG-INFO` & `spellbook_serve_client-0.0.0a1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: spellbook-serve-client
-Version: 0.0.0a0
+Version: 0.0.0a1
 Summary: Spellbok Serve Python Client
-Home-page: https://github.com/scaleapi/spellbook-serve
+Home-page: https://scaleapi.github.io/spellbook-serve/
 License: Apache-2.0
 Author: Phil Chen
 Author-email: phil.chen@scale.com
 Maintainer: Phil Chen
 Maintainer-email: phil.chen@scale.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 Project-URL: Repository, https://github.com/scaleapi/spellbook-serve
 Description-Content-Type: text/markdown
 
 # Spellbook Serve
 
 The Spellbook Serve Python library provides a convenient way of interfacing with a
 `spellbook-serve` endpoint running on
-[Scale Spellbook Serve](https://spellbook.readme.io/docs/) or on your own infrastructure.
+[Scale Spellbook Serve](https://scaleapi.github.io/spellbook-serve/) or on your own infrastructure.
 
 ## Get Started
 
 ### Install
 
 ```shell
 pip install spellbook-serve-client
@@ -46,15 +46,20 @@
 `SPELLBOOK_SERVE_BASE_PATH` environment variable to the base URL of your
 self-hosted `spellbook-serve` endpoint.
 
 ```python
 from spellbook_serve_client import Completion
 
 response = Completion.create(
-    model_name="llama-7b-text-generation-inference",
+    model_name="llama-7b",
     prompt="Hello, my name is",
     max_new_tokens=10,
     temperature=0.2,
 )
 print(response.outputs[0].text)
 ```
 
+## Documentation
+
+Documentation is available at
+[https://scaleapi.github.io/spellbook-serve/](https://scaleapi.github.io/spellbook-serve/).
+
```

