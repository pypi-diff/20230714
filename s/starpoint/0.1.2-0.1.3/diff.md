# Comparing `tmp/starpoint-0.1.2.tar.gz` & `tmp/starpoint-0.1.3.tar.gz`

## Comparing `starpoint-0.1.2.tar` & `starpoint-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    47395 2020-02-02 00:00:00.000000 starpoint-0.1.2/dev-requirements.txt
--rw-r--r--   0        0        0    34194 2020-02-02 00:00:00.000000 starpoint-0.1.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starpoint-0.1.2/starpoint/__init__.py
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 starpoint-0.1.2/starpoint/db.py
--rw-r--r--   0        0        0    26903 2020-02-02 00:00:00.000000 starpoint-0.1.2/tests/test_db.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 starpoint-0.1.2/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 starpoint-0.1.2/LICENSE
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 starpoint-0.1.2/README.md
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 starpoint-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 starpoint-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    47395 2020-02-02 00:00:00.000000 starpoint-0.1.3/dev-requirements.txt
+-rw-r--r--   0        0        0    34194 2020-02-02 00:00:00.000000 starpoint-0.1.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starpoint-0.1.3/starpoint/__init__.py
+-rw-r--r--   0        0        0    20425 2020-02-02 00:00:00.000000 starpoint-0.1.3/starpoint/db.py
+-rw-r--r--   0        0        0    26784 2020-02-02 00:00:00.000000 starpoint-0.1.3/tests/test_db.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 starpoint-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 starpoint-0.1.3/LICENSE
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 starpoint-0.1.3/README.md
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 starpoint-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 starpoint-0.1.3/PKG-INFO
```

### Comparing `starpoint-0.1.2/dev-requirements.txt` & `starpoint-0.1.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.2/requirements.txt` & `starpoint-0.1.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.2/starpoint/db.py` & `starpoint-0.1.3/starpoint/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             LOGGER.error(
                 f"Request failed with status code {response.status_code} "
                 f"and the following message:\n{response.text}"
             )
             return {}
         return response.json()
 
-    def transpose_and_insert(
+    def column_insert(
         self,
         embeddings: List[float],
         document_metadatas: List[Dict[Any, Any]],
         collection_id: Optional[UUID] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
         if len(embeddings) != len(document_metadatas):
@@ -461,22 +461,22 @@
     ) -> Dict[Any, Any]:
         return self.writer.insert(
             documents=documents,
             collection_id=collection_id,
             collection_name=collection_name,
         )
 
-    def transpose_and_insert(
+    def column_insert(
         self,
         embeddings: List[float],
         document_metadatas: List[Dict[Any, Any]],
         collection_id: Optional[UUID] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
-        return self.writer.transpose_and_insert(
+        return self.writer.column_insert(
             embeddings=embeddings,
             document_metadatas=document_metadatas,
             collection_id=collection_id,
             collection_name=collection_name,
         )
 
     def query(
@@ -594,15 +594,15 @@
             else:
                 document_metadatas = [{"input": data} for data in input_data]
 
         # Return the embedding response no matter what issues/bugs we might run into in the sdk
         try:
             sorted_embedding_data = sorted(embedding_data, key=lambda x: x["index"])
             embeddings = map(lambda x: x.get("embedding"), sorted_embedding_data)
-            self.transpose_and_insert(
+            self.column_insert(
                 embeddings=embeddings,
                 document_metadatas=document_metadatas,
                 collection_id=collection_id,
                 collection_name=collection_name,
             )
         except Exception as e:
             LOGGER.error(
```

### Comparing `starpoint-0.1.2/tests/test_db.py` & `starpoint-0.1.3/tests/test_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,115 +273,115 @@
     with pytest.raises(SSLError, match="mock exception"):
         writer.insert(documents=[uuid4()], collection_name="mock_collection_name")
 
     logger_mock.error.assert_called_once_with(db.SSL_ERROR_MSG)
 
 
 @patch("starpoint.db.Writer.insert")
-def test_writer_transpose_and_insert(insert_mock: MagicMock, writer: db.Writer):
+def test_writer_column_insert(insert_mock: MagicMock, writer: db.Writer):
     test_embeddings = [0.88, 0.71]
     test_document_metadatas = [{"mock": "metadata"}, {"mock2": "metadata2"}]
     expected_insert_document = [
         {
             "embedding": test_embeddings[0],
             "metadata": test_document_metadatas[0],
         },
         {
             "embedding": test_embeddings[1],
             "metadata": test_document_metadatas[1],
         },
     ]
 
-    writer.transpose_and_insert(
+    writer.column_insert(
         embeddings=test_embeddings, document_metadatas=test_document_metadatas
     )
 
     insert_mock.assert_called_once_with(
         document=expected_insert_document,
         collection_id=None,
         collection_name=None,
     )
 
 
 @patch("starpoint.db.Writer.insert")
-def test_writer_transpose_and_insert_collection_id_collection_name_passed_through(
+def test_writer_column_insert_collection_id_collection_name_passed_through(
     insert_mock: MagicMock, writer: db.Writer
 ):
     test_embeddings = [0.88]
     test_document_metadatas = [{"mock": "metadata"}]
     expected_insert_document = [
         {
             "embedding": test_embeddings[0],
             "metadata": test_document_metadatas[0],
         },
     ]
     expected_collection_id = "mock_id"
     expected_collection_name = "mock_name"
 
-    writer.transpose_and_insert(
+    writer.column_insert(
         embeddings=test_embeddings,
         document_metadatas=test_document_metadatas,
         collection_id=expected_collection_id,
         collection_name=expected_collection_name,
     )
 
     insert_mock.assert_called_once_with(
         document=expected_insert_document,
         collection_id=expected_collection_id,
         collection_name=expected_collection_name,
     )
 
 
 @patch("starpoint.db.Writer.insert")
-def test_writer_transpose_and_insert_shorter_metadatas_length(
+def test_writer_column_insert_shorter_metadatas_length(
     insert_mock: MagicMock, writer: db.Writer, monkeypatch: MonkeyPatch
 ):
     test_embeddings = [0.88, 0.71]
     test_document_metadatas = [{"mock": "metadata"}]
     expected_insert_document = [
         {
             "embedding": test_embeddings[0],
             "metadata": test_document_metadatas[0],
         },
     ]
 
     logger_mock = MagicMock()
     monkeypatch.setattr(db, "LOGGER", logger_mock)
 
-    writer.transpose_and_insert(
+    writer.column_insert(
         embeddings=test_embeddings, document_metadatas=test_document_metadatas
     )
 
     logger_mock.warning.assert_called_once_with(
         db.EMBEDDING_METADATA_LENGTH_MISMATCH_WARNING
     )
     insert_mock.assert_called_once_with(
         document=expected_insert_document,
         collection_id=None,
         collection_name=None,
     )
 
 
 @patch("starpoint.db.Writer.insert")
-def test_writer_transpose_and_insert_shorter_embeddings_length(
+def test_writer_column_insert_shorter_embeddings_length(
     insert_mock: MagicMock, writer: db.Writer, monkeypatch: MonkeyPatch
 ):
     test_embeddings = [0.88]
     test_document_metadatas = [{"mock": "metadata"}, {"mock2": "metadata2"}]
     expected_insert_document = [
         {
             "embedding": test_embeddings[0],
             "metadata": test_document_metadatas[0],
         },
     ]
 
     logger_mock = MagicMock()
     monkeypatch.setattr(db, "LOGGER", logger_mock)
 
-    writer.transpose_and_insert(
+    writer.column_insert(
         embeddings=test_embeddings, document_metadatas=test_document_metadatas
     )
 
     logger_mock.warning.assert_called_once_with(
         db.EMBEDDING_METADATA_LENGTH_MISMATCH_WARNING
     )
     insert_mock.assert_called_once_with(
@@ -593,21 +593,21 @@
 
     mock_reader.assert_called_once()  # Only called during init
     mock_writer().insert.assert_called_once()
 
 
 @patch("starpoint.db.Reader")
 @patch("starpoint.db.Writer")
-def test_client_transpose_and_insert(mock_writer: MagicMock, mock_reader: MagicMock):
+def test_client_column_insert(mock_writer: MagicMock, mock_reader: MagicMock):
     client = db.Client(api_key=uuid4())
 
-    client.transpose_and_insert(embeddings=[1.1], document_metadatas={"mock": "value"})
+    client.column_insert(embeddings=[1.1], document_metadatas={"mock": "value"})
 
     mock_reader.assert_called_once()  # Only called during init
-    mock_writer().transpose_and_insert.assert_called_once()
+    mock_writer().column_insert.assert_called_once()
 
 
 @patch("starpoint.db.Reader")
 @patch("starpoint.db.Writer")
 def test_client_query(mock_writer: MagicMock, mock_reader: MagicMock):
     client = db.Client(api_key=uuid4())
 
@@ -746,18 +746,18 @@
 
     actual_embedding_response = client.build_and_insert_embeddings_from_openai(
         model=mock_model, input_data=mock_input
     )
 
     assert actual_embedding_response == expected_embedding_response
     collision_mock.assert_called_once()
-    mock_writer().transpose_and_insert.assert_called_once()
+    mock_writer().column_insert.assert_called_once()
 
     # independently check args since embeddings is a map() generator and cannot be checked against simple equality
-    insert_call_kwargs = mock_writer().transpose_and_insert.call_args.kwargs
+    insert_call_kwargs = mock_writer().column_insert.call_args.kwargs
     assert [mock_embedding] == list(insert_call_kwargs.get("embeddings"))
     assert [{"input": mock_input}] == insert_call_kwargs.get("document_metadatas")
     assert insert_call_kwargs.get("collection_id") is None  # default value
     assert insert_call_kwargs.get("collection_name") is None  # default value
 
 
 @patch("starpoint.db._check_collection_identifier_collision")
@@ -791,18 +791,18 @@
 
     actual_embedding_response = client.build_and_insert_embeddings_from_openai(
         model=mock_model, input_data=mock_input
     )
 
     assert actual_embedding_response == expected_embedding_response
     collision_mock.assert_called_once()
-    mock_writer().transpose_and_insert.assert_called_once()
+    mock_writer().column_insert.assert_called_once()
 
     # independently check args since embeddings is a map() generator and cannot be checked against simple equality
-    insert_call_kwargs = mock_writer().transpose_and_insert.call_args.kwargs
+    insert_call_kwargs = mock_writer().column_insert.call_args.kwargs
     assert [0.77, 0.88] == list(insert_call_kwargs.get("embeddings"))
     assert [
         {"input": "mock_input1"},
         {"input": "mock_input2"},
     ] == insert_call_kwargs.get("document_metadatas")
     assert insert_call_kwargs.get("collection_id") is None  # default value
     assert insert_call_kwargs.get("collection_name") is None  # default value
@@ -832,15 +832,15 @@
 
     actual_embedding_response = client.build_and_insert_embeddings_from_openai(
         model=mock_model, input_data=mock_input
     )
 
     assert actual_embedding_response == expected_embedding_response
     collision_mock.assert_called_once()
-    mock_writer().transpose_and_insert.assert_not_called()
+    mock_writer().column_insert.assert_not_called()
     logger_mock.warning.assert_called_once_with(db.NO_EMBEDDING_DATA_FOUND)
 
 
 @patch("starpoint.db._check_collection_identifier_collision")
 @patch("starpoint.db.Reader")
 @patch("starpoint.db.Writer")
 def test_client_build_and_insert_embeddings_from_openai_exception_during_write(
@@ -859,15 +859,15 @@
                 "embedding": 0.77,
                 "index": 0,
             }
         ]
     }
     openai_mock.Embedding.create.return_value = expected_embedding_response
 
-    mock_writer().transpose_and_insert.side_effect = RuntimeError("Test Exception")
+    mock_writer().column_insert.side_effect = RuntimeError("Test Exception")
 
     logger_mock = MagicMock()
     monkeypatch.setattr(db, "LOGGER", logger_mock)
 
     mock_input = "mock_input"
     mock_model = "mock-model"
```

### Comparing `starpoint-0.1.2/LICENSE` & `starpoint-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.2/README.md` & `starpoint-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.2/pyproject.toml` & `starpoint-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "starpoint"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{ name = "pointable", email = "package-maintainers@pointable.ai" }]
 description = "SDK for Starpoint DB"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `starpoint-0.1.2/PKG-INFO` & `starpoint-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starpoint
-Version: 0.1.2
+Version: 0.1.3
 Summary: SDK for Starpoint DB
 Project-URL: Homepage, https://github.com/starpoint-ai/sdk
 Project-URL: Bug Tracker, https://github.com/starpoint-ai/sdk/issues
 Author-email: pointable <package-maintainers@pointable.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

