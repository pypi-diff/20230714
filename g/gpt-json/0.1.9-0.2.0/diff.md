# Comparing `tmp/gpt_json-0.1.9.tar.gz` & `tmp/gpt_json-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_json-0.1.9.tar", max compression
+gzip compressed data, was "gpt_json-0.2.0.tar", max compression
```

## Comparing `gpt_json-0.1.9.tar` & `gpt_json-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,31 @@
--rw-r--r--   0        0        0     1071 2023-05-19 18:58:38.927164 gpt_json-0.1.9/LICENSE
--rw-r--r--   0        0        0     8963 2023-05-19 18:58:38.927164 gpt_json-0.1.9/README.md
--rw-r--r--   0        0        0       79 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/enums.py
--rw-r--r--   0        0        0      135 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/exceptions.py
--rw-r--r--   0        0        0    11997 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/gpt.py
--rw-r--r--   0        0        0      783 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/models.py
--rw-r--r--   0        0        0     1535 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/parsers.py
--rw-r--r--   0        0        0     2005 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/prompts.py
--rw-r--r--   0        0        0        0 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/__init__.py
--rw-r--r--   0        0        0      355 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/conftest.py
--rw-r--r--   0        0        0      256 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/shared.py
--rw-r--r--   0        0        0      381 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_api.py
--rw-r--r--   0        0        0      292 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_fixtures.py
--rw-r--r--   0        0        0     8987 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_gpt.py
--rw-r--r--   0        0        0      830 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_models.py
--rw-r--r--   0        0        0     1273 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_parsers.py
--rw-r--r--   0        0        0     1208 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_prompts.py
--rw-r--r--   0        0        0     4078 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_transformations.py
--rw-r--r--   0        0        0     2822 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/transformations.py
--rw-r--r--   0        0        0      628 2023-05-19 18:58:38.935164 gpt_json-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     9515 1970-01-01 00:00:00.000000 gpt_json-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-14 19:44:00.880030 gpt_json-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9021 2023-07-14 19:44:00.880030 gpt_json-0.2.0/README.md
+-rw-r--r--   0        0        0       79 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/enums.py
+-rw-r--r--   0        0        0      135 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/exceptions.py
+-rw-r--r--   0        0        0     2324 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/generics.py
+-rw-r--r--   0        0        0    20342 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/gpt.py
+-rw-r--r--   0        0        0     1438 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/models.py
+-rw-r--r--   0        0        0     1372 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/parsers.py
+-rw-r--r--   0        0        0     1727 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/prompts.py
+-rw-r--r--   0        0        0        0 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/py.typed
+-rw-r--r--   0        0        0     4037 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/streaming.py
+-rw-r--r--   0        0        0        0 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/tests/__init__.py
+-rw-r--r--   0        0        0      355 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/tests/conftest.py
+-rw-r--r--   0        0        0      256 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/tests/shared.py
+-rw-r--r--   0        0        0      381 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/tests/test_api.py
+-rw-r--r--   0        0        0      292 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/tests/test_fixtures.py
+-rw-r--r--   0        0        0    10995 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/tests/test_gpt.py
+-rw-r--r--   0        0        0      830 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/tests/test_models.py
+-rw-r--r--   0        0        0     1345 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/tests/test_parsers.py
+-rw-r--r--   0        0        0     1381 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/tests/test_prompts.py
+-rw-r--r--   0        0        0     4747 2023-07-14 19:44:00.884030 gpt_json-0.2.0/gpt_json/tests/test_streaming.py
+-rw-r--r--   0        0        0     6027 2023-07-14 19:44:00.888030 gpt_json-0.2.0/gpt_json/tests/test_transformations.py
+-rw-r--r--   0        0        0     4319 2023-07-14 19:44:00.888030 gpt_json-0.2.0/gpt_json/tests/test_truncation.py
+-rw-r--r--   0        0        0     3177 2023-07-14 19:44:00.888030 gpt_json-0.2.0/gpt_json/tests/utils/streaming_utils.py
+-rw-r--r--   0        0        0     9903 2023-07-14 19:44:00.888030 gpt_json-0.2.0/gpt_json/tests/utils/test_streaming_utils.py
+-rw-r--r--   0        0        0     4731 2023-07-14 19:44:00.888030 gpt_json-0.2.0/gpt_json/transformations.py
+-rw-r--r--   0        0        0     3351 2023-07-14 19:44:00.888030 gpt_json-0.2.0/gpt_json/truncation.py
+-rw-r--r--   0        0        0      383 2023-07-14 19:44:00.888030 gpt_json-0.2.0/gpt_json/types_oai.py
+-rw-r--r--   0        0        0      628 2023-07-14 19:44:00.892030 gpt_json-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9522 1970-01-01 00:00:00.000000 gpt_json-0.2.0/PKG-INFO
```

### Comparing `gpt_json-0.1.9/LICENSE` & `gpt_json-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.9/README.md` & `gpt_json-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,19 +59,21 @@
 ```bash
 sentiment='positive'
 Detected sentiment: positive
 ```
 
 The `json_schema` is a special keyword that will be replaced with the schema definition at runtime. You should always include this in your payload to ensure the model knows how to format results. However, you can play around with _where_ to include this schema definition; in the system prompt, in the user prompt, at the beginning, or at the end.
 
-You can either typehint the model to return a BaseSchema back, or to provide a list of Multiple BaseSchema. Both of these work:
+You can either typehint the model to return a BaseSchema back, or to provide a list of multiple BaseSchema. Both of these work:
 
 ```python
+from gpt_json.gpt import GPTJSON, ListResponse
+
 gpt_json_single = GPTJSON[SentimentSchema](API_KEY)
-gpt_json_single = GPTJSON[list[SentimentSchema]](API_KEY)
+gpt_json_multiple = GPTJSON[ListResponse[SentimentSchema]](API_KEY)
 ```
 
 If you want to get more specific about how you expect the model to populate a field, add hints about the value through the "description" field. This helps the model understand what you're looking for, and will help it generate better results.
 
 ```python
 from pydantic import BaseModel, Field
```

### Comparing `gpt_json-0.1.9/gpt_json/parsers.py` & `gpt_json-0.2.0/gpt_json/parsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,15 @@
     """
     Takes a full response that might contain other strings and attempts to extract the JSON payload.
     Has support for truncated JSON where the JSON begins but the token window ends before the json is
     is properly closed.
 
     """
     # Deal with fully included responses as well as truncated responses that only have one
-    if extract_type == ResponseType.LIST:
-        extracted_responses = list(
-            finditer(r"(\[[^\]]*$|\[.*\])", full_response, flags=DOTALL)
-        )
-    elif extract_type == ResponseType.DICTIONARY:
+    if extract_type == ResponseType.DICTIONARY:
         extracted_responses = list(
             finditer(r"({[^}]*$|{.*})", full_response, flags=DOTALL)
         )
     else:
         raise ValueError("Unknown extract_type")
 
     if not extracted_responses:
```

### Comparing `gpt_json-0.1.9/gpt_json/prompts.py` & `gpt_json-0.2.0/gpt_json/prompts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,42 @@
 from types import UnionType
 from typing import List, Type, get_args, get_origin
 
 from pydantic import BaseModel
 
 
-def generate_schema_prompt(schema: Type[BaseModel] | list[Type[BaseModel]]) -> str:
+def generate_schema_prompt(schema: Type[BaseModel]) -> str:
     """
     Converts the pydantic schema into a text representation that can be embedded
     into the prompt payload.
 
     """
 
-    def generate_payload(model):
+    def generate_payload(model: Type[BaseModel]):
         payload = []
         for key, value in model.__fields__.items():
             field_annotation = model.__annotations__[key]
             annotation_origin = get_origin(field_annotation)
             annotation_arguments = get_args(field_annotation)
 
             if annotation_origin in {list, List}:
-                payload.append(f'"{key}": {annotation_arguments[0].__name__}[]')
+                if issubclass(annotation_arguments[0], BaseModel):
+                    payload.append(
+                        f'"{key}": {generate_payload(annotation_arguments[0])}[]'
+                    )
+                else:
+                    payload.append(f'"{key}": {annotation_arguments[0].__name__}[]')
             elif annotation_origin == UnionType:
                 payload.append(
                     f'"{key}": {" | ".join([arg.__name__.lower() for arg in annotation_arguments])}'
                 )
             elif issubclass(value.type_, BaseModel):
                 payload.append(f'"{key}": {generate_payload(value.type_)}')
             else:
                 payload.append(f'"{key}": {value.type_.__name__.lower()}')
             if value.field_info.description:
                 payload[-1] += f" // {value.field_info.description}"
         # All brackets are double defined so they will passthrough a call to `.format()` where we
         # pass custom variables
         return "{{\n" + ",\n".join(payload) + "\n}}"
 
-    origin = get_origin(schema)
-    args = get_args(schema)
-
-    if origin == list:
-        if len(args) > 1:
-            raise ValueError("Only one list schema is supported at this time")
-
-        return (
-            "["
-            + "\n".join(
-                [
-                    generate_payload(sub_schema)
-                    + ", // Repeat for as many objects as are relevant"
-                    for sub_schema in args
-                ]
-            )
-            + "]"
-        )
-    else:
-        return generate_payload(schema)
+    return generate_payload(schema)
```

### Comparing `gpt_json-0.1.9/gpt_json/tests/test_gpt.py` & `gpt_json-0.2.0/gpt_json/tests/test_gpt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-from unittest.mock import patch
+import asyncio
+from json import dumps as json_dumps
+from time import time
+from unittest.mock import AsyncMock, patch
 
 import openai
 import pytest
+from openai.error import Timeout as OpenAITimeout
 from pydantic import BaseModel, Field
 
-from gpt_json.gpt import GPTJSON
+from gpt_json.gpt import GPTJSON, ListResponse
 from gpt_json.models import FixTransforms, GPTMessage, GPTMessageRole, GPTModelVersion
 from gpt_json.tests.shared import MySchema, MySubSchema
+from gpt_json.transformations import JsonFixEnum
 
 
 def test_throws_error_if_no_model_specified():
     with pytest.raises(
         ValueError, match="needs to be instantiated with a schema model"
     ):
         GPTJSON(None)
@@ -62,39 +67,43 @@
                 numerical=123,
                 sub_element=MySubSchema(name="Test"),
                 reason=True,
             ),
             FixTransforms(),
         ),
         (
-            list[MySchema],
+            ListResponse[MySchema],
             """
             Your response is as follows:
-            [
-                {
-                    "text": "Test",
-                    "items": ["Item 1", "Item 2"],
-                    "numerical": 123,
-                    "sub_element": {
-                        "name": "Test"
-                    },
-                    "reason": true
-                }
-            ]
+            {
+                "items": [
+                    {
+                        "text": "Test",
+                        "items": ["Item 1", "Item 2"],
+                        "numerical": 123,
+                        "sub_element": {
+                            "name": "Test"
+                        },
+                        "reason": true
+                    }
+                ]
+            }
             Your response is above.
             """,
-            [
-                MySchema(
-                    text="Test",
-                    items=["Item 1", "Item 2"],
-                    numerical=123,
-                    sub_element=MySubSchema(name="Test"),
-                    reason=True,
-                )
-            ],
+            ListResponse(
+                items=[
+                    MySchema(
+                        text="Test",
+                        items=["Item 1", "Item 2"],
+                        numerical=123,
+                        sub_element=MySubSchema(name="Test"),
+                        reason=True,
+                    )
+                ]
+            ),
             FixTransforms(),
         ),
         (
             MySchema,
             """
             Your response is as follows:
             {
@@ -110,15 +119,17 @@
             MySchema(
                 text="Test",
                 items=["Item 1", "Item 2"],
                 numerical=123,
                 sub_element=MySubSchema(name="Test"),
                 reason=True,
             ),
-            FixTransforms(fixed_bools=True, fixed_truncation=True),
+            FixTransforms(
+                fixed_bools=True, fixed_truncation=JsonFixEnum.UNCLOSED_VALUE
+            ),
         ),
     ],
 )
 async def test_acreate(
     schema_typehint, response_raw, parsed, expected_transformations: FixTransforms
 ):
     model_version = GPTModelVersion.GPT_3_5
@@ -165,16 +176,16 @@
                 {
                     "role": message.role.value,
                     "content": message.content,
                 }
                 for message in messages
             ],
             temperature=0.0,
-            timeout=60,
             api_key=None,
+            stream=False,
         )
 
     assert response == parsed
     assert transformations == expected_transformations
 
 
 @pytest.mark.parametrize(
@@ -263,15 +274,15 @@
     gpt = GPTJSON[MySchema](None)
 
     with patch.object(
         gpt,
         "submit_request",
         return_value={"choices": [{"message": {"content": "some content"}}]},
     ), patch.object(
-        gpt, "extract_json", return_value=(None, FixTransforms(False, False))
+        gpt, "extract_json", return_value=(None, FixTransforms(None, False))
     ):
         result, _ = await gpt.run(
             [GPTMessage(GPTMessageRole.SYSTEM, "message content")]
         )
         assert result is None
 
 
@@ -291,19 +302,72 @@
     gpt = GPTJSON[MySchema](None)
 
     with patch.object(
         gpt,
         "submit_request",
         return_value={"choices": [{"message": {"content": "some content"}}]},
     ), patch.object(
-        gpt, "extract_json", return_value=(None, FixTransforms(False, False))
+        gpt, "extract_json", return_value=(None, FixTransforms(None, False))
     ):
         result, _ = await gpt.run(
             [GPTMessage(GPTMessageRole.SYSTEM, "message content")]
         )
         assert result is None
 
 
 @pytest.mark.asyncio
 async def test_unknown_model_to_infer_max_tokens():
     with pytest.raises(ValueError):
         GPTJSON[MySchema](model="UnknownModel", auto_trim=True)
+
+
+@pytest.mark.asyncio
+async def test_timeout():
+    class MockResponse:
+        """
+        We need to build an actual response class here because the internal openai
+        code postprocesses with the aiohttp response.
+
+        """
+
+        def __init__(self, response_text: str):
+            self.status = 200
+            self.headers: dict[str, str] = {}
+            self.response_text = response_text
+
+        async def read(self):
+            mock_response = {
+                "choices": [
+                    {
+                        "message": {
+                            "role": "assistant",
+                            "content": self.response_text,
+                        },
+                        "index": 0,
+                        "finish_reason": "stop",
+                    }
+                ]
+            }
+            return json_dumps(mock_response).encode()
+
+    with patch("aiohttp.ClientSession.request", new_callable=AsyncMock) as mock_request:
+        # Mock a stalling request
+        async def side_effect(*args, **kwargs):
+            await asyncio.sleep(4)
+            return MockResponse("TEST_RESPONSE")
+
+        mock_request.side_effect = side_effect
+
+        gpt = GPTJSON[MySchema](api_key="ABC", timeout=2)
+
+        start_time = time()
+
+        with pytest.raises(OpenAITimeout):
+            await gpt.run(
+                [GPTMessage(GPTMessageRole.SYSTEM, "message content")],
+            )
+
+        end_time = time()
+        duration = end_time - start_time
+
+        # Assert duration is about 2 seconds
+        pytest.approx(duration, 2, 0.2)
```

### Comparing `gpt_json-0.1.9/gpt_json/tests/test_models.py` & `gpt_json-0.2.0/gpt_json/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.9/gpt_json/tests/test_prompts.py` & `gpt_json-0.2.0/gpt_json/tests/test_prompts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from re import sub
 
 import pytest
 
+from gpt_json.generics import resolve_generic_model
+from gpt_json.gpt import ListResponse
 from gpt_json.prompts import generate_schema_prompt
 from gpt_json.tests.shared import MySchema
 
 
 def strip_whitespace(input_string: str):
     return sub(r"\s+", "", input_string)
 
@@ -24,28 +26,28 @@
                     "name": str
                 }},
                 "reason": bool // Explanation
             }}
             """,
         ),
         (
-            list[MySchema],
+            ListResponse[MySchema],
             """
-            [
             {{
-            "text": str,
-            "items": str[],
-            "numerical": int | float,
-            "sub_element": {{
-                "name": str
-            }},
-            "reason": bool // Explanation
-            }}, // Repeat for as many objects as are relevant
-            ]
+            "items": {{
+                "text": str,
+                "items": str[],
+                "numerical": int | float,
+                "sub_element": {{
+                    "name": str
+                }},
+                "reason": bool // Explanation            
+            }}[] // Repeat for as many objects as are relevant
+            }}
             """,
         ),
     ],
 )
 def test_generate_schema_prompt(schema_definition, expected: str):
     assert strip_whitespace(
-        generate_schema_prompt(schema_definition)
+        generate_schema_prompt(resolve_generic_model(schema_definition))
     ) == strip_whitespace(expected)
```

### Comparing `gpt_json-0.1.9/pyproject.toml` & `gpt_json-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "gpt-json"
-version = "0.1.9"
+version = "0.2.0"
 description = "Structured and typehinted GPT responses in Python."
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 packages = [{include = "gpt_json"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 tiktoken = "^0.3.3"
 openai = "^0.27.6"
 pydantic = "^1.10.7"
 backoff = "^2.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `gpt_json-0.1.9/PKG-INFO` & `gpt_json-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: gpt-json
-Version: 0.1.9
+Version: 0.2.0
 Summary: Structured and typehinted GPT responses in Python.
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Description-Content-Type: text/markdown
 
@@ -75,19 +74,21 @@
 ```bash
 sentiment='positive'
 Detected sentiment: positive
 ```
 
 The `json_schema` is a special keyword that will be replaced with the schema definition at runtime. You should always include this in your payload to ensure the model knows how to format results. However, you can play around with _where_ to include this schema definition; in the system prompt, in the user prompt, at the beginning, or at the end.
 
-You can either typehint the model to return a BaseSchema back, or to provide a list of Multiple BaseSchema. Both of these work:
+You can either typehint the model to return a BaseSchema back, or to provide a list of multiple BaseSchema. Both of these work:
 
 ```python
+from gpt_json.gpt import GPTJSON, ListResponse
+
 gpt_json_single = GPTJSON[SentimentSchema](API_KEY)
-gpt_json_single = GPTJSON[list[SentimentSchema]](API_KEY)
+gpt_json_multiple = GPTJSON[ListResponse[SentimentSchema]](API_KEY)
 ```
 
 If you want to get more specific about how you expect the model to populate a field, add hints about the value through the "description" field. This helps the model understand what you're looking for, and will help it generate better results.
 
 ```python
 from pydantic import BaseModel, Field
```

