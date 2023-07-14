# Comparing `tmp/firetail-1.0.8.tar.gz` & `tmp/firetail-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firetail-1.0.8.tar", last modified: Mon Nov 28 15:57:34 2022, max compression
+gzip compressed data, was "firetail-1.0.9.tar", last modified: Fri Jul 14 15:05:43 2023, max compression
```

## Comparing `firetail-1.0.8.tar` & `firetail-1.0.9.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.304653 firetail-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2022-11-28 15:57:27.000000 firetail-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-11-28 15:57:27.000000 firetail-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25990 2022-11-28 15:57:34.304653 firetail-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25592 2022-11-28 15:57:27.000000 firetail-1.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.296652 firetail-1.0.8/firetail/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1779 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.296652 firetail-1.0.8/firetail/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/apis/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/apis/aiohttp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13906 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/apis/flask_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/apis/flask_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.296652 firetail-1.0.8/firetail/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/apps/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/apps/aiohttp_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/apps/flask_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/auditor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.300653 firetail-1.0.8/firetail/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/decorators/coroutine_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/decorators/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/decorators/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/decorators/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/decorators/produces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/decorators/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12340 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/decorators/uri_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15976 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/decorators/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/flusher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/http_facts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/jsonifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.300653 firetail-1.0.8/firetail/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/middleware/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/middleware/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/middleware/swagger_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.300653 firetail-1.0.8/firetail/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15904 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/operations/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/operations/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    15683 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/operations/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/operations/secure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/operations/swagger2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.288652 firetail-1.0.8/firetail/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.292652 firetail-1.0.8/firetail/resources/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.300653 firetail-1.0.8/firetail/resources/schemas/v2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    40020 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/resources/schemas/v2.0/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.300653 firetail-1.0.8/firetail/resources/schemas/v3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35456 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/resources/schemas/v3.0/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.304653 firetail-1.0.8/firetail/security/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/security/aiohttp_security_handler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/security/async_security_handler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/security/flask_security_handler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15850 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/security/security_handler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     9523 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2022-11-28 15:57:27.000000 firetail-1.0.8/firetail/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:57:34.296652 firetail-1.0.8/firetail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25990 2022-11-28 15:57:34.000000 firetail-1.0.8/firetail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2022-11-28 15:57:34.000000 firetail-1.0.8/firetail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-28 15:57:34.000000 firetail-1.0.8/firetail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-11-28 15:57:34.000000 firetail-1.0.8/firetail.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      520 2022-11-28 15:57:34.000000 firetail-1.0.8/firetail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-11-28 15:57:34.000000 firetail-1.0.8/firetail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-11-28 15:57:34.304653 firetail-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2022-11-28 15:57:27.000000 firetail-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.408339 firetail-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-07-14 15:05:37.000000 firetail-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 15:05:37.000000 firetail-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-07-14 15:05:43.408339 firetail-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25592 2023-07-14 15:05:37.000000 firetail-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 15:05:37.000000 firetail-1.0.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.404339 firetail-1.0.9/firetail/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1800 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.404339 firetail-1.0.9/firetail/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18733 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/apis/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15379 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/apis/aiohttp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/apis/flask_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/apis/flask_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.408339 firetail-1.0.9/firetail/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/apps/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/apps/aiohttp_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/apps/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/auditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.408339 firetail-1.0.9/firetail/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/decorators/coroutine_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/decorators/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/decorators/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/decorators/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/decorators/produces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/decorators/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/decorators/uri_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/decorators/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/flusher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/http_facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/jsonifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.408339 firetail-1.0.9/firetail/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/middleware/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/middleware/swagger_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.408339 firetail-1.0.9/firetail/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/operations/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/operations/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/operations/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/operations/secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/operations/swagger2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.400339 firetail-1.0.9/firetail/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.400339 firetail-1.0.9/firetail/resources/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.408339 firetail-1.0.9/firetail/resources/schemas/v2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    40020 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/resources/schemas/v2.0/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.408339 firetail-1.0.9/firetail/resources/schemas/v3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35456 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/resources/schemas/v3.0/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.408339 firetail-1.0.9/firetail/security/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/security/aiohttp_security_handler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/security/async_security_handler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/security/flask_security_handler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/security/security_handler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-14 15:05:37.000000 firetail-1.0.9/firetail/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:05:43.404339 firetail-1.0.9/firetail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-07-14 15:05:43.000000 firetail-1.0.9/firetail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-14 15:05:43.000000 firetail-1.0.9/firetail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:05:43.000000 firetail-1.0.9/firetail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 15:05:43.000000 firetail-1.0.9/firetail.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-14 15:05:43.000000 firetail-1.0.9/firetail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 15:05:43.000000 firetail-1.0.9/firetail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-14 15:05:37.000000 firetail-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 15:05:43.408339 firetail-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-14 15:05:37.000000 firetail-1.0.9/setup.py
```

### Comparing `firetail-1.0.8/LICENSE.txt` & `firetail-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `firetail-1.0.8/PKG-INFO` & `firetail-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firetail
-Version: 1.0.8
+Version: 1.0.9
 Summary: Firetail - API first applications with OpenAPI/Swagger and Flask
 Home-page: https://github.com/FireTail-io/firetail-py-lib
 Author: FireTail International (TM)
 License: LGPLv3
 Keywords: openapi oai swagger rest api oauth flask microservice framework
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `firetail-1.0.8/README.rst` & `firetail-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `firetail-1.0.8/firetail/__init__.py` & `firetail-1.0.9/firetail/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # add operation for backwards compatibility
 from .operations import compat
 from .problem import problem  # NOQA
 from .resolver import Resolution, Resolver, RestyResolver  # NOQA
 from .utils import not_installed_error  # NOQA
 
-full_name = f'{__package__}.operation'
+full_name = f"{__package__}.operation"
 sys.modules[full_name] = sys.modules[compat.__name__]
 
 
 try:
     from flask import request  # NOQA
 
     from .apis.flask_api import FlaskApi, context  # NOQA
@@ -44,8 +44,10 @@
     from .apps.aiohttp_app import AioHttpApp
 except ImportError as e:  # pragma: no cover
     _aiohttp_not_installed_error = not_installed_error(e)
     AioHttpApi = _aiohttp_not_installed_error
     AioHttpApp = _aiohttp_not_installed_error
 
 # This version is replaced during release process.
-__version__ = 'v1.0.8'
+# fmt: off
+__version__ = 'v1.0.9'
+# fmt: on
```

### Comparing `firetail-1.0.8/firetail/apis/__init__.py` & `firetail-1.0.9/firetail/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `firetail-1.0.8/firetail/apis/abstract.py` & `firetail-1.0.9/firetail/apis/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,36 +18,46 @@
 from ..operations import make_operation
 from ..options import FiretailOptions
 from ..resolver import Resolver
 from ..spec import Specification
 from ..utils import is_json_mimetype
 
 MODULE_PATH = pathlib.Path(__file__).absolute().parent.parent
-SWAGGER_UI_URL = 'ui'
+SWAGGER_UI_URL = "ui"
 
-logger = logging.getLogger('firetail.apis.abstract')
+logger = logging.getLogger("firetail.apis.abstract")
 
 
 class AbstractAPIMeta(abc.ABCMeta):
-
     def __init__(cls, name, bases, attrs):
         abc.ABCMeta.__init__(cls, name, bases, attrs)
         cls._set_jsonifier()
 
 
 class AbstractAPI(metaclass=AbstractAPIMeta):
     """
     Defines an abstract interface for a Swagger API
     """
 
-    def __init__(self, specification, base_path=None, arguments=None,
-                 validate_responses=False, strict_validation=False, resolver=None,
-                 auth_all_paths=False, debug=False, resolver_error_handler=None,
-                 validator_map=None, pythonic_params=False, pass_context_arg_name=None, options=None,
-                 ):
+    def __init__(
+        self,
+        specification,
+        base_path=None,
+        arguments=None,
+        validate_responses=False,
+        strict_validation=False,
+        resolver=None,
+        auth_all_paths=False,
+        debug=False,
+        resolver_error_handler=None,
+        validator_map=None,
+        pythonic_params=False,
+        pass_context_arg_name=None,
+        options=None,
+    ):
         """
         :type specification: pathlib.Path | dict
         :type base_path: str | None
         :type arguments: dict | None
         :type validate_responses: bool
         :type strict_validation: bool
         :type auth_all_paths: bool
@@ -67,66 +77,72 @@
             will be passed the framework's request context.
         :type pass_context_arg_name: str | None
         """
         self.debug = debug
         self.validator_map = validator_map
         self.resolver_error_handler = resolver_error_handler
 
-        logger.debug('Loading specification: %s', specification,
-                     extra={'swagger_yaml': specification,
-                            'base_path': base_path,
-                            'arguments': arguments,
-                            'auth_all_paths': auth_all_paths})
+        logger.debug(
+            "Loading specification: %s",
+            specification,
+            extra={
+                "swagger_yaml": specification,
+                "base_path": base_path,
+                "arguments": arguments,
+                "auth_all_paths": auth_all_paths,
+            },
+        )
 
         # Avoid validator having ability to modify specification
         self.specification = Specification.load(specification, arguments=arguments)
 
-        logger.debug('Read specification', extra={'spec': self.specification})
+        logger.debug("Read specification", extra={"spec": self.specification})
 
         self.options = FiretailOptions(options, oas_version=self.specification.version)
 
-        logger.debug('Options Loaded',
-                     extra={'swagger_ui': self.options.openapi_console_ui_available,
-                            'swagger_path': self.options.openapi_console_ui_from_dir,
-                            'swagger_url': self.options.openapi_console_ui_path})
+        logger.debug(
+            "Options Loaded",
+            extra={
+                "swagger_ui": self.options.openapi_console_ui_available,
+                "swagger_path": self.options.openapi_console_ui_from_dir,
+                "swagger_url": self.options.openapi_console_ui_path,
+            },
+        )
 
         self._set_base_path(base_path)
 
-        logger.debug('Security Definitions: %s', self.specification.security_definitions)
+        logger.debug("Security Definitions: %s", self.specification.security_definitions)
 
         self.resolver = resolver or Resolver()
 
-        logger.debug('Validate Responses: %s', str(validate_responses))
+        logger.debug("Validate Responses: %s", str(validate_responses))
         self.validate_responses = validate_responses
 
-        logger.debug('Strict Request Validation: %s', str(strict_validation))
+        logger.debug("Strict Request Validation: %s", str(strict_validation))
         self.strict_validation = strict_validation
 
-        logger.debug('Pythonic params: %s', str(pythonic_params))
+        logger.debug("Pythonic params: %s", str(pythonic_params))
         self.pythonic_params = pythonic_params
 
-        logger.debug('pass_context_arg_name: %s', pass_context_arg_name)
+        logger.debug("pass_context_arg_name: %s", pass_context_arg_name)
         self.pass_context_arg_name = pass_context_arg_name
 
         self.security_handler_factory = self.make_security_handler_factory(pass_context_arg_name)
 
         if self.options.openapi_spec_available:
             self.add_openapi_json()
             self.add_openapi_yaml()
 
         if self.options.openapi_console_ui_available:
             self.add_swagger_ui()
 
         self.add_paths()
 
         if auth_all_paths:
-            self.add_auth_on_not_found(
-                self.specification.security,
-                self.specification.security_definitions
-            )
+            self.add_auth_on_not_found(self.specification.security, self.specification.security_definitions)
 
     def _set_base_path(self, base_path=None):
         if base_path is not None:
             # update spec to include user-provided base_path
             self.specification.base_path = base_path
             self.base_path = base_path
         else:
@@ -150,15 +166,15 @@
         """
         Adds a 404 error handler to authenticate and only expose the 404 status if the security validation pass.
         """
 
     @staticmethod
     @abc.abstractmethod
     def make_security_handler_factory(pass_context_arg_name):
-        """ Create SecurityHandlerFactory to create all security check handlers """
+        """Create SecurityHandlerFactory to create all security check handlers"""
 
     def add_operation(self, path, method):
         """
         Adds one operation to the api.
 
         This method uses the OperationID identify the module and function that will handle the operation
 
@@ -179,15 +195,15 @@
             method,
             self.resolver,
             validate_responses=self.validate_responses,
             validator_map=self.validator_map,
             strict_validation=self.strict_validation,
             pythonic_params=self.pythonic_params,
             uri_parser_class=self.options.uri_parser_class,
-            pass_context_arg_name=self.pass_context_arg_name
+            pass_context_arg_name=self.pass_context_arg_name,
         )
         self._add_operation_internal(method, path, operation)
 
     @abc.abstractmethod
     def _add_operation_internal(self, method, path, operation):
         """
         Adds the operation according to the user framework in use.
@@ -195,29 +211,27 @@
         """
 
     def _add_resolver_error_handler(self, method, path, err):
         """
         Adds a handler for ResolverError for the given method and path.
         """
         operation = self.resolver_error_handler(
-            err,
-            security=self.specification.security,
-            security_definitions=self.specification.security_definitions
+            err, security=self.specification.security, security_definitions=self.specification.security_definitions
         )
         self._add_operation_internal(method, path, operation)
 
     def add_paths(self, paths=None):
         """
         Adds the paths defined in the specification as endpoints
 
         :type paths: list
         """
-        paths = paths or self.specification.get('paths', dict())
+        paths = paths or self.specification.get("paths", dict())
         for path, methods in paths.items():
-            logger.debug('Adding %s%s...', self.base_path, path)
+            logger.debug("Adding %s%s...", self.base_path, path)
 
             for method in methods:
                 if method not in METHODS:
                     continue
                 try:
                     self.add_operation(path, method)
                 except ResolverError as err:
@@ -228,18 +242,16 @@
                     else:
                         self._handle_add_operation_error(path, method, err.exc_info)
                 except Exception:
                     # All other relevant exceptions should be handled as well.
                     self._handle_add_operation_error(path, method, sys.exc_info())
 
     def _handle_add_operation_error(self, path, method, exc_info):
-        url = f'{self.base_path}{path}'
-        error_msg = 'Failed to add operation for {method} {url}'.format(
-            method=method.upper(),
-            url=url)
+        url = f"{self.base_path}{path}"
+        error_msg = "Failed to add operation for {method} {url}".format(method=method.upper(), url=url)
         if self.debug:
             logger.exception(error_msg)
         else:
             logger.error(error_msg)
             _type, value, traceback = exc_info
             raise value.with_traceback(traceback)
 
@@ -273,40 +285,35 @@
         :param mimetype: The response mimetype.
         :type mimetype: Union[None, str]
         :param extra_context: dict of extra details, like url, to include in logs
         :type extra_context: Union[None, dict]
         """
         if extra_context is None:
             extra_context = {}
-        logger.debug('Getting data and status code',
-                     extra={
-                         'data': response,
-                         'data_type': type(response),
-                         **extra_context
-                     })
+        logger.debug(
+            "Getting data and status code", extra={"data": response, "data_type": type(response), **extra_context}
+        )
 
         if isinstance(response, FiretailResponse):
             framework_response = cls._firetail_to_framework_response(response, mimetype, extra_context)
         else:
             framework_response = cls._response_from_handler(response, mimetype, extra_context)
 
-        logger.debug('Got framework response',
-                     extra={
-                         'response': framework_response,
-                         'response_type': type(framework_response),
-                         **extra_context
-                     })
+        logger.debug(
+            "Got framework response",
+            extra={"response": framework_response, "response_type": type(framework_response), **extra_context},
+        )
         return framework_response
 
     @classmethod
     def _response_from_handler(
-            cls,
-            response: t.Union[t.Any, str, t.Tuple[str], t.Tuple[str, int], t.Tuple[str, int, dict]],
-            mimetype: str,
-            extra_context: t.Optional[dict] = None
+        cls,
+        response: t.Union[t.Any, str, t.Tuple[str], t.Tuple[str, int], t.Tuple[str, int, dict]],
+        mimetype: str,
+        extra_context: t.Optional[dict] = None,
     ) -> t.Any:
         """
         Create a framework response from the operation handler data.
         An operation handler can return:
         - a framework response
         - a body (str / binary / dict / list), a response will be created
         with a status code 200 by default and empty headers.
@@ -319,74 +326,74 @@
         """
         if cls._is_framework_response(response):
             return response
 
         if isinstance(response, tuple):
             len_response = len(response)
             if len_response == 1:
-                data, = response
+                (data,) = response
                 return cls._build_response(mimetype=mimetype, data=data, extra_context=extra_context)
             if len_response == 2:
                 if isinstance(response[1], (int, Enum)):
                     data, status_code = response
-                    return cls._build_response(mimetype=mimetype, data=data, status_code=status_code, extra_context=extra_context)
+                    return cls._build_response(
+                        mimetype=mimetype, data=data, status_code=status_code, extra_context=extra_context
+                    )
                 else:
                     data, headers = response
                 return cls._build_response(mimetype=mimetype, data=data, headers=headers, extra_context=extra_context)
             elif len_response == 3:
                 data, status_code, headers = response
-                return cls._build_response(mimetype=mimetype,
-                                           data=data,
-                                           status_code=status_code,
-                                           headers=headers,
-                                           extra_context=extra_context)
+                return cls._build_response(
+                    mimetype=mimetype, data=data, status_code=status_code, headers=headers, extra_context=extra_context
+                )
             else:
                 raise TypeError(
-                    'The view function did not return a valid response tuple.'
-                    ' The tuple must have the form (body), (body, status, headers),'
-                    ' (body, status), or (body, headers).'
+                    "The view function did not return a valid response tuple."
+                    " The tuple must have the form (body), (body, status, headers),"
+                    " (body, status), or (body, headers)."
                 )
         else:
             return cls._build_response(mimetype=mimetype, data=response, extra_context=extra_context)
 
     @classmethod
     def get_firetail_response(cls, response, mimetype=None):
-        """ Cast framework dependent response to FiretailResponse used for schema validation """
+        """Cast framework dependent response to FiretailResponse used for schema validation"""
         if isinstance(response, FiretailResponse):
             # If body in FiretailResponse is not byte, it may not pass schema validation.
             # In this case, rebuild response with aiohttp to have consistency
             if response.body is None or isinstance(response.body, bytes):
                 return response
             else:
                 response = cls._build_response(
                     data=response.body,
                     mimetype=mimetype,
                     content_type=response.content_type,
                     headers=response.headers,
-                    status_code=response.status_code
+                    status_code=response.status_code,
                 )
 
         if not cls._is_framework_response(response):
             response = cls._response_from_handler(response, mimetype)
         return cls._framework_to_firetail_response(response=response, mimetype=mimetype)
 
     @classmethod
     @abc.abstractmethod
     def _is_framework_response(cls, response):
-        """ Return True if `response` is a framework response class """
+        """Return True if `response` is a framework response class"""
 
     @classmethod
     @abc.abstractmethod
     def _framework_to_firetail_response(cls, response, mimetype):
-        """ Cast framework response class to FiretailResponse used for schema validation """
+        """Cast framework response class to FiretailResponse used for schema validation"""
 
     @classmethod
     @abc.abstractmethod
     def _firetail_to_framework_response(cls, response, mimetype, extra_context=None):
-        """ Cast FiretailResponse to framework response class """
+        """Cast FiretailResponse to framework response class"""
 
     @classmethod
     @abc.abstractmethod
     def _build_response(cls, data, mimetype, content_type=None, status_code=None, headers=None, extra_context=None):
         """
         Create a framework response from the provided arguments.
         :param data: Body data.
@@ -420,20 +427,15 @@
         if data is not None:
             body, mimetype = cls._serialize_data(data, mimetype)
         else:
             body = data
 
         if extra_context is None:
             extra_context = {}
-        logger.debug('Prepared body and status code (%d)',
-                     status_code,
-                     extra={
-                         'body': body,
-                         **extra_context
-                     })
+        logger.debug("Prepared body and status code (%d)", status_code, extra={"body": body, **extra_context})
 
         return body, status_code, mimetype
 
     @classmethod
     def _serialize_data(cls, data, mimetype):
         # TODO: Harmonize with flask_api. Currently this is the backwards compatible with aiohttp_api._cast_body.
         if not isinstance(data, bytes):
@@ -445,15 +447,15 @@
                 warnings.warn(
                     "Implicit (aiohttp) serialization with str() will change in the next major version. "
                     "This is triggered because a non-JSON response body is being stringified. "
                     "This will be replaced by something that is mimetype-specific and may "
                     "serialize some things as JSON or throw an error instead of silently "
                     "stringifying unknown response bodies. "
                     "Please make sure to specify media/mime types in your specs.",
-                    FutureWarning  # a Deprecation targeted at application users.
+                    FutureWarning,  # a Deprecation targeted at application users.
                 )
                 body = str(data)
         else:
             body = data
         return body, mimetype
 
     def json_loads(self, data):
```

### Comparing `firetail-1.0.8/firetail/apis/aiohttp_api.py` & `firetail-1.0.9/firetail/apis/aiohttp_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from firetail.handlers import AuthErrorHandler
 from firetail.jsonifier import JSONEncoder, Jsonifier
 from firetail.lifecycle import FiretailRequest, FiretailResponse
 from firetail.problem import problem
 from firetail.security import AioHttpSecurityHandlerFactory
 from firetail.utils import yamldumper
 
-logger = logging.getLogger('firetail.apis.aiohttp_api')
+logger = logging.getLogger("firetail.apis.aiohttp_api")
 
 
 def _generic_problem(http_status: HTTPStatus, exc: Exception = None):
     extra = None
     if exc is not None:
         loop = asyncio.get_event_loop()
         if loop.get_debug():
@@ -50,16 +50,23 @@
 
 
 @web.middleware
 async def problems_middleware(request, handler):
     try:
         response = await handler(request)
     except ProblemException as exc:
-        response = problem(status=exc.status, detail=exc.detail, title=exc.title,
-                           type=exc.type, instance=exc.instance, headers=exc.headers, ext=exc.ext)
+        response = problem(
+            status=exc.status,
+            detail=exc.detail,
+            title=exc.title,
+            type=exc.type,
+            instance=exc.instance,
+            headers=exc.headers,
+            ext=exc.ext,
+        )
     except (werkzeug_HTTPException, _HttpNotFoundError) as exc:
         response = problem(status=exc.code, title=exc.name, detail=exc.description)
     except web.HTTPError as exc:
         if exc.text == f"{exc.status}: {exc.reason}":
             detail = HTTPStatus(exc.status).description
         else:
             detail = exc.text
@@ -68,65 +75,52 @@
         web.HTTPException,  # eg raised HTTPRedirection or HTTPSuccessful
         asyncio.CancelledError,  # skipped in default web_protocol
     ):
         # leave this to default handling in aiohttp.web_protocol.RequestHandler.start()
         raise
     except asyncio.TimeoutError as exc:
         # overrides 504 from aiohttp.web_protocol.RequestHandler.start()
-        logger.debug('Request handler timed out.', exc_info=exc)
+        logger.debug("Request handler timed out.", exc_info=exc)
         response = _generic_problem(HTTPStatus.GATEWAY_TIMEOUT, exc)
     except Exception as exc:
         # overrides 500 from aiohttp.web_protocol.RequestHandler.start()
-        logger.exception('Error handling request', exc_info=exc)
+        logger.exception("Error handling request", exc_info=exc)
         response = _generic_problem(HTTPStatus.INTERNAL_SERVER_ERROR, exc)
 
     if isinstance(response, FiretailResponse):
         response = await AioHttpApi.get_response(response)
     return response
 
 
 class AioHttpApi(AbstractAPI):
     def __init__(self, *args, **kwargs):
         # NOTE we use HTTPPermanentRedirect (308) because
         # clients sometimes turn POST requests into GET requests
         # on 301, 302, or 303
         # see https://tools.ietf.org/html/rfc7538
-        trailing_slash_redirect = normalize_path_middleware(
-            append_slash=True,
-            redirect_class=HTTPPermanentRedirect
-        )
-        self.subapp = web.Application(
-            middlewares=[
-                problems_middleware,
-                trailing_slash_redirect
-            ]
-        )
+        trailing_slash_redirect = normalize_path_middleware(append_slash=True, redirect_class=HTTPPermanentRedirect)
+        self.subapp = web.Application(middlewares=[problems_middleware, trailing_slash_redirect])
         AbstractAPI.__init__(self, *args, **kwargs)
 
-        aiohttp_jinja2.setup(
-            self.subapp,
-            loader=jinja2.FileSystemLoader(
-                str(self.options.openapi_console_ui_from_dir)
-            )
-        )
-        middlewares = self.options.as_dict().get('middlewares', [])
+        aiohttp_jinja2.setup(self.subapp, loader=jinja2.FileSystemLoader(str(self.options.openapi_console_ui_from_dir)))
+        middlewares = self.options.as_dict().get("middlewares", [])
         self.subapp.middlewares.extend(middlewares)
 
     @staticmethod
     def make_security_handler_factory(pass_context_arg_name):
-        """ Create default SecurityHandlerFactory to create all security check handlers """
+        """Create default SecurityHandlerFactory to create all security check handlers"""
         return AioHttpSecurityHandlerFactory(pass_context_arg_name)
 
     def _set_base_path(self, base_path):
         AbstractAPI._set_base_path(self, base_path)
         self._api_name = AioHttpApi.normalize_string(self.base_path)
 
     @staticmethod
     def normalize_string(string):
-        return re.sub(r'[^a-zA-Z0-9]', '_', string.strip('/'))
+        return re.sub(r"[^a-zA-Z0-9]", "_", string.strip("/"))
 
     def _base_path_for_prefix(self, request):
         """
         returns a modified basePath which includes the incoming request's
         path prefix.
         """
         base_path = self.base_path
@@ -145,181 +139,130 @@
         return self.specification.with_base_path(base_path).raw
 
     def add_openapi_json(self):
         """
         Adds openapi json to {base_path}/openapi.json
              (or {base_path}/swagger.json for swagger2)
         """
-        logger.debug('Adding spec json: %s/%s', self.base_path,
-                     self.options.openapi_spec_path)
-        self.subapp.router.add_route(
-            'GET',
-            self.options.openapi_spec_path,
-            self._get_openapi_json
-        )
+        logger.debug("Adding spec json: %s/%s", self.base_path, self.options.openapi_spec_path)
+        self.subapp.router.add_route("GET", self.options.openapi_spec_path, self._get_openapi_json)
 
     def add_openapi_yaml(self):
         """
         Adds openapi json to {base_path}/openapi.json
              (or {base_path}/swagger.json for swagger2)
         """
         if not self.options.openapi_spec_path.endswith("json"):
             return
 
-        openapi_spec_path_yaml = \
-            self.options.openapi_spec_path[:-len("json")] + "yaml"
-        logger.debug('Adding spec yaml: %s/%s', self.base_path,
-                     openapi_spec_path_yaml)
-        self.subapp.router.add_route(
-            'GET',
-            openapi_spec_path_yaml,
-            self._get_openapi_yaml
-        )
+        openapi_spec_path_yaml = self.options.openapi_spec_path[: -len("json")] + "yaml"
+        logger.debug("Adding spec yaml: %s/%s", self.base_path, openapi_spec_path_yaml)
+        self.subapp.router.add_route("GET", openapi_spec_path_yaml, self._get_openapi_yaml)
 
     async def _get_openapi_json(self, request):
         return web.Response(
-            status=200,
-            content_type='application/json',
-            body=self.jsonifier.dumps(self._spec_for_prefix(request))
+            status=200, content_type="application/json", body=self.jsonifier.dumps(self._spec_for_prefix(request))
         )
 
     async def _get_openapi_yaml(self, request):
-        return web.Response(
-            status=200,
-            content_type='text/yaml',
-            body=yamldumper(self._spec_for_prefix(request))
-        )
+        return web.Response(status=200, content_type="text/yaml", body=yamldumper(self._spec_for_prefix(request)))
 
     def add_swagger_ui(self):
         """
         Adds swagger ui to {base_path}/ui/
         """
-        console_ui_path = self.options.openapi_console_ui_path.strip().rstrip('/')
-        logger.debug('Adding swagger-ui: %s%s/',
-                     self.base_path,
-                     console_ui_path)
+        console_ui_path = self.options.openapi_console_ui_path.strip().rstrip("/")
+        logger.debug("Adding swagger-ui: %s%s/", self.base_path, console_ui_path)
 
         for path in (
-            console_ui_path + '/',
-            console_ui_path + '/index.html',
+            console_ui_path + "/",
+            console_ui_path + "/index.html",
         ):
-            self.subapp.router.add_route(
-                'GET',
-                path,
-                self._get_swagger_ui_home
-            )
+            self.subapp.router.add_route("GET", path, self._get_swagger_ui_home)
 
         if self.options.openapi_console_ui_config is not None:
             self.subapp.router.add_route(
-                'GET',
-                console_ui_path + '/swagger-ui-config.json',
-                self._get_swagger_ui_config
+                "GET", console_ui_path + "/swagger-ui-config.json", self._get_swagger_ui_config
             )
 
         # we have to add an explicit redirect instead of relying on the
         # normalize_path_middleware because we also serve static files
         # from this dir (below)
 
         async def redirect(request):
-            raise web.HTTPMovedPermanently(
-                location=self.base_path + console_ui_path + '/'
-            )
+            raise web.HTTPMovedPermanently(location=self.base_path + console_ui_path + "/")
 
-        self.subapp.router.add_route(
-            'GET',
-            console_ui_path,
-            redirect
-        )
+        self.subapp.router.add_route("GET", console_ui_path, redirect)
 
         # this route will match and get a permission error when trying to
         # serve index.html, so we add the redirect above.
         self.subapp.router.add_static(
-            console_ui_path,
-            path=str(self.options.openapi_console_ui_from_dir),
-            name='swagger_ui_static'
+            console_ui_path, path=str(self.options.openapi_console_ui_from_dir), name="swagger_ui_static"
         )
 
-    @aiohttp_jinja2.template('index.j2')
+    @aiohttp_jinja2.template("index.j2")
     async def _get_swagger_ui_home(self, req):
         base_path = self._base_path_for_prefix(req)
         template_variables = {
-            'openapi_spec_url': (base_path + self.options.openapi_spec_path),
+            "openapi_spec_url": (base_path + self.options.openapi_spec_path),
             **self.options.openapi_console_ui_index_template_variables,
         }
         if self.options.openapi_console_ui_config is not None:
-            template_variables['configUrl'] = 'swagger-ui-config.json'
+            template_variables["configUrl"] = "swagger-ui-config.json"
         return template_variables
 
     async def _get_swagger_ui_config(self, req):
         return web.Response(
-            status=200,
-            content_type='text/json',
-            body=self.jsonifier.dumps(self.options.openapi_console_ui_config)
+            status=200, content_type="text/json", body=self.jsonifier.dumps(self.options.openapi_console_ui_config)
         )
 
     def add_auth_on_not_found(self, security, security_definitions):
         """
         Adds a 404 error handler to authenticate and only expose the 404 status if the security validation pass.
         """
-        logger.debug('Adding path not found authentication')
+        logger.debug("Adding path not found authentication")
         not_found_error = AuthErrorHandler(
-            self, _HttpNotFoundError(),
-            security=security,
-            security_definitions=security_definitions
+            self, _HttpNotFoundError(), security=security, security_definitions=security_definitions
         )
         endpoint_name = f"{self._api_name}_not_found"
-        self.subapp.router.add_route(
-            '*',
-            '/{not_found_path}',
-            not_found_error.function,
-            name=endpoint_name
-        )
+        self.subapp.router.add_route("*", "/{not_found_path}", not_found_error.function, name=endpoint_name)
 
     def _add_operation_internal(self, method, path, operation):
         method = method.upper()
         operation_id = operation.operation_id or path
 
-        logger.debug('... Adding %s -> %s', method, operation_id,
-                     extra=vars(operation))
+        logger.debug("... Adding %s -> %s", method, operation_id, extra=vars(operation))
 
         handler = operation.function
-        endpoint_name = '{}_{}_{}'.format(
-            self._api_name,
-            AioHttpApi.normalize_string(path),
-            method.lower()
-        )
-        self.subapp.router.add_route(
-            method, path, handler, name=endpoint_name
-        )
+        endpoint_name = "{}_{}_{}".format(self._api_name, AioHttpApi.normalize_string(path), method.lower())
+        self.subapp.router.add_route(method, path, handler, name=endpoint_name)
 
-        if not path.endswith('/'):
-            self.subapp.router.add_route(
-                method, path + '/', handler, name=endpoint_name + '_'
-            )
+        if not path.endswith("/"):
+            self.subapp.router.add_route(method, path + "/", handler, name=endpoint_name + "_")
 
     @classmethod
     async def get_request(cls, req):
         """Convert aiohttp request to firetail
 
         :param req: instance of aiohttp.web.Request
         :return: firetail request instance
         :rtype: FiretailRequest
         """
         url = str(req.url)
 
         logger.debug(
-            'Getting data and status code',
+            "Getting data and status code",
             extra={
                 # has_body | can_read_body report if
                 # body has been read or not
                 # body_exists refers to underlying stream of data
-                'body_exists': req.body_exists,
-                'can_read_body': req.can_read_body,
-                'content_type': req.content_type,
-                'url': url,
+                "body_exists": req.body_exists,
+                "can_read_body": req.can_read_body,
+                "content_type": req.content_type,
+                "url": url,
             },
         )
 
         query = parse_qs(req.rel_url.query_string)
         headers = req.headers
         body = None
 
@@ -327,15 +270,15 @@
         #       then `post_data` will be left an empty dict and the stream will not be consumed.
         post_data = await req.post()
 
         files = {}
         form = {}
 
         if post_data:
-            logger.debug('Reading multipart data from request')
+            logger.debug("Reading multipart data from request")
             for k, v in post_data.items():
                 if isinstance(v, web.FileField):
                     if k in files:
                         # if multiple files arrive under the same name in the
                         # request, downstream requires that we put them all into
                         # a list under the same key in the files dict.
                         if isinstance(files[k], list):
@@ -344,86 +287,87 @@
                             files[k] = [files[k], v]
                     else:
                         files[k] = v
                 else:
                     # put normal fields as an array, that's how werkzeug does that for Flask
                     # and that's what Firetail expects in its processing functions
                     form[k] = [v]
-            body = b''
+            body = b""
         else:
-            logger.debug('Reading data from request')
+            logger.debug("Reading data from request")
             body = await req.read()
 
-        return FiretailRequest(url=url,
-                               method=req.method.lower(),
-                               path_params=dict(req.match_info),
-                               query=query,
-                               headers=headers,
-                               body=body,
-                               json_getter=lambda: cls.jsonifier.loads(body),
-                               form=form,
-                               files=files,
-                               context=req,
-                               cookies=req.cookies)
+        return FiretailRequest(
+            url=url,
+            method=req.method.lower(),
+            path_params=dict(req.match_info),
+            query=query,
+            headers=headers,
+            body=body,
+            json_getter=lambda: cls.jsonifier.loads(body),
+            form=form,
+            files=files,
+            context=req,
+            cookies=req.cookies,
+        )
 
     @classmethod
     async def get_response(cls, response, mimetype=None, request=None):
         """Get response.
         This method is used in the lifecycle decorators
 
         :type response: aiohttp.web.StreamResponse | (Any,) | (Any, int) | (Any, dict) | (Any, int, dict)
         :rtype: aiohttp.web.Response
         """
         while asyncio.iscoroutine(response):
             response = await response
 
-        url = str(request.url) if request else ''
+        url = str(request.url) if request else ""
 
         return cls._get_response(response, mimetype=mimetype, extra_context={"url": url})
 
     @classmethod
     def _is_framework_response(cls, response):
-        """ Return True if `response` is a framework response class """
+        """Return True if `response` is a framework response class"""
         return isinstance(response, web.StreamResponse)
 
     @classmethod
     def _framework_to_firetail_response(cls, response, mimetype):
-        """ Cast framework response class to FiretailResponse used for schema validation """
+        """Cast framework response class to FiretailResponse used for schema validation"""
         body = None
         if hasattr(response, "body"):  # StreamResponse and FileResponse don't have body
             body = response.body
         return FiretailResponse(
             status_code=response.status,
             mimetype=mimetype,
             content_type=response.content_type,
             headers=response.headers,
-            body=body
+            body=body,
         )
 
     @classmethod
     def _firetail_to_framework_response(cls, response, mimetype, extra_context=None):
-        """ Cast FiretailResponse to framework response class """
+        """Cast FiretailResponse to framework response class"""
         return cls._build_response(
             mimetype=response.mimetype or mimetype,
             status_code=response.status_code,
             content_type=response.content_type,
             headers=response.headers,
             data=response.body,
             extra_context=extra_context,
         )
 
     @classmethod
     def _build_response(cls, data, mimetype, content_type=None, headers=None, status_code=None, extra_context=None):
         if cls._is_framework_response(data):
             raise TypeError("Cannot return web.StreamResponse in tuple. Only raw data can be returned in tuple.")
 
-        data, status_code, serialized_mimetype = cls._prepare_body_and_status_code(data=data,
-                                                                                   mimetype=mimetype,
-                                                                                   status_code=status_code,
-                                                                                   extra_context=extra_context)
+        data, status_code, serialized_mimetype = cls._prepare_body_and_status_code(
+            data=data, mimetype=mimetype, status_code=status_code, extra_context=extra_context
+        )
 
         if isinstance(data, str):
             text = data
             body = None
         else:
             text = None
             body = data
@@ -434,17 +378,17 @@
     @classmethod
     def _set_jsonifier(cls):
         cls.jsonifier = Jsonifier(cls=JSONEncoder)
 
 
 class _HttpNotFoundError(HTTPNotFound):
     def __init__(self):
-        self.name = 'Not Found'
+        self.name = "Not Found"
         self.description = (
-            'The requested URL was not found on the server. '
-            'If you entered the URL manually please check your spelling and '
-            'try again.'
+            "The requested URL was not found on the server. "
+            "If you entered the URL manually please check your spelling and "
+            "try again."
         )
         self.code = type(self).status_code
         self.empty_body = True
 
         HTTPNotFound.__init__(self, reason=self.name)
```

### Comparing `firetail-1.0.8/firetail/apis/flask_api.py` & `firetail-1.0.9/firetail/apis/flask_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,223 +2,206 @@
 This module defines a Flask Firetail API which implements translations between Flask and
 Firetail requests / responses.
 """
 
 import logging
 import pathlib
 import warnings
-from typing import Any
+from typing import Any  # noqa
 
 import flask
 import werkzeug.exceptions
 from werkzeug.local import LocalProxy
 
 from firetail.apis import flask_utils
 from firetail.apis.abstract import AbstractAPI
 from firetail.handlers import AuthErrorHandler
 from firetail.jsonifier import Jsonifier
 from firetail.lifecycle import FiretailRequest, FiretailResponse
 from firetail.security import FlaskSecurityHandlerFactory
 from firetail.utils import is_json_mimetype, yamldumper
 
-logger = logging.getLogger('firetail.apis.flask_api')
+logger = logging.getLogger("firetail.apis.flask_api")
 
 
 class FlaskApi(AbstractAPI):
-
     @staticmethod
     def make_security_handler_factory(pass_context_arg_name):
-        """ Create default SecurityHandlerFactory to create all security check handlers """
+        """Create default SecurityHandlerFactory to create all security check handlers"""
         return FlaskSecurityHandlerFactory(pass_context_arg_name)
 
     def _set_base_path(self, base_path):
         super()._set_base_path(base_path)
         self._set_blueprint()
 
     def _set_blueprint(self):
-        logger.debug('Creating API blueprint: %s', self.base_path)
+        logger.debug("Creating API blueprint: %s", self.base_path)
         endpoint = flask_utils.flaskify_endpoint(self.base_path)
-        self.blueprint = flask.Blueprint(endpoint, __name__, url_prefix=self.base_path,
-                                         template_folder=str(self.options.openapi_console_ui_from_dir))
+        self.blueprint = flask.Blueprint(
+            endpoint, __name__, url_prefix=self.base_path, template_folder=str(self.options.openapi_console_ui_from_dir)
+        )
 
     def add_openapi_json(self):
         """
         Adds spec json to {base_path}/swagger.json
         or {base_path}/openapi.json (for oas3)
         """
-        logger.debug('Adding spec json: %s/%s', self.base_path,
-                     self.options.openapi_spec_path)
+        logger.debug("Adding spec json: %s/%s", self.base_path, self.options.openapi_spec_path)
         endpoint_name = f"{self.blueprint.name}_openapi_json"
 
-        self.blueprint.add_url_rule(self.options.openapi_spec_path,
-                                    endpoint_name,
-                                    self._handlers.get_json_spec)
+        self.blueprint.add_url_rule(self.options.openapi_spec_path, endpoint_name, self._handlers.get_json_spec)
 
     def add_openapi_yaml(self):
         """
         Adds spec yaml to {base_path}/swagger.yaml
         or {base_path}/openapi.yaml (for oas3)
         """
         if not self.options.openapi_spec_path.endswith("json"):
             return
 
-        openapi_spec_path_yaml = \
-            self.options.openapi_spec_path[:-len("json")] + "yaml"
-        logger.debug('Adding spec yaml: %s/%s', self.base_path,
-                     openapi_spec_path_yaml)
+        openapi_spec_path_yaml = self.options.openapi_spec_path[: -len("json")] + "yaml"
+        logger.debug("Adding spec yaml: %s/%s", self.base_path, openapi_spec_path_yaml)
         endpoint_name = f"{self.blueprint.name}_openapi_yaml"
-        self.blueprint.add_url_rule(
-            openapi_spec_path_yaml,
-            endpoint_name,
-            self._handlers.get_yaml_spec
-        )
+        self.blueprint.add_url_rule(openapi_spec_path_yaml, endpoint_name, self._handlers.get_yaml_spec)
 
     def add_swagger_ui(self):
         """
         Adds swagger ui to {base_path}/ui/
         """
-        console_ui_path = self.options.openapi_console_ui_path.strip('/')
-        logger.debug('Adding swagger-ui: %s/%s/',
-                     self.base_path,
-                     console_ui_path)
+        console_ui_path = self.options.openapi_console_ui_path.strip("/")
+        logger.debug("Adding swagger-ui: %s/%s/", self.base_path, console_ui_path)
 
         if self.options.openapi_console_ui_config is not None:
             config_endpoint_name = f"{self.blueprint.name}_swagger_ui_config"
-            config_file_url = '/{console_ui_path}/swagger-ui-config.json'.format(
-                console_ui_path=console_ui_path)
+            config_file_url = "/{console_ui_path}/swagger-ui-config.json".format(console_ui_path=console_ui_path)
 
-            self.blueprint.add_url_rule(config_file_url,
-                                        config_endpoint_name,
-                                        lambda: flask.jsonify(self.options.openapi_console_ui_config))
+            self.blueprint.add_url_rule(
+                config_file_url, config_endpoint_name, lambda: flask.jsonify(self.options.openapi_console_ui_config)
+            )
 
         static_endpoint_name = f"{self.blueprint.name}_swagger_ui_static"
-        static_files_url = '/{console_ui_path}/<path:filename>'.format(
-            console_ui_path=console_ui_path)
+        static_files_url = "/{console_ui_path}/<path:filename>".format(console_ui_path=console_ui_path)
 
-        self.blueprint.add_url_rule(static_files_url,
-                                    static_endpoint_name,
-                                    self._handlers.console_ui_static_files)
+        self.blueprint.add_url_rule(static_files_url, static_endpoint_name, self._handlers.console_ui_static_files)
 
         index_endpoint_name = f"{self.blueprint.name}_swagger_ui_index"
-        console_ui_url = '/{console_ui_path}/'.format(
-            console_ui_path=console_ui_path)
+        console_ui_url = "/{console_ui_path}/".format(console_ui_path=console_ui_path)
 
-        self.blueprint.add_url_rule(console_ui_url,
-                                    index_endpoint_name,
-                                    self._handlers.console_ui_home)
+        self.blueprint.add_url_rule(console_ui_url, index_endpoint_name, self._handlers.console_ui_home)
 
     def add_auth_on_not_found(self, security, security_definitions):
         """
         Adds a 404 error handler to authenticate and only expose the 404 status if the security validation pass.
         """
-        logger.debug('Adding path not found authentication')
-        not_found_error = AuthErrorHandler(self, werkzeug.exceptions.NotFound(), security=security,
-                                           security_definitions=security_definitions)
+        logger.debug("Adding path not found authentication")
+        not_found_error = AuthErrorHandler(
+            self, werkzeug.exceptions.NotFound(), security=security, security_definitions=security_definitions
+        )
         endpoint_name = f"{self.blueprint.name}_not_found"
-        self.blueprint.add_url_rule('/<path:invalid_path>', endpoint_name, not_found_error.function)
+        self.blueprint.add_url_rule("/<path:invalid_path>", endpoint_name, not_found_error.function)
 
     def _add_operation_internal(self, method, path, operation):
         operation_id = operation.operation_id
-        logger.debug('... Adding %s -> %s', method.upper(), operation_id,
-                     extra=vars(operation))
+        logger.debug("... Adding %s -> %s", method.upper(), operation_id, extra=vars(operation))
 
         flask_path = flask_utils.flaskify_path(path, operation.get_path_parameter_types())
-        endpoint_name = flask_utils.flaskify_endpoint(operation.operation_id,
-                                                      operation.randomize_endpoint)
+        endpoint_name = flask_utils.flaskify_endpoint(operation.operation_id, operation.randomize_endpoint)
         function = operation.function
         self.blueprint.add_url_rule(flask_path, endpoint_name, function, methods=[method])
 
     @property
     def _handlers(self):
         # type: () -> InternalHandlers
-        if not hasattr(self, '_internal_handlers'):
+        if not hasattr(self, "_internal_handlers"):
             self._internal_handlers = InternalHandlers(self.base_path, self.options, self.specification)
         return self._internal_handlers
 
     @classmethod
     def get_response(cls, response, mimetype=None, request=None):
         """Gets FiretailResponse instance for the operation handler
         result. Status Code and Headers for response.  If only body
         data is returned by the endpoint function, then the status
         code will be set to 200 and no headers will be added.
 
         If the returned object is a flask.Response then it will just
         pass the information needed to recreate it.
 
-        :type response: flask.Response | (flask.Response,) | (flask.Response, int) | (flask.Response, dict) | (flask.Response, int, dict)
+        :type response: flask.Response | (flask.Response,) |
+           (flask.Response, int) | (flask.Response, dict) | (flask.Response, int, dict)
         :rtype: FiretailResponse
         """
         return cls._get_response(response, mimetype=mimetype, extra_context={"url": flask.request.url})
 
     @classmethod
     def _is_framework_response(cls, response):
-        """ Return True if provided response is a framework type """
+        """Return True if provided response is a framework type"""
         return flask_utils.is_flask_response(response)
 
     @classmethod
     def _framework_to_firetail_response(cls, response, mimetype):
-        """ Cast framework response class to FiretailResponse used for schema validation """
+        """Cast framework response class to FiretailResponse used for schema validation"""
         return FiretailResponse(
             status_code=response.status_code,
             mimetype=response.mimetype,
             content_type=response.content_type,
             headers=response.headers,
             body=response.get_data() if not response.direct_passthrough else None,
-            is_streamed=response.is_streamed
+            is_streamed=response.is_streamed,
         )
 
     @classmethod
     def _firetail_to_framework_response(cls, response, mimetype, extra_context=None):
-        """ Cast FiretailResponse to framework response class """
+        """Cast FiretailResponse to framework response class"""
         flask_response = cls._build_response(
             mimetype=response.mimetype or mimetype,
             content_type=response.content_type,
             headers=response.headers,
             status_code=response.status_code,
             data=response.body,
             extra_context=extra_context,
-            )
+        )
 
         return flask_response
 
     @classmethod
-    def _build_response(cls, mimetype, content_type=None, headers=None, status_code=None, data=None, extra_context=None):
+    def _build_response(
+        cls, mimetype, content_type=None, headers=None, status_code=None, data=None, extra_context=None
+    ):
         if cls._is_framework_response(data):
             return flask.current_app.make_response((data, status_code, headers))
 
-        data, status_code, serialized_mimetype = cls._prepare_body_and_status_code(data=data,
-                                                                                   mimetype=mimetype,
-                                                                                   status_code=status_code,
-                                                                                   extra_context=extra_context)
+        data, status_code, serialized_mimetype = cls._prepare_body_and_status_code(
+            data=data, mimetype=mimetype, status_code=status_code, extra_context=extra_context
+        )
 
         kwargs = {
-            'mimetype': mimetype or serialized_mimetype,
-            'content_type': content_type,
-            'headers': headers,
-            'response': data,
-            'status': status_code
+            "mimetype": mimetype or serialized_mimetype,
+            "content_type": content_type,
+            "headers": headers,
+            "response": data,
+            "status": status_code,
         }
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         return flask.current_app.response_class(**kwargs)
 
     @classmethod
     def _serialize_data(cls, data, mimetype):
         # TODO: harmonize flask and aiohttp serialization when mimetype=None or mimetype is not JSON
         #       (cases where it might not make sense to jsonify the data)
-        if (isinstance(mimetype, str) and is_json_mimetype(mimetype)):
+        if isinstance(mimetype, str) and is_json_mimetype(mimetype):
             body = cls.jsonifier.dumps(data)
         elif not (isinstance(data, bytes) or isinstance(data, str)):
             warnings.warn(
                 "Implicit (flask) JSON serialization will change in the next major version. "
                 "This is triggered because a response body is being serialized as JSON "
                 "even though the mimetype is not a JSON type. "
                 "This will be replaced by something that is mimetype-specific and may "
                 "raise an error instead of silently converting everything to JSON. "
                 "Please make sure to specify media/mime types in your specs.",
-                FutureWarning  # a Deprecation targeted at application users.
+                FutureWarning,  # a Deprecation targeted at application users.
             )
             body = cls.jsonifier.dumps(data)
         else:
             body = data
 
         return body, mimetype
 
@@ -232,47 +215,45 @@
 
         If the returned object is a flask.Response then it will just
         pass the information needed to recreate it.
 
         :rtype: FiretailRequest
         """
         context_dict = {}
-        setattr(flask._request_ctx_stack.top, 'firetail_context', context_dict)
+        setattr(flask._request_ctx_stack.top, "firetail_context", context_dict)
         flask_request = flask.request
         request = FiretailRequest(
             flask_request.url,
             flask_request.method,
             headers=flask_request.headers,
             form=flask_request.form,
             query=flask_request.args,
             body=flask_request.get_data(),
             json_getter=lambda: flask_request.get_json(silent=True),
             files=flask_request.files,
             path_params=params,
             context=context_dict,
             cookies=flask_request.cookies,
         )
-        logger.debug('Getting data and status code',
-                     extra={
-                         'data': request.body,
-                         'data_type': type(request.body),
-                         'url': request.url
-                     })
+        logger.debug(
+            "Getting data and status code",
+            extra={"data": request.body, "data_type": type(request.body), "url": request.url},
+        )
         return request
 
     @classmethod
     def _set_jsonifier(cls):
         """
         Use Flask specific JSON loader
         """
         cls.jsonifier = Jsonifier(flask.json, indent=2)
 
 
 def _get_context():
-    return getattr(flask._request_ctx_stack.top, 'firetail_context')
+    return getattr(flask._request_ctx_stack.top, "firetail_context")
 
 
 context = LocalProxy(_get_context)
 
 
 class InternalHandlers:
     """
@@ -288,30 +269,27 @@
         """
         Home page of the OpenAPI Console UI.
 
         :return:
         """
         openapi_json_route_name = "{blueprint}.{prefix}_openapi_json"
         escaped = flask_utils.flaskify_endpoint(self.base_path)
-        openapi_json_route_name = openapi_json_route_name.format(
-            blueprint=escaped,
-            prefix=escaped
-        )
+        openapi_json_route_name = openapi_json_route_name.format(blueprint=escaped, prefix=escaped)
         template_variables = {
-            'openapi_spec_url': flask.url_for(openapi_json_route_name),
+            "openapi_spec_url": flask.url_for(openapi_json_route_name),
             **self.options.openapi_console_ui_index_template_variables,
         }
         if self.options.openapi_console_ui_config is not None:
-            template_variables['configUrl'] = 'swagger-ui-config.json'
+            template_variables["configUrl"] = "swagger-ui-config.json"
 
         # Use `render_template_string` instead of `render_template` to circumvent the flask
         # template lookup mechanism and explicitly render the template of the current blueprint.
         # https://github.com/zalando/firetail/issues/1289#issuecomment-884105076
         template_dir = pathlib.Path(self.options.openapi_console_ui_from_dir)
-        index_path = template_dir / 'index.j2'
+        index_path = template_dir / "index.j2"
         return flask.render_template_string(index_path.read_text(), **template_variables)
 
     def console_ui_static_files(self, filename):
         """
         Servers the static files for the OpenAPI Console UI.
 
         :param filename: Requested file contents.
```

### Comparing `firetail-1.0.8/firetail/apis/flask_utils.py` & `firetail-1.0.9/firetail/apis/flask_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,53 +6,47 @@
 import random
 import re
 import string
 
 import flask
 import werkzeug.wrappers
 
-PATH_PARAMETER = re.compile(r'\{([^}]*)\}')
+PATH_PARAMETER = re.compile(r"\{([^}]*)\}")
 
 # map Swagger type to flask path converter
 # see http://flask.pocoo.org/docs/0.10/api/#url-route-registrations
-PATH_PARAMETER_CONVERTERS = {
-    'integer': 'int',
-    'number': 'float',
-    'path': 'path'
-}
+PATH_PARAMETER_CONVERTERS = {"integer": "int", "number": "float", "path": "path"}
 
 
 def flaskify_endpoint(identifier, randomize=None):
     """
     Converts the provided identifier in a valid flask endpoint name
 
     :type identifier: str
     :param randomize: If specified, add this many random characters (upper case
         and digits) to the endpoint name, separated by a pipe character.
     :type randomize: int | None
     :rtype: str
 
     """
-    result = identifier.replace('.', '_')
+    result = identifier.replace(".", "_")
     if randomize is None:
         return result
 
     chars = string.ascii_uppercase + string.digits
     return "{result}|{random_string}".format(
-        result=result,
-        random_string=''.join(random.SystemRandom().choice(chars) for _ in range(randomize)))
+        result=result, random_string="".join(random.SystemRandom().choice(chars) for _ in range(randomize))
+    )
 
 
 def convert_path_parameter(match, types):
     name = match.group(1)
     swagger_type = types.get(name)
     converter = PATH_PARAMETER_CONVERTERS.get(swagger_type)
-    return '<{}{}{}>'.format(
-        converter or '', ':' if converter else '', name.replace('-', '_')
-    )
+    return "<{}{}{}>".format(converter or "", ":" if converter else "", name.replace("-", "_"))
 
 
 def flaskify_path(swagger_path, types=None):
     """
     Convert swagger path templates to flask path templates
 
     :type swagger_path: str
```

### Comparing `firetail-1.0.8/firetail/apps/abstract.py` & `firetail-1.0.9/firetail/apps/abstract.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,21 +6,34 @@
 import abc
 import logging
 import pathlib
 
 from ..options import FiretailOptions
 from ..resolver import Resolver
 
-logger = logging.getLogger('firetail.app')
+logger = logging.getLogger("firetail.app")
 
 
 class AbstractApp(metaclass=abc.ABCMeta):
-    def __init__(self, import_name, api_cls, port=None, specification_dir='',
-                 host=None, server=None, server_args=None, arguments=None, auth_all_paths=False, debug=None,
-                 resolver=None, options=None, skip_error_handlers=False):
+    def __init__(
+        self,
+        import_name,
+        api_cls,
+        port=None,
+        specification_dir="",
+        host=None,
+        server=None,
+        server_args=None,
+        arguments=None,
+        auth_all_paths=False,
+        debug=None,
+        resolver=None,
+        options=None,
+        skip_error_handlers=False,
+    ):
         """
         :param import_name: the name of the application package
         :type import_name: str
         :param host: the host interface to bind on.
         :type host: str
         :param port: port to listen to
         :type port: int
@@ -54,26 +67,26 @@
 
         self.server = server
         self.server_args = dict() if server_args is None else server_args
         self.app = self.create_app()
 
         # we get our application root path to avoid duplicating logic
         self.root_path = self.get_root_path()
-        logger.debug('Root Path: %s', self.root_path)
+        logger.debug("Root Path: %s", self.root_path)
 
         specification_dir = pathlib.Path(specification_dir)  # Ensure specification dir is a Path
         if specification_dir.is_absolute():
             self.specification_dir = specification_dir
         else:
             self.specification_dir = self.root_path / specification_dir
 
-        logger.debug('Specification directory: %s', self.specification_dir)
+        logger.debug("Specification directory: %s", self.specification_dir)
 
         if not skip_error_handlers:
-            logger.debug('Setting error handlers')
+            logger.debug("Setting error handlers")
             self.set_errors_handlers()
 
     @abc.abstractmethod
     def create_app(self):
         """
         Creates the user framework application
         """
@@ -86,19 +99,29 @@
 
     @abc.abstractmethod
     def set_errors_handlers(self):
         """
         Sets all errors handlers of the user framework application
         """
 
-    def add_api(self, specification, base_path=None, arguments=None,
-                auth_all_paths=None, validate_responses=False,
-                strict_validation=False, resolver=None, resolver_error=None,
-                pythonic_params=False, pass_context_arg_name=None, options=None,
-                validator_map=None):
+    def add_api(
+        self,
+        specification,
+        base_path=None,
+        arguments=None,
+        auth_all_paths=None,
+        validate_responses=False,
+        strict_validation=False,
+        resolver=None,
+        resolver_error=None,
+        pythonic_params=False,
+        pass_context_arg_name=None,
+        options=None,
+        validator_map=None,
+    ):
         """
         Adds an API to the application based on a swagger file or API dict
 
         :param specification: swagger file with the specification | specification dict
         :type specification: pathlib.Path or str or dict
         :param base_path: base path where to add this api
         :type base_path: str | None
@@ -128,45 +151,48 @@
         # Turn the resolver_error code into a handler object
         self.resolver_error = resolver_error
         resolver_error_handler = None
         if self.resolver_error is not None:
             resolver_error_handler = self._resolver_error_handler
 
         resolver = resolver or self.resolver
-        resolver = Resolver(resolver) if hasattr(resolver, '__call__') else resolver
+        resolver = Resolver(resolver) if hasattr(resolver, "__call__") else resolver
 
         auth_all_paths = auth_all_paths if auth_all_paths is not None else self.auth_all_paths
         # TODO test if base_path starts with an / (if not none)
         arguments = arguments or dict()
         arguments = dict(self.arguments, **arguments)  # copy global arguments and update with api specific
 
         if isinstance(specification, dict):
             specification = specification
         else:
             specification = self.specification_dir / specification
 
         api_options = self.options.extend(options)
 
-        api = self.api_cls(specification,
-                           base_path=base_path,
-                           arguments=arguments,
-                           resolver=resolver,
-                           resolver_error_handler=resolver_error_handler,
-                           validate_responses=validate_responses,
-                           strict_validation=strict_validation,
-                           auth_all_paths=auth_all_paths,
-                           debug=self.debug,
-                           validator_map=validator_map,
-                           pythonic_params=pythonic_params,
-                           pass_context_arg_name=pass_context_arg_name,
-                           options=api_options.as_dict())
+        api = self.api_cls(
+            specification,
+            base_path=base_path,
+            arguments=arguments,
+            resolver=resolver,
+            resolver_error_handler=resolver_error_handler,
+            validate_responses=validate_responses,
+            strict_validation=strict_validation,
+            auth_all_paths=auth_all_paths,
+            debug=self.debug,
+            validator_map=validator_map,
+            pythonic_params=pythonic_params,
+            pass_context_arg_name=pass_context_arg_name,
+            options=api_options.as_dict(),
+        )
         return api
 
     def _resolver_error_handler(self, *args, **kwargs):
         from firetail.handlers import ResolverErrorHandler
+
         return ResolverErrorHandler(self.api_cls, self.resolver_error, *args, **kwargs)
 
     def add_url_rule(self, rule, endpoint=None, view_func=None, **options):
         """
         Connects a URL rule.  Works exactly like the `route` decorator.  If a view_func is provided it will be
         registered with the endpoint.
 
@@ -197,17 +223,17 @@
         :param view_func: the function to call when serving a request to the provided endpoint
         :type view_func: types.FunctionType
         :param options: the options to be forwarded to the underlying `werkzeug.routing.Rule` object.  A change
                         to Werkzeug is handling of method options. methods is a list of methods this rule should be
                         limited to (`GET`, `POST` etc.).  By default a rule just listens for `GET` (and implicitly
                         `HEAD`).
         """
-        log_details = {'endpoint': endpoint, 'view_func': view_func.__name__}
+        log_details = {"endpoint": endpoint, "view_func": view_func.__name__}
         log_details.update(options)
-        logger.debug('Adding %s', rule, extra=log_details)
+        logger.debug("Adding %s", rule, extra=log_details)
         self.app.add_url_rule(rule, endpoint, view_func, **options)
 
     def route(self, rule, **options):
         """
         A decorator that is used to register a view function for a
         given URL rule.  This does the same thing as `add_url_rule`
         but is intended for decorator usage::
@@ -222,15 +248,15 @@
                          itself assumes the name of the view function as
                          endpoint
         :param options: the options to be forwarded to the underlying `werkzeug.routing.Rule` object.  A change
                         to Werkzeug is handling of method options.  methods is a list of methods this rule should be
                         limited to (`GET`, `POST` etc.).  By default a rule just listens for `GET` (and implicitly
                         `HEAD`).
         """
-        logger.debug('Adding %s with decorator', rule, extra=options)
+        logger.debug("Adding %s with decorator", rule, extra=options)
         return self.app.route(rule, **options)
 
     @abc.abstractmethod
     def run(self, port=None, server=None, debug=None, host=None, **options):  # pragma: no cover
         """
         Runs the application on a local development server.
         :param host: the host interface to bind on.
```

### Comparing `firetail-1.0.8/firetail/apps/aiohttp_app.py` & `firetail-1.0.9/firetail/apps/aiohttp_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,36 +9,35 @@
 
 from aiohttp import web
 
 from ..apis.aiohttp_api import AioHttpApi
 from ..exceptions import FiretailException
 from .abstract import AbstractApp
 
-logger = logging.getLogger('firetail.aiohttp_app')
+logger = logging.getLogger("firetail.aiohttp_app")
 
 
 class AioHttpApp(AbstractApp):
-
     def __init__(self, import_name, only_one_api=False, **kwargs):
-        super().__init__(import_name, AioHttpApi, server='aiohttp', **kwargs)
+        super().__init__(import_name, AioHttpApi, server="aiohttp", **kwargs)
         self._only_one_api = only_one_api
         self._api_added = False
 
     def create_app(self):
         return web.Application(**self.server_args)
 
     def get_root_path(self):
         mod = sys.modules.get(self.import_name)
-        if mod is not None and hasattr(mod, '__file__'):
+        if mod is not None and hasattr(mod, "__file__"):
             return pathlib.Path(mod.__file__).resolve().parent
 
         loader = pkgutil.get_loader(self.import_name)
         filepath = None
 
-        if hasattr(loader, 'get_filename'):
+        if hasattr(loader, "get_filename"):
             filepath = loader.get_filename(self.import_name)
 
         if filepath is None:
             raise RuntimeError(f"Invalid import name '{self.import_name}'")
 
         return pathlib.Path(filepath).resolve().parent
 
@@ -59,41 +58,40 @@
                 return self.app
 
         api = self._get_api(specification, kwargs)
         try:
             self.app.add_subapp(api.base_path, api.subapp)
         except ValueError:
             raise FiretailException(
-                "aiohttp doesn't allow to set empty base_path ('/'), "
-                "use non-empty instead, e.g /api"
+                "aiohttp doesn't allow to set empty base_path ('/'), " "use non-empty instead, e.g /api"
             )
 
         return api
 
     def _get_api(self, specification, kwargs):
         return super().add_api(specification, **kwargs)
 
     def run(self, port=None, server=None, debug=None, host=None, **options):
         if port is not None:
             self.port = port
         elif self.port is None:
             self.port = 5000
 
         self.server = server or self.server
-        self.host = host or self.host or '0.0.0.0'
+        self.host = host or self.host or "0.0.0.0"
 
         if debug is not None:
             self.debug = debug
 
-        logger.debug('Starting %s HTTP server..', self.server, extra=vars(self))
+        logger.debug("Starting %s HTTP server..", self.server, extra=vars(self))
 
-        if self.server == 'aiohttp':
-            logger.info('Listening on %s:%s..', self.host, self.port)
+        if self.server == "aiohttp":
+            logger.info("Listening on %s:%s..", self.host, self.port)
 
-            access_log = options.pop('access_log', None)
+            access_log = options.pop("access_log", None)
 
-            if options.pop('use_default_access_log', None):
+            if options.pop("use_default_access_log", None):
                 access_log = logger
 
             web.run_app(self.app, port=self.port, host=self.host, access_log=access_log, **options)
         else:
-            raise Exception(f'Server {self.server} not recognized')
+            raise Exception(f"Server {self.server} not recognized")
```

### Comparing `firetail-1.0.8/firetail/apps/flask_app.py` & `firetail-1.0.9/firetail/apps/flask_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 from flask import json, signals
 
 from ..apis.flask_api import FlaskApi
 from ..exceptions import ProblemException
 from ..problem import problem
 from .abstract import AbstractApp
 
-logger = logging.getLogger('firetail.app')
+logger = logging.getLogger("firetail.app")
 
 
 class FlaskApp(AbstractApp):
-    def __init__(self, import_name, server='flask', extra_files=None, **kwargs):
+    def __init__(self, import_name, server="flask", extra_files=None, **kwargs):
         """
         :param extra_files: additional files to be watched by the reloader, defaults to the swagger specs of added apis
         :type extra_files: list[str | pathlib.Path], optional
 
-        See :class:`~firetail.AbstractApp` for additional parameters.
+        See :class:`~firetail.AbstractApp` for additional parameters.  # noqa RST304
         """
         super().__init__(import_name, FlaskApi, server=server, **kwargs)
         self.extra_files = extra_files or []
 
     def create_app(self):
         app = flask.Flask(self.import_name, **self.server_args)
         app.json_encoder = FlaskJSONEncoder
-        app.url_map.converters['float'] = NumberConverter
-        app.url_map.converters['int'] = IntegerConverter
+        app.url_map.converters["float"] = NumberConverter
+        app.url_map.converters["int"] = IntegerConverter
         return app
 
     def get_root_path(self):
         return pathlib.Path(self.app.root_path)
 
     def set_errors_handlers(self):
         for error_code in werkzeug.exceptions.default_exceptions:
@@ -50,46 +50,47 @@
     def common_error_handler(self, exception):
         """
         :type exception: Exception
         """
         signals.got_request_exception.send(self.app, exception=exception)
         if isinstance(exception, ProblemException):
             response = problem(
-                status=exception.status, title=exception.title, detail=exception.detail,
-                type=exception.type, instance=exception.instance, headers=exception.headers,
-                ext=exception.ext)
+                status=exception.status,
+                title=exception.title,
+                detail=exception.detail,
+                type=exception.type,
+                instance=exception.instance,
+                headers=exception.headers,
+                ext=exception.ext,
+            )
         else:
             if not isinstance(exception, werkzeug.exceptions.HTTPException):
                 exception = werkzeug.exceptions.InternalServerError()
 
-            response = problem(title=exception.name,
-                               detail=exception.description,
-                               status=exception.code,
-                               headers=exception.get_headers())
+            response = problem(
+                title=exception.name,
+                detail=exception.description,
+                status=exception.code,
+                headers=exception.get_headers(),
+            )
 
         return FlaskApi.get_response(response)
 
     def add_api(self, specification, **kwargs):
         api = super().add_api(specification, **kwargs)
         self.app.register_blueprint(api.blueprint)
         if isinstance(specification, (str, pathlib.Path)):
             self.extra_files.append(self.specification_dir / specification)
         return api
 
     def add_error_handler(self, error_code, function):
         # type: (int, FunctionType) -> None
         self.app.register_error_handler(error_code, function)
 
-    def run(self,
-            port=None,
-            server=None,
-            debug=None,
-            host=None,
-            extra_files=None,
-            **options):  # pragma: no cover
+    def run(self, port=None, server=None, debug=None, host=None, extra_files=None, **options):  # pragma: no cover
         """
         Runs the application on a local development server.
 
         :param host: the host interface to bind on.
         :type host: str
         :param port: port to listen to
         :type port: int
@@ -105,80 +106,81 @@
 
         # overwrite constructor parameter
         if port is not None:
             self.port = port
         elif self.port is None:
             self.port = 5000
 
-        self.host = host or self.host or '0.0.0.0'
+        self.host = host or self.host or "0.0.0.0"
 
         if server is not None:
             self.server = server
 
         if debug is not None:
             self.debug = debug
 
         if extra_files is not None:
             self.extra_files.extend(extra_files)
 
-        logger.debug('Starting %s HTTP server..', self.server, extra=vars(self))
-        if self.server == 'flask':
-            self.app.run(self.host, port=self.port, debug=self.debug,
-                         extra_files=self.extra_files, **options)
-        elif self.server == 'tornado':
+        logger.debug("Starting %s HTTP server..", self.server, extra=vars(self))
+        if self.server == "flask":
+            self.app.run(self.host, port=self.port, debug=self.debug, extra_files=self.extra_files, **options)
+        elif self.server == "tornado":
             try:
                 import tornado.httpserver
                 import tornado.ioloop
                 import tornado.wsgi
             except ImportError:
-                raise Exception('tornado library not installed')
+                raise Exception("tornado library not installed")
             wsgi_container = tornado.wsgi.WSGIContainer(self.app)
             http_server = tornado.httpserver.HTTPServer(wsgi_container, **options)
             http_server.listen(self.port, address=self.host)
-            logger.info('Listening on %s:%s..', self.host, self.port)
+            logger.info("Listening on %s:%s..", self.host, self.port)
             tornado.ioloop.IOLoop.instance().start()
-        elif self.server == 'gevent':
+        elif self.server == "gevent":
             try:
                 import gevent.pywsgi
             except ImportError:
-                raise Exception('gevent library not installed')
+                raise Exception("gevent library not installed")
             http_server = gevent.pywsgi.WSGIServer((self.host, self.port), self.app, **options)
-            logger.info('Listening on %s:%s..', self.host, self.port)
+            logger.info("Listening on %s:%s..", self.host, self.port)
             http_server.serve_forever()
         else:
-            raise Exception(f'Server {self.server} not recognized')
+            raise Exception(f"Server {self.server} not recognized")
 
 
 class FlaskJSONEncoder(json.JSONEncoder):
     def default(self, o):
         if isinstance(o, datetime.datetime):
             if o.tzinfo:
                 # eg: '2015-09-25T23:14:42.588601+00:00'
-                return o.isoformat('T')
+                return o.isoformat("T")
             else:
                 # No timezone present - assume UTC.
                 # eg: '2015-09-25T23:14:42.588601Z'
-                return o.isoformat('T') + 'Z'
+                return o.isoformat("T") + "Z"
 
         if isinstance(o, datetime.date):
             return o.isoformat()
 
         if isinstance(o, Decimal):
             return float(o)
 
         return json.JSONEncoder.default(self, o)
 
 
 class NumberConverter(werkzeug.routing.BaseConverter):
-    """ Flask converter for OpenAPI number type """
+    """Flask converter for OpenAPI number type"""
+
     regex = r"[+-]?[0-9]*(\.[0-9]*)?"
 
     def to_python(self, value):
         return float(value)
 
 
 class IntegerConverter(werkzeug.routing.BaseConverter):
-    """ Flask converter for OpenAPI integer type """
+    """Flask converter for OpenAPI integer type"""
+
     regex = r"[+-]?[0-9]+"
 
     def to_python(self, value):
         return int(value)
```

### Comparing `firetail-1.0.8/firetail/auditor.py` & `firetail-1.0.9/firetail/auditor.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,33 @@
 
 import jwt
 import requests
 from flask import g, request
 
 from .logger import get_stdout_logger
 
+DEFAULT_LOG_ENDPOINT = "https://api.logging.eu-west-1.prod.firetail.app/logs/bulk"
+
 
 class cloud_logger(object):
-    def __init__(self,
-                 app,
-                 url='https://api.logging.eu-west-1.sandbox.firetail.app/logs/bulk',
-                 debug=False,
-                 custom_backend=False,
-                 token=None,
-                 backup_logs=True,
-                 network_timeout=10.0,
-                 number_of_retries=4,
-                 retry_timeout=2,
-                 logs_drain_timeout=5,
-                 scrub_headers=['set-cookie', 'cookie', 'authorization', 'x-api-key', 'token', 'api-token', 'api-key'],
-                 enrich_oauth=True
-                 ):
+    def __init__(
+        self,
+        app,
+        url=DEFAULT_LOG_ENDPOINT,
+        debug=False,
+        custom_backend=False,
+        token=None,
+        backup_logs=False,
+        network_timeout=10.0,
+        number_of_retries=4,
+        retry_timeout=2,
+        logs_drain_timeout=5,
+        scrub_headers=["set-cookie", "cookie", "authorization", "x-api-key", "token", "api-token", "api-key"],
+        enrich_oauth=True,
+    ):
         self.startThread = True
         self.custom_backend = custom_backend
         self.requests_session = requests.Session()
         self.url = url
         self.token = token
         self.auth_token = None
         self.logs_drain_timeout = logs_drain_timeout
@@ -40,83 +43,72 @@
         self.number_of_retries = number_of_retries
         self.retry_timeout = retry_timeout
         self.oauth = False
         self.logger = None
         self.enrich_oauth = enrich_oauth
         self.scrub_headers = scrub_headers
         self.LOGGING = {
-            'version': 1,
-            'disable_existing_loggers': False,
-            'formatters': {
-                'firetailFormat': {
-                    'format': '{"additional_field": "value"}',
-                    'validate': False
-                }
-            },
-            'handlers': {
-                'firetail': {
-                    'class': 'firetail.handlers.FiretailHandler',
-                    'level': 'DEBUG',
-                    'formatter': 'firetailFormat',
-                    'token': self.token,
-                    'custom_backend': self.custom_backend,
-                    'logs_drain_timeout': 5,
-                    'url': self.url,
-                    'retries_no': 4,
-                    'retry_timeout': 2,
+            "version": 1,
+            "disable_existing_loggers": False,
+            "formatters": {"firetailFormat": {"format": '{"additional_field": "value"}', "validate": False}},
+            "handlers": {
+                "firetail": {
+                    "class": "firetail.handlers.FiretailHandler",
+                    "level": "DEBUG",
+                    "formatter": "firetailFormat",
+                    "token": self.token,
+                    "custom_backend": self.custom_backend,
+                    "logs_drain_timeout": 5,
+                    "url": self.url,
+                    "retries_no": 4,
+                    "retry_timeout": 2,
                 }
             },
-            'loggers': {
-                '': {
-                    'level': 'DEBUG',
-                    'handlers': ['firetail'],
-                    'propagate': True
-                }
-            }
+            "loggers": {"": {"level": "DEBUG", "handlers": ["firetail"], "propagate": True}},
         }
         if app:
             self.init_app(app, token)
 
     def init_app(self, app, token):
         create_before_request = make_before_request_function()
         app.before_request(create_before_request)
         create_after_request = make_after_request_function(self, token)
         app.after_request(create_after_request)
 
     def set_token(self, token_secret):
         self.token = token_secret
 
     def sha1_hash(self, value):
-        hash_object = hashlib.sha1(value.encode('utf-8'))
+        hash_object = hashlib.sha1(value.encode("utf-8"))
         return "sha1:" + hash_object.hexdigest()
 
     def clean_pii(self, payload):
         clean_headers = self.scrub_headers
-        if 'req' in payload and 'headers' in payload['req']:
-            for k, v in payload['req']['headers'].items():
+        if "req" in payload and "headers" in payload["req"]:
+            for k, v in payload["req"]["headers"].items():
                 if k.lower() in clean_headers:
-                    if k.lower() == 'authorization' and 'bearer ' in v.lower():
+                    if k.lower() == "authorization" and "bearer " in v.lower():
                         self.oauth = True
                         v = v.split(" ")[1]
                         self.auth_token = v
-                    payload['req']['headers'][k] = self.sha1_hash(v)
-        if 'res' in payload and 'headers' in payload['res']:
-            for k, v in payload['res']['headers'].items():
+                    payload["req"]["headers"][k] = self.sha1_hash(v)
+        if "res" in payload and "headers" in payload["res"]:
+            for k, v in payload["res"]["headers"].items():
                 if k.lower() in clean_headers:
-                    payload['req']['headers'][k] = self.sha1_hash(v)
+                    payload["req"]["headers"][k] = self.sha1_hash(v)
 
         if self.oauth and self.enrich_oauth:
             try:
                 jwt_decoded = jwt.decode(self.auth_token, options={"verify_signature": False, "verify_exp": False})
             except jwt.exceptions.DecodeError:
                 self.oauth = False
             if self.oauth:
-                payload['oauth'] = {'sub': jwt_decoded['sub']}
-                if 'email' in jwt_decoded:
-                    payload['oauth']['email'] = jwt_decoded['email']
+                payload["oauth"] = {"sub": jwt_decoded["sub"]}
+                if "email" in jwt_decoded:
+                    payload["oauth"]["email"] = jwt_decoded["email"]
         return payload
 
     def format_headers(self, req_headers):
         result = {}
         for x, y in req_headers.items():
             result[x] = [y]
         return result
@@ -124,38 +116,38 @@
     def create(self, response, token, diff=-1, scrub_headers=None, debug=False):
         if debug:
             self.stdout_logger = get_stdout_logger(True)
         if scrub_headers and isinstance(scrub_headers, list):
             self.scrub_headers = scrub_headers
         self.token = token
         if not self.logger:
-            self.LOGGING['handlers']['firetail']['token'] = token
+            self.LOGGING["handlers"]["firetail"]["token"] = token
             logging.config.dictConfig(self.LOGGING)
-            self.logger = logging.getLogger('firetailLogger')
+            self.logger = logging.getLogger("firetailLogger")
         try:
-            response_data = response.get_json() if response.is_json else str(response.response[0].decode('utf-8'))
+            response_data = response.get_json() if response.is_json else str(response.response[0].decode("utf-8"))
         except Exception:
             response_data = ""
         payload = {
             "version": "1.0.0-alpha",
             "dateCreated": int(time.time() * 1000),
             "executionTime": diff,
             "request": {
-                "httpProtocol": request.environ.get('SERVER_PROTOCOL', "HTTP/1.1"),
+                "httpProtocol": request.environ.get("SERVER_PROTOCOL", "HTTP/1.1"),
                 "uri": request.url,
                 "headers": self.format_headers(dict(request.headers)),
-                "resource":  request.url_rule.rule if request.url_rule is not None else request.path,
+                "resource": request.url_rule.rule if request.url_rule is not None else request.path,
                 "method": request.method,
                 "body": str(request.data),
-                "ip": request.remote_addr
+                "ip": request.remote_addr,
             },
             "response": {
                 "statusCode": response.status_code,
                 "body": str(response_data),
-                "headers": self.format_headers(dict(response.headers))
+                "headers": self.format_headers(dict(response.headers)),
             },
         }
         try:
             if self.token or self.custom_backend:
                 self.logger.info(json.dumps(self.clean_pii(payload)))
         except TypeError:
             pass
@@ -164,14 +156,15 @@
 
 def make_after_request_function(cl, token):
     def logs_after_request(resp):
         diff = time.time() - g.start
         time_diff = diff * 1000
         cl.create(resp, token, round(time_diff, 2))
         return resp
+
     return logs_after_request
 
 
 def make_before_request_function():
     def logs_before_request():
         g.start = time.time()
```

### Comparing `firetail-1.0.8/firetail/cli.py` & `firetail-1.0.9/firetail/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,208 +9,214 @@
 
 import click
 from clickclick import AliasedGroup, fatal_error
 
 import firetail
 from firetail.mock import MockResolver
 
-logger = logging.getLogger('firetail.cli')
-CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
-FLASK_APP = 'flask'
-AIOHTTP_APP = 'aiohttp'
-AVAILABLE_SERVERS = {
-    'flask': [FLASK_APP],
-    'gevent': [FLASK_APP],
-    'tornado': [FLASK_APP],
-    'aiohttp': [AIOHTTP_APP]
-}
-AVAILABLE_APPS = {
-    FLASK_APP: 'firetail.apps.flask_app.FlaskApp',
-    AIOHTTP_APP: 'firetail.apps.aiohttp_app.AioHttpApp'
-}
-DEFAULT_SERVERS = {
-    FLASK_APP: FLASK_APP,
-    AIOHTTP_APP: AIOHTTP_APP
-}
+logger = logging.getLogger("firetail.cli")
+CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
+FLASK_APP = "flask"
+AIOHTTP_APP = "aiohttp"
+AVAILABLE_SERVERS = {"flask": [FLASK_APP], "gevent": [FLASK_APP], "tornado": [FLASK_APP], "aiohttp": [AIOHTTP_APP]}
+AVAILABLE_APPS = {FLASK_APP: "firetail.apps.flask_app.FlaskApp", AIOHTTP_APP: "firetail.apps.aiohttp_app.AioHttpApp"}
+DEFAULT_SERVERS = {FLASK_APP: FLASK_APP, AIOHTTP_APP: AIOHTTP_APP}
 
 
 def validate_server_requirements(ctx, param, value):
-    if value == 'gevent':
+    if value == "gevent":
         try:
             import gevent  # NOQA
         except ImportError:
-            fatal_error('gevent library is not installed')
-    elif value == 'tornado':
+            fatal_error("gevent library is not installed")
+    elif value == "tornado":
         try:
             import tornado  # NOQA
         except ImportError:
-            fatal_error('tornado library is not installed')
+            fatal_error("tornado library is not installed")
     else:
         return value
 
 
 def print_version(ctx, param, value):
     if not value or ctx.resilient_parsing:
         return
-    click.echo(f'Firetail {firetail.__version__}')
+    click.echo(f"Firetail {firetail.__version__}")
     ctx.exit()
 
 
 @click.group(cls=AliasedGroup, context_settings=CONTEXT_SETTINGS)
-@click.option('-V', '--version', is_flag=True, callback=print_version, expose_value=False, is_eager=True,
-              help='Print the current version number and exit.')
+@click.option(
+    "-V",
+    "--version",
+    is_flag=True,
+    callback=print_version,
+    expose_value=False,
+    is_eager=True,
+    help="Print the current version number and exit.",
+)
 def main():
     pass
 
 
 @main.command()
-@click.argument('spec_file')
-@click.argument('base_module_path', required=False)
-@click.option('--port', '-p', default=5000, type=int, help='Port to listen.')
-@click.option('--host', '-H', type=str, help='Host interface to bind on.')
-@click.option('--wsgi-server', '-w',
-              type=click.Choice(AVAILABLE_SERVERS.keys()),
-              callback=validate_server_requirements,
-              help='Which WSGI server container to use. (deprecated, use --server instead)')
-@click.option('--server', '-s',
-              type=click.Choice(AVAILABLE_SERVERS.keys()),
-              callback=validate_server_requirements,
-              help='Which server container to use.')
-@click.option('--stub',
-              help='Returns status code 501, and `Not Implemented Yet` payload, for '
-              'the endpoints which handlers are not found.',
-              is_flag=True, default=False)
-@click.option('--mock', type=click.Choice(['all', 'notimplemented']),
-              help='Returns example data for all endpoints or for which handlers are not found.')
-@click.option('--hide-spec',
-              help='Hides the API spec in JSON format which is by default available at `/swagger.json`.',
-              is_flag=True, default=False)
-@click.option('--hide-console-ui',
-              help='Hides the the API console UI which is by default available at `/ui`.',
-              is_flag=True, default=False)
-@click.option('--console-ui-url', metavar='URL',
-              help='Personalize what URL path the API console UI will be mounted.')
-@click.option('--console-ui-from', metavar='PATH',
-              help='Path to a customized API console UI dashboard.')
-@click.option('--auth-all-paths',
-              help='Enable authentication to paths not defined in the spec.',
-              is_flag=True, default=False)
-@click.option('--validate-responses',
-              help='Enable validation of response values from operation handlers.',
-              is_flag=True, default=False)
-@click.option('--strict-validation',
-              help='Enable strict validation of request payloads.',
-              is_flag=True, default=False)
-@click.option('--debug', '-d', help='Show debugging information.',
-              is_flag=True, default=False)
-@click.option('--verbose', '-v', help='Show verbose information.', count=True)
-@click.option('--base-path', metavar='PATH',
-              help='Override the basePath in the API spec.')
-@click.option('--app-framework', '-f', default=FLASK_APP,
-              type=click.Choice(AVAILABLE_APPS.keys()),
-              help='The app framework used to run the server')
-def run(spec_file,
-        base_module_path,
-        port,
-        host,
-        wsgi_server,
-        server,
-        stub,
-        mock,
-        hide_spec,
-        hide_console_ui,
-        console_ui_url,
-        console_ui_from,
-        auth_all_paths,
-        validate_responses,
-        strict_validation,
-        debug,
-        verbose,
-        base_path,
-        app_framework):
+@click.argument("spec_file")
+@click.argument("base_module_path", required=False)
+@click.option("--port", "-p", default=5000, type=int, help="Port to listen.")
+@click.option("--host", "-H", type=str, help="Host interface to bind on.")
+@click.option(
+    "--wsgi-server",
+    "-w",
+    type=click.Choice(AVAILABLE_SERVERS.keys()),
+    callback=validate_server_requirements,
+    help="Which WSGI server container to use. (deprecated, use --server instead)",
+)
+@click.option(
+    "--server",
+    "-s",
+    type=click.Choice(AVAILABLE_SERVERS.keys()),
+    callback=validate_server_requirements,
+    help="Which server container to use.",
+)
+@click.option(
+    "--stub",
+    help="Returns status code 501, and `Not Implemented Yet` payload, for "
+    "the endpoints which handlers are not found.",
+    is_flag=True,
+    default=False,
+)
+@click.option(
+    "--mock",
+    type=click.Choice(["all", "notimplemented"]),
+    help="Returns example data for all endpoints or for which handlers are not found.",
+)
+@click.option(
+    "--hide-spec",
+    help="Hides the API spec in JSON format which is by default available at `/swagger.json`.",
+    is_flag=True,
+    default=False,
+)
+@click.option(
+    "--hide-console-ui",
+    help="Hides the the API console UI which is by default available at `/ui`.",
+    is_flag=True,
+    default=False,
+)
+@click.option("--console-ui-url", metavar="URL", help="Personalize what URL path the API console UI will be mounted.")
+@click.option("--console-ui-from", metavar="PATH", help="Path to a customized API console UI dashboard.")
+@click.option(
+    "--auth-all-paths", help="Enable authentication to paths not defined in the spec.", is_flag=True, default=False
+)
+@click.option(
+    "--validate-responses",
+    help="Enable validation of response values from operation handlers.",
+    is_flag=True,
+    default=False,
+)
+@click.option("--strict-validation", help="Enable strict validation of request payloads.", is_flag=True, default=False)
+@click.option("--debug", "-d", help="Show debugging information.", is_flag=True, default=False)
+@click.option("--verbose", "-v", help="Show verbose information.", count=True)
+@click.option("--base-path", metavar="PATH", help="Override the basePath in the API spec.")
+@click.option(
+    "--app-framework",
+    "-f",
+    default=FLASK_APP,
+    type=click.Choice(AVAILABLE_APPS.keys()),
+    help="The app framework used to run the server",
+)
+def run(
+    spec_file,
+    base_module_path,
+    port,
+    host,
+    wsgi_server,
+    server,
+    stub,
+    mock,
+    hide_spec,
+    hide_console_ui,
+    console_ui_url,
+    console_ui_from,
+    auth_all_paths,
+    validate_responses,
+    strict_validation,
+    debug,
+    verbose,
+    base_path,
+    app_framework,
+):
     """
     Runs a server compliant with a OpenAPI/Swagger 2.0 Specification file.
 
     Arguments:
 
     - SPEC_FILE: specification file that describes the server endpoints.
 
     - BASE_MODULE_PATH (optional): filesystem path where the API endpoints handlers are going to be imported from.
     """
     if wsgi_server and server:
-        raise click.BadParameter(
-            "these options are mutually exclusive",
-            param_hint="'wsgi-server' and 'server'"
-        )
+        raise click.BadParameter("these options are mutually exclusive", param_hint="'wsgi-server' and 'server'")
     elif wsgi_server:
         server = wsgi_server
 
     if server is None:
         server = DEFAULT_SERVERS[app_framework]
 
     if app_framework not in AVAILABLE_SERVERS[server]:
-        message = "Invalid server '{}' for app-framework '{}'".format(
-            server, app_framework
-        )
+        message = "Invalid server '{}' for app-framework '{}'".format(server, app_framework)
         raise click.UsageError(message)
 
     if app_framework == AIOHTTP_APP:
         try:
             import aiohttp  # NOQA
         except Exception:
-            fatal_error('aiohttp library is not installed')
+            fatal_error("aiohttp library is not installed")
 
     logging_level = logging.WARN
     if verbose > 0:
         logging_level = logging.INFO
 
     if debug or verbose > 1:
         logging_level = logging.DEBUG
         debug = True
 
     logging.basicConfig(level=logging_level)
 
     spec_file_full_path = path.abspath(spec_file)
     py_module_path = base_module_path or path.dirname(spec_file_full_path)
     sys.path.insert(1, path.abspath(py_module_path))
-    logger.debug(f'Added {py_module_path} to system path.')
+    logger.debug(f"Added {py_module_path} to system path.")
 
     resolver_error = None
     if stub:
         resolver_error = 501
 
     api_extra_args = {}
     if mock:
-        resolver = MockResolver(mock_all=mock == 'all')
-        api_extra_args['resolver'] = resolver
+        resolver = MockResolver(mock_all=mock == "all")
+        api_extra_args["resolver"] = resolver
 
-    app_cls = firetail.utils.get_function_from_name(
-      AVAILABLE_APPS[app_framework]
-    )
+    app_cls = firetail.utils.get_function_from_name(AVAILABLE_APPS[app_framework])
 
     options = {
         "serve_spec": not hide_spec,
         "swagger_path": console_ui_from or None,
         "swagger_ui": not hide_console_ui,
-        "swagger_url": console_ui_url or None
+        "swagger_url": console_ui_url or None,
     }
 
-    app = app_cls(__name__,
-                  debug=debug,
-                  auth_all_paths=auth_all_paths,
-                  options=options)
-
-    app.add_api(spec_file_full_path,
-                base_path=base_path,
-                resolver_error=resolver_error,
-                validate_responses=validate_responses,
-                strict_validation=strict_validation,
-                **api_extra_args)
-
-    app.run(port=port,
-            host=host,
-            server=server,
-            debug=debug)
+    app = app_cls(__name__, debug=debug, auth_all_paths=auth_all_paths, options=options)
+
+    app.add_api(
+        spec_file_full_path,
+        base_path=base_path,
+        resolver_error=resolver_error,
+        validate_responses=validate_responses,
+        strict_validation=strict_validation,
+        **api_extra_args,
+    )
+
+    app.run(port=port, host=host, server=server, debug=debug)
 
 
-if __name__ == '__main__':  # pragma: no cover
+if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `firetail-1.0.8/firetail/decorators/decorator.py` & `firetail-1.0.9/firetail/decorators/decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,31 +5,30 @@
 
 import asyncio
 import functools
 import logging
 
 from ..utils import has_coroutine
 
-logger = logging.getLogger('firetail.decorators.decorator')
+logger = logging.getLogger("firetail.decorators.decorator")
 
 
 class BaseDecorator:
-
     def __call__(self, function):
         """
         :type function: types.FunctionType
         :rtype: types.FunctionType
         """
         return function
 
     def __repr__(self):  # pragma: no cover
         """
         :rtype: str
         """
-        return '<BaseDecorator>'
+        return "<BaseDecorator>"
 
 
 class RequestResponseDecorator(BaseDecorator):
     """Manages the lifecycle of the request internally in Firetail.
     Filter the FiretailRequest instance to return the corresponding
     framework specific object.
     """
@@ -40,32 +39,33 @@
 
     def __call__(self, function):
         """
         :type function: types.FunctionType
         :rtype: types.FunctionType
         """
         if has_coroutine(function, self.api):
+
             @functools.wraps(function)
             async def wrapper(*args, **kwargs):
                 firetail_request = self.api.get_request(*args, **kwargs)
                 while asyncio.iscoroutine(firetail_request):
                     firetail_request = await firetail_request
 
                 firetail_response = function(firetail_request)
                 while asyncio.iscoroutine(firetail_response):
                     firetail_response = await firetail_response
 
-                framework_response = self.api.get_response(firetail_response, self.mimetype,
-                                                           firetail_request)
+                framework_response = self.api.get_response(firetail_response, self.mimetype, firetail_request)
                 while asyncio.iscoroutine(framework_response):
                     framework_response = await framework_response
 
                 return framework_response
 
         else:  # pragma: no cover
+
             @functools.wraps(function)
             def wrapper(*args, **kwargs):
                 request = self.api.get_request(*args, **kwargs)
                 response = function(request)
                 return self.api.get_response(response, self.mimetype, request)
 
         return wrapper
```

### Comparing `firetail-1.0.8/firetail/decorators/metrics.py` & `firetail-1.0.9/firetail/decorators/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 
 from werkzeug.exceptions import HTTPException
 
 from firetail.exceptions import ProblemException
 
 try:
     import uwsgi_metrics
+
     HAS_UWSGI_METRICS = True  # pragma: no cover
 except ImportError:
     uwsgi_metrics = None
     HAS_UWSGI_METRICS = False
 
 
 class UWSGIMetricsCollector:
     def __init__(self, path, method):
         self.path = path
         self.method = method
-        swagger_path = path.strip('/').replace('/', '.').replace('<', '{').replace('>', '}')
-        self.key_suffix = f'{method.upper()}.{swagger_path}'
-        self.prefix = os.getenv('HTTP_METRICS_PREFIX', 'firetail.response')
+        swagger_path = path.strip("/").replace("/", ".").replace("<", "{").replace(">", "}")
+        self.key_suffix = f"{method.upper()}.{swagger_path}"
+        self.prefix = os.getenv("HTTP_METRICS_PREFIX", "firetail.response")
 
     @staticmethod
     def is_available():
         return HAS_UWSGI_METRICS
 
     def __call__(self, function):
         """
@@ -50,12 +51,12 @@
             except ProblemException as prob_e:
                 status = prob_e.status
                 raise prob_e
             finally:
                 end_time_s = time.time()
                 delta_s = end_time_s - start_time_s
                 delta_ms = delta_s * 1000
-                key = f'{status}.{self.key_suffix}'
+                key = f"{status}.{self.key_suffix}"
                 uwsgi_metrics.timer(self.prefix, key, delta_ms)
             return response
 
         return wrapper
```

### Comparing `firetail-1.0.8/firetail/decorators/parameter.py` & `firetail-1.0.9/firetail/decorators/parameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import builtins
 import functools
 import inspect
 import keyword
 import logging
 import re
-from typing import Any
+from typing import Any  # noqa
 
 import inflection
 
 from ..http_facts import FORM_CONTENT_TYPES
 from ..lifecycle import FiretailRequest  # NOQA
 from ..utils import all_json
 
@@ -24,16 +24,15 @@
     Returns the list of variables names of a function and if it
     accepts keyword arguments.
 
     :type function: Callable
     :rtype: tuple[list[str], bool]
     """
     parameters = inspect.signature(function).parameters
-    bound_arguments = [name for name, p in parameters.items()
-                       if p.kind not in (p.VAR_POSITIONAL, p.VAR_KEYWORD)]
+    bound_arguments = [name for name, p in parameters.items() if p.kind not in (p.VAR_POSITIONAL, p.VAR_KEYWORD)]
     has_kwargs = any(p.kind == p.VAR_KEYWORD for p in parameters.values())
     return list(bound_arguments), has_kwargs
 
 
 def snake_and_shadow(name):
     """
     Converts the given name into Pythonic form. Firstly it converts CamelCase names to snake_case. Secondly it looks to
@@ -45,26 +44,23 @@
     snake = inflection.underscore(name)
     if snake in builtins.__dict__ or keyword.iskeyword(snake):
         return f"{snake}_"
     return snake
 
 
 def sanitized(name):
-    return name and re.sub('^[^a-zA-Z_]+', '',
-                           re.sub('[^0-9a-zA-Z_]', '',
-                                  re.sub(r'\[(?!])', '_', name)))
+    return name and re.sub("^[^a-zA-Z_]+", "", re.sub("[^0-9a-zA-Z_]", "", re.sub(r"\[(?!])", "_", name)))
 
 
 def pythonic(name):
     name = name and snake_and_shadow(name)
     return sanitized(name)
 
 
-def parameter_to_arg(operation, function, pythonic_params=False,
-                     pass_context_arg_name=None):
+def parameter_to_arg(operation, function, pythonic_params=False, pass_context_arg_name=None):
     """
     Pass query and body parameters as keyword arguments to handler function.
 
     See (https://github.com/zalando/firetail/issues/59)
     :param operation: The operation being called
     :type operation: firetail.operations.AbstractOperation
     :param pythonic_params: When True CamelCase parameters are converted to snake_case and an underscore is appended to
@@ -78,15 +74,15 @@
 
     sanitize = pythonic if pythonic_params else sanitized
     arguments, has_kwargs = inspect_function_arguments(function)
 
     @functools.wraps(function)
     def wrapper(request):
         # type: (FiretailRequest) -> Any
-        logger.debug('Function Arguments: %s', arguments)
+        logger.debug("Function Arguments: %s", arguments)
         kwargs = {}
 
         if all_json(consumes):
             request_body = request.json
         elif consumes[0] in FORM_CONTENT_TYPES:
             request_body = request.form
         else:
@@ -94,16 +90,17 @@
 
         try:
             query = request.query.to_dict(flat=False)
         except AttributeError:
             query = dict(request.query.items())
 
         kwargs.update(
-            operation.get_arguments(request.path_params, query, request_body,
-                                    request.files, arguments, has_kwargs, sanitize)
+            operation.get_arguments(
+                request.path_params, query, request_body, request.files, arguments, has_kwargs, sanitize
+            )
         )
 
         # optionally convert parameter variable names to un-shadowed, snake_case form
         if pythonic_params:
             kwargs = {snake_and_shadow(k): v for k, v in kwargs.items()}
 
         # add context info (e.g. from security decorator)
```

### Comparing `firetail-1.0.8/firetail/decorators/produces.py` & `firetail-1.0.9/firetail/decorators/produces.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,50 +3,49 @@
 """
 
 import functools
 import logging
 
 from .decorator import BaseDecorator
 
-logger = logging.getLogger('firetail.decorators.produces')
+logger = logging.getLogger("firetail.decorators.produces")
 
 # special marker object to return empty content for any status code
 # e.g. in app method do "return NoContent, 201"
 NoContent = object()
 
 
 class BaseSerializer(BaseDecorator):
-    def __init__(self, mimetype='text/plain'):
+    def __init__(self, mimetype="text/plain"):
         """
         :type mimetype: str
         """
         self.mimetype = mimetype
 
     def __repr__(self):
         """
         :rtype: str
         """
-        return f'<BaseSerializer: {self.mimetype}>'  # pragma: no cover
+        return f"<BaseSerializer: {self.mimetype}>"  # pragma: no cover
 
 
 class Produces(BaseSerializer):
     def __call__(self, function):
         """
         :type function: types.FunctionType
         :rtype: types.FunctionType
         """
 
         @functools.wraps(function)
         def wrapper(request):
             url = request.url
             response = function(request)
-            logger.debug('Returning %s', url,
-                         extra={'url': url, 'mimetype': self.mimetype})
+            logger.debug("Returning %s", url, extra={"url": url, "mimetype": self.mimetype})
             return response
 
         return wrapper
 
     def __repr__(self):
         """
         :rtype: str
         """
-        return f'<Produces: {self.mimetype}>'  # pragma: no cover
+        return f"<Produces: {self.mimetype}>"  # pragma: no cover
```

### Comparing `firetail-1.0.8/firetail/decorators/response.py` & `firetail-1.0.9/firetail/decorators/response.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from jsonschema import ValidationError
 
 from ..exceptions import NonConformingResponseBody, NonConformingResponseHeaders
 from ..utils import all_json, has_coroutine
 from .decorator import BaseDecorator
 from .validation import ResponseBodyValidator
 
-logger = logging.getLogger('firetail.decorators.response')
+logger = logging.getLogger("firetail.decorators.response")
 
 
 class ResponseValidator(BaseDecorator):
     def __init__(self, operation, mimetype, validator=None):
         """
         :type operation: Operation
         :type mimetype: str
@@ -50,71 +50,72 @@
             try:
                 data = self.operation.json_loads(data)
                 v.validate_schema(data, url)
             except ValidationError as e:
                 raise NonConformingResponseBody(message=str(e))
 
         if response_definition and response_definition.get("headers"):
-            required_header_keys = {k for (k, v) in response_definition.get("headers").items()
-                                    if v.get("required", False)}
+            required_header_keys = {
+                k for (k, v) in response_definition.get("headers").items() if v.get("required", False)
+            }
             header_keys = set(headers.keys())
             missing_keys = required_header_keys - header_keys
             if missing_keys:
-                pretty_list = ', '.join(missing_keys)
-                msg = ("Keys in header don't match response specification. "
-                       "Difference: {}").format(pretty_list)
+                pretty_list = ", ".join(missing_keys)
+                msg = ("Keys in header don't match response specification. " "Difference: {}").format(pretty_list)
                 raise NonConformingResponseHeaders(message=msg)
         return True
 
     def is_json_schema_compatible(self, response_schema: dict) -> bool:
         """
         Verify if the specified operation responses are JSON schema
         compatible.
 
         All operations that specify a JSON schema and have content
         type "application/json" or "text/plain" can be validated using
         json_schema package.
         """
         if not response_schema:
             return False
-        return all_json([self.mimetype]) or self.mimetype == 'text/plain'
+        return all_json([self.mimetype]) or self.mimetype == "text/plain"
 
     def __call__(self, function):
         """
         :type function: types.FunctionType
         :rtype: types.FunctionType
         """
 
         def _wrapper(request, response):
-            firetail_response = \
-                self.operation.api.get_firetail_response(response, self.mimetype)
+            firetail_response = self.operation.api.get_firetail_response(response, self.mimetype)
             if not firetail_response.is_streamed:
                 self.validate_response(
-                    firetail_response.body, firetail_response.status_code,
-                    firetail_response.headers, request.url)
+                    firetail_response.body, firetail_response.status_code, firetail_response.headers, request.url
+                )
             else:
                 logger.warning("Skipping response validation for streamed response.")
 
             return response
 
         if has_coroutine(function):
+
             @functools.wraps(function)
             async def wrapper(request):
                 response = function(request)
                 while asyncio.iscoroutine(response):
                     response = await response
 
                 return _wrapper(request, response)
 
         else:  # pragma: no cover
+
             @functools.wraps(function)
             def wrapper(request):
                 response = function(request)
                 return _wrapper(request, response)
 
         return wrapper
 
     def __repr__(self):
         """
         :rtype: str
         """
-        return '<ResponseValidator>'  # pragma: no cover
+        return "<ResponseValidator>"  # pragma: no cover
```

### Comparing `firetail-1.0.8/firetail/decorators/uri_parsing.py` & `firetail-1.0.9/firetail/decorators/uri_parsing.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,17 @@
 import json
 import logging
 import re
 
 from .. import utils
 from .decorator import BaseDecorator
 
-logger = logging.getLogger('firetail.decorators.uri_parsing')
+logger = logging.getLogger("firetail.decorators.uri_parsing")
 
-QUERY_STRING_DELIMITERS = {
-    'spaceDelimited': ' ',
-    'pipeDelimited': '|',
-    'simple': ',',
-    'form': ','
-}
+QUERY_STRING_DELIMITERS = {"spaceDelimited": " ", "pipeDelimited": "|", "simple": ",", "form": ","}
 
 
 class AbstractURIParser(BaseDecorator, metaclass=abc.ABCMeta):
     parsable_parameters = ["query", "path"]
 
     def __init__(self, param_defns, body_defn):
         """
@@ -31,17 +26,15 @@
         both in the path and query according to the spec.
         Some examples include:
         - https://mysite.fake/in/path/1,2,3/            # path parameters
         - https://mysite.fake/?in_query=a,b,c           # simple query params
         - https://mysite.fake/?in_query=a|b|c           # various separators
         - https://mysite.fake/?in_query=a&in_query=b,c  # complex query params
         """
-        self._param_defns = {p["name"]: p
-                             for p in param_defns
-                             if p["in"] in self.parsable_parameters}
+        self._param_defns = {p["name"]: p for p in param_defns if p["in"] in self.parsable_parameters}
         self._body_schema = body_defn.get("schema", {})
         self._body_encoding = body_defn.get("encoding", {})
 
     @property
     @abc.abstractmethod
     def param_defns(self):
         """
@@ -55,38 +48,34 @@
         returns the parameter schemas by name
         """
 
     def __repr__(self):
         """
         :rtype: str
         """
-        return "<{classname}>".format(
-            classname=self.__class__.__name__)  # pragma: no cover
+        return "<{classname}>".format(classname=self.__class__.__name__)  # pragma: no cover
 
     @abc.abstractmethod
     def resolve_form(self, form_data):
-        """ Resolve cases where form parameters are provided multiple times.
-        """
+        """Resolve cases where form parameters are provided multiple times."""
 
     @abc.abstractmethod
     def resolve_query(self, query_data):
-        """ Resolve cases where query parameters are provided multiple times.
-        """
+        """Resolve cases where query parameters are provided multiple times."""
 
     @abc.abstractmethod
     def resolve_path(self, path):
-        """ Resolve cases where path parameters include lists
-        """
+        """Resolve cases where path parameters include lists"""
 
     @abc.abstractmethod
     def _resolve_param_duplicates(self, values, param_defn, _in):
-        """ Resolve cases where query parameters are provided multiple times.
-            For example, if the query string is '?a=1,2,3&a=4,5,6' the value of
-            `a` could be "4,5,6", or "1,2,3" or "1,2,3,4,5,6" depending on the
-            implementation.
+        """Resolve cases where query parameters are provided multiple times.
+        For example, if the query string is '?a=1,2,3&a=4,5,6' the value of
+        `a` could be "4,5,6", or "1,2,3" or "1,2,3,4,5,6" depending on the
+        implementation.
         """
 
     @abc.abstractmethod
     def _split(self, value, param_defn, _in):
         """
         takes a string, a parameter definition, and a parameter type
         and returns an array that has been constructed according to
@@ -105,19 +94,19 @@
             param_schema = self.param_schemas.get(k)
 
             if not (param_defn or param_schema):
                 # rely on validation
                 resolved_param[k] = values
                 continue
 
-            if _in == 'path':
+            if _in == "path":
                 # multiple values in a path is impossible
                 values = [values]
 
-            if param_schema and param_schema['type'] == 'array':
+            if param_schema and param_schema["type"] == "array":
                 # resolve variable re-assignment, handle explode
                 values = self._resolve_param_duplicates(values, param_defn, _in)
                 # handle array styles
                 resolved_param[k] = self._split(values, param_defn, _in)
             else:
                 resolved_param[k] = values[-1]
 
@@ -128,16 +117,15 @@
         :type function: types.FunctionType
         :rtype: types.FunctionType
         """
 
         @functools.wraps(function)
         def wrapper(request):
             def coerce_dict(md):
-                """ MultiDict -> dict of lists
-                """
+                """MultiDict -> dict of lists"""
                 try:
                     return md.to_dict(flat=False)
                 except AttributeError:
                     return dict(md.items())
 
             query = coerce_dict(request.query)
             path_params = coerce_dict(request.path_params)
@@ -149,203 +137,201 @@
             response = function(request)
             return response
 
         return wrapper
 
 
 class OpenAPIURIParser(AbstractURIParser):
-    style_defaults = {"path": "simple", "header": "simple",
-                      "query": "form", "cookie": "form",
-                      "form": "form"}
+    style_defaults = {"path": "simple", "header": "simple", "query": "form", "cookie": "form", "form": "form"}
 
     @property
     def param_defns(self):
         return self._param_defns
 
     @property
     def form_defns(self):
-        return {k: v for k, v in self._body_schema.get('properties', {}).items()}
+        return {k: v for k, v in self._body_schema.get("properties", {}).items()}
 
     @property
     def param_schemas(self):
-        return {k: v.get('schema', {}) for k, v in self.param_defns.items()}
+        return {k: v.get("schema", {}) for k, v in self.param_defns.items()}
 
     def resolve_form(self, form_data):
-        if self._body_schema is None or self._body_schema.get('type') != 'object':
+        if self._body_schema is None or self._body_schema.get("type") != "object":
             return form_data
         for k in form_data:
             encoding = self._body_encoding.get(k, {"style": "form"})
             defn = self.form_defns.get(k, {})
             # TODO support more form encoding styles
-            form_data[k] = \
-                self._resolve_param_duplicates(form_data[k], encoding, 'form')
+            form_data[k] = self._resolve_param_duplicates(form_data[k], encoding, "form")
             if defn and defn["type"] == "array":
-                form_data[k] = self._split(form_data[k], encoding, 'form')
-            elif 'contentType' in encoding and utils.all_json([encoding.get('contentType')]):
+                form_data[k] = self._split(form_data[k], encoding, "form")
+            elif "contentType" in encoding and utils.all_json([encoding.get("contentType")]):
                 form_data[k] = json.loads(form_data[k])
         return form_data
 
     def _make_deep_object(self, k, v):
-        """ consumes keys, value pairs like (a[foo][bar], "baz")
-            returns (a, {"foo": {"bar": "baz"}}}, is_deep_object)
+        """consumes keys, value pairs like (a[foo][bar], "baz")
+        returns (a, {"foo": {"bar": "baz"}}}, is_deep_object)
         """
         root_key = None
         if k in self.param_schemas.keys():
             return k, v, False
         else:
             for key in self.param_schemas.keys():
                 if k.startswith(key) and "[" in k:
-                    root_key = key.replace(k, '')
+                    root_key = key.replace(k, "")
 
         if not root_key:
             root_key = k.split("[", 1)[0]
             if k == root_key:
                 return k, v, False
 
         if not self._is_deep_object_style_param(root_key):
             return k, v, False
 
-        key_path = re.findall(r'\[([^\[\]]*)\]', k)
+        key_path = re.findall(r"\[([^\[\]]*)\]", k)
         root = prev = node = {}
         for k in key_path:
             node[k] = {}
             prev = node
             node = node[k]
         prev[k] = v[0]
         return root_key, [root], True
 
     def _is_deep_object_style_param(self, param_name):
         default_style = self.style_defaults["query"]
-        style = self.param_defns.get(param_name, {}).get('style', default_style)
+        style = self.param_defns.get(param_name, {}).get("style", default_style)
         return style == "deepObject"
 
     def _preprocess_deep_objects(self, query_data):
-        """ deep objects provide a way of rendering nested objects using query
-            parameters.
+        """deep objects provide a way of rendering nested objects using query
+        parameters.
         """
         deep = [self._make_deep_object(k, v) for k, v in query_data.items()]
         root_keys = [k for k, v, is_deep_object in deep]
         ret = dict.fromkeys(root_keys, [{}])
         for k, v, is_deep_object in deep:
             if is_deep_object:
                 ret[k] = [utils.deep_merge(v[0], ret[k][0])]
             else:
                 ret[k] = v
         return ret
 
     def resolve_query(self, query_data):
         query_data = self._preprocess_deep_objects(query_data)
-        return self.resolve_params(query_data, 'query')
+        return self.resolve_params(query_data, "query")
 
     def resolve_path(self, path_data):
-        return self.resolve_params(path_data, 'path')
+        return self.resolve_params(path_data, "path")
 
     @staticmethod
     def _resolve_param_duplicates(values, param_defn, _in):
-        """ Resolve cases where query parameters are provided multiple times.
-            The default behavior is to use the first-defined value.
-            For example, if the query string is '?a=1,2,3&a=4,5,6' the value of
-            `a` would be "4,5,6".
-            However, if 'explode' is 'True' then the duplicate values
-            are concatenated together and `a` would be "1,2,3,4,5,6".
+        """Resolve cases where query parameters are provided multiple times.
+        The default behavior is to use the first-defined value.
+        For example, if the query string is '?a=1,2,3&a=4,5,6' the value of
+        `a` would be "4,5,6".
+        However, if 'explode' is 'True' then the duplicate values
+        are concatenated together and `a` would be "1,2,3,4,5,6".
         """
         default_style = OpenAPIURIParser.style_defaults[_in]
-        style = param_defn.get('style', default_style)
-        delimiter = QUERY_STRING_DELIMITERS.get(style, ',')
-        is_form = (style == 'form')
-        explode = param_defn.get('explode', is_form)
+        style = param_defn.get("style", default_style)
+        delimiter = QUERY_STRING_DELIMITERS.get(style, ",")
+        is_form = style == "form"
+        explode = param_defn.get("explode", is_form)
         if explode:
             return delimiter.join(values)
 
         # default to last defined value
         return values[-1]
 
     @staticmethod
     def _split(value, param_defn, _in):
         default_style = OpenAPIURIParser.style_defaults[_in]
-        style = param_defn.get('style', default_style)
-        delimiter = QUERY_STRING_DELIMITERS.get(style, ',')
+        style = param_defn.get("style", default_style)
+        delimiter = QUERY_STRING_DELIMITERS.get(style, ",")
         return value.split(delimiter)
 
 
 class Swagger2URIParser(AbstractURIParser):
     """
     Adheres to the Swagger2 spec,
     Assumes the the last defined query parameter should be used.
     """
+
     parsable_parameters = ["query", "path", "formData"]
 
     @property
     def param_defns(self):
         return self._param_defns
 
     @property
     def param_schemas(self):
         return self._param_defns  # swagger2 conflates defn and schema
 
     def resolve_form(self, form_data):
-        return self.resolve_params(form_data, 'form')
+        return self.resolve_params(form_data, "form")
 
     def resolve_query(self, query_data):
-        return self.resolve_params(query_data, 'query')
+        return self.resolve_params(query_data, "query")
 
     def resolve_path(self, path_data):
-        return self.resolve_params(path_data, 'path')
+        return self.resolve_params(path_data, "path")
 
     @staticmethod
     def _resolve_param_duplicates(values, param_defn, _in):
-        """ Resolve cases where query parameters are provided multiple times.
-            The default behavior is to use the first-defined value.
-            For example, if the query string is '?a=1,2,3&a=4,5,6' the value of
-            `a` would be "4,5,6".
-            However, if 'collectionFormat' is 'multi' then the duplicate values
-            are concatenated together and `a` would be "1,2,3,4,5,6".
+        """Resolve cases where query parameters are provided multiple times.
+        The default behavior is to use the first-defined value.
+        For example, if the query string is '?a=1,2,3&a=4,5,6' the value of
+        `a` would be "4,5,6".
+        However, if 'collectionFormat' is 'multi' then the duplicate values
+        are concatenated together and `a` would be "1,2,3,4,5,6".
         """
-        if param_defn.get('collectionFormat') == 'multi':
-            return ','.join(values)
+        if param_defn.get("collectionFormat") == "multi":
+            return ",".join(values)
         # default to last defined value
         return values[-1]
 
     @staticmethod
     def _split(value, param_defn, _in):
-        if param_defn.get("collectionFormat") == 'pipes':
-            return value.split('|')
-        return value.split(',')
+        if param_defn.get("collectionFormat") == "pipes":
+            return value.split("|")
+        return value.split(",")
 
 
 class FirstValueURIParser(Swagger2URIParser):
     """
     Adheres to the Swagger2 spec
     Assumes that the first defined query parameter should be used
     """
 
     @staticmethod
     def _resolve_param_duplicates(values, param_defn, _in):
-        """ Resolve cases where query parameters are provided multiple times.
-            The default behavior is to use the first-defined value.
-            For example, if the query string is '?a=1,2,3&a=4,5,6' the value of
-            `a` would be "1,2,3".
-            However, if 'collectionFormat' is 'multi' then the duplicate values
-            are concatenated together and `a` would be "1,2,3,4,5,6".
+        """Resolve cases where query parameters are provided multiple times.
+        The default behavior is to use the first-defined value.
+        For example, if the query string is '?a=1,2,3&a=4,5,6' the value of
+        `a` would be "1,2,3".
+        However, if 'collectionFormat' is 'multi' then the duplicate values
+        are concatenated together and `a` would be "1,2,3,4,5,6".
         """
-        if param_defn.get('collectionFormat') == 'multi':
-            return ','.join(values)
+        if param_defn.get("collectionFormat") == "multi":
+            return ",".join(values)
         # default to first defined value
         return values[0]
 
 
 class AlwaysMultiURIParser(Swagger2URIParser):
     """
     Does not adhere to the Swagger2 spec, but is backwards compatible with
     firetail behavior in version 1.4.2
     """
 
     @staticmethod
     def _resolve_param_duplicates(values, param_defn, _in):
-        """ Resolve cases where query parameters are provided multiple times.
-            The default behavior is to join all provided parameters together.
-            For example, if the query string is '?a=1,2,3&a=4,5,6' the value of
-            `a` would be "1,2,3,4,5,6".
-        """
-        if param_defn.get('collectionFormat') == 'pipes':
-            return '|'.join(values)
-        return ','.join(values)
+        """Resolve cases where query parameters are provided multiple times.
+        The default behavior is to join all provided parameters together.
+        For example, if the query string is '?a=1,2,3&a=4,5,6' the value of
+        `a` would be "1,2,3,4,5,6".
+        """
+        if param_defn.get("collectionFormat") == "pipes":
+            return "|".join(values)
+        return ",".join(values)
```

### Comparing `firetail-1.0.8/firetail/decorators/validation.py` & `firetail-1.0.9/firetail/decorators/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module defines view function decorators to validate request and response parameters and bodies.
 """
 
 import collections
 import copy
 import functools
 import logging
-from typing import AnyStr, Union
+from typing import AnyStr, Union  # noqa
 
 try:
     from importlib.metadata import version
 except ImportError:
     from importlib_metadata import version
 
 from jsonschema import Draft4Validator, ValidationError, draft4_format_checker
@@ -21,27 +21,22 @@
 from ..exceptions import (
     BadRequestProblem,
     ExtraParameterProblem,
     UnsupportedMediaTypeProblem,
 )
 from ..http_facts import FORM_CONTENT_TYPES
 from ..json_schema import Draft4RequestValidator, Draft4ResponseValidator
-from ..lifecycle import FiretailResponse
+from ..lifecycle import FiretailResponse  # noqa
 from ..utils import all_json, boolean, is_json_mimetype, is_null, is_nullable
 
 _jsonschema_3_or_newer = Version(version("jsonschema")) >= Version("3.0.0")
 
-logger = logging.getLogger('firetail.decorators.validation')
+logger = logging.getLogger("firetail.decorators.validation")
 
-TYPE_MAP = {
-    'integer': int,
-    'number': float,
-    'boolean': boolean,
-    'object': dict
-}
+TYPE_MAP = {"integer": int, "number": float, "boolean": boolean, "object": dict}
 
 
 class TypeValidationError(Exception):
     def __init__(self, schema_type, parameter_type, parameter_name):
         """
         Exception raise when type validation fails
 
@@ -56,47 +51,47 @@
 
     def __str__(self):
         msg = "Wrong type, expected '{schema_type}' for {parameter_type} parameter '{parameter_name}'"
         return msg.format(**vars(self))
 
 
 def coerce_type(param, value, parameter_type, parameter_name=None):
-
     def make_type(value, type_literal):
         type_func = TYPE_MAP.get(type_literal)
         return type_func(value)
 
     param_schema = param.get("schema", param)
     if is_nullable(param_schema) and is_null(value):
         return None
 
-    param_type = param_schema.get('type')
-    parameter_name = parameter_name if parameter_name else param.get('name')
+    param_type = param_schema.get("type")
+    parameter_name = parameter_name if parameter_name else param.get("name")
     if param_type == "array":
         converted_params = []
         if parameter_type == "header":
-            value = value.split(',')
+            value = value.split(",")
         for v in value:
             try:
                 converted = make_type(v, param_schema["items"]["type"])
             except (ValueError, TypeError):
                 converted = v
             converted_params.append(converted)
         return converted_params
-    elif param_type == 'object':
-        if param_schema.get('properties'):
+    elif param_type == "object":
+        if param_schema.get("properties"):
+
             def cast_leaves(d, schema):
                 if type(d) is not dict:
                     try:
-                        return make_type(d, schema['type'])
+                        return make_type(d, schema["type"])
                     except (ValueError, TypeError):
                         return d
                 for k, v in d.items():
-                    if k in schema['properties']:
-                        d[k] = cast_leaves(v, schema['properties'][k])
+                    if k in schema["properties"]:
+                        d[k] = cast_leaves(v, schema["properties"][k])
                 return d
 
             return cast_leaves(value, param_schema)
         return value
     else:
         try:
             return make_type(value, param_type)
@@ -110,88 +105,87 @@
     request_params = set(request_params)
     spec_params = set(spec_params)
 
     return request_params.difference(spec_params)
 
 
 class RequestBodyValidator:
-
-    def __init__(self, schema, consumes, api, is_null_value_valid=False, validator=None,
-                 strict_validation=False):
+    def __init__(self, schema, consumes, api, is_null_value_valid=False, validator=None, strict_validation=False):
         """
         :param schema: The schema of the request body
         :param consumes: The list of content types the operation consumes
         :param is_null_value_valid: Flag to indicate if null is accepted as valid value.
         :param validator: Validator class that should be used to validate passed data
                           against API schema. Default is jsonschema.Draft4Validator.
         :type validator: jsonschema.IValidator
         :param strict_validation: Flag indicating if parameters not in spec are allowed
         """
         self.consumes = consumes
         self.schema = schema
-        self.has_default = schema.get('default', False)
+        self.has_default = schema.get("default", False)
         self.is_null_value_valid = is_null_value_valid
         validatorClass = validator or Draft4RequestValidator
         self.validator = validatorClass(schema, format_checker=draft4_format_checker)
         self.api = api
         self.strict_validation = strict_validation
 
     def validate_formdata_parameter_list(self, request):
         request_params = request.form.keys()
-        spec_params = self.schema.get('properties', {}).keys()
+        spec_params = self.schema.get("properties", {}).keys()
         return validate_parameter_list(request_params, spec_params)
 
     def __call__(self, function):
         """
         :type function: types.FunctionType
         :rtype: types.FunctionType
         """
 
         @functools.wraps(function)
         def wrapper(request):
             if all_json(self.consumes):
                 data = request.json
 
-                empty_body = not(request.body or request.form or request.files)
+                empty_body = not (request.body or request.form or request.files)
                 if data is None and not empty_body and not self.is_null_value_valid:
                     try:
                         ctype_is_json = is_json_mimetype(request.headers.get("Content-Type", ""))
                     except ValueError:
                         ctype_is_json = False
 
                     if ctype_is_json:
                         # Content-Type is json but actual body was not parsed
                         raise BadRequestProblem(detail="Request body is not valid JSON")
                     else:
                         # the body has contents that were not parsed as JSON
                         raise UnsupportedMediaTypeProblem(
-                                       detail="Invalid Content-type ({content_type}), expected JSON data".format(
-                                           content_type=request.headers.get("Content-Type", "")
-                                       ))
+                            detail="Invalid Content-type ({content_type}), expected JSON data".format(
+                                content_type=request.headers.get("Content-Type", "")
+                            )
+                        )
 
                 logger.debug("%s validating schema...", request.url)
                 if data is not None or not self.has_default:
                     self.validate_schema(data, request.url)
             elif self.consumes[0] in FORM_CONTENT_TYPES:
                 data = dict(request.form.items()) or (request.body if len(request.body) > 0 else {})
-                data.update(dict.fromkeys(request.files, ''))  # validator expects string..
-                logger.debug('%s validating schema...', request.url)
+                data.update(dict.fromkeys(request.files, ""))  # validator expects string..
+                logger.debug("%s validating schema...", request.url)
 
                 if self.strict_validation:
                     formdata_errors = self.validate_formdata_parameter_list(request)
                     if formdata_errors:
                         raise ExtraParameterProblem(formdata_errors, [])
 
                 if data:
                     props = self.schema.get("properties", {})
                     errs = []
                     for k, param_defn in props.items():
                         if k in data:
                             try:
-                                data[k] = coerce_type(param_defn, data[k], 'requestBody', k)
+                                data[k] = coerce_type(param_defn, data[k], "requestBody", k)
                             except TypeValidationError as e:
                                 errs += [str(e)]
                                 print(errs)
                     if errs:
                         raise BadRequestProblem(detail=errs)
 
                 self.validate_schema(data, request.url)
@@ -199,35 +193,36 @@
             response = function(request)
             return response
 
         return wrapper
 
     @classmethod
     def _error_path_message(cls, exception):
-        error_path = '.'.join(str(item) for item in exception.path)
+        error_path = ".".join(str(item) for item in exception.path)
         error_path_msg = f" - '{error_path}'" if error_path else ""
         return error_path_msg
 
     def validate_schema(self, data, url):
         # type: (dict, AnyStr) -> Union[FiretailResponse, None]
         if self.is_null_value_valid and is_null(data):
             return None
 
         try:
             self.validator.validate(data)
         except ValidationError as exception:
             error_path_msg = self._error_path_message(exception=exception)
             logger.error(
                 "{url} validation error: {error}{error_path_msg}".format(
-                    url=url, error=exception.message,
-                    error_path_msg=error_path_msg),
-                extra={'validator': 'body'})
-            raise BadRequestProblem(detail="{message}{error_path_msg}".format(
-                               message=exception.message,
-                               error_path_msg=error_path_msg))
+                    url=url, error=exception.message, error_path_msg=error_path_msg
+                ),
+                extra={"validator": "body"},
+            )
+            raise BadRequestProblem(
+                detail="{message}{error_path_msg}".format(message=exception.message, error_path_msg=error_path_msg)
+            )
 
         return None
 
 
 class ResponseBodyValidator:
     def __init__(self, schema, validator=None):
         """
@@ -240,32 +235,32 @@
         self.validator = ValidatorClass(schema, format_checker=draft4_format_checker)
 
     def validate_schema(self, data, url):
         # type: (dict, AnyStr) -> Union[FiretailResponse, None]
         try:
             self.validator.validate(data)
         except ValidationError as exception:
-            logger.error("{url} validation error: {error}".format(url=url,
-                                                                  error=exception),
-                         extra={'validator': 'response'})
+            logger.error(
+                "{url} validation error: {error}".format(url=url, error=exception), extra={"validator": "response"}
+            )
             raise exception
 
         return None
 
 
 class ParameterValidator:
     def __init__(self, parameters, api, strict_validation=False):
         """
         :param parameters: List of request parameter dictionaries
         :param api: api that the validator is attached to
         :param strict_validation: Flag indicating if parameters not in spec are allowed
         """
         self.parameters = collections.defaultdict(list)
         for p in parameters:
-            self.parameters[p['in']].append(p)
+            self.parameters[p["in"]].append(p)
 
         self.api = api
         self.strict_validation = strict_validation
 
     @staticmethod
     def validate_parameter(parameter_type, value, param, param_name=None):
         if value is not None:
@@ -274,92 +269,91 @@
 
             try:
                 converted_value = coerce_type(param, value, parameter_type, param_name)
             except TypeValidationError as e:
                 return str(e)
 
             param = copy.deepcopy(param)
-            param = param.get('schema', param)
-            if 'required' in param:
-                del param['required']
+            param = param.get("schema", param)
+            if "required" in param:
+                del param["required"]
             try:
-                if parameter_type == 'formdata' and param.get('type') == 'file':
+                if parameter_type == "formdata" and param.get("type") == "file":
                     if _jsonschema_3_or_newer:
                         extend(
                             Draft4Validator,
                             type_checker=Draft4Validator.TYPE_CHECKER.redefine(
-                                "file",
-                                lambda checker, instance: isinstance(instance, FileStorage)
-                            )
+                                "file", lambda checker, instance: isinstance(instance, FileStorage)
+                            ),
                         )(param, format_checker=draft4_format_checker).validate(converted_value)
                     else:
                         Draft4Validator(
-                            param,
-                            format_checker=draft4_format_checker,
-                            types={'file': FileStorage}).validate(converted_value)
+                            param, format_checker=draft4_format_checker, types={"file": FileStorage}
+                        ).validate(converted_value)
                 else:
-                    Draft4Validator(
-                        param, format_checker=draft4_format_checker).validate(converted_value)
+                    Draft4Validator(param, format_checker=draft4_format_checker).validate(converted_value)
             except ValidationError as exception:
-                debug_msg = 'Error while converting value {converted_value} from param ' \
-                            '{type_converted_value} of type real type {param_type} to the declared type {param}'
+                debug_msg = (
+                    "Error while converting value {converted_value} from param "
+                    "{type_converted_value} of type real type {param_type} to the declared type {param}"
+                )
                 fmt_params = dict(
                     converted_value=str(converted_value),
                     type_converted_value=type(converted_value),
-                    param_type=param.get('type'),
-                    param=param
+                    param_type=param.get("type"),
+                    param=param,
                 )
                 logger.info(debug_msg.format(**fmt_params))
                 return str(exception)
 
-        elif param.get('required'):
+        elif param.get("required"):
             return "Missing {parameter_type} parameter '{param[name]}'".format(**locals())
 
     def validate_query_parameter_list(self, request):
         request_params = request.query.keys()
-        spec_params = [x['name'] for x in self.parameters.get('query', [])]
+        spec_params = [x["name"] for x in self.parameters.get("query", [])]
         return validate_parameter_list(request_params, spec_params)
 
     def validate_formdata_parameter_list(self, request):
         request_params = request.form.keys()
-        if 'formData' in self.parameters:  # Swagger 2:
-            spec_params = [x['name'] for x in self.parameters['formData']]
+        if "formData" in self.parameters:  # Swagger 2:
+            spec_params = [x["name"] for x in self.parameters["formData"]]
         else:  # OAS 3
             return set()
         return validate_parameter_list(request_params, spec_params)
 
     def validate_query_parameter(self, param, request):
         """
         Validate a single query parameter (request.args in Flask)
 
         :type param: dict
         :rtype: str
         """
-        val = request.query.get(param['name'])
-        return self.validate_parameter('query', val, param)
+        val = request.query.get(param["name"])
+        return self.validate_parameter("query", val, param)
 
     def validate_path_parameter(self, param, request):
-        val = request.path_params.get(param['name'].replace('-', '_'))
-        return self.validate_parameter('path', val, param)
+        val = request.path_params.get(param["name"].replace("-", "_"))
+        return self.validate_parameter("path", val, param)
 
     def validate_header_parameter(self, param, request):
-        val = request.headers.get(param['name'])
-        return self.validate_parameter('header', val, param)
+        val = request.headers.get(param["name"])
+        return self.validate_parameter("header", val, param)
 
     def validate_cookie_parameter(self, param, request):
-        val = request.cookies.get(param['name'])
-        return self.validate_parameter('cookie', val, param)
+        val = request.cookies.get(param["name"])
+        return self.validate_parameter("cookie", val, param)
 
     def validate_formdata_parameter(self, param_name, param, request):
-        if param.get('type') == 'file' or param.get('format') == 'binary':
+        if param.get("type") == "file" or param.get("format") == "binary":
             val = request.files.get(param_name)
         else:
             val = request.form.get(param_name)
 
-        return self.validate_parameter('formdata', val, param)
+        return self.validate_parameter("formdata", val, param)
 
     def __call__(self, function):
         """
         :type function: types.FunctionType
         :rtype: types.FunctionType
         """
 
@@ -370,35 +364,35 @@
             if self.strict_validation:
                 query_errors = self.validate_query_parameter_list(request)
                 formdata_errors = self.validate_formdata_parameter_list(request)
 
                 if formdata_errors or query_errors:
                     raise ExtraParameterProblem(formdata_errors, query_errors)
 
-            for param in self.parameters.get('query', []):
+            for param in self.parameters.get("query", []):
                 error = self.validate_query_parameter(param, request)
                 if error:
                     raise BadRequestProblem(detail=error)
 
-            for param in self.parameters.get('path', []):
+            for param in self.parameters.get("path", []):
                 error = self.validate_path_parameter(param, request)
                 if error:
                     raise BadRequestProblem(detail=error)
 
-            for param in self.parameters.get('header', []):
+            for param in self.parameters.get("header", []):
                 error = self.validate_header_parameter(param, request)
                 if error:
                     raise BadRequestProblem(detail=error)
 
-            for param in self.parameters.get('cookie', []):
+            for param in self.parameters.get("cookie", []):
                 error = self.validate_cookie_parameter(param, request)
                 if error:
                     raise BadRequestProblem(detail=error)
 
-            for param in self.parameters.get('formData', []):
+            for param in self.parameters.get("formData", []):
                 error = self.validate_formdata_parameter(param["name"], param, request)
                 if error:
                     raise BadRequestProblem(detail=error)
 
             return function(request)
 
         return wrapper
```

### Comparing `firetail-1.0.8/firetail/exceptions.py` & `firetail-1.0.9/firetail/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
 
 class FiretailException(Exception):
     pass
 
 
 class ProblemException(FiretailException):
-    def __init__(self, status=400, title=None, detail=None, type=None,
-                 instance=None, headers=None, ext=None):
+    def __init__(self, status=400, title=None, detail=None, type=None, instance=None, headers=None, ext=None):
         """
         This exception holds arguments that are going to be passed to the
         `firetail.problem` function to generate a proper response.
         """
         self.status = status
         self.title = title
         self.detail = detail
@@ -28,80 +27,84 @@
         self.instance = instance
         self.headers = headers
         self.ext = ext
 
     def to_problem(self):
         warnings.warn(
             "'to_problem' is planned to be removed in a future release. "
-            "Call firetail.problem.problem(..) instead to maintain the existing error response.", DeprecationWarning)
-        return problem(status=self.status, title=self.title, detail=self.detail,
-                       type=self.type, instance=self.instance, headers=self.headers,
-                       ext=self.ext)
+            "Call firetail.problem.problem(..) instead to maintain the existing error response.",
+            DeprecationWarning,
+        )
+        return problem(
+            status=self.status,
+            title=self.title,
+            detail=self.detail,
+            type=self.type,
+            instance=self.instance,
+            headers=self.headers,
+            ext=self.ext,
+        )
 
 
 class ResolverError(LookupError):
-    def __init__(self, reason='Unknown reason', exc_info=None):
+    def __init__(self, reason="Unknown reason", exc_info=None):
         """
         :param reason: Reason why the resolver failed.
         :type reason: str
         :param exc_info: If specified, gives details of the original exception
             as returned by sys.exc_info()
         :type exc_info: tuple | None
         """
         self.reason = reason
         self.exc_info = exc_info
 
     def __str__(self):  # pragma: no cover
-        return f'<ResolverError: {self.reason}>'
+        return f"<ResolverError: {self.reason}>"
 
     def __repr__(self):  # pragma: no cover
-        return f'<ResolverError: {self.reason}>'
+        return f"<ResolverError: {self.reason}>"
 
 
 class InvalidSpecification(FiretailException, ValidationError):
     pass
 
 
 class NonConformingResponse(ProblemException):
-    def __init__(self, reason='Unknown Reason', message=None):
+    def __init__(self, reason="Unknown Reason", message=None):
         """
         :param reason: Reason why the response did not conform to the specification
         :type reason: str
         """
         super().__init__(status=500, title=reason, detail=message)
         self.reason = reason
         self.message = message
 
     def __str__(self):  # pragma: no cover
-        return f'<NonConformingResponse: {self.reason}>'
+        return f"<NonConformingResponse: {self.reason}>"
 
     def __repr__(self):  # pragma: no cover
-        return f'<NonConformingResponse: {self.reason}>'
+        return f"<NonConformingResponse: {self.reason}>"
 
 
 class AuthenticationProblem(ProblemException):
-
     def __init__(self, status, title, detail):
         super().__init__(status=status, title=title, detail=detail)
 
 
 class ResolverProblem(ProblemException):
-
     def __init__(self, status, title, detail):
         super().__init__(status=status, title=title, detail=detail)
 
 
 class BadRequestProblem(ProblemException):
-
-    def __init__(self, title='Bad Request', detail=None):
+    def __init__(self, title="Bad Request", detail=None):
         super().__init__(status=400, title=title, detail=detail)
 
 
 class UnsupportedMediaTypeProblem(ProblemException):
-
     def __init__(self, title="Unsupported Media Type", detail=None):
         super().__init__(status=415, title=title, detail=detail)
 
 
 class NonConformingResponseBody(NonConformingResponse):
     def __init__(self, message, reason="Response body does not conform to specification"):
         super().__init__(reason=reason, message=message)
@@ -134,14 +137,16 @@
     def __init__(self, formdata_parameters, query_parameters, title=None, detail=None, **kwargs):
         self.extra_formdata = formdata_parameters
         self.extra_query = query_parameters
 
         # This keep backwards compatibility with the old returns
         if detail is None:
             if self.extra_query:
-                detail = "Extra {parameter_type} parameter(s) {extra_params} not in spec"\
-                    .format(parameter_type='query', extra_params=', '.join(self.extra_query))
+                detail = "Extra {parameter_type} parameter(s) {extra_params} not in spec".format(
+                    parameter_type="query", extra_params=", ".join(self.extra_query)
+                )
             elif self.extra_formdata:
-                detail = "Extra {parameter_type} parameter(s) {extra_params} not in spec"\
-                    .format(parameter_type='formData', extra_params=', '.join(self.extra_formdata))
+                detail = "Extra {parameter_type} parameter(s) {extra_params} not in spec".format(
+                    parameter_type="formData", extra_params=", ".join(self.extra_formdata)
+                )
 
         super().__init__(title=title, detail=detail, **kwargs)
```

### Comparing `firetail-1.0.8/firetail/flusher.py` & `firetail-1.0.9/firetail/flusher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import functools
 import logging
 
 
 class FiretailFlusher(logging.Logger):
-
     def __init__(self, logger):
         self.logger = logger
 
     def __call__(self, function):
         @functools.wraps(function)
         def wrapper(*args, **kwargs):
             try:
                 return function(*args, **kwargs)
             except Exception as e:
-                self.logger.exception('call failed: {}'.format(e))
+                self.logger.exception("call failed: {}".format(e))
                 raise
             finally:
                 [h.flush() for h in self.logger.root.handlers]
+
         return wrapper
```

### Comparing `firetail-1.0.8/firetail/handlers.py` & `firetail-1.0.9/firetail/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import traceback
 
 from .exceptions import AuthenticationProblem, FiretailException, ResolverProblem
 from .logger import get_stdout_logger
 from .operations.secure import SecureOperation
 from .sender import FiretailSender
 
-logger = logging.getLogger('firetail.handlers')
+logger = logging.getLogger("firetail.handlers")
 
 RESOLVER_ERROR_ENDPOINT_RANDOM_DIGITS = 6
 
 
 class AuthErrorHandler(SecureOperation):
     """
     Wraps an error with authentication.
@@ -40,28 +40,26 @@
 
     @property
     def function(self):
         """
         Configured error auth handler.
         """
         security_decorator = self.security_decorator
-        logger.debug('... Adding security decorator (%r)', security_decorator, extra=vars(self))
+        logger.debug("... Adding security decorator (%r)", security_decorator, extra=vars(self))
         function = self.handle
         function = security_decorator(function)
         function = self._request_response_decorator(function)
         return function
 
     def handle(self, *args, **kwargs):
         """
         Actual handler for the execution after authentication.
         """
         raise AuthenticationProblem(
-            title=self.exception.name,
-            detail=self.exception.description,
-            status=self.exception.code
+            title=self.exception.name, detail=self.exception.description, status=self.exception.code
         )
 
 
 class ResolverErrorHandler(SecureOperation):
     """
     Handler for responding to ResolverError.
     """
@@ -72,19 +70,15 @@
         super().__init__(api, security, security_definitions)
 
     @property
     def function(self):
         return self.handle
 
     def handle(self, *args, **kwargs):
-        raise ResolverProblem(
-            title='Not Implemented',
-            detail=self.exception.reason,
-            status=self.status_code
-        )
+        raise ResolverProblem(title="Not Implemented", detail=self.exception.reason, status=self.status_code)
 
     @property
     def operation_id(self):
         return "noop"
 
     @property
     def randomize_endpoint(self):
@@ -104,15 +98,14 @@
         logs_drain_timeout=3,
         debug=False,
         backup_logs=True,
         network_timeout=10.0,
         retries_no=4,
         retry_timeout=2,
     ):
-
         if not token and not custom_backend:
             raise FiretailException("firetail Token must be provided")
 
         self.firetail_type = firetail_type
 
         self.firetail_sender = FiretailSender(
             token=token,
@@ -126,15 +119,14 @@
         )
         logging.Handler.__init__(self)
 
     def __del__(self):
         del self.firetail_sender
 
     def extra_fields(self, message):
-
         not_allowed_keys = (
             "args",
             "asctime",
             "created",
             "exc_info",
             "stack_info",
             "exc_text",
```

### Comparing `firetail-1.0.8/firetail/json_schema.py` & `firetail-1.0.9/firetail/json_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,17 +41,15 @@
         with open(filepath) as fh:
             return yaml.load(fh, ExtendedSafeLoader)
 
     @staticmethod
     def _uri_to_path(uri):
         parsed = urllib.parse.urlparse(uri)
         host = "{0}{0}{mnt}{0}".format(os.path.sep, mnt=parsed.netloc)
-        return os.path.abspath(
-            os.path.join(host, urllib.request.url2pathname(parsed.path))
-        )
+        return os.path.abspath(os.path.join(host, urllib.request.url2pathname(parsed.path)))
 
 
 class URLHandler:
     """Handler to resolve url refs."""
 
     def __call__(self, uri):
         response = requests.get(uri)
@@ -59,42 +57,42 @@
 
         data = io.StringIO(response.text)
         with contextlib.closing(data) as fh:
             return yaml.load(fh, ExtendedSafeLoader)
 
 
 default_handlers = {
-    'http': URLHandler(),
-    'https': URLHandler(),
-    'file': FileHandler(),
+    "http": URLHandler(),
+    "https": URLHandler(),
+    "file": FileHandler(),
 }
 
 
 def resolve_refs(spec, store=None, handlers=None):
     """
     Resolve JSON references like {"$ref": <some URI>} in a spec.
     Optionally takes a store, which is a mapping from reference URLs to a
     dereferenced objects. Prepopulating the store can avoid network calls.
     """
     spec = deepcopy(spec)
     store = store or {}
     handlers = handlers or default_handlers
-    resolver = RefResolver('', spec, store, handlers=handlers)
+    resolver = RefResolver("", spec, store, handlers=handlers)
 
     def _do_resolve(node):
-        if isinstance(node, Mapping) and '$ref' in node:
-            path = node['$ref'][2:].split("/")
+        if isinstance(node, Mapping) and "$ref" in node:
+            path = node["$ref"][2:].split("/")
             try:
                 # resolve known references
                 node.update(deep_get(spec, path))
-                del node['$ref']
+                del node["$ref"]
                 return node
             except KeyError:
                 # resolve external references
-                with resolver.resolving(node['$ref']) as resolved:
+                with resolver.resolving(node["$ref"]) as resolved:
                     return resolved
         elif isinstance(node, Mapping):
             for k, v in node.items():
                 node[k] = _do_resolve(v)
         elif isinstance(node, (list, tuple)):
             for i, _ in enumerate(node):
                 node[i] = _do_resolve(node[i])
@@ -104,57 +102,65 @@
     return res
 
 
 def allow_nullable(validation_fn: t.Callable) -> t.Callable:
     """Extend an existing validation function, so it allows nullable values to be null."""
 
     def nullable_validation_fn(validator, to_validate, instance, schema):
-        if instance is None and (schema.get('x-nullable') is True or schema.get('nullable')):
+        if instance is None and (schema.get("x-nullable") is True or schema.get("nullable")):
             return
 
         yield from validation_fn(validator, to_validate, instance, schema)
 
     return nullable_validation_fn
 
 
 def validate_required(validator, required, instance, schema):
     if not validator.is_type(instance, "object"):
         return
 
     for prop in required:
         if prop not in instance:
-            properties = schema.get('properties')
+            properties = schema.get("properties")
             if properties is not None:
                 subschema = properties.get(prop)
                 if subschema is not None:
-                    if 'readOnly' in validator.VALIDATORS and subschema.get('readOnly'):
+                    if "readOnly" in validator.VALIDATORS and subschema.get("readOnly"):
                         continue
-                    if 'writeOnly' in validator.VALIDATORS and subschema.get('writeOnly'):
+                    if "writeOnly" in validator.VALIDATORS and subschema.get("writeOnly"):
                         continue
-                    if 'x-writeOnly' in validator.VALIDATORS and subschema.get('x-writeOnly') is True:
+                    if "x-writeOnly" in validator.VALIDATORS and subschema.get("x-writeOnly") is True:
                         continue
             yield ValidationError("%r is a required property" % prop)
 
 
 def validate_readOnly(validator, ro, instance, schema):
     yield ValidationError("Property is read-only")
 
 
 def validate_writeOnly(validator, wo, instance, schema):
     yield ValidationError("Property is write-only")
 
 
-NullableTypeValidator = allow_nullable(Draft4Validator.VALIDATORS['type'])
-NullableEnumValidator = allow_nullable(Draft4Validator.VALIDATORS['enum'])
+NullableTypeValidator = allow_nullable(Draft4Validator.VALIDATORS["type"])
+NullableEnumValidator = allow_nullable(Draft4Validator.VALIDATORS["enum"])
 
-Draft4RequestValidator = extend(Draft4Validator, {
-                                'type': NullableTypeValidator,
-                                'enum': NullableEnumValidator,
-                                'required': validate_required,
-                                'readOnly': validate_readOnly})
-
-Draft4ResponseValidator = extend(Draft4Validator, {
-                                 'type': NullableTypeValidator,
-                                 'enum': NullableEnumValidator,
-                                 'required': validate_required,
-                                 'writeOnly': validate_writeOnly,
-                                 'x-writeOnly': validate_writeOnly})
+Draft4RequestValidator = extend(
+    Draft4Validator,
+    {
+        "type": NullableTypeValidator,
+        "enum": NullableEnumValidator,
+        "required": validate_required,
+        "readOnly": validate_readOnly,
+    },
+)
+
+Draft4ResponseValidator = extend(
+    Draft4Validator,
+    {
+        "type": NullableTypeValidator,
+        "enum": NullableEnumValidator,
+        "required": validate_required,
+        "writeOnly": validate_writeOnly,
+        "x-writeOnly": validate_writeOnly,
+    },
+)
```

### Comparing `firetail-1.0.8/firetail/jsonifier.py` & `firetail-1.0.9/firetail/jsonifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,63 +5,64 @@
 import datetime
 import json
 import uuid
 
 
 class JSONEncoder(json.JSONEncoder):
     """The default Firetail JSON encoder. Handles extra types compared to the
-    built-in :class:`json.JSONEncoder`.
+    built-in :class:`json.JSONEncoder`. # noqa RST304
 
-    -   :class:`datetime.datetime` and :class:`datetime.date` are
+    -   :class:`datetime.datetime` and :class:`datetime.date` are   # noqa RST304
         serialized to :rfc:`822` strings. This is the same as the HTTP
         date format.
-    -   :class:`uuid.UUID` is serialized to a string.
+    -   :class:`uuid.UUID` is serialized to a string.  # noqa RST304
     """
 
     def default(self, o):
         if isinstance(o, datetime.datetime):
             if o.tzinfo:
                 # eg: '2015-09-25T23:14:42.588601+00:00'
-                return o.isoformat('T')
+                return o.isoformat("T")
             else:
                 # No timezone present - assume UTC.
                 # eg: '2015-09-25T23:14:42.588601Z'
-                return o.isoformat('T') + 'Z'
+                return o.isoformat("T") + "Z"
 
         if isinstance(o, datetime.date):
             return o.isoformat()
 
         if isinstance(o, uuid.UUID):
             return str(o)
 
         return json.JSONEncoder.default(self, o)
 
 
 class Jsonifier:
     """
     Central point to serialize and deserialize to/from JSon in Firetail.
     """
+
     def __init__(self, json_=json, **kwargs):
         """
         :param json_: json library to use. Must have loads() and dumps() method  # NOQA
         :param kwargs: default arguments to pass to json.dumps()
         """
         self.json = json_
         self.dumps_args = kwargs
 
     def dumps(self, data, **kwargs):
-        """ Central point where JSON serialization happens inside
+        """Central point where JSON serialization happens inside
         Firetail.
         """
         for k, v in self.dumps_args.items():
             kwargs.setdefault(k, v)
-        return self.json.dumps(data, **kwargs) + '\n'
+        return self.json.dumps(data, **kwargs) + "\n"
 
     def loads(self, data):
-        """ Central point where JSON deserialization happens inside
+        """Central point where JSON deserialization happens inside
         Firetail.
         """
         if isinstance(data, bytes):
             data = data.decode()
 
         try:
             return self.json.loads(data)
```

### Comparing `firetail-1.0.8/firetail/lifecycle.py` & `firetail-1.0.9/firetail/lifecycle.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,53 +2,51 @@
 This module defines interfaces for requests and responses used in Firetail for authentication,
 validation, serialization, etc.
 """
 
 
 class FiretailRequest:
     """Firetail interface for a request."""
-    def __init__(self,
-                 url,
-                 method,
-                 path_params=None,
-                 query=None,
-                 headers=None,
-                 form=None,
-                 body=None,
-                 json_getter=None,
-                 files=None,
-                 context=None,
-                 cookies=None):
+
+    def __init__(
+        self,
+        url,
+        method,
+        path_params=None,
+        query=None,
+        headers=None,
+        form=None,
+        body=None,
+        json_getter=None,
+        files=None,
+        context=None,
+        cookies=None,
+    ):
         self.url = url
         self.method = method
         self.path_params = path_params or {}
         self.query = query or {}
         self.headers = headers or {}
         self.form = form or {}
         self.body = body
         self.json_getter = json_getter
         self.files = files
         self.context = context if context is not None else {}
         self.cookies = cookies or {}
 
     @property
     def json(self):
-        if not hasattr(self, '_json'):
+        if not hasattr(self, "_json"):
             self._json = self.json_getter()
         return self._json
 
 
 class FiretailResponse:
     """Firetail interface for a response."""
-    def __init__(self,
-                 status_code=200,
-                 mimetype=None,
-                 content_type=None,
-                 body=None,
-                 headers=None,
-                 is_streamed=False):
+
+    def __init__(self, status_code=200, mimetype=None, content_type=None, body=None, headers=None, is_streamed=False):
         self.status_code = status_code
         self.mimetype = mimetype
         self.content_type = content_type
         self.body = body
         self.headers = headers or {}
         self.is_streamed = is_streamed
```

### Comparing `firetail-1.0.8/firetail/logger.py` & `firetail-1.0.9/firetail/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 
 def get_logger(debug):
     return __get_logger(debug, __name__)
 
 
 def get_stdout_logger(debug):
-    stdout_logger = __get_logger(
-        debug, __name__ + '_stdout', logging.StreamHandler(sys.stdout))
+    stdout_logger = __get_logger(debug, __name__ + "_stdout", logging.StreamHandler(sys.stdout))
     stdout_logger.propagate = False
     return stdout_logger
 
 
 def __get_logger(debug, name, handler=None):
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG if debug else logging.INFO)
```

### Comparing `firetail-1.0.8/firetail/middleware/main.py` & `firetail-1.0.9/firetail/middleware/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,39 +5,33 @@
 from starlette.types import ASGIApp, Receive, Scope, Send
 
 from firetail.middleware.base import AppMiddleware
 from firetail.middleware.swagger_ui import SwaggerUIMiddleware
 
 
 class FiretailMiddleware:
-
     default_middlewares = [
         ExceptionMiddleware,
         SwaggerUIMiddleware,
     ]
 
-    def __init__(
-            self,
-            app: ASGIApp,
-            middlewares: t.Optional[t.List[t.Type[ASGIApp]]] = None
-    ):
+    def __init__(self, app: ASGIApp, middlewares: t.Optional[t.List[t.Type[ASGIApp]]] = None):
         """High level Firetail middleware that manages a list o middlewares wrapped around an
         application.
 
         :param app: App to wrap middleware around.
         :param middlewares: List of middlewares to wrap around app. The list should be ordered
                             from outer to inner middleware.
         """
         if middlewares is None:
             middlewares = self.default_middlewares
         self.app, self.apps = self._apply_middlewares(app, middlewares)
 
     @staticmethod
-    def _apply_middlewares(app: ASGIApp, middlewares: t.List[t.Type[ASGIApp]]) \
-            -> t.Tuple[ASGIApp, t.Iterable[ASGIApp]]:
+    def _apply_middlewares(app: ASGIApp, middlewares: t.List[t.Type[ASGIApp]]) -> t.Tuple[ASGIApp, t.Iterable[ASGIApp]]:
         """Apply all middlewares to the provided app.
 
         :param app: App to wrap in middlewares.
         :param middlewares: List of middlewares to wrap around app. The list should be ordered
                             from outer to inner middleware.
 
         :return: App with all middlewares applied.
@@ -45,26 +39,25 @@
         apps = []
         for middleware in reversed(middlewares):
             app = middleware(app)
             apps.append(app)
         return app, reversed(apps)
 
     def add_api(
-            self,
-            specification: t.Union[pathlib.Path, str, dict],
-            base_path: t.Optional[str] = None,
-            arguments: t.Optional[dict] = None,
-            **kwargs
+        self,
+        specification: t.Union[pathlib.Path, str, dict],
+        base_path: t.Optional[str] = None,
+        arguments: t.Optional[dict] = None,
+        **kwargs
     ) -> None:
         """Add an API to the underlying routing middleware based on a OpenAPI spec.
 
         :param specification: OpenAPI spec as dict or path to file.
         :param base_path: Base path where to add this API.
         :param arguments: Jinja arguments to replace in the spec.
         """
         for app in self.apps:
             if isinstance(app, AppMiddleware):
-                app.add_api(specification, base_path=base_path,
-                            arguments=arguments, **kwargs)
+                app.add_api(specification, base_path=base_path, arguments=arguments, **kwargs)
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         await self.app(scope, receive, send)
```

### Comparing `firetail-1.0.8/firetail/middleware/swagger_ui.py` & `firetail-1.0.9/firetail/middleware/swagger_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,46 +13,44 @@
 
 from firetail.apis import AbstractSwaggerUIAPI
 from firetail.jsonifier import JSONEncoder, Jsonifier
 from firetail.utils import yamldumper
 
 from .base import AppMiddleware
 
-logger = logging.getLogger('firetail.middleware.swagger_ui')
+logger = logging.getLogger("firetail.middleware.swagger_ui")
 
 
-_original_scope: ContextVar[Scope] = ContextVar('SCOPE')
+_original_scope: ContextVar[Scope] = ContextVar("SCOPE")
 
 
 class SwaggerUIMiddleware(AppMiddleware):
-
     def __init__(self, app: ASGIApp) -> None:
         """Middleware that hosts a swagger UI.
 
         :param app: app to wrap in middleware.
         """
         self.app = app
         # Set default to pass unknown routes to next app
         self.router = Router(default=self.default_fn)
 
     def add_api(
-            self,
-            specification: t.Union[pathlib.Path, str, dict],
-            base_path: t.Optional[str] = None,
-            arguments: t.Optional[dict] = None,
-            **kwargs
+        self,
+        specification: t.Union[pathlib.Path, str, dict],
+        base_path: t.Optional[str] = None,
+        arguments: t.Optional[dict] = None,
+        **kwargs
     ) -> None:
         """Add an API to the router based on a OpenAPI spec.
 
         :param specification: OpenAPI spec as dict or path to file.
         :param base_path: Base path where to add this API.
         :param arguments: Jinja arguments to replace in the spec.
         """
-        api = SwaggerUIAPI(specification, base_path=base_path, arguments=arguments,
-                           default=self.default_fn, **kwargs)
+        api = SwaggerUIAPI(specification, base_path=base_path, arguments=arguments, default=self.default_fn, **kwargs)
         self.router.mount(api.base_path, app=api.router)
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         _original_scope.set(scope.copy())
         await self.router(scope, receive, send)
 
     async def default_fn(self, _scope: Scope, receive: Receive, send: Send) -> None:
@@ -66,23 +64,20 @@
         This is caused by https://github.com/encode/starlette/issues/1336.
         """
         original_scope = _original_scope.get()
         await self.app(original_scope, receive, send)
 
 
 class SwaggerUIAPI(AbstractSwaggerUIAPI):
-
     def __init__(self, *args, default: ASGIApp, **kwargs):
         self.router = Router(default=default)
 
         super().__init__(*args, **kwargs)
 
-        self._templates = Jinja2Templates(
-            directory=str(self.options.openapi_console_ui_from_dir)
-        )
+        self._templates = Jinja2Templates(directory=str(self.options.openapi_console_ui_from_dir))
 
     @staticmethod
     def normalize_string(string):
         return re.sub(r"[^a-zA-Z0-9]", "_", string.strip("/"))
 
     def _base_path_for_prefix(self, request):
         """
@@ -152,20 +147,18 @@
         """
         Adds swagger ui to {base_path}/ui/
         """
         console_ui_path = self.options.openapi_console_ui_path.strip().rstrip("/")
         logger.debug("Adding swagger-ui: %s%s/", self.base_path, console_ui_path)
 
         for path in (
-                console_ui_path + "/",
-                console_ui_path + "/index.html",
+            console_ui_path + "/",
+            console_ui_path + "/index.html",
         ):
-            self.router.add_route(
-                methods=["GET"], path=path, endpoint=self._get_swagger_ui_home
-            )
+            self.router.add_route(methods=["GET"], path=path, endpoint=self._get_swagger_ui_home)
 
         if self.options.openapi_console_ui_config is not None:
             self.router.add_route(
                 methods=["GET"],
                 path=console_ui_path + "/swagger-ui-config.json",
                 endpoint=self._get_swagger_ui_config,
             )
```

### Comparing `firetail-1.0.8/firetail/mock.py` & `firetail-1.0.9/firetail/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,45 +7,46 @@
 
 from firetail.resolver import Resolution, Resolver, ResolverError
 
 logger = logging.getLogger(__name__)
 
 
 class MockResolver(Resolver):
-
     def __init__(self, mock_all):
         super().__init__()
         self.mock_all = mock_all
         self._operation_id_counter = 1
 
     def resolve(self, operation):
         """
         Mock operation resolver
 
         :type operation: firetail.operations.AbstractOperation
         """
         operation_id = self.resolve_operation_id(operation)
         if not operation_id:
             # just generate an unique operation ID
-            operation_id = f'mock-{self._operation_id_counter}'
+            operation_id = f"mock-{self._operation_id_counter}"
             self._operation_id_counter += 1
 
         mock_func = functools.partial(self.mock_operation, operation=operation)
         if self.mock_all:
             func = mock_func
         else:
             try:
                 func = self.resolve_function_from_operation_id(operation_id)
                 msg = "... Successfully resolved operationId '{}'! Mock is *not* used for this operation.".format(
-                    operation_id)
+                    operation_id
+                )
                 logger.debug(msg)
             except ResolverError as resolution_error:
-                logger.debug('... {}! Mock function is used for this operation.'.format(
-                    resolution_error.reason.capitalize()))
+                logger.debug(
+                    "... {}! Mock function is used for this operation.".format(resolution_error.reason.capitalize())
+                )
                 func = mock_func
         return Resolution(func, operation_id)
 
     def mock_operation(self, operation, *args, **kwargs):
         resp, code = operation.example_response()
         if resp is not None:
             return resp, code
-        return 'No example response was defined.', code
+        return "No example response was defined.", code
```

### Comparing `firetail-1.0.8/firetail/operations/__init__.py` & `firetail-1.0.9/firetail/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `firetail-1.0.8/firetail/operations/abstract.py` & `firetail-1.0.9/firetail/operations/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 from ..decorators.metrics import UWSGIMetricsCollector
 from ..decorators.parameter import parameter_to_arg
 from ..decorators.produces import BaseSerializer, Produces
 from ..decorators.response import ResponseValidator
 from ..decorators.validation import ParameterValidator, RequestBodyValidator
 from ..utils import all_json, is_nullable
 
-logger = logging.getLogger('firetail.operations.abstract')
+logger = logging.getLogger("firetail.operations.abstract")
 
-DEFAULT_MIMETYPE = 'application/json'
+DEFAULT_MIMETYPE = "application/json"
 
 VALIDATOR_MAP = {
-    'parameter': ParameterValidator,
-    'body': RequestBodyValidator,
-    'response': ResponseValidator,
+    "parameter": ParameterValidator,
+    "body": RequestBodyValidator,
+    "response": ResponseValidator,
 }
 
 
 class AbstractOperation(SecureOperation, metaclass=abc.ABCMeta):
 
     """
     An API routes requests to an Operation by a (path, method) pair.
@@ -40,20 +40,32 @@
         @deserialize_function_inputs
         @serialize_function_outputs
         @validate_outputs
         def user_provided_handler_function(important, stuff):
             if important:
                 serious_business(stuff)
     """
-    def __init__(self, api, method, path, operation, resolver,
-                 app_security=None, security_schemes=None,
-                 validate_responses=False, strict_validation=False,
-                 randomize_endpoint=None, validator_map=None,
-                 pythonic_params=False, uri_parser_class=None,
-                 pass_context_arg_name=None):
+
+    def __init__(
+        self,
+        api,
+        method,
+        path,
+        operation,
+        resolver,
+        app_security=None,
+        security_schemes=None,
+        validate_responses=False,
+        strict_validation=False,
+        randomize_endpoint=None,
+        validator_map=None,
+        pythonic_params=False,
+        uri_parser_class=None,
+        pass_context_arg_name=None,
+    ):
         """
         :param api: api that this operation is attached to
         :type api: apis.AbstractAPI
         :param method: HTTP method
         :type method: str
         :param path:
         :type path: str
@@ -183,32 +195,30 @@
 
     @abc.abstractmethod
     def _get_val_from_param(self, value, query_defn):
         """
         Convert input parameters into the correct type
         """
 
-    def _query_args_helper(self, query_defns, query_arguments,
-                           function_arguments, has_kwargs, sanitize):
+    def _query_args_helper(self, query_defns, query_arguments, function_arguments, has_kwargs, sanitize):
         res = {}
         for key, value in query_arguments.items():
             sanitized_key = sanitize(key)
             if not has_kwargs and sanitized_key not in function_arguments:
-                logger.debug("Query Parameter '%s' (sanitized: '%s') not in function arguments",
-                             key, sanitized_key)
+                logger.debug("Query Parameter '%s' (sanitized: '%s') not in function arguments", key, sanitized_key)
             else:
-                logger.debug("Query Parameter '%s' (sanitized: '%s') in function arguments",
-                             key, sanitized_key)
+                logger.debug("Query Parameter '%s' (sanitized: '%s') in function arguments", key, sanitized_key)
                 try:
                     query_defn = query_defns[key]
                 except KeyError:  # pragma: no cover
-                    logger.error("Function argument '%s' (non-sanitized: %s) not defined in specification",
-                                 sanitized_key, key)
+                    logger.error(
+                        "Function argument '%s' (non-sanitized: %s) not defined in specification", sanitized_key, key
+                    )
                 else:
-                    logger.debug('%s is a %s', key, query_defn)
+                    logger.debug("%s is a %s", key, query_defn)
                     res.update({sanitized_key: self._get_val_from_param(value, query_defn)})
         return res
 
     @abc.abstractmethod
     def _get_query_arguments(self, query, arguments, has_kwargs, sanitize):
         """
         extract handler function arguments from the query parameters
@@ -266,40 +276,33 @@
     @abc.abstractmethod
     def body_definition(self):
         """
         The body definition for this operation.
         :rtype: dict
         """
 
-    def get_arguments(self, path_params, query_params, body, files, arguments,
-                      has_kwargs, sanitize):
+    def get_arguments(self, path_params, query_params, body, files, arguments, has_kwargs, sanitize):
         """
         get arguments for handler function
         """
         ret = {}
         ret.update(self._get_path_arguments(path_params, sanitize))
-        ret.update(self._get_query_arguments(query_params, arguments,
-                                             has_kwargs, sanitize))
+        ret.update(self._get_query_arguments(query_params, arguments, has_kwargs, sanitize))
 
         if self.method.upper() in ["PATCH", "POST", "PUT"]:
-            ret.update(self._get_body_argument(body, arguments,
-                                               has_kwargs, sanitize))
+            ret.update(self._get_body_argument(body, arguments, has_kwargs, sanitize))
             ret.update(self._get_file_arguments(files, arguments, has_kwargs))
         return ret
 
-    def response_definition(self, status_code=None,
-                            content_type=None):
+    def response_definition(self, status_code=None, content_type=None):
         """
         response definition for this endpoint
         """
         content_type = content_type or self.get_mimetype()
-        response_definition = self.responses.get(
-            str(status_code),
-            self.responses.get("default", {})
-        )
+        response_definition = self.responses.get(str(status_code), self.responses.get("default", {}))
         return response_definition
 
     @abc.abstractmethod
     def response_schema(self, status_code=None, content_type=None):
         """
         response schema for this endpoint
         """
@@ -352,38 +355,35 @@
     @property
     def function(self):
         """
         Operation function with decorators
 
         :rtype: types.FunctionType
         """
-        function = parameter_to_arg(
-            self, self._resolution.function, self.pythonic_params,
-            self._pass_context_arg_name
-        )
+        function = parameter_to_arg(self, self._resolution.function, self.pythonic_params, self._pass_context_arg_name)
 
         if self.validate_responses:
-            logger.debug('... Response validation enabled.')
+            logger.debug("... Response validation enabled.")
             response_decorator = self.__response_validation_decorator
-            logger.debug('... Adding response decorator (%r)', response_decorator)
+            logger.debug("... Adding response decorator (%r)", response_decorator)
             function = response_decorator(function)
 
         produces_decorator = self.__content_type_decorator
-        logger.debug('... Adding produces decorator (%r)', produces_decorator)
+        logger.debug("... Adding produces decorator (%r)", produces_decorator)
         function = produces_decorator(function)
 
         for validation_decorator in self.__validation_decorators:
             function = validation_decorator(function)
 
         uri_parsing_decorator = self._uri_parsing_decorator
         function = uri_parsing_decorator(function)
 
         # NOTE: the security decorator should be applied last to check auth before anything else :-)
         security_decorator = self.security_decorator
-        logger.debug('... Adding security decorator (%r)', security_decorator)
+        logger.debug("... Adding security decorator (%r)", security_decorator)
         function = security_decorator(function)
 
         function = self._request_response_decorator(function)
 
         if UWSGIMetricsCollector.is_available():  # pragma: no cover
             decorator = UWSGIMetricsCollector(self.path, self.method)
             function = decorator(function)
@@ -403,53 +403,55 @@
 
         A list of MIME types the operation can produce. This overrides the produces definition at the Swagger Object.
         An empty value MAY be used to clear the global definition.
 
         :rtype: types.FunctionType
         """
 
-        logger.debug('... Produces: %s', self.produces, extra=vars(self))
+        logger.debug("... Produces: %s", self.produces, extra=vars(self))
 
         mimetype = self.get_mimetype()
         if all_json(self.produces):  # endpoint will return json
-            logger.debug('... Produces json', extra=vars(self))
+            logger.debug("... Produces json", extra=vars(self))
             # TODO: Refactor this.
             return lambda f: f
 
         elif len(self.produces) == 1:
-            logger.debug('... Produces %s', mimetype, extra=vars(self))
+            logger.debug("... Produces %s", mimetype, extra=vars(self))
             decorator = Produces(mimetype)
             return decorator
 
         else:
             return BaseSerializer()
 
     @property
     def __validation_decorators(self):
         """
         :rtype: types.FunctionType
         """
-        ParameterValidator = self.validator_map['parameter']
-        RequestBodyValidator = self.validator_map['body']
+        ParameterValidator = self.validator_map["parameter"]
+        RequestBodyValidator = self.validator_map["body"]
         if self.parameters:
-            yield ParameterValidator(self.parameters,
-                                     self.api,
-                                     strict_validation=self.strict_validation)
+            yield ParameterValidator(self.parameters, self.api, strict_validation=self.strict_validation)
         if self.body_schema:
-            yield RequestBodyValidator(self.body_schema, self.consumes, self.api,
-                                       is_nullable(self.body_definition),
-                                       strict_validation=self.strict_validation)
+            yield RequestBodyValidator(
+                self.body_schema,
+                self.consumes,
+                self.api,
+                is_nullable(self.body_definition),
+                strict_validation=self.strict_validation,
+            )
 
     @property
     def __response_validation_decorator(self):
         """
         Get a decorator for validating the generated Response.
         :rtype: types.FunctionType
         """
-        ResponseValidator = self.validator_map['response']
+        ResponseValidator = self.validator_map["response"]
         return ResponseValidator(self, self.get_mimetype())
 
     def json_loads(self, data):
         """
         A wrapper for calling the API specific JSON loader.
 
         :param data: The JSON data in textual form.
```

### Comparing `firetail-1.0.8/firetail/operations/openapi.py` & `firetail-1.0.9/firetail/operations/openapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,32 @@
 
 class OpenAPIOperation(AbstractOperation):
 
     """
     A single API operation on a path.
     """
 
-    def __init__(self, api, method, path, operation, resolver, path_parameters=None,
-                 app_security=None, components=None, validate_responses=False,
-                 strict_validation=False, randomize_endpoint=None, validator_map=None,
-                 pythonic_params=False, uri_parser_class=None, pass_context_arg_name=None):
+    def __init__(
+        self,
+        api,
+        method,
+        path,
+        operation,
+        resolver,
+        path_parameters=None,
+        app_security=None,
+        components=None,
+        validate_responses=False,
+        strict_validation=False,
+        randomize_endpoint=None,
+        validator_map=None,
+        pythonic_params=False,
+        uri_parser_class=None,
+        pass_context_arg_name=None,
+    ):
         """
         This class uses the OperationID identify the module and function that will handle the operation
 
         From Swagger Specification:
 
         **OperationID**
 
@@ -68,19 +82,19 @@
         """
         self.components = components or {}
 
         def component_get(oas3_name):
             return self.components.get(oas3_name, {})
 
         # operation overrides globals
-        security_schemes = component_get('securitySchemes')
-        app_security = operation.get('security', app_security)
+        security_schemes = component_get("securitySchemes")
+        app_security = operation.get("security", app_security)
         uri_parser_class = uri_parser_class or OpenAPIURIParser
 
-        self._router_controller = operation.get('x-openapi-router-controller')
+        self._router_controller = operation.get("x-openapi-router-controller")
 
         super().__init__(
             api=api,
             method=method,
             path=path,
             operation=operation,
             resolver=resolver,
@@ -88,64 +102,64 @@
             security_schemes=security_schemes,
             validate_responses=validate_responses,
             strict_validation=strict_validation,
             randomize_endpoint=randomize_endpoint,
             validator_map=validator_map,
             pythonic_params=pythonic_params,
             uri_parser_class=uri_parser_class,
-            pass_context_arg_name=pass_context_arg_name
+            pass_context_arg_name=pass_context_arg_name,
         )
 
         self._definitions_map = {
-            'components': {
-                'schemas': component_get('schemas'),
-                'examples': component_get('examples'),
-                'requestBodies': component_get('requestBodies'),
-                'parameters': component_get('parameters'),
-                'securitySchemes': component_get('securitySchemes'),
-                'responses': component_get('responses'),
-                'headers': component_get('headers'),
+            "components": {
+                "schemas": component_get("schemas"),
+                "examples": component_get("examples"),
+                "requestBodies": component_get("requestBodies"),
+                "parameters": component_get("parameters"),
+                "securitySchemes": component_get("securitySchemes"),
+                "responses": component_get("responses"),
+                "headers": component_get("headers"),
             }
         }
 
-        self._request_body = operation.get('requestBody', {})
+        self._request_body = operation.get("requestBody", {})
 
-        self._parameters = operation.get('parameters', [])
+        self._parameters = operation.get("parameters", [])
         if path_parameters:
             self._parameters += path_parameters
 
-        self._responses = operation.get('responses', {})
+        self._responses = operation.get("responses", {})
 
         # TODO figure out how to support multiple mimetypes
         # NOTE we currently just combine all of the possible mimetypes,
         #      but we need to refactor to support mimetypes by response code
         response_content_types = []
         for _, defn in self._responses.items():
-            response_content_types += defn.get('content', {}).keys()
-        self._produces = response_content_types or ['application/json']
+            response_content_types += defn.get("content", {}).keys()
+        self._produces = response_content_types or ["application/json"]
 
-        request_content = self._request_body.get('content', {})
-        self._consumes = list(request_content.keys()) or ['application/json']
+        request_content = self._request_body.get("content", {})
+        self._consumes = list(request_content.keys()) or ["application/json"]
 
-        logger.debug('consumes: %s' % self.consumes)
-        logger.debug('produces: %s' % self.produces)
+        logger.debug("consumes: %s" % self.consumes)
+        logger.debug("produces: %s" % self.produces)
 
     @classmethod
     def from_spec(cls, spec, api, path, method, resolver, *args, **kwargs):
         return cls(
             api,
             method,
             path,
             spec.get_operation(path, method),
             resolver=resolver,
             path_parameters=spec.get_path_params(path),
             app_security=spec.security,
             components=spec.components,
             *args,
-            **kwargs
+            **kwargs,
         )
 
     @property
     def request_body(self):
         return self._request_body
 
     @property
@@ -158,139 +172,130 @@
 
     @property
     def produces(self):
         return self._produces
 
     def with_definitions(self, schema):
         if self.components:
-            schema['schema']['components'] = self.components
+            schema["schema"]["components"] = self.components
         return schema
 
     def response_schema(self, status_code=None, content_type=None):
-        response_definition = self.response_definition(
-            status_code, content_type
-        )
+        response_definition = self.response_definition(status_code, content_type)
         content_definition = response_definition.get("content", response_definition)
         content_definition = content_definition.get(content_type, content_definition)
         if "schema" in content_definition:
             return self.with_definitions(content_definition).get("schema", {})
         return {}
 
     def example_response(self, status_code=None, content_type=None):
         """
         Returns example response from spec
         """
         # simply use the first/lowest status code, this is probably 200 or 201
         status_code = status_code or sorted(self._responses.keys())[0]
 
         content_type = content_type or self.get_mimetype()
-        examples_path = [str(status_code), 'content', content_type, 'examples']
-        example_path = [str(status_code), 'content', content_type, 'example']
-        schema_example_path = [
-            str(status_code), 'content', content_type, 'schema', 'example'
-        ]
-        schema_path = [str(status_code), 'content', content_type, 'schema']
+        examples_path = [str(status_code), "content", content_type, "examples"]
+        example_path = [str(status_code), "content", content_type, "example"]
+        schema_example_path = [str(status_code), "content", content_type, "schema", "example"]
+        schema_path = [str(status_code), "content", content_type, "schema"]
 
         try:
             status_code = int(status_code)
         except ValueError:
             status_code = 200
         try:
             # TODO also use example header?
-            return (
-                list(deep_get(self._responses, examples_path).values())[0]['value'],
-                status_code
-            )
+            return (list(deep_get(self._responses, examples_path).values())[0]["value"], status_code)
         except (KeyError, IndexError):
             pass
         try:
             return (deep_get(self._responses, example_path), status_code)
         except KeyError:
             pass
         try:
-            return (deep_get(self._responses, schema_example_path),
-                    status_code)
+            return (deep_get(self._responses, schema_example_path), status_code)
         except KeyError:
             pass
 
         try:
-            return (self._nested_example(deep_get(self._responses, schema_path)),
-                    status_code)
+            return (self._nested_example(deep_get(self._responses, schema_path)), status_code)
         except KeyError:
             return (None, status_code)
 
     def _nested_example(self, schema):
         try:
             return schema["example"]
         except KeyError:
             pass
         try:
             # Recurse if schema is an object
-            return {key: self._nested_example(value)
-                    for (key, value) in schema["properties"].items()}
+            return {key: self._nested_example(value) for (key, value) in schema["properties"].items()}
         except KeyError:
             pass
         try:
             # Recurse if schema is an array
             return [self._nested_example(schema["items"])]
         except KeyError:
             raise
 
     def get_path_parameter_types(self):
         types = {}
         path_parameters = (p for p in self.parameters if p["in"] == "path")
         for path_defn in path_parameters:
             path_schema = path_defn["schema"]
-            if path_schema.get('type') == 'string' and path_schema.get('format') == 'path':
+            if path_schema.get("type") == "string" and path_schema.get("format") == "path":
                 # path is special case for type 'string'
-                path_type = 'path'
+                path_type = "path"
             else:
-                path_type = path_schema.get('type')
-            types[path_defn['name']] = path_type
+                path_type = path_schema.get("type")
+            types[path_defn["name"]] = path_type
         return types
 
     @property
     def body_schema(self):
         """
         The body schema definition for this operation.
         """
-        return self.body_definition.get('schema', {})
+        return self.body_definition.get("schema", {})
 
     @property
     def body_definition(self):
         """
         The body complete definition for this operation.
 
         **There can be one "body" parameter at most.**
 
         :rtype: dict
         """
         if self._request_body:
             if len(self.consumes) > 1:
-                logger.warning(
-                    'this operation accepts multiple content types, using %s',
-                    self.consumes[0])
-            res = self._request_body.get('content', {}).get(self.consumes[0], {})
+                logger.warning("this operation accepts multiple content types, using %s", self.consumes[0])
+            res = self._request_body.get("content", {}).get(self.consumes[0], {})
             return self.with_definitions(res)
         return {}
 
     def _get_body_argument(self, body, arguments, has_kwargs, sanitize):
         if len(arguments) <= 0 and not has_kwargs:
             return {}
 
         # get the deprecated name from the body-schema for legacy firetail compat
-        x_body_name = sanitize(self.body_schema.get('x-body-name'))
+        x_body_name = sanitize(self.body_schema.get("x-body-name"))
 
         if x_body_name:
-            warnings.warn('x-body-name within the requestBody schema will be deprecated in the '
-                          'next major version. It should be provided directly under '
-                          'the requestBody instead.', DeprecationWarning)
+            warnings.warn(
+                "x-body-name within the requestBody schema will be deprecated in the "
+                "next major version. It should be provided directly under "
+                "the requestBody instead.",
+                DeprecationWarning,
+            )
 
         # prefer the x-body-name as an extension of requestBody, fallback to deprecated schema name, default 'body'
-        x_body_name = sanitize(self.request_body.get('x-body-name', x_body_name or 'body'))
+        x_body_name = sanitize(self.request_body.get("x-body-name", x_body_name or "body"))
 
         if self.consumes[0] in FORM_CONTENT_TYPES:
             result = self._get_body_argument_form(body)
         else:
             result = self._get_body_argument_json(body)
 
         if x_body_name in arguments or has_kwargs:
@@ -300,24 +305,23 @@
     def _get_body_argument_json(self, body):
         # if the body came in null, and the schema says it can be null, we decide
         # to include no value for the body argument, rather than the default body
         if is_nullable(self.body_schema) and is_null(body):
             return None
 
         if body is None:
-            default_body = self.body_schema.get('default', {})
+            default_body = self.body_schema.get("default", {})
             return deepcopy(default_body)
 
         return body
 
     def _get_body_argument_form(self, body):
         # now determine the actual value for the body (whether it came in or is default)
-        default_body = self.body_schema.get('default', {})
-        body_props = {k: {"schema": v} for k, v
-                      in self.body_schema.get("properties", {}).items()}
+        default_body = self.body_schema.get("default", {})
+        body_props = {k: {"schema": v} for k, v in self.body_schema.get("properties", {}).items()}
 
         # by OpenAPI specification `additionalProperties` defaults to `true`
         # see: https://github.com/OAI/OpenAPI-Specification/blame/3.0.2/versions/3.0.2.md#L2305
         additional_props = self.body_schema.get("additionalProperties", True)
 
         body_arg = deepcopy(default_body)
         body_arg.update(body or {})
@@ -351,22 +355,21 @@
                 if additional_props_defn is not None:
                     value = self._get_val_from_param(value, additional_props_defn)
                 res[key] = value
 
         return res
 
     def _build_default_obj_recursive(self, _properties, res):
-        """ takes disparate and nested default keys, and builds up a default object
-        """
+        """takes disparate and nested default keys, and builds up a default object"""
         for key, prop in _properties.items():
-            if 'default' in prop and key not in res:
-                res[key] = copy(prop['default'])
-            elif prop.get('type') == 'object' and 'properties' in prop:
+            if "default" in prop and key not in res:
+                res[key] = copy(prop["default"])
+            elif prop.get("type") == "object" and "properties" in prop:
                 res.setdefault(key, {})
-                res[key] = self._build_default_obj_recursive(prop['properties'], res[key])
+                res[key] = self._build_default_obj_recursive(prop["properties"], res[key])
         return res
 
     def _get_default_obj(self, schema):
         try:
             return deepcopy(schema["default"])
         except KeyError:
             _properties = schema.get("properties", {})
@@ -381,23 +384,20 @@
                 else:
                     defaults[k] = v["schema"]["default"]
             except KeyError:
                 pass
         return defaults
 
     def _get_query_arguments(self, query, arguments, has_kwargs, sanitize):
-        query_defns = {p["name"]: p
-                       for p in self.parameters
-                       if p["in"] == "query"}
+        query_defns = {p["name"]: p for p in self.parameters if p["in"] == "query"}
         default_query_params = self._get_query_defaults(query_defns)
 
         query_arguments = deepcopy(default_query_params)
         query_arguments = deep_merge(query_arguments, query)
-        return self._query_args_helper(query_defns, query_arguments,
-                                       arguments, has_kwargs, sanitize)
+        return self._query_args_helper(query_defns, query_arguments, arguments, has_kwargs, sanitize)
 
     def _get_val_from_param(self, value, query_defn):
         query_schema = query_defn["schema"]
 
         if is_nullable(query_schema) and is_null(value):
             return None
```

### Comparing `firetail-1.0.8/firetail/operations/secure.py` & `firetail-1.0.9/firetail/operations/secure.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 import functools
 import logging
 
 from ..decorators.decorator import RequestResponseDecorator
 
 logger = logging.getLogger("firetail.operations.secure")
 
-DEFAULT_MIMETYPE = 'application/json'
+DEFAULT_MIMETYPE = "application/json"
 
 
 class SecureOperation:
-
     def __init__(self, api, security, security_schemes):
         """
         :param security: list of security rules the application uses by default
         :type security: list
         :param security_definitions: `Security Definitions Object
             <https://github.com/swagger-api/swagger-spec/blob/master/versions/2.0.md#security-definitions-object>`_
         :type security_definitions: dict
@@ -66,92 +65,97 @@
         Lists the required security schemes to execute this operation. The object can have multiple security schemes
         declared in it which are all required (that is, there is a logical AND between the schemes).
 
         The name used for each property **MUST** correspond to a security scheme declared in the Security Definitions.
 
         :rtype: types.FunctionType
         """
-        logger.debug('... Security: %s', self.security, extra=vars(self))
+        logger.debug("... Security: %s", self.security, extra=vars(self))
         if not self.security:
             return self._api.security_handler_factory.security_passthrough
 
         auth_funcs = []
         for security_req in self.security:
             if not security_req:
                 auth_funcs.append(self._api.security_handler_factory.verify_none())
                 continue
 
             sec_req_funcs = {}
             oauth = False
             for scheme_name, required_scopes in security_req.items():
                 security_scheme = self.security_schemes[scheme_name]
 
-                if security_scheme['type'] == 'oauth2':
+                if security_scheme["type"] == "oauth2":
                     if oauth:
-                        logger.warning("... multiple OAuth2 security schemes in AND fashion not supported", extra=vars(self))
+                        logger.warning(
+                            "... multiple OAuth2 security schemes in AND fashion not supported", extra=vars(self)
+                        )
                         break
                     oauth = True
                     token_info_func = self._api.security_handler_factory.get_tokeninfo_func(security_scheme)
                     scope_validate_func = self._api.security_handler_factory.get_scope_validate_func(security_scheme)
                     if not token_info_func:
                         logger.warning("... x-tokenInfoFunc missing", extra=vars(self))
                         break
 
                     sec_req_funcs[scheme_name] = self._api.security_handler_factory.verify_oauth(
-                        token_info_func, scope_validate_func, required_scopes)
+                        token_info_func, scope_validate_func, required_scopes
+                    )
 
                 # Swagger 2.0
-                elif security_scheme['type'] == 'basic':
+                elif security_scheme["type"] == "basic":
                     basic_info_func = self._api.security_handler_factory.get_basicinfo_func(security_scheme)
                     if not basic_info_func:
                         logger.warning("... x-basicInfoFunc missing", extra=vars(self))
                         break
 
                     sec_req_funcs[scheme_name] = self._api.security_handler_factory.verify_basic(basic_info_func)
 
                 # OpenAPI 3.0.0
-                elif security_scheme['type'] == 'http':
-                    scheme = security_scheme['scheme'].lower()
-                    if scheme == 'basic':
+                elif security_scheme["type"] == "http":
+                    scheme = security_scheme["scheme"].lower()
+                    if scheme == "basic":
                         basic_info_func = self._api.security_handler_factory.get_basicinfo_func(security_scheme)
                         if not basic_info_func:
                             logger.warning("... x-basicInfoFunc missing", extra=vars(self))
                             break
 
                         sec_req_funcs[scheme_name] = self._api.security_handler_factory.verify_basic(basic_info_func)
-                    elif scheme == 'bearer':
+                    elif scheme == "bearer":
                         bearer_info_func = self._api.security_handler_factory.get_bearerinfo_func(security_scheme)
                         if not bearer_info_func:
                             logger.warning("... x-bearerInfoFunc missing", extra=vars(self))
                             break
                         sec_req_funcs[scheme_name] = self._api.security_handler_factory.verify_bearer(bearer_info_func)
                     else:
                         logger.warning("... Unsupported http authorization scheme %s" % scheme, extra=vars(self))
                         break
 
-                elif security_scheme['type'] == 'apiKey':
-                    scheme = security_scheme.get('x-authentication-scheme', '').lower()
-                    if scheme == 'bearer':
+                elif security_scheme["type"] == "apiKey":
+                    scheme = security_scheme.get("x-authentication-scheme", "").lower()
+                    if scheme == "bearer":
                         bearer_info_func = self._api.security_handler_factory.get_bearerinfo_func(security_scheme)
                         if not bearer_info_func:
                             logger.warning("... x-bearerInfoFunc missing", extra=vars(self))
                             break
                         sec_req_funcs[scheme_name] = self._api.security_handler_factory.verify_bearer(bearer_info_func)
                     else:
                         apikey_info_func = self._api.security_handler_factory.get_apikeyinfo_func(security_scheme)
                         if not apikey_info_func:
                             logger.warning("... x-apikeyInfoFunc missing", extra=vars(self))
                             break
 
                         sec_req_funcs[scheme_name] = self._api.security_handler_factory.verify_api_key(
-                            apikey_info_func, security_scheme['in'], security_scheme['name']
+                            apikey_info_func, security_scheme["in"], security_scheme["name"]
                         )
 
                 else:
-                    logger.warning("... Unsupported security scheme type %s" % security_scheme['type'], extra=vars(self))
+                    logger.warning(
+                        "... Unsupported security scheme type %s" % security_scheme["type"], extra=vars(self)
+                    )
                     break
             else:
                 # No break encountered: no missing funcs
                 if len(sec_req_funcs) == 1:
                     (func,) = sec_req_funcs.values()
                     auth_funcs.append(func)
                 else:
```

### Comparing `firetail-1.0.8/firetail/operations/swagger2.py` & `firetail-1.0.9/firetail/operations/swagger2.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,37 @@
     to the API. A Swagger2Operation is plugged into the API with the provided
     (path, method) pair. It resolves the handler function for this operation
     with the provided resolver, and wraps the handler function with multiple
     decorators that provide security, validation, serialization,
     and deserialization.
     """
 
-    def __init__(self, api, method, path, operation, resolver, app_produces, app_consumes,
-                 path_parameters=None, app_security=None, security_definitions=None,
-                 definitions=None, parameter_definitions=None,
-                 response_definitions=None, validate_responses=False, strict_validation=False,
-                 randomize_endpoint=None, validator_map=None, pythonic_params=False,
-                 uri_parser_class=None, pass_context_arg_name=None):
+    def __init__(
+        self,
+        api,
+        method,
+        path,
+        operation,
+        resolver,
+        app_produces,
+        app_consumes,
+        path_parameters=None,
+        app_security=None,
+        security_definitions=None,
+        definitions=None,
+        parameter_definitions=None,
+        response_definitions=None,
+        validate_responses=False,
+        strict_validation=False,
+        randomize_endpoint=None,
+        validator_map=None,
+        pythonic_params=False,
+        uri_parser_class=None,
+        pass_context_arg_name=None,
+    ):
         """
         :param api: api that this operation is attached to
         :type api: apis.AbstractAPI
         :param method: HTTP method
         :type method: str
         :param path: relative path to this operation
         :type path: str
@@ -74,18 +91,18 @@
         :type pythonic_params: bool
         :param uri_parser_class: class to use for uri parsing
         :type uri_parser_class: AbstractURIParser
         :param pass_context_arg_name: If not None will try to inject the request context to the function using this
             name.
         :type pass_context_arg_name: str|None
         """
-        app_security = operation.get('security', app_security)
+        app_security = operation.get("security", app_security)
         uri_parser_class = uri_parser_class or Swagger2URIParser
 
-        self._router_controller = operation.get('x-swagger-router-controller')
+        self._router_controller = operation.get("x-swagger-router-controller")
 
         super().__init__(
             api=api,
             method=method,
             path=path,
             operation=operation,
             resolver=resolver,
@@ -93,37 +110,37 @@
             security_schemes=security_definitions,
             validate_responses=validate_responses,
             strict_validation=strict_validation,
             randomize_endpoint=randomize_endpoint,
             validator_map=validator_map,
             pythonic_params=pythonic_params,
             uri_parser_class=uri_parser_class,
-            pass_context_arg_name=pass_context_arg_name
+            pass_context_arg_name=pass_context_arg_name,
         )
 
-        self._produces = operation.get('produces', app_produces)
-        self._consumes = operation.get('consumes', app_consumes)
+        self._produces = operation.get("produces", app_produces)
+        self._consumes = operation.get("consumes", app_consumes)
 
         self.definitions = definitions or {}
 
         self.definitions_map = {
-            'definitions': self.definitions,
-            'parameters': parameter_definitions,
-            'responses': response_definitions
+            "definitions": self.definitions,
+            "parameters": parameter_definitions,
+            "responses": response_definitions,
         }
 
-        self._parameters = operation.get('parameters', [])
+        self._parameters = operation.get("parameters", [])
         if path_parameters:
             self._parameters += path_parameters
 
-        self._responses = operation.get('responses', {})
+        self._responses = operation.get("responses", {})
         logger.debug(self._responses)
 
-        logger.debug('consumes: %s', self.consumes)
-        logger.debug('produces: %s', self.produces)
+        logger.debug("consumes: %s", self.consumes)
+        logger.debug("produces: %s", self.produces)
 
     @classmethod
     def from_spec(cls, spec, api, path, method, resolver, *args, **kwargs):
         return cls(
             api,
             method,
             path,
@@ -153,133 +170,115 @@
     def produces(self):
         return self._produces
 
     def get_path_parameter_types(self):
         types = {}
         path_parameters = (p for p in self.parameters if p["in"] == "path")
         for path_defn in path_parameters:
-            if path_defn.get('type') == 'string' and path_defn.get('format') == 'path':
+            if path_defn.get("type") == "string" and path_defn.get("format") == "path":
                 # path is special case for type 'string'
-                path_type = 'path'
+                path_type = "path"
             else:
-                path_type = path_defn.get('type')
-            types[path_defn['name']] = path_type
+                path_type = path_defn.get("type")
+            types[path_defn["name"]] = path_type
         return types
 
     def with_definitions(self, schema):
         if "schema" in schema:
-            schema['schema']['definitions'] = self.definitions
+            schema["schema"]["definitions"] = self.definitions
         return schema
 
     def response_schema(self, status_code=None, content_type=None):
-        response_definition = self.response_definition(
-            status_code, content_type
-        )
+        response_definition = self.response_definition(status_code, content_type)
         return self.with_definitions(response_definition.get("schema", {}))
 
     def example_response(self, status_code=None, *args, **kwargs):
         """
         Returns example response from spec
         """
         # simply use the first/lowest status code, this is probably 200 or 201
         status_code = status_code or sorted(self._responses.keys())[0]
-        examples_path = [str(status_code), 'examples']
-        schema_example_path = [str(status_code), 'schema', 'example']
-        schema_path = [str(status_code), 'schema']
+        examples_path = [str(status_code), "examples"]
+        schema_example_path = [str(status_code), "schema", "example"]
+        schema_path = [str(status_code), "schema"]
 
         try:
             status_code = int(status_code)
         except ValueError:
             status_code = 200
         try:
-            return (
-                list(deep_get(self._responses, examples_path).values())[0],
-                status_code
-            )
+            return (list(deep_get(self._responses, examples_path).values())[0], status_code)
         except KeyError:
             pass
         try:
-            return (deep_get(self._responses, schema_example_path),
-                    status_code)
+            return (deep_get(self._responses, schema_example_path), status_code)
         except KeyError:
             pass
 
         try:
-            return (self._nested_example(deep_get(self._responses, schema_path)),
-                    status_code)
+            return (self._nested_example(deep_get(self._responses, schema_path)), status_code)
         except KeyError:
             return (None, status_code)
 
     def _nested_example(self, schema):
         try:
             return schema["example"]
         except KeyError:
             pass
         try:
             # Recurse if schema is an object
-            return {key: self._nested_example(value)
-                    for (key, value) in schema["properties"].items()}
+            return {key: self._nested_example(value) for (key, value) in schema["properties"].items()}
         except KeyError:
             pass
         try:
             # Recurse if schema is an array
             return [self._nested_example(schema["items"])]
         except KeyError:
             raise
 
     @property
     def body_schema(self):
         """
         The body schema definition for this operation.
         """
-        return self.with_definitions(self.body_definition).get('schema', {})
+        return self.with_definitions(self.body_definition).get("schema", {})
 
     @property
     def body_definition(self):
         """
         The body complete definition for this operation.
 
         **There can be one "body" parameter at most.**
 
         :rtype: dict
         """
-        body_parameters = [p for p in self.parameters if p['in'] == 'body']
+        body_parameters = [p for p in self.parameters if p["in"] == "body"]
         if len(body_parameters) > 1:
             raise InvalidSpecification(
-                "{method} {path} There can be one 'body' parameter at most".format(
-                    method=self.method,
-                    path=self.path))
+                "{method} {path} There can be one 'body' parameter at most".format(method=self.method, path=self.path)
+            )
         return body_parameters[0] if body_parameters else {}
 
     def _get_query_arguments(self, query, arguments, has_kwargs, sanitize):
-        query_defns = {p["name"]: p
-                       for p in self.parameters
-                       if p["in"] == "query"}
-        default_query_params = {k: v['default']
-                                for k, v in query_defns.items()
-                                if 'default' in v}
+        query_defns = {p["name"]: p for p in self.parameters if p["in"] == "query"}
+        default_query_params = {k: v["default"] for k, v in query_defns.items() if "default" in v}
         query_arguments = deepcopy(default_query_params)
         query_arguments.update(query)
-        return self._query_args_helper(query_defns, query_arguments,
-                                       arguments, has_kwargs, sanitize)
+        return self._query_args_helper(query_defns, query_arguments, arguments, has_kwargs, sanitize)
 
     def _get_body_argument(self, body, arguments, has_kwargs, sanitize):
         kwargs = {}
-        body_parameters = [p for p in self.parameters if p['in'] == 'body'] or [{}]
+        body_parameters = [p for p in self.parameters if p["in"] == "body"] or [{}]
         if body is None:
-            body = deepcopy(body_parameters[0].get('schema', {}).get('default'))
-        body_name = sanitize(body_parameters[0].get('name'))
+            body = deepcopy(body_parameters[0].get("schema", {}).get("default"))
+        body_name = sanitize(body_parameters[0].get("name"))
+
+        form_defns = {p["name"]: p for p in self.parameters if p["in"] == "formData"}
 
-        form_defns = {p['name']: p
-                      for p in self.parameters
-                      if p['in'] == 'formData'}
-
-        default_form_params = {k: v['default']
-                               for k, v in form_defns.items()
-                               if 'default' in v}
+        default_form_params = {k: v["default"] for k, v in form_defns.items() if "default" in v}
 
         # Add body parameters
         if body_name:
             if not has_kwargs and body_name not in arguments:
                 logger.debug("Body parameter '%s' not in function arguments", body_name)
             else:
                 logger.debug("Body parameter '%s' in function arguments", body_name)
@@ -288,24 +287,23 @@
         # Add formData parameters
         form_arguments = deepcopy(default_form_params)
         if form_defns and body:
             form_arguments.update(body)
         for key, value in form_arguments.items():
             sanitized_key = sanitize(key)
             if not has_kwargs and sanitized_key not in arguments:
-                logger.debug("FormData parameter '%s' (sanitized: '%s') not in function arguments",
-                             key, sanitized_key)
+                logger.debug("FormData parameter '%s' (sanitized: '%s') not in function arguments", key, sanitized_key)
             else:
-                logger.debug("FormData parameter '%s' (sanitized: '%s') in function arguments",
-                             key, sanitized_key)
+                logger.debug("FormData parameter '%s' (sanitized: '%s') in function arguments", key, sanitized_key)
                 try:
                     form_defn = form_defns[key]
                 except KeyError:  # pragma: no cover
-                    logger.error("Function argument '%s' (non-sanitized: %s) not defined in specification",
-                                 key, sanitized_key)
+                    logger.error(
+                        "Function argument '%s' (non-sanitized: %s) not defined in specification", key, sanitized_key
+                    )
                 else:
                     kwargs[sanitized_key] = self._get_val_from_param(value, form_defn)
         return kwargs
 
     def _get_val_from_param(self, value, query_defn):
         if is_nullable(query_defn) and is_null(value):
             return None
```

### Comparing `firetail-1.0.8/firetail/options.py` & `firetail-1.0.9/firetail/options.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from typing import Optional  # NOQA
 
 try:
     from swagger_ui_bundle import swagger_ui_2_path, swagger_ui_3_path
 except ImportError:
     swagger_ui_2_path = swagger_ui_3_path = None
 
-from firetail.decorators.uri_parsing import AbstractURIParser
+from firetail.decorators.uri_parsing import AbstractURIParser  # noqa
 
 logger = logging.getLogger("firetail.options")
 
 
 class FiretailOptions:
     """Class holding firetail specific options."""
 
     def __init__(self, options=None, oas_version=(2,)):
         self._options = {}
         self.oas_version = oas_version
         if self.oas_version >= (3, 0, 0):
-            self.openapi_spec_name = '/openapi.json'
+            self.openapi_spec_name = "/openapi.json"
             self.swagger_ui_local_path = swagger_ui_3_path
         else:
-            self.openapi_spec_name = '/swagger.json'
+            self.openapi_spec_name = "/swagger.json"
             self.swagger_ui_local_path = swagger_ui_2_path
 
         if options:
             self._options.update(filter_values(options))
 
     def extend(self, new_values=None):
         # type: (Optional[dict]) -> FiretailOptions
@@ -52,95 +52,93 @@
         # type: () -> bool
         """
         Whether to make available the OpenAPI Specification under
         `openapi_spec_path`.
 
         Default: True
         """
-        deprecated_option = self._options.get('swagger_json', True)
-        serve_spec = self._options.get('serve_spec', deprecated_option)
-        if 'swagger_json' in self._options:
-            deprecation_warning = ("The 'swagger_json' option is deprecated. "
-                                   "Please use 'serve_spec' instead")
+        deprecated_option = self._options.get("swagger_json", True)
+        serve_spec = self._options.get("serve_spec", deprecated_option)
+        if "swagger_json" in self._options:
+            deprecation_warning = "The 'swagger_json' option is deprecated. " "Please use 'serve_spec' instead"
             logger.warning(deprecation_warning)
         return serve_spec
 
     @property
     def openapi_console_ui_available(self):
         # type: () -> bool
         """
         Whether to make the OpenAPI Console UI available under the path
         defined in `openapi_console_ui_path` option.
 
         Default: True
         """
-        if (self._options.get('swagger_ui', True) and
-                self.openapi_console_ui_from_dir is None):
+        if self._options.get("swagger_ui", True) and self.openapi_console_ui_from_dir is None:
             return False
-        return self._options.get('swagger_ui', True)
+        return self._options.get("swagger_ui", True)
 
     @property
     def openapi_spec_path(self):
         # type: () -> str
         """
         Path to mount the OpenAPI Console UI and make it accessible via a browser.
 
         Default: /openapi.json for openapi3, otherwise /swagger.json
         """
-        return self._options.get('openapi_spec_path', self.openapi_spec_name)
+        return self._options.get("openapi_spec_path", self.openapi_spec_name)
 
     @property
     def openapi_console_ui_path(self):
         # type: () -> str
         """
         Path to mount the OpenAPI Console UI and make it accessible via a browser.
 
         Default: /ui
         """
-        return self._options.get('swagger_url', '/ui')
+        return self._options.get("swagger_url", "/ui")
 
     @property
     def openapi_console_ui_from_dir(self):
         # type: () -> str
         """
         Custom OpenAPI Console UI directory from where Firetail will serve
         the static files.
 
         Default: Firetail's vendored version of the OpenAPI Console UI.
         """
-        return self._options.get('swagger_path', self.swagger_ui_local_path)
+        return self._options.get("swagger_path", self.swagger_ui_local_path)
 
     @property
     def openapi_console_ui_config(self):
         # type: () -> dict
         """
         Custom OpenAPI Console UI config.
 
         Default: None
         """
-        return self._options.get('swagger_ui_config', None)
+        return self._options.get("swagger_ui_config", None)
 
     @property
     def openapi_console_ui_index_template_variables(self):
         # type: () -> dict
         """
         Custom variables passed to the OpenAPI Console UI template.
 
         Default: {}
         """
-        return self._options.get('swagger_ui_template_arguments', {})
+        return self._options.get("swagger_ui_template_arguments", {})
 
     @property
     def uri_parser_class(self):
         # type: () -> AbstractURIParser
         """
         The class to use for parsing URIs into path and query parameters.
         Default: None
         """
-        return self._options.get('uri_parser_class', None)
+        return self._options.get("uri_parser_class", None)
 
 
 def filter_values(dictionary):
     # type: (dict) -> dict
     """
     Remove `None` value entries in the dictionary.
```

### Comparing `firetail-1.0.8/firetail/problem.py` & `firetail-1.0.9/firetail/problem.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,21 +30,17 @@
     :type headers: dict | None
     :param ext: Extension members to include in the body
     :type ext: dict | None
     :return: error response
     :rtype: FiretailResponse
     """
     if not type:
-        type = 'about:blank'
+        type = "about:blank"
 
-    problem_response = {'type': type, 'title': title, 'detail': detail, 'status': status}
+    problem_response = {"type": type, "title": title, "detail": detail, "status": status}
     if instance:
-        problem_response['instance'] = instance
+        problem_response["instance"] = instance
     if ext:
         problem_response.update(ext)
 
-    mimetype = content_type = 'application/problem+json'
-    return FiretailResponse(status,
-                            mimetype,
-                            content_type,
-                            body=problem_response,
-                            headers=headers)
+    mimetype = content_type = "application/problem+json"
+    return FiretailResponse(status, mimetype, content_type, body=problem_response, headers=headers)
```

### Comparing `firetail-1.0.8/firetail/resolver.py` & `firetail-1.0.9/firetail/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import sys
 
 from inflection import camelize
 
 import firetail.utils as utils
 from firetail.exceptions import ResolverError
 
-logger = logging.getLogger('firetail.resolver')
+logger = logging.getLogger("firetail.resolver")
 
 
 class Resolution:
     def __init__(self, function, operation_id):
         """
         Represents the result of operation resolution
 
@@ -52,15 +52,15 @@
 
         :type operation: firetail.operations.AbstractOperation
         """
         operation_id = operation.operation_id
         router_controller = operation.router_controller
         if router_controller is None:
             return operation_id
-        return f'{router_controller}.{operation_id}'
+        return f"{router_controller}.{operation_id}"
 
     def resolve_function_from_operation_id(self, operation_id):
         """
         Invokes the function_resolver
 
         :type operation_id: str
         """
@@ -73,14 +73,15 @@
             raise ResolverError(str(e), sys.exc_info())
 
 
 class RelativeResolver(Resolver):
     """
     Resolves endpoint functions relative to a given root path or module.
     """
+
     def __init__(self, root_path, function_resolver=utils.get_function_from_name):
         """
         :param root_path: The root path relative to which an operationId is resolved.
             Can also be a module. Has the same effect as setting
             `x-swagger-router-controller` or `x-openapi-router-controller` equal to
             `root_path` for every operation individually.
         :type root_path: typing.Union[str, types.ModuleType]
@@ -99,24 +100,24 @@
 
         :param operation: The operation to resolve
         :type operation: firetail.operations.AbstractOperation
         """
         operation_id = operation.operation_id
         router_controller = operation.router_controller
         if router_controller is None:
-            return f'{self.root_path}.{operation_id}'
-        return f'{router_controller}.{operation_id}'
+            return f"{self.root_path}.{operation_id}"
+        return f"{router_controller}.{operation_id}"
 
 
 class RestyResolver(Resolver):
     """
     Resolves endpoint functions using REST semantics (unless overridden by specifying operationId)
     """
 
-    def __init__(self, default_module_name, collection_endpoint_name='search'):
+    def __init__(self, default_module_name, collection_endpoint_name="search"):
         """
         :param default_module_name: Default module name for operations
         :type default_module_name: str
         """
         super().__init__()
         self.default_module_name = default_module_name
         self.collection_endpoint_name = collection_endpoint_name
@@ -136,48 +137,43 @@
         """
         Resolves the operationId using REST semantics
 
         :type operation: firetail.operations.AbstractOperation
         """
 
         # Split the path into components delimited by '/'
-        path_components = [c for c in operation.path.split('/') if len(c)]
+        path_components = [c for c in operation.path.split("/") if len(c)]
 
         def is_var(component):
             """True if the path component is a var. eg, '{id}'"""
-            return (component[0] == '{') and (component[-1] == '}')
+            return (component[0] == "{") and (component[-1] == "}")
 
-        resource_name = '.'.join(
-            [c for c in path_components if not is_var(c)]
-        ).replace('-', '_')
+        resource_name = ".".join([c for c in path_components if not is_var(c)]).replace("-", "_")
 
         def get_controller_name():
             x_router_controller = operation.router_controller
 
             name = self.default_module_name
 
             if x_router_controller:
                 name = x_router_controller
 
             elif resource_name:
-                name += '.' + resource_name
+                name += "." + resource_name
 
             return name
 
         def get_function_name():
             method = operation.method
 
-            is_collection_endpoint = \
-                method.lower() == 'get' \
-                and len(resource_name) \
-                and not is_var(path_components[-1])
+            is_collection_endpoint = method.lower() == "get" and len(resource_name) and not is_var(path_components[-1])
 
             return self.collection_endpoint_name if is_collection_endpoint else method.lower()
 
-        return f'{get_controller_name()}.{get_function_name()}'
+        return f"{get_controller_name()}.{get_function_name()}"
 
 
 class MethodViewResolver(RestyResolver):
     """
     Resolves endpoint functions based on Flask's MethodView semantics, e.g. ::
 
             paths:
@@ -206,29 +202,29 @@
         """
         if operation.operation_id:
             # If operation_id is defined then use the higher level API to resolve
             return RestyResolver.resolve_operation_id(self, operation)
 
         # Use RestyResolver to get operation_id for us (follow their naming conventions/structure)
         operation_id = self.resolve_operation_id_using_rest_semantics(operation)
-        module_name, view_base, meth_name = operation_id.rsplit('.', 2)
-        view_name = camelize(view_base) + 'View'
+        module_name, view_base, meth_name = operation_id.rsplit(".", 2)
+        view_name = camelize(view_base) + "View"
 
         return f"{module_name}.{view_name}.{meth_name}"
 
     def resolve_function_from_operation_id(self, operation_id):
         """
         Invokes the function_resolver
 
         :type operation_id: str
         """
 
         try:
-            module_name, view_name, meth_name = operation_id.rsplit('.', 2)
-            if operation_id and not view_name.endswith('View'):
+            module_name, view_name, meth_name = operation_id.rsplit(".", 2)
+            if operation_id and not view_name.endswith("View"):
                 # If operation_id is not a view then assume it is a standard function
                 return self.function_resolver(operation_id)
 
             mod = __import__(module_name, fromlist=[view_name])
             view_cls = getattr(mod, view_name)
             # Find the class and instantiate it
             view = None
@@ -239,12 +235,11 @@
             if view is None:
                 view = view_cls()
                 self.initialized_views.append(view)
             func = getattr(view, meth_name)
             # Return the method function of the class
             return func
         except ImportError as e:
-            msg = 'Cannot resolve operationId "{}"! Import error was "{}"'.format(
-                operation_id, str(e))
+            msg = 'Cannot resolve operationId "{}"! Import error was "{}"'.format(operation_id, str(e))
             raise ResolverError(msg, sys.exc_info())
         except (AttributeError, ValueError) as e:
             raise ResolverError(str(e), sys.exc_info())
```

### Comparing `firetail-1.0.8/firetail/resources/schemas/v2.0/schema.json` & `firetail-1.0.9/firetail/resources/schemas/v2.0/schema.json`

 * *Files identical despite different names*

### Comparing `firetail-1.0.8/firetail/resources/schemas/v3.0/schema.json` & `firetail-1.0.9/firetail/resources/schemas/v3.0/schema.json`

 * *Files identical despite different names*

### Comparing `firetail-1.0.8/firetail/security/__init__.py` & `firetail-1.0.9/firetail/security/__init__.py`

 * *Files identical despite different names*

### Comparing `firetail-1.0.8/firetail/security/aiohttp_security_handler_factory.py` & `firetail-1.0.9/firetail/security/aiohttp_security_handler_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import logging
 
 import aiohttp
 
 from .async_security_handler_factory import AbstractAsyncSecurityHandlerFactory
 
-logger = logging.getLogger('firetail.api.security')
+logger = logging.getLogger("firetail.api.security")
 
 
 class AioHttpSecurityHandlerFactory(AbstractAsyncSecurityHandlerFactory):
     def __init__(self, pass_context_arg_name):
         super().__init__(pass_context_arg_name=pass_context_arg_name)
         self.client_session = None
 
@@ -23,17 +23,19 @@
         Returned function must accept oauth token in parameter.
         It must return a token_info dict in case of success, None otherwise.
 
         :param token_info_url: Url to get information about the token
         :type token_info_url: str
         :rtype: types.FunctionType
         """
+
         async def wrapper(token):
             if not self.client_session:
                 # Must be created in a coroutine
                 self.client_session = aiohttp.ClientSession()
-            headers = {'Authorization': f'Bearer {token}'}
+            headers = {"Authorization": f"Bearer {token}"}
             token_request = await self.client_session.get(token_info_url, headers=headers, timeout=5)
             if token_request.status != 200:
                 return None
             return token_request.json()
+
         return wrapper
```

### Comparing `firetail-1.0.8/firetail/security/async_security_handler_factory.py` & `firetail-1.0.9/firetail/security/async_security_handler_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import asyncio
 import functools
 import logging
 
 from ..exceptions import OAuthProblem, OAuthResponseProblem, OAuthScopeProblem
 from .security_handler_factory import AbstractSecurityHandlerFactory
 
-logger = logging.getLogger('firetail.api.security')
+logger = logging.getLogger("firetail.api.security")
 
 
 class AbstractAsyncSecurityHandlerFactory(AbstractSecurityHandlerFactory):
     def _generic_check(self, func, exception_msg):
         need_to_add_context, need_to_add_required_scopes = self._need_to_add_context_or_scopes(func)
 
         async def wrapper(request, *args, required_scopes=None):
@@ -32,37 +32,38 @@
             if token_info is None:
                 raise OAuthResponseProblem(description=exception_msg, token_response=None)
             return token_info
 
         return wrapper
 
     def check_oauth_func(self, token_info_func, scope_validate_func):
-        get_token_info = self._generic_check(token_info_func, 'Provided token is not valid')
+        get_token_info = self._generic_check(token_info_func, "Provided token is not valid")
         need_to_add_context, _ = self._need_to_add_context_or_scopes(scope_validate_func)
 
         async def wrapper(request, token, required_scopes):
             token_info = await get_token_info(request, token, required_scopes=required_scopes)
 
             # Fallback to 'scopes' for backward compatibility
-            token_scopes = token_info.get('scope', token_info.get('scopes', ''))
+            token_scopes = token_info.get("scope", token_info.get("scopes", ""))
 
             kwargs = {}
             if need_to_add_context:
                 kwargs[self.pass_context_arg_name] = request.context
             validation = scope_validate_func(required_scopes, token_scopes, **kwargs)
             while asyncio.iscoroutine(validation):
                 validation = await validation
             if not validation:
                 raise OAuthScopeProblem(
-                    description='Provided token doesn\'t have the required scope',
+                    description="Provided token doesn't have the required scope",
                     required_scopes=required_scopes,
-                    token_scopes=token_scopes
-                    )
+                    token_scopes=token_scopes,
+                )
 
             return token_info
+
         return wrapper
 
     @classmethod
     def verify_security(cls, auth_funcs, function):
         @functools.wraps(function)
         async def wrapper(request):
             token_info = cls.no_value
@@ -78,19 +79,19 @@
                     errors.append(err)
 
             else:
                 if errors != []:
                     cls._raise_most_specific(errors)
                 else:
                     logger.info("... No auth provided. Aborting with 401.")
-                    raise OAuthProblem(description='No authorization token provided')
+                    raise OAuthProblem(description="No authorization token provided")
 
             # Fallback to 'uid' for backward compatibility
-            request.context['user'] = token_info.get('sub', token_info.get('uid'))
-            request.context['token_info'] = token_info
+            request.context["user"] = token_info.get("sub", token_info.get("uid"))
+            request.context["token_info"] = token_info
             return function(request)
 
         return wrapper
 
     @abc.abstractmethod
     def get_token_info_remote(self, token_info_url):
         """
```

### Comparing `firetail-1.0.8/firetail/security/flask_security_handler_factory.py` & `firetail-1.0.9/firetail/security/flask_security_handler_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,36 +5,38 @@
 import requests
 
 from .security_handler_factory import AbstractSecurityHandlerFactory
 
 # use connection pool for OAuth tokeninfo
 adapter = requests.adapters.HTTPAdapter(pool_connections=100, pool_maxsize=100)
 session = requests.Session()
-session.mount('http://', adapter)
-session.mount('https://', adapter)
+session.mount("http://", adapter)
+session.mount("https://", adapter)
 
 
 class FlaskSecurityHandlerFactory(AbstractSecurityHandlerFactory):
     def get_token_info_remote(self, token_info_url):
         """
         Return a function which will call `token_info_url` to retrieve token info.
 
         Returned function must accept oauth token in parameter.
         It must return a token_info dict in case of success, None otherwise.
 
         :param token_info_url: Url to get information about the token
         :type token_info_url: str
         :rtype: types.FunctionType
         """
+
         def wrapper(token):
             """
             Retrieve oauth token_info remotely using HTTP
             :param token: oauth token from authorization header
             :type token: str
             :rtype: dict
             """
-            headers = {'Authorization': f'Bearer {token}'}
+            headers = {"Authorization": f"Bearer {token}"}
             token_request = session.get(token_info_url, headers=headers, timeout=5)
             if not token_request.ok:
                 return None
             return token_request.json()
+
         return wrapper
```

### Comparing `firetail-1.0.8/firetail/security/security_handler_factory.py` & `firetail-1.0.9/firetail/security/security_handler_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     FiretailException,
     OAuthProblem,
     OAuthResponseProblem,
     OAuthScopeProblem,
 )
 from ..utils import get_function_from_name
 
-logger = logging.getLogger('firetail.api.security')
+logger = logging.getLogger("firetail.api.security")
 
 
 class AbstractSecurityHandlerFactory(abc.ABC):
     """
     get_*_func -> _get_function -> get_function_from_name (name=security function defined in spec)
         (if url defined instead of a function -> get_token_info_remote)
 
@@ -34,16 +34,17 @@
     verify_* -> returns a security wrapper around the security function
         check_* -> returns a function tasked with doing auth for use inside the verify wrapper
             check helpers (used outside wrappers): _need_to_add_context_or_scopes
             the security function
 
         verify helpers (used inside wrappers): get_auth_header_value, get_cookie_value
     """
+
     no_value = object()
-    required_scopes_kw = 'required_scopes'
+    required_scopes_kw = "required_scopes"
 
     def __init__(self, pass_context_arg_name):
         self.pass_context_arg_name = pass_context_arg_name
 
     @staticmethod
     def _get_function(security_definition, security_definition_key, environ_key, default=None):
         """
@@ -57,68 +58,67 @@
     def get_tokeninfo_func(self, security_definition: dict) -> t.Optional[t.Callable]:
         """
         :type security_definition: dict
 
         >>> get_tokeninfo_url({'x-tokenInfoFunc': 'foo.bar'})
         '<function foo.bar>'
         """
-        token_info_func = self._get_function(security_definition, "x-tokenInfoFunc", 'TOKENINFO_FUNC')
+        token_info_func = self._get_function(security_definition, "x-tokenInfoFunc", "TOKENINFO_FUNC")
         if token_info_func:
             return token_info_func
 
-        token_info_url = (security_definition.get('x-tokenInfoUrl') or
-                          os.environ.get('TOKENINFO_URL'))
+        token_info_url = security_definition.get("x-tokenInfoUrl") or os.environ.get("TOKENINFO_URL")
         if token_info_url:
             return self.get_token_info_remote(token_info_url)
 
         return None
 
     @classmethod
     def get_scope_validate_func(cls, security_definition):
         """
         :type security_definition: dict
         :rtype: function
 
         >>> get_scope_validate_func({'x-scopeValidateFunc': 'foo.bar'})
         '<function foo.bar>'
         """
-        return cls._get_function(security_definition, "x-scopeValidateFunc", 'SCOPEVALIDATE_FUNC', cls.validate_scope)
+        return cls._get_function(security_definition, "x-scopeValidateFunc", "SCOPEVALIDATE_FUNC", cls.validate_scope)
 
     @classmethod
     def get_basicinfo_func(cls, security_definition):
         """
         :type security_definition: dict
         :rtype: function
 
         >>> get_basicinfo_func({'x-basicInfoFunc': 'foo.bar'})
         '<function foo.bar>'
         """
-        return cls._get_function(security_definition, "x-basicInfoFunc", 'BASICINFO_FUNC')
+        return cls._get_function(security_definition, "x-basicInfoFunc", "BASICINFO_FUNC")
 
     @classmethod
     def get_apikeyinfo_func(cls, security_definition):
         """
         :type security_definition: dict
         :rtype: function
 
         >>> get_apikeyinfo_func({'x-apikeyInfoFunc': 'foo.bar'})
         '<function foo.bar>'
         """
-        return cls._get_function(security_definition, "x-apikeyInfoFunc", 'APIKEYINFO_FUNC')
+        return cls._get_function(security_definition, "x-apikeyInfoFunc", "APIKEYINFO_FUNC")
 
     @classmethod
     def get_bearerinfo_func(cls, security_definition):
         """
         :type security_definition: dict
         :rtype: function
 
         >>> get_bearerinfo_func({'x-bearerInfoFunc': 'foo.bar'})
         '<function foo.bar>'
         """
-        return cls._get_function(security_definition, "x-bearerInfoFunc", 'BEARERINFO_FUNC')
+        return cls._get_function(security_definition, "x-bearerInfoFunc", "BEARERINFO_FUNC")
 
     @staticmethod
     def security_passthrough(function):
         """
         :type function: types.FunctionType
         :rtype: types.FunctionType
         """
@@ -147,112 +147,116 @@
         if isinstance(token_scopes, list):
             token_scopes = set(token_scopes)
         else:
             token_scopes = set(token_scopes.split())
         logger.debug("... Scopes required: %s", required_scopes)
         logger.debug("... Token scopes: %s", token_scopes)
         if not required_scopes <= token_scopes:
-            logger.info(textwrap.dedent("""
+            logger.info(
+                textwrap.dedent(
+                    """
                         ... Token scopes (%s) do not match the scopes necessary to call endpoint (%s).
-                         Aborting with 403.""").replace('\n', ''),
-                        token_scopes, required_scopes)
+                         Aborting with 403."""
+                ).replace("\n", ""),
+                token_scopes,
+                required_scopes,
+            )
             return False
         return True
 
     @staticmethod
     def get_auth_header_value(request):
         """
         Called inside security wrapper functions
 
         Return Authorization type and value if any.
         If not Authorization, return (None, None)
         Raise OAuthProblem for invalid Authorization header
         """
-        authorization = request.headers.get('Authorization')
+        authorization = request.headers.get("Authorization")
         if not authorization:
             return None, None
 
         try:
             auth_type, value = authorization.split(None, 1)
         except ValueError:
-            raise OAuthProblem(description='Invalid authorization header')
+            raise OAuthProblem(description="Invalid authorization header")
         return auth_type.lower(), value
 
     def verify_oauth(self, token_info_func, scope_validate_func, required_scopes):
         check_oauth_func = self.check_oauth_func(token_info_func, scope_validate_func)
 
         def wrapper(request):
             auth_type, token = self.get_auth_header_value(request)
-            if auth_type != 'bearer':
+            if auth_type != "bearer":
                 return self.no_value
 
             return check_oauth_func(request, token, required_scopes=required_scopes)
 
         return wrapper
 
     def verify_basic(self, basic_info_func):
         check_basic_info_func = self.check_basic_auth(basic_info_func)
 
         def wrapper(request):
             auth_type, user_pass = self.get_auth_header_value(request)
-            if auth_type != 'basic':
+            if auth_type != "basic":
                 return self.no_value
 
             try:
-                username, password = base64.b64decode(user_pass).decode('latin1').split(':', 1)
+                username, password = base64.b64decode(user_pass).decode("latin1").split(":", 1)
             except Exception:
-                raise OAuthProblem(description='Invalid authorization header')
+                raise OAuthProblem(description="Invalid authorization header")
 
             return check_basic_info_func(request, username, password)
 
         return wrapper
 
     @staticmethod
     def get_cookie_value(cookies, name):
-        '''
+        """
         Called inside security wrapper functions
 
         Returns cookie value by its name. None if no such value.
         :param cookies: str: cookies raw data
         :param name: str: cookies key
-        '''
+        """
         cookie_parser = http.cookies.SimpleCookie()
         cookie_parser.load(str(cookies))
         try:
             return cookie_parser[name].value
         except KeyError:
             return None
 
     def verify_api_key(self, api_key_info_func, loc, name):
         check_api_key_func = self.check_api_key(api_key_info_func)
 
         def wrapper(request):
-
             def _immutable_pop(_dict, key):
                 """
                 Pops the key from an immutable dict and returns the value that was popped,
                 and a new immutable dict without the popped key.
                 """
                 cls = type(_dict)
                 try:
                     _dict = _dict.to_dict(flat=False)
                     return _dict.pop(key)[0], cls(_dict)
                 except AttributeError:
                     _dict = dict(_dict.items())
                     return _dict.pop(key), cls(_dict)
 
-            if loc == 'query':
+            if loc == "query":
                 try:
                     api_key, request.query = _immutable_pop(request.query, name)
                 except KeyError:
                     api_key = None
-            elif loc == 'header':
+            elif loc == "header":
                 api_key = request.headers.get(name)
-            elif loc == 'cookie':
-                cookie_list = request.headers.get('Cookie')
+            elif loc == "cookie":
+                cookie_list = request.headers.get("Cookie")
                 api_key = self.get_cookie_value(cookie_list, name)
             else:
                 return self.no_value
 
             if api_key is None:
                 return self.no_value
 
@@ -265,15 +269,15 @@
         :param token_info_func: types.FunctionType
         :rtype: types.FunctionType
         """
         check_bearer_func = self.check_bearer_token(token_info_func)
 
         def wrapper(request):
             auth_type, token = self.get_auth_header_value(request)
-            if auth_type != 'bearer':
+            if auth_type != "bearer":
                 return self.no_value
             return check_bearer_func(request, token)
 
         return wrapper
 
     def verify_multiple_schemes(self, schemes):
         """
@@ -329,44 +333,45 @@
             if token_info is None:
                 raise OAuthResponseProblem(description=exception_msg, token_response=None)
             return token_info
 
         return wrapper
 
     def check_bearer_token(self, token_info_func):
-        return self._generic_check(token_info_func, 'Provided token is not valid')
+        return self._generic_check(token_info_func, "Provided token is not valid")
 
     def check_basic_auth(self, basic_info_func):
-        return self._generic_check(basic_info_func, 'Provided authorization is not valid')
+        return self._generic_check(basic_info_func, "Provided authorization is not valid")
 
     def check_api_key(self, api_key_info_func):
-        return self._generic_check(api_key_info_func, 'Provided apikey is not valid')
+        return self._generic_check(api_key_info_func, "Provided apikey is not valid")
 
     def check_oauth_func(self, token_info_func, scope_validate_func):
-        get_token_info = self._generic_check(token_info_func, 'Provided token is not valid')
+        get_token_info = self._generic_check(token_info_func, "Provided token is not valid")
         need_to_add_context, _ = self._need_to_add_context_or_scopes(scope_validate_func)
 
         def wrapper(request, token, required_scopes):
             token_info = get_token_info(request, token, required_scopes=required_scopes)
 
             # Fallback to 'scopes' for backward compatibility
-            token_scopes = token_info.get('scope', token_info.get('scopes', ''))
+            token_scopes = token_info.get("scope", token_info.get("scopes", ""))
 
             kwargs = {}
             if need_to_add_context:
                 kwargs[self.pass_context_arg_name] = request.context
             validation = scope_validate_func(required_scopes, token_scopes, **kwargs)
             if not validation:
                 raise OAuthScopeProblem(
-                    description='Provided token doesn\'t have the required scope',
+                    description="Provided token doesn't have the required scope",
                     required_scopes=required_scopes,
-                    token_scopes=token_scopes
-                    )
+                    token_scopes=token_scopes,
+                )
 
             return token_info
+
         return wrapper
 
     @classmethod
     def verify_security(cls, auth_funcs, function):
         @functools.wraps(function)
         def wrapper(request):
             token_info = cls.no_value
@@ -380,19 +385,19 @@
                     errors.append(err)
 
             else:
                 if errors != []:
                     cls._raise_most_specific(errors)
                 else:
                     logger.info("... No auth provided. Aborting with 401.")
-                    raise OAuthProblem(description='No authorization token provided')
+                    raise OAuthProblem(description="No authorization token provided")
 
             # Fallback to 'uid' for backward compatibility
-            request.context['user'] = token_info.get('sub', token_info.get('uid'))
-            request.context['token_info'] = token_info
+            request.context["user"] = token_info.get("sub", token_info.get("uid"))
+            request.context["token_info"] = token_info
             return function(request)
 
         return wrapper
 
     @staticmethod
     def _raise_most_specific(exceptions: t.List[Exception]) -> None:
         """Raises the most specific error from a list of exceptions by status code.
@@ -408,18 +413,15 @@
         :param errors: List of exceptions.
         :type errors: t.List[Exception]
         """
         if not exceptions:
             return
         # We only use status code attributes from exceptions
         # We use 600 as default because 599 is highest valid status code
-        status_to_exc = {
-            getattr(exc, 'code', getattr(exc, 'status', 600)): exc
-            for exc in exceptions
-        }
+        status_to_exc = {getattr(exc, "code", getattr(exc, "status", 600)): exc for exc in exceptions}
         if 403 in status_to_exc:
             raise status_to_exc[403]
         elif 401 in status_to_exc:
             raise status_to_exc[401]
         else:
             lowest_status_code = min(status_to_exc)
             raise status_to_exc[lowest_status_code]
```

### Comparing `firetail-1.0.8/firetail/sender.py` & `firetail-1.0.9/firetail/sender.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,58 +19,58 @@
 #                             level=loger4.DEBUG)
 
 
 MAX_BULK_SIZE_IN_BYTES = 1 * 1024 * 1024  # 1 MB
 
 
 def backup_logs(logs, logger):
-    timestamp = datetime.now().strftime('%d%m%Y-%H%M%S')
-    logger.info(
-        'Backing up your logs to firetail-failures-%s.txt', timestamp)
-    with open('firetail-failures-{}.txt'.format(timestamp), 'a') as f:
-        f.writelines('\n'.join(logs))
+    timestamp = datetime.now().strftime("%d%m%Y-%H%M%S")
+    logger.info("Backing up your logs to firetail-failures-%s.txt", timestamp)
+    with open("firetail-failures-{}.txt".format(timestamp), "a") as f:
+        f.writelines("\n".join(logs))
 
 
 class FiretailSender:
-    def __init__(self,
-                 token,
-                 url,
-                 logs_drain_timeout=5,
-                 debug=False,
-                 backup_logs=True,
-                 network_timeout=10.0,
-                 number_of_retries=4,
-                 retry_timeout=2):
+    def __init__(
+        self,
+        token,
+        url,
+        logs_drain_timeout=5,
+        debug=False,
+        backup_logs=True,
+        network_timeout=10.0,
+        number_of_retries=4,
+        retry_timeout=2,
+    ):
         self.token = token
         self.url = url
         self.logs_drain_timeout = logs_drain_timeout
         self.stdout_logger = get_stdout_logger(debug)
         self.backup_logs = backup_logs
         self.network_timeout = network_timeout
         self.requests_session = requests.Session()
         self.number_of_retries = number_of_retries
         self.retry_timeout = retry_timeout
 
         # Function to see if the main thread is alive
-        self.is_main_thread_active = lambda: any(
-            (i.name == 'MainThread') and i.is_alive() for i in enumerate())
+        self.is_main_thread_active = lambda: any((i.name == "MainThread") and i.is_alive() for i in enumerate())
 
         # Create a queue to hold logs
         self.queue = queue.Queue()
         self._initialize_sending_thread()
 
     def __del__(self):
         del self.stdout_logger
         del self.backup_logs
         del self.queue
 
     def _initialize_sending_thread(self):
         self.sending_thread = Thread(target=self._drain_queue)
         self.sending_thread.daemon = False
-        self.sending_thread.name = 'firetail-sending-thread'
+        self.sending_thread.name = "firetail-sending-thread"
         self.sending_thread.start()
 
     def append(self, logs_message):
         if not self.sending_thread.is_alive():
             self._initialize_sending_thread()
 
         # Queue lib is thread safe, no issue here
@@ -82,101 +82,98 @@
     def _drain_queue(self):
         last_try = False
 
         while not last_try:
             # If main is exited, we should run one last time and try to remove
             # all logs
             if not self.is_main_thread_active():
-                self.stdout_logger.debug(
-                    'Identified quit of main thread, sending logs one '
-                    'last time')
+                self.stdout_logger.debug("Identified quit of main thread, sending logs one " "last time")
                 last_try = True
 
             try:
                 self._flush_queue()
             except Exception as e:
                 self.stdout_logger.debug(
-                    'Unexpected exception while draining queue to firetail, '
-                    'swallowing. Exception: %s', e)
+                    "Unexpected exception while draining queue to firetail, " "swallowing. Exception: %s", e
+                )
 
             if not last_try:
                 sleep(self.logs_drain_timeout)
 
     def _flush_queue(self):
         # Sending logs until queue is empty
         loger4.info(self.url)
         while not self.queue.empty():
             logs_list = self._get_messages_up_to_max_allowed_size()
-            self.stdout_logger.debug(
-                'Starting to drain %s logs to firetail', len(logs_list))
+            self.stdout_logger.debug("Starting to drain %s logs to firetail", len(logs_list))
 
             # Not configurable from the outside
             sleep_between_retries = self.retry_timeout
             self.number_of_retries = self.number_of_retries
 
             should_backup_to_disk = True
-            headers = {
-                "Content-type": "application/x-ndjson",
-                'x-ft-api-key': self.token
-                }
+            headers = {"Content-type": "application/x-ndjson", "x-ft-api-key": self.token}
 
             for current_try in range(self.number_of_retries):
                 should_retry = False
                 try:
                     response = self.requests_session.post(
-                        self.url, headers=headers, data='\n'.join(logs_list),
-                        timeout=self.network_timeout)
+                        self.url, headers=headers, data="\n".join(logs_list), timeout=self.network_timeout
+                    )
                     # loger4.info(response.text)
                     # self.stdout_logger.info(str(response.status_code))
                     if response.status_code != 200:
                         if response.status_code == 400:
                             self.stdout_logger.debug(
-                                'Got 400 code from firetail. This means that '
-                                'some of your logs are too big, or badly '
-                                'formatted. response: %s', response.text)
+                                "Got 400 code from firetail. This means that "
+                                "some of your logs are too big, or badly "
+                                "formatted. response: %s",
+                                response.text,
+                            )
                             should_backup_to_disk = False
                             should_retry = False
                             break
 
                         if response.status_code == 401:
                             self.stdout_logger.debug(
-                                'You are not authorized with firetail! Token '
-                                'OK? dropping logs...')
+                                "You are not authorized with firetail! Token " "OK? dropping logs..."
+                            )
                             should_backup_to_disk = False
                             break
                         else:
                             self.stdout_logger.debug(
-                                'Got %s while sending logs to firetail, '
-                                'Try (%s/%s). Response: %s',
+                                "Got %s while sending logs to firetail, " "Try (%s/%s). Response: %s",
                                 response.status_code,
                                 current_try + 1,
                                 self.number_of_retries,
-                                response.status_code)
+                                response.status_code,
+                            )
                             should_retry = False
                     else:
-                        self.stdout_logger.debug(
-                            'Successfully sent bulk of %s logs to '
-                            'firetail', len(logs_list))
+                        self.stdout_logger.debug("Successfully sent bulk of %s logs to " "firetail", len(logs_list))
                         should_backup_to_disk = False
                         break
                 except Exception as e:
                     self.stdout_logger.warning(
-                        'Got exception while sending logs to firetail, '
-                        'Try (%s/%s). Message: %s',
-                        current_try + 1, self.number_of_retries, e)
+                        "Got exception while sending logs to firetail, " "Try (%s/%s). Message: %s",
+                        current_try + 1,
+                        self.number_of_retries,
+                        e,
+                    )
                     should_retry = True
 
                 if should_retry:
                     sleep(sleep_between_retries)
 
             if should_backup_to_disk and self.backup_logs:
                 # Write to file
                 self.stdout_logger.error(
-                    'Could not send logs to firetail after %s tries, '
-                    'backing up to local file system', self.number_of_retries)
+                    "Could not send logs to firetail after %s tries, " "backing up to local file system",
+                    self.number_of_retries,
+                )
                 backup_logs(logs_list, self.stdout_logger)
 
             del logs_list
 
     def _get_messages_up_to_max_allowed_size(self):
         logs_list = []
         current_size = 0
```

### Comparing `firetail-1.0.8/firetail/spec.py` & `firetail-1.0.9/firetail/spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,31 +27,31 @@
 def create_spec_validator(spec: dict) -> Draft4Validator:
     """Create a Validator to validate an OpenAPI spec against the OpenAPI schema.
 
     :param spec: specification to validate
     """
     # Create an instance validator, which validates defaults against the spec itself instead of
     # against the OpenAPI schema.
-    InstanceValidator = extend_validator(Draft4Validator, {'type': NullableTypeValidator})
+    InstanceValidator = extend_validator(Draft4Validator, {"type": NullableTypeValidator})
     instance_validator = InstanceValidator(spec)
 
     def validate_defaults(validator, properties, instance, schema):
         """Validation function to validate the `properties` subschema, enforcing each default
         value validates against the schema in which it resides.
         """
         valid = True
         for error in validate_properties(validator, properties, instance, schema):
             valid = False
             yield error
 
         # Validate default only when the subschema has validated successfully
         if not valid:
             return
-        if isinstance(instance, dict) and 'default' in instance:
-            for error in instance_validator.iter_errors(instance['default'], instance):
+        if isinstance(instance, dict) and "default" in instance:
+            for error in instance_validator.iter_errors(instance["default"], instance):
                 yield error
 
     SpecValidator = extend_validator(Draft4Validator, {"properties": validate_defaults})
     return SpecValidator
 
 
 NO_SPEC_VERSION_ERR_MSG = """Unable to get the spec version.
@@ -59,35 +59,32 @@
 from the top level of your spec."""
 
 
 def canonical_base_path(base_path):
     """
     Make given "basePath" a canonical base URL which can be prepended to paths starting with "/".
     """
-    return base_path.rstrip('/')
+    return base_path.rstrip("/")
 
 
 class Specification(Mapping):
-
     def __init__(self, raw_spec):
         self._raw_spec = copy.deepcopy(raw_spec)
         self._set_defaults(raw_spec)
         self._validate_spec(raw_spec)
         self._spec = resolve_refs(raw_spec)
 
     @classmethod
     @abc.abstractmethod
     def _set_defaults(cls, spec):
-        """ set some default values in the spec
-        """
+        """set some default values in the spec"""
 
     @classmethod
     def _validate_spec(cls, spec):
-        """ validate spec against schema
-        """
+        """validate spec against schema"""
         try:
             OpenApiValidator = create_spec_validator(spec)
             validator = OpenApiValidator(cls.openapi_schema)
             validator.validate(spec)
         except jsonschema.exceptions.ValidationError as e:
             raise InvalidSpecification.create_from(e)
 
@@ -103,15 +100,15 @@
 
     @property
     def version(self):
         return self._get_spec_version(self._spec)
 
     @property
     def security(self):
-        return self._spec.get('security')
+        return self._spec.get("security")
 
     def __getitem__(self, k):
         return self._spec[k]
 
     def __iter__(self):
         return self._spec.__iter__()
 
@@ -124,20 +121,20 @@
         Loads a YAML specification file, optionally rendering it with Jinja2.
 
         :param arguments: passed to Jinja2 renderer
         :param specification: path to specification
         """
         arguments = arguments or {}
 
-        with specification.open(mode='rb') as openapi_yaml:
+        with specification.open(mode="rb") as openapi_yaml:
             contents = openapi_yaml.read()
             try:
                 openapi_template = contents.decode()
             except UnicodeDecodeError:
-                openapi_template = contents.decode('utf-8', 'replace')
+                openapi_template = contents.decode("utf-8", "replace")
 
             openapi_string = jinja2.Template(openapi_template).render(**arguments)
             return yaml.safe_load(openapi_string)
 
     @classmethod
     def from_file(cls, spec, arguments=None):
         """
@@ -146,41 +143,37 @@
         specification_path = pathlib.Path(spec)
         spec = cls._load_spec_from_file(arguments, specification_path)
         return cls.from_dict(spec)
 
     @staticmethod
     def _get_spec_version(spec):
         try:
-            version_string = spec.get('openapi') or spec.get('swagger')
+            version_string = spec.get("openapi") or spec.get("swagger")
         except AttributeError:
             raise InvalidSpecification(NO_SPEC_VERSION_ERR_MSG)
         if version_string is None:
             raise InvalidSpecification(NO_SPEC_VERSION_ERR_MSG)
         try:
             version_tuple = tuple(map(int, version_string.split(".")))
         except TypeError:
-            err = ('Unable to convert version string to semantic version tuple: '
-                   '{version_string}.')
+            err = "Unable to convert version string to semantic version tuple: " "{version_string}."
             err = err.format(version_string=version_string)
             raise InvalidSpecification(err)
         return version_tuple
 
     @classmethod
     def from_dict(cls, spec):
         """
         Takes in a dictionary, and returns a Specification
         """
+
         def enforce_string_keys(obj):
             # YAML supports integer keys, but JSON does not
             if isinstance(obj, dict):
-                return {
-                    str(k): enforce_string_keys(v)
-                    for k, v
-                    in obj.items()
-                }
+                return {str(k): enforce_string_keys(v) for k, v in obj.items()}
             return obj
 
         spec = enforce_string_keys(spec)
         version = cls._get_spec_version(spec)
         if version < (3, 0, 0):
             return Swagger2Specification(spec)
         return OpenAPISpecification(spec)
@@ -199,101 +192,94 @@
         new_spec.base_path = base_path
         return new_spec
 
 
 class Swagger2Specification(Specification):
     """Python interface for a Swagger 2 specification."""
 
-    yaml_name = 'swagger.yaml'
+    yaml_name = "swagger.yaml"
     operation_cls = Swagger2Operation
 
-    openapi_schema = json.loads(
-        pkgutil.get_data('firetail', 'resources/schemas/v2.0/schema.json')
-    )
+    openapi_schema = json.loads(pkgutil.get_data("firetail", "resources/schemas/v2.0/schema.json"))
 
     @classmethod
     def _set_defaults(cls, spec):
-        spec.setdefault('produces', [])
-        spec.setdefault('consumes', ['application/json'])
-        spec.setdefault('definitions', {})
-        spec.setdefault('parameters', {})
-        spec.setdefault('responses', {})
+        spec.setdefault("produces", [])
+        spec.setdefault("consumes", ["application/json"])
+        spec.setdefault("definitions", {})
+        spec.setdefault("parameters", {})
+        spec.setdefault("responses", {})
 
     @property
     def produces(self):
-        return self._spec['produces']
+        return self._spec["produces"]
 
     @property
     def consumes(self):
-        return self._spec['consumes']
+        return self._spec["consumes"]
 
     @property
     def definitions(self):
-        return self._spec['definitions']
+        return self._spec["definitions"]
 
     @property
     def parameter_definitions(self):
-        return self._spec['parameters']
+        return self._spec["parameters"]
 
     @property
     def response_definitions(self):
-        return self._spec['responses']
+        return self._spec["responses"]
 
     @property
     def security_definitions(self):
-        return self._spec.get('securityDefinitions', {})
+        return self._spec.get("securityDefinitions", {})
 
     @property
     def base_path(self):
-        return canonical_base_path(self._spec.get('basePath', ''))
+        return canonical_base_path(self._spec.get("basePath", ""))
 
     @base_path.setter
     def base_path(self, base_path):
         base_path = canonical_base_path(base_path)
-        self._raw_spec['basePath'] = base_path
-        self._spec['basePath'] = base_path
+        self._raw_spec["basePath"] = base_path
+        self._spec["basePath"] = base_path
 
 
 class OpenAPISpecification(Specification):
     """Python interface for an OpenAPI 3 specification."""
 
-    yaml_name = 'openapi.yaml'
+    yaml_name = "openapi.yaml"
     operation_cls = OpenAPIOperation
 
-    openapi_schema = json.loads(
-        pkgutil.get_data('firetail', 'resources/schemas/v3.0/schema.json')
-    )
+    openapi_schema = json.loads(pkgutil.get_data("firetail", "resources/schemas/v3.0/schema.json"))
 
     @classmethod
     def _set_defaults(cls, spec):
-        spec.setdefault('components', {})
+        spec.setdefault("components", {})
 
     @property
     def security_definitions(self):
-        return self._spec['components'].get('securitySchemes', {})
+        return self._spec["components"].get("securitySchemes", {})
 
     @property
     def components(self):
-        return self._spec['components']
+        return self._spec["components"]
 
     @property
     def base_path(self):
-        servers = self._spec.get('servers', [])
+        servers = self._spec.get("servers", [])
         try:
             # assume we're the first server in list
             server = copy.deepcopy(servers[0])
             server_vars = server.pop("variables", {})
-            server['url'] = server['url'].format(
-                **{k: v['default'] for k, v
-                   in server_vars.items()}
-            )
-            base_path = urlsplit(server['url']).path
+            server["url"] = server["url"].format(**{k: v["default"] for k, v in server_vars.items()})
+            base_path = urlsplit(server["url"]).path
         except IndexError:
-            base_path = ''
+            base_path = ""
         return canonical_base_path(base_path)
 
     @base_path.setter
     def base_path(self, base_path):
         base_path = canonical_base_path(base_path)
-        user_servers = [{'url': base_path}]
-        self._raw_spec['servers'] = user_servers
-        self._spec['servers'] = user_servers
+        user_servers = [{"url": base_path}]
+        self._raw_spec["servers"] = user_servers
+        self._spec["servers"] = user_servers
```

### Comparing `firetail-1.0.8/firetail/utils.py` & `firetail-1.0.9/firetail/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,41 +17,43 @@
     True
 
     >>> boolean('false')
     False
     """
     if isinstance(s, bool):
         return s
-    elif not hasattr(s, 'lower'):
-        raise ValueError('Invalid boolean value')
-    elif s.lower() == 'true':
+    elif not hasattr(s, "lower"):
+        raise ValueError("Invalid boolean value")
+    elif s.lower() == "true":
         return True
-    elif s.lower() == 'false':
+    elif s.lower() == "false":
         return False
     else:
-        raise ValueError('Invalid boolean value')
+        raise ValueError("Invalid boolean value")
 
 
 # https://github.com/swagger-api/swagger-spec/blob/master/versions/2.0.md#data-types
-TYPE_MAP = {'integer': int,
-            'number': float,
-            'string': str,
-            'boolean': boolean,
-            'array': list,
-            'object': dict}  # map of swagger types to python types
+TYPE_MAP = {
+    "integer": int,
+    "number": float,
+    "string": str,
+    "boolean": boolean,
+    "array": list,
+    "object": dict,
+}  # map of swagger types to python types
 
 
 def make_type(value, _type):
     type_func = TYPE_MAP[_type]  # convert value to right type
     return type_func(value)
 
 
 def deep_merge(a, b):
-    """ merges b into a
-        in case of conflict the value from b is used
+    """merges b into a
+    in case of conflict the value from b is used
     """
     for key in b:
         if key in a:
             if isinstance(a[key], dict) and isinstance(b[key], dict):
                 deep_merge(a[key], b[key])
             elif a[key] == b[key]:
                 pass
@@ -64,15 +66,15 @@
 
 
 def deep_getattr(obj, attr):
     """
     Recurses through an attribute chain to get the ultimate value.
     """
 
-    attrs = attr.split('.')
+    attrs = attr.split(".")
 
     return functools.reduce(getattr, attrs, obj)
 
 
 def deep_get(obj, keys):
     """
     Recurses through a nested object get a leaf value.
@@ -98,31 +100,31 @@
     Tries to get function by fully qualified name (e.g. "mymodule.myobj.myfunc")
 
     :type function_name: str
     """
     if function_name is None:
         raise ValueError("Empty function name")
 
-    if '.' in function_name:
-        module_name, attr_path = function_name.rsplit('.', 1)
+    if "." in function_name:
+        module_name, attr_path = function_name.rsplit(".", 1)
     else:
-        module_name = ''
+        module_name = ""
         attr_path = function_name
 
     module = None
     last_import_error = None
 
     while not module:
         try:
             module = importlib.import_module(module_name)
         except ImportError as import_error:
             last_import_error = import_error
-            if '.' in module_name:
-                module_name, attr_path1 = module_name.rsplit('.', 1)
-                attr_path = f'{attr_path1}.{attr_path}'
+            if "." in module_name:
+                module_name, attr_path1 = module_name.rsplit(".", 1)
+                attr_path = f"{attr_path1}.{attr_path}"
             else:
                 raise
     try:
         function = deep_getattr(module, attr_path)
     except AttributeError:
         if last_import_error:
             raise last_import_error
@@ -132,16 +134,16 @@
 
 
 def is_json_mimetype(mimetype):
     """
     :type mimetype: str
     :rtype: bool
     """
-    maintype, subtype = mimetype.split('/')  # type: str, str
-    return maintype == 'application' and (subtype == 'json' or subtype.endswith('+json'))
+    maintype, subtype = mimetype.split("/")  # type: str, str
+    return maintype == "application" and (subtype == "json" or subtype.endswith("+json"))
 
 
 def all_json(mimetypes):
     """
     Returns True if all mimetypes are serialized with json
 
     :type mimetypes: list
@@ -162,90 +164,85 @@
     >>> all_json(['application/json', 'application/x.custom+json'])
     True
     """
     return all(is_json_mimetype(mimetype) for mimetype in mimetypes)
 
 
 def is_nullable(param_def):
-    return (
-        param_def.get('schema', param_def).get('nullable', False) or
-        param_def.get('x-nullable', False)  # swagger2
-    )
+    return param_def.get("schema", param_def).get("nullable", False) or param_def.get("x-nullable", False)  # swagger2
 
 
 def is_null(value):
-    if hasattr(value, 'strip') and value.strip() in ['null', 'None']:
+    if hasattr(value, "strip") and value.strip() in ["null", "None"]:
         return True
 
     if value is None:
         return True
 
     return False
 
 
 def has_coroutine(function, api=None):
     """
     Checks if function is a coroutine.
     If ``function`` is a decorator (has a ``__wrapped__`` attribute)
     this function will also look at the wrapped function.
     """
+
     def iscorofunc(func):
         iscorofunc = asyncio.iscoroutinefunction(func)
-        while not iscorofunc and hasattr(func, '__wrapped__'):
+        while not iscorofunc and hasattr(func, "__wrapped__"):
             func = func.__wrapped__
             iscorofunc = asyncio.iscoroutinefunction(func)
         return iscorofunc
 
     if api is None:
         return iscorofunc(function)
 
     else:
-        return any(
-            iscorofunc(func) for func in (
-                function, api.get_request, api.get_response
-            )
-        )
+        return any(iscorofunc(func) for func in (function, api.get_request, api.get_response))
 
 
 def yamldumper(openapi):
     """
     Returns a nicely-formatted yaml spec.
     :param openapi: a spec dictionary.
     :return: a nicely-formatted, serialized yaml spec.
     """
+
     def should_use_block(value):
         char_list = (
-          "\u000a"  # line feed
-          "\u000d"  # carriage return
-          "\u001c"  # file separator
-          "\u001d"  # group separator
-          "\u001e"  # record separator
-          "\u0085"  # next line
-          "\u2028"  # line separator
-          "\u2029"  # paragraph separator
+            "\u000a"  # line feed
+            "\u000d"  # carriage return
+            "\u001c"  # file separator
+            "\u001d"  # group separator
+            "\u001e"  # record separator
+            "\u0085"  # next line
+            "\u2028"  # line separator
+            "\u2029"  # paragraph separator
         )
         for c in char_list:
             if c in value:
                 return True
         return False
 
     def my_represent_scalar(self, tag, value, style=None):
         if should_use_block(value):
-            style = '|'
+            style = "|"
         else:
             style = self.default_style
 
         node = yaml.representer.ScalarNode(tag, value, style=style)
         if self.alias_key is not None:
             self.represented_objects[self.alias_key] = node
         return node
 
     class NoAnchorDumper(yaml.dumper.SafeDumper):
         """A yaml Dumper that does not replace duplicate entries
-           with yaml anchors.
+        with yaml anchors.
         """
 
         def ignore_aliases(self, *args):
             return True
 
     # Dump long lines as "|".
     yaml.representer.SafeRepresenter.represent_scalar = my_represent_scalar
```

### Comparing `firetail-1.0.8/firetail.egg-info/PKG-INFO` & `firetail-1.0.9/firetail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firetail
-Version: 1.0.8
+Version: 1.0.9
 Summary: Firetail - API first applications with OpenAPI/Swagger and Flask
 Home-page: https://github.com/FireTail-io/firetail-py-lib
 Author: FireTail International (TM)
 License: LGPLv3
 Keywords: openapi oai swagger rest api oauth flask microservice framework
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `firetail-1.0.8/firetail.egg-info/SOURCES.txt` & `firetail-1.0.9/firetail.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+dev-requirements.txt
+requirements.txt
 setup.cfg
 setup.py
 firetail/__init__.py
 firetail/__main__.py
 firetail/auditor.py
 firetail/cli.py
 firetail/exceptions.py
```

### Comparing `firetail-1.0.8/firetail.egg-info/requires.txt` & `firetail-1.0.9/firetail.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 clickclick<21,>=1.2
 jsonschema<5,>=4.0.1
-PyYAML<7,>=5.1
-PyJWT>=2.3.0
-requests<3,>=2.27
+PyYAML<7,>=5.4
+PyJWT>=2.4.0
+requests<3,>=2.31
 inflection<0.6,>=0.3.1
-werkzeug<3,>=2.2.1
-starlette<1,>=0.15
+werkzeug<3,>=2.2.2
+starlette<1,>=0.27
 flask[async]<3,>=2.2
 a2wsgi<2,>=1.4
 
 [docs]
 sphinx-autoapi==1.8.1
 
 [flask]
```

### Comparing `firetail-1.0.8/setup.py` & `firetail-1.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,126 +7,116 @@
 from setuptools import find_packages, setup
 from setuptools.command.test import test as TestCommand
 
 __location__ = os.path.join(os.getcwd(), os.path.dirname(inspect.getfile(inspect.currentframe())))
 
 
 def read_version(package):
-    with open(os.path.join(package, '__init__.py')) as fd:
+    with open(os.path.join(package, "__init__.py")) as fd:
         for line in fd:
-            if line.startswith('__version__ = '):
+            if line.startswith("__version__ = "):
                 return line.split()[-1].strip().strip("'")
 
 
-version = read_version('firetail')
+version = read_version("firetail")
 
 install_requires = [
-    'clickclick>=1.2,<21',
-    'jsonschema>=4.0.1,<5',
-    'PyYAML>=5.1,<7',
-    'PyJWT>=2.3.0',
-    'requests>=2.27,<3',
-    'inflection>=0.3.1,<0.6',
-    'werkzeug>=2.2.1,<3',
-    'starlette>=0.15,<1',
+    "clickclick>=1.2,<21",
+    "jsonschema>=4.0.1,<5",
+    "PyYAML>=5.4,<7",
+    "PyJWT>=2.4.0",
+    "requests>=2.31,<3",
+    "inflection>=0.3.1,<0.6",
+    "werkzeug>=2.2.2,<3",
+    "starlette>=0.27,<1",
 ]
 
-swagger_ui_require = 'swagger-ui-bundle>=0.0.2,<0.1'
+swagger_ui_require = "swagger-ui-bundle>=0.0.2,<0.1"
 
 flask_require = [
-    'flask[async]>=2.2,<3',
-    'a2wsgi>=1.4,<2',
+    "flask[async]>=2.2,<3",
+    "a2wsgi>=1.4,<2",
 ]
 
 aiohttp_require = [
-    'aiohttp>=2.3.10,<4',
-    'aiohttp-jinja2>=0.14.0,<2',
-    'MarkupSafe>=0.23',
+    "aiohttp>=2.3.10,<4",
+    "aiohttp-jinja2>=0.14.0,<2",
+    "MarkupSafe>=0.23",
 ]
 
-tests_require = [
-    'pytest>=6,<7',
-    'pytest-cov>=2,<3',
-    'testfixtures>=6,<7',
-    *flask_require,
-    swagger_ui_require
-]
+tests_require = ["pytest>=6,<7", "pytest-cov>=2,<3", "testfixtures>=6,<7", *flask_require, swagger_ui_require]
 
 tests_require.extend(aiohttp_require)
-tests_require.append('pytest-aiohttp')
-tests_require.append('aiohttp-remotes')
+tests_require.append("pytest-aiohttp")
+tests_require.append("aiohttp-remotes")
 
-docs_require = [
-    'sphinx-autoapi==1.8.1'
-]
+docs_require = ["sphinx-autoapi==1.8.1"]
 
 
 class PyTest(TestCommand):
-
-    user_options = [('cov-html=', None, 'Generate junit html report')]
+    user_options = [("cov-html=", None, "Generate junit html report")]
 
     def initialize_options(self):
         TestCommand.initialize_options(self)
         self.cov = None
-        self.pytest_args = ['--cov', 'firetail',
-                            '--cov-report', 'term-missing', '-v']
+        self.pytest_args = ["--cov", "firetail", "--cov-report", "term-missing", "-v"]
         self.cov_html = False
 
     def finalize_options(self):
         TestCommand.finalize_options(self)
         if self.cov_html:
-            self.pytest_args.extend(['--cov-report', 'html'])
-        self.pytest_args.extend(['tests'])
+            self.pytest_args.extend(["--cov-report", "html"])
+        self.pytest_args.extend(["tests"])
 
     def run_tests(self):
         import pytest
 
         errno = pytest.main(self.pytest_args)
         sys.exit(errno)
 
 
 def readme():
     try:
-        return open('README.rst', encoding='utf-8').read()
+        return open("README.rst", encoding="utf-8").read()
     except TypeError:
-        return open('README.rst').read()
+        return open("README.rst").read()
 
 
 setup(
-    name='firetail',
+    name="firetail",
     packages=find_packages(),
     version=version,
-    description='Firetail - API first applications with OpenAPI/Swagger and Flask',
+    description="Firetail - API first applications with OpenAPI/Swagger and Flask",
     long_description=readme(),
     # long_description_content_type="text/x-rst",
-    author='FireTail International (TM)',
-    url='https://github.com/FireTail-io/firetail-py-lib',
-    keywords='openapi oai swagger rest api oauth flask microservice framework',
-    license='LGPLv3',
+    author="FireTail International (TM)",
+    url="https://github.com/FireTail-io/firetail-py-lib",
+    keywords="openapi oai swagger rest api oauth flask microservice framework",
+    license="LGPLv3",
     # setup_requires=['flake8'],
     python_requires=">=3.6",
     install_requires=install_requires + flask_require,
     tests_require=tests_require,
     extras_require={
-        'tests': tests_require,
-        'flask': flask_require,
-        'swagger-ui': swagger_ui_require,
-        'docs': docs_require
+        "tests": tests_require,
+        "flask": flask_require,
+        "swagger-ui": swagger_ui_require,
+        "docs": docs_require,
     },
-    cmdclass={'test': PyTest},
-    test_suite='tests',
+    cmdclass={"test": PyTest},
+    test_suite="tests",
     classifiers=[
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Operating System :: OS Independent',
-        'Topic :: Internet :: WWW/HTTP :: WSGI :: Application',
-        'Topic :: Software Development :: Libraries :: Application Frameworks'
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Operating System :: OS Independent",
+        "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
     ],
     # needed to include swagger-ui (see MANIFEST.in)
     include_package_data=True,
-    entry_points={'console_scripts': ['Firetail = Firetail.cli:main']}
+    entry_points={"console_scripts": ["Firetail = Firetail.cli:main"]},
 )
```

