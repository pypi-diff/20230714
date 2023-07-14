# Comparing `tmp/starpoint-0.1.0.tar.gz` & `tmp/starpoint-0.1.2.tar.gz`

## Comparing `starpoint-0.1.0.tar` & `starpoint-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 starpoint-0.1.0/.coverage
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 starpoint-0.1.0/dev-requirements.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 starpoint-0.1.0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starpoint-0.1.0/starpoint/__init__.py
--rw-r--r--   0        0        0    17838 2020-02-02 00:00:00.000000 starpoint-0.1.0/starpoint/db.py
--rw-r--r--   0        0        0    26905 2020-02-02 00:00:00.000000 starpoint-0.1.0/tests/test_db.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 starpoint-0.1.0/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 starpoint-0.1.0/LICENSE
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 starpoint-0.1.0/README.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 starpoint-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 starpoint-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    47395 2020-02-02 00:00:00.000000 starpoint-0.1.2/dev-requirements.txt
+-rw-r--r--   0        0        0    34194 2020-02-02 00:00:00.000000 starpoint-0.1.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starpoint-0.1.2/starpoint/__init__.py
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 starpoint-0.1.2/starpoint/db.py
+-rw-r--r--   0        0        0    26903 2020-02-02 00:00:00.000000 starpoint-0.1.2/tests/test_db.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 starpoint-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 starpoint-0.1.2/LICENSE
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 starpoint-0.1.2/README.md
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 starpoint-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 starpoint-0.1.2/PKG-INFO
```

### Comparing `starpoint-0.1.0/starpoint/db.py` & `starpoint-0.1.2/starpoint/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 import openai
 import requests
 import validators
 
 LOGGER = logging.getLogger(__name__)
 
+COLLECTIONS_PATH = "/api/v1/collections"
 DOCUMENTS_PATH = "/api/v1/documents"
 QUERY_PATH = "/api/v1/query"
 INFER_SCHEMA_PATH = "/api/v1/infer_schema"
 API_HEADER_KEY = "x-starpoint-key"
 
-READER_URL = "https://grimoire.starpoint.ai"
-COMPOSER_URL = "https://warden.starpoint.ai"
+READER_URL = "https://reader.starpoint.ai"
+WRITER_URL = "https://writer.starpoint.ai"
 
-HEALTH_CHECK_MESSAGE = "hello"
+HEALTH_CHECK_MESSAGE = "hello."
 
 NO_HOST_ERROR = "No host value provided. A host must be provided."
 NO_COLLECTION_VALUE_ERROR = (
     "Please provide at least one value for either collection_id or collection_name."
 )
 MULTI_COLLECTION_VALUE_ERROR = (
     "Please only provide either collection_id or collection_name in your request."
@@ -33,14 +34,15 @@
 EMBEDDING_METADATA_LENGTH_MISMATCH_WARNING = (
     "The length of the embeddings and document_metadata provided are different. There may be a mismatch "
     "between embeddings and the expected document metadata length; this may cause undesired collection insert or update."
 )
 NO_EMBEDDING_DATA_FOUND = (
     "No embedding data found in the embedding response from OpenAI."
 )
+DIMENSIONALITY_ERROR = "Dimensionality must be greater than 0."
 
 
 def _build_header(api_key: UUID, additional_headers: Optional[Dict[str, str]] = None):
     header = {API_HEADER_KEY: str(api_key)}
     if additional_headers is not None:
         header.update(additional_headers)
     return header
@@ -82,15 +84,15 @@
 
 
 class Writer(object):
     """docstring for Writer"""
 
     def __init__(self, api_key: UUID, host: Optional[str] = None):
         if host is None:
-            host = COMPOSER_URL
+            host = WRITER_URL
 
         self.host = _set_and_validate_host(host)
         self.api_key = api_key
 
     def delete(
         self,
         documents: List[UUID],
@@ -254,14 +256,83 @@
             LOGGER.error(
                 f"Request failed with status code {response.status_code} "
                 f"and the following message:\n{response.text}"
             )
             return {}
         return response.json()
 
+    def create_collection(
+        self, collection_name: str, dimensionality: int
+    ) -> Dict[Any, Any]:
+        """
+        dict(
+            name="collection_name_example",
+            dimensionality=1024,
+        )
+        """
+
+        if dimensionality <= 0:
+            raise ValueError(DIMENSIONALITY_ERROR)
+
+        request_data = dict(
+            name=collection_name,
+            dimensionality=dimensionality,
+        )
+        try:
+            response = requests.post(
+                url=f"{self.host}{COLLECTIONS_PATH}",
+                json=request_data,
+                headers=_build_header(
+                    api_key=self.api_key,
+                    additional_headers={"Content-Type": "application/json"},
+                ),
+            )
+        except requests.exceptions.SSLError as e:
+            LOGGER.error(SSL_ERROR_MSG)
+            raise e
+
+        if not response.ok:
+            LOGGER.error(
+                f"Request failed with status code {response.status_code} "
+                f"and the following message:\n{response.text}"
+            )
+            return {}
+        return response.json()
+
+    def delete_collection(self, collection_id: UUID) -> Dict[Any, Any]:
+        """
+        dict(
+            collection_id="collection_id_example",
+        )
+        """
+
+        request_data = dict(
+            collection_id=collection_id,
+        )
+        try:
+            response = requests.delete(
+                url=f"{self.host}{COLLECTIONS_PATH}",
+                json=request_data,
+                headers=_build_header(
+                    api_key=self.api_key,
+                    additional_headers={"Content-Type": "application/json"},
+                ),
+            )
+        except requests.exceptions.SSLError as e:
+            LOGGER.error(SSL_ERROR_MSG)
+            raise e
+
+        if not response.ok:
+            LOGGER.error(
+                f"Request failed with status code {response.status_code} "
+                f"and the following message:\n{response.text}"
+            )
+            return {}
+        return response.json()
+
 
 class Reader(object):
     """docstring for Reader"""
 
     def __init__(self, api_key: UUID, host: Optional[str] = None):
         if host is None:
             host = READER_URL
@@ -442,14 +513,27 @@
     ) -> Dict[Any, Any]:
         return self.writer.update(
             documents=documents,
             collection_id=collection_id,
             collection_name=collection_name,
         )
 
+    def create_collection(
+        self, collection_name: str, dimensionality: int
+    ) -> Dict[Any, Any]:
+        return self.writer.create_collection(
+            collection_name=collection_name,
+            dimensionality=dimensionality,
+        )
+
+    def delete_collection(self, collection_id: UUID) -> Dict[Any, Any]:
+        return self.writer.delete_collection(
+            collection_id=collection_id,
+        )
+
     """
     OpenAI convenience wrappers
     """
 
     def init_openai(
         self,
         openai_key: Optional[str] = None,
```

### Comparing `starpoint-0.1.0/tests/test_db.py` & `starpoint-0.1.2/tests/test_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 @patch("starpoint.db._check_host_health")
 def writer(host_health_mock: MagicMock, api_uuid: UUID) -> db.Writer:
     return db.Writer(api_uuid)
 
 
 def test_writer_default_init(writer: db.Writer, api_uuid: UUID):
     assert writer.host
-    assert writer.host == db.COMPOSER_URL
+    assert writer.host == db.WRITER_URL
     assert writer.api_key == api_uuid
 
 
 def test_writer_init_non_default_host(api_uuid: UUID):
     test_host = "http://www.example.com"
     writer = db.Writer(api_key=api_uuid, host=test_host)
```

### Comparing `starpoint-0.1.0/LICENSE` & `starpoint-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.0/PKG-INFO` & `starpoint-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: starpoint
-Version: 0.1.0
+Version: 0.1.2
 Summary: SDK for Starpoint DB
 Project-URL: Homepage, https://github.com/starpoint-ai/sdk
 Project-URL: Bug Tracker, https://github.com/starpoint-ai/sdk/issues
 Author-email: pointable <package-maintainers@pointable.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: openai~=0.27
 Requires-Dist: requests~=2.28
 Requires-Dist: validators~=0.20
+Provides-Extra: dev
+Requires-Dist: pip-tools~=6.14; extra == 'dev'
+Requires-Dist: pre-commit~=3.3; extra == 'dev'
+Requires-Dist: pytest-cov~=4.1; extra == 'dev'
+Requires-Dist: pytest~=7.3; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Starpoint AI SDK
 
 ## Installation
 
 `pip install starpoint`
@@ -39,7 +45,19 @@
   },
 ]
 
 // Instead of collection_name you can also use collection_id="COLLECTION_ID"
 client.insert(documents=documents, collection_name="COLLECTION_NAME")
 
 ```
+
+## Contributing
+
+Make sure you have installed dev requirements
+```
+pip install -r dev-requirements.txt
+```
+
+Unit tests should be passing. You can run them via
+```
+pytest ./tests
+```
```

