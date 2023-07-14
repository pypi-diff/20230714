# Comparing `tmp/hyperdx_opentelemetry-0.0.1.tar.gz` & `tmp/hyperdx_opentelemetry-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdx_opentelemetry-0.0.1.tar", max compression
+gzip compressed data, was "hyperdx_opentelemetry-0.0.2.tar", max compression
```

## Comparing `hyperdx_opentelemetry-0.0.1.tar` & `hyperdx_opentelemetry-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-07-13 00:34:40.461547 hyperdx_opentelemetry-0.0.1/LICENSE
--rw-r--r--   0        0        0     1580 2023-07-13 07:05:50.722511 hyperdx_opentelemetry-0.0.1/README.md
--rw-r--r--   0        0        0      820 2023-07-13 07:20:25.744484 hyperdx_opentelemetry-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      122 2023-07-13 06:39:41.676876 hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/__init__.py
--rw-r--r--   0        0        0     1373 2023-07-13 06:54:02.327463 hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/baggage.py
--rw-r--r--   0        0        0     2672 2023-07-13 06:39:09.453479 hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/distro.py
--rw-r--r--   0        0        0     1601 2023-07-13 06:39:14.131376 hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/metrics.py
--rw-r--r--   0        0        0    15103 2023-07-13 06:31:54.162307 hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/options.py
--rw-r--r--   0        0        0      826 2023-07-13 06:35:40.043017 hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/resource.py
--rw-r--r--   0        0        0     3172 2023-07-13 06:34:37.078271 hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/sampler.py
--rw-r--r--   0        0        0     1818 2023-07-13 06:33:47.851726 hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/trace.py
--rw-r--r--   0        0        0       99 2023-07-13 01:54:38.990328 hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/version.py
--rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 hyperdx_opentelemetry-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-13 00:34:40.461547 hyperdx_opentelemetry-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1580 2023-07-13 07:05:50.722511 hyperdx_opentelemetry-0.0.2/README.md
+-rw-r--r--   0        0        0      820 2023-07-14 00:22:56.720578 hyperdx_opentelemetry-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-07-13 23:59:18.772014 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/__init__.py
+-rw-r--r--   0        0        0     1373 2023-07-13 06:54:02.327463 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/baggage.py
+-rw-r--r--   0        0        0     3020 2023-07-14 00:22:56.721145 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/distro.py
+-rw-r--r--   0        0        0     1601 2023-07-14 00:22:56.721389 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/logs.py
+-rw-r--r--   0        0        0     3313 2023-07-14 00:22:56.721663 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/manual.py
+-rw-r--r--   0        0        0     1601 2023-07-13 06:39:14.131376 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/metrics.py
+-rw-r--r--   0        0        0    17854 2023-07-14 00:22:56.721984 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/options.py
+-rw-r--r--   0        0        0      826 2023-07-13 06:35:40.043017 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/resource.py
+-rw-r--r--   0        0        0     3172 2023-07-13 06:34:37.078271 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/sampler.py
+-rw-r--r--   0        0        0     1818 2023-07-13 06:33:47.851726 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/trace.py
+-rw-r--r--   0        0        0       99 2023-07-13 01:54:38.990328 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/version.py
+-rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 hyperdx_opentelemetry-0.0.2/PKG-INFO
```

### Comparing `hyperdx_opentelemetry-0.0.1/LICENSE` & `hyperdx_opentelemetry-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.1/README.md` & `hyperdx_opentelemetry-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.1/pyproject.toml` & `hyperdx_opentelemetry-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperdx-opentelemetry"
-version = "0.0.1"
+version = "0.0.2"
 description = "HyperDX OpenTelemetry Distro for Python"
 authors = ["HyperDX <support@hyperdx.io>"]
 readme = "README.md"
 packages = [{include = "hyperdx", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.7, >= 3.7.2"
```

### Comparing `hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/baggage.py` & `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/baggage.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/distro.py` & `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/distro.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 from logging import getLogger
 from typing import Optional
 
 from opentelemetry.instrumentation.distro import BaseDistro
 from opentelemetry.metrics import set_meter_provider
 from opentelemetry.trace import set_tracer_provider
 
+from hyperdx.opentelemetry.logs import set_logging_handler
+from hyperdx.opentelemetry.manual import (
+    configure_custom_env_vars,
+    instrument_custom_libs,
+)
 from hyperdx.opentelemetry.metrics import create_meter_provider
 from hyperdx.opentelemetry.options import HyperDXOptions
 from hyperdx.opentelemetry.resource import create_resource
 from hyperdx.opentelemetry.trace import create_tracer_provider
 
 _logger = getLogger(__name__)
 
@@ -45,18 +50,24 @@
         Note: API key is a required option.
     """
     if options is None:
         options = HyperDXOptions()
     _logger.info("Configuring OpenTelemetry using HyperDX distro")
     _logger.debug(vars(options))
     resource = create_resource(options)
-    set_tracer_provider(create_tracer_provider(options, resource))
+    configure_custom_env_vars(options, resource)
+
+    tracer_provider = create_tracer_provider(options, resource)
+    set_tracer_provider(tracer_provider)
+    set_logging_handler(options)
     if options.metrics_dataset:
         set_meter_provider(create_meter_provider(options, resource))
 
+    instrument_custom_libs(options, resource, tracer_provider)
+
 
 # pylint: disable=too-few-public-methods
 class HyperDXDistro(BaseDistro):
     """
     An extension of the base python OpenTelemetry distro, which provides
     a mechanism to automatically configure some of the more common options
     for users. This class is auto-detected by the `opentelemetry-instrument`
```

### Comparing `hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/metrics.py` & `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/metrics.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/options.py` & `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/options.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,91 @@
 import logging
 import os
 from opentelemetry.sdk.environment_variables import (
     OTEL_EXPORTER_OTLP_ENDPOINT,
     OTEL_EXPORTER_OTLP_INSECURE,
+    OTEL_EXPORTER_OTLP_LOGS_ENDPOINT,
+    OTEL_EXPORTER_OTLP_LOGS_INSECURE,
+    OTEL_EXPORTER_OTLP_LOGS_PROTOCOL,
     OTEL_EXPORTER_OTLP_METRICS_ENDPOINT,
     OTEL_EXPORTER_OTLP_METRICS_INSECURE,
     OTEL_EXPORTER_OTLP_METRICS_PROTOCOL,
     OTEL_EXPORTER_OTLP_PROTOCOL,
     OTEL_EXPORTER_OTLP_TRACES_ENDPOINT,
     OTEL_EXPORTER_OTLP_TRACES_INSECURE,
     OTEL_EXPORTER_OTLP_TRACES_PROTOCOL,
     OTEL_LOG_LEVEL,
-    OTEL_SERVICE_NAME
+    OTEL_SERVICE_NAME,
 )
 from grpc import ssl_channel_credentials
 
 # Environment Variable Names
-OTEL_SERVICE_VERSION = "OTEL_SERVICE_VERSION"
 DEBUG = "DEBUG"
 HYPERDX_ENABLE_LOCAL_VISUALIZATIONS = "HYPERDX_ENABLE_LOCAL_VISUALIZATIONS"
+OTEL_SERVICE_VERSION = "OTEL_SERVICE_VERSION"
 SAMPLE_RATE = "SAMPLE_RATE"
 
 # HNY Credential Names
-HYPERDX_API_KEY = "HYPERDX_API_KEY"
 HYPERDX_API_ENDPOINT = "HYPERDX_API_ENDPOINT"
-HYPERDX_TRACES_APIKEY = "HYPERDX_TRACES_APIKEY"
+HYPERDX_API_KEY = "HYPERDX_API_KEY"
 HYPERDX_DATASET = "HYPERDX_DATASET"
+HYPERDX_LOGS_APIKEY = "HYPERDX_LOGS_APIKEY"
 HYPERDX_METRICS_APIKEY = "HYPERDX_METRICS_APIKEY"
 HYPERDX_METRICS_DATASET = "HYPERDX_METRICS_DATASET"
+HYPERDX_TRACES_APIKEY = "HYPERDX_TRACES_APIKEY"
 
 # Default values
 DEFAULT_API_ENDPOINT = "https://in-otel.hyperdx.io"
 DEFAULT_EXPORTER_PROTOCOL = "http/protobuf"
-DEFAULT_SERVICE_NAME = "unknown_service:python"
 DEFAULT_LOG_LEVEL = "ERROR"
 DEFAULT_SAMPLE_RATE = 1
+DEFAULT_SERVICE_NAME = "unknown_service:python"
 
 # Errors and Warnings
-INVALID_DEBUG_ERROR = "Unable to parse DEBUG environment variable. " + \
-    "Defaulting to False."
-INVALID_INSECURE_ERROR = "Unable to parse " + \
-    "OTEL_EXPORTER_OTLP_INSECURE. Defaulting to False."
-INVALID_LOCAL_VIS_ERROR = "Unable to parse " + \
-    "HYPERDX_ENABLE_LOCAL_VISUALIZATIONS environment variable. " + \
-    "Defaulting to false."
-INVALID_METRICS_INSECURE_ERROR = "Unable to parse " + \
-    "OTEL_EXPORTER_OTLP_METRICS_INSECURE. Defaulting to False."
-INVALID_TRACES_INSECURE_ERROR = "Unable to parse " + \
-    "OTEL_EXPORTER_OTLP_TRACES_INSECURE. Defaulting to False."
-INVALID_SAMPLE_RATE_ERROR = "Unable to parse SAMPLE_RATE. " + \
-    "Using sample rate of 1."
-INVALID_EXPORTER_PROTOCOL_ERROR = "Invalid OTLP exporter protocol " + \
-    "detected. Must be one of ['grpc', 'http/protobuf']. Defaulting to grpc."
-MISSING_API_KEY_ERROR = "Missing API key. Specify either " + \
-    "HYPERDX_API_KEY environment variable or apikey in the options" + \
-    "parameter."
-MISSING_SERVICE_NAME_ERROR = "Missing service name. Specify either " + \
-    "OTEL_SERVICE_NAME environment variable or service_name in the " + \
-    "options parameter. If left unset, this will show up in HyperDX " + \
-    "as unknown_service:python"
-MISSING_DATASET_ERROR = "Missing dataset. Specify either " + \
-    "HYPERDX_DATASET environment variable or dataset in the options " + \
-    "parameter."
+INVALID_DEBUG_ERROR = (
+    "Unable to parse DEBUG environment variable. " + "Defaulting to False."
+)
+INVALID_INSECURE_ERROR = (
+    "Unable to parse " + "OTEL_EXPORTER_OTLP_INSECURE. Defaulting to False."
+)
+INVALID_LOCAL_VIS_ERROR = (
+    "Unable to parse "
+    + "HYPERDX_ENABLE_LOCAL_VISUALIZATIONS environment variable. "
+    + "Defaulting to false."
+)
+INVALID_LOGS_INSECURE_ERROR = (
+    "Unable to parse " + "OTEL_EXPORTER_OTLP_LOGS_INSECURE. Defaulting to False."
+)
+INVALID_METRICS_INSECURE_ERROR = (
+    "Unable to parse " + "OTEL_EXPORTER_OTLP_METRICS_INSECURE. Defaulting to False."
+)
+INVALID_TRACES_INSECURE_ERROR = (
+    "Unable to parse " + "OTEL_EXPORTER_OTLP_TRACES_INSECURE. Defaulting to False."
+)
+INVALID_SAMPLE_RATE_ERROR = "Unable to parse SAMPLE_RATE. " + "Using sample rate of 1."
+INVALID_EXPORTER_PROTOCOL_ERROR = (
+    "Invalid OTLP exporter protocol "
+    + "detected. Must be one of ['grpc', 'http/protobuf']. Defaulting to http/protobuf."
+)
+MISSING_API_KEY_ERROR = (
+    "Missing API key. Specify either "
+    + "HYPERDX_API_KEY environment variable or apikey in the options"
+    + "parameter."
+)
+MISSING_SERVICE_NAME_ERROR = (
+    "Missing service name. Specify either "
+    + "OTEL_SERVICE_NAME environment variable or service_name in the "
+    + "options parameter. If left unset, this will show up in HyperDX "
+    + "as unknown_service:python"
+)
+MISSING_DATASET_ERROR = (
+    "Missing dataset. Specify either "
+    + "HYPERDX_DATASET environment variable or dataset in the options "
+    + "parameter."
+)
 IGNORED_DATASET_ERROR = "Dataset is ignored in favor of service name."
 # not currently supported in OTel SDK, open PR:
 # https://github.com/open-telemetry/opentelemetry-specification/issues/1901
 
 log_levels = {
     "NOTSET": logging.NOTSET,
     "DEBUG": logging.DEBUG,
@@ -74,18 +94,15 @@
     "ERROR": logging.ERROR,
     "CRITICAL": logging.CRITICAL,
 }
 
 EXPORTER_PROTOCOL_GRPC = "grpc"
 EXPORTER_PROTOCOL_HTTP_PROTO = "http/protobuf"
 
-exporter_protocols = {
-    EXPORTER_PROTOCOL_GRPC,
-    EXPORTER_PROTOCOL_HTTP_PROTO
-}
+exporter_protocols = {EXPORTER_PROTOCOL_GRPC, EXPORTER_PROTOCOL_HTTP_PROTO}
 
 _logger = logging.getLogger(__name__)
 
 
 def is_classic(apikey: str) -> bool:
     """
     Determines whether the passed in API key is a classic API key or not.
@@ -94,17 +111,17 @@
 
     Returns:
         bool: true if the api key is a classic key, false if not
     """
     return apikey and len(apikey) == 32
 
 
-def parse_bool(environment_variable: str,
-               default_value: bool,
-               error_message: str) -> bool:
+def parse_bool(
+    environment_variable: str, default_value: bool, error_message: str
+) -> bool:
     """
     Attempts to parse the provided environment variable into a bool. If it
     does not exist or fails parse, the default value is returned instead.
 
     Args:
         environment_variable (str): the environment variable name to use
         default_value (bool): the default value if not found or unable parse
@@ -118,18 +135,17 @@
         try:
             return bool(val)
         except ValueError:
             _logger.warning(error_message)
     return default_value
 
 
-def parse_int(environment_variable: str,
-              param: int,
-              default_value: int,
-              error_message: str) -> int:
+def parse_int(
+    environment_variable: str, param: int, default_value: int, error_message: str
+) -> int:
     """
     Attempts to parse the provided environment variable into an int. If it
     does not exist or fails parse, the default value is returned instead.
 
     Args:
         environment_variable (str): the environment variable name to use
         param(int): fallback parameter to check before setting default
@@ -174,228 +190,271 @@
         string: the endpoint, optionally appended with metrics path
     """
     if endpoint and protocol == "http/protobuf":
         return "/".join([endpoint.strip("/"), "v1/metrics"])
     return endpoint
 
 
+def _append_logs_path(protocol: str, endpoint: str) -> str:
+    """
+    Appends the OTLP metrics HTTP path '/v1/metrics' to the endpoint if the
+    protocol is http/protobuf.
+
+    Returns:
+        string: the endpoint, optionally appended with metrics path
+    """
+    if endpoint and protocol == "http/protobuf":
+        return "/".join([endpoint.strip("/"), "v1/logs"])
+    return endpoint
+
+
 # pylint: disable=too-many-arguments,too-many-instance-attributes
 class HyperDXOptions:
     """
     HyperDX Options used to configure the OpenTelemetry SDK.
 
     Setting the debug flag TRUE enables verbose logging and sets the
     OTEL_LOG_LEVEL to DEBUG.
 
     An option set as an environment variable will override any existing
     options declared as parameter variables, if neither are present it
     will fall back to the default value.
 
     Defaults are declared at the top of this file, i.e. DEFAULT_SAMPLE_RATE = 1
     """
+
     traces_apikey = None
     metrics_apikey = None
+    logs_apikey = None
     service_name = DEFAULT_SERVICE_NAME
     service_version = None
     endpoint = DEFAULT_API_ENDPOINT
     traces_endpoint = None
     metrics_endpoint = None
+    logs_endpoint = None
     traces_endpoint_insecure = False
     metrics_endpoint_insecure = False
+    logs_endpoint_insecure = False
     traces_exporter_protocol = DEFAULT_EXPORTER_PROTOCOL
     metrics_exporter_protocol = DEFAULT_EXPORTER_PROTOCOL
+    logs_exporter_protocol = DEFAULT_EXPORTER_PROTOCOL
     sample_rate = DEFAULT_SAMPLE_RATE
     debug = False
     log_level = DEFAULT_LOG_LEVEL
     dataset = None
     metrics_dataset = None
     enable_local_visualizations = False
 
     # pylint: disable=too-many-locals,too-many-branches,too-many-statements
     def __init__(
         self,
         apikey: str = None,
         traces_apikey: str = None,
         metrics_apikey: str = None,
+        logs_apikey: str = None,
         service_name: str = None,
         service_version: str = None,
         endpoint: str = None,
         traces_endpoint: str = None,
         metrics_endpoint: str = None,
+        logs_endpoint: str = None,
         endpoint_insecure: bool = False,
         traces_endpoint_insecure: bool = False,
         metrics_endpoint_insecure: bool = False,
+        logs_endpoint_insecure: bool = False,
         sample_rate: int = None,
         debug: bool = False,
         log_level: str = None,
         dataset: str = None,
         metrics_dataset: str = None,
         enable_local_visualizations: bool = False,
-        exporter_protocol: str = EXPORTER_PROTOCOL_GRPC,
+        exporter_protocol: str = EXPORTER_PROTOCOL_HTTP_PROTO,
         traces_exporter_protocol: str = None,
-        metrics_exporter_protocol: str = None
+        metrics_exporter_protocol: str = None,
+        logs_exporter_protocol: str = None,
     ):
-        self.debug = parse_bool(
-            DEBUG,
-            (debug or False),
-            INVALID_DEBUG_ERROR
-        )
+        self.debug = parse_bool(DEBUG, (debug or False), INVALID_DEBUG_ERROR)
         if self.debug:
             self.log_level = "DEBUG"
         else:
             log_level = os.environ.get(OTEL_LOG_LEVEL, log_level)
             if log_level and log_level.upper() in log_levels:
                 self.log_level = log_level.upper()
         logging.basicConfig(level=log_levels[self.log_level])
 
         self.traces_apikey = os.environ.get(
             HYPERDX_TRACES_APIKEY,
-            os.environ.get(
-                HYPERDX_API_KEY,
-                (traces_apikey or apikey)
-            )
+            os.environ.get(HYPERDX_API_KEY, (traces_apikey or apikey)),
         )
         if not self.traces_apikey:
             _logger.warning(MISSING_API_KEY_ERROR)
 
         self.metrics_apikey = os.environ.get(
             HYPERDX_METRICS_APIKEY,
-            os.environ.get(
-                HYPERDX_API_KEY,
-                (metrics_apikey or apikey)
-            )
+            os.environ.get(HYPERDX_API_KEY, (metrics_apikey or apikey)),
         )
         if not self.traces_apikey:
             _logger.warning(MISSING_API_KEY_ERROR)
 
+        self.logs_apikey = os.environ.get(
+            HYPERDX_LOGS_APIKEY,
+            os.environ.get(HYPERDX_API_KEY, (logs_apikey or apikey)),
+        )
+        if not self.logs_apikey:
+            _logger.warning(MISSING_API_KEY_ERROR)
+
         self.service_name = os.environ.get(OTEL_SERVICE_NAME, service_name)
         if not self.service_name:
             _logger.warning(MISSING_SERVICE_NAME_ERROR)
             self.service_name = DEFAULT_SERVICE_NAME
-        self.service_version = os.environ.get(
-            OTEL_SERVICE_VERSION, service_version)
+        self.service_version = os.environ.get(OTEL_SERVICE_VERSION, service_version)
 
         exporter_protocol = os.environ.get(
             OTEL_EXPORTER_OTLP_PROTOCOL,
-            (exporter_protocol or DEFAULT_EXPORTER_PROTOCOL))
+            (exporter_protocol or DEFAULT_EXPORTER_PROTOCOL),
+        )
         if exporter_protocol not in exporter_protocols:
             _logger.warning(INVALID_EXPORTER_PROTOCOL_ERROR)
             exporter_protocol = DEFAULT_EXPORTER_PROTOCOL
 
         self.traces_exporter_protocol = os.environ.get(
             OTEL_EXPORTER_OTLP_TRACES_PROTOCOL,
-            (traces_exporter_protocol or exporter_protocol))
+            (traces_exporter_protocol or exporter_protocol),
+        )
         if traces_exporter_protocol and (
-                traces_exporter_protocol not in exporter_protocols):
+            traces_exporter_protocol not in exporter_protocols
+        ):
             _logger.warning(INVALID_EXPORTER_PROTOCOL_ERROR)
             self.traces_exporter_protocol = exporter_protocol
 
         self.metrics_exporter_protocol = os.environ.get(
             OTEL_EXPORTER_OTLP_METRICS_PROTOCOL,
-            (metrics_exporter_protocol or exporter_protocol))
+            (metrics_exporter_protocol or exporter_protocol),
+        )
         if metrics_exporter_protocol and (
-                metrics_exporter_protocol not in exporter_protocols):
+            metrics_exporter_protocol not in exporter_protocols
+        ):
             _logger.warning(INVALID_EXPORTER_PROTOCOL_ERROR)
             self.metrics_exporter_protocol = exporter_protocol
 
-        self.endpoint = os.environ.get(
-            HYPERDX_API_ENDPOINT,
-            endpoint
-        )
+        self.logs_exporter_protocol = os.environ.get(
+            OTEL_EXPORTER_OTLP_LOGS_PROTOCOL,
+            (logs_exporter_protocol or exporter_protocol),
+        )
+        if logs_exporter_protocol and (
+            logs_exporter_protocol not in exporter_protocols
+        ):
+            _logger.warning(INVALID_EXPORTER_PROTOCOL_ERROR)
+            self.logs_exporter_protocol = exporter_protocol
+
+        self.endpoint = os.environ.get(HYPERDX_API_ENDPOINT, endpoint)
 
         if not self.endpoint:
             self.endpoint = DEFAULT_API_ENDPOINT
 
-        self.traces_endpoint = os.environ.get(
-            OTEL_EXPORTER_OTLP_TRACES_ENDPOINT,
-            None
-        )
+        self.traces_endpoint = os.environ.get(OTEL_EXPORTER_OTLP_TRACES_ENDPOINT, None)
         if not self.traces_endpoint:
             self.traces_endpoint = _append_traces_path(
                 self.traces_exporter_protocol,
-                os.environ.get(OTEL_EXPORTER_OTLP_ENDPOINT, None)
+                os.environ.get(OTEL_EXPORTER_OTLP_ENDPOINT, None),
             )
             if not self.traces_endpoint:
                 self.traces_endpoint = traces_endpoint
                 if not self.traces_endpoint:
                     self.traces_endpoint = _append_traces_path(
-                        self.traces_exporter_protocol,
-                        self.endpoint
+                        self.traces_exporter_protocol, self.endpoint
                     )
 
         # if http/protobuf protocol and using generic env or param
         # append /v1/metrics path
         self.metrics_endpoint = os.environ.get(
-            OTEL_EXPORTER_OTLP_METRICS_ENDPOINT,
-            None
+            OTEL_EXPORTER_OTLP_METRICS_ENDPOINT, None
         )
         if not self.metrics_endpoint:
             self.metrics_endpoint = _append_metrics_path(
                 self.metrics_exporter_protocol,
-                os.environ.get(OTEL_EXPORTER_OTLP_ENDPOINT, None)
+                os.environ.get(OTEL_EXPORTER_OTLP_ENDPOINT, None),
             )
             if not self.metrics_endpoint:
                 self.metrics_endpoint = metrics_endpoint
                 if not self.metrics_endpoint:
                     self.metrics_endpoint = _append_metrics_path(
-                        self.metrics_exporter_protocol,
-                        self.endpoint
+                        self.metrics_exporter_protocol, self.endpoint
+                    )
+
+        self.logs_endpoint = os.environ.get(OTEL_EXPORTER_OTLP_LOGS_ENDPOINT, None)
+        if not self.logs_endpoint:
+            self.logs_endpoint = _append_logs_path(
+                self.logs_exporter_protocol,
+                os.environ.get(OTEL_EXPORTER_OTLP_ENDPOINT, None),
+            )
+            if not self.logs_endpoint:
+                self.logs_endpoint = logs_endpoint
+                if not self.logs_endpoint:
+                    self.logs_endpoint = _append_logs_path(
+                        self.logs_exporter_protocol, self.endpoint
                     )
 
         self.sample_rate = parse_int(
-            SAMPLE_RATE,
-            sample_rate,
-            DEFAULT_SAMPLE_RATE,
-            INVALID_SAMPLE_RATE_ERROR
+            SAMPLE_RATE, sample_rate, DEFAULT_SAMPLE_RATE, INVALID_SAMPLE_RATE_ERROR
         )
 
         endpoint_insecure = parse_bool(
             OTEL_EXPORTER_OTLP_INSECURE,
             (endpoint_insecure or False),
-            INVALID_INSECURE_ERROR
+            INVALID_INSECURE_ERROR,
         )
         self.traces_endpoint_insecure = parse_bool(
             OTEL_EXPORTER_OTLP_TRACES_INSECURE,
             (traces_endpoint_insecure or endpoint_insecure),
-            INVALID_TRACES_INSECURE_ERROR
+            INVALID_TRACES_INSECURE_ERROR,
         )
         self.metrics_endpoint_insecure = parse_bool(
             OTEL_EXPORTER_OTLP_METRICS_INSECURE,
             (metrics_endpoint_insecure or endpoint_insecure),
-            INVALID_METRICS_INSECURE_ERROR
+            INVALID_METRICS_INSECURE_ERROR,
+        )
+        self.logs_endpoint_insecure = parse_bool(
+            OTEL_EXPORTER_OTLP_LOGS_INSECURE,
+            (logs_endpoint_insecure or endpoint_insecure),
+            INVALID_LOGS_INSECURE_ERROR,
         )
 
-        self.dataset = os.environ.get(
-            HYPERDX_DATASET, dataset)
+        self.dataset = os.environ.get(HYPERDX_DATASET, dataset)
         if self.dataset and not is_classic(self.traces_apikey):
             _logger.warning(IGNORED_DATASET_ERROR)
         if not self.dataset and is_classic(self.traces_apikey):
             _logger.warning(MISSING_DATASET_ERROR)
 
-        self.metrics_dataset = os.environ.get(
-            HYPERDX_METRICS_DATASET, metrics_dataset)
+        self.metrics_dataset = os.environ.get(HYPERDX_METRICS_DATASET, metrics_dataset)
 
         self.enable_local_visualizations = parse_bool(
             HYPERDX_ENABLE_LOCAL_VISUALIZATIONS,
             enable_local_visualizations,
-            INVALID_LOCAL_VIS_ERROR
+            INVALID_LOCAL_VIS_ERROR,
         )
 
     def get_traces_endpoint(self) -> str:
         """
         Returns the OTLP traces endpoint to send spans to.
         """
         return self.traces_endpoint
 
     def get_metrics_endpoint(self) -> str:
         """
         Returns the OTLP metrics endpoint to send metrics to.
         """
         return self.metrics_endpoint
 
+    def get_logs_endpoint(self) -> str:
+        """
+        Returns the OTLP logs endpoint to send logs to.
+        """
+        return self.logs_endpoint
+
     def get_trace_endpoint_credentials(self):
         """
         Get the grpc credentials to use when sending to the traces endpoint.
         """
         if self.traces_endpoint_insecure:
             return None
         return ssl_channel_credentials()
@@ -404,14 +463,22 @@
         """
         Get the grpc credentials to use when sending to the metrics endpoint.
         """
         if self.metrics_endpoint_insecure:
             return None
         return ssl_channel_credentials()
 
+    def get_logs_endpoint_credentials(self):
+        """
+        Get the grpc credentials to use when sending to the logs endpoint.
+        """
+        if self.logs_endpoint_insecure:
+            return None
+        return ssl_channel_credentials()
+
     def get_trace_headers(self):
         """
         Gets the headers to send traces telemetry.
         """
         headers = {
             "authorization": self.traces_apikey,
         }
@@ -419,13 +486,20 @@
             headers["x-hyperdx-dataset"] = self.dataset
         return headers
 
     def get_metrics_headers(self):
         """
         Gets the headers to send metrics telemetry.
         """
-        headers = {
-            "authorization": self.metrics_apikey
-        }
+        headers = {"authorization": self.metrics_apikey}
         if self.metrics_dataset:
             headers["x-hyperdx-dataset"] = self.metrics_dataset
         return headers
+
+    def get_logs_headers(self):
+        """
+        Gets the headers to send logs telemetry.
+        """
+        headers = {"authorization": self.logs_apikey}
+        if self.dataset and is_classic(self.logs_apikey):
+            headers["x-hyperdx-dataset"] = self.dataset
+        return headers
```

### Comparing `hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/resource.py` & `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/resource.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/sampler.py` & `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/sampler.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.1/src/hyperdx/opentelemetry/trace.py` & `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/trace.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.1/PKG-INFO` & `hyperdx_opentelemetry-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdx-opentelemetry
-Version: 0.0.1
+Version: 0.0.2
 Summary: HyperDX OpenTelemetry Distro for Python
 Author: HyperDX
 Author-email: support@hyperdx.io
 Requires-Python: >=3.7.2,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

