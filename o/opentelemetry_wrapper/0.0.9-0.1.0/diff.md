# Comparing `tmp/opentelemetry_wrapper-0.0.9.tar.gz` & `tmp/opentelemetry_wrapper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_wrapper-0.0.9.tar", last modified: Tue Nov 29 10:18:45 2022, max compression
+gzip compressed data, was "opentelemetry_wrapper-0.1.0.tar", last modified: Fri Jul 14 06:44:46 2023, max compression
```

## Comparing `opentelemetry_wrapper-0.0.9.tar` & `opentelemetry_wrapper-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,31 @@
--rw-r--r--   0        0        0     2311 2022-09-27 08:12:51.286165 opentelemetry_wrapper-0.0.9/.gitignore
--rw-r--r--   0        0        0     9229 2022-09-28 02:55:55.816861 opentelemetry_wrapper-0.0.9/LICENSE
--rw-r--r--   0        0        0     2501 2022-11-29 10:18:17.706896 opentelemetry_wrapper-0.0.9/README.md
--rw-r--r--   0        0        0     3775 2022-11-28 10:31:15.575275 opentelemetry_wrapper-0.0.9/TODO.md
--rw-r--r--   0        0        0       60 2022-09-27 08:12:51.287162 opentelemetry_wrapper-0.0.9/aaaa/bbbb.py
--rw-r--r--   0        0        0     3237 2022-09-27 08:12:51.287162 opentelemetry_wrapper-0.0.9/experiment_otel_logging.py
--rw-r--r--   0        0        0     2486 2022-09-27 08:12:51.288159 opentelemetry_wrapper-0.0.9/fastapi_main.py
--rw-r--r--   0        0        0     1055 2022-11-29 10:18:33.859577 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/__init__.py
--rw-r--r--   0        0        0     1433 2022-11-29 09:50:36.908078 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/config/config.py
--rw-r--r--   0        0        0     1024 2022-11-29 09:49:22.064362 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/config/log_level.py
--rw-r--r--   0        0        0     5882 2022-11-29 10:17:05.115821 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/config/service_name.py
--rw-r--r--   0        0        0     1277 2022-11-29 07:53:02.319884 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_dataclasses.py
--rw-r--r--   0        0        0     8818 2022-11-29 07:53:02.283982 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_decorator.py
--rw-r--r--   0        0        0     2656 2022-11-29 07:53:02.335844 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_fastapi.py
--rw-r--r--   0        0        0     4477 2022-11-29 10:17:51.984560 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_logging.py
--rw-r--r--   0        0        0      605 2022-11-29 07:53:02.303929 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_requests.py
--rw-r--r--   0        0        0    14550 2022-11-29 03:14:30.775550 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/introspect.py
--rw-r--r--   0        0        0     7512 2022-09-28 03:30:31.950785 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/json_encoder.py
--rw-r--r--   0        0        0     6002 2022-09-28 03:29:48.386634 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/logging_json_formatter.py
--rw-r--r--   0        0        0     2117 2022-11-29 10:05:37.035599 opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/tracers.py
--rw-r--r--   0        0        0      889 2022-11-29 07:31:46.479401 opentelemetry_wrapper-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      299 2022-11-29 07:31:46.497354 opentelemetry_wrapper-0.0.9/requirements.txt
--rw-r--r--   0        0        0     1496 2022-09-27 08:12:51.295142 opentelemetry_wrapper-0.0.9/setup_otel_logging.py
--rw-r--r--   0        0        0     3294 1970-01-01 00:00:00.000000 opentelemetry_wrapper-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     2311 2022-12-13 07:19:54.176205 opentelemetry_wrapper-0.1.0/.gitignore
+-rw-r--r--   0        0        0     9229 2022-12-13 07:19:54.177203 opentelemetry_wrapper-0.1.0/LICENSE
+-rw-r--r--   0        0        0     6714 2023-04-11 07:27:42.652914 opentelemetry_wrapper-0.1.0/README.md
+-rw-r--r--   0        0        0     2354 2023-06-05 08:01:06.339401 opentelemetry_wrapper-0.1.0/TODO.md
+-rw-r--r--   0        0        0       60 2022-12-13 07:19:54.179199 opentelemetry_wrapper-0.1.0/aaaa/bbbb.py
+-rw-r--r--   0        0        0     3197 2022-12-14 03:19:01.348649 opentelemetry_wrapper-0.1.0/experiment_otel_logging.py
+-rw-r--r--   0        0        0     2487 2023-02-09 03:17:32.396749 opentelemetry_wrapper-0.1.0/fastapi_main.py
+-rw-r--r--   0        0        0     1870 2023-07-14 06:41:00.219877 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/__init__.py
+-rw-r--r--   0        0        0     3652 2023-06-05 02:58:25.364476 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/config/otel_exporter_otlp.py
+-rw-r--r--   0        0        0     1254 2023-02-07 07:06:29.733238 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/config/otel_header_attributes.py
+-rw-r--r--   0        0        0     2230 2022-12-15 07:50:47.979391 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/config/otel_headers.py
+-rw-r--r--   0        0        0     1359 2022-12-13 07:19:54.183188 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/config/otel_log_level.py
+-rw-r--r--   0        0        0     6154 2022-12-14 06:49:31.121402 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/config/otel_service_name.py
+-rw-r--r--   0        0        0      369 2023-02-09 01:34:22.185175 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/fastapi/fastapi_typedef.py
+-rw-r--r--   0        0        0     1310 2022-12-14 06:03:08.846216 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/instrument_dataclasses.py
+-rw-r--r--   0        0        0     9376 2022-12-14 06:03:08.797680 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/instrument_decorator.py
+-rw-r--r--   0        0        0     2438 2023-02-09 01:34:22.138037 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/instrument_fastapi.py
+-rw-r--r--   0        0        0     4757 2023-02-08 09:23:36.385976 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/instrument_logging.py
+-rw-r--r--   0        0        0      638 2022-12-14 06:03:08.959063 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/instrument_requests.py
+-rw-r--r--   0        0        0     3388 2023-02-09 01:34:22.212343 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/instrument_sqlalchemy.py
+-rw-r--r--   0        0        0      153 2022-12-14 03:26:52.894387 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/resource_detector.py
+-rw-r--r--   0        0        0     2864 2023-01-19 09:04:43.095332 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/tracers.py
+-rw-r--r--   0        0        0     1034 2023-02-09 01:34:22.159920 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/sqlalchemy/engine_typedef.py
+-rw-r--r--   0        0        0    14882 2022-12-14 03:46:12.795251 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/utils/introspect.py
+-rw-r--r--   0        0        0     4476 2022-12-14 03:09:31.646597 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/utils/json_encoder.py
+-rw-r--r--   0        0        0     6412 2022-12-14 03:45:32.490449 opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/utils/logging_json_formatter.py
+-rw-r--r--   0        0        0      931 2023-01-16 02:06:31.195899 opentelemetry_wrapper-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      364 2023-01-16 02:06:31.172959 opentelemetry_wrapper-0.1.0/requirements.txt
+-rw-r--r--   0        0        0     1514 2022-12-15 09:33:55.784575 opentelemetry_wrapper-0.1.0/setup_otel_logging.py
+-rw-r--r--   0        0        0      981 2023-02-08 09:20:28.217864 opentelemetry_wrapper-0.1.0/sqlalchemy_example.py
+-rw-r--r--   0        0        0     7521 1970-01-01 00:00:00.000000 opentelemetry_wrapper-0.1.0/PKG-INFO
```

### Comparing `opentelemetry_wrapper-0.0.9/.gitignore` & `opentelemetry_wrapper-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.9/LICENSE` & `opentelemetry_wrapper-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.0.9/experiment_otel_logging.py` & `opentelemetry_wrapper-0.1.0/experiment_otel_logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import logging
 import time
 
 from asgiref.sync import async_to_sync
 from asgiref.sync import sync_to_async
 
-from opentelemetry_wrapper.instrument_decorator import instrument_decorate
-from opentelemetry_wrapper.instrument_logging import instrument_logging
+from opentelemetry_wrapper import instrument_decorate
+from opentelemetry_wrapper import instrument_logging
 
 instrument_logging()
 
 
 @instrument_decorate
 async def bitshift(x: int, shift_by: int):
     """
```

### Comparing `opentelemetry_wrapper-0.0.9/fastapi_main.py` & `opentelemetry_wrapper-0.1.0/fastapi_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 @app.get('/hello')
 def hello() -> str:
     logging.info('called `hello`')
     return 'hello'
 
 
 @app.get('/hello/{name}')
-def hello(name: str) -> str:
+def hello2(name: str) -> str:
     logging.info(f'called `hello/{name}`')
     return 'hello'
 
 
 @app.get('/hello-hello')
 def hello_hello() -> str:
     logging.info('called `hello-hello`')
@@ -65,13 +65,13 @@
     return r.text
 
 
 if __name__ == '__main__':
     uvicorn.run(f'{inspect.getmodulename(__file__)}:app',
                 host='localhost',
                 port=8000,
-                reload=True,
+                # reload=True,
                 access_log=True,
-                # workers=2,  # not valid with reload=True
+                workers=2,  # not valid with reload=True
                 # proxy_headers=True,  # github.com/encode/uvicorn/blob/master/uvicorn/middleware/proxy_headers.py
                 limit_concurrency=128,
                 )
```

### Comparing `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/__init__.py` & `opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 """
 a wrapper around `opentelemetry` and `opentelemetry-instrumentation-*` to make life a bit easier
 """
 
-__version__ = '0.0.9'
+__version__ = '0.1.0'
 
-from opentelemetry_wrapper.config.config import OTEL_WRAPPER_DISABLED
-from opentelemetry_wrapper.instrument_dataclasses import instrument_dataclasses
-from opentelemetry_wrapper.instrument_decorator import instrument_decorate
-from opentelemetry_wrapper.instrument_fastapi import instrument_fastapi
-from opentelemetry_wrapper.instrument_logging import instrument_logging
-from opentelemetry_wrapper.instrument_requests import instrument_requests
+from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_dataclasses import instrument_dataclasses
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_decorator import instrument_decorate
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_fastapi import instrument_fastapi
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_fastapi import instrument_fastapi_app
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_logging import instrument_logging
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_requests import instrument_requests
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_sqlalchemy import instrument_sqlalchemy
 
 
 @instrument_decorate
-def instrument_all():
-
+def instrument_all(dataclasses: bool = True,
+                   logging: bool = True,
+                   fastapi: bool = True,
+                   requests: bool = True,
+                   sqlalchemy: bool = False,  # too noisy for a default
+                   log_json: bool = True,
+                   ):
     # no-op
     if OTEL_WRAPPER_DISABLED:
         return
 
-    # todo: accept kwargs to disable/enable some of these
-    instrument_dataclasses()
-    instrument_logging()
-    instrument_fastapi()
-    instrument_requests()
+    if dataclasses:
+        instrument_dataclasses()
+    if logging:
+        instrument_logging(print_json=log_json)
+    if fastapi:
+        instrument_fastapi()
+    if requests:
+        instrument_requests()
+    if sqlalchemy:
+        instrument_sqlalchemy()
 
 
 __all__ = (
-    __version__,
-    instrument_decorate,
-    instrument_dataclasses,
-    instrument_logging,
-    instrument_fastapi,
-    instrument_requests,
-    instrument_all,
+    '__version__',
+    'instrument_all',
+    'instrument_decorate',
+    'instrument_dataclasses',
+    'instrument_logging',
+    'instrument_fastapi',
+    'instrument_fastapi_app',
+    'instrument_requests',
+    'instrument_sqlalchemy',
 )
```

### Comparing `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/config/log_level.py` & `opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/config/otel_log_level.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 import logging
 import os
 from functools import lru_cache
 
+DEFAULT_LOG_LEVEL = logging.INFO
+
+# https://stackoverflow.com/questions/2031163/when-to-use-the-different-log-levels
+# https://sematext.com/blog/logging-levels/
+# https://www.ibm.com/docs/en/cognos-analytics/10.2.2?topic=SSEP7J_10.2.2/com.ibm.swg.ba.cognos.ug_rtm_wb.10.2.2.doc/c_n30e74.html
 # see logging._nameToLevel, which is protected
-NAME_TO_LEVEL = {
+_NAME_TO_LEVEL = {
     'critical': logging.CRITICAL,
     'fatal':    logging.FATAL,
     'error':    logging.ERROR,
     'warn':     logging.WARNING,
     'warning':  logging.WARNING,
     'info':     logging.INFO,
     'debug':    logging.DEBUG,
+    'trace':    logging.DEBUG,
     'notset':   logging.NOTSET,
 }
 
 
 @lru_cache
-def get_log_level(default=logging.NOTSET) -> int:
+def get_log_level(default=DEFAULT_LOG_LEVEL) -> int:
     _level = os.getenv('OTEL_LOG_LEVEL', '').casefold().strip()
 
     # default
     if not _level:
         return default
 
     # it's an integer, todo: should this be allowed? should there be a min/max?
     if _level.isdigit():
         return int(_level)
 
     # a known level name
-    if _level in NAME_TO_LEVEL:
-        return NAME_TO_LEVEL[_level]
+    if _level in _NAME_TO_LEVEL:
+        return _NAME_TO_LEVEL[_level]
 
     # is it a user-defined level?
     if isinstance(logging.getLevelName(_level), int):
         return logging.getLevelName(_level)
 
     # don't error or warn, just default
     return default
```

### Comparing `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/config/service_name.py` & `opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/config/otel_service_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import getpass
 import os
 import platform
 import socket
 from functools import lru_cache
 from pathlib import Path
 
-from opentelemetry.sdk.resources import OTELResourceDetector
+from opentelemetry_wrapper.dependencies.opentelemetry.resource_detector import get_resource_attributes
 
 
 @lru_cache
 def get_username() -> str:
     # noinspection PyBroadException
     try:
         return getpass.getuser().strip()
@@ -116,24 +116,14 @@
     # todo: also try getting the primary dns suffix from the dns suffix search list
 
     # everything failed, return nothing
     return ''
 
 
 @lru_cache
-def get_namespace() -> str:
-    # get k8s namespace
-    if get_k8s_namespace():
-        return get_k8s_namespace()
-
-    # not in k8s, try to get domain instead
-    return get_domain()
-
-
-@lru_cache
 def get_main_filename() -> str:
     if getattr(__main__, '__file__', None):
         main_full_path = Path(__main__.__file__)  # can be undefined, e.g. C modules or Jupyter notebooks
         if main_full_path.is_file():  # should always be true
             return main_full_path.name
 
     return ''
@@ -149,25 +139,25 @@
     note that this does not follow the opentelemetry spec for `service.name`, which is here:
     https://opentelemetry.io/docs/reference/specification/resource/semantic_conventions/#service
     because this tries to uniquely represent the current running instance
 
     it would be more correct to just return the namespace instead,
     but my preference (for now at least) is to isolate the instance for further debugging
 
-    :return: {username}@{hostname}.{namespace or domain}:<{filename of main}> or an empty string
+    :return: {k8s namespace}/{k8s pod name} or {username}@{hostname}.{domain}:<{filename of main}> or ''
     """
 
     # try return just namespace/pod by default
     if get_k8s_namespace():
         return f'{get_k8s_namespace()}/{get_k8s_pod_name()}'
 
     # formatting
     _username = f'{get_username()}@' if get_username() else ''
     _hostname = get_hostname()
-    _namespace = f'.{get_namespace()}' if get_namespace() else ''
+    _namespace = f'.{get_domain()}' if get_domain() else ''
     _filename = f':<{get_main_filename()}>' if get_main_filename() else ''
 
     # if at least one of the above succeeded, then make sure hostname is not blank
     # _hostname = _hostname if _hostname or not (_username or _namespace or _filename) else '<UNKNOWN_HOST>'
     if not _hostname:
         if _username or _namespace or _filename:
             _hostname = '<UNKNOWN_HOST>'
@@ -180,9 +170,21 @@
     """
     tries these 2 things, in order:
     1. `OTEL_SERVICE_NAME` env var
     2. `service.name` property from `OTEL_RESOURCE_ATTRIBUTES` env var
 
     otherwise, returns an empty string
     """
-    otel_detected_service_name = OTELResourceDetector().detect().attributes.get('service.name', '') or ''
+    otel_detected_service_name = get_resource_attributes().get('service.name', '') or ''
     return str(otel_detected_service_name).strip()
+
+
+def getenv_otel_service_namespace() -> str:
+    """
+    tries these 2 things, in order:
+    1. `OTEL_SERVICE_NAME` env var
+    2. `service.name` property from `OTEL_RESOURCE_ATTRIBUTES` env var
+
+    otherwise, returns an empty string
+    """
+    otel_detected_service_name = get_resource_attributes().get('service.namespace', '') or ''
+    return os.getenv('OTEL_SERVICE_NAMESPACE', '').strip() or str(otel_detected_service_name).strip()
```

### Comparing `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_dataclasses.py` & `opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/instrument_dataclasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 import inspect
 from functools import wraps
 
-from opentelemetry_wrapper.config.config import OTEL_WRAPPER_DISABLED
-from opentelemetry_wrapper.instrument_decorator import instrument_decorate
+from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_decorator import instrument_decorate
 
 _ORIGINAL = None
 
 
 @instrument_decorate
 def instrument_dataclasses() -> None:
     """
```

### Comparing `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_decorator.py` & `opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/instrument_decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import asyncio
 import inspect
 from functools import cached_property
 from functools import wraps
 from typing import Callable
 from typing import Coroutine
+from typing import Dict
 from typing import Optional
 from typing import TypeVar
+from typing import Union
 
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import Status
 from opentelemetry.trace import StatusCode
 
 from opentelemetry_wrapper import __version__  # don't worry, this does not create an infinite import loop
-from opentelemetry_wrapper.config.config import OTEL_WRAPPER_DISABLED
+from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
+from opentelemetry_wrapper.dependencies.opentelemetry.tracers import get_tracer
 from opentelemetry_wrapper.utils.introspect import CodeInfo
-from opentelemetry_wrapper.utils.tracers import get_tracer
 
 _TRACER = get_tracer(__name__, __version__)
-_CACHE_INSTRUMENTED = dict()
-_CACHE_GETATTRIBUTE = dict()
 
-InstrumentableThing = TypeVar("InstrumentableThing", Callable, Coroutine, type)
+InstrumentableThing = TypeVar('InstrumentableThing', Callable, Coroutine, type)
+
+_CACHE_INSTRUMENTED: Dict[InstrumentableThing, Optional[InstrumentableThing]] = dict()  # type: ignore[valid-type]
+_CACHE_GETATTRIBUTE: Dict[InstrumentableThing, InstrumentableThing] = dict()  # type: ignore[valid-type]
 
 
 def instrument_decorate(func: InstrumentableThing,
                         /, *,
                         func_name: Optional[str] = None,
                         ) -> InstrumentableThing:
     """
@@ -51,42 +54,44 @@
     # no-op
     if OTEL_WRAPPER_DISABLED:
         return func
 
     # avoid re-instrumenting (or double-instrumenting) things
     # this requires slightly more complex logic than lru_cache provides
     if func in _CACHE_INSTRUMENTED:
-        if _CACHE_INSTRUMENTED[func] is None:
-            return func
-        return _CACHE_INSTRUMENTED[func]
+        ret = _CACHE_INSTRUMENTED[func]
+        if ret is not None:
+            return ret
+        return func
 
     # if not provided, try to find the function name
     code_info = CodeInfo(func)
     func_name = func_name or code_info.name
 
     # build span attributes for this class / function / method / builtin / etc
-    span_attributes = dict()
+    span_attributes: Dict[str, Union[str, None, int]] = dict()
     if code_info.function_name:
         span_attributes[SpanAttributes.CODE_FUNCTION] = code_info.function_name
     if code_info.module_name:
         span_attributes[SpanAttributes.CODE_NAMESPACE] = code_info.module_name
     if code_info.path:
         span_attributes[SpanAttributes.CODE_FILEPATH] = str(code_info.path)
     if code_info.lineno:
         span_attributes[SpanAttributes.CODE_LINENO] = code_info.lineno
 
+    wrapped: InstrumentableThing
     if inspect.isclass(func):
         # noinspection PyTypeChecker
-        wrapped = _instrument_class(func, func_name, span_attributes)
+        wrapped = _instrument_class(func, func_name, span_attributes)  # type: ignore[assignment]
 
     elif asyncio.iscoroutinefunction(func):  # coroutine functions are also functions, so this must be checked first
-        wrapped = _instrument_coroutine(func, func_name, span_attributes)
+        wrapped = _instrument_coroutine(func, func_name, span_attributes)  # type: ignore[assignment]
 
     elif inspect.isroutine(func):
-        wrapped = _instrument_routine(func, func_name, span_attributes)
+        wrapped = _instrument_routine(func, func_name, span_attributes)  # type: ignore[assignment]
 
     # what is this?
     else:
         raise TypeError(type(func))
 
     # add to cache and return
     _CACHE_INSTRUMENTED[func] = wrapped
@@ -108,15 +113,15 @@
     """
 
     # no-op
     if OTEL_WRAPPER_DISABLED:
         return coro
 
     # sanity checks
-    assert isinstance(coro, Callable)
+    assert isinstance(coro, Callable)  # type: ignore[arg-type]
     assert not isinstance(coro, type)
     assert asyncio.iscoroutinefunction(coro)
 
     @wraps(coro)
     async def wrapped(*args, **kwargs):
         with _TRACER.start_as_current_span(f'async {coro_name}', attributes=span_attributes) as span:
             ret = await coro(*args, **kwargs)
@@ -142,15 +147,15 @@
     """
 
     # no-op
     if OTEL_WRAPPER_DISABLED:
         return func
 
     # sanity checks
-    assert isinstance(func, Callable)
+    assert isinstance(func, Callable)  # type: ignore[arg-type]
     assert not isinstance(func, type)
     assert inspect.isroutine(func)
     assert not asyncio.iscoroutinefunction(func)
 
     @wraps(func)
     def wrapped(*args, **kwargs):
         with _TRACER.start_as_current_span(func_name, attributes=span_attributes) as span:
@@ -189,15 +194,16 @@
 
     # wrap the constructors if they exist
     if cls.__new__ is not object.__new__:
         cls.__new__ = instrument_decorate(cls.__new__, func_name=f'{class_name}.__new__')
     if cls.__init__ is not object.__init__:
         # noinspection PyTypeChecker
         cls.__init__ = instrument_decorate(cls.__init__, func_name=f'{class_name}.__init__')
-    # todo: also wrap __post_init__
+    if hasattr(cls, '__post_init__'):
+        cls.__post_init__ = instrument_decorate(cls.__post_init__, func_name=f'{class_name}.__post_init__')
 
     # also wrap the call method, if it exists
     if not isinstance(cls.__call__, type(object.__call__)):
         cls.__call__ = instrument_decorate(cls.__call__, func_name=f'{class_name}.__call__')
 
     # wrap the generic attribute getter to auto-wrap all methods
     _original_getattribute = cls.__getattribute__
```

### Comparing `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_logging.py` & `opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/instrument_logging.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 import logging
 import sys
 from functools import lru_cache
 from functools import update_wrapper
 from functools import wraps
 from pathlib import Path
 from typing import Optional
+from typing import Set
 from typing import TextIO
 
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
 
-from opentelemetry_wrapper.config.config import OTEL_LOG_LEVEL
-from opentelemetry_wrapper.config.config import OTEL_WRAPPER_DISABLED
-from opentelemetry_wrapper.instrument_decorator import instrument_decorate
+from opentelemetry_wrapper.config.otel_headers import OTEL_LOG_LEVEL
+from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_decorator import instrument_decorate
 from opentelemetry_wrapper.utils.logging_json_formatter import JsonFormatter
 
-# write IDs as 0xBEEF instead of BEEF so it matches the trace json exactly
+# write IDs as 0xBEEF instead of BEEF, so it matches the trace json exactly
 LOGGING_FORMAT_VERBOSE = (
     '%(asctime)s '
     '%(levelname)-8s '
     '[%(name)s] '
     '[%(filename)s:%(funcName)s:%(lineno)d] '
     '[trace_id=0x%(otelTraceID)s span_id=0x%(otelSpanID)s resource.service.name=%(otelServiceName)s] '
     '- %(message)s'
 )
 
-# in the short format, write it as a [traceparent header](https://www.w3.org/TR/trace-context/#traceparent-header)
-LOGGING_FORMAT_MINIMAL = (
-    '%(levelname)-8s '
-    '%(otelServiceName)s '
-    '[00-%(otelTraceID)s-%(otelSpanID)s-01] '
-    '[%(name)s:%(module)s:%(funcName)s] '
-    '%(message)s'
-)
+_CURRENT_ROOT_JSON_HANDLERS: Set[logging.Handler] = set()
 
 
 @lru_cache  # avoid creating duplicate handlers
 def get_json_handler(*,
                      level: int = OTEL_LOG_LEVEL,
                      path: Optional[Path] = None,
                      stream: Optional[TextIO] = None,
                      ) -> logging.Handler:
     if path is not None and stream is not None:
         raise ValueError('cannot set both path and stream')
 
+    handler: logging.Handler
     if path is not None:
         handler = logging.FileHandler(path)
     elif stream is not None:
         handler = logging.StreamHandler(stream=stream)
     else:
         handler = logging.StreamHandler(stream=sys.stderr)
 
@@ -54,70 +49,81 @@
     handler.setLevel(level)
     return handler
 
 
 @instrument_decorate
 def instrument_logging(*,
                        level: int = OTEL_LOG_LEVEL,
+                       path: Optional[Path] = None,
+                       stream: Optional[TextIO] = None,
                        print_json: bool = True,
-                       verbose: bool = True,
-                       force_reinstrumentation: bool = False,
                        ) -> None:
     """
     this function is (by default) idempotent; calling it multiple times has no additional side effects
 
-    :param print_json:
-    :param verbose:
-    :param force_reinstrumentation:
     :param level:
+    :param path:
+    :param stream:
+    :param print_json:
     :return:
     """
+    global _CURRENT_ROOT_JSON_HANDLERS
 
     # no-op
     if OTEL_WRAPPER_DISABLED:
         return
 
     _instrumentor = LoggingInstrumentor()
     if _instrumentor.is_instrumented_by_opentelemetry:
-        if force_reinstrumentation:
-            _instrumentor.uninstrument()
-        else:
-            return
+        _instrumentor.uninstrument()
     _instrumentor.instrument(set_logging_format=False)
     old_factory = logging.getLogRecordFactory()
 
     # the instrumentor failed to use the @wraps decorator so let's do it for them
     # noinspection PyProtectedMember
     if LoggingInstrumentor._old_factory is not None:
         # noinspection PyProtectedMember
         update_wrapper(old_factory, LoggingInstrumentor._old_factory)
 
     @wraps(old_factory)
     def record_factory(*args, **kwargs):
         record = old_factory(*args, **kwargs)
 
         # we want the trace-id and span-id in a log to match the span it was created in
-        # so we format it to match
+        # therefore we format it to match
         # note that logs outside a span will be assigned an invalid trace-id and span-id (all zeroes)
         record.otelTraceID = f'0x{int(record.otelTraceID, 16):032x}'
         record.otelSpanID = f'0x{int(record.otelSpanID, 16):016x}'
 
         return record
 
     logging.setLogRecordFactory(record_factory)
 
+    # un-instrument logging root handler
+    while _CURRENT_ROOT_JSON_HANDLERS:
+        logging.root.removeHandler(_CURRENT_ROOT_JSON_HANDLERS.pop())
+
     # output as json
     if print_json:
-        # todo: take in appropriate args to specify an output (e.g. to a path or stream)
-        # todo: re-instrument correctly if args are different
-        json_handler = get_json_handler(level=level)
-        if json_handler not in logging.root.handlers:
-            logging.root.addHandler(json_handler)
-        logging.root.setLevel(level)
+        if path is not None:
+            _CURRENT_ROOT_JSON_HANDLERS.add(get_json_handler(level=level, path=path))
+        if stream is not None or path is None:
+            _CURRENT_ROOT_JSON_HANDLERS.add(get_json_handler(level=level, stream=stream))
 
-    # output as above logging string format
+    # output as text, using the templated logging string format
     else:
-        # force overwrite of logging basic config since their instrumentor doesn't do it correctly
-        logging.basicConfig(format=LOGGING_FORMAT_VERBOSE if verbose else LOGGING_FORMAT_MINIMAL,
-                            level=level,
-                            force=True,
-                            )
+        # equivalent to logging.basicConfig(format=..., level=level)
+        _formatter = logging.Formatter(fmt=LOGGING_FORMAT_VERBOSE)
+
+        if path is not None:
+            _file_handler = logging.FileHandler(path)
+            _file_handler.setFormatter(_formatter)
+            _CURRENT_ROOT_JSON_HANDLERS.add(_file_handler)
+        if stream is not None or path is None:
+            _stream_handler = logging.StreamHandler(stream)
+            _stream_handler.setFormatter(_formatter)
+            _CURRENT_ROOT_JSON_HANDLERS.add(_stream_handler)
+
+    # set root handlers
+    for _handler in _CURRENT_ROOT_JSON_HANDLERS:
+        logging.root.addHandler(_handler)
+    logging.root.setLevel(level)
```

### Comparing `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/instrument_requests.py` & `opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/instrument_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 
-from opentelemetry_wrapper.config.config import OTEL_WRAPPER_DISABLED
-from opentelemetry_wrapper.instrument_decorator import instrument_decorate
+from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
+from opentelemetry_wrapper.dependencies.opentelemetry.instrument_decorator import instrument_decorate
 
 
 @instrument_decorate
 def instrument_requests():
     """
     this function is idempotent; calling it multiple times has no additional side effects
```

### Comparing `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/introspect.py` & `opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/utils/introspect.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,14 +111,16 @@
 
             # use qualname instead of name if possible, but strip out the class name
             if hasattr(self.__unwrapped_code_object, '__qualname__'):
                 return self.__unwrapped_code_object.__qualname__
         except Exception:
             pass
 
+        return None
+
     @cached_property
     def function_name(self) -> Optional[str]:
         try:
             # a class does not have a function name
             if self.is_class:
                 return None
 
@@ -139,20 +141,22 @@
             # use the code name
             if self.__code__ is not None:
                 if getattr(self.__code__, 'co_name', None):
                     return self.__code__.co_name
         except Exception:
             pass
 
+        return None
+
     @cached_property
     def module(self) -> Optional[ModuleType]:
         try:
             return inspect.getmodule(self.__unwrapped_code_object)
         except Exception:
-            pass
+            return None
 
     @cached_property
     def module_name(self) -> Optional[str]:
         try:
             if self.module is not None:
                 return self.module.__name__
 
@@ -161,32 +165,34 @@
                 _module_name = inspect.getmodulename(str(self.path))
                 if _module_name is not None:
                     _lineno = f':{self.lineno}' if self.lineno else ''
                     return f'<{_module_name}.py{_lineno}>'
         except Exception:
             pass
 
+        return None
+
     @cached_property
-    # flake8: noqa: C901
     def cls(self) -> Optional[type]:
         try:
             # if we already are a class
             if self.is_class:
                 return self.__unwrapped_code_object
 
             # get class of method
             if inspect.ismethod(self.__unwrapped_code_object) or \
                     (inspect.isbuiltin(self.__unwrapped_code_object) and
                      hasattr(self.__unwrapped_code_object, '__self__')):
                 for _attr_name in ('__class__', '__slots__'):
                     _attr = getattr(self.__unwrapped_code_object.__self__, _attr_name, None)
                     if _attr is not None and hasattr(_attr, '__mro__'):
-                        for _cls in inspect.getmro(_attr):
-                            if inspect.isclass(_cls) and self.__unwrapped_code_object.__name__ in _cls.__dict__:
-                                return _cls
+                        for _mro_cls in inspect.getmro(_attr):
+                            if inspect.isclass(_mro_cls):
+                                if self.__unwrapped_code_object.__name__ in _mro_cls.__dict__:
+                                    return _mro_cls
 
             # get class qualname
             if hasattr(self.__unwrapped_code_object, '__qualname__'):
                 _cls_qualname = self.__unwrapped_code_object.__qualname__.split('.<locals>')[0]
                 if '.' in _cls_qualname:
                     _cls_qualname = _cls_qualname.rsplit('.', 1)[0]
                 else:
@@ -216,37 +222,43 @@
             # try harder: load module from path and search inside it to find the class qualname
             if self._maybe_unsafe__try_very_hard_to_find_class and _cls_qualname and not self.module and self.path:
                 _temp_module_name = f'__introspected_file__.{self.path}'
                 if _temp_module_name in sys.modules:
                     _cls = sys.modules[_temp_module_name]
                 else:
                     spec = importlib.util.spec_from_file_location(_temp_module_name, self.path)
-                    _cls = importlib.util.module_from_spec(spec)
-                    sys.modules[_temp_module_name] = _cls
-                    spec.loader.exec_module(_cls)
+                    if spec is not None:
+                        _cls = importlib.util.module_from_spec(spec)
+                        sys.modules[_temp_module_name] = _cls
+                        if spec.loader is not None:
+                            spec.loader.exec_module(_cls)
 
                 for _cls_name in _cls_qualname.split('.'):
                     if _cls is None:
                         break
                     _cls = getattr(_cls, _cls_name, None)
                 else:
                     if _cls is not None:
                         if inspect.isclass(_cls):
                             return _cls
         except Exception:
             pass
 
+        return None
+
     @cached_property
     def class_name(self) -> Optional[str]:
         try:
             if self.cls:
                 return self.cls.__name__
         except Exception:
             pass
 
+        return None
+
     @cached_property
     def path(self) -> Optional[Path]:
         try:
             try:
                 _source_file = inspect.getsourcefile(self.__unwrapped_code_object)
                 if _source_file:
                     return Path(_source_file)
@@ -255,14 +267,16 @@
 
             if self.__code__ is not None:
                 if getattr(self.__code__, 'co_filename', None):
                     return Path(self.__code__.co_filename)
         except Exception:
             pass
 
+        return None
+
     @cached_property
     def lineno(self) -> Optional[int]:
         try:
             try:
                 _source_lines = inspect.getsourcelines(self.__unwrapped_code_object)
                 if _source_lines:
                     return _source_lines[1]
@@ -271,19 +285,21 @@
 
             if self.__code__ is not None:
                 if getattr(self.__code__, 'co_firstlineno', None):
                     return self.__code__.co_firstlineno
         except Exception:
             pass
 
+        return None
+
     @staticmethod
     def __is_supported_type(code_object) -> bool:
         if callable(code_object):
             return True
-        if isinstance(code_object, (Callable, Coroutine, cached_property)):
+        if isinstance(code_object, (Callable, Coroutine, cached_property)):  # type: ignore[arg-type]
             return True
         if isinstance(code_object, asyncio.Task):
             return True
 
         return False
 
     @cached_property
```

### Comparing `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/logging_json_formatter.py` & `opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/utils/logging_json_formatter.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 
     def usesTime(self):
         return self._keys is None or 'asctime' in self._keys
 
     def formatMessage(self, record: logging.LogRecord):
         raise DeprecationWarning
 
-    # flake8: noqa: C901
     def format(self, record):
         """
         Format the specified record as text.
 
         The record's attribute dictionary is used as the operand to a
         string formatting operation which yields the returned string.
         Before formatting the dictionary, a couple of preparatory steps
@@ -135,19 +134,27 @@
                 else:
                     # noinspection PyBroadException
                     try:
                         safe_log_data[k] = repr(v)
                     except Exception:
                         continue  # failed, skip key
 
-        # truncate extremely long things
-        # todo: handle other jsonable object types more intelligently
-        for k, v in safe_log_data.items():
-            if isinstance(v, str) and len(v) > self.max_string_length:
-                safe_log_data[k] = f'{v[:self.max_string_length - 15]}... (TRUNCATED)'
+        # truncate extremely long strings (values nested in dicts and lists, but not dict keys)
+        stack = [safe_log_data]
+        while stack:
+            elem = stack.pop()
+            if isinstance(elem, dict):
+                for k, v in elem.items():
+                    if isinstance(v, (dict, list)):
+                        stack.append(v)
+                    if isinstance(v, str) and len(v) > self.max_string_length:
+                        elem[k] = f'{v[:self.max_string_length - 15]}... (TRUNCATED)'[:self.max_string_length]
+            if isinstance(elem, list):
+                for i, item in enumerate(elem):
+                    elem[i] = f'{item[:self.max_string_length - 15]}... (TRUNCATED)'[:self.max_string_length]
 
         return json.dumps(safe_log_data,
                           ensure_ascii=self.ensure_ascii,
                           allow_nan=self.allow_nan,
                           indent=self.indent,
                           separators=self.separators,
                           sort_keys=self.sort_keys)
```

### Comparing `opentelemetry_wrapper-0.0.9/opentelemetry_wrapper/utils/tracers.py` & `opentelemetry_wrapper-0.1.0/opentelemetry_wrapper/dependencies/opentelemetry/tracers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,57 @@
+import json
 from functools import lru_cache
 from typing import Optional
 
 from opentelemetry import trace
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.resources import SERVICE_NAME
 from opentelemetry.sdk.resources import SERVICE_NAMESPACE
 from opentelemetry.sdk.trace import ReadableSpan
-from opentelemetry.sdk.trace import Tracer
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.sdk.trace.export import ConsoleSpanExporter
 
-from opentelemetry_wrapper.config.config import OTEL_EXPORTER_OTLP_ENDPOINT
-from opentelemetry_wrapper.config.config import OTEL_SERVICE_NAME
-from opentelemetry_wrapper.config.config import OTEL_SERVICE_NAMESPACE
+from opentelemetry_wrapper.config.otel_headers import OTEL_EXPORTER_OTLP_ENDPOINT
+from opentelemetry_wrapper.config.otel_headers import OTEL_EXPORTER_OTLP_HEADER
+from opentelemetry_wrapper.config.otel_headers import OTEL_EXPORTER_OTLP_INSECURE
+from opentelemetry_wrapper.config.otel_headers import OTEL_SERVICE_NAME
+from opentelemetry_wrapper.config.otel_headers import OTEL_SERVICE_NAMESPACE
 
 
 @lru_cache  # only run once
-def init_tracer():
+def init_tracer_provider():
     if OTEL_SERVICE_NAMESPACE:
         tp = TracerProvider(resource=Resource.create({SERVICE_NAME:      OTEL_SERVICE_NAME,
                                                       SERVICE_NAMESPACE: OTEL_SERVICE_NAMESPACE}))
     else:
         tp = TracerProvider(resource=Resource.create({SERVICE_NAME: OTEL_SERVICE_NAME}))
 
     # noinspection PyProtectedMember
     trace._set_tracer_provider(tp, log=False)  # try to set, but don't warn otherwise
     if trace.get_tracer_provider() is tp:  # if we succeeded in setting it, set it up
         def format_span(span: ReadableSpan) -> str:
-            return f'{span.to_json(indent=None)}\n'
+            span_json_str = span.to_json(indent=None)
+
+            # add duration in seconds
+            if span.start_time and span.end_time:
+                span_json_obj = json.loads(span_json_str)
+                span_json_obj['duration_ns'] = span.end_time - span.start_time
+                span_json_str = json.dumps(span_json_obj, indent=None)
+
+            return f'{span_json_str}\n'
 
         tp.add_span_processor(BatchSpanProcessor(ConsoleSpanExporter(formatter=format_span)))
 
         if OTEL_EXPORTER_OTLP_ENDPOINT:
-            tp.add_span_processor(BatchSpanProcessor(OTLPSpanExporter(OTEL_EXPORTER_OTLP_ENDPOINT)))
+            tp.add_span_processor(BatchSpanProcessor(OTLPSpanExporter(endpoint=OTEL_EXPORTER_OTLP_ENDPOINT,
+                                                                      headers=OTEL_EXPORTER_OTLP_HEADER,
+                                                                      insecure=OTEL_EXPORTER_OTLP_INSECURE)))
 
 
 def get_tracer(instrumenting_module_name: str,
                instrumenting_library_version: Optional[str] = None,
-               ) -> Tracer:
-    init_tracer()
+               ) -> trace.Tracer:
+    init_tracer_provider()
     return trace.get_tracer(instrumenting_module_name=instrumenting_module_name,
                             instrumenting_library_version=instrumenting_library_version)
```

### Comparing `opentelemetry_wrapper-0.0.9/pyproject.toml` & `opentelemetry_wrapper-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "opentelemetry_wrapper"
-authors = [{name = "Avery Khoo", email = "averykhoo@gmail.com"}]
+authors = [{ name = "Avery Khoo", email = "averykhoo@gmail.com" }]
 readme = "README.md"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 dynamic = ["version", "description"]
 requires-python = ">3.8.0"
+
+# NOTE: also update requirements.txt
 dependencies = [
     "asgiref",
     "fastapi",
     "itsdangerous",
     "opentelemetry-api",
     "opentelemetry-exporter-otlp",
     "opentelemetry-instrumentation-fastapi",
     "opentelemetry-instrumentation-logging",
     "opentelemetry-instrumentation-requests",
-#    "opentelemetry-instrumentation-sqlalchemy",
+    "opentelemetry-instrumentation-sqlalchemy",
     "opentelemetry-sdk",
     "requests",
-#    "sqlalchemy",
+    "sqlalchemy",
     "starlette",
     "uvicorn",
 ]
 
 [project.urls]
 Home = "https://github.com/averykhoo/opentelemetry_wrapper"
```

### Comparing `opentelemetry_wrapper-0.0.9/setup_otel_logging.py` & `opentelemetry_wrapper-0.1.0/setup_otel_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from functools import lru_cache
 
-from opentelemetry_wrapper.instrument_dataclasses import instrument_dataclasses
-from opentelemetry_wrapper.instrument_decorator import instrument_decorate
-from opentelemetry_wrapper.instrument_logging import instrument_logging
+from opentelemetry_wrapper import instrument_dataclasses
+from opentelemetry_wrapper import instrument_decorate
+from opentelemetry_wrapper import instrument_logging
 
 if __name__ == '__main__':
     instrument_dataclasses()
     from dataclasses import dataclass
 
 
     @dataclass  # (frozen=True)
@@ -45,21 +45,26 @@
             return
 
         @property
         def e(self):
             logging.info('A.e')
             return 1
 
+        @e.setter
+        def e(self, value):
+            return
+
 
     @instrument_decorate
     @lru_cache
     def f(x):
         return x + 1
 
 
     instrument_logging()
     A().b()
     A().c()()
     A()()
     A().__class__
     A().e
+    A().e
     A().x
```

