# Comparing `tmp/gpru-0.2.0.tar.gz` & `tmp/gpru-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Tue Jan  1 00:00:00 1980, max compression
```

## Comparing `gpru-0.2.0.tar` & `gpru-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/__about__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/__init__.py
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/_client.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/_logger.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/__init__.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/_api.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/_utils.py
--rw-r--r--   0        0        0    37103 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/preview_2022_03_01.py
--rw-r--r--   0        0        0    40310 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/preview_2022_06_01.py
--rw-r--r--   0        0        0    54413 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/preview_2023_03_15.py
--rw-r--r--   0        0        0    59066 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/preview_2023_06_01.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/py.typed
--rw-r--r--   0        0        0    46831 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/stable_2022_12_01.py
--rw-r--r--   0        0        0    49153 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/azure/stable_2023_05_15.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/openai/__init__.py
--rw-r--r--   0        0        0    58302 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/openai/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.2.0/gpru/openai/py.typed
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 gpru-0.2.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpru-0.2.0/LICENSE
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 gpru-0.2.0/README.md
--rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 gpru-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 gpru-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/__about__.py
+-rw-r--r--   0        0        0       83 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/__init__.py
+-rw-r--r--   0        0        0     4004 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/_client.py
+-rw-r--r--   0        0        0       51 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/_logger.py
+-rw-r--r--   0        0        0      652 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/exceptions.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/py.typed
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/azure/__init__.py
+-rw-r--r--   0        0        0     1559 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/azure/_api.py
+-rw-r--r--   0        0        0      302 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/azure/_utils.py
+-rw-r--r--   0        0        0    37207 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/azure/preview_2022_03_01.py
+-rw-r--r--   0        0        0    40420 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/azure/preview_2022_06_01.py
+-rw-r--r--   0        0        0    54540 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/azure/preview_2023_03_15.py
+-rw-r--r--   0        0        0    59188 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/azure/preview_2023_06_01.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/azure/py.typed
+-rw-r--r--   0        0        0    46946 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/azure/stable_2022_12_01.py
+-rw-r--r--   0        0        0    49248 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/azure/stable_2023_05_15.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/openai/__init__.py
+-rw-r--r--   0        0        0    58493 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/openai/api.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 gpru-0.3.0/gpru/openai/py.typed
+-rw-r--r--   0        0        0     3210 1980-01-01 00:00:00.000000 gpru-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1070 1980-01-01 00:00:00.000000 gpru-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4150 1980-01-01 00:00:00.000000 gpru-0.3.0/README.md
+-rw-r--r--   0        0        0     4720 1980-01-01 00:00:00.000000 gpru-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5608 1980-01-01 00:00:00.000000 gpru-0.3.0/PKG-INFO
```

### Comparing `gpru-0.2.0/gpru/_client.py` & `gpru-0.3.0/gpru/_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from enum import Enum
 from pathlib import Path
 from typing import Any, Callable, Dict, Generator, Type, TypeVar
 
 import httpx
 from httpx._exceptions import HTTPError, ReadTimeout, StreamError
 from pydantic import BaseModel
-from pydantic.error_wrappers import ValidationError
+from pydantic_core import ValidationError
 from tenacity import (
     before_log,
     retry,
     retry_if_exception,
     stop_after_attempt,
     wait_random_exponential,
 )
@@ -24,15 +24,15 @@
 _API_FAILED = "API request failed."
 _IMPLEMENTATION_ERROR = f"Implementation error in gpru@{__version__}."
 
 
 def _raise_api_error(error_response_model: Type[T], response: httpx.Response) -> None:
     logger.error(_API_FAILED)
     logger.debug(response.json())
-    error_response = error_response_model.parse_obj(response.json())
+    error_response = error_response_model.model_validate(response.json())
     error = error_response.error if hasattr(error_response, "error") else error_response
     raise ApiError(response.status_code, error)
 
 
 def _retry_condition(e: BaseException) -> bool:
     if type(e) == ApiError:
         return isinstance(e.error, ReadTimeout)
@@ -106,14 +106,14 @@
 
     return stream
 
 
 def kwargs_for_uploading(request_model: T) -> Dict[str, Any]:
     data: Dict[str, Any] = {}
     files: Dict[str, Any] = {}
-    for k, v in request_model.dict(exclude_none=True).items():
+    for k, v in request_model.model_dump(exclude_none=True).items():
         if isinstance(v, Path):
             files[k] = v.open("rb")
         else:
             value = v.value if isinstance(v, Enum) else v
             data[k] = value
     return {"data": data or None, "files": files or None}
```

### Comparing `gpru-0.2.0/gpru/exceptions.py` & `gpru-0.3.0/gpru/exceptions.py`

 * *Files identical despite different names*

### Comparing `gpru-0.2.0/gpru/azure/_api.py` & `gpru-0.3.0/gpru/azure/_api.py`

 * *Files identical despite different names*

### Comparing `gpru-0.2.0/gpru/azure/preview_2022_03_01.py` & `gpru-0.3.0/gpru/azure/preview_2022_03_01.py`

 * *Files 2% similar despite different names*

```diff
@@ -730,15 +730,15 @@
 
         Returns
         -------
         DeploymentList
             `DeploymentList` instance.
         """
         response = self._request("GET", "/deployments")
-        return DeploymentList.parse_obj(response.json())
+        return DeploymentList.model_validate(response.json())
 
     def create_deployment(self, deployment: Deployment) -> Deployment:
         """
         Create a new deployment for the Azure OpenAI resource according to the given
         specification.
 
         Parameters
@@ -749,17 +749,17 @@
 
         Returns
         -------
         Deployment
             Created `Deployment` instance.
         """
         response = self._request(
-            "POST", "/deployments", json=deployment.dict(exclude_none=True)
+            "POST", "/deployments", json=deployment.model_dump(exclude_none=True)
         )
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def get_deployment(self, deployment_id: str) -> Deployment:
         """
         Get details for a single deployment specified by the given `deployment_id`.
 
         Parameters
         ----------
@@ -768,15 +768,15 @@
 
         Returns
         -------
         Deployment
             Specified `Deployment` instance.
         """
         response = self._request("GET", f"/deployments/{deployment_id}")
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def update_deployment(
         self,
         deployment_id: str,
         model: Optional[str] = None,
         scale_settings: Optional[ScaleSettings] = None,
     ) -> Deployment:
@@ -796,22 +796,22 @@
         Returns
         -------
         Deployment
             Updated `Deployment` instance.
         """
         data: Dict[str, Any] = {"model": model}
         if scale_settings is not None:
-            data["scale_settings"] = scale_settings.dict(exclude_none=True)
+            data["scale_settings"] = scale_settings.model_dump(exclude_none=True)
         response = self._request(
             "PATCH",
             f"/deployments/{deployment_id}",
             headers={"Content-Type": "application/merge-patch+json"},
             data=data,
         )
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def delete_deployment(self, deployment_id: str) -> None:
         """
         Delete the deployment specified by the given `deployment_id`.
 
         Parameters
         ----------
@@ -830,15 +830,15 @@
 
         Returns
         -------
         FileList
             `FileList` instance.
         """
         response = self._request("GET", "/files")
-        return FileList.parse_obj(response.json())
+        return FileList.model_validate(response.json())
 
     def upload_file(self, file: Path, purpose: Purpose) -> File:
         """
         Create a new file entity by uploading data from a local machine. Uploaded files
         can, for example, be used for training or evaluating fine-tuned models.
 
         Parameters
@@ -853,15 +853,15 @@
         -------
         File
             Uploaded `File` instance.
         """
         data = {"purpose": purpose.value}
         files = {"file": file.open("rb")}
         response = self._request("POST", "/files", data=data, files=files)
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def get_file(self, file_id: str) -> File:
         """
         Get details for a single file specified by the given `file_id` including status,
         size, purpose, etc.
 
         Parameters
@@ -871,15 +871,15 @@
 
         Returns
         -------
         File
             Specified `File` instance.
         """
         response = self._request("GET", f"/files/{file_id}")
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def delete_file(self, file_id: str) -> None:
         """
         Delete the file with the given `file_id`. Deletion is also allowed if a file was
         used, e.g., as training file in a fine-tune job.
 
         Parameters
@@ -936,15 +936,15 @@
             "/files/import",
             json={
                 "content_url": content_url,
                 "filename": filename,
                 "purpose": purpose.value,
             },
         )
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def list_fine_tunes(self) -> FineTuneList:
         """
         Get a list of all fine-tune jobs owned by the Azure OpenAI resource. The details
         that are returned for each fine-tune job contain besides its identifier the base
         model, training and validation files, hyper parameters, time stamps, status and
         events. Events are created when the job status changes, e.g. running or
@@ -952,15 +952,15 @@
 
         Returns
         -------
         FineTuneList
             `FineTuneList` instance.
         """
         response = self._request("GET", "/fine-tunes")
-        return FineTuneList.parse_obj(response.json())
+        return FineTuneList.model_validate(response.json())
 
     def create_fine_tune(self, fine_tune_request: FineTuneRequest) -> FineTune:
         """
         Create a job that fine-tunes a specified model from a given training file.
         Response includes details of the enqueued job including job status and hyper
         parameters. The name of the fine-tuned model is added to the response once
         complete.
@@ -976,17 +976,17 @@
 
         Returns
         -------
         FineTune
             Created `FineTune` instance.
         """
         response = self._request(
-            "POST", "/fine-tunes", json=fine_tune_request.dict(exclude_none=True)
+            "POST", "/fine-tunes", json=fine_tune_request.model_dump(exclude_none=True)
         )
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def get_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Get details for a single fine-tune job specified by the given `fine_tune_id`.
         The details contain the base model, training and validation files, hyper
         parameters, time stamps, status and events. Events are created when the job
         status changes, e.g. running or complete, and when results are uploaded.
@@ -998,15 +998,15 @@
 
         Returns
         -------
         FineTune
             Specified `FineTune` instance.
         """
         response = self._request("GET", f"/fine-tunes/{fine_tune_id}")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def delete_fine_tune(self, fine_tune_id: str) -> None:
         """
         Delete the fine-tune job specified by the given `fine_tune_id`.
 
         Parameters
         ----------
@@ -1042,15 +1042,15 @@
             "params": None if stream is None else {"stream": stream},
         }
 
         if stream is True:
             return self._stream(FineTuneEvent, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return FineTuneEventList.parse_obj(response.json())
+        return FineTuneEventList.model_validate(response.json())
 
     def cancel_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Cancel the processing of the fine-tune job specified by the given
         `fine_tune_id`.
 
         Parameters
@@ -1060,29 +1060,29 @@
 
         Returns
         -------
         FineTune
             Canceled `FineTune` instance.
         """
         response = self._request("POST", f"/fine-tunes/{fine_tune_id}/cancel")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def list_models(self) -> ModelList:
         """
         Get a list of all models that are accessible by the Azure OpenAI resource. These
         include base models as well as all successfully completed fine-tuned models
         owned by the Azure OpenAI resource.
 
         Returns
         -------
         ModelList
             `ModelList` instance.
         """
         response = self._request("GET", "/models")
-        return ModelList.parse_obj(response.json())
+        return ModelList.model_validate(response.json())
 
     def get_model(self, model_id: str) -> Model:
         """
         Get details for the model specified by the given `model_id`.
 
         Parameters
         ----------
@@ -1091,15 +1091,15 @@
 
         Returns
         -------
         Model
             Specified `Model` instance.
         """
         response = self._request("GET", f"/models/{model_id}")
-        return Model.parse_obj(response.json())
+        return Model.model_validate(response.json())
 
     def create_completion(
         self, deployment_id: str, completion_request: CompletionRequest
     ) -> Union[Generator[Completion, None, None], Completion]:
         """
         Create a completion from a chosen model.
 
@@ -1115,15 +1115,15 @@
         Union[Generator[Completion, None, None], Completion]:
             Generator that streams the `Completion` if `completion_request.stream` is
             `True`, or created `Completion` instance otherwise.
         """
         kwargs = {
             "method": "POST",
             "path": f"/deployments/{deployment_id}/completions",
-            "json": completion_request.dict(exclude_none=True),
+            "json": completion_request.model_dump(exclude_none=True),
         }
 
         if completion_request.stream is True:
             return self._stream(Completion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return Completion.parse_obj(response.json())
+        return Completion.model_validate(response.json())
```

### Comparing `gpru-0.2.0/gpru/azure/preview_2022_06_01.py` & `gpru-0.3.0/gpru/azure/preview_2022_06_01.py`

 * *Files 2% similar despite different names*

```diff
@@ -787,15 +787,15 @@
 
         Returns
         -------
         DeploymentList
             `DeploymentList` instance.
         """
         response = self._request("GET", "/deployments")
-        return DeploymentList.parse_obj(response.json())
+        return DeploymentList.model_validate(response.json())
 
     def create_deployment(self, deployment: Deployment) -> Deployment:
         """
         Create a new deployment for the Azure OpenAI resource according to the given
         specification.
 
         Parameters
@@ -806,17 +806,17 @@
 
         Returns
         -------
         Deployment
             Created `Deployment` instance.
         """
         response = self._request(
-            "POST", "/deployments", json=deployment.dict(exclude_none=True)
+            "POST", "/deployments", json=deployment.model_dump(exclude_none=True)
         )
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def get_deployment(self, deployment_id: str) -> Deployment:
         """
         Get details for a single deployment specified by the given `deployment_id`.
 
         Parameters
         ----------
@@ -825,15 +825,15 @@
 
         Returns
         -------
         Deployment
             Specified `Deployment` instance.
         """
         response = self._request("GET", f"/deployments/{deployment_id}")
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def update_deployment(
         self,
         deployment_id: str,
         model: Optional[str] = None,
         scale_settings: Optional[ScaleSettings] = None,
     ) -> Deployment:
@@ -853,22 +853,22 @@
         Returns
         -------
         Deployment
             Updated `Deployment` instance.
         """
         data: Dict[str, Any] = {"model": model}
         if scale_settings is not None:
-            data["scale_settings"] = scale_settings.dict(exclude_none=True)
+            data["scale_settings"] = scale_settings.model_dump(exclude_none=True)
         response = self._request(
             "PATCH",
             f"/deployments/{deployment_id}",
             headers={"Content-Type": "application/merge-patch+json"},
             data=data,
         )
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def delete_deployment(self, deployment_id: str) -> None:
         """
         Delete the deployment specified by the given `deployment_id`.
 
         Parameters
         ----------
@@ -887,15 +887,15 @@
 
         Returns
         -------
         FileList
             `FileList` instance.
         """
         response = self._request("GET", "/files")
-        return FileList.parse_obj(response.json())
+        return FileList.model_validate(response.json())
 
     def upload_file(self, file: Path, purpose: Purpose) -> File:
         """
         Create a new file entity by uploading data from a local machine. Uploaded files
         can, for example, be used for training or evaluating fine-tuned models.
 
         Parameters
@@ -910,15 +910,15 @@
         -------
         File
             Uploaded `File` instance.
         """
         data = {"purpose": purpose.value}
         files = {"file": file.open("rb")}
         response = self._request("POST", "/files", data=data, files=files)
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def get_file(self, file_id: str) -> File:
         """
         Get details for a single file specified by the given `file_id` including status,
         size, purpose, etc.
 
         Parameters
@@ -928,15 +928,15 @@
 
         Returns
         -------
         File
             Specified `File` instance.
         """
         response = self._request("GET", f"/files/{file_id}")
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def delete_file(self, file_id: str) -> None:
         """
         Delete the file with the given `file_id`. Deletion is also allowed if a file was
         used, e.g., as training file in a fine-tune job.
 
         Parameters
@@ -993,15 +993,15 @@
             "/files/import",
             json={
                 "content_url": content_url,
                 "filename": filename,
                 "purpose": purpose.value,
             },
         )
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def list_fine_tunes(self) -> FineTuneList:
         """
         Get a list of all fine-tune jobs owned by the Azure OpenAI resource. The details
         that are returned for each fine-tune job contain besides its identifier the base
         model, training and validation files, hyper parameters, time stamps, status and
         events. Events are created when the job status changes, e.g. running or
@@ -1009,15 +1009,15 @@
 
         Returns
         -------
         FineTuneList
             `FineTuneList` instance.
         """
         response = self._request("GET", "/fine-tunes")
-        return FineTuneList.parse_obj(response.json())
+        return FineTuneList.model_validate(response.json())
 
     def create_fine_tune(self, fine_tune_request: FineTuneRequest) -> FineTune:
         """
         Create a job that fine-tunes a specified model from a given training file.
         Response includes details of the enqueued job including job status and hyper
         parameters. The name of the fine-tuned model is added to the response once
         complete.
@@ -1033,17 +1033,17 @@
 
         Returns
         -------
         FineTune
             Created `FineTune` instance.
         """
         response = self._request(
-            "POST", "/fine-tunes", json=fine_tune_request.dict(exclude_none=True)
+            "POST", "/fine-tunes", json=fine_tune_request.model_dump(exclude_none=True)
         )
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def get_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Get details for a single fine-tune job specified by the given `fine_tune_id`.
         The details contain the base model, training and validation files, hyper
         parameters, time stamps, status and events. Events are created when the job
         status changes, e.g. running or complete, and when results are uploaded.
@@ -1055,15 +1055,15 @@
 
         Returns
         -------
         FineTune
             Specified `FineTune` instance.
         """
         response = self._request("GET", f"/fine-tunes/{fine_tune_id}")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def delete_fine_tune(self, fine_tune_id: str) -> None:
         """
         Delete the fine-tune job specified by the given `fine_tune_id`.
 
         Parameters
         ----------
@@ -1099,15 +1099,15 @@
             "params": None if stream is None else {"stream": stream},
         }
 
         if stream is True:
             return self._stream(FineTuneEvent, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return FineTuneEventList.parse_obj(response.json())
+        return FineTuneEventList.model_validate(response.json())
 
     def cancel_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Cancel the processing of the fine-tune job specified by the given
         `fine_tune_id`.
 
         Parameters
@@ -1117,29 +1117,29 @@
 
         Returns
         -------
         FineTune
             Canceled `FineTune` instance.
         """
         response = self._request("POST", f"/fine-tunes/{fine_tune_id}/cancel")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def list_models(self) -> ModelList:
         """
         Get a list of all models that are accessible by the Azure OpenAI resource. These
         include base models as well as all successfully completed fine-tuned models
         owned by the Azure OpenAI resource.
 
         Returns
         -------
         ModelList
             `ModelList` instance.
         """
         response = self._request("GET", "/models")
-        return ModelList.parse_obj(response.json())
+        return ModelList.model_validate(response.json())
 
     def get_model(self, model_id: str) -> Model:
         """
         Get details for the model specified by the given `model_id`.
 
         Parameters
         ----------
@@ -1148,15 +1148,15 @@
 
         Returns
         -------
         Model
             Specified `Model` instance.
         """
         response = self._request("GET", f"/models/{model_id}")
-        return Model.parse_obj(response.json())
+        return Model.model_validate(response.json())
 
     def create_completion(
         self, deployment_id: str, completion_request: CompletionRequest
     ) -> Union[Generator[Completion, None, None], Completion]:
         """
         Create a completion from a chosen model.
 
@@ -1172,22 +1172,22 @@
         Union[Generator[Completion, None, None], Completion]:
             Generator that streams the `Completion` if `completion_request.stream` is
             `True`, or created `Completion` instance otherwise.
         """
         kwargs = {
             "method": "POST",
             "path": f"/deployments/{deployment_id}/completions",
-            "json": completion_request.dict(exclude_none=True),
+            "json": completion_request.model_dump(exclude_none=True),
         }
 
         if completion_request.stream is True:
             return self._stream(Completion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return Completion.parse_obj(response.json())
+        return Completion.model_validate(response.json())
 
     def create_embedding(
         self, deployment_id: str, embedding_request: EmbeddingRequest
     ) -> str:
         """
         Return the embeddings for a given prompt.
 
@@ -1202,10 +1202,10 @@
         -------
         str
             Created embedding.
         """
         response = self._request(
             "POST",
             f"/deployments/{deployment_id}/embeddings",
-            json=embedding_request.dict(exclude_none=True),
+            json=embedding_request.model_dump(exclude_none=True),
         )
         return str(response.text)
```

### Comparing `gpru-0.2.0/gpru/azure/preview_2023_03_15.py` & `gpru-0.3.0/gpru/azure/preview_2023_03_15.py`

 * *Files 2% similar despite different names*

```diff
@@ -1054,15 +1054,15 @@
         content : str
             The contents of the message.
         """
         super().__init__(role=Role.ASSISTANT, content=content)
 
 
 class ChatCompletionRequest(BaseModel):
-    messages: List[Message] = Field(..., min_items=1)
+    messages: List[Message] = Field(..., min_length=1)
     """The messages to generate chat completions for, in the chat format."""
     temperature: Optional[float] = Field(1.0, ge=0.0, le=2.0)
     """
     What sampling temperature to use, between 0 and 2.
 
     Higher values like 0.8 will make the output more random, while lower values like 0.2
     will make it more focused and deterministic. We generally recommend altering this or
@@ -1188,15 +1188,15 @@
 
         Returns
         -------
         DeploymentList
             `DeploymentList` instance.
         """
         response = self._request("GET", "/deployments")
-        return DeploymentList.parse_obj(response.json())
+        return DeploymentList.model_validate(response.json())
 
     def create_deployment(self, deployment: Deployment) -> Deployment:
         """
         Create a new deployment for the Azure OpenAI resource according to the given
         specification.
 
         Parameters
@@ -1207,17 +1207,17 @@
 
         Returns
         -------
         Deployment
             Created `Deployment` instance.
         """
         response = self._request(
-            "POST", "/deployments", json=deployment.dict(exclude_none=True)
+            "POST", "/deployments", json=deployment.model_dump(exclude_none=True)
         )
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def get_deployment(self, deployment_id: str) -> Deployment:
         """
         Get details for a single deployment specified by the given `deployment_id`.
 
         Parameters
         ----------
@@ -1226,15 +1226,15 @@
 
         Returns
         -------
         Deployment
             Specified `Deployment` instance.
         """
         response = self._request("GET", f"/deployments/{deployment_id}")
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def update_deployment(
         self,
         deployment_id: str,
         model: Optional[str] = None,
         scale_settings: Optional[ScaleSettings] = None,
     ) -> Deployment:
@@ -1254,22 +1254,22 @@
         Returns
         -------
         Deployment
             Updated `Deployment` instance.
         """
         data: Dict[str, Any] = {"model": model}
         if scale_settings is not None:
-            data["scale_settings"] = scale_settings.dict(exclude_none=True)
+            data["scale_settings"] = scale_settings.model_dump(exclude_none=True)
         response = self._request(
             "PATCH",
             f"/deployments/{deployment_id}",
             headers={"Content-Type": "application/merge-patch+json"},
             data=data,
         )
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def delete_deployment(self, deployment_id: str) -> None:
         """
         Delete the deployment specified by the given `deployment_id`.
 
         Parameters
         ----------
@@ -1288,15 +1288,15 @@
 
         Returns
         -------
         FileList
             `FileList` instance.
         """
         response = self._request("GET", "/files")
-        return FileList.parse_obj(response.json())
+        return FileList.model_validate(response.json())
 
     def upload_file(self, file: Path, purpose: Purpose) -> File:
         """
         Create a new file entity by uploading data from a local machine. Uploaded files
         can, for example, be used for training or evaluating fine-tuned models.
 
         Parameters
@@ -1311,15 +1311,15 @@
         -------
         File
             Uploaded `File` instance.
         """
         data = {"purpose": purpose.value}
         files = {"file": file.open("rb")}
         response = self._request("POST", "/files", data=data, files=files)
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def get_file(self, file_id: str) -> File:
         """
         Get details for a single file specified by the given `file_id` including status,
         size, purpose, etc.
 
         Parameters
@@ -1329,15 +1329,15 @@
 
         Returns
         -------
         File
             Specified `File` instance.
         """
         response = self._request("GET", f"/files/{file_id}")
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def delete_file(self, file_id: str) -> None:
         """
         Delete the file with the given `file_id`. Deletion is also allowed if a file was
         used, e.g., as training file in a fine-tune job.
 
         Parameters
@@ -1394,15 +1394,15 @@
             "/files/import",
             json={
                 "content_url": content_url,
                 "filename": filename,
                 "purpose": purpose.value,
             },
         )
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def list_fine_tunes(self) -> FineTuneList:
         """
         Get a list of all fine-tune jobs owned by the Azure OpenAI resource. The details
         that are returned for each fine-tune job contain besides its identifier the base
         model, training and validation files, hyper parameters, time stamps, status and
         events. Events are created when the job status changes, e.g. running or
@@ -1410,15 +1410,15 @@
 
         Returns
         -------
         FineTuneList
             `FineTuneList` instance.
         """
         response = self._request("GET", "/fine-tunes")
-        return FineTuneList.parse_obj(response.json())
+        return FineTuneList.model_validate(response.json())
 
     def create_fine_tune(self, fine_tune_request: FineTuneRequest) -> FineTune:
         """
         Create a job that fine-tunes a specified model from a given training file.
         Response includes details of the enqueued job including job status and hyper
         parameters. The name of the fine-tuned model is added to the response once
         complete.
@@ -1434,17 +1434,17 @@
 
         Returns
         -------
         FineTune
             Created `FineTune` instance.
         """
         response = self._request(
-            "POST", "/fine-tunes", json=fine_tune_request.dict(exclude_none=True)
+            "POST", "/fine-tunes", json=fine_tune_request.model_dump(exclude_none=True)
         )
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def get_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Get details for a single fine-tune job specified by the given `fine_tune_id`.
         The details contain the base model, training and validation files, hyper
         parameters, time stamps, status and events. Events are created when the job
         status changes, e.g. running or complete, and when results are uploaded.
@@ -1456,15 +1456,15 @@
 
         Returns
         -------
         FineTune
             Specified `FineTune` instance.
         """
         response = self._request("GET", f"/fine-tunes/{fine_tune_id}")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def delete_fine_tune(self, fine_tune_id: str) -> None:
         """
         Delete the fine-tune job specified by the given `fine_tune_id`.
 
         Parameters
         ----------
@@ -1500,15 +1500,15 @@
             "params": None if stream is None else {"stream": stream},
         }
 
         if stream is True:
             return self._stream(FineTuneEvent, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return FineTuneEventList.parse_obj(response.json())
+        return FineTuneEventList.model_validate(response.json())
 
     def cancel_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Cancel the processing of the fine-tune job specified by the given
         `fine_tune_id`.
 
         Parameters
@@ -1518,29 +1518,29 @@
 
         Returns
         -------
         FineTune
             Canceled `FineTune` instance.
         """
         response = self._request("POST", f"/fine-tunes/{fine_tune_id}/cancel")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def list_models(self) -> ModelList:
         """
         Get a list of all models that are accessible by the Azure OpenAI resource. These
         include base models as well as all successfully completed fine-tuned models
         owned by the Azure OpenAI resource.
 
         Returns
         -------
         ModelList
             `ModelList` instance.
         """
         response = self._request("GET", "/models")
-        return ModelList.parse_obj(response.json())
+        return ModelList.model_validate(response.json())
 
     def get_model(self, model_id: str) -> Model:
         """
         Get details for the model specified by the given `model_id`.
 
         Parameters
         ----------
@@ -1549,15 +1549,15 @@
 
         Returns
         -------
         Model
             Specified `Model` instance.
         """
         response = self._request("GET", f"/models/{model_id}")
-        return Model.parse_obj(response.json())
+        return Model.model_validate(response.json())
 
     def create_completion(
         self, deployment_id: str, completion_request: CompletionRequest
     ) -> Union[Generator[Completion, None, None], Completion]:
         """
         Create a completion for the provided prompt, parameters and chosen model.
 
@@ -1573,22 +1573,22 @@
         Union[Generator[Completion, None, None], Completion]:
             Generator that streams the `Completion` if `completion_request.stream` is
             `True`, or created `Completion` instance otherwise.
         """
         kwargs = {
             "method": "POST",
             "path": f"/deployments/{deployment_id}/completions",
-            "json": completion_request.dict(exclude_none=True),
+            "json": completion_request.model_dump(exclude_none=True),
         }
 
         if completion_request.stream is True:
             return self._stream(Completion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return Completion.parse_obj(response.json())
+        return Completion.model_validate(response.json())
 
     def create_embedding(
         self, deployment_id: str, embedding_request: EmbeddingRequest
     ) -> Embedding:
         """
         Get a vector representation of a given input that can be easily consumed by
         machine learning models and algorithms.
@@ -1604,17 +1604,17 @@
         -------
         Embedding
             Created `Embedding` instance.
         """
         response = self._request(
             "POST",
             f"/deployments/{deployment_id}/embeddings",
-            json=embedding_request.dict(exclude_none=True),
+            json=embedding_request.model_dump(exclude_none=True),
         )
-        return Embedding.parse_obj(response.json())
+        return Embedding.model_validate(response.json())
 
     def create_chat_completion(
         self, deployment_id: str, chat_completion_request: ChatCompletionRequest
     ) -> Union[Generator[ChatCompletion, None, None], ChatCompletion]:
         """
         Create a completion for the chat message.
 
@@ -1631,15 +1631,15 @@
             Generator that streams the `ChatCompletion` if
             `chat_completion_request.stream` is `True`, or created `ChatCompletion`
             instance otherwise.
         """
         kwargs = {
             "method": "POST",
             "path": f"/deployments/{deployment_id}/chat/completions",
-            "json": chat_completion_request.dict(exclude_none=True),
+            "json": chat_completion_request.model_dump(exclude_none=True),
         }
 
         if chat_completion_request.stream is True:
             return self._stream(ChatCompletion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return ChatCompletion.parse_obj(response.json())
+        return ChatCompletion.model_validate(response.json())
```

### Comparing `gpru-0.2.0/gpru/azure/preview_2023_06_01.py` & `gpru-0.3.0/gpru/azure/preview_2023_06_01.py`

 * *Files 2% similar despite different names*

```diff
@@ -1199,15 +1199,15 @@
     user: Optional[str] = None
     """A unique identifier representing your end-user, which can help Azure OpenAI to
     monitor and detect abuse.
     """
 
 
 class ChatCompletionRequest(_ChatCompletionRequestCommon):
-    messages: List[Message] = Field(..., min_items=1)
+    messages: List[Message] = Field(..., min_length=1)
     """The messages to generate chat completions for, in the chat format."""
     n: Optional[int] = Field(1, ge=1, le=128)
     """How many chat completion choices to generate for each input message."""
 
 
 class ExtensionMessage(BaseModel):
     """A chat message for extensions."""
@@ -1331,15 +1331,15 @@
 
         Returns
         -------
         FileList
             `FileList` instance.
         """
         response = self._request("GET", "/files")
-        return FileList.parse_obj(response.json())
+        return FileList.model_validate(response.json())
 
     def upload_file(self, file: Path, purpose: Purpose) -> File:
         """
         Create a new file entity by uploading data from a local machine. Uploaded files
         can, for example, be used for training or evaluating fine-tuned models.
 
         Parameters
@@ -1354,15 +1354,15 @@
         -------
         File
             Uploaded `File` instance.
         """
         data = {"purpose": purpose.value}
         files = {"file": file.open("rb")}
         response = self._request("POST", "/files", data=data, files=files)
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def get_file(self, file_id: str) -> File:
         """
         Get details for a single file specified by the given `file_id` including status,
         size, purpose, etc.
 
         Parameters
@@ -1372,15 +1372,15 @@
 
         Returns
         -------
         File
             Specified `File` instance.
         """
         response = self._request("GET", f"/files/{file_id}")
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def delete_file(self, file_id: str) -> None:
         """
         Delete the file with the given `file_id`. Deletion is also allowed if a file was
         used, e.g., as training file in a fine-tune job.
 
         Parameters
@@ -1437,15 +1437,15 @@
             "/files/import",
             json={
                 "content_url": content_url,
                 "filename": filename,
                 "purpose": purpose.value,
             },
         )
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def list_fine_tunes(self) -> FineTuneList:
         """
         Get a list of all fine-tune jobs owned by the Azure OpenAI resource. The details
         that are returned for each fine-tune job contain besides its identifier the base
         model, training and validation files, hyper parameters, time stamps, status and
         events. Events are created when the job status changes, e.g. running or
@@ -1453,15 +1453,15 @@
 
         Returns
         -------
         FineTuneList
             `FineTuneList` instance.
         """
         response = self._request("GET", "/fine-tunes")
-        return FineTuneList.parse_obj(response.json())
+        return FineTuneList.model_validate(response.json())
 
     def create_fine_tune(self, fine_tune_request: FineTuneRequest) -> FineTune:
         """
         Create a job that fine-tunes a specified model from a given training file.
         Response includes details of the enqueued job including job status and hyper
         parameters. The name of the fine-tuned model is added to the response once
         complete.
@@ -1477,17 +1477,17 @@
 
         Returns
         -------
         FineTune
             Created `FineTune` instance.
         """
         response = self._request(
-            "POST", "/fine-tunes", json=fine_tune_request.dict(exclude_none=True)
+            "POST", "/fine-tunes", json=fine_tune_request.model_dump(exclude_none=True)
         )
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def get_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Get details for a single fine-tune job specified by the given `fine_tune_id`.
         The details contain the base model, training and validation files, hyper
         parameters, time stamps, status and events. Events are created when the job
         status changes, e.g. running or complete, and when results are uploaded.
@@ -1499,15 +1499,15 @@
 
         Returns
         -------
         FineTune
             Specified `FineTune` instance.
         """
         response = self._request("GET", f"/fine-tunes/{fine_tune_id}")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def delete_fine_tune(self, fine_tune_id: str) -> None:
         """
         Delete the fine-tune job specified by the given `fine_tune_id`.
 
         Parameters
         ----------
@@ -1543,15 +1543,15 @@
             "params": None if stream is None else {"stream": stream},
         }
 
         if stream is True:
             return self._stream(FineTuneEvent, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return FineTuneEventList.parse_obj(response.json())
+        return FineTuneEventList.model_validate(response.json())
 
     def cancel_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Cancel the processing of the fine-tune job specified by the given
         `fine_tune_id`.
 
         Parameters
@@ -1561,15 +1561,15 @@
 
         Returns
         -------
         FineTune
             Canceled `FineTune` instance.
         """
         response = self._request("POST", f"/fine-tunes/{fine_tune_id}/cancel")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def create_images(self, image_request: ImageRequest) -> ImageOperation:
         """
         Generate a batch of images from a text caption.
 
         Parameters
         ----------
@@ -1580,31 +1580,31 @@
         -------
         ImageOperation
             Created `ImageOperation` instance.
         """
         response = self._request(
             "POST",
             "/images/generations:submit",
-            json=image_request.dict(exclude_none=True),
+            json=image_request.model_dump(exclude_none=True),
         )
-        return ImageOperation.parse_obj(response.json())
+        return ImageOperation.model_validate(response.json())
 
     def list_models(self) -> ModelList:
         """
         Get a list of all models that are accessible by the Azure OpenAI resource. These
         include base models as well as all successfully completed fine-tuned models
         owned by the Azure OpenAI resource.
 
         Returns
         -------
         ModelList
             `ModelList` instance.
         """
         response = self._request("GET", "/models")
-        return ModelList.parse_obj(response.json())
+        return ModelList.model_validate(response.json())
 
     def get_model(self, model_id: str) -> Model:
         """
         Get details for the model specified by the given `model_id`.
 
         Parameters
         ----------
@@ -1613,15 +1613,15 @@
 
         Returns
         -------
         Model
             Specified `Model` instance.
         """
         response = self._request("GET", f"/models/{model_id}")
-        return Model.parse_obj(response.json())
+        return Model.model_validate(response.json())
 
     def get_image_operation(self, operation_id: str) -> Operation:
         """
         Return the status of the images operation.
 
         Parameters
         ----------
@@ -1630,15 +1630,15 @@
 
         Returns
         -------
         Operation
             Specified `Operation` instance.
         """
         response = self._request("GET", f"/operations/images/{operation_id}")
-        return Operation.parse_obj(response.json())
+        return Operation.model_validate(response.json())
 
     def delete_image_operation(self, operation_id: str) -> None:
         """
         Delete an operation (if in terminal state) and all generated and user provided
         images associated with the operation.
 
         Parameters
@@ -1666,22 +1666,22 @@
         Union[Generator[Completion, None, None], Completion]:
             Generator that streams the `Completion` if `completion_request.stream` is
             `True`, or created `Completion` instance otherwise.
         """
         kwargs = {
             "method": "POST",
             "path": f"/deployments/{deployment_id}/completions",
-            "json": completion_request.dict(exclude_none=True),
+            "json": completion_request.model_dump(exclude_none=True),
         }
 
         if completion_request.stream is True:
             return self._stream(Completion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return Completion.parse_obj(response.json())
+        return Completion.model_validate(response.json())
 
     def create_embedding(
         self, deployment_id: str, embedding_request: EmbeddingRequest
     ) -> Embedding:
         """
         Get a vector representation of a given input that can be easily consumed by
         machine learning models and algorithms.
@@ -1697,17 +1697,17 @@
         -------
         Embedding
             Created `Embedding` instance.
         """
         response = self._request(
             "POST",
             f"/deployments/{deployment_id}/embeddings",
-            json=embedding_request.dict(exclude_none=True),
+            json=embedding_request.model_dump(exclude_none=True),
         )
-        return Embedding.parse_obj(response.json())
+        return Embedding.model_validate(response.json())
 
     def create_chat_completion(
         self, deployment_id: str, chat_completion_request: ChatCompletionRequest
     ) -> Union[Generator[ChatCompletion, None, None], ChatCompletion]:
         """
         Create a completion for the chat message.
 
@@ -1724,22 +1724,22 @@
             Generator that streams the `ChatCompletion` if
             `chat_completion_request.stream` is `True`, or created `ChatCompletion`
             instance otherwise.
         """
         kwargs = {
             "method": "POST",
             "path": f"/deployments/{deployment_id}/chat/completions",
-            "json": chat_completion_request.dict(exclude_none=True),
+            "json": chat_completion_request.model_dump(exclude_none=True),
         }
 
         if chat_completion_request.stream is True:
             return self._stream(ChatCompletion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return ChatCompletion.parse_obj(response.json())
+        return ChatCompletion.model_validate(response.json())
 
     def create_extension_chat_completion(
         self,
         deployment_id: str,
         extension_chat_completion_request: ExtensionChatCompletionRequest,
     ) -> Union[Generator[ExtensionChatCompletion, None, None], ExtensionChatCompletion]:
         """
@@ -1758,15 +1758,15 @@
             Generator that streams the `ExtensionChatCompletion` if
             `extension_chat_completion_request.stream` is `True`, or created
             `ExtensionChatCompletion` instance otherwise.
         """
         kwargs = {
             "method": "POST",
             "path": f"/deployments/{deployment_id}/extensions/chat/completions",
-            "json": extension_chat_completion_request.dict(exclude_none=True),
+            "json": extension_chat_completion_request.model_dump(exclude_none=True),
         }
 
         if extension_chat_completion_request.stream is True:
             return self._stream(ExtensionChatCompletion, **kwargs)  # type: ignore[return-value] # noqa: E501
 
         response = self._request(**kwargs)
-        return ExtensionChatCompletion.parse_obj(response.json())
+        return ExtensionChatCompletion.model_validate(response.json())
```

### Comparing `gpru-0.2.0/gpru/azure/stable_2022_12_01.py` & `gpru-0.3.0/gpru/azure/stable_2022_12_01.py`

 * *Files 3% similar despite different names*

```diff
@@ -974,15 +974,15 @@
 
         Returns
         -------
         DeploymentList
             `DeploymentList` instance.
         """
         response = self._request("GET", "/deployments")
-        return DeploymentList.parse_obj(response.json())
+        return DeploymentList.model_validate(response.json())
 
     def create_deployment(self, deployment: Deployment) -> Deployment:
         """
         Create a new deployment for the Azure OpenAI resource according to the given
         specification.
 
         Parameters
@@ -993,17 +993,17 @@
 
         Returns
         -------
         Deployment
             Created `Deployment` instance.
         """
         response = self._request(
-            "POST", "/deployments", json=deployment.dict(exclude_none=True)
+            "POST", "/deployments", json=deployment.model_dump(exclude_none=True)
         )
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def get_deployment(self, deployment_id: str) -> Deployment:
         """
         Get details for a single deployment specified by the given `deployment_id`.
 
         Parameters
         ----------
@@ -1012,15 +1012,15 @@
 
         Returns
         -------
         Deployment
             Specified `Deployment` instance.
         """
         response = self._request("GET", f"/deployments/{deployment_id}")
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def update_deployment(
         self,
         deployment_id: str,
         model: Optional[str] = None,
         scale_settings: Optional[ScaleSettings] = None,
     ) -> Deployment:
@@ -1040,22 +1040,22 @@
         Returns
         -------
         Deployment
             Updated `Deployment` instance.
         """
         data: Dict[str, Any] = {"model": model}
         if scale_settings is not None:
-            data["scale_settings"] = scale_settings.dict(exclude_none=True)
+            data["scale_settings"] = scale_settings.model_dump(exclude_none=True)
         response = self._request(
             "PATCH",
             f"/deployments/{deployment_id}",
             headers={"Content-Type": "application/merge-patch+json"},
             data=data,
         )
-        return Deployment.parse_obj(response.json())
+        return Deployment.model_validate(response.json())
 
     def delete_deployment(self, deployment_id: str) -> None:
         """
         Delete the deployment specified by the given `deployment_id`.
 
         Parameters
         ----------
@@ -1074,15 +1074,15 @@
 
         Returns
         -------
         FileList
             `FileList` instance.
         """
         response = self._request("GET", "/files")
-        return FileList.parse_obj(response.json())
+        return FileList.model_validate(response.json())
 
     def upload_file(self, file: Path, purpose: Purpose) -> File:
         """
         Create a new file entity by uploading data from a local machine. Uploaded files
         can, for example, be used for training or evaluating fine-tuned models.
 
         Parameters
@@ -1097,15 +1097,15 @@
         -------
         File
             Uploaded `File` instance.
         """
         data = {"purpose": purpose.value}
         files = {"file": file.open("rb")}
         response = self._request("POST", "/files", data=data, files=files)
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def get_file(self, file_id: str) -> File:
         """
         Get details for a single file specified by the given `file_id` including status,
         size, purpose, etc.
 
         Parameters
@@ -1115,15 +1115,15 @@
 
         Returns
         -------
         File
             Specified `File` instance.
         """
         response = self._request("GET", f"/files/{file_id}")
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def delete_file(self, file_id: str) -> None:
         """
         Delete the file with the given `file_id`. Deletion is also allowed if a file was
         used, e.g., as training file in a fine-tune job.
 
         Parameters
@@ -1180,15 +1180,15 @@
             "/files/import",
             json={
                 "content_url": content_url,
                 "filename": filename,
                 "purpose": purpose.value,
             },
         )
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def list_fine_tunes(self) -> FineTuneList:
         """
         Get a list of all fine-tune jobs owned by the Azure OpenAI resource. The details
         that are returned for each fine-tune job contain besides its identifier the base
         model, training and validation files, hyper parameters, time stamps, status and
         events. Events are created when the job status changes, e.g. running or
@@ -1196,15 +1196,15 @@
 
         Returns
         -------
         FineTuneList
             `FineTuneList` instance.
         """
         response = self._request("GET", "/fine-tunes")
-        return FineTuneList.parse_obj(response.json())
+        return FineTuneList.model_validate(response.json())
 
     def create_fine_tune(self, fine_tune_request: FineTuneRequest) -> FineTune:
         """
         Create a job that fine-tunes a specified model from a given training file.
         Response includes details of the enqueued job including job status and hyper
         parameters. The name of the fine-tuned model is added to the response once
         complete.
@@ -1220,17 +1220,17 @@
 
         Returns
         -------
         FineTune
             Created `FineTune` instance.
         """
         response = self._request(
-            "POST", "/fine-tunes", json=fine_tune_request.dict(exclude_none=True)
+            "POST", "/fine-tunes", json=fine_tune_request.model_dump(exclude_none=True)
         )
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def get_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Get details for a single fine-tune job specified by the given `fine_tune_id`.
         The details contain the base model, training and validation files, hyper
         parameters, time stamps, status and events. Events are created when the job
         status changes, e.g. running or complete, and when results are uploaded.
@@ -1242,15 +1242,15 @@
 
         Returns
         -------
         FineTune
             Specified `FineTune` instance.
         """
         response = self._request("GET", f"/fine-tunes/{fine_tune_id}")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def delete_fine_tune(self, fine_tune_id: str) -> None:
         """
         Delete the fine-tune job specified by the given `fine_tune_id`.
 
         Parameters
         ----------
@@ -1286,15 +1286,15 @@
             "params": None if stream is None else {"stream": stream},
         }
 
         if stream is True:
             return self._stream(FineTuneEvent, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return FineTuneEventList.parse_obj(response.json())
+        return FineTuneEventList.model_validate(response.json())
 
     def cancel_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Cancel the processing of the fine-tune job specified by the given
         `fine_tune_id`.
 
         Parameters
@@ -1304,29 +1304,29 @@
 
         Returns
         -------
         FineTune
             Canceled `FineTune` instance.
         """
         response = self._request("POST", f"/fine-tunes/{fine_tune_id}/cancel")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def list_models(self) -> ModelList:
         """
         Get a list of all models that are accessible by the Azure OpenAI resource. These
         include base models as well as all successfully completed fine-tuned models
         owned by the Azure OpenAI resource.
 
         Returns
         -------
         ModelList
             `ModelList` instance.
         """
         response = self._request("GET", "/models")
-        return ModelList.parse_obj(response.json())
+        return ModelList.model_validate(response.json())
 
     def get_model(self, model_id: str) -> Model:
         """
         Get details for the model specified by the given `model_id`.
 
         Parameters
         ----------
@@ -1335,15 +1335,15 @@
 
         Returns
         -------
         Model
             Specified `Model` instance.
         """
         response = self._request("GET", f"/models/{model_id}")
-        return Model.parse_obj(response.json())
+        return Model.model_validate(response.json())
 
     def create_completion(
         self, deployment_id: str, completion_request: CompletionRequest
     ) -> Union[Generator[Completion, None, None], Completion]:
         """
         Create a completion for the provided prompt, parameters and chosen model.
 
@@ -1359,22 +1359,22 @@
         Union[Generator[Completion, None, None], Completion]:
             Generator that streams the `Completion` if `completion_request.stream` is
             `True`, or created `Completion` instance otherwise.
         """
         kwargs = {
             "method": "POST",
             "path": f"/deployments/{deployment_id}/completions",
-            "json": completion_request.dict(exclude_none=True),
+            "json": completion_request.model_dump(exclude_none=True),
         }
 
         if completion_request.stream is True:
             return self._stream(Completion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return Completion.parse_obj(response.json())
+        return Completion.model_validate(response.json())
 
     def create_embedding(
         self, deployment_id: str, embedding_request: EmbeddingRequest
     ) -> Embedding:
         """
         Get a vector representation of a given input that can be easily consumed by
         machine learning models and algorithms.
@@ -1390,10 +1390,10 @@
         -------
         Embedding
             Created `Embedding` instance.
         """
         response = self._request(
             "POST",
             f"/deployments/{deployment_id}/embeddings",
-            json=embedding_request.dict(exclude_none=True),
+            json=embedding_request.model_dump(exclude_none=True),
         )
-        return Embedding.parse_obj(response.json())
+        return Embedding.model_validate(response.json())
```

### Comparing `gpru-0.2.0/gpru/azure/stable_2023_05_15.py` & `gpru-0.3.0/gpru/azure/stable_2023_05_15.py`

 * *Files 2% similar despite different names*

```diff
@@ -976,15 +976,15 @@
         content : str
             The contents of the message.
         """
         super().__init__(role=Role.ASSISTANT, content=content)
 
 
 class ChatCompletionRequest(BaseModel):
-    messages: List[Message] = Field(..., min_items=1)
+    messages: List[Message] = Field(..., min_length=1)
     """The messages to generate chat completions for, in the chat format."""
     temperature: Optional[float] = Field(1.0, ge=0.0, le=2.0)
     """
     What sampling temperature to use, between 0 and 2.
 
     Higher values like 0.8 will make the output more random, while lower values like 0.2
     will make it more focused and deterministic. We generally recommend altering this or
@@ -1114,15 +1114,15 @@
 
         Returns
         -------
         FileList
             `FileList` instance.
         """
         response = self._request("GET", "/files")
-        return FileList.parse_obj(response.json())
+        return FileList.model_validate(response.json())
 
     def upload_file(self, file: Path, purpose: Purpose) -> File:
         """
         Create a new file entity by uploading data from a local machine. Uploaded files
         can, for example, be used for training or evaluating fine-tuned models.
 
         Parameters
@@ -1137,15 +1137,15 @@
         -------
         File
             Uploaded `File` instance.
         """
         data = {"purpose": purpose.value}
         files = {"file": file.open("rb")}
         response = self._request("POST", "/files", data=data, files=files)
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def get_file(self, file_id: str) -> File:
         """
         Get details for a single file specified by the given `file_id` including status,
         size, purpose, etc.
 
         Parameters
@@ -1155,15 +1155,15 @@
 
         Returns
         -------
         File
             Specified `File` instance.
         """
         response = self._request("GET", f"/files/{file_id}")
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def delete_file(self, file_id: str) -> None:
         """
         Delete the file with the given `file_id`. Deletion is also allowed if a file was
         used, e.g., as training file in a fine-tune job.
 
         Parameters
@@ -1220,15 +1220,15 @@
             "/files/import",
             json={
                 "content_url": content_url,
                 "filename": filename,
                 "purpose": purpose.value,
             },
         )
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def list_fine_tunes(self) -> FineTuneList:
         """
         Get a list of all fine-tune jobs owned by the Azure OpenAI resource. The details
         that are returned for each fine-tune job contain besides its identifier the base
         model, training and validation files, hyper parameters, time stamps, status and
         events. Events are created when the job status changes, e.g. running or
@@ -1236,15 +1236,15 @@
 
         Returns
         -------
         FineTuneList
             `FineTuneList` instance.
         """
         response = self._request("GET", "/fine-tunes")
-        return FineTuneList.parse_obj(response.json())
+        return FineTuneList.model_validate(response.json())
 
     def create_fine_tune(self, fine_tune_request: FineTuneRequest) -> FineTune:
         """
         Create a job that fine-tunes a specified model from a given training file.
         Response includes details of the enqueued job including job status and hyper
         parameters. The name of the fine-tuned model is added to the response once
         complete.
@@ -1260,17 +1260,17 @@
 
         Returns
         -------
         FineTune
             Created `FineTune` instance.
         """
         response = self._request(
-            "POST", "/fine-tunes", json=fine_tune_request.dict(exclude_none=True)
+            "POST", "/fine-tunes", json=fine_tune_request.model_dump(exclude_none=True)
         )
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def get_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Get details for a single fine-tune job specified by the given `fine_tune_id`.
         The details contain the base model, training and validation files, hyper
         parameters, time stamps, status and events. Events are created when the job
         status changes, e.g. running or complete, and when results are uploaded.
@@ -1282,15 +1282,15 @@
 
         Returns
         -------
         FineTune
             Specified `FineTune` instance.
         """
         response = self._request("GET", f"/fine-tunes/{fine_tune_id}")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def delete_fine_tune(self, fine_tune_id: str) -> None:
         """
         Delete the fine-tune job specified by the given `fine_tune_id`.
 
         Parameters
         ----------
@@ -1326,15 +1326,15 @@
             "params": None if stream is None else {"stream": stream},
         }
 
         if stream is True:
             return self._stream(FineTuneEvent, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return FineTuneEventList.parse_obj(response.json())
+        return FineTuneEventList.model_validate(response.json())
 
     def cancel_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Cancel the processing of the fine-tune job specified by the given
         `fine_tune_id`.
 
         Parameters
@@ -1344,29 +1344,29 @@
 
         Returns
         -------
         FineTune
             Canceled `FineTune` instance.
         """
         response = self._request("POST", f"/fine-tunes/{fine_tune_id}/cancel")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def list_models(self) -> ModelList:
         """
         Get a list of all models that are accessible by the Azure OpenAI resource. These
         include base models as well as all successfully completed fine-tuned models
         owned by the Azure OpenAI resource.
 
         Returns
         -------
         ModelList
             `ModelList` instance.
         """
         response = self._request("GET", "/models")
-        return ModelList.parse_obj(response.json())
+        return ModelList.model_validate(response.json())
 
     def get_model(self, model_id: str) -> Model:
         """
         Get details for the model specified by the given `model_id`.
 
         Parameters
         ----------
@@ -1375,15 +1375,15 @@
 
         Returns
         -------
         Model
             Specified `Model` instance.
         """
         response = self._request("GET", f"/models/{model_id}")
-        return Model.parse_obj(response.json())
+        return Model.model_validate(response.json())
 
     def create_completion(
         self, deployment_id: str, completion_request: CompletionRequest
     ) -> Union[Generator[Completion, None, None], Completion]:
         """
         Create a completion for the provided prompt, parameters and chosen model.
 
@@ -1399,22 +1399,22 @@
         Union[Generator[Completion, None, None], Completion]:
             Generator that streams the `Completion` if `completion_request.stream` is
             `True`, or created `Completion` instance otherwise.
         """
         kwargs = {
             "method": "POST",
             "path": f"/deployments/{deployment_id}/completions",
-            "json": completion_request.dict(exclude_none=True),
+            "json": completion_request.model_dump(exclude_none=True),
         }
 
         if completion_request.stream is True:
             return self._stream(Completion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return Completion.parse_obj(response.json())
+        return Completion.model_validate(response.json())
 
     def create_embedding(
         self, deployment_id: str, embedding_request: EmbeddingRequest
     ) -> Embedding:
         """
         Get a vector representation of a given input that can be easily consumed by
         machine learning models and algorithms.
@@ -1430,17 +1430,17 @@
         -------
         Embedding
             Created `Embedding` instance.
         """
         response = self._request(
             "POST",
             f"/deployments/{deployment_id}/embeddings",
-            json=embedding_request.dict(exclude_none=True),
+            json=embedding_request.model_dump(exclude_none=True),
         )
-        return Embedding.parse_obj(response.json())
+        return Embedding.model_validate(response.json())
 
     def create_chat_completion(
         self, deployment_id: str, chat_completion_request: ChatCompletionRequest
     ) -> Union[Generator[ChatCompletion, None, None], ChatCompletion]:
         """
         Create a completion for the chat message.
 
@@ -1457,15 +1457,15 @@
             Generator that streams the `ChatCompletion` if
             `chat_completion_request.stream` is `True`, or created `ChatCompletion`
             instance otherwise.
         """
         kwargs = {
             "method": "POST",
             "path": f"/deployments/{deployment_id}/chat/completions",
-            "json": chat_completion_request.dict(exclude_none=True),
+            "json": chat_completion_request.model_dump(exclude_none=True),
         }
 
         if chat_completion_request.stream is True:
             return self._stream(ChatCompletion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return ChatCompletion.parse_obj(response.json())
+        return ChatCompletion.model_validate(response.json())
```

### Comparing `gpru-0.2.0/gpru/openai/api.py` & `gpru-0.3.0/gpru/openai/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,17 +185,17 @@
     model: Union[str, ChatCompletionModel]
     """
     ID of the model to use.
 
     See the [model endpoint compatibility](https://platform.openai.com/docs/models/model-endpoint-compatibility)
     table for details on which models work with the Chat API.
     """
-    messages: List[Message] = Field(..., min_items=1)
+    messages: List[Message] = Field(..., min_length=1)
     """A list of messages comprising the conversation so far."""
-    functions: Optional[List[Function]] = Field(None, min_items=1)
+    functions: Optional[List[Function]] = Field(None, min_length=1)
     """A list of functions the model may generate JSON inputs for."""
     function_call: Union[str, Dict[str, str], None] = None
     """
     Controls how the model responds to function calls.
 
     "none" means the model does not call a function, and responds to the end-user.
     "auto" means the model can pick between an end-user or calling a function.
@@ -1149,18 +1149,20 @@
     input: Union[str, List[str]]
     """The input text to classify."""
     model: Optional[
         Union[str, ModerationModel]
     ] = ModerationModel.TEXT_MODERATION_LATEST
     """
     The default is `ModerationModel.TEXT_MODERATION_LATEST` which will be automatically
-    upgraded over time. This ensures you are always using our most accurate model. If
-    you use `ModerationModel.TEXT_MODERATION_STABLE`, we will provide advanced notice
-    before updating the model. Accuracy of `ModerationModel.TEXT_MODERATION_STABLE` may
-    be slightly lower than for `ModerationModel.TEXT_MODERATION_LATEST`.
+    upgraded over time.
+
+    This ensures you are always using our most accurate model. If you use
+    `ModerationModel.TEXT_MODERATION_STABLE`, we will provide advanced notice before
+    updating the model. Accuracy of `ModerationModel.TEXT_MODERATION_STABLE` may be
+    slightly lower than for `ModerationModel.TEXT_MODERATION_LATEST`.
     """
 
 
 class Categories(BaseModel):
     hate: bool
     hate_threatening: bool = Field(..., alias="hate/threatening")
     self_harm: bool = Field(..., alias="self-harm")
@@ -1293,22 +1295,22 @@
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/chat/create)
         """
         kwargs = {
             "method": "POST",
             "path": "/chat/completions",
-            "json": req.dict(exclude_none=True),
+            "json": req.model_dump(exclude_none=True),
         }
 
         if req.stream is True:
             return self._stream(ChatCompletion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return ChatCompletion.parse_obj(response.json())
+        return ChatCompletion.model_validate(response.json())
 
     def create_completion(
         self, req: CompletionRequest
     ) -> Union[Generator[Completion, None, None], Completion]:
         """
         Create a completion for the provided prompt and parameters.
 
@@ -1326,22 +1328,22 @@
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/completions/create)
         """
         kwargs = {
             "method": "POST",
             "path": "/completions",
-            "json": req.dict(exclude_none=True),
+            "json": req.model_dump(exclude_none=True),
         }
 
         if req.stream is True:
             return self._stream(Completion, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return Completion.parse_obj(response.json())
+        return Completion.model_validate(response.json())
 
     def create_edit(self, req: EditRequest) -> Edit:
         """
         Create a new edit for the provided input, instruction, and parameters.
 
         Parameters
         ----------
@@ -1353,16 +1355,18 @@
         Edit
             Created `Edit` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/edits/create)
         """
-        response = self._request("POST", "/edits", json=req.dict(exclude_none=True))
-        return Edit.parse_obj(response.json())
+        response = self._request(
+            "POST", "/edits", json=req.model_dump(exclude_none=True)
+        )
+        return Edit.model_validate(response.json())
 
     def create_images(self, req: ImageRequest) -> ImageList:
         """
         Create images given a prompt.
 
         Parameters
         ----------
@@ -1375,17 +1379,17 @@
             Created `ImageList` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/images/create)
         """
         response = self._request(
-            "POST", "/images/generations", json=req.dict(exclude_none=True)
+            "POST", "/images/generations", json=req.model_dump(exclude_none=True)
         )
-        return ImageList.parse_obj(response.json())
+        return ImageList.model_validate(response.json())
 
     def edit_image(self, req: ImageEditRequest) -> ImageList:
         """
         Create edited or extended images given an original image and a prompt.
 
         Parameters
         ----------
@@ -1398,15 +1402,15 @@
             Edited or extended `ImageList` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/images/create-edit)
         """
         response = self._request("POST", "/images/edits", **kwargs_for_uploading(req))
-        return ImageList.parse_obj(response.json())
+        return ImageList.model_validate(response.json())
 
     def create_image_variation(self, req: ImageVariationRequest) -> ImageList:
         """
         Create a variation of a given image.
 
         Parameters
         ----------
@@ -1421,15 +1425,15 @@
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/images/create-variation)
         """
         response = self._request(
             "POST", "/images/variations", **kwargs_for_uploading(req)
         )
-        return ImageList.parse_obj(response.json())
+        return ImageList.model_validate(response.json())
 
     def create_embedding(self, req: EmbeddingRequest) -> Embedding:
         """
         Create an embedding vector representing the input text.
 
         Parameters
         ----------
@@ -1442,17 +1446,17 @@
             Created `Embedding` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/embeddings/create)
         """
         response = self._request(
-            "POST", "/embeddings", json=req.dict(exclude_none=True)
+            "POST", "/embeddings", json=req.model_dump(exclude_none=True)
         )
-        return Embedding.parse_obj(response.json())
+        return Embedding.model_validate(response.json())
 
     def transcribe_audio(
         self, req: TranscriptionRequest
     ) -> Union[TranscriptionJson, TranscriptionVerboseJson, str]:
         """
         Transcribe audio into the input language.
 
@@ -1476,18 +1480,18 @@
         response = self._request(
             "POST",
             "/audio/transcriptions",
             **kwargs_for_uploading(req),
         )
 
         if req.response_format is TranscriptionFormat.JSON:
-            return TranscriptionJson.parse_obj(response.json())
+            return TranscriptionJson.model_validate(response.json())
 
         if req.response_format is TranscriptionFormat.VERBOSE_JSON:
-            return TranscriptionVerboseJson.parse_obj(response.json())
+            return TranscriptionVerboseJson.model_validate(response.json())
 
         # text, srt or vtt
         return str(response.text)
 
     def translate_audio(
         self, req: TranslationRequest
     ) -> Union[TranscriptionJson, TranscriptionVerboseJson, str]:
@@ -1512,18 +1516,18 @@
         [Official API reference](https://platform.openai.com/docs/api-reference/audio/create)
         """
         response = self._request(
             "POST", "/audio/translations", **kwargs_for_uploading(req)
         )
 
         if req.response_format is TranscriptionFormat.JSON:
-            return TranscriptionJson.parse_obj(response.json())
+            return TranscriptionJson.model_validate(response.json())
 
         if req.response_format is TranscriptionFormat.VERBOSE_JSON:
-            return TranscriptionVerboseJson.parse_obj(response.json())
+            return TranscriptionVerboseJson.model_validate(response.json())
 
         # text, srt or vtt
         return str(response.text)
 
     def list_files(self) -> FileList:
         """
         Return a list of files that belong to the user's organization.
@@ -1534,15 +1538,15 @@
             `FileList` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/files/list)
         """
         response = self._request("GET", "/files")
-        return FileList.parse_obj(response.json())
+        return FileList.model_validate(response.json())
 
     def upload_file(self, file: Path, purpose: str) -> File:
         """
         Upload a file that contains document(s) to be used across various
         endpoints/features. Currently, the size of all the files uploaded by one
         organization can be up to 1 GB.
 
@@ -1566,15 +1570,15 @@
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/files/upload)
         """
         data = {"purpose": purpose}
         files = {"file": file.open("rb")}
         response = self._request("POST", "/files", data=data, files=files)
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def delete_file(self, file_id: str) -> DeletionResult:
         """
         Delete a file.
 
         Parameters
         ----------
@@ -1587,15 +1591,15 @@
             `DeletionResult` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/files/delete)
         """
         response = self._request("DELETE", f"/files/{file_id}")
-        return DeletionResult.parse_obj(response.json())
+        return DeletionResult.model_validate(response.json())
 
     def get_file(self, file_id: str) -> File:
         """
         Return information about a specific file.
 
         Parameters
         ----------
@@ -1608,15 +1612,15 @@
             Specified `File` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/files/retrieve)
         """
         response = self._request("GET", f"/files/{file_id}")
-        return File.parse_obj(response.json())
+        return File.model_validate(response.json())
 
     def download_file(self, file_id: str) -> str:
         """
         Return the contents of the specified file.
 
         Parameters
         ----------
@@ -1654,17 +1658,17 @@
 
         See Also
         --------
         - [Official API reference](https://platform.openai.com/docs/api-reference/fine-tunes/create)
         - [Learn more about Fine-tuning](https://platform.openai.com/docs/guides/fine-tuning)
         """
         response = self._request(
-            "POST", "/fine-tunes", json=req.dict(exclude_none=True)
+            "POST", "/fine-tunes", json=req.model_dump(exclude_none=True)
         )
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def list_fine_tunes(self) -> FineTuneList:
         """
         List your organization's fine-tuning jobs.
 
         Returns
         -------
@@ -1672,15 +1676,15 @@
             `FineTuneList` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/fine-tunes/list)
         """
         response = self._request("GET", "/fine-tunes")
-        return FineTuneList.parse_obj(response.json())
+        return FineTuneList.model_validate(response.json())
 
     def get_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Get info about the fine-tune job.
 
         Parameters
         ----------
@@ -1694,15 +1698,15 @@
 
         See Also
         --------
         - [Official API reference](https://platform.openai.com/docs/api-reference/fine-tunes/retrieve)
         - [Learn more about Fine-tuning](https://platform.openai.com/docs/guides/fine-tuning)
         """
         response = self._request("GET", f"/fine-tunes/{fine_tune_id}")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def cancel_fine_tune(self, fine_tune_id: str) -> FineTune:
         """
         Immediately cancel a fine-tune job.
 
         Parameters
         ----------
@@ -1715,15 +1719,15 @@
             Canceled `FineTune` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/fine-tunes/cancel)
         """
         response = self._request("POST", f"/fine-tunes/{fine_tune_id}/cancel")
-        return FineTune.parse_obj(response.json())
+        return FineTune.model_validate(response.json())
 
     def list_fine_tune_events(
         self, fine_tune_id: str, stream: Optional[bool] = None
     ) -> Union[Generator[FineTuneEvent, None, None], FineTuneEventList]:
         """
         Get fine-grained status updates for a fine-tune job.
 
@@ -1750,15 +1754,15 @@
             "params": None if stream is None else {"stream": stream},
         }
 
         if stream is True:
             return self._stream(FineTuneEvent, **kwargs)  # type: ignore[return-value]
 
         response = self._request(**kwargs)
-        return FineTuneEventList.parse_obj(response.json())
+        return FineTuneEventList.model_validate(response.json())
 
     def list_models(self) -> ModelList:
         """
         List the currently available models, and provides basic information about each
         one such as the owner and availability.
 
         Returns
@@ -1767,15 +1771,15 @@
             `ModelList` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/models/list)
         """
         response = self._request("GET", "/models")
-        return ModelList.parse_obj(response.json())
+        return ModelList.model_validate(response.json())
 
     def get_model(self, model_id: str) -> Model:
         """
         Retrieve a model instance, providing basic information about the model such as
         the owner and permissioning.
 
         Parameters
@@ -1789,15 +1793,15 @@
             Specified `Model` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/models/retrieve)
         """
         response = self._request("GET", f"/models/{model_id}")
-        return Model.parse_obj(response.json())
+        return Model.model_validate(response.json())
 
     def delete_model(self, model_id: str) -> DeletionResult:
         """
         Delete a fine-tuned model. You must have the owner role in your organization.
 
         Parameters
         ----------
@@ -1810,15 +1814,15 @@
             `DeletionResult` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/fine-tunes/delete-model)
         """
         response = self._request("DELETE", f"/models/{model_id}")
-        return DeletionResult.parse_obj(response.json())
+        return DeletionResult.model_validate(response.json())
 
     def create_moderation(self, req: ModerationRequest) -> Moderation:
         """
         Classify if text violates OpenAI's Content Policy.
 
         Notes
         -----
@@ -1837,10 +1841,10 @@
             Created `Moderation` instance.
 
         See Also
         --------
         [Official API reference](https://platform.openai.com/docs/api-reference/moderations/create)
         """
         response = self._request(
-            "POST", "/moderations", json=req.dict(exclude_none=True)
+            "POST", "/moderations", json=req.model_dump(exclude_none=True)
         )
-        return Moderation.parse_obj(response.json())
+        return Moderation.model_validate(response.json())
```

### Comparing `gpru-0.2.0/.gitignore` & `gpru-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gpru-0.2.0/LICENSE` & `gpru-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpru-0.2.0/README.md` & `gpru-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gpru-0.2.0/pyproject.toml` & `gpru-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Communications :: Chat",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
   "httpx[http2]>=0.24.1",
-  "pydantic>=1.10.9",
+  "pydantic>=2.0.2",
   "tenacity>=8.2.2",
 ]
 description = "Unofficial Python client library for the OpenAI and Azure OpenAI APIs"
 dynamic = ["version"]
 keywords = ["openai", "azure", "chatgpt", "gpt", "gpt-3", "gpt-4", "asyncio", "pydantic"]
 license = "MIT"
 name = "gpru"
@@ -70,15 +70,15 @@
   "coverage report --show-missing",
 ]
 gen-model = "datamodel-codegen --openapi-scopes=schemas --snake-case-field --use-schema-description --use-field-description --reuse-model --capitalise-enum-members --use-subclass-enum --target-python-version=3.7 --wrap-string-literal --output=models.py {args:}"
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 
 [[tool.hatch.envs.all.matrix]]
-# If you are using pyenv, just run `pyenv global 3.7 3.8 3.9 3.10 3.11` beforehand.
+# If you are using pyenv, just run `pyenv shell 3.7 3.8 3.9 3.10 3.11` beforehand.
 python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.docs]
 dependencies = [
   "mkdocs",
 ]
 detached = true
```

### Comparing `gpru-0.2.0/PKG-INFO` & `gpru-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpru
-Version: 0.2.0
+Version: 0.3.0
 Summary: Unofficial Python client library for the OpenAI and Azure OpenAI APIs
 Project-URL: Documentation, https://github.com/sincekmori/gpru#readme
 Project-URL: Issues, https://github.com/sincekmori/gpru/issues
 Project-URL: Source, https://github.com/sincekmori/gpru
 Author-email: Shinsuke Mori <sincekmori@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Requires-Dist: httpx[http2]>=0.24.1
-Requires-Dist: pydantic>=1.10.9
+Requires-Dist: pydantic>=2.0.2
 Requires-Dist: tenacity>=8.2.2
 Description-Content-Type: text/markdown
 
 # GPRU: Unofficial Python Client Library for the OpenAI and Azure OpenAI APIs
 
 **PyPI**
 [![PyPI - Version](https://img.shields.io/pypi/v/gpru.svg)](https://pypi.org/project/gpru)
```

