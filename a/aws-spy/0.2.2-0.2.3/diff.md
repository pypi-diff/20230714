# Comparing `tmp/aws_spy-0.2.2.tar.gz` & `tmp/aws_spy-0.2.3.tar.gz`

## Comparing `aws_spy-0.2.2.tar` & `aws_spy-0.2.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aws_spy-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aws_spy-0.2.2/Makefile
--rw-r--r--   0        0        0    72078 2020-02-02 00:00:00.000000 aws_spy-0.2.2/pdm.lock
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aws_spy-0.2.2/.vscode/settings.json
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/dependencies.py
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/main.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/responses.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/test.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/core/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/core/encoders.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/core/event_utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/core/exceptions.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/core/logging.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/core/params.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/core/params_alias.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/core/responses.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/core/schemas.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/core/schemas_utils.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/core/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/helpers/__init__.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/helpers/cli.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/helpers/documentation.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/helpers/exceptions.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/helpers/utils.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 aws_spy-0.2.2/aws_spy/layer/spy-layer.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/test_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/integration/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/integration/test_params.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/integration/test_request_body.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/integration/test_response_class.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/integration/test_test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/unit/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/unit/test_encoders.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/unit/test_event_utils.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/unit/test_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/unit/test_schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.2/tests/unit/test_utils.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 aws_spy-0.2.2/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aws_spy-0.2.2/LICENSE
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 aws_spy-0.2.2/README.md
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aws_spy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 aws_spy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aws_spy-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 aws_spy-0.2.3/Makefile
+-rw-r--r--   0        0        0    72078 2020-02-02 00:00:00.000000 aws_spy-0.2.3/pdm.lock
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aws_spy-0.2.3/.vscode/settings.json
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/dependencies.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/main.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/responses.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/test.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/core/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/core/encoders.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/core/event_utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/core/exceptions.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/core/logging.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/core/params.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/core/params_alias.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/core/responses.py
+-rw-r--r--   0        0        0     8910 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/core/schemas.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/core/schemas_utils.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/core/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/helpers/__init__.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/helpers/cli.py
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/helpers/documentation.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/helpers/exceptions.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/helpers/utils.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 aws_spy-0.2.3/aws_spy/layer/spy-layer.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/test_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/integration/test_params.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/integration/test_request_body.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/integration/test_response_class.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/integration/test_test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/unit/test_encoders.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/unit/test_event_utils.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/unit/test_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/unit/test_schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.3/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 aws_spy-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aws_spy-0.2.3/LICENSE
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 aws_spy-0.2.3/README.md
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aws_spy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 aws_spy-0.2.3/PKG-INFO
```

### Comparing `aws_spy-0.2.2/.pre-commit-config.yaml` & `aws_spy-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/pdm.lock` & `aws_spy-0.2.3/pdm.lock`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/aws_spy/__init__.py` & `aws_spy-0.2.3/aws_spy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ServerlessPy package ;D"""
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 from aws_spy import responses
 from aws_spy.core.logging import logger
 from aws_spy.core.params_alias import Header, Path, Query
 from aws_spy.core.schemas import (
     CORS,
     VPC,
```

### Comparing `aws_spy-0.2.2/aws_spy/dependencies.py` & `aws_spy-0.2.3/aws_spy/dependencies.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/aws_spy/main.py` & `aws_spy-0.2.3/aws_spy/main.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/aws_spy/responses.py` & `aws_spy-0.2.3/aws_spy/responses.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/aws_spy/test.py` & `aws_spy-0.2.3/aws_spy/test.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/aws_spy/core/event_utils.py` & `aws_spy-0.2.3/aws_spy/core/event_utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/aws_spy/core/schemas.py` & `aws_spy-0.2.3/aws_spy/core/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
                 )
             ),
         )
 
 
 class Provider(BaseModel):
     name: str = "aws"
-    runtime: str = "python3.9"
+    runtime: str = "python3.10"
     region: str = "eu_central_1"
     role: str | CloudFormationRef | JSONFileRef | None = Field(None)
     httpApi: HTTPApi | None = Field(None)  # noqa: N815
     vpc: VPC | None = Field(None)
 
 
 class ServerlessConfig(YamlModel):
```

### Comparing `aws_spy-0.2.2/aws_spy/core/schemas_utils.py` & `aws_spy-0.2.3/aws_spy/core/schemas_utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/aws_spy/core/types.py` & `aws_spy-0.2.3/aws_spy/core/types.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/aws_spy/helpers/cli.py` & `aws_spy-0.2.3/aws_spy/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/aws_spy/helpers/documentation.py` & `aws_spy-0.2.3/aws_spy/helpers/documentation.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/aws_spy/helpers/utils.py` & `aws_spy-0.2.3/aws_spy/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/tests/conftest.py` & `aws_spy-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/tests/test_app.py` & `aws_spy-0.2.3/tests/test_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 from aws_spy import ServerlessConfig, SpyAPI, SpyRouter, __version__
 from aws_spy.core.schemas import Methods
 
 
 def test_app() -> None:
-    assert __version__ == "0.2.2"
+    assert __version__ == "0.2.3"
 
 
 def test_app_conf(app: SpyAPI, config: ServerlessConfig) -> None:
     assert app.config == config
 
 
 @pytest.mark.parametrize("prefix", ["api", "/api", "/somet_other_prefix"])
```

### Comparing `aws_spy-0.2.2/tests/integration/test_params.py` & `aws_spy-0.2.3/tests/integration/test_params.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/tests/integration/test_request_body.py` & `aws_spy-0.2.3/tests/integration/test_request_body.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/tests/integration/test_response_class.py` & `aws_spy-0.2.3/tests/integration/test_response_class.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/tests/unit/test_encoders.py` & `aws_spy-0.2.3/tests/unit/test_encoders.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/tests/unit/test_event_utils.py` & `aws_spy-0.2.3/tests/unit/test_event_utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/tests/unit/test_responses.py` & `aws_spy-0.2.3/tests/unit/test_responses.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/.gitignore` & `aws_spy-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/LICENSE` & `aws_spy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/pyproject.toml` & `aws_spy-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.2/PKG-INFO` & `aws_spy-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-spy
-Version: 0.2.2
+Version: 0.2.3
 Project-URL: Homepage, https://github.com/PiochU19/aws-spy
 Project-URL: Documentation, https://github.com/PiochU19/aws-spy#readme
 Project-URL: Issues, https://github.com/PiochU19/aws-spy/issues
 Project-URL: Source, https://github.com/PiochU19/aws-spy
 Author-email: Dominik Pioś <792954018@wp.pl>
 License: The MIT License (MIT)
```

