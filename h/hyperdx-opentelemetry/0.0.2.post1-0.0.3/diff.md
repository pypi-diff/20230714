# Comparing `tmp/hyperdx_opentelemetry-0.0.2.post1.tar.gz` & `tmp/hyperdx_opentelemetry-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdx_opentelemetry-0.0.2.post1.tar", max compression
+gzip compressed data, was "hyperdx_opentelemetry-0.0.3.tar", max compression
```

## Comparing `hyperdx_opentelemetry-0.0.2.post1.tar` & `hyperdx_opentelemetry-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-07-13 00:34:40.461547 hyperdx_opentelemetry-0.0.2.post1/LICENSE
--rw-r--r--   0        0        0     1184 2023-07-14 00:40:33.579362 hyperdx_opentelemetry-0.0.2.post1/README.md
--rw-r--r--   0        0        0      822 2023-07-14 02:28:25.436987 hyperdx_opentelemetry-0.0.2.post1/pyproject.toml
--rw-r--r--   0        0        0      122 2023-07-13 23:59:18.772014 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/__init__.py
--rw-r--r--   0        0        0     1373 2023-07-13 06:54:02.327463 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/baggage.py
--rw-r--r--   0        0        0     3072 2023-07-14 01:15:59.983930 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/distro.py
--rw-r--r--   0        0        0     1601 2023-07-14 00:22:56.721389 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/logs.py
--rw-r--r--   0        0        0     5405 2023-07-14 02:21:53.344267 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/manual.py
--rw-r--r--   0        0        0     1601 2023-07-13 06:39:14.131376 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/metrics.py
--rw-r--r--   0        0        0    18089 2023-07-14 01:13:04.588438 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/options.py
--rw-r--r--   0        0        0      826 2023-07-13 06:35:40.043017 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/resource.py
--rw-r--r--   0        0        0     3172 2023-07-13 06:34:37.078271 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/sampler.py
--rw-r--r--   0        0        0     1818 2023-07-13 06:33:47.851726 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/trace.py
--rw-r--r--   0        0        0       99 2023-07-13 01:54:38.990328 hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/version.py
--rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 hyperdx_opentelemetry-0.0.2.post1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-13 00:34:40.461547 hyperdx_opentelemetry-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1184 2023-07-14 00:40:33.579362 hyperdx_opentelemetry-0.0.3/README.md
+-rw-r--r--   0        0        0      820 2023-07-14 06:41:32.032971 hyperdx_opentelemetry-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-07-13 23:59:18.772014 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/__init__.py
+-rw-r--r--   0        0        0     1373 2023-07-13 06:54:02.327463 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/baggage.py
+-rw-r--r--   0        0        0     3072 2023-07-14 01:15:59.983930 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/distro.py
+-rw-r--r--   0        0        0     1601 2023-07-14 00:22:56.721389 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/logs.py
+-rw-r--r--   0        0        0     5499 2023-07-14 06:32:50.848960 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/manual.py
+-rw-r--r--   0        0        0     1601 2023-07-13 06:39:14.131376 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/metrics.py
+-rw-r--r--   0        0        0    18089 2023-07-14 01:13:04.588438 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/options.py
+-rw-r--r--   0        0        0      826 2023-07-13 06:35:40.043017 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/resource.py
+-rw-r--r--   0        0        0     3172 2023-07-13 06:34:37.078271 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/sampler.py
+-rw-r--r--   0        0        0     1818 2023-07-13 06:33:47.851726 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/trace.py
+-rw-r--r--   0        0        0       99 2023-07-13 01:54:38.990328 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/version.py
+-rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 hyperdx_opentelemetry-0.0.3/PKG-INFO
```

### Comparing `hyperdx_opentelemetry-0.0.2.post1/LICENSE` & `hyperdx_opentelemetry-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2.post1/README.md` & `hyperdx_opentelemetry-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2.post1/pyproject.toml` & `hyperdx_opentelemetry-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperdx-opentelemetry"
-version = "0.0.2-1"
+version = "0.0.3"
 description = "HyperDX OpenTelemetry Distro for Python"
 authors = ["HyperDX <support@hyperdx.io>"]
 readme = "README.md"
 packages = [{include = "hyperdx", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.7, >= 3.7.2"
```

### Comparing `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/baggage.py` & `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/baggage.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/distro.py` & `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/distro.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/logs.py` & `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/logs.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/manual.py` & `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/manual.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,39 +45,40 @@
             response_hook=response_hook,
             tracer_provider=tracer_provider,
         )
     except ImportError as e:
         pass
 
 
-# FIXME: capture headers + body
 def _instrument_urllib(
     options: HyperDXOptions,
     tracer_provider: TracerProvider,
     meter_provider: MeterProvider,
 ):
     try:
         from http import client
-        from opentelemetry.instrumentation.urllib import urllibinstrumentor
+        from opentelemetry.instrumentation.urllib import URLLibInstrumentor
         from urllib.request import Request
 
         def request_hook(span, request_obj: Request):
             for header in request_obj.header_items():
                 k, v = header
                 span.set_attribute("http.request.header.%s" % k.lower(), v)
             if request_obj.data:
                 span.set_attribute("http.request.body", decode_body(request_obj.data))
 
         def response_hook(span, request_obj, response: client.HTTPResponse):
-            for k, v in response.headers.items():
+            headers = dict(response.info())
+            for k, v in headers.items():
                 span.set_attribute("http.response.header.%s" % k.lower(), v)
-            # if response.text:
-            #     span.set_attribute("http.response.body", response.text)
+            body = response.read()
+            if body:
+                span.set_attribute("http.response.body", decode_body(body))
 
-        urllibinstrumentor().instrument(
+        URLLibInstrumentor().instrument(
             excluded_urls=",".join(options.get_all_endpoints()),
             meter_provider=meter_provider,
             request_hook=request_hook,
             response_hook=response_hook,
             tracer_provider=tracer_provider,
         )
     except ImportError as e:
@@ -147,10 +148,11 @@
 
 def instrument_custom_libs(
     options: HyperDXOptions,
     resource: Resource,
     tracer_provider: TracerProvider,
     meter_provider: MeterProvider,
 ):
+    _instrument_urllib(options, tracer_provider, meter_provider)
     _instrument_requests(options, tracer_provider, meter_provider)
     _instrument_flask(options, tracer_provider, meter_provider)
     _instrument_fastapi(options, tracer_provider, meter_provider)
```

### Comparing `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/metrics.py` & `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/metrics.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/options.py` & `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/options.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/resource.py` & `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/resource.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/sampler.py` & `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/sampler.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2.post1/src/hyperdx/opentelemetry/trace.py` & `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/trace.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.2.post1/PKG-INFO` & `hyperdx_opentelemetry-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdx-opentelemetry
-Version: 0.0.2.post1
+Version: 0.0.3
 Summary: HyperDX OpenTelemetry Distro for Python
 Author: HyperDX
 Author-email: support@hyperdx.io
 Requires-Python: >=3.7.2,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

