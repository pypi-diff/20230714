# Comparing `tmp/hyperdx_opentelemetry-0.0.2.tar.gz` & `tmp/hyperdx_opentelemetry-0.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdx_opentelemetry-0.0.2.tar", max compression
+gzip compressed data, was "hyperdx_opentelemetry-0.0.2.post1.tar", max compression
```

## Comparing `hyperdx_opentelemetry-0.0.2.tar` & `hyperdx_opentelemetry-0.0.2.post1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-07-13 00:34:40.461547 hyperdx_opentelemetry-0.0.2/LICENSE
--rw-r--r--   0        0        0     1580 2023-07-13 07:05:50.722511 hyperdx_opentelemetry-0.0.2/README.md
--rw-r--r--   0        0        0      820 2023-07-14 00:22:56.720578 hyperdx_opentelemetry-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      122 2023-07-13 23:59:18.772014 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/__init__.py
--rw-r--r--   0        0        0     1373 2023-07-13 06:54:02.327463 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/baggage.py
--rw-r--r--   0        0        0     3020 2023-07-14 00:22:56.721145 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/distro.py
--rw-r--r--   0        0        0     1601 2023-07-14 00:22:56.721389 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/logs.py
--rw-r--r--   0        0        0     3313 2023-07-14 00:22:56.721663 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/manual.py
--rw-r--r--   0        0        0     1601 2023-07-13 06:39:14.131376 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/metrics.py
--rw-r--r--   0        0        0    17854 2023-07-14 00:22:56.721984 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/options.py
--rw-r--r--   0        0        0      826 2023-07-13 06:35:40.043017 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/resource.py
--rw-r--r--   0        0        0     3172 2023-07-13 06:34:37.078271 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/sampler.py
--rw-r--r--   0        0        0     1818 2023-07-13 06:33:47.851726 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/trace.py
--rw-r--r--   0        0        0       99 2023-07-13 01:54:38.990328 hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/version.py
--rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 hyperdx_opentelemetry-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-13 00:34:40.461547 hyperdx_opentelemetry-0.0.2.post1/LICENSE
+-rw-r--r--   0        0        0     1184 2023-07-14 00:40:33.579362 hyperdx_opentelemetry-0.0.2.post1/README.md
+-rw-r--r--   0        0        0      822 2023-07-14 02:28:25.436987 hyperdx_opentelemetry-0.0.2.post1/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-07-13 23:59:18.772014 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/__init__.py
+-rw-r--r--   0        0        0     1373 2023-07-13 06:54:02.327463 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/baggage.py
+-rw-r--r--   0        0        0     3072 2023-07-14 01:15:59.983930 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/distro.py
+-rw-r--r--   0        0        0     1601 2023-07-14 00:22:56.721389 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/logs.py
+-rw-r--r--   0        0        0     5405 2023-07-14 02:21:53.344267 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/manual.py
+-rw-r--r--   0        0        0     1601 2023-07-13 06:39:14.131376 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/metrics.py
+-rw-r--r--   0        0        0    18089 2023-07-14 01:13:04.588438 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/options.py
+-rw-r--r--   0        0        0      826 2023-07-13 06:35:40.043017 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/resource.py
+-rw-r--r--   0        0        0     3172 2023-07-13 06:34:37.078271 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/sampler.py
+-rw-r--r--   0        0        0     1818 2023-07-13 06:33:47.851726 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/trace.py
+-rw-r--r--   0        0        0       99 2023-07-13 01:54:38.990328 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/version.py
+-rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 hyperdx_opentelemetry-0.0.2.post1/PKG-INFO
```

### Comparing `hyperdx_opentelemetry-0.0.2/LICENSE` & `hyperdx_opentelemetry-0.0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2/README.md` & `hyperdx_opentelemetry-0.0.2.post1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,32 +8,22 @@
 You're welcome to try it, and let us know your feedback in the issues!
 
 This is HyperDX's Distribution of OpenTelemetry for Python.
 It makes getting started with OpenTelemetry and HyperDX easier!
 
 Latest release built with:
 
-- [OpenTelemetry version 1.17.0/0.38b0](https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.17.0)
+- [OpenTelemetry version 1.18.0/0.39b0](https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.18.0)
 
 ## Requirements
 
 - Python 3.7 or higher
 
 ## Getting Started
 
 HyperDX's Distribution of OpenTelemetry for Python allows you to streamline configuration and to instrument as quickly and easily as possible.
 
-- [Documentation](https://docs.hyperdx.io/getting-data-in/opentelemetry/python/)
-- [Examples](/examples/)
-- See [DEVELOPING.md](/DEVELOPING.md) for additional instructions for building and testing this project in development.
-
-## Why would I want to use this?
-
-- Streamlined configuration for sending data to HyperDX!
-- Easy interop with existing instrumentation with OpenTelemetry!
-- Deterministic sampling!
-- Multi-span attributes!
-- Local visualizations!
+- [Documentation](https://www.hyperdx.io/docs/install/python)
 
 ## License
 
 [Apache 2.0 License](./LICENSE).
```

### Comparing `hyperdx_opentelemetry-0.0.2/pyproject.toml` & `hyperdx_opentelemetry-0.0.2.post1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperdx-opentelemetry"
-version = "0.0.2"
+version = "0.0.2-1"
 description = "HyperDX OpenTelemetry Distro for Python"
 authors = ["HyperDX <support@hyperdx.io>"]
 readme = "README.md"
 packages = [{include = "hyperdx", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.7, >= 3.7.2"
```

### Comparing `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/baggage.py` & `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/baggage.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/distro.py` & `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/distro.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,20 +53,21 @@
         options = HyperDXOptions()
     _logger.info("Configuring OpenTelemetry using HyperDX distro")
     _logger.debug(vars(options))
     resource = create_resource(options)
     configure_custom_env_vars(options, resource)
 
     tracer_provider = create_tracer_provider(options, resource)
+    meter_provider = create_meter_provider(options, resource)
     set_tracer_provider(tracer_provider)
     set_logging_handler(options)
     if options.metrics_dataset:
-        set_meter_provider(create_meter_provider(options, resource))
+        set_meter_provider(meter_provider)
 
-    instrument_custom_libs(options, resource, tracer_provider)
+    instrument_custom_libs(options, resource, tracer_provider, meter_provider)
 
 
 # pylint: disable=too-few-public-methods
 class HyperDXDistro(BaseDistro):
     """
     An extension of the base python OpenTelemetry distro, which provides
     a mechanism to automatically configure some of the more common options
```

### Comparing `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/logs.py` & `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/logs.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/metrics.py` & `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/metrics.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/options.py` & `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,7 +499,17 @@
         """
         Gets the headers to send logs telemetry.
         """
         headers = {"authorization": self.logs_apikey}
         if self.dataset and is_classic(self.logs_apikey):
             headers["x-hyperdx-dataset"] = self.dataset
         return headers
+
+    def get_all_endpoints(self):
+        """
+        Returns all endpoints.
+        """
+        return [
+            self.get_traces_endpoint(),
+            self.get_metrics_endpoint(),
+            self.get_logs_endpoint(),
+        ]
```

### Comparing `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/resource.py` & `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/resource.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/sampler.py` & `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/sampler.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2/src/hyperdx/opentelemetry/trace.py` & `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/trace.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2/PKG-INFO` & `hyperdx_opentelemetry-0.0.2.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdx-opentelemetry
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: HyperDX OpenTelemetry Distro for Python
 Author: HyperDX
 Author-email: support@hyperdx.io
 Requires-Python: >=3.7.2,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -26,33 +26,23 @@
 You're welcome to try it, and let us know your feedback in the issues!
 
 This is HyperDX's Distribution of OpenTelemetry for Python.
 It makes getting started with OpenTelemetry and HyperDX easier!
 
 Latest release built with:
 
-- [OpenTelemetry version 1.17.0/0.38b0](https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.17.0)
+- [OpenTelemetry version 1.18.0/0.39b0](https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.18.0)
 
 ## Requirements
 
 - Python 3.7 or higher
 
 ## Getting Started
 
 HyperDX's Distribution of OpenTelemetry for Python allows you to streamline configuration and to instrument as quickly and easily as possible.
 
-- [Documentation](https://docs.hyperdx.io/getting-data-in/opentelemetry/python/)
-- [Examples](/examples/)
-- See [DEVELOPING.md](/DEVELOPING.md) for additional instructions for building and testing this project in development.
-
-## Why would I want to use this?
-
-- Streamlined configuration for sending data to HyperDX!
-- Easy interop with existing instrumentation with OpenTelemetry!
-- Deterministic sampling!
-- Multi-span attributes!
-- Local visualizations!
+- [Documentation](https://www.hyperdx.io/docs/install/python)
 
 ## License
 
 [Apache 2.0 License](./LICENSE).
```

