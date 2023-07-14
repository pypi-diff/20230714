# Comparing `tmp/django_api_decorator-0.1.6.tar.gz` & `tmp/django_api_decorator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_api_decorator-0.1.6.tar", max compression
+gzip compressed data, was "django_api_decorator-0.1.7.tar", max compression
```

## Comparing `django_api_decorator-0.1.6.tar` & `django_api_decorator-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1076 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/LICENSE
--rw-r--r--   0        0        0      373 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/__init__.py
--rw-r--r--   0        0        0      391 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/apps.py
--rw-r--r--   0        0        0    17625 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/decorators.py
--rw-r--r--   0        0        0        0 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/management/__init__.py
--rw-r--r--   0        0        0        0 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/management/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/management/commands/generate_api_schemas.py
--rw-r--r--   0        0        0    13104 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/openapi.py
--rw-r--r--   0        0        0        0 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/py.typed
--rw-r--r--   0        0        0     1574 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/schema_file.py
--rw-r--r--   0        0        0     1601 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/type_utils.py
--rw-r--r--   0        0        0      870 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/types.py
--rw-r--r--   0        0        0     1993 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/django_api_decorator/utils.py
--rw-r--r--   0        0        0     1119 2023-02-15 09:56:58.888101 django_api_decorator-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1188 1970-01-01 00:00:00.000000 django_api_decorator-0.1.6/setup.py
--rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 django_api_decorator-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/LICENSE
+-rw-r--r--   0        0        0      373 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/apps.py
+-rw-r--r--   0        0        0    17702 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/decorators.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/management/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/management/commands/generate_api_schemas.py
+-rw-r--r--   0        0        0    13052 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/openapi.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/py.typed
+-rw-r--r--   0        0        0     1574 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/schema_file.py
+-rw-r--r--   0        0        0     1585 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/type_utils.py
+-rw-r--r--   0        0        0      870 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/types.py
+-rw-r--r--   0        0        0     1993 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/utils.py
+-rw-r--r--   0        0        0     1075 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 django_api_decorator-0.1.7/PKG-INFO
```

### Comparing `django_api_decorator-0.1.6/LICENSE` & `django_api_decorator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.1.6/django_api_decorator/decorators.py` & `django_api_decorator-0.1.7/django_api_decorator/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
     _auth_check = (
         auth_check
         if auth_check is not None
         else getattr(settings, "API_DECORATOR_AUTH_CHECK", default_auth_check)
     )
 
     def decorator(func: Callable[..., Any]) -> Callable[..., HttpResponse]:
-
         signature = inspect.signature(func)
 
         # Get a function that we can call to extract view parameters from
         # the requests query parameters.
         parse_query_params = _get_query_param_parser(
             parameters=signature.parameters, query_params=query_params or []
         )
@@ -111,15 +110,14 @@
             type_annotation=signature.return_annotation
         )
 
         @functools.wraps(func)
         @transaction.non_atomic_requests()
         @require_http_methods([method])
         def inner(request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
-
             # Check if the view requires the user to be logged in and if so make
             # sure the user is actually logged in.
             if login_required and not _auth_check(request):
                 return JsonResponse({"errors": ["Login required"]}, status=401)
 
             try:
                 extra_kwargs = {}
@@ -209,36 +207,33 @@
     try:
         return int(value)
     except (TypeError, ValueError):
         raise ValidationError(f"{query_param_name} must be an integer")
 
 
 def _validate_bool(value: str, *, query_param_name: str) -> bool:
-
     value = value.lower().strip()
 
     if value in ("", "yes", "on", "true", "1"):
         return True
 
     if value in ("no", "off", "false", "0"):
         return False
 
     raise ValidationError(f"{query_param_name} must be a boolean")
 
 
 def _validate_date(value: str, *, query_param_name: str) -> datetime.date:
-
     try:
         return datetime.date.fromisoformat(value)
     except ValueError:
         raise ValidationError(f"{query_param_name} must be a valid date")
 
 
 def _get_validator(parameter: inspect.Parameter) -> Validator:
-
     annotation = parameter.annotation
     if annotation is inspect.Parameter.empty:
         raise ValueError(
             f"Parameter {parameter.name} specified as a query param must have a"
             f" type annotation."
         )
 
@@ -272,15 +267,14 @@
 
 
 def _get_query_param_parser(
     *,
     parameters: Mapping[str, inspect.Parameter],
     query_params: list[str],
 ) -> Callable[[HttpRequest], Mapping[str, Any]]:
-
     query_param_mapping = (
         {query_param.replace("_", "-"): query_param for query_param in query_params}
         if query_params
         else {}
     )
     query_param_validators = {
         query_param: _get_validator(parameters[arg_name])
@@ -289,15 +283,14 @@
     required_params = {
         arg_name
         for query_param, arg_name in query_param_mapping.items()
         if parameters[arg_name].default is inspect.Parameter.empty
     }
 
     def parser(request: HttpRequest) -> Mapping[str, Any]:
-
         validated = {}
 
         for query_param, arg_name in query_param_mapping.items():
             validator = query_param_validators[query_param]
             value = request.GET.get(query_param, _missing)
 
             # If the argument is required, make sure it has a value
@@ -327,15 +320,14 @@
 
 
 def _can_have_body(method: str | None) -> bool:
     return method in ("POST", "PATCH", "PUT")
 
 
 def _get_body_parser(*, parameter: inspect.Parameter) -> BodyParser:
-
     annotation = parameter.annotation
     if annotation is inspect.Parameter.empty:
         raise TypeError("The body parameter must have a type annotation")
 
     body_is_list = is_list(type_annotation=annotation)
     if body_is_list:
         annotation = unwrap_list_item_type(type_annotation=annotation)
@@ -392,23 +384,21 @@
 
 class ResponseEncoder(Protocol):
     def __call__(self, *, payload: Any, status: int) -> HttpResponse:
         ...
 
 
 def _is_class(*, type_annotation: Annotation) -> bool:
-
     return inspect.isclass(type_annotation) and (
         type(type_annotation)
         is not types.GenericAlias  # type: ignore[comparison-overlap]
     )
 
 
 def _get_response_encoder(*, type_annotation: Annotation) -> ResponseEncoder:
-
     type_is_class = _is_class(type_annotation=type_annotation)
 
     if type_is_class and issubclass(type_annotation, HttpResponse):
         return lambda payload, status: payload
 
     if dataclasses.is_dataclass(type_annotation):
         return _dataclass_encoder
@@ -445,15 +435,20 @@
 
     # Assume any other response can be JSON encoded. We might want to restrict
     # this to some verified types 🤔
     return _json_encoder
 
 
 def _json_encoder(*, payload: Any, status: int) -> HttpResponse:
-    return JsonResponse(payload, status=status, safe=False)
+    return JsonResponse(
+        payload,
+        status=status,
+        json_dumps_params={"default": pydantic_encoder},
+        safe=False,
+    )
 
 
 def _pydantic_encoder(payload: Any, status: int) -> HttpResponse:
     return JsonResponse(
         payload,
         status=status,
         json_dumps_params={"default": pydantic_encoder},
@@ -476,15 +471,14 @@
     msg: str
 
 
 def handle_validation_error(
     *,
     exception: (ValidationError | pydantic.ValidationError),
 ) -> HttpResponse:
-
     errors: list[str]
     field_errors: Mapping[str, FieldError]
 
     if isinstance(exception, pydantic.ValidationError):
 
         def error_loc(loc: tuple[int | str, ...]) -> str:
             return ".".join(map(str, loc))
```

### Comparing `django_api_decorator-0.1.6/django_api_decorator/management/commands/generate_api_schemas.py` & `django_api_decorator-0.1.7/django_api_decorator/management/commands/generate_api_schemas.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.1.6/django_api_decorator/openapi.py` & `django_api_decorator-0.1.7/django_api_decorator/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,14 @@
 
     return None, []
 
 
 def paths_and_types_for_view(
     *, view_name: str, callback: Callable[..., HttpResponse], resolved_url: str
 ) -> tuple[dict[str, Any], list[type]]:
-
     api_meta: ApiMeta | None = getattr(callback, "_api_meta", None)
 
     assert api_meta is not None
 
     signature = inspect.signature(callback)
 
     # Types that should be included in the schema object (referenced via
@@ -250,15 +249,15 @@
                 # Tags are useful for grouping operations in codegen
                 "tags": [app_name],
                 "parameters": url_parameters + query_parameters,
                 **additional_data,
                 "responses": {
                     api_meta.response_status: {
                         "description": "",
-                        **api_response,  # type: ignore
+                        **api_response,
                     }
                 },
             }
         }
     }
 
     return paths, types
@@ -316,15 +315,14 @@
             }
         )
 
     return parameters
 
 
 def schemas_for_types(api_types: list[type]) -> dict[str, Any]:
-
     # This only supports Pydantic models for now.
     assert all(
         hasattr(t, "__pydantic_model__") or issubclass(t, BaseModel) for t in api_types
     )
 
     return cast(
         dict[str, Any],
@@ -359,25 +357,24 @@
             continue
 
         if hasattr(pattern.callback, "_method_router_views"):
             # Special handling for method_router(), which has multiple views on the
             # same URL
             for method, callback in cast(
                 dict[str, Callable[..., HttpResponse]],
-                pattern.callback._method_router_views,  # type: ignore
+                pattern.callback._method_router_views,
             ).items():
-
                 if not hasattr(callback, "_api_meta"):
                     logger.debug(
                         "Skipping view %s because it is not using @api decorator",
                         pattern.name,
                     )
                     continue
 
-                api_meta: ApiMeta = callback._api_meta  # type: ignore
+                api_meta: ApiMeta = callback._api_meta
                 assert method == api_meta.method
 
                 operations.append(
                     OpenApiOperation(
                         callback=callback,
                         name=(
                             f"{method.lower()}"
@@ -402,15 +399,14 @@
                 "Skipping view %s because it is not using @api decorator", pattern.name
             )
 
     api_paths: dict[str, Any] = {}
     api_types = []
 
     for operation in operations:
-
         paths, types = paths_and_types_for_view(
             view_name=operation.name,
             callback=operation.callback,
             resolved_url=operation.url,
         )
         api_types += types
```

### Comparing `django_api_decorator-0.1.6/django_api_decorator/schema_file.py` & `django_api_decorator-0.1.7/django_api_decorator/schema_file.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.1.6/django_api_decorator/type_utils.py` & `django_api_decorator-0.1.7/django_api_decorator/type_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,9 +47,9 @@
         type_annotation = unwrap_list_item_type(type_annotation=type_annotation)
     return type_annotation, type_is_list
 
 
 def is_pydantic_model(t: type) -> bool:
     return issubclass(t, pydantic.BaseModel) or (
         hasattr(t, "__pydantic_model__")
-        and issubclass(t.__pydantic_model__, pydantic.BaseModel)  # type: ignore
+        and issubclass(t.__pydantic_model__, pydantic.BaseModel)
     )
```

### Comparing `django_api_decorator-0.1.6/django_api_decorator/types.py` & `django_api_decorator-0.1.7/django_api_decorator/types.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.1.6/django_api_decorator/utils.py` & `django_api_decorator-0.1.7/django_api_decorator/utils.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.1.6/pyproject.toml` & `django_api_decorator-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-api-decorator"
-version = "0.1.6"
+version = "0.1.7"
 description = "A collection of tools to build function based Django APIs"
 authors = ["Oda <tech@oda.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/django-api-decorator"
 repository = "https://github.com/kolonialno/django-api-decorator"
 packages = [{include = "django_api_decorator"}]
@@ -12,23 +12,23 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 Django = ">=3"
 pydantic = "^1.10.2"
 
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-black = "^22.12.0"
-isort = "^5.11.3"
+pytest = "^7.4.0"
+black = "^23.3.0"
+isort = "^5.12.0"
 flake8 = "^6.0.0"
 pytest-django = "^4.5.2"
 flake8-black = "^0.3.6"
-mypy = "^0.981"
-django-stubs = {extras = ["compatible-mypy"], version = "^1.13.1"}
-pytest-mock = "^3.10.0"
+mypy = "^1.4.1"
+django-stubs = "^4.2.3"
+pytest-mock = "^3.11.1"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 target-version = ["py310"]
 line-length = 88
```

### Comparing `django_api_decorator-0.1.6/PKG-INFO` & `django_api_decorator-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-decorator
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of tools to build function based Django APIs
 Home-page: https://github.com/kolonialno/django-api-decorator
 License: MIT
 Author: Oda
 Author-email: tech@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

