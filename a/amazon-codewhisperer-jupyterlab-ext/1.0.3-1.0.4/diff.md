# Comparing `tmp/amazon-codewhisperer-jupyterlab-ext-1.0.3.tar.gz` & `tmp/amazon-codewhisperer-jupyterlab-ext-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-codewhisperer-jupyterlab-ext-1.0.3.tar", last modified: Fri Jun  9 16:25:20 2023, max compression
+gzip compressed data, was "amazon-codewhisperer-jupyterlab-ext-1.0.4.tar", last modified: Fri Jul 14 18:41:14 2023, max compression
```

## Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3.tar` & `amazon-codewhisperer-jupyterlab-ext-1.0.4.tar`

### file list

```diff
@@ -1,143 +1,181 @@
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.903294 amazon-codewhisperer-jupyterlab-ext-1.0.3/
--rw-r--r--   0 zoelin     (505) staff       (20)    11357 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/LICENSE
--rw-r--r--   0 zoelin     (505) staff       (20)      503 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/MANIFEST.in
--rw-r--r--   0 zoelin     (505) staff       (20)      103 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/NOTICE
--rw-r--r--   0 zoelin     (505) staff       (20)     5210 2023-06-09 16:25:20.902803 amazon-codewhisperer-jupyterlab-ext-1.0.3/PKG-INFO
--rw-r--r--   0 zoelin     (505) staff       (20)     4309 2023-06-09 16:24:07.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/README.md
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.855773 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/
--rw-r--r--   0 zoelin     (505) staff       (20)     1039 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/__init__.py
--rw-r--r--   0 zoelin     (505) staff       (20)      443 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/_version.py
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.859841 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/auth/
--rw-r--r--   0 zoelin     (505) staff       (20)       98 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/auth/__init__.py
--rw-r--r--   0 zoelin     (505) staff       (20)     3422 2023-06-08 22:48:03.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/auth/sso_auth_manager.py
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.860757 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/
--rw-r--r--   0 zoelin     (505) staff       (20)        0 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/__init__.py
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.862714 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/
--rw-r--r--   0 zoelin     (505) staff       (20)      281 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/__init__.py
--rw-r--r--   0 zoelin     (505) staff       (20)     1277 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/client_manager.py
--rw-r--r--   0 zoelin     (505) staff       (20)      794 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/iam_client_manager.py
--rw-r--r--   0 zoelin     (505) staff       (20)     1395 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/sso_client_manager.py
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.839493 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.838622 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.863279 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/
--rw-r--r--   0 zoelin     (505) staff       (20)    15547 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.839234 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.863946 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/
--rw-r--r--   0 zoelin     (505) staff       (20)    24832 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.839638 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.864558 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/
--rw-r--r--   0 zoelin     (505) staff       (20)     4536 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.865497 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/telemetry/
--rw-r--r--   0 zoelin     (505) staff       (20)       72 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/telemetry/__init__.py
--rw-r--r--   0 zoelin     (505) staff       (20)     3443 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py
--rw-r--r--   0 zoelin     (505) staff       (20)     1732 2023-06-09 16:24:07.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/constants.py
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.866791 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/env/
--rw-r--r--   0 zoelin     (505) staff       (20)       64 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/env/__init__.py
--rw-r--r--   0 zoelin     (505) staff       (20)     1660 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/env/environment.py
--rw-r--r--   0 zoelin     (505) staff       (20)     7057 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/handlers.py
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.867414 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/
--rw-r--r--   0 zoelin     (505) staff       (20)     5188 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/package.json
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.841002 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.868220 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/
--rw-r--r--   0 zoelin     (505) staff       (20)     2661 2023-06-09 16:25:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json
--rw-r--r--   0 zoelin     (505) staff       (20)     5046 2023-06-09 16:25:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.871505 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/
--rw-r--r--   0 zoelin     (505) staff       (20)    79921 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.c0e5b626da6cbe06eb5e.js
--rw-r--r--   0 zoelin     (505) staff       (20)      368 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.c0e5b626da6cbe06eb5e.js.LICENSE.txt
--rw-r--r--   0 zoelin     (505) staff       (20)     6607 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.3582fd184eff1ff4b836.js
--rw-r--r--   0 zoelin     (505) staff       (20)     5640 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.462ff5e5d49d87208721.js
--rw-r--r--   0 zoelin     (505) staff       (20)     8370 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.9bf04351778104e8e5cd.js
--rw-r--r--   0 zoelin     (505) staff       (20)      178 2023-06-09 16:25:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/style.js
--rw-r--r--   0 zoelin     (505) staff       (20)     5075 2023-06-09 16:25:18.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json
--rw-r--r--   0 zoelin     (505) staff       (20)     2715 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/utils.py
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.872532 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/
--rw-r--r--   0 zoelin     (505) staff       (20)       67 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/__init__.py
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.873091 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/schemas/
--rw-r--r--   0 zoelin     (505) staff       (20)     1286 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json
--rw-r--r--   0 zoelin     (505) staff       (20)      782 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/validator.py
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.858847 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/
--rw-r--r--   0 zoelin     (505) staff       (20)     5210 2023-06-09 16:25:20.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO
--rw-r--r--   0 zoelin     (505) staff       (20)     4229 2023-06-09 16:25:20.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt
--rw-r--r--   0 zoelin     (505) staff       (20)        1 2023-06-09 16:25:20.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/dependency_links.txt
--rw-r--r--   0 zoelin     (505) staff       (20)        1 2023-06-06 01:34:05.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/not-zip-safe
--rw-r--r--   0 zoelin     (505) staff       (20)       15 2023-06-09 16:25:20.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/requires.txt
--rw-r--r--   0 zoelin     (505) staff       (20)       36 2023-06-09 16:25:20.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/top_level.txt
--rw-r--r--   0 zoelin     (505) staff       (20)      231 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/install.json
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.873713 amazon-codewhisperer-jupyterlab-ext-1.0.3/jupyter-config/
--rw-r--r--   0 zoelin     (505) staff       (20)      119 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/jupyter-config/amazon_codewhisperer_jupyterlab_ext.json
--rw-r--r--   0 zoelin     (505) staff       (20)     5046 2023-06-09 16:24:07.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/package.json
--rw-r--r--   0 zoelin     (505) staff       (20)      675 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/pyproject.toml
--rw-r--r--   0 zoelin     (505) staff       (20)       38 2023-06-09 16:25:20.903421 amazon-codewhisperer-jupyterlab-ext-1.0.3/setup.cfg
--rw-r--r--   0 zoelin     (505) staff       (20)     2716 2023-06-09 00:41:39.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/setup.py
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.877266 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.877806 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.878348 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/autotrigger/
--rw-r--r--   0 zoelin     (505) staff       (20)     2034 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/autotrigger/autotrigger.spec.ts
--rw-r--r--   0 zoelin     (505) staff       (20)      109 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/index.spec.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.879316 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/recommendation/
--rw-r--r--   0 zoelin     (505) staff       (20)     5855 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/recommendation/recommendationStateHandler.spec.ts
--rw-r--r--   0 zoelin     (505) staff       (20)     2789 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/application.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.880312 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/auth/
--rw-r--r--   0 zoelin     (505) staff       (20)     9598 2023-06-08 22:48:03.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/auth/authManager.tsx
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.881092 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/autotrigger/
--rw-r--r--   0 zoelin     (505) staff       (20)     6990 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/autotrigger/autotrigger.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.882715 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/aws_vector_consolas_jupyter_lab3_extension/
--rw-r--r--   0 zoelin     (505) staff       (20)       28 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/aws_vector_consolas_jupyter_lab3_extension/__init__.py
--rw-r--r--   0 zoelin     (505) staff       (20)       58 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/aws_vector_consolas_jupyter_lab3_extension/py.typed
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.885084 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/
--rw-r--r--   0 zoelin     (505) staff       (20)     1811 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/apiclient.ts
--rw-r--r--   0 zoelin     (505) staff       (20)    15283 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/codewhispererclient.d.ts
--rw-r--r--   0 zoelin     (505) staff       (20)     7900 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/codewhispereruserclient.d.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.886554 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/connector/
--rw-r--r--   0 zoelin     (505) staff       (20)     2252 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/connector/codewhispererconnector.ts
--rw-r--r--   0 zoelin     (505) staff       (20)     2687 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/connector/mergeconnector.ts
--rw-r--r--   0 zoelin     (505) staff       (20)     1225 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/handler.ts
--rw-r--r--   0 zoelin     (505) staff       (20)     2444 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/icons.ts
--rw-r--r--   0 zoelin     (505) staff       (20)    13178 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/index.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.887189 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/inline/
--rw-r--r--   0 zoelin     (505) staff       (20)    26396 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/inline/inline.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.887826 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/keybindings/
--rw-r--r--   0 zoelin     (505) staff       (20)      937 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/keybindings/keybindings.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.888427 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/logging/
--rw-r--r--   0 zoelin     (505) staff       (20)      524 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/logging/logger.tsx
--rw-r--r--   0 zoelin     (505) staff       (20)      127 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/messages.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.888975 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/notifications/
--rw-r--r--   0 zoelin     (505) staff       (20)     3833 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/notifications/notifications.tsx
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.890334 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/
--rw-r--r--   0 zoelin     (505) staff       (20)     4707 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/extractor.ts
--rw-r--r--   0 zoelin     (505) staff       (20)    11143 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/recommendationStateHandler.ts
--rw-r--r--   0 zoelin     (505) staff       (20)    10773 2023-06-08 22:48:03.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/worker.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.890818 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/referencetracker/
--rw-r--r--   0 zoelin     (505) staff       (20)     3067 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/referencetracker/referencetracker.tsx
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.891267 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/statusbar/
--rw-r--r--   0 zoelin     (505) staff       (20)    14594 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/statusbar/statusbarwidget.tsx
--rw-r--r--   0 zoelin     (505) staff       (20)       78 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/svg.d.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.893516 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/
--rw-r--r--   0 zoelin     (505) staff       (20)     4333 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/clienttelemetry.d.ts
--rw-r--r--   0 zoelin     (505) staff       (20)   150822 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetry.gen.ts
--rw-r--r--   0 zoelin     (505) staff       (20)     4292 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetry.ts
--rw-r--r--   0 zoelin     (505) staff       (20)      899 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetryClient.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.895973 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/
--rw-r--r--   0 zoelin     (505) staff       (20)     3508 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/constants.ts
--rw-r--r--   0 zoelin     (505) staff       (20)      359 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/licenseUtils.ts
--rw-r--r--   0 zoelin     (505) staff       (20)     1135 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/models.ts
--rw-r--r--   0 zoelin     (505) staff       (20)      292 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/stateKeys.ts
--rw-r--r--   0 zoelin     (505) staff       (20)     2974 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/utils.ts
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.897701 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/
--rw-r--r--   0 zoelin     (505) staff       (20)     2123 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/base.css
-drwxr-xr-x   0 zoelin     (505) staff       (20)        0 2023-06-09 16:25:20.902311 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/
--rw-r--r--   0 zoelin     (505) staff       (20)     3451 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/codewhisperer.svg
--rw-r--r--   0 zoelin     (505) staff       (20)      234 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/connected.svg
--rw-r--r--   0 zoelin     (505) staff       (20)      767 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/disconnected.svg
--rw-r--r--   0 zoelin     (505) staff       (20)      222 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/documentation.svg
--rw-r--r--   0 zoelin     (505) staff       (20)      234 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/loading.svg
--rw-r--r--   0 zoelin     (505) staff       (20)      746 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/log.svg
--rw-r--r--   0 zoelin     (505) staff       (20)      420 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/pause.svg
--rw-r--r--   0 zoelin     (505) staff       (20)      463 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/resume.svg
--rw-r--r--   0 zoelin     (505) staff       (20)      660 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/signout.svg
--rw-r--r--   0 zoelin     (505) staff       (20)      379 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/start.svg
--rw-r--r--   0 zoelin     (505) staff       (20)      599 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/visual-cue-arrow.svg
--rw-r--r--   0 zoelin     (505) staff       (20)       25 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/index.css
--rw-r--r--   0 zoelin     (505) staff       (20)       21 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/style/index.js
--rw-r--r--   0 zoelin     (505) staff       (20)      658 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/tsconfig.json
--rw-r--r--   0 zoelin     (505) staff       (20)       33 2023-06-06 00:10:34.000000 amazon-codewhisperer-jupyterlab-ext-1.0.3/tsconfig.test.json
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.493477 amazon-codewhisperer-jupyterlab-ext-1.0.4/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    11357 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/LICENSE
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      503 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/MANIFEST.in
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      103 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/NOTICE
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     5252 2023-07-14 18:41:14.492605 amazon-codewhisperer-jupyterlab-ext-1.0.4/PKG-INFO
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     4351 2023-07-13 19:44:28.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/README.md
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.363574 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     1039 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/__init__.py
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      443 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/_version.py
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.372686 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/auth/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       98 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/auth/__init__.py
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     3422 2023-07-06 19:59:35.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/auth/sso_auth_manager.py
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.373906 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)        0 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/__init__.py
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.377699 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      281 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/__init__.py
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     1277 2023-05-24 08:59:05.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/client_manager.py
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      794 2023-05-24 08:59:05.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/iam_client_manager.py
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     1395 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/sso_client_manager.py
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.339513 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.338737 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.378422 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    15547 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.339213 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.379286 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    24832 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.339741 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.380337 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     4536 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.382193 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/telemetry/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       72 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/telemetry/__init__.py
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     3443 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     1879 2023-07-13 19:44:28.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/constants.py
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.383913 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/env/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       64 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/env/__init__.py
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2097 2023-07-11 20:29:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/env/environment.py
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     7057 2023-07-12 21:53:39.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/handlers.py
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.385262 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     5188 2023-07-14 18:41:10.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/package.json
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.341179 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.386324 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2661 2023-07-14 18:41:08.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     5046 2023-07-14 18:41:08.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.391330 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    82632 2023-07-14 18:41:10.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.5e4ac436f86b65d9e70f.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      368 2023-07-14 18:41:10.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.5e4ac436f86b65d9e70f.js.LICENSE.txt
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     6607 2023-07-14 18:41:10.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.3582fd184eff1ff4b836.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     6047 2023-07-14 18:41:10.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.4a2fe27171322cd7b67e.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     8370 2023-07-14 18:41:10.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.f27b2e72fdec8f3ccdff.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      178 2023-07-14 18:41:08.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/style.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     5075 2023-07-14 18:41:10.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2715 2023-05-10 03:22:51.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/utils.py
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.392909 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/validator/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       67 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/validator/__init__.py
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.394276 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/validator/schemas/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     1286 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      782 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/validator/validator.py
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.371016 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext.egg-info/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     5252 2023-07-14 18:41:14.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     5335 2023-07-14 18:41:14.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 yuxqiang   (505) staff       (20)        1 2023-07-14 18:41:14.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 yuxqiang   (505) staff       (20)        1 2023-05-08 03:26:53.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext.egg-info/not-zip-safe
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       15 2023-07-14 18:41:14.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext.egg-info/requires.txt
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       36 2023-07-14 18:41:14.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext.egg-info/top_level.txt
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      231 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/install.json
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.396716 amazon-codewhisperer-jupyterlab-ext-1.0.4/jupyter-config/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      119 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/jupyter-config/amazon_codewhisperer_jupyterlab_ext.json
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     5046 2023-07-13 19:44:28.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/package.json
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      675 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/pyproject.toml
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       38 2023-07-14 18:41:14.493796 amazon-codewhisperer-jupyterlab-ext-1.0.4/setup.cfg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2716 2023-05-08 19:59:53.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/setup.py
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.411630 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.412466 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/__tests__/
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.413531 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/__tests__/autotrigger/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2034 2023-05-08 19:59:53.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/__tests__/autotrigger/autotrigger.spec.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      109 2023-05-08 19:59:53.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/__tests__/index.spec.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.417147 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/__tests__/recommendation/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     6333 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/__tests__/recommendation/recommendationStateHandler.spec.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     3697 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/__tests__/recommendation/recommendationStateHandler.spec.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     5855 2023-05-22 17:48:21.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/__tests__/recommendation/recommendationStateHandler.spec.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     6731 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/application.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     1883 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/application.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     3183 2023-07-12 18:34:07.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/application.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.419175 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/auth/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     9594 2023-07-12 17:18:41.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/auth/authManager.tsx
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.425351 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/autotrigger/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     9806 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/autotrigger/autotrigger.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     4520 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/autotrigger/autotrigger.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     6990 2023-05-08 19:59:53.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/autotrigger/autotrigger.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.427185 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/aws_vector_consolas_jupyter_lab3_extension/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       28 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/aws_vector_consolas_jupyter_lab3_extension/__init__.py
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       58 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/aws_vector_consolas_jupyter_lab3_extension/py.typed
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.432038 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/client/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     4154 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/client/apiclient.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      724 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/client/apiclient.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     1811 2023-07-12 21:57:06.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/client/apiclient.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    15283 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/client/codewhispererclient.d.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     7900 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/client/codewhispereruserclient.d.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.433524 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/connector/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2252 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/connector/codewhispererconnector.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2687 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/connector/mergeconnector.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     4283 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/handler.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      783 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/handler.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     1225 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/handler.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2712 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/icons.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     1373 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/icons.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2444 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/icons.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    13231 2023-07-11 20:29:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/index.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.437774 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/inline/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    30765 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/inline/inline.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    19624 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/inline/inline.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    26396 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/inline/inline.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.439042 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/keybindings/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      937 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/keybindings/keybindings.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.439941 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/logging/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      524 2023-05-22 17:48:21.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/logging/logger.tsx
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      239 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/messages.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      235 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/messages.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      127 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/messages.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.441239 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/notifications/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     3833 2023-07-11 20:29:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/notifications/notifications.tsx
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.449922 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     4522 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/extractor.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     3872 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/extractor.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     4707 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/extractor.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    11952 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/recommendationStateHandler.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     6395 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/recommendationStateHandler.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    11143 2023-05-22 17:48:21.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/recommendationStateHandler.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    15660 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/worker.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     5920 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/worker.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    10893 2023-07-11 20:29:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/worker.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.450853 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/referencetracker/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     3067 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/referencetracker/referencetracker.tsx
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.451490 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/statusbar/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    18346 2023-07-14 18:40:36.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/statusbar/statusbarwidget.tsx
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       78 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/svg.d.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.463436 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     4333 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/clienttelemetry.d.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)   115455 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetry.gen.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)    53762 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetry.gen.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)   150822 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetry.gen.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     8017 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetry.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     3070 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetry.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     4381 2023-07-11 20:29:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetry.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     4110 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetryClient.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      626 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetryClient.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      899 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetryClient.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.481666 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     4576 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/constants.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     1946 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/constants.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     3659 2023-07-11 20:29:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/constants.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      569 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/licenseUtils.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      440 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/licenseUtils.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      359 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/licenseUtils.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       75 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/models.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       97 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/models.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     1135 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/models.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      482 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/stateKeys.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      240 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/stateKeys.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      292 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/stateKeys.ts
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     7234 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/utils.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2295 2023-07-12 21:36:59.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/utils.js.map
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2974 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/utils.ts
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.483581 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     2510 2023-07-11 20:29:16.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/base.css
+drwxr-xr-x   0 yuxqiang   (505) staff       (20)        0 2023-07-14 18:41:14.491686 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/
+-rw-r--r--   0 yuxqiang   (505) staff       (20)     3451 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/codewhisperer.svg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      234 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/connected.svg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      767 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/disconnected.svg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      222 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/documentation.svg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      234 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/loading.svg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      746 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/log.svg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      420 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/pause.svg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      463 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/resume.svg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      660 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/signout.svg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      379 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/start.svg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      599 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/visual-cue-arrow.svg
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       25 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/index.css
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       21 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/style/index.js
+-rw-r--r--   0 yuxqiang   (505) staff       (20)      658 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/tsconfig.json
+-rw-r--r--   0 yuxqiang   (505) staff       (20)       33 2023-05-08 03:24:04.000000 amazon-codewhisperer-jupyterlab-ext-1.0.4/tsconfig.test.json
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/LICENSE` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/PKG-INFO` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-codewhisperer-jupyterlab-ext
-Version: 1.0.3
+Version: 1.0.4
 Summary: Amazon CodeWhisperer for JupyterLab
 Home-page: https://aws.amazon.com/codewhisperer/
 Author: Amazon CodeWhisperer
 Author-email: codewhisperer@amazon.com
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Amazon CodeWhisperer,CodeWhisperer,Code,Whisperer
 Platform: Linux
@@ -93,14 +93,17 @@
 
 * [CodeWhisperer User Guide](https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html)
 * [Setting up Amazon CodeWhisperer with JupyterLab](https://docs.aws.amazon.com/codewhisperer/latest/userguide/jupyterlab-setup.html)
 * [Setting up CodeWhisperer with Amazon SageMaker Studio](https://docs.aws.amazon.com/codewhisperer/latest/userguide/sagemaker-setup.html)
 
 ## Change Log
 
+1.0.4
+* Add Glue Studio Notebook support
+
 1.0.3
 * Bug fix: No recommendation when user turn off code suggestions with references in settings.
 * Bug fix: Issue with browser login flow for some Builder ID users.
 * Bug fix: Fix an issue where SageMaker Studio users will incorrectly see the `Share content with Amazon CodeWhisperer` settings option.
 
 1.0.0
 * Initial release
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/README.md` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 
 * [CodeWhisperer User Guide](https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html)
 * [Setting up Amazon CodeWhisperer with JupyterLab](https://docs.aws.amazon.com/codewhisperer/latest/userguide/jupyterlab-setup.html)
 * [Setting up CodeWhisperer with Amazon SageMaker Studio](https://docs.aws.amazon.com/codewhisperer/latest/userguide/sagemaker-setup.html)
 
 ## Change Log
 
+1.0.4
+* Add Glue Studio Notebook support
+
 1.0.3
 * Bug fix: No recommendation when user turn off code suggestions with references in settings.
 * Bug fix: Issue with browser login flow for some Builder ID users.
 * Bug fix: Fix an issue where SageMaker Studio users will incorrectly see the `Share content with Amazon CodeWhisperer` settings option.
 
 1.0.0
 * Initial release
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/__init__.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/auth/sso_auth_manager.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/auth/sso_auth_manager.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/client_manager.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/client_manager.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/iam_client_manager.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/iam_client_manager.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/sso_client_manager.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/codewhisperer/sso_client_manager.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/bearer/2022-11-11/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/sigv4/2022-06-15/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/service_models/telemetry/2017-07-25/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/constants.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-CURRENT_VERSION = "1.0.3"
-# TODO : Update URL to CodeWhisperer PyPI JSON URL
+CURRENT_VERSION = "1.0.4"
 CODEWHISPERER_PYPI_JSON_URL = "https://pypi.org/pypi/amazon-codewhisperer-jupyterlab-ext/json"
 
 TELEMETRY_PROD_ENDPOINT = "https://client-telemetry.us-east-1.amazonaws.com"
 PROD_COGNITO_POOL_ID = "us-east-1:820fd6d1-95c0-4ca4-bffb-3f01d32da842"
 
 INVALID_TOKEN_EXCEPTION_MESSAGE = "The security token included in the request is expired"
 RTS_PROD_ENDPOINT = "https://codewhisperer.us-east-1.amazonaws.com/"
@@ -37,7 +36,11 @@
 SCOPES = ["codewhisperer:completions"]
 CLIENT_NAME = "CodeWhisperer for JupyterLab"
 CLIENT_REGISTRATION_TYPE = "public"
 DEVICE_GRANT_TYPE = "urn:ietf:params:oauth:grant-type:device_code"
 REFRESH_GRANT_TYPE = "refresh_token"
 SM_STUDIO_ENV_NAME = "SageMaker Studio"
 JUPYTER_OSS_ENV_NAME = "Jupyter OSS"
+
+# The environment variable to identify which instance is this (e.g. Glue Studio Notebook or SageMaker Studio)
+CONSUMER_ENV_KEY = "CONSUMER_ID"
+CONSUMER_ENV_VALUE_GLUE_STUDIO = "GlueStudioNotebook"
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/env/environment.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/env/environment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import json
 import os
 import requests
 from packaging.version import Version
-from amazon_codewhisperer_jupyterlab_ext.constants import CURRENT_VERSION, CODEWHISPERER_PYPI_JSON_URL, NEW_VERSION_USER_MESSAGE
+from amazon_codewhisperer_jupyterlab_ext.constants import CURRENT_VERSION, CODEWHISPERER_PYPI_JSON_URL, \
+    NEW_VERSION_USER_MESSAGE, CONSUMER_ENV_KEY, CONSUMER_ENV_VALUE_GLUE_STUDIO
+
 
 class Environment:
     SM_STUDIO = "SageMaker Studio"
     JUPYTER_OSS = "Jupyter OSS"
-
-    # TODO : Update version for new release to get notification
-    CURRENT_VERSION = "0.1.0"
+    GLUE_STUDIO_NOTEBOOK = "Glue Studio Notebook"
 
     @staticmethod
     def get_update_notification():
         try:
+            # Glue Studio environment doesn't want any update and update notification
+            if Environment.is_glue_studio():
+                return "", ""
+
             # Get the URL from environment variable or fall back to default
             url = os.environ.get("JSON_URL", CODEWHISPERER_PYPI_JSON_URL)
 
             # Download the JSON data
             response = requests.get(url)
             response.raise_for_status()
             data = response.json()
@@ -30,20 +34,26 @@
                 return NEW_VERSION_USER_MESSAGE.format(latest_version), latest_version
             else:
                 return "", ""
         except Exception as e:
             print(f"Error: {e}")
             return "", ""
     
-
     @staticmethod
     def get_environment():
         env = Environment.JUPYTER_OSS
         try:
+            if Environment.is_glue_studio():
+                return Environment.GLUE_STUDIO_NOTEBOOK
+
             with open('/opt/ml/metadata/resource-metadata.json', 'r') as f:
                 data = json.load(f)
                 if 'ResourceArn' in data:
                     env = Environment.SM_STUDIO
         except Exception as e:
             # Default to Builder ID / Jupyter OSS for all errors
             pass
         return env
+
+    @staticmethod
+    def is_glue_studio():
+        return CONSUMER_ENV_KEY in os.environ and os.environ.get(CONSUMER_ENV_KEY) == CONSUMER_ENV_VALUE_GLUE_STUDIO
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/handlers.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class RecommendationHandler(APIHandler, ABC):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         environment = Environment.get_environment()
         self.input_validator = InputValidator()
         self.codewhisperer_client = CodeWhispererIamClientManager() \
-            if environment == Environment.SM_STUDIO \
+            if environment != Environment.JUPYTER_OSS \
             else CodeWhispererSsoClientManager()
 
     @tornado.web.authenticated
     def post(self):
         input_data = self.get_json_body()
         try:
             if not self.input_validator.is_valid_input("generate_recommendations", input_data):
@@ -126,16 +126,16 @@
     @tornado.web.authenticated
     def get(self):
         update_notification, latest_version = Environment.get_update_notification()
         self.finish(json.dumps(ServiceResponse(
             ServiceResponseStatus.SUCCESS,
             {
                 'environment': Environment.get_environment(),
-                'version_notification' : update_notification,
-                'latest_version' : latest_version
+                'version_notification': update_notification,
+                'latest_version': latest_version
             },
             None,
             None,
             None
         ).__dict__))
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/package.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9757936507936508%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f27b2e72fdec8f3ccdff.js'}}",*

 * * "'version'": "'1.0.4'"}*

```diff
@@ -70,15 +70,15 @@
         "style/img/*.{svg}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/aws",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9bf04351778104e8e5cd.js",
+            "load": "static/remoteEntry.f27b2e72fdec8f3ccdff.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/completer-extension:notebooks",
             "@jupyterlab/completer-extension:files"
         ],
         "extension": true,
@@ -135,9 +135,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "1.0.4"
 }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.0.4'"}*

```diff
@@ -130,9 +130,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "1.0.4"
 }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.c0e5b626da6cbe06eb5e.js` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/568.5e4ac436f86b65d9e70f.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 568.c0e5b626da6cbe06eb5e.js.LICENSE.txt */
+/*! For license information please see 568.5e4ac436f86b65d9e70f.js.LICENSE.txt */
 "use strict";
 (self.webpackChunkamazon_codewhisperer_jupyterlab_ext = self.webpackChunkamazon_codewhisperer_jupyterlab_ext || []).push([
     [568], {
         4442: (e, t, n) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.Application = void 0;
@@ -10,47 +10,50 @@
                 o = n(4657),
                 s = n(4872),
                 r = n(1708),
                 a = n(3311),
                 c = n(2531),
                 l = n(9513),
                 d = n(7790),
-                u = n(9513),
-                g = n(1174);
+                g = n(9513),
+                u = n(1174);
             class h {
                 constructor() {
-                    this._environment = void 0, this.loadStateSignal = new i.Signal(this)
+                    this._environment = void 0, this.loadStateSignal = new i.Signal(this), this.toggleSettingSignal = new i.Signal(this)
                 }
                 static getInstance() {
                     return h.instance || (h.instance = new h), h.instance
                 }
                 async _fetchEnvironment() {
                     const e = await a.requestAPI("get_environment");
                     if (e.status !== l.HttpStatusCode.OK) return;
                     const t = await e.json();
                     this._environment = c.getResponseData(t).environment;
                     const n = c.getResponseData(t).version_notification,
                         i = c.getResponseData(t).latest_version;
-                    n && d.NotificationManager.getInstance().postNotificationForUpdateInformation(n, i, g.message("codewhisperer_update_now"), u.UPDATE_NOTIFICATION_URL).then()
+                    n && d.NotificationManager.getInstance().postNotificationForUpdateInformation(n, i, u.message("codewhisperer_update_now"), g.UPDATE_NOTIFICATION_URL).then()
                 }
                 isJupyterOSS() {
-                    return this._environment === p.JUPYTER_OSS
+                    return this._environment === m.JUPYTER_OSS
                 }
                 isSageMakerStudio() {
-                    return this._environment === p.SM_STUDIO
+                    return this._environment === m.SM_STUDIO
+                }
+                isGlueStudioNoteBook() {
+                    return this._environment === m.GLUE_STUDIO_NOTEBOOK
                 }
                 async loadServices(e, t) {
                     this.stateDB = e, this.jupyterApp = t, await this._fetchEnvironment(), s.Worker.getInstance(), o.AutoTrigger.getInstance(), r.AuthManager.getInstance()
                 }
             }
-            var p;
+            var m;
             t.Application = h,
                 function(e) {
-                    e.JUPYTER_OSS = "Jupyter OSS", e.SM_STUDIO = "SageMaker Studio"
-                }(p || (p = {}))
+                    e.JUPYTER_OSS = "Jupyter OSS", e.SM_STUDIO = "SageMaker Studio", e.GLUE_STUDIO_NOTEBOOK = "Glue Studio Notebook"
+                }(m || (m = {}))
         },
         1708: function(e, t, n) {
             var i = this && this.__importDefault || function(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             };
@@ -60,57 +63,57 @@
             const o = n(3311),
                 s = n(2531),
                 r = n(6168),
                 a = n(5185),
                 c = n(1174),
                 l = n(5185),
                 d = i(n(6271)),
-                u = n(2194),
-                g = n(7790),
+                g = n(2194),
+                u = n(7790),
                 h = n(4442),
-                p = n(9513),
-                m = n(9513);
+                m = n(9513),
+                p = n(9513);
             class _ {
                 constructor() {
                     this._authState = C.UNAUTHENTICATED, this._refreshIntervalInMs = 3e6, this.authStateChangedSignal = new r.Signal(this), this.authStateChangedSignal.connect(this._onAuthStateChanged, this), this._refreshToken = async () => {
                         this.isAuthenticated() && await this.refresh()
                     }
                 }
                 static getInstance() {
                     return _.instance || (_.instance = new _), _.instance
                 }
                 _onAuthStateChanged(e, t) {
                     this.authState = t, t !== C.UNAUTHENTICATED && t !== C.AUTHENTICATION_IN_PROGRESS && setTimeout(this._refreshToken, this._refreshIntervalInMs)
                 }
                 isAuthenticated() {
-                    return this.authState === C.AUTHENTICATED || h.Application.getInstance().isSageMakerStudio()
+                    return this.authState === C.AUTHENTICATED || !h.Application.getInstance().isJupyterOSS()
                 }
                 isAuthenticationInProgress() {
                     return this.authState === C.AUTHENTICATION_IN_PROGRESS
                 }
                 get authState() {
                     return this._authState
                 }
                 set authState(e) {
                     this._authState = e
                 }
                 async login() {
-                    let e = await s.loadState(u.CLIENT_REGISTRATION);
+                    let e = await s.loadState(g.CLIENT_REGISTRATION);
                     if (void 0 === e) {
                         const t = await o.requestAPI("register_client"),
                             n = await t.json();
-                        if (!s.isResponseSuccess(n)) return void await g.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(n), c.message("codewhisperer_learn_more"), m.LEARN_MORE_NOTIFICATION_URL);
-                        e = s.getResponseData(n), s.saveState(u.CLIENT_REGISTRATION, e).then()
+                        if (!s.isResponseSuccess(n)) return void await u.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(n), c.message("codewhisperer_learn_more"), p.LEARN_MORE_NOTIFICATION_URL);
+                        e = s.getResponseData(n), s.saveState(g.CLIENT_REGISTRATION, e).then()
                     }
                     const t = await o.requestAPI("device_authorization", {
                             body: JSON.stringify(e),
                             method: "POST"
                         }),
                         n = await t.json();
-                    if (!s.isResponseSuccess(n)) return void await g.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(n), c.message("codewhisperer_learn_more"), m.LEARN_MORE_NOTIFICATION_URL);
+                    if (!s.isResponseSuccess(n)) return void await u.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(n), c.message("codewhisperer_learn_more"), p.LEARN_MORE_NOTIFICATION_URL);
                     const i = s.getResponseData(n);
                     if (!(await l.showDialog({
                             title: c.message("codewhisperer_copy_code_and_proceed_dialog_title"),
                             body: d.default.createElement("p", null, d.default.createElement("br", null), d.default.createElement("li", null, c.message("codewhisperer_copy_code_and_proceed_dialog_message_first_li"), d.default.createElement("a", {
                                 href: "https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html",
                                 className: "cwspr-learn-more-link"
                             }, c.message("codewhisperer_copy_code_and_proceed_dialog_message_first_li_learn_more"))), d.default.createElement("br", null), d.default.createElement("li", null, c.message("codewhisperer_copy_code_and_proceed_dialog_message_second_li")), d.default.createElement("br", null), d.default.createElement("li", null, c.message("codewhisperer_copy_code_and_proceed_dialog_message_third_li"), i.userCode), d.default.createElement("br", null)),
@@ -125,36 +128,36 @@
                     };
                     o.requestAPI("create_token", {
                         body: JSON.stringify(r),
                         method: "POST"
                     }).then((async e => {
                         const t = await e.json();
                         if (!t) return;
-                        if (!s.isResponseSuccess(t)) return await g.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(t), c.message("codewhisperer_learn_more"), m.LEARN_MORE_NOTIFICATION_URL), void this.authStateChangedSignal.emit(C.UNAUTHENTICATED);
+                        if (!s.isResponseSuccess(t)) return await u.NotificationManager.getInstance().postNotificationForApiExceptions(s.getErrorResponseUserMessage(t), c.message("codewhisperer_learn_more"), p.LEARN_MORE_NOTIFICATION_URL), void this.authStateChangedSignal.emit(C.UNAUTHENTICATED);
                         const n = s.getResponseData(t);
-                        await s.saveState(u.SSO_TOKEN, n), this.authStateChangedSignal.emit(C.AUTHENTICATED)
+                        await s.saveState(g.SSO_TOKEN, n), this.authStateChangedSignal.emit(C.AUTHENTICATED)
                     }))
                 }
                 cancelLogin() {
                     o.requestAPI("cancel_login").then(), this.authStateChangedSignal.emit(C.UNAUTHENTICATED)
                 }
                 async refresh() {
-                    const e = await s.loadState(u.SSO_TOKEN);
+                    const e = await s.loadState(g.SSO_TOKEN);
                     if (void 0 === e) return;
-                    const t = await s.loadState(u.CLIENT_REGISTRATION);
+                    const t = await s.loadState(g.CLIENT_REGISTRATION);
                     if (void 0 === t) return;
                     const n = {
                             clientRegistration: t,
                             token: e
                         },
                         i = await o.requestAPI("refresh", {
                             body: JSON.stringify(n),
                             method: "POST"
                         });
-                    if (i.status === p.HttpStatusCode.NOT_FOUND) return;
+                    if (i.status === m.HttpStatusCode.NOT_FOUND) return;
                     const r = await i.json();
                     if (!s.isResponseSuccess(r)) {
                         const e = a.Notification.emit(c.message("codewhisperer_expiry_notification_message"), "default", {
                             autoClose: 1e4,
                             actions: [{
                                 label: c.message("codewhisperer_expiry_notification_button_authenticate"),
                                 callback: async () => {
@@ -167,18 +170,18 @@
                                     a.Notification.dismiss(e)
                                 }
                             }]
                         });
                         return
                     }
                     const l = s.getResponseData(r);
-                    await s.saveState(u.SSO_TOKEN, l), this.authStateChangedSignal.emit(C.AUTHENTICATED)
+                    await s.saveState(g.SSO_TOKEN, l), this.authStateChangedSignal.emit(C.AUTHENTICATED)
                 }
                 async logout() {
-                    await s.removeState(u.SSO_TOKEN), await s.removeState(u.CLIENT_REGISTRATION), this.authStateChangedSignal.emit(C.UNAUTHENTICATED)
+                    await s.removeState(g.SSO_TOKEN), await s.removeState(g.CLIENT_REGISTRATION), this.authStateChangedSignal.emit(C.UNAUTHENTICATED)
                 }
             }
             var C;
             t.AuthManager = _,
                 function(e) {
                     e[e.AUTHENTICATED = 0] = "AUTHENTICATED", e[e.UNAUTHENTICATED = 1] = "UNAUTHENTICATED", e[e.AUTHENTICATION_IN_PROGRESS = 2] = "AUTHENTICATION_IN_PROGRESS"
                 }(C = t.AuthState || (t.AuthState = {}))
@@ -385,23 +388,23 @@
             const o = n(968),
                 s = i(n(3994)),
                 r = i(n(1563)),
                 a = i(n(8177)),
                 c = i(n(9107)),
                 l = i(n(6445)),
                 d = i(n(4268)),
-                u = i(n(6389)),
-                g = i(n(9206)),
+                g = i(n(6389)),
+                u = i(n(9206)),
                 h = i(n(2431)),
-                p = i(n(6140)),
-                m = i(n(1590));
+                m = i(n(6140)),
+                p = i(n(1590));
             class _ {}
             t.Icons = _, _.visualCueArrowIcon = new o.LabIcon({
                 name: "visual-cue-arrow",
-                svgstr: g.default
+                svgstr: u.default
             }), _.logoIcon = new o.LabIcon({
                 name: "codewhisperer:logo",
                 svgstr: s.default
             }), _.documentationIcon = new o.LabIcon({
                 name: "codewhisperer:documentation",
                 svgstr: r.default
             }), _.referenceLogIcon = new o.LabIcon({
@@ -414,24 +417,24 @@
                 name: "codewhisperer:resume",
                 svgstr: l.default
             }), _.signOutIcon = new o.LabIcon({
                 name: "codewhisperer:signOut",
                 svgstr: d.default
             }), _.startIcon = new o.LabIcon({
                 name: "codewhisperer:start",
-                svgstr: u.default
+                svgstr: g.default
             }), _.connectedIcon = new o.LabIcon({
                 name: "codewhisperer:connected",
                 svgstr: h.default
             }), _.disconnectedIcon = new o.LabIcon({
                 name: "codewhisperer:disconnected",
-                svgstr: p.default
+                svgstr: m.default
             }), _.loadingIcon = new o.LabIcon({
                 name: "codewhisperer:loading",
-                svgstr: m.default
+                svgstr: p.default
             })
         },
         1568: function(e, t, n) {
             var i = this && this.__importDefault || function(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
@@ -442,52 +445,52 @@
             const o = n(3961),
                 s = n(2766),
                 r = n(7681),
                 a = n(7363),
                 c = n(370),
                 l = n(4872),
                 d = n(6817),
-                u = n(6186),
-                g = n(8826),
+                g = n(6186),
+                u = n(8826),
                 h = n(7037),
-                p = n(4657),
-                m = n(1797),
+                m = n(4657),
+                p = n(1797),
                 _ = n(9805),
                 C = i(n(5313)),
-                v = n(5231),
-                I = n(1708),
+                I = n(5231),
+                v = n(1708),
                 w = n(6947),
                 f = n(4442),
                 y = n(6143),
                 S = n(3770),
                 T = n(9513),
                 b = n(5064),
                 E = {
                     id: T.PLUGIN_ID,
                     autoStart: !0,
-                    requires: [a.ISettingRegistry, o.ICompletionManager, s.INotebookTracker, r.IEditorTracker, d.IStateDB, g.IStatusBar, y.IRenderMimeRegistry],
-                    activate: async (e, t, n, i, r, a, d, g) => {
+                    requires: [a.ISettingRegistry, o.ICompletionManager, s.INotebookTracker, r.IEditorTracker, d.IStateDB, u.IStatusBar, y.IRenderMimeRegistry],
+                    activate: async (e, t, n, i, r, a, d, u) => {
                         const y = w.Logger.getInstance({
                                 name: "codewhisperer"
                             }),
                             E = performance.now();
                         e.restored.then((async () => {
                             a.fetch(T.PLUGIN_ID).then((e => {
-                                e ? (_.Telemetry.clientId = e.clientId, y.debug(`Restored - clientId: ${_.Telemetry.clientId}`)) : (_.Telemetry.clientId = m.UUID.uuid4(), a.save(T.PLUGIN_ID, {
+                                e ? (_.Telemetry.clientId = e.clientId, y.debug(`Restored - clientId: ${_.Telemetry.clientId}`)) : (_.Telemetry.clientId = p.UUID.uuid4(), a.save(T.PLUGIN_ID, {
                                     clientId: _.Telemetry.clientId
                                 }), y.debug(`Generated - clientId: ${_.Telemetry.clientId}`))
                             }));
                             const n = t => {
-                                if (_.Telemetry.getInstance().enableTelemetry(t.get(T.SettingIDs.keyTelemetry).composite), l.Worker.getInstance().setOptOut(!t.get(T.SettingIDs.keyOptOut).composite), l.Worker.getInstance().setSuggestionsWithCodeReferences(t.get(T.SettingIDs.keyReferences).composite), w.Logger.setLogLevel(t.get(T.SettingIDs.keyLogLevel).composite), b.Keybindings.getInstance().keyBindings = [...e.commands.keyBindings], y.debug("Loaded settings"), f.Application.getInstance().isJupyterOSS()) return;
+                                if (f.Application.getInstance().setting = t, _.Telemetry.getInstance().enableTelemetry(t.get(T.SettingIDs.keyTelemetry).composite), l.Worker.getInstance().setOptOut(!t.get(T.SettingIDs.keyOptOut).composite), l.Worker.getInstance().setSuggestionsWithCodeReferences(t.get(T.SettingIDs.keyReferences).composite), w.Logger.setLogLevel(t.get(T.SettingIDs.keyLogLevel).composite), b.Keybindings.getInstance().keyBindings = [...e.commands.keyBindings], y.debug("Loaded settings"), f.Application.getInstance().isJupyterOSS()) return;
                                 const n = document.createElement("style");
                                 n.textContent = "\n#jp-SettingsEditor-amazon-codewhisperer-jupyterlab-ext\\:completer > div:first-of-type {\n  display: none !important;\n}\n\n#jp-SettingsEditor-amazon-codewhisperer-jupyterlab-ext\\:completer > div:first-of-type > input {\n  pointer-events: none;\n  opacity: 0.5;\n}\n        ", document.head.appendChild(n)
                             };
                             Promise.all([e.restored, t.load(T.PLUGIN_ID)]).then((([, e]) => {
                                 n(e), e.changed.connect(n)
-                            })), f.Application.getInstance().loadStateSignal.emit(null), await I.AuthManager.getInstance().refresh();
+                            })), f.Application.getInstance().loadStateSignal.emit(null), await v.AuthManager.getInstance().refresh();
                             const i = new C.default;
                             d.registerStatusItem("aws-codewhisperer:status-bar-widget", {
                                 item: i,
                                 align: "left",
                                 isActive: () => !0,
                                 rank: 100
                             })
@@ -495,41 +498,41 @@
                             var r, a;
                             y.debug(`Notebookpanel added - ${i.id}`);
                             let l = null !== (a = null === (r = i.content.activeCell) || void 0 === r ? void 0 : r.editor) && void 0 !== a ? a : null;
                             const d = {
                                     session: i.sessionContext.session,
                                     editor: l
                                 },
-                                u = new c.MergeConnector,
-                                g = n.register({
-                                    connector: u,
+                                g = new c.MergeConnector,
+                                u = n.register({
+                                    connector: g,
                                     editor: l,
                                     parent: i
                                 }),
-                                m = () => {
+                                p = () => {
                                     var t, n;
-                                    y.debug(`Notebookpanel updated - ${i.id}`), l = null !== (n = null === (t = i.content.activeCell) || void 0 === t ? void 0 : t.editor) && void 0 !== n ? n : null, d.session = i.sessionContext.session, d.editor = l, g.editor = l;
+                                    y.debug(`Notebookpanel updated - ${i.id}`), l = null !== (n = null === (t = i.content.activeCell) || void 0 === t ? void 0 : t.editor) && void 0 !== n ? n : null, d.session = i.sessionContext.session, d.editor = l, u.editor = l;
                                     const r = new o.KernelConnector(d),
                                         a = new o.ContextConnector(d),
-                                        u = new v.CodeWhispererConnector({
+                                        g = new I.CodeWhispererConnector({
                                             notebookPanel: i
                                         });
-                                    g.connector = new c.MergeConnector(u, r, a), p.AutoTrigger.getInstance().registerListener(l, i);
+                                    u.connector = new c.MergeConnector(g, r, a), m.AutoTrigger.getInstance().registerListener(l, i);
                                     const h = e.shell.currentWidget;
-                                    h && h instanceof s.NotebookPanel && performance.now() - E > T.NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS && p.AutoTrigger.getInstance().onSwitchToNewCell(l, i)
+                                    h && h instanceof s.NotebookPanel && performance.now() - E > T.NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS && m.AutoTrigger.getInstance().onSwitchToNewCell(l, i)
                                 };
-                            i.content.activeCellChanged.connect((() => m())), i.sessionContext.sessionChanged.connect((() => m()));
+                            i.content.activeCellChanged.connect((() => p())), i.sessionContext.sessionChanged.connect((() => p()));
                             const _ = () => {
                                 y.debug(`Notebookpanel focus out - ${i.id}`), h.Inline.getInstance().onFocusOut()
                             };
                             i.node.removeEventListener("focusout", _), i.node.addEventListener("focusout", _)
                         })), r.widgetAdded.connect(((e, t) => {
                             y.debug(`Editor added - ${t.id}`), t.content.editor.host.addEventListener("focusin", (() => {
                                 const e = t.context.path.split("/").pop();
-                                p.AutoTrigger.getInstance().registerListener(t.content.editor, void 0, e)
+                                m.AutoTrigger.getInstance().registerListener(t.content.editor, void 0, e)
                             }))
                         })), e.commands.hasCommand(T.CommandIDs.invokeNotebook) || e.commands.addCommand(T.CommandIDs.invokeNotebook, {
                             execute: () => {
                                 var t;
                                 if (y.debug("Executing command : invokeNotebook"), h.Inline.getInstance().isInlineSessionActive()) return void h.Inline.getInstance().acceptCompletion();
                                 l.Worker.getInstance().isGetCompletionsRunning && h.Inline.getInstance().removeCompletion();
                                 const n = i.currentWidget;
@@ -551,28 +554,28 @@
                                 const t = i.currentWidget && i.currentWidget.id;
                                 if (t) return e.commands.execute(T.CommandIDs.select, {
                                     id: t
                                 })
                             }
                         })), e.commands.hasCommand(T.CommandIDs.login) || (y.debug("Executing command : login"), e.commands.addCommand(T.CommandIDs.login, {
                             execute: async () => {
-                                await I.AuthManager.getInstance().login()
+                                await v.AuthManager.getInstance().login()
                             }
                         })), e.commands.hasCommand(T.CommandIDs.invokeInline) || e.commands.addCommand(T.CommandIDs.invokeInline, {
                             execute: async () => {
                                 y.debug("Executing command : invokeInline");
                                 const t = e.shell.currentWidget;
                                 if (t && t instanceof s.NotebookPanel) y.debug("Invoking Inline in NotebookPanel"), await h.Inline.getInstance().getCompletionsInNotebookPanel(t, {
                                     triggerType: "OnDemand",
                                     triggerCharacter: void 0,
                                     automatedTriggerType: void 0,
                                     language: "ipynb",
                                     triggerTime: performance.now()
                                 });
-                                else if (t && t instanceof u.DocumentWidget) {
+                                else if (t && t instanceof g.DocumentWidget) {
                                     y.debug("Invoking Inline in Document");
                                     const e = t,
                                         n = e.context.path.split("/").pop();
                                     await h.Inline.getInstance().getCompletionsInEditor(e.content.editor, n, {
                                         triggerType: "OnDemand",
                                         triggerCharacter: void 0,
                                         automatedTriggerType: void 0,
@@ -593,15 +596,15 @@
                             execute: async () => {
                                 h.Inline.getInstance().showNext()
                             }
                         })), e.commands.hasCommand(T.CommandIDs.showPrev) || (y.debug("Executing command : showNext"), e.commands.addCommand(T.CommandIDs.showPrev, {
                             execute: async () => {
                                 h.Inline.getInstance().showPrev()
                             }
-                        })), S.ReferenceTracker.createInstance(g), _.Telemetry.init(), y.info("JupyterLab CodeWhisperer extension is activated!")
+                        })), S.ReferenceTracker.createInstance(u), _.Telemetry.init(), y.info("JupyterLab CodeWhisperer extension is activated!")
                     }
                 };
             t.default = E
         },
         7037: (e, t, n) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
@@ -610,21 +613,21 @@
                 o = n(4865),
                 s = n(9513),
                 r = n(4657),
                 a = n(8353),
                 c = n(1708),
                 l = n(3770),
                 d = n(6551),
-                u = "jp-mod-inlinecompleter-active";
-            class g {
+                g = "jp-mod-inlinecompleter-active";
+            class u {
                 constructor() {
                     this.completions = [], this.currentIndex = 0, this.typeahead = "", this.cursorObserver = void 0, this.invokeFileName = "", this.visualCueLeftMargin = 0
                 }
                 static getInstance() {
-                    return g.instance || (g.instance = new g), g.instance
+                    return u.instance || (u.instance = new u), u.instance
                 }
                 getVisualCueHtmlElement() {
                     const e = document.createElement("span"),
                         t = this.completions[this.currentIndex].references;
                     e.textContent = ` Suggestion ${this.currentIndex+1} of ${this.completions.length} from CodeWhisperer${this.getReferenceLogMessage(t)}`, e.style.opacity = "0.60", e.style.fontSize = this.invokeEditor.getOption("fontSize") - 1 + "px", e.style.whiteSpace = "pre", e.style.color = "var(--jp-content-font-color1)";
                     const n = o.Icons.visualCueArrowIcon.element(),
                         i = Math.max(this.invokeEditor.lineHeight - 4, 4);
@@ -810,15 +813,15 @@
                         const {
                             left: o,
                             top: c
                         } = s.cursorCoords(!1, "local");
                         return this.ghostTextWidget = this.getElement(t.substring(this.typeahead.length)), null === (n = this.marker) || void 0 === n || n.clear(), this.marker = s.doc.setBookmark(r, {
                             widget: this.ghostTextWidget,
                             insertLeft: !0
-                        }), this.markerPosition = r, null === (i = this.invokeEditor) || void 0 === i || i.host.classList.add(u), this.setupVisualCueOnHover(o, c), a.RecommendationStateHandler.instance.setSuggestionState(this.currentIndex, "Showed"), this.adjustCursorSizeAndPosition(e), !0
+                        }), this.markerPosition = r, null === (i = this.invokeEditor) || void 0 === i || i.host.classList.add(g), this.setupVisualCueOnHover(o, c), a.RecommendationStateHandler.instance.setSuggestionState(this.currentIndex, "Showed"), this.adjustCursorSizeAndPosition(e), !0
                     }
                     return this.removeCompletion(), !1
                 }
                 adjustCursorSizeAndPosition(e) {
                     const t = document.querySelector("div.CodeMirror-cursor"),
                         n = `${e.lineHeight}px`;
                     if (t) {
@@ -852,15 +855,15 @@
                         attributes: !0,
                         childList: !0,
                         subtree: !0
                     })
                 }
                 removeCompletion() {
                     var e, t, n, o, s;
-                    i.Worker.getInstance().isInvocationCancelled = !0, null === (e = this.marker) || void 0 === e || e.clear(), null === (t = this.visualCueWidget) || void 0 === t || t.remove(), this.visualCueWidget = void 0, this.visualCueLeftMargin = 0, null === (n = this.invokeEditor) || void 0 === n || n.model.selections.changed.disconnect(this.onCursorChange, this), null === (o = this.invokeEditor) || void 0 === o || o.host.classList.remove(u), i.Worker.getInstance().isGetCompletionsRunning || a.RecommendationStateHandler.instance.rejectRecommendationSignal.emit(-1), null === (s = this.cursorObserver) || void 0 === s || s.disconnect(), this.cursorObserver = void 0, this.completions = [], this.currentIndex = 0, this.typeahead = "", this.invokePosition = void 0, this.markerPosition = void 0, this.ghostTextWidget = void 0, this.invokeEditor = void 0, this.invokePanel = void 0, this.invokeFileName = "", this.showCompletionTimer && (clearInterval(this.showCompletionTimer), this.showCompletionTimer = void 0), this.forceClearGhostText()
+                    i.Worker.getInstance().isInvocationCancelled = !0, null === (e = this.marker) || void 0 === e || e.clear(), null === (t = this.visualCueWidget) || void 0 === t || t.remove(), this.visualCueWidget = void 0, this.visualCueLeftMargin = 0, null === (n = this.invokeEditor) || void 0 === n || n.model.selections.changed.disconnect(this.onCursorChange, this), null === (o = this.invokeEditor) || void 0 === o || o.host.classList.remove(g), i.Worker.getInstance().isGetCompletionsRunning || a.RecommendationStateHandler.instance.rejectRecommendationSignal.emit(-1), null === (s = this.cursorObserver) || void 0 === s || s.disconnect(), this.cursorObserver = void 0, this.completions = [], this.currentIndex = 0, this.typeahead = "", this.invokePosition = void 0, this.markerPosition = void 0, this.ghostTextWidget = void 0, this.invokeEditor = void 0, this.invokePanel = void 0, this.invokeFileName = "", this.showCompletionTimer && (clearInterval(this.showCompletionTimer), this.showCompletionTimer = void 0), this.forceClearGhostText()
                 }
                 async forceClearGhostText() {
                     const e = document.querySelector("span.cw-inline");
                     e && e.remove()
                 }
                 isInlineSessionActive() {
                     return void 0 !== this.invokeEditor && void 0 !== this.ghostTextWidget
@@ -889,15 +892,15 @@
                     }
                     this.removeCompletion()
                 }
                 onEditorChange(e) {
                     this.removeCompletion()
                 }
             }
-            t.Inline = g
+            t.Inline = u
         },
         5064: (e, t) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.Keybindings = void 0;
             class n {
                 constructor() {}
@@ -1041,47 +1044,47 @@
                 var t;
                 const n = e.content,
                     i = n.activeCell,
                     a = null === (t = n.activeCell) || void 0 === t ? void 0 : t.editor,
                     c = n.model.cells.length,
                     l = i.model.type,
                     d = null == a ? void 0 : a.getCursorPosition().line,
-                    u = null == a ? void 0 : a.getOffsetAt(a.getCursorPosition());
-                let g;
+                    g = null == a ? void 0 : a.getOffsetAt(a.getCursorPosition());
+                let u;
                 if (a && i) {
                     const t = n.model.cells;
                     let i = "",
                         c = "";
                     for (let e = 0; e < t.length; e++) {
                         const o = t.get(e);
                         if (e < n.activeCellIndex) i += r(o);
                         else if (e === n.activeCellIndex) {
                             const e = a.getCursorPosition(),
                                 t = a.getOffsetAt(e),
                                 n = a.model.value.text;
                             i += n.substring(0, t), c += n.substring(t, n.length)
                         } else c += r(o)
                     }
-                    s.debug(`Notebook content length - left:${i.slice.length} right:${i.slice.length}`), g = {
+                    s.debug(`Notebook content length - left:${i.slice.length} right:${i.slice.length}`), u = {
                         leftFileContent: i.slice(-o.MAX_LENGTH),
                         rightFileContent: c.slice(0, o.MAX_LENGTH),
                         filename: e.context.path.split("/").pop(),
                         programmingLanguage: {
                             languageName: "python"
                         }
                     }
                 }
                 return {
-                    fileContext: g,
+                    fileContext: u,
                     fileContextMetadata: {
                         activeCellIdx: n.activeCellIndex,
                         cellCount: c,
                         cellType: l,
                         lineNumber: d,
-                        cursorOffset: u
+                        cursorOffset: g
                     }
                 }
             }, t.getFileContextFromEditor = function(e, t) {
                 let n, i, r;
                 if (e) {
                     i = e.getCursorPosition(), r = e.getOffsetAt(i);
                     const a = e.model.value.text,
@@ -1120,18 +1123,18 @@
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.RecommendationStateHandler = void 0;
             const a = n(9805),
                 c = n(9513),
                 l = n(7126),
                 d = n(6168),
-                u = n(6947);
-            class g {
+                g = n(6947);
+            class u {
                 constructor() {
-                    this.acceptedIndex = -1, this.timeSinceLastUserDecision = void 0, this.timeSinceLastDocumentChange = void 0, this.recommendations = [], this.recommendationSuggestionState = new Map, this.acceptRecommendationSignal = new d.Signal(this), this.acceptRecommendationSignal.connect(this.userDecisionSignalListener, this), this.rejectRecommendationSignal = new d.Signal(this), this.rejectRecommendationSignal.connect(this.userDecisionSignalListener, this), this.logger = u.Logger.getInstance({
+                    this.acceptedIndex = -1, this.timeSinceLastUserDecision = void 0, this.timeSinceLastDocumentChange = void 0, this.recommendations = [], this.recommendationSuggestionState = new Map, this.acceptRecommendationSignal = new d.Signal(this), this.acceptRecommendationSignal.connect(this.userDecisionSignalListener, this), this.rejectRecommendationSignal = new d.Signal(this), this.rejectRecommendationSignal.connect(this.userDecisionSignalListener, this), this.logger = g.Logger.getInstance({
                         name: "codewhisperer",
                         component: "recommendationStateHandler"
                     })
                 }
                 reset() {
                     this.timeToFirstRecommendation = void 0, this.requestId = void 0, this.firstRequestId = void 0, this.invocationMetadata = void 0, this.acceptedIndex = -1, this.recommendations = [], this.recommendationSuggestionState = new Map
                 }
@@ -1150,19 +1153,19 @@
                 }
                 addRecommendation(e) {
                     this.recommendations.push(e)
                 }
                 updateRecommendationState(e) {
                     const t = this.recommendations.length;
                     e.length > 0 ? e.forEach(((e, n) => {
-                        g.instance.setSuggestionState(t + n, "Discard"), g.instance.addRecommendation(e)
-                    })) : (g.instance.addRecommendation({
+                        u.instance.setSuggestionState(t + n, "Discard"), u.instance.addRecommendation(e)
+                    })) : (u.instance.addRecommendation({
                         content: "",
                         references: []
-                    }), g.instance.setSuggestionState(t, "Empty"))
+                    }), u.instance.setSuggestionState(t, "Empty"))
                 }
                 userDecisionSignalListener(e, t) {
                     this.acceptedIndex = t, this.recordUserDecisionTelemetry()
                 }
                 recordUserDecisionTelemetry() {
                     if (!this.invocationMetadata) return void this.reset();
                     const e = [];
@@ -1225,15 +1228,15 @@
                         if ("Accept" === n.codewhispererSuggestionState) return "Accept";
                         if ("Reject" === n.codewhispererSuggestionState) return "Reject";
                         "Empty" !== n.codewhispererSuggestionState && (t = !1)
                     }
                     return t ? "Empty" : "Discard"
                 }
             }
-            t.RecommendationStateHandler = g, i = g, o = {
+            t.RecommendationStateHandler = u, i = u, o = {
                 value: void 0
             }
         },
         4872: (e, t, n) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.Worker = void 0;
@@ -1241,84 +1244,84 @@
                 o = n(6551),
                 s = n(9513),
                 r = n(1174),
                 a = n(6168),
                 c = n(6947),
                 l = n(7790),
                 d = n(2531),
-                u = n(8353);
-            class g {
+                g = n(8353);
+            class u {
                 constructor() {
                     this._isGetCompletionsRunning = !1, this.isInvocationCancelled = !1, this.optOut = !1, this.client = new i.ApiClient, this.receivedResponseSignal = new a.Signal(this), this.serviceInvocationSignal = new a.Signal(this), this.invocationStatusChangedSignal = new a.Signal(this), this.logger = c.Logger.getInstance({
                         name: "codewhisperer",
                         component: "worker"
                     })
                 }
                 static getInstance() {
-                    return g.instance || (g.instance = new g), g.instance
+                    return u.instance || (u.instance = new u), u.instance
                 }
                 get isGetCompletionsRunning() {
                     return this._isGetCompletionsRunning
                 }
                 set isGetCompletionsRunning(e) {
                     this._isGetCompletionsRunning = e, this.invocationStatusChangedSignal.emit(e)
                 }
                 async getCompletionsPaginated(e, t, n) {
-                    let i, o, a, c, g = "",
+                    let i, o, a, c, u = "",
                         h = "",
-                        p = "",
-                        m = 0,
+                        m = "",
+                        p = 0,
                         _ = 0,
                         C = !0;
                     if (!this._isGetCompletionsRunning) {
-                        for (u.RecommendationStateHandler.instance.rejectRecommendationSignal.emit(-1), this.isInvocationCancelled = !1; !this.isInvocationCancelled && m < s.MAX_PAGINATION_CALLS;) {
+                        for (g.RecommendationStateHandler.instance.rejectRecommendationSignal.emit(-1), this.isInvocationCancelled = !1; !this.isInvocationCancelled && p < s.MAX_PAGINATION_CALLS;) {
                             this.isGetCompletionsRunning = !0;
                             try {
                                 o = Date.now();
                                 const t = await this.client.generateRecommendations(e, this.optOut);
-                                i = await t.json(), this.logger.debug("responseJson", i), g = i["x-amzn-requestid"], h = i["x-amzn-sessionid"], c = "Succeeded"
+                                i = await t.json(), this.logger.debug("responseJson", i), u = i["x-amzn-requestid"], h = i["x-amzn-sessionid"], c = "Succeeded"
                             } catch (e) {
                                 this.logger.error("Error in calling generateRecommendations API ", e), a = e, c = "Failed"
                             } finally {
                                 if (i && !d.isResponseSuccess(i)) {
                                     const e = d.getErrorResponseUserMessage(i);
                                     await l.NotificationManager.getInstance().postNotificationForApiExceptions(e, r.message("codewhisperer_learn_more"), s.LEARN_MORE_NOTIFICATION_URL), a = e, i.message && i.message.includes("Invalid input data") && (C = !1, this.logger.debug("Invalid input data, not recording service invocation")), c = "Failed"
                                 }
-                                let v;
-                                i && d.isResponseSuccess(i) && ("recommendations" in i.data ? v = i.data.recommendations : "completions" in i.data && (v = i.data.completions, p = s.AWS_BUILDER_ID_START_URL), this.suggestionsWithCodeReferences || (v = v.filter((e => !Array.isArray(e.references) || 0 === e.references.length)))), v && (this.receivedResponseSignal.emit(v), _ += v.length > 0 ? v.length : 1, this.logger.debug("successfully received valid recommendations"));
-                                const I = d.detectCompletionType(v);
+                                let I;
+                                i && d.isResponseSuccess(i) && ("recommendations" in i.data ? I = i.data.recommendations : "completions" in i.data && (I = i.data.completions, m = s.AWS_BUILDER_ID_START_URL), this.suggestionsWithCodeReferences || (I = I.filter((e => !Array.isArray(e.references) || 0 === e.references.length)))), I && (this.receivedResponseSignal.emit(I), _ += I.length > 0 ? I.length : 1, this.logger.debug("successfully received valid recommendations"));
+                                const v = d.detectCompletionType(I);
                                 if (C && this.serviceInvocationSignal.emit({
-                                        codewhispererRequestId: g,
-                                        credentialStartUrl: p,
+                                        codewhispererRequestId: u,
+                                        credentialStartUrl: m,
                                         duration: Date.now() - o,
                                         reason: a,
                                         result: c,
-                                        codewhispererCompletionType: I,
+                                        codewhispererCompletionType: v,
                                         codewhispererTriggerType: t.triggerType,
                                         codewhispererAutomatedTriggerType: t.automatedTriggerType,
                                         codewhispererSessionId: h,
                                         codewhispererJupyterLabCellCount: n.cellCount,
                                         codewhispererJupyterLabCellIndex: n.activeCellIdx,
                                         codewhispererJupyterLabCellType: n.cellType,
                                         codewhispererLanguage: t.language,
-                                        codewhispererLastSuggestionIndex: "Succeeded" === c && v ? _ - 1 : -1,
+                                        codewhispererLastSuggestionIndex: "Succeeded" === c && I ? _ - 1 : -1,
                                         codewhispererCursorOffset: n.cursorOffset,
                                         codewhispererLineNumber: n.lineNumber
-                                    }), "Succeeded" === c && (u.RecommendationStateHandler.instance.updateInvocationMetadata({
-                                        completionType: I,
-                                        credentialStartUrl: p,
+                                    }), "Succeeded" === c && (g.RecommendationStateHandler.instance.updateInvocationMetadata({
+                                        completionType: v,
+                                        credentialStartUrl: m,
                                         sessionId: h,
                                         paginationProgress: _,
                                         fileContextMetadata: n,
                                         triggerMetadata: t
-                                    }, g, 0 === m), v && u.RecommendationStateHandler.instance.addRecommendations(v)), !i || !d.isResponseSuccess(i) || "" === i.data.nextToken) break;
-                                e.nextToken = i.data.nextToken, m++
+                                    }, u, 0 === p), I && g.RecommendationStateHandler.instance.addRecommendations(I)), !i || !d.isResponseSuccess(i) || "" === i.data.nextToken) break;
+                                e.nextToken = i.data.nextToken, p++
                             }
                         }
-                        this.isInvocationCancelled && u.RecommendationStateHandler.instance.rejectRecommendationSignal.emit(-1), this.isGetCompletionsRunning = !1
+                        this.isInvocationCancelled && g.RecommendationStateHandler.instance.rejectRecommendationSignal.emit(-1), this.isGetCompletionsRunning = !1
                     }
                 }
                 async getCompletionsPaginatedInNotebookPanel(e, t) {
                     const {
                         fileContext: n,
                         fileContextMetadata: i
                     } = o.getFileContextFromNotebook(e);
@@ -1346,19 +1349,22 @@
                         nextToken: ""
                     };
                     await this.getCompletionsPaginated(a, n, r)
                 }
                 setSuggestionsWithCodeReferences(e) {
                     this.suggestionsWithCodeReferences = e
                 }
+                isSuggestionsWithCodeReferencesEnabled() {
+                    return this.suggestionsWithCodeReferences
+                }
                 setOptOut(e) {
                     this.optOut = e
                 }
             }
-            t.Worker = g
+            t.Worker = u
         },
         3770: (e, t, n) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.ReferenceTracker = t.LOG_SOURCE = void 0;
             const i = n(5185),
                 o = n(9303),
@@ -1437,244 +1443,300 @@
             const o = n(5185),
                 s = n(8826),
                 r = i(n(6271)),
                 a = n(3706),
                 c = n(4968),
                 l = n(4865),
                 d = n(1174),
-                u = n(9462),
-                g = n(1708),
+                g = n(9462),
+                u = n(1708),
                 h = n(4657),
-                p = n(4872),
-                m = n(3770),
+                m = n(4872),
+                p = n(3770),
                 _ = n(4442),
                 C = n(5064),
-                v = n(9513),
-                I = n(2194),
-                w = n(2531);
-            class f extends o.VDomModel {
+                I = n(9513),
+                v = n(2194),
+                w = n(2531),
+                f = n(9805);
+            class y extends o.VDomModel {
                 constructor() {
                     super()
                 }
             }
-            class y extends o.VDomRenderer {
+            class S extends o.VDomRenderer {
                 constructor() {
-                    super(new f), this._popup = null, this._commandsForNotAuthenticated = new c.CommandRegistry, this._commandsForAuthenticationInProgress = new c.CommandRegistry, this._commandsForAutoSuggestionEnabled = new c.CommandRegistry, this._commandsForAutosuggestionDisabled = new c.CommandRegistry, this._renderer = new S, this._keyShortcutsInfoRows = 5, this.addClass(s.interactiveItem), this.addClass("jp-Notebook-ExecutionIndicator"), this.addClass("cwspr-statusbarwidget-parent"), this._initializeCommands(), g.AuthManager.getInstance().authStateChangedSignal.connect(this._onAuthStateChanged, this), p.Worker.getInstance().invocationStatusChangedSignal.connect(this._onInvocationStatusChanged, this)
+                    super(new y), this._popup = null, this._menu = null, this._commandsForNotAuthenticated = new c.CommandRegistry, this._commandsForAuthenticationInProgress = new c.CommandRegistry, this._commandsForAutoSuggestionEnabled = new c.CommandRegistry, this._commandsForAutosuggestionDisabled = new c.CommandRegistry, this._renderer = new T, this._keyShortcutsInfoRows = 5, this._toggleSettingsforGlueStudioRows = 9, this.addClass(s.interactiveItem), this.addClass("cwspr-statusbarwidget-parent"), this._initializeCommands(), u.AuthManager.getInstance().authStateChangedSignal.connect(this._onAuthStateChanged, this), m.Worker.getInstance().invocationStatusChangedSignal.connect(this._onInvocationStatusChanged, this), _.Application.getInstance().toggleSettingSignal.connect(this._onToggleSettingButton, this)
                 }
                 _onAuthStateChanged(e, t) {
                     this.update()
                 }
                 _onInvocationStatusChanged(e, t) {
                     this.update()
                 }
+                async _onToggleSettingButton(e, t) {
+                    const n = _.Application.getInstance().setting;
+                    if (t == I.CommandIDs.toggleTelemetry) {
+                        const e = n.get(I.SettingIDs.keyTelemetry).composite;
+                        await n.set(I.SettingIDs.keyTelemetry, !e)
+                    } else if (t == I.CommandIDs.toggleCodeReferences) {
+                        const e = n.get(I.SettingIDs.keyReferences).composite;
+                        await n.set(I.SettingIDs.keyReferences, !e)
+                    }
+                    this._menu && this._menu.update()
+                }
                 _addKeyShortcutsInfo(e) {
-                    e.addCommand(v.CommandIDs.keyShortcutTitle, {
+                    e.addCommand(I.CommandIDs.keyShortcutTitle, {
                         label: d.message("codewhisperer_key_shortcut_title"),
                         icon: null,
                         execute: async () => {},
                         isEnabled: () => !1
-                    }), e.addCommand(v.CommandIDs.keyShortcutAccept, {
+                    }), e.addCommand(I.CommandIDs.keyShortcutAccept, {
                         label: d.message("codewhisperer_key_shortcut_accept"),
                         icon: null,
                         execute: async () => {},
                         isEnabled: () => !1
-                    }), e.addCommand(v.CommandIDs.keyShortcutManualTrigger, {
+                    }), e.addCommand(I.CommandIDs.keyShortcutManualTrigger, {
                         label: d.message("codewhisperer_key_shortcut_manual_trigger"),
                         icon: null,
                         execute: async () => {},
                         isEnabled: () => !1
-                    }), e.addCommand(v.CommandIDs.keyShortcutNavigate, {
+                    }), e.addCommand(I.CommandIDs.keyShortcutNavigate, {
                         label: d.message("codewhisperer_key_shortcut_navigate"),
                         icon: null,
                         execute: async () => {},
                         isEnabled: () => !1
-                    }), e.addCommand(v.CommandIDs.keyShortcutReject, {
+                    }), e.addCommand(I.CommandIDs.keyShortcutReject, {
                         label: d.message("codewhisperer_key_shortcut_reject"),
                         icon: null,
                         execute: async () => {},
                         isEnabled: () => !1
                     })
                 }
                 _addCommandsForUnauthenticated() {
-                    _.Application.getInstance().isJupyterOSS() && this._commandsForNotAuthenticated.addCommand(v.CommandIDs.startCodeWhisperer, {
+                    _.Application.getInstance().isJupyterOSS() && this._commandsForNotAuthenticated.addCommand(I.CommandIDs.startCodeWhisperer, {
                         label: d.message("codewhisperer_start"),
                         icon: l.Icons.startIcon,
                         caption: d.message("codewhisperer_start"),
                         execute: async () => {
-                            this._handleClick(), g.AuthManager.getInstance().isAuthenticated() || g.AuthManager.getInstance().isAuthenticationInProgress() || await g.AuthManager.getInstance().login()
+                            this._handleClick(), u.AuthManager.getInstance().isAuthenticated() || u.AuthManager.getInstance().isAuthenticationInProgress() || await u.AuthManager.getInstance().login()
                         }
-                    }), this._commandsForNotAuthenticated.addCommand(v.CommandIDs.openDocumentation, {
+                    }), this._commandsForNotAuthenticated.addCommand(I.CommandIDs.openDocumentation, {
                         label: d.message("codewhisperer_documentation_open"),
                         icon: l.Icons.documentationIcon,
                         caption: d.message("codewhisperer_documentation_open"),
                         execute: async () => {
-                            window.open(v.CWSPR_DOCUMENTATION, "_blank"), this._handleClick()
+                            window.open(I.CWSPR_DOCUMENTATION, "_blank"), this._handleClick()
                         }
                     })
                 }
                 _addCommandsForAuthenticationInProgress() {
-                    this._commandsForAuthenticationInProgress.addCommand(v.CommandIDs.cancelLogin, {
+                    this._commandsForAuthenticationInProgress.addCommand(I.CommandIDs.cancelLogin, {
                         label: d.message("codewhisperer_cancel_login"),
                         icon: l.Icons.startIcon,
                         caption: d.message("codewhisperer_cancel_login"),
                         execute: async () => {
-                            this._handleClick(), g.AuthManager.getInstance().isAuthenticationInProgress() && await g.AuthManager.getInstance().cancelLogin()
+                            this._handleClick(), u.AuthManager.getInstance().isAuthenticationInProgress() && await u.AuthManager.getInstance().cancelLogin()
                         }
-                    }), this._commandsForAuthenticationInProgress.addCommand(v.CommandIDs.openDocumentation, {
+                    }), this._commandsForAuthenticationInProgress.addCommand(I.CommandIDs.openDocumentation, {
                         label: d.message("codewhisperer_documentation_open"),
                         icon: l.Icons.documentationIcon,
                         caption: d.message("codewhisperer_documentation_open"),
                         execute: async () => {
-                            window.open(v.CWSPR_DOCUMENTATION, "_blank"), this._handleClick()
+                            window.open(I.CWSPR_DOCUMENTATION, "_blank"), this._handleClick()
                         }
                     })
                 }
                 _addCommandsForAuthenticatedCommon(e) {
-                    e.addCommand(v.CommandIDs.openReferenceLog, {
+                    e.addCommand(I.CommandIDs.openReferenceLog, {
                         label: d.message("codewhisperer_reference_log_open"),
                         icon: l.Icons.referenceLogIcon,
                         caption: d.message("codewhisperer_reference_log_open"),
-                        isToggled: () => m.ReferenceTracker.getInstance().isReferenceLogDisposed(),
+                        isToggled: () => p.ReferenceTracker.getInstance().isReferenceLogDisposed(),
                         execute: async () => {
-                            m.ReferenceTracker.getInstance().isReferenceLogDisposed() ? _.Application.getInstance().jupyterApp.shell.add(m.ReferenceTracker.getInstance().createReferenceLogWidget(), "down", {
-                                ref: m.LOG_SOURCE,
+                            p.ReferenceTracker.getInstance().isReferenceLogDisposed() ? _.Application.getInstance().jupyterApp.shell.add(p.ReferenceTracker.getInstance().createReferenceLogWidget(), "down", {
+                                ref: p.LOG_SOURCE,
                                 mode: "split-bottom"
-                            }) : m.ReferenceTracker.getInstance().disposeReferenceLogWidget(), this._handleClick()
+                            }) : p.ReferenceTracker.getInstance().disposeReferenceLogWidget(), this._handleClick()
                         }
-                    }), e.addCommand(v.CommandIDs.openDocumentation, {
+                    }), e.addCommand(I.CommandIDs.openDocumentation, {
                         label: d.message("codewhisperer_documentation_open"),
                         icon: l.Icons.documentationIcon,
                         caption: d.message("codewhisperer_documentation_open"),
                         execute: async () => {
-                            window.open(v.CWSPR_DOCUMENTATION, "_blank"), this._handleClick()
+                            const e = document.createElement("a");
+                            e.setAttribute("href", I.CWSPR_DOCUMENTATION), e.setAttribute("target", "_blank"), e.click(), this._handleClick()
                         }
-                    }), _.Application.getInstance().isSageMakerStudio() || e.addCommand(v.CommandIDs.signOut, {
+                    }), _.Application.getInstance().isJupyterOSS() && e.addCommand(I.CommandIDs.signOut, {
                         label: d.message("codewhisperer_sign_out"),
                         icon: l.Icons.signOutIcon,
                         caption: d.message("codewhisperer_sign_out"),
                         execute: async () => {
-                            this._handleClick(), g.AuthManager.getInstance().isAuthenticated() && await g.AuthManager.getInstance().logout()
+                            this._handleClick(), u.AuthManager.getInstance().isAuthenticated() && await u.AuthManager.getInstance().logout()
                         }
                     })
                 }
+                _addCommandsForAuthenticatedGlueStudio(e) {
+                    e.addCommand(I.CommandIDs.toggleTelemetry, {
+                        label: d.message("codewhisperer_toggle_telemetry"),
+                        icon: null,
+                        execute: async () => {},
+                        isEnabled: () => !1
+                    }), e.addCommand(I.CommandIDs.toggleCodeReferences, {
+                        label: d.message("codewhisperer_toggle_code_references"),
+                        icon: null,
+                        execute: async () => {},
+                        isEnabled: () => !1
+                    })
+                }
                 _initializeCommands() {
-                    this._addCommandsForUnauthenticated(), this._addCommandsForAuthenticationInProgress(), this._addKeyShortcutsInfo(this._commandsForAutosuggestionDisabled), this._commandsForAutosuggestionDisabled.addCommand(v.CommandIDs.resumeAutoSuggestion, {
+                    this._addCommandsForUnauthenticated(), this._addCommandsForAuthenticationInProgress(), this._addKeyShortcutsInfo(this._commandsForAutosuggestionDisabled), this._commandsForAutosuggestionDisabled.addCommand(I.CommandIDs.resumeAutoSuggestion, {
                         label: d.message("codewhisperer_resume_auto_suggestion"),
                         icon: l.Icons.resumeIcon,
                         caption: d.message("codewhisperer_resume_auto_suggestion"),
                         execute: async () => {
-                            this._handleClick(), h.AutoTrigger.getInstance().enabled = !0, await w.saveState(I.AUTO_SUGGESTION, !0)
+                            this._handleClick(), h.AutoTrigger.getInstance().enabled = !0, await w.saveState(v.AUTO_SUGGESTION, !0)
                         }
-                    }), this._addCommandsForAuthenticatedCommon(this._commandsForAutosuggestionDisabled), this._addKeyShortcutsInfo(this._commandsForAutoSuggestionEnabled), this._commandsForAutoSuggestionEnabled.addCommand(v.CommandIDs.pauseAutoSuggestion, {
+                    }), this._addCommandsForAuthenticatedCommon(this._commandsForAutosuggestionDisabled), _.Application.getInstance().isGlueStudioNoteBook() && this._addCommandsForAuthenticatedGlueStudio(this._commandsForAutosuggestionDisabled), this._addKeyShortcutsInfo(this._commandsForAutoSuggestionEnabled), this._commandsForAutoSuggestionEnabled.addCommand(I.CommandIDs.pauseAutoSuggestion, {
                         label: d.message("codewhisperer_pause_auto_suggestion"),
                         icon: l.Icons.pauseIcon,
                         caption: d.message("codewhisperer_pause_auto_suggestion"),
                         execute: async () => {
-                            this._handleClick(), h.AutoTrigger.getInstance().enabled = !1, await w.saveState(I.AUTO_SUGGESTION, !1)
+                            this._handleClick(), h.AutoTrigger.getInstance().enabled = !1, await w.saveState(v.AUTO_SUGGESTION, !1)
                         }
-                    }), this._addCommandsForAuthenticatedCommon(this._commandsForAutoSuggestionEnabled)
+                    }), this._addCommandsForAuthenticatedCommon(this._commandsForAutoSuggestionEnabled), _.Application.getInstance().isGlueStudioNoteBook() && this._addCommandsForAuthenticatedGlueStudio(this._commandsForAutoSuggestionEnabled)
                 }
                 render() {
-                    const e = p.Worker.getInstance().isGetCompletionsRunning,
-                        t = g.AuthManager.getInstance().isAuthenticated() ? e ? r.default.createElement(l.Icons.loadingIcon.react, {
+                    const e = m.Worker.getInstance().isGetCompletionsRunning,
+                        t = u.AuthManager.getInstance().isAuthenticated() ? e ? r.default.createElement(l.Icons.loadingIcon.react, {
                             tag: "span",
                             className: "cwspr-statusbarwidget-icon"
                         }) : r.default.createElement(l.Icons.connectedIcon.react, {
                             tag: "span",
                             className: "cwspr-statusbarwidget-icon"
-                        }) : g.AuthManager.getInstance().isAuthenticationInProgress() ? r.default.createElement(l.Icons.loadingIcon.react, {
+                        }) : u.AuthManager.getInstance().isAuthenticationInProgress() ? r.default.createElement(l.Icons.loadingIcon.react, {
                             tag: "span",
                             className: "cwspr-statusbarwidget-icon"
                         }) : r.default.createElement(l.Icons.disconnectedIcon.react, {
                             tag: "span",
                             className: "cwspr-statusbarwidget-icon"
                         });
-                    return r.default.createElement("div", {
-                        className: "cwspr-statusbarwidget",
-                        onClick: () => this._handleClick()
-                    }, t, r.default.createElement("span", null, this._getStatusBarWidgetDisplayText()))
+                    return r.default.createElement(s.GroupItem, {
+                        spacing: 0,
+                        onClick: () => this._handleClick(),
+                        className: "cwspr-statusbarwidget"
+                    }, t, r.default.createElement(s.TextItem, {
+                        source: this._getStatusBarWidgetDisplayText()
+                    }))
                 }
                 _getStatusBarWidgetDisplayText() {
-                    return g.AuthManager.getInstance().isAuthenticated() ? d.message("codewhisperer_status_widget_text_authenticated") : g.AuthManager.getInstance().isAuthenticationInProgress() ? d.message("codewhisperer_status_widget_text_auth_in_progress") : d.message("codewhisperer_status_widget_text_not_authenticated")
+                    return u.AuthManager.getInstance().isAuthenticated() ? d.message("codewhisperer_status_widget_text_authenticated") : u.AuthManager.getInstance().isAuthenticationInProgress() ? d.message("codewhisperer_status_widget_text_auth_in_progress") : d.message("codewhisperer_status_widget_text_not_authenticated")
                 }
                 _handleClick() {
                     const e = this._getMenu();
                     if (null !== this._popup && !this._popup.isDisposed) return this._popup.dispose(), void(this._popup = null);
-                    this._menuToggled(), e.aboutToClose.connect(this._menuToggled, this), this._popup = s.showPopup({
+                    this._popup = s.showPopup({
                         body: e,
                         anchor: this,
                         align: "left"
-                    })
-                }
-                _menuToggled() {
-                    this.toggleClass("jp-mod-clicked")
+                    }), this._menu = e
                 }
                 _getMenu() {
                     const e = h.AutoTrigger.getInstance().enabled;
                     let t;
-                    t = g.AuthManager.getInstance().isAuthenticated() ? e ? this._commandsForAutoSuggestionEnabled : this._commandsForAutosuggestionDisabled : g.AuthManager.getInstance().isAuthenticationInProgress() ? this._commandsForAuthenticationInProgress : this._commandsForNotAuthenticated;
+                    t = u.AuthManager.getInstance().isAuthenticated() ? e ? this._commandsForAutoSuggestionEnabled : this._commandsForAutosuggestionDisabled : u.AuthManager.getInstance().isAuthenticationInProgress() ? this._commandsForAuthenticationInProgress : this._commandsForNotAuthenticated;
                     const n = new a.Menu({
                         commands: t,
                         renderer: this._renderer
                     });
-                    return n.addClass("cwspr-statusbarwidget-menu"), this._addCommands(n, t), g.AuthManager.getInstance().isAuthenticated() && n.insertItem(this._keyShortcutsInfoRows, {
+                    return n.addClass("cwspr-statusbarwidget-menu"), this._addCommands(n, t), u.AuthManager.getInstance().isAuthenticated() && n.insertItem(this._keyShortcutsInfoRows, {
+                        type: "separator"
+                    }), _.Application.getInstance().isGlueStudioNoteBook() && n.insertItem(this._toggleSettingsforGlueStudioRows, {
                         type: "separator"
                     }), n.update(), n
                 }
                 _addCommands(e, t) {
                     for (let n = 0; n < t.listCommands().length; n++) e.addItem({
                         command: t.listCommands()[n]
                     });
                     e.update()
                 }
             }
-            class S extends a.Menu.Renderer {
+            class T extends a.Menu.Renderer {
                 renderItem(e) {
                     let t = this.createItemClass(e),
                         n = this.createItemDataset(e),
-                        i = this.createItemARIA(e);
-                    return u.h.li({
+                        i = this.createItemARIA(e),
+                        o = [this.renderIcon(e), this.renderLabel(e), this.renderShortcut(e), this.renderSubmenu(e)];
+                    return this._isToggleButton(e) ? o.push(this._renderSettingToggleButton(e)) : o.push(this._renderCodeWhispererShortCut(e)), g.h.li({
                         className: t,
                         dataset: n,
                         tabindex: "0",
                         onfocus: e.onfocus,
                         ...i
-                    }, this.renderIcon(e), this.renderLabel(e), this.renderShortcut(e), this.renderSubmenu(e), this._renderCodeWhispererShortCut(e))
+                    }, ...o)
                 }
                 _renderCodeWhispererShortCut(e) {
                     const t = this._getKeyShortcutButtons(e);
-                    return u.h.div({
+                    return g.h.div({
                         className: "cwspr-key-shortcut-menu"
                     }, ...t)
                 }
                 _getKeyShortcutButtons(e) {
                     if (e.item.isEnabled || e.item.label == d.message("codewhisperer_key_shortcut_title")) return [""];
                     let t;
                     switch (e.item.label) {
                         case d.message("codewhisperer_key_shortcut_accept"):
-                            t = C.Keybindings.getInstance().getKeybinding(v.MESSAGE_TO_CMD_ID_MAP.codewhisperer_key_shortcut_accept);
+                            t = C.Keybindings.getInstance().getKeybinding(I.MESSAGE_TO_CMD_ID_MAP.codewhisperer_key_shortcut_accept);
                             break;
                         case d.message("codewhisperer_key_shortcut_manual_trigger"):
-                            t = C.Keybindings.getInstance().getKeybinding(v.MESSAGE_TO_CMD_ID_MAP.codewhisperer_key_shortcut_manual_trigger);
+                            t = C.Keybindings.getInstance().getKeybinding(I.MESSAGE_TO_CMD_ID_MAP.codewhisperer_key_shortcut_manual_trigger);
                             break;
                         case d.message("codewhisperer_key_shortcut_navigate"):
                             t = ["Up & Down"];
                             break;
                         case d.message("codewhisperer_key_shortcut_reject"):
-                            t = C.Keybindings.getInstance().getKeybinding(v.MESSAGE_TO_CMD_ID_MAP.codewhisperer_key_shortcut_reject);
+                            t = C.Keybindings.getInstance().getKeybinding(I.MESSAGE_TO_CMD_ID_MAP.codewhisperer_key_shortcut_reject);
                             break;
                         default:
                             t = []
                     }
-                    return t.map((e => u.h.div({
+                    return t.map((e => g.h.div({
                         className: "cwspr-key-shortcut-button"
                     }, e)))
                 }
+                _renderSettingToggleButton(e) {
+                    const t = this._getToggleButton(e);
+                    return g.h.div({
+                        className: "cwspr-key-shortcut-menu"
+                    }, t)
+                }
+                _getToggleButton(e) {
+                    if (!this._isToggleButton(e)) return [""];
+                    const t = e.item.label == d.message("codewhisperer_toggle_telemetry"),
+                        n = t ? f.Telemetry.getInstance().isTelemetryEnabled() ? "true" : "false" : m.Worker.getInstance().isSuggestionsWithCodeReferencesEnabled() ? "true" : "false",
+                        i = t ? I.CommandIDs.toggleTelemetry : I.CommandIDs.toggleCodeReferences;
+                    return g.h.button({
+                        id: i,
+                        className: "jp-switch cwspr-menu-toggle-button",
+                        role: "switch",
+                        "aria-checked": n,
+                        onclick: () => {
+                            _.Application.getInstance().toggleSettingSignal.emit(i)
+                        }
+                    }, g.h.div({
+                        className: "jp-switch-track",
+                        "aria-hidden": "true"
+                    }, null))
+                }
+                _isToggleButton(e) {
+                    return e.item.label == d.message("codewhisperer_toggle_telemetry") || e.item.label == d.message("codewhisperer_toggle_code_references")
+                }
             }
-            t.default = y
+            t.default = S
         },
         9805: (e, t, n) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.Telemetry = void 0;
             const i = n(7857),
                 o = n(4872),
@@ -1722,14 +1784,17 @@
                             this.logger.error(e)
                         }
                     }), c.defaultFlushPeriodMillis)
                 }
                 enableTelemetry(e) {
                     this._telemetryEnabled = e
                 }
+                isTelemetryEnabled() {
+                    return this._telemetryEnabled
+                }
                 closeTimer() {
                     void 0 !== this._timer && (clearTimeout(this._timer), this._timer = void 0)
                 }
                 async flush() {
                     if (this._telemetryEnabled && (void 0 === this.telemetryClient && (this.telemetryClient = new i.TelemetryApiClient), void 0 !== this.telemetryClient)) {
                         for (; 0 !== this._eventQueue.length;) {
                             const e = this._eventQueue.splice(0, c.defaultMaxBatchSize);
@@ -1780,15 +1845,15 @@
         },
         9513: (e, t) => {
             var n, i, o;
             Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.SettingIDs = t.HttpStatusCode = t.MESSAGE_TO_CMD_ID_MAP = t.PLUGIN_ID = t.CommandIDs = t.NOTIFICATION_TEXT_LIMIT = t.NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS = t.SHOW_COMPLETION_TIMER_POLL_PERIOD = t.INLINE_COMPLETION_SHOW_DELAY = t.AWS_BUILDER_ID_START_URL = t.MAX_PAGINATION_CALLS = t.MAX_RECOMMENDATIONS = t.MAX_LENGTH = t.CWSPR_DOCUMENTATION = t.UPDATE_NOTIFICATION_URL = t.LEARN_MORE_NOTIFICATION_URL = t.TELEMETRY_USER_TRIGGER_DECISION_METRIC_NAME = t.TELEMETRY_USER_DECISION_METRIC_NAME = t.TELEMETRY_SERVICE_INVOCATION_METRIC_NAME = void 0, t.TELEMETRY_SERVICE_INVOCATION_METRIC_NAME = "codewhisperer_serviceInvocation", t.TELEMETRY_USER_DECISION_METRIC_NAME = "codewhisperer_userDecision", t.TELEMETRY_USER_TRIGGER_DECISION_METRIC_NAME = "codewhisperer_userTriggerDecision", t.LEARN_MORE_NOTIFICATION_URL = "https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html", t.UPDATE_NOTIFICATION_URL = "https://pypi.org/project/amazon-codewhisperer-jupyterlab-ext/", t.CWSPR_DOCUMENTATION = "https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html", t.MAX_LENGTH = 10240, t.MAX_RECOMMENDATIONS = 5, t.MAX_PAGINATION_CALLS = 10, t.AWS_BUILDER_ID_START_URL = "https://view.awsapps.com/start", t.INLINE_COMPLETION_SHOW_DELAY = 250, t.SHOW_COMPLETION_TIMER_POLL_PERIOD = 25, t.NEW_CELL_AUTO_TRIGGER_DELAY_IN_MS = 1e4, t.NOTIFICATION_TEXT_LIMIT = 140,
                 function(e) {
-                    e.invoke = "completer:invoke", e.invokeNotebook = "completer:invoke-notebook", e.invokeFile = "completer:invoke-file", e.select = "completer:select", e.selectNotebook = "completer:select-notebook", e.login = "codewhisperer:login", e.invokeInline = "codewhisperer:invoke-inline", e.rejectInline = "codewhisperer:reject-inline", e.acceptInline = "codewhisperer:accept-inline", e.showNext = "codewhisperer:show-next", e.showPrev = "codewhisperer:show-prev", e.startCodeWhisperer = "codewhisperer:start", e.cancelLogin = "codewhisperer:cancel-login", e.openDocumentation = "codewhisperer:documentation", e.pauseAutoSuggestion = "codewhisperer:pause-auto-suggestion", e.resumeAutoSuggestion = "codewhisperer:resume-auto-suggestion", e.openReferenceLog = "codewhisperer:open-reference-log", e.signOut = "codewhisperer:sign-out", e.keyShortcutTitle = "codewhisperer:key-shortcut-title", e.keyShortcutAccept = "codewhisperer:key-shortcut-accept", e.keyShortcutManualTrigger = "codewhisperer:key-shortcut-manual-trigger", e.keyShortcutNavigate = "codewhisperer:key-shortcut-navigate", e.keyShortcutReject = "codewhisperer:key-shortcut-reject"
+                    e.invoke = "completer:invoke", e.invokeNotebook = "completer:invoke-notebook", e.invokeFile = "completer:invoke-file", e.select = "completer:select", e.selectNotebook = "completer:select-notebook", e.login = "codewhisperer:login", e.invokeInline = "codewhisperer:invoke-inline", e.rejectInline = "codewhisperer:reject-inline", e.acceptInline = "codewhisperer:accept-inline", e.showNext = "codewhisperer:show-next", e.showPrev = "codewhisperer:show-prev", e.startCodeWhisperer = "codewhisperer:start", e.cancelLogin = "codewhisperer:cancel-login", e.openDocumentation = "codewhisperer:documentation", e.pauseAutoSuggestion = "codewhisperer:pause-auto-suggestion", e.resumeAutoSuggestion = "codewhisperer:resume-auto-suggestion", e.openReferenceLog = "codewhisperer:open-reference-log", e.signOut = "codewhisperer:sign-out", e.keyShortcutTitle = "codewhisperer:key-shortcut-title", e.keyShortcutAccept = "codewhisperer:key-shortcut-accept", e.keyShortcutManualTrigger = "codewhisperer:key-shortcut-manual-trigger", e.keyShortcutNavigate = "codewhisperer:key-shortcut-navigate", e.keyShortcutReject = "codewhisperer:key-shortcut-reject", e.toggleTelemetry = "codewhisperer:toggle-telemetry", e.toggleCodeReferences = "codewhisperer:toggle-code-references"
                 }(n = t.CommandIDs || (t.CommandIDs = {})), t.PLUGIN_ID = "amazon-codewhisperer-jupyterlab-ext:completer", t.MESSAGE_TO_CMD_ID_MAP = {
                     codewhisperer_key_shortcut_accept: n.acceptInline,
                     codewhisperer_key_shortcut_manual_trigger: n.invokeInline,
                     codewhisperer_key_shortcut_reject: n.rejectInline
                 }, (o = t.HttpStatusCode || (t.HttpStatusCode = {}))[o.OK = 200] = "OK", o[o.NOT_FOUND = 404] = "NOT_FOUND", (i = t.SettingIDs || (t.SettingIDs = {})).keyOptOut = "shareCodeWhispererContentWithAWS", i.keyTelemetry = "codeWhispererTelemetry", i.keyReferences = "suggestionsWithCodeReferences", i.keyLogLevel = "codeWhispererLogLevel"
         },
         7126: (e, t) => {
@@ -1912,14 +1977,14 @@
         9206: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => i
             });
             const i = '<?xml version="1.0" encoding="utf-8"?>\n\x3c!-- Generator: Adobe Illustrator 27.4.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  --\x3e\n<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"\n\t viewBox="0 0 17 17" style="enable-background:new 0 0 17 17;" xml:space="preserve">\n<circle class="jp-icon2" fill="#424242" cx="8.5" cy="8.5" r="8.5"/>\n<g>\n\t<path class="jp-icon-accent1" fill="#FFFFFF" d="M8.5,5.3L10.1,7l0.7-0.7L8.5,3.9L6.2,6.2L6.9,7L8.5,5.3z M8.5,11.7L6.9,10l-0.7,0.7l2.3,2.4l2.3-2.4L10.1,10\n\t\tL8.5,11.7z"/>\n</g>\n</svg>\n'
         },
         8123: e => {
-            e.exports = JSON.parse('{"codewhisperer_status_widget_text_not_authenticated":"CodeWhisperer","codewhisperer_status_widget_text_auth_in_progress":"CodeWhisperer(Connecting...)","codewhisperer_status_widget_text_authenticated":"CodeWhisperer","codewhisperer_start":"Start CodeWhisperer","codewhisperer_cancel_login":"Cancel Login","codewhisperer_learn_more":"Learn More","codewhisperer_update_now":"Update Now","codewhisperer_documentation_open":"Documentation","codewhisperer_pause_auto_suggestion":"Pause Auto-Suggestions","codewhisperer_resume_auto_suggestion":"Resume Auto-Suggestions","codewhisperer_reference_log_open":"Open Code Reference Log","codewhisperer_sign_out":"Sign Out","codewhisperer_key_shortcut_title":"SHORTCUTS","codewhisperer_key_shortcut_accept":"Accept","codewhisperer_key_shortcut_manual_trigger":"Manual Invoke","codewhisperer_key_shortcut_navigate":"Navigate","codewhisperer_key_shortcut_reject":"Reject","codewhisperer_expiry_notification_message":"CodeWhisperer connection expired. Reauthenticate with AWS Builder ID to use CodeWhisperer.","codewhisperer_expiry_notification_button_authenticate":"Authenticate","codewhisperer_expiry_notification_button_cancel":"Cancel","codewhisperer_copy_code_and_proceed_dialog_title":"Start CodeWhisperer with AWS Builder ID","codewhisperer_copy_code_and_proceed_dialog_button_yes":"Copy Code and Proceed","codewhisperer_copy_code_and_proceed_dialog_message_first_li":"To use CodeWhisperer, individual developers must sign in using AWS Builder ID. ","codewhisperer_copy_code_and_proceed_dialog_message_first_li_learn_more":"Learn More","codewhisperer_copy_code_and_proceed_dialog_message_second_li":"A login page will open on an external website: https://device.sso.us-east-1.amazonaws.com","codewhisperer_copy_code_and_proceed_dialog_message_third_li":"Provide this code to confirm the access request: ","codewhisperer_server_extension_not_enabled_message":"CodeWhisperer isn\'t enabled. Run `jupyter server extension enable amazon_codewhisperer_jupyterlab_ext`, then restart server & refresh browser.","codewhisperer_update_notification_skip_this_version":"Skip this version","codewhisperer_notification_show_full_message_button_title":"Expand"}')
+            e.exports = JSON.parse('{"codewhisperer_status_widget_text_not_authenticated":"CodeWhisperer","codewhisperer_status_widget_text_auth_in_progress":"CodeWhisperer(Connecting...)","codewhisperer_status_widget_text_authenticated":"CodeWhisperer","codewhisperer_start":"Start CodeWhisperer","codewhisperer_cancel_login":"Cancel Login","codewhisperer_learn_more":"Learn More","codewhisperer_update_now":"Update Now","codewhisperer_documentation_open":"Documentation","codewhisperer_pause_auto_suggestion":"Pause Auto-Suggestions","codewhisperer_resume_auto_suggestion":"Resume Auto-Suggestions","codewhisperer_reference_log_open":"Open Code Reference Log","codewhisperer_sign_out":"Sign Out","codewhisperer_toggle_telemetry":"Share telemetry with AWS","codewhisperer_toggle_code_references":"Code with references","codewhisperer_key_shortcut_title":"SHORTCUTS","codewhisperer_key_shortcut_accept":"Accept","codewhisperer_key_shortcut_manual_trigger":"Manual Invoke","codewhisperer_key_shortcut_navigate":"Navigate","codewhisperer_key_shortcut_reject":"Reject","codewhisperer_expiry_notification_message":"CodeWhisperer connection expired. Reauthenticate with AWS Builder ID to use CodeWhisperer.","codewhisperer_expiry_notification_button_authenticate":"Authenticate","codewhisperer_expiry_notification_button_cancel":"Cancel","codewhisperer_copy_code_and_proceed_dialog_title":"Start CodeWhisperer with AWS Builder ID","codewhisperer_copy_code_and_proceed_dialog_button_yes":"Copy Code and Proceed","codewhisperer_copy_code_and_proceed_dialog_message_first_li":"To use CodeWhisperer, individual developers must sign in using AWS Builder ID. ","codewhisperer_copy_code_and_proceed_dialog_message_first_li_learn_more":"Learn More","codewhisperer_copy_code_and_proceed_dialog_message_second_li":"A login page will open on an external website: https://device.sso.us-east-1.amazonaws.com","codewhisperer_copy_code_and_proceed_dialog_message_third_li":"Provide this code to confirm the access request: ","codewhisperer_server_extension_not_enabled_message":"CodeWhisperer isn\'t enabled. Run `jupyter server extension enable amazon_codewhisperer_jupyterlab_ext`, then restart server & refresh browser.","codewhisperer_update_notification_skip_this_version":"Skip this version","codewhisperer_notification_show_full_message_button_title":"Expand"}')
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"amazon-codewhisperer-jupyterlab-ext","version":"1.0.3","description":"Amazon CodeWhisperer for JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","codewhisperer","amazon-codewhisperer"],"homepage":"https://github.com/aws","bugs":{"url":"https://aws.amazon.com/codewhisperer/","email":"codewhisperer@amazon.com"},"license":"Apache 2.0","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"author":{"name":"Amazon CodeWhisperer","email":"codewhisperer@amazon.com"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,eot,js,gif,html,jpg,json,png,svg,woff2,ttf}","style/img/*.{svg}","schema/*.json"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","config":{"vars":{"builddir":"./build/lib/amazon-codewhisperer-jupyterlab-ext","jupyterCorePath":"./build-tools/jupyter-staging"}},"npm-pretty-much":{"https://w/?NpmPrettyMuch/UndeclaredTransitiveDependencies":true,"legacyPackageNameAlias":"amazon-codewhisperer-jupyterlab-ext","runTest":"always","runRelease":"always"},"scripts":{"build":"npm run clean && npm run build:lib && npm run build:labextension","postbuild":"mkdir -p $npm_package_config_vars_builddir && rsync package.json $npm_package_config_vars_builddir && rsync -a --exclude={‘*.spec.d.ts’,’*.spec.js’} lib $npm_package_config_vars_builddir && rsync -a style $npm_package_config_vars_builddir","build:all":"npm run build:lib && npm run build:labextension","build:labextension":"build-labextension --core-path $npm_package_config_vars_jupyterCorePath .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:prod":"npm run clean && npm run build:lib && npm run build:labextension","clean":"npm run clean:lib","clean:all":"npm run clean:lib && npm run clean:labextension","clean:labextension":"rimraf amazon_codewhisperer_jupyterlab_ext/labextension","clean:lib":"rimraf lib tsconfig.tsbuildinfo","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"npm run build","dev":"npm run clean && npm run build:lib && npm run build:labextension:dev","dist":"python setup.py sdist","release":"npm run build && npm run postbuild && npm run dist","watch":"run-p watch:src watch:labextension","watch:labextension":"jupyter labextension watch .","watch:src":"tsc -w","generateTelemetry":"node node_modules/@aws-toolkits/telemetry/lib/generateTelemetry.js --output=src/telemetry/telemetry.gen.ts","generateClients":"ts-node ./scripts/build/generateServiceClient.ts ","test":"jest --no-cache"},"dependencies":{"@jupyterlab/application":"^3.1.0","@jupyterlab/apputils":"^3.1.0","@jupyterlab/codeeditor":"^3.1.0","@jupyterlab/codemirror":"^3.1.0","@jupyterlab/completer":"^3.1.0","@jupyterlab/fileeditor":"^3.1.0","@jupyterlab/launcher":"^3.1.0","@jupyterlab/logconsole":"^3.6.3","@jupyterlab/nbformat":"^3.6.3","@jupyterlab/notebook":"^3.1.0","@jupyterlab/outputarea":"^3.1.0","@jupyterlab/rendermime":"^3.6.3","@jupyterlab/settingregistry":"^3.1.0","@jupyterlab/statedb":"^3.6.3","@jupyterlab/translation":"^3.1.0","@lumino/algorithm":"^1.6.0","@lumino/coreutils":"^1.8.0","@lumino/datagrid":"^0.27.0","@lumino/disposable":"^1.7.0","aws-sdk":"^2.1267.0","pino":"^8.11.0"},"devDependencies":{"@aws-toolkits/telemetry":"^1.0.120","@babel/core":"^7.21.5","@babel/preset-env":"^7.21.5","@jupyterlab/builder":"^3.6.3","@jupyterlab/testutils":"^3.6.3","@types/codemirror":"^5.60.7","@types/fs-extra":"^9.0.11","@types/jest":"27.0.0","@types/node":"^16.0.0","@typescript-eslint/eslint-plugin":"^4.8.1","@typescript-eslint/parser":"^4.8.1","eslint":"^7.14.0","eslint-config-prettier":"^6.15.0","eslint-plugin-jsdoc":"^40.0.0","eslint-plugin-prettier":"^3.1.4","eslint-plugin-react":"^7.18.3","jest":"27.0.0","jest-fetch-mock":"^1.6.6","npm-run-all":"^4.1.5","prettier":"^2.1.1","rimraf":"^3.0.2","ts-jest":"27.0.0","typescript":"~4.3.0","jest-environment-jsdom":"^27.0.0","pino-pretty":"10.0.0"},"sideEffects":["style/*.css","style/index.js"],"jupyterlab":{"extension":true,"schemaDir":"schema","outputDir":"amazon_codewhisperer_jupyterlab_ext/labextension","disabledExtensions":["@jupyterlab/completer-extension:notebooks","@jupyterlab/completer-extension:files"]},"styleModule":"style/index.js"}')
+            e.exports = JSON.parse('{"name":"amazon-codewhisperer-jupyterlab-ext","version":"1.0.4","description":"Amazon CodeWhisperer for JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","codewhisperer","amazon-codewhisperer"],"homepage":"https://github.com/aws","bugs":{"url":"https://aws.amazon.com/codewhisperer/","email":"codewhisperer@amazon.com"},"license":"Apache 2.0","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"author":{"name":"Amazon CodeWhisperer","email":"codewhisperer@amazon.com"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,eot,js,gif,html,jpg,json,png,svg,woff2,ttf}","style/img/*.{svg}","schema/*.json"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","config":{"vars":{"builddir":"./build/lib/amazon-codewhisperer-jupyterlab-ext","jupyterCorePath":"./build-tools/jupyter-staging"}},"npm-pretty-much":{"https://w/?NpmPrettyMuch/UndeclaredTransitiveDependencies":true,"legacyPackageNameAlias":"amazon-codewhisperer-jupyterlab-ext","runTest":"always","runRelease":"always"},"scripts":{"build":"npm run clean && npm run build:lib && npm run build:labextension","postbuild":"mkdir -p $npm_package_config_vars_builddir && rsync package.json $npm_package_config_vars_builddir && rsync -a --exclude={‘*.spec.d.ts’,’*.spec.js’} lib $npm_package_config_vars_builddir && rsync -a style $npm_package_config_vars_builddir","build:all":"npm run build:lib && npm run build:labextension","build:labextension":"build-labextension --core-path $npm_package_config_vars_jupyterCorePath .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:prod":"npm run clean && npm run build:lib && npm run build:labextension","clean":"npm run clean:lib","clean:all":"npm run clean:lib && npm run clean:labextension","clean:labextension":"rimraf amazon_codewhisperer_jupyterlab_ext/labextension","clean:lib":"rimraf lib tsconfig.tsbuildinfo","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"npm run build","dev":"npm run clean && npm run build:lib && npm run build:labextension:dev","dist":"python setup.py sdist","release":"npm run build && npm run postbuild && npm run dist","watch":"run-p watch:src watch:labextension","watch:labextension":"jupyter labextension watch .","watch:src":"tsc -w","generateTelemetry":"node node_modules/@aws-toolkits/telemetry/lib/generateTelemetry.js --output=src/telemetry/telemetry.gen.ts","generateClients":"ts-node ./scripts/build/generateServiceClient.ts ","test":"jest --no-cache"},"dependencies":{"@jupyterlab/application":"^3.1.0","@jupyterlab/apputils":"^3.1.0","@jupyterlab/codeeditor":"^3.1.0","@jupyterlab/codemirror":"^3.1.0","@jupyterlab/completer":"^3.1.0","@jupyterlab/fileeditor":"^3.1.0","@jupyterlab/launcher":"^3.1.0","@jupyterlab/logconsole":"^3.6.3","@jupyterlab/nbformat":"^3.6.3","@jupyterlab/notebook":"^3.1.0","@jupyterlab/outputarea":"^3.1.0","@jupyterlab/rendermime":"^3.6.3","@jupyterlab/settingregistry":"^3.1.0","@jupyterlab/statedb":"^3.6.3","@jupyterlab/translation":"^3.1.0","@lumino/algorithm":"^1.6.0","@lumino/coreutils":"^1.8.0","@lumino/datagrid":"^0.27.0","@lumino/disposable":"^1.7.0","aws-sdk":"^2.1267.0","pino":"^8.11.0"},"devDependencies":{"@aws-toolkits/telemetry":"^1.0.120","@babel/core":"^7.21.5","@babel/preset-env":"^7.21.5","@jupyterlab/builder":"^3.6.3","@jupyterlab/testutils":"^3.6.3","@types/codemirror":"^5.60.7","@types/fs-extra":"^9.0.11","@types/jest":"27.0.0","@types/node":"^16.0.0","@typescript-eslint/eslint-plugin":"^4.8.1","@typescript-eslint/parser":"^4.8.1","eslint":"^7.14.0","eslint-config-prettier":"^6.15.0","eslint-plugin-jsdoc":"^40.0.0","eslint-plugin-prettier":"^3.1.4","eslint-plugin-react":"^7.18.3","jest":"27.0.0","jest-fetch-mock":"^1.6.6","npm-run-all":"^4.1.5","prettier":"^2.1.1","rimraf":"^3.0.2","ts-jest":"27.0.0","typescript":"~4.3.0","jest-environment-jsdom":"^27.0.0","pino-pretty":"10.0.0"},"sideEffects":["style/*.css","style/index.js"],"jupyterlab":{"extension":true,"schemaDir":"schema","outputDir":"amazon_codewhisperer_jupyterlab_ext/labextension","disabledExtensions":["@jupyterlab/completer-extension:notebooks","@jupyterlab/completer-extension:files"]},"styleModule":"style/index.js"}')
         }
     }
 ]);
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.3582fd184eff1ff4b836.js` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/571.3582fd184eff1ff4b836.js`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.462ff5e5d49d87208721.js` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/747.4a2fe27171322cd7b67e.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
             t.d(e, {
                 Z: () => a
             });
             var r = t(3645),
                 i = t.n(r)()((function(n) {
                     return n[1]
                 }));
-            i.push([n.id, '.cwspr-statusbarwidget-parent.jp-mod-clicked div span {\n    color: white;\n}\n\n.cwspr-statusbarwidget-menu {\n    width: 225px !important;\n}\n\n.cwspr-statusbarwidget, .cwspr-statusbarwidget-icon {\n    vertical-align: middle;\n}\n\n.cwspr-statusbarwidget-icon {\n    line-height: initial !important;\n    padding-right: 3px;\n}\n\n.cwspr-statusbarwidget span {\n    display: inline-block;\n}\n\nli[data-command^="codewhisperer:"] {\n    display: list-item;\n    width: 225px;\n}\n\nli[data-command^="codewhisperer:key-shortcut-"] .lm-Menu-itemLabel, .p-Menu-itemLabel, .cwspr-key-shortcut-menu {\n    color: var(--jp-ui-font-color1)\n}\n\nli[data-command^="codewhisperer:key-shortcut-"] .lm-Menu-itemIcon {\n    width: 0;\n    padding-right: 3px;\n}\n\nli[data-command^="codewhisperer:key-shortcut-"] .p-Menu-itemIcon {\n    width: 0;\n    padding-right: 3px;\n}\n\nli[data-command^="codewhisperer:"] .lm-Menu-itemLabel {\n    padding-right: 0;\n}\n\nli[data-command^="codewhisperer:"] .p-Menu-itemLabel {\n    padding-right: 0;\n}\n\nli[data-command="codewhisperer:key-shortcut-title"] {\n    font-weight: bold;\n}\n\nli[data-command^="codewhisperer:"] svg {\n    vertical-align: text-top;\n    padding: 0 3px 0 5px;\n}\n\n.cwspr-key-shortcut-menu {\n    display: table-cell;\n    text-align: right;\n    width: inherit;\n    padding-right: 10px;\n}\n\n.cwspr-key-shortcut-button {\n    display: inline-block;\n    padding-left: 4px;\n    padding-right: 4px;\n    border: 2px solid #F4F4F4;\n    line-height: 17px;\n    margin-left: 4px;\n    border-radius: 2px;\n}\n\n.cwspr-learn-more-link {\n    color: #106ba3\n}\n\n.cwspr-spinner {\n    animation: cwspr-spinner-rotator 1.4s linear infinite;\n}\n\n@keyframes cwspr-spinner-rotator {\n    0% { transform: rotate(0deg); }\n    100% { transform: rotate(270deg); }\n}\n\n.path {\n    fill: none;\n    stroke-dasharray: 187;\n    stroke-dashoffset: 0;\n    transform-origin: center;\n    animation:\n    dash 1.4s ease-in-out infinite;\n}\n\n@keyframes dash {\n    0% { stroke-dashoffset: 187; }\n    50% {\n        stroke-dashoffset: 46.75;\n        transform:rotate(135deg);\n    }\n    100% {\n        stroke-dashoffset: 187;\n        transform:rotate(450deg);\n    }\n}\n', ""]);
+            i.push([n.id, '.cwspr-statusbarwidget-parent.jp-mod-clicked div span {\n    color: white;\n}\n\n.cwspr-statusbarwidget-menu {\n    width: 225px !important;\n}\n\n.cwspr-statusbarwidget, .cwspr-statusbarwidget-icon {\n    vertical-align: middle;\n}\n\n.cwspr-statusbarwidget-icon {\n    line-height: initial !important;\n    padding-right: 3px;\n}\n\n.cwspr-statusbarwidget span {\n    display: inline-block;\n}\n\nli[data-command^="codewhisperer:"] {\n    display: list-item;\n    width: 225px;\n}\n\nli[data-command^="codewhisperer:key-shortcut-"] .lm-Menu-itemLabel, .p-Menu-itemLabel, .cwspr-key-shortcut-menu {\n    color: var(--jp-ui-font-color1)\n}\n\nli[data-command^="codewhisperer:key-shortcut-"] .lm-Menu-itemIcon {\n    width: 0;\n    padding-right: 3px;\n}\n\nli[data-command^="codewhisperer:key-shortcut-"] .p-Menu-itemIcon {\n    width: 0;\n    padding-right: 3px;\n}\n\nli[data-command^="codewhisperer:toggle"] .lm-Menu-itemIcon {\n    width: 0;\n    padding-right: 3px;\n}\n\nli[data-command^="codewhisperer:toggle"] .p-Menu-itemIcon {\n    width: 0;\n    padding-right: 3px;\n}\n\nli[data-command^="codewhisperer:"] .lm-Menu-itemLabel {\n    padding-right: 0;\n}\n\nli[data-command^="codewhisperer:"] .p-Menu-itemLabel {\n    padding-right: 0;\n}\n\nli[data-command="codewhisperer:key-shortcut-title"] {\n    font-weight: bold;\n}\n\nli[data-command^="codewhisperer:"] svg {\n    vertical-align: text-top;\n    padding: 0 3px 0 5px;\n}\n\n.cwspr-key-shortcut-menu {\n    display: table-cell;\n    text-align: right;\n    width: inherit;\n    padding-right: 10px;\n}\n\n.cwspr-key-shortcut-button {\n    display: inline-block;\n    padding-left: 4px;\n    padding-right: 4px;\n    border: 2px solid #F4F4F4;\n    line-height: 17px;\n    margin-left: 4px;\n    border-radius: 2px;\n}\n\n.cwspr-learn-more-link {\n    color: #106ba3\n}\n\n.cwspr-spinner {\n    animation: cwspr-spinner-rotator 1.4s linear infinite;\n}\n\n@keyframes cwspr-spinner-rotator {\n    0% { transform: rotate(0deg); }\n    100% { transform: rotate(270deg); }\n}\n\n.path {\n    fill: none;\n    stroke-dasharray: 187;\n    stroke-dashoffset: 0;\n    transform-origin: center;\n    animation:\n    dash 1.4s ease-in-out infinite;\n}\n\n@keyframes dash {\n    0% { stroke-dashoffset: 187; }\n    50% {\n        stroke-dashoffset: 46.75;\n        transform:rotate(135deg);\n    }\n    100% {\n        stroke-dashoffset: 187;\n        transform:rotate(450deg);\n    }\n}\n\n.cwspr-menu-toggle-button {\n    vertical-align: middle;\n    display: inline-flex;\n    padding-bottom: 2.5px;\n}\n\n.cwspr-menu-toggle-button:hover {\n    background-color: transparent;\n}\n', ""]);
             const a = i
         },
         3645: n => {
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
@@ -27,16 +27,16 @@
                     var i = {};
                     if (r)
                         for (var a = 0; a < this.length; a++) {
                             var o = this[a][0];
                             null != o && (i[o] = !0)
                         }
                     for (var s = 0; s < n.length; s++) {
-                        var c = [].concat(n[s]);
-                        r && i[c[0]] || (t && (c[2] ? c[2] = "".concat(t, " and ").concat(c[2]) : c[2] = t), e.push(c))
+                        var d = [].concat(n[s]);
+                        r && i[d[0]] || (t && (d[2] ? d[2] = "".concat(t, " and ").concat(d[2]) : d[2] = t), e.push(d))
                     }
                 }, e
             }
         },
         3379: (n, e, t) => {
             var r, i = function() {
                     var n = {};
@@ -62,33 +62,33 @@
                         break
                     } return e
             }
 
             function s(n, e) {
                 for (var t = {}, r = [], i = 0; i < n.length; i++) {
                     var s = n[i],
-                        c = e.base ? s[0] + e.base : s[0],
-                        d = t[c] || 0,
-                        l = "".concat(c, " ").concat(d);
-                    t[c] = d + 1;
+                        d = e.base ? s[0] + e.base : s[0],
+                        c = t[d] || 0,
+                        l = "".concat(d, " ").concat(c);
+                    t[d] = c + 1;
                     var p = o(l),
                         u = {
                             css: s[1],
                             media: s[2],
                             sourceMap: s[3]
                         }; - 1 !== p ? (a[p].references++, a[p].updater(u)) : a.push({
                         identifier: l,
                         updater: m(u, e),
                         references: 1
                     }), r.push(l)
                 }
                 return r
             }
 
-            function c(n) {
+            function d(n) {
                 var e = document.createElement("style"),
                     r = n.attributes || {};
                 if (void 0 === r.nonce) {
                     var a = t.nc;
                     a && (r.nonce = a)
                 }
                 if (Object.keys(r).forEach((function(n) {
@@ -97,16 +97,16 @@
                 else {
                     var o = i(n.insert || "head");
                     if (!o) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                     o.appendChild(e)
                 }
                 return e
             }
-            var d, l = (d = [], function(n, e) {
-                return d[n] = e, d.filter(Boolean).join("\n")
+            var c, l = (c = [], function(n, e) {
+                return c[n] = e, c.filter(Boolean).join("\n")
             });
 
             function p(n, e, t, r) {
                 var i = t ? "" : r.media ? "@media ".concat(r.media, " {").concat(r.css, "}") : r.css;
                 if (n.styleSheet) n.styleSheet.cssText = l(e, i);
                 else {
                     var a = document.createTextNode(i),
@@ -121,23 +121,23 @@
                     a = t.sourceMap;
                 if (i ? n.setAttribute("media", i) : n.removeAttribute("media"), a && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a)))), " */")), n.styleSheet) n.styleSheet.cssText = r;
                 else {
                     for (; n.firstChild;) n.removeChild(n.firstChild);
                     n.appendChild(document.createTextNode(r))
                 }
             }
-            var f = null,
-                h = 0;
+            var h = null,
+                f = 0;
 
             function m(n, e) {
                 var t, r, i;
                 if (e.singleton) {
-                    var a = h++;
-                    t = f || (f = c(e)), r = p.bind(null, t, a, !1), i = p.bind(null, t, a, !0)
-                } else t = c(e), r = u.bind(null, t, e), i = function() {
+                    var a = f++;
+                    t = h || (h = d(e)), r = p.bind(null, t, a, !1), i = p.bind(null, t, a, !0)
+                } else t = d(e), r = u.bind(null, t, e), i = function() {
                     ! function(n) {
                         if (null === n.parentNode) return !1;
                         n.parentNode.removeChild(n)
                     }(t)
                 };
                 return r(n),
                     function(e) {
@@ -152,19 +152,19 @@
                 var t = s(n = n || [], e);
                 return function(n) {
                     if (n = n || [], "[object Array]" === Object.prototype.toString.call(n)) {
                         for (var r = 0; r < t.length; r++) {
                             var i = o(t[r]);
                             a[i].references--
                         }
-                        for (var c = s(n, e), d = 0; d < t.length; d++) {
-                            var l = o(t[d]);
+                        for (var d = s(n, e), c = 0; c < t.length; c++) {
+                            var l = o(t[c]);
                             0 === a[l].references && (a[l].updater(), a.splice(l, 1))
                         }
-                        t = c
+                        t = d
                     }
                 }
             }
         },
         9747: (n, e, t) => {
             t.r(e);
             var r = t(3379),
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.9bf04351778104e8e5cd.js` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.f27b2e72fdec8f3ccdff.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, d, s, f, p, c, h, v, b, m, y, g, j, w, S, x = {
-            6972: (e, r, t) => {
-                var n = {
+    var e, r, t, a, n, o, i, u, l, s, d, f, p, c, h, v, b, m, y, g, j, w, S, x = {
+            8908: (e, r, t) => {
+                var a = {
                         "./index": () => t.e(568).then((() => () => t(1568))),
                         "./extension": () => t.e(568).then((() => () => t(1568))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
-                            var n = "default",
-                                o = t.S[n];
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[n] = e, t.I(n, r)
+                            var a = "default",
+                                n = t.S[a];
+                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[a] = e, t.I(a, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
-                    init: () => a
+                    get: () => n,
+                    init: () => o
                 })
             }
         },
         k = {};
 
     function E(e) {
         var r = k[e];
@@ -43,45 +43,45 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        568: "c0e5b626da6cbe06eb5e",
+        568: "5e4ac436f86b65d9e70f",
         571: "3582fd184eff1ff4b836",
-        747: "462ff5e5d49d87208721"
+        747: "4a2fe27171322cd7b67e"
     } [e] + ".js?v=" + {
-        568: "c0e5b626da6cbe06eb5e",
+        568: "5e4ac436f86b65d9e70f",
         571: "3582fd184eff1ff4b836",
-        747: "462ff5e5d49d87208721"
+        747: "4a2fe27171322cd7b67e"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "amazon-codewhisperer-jupyterlab-ext:", E.l = (t, n, o, a) => {
-        if (e[t]) e[t].push(n);
+    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "amazon-codewhisperer-jupyterlab-ext:", E.l = (t, a, n, o) => {
+        if (e[t]) e[t].push(a);
         else {
             var i, u;
-            if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var s = l[d];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+            if (void 0 !== n)
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var d = l[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
+                        i = d;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var f = (r, n) => {
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
+            var f = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(p);
-                    var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+                    var n = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
                 p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
@@ -91,147 +91,147 @@
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         E.S = {};
         var e = {},
             r = {};
-        E.I = (t, n) => {
-            n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
+        E.I = (t, a) => {
+            a || (a = []);
+            var n = r[t];
+            if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
+                if (a.push(n), e[t]) return e[t];
                 E.o(E.S, t) || (E.S[t] = {});
-                var a = E.S[t],
+                var o = E.S[t],
                     i = "amazon-codewhisperer-jupyterlab-ext",
-                    u = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
-                            u = o[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
+                    u = (e, r, t, a) => {
+                        var n = o[e] = o[e] || {},
+                            u = n[r];
+                        (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
-                            eager: !!n
+                            eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("amazon-codewhisperer-jupyterlab-ext", "1.0.3", (() => E.e(568).then((() => () => E(1568))))), u("pino", "8.11.0", (() => E.e(571).then((() => () => E(5571)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("amazon-codewhisperer-jupyterlab-ext", "1.0.4", (() => E.e(568).then((() => () => E(1568))))), u("pino", "8.11.0", (() => E.e(571).then((() => () => E(5571)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
-                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
+                for (var a = t.length - 1; a > -1 && !e;) e = t[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), E.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            n = t[1] ? r(t[1]) : [];
-        return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
-    }, n = (e, r) => {
+            a = t[1] ? r(t[1]) : [];
+        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
+    }, a = (e, r) => {
         e = t(e), r = t(r);
-        for (var n = 0;;) {
-            if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
-            var i = r[n],
+        for (var a = 0;;) {
+            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
+            var n = e[a],
+                o = (typeof n)[0];
+            if (a >= r.length) return "u" == o;
+            var i = r[a],
                 u = (typeof i)[0];
-            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
-            n++
+            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
+            if ("o" != o && "u" != o && n != i) return n < i;
+            a++
         }
-    }, o = e => {
+    }, n = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, u);
             return t
         }
         var i = [];
-        for (a = 1; a < e.length; a++) {
-            var u = e[a];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+        for (o = 1; o < e.length; o++) {
+            var u = e[o];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : n(u))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
-            var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
+            var a = e[0],
+                n = a < 0;
+            n && (a = -a - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
-                if ("u" == s) {
+                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > a && !n : "" == f != n);
+                if ("u" == d) {
                     if (!l || "u" != f) return !1
                 } else if (l)
-                    if (f == s)
-                        if (u <= n) {
-                            if (d != e[u]) return !1
+                    if (f == d)
+                        if (u <= a) {
+                            if (s != e[u]) return !1
                         } else {
-                            if (o ? d > e[u] : d < e[u]) return !1;
-                            d != e[u] && (l = !1)
+                            if (n ? s > e[u] : s < e[u]) return !1;
+                            s != e[u] && (l = !1)
                         }
                 else if ("s" != f && "n" != f) {
-                    if (o || u <= n) return !1;
+                    if (n || u <= a) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || s < f != o) return !1;
+                    if (u <= a || d < f != n) return !1;
                     l = !1
                 } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
-        return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
+        return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
-        var o = l(e, t);
-        return a(n, o) || c(d(e, t, o, n)), v(e[t][o])
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
+    }, s = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", d = (e, r, t, a) => {
+        var n = l(e, t);
+        return o(a, n) || c(s(e, t, n, a)), v(e[t][n])
     }, f = (e, r, t) => {
-        var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, p = (e, r, t, n) => {
-        var a = e[t];
-        return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
+        var n = e[r];
+        return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
+    }, p = (e, r, t, a) => {
+        var o = e[t];
+        return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, h = (e, r, t, n) => {
-        c(p(e, r, t, n))
-    }, v = e => (e.loaded = 1, e.get()), m = (b = e => function(r, t, n, o) {
-        var a = E.I(r);
-        return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), v(f(r, t, n) || h(r, e, t, n) || u(r, t))))), y = b(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
-        var a = r && E.o(r, t) && f(r, t, n);
-        return a ? v(a) : o()
+    }, h = (e, r, t, a) => {
+        c(p(e, r, t, a))
+    }, v = e => (e.loaded = 1, e.get()), m = (b = e => function(r, t, a, n) {
+        var o = E.I(r);
+        return o && o.then ? o.then(e.bind(e, r, E.S[r], t, a, n)) : e(r, E.S[r], t, a, n)
+    })(((e, r, t, a) => (i(e, t), v(f(r, t, a) || h(r, e, t, a) || u(r, t))))), y = b(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), g = b(((e, r, t, a, n) => {
+        var o = r && E.o(r, t) && f(r, t, a);
+        return o ? v(o) : n()
     })), j = {}, w = {
         968: () => y("default", "@jupyterlab/ui-components", [1, 3, 1, 11]),
         1396: () => y("default", "@jupyterlab/coreutils", [1, 5, 1, 11]),
         1797: () => y("default", "@lumino/coreutils", [1, 1, 5, 3]),
         2766: () => y("default", "@jupyterlab/notebook", [1, 3, 1, 11]),
         3706: () => y("default", "@lumino/widgets", [1, 1, 19, 0]),
         3961: () => y("default", "@jupyterlab/completer", [1, 3, 1, 11]),
@@ -255,56 +255,56 @@
         E.o(S, e) && S[e].forEach((e => {
             if (E.o(j, e)) return r.push(j[e]);
             var t = r => {
                     j[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
                     }
                 },
-                n = r => {
+                a = r => {
                     delete j[e], E.m[e] = t => {
                         throw delete E.c[e], r
                     }
                 };
             try {
-                var o = w[e]();
-                o.then ? r.push(j[e] = o.then(t).catch(n)) : t(o)
+                var n = w[e]();
+                n.then ? r.push(j[e] = n.then(t).catch(a)) : t(n)
             } catch (e) {
-                n(e)
+                a(e)
             }
         }))
     }, (() => {
         var e = {
             825: 0
         };
         E.f.j = (r, t) => {
-            var n = E.o(e, r) ? e[r] : void 0;
-            if (0 !== n)
-                if (n) t.push(n[2]);
+            var a = E.o(e, r) ? e[r] : void 0;
+            if (0 !== a)
+                if (a) t.push(a[2]);
                 else {
-                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                    t.push(n[2] = o);
-                    var a = E.p + E.u(r),
+                    var n = new Promise(((t, n) => a = e[r] = [t, n]));
+                    t.push(a[2] = n);
+                    var o = E.p + E.u(r),
                         i = new Error;
-                    E.l(a, (t => {
-                        if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var o = t && ("load" === t.type ? "missing" : t.type),
-                                a = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                    E.l(o, (t => {
+                        if (E.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
+                            var n = t && ("load" === t.type ? "missing" : t.type),
+                                o = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", i.name = "ChunkLoadError", i.type = n, i.request = o, a[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, o, [a, i, u] = t,
+                var a, n, [o, i, u] = t,
                     l = 0;
-                if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) E.o(i, n) && (E.m[n] = i[n]);
+                if (o.some((r => 0 !== e[r]))) {
+                    for (a in i) E.o(i, a) && (E.m[a] = i[a]);
                     u && u(E)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < o.length; l++) n = o[l], E.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunkamazon_codewhisperer_jupyterlab_ext = self.webpackChunkamazon_codewhisperer_jupyterlab_ext || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
-    var _ = E(6972);
+    var _ = E(8908);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["amazon-codewhisperer-jupyterlab-ext"] = _
 })();
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/utils.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/utils.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext/validator/validator.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext/validator/validator.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-codewhisperer-jupyterlab-ext
-Version: 1.0.3
+Version: 1.0.4
 Summary: Amazon CodeWhisperer for JupyterLab
 Home-page: https://aws.amazon.com/codewhisperer/
 Author: Amazon CodeWhisperer
 Author-email: codewhisperer@amazon.com
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Amazon CodeWhisperer,CodeWhisperer,Code,Whisperer
 Platform: Linux
@@ -93,14 +93,17 @@
 
 * [CodeWhisperer User Guide](https://docs.aws.amazon.com/codewhisperer/latest/userguide/what-is-cwspr.html)
 * [Setting up Amazon CodeWhisperer with JupyterLab](https://docs.aws.amazon.com/codewhisperer/latest/userguide/jupyterlab-setup.html)
 * [Setting up CodeWhisperer with Amazon SageMaker Studio](https://docs.aws.amazon.com/codewhisperer/latest/userguide/sagemaker-setup.html)
 
 ## Change Log
 
+1.0.4
+* Add Glue Studio Notebook support
+
 1.0.3
 * Bug fix: No recommendation when user turn off code suggestions with references in settings.
 * Bug fix: Issue with browser login flow for some Builder ID users.
 * Bug fix: Fix an issue where SageMaker Studio users will incorrectly see the `Share content with Amazon CodeWhisperer` settings option.
 
 1.0.0
 * Initial release
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/amazon_codewhisperer_jupyterlab_ext.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -32,60 +32,98 @@
 amazon_codewhisperer_jupyterlab_ext/client/telemetry/__init__.py
 amazon_codewhisperer_jupyterlab_ext/client/telemetry/telemetry.py
 amazon_codewhisperer_jupyterlab_ext/env/__init__.py
 amazon_codewhisperer_jupyterlab_ext/env/environment.py
 amazon_codewhisperer_jupyterlab_ext/labextension/package.json
 amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/completer.json
 amazon_codewhisperer_jupyterlab_ext/labextension/schemas/amazon-codewhisperer-jupyterlab-ext/package.json.orig
-amazon_codewhisperer_jupyterlab_ext/labextension/static/568.c0e5b626da6cbe06eb5e.js
-amazon_codewhisperer_jupyterlab_ext/labextension/static/568.c0e5b626da6cbe06eb5e.js.LICENSE.txt
+amazon_codewhisperer_jupyterlab_ext/labextension/static/568.5e4ac436f86b65d9e70f.js
+amazon_codewhisperer_jupyterlab_ext/labextension/static/568.5e4ac436f86b65d9e70f.js.LICENSE.txt
 amazon_codewhisperer_jupyterlab_ext/labextension/static/571.3582fd184eff1ff4b836.js
-amazon_codewhisperer_jupyterlab_ext/labextension/static/747.462ff5e5d49d87208721.js
-amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.9bf04351778104e8e5cd.js
+amazon_codewhisperer_jupyterlab_ext/labextension/static/747.4a2fe27171322cd7b67e.js
+amazon_codewhisperer_jupyterlab_ext/labextension/static/remoteEntry.f27b2e72fdec8f3ccdff.js
 amazon_codewhisperer_jupyterlab_ext/labextension/static/style.js
 amazon_codewhisperer_jupyterlab_ext/labextension/static/third-party-licenses.json
 amazon_codewhisperer_jupyterlab_ext/validator/__init__.py
 amazon_codewhisperer_jupyterlab_ext/validator/validator.py
 amazon_codewhisperer_jupyterlab_ext/validator/schemas/generate_recommendations.json
 jupyter-config/amazon_codewhisperer_jupyterlab_ext.json
+src/application.js
+src/application.js.map
 src/application.ts
+src/handler.js
+src/handler.js.map
 src/handler.ts
+src/icons.js
+src/icons.js.map
 src/icons.ts
 src/index.ts
+src/messages.js
+src/messages.js.map
 src/messages.ts
 src/svg.d.ts
 src/__tests__/index.spec.ts
 src/__tests__/autotrigger/autotrigger.spec.ts
+src/__tests__/recommendation/recommendationStateHandler.spec.js
+src/__tests__/recommendation/recommendationStateHandler.spec.js.map
 src/__tests__/recommendation/recommendationStateHandler.spec.ts
 src/auth/authManager.tsx
+src/autotrigger/autotrigger.js
+src/autotrigger/autotrigger.js.map
 src/autotrigger/autotrigger.ts
 src/aws_vector_consolas_jupyter_lab3_extension/__init__.py
 src/aws_vector_consolas_jupyter_lab3_extension/py.typed
+src/client/apiclient.js
+src/client/apiclient.js.map
 src/client/apiclient.ts
 src/client/codewhispererclient.d.ts
 src/client/codewhispereruserclient.d.ts
 src/connector/codewhispererconnector.ts
 src/connector/mergeconnector.ts
+src/inline/inline.js
+src/inline/inline.js.map
 src/inline/inline.ts
 src/keybindings/keybindings.ts
 src/logging/logger.tsx
 src/notifications/notifications.tsx
+src/recommendation/extractor.js
+src/recommendation/extractor.js.map
 src/recommendation/extractor.ts
+src/recommendation/recommendationStateHandler.js
+src/recommendation/recommendationStateHandler.js.map
 src/recommendation/recommendationStateHandler.ts
+src/recommendation/worker.js
+src/recommendation/worker.js.map
 src/recommendation/worker.ts
 src/referencetracker/referencetracker.tsx
 src/statusbar/statusbarwidget.tsx
 src/telemetry/clienttelemetry.d.ts
+src/telemetry/telemetry.gen.js
+src/telemetry/telemetry.gen.js.map
 src/telemetry/telemetry.gen.ts
+src/telemetry/telemetry.js
+src/telemetry/telemetry.js.map
 src/telemetry/telemetry.ts
+src/telemetry/telemetryClient.js
+src/telemetry/telemetryClient.js.map
 src/telemetry/telemetryClient.ts
+src/utils/constants.js
+src/utils/constants.js.map
 src/utils/constants.ts
+src/utils/licenseUtils.js
+src/utils/licenseUtils.js.map
 src/utils/licenseUtils.ts
+src/utils/models.js
+src/utils/models.js.map
 src/utils/models.ts
+src/utils/stateKeys.js
+src/utils/stateKeys.js.map
 src/utils/stateKeys.ts
+src/utils/utils.js
+src/utils/utils.js.map
 src/utils/utils.ts
 style/base.css
 style/index.css
 style/index.js
 style/img/codewhisperer.svg
 style/img/connected.svg
 style/img/disconnected.svg
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/package.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.0.4'"}*

```diff
@@ -130,9 +130,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "1.0.4"
 }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/pyproject.toml` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/setup.py` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/autotrigger/autotrigger.spec.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/__tests__/autotrigger/autotrigger.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/__tests__/recommendation/recommendationStateHandler.spec.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/__tests__/recommendation/recommendationStateHandler.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/application.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/application.ts`

 * *Files 22% similar despite different names*

```diff
@@ -10,43 +10,47 @@
 import { getResponseData } from "./utils/utils";
 import { HttpStatusCode } from "./utils/constants";
 import { NotificationManager } from "./notifications/notifications";
 import {  UPDATE_NOTIFICATION_URL } from "./utils/constants";
 import { message } from "./messages";
 import { IStateDB } from "@jupyterlab/statedb";
 import { JupyterFrontEnd } from "@jupyterlab/application";
+import { ISettingRegistry } from "@jupyterlab/settingregistry";
 
 export class Application {
     private static instance: Application;
     public loadStateSignal: Signal<any, any>;
     private _environment: Environment = undefined;
     public stateDB: IStateDB;
     public jupyterApp: JupyterFrontEnd;
+    public setting: ISettingRegistry.ISettings;
+    public toggleSettingSignal: Signal<any, string>
 
     public static getInstance(): Application {
         if (!Application.instance) {
             Application.instance = new Application()
         }
         return Application.instance;
     }
 
     private constructor() {
         this.loadStateSignal = new Signal(this);
+        this.toggleSettingSignal = new Signal(this);
     }
 
     private async _fetchEnvironment() {
         const getEnvironmentResponse = await requestAPI<Response>('get_environment')
         if (getEnvironmentResponse.status !== HttpStatusCode.OK) return;
         const getEnvironmentResponseJson = await getEnvironmentResponse.json()
         this._environment = getResponseData(getEnvironmentResponseJson)['environment'];
-        const versionNotificaion = getResponseData(getEnvironmentResponseJson)['version_notification'];
+        const versionNotification = getResponseData(getEnvironmentResponseJson)['version_notification'];
         const latestVersion = getResponseData(getEnvironmentResponseJson)['latest_version'];
-        if(versionNotificaion) {
+        if(versionNotification) {
             NotificationManager.getInstance().postNotificationForUpdateInformation(
-                versionNotificaion,
+                versionNotification,
                 latestVersion,
                 message("codewhisperer_update_now"),
                 UPDATE_NOTIFICATION_URL
             ).then();
         }
     }
 
@@ -54,14 +58,18 @@
         return this._environment === Environment.JUPYTER_OSS;
     }
 
     public isSageMakerStudio(): boolean {
         return this._environment === Environment.SM_STUDIO;
     }
 
+    public isGlueStudioNoteBook(): boolean {
+        return this._environment === Environment.GLUE_STUDIO_NOTEBOOK;
+    }
+
     // Initialize all the application singletons here
     public async loadServices(stateDB: IStateDB, jupyterApp: JupyterFrontEnd) {
         this.stateDB = stateDB;
         this.jupyterApp = jupyterApp;
 
         await this._fetchEnvironment()
 
@@ -69,9 +77,10 @@
         AutoTrigger.getInstance();
         AuthManager.getInstance();
     }
 }
 
 enum Environment {
     JUPYTER_OSS = 'Jupyter OSS',
-    SM_STUDIO = 'SageMaker Studio'
+    SM_STUDIO = 'SageMaker Studio',
+    GLUE_STUDIO_NOTEBOOK = 'Glue Studio Notebook'
 }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/auth/authManager.tsx` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/auth/authManager.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         if (authState === AuthState.UNAUTHENTICATED || authState === AuthState.AUTHENTICATION_IN_PROGRESS) return;
 
         // Schedule the next refresh task whenever the current login/refresh succeeds
         setTimeout(this._refreshToken, this._refreshIntervalInMs);
     }
 
     public isAuthenticated(): boolean {
-        return this.authState === AuthState.AUTHENTICATED || Application.getInstance().isSageMakerStudio()
+        return this.authState === AuthState.AUTHENTICATED || !Application.getInstance().isJupyterOSS()
     }
 
     public isAuthenticationInProgress(): boolean {
         return this.authState === AuthState.AUTHENTICATION_IN_PROGRESS
     }
 
     private get authState(): AuthState {
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/autotrigger/autotrigger.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/autotrigger/autotrigger.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/apiclient.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/client/apiclient.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/codewhispererclient.d.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/client/codewhispererclient.d.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/client/codewhispereruserclient.d.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/client/codewhispereruserclient.d.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/connector/codewhispererconnector.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/connector/codewhispererconnector.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/connector/mergeconnector.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/connector/mergeconnector.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/handler.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/icons.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/icons.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/index.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/index.ts`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
           // save clientId to state
           state.save(PLUGIN_ID, { "clientId": Telemetry.clientId });
           logger.debug(`Generated - clientId: ${Telemetry.clientId}`);
         }
       });
 
       const loadSetting = (setting: ISettingRegistry.ISettings) => {
+        Application.getInstance().setting = setting;
         Telemetry.getInstance().enableTelemetry(setting.get(SettingIDs.keyTelemetry).composite as boolean);
         Worker.getInstance().setOptOut(!(setting.get(SettingIDs.keyOptOut).composite as boolean));
         Worker.getInstance().setSuggestionsWithCodeReferences(setting.get(SettingIDs.keyReferences).composite as boolean);
         Logger.setLogLevel(setting.get(SettingIDs.keyLogLevel).composite as string);
         Keybindings.getInstance().keyBindings = [...app.commands.keyBindings];
         logger.debug(`Loaded settings`);
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/inline/inline.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/inline/inline.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/keybindings/keybindings.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/keybindings/keybindings.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/logging/logger.tsx` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/logging/logger.tsx`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/notifications/notifications.tsx` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/notifications/notifications.tsx`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/extractor.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/extractor.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/recommendationStateHandler.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/recommendationStateHandler.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/recommendation/worker.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/recommendation/worker.ts`

 * *Files 2% similar despite different names*

```diff
@@ -243,11 +243,15 @@
         );
     }
 
     public setSuggestionsWithCodeReferences(suggestionsWithCodeReferences : boolean): void {
         this.suggestionsWithCodeReferences = suggestionsWithCodeReferences;
     }
 
+    public isSuggestionsWithCodeReferencesEnabled(): Boolean {
+        return this.suggestionsWithCodeReferences
+    }
+
     public setOptOut(optOut : boolean): void {
         this.optOut = optOut;
     }
 }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/referencetracker/referencetracker.tsx` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/referencetracker/referencetracker.tsx`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/statusbar/statusbarwidget.tsx` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/statusbar/statusbarwidget.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,78 @@
 import { VDomModel, VDomRenderer } from '@jupyterlab/apputils';
-import { interactiveItem, Popup, showPopup } from '@jupyterlab/statusbar';
+import { interactiveItem, Popup, showPopup, GroupItem, TextItem } from '@jupyterlab/statusbar';
 import React from "react";
 import { Menu } from '@lumino/widgets';
 import { CommandRegistry } from '@lumino/commands';
 import { Icons } from '../icons';
 import { message } from "../messages";
 import { h, VirtualElement } from '@lumino/virtualdom';
 import { AuthManager, AuthState } from "../auth/authManager";
 import { AutoTrigger } from "../autotrigger/autotrigger";
 import { Worker } from "../recommendation/worker";
 import { LOG_SOURCE, ReferenceTracker } from '../referencetracker/referencetracker';
 import { Application } from "../application";
 import { Keybindings } from '../keybindings/keybindings';
-import { CommandIDs, MESSAGE_TO_CMD_ID_MAP, CWSPR_DOCUMENTATION } from '../utils/constants';
+import { CommandIDs, MESSAGE_TO_CMD_ID_MAP, CWSPR_DOCUMENTATION, SettingIDs } from '../utils/constants';
 import { AUTO_SUGGESTION } from '../utils/stateKeys';
 import { saveState } from "../utils/utils";
+import { Telemetry } from "../telemetry/telemetry";
 
 // TODO: figure out the right way to use this
 class StatusBarWidgetModel extends VDomModel {
     constructor() {
         super();
     }
 }
 
 class StatusBarWidget extends VDomRenderer<StatusBarWidgetModel> {
     private _popup: Popup | null = null;
+    private _menu: Menu | null = null;
     private _commandsForNotAuthenticated: CommandRegistry = new CommandRegistry();
     private _commandsForAuthenticationInProgress: CommandRegistry = new CommandRegistry();
     private _commandsForAutoSuggestionEnabled: CommandRegistry = new CommandRegistry();
     private _commandsForAutosuggestionDisabled: CommandRegistry = new CommandRegistry();
     private _renderer: Menu.IRenderer = new StatusBarWidgetRenderer();
     private _keyShortcutsInfoRows = 5;
+    private _toggleSettingsforGlueStudioRows = 9;
 
     constructor() {
         super(new StatusBarWidgetModel());
         this.addClass(interactiveItem)
-        this.addClass("jp-Notebook-ExecutionIndicator")
         this.addClass("cwspr-statusbarwidget-parent")
 
         this._initializeCommands()
         AuthManager.getInstance().authStateChangedSignal.connect(this._onAuthStateChanged, this);
         Worker.getInstance().invocationStatusChangedSignal.connect(this._onInvocationStatusChanged, this);
+        Application.getInstance().toggleSettingSignal.connect(this._onToggleSettingButton, this);
     }
 
     private _onAuthStateChanged(sender: any, authState: AuthState) {
         this.update()
     }
 
     private _onInvocationStatusChanged(sender: any, status: boolean) {
         this.update()
     }
 
+    private async _onToggleSettingButton(sender: any, settingId: string) {
+        const setting = Application.getInstance().setting
+        if (settingId == CommandIDs.toggleTelemetry) {
+            const oldValue = setting.get(SettingIDs.keyTelemetry).composite as boolean
+            await setting.set(SettingIDs.keyTelemetry, !oldValue)
+        } else if (settingId == CommandIDs.toggleCodeReferences) {
+            const oldValue = setting.get(SettingIDs.keyReferences).composite as boolean
+            await setting.set(SettingIDs.keyReferences, !oldValue)
+        }
+        if (!this._menu) {
+            return
+        }
+        this._menu.update()
+    }
+
     private _addKeyShortcutsInfo(commands: CommandRegistry) {
         commands.addCommand(CommandIDs.keyShortcutTitle, {
             label: message('codewhisperer_key_shortcut_title'),
             icon: null,
             execute: async () => {},
             isEnabled: () => false,
         })
@@ -155,33 +173,52 @@
             }
         });
         commands.addCommand(CommandIDs.openDocumentation, {
             label: message('codewhisperer_documentation_open'),
             icon: Icons.documentationIcon,
             caption: message('codewhisperer_documentation_open'),
             execute: async () => {
-                window.open(CWSPR_DOCUMENTATION, '_blank');
+                const anchor = document.createElement('a')
+                anchor.setAttribute('href', CWSPR_DOCUMENTATION)
+                anchor.setAttribute('target', '_blank')
+
+                anchor.click();
                 this._handleClick();
             }
         });
 
-        if (Application.getInstance().isSageMakerStudio()) return;
+        if (!Application.getInstance().isJupyterOSS()) return;
 
         commands.addCommand(CommandIDs.signOut, {
             label: message('codewhisperer_sign_out'),
             icon: Icons.signOutIcon,
             caption: message('codewhisperer_sign_out'),
             execute: async () => {
                 this._handleClick();
                 if (!AuthManager.getInstance().isAuthenticated()) return;
                 await AuthManager.getInstance().logout()
             }
         });
     }
 
+    private _addCommandsForAuthenticatedGlueStudio(commands: CommandRegistry) {
+        commands.addCommand(CommandIDs.toggleTelemetry, {
+            label: message('codewhisperer_toggle_telemetry'),
+            icon: null,
+            execute: async () => {},
+            isEnabled: () => false
+        });
+        commands.addCommand(CommandIDs.toggleCodeReferences, {
+            label: message('codewhisperer_toggle_code_references'),
+            icon: null,
+            execute: async () => {},
+            isEnabled: () => false
+        });
+    }
+
     private _initializeCommands() {
         this._addCommandsForUnauthenticated()
         this._addCommandsForAuthenticationInProgress()
 
         this._addKeyShortcutsInfo(this._commandsForAutosuggestionDisabled)
         this._commandsForAutosuggestionDisabled.addCommand(CommandIDs.resumeAutoSuggestion, {
             label: message('codewhisperer_resume_auto_suggestion'),
@@ -190,27 +227,33 @@
             execute: async () => {
                 this._handleClick();
                 AutoTrigger.getInstance().enabled = true;
                 await saveState(AUTO_SUGGESTION, true)
             }
         });
         this._addCommandsForAuthenticatedCommon(this._commandsForAutosuggestionDisabled)
+        if (Application.getInstance().isGlueStudioNoteBook()) {
+            this._addCommandsForAuthenticatedGlueStudio(this._commandsForAutosuggestionDisabled)
+        }
 
         this._addKeyShortcutsInfo(this._commandsForAutoSuggestionEnabled)
         this._commandsForAutoSuggestionEnabled.addCommand(CommandIDs.pauseAutoSuggestion, {
             label: message('codewhisperer_pause_auto_suggestion'),
             icon: Icons.pauseIcon,
             caption: message('codewhisperer_pause_auto_suggestion'),
             execute: async () => {
                 this._handleClick();
                 AutoTrigger.getInstance().enabled = false;
                 await saveState(AUTO_SUGGESTION, false);
             }
         });
         this._addCommandsForAuthenticatedCommon(this._commandsForAutoSuggestionEnabled)
+        if (Application.getInstance().isGlueStudioNoteBook()) {
+            this._addCommandsForAuthenticatedGlueStudio(this._commandsForAutoSuggestionEnabled)
+        }
     }
 
     render(): React.ReactElement {
         const isInvocationInProgress = Worker.getInstance().isGetCompletionsRunning;
         const icon =
             AuthManager.getInstance().isAuthenticated() ?
                 isInvocationInProgress ? (
@@ -221,18 +264,19 @@
             AuthManager.getInstance().isAuthenticationInProgress() ? (
                 <Icons.loadingIcon.react tag="span" className="cwspr-statusbarwidget-icon" />
             ) : (
                 <Icons.disconnectedIcon.react tag="span" className="cwspr-statusbarwidget-icon" />
             );
 
         return (
-            <div className='cwspr-statusbarwidget' onClick={() => this._handleClick()}>
+            <GroupItem spacing={0} onClick={() => this._handleClick()} className='cwspr-statusbarwidget'>
                 {icon}
-                <span>{this._getStatusBarWidgetDisplayText()}</span>
-            </div>
+                <TextItem source={this._getStatusBarWidgetDisplayText()}>
+                </TextItem>
+            </GroupItem>
         );
     }
 
     private _getStatusBarWidgetDisplayText(): string {
         if (AuthManager.getInstance().isAuthenticated()) {
             return message('codewhisperer_status_widget_text_authenticated');
         } else if (AuthManager.getInstance().isAuthenticationInProgress()) {
@@ -248,26 +292,21 @@
     private _handleClick(): void {
         const menu = this._getMenu();
         if (this._popup !== null && !this._popup.isDisposed) {
             this._popup.dispose();
             this._popup = null;
             return;
         }
-        this._menuToggled()
-        menu.aboutToClose.connect(this._menuToggled, this);
 
         this._popup = showPopup({
             body: menu,
             anchor: this,
             align: 'left'
         });
-    }
-
-    private _menuToggled(): void {
-        this.toggleClass('jp-mod-clicked');
+        this._menu = menu
     }
 
     private _getMenu(): Menu {
         const autoTriggerEnabled = AutoTrigger.getInstance().enabled;
         let commands;
 
         if (AuthManager.getInstance().isAuthenticated()) {
@@ -285,14 +324,17 @@
         const menu = new Menu({ commands: commands, renderer: this._renderer });
         menu.addClass('cwspr-statusbarwidget-menu');
 
         this._addCommands(menu, commands);
         if (AuthManager.getInstance().isAuthenticated()) {
             menu.insertItem(this._keyShortcutsInfoRows, { type: 'separator' });
         }
+        if (Application.getInstance().isGlueStudioNoteBook()) {
+            menu.insertItem(this._toggleSettingsforGlueStudioRows, {type: 'separator'})
+        }
 
         menu.update()
         return menu;
     }
 
     private _addCommands(menu: Menu, commands: CommandRegistry) {
         for (let i = 0; i < commands.listCommands().length; i++) {
@@ -305,42 +347,50 @@
 }
 
 class StatusBarWidgetRenderer extends Menu.Renderer {
     renderItem(data: Menu.IRenderData): VirtualElement {
         let className = this.createItemClass(data);
         let dataset = this.createItemDataset(data);
         let aria = this.createItemARIA(data);
+        let itemList = [
+            this.renderIcon(data),
+            this.renderLabel(data),
+            this.renderShortcut(data),
+            this.renderSubmenu(data),
+        ]
+        if (this._isToggleButton(data)) {
+            itemList.push(this._renderSettingToggleButton(data))
+        } else {
+            itemList.push(this._renderCodeWhispererShortCut(data))
+        }
         return h.li(
             {
                 className,
                 dataset,
                 tabindex: '0',
                 onfocus: data.onfocus,
                 ...aria
             },
-            this.renderIcon(data),
-            this.renderLabel(data),
-            this.renderShortcut(data),
-            this.renderSubmenu(data),
-            this._renderCodeWhispererShortCut(data)
+            ...itemList
         );
     }
 
     _renderCodeWhispererShortCut(data: Menu.IRenderData): VirtualElement {
         const keyShortcutButtons = this._getKeyShortcutButtons(data)
         return h.div(
             {
                 className: 'cwspr-key-shortcut-menu'
             },
             ...keyShortcutButtons
         );
     }
 
-    _getKeyShortcutButtons(data: Menu.IRenderData): h.Child[] {
+    private _getKeyShortcutButtons(data: Menu.IRenderData): h.Child[] {
         if (data.item.isEnabled || data.item.label == message('codewhisperer_key_shortcut_title')) return [""]
+
         let children: h.Child[]
         switch (data.item.label) {
             case message("codewhisperer_key_shortcut_accept"):
                 children = Keybindings.getInstance().getKeybinding(MESSAGE_TO_CMD_ID_MAP["codewhisperer_key_shortcut_accept"]);
                 break;
             case message("codewhisperer_key_shortcut_manual_trigger"):
                 children = Keybindings.getInstance().getKeybinding(MESSAGE_TO_CMD_ID_MAP["codewhisperer_key_shortcut_manual_trigger"]);
@@ -353,10 +403,49 @@
                 break;
             default:
                 children = [];
                 break;
         }
         return children.map((text) => h.div({className: 'cwspr-key-shortcut-button'}, text))
     }
+
+    _renderSettingToggleButton(data: Menu.IRenderData): VirtualElement {
+        const toggleButton = this._getToggleButton(data);
+        return h.div(
+            { className: 'cwspr-key-shortcut-menu' },
+            toggleButton
+        );
+    }
+
+    private _getToggleButton(data: Menu.IRenderData): h.Child {
+        if (!this._isToggleButton(data)) {
+            return [""]
+        }
+        const isTelemetryToggle = data.item.label == message('codewhisperer_toggle_telemetry')
+        const isToggledOn = isTelemetryToggle ?
+            (Telemetry.getInstance().isTelemetryEnabled() ? 'true' : 'false') :
+            (Worker.getInstance().isSuggestionsWithCodeReferencesEnabled() ? 'true' : 'false');
+        const settingId = isTelemetryToggle ? CommandIDs.toggleTelemetry : CommandIDs.toggleCodeReferences
+        return h.button(
+            {
+                id: settingId,
+                className: 'jp-switch cwspr-menu-toggle-button',
+                role: 'switch',
+                "aria-checked": isToggledOn,
+                onclick: () => {
+                    Application.getInstance().toggleSettingSignal.emit(settingId)
+                }
+            },
+            h.div(
+                { className: 'jp-switch-track', 'aria-hidden': 'true'},
+                null
+            )
+        )
+    }
+
+    _isToggleButton(data: Menu.IRenderData): boolean {
+        return data.item.label == message('codewhisperer_toggle_telemetry') ||
+            data.item.label == message('codewhisperer_toggle_code_references')
+    }
 }
 
 export default StatusBarWidget;
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/clienttelemetry.d.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/clienttelemetry.d.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetry.gen.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetry.gen.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetry.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetry.ts`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,18 @@
         }, Telemetry.defaultFlushPeriodMillis)
     }
 
     public enableTelemetry(telemetryEnabled: boolean): void {
         this._telemetryEnabled = telemetryEnabled;
     }
 
+    public isTelemetryEnabled(): boolean {
+        return this._telemetryEnabled;
+    }
+
     public closeTimer() {
         if (this._timer !== undefined) {
             clearTimeout(this._timer)
             this._timer = undefined
         }
     }
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/telemetry/telemetryClient.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/telemetry/telemetryClient.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/constants.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/constants.ts`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,18 @@
     export const openReferenceLog = 'codewhisperer:open-reference-log';
     export const signOut = 'codewhisperer:sign-out';
     export const keyShortcutTitle = 'codewhisperer:key-shortcut-title';
     export const keyShortcutAccept = 'codewhisperer:key-shortcut-accept';
     export const keyShortcutManualTrigger = 'codewhisperer:key-shortcut-manual-trigger';
     export const keyShortcutNavigate = 'codewhisperer:key-shortcut-navigate';
     export const keyShortcutReject = 'codewhisperer:key-shortcut-reject';
+
+    export const toggleTelemetry = 'codewhisperer:toggle-telemetry';
+
+    export const toggleCodeReferences = 'codewhisperer:toggle-code-references';
   }
   
   export const PLUGIN_ID = 'amazon-codewhisperer-jupyterlab-ext:completer';
 
 export const MESSAGE_TO_CMD_ID_MAP = {
     "codewhisperer_key_shortcut_accept": CommandIDs.acceptInline,
     "codewhisperer_key_shortcut_manual_trigger": CommandIDs.invokeInline,
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/models.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/models.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/src/utils/utils.ts` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/src/utils/utils.ts`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/base.css` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/style/base.css`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,24 @@
 }
 
 li[data-command^="codewhisperer:key-shortcut-"] .p-Menu-itemIcon {
     width: 0;
     padding-right: 3px;
 }
 
+li[data-command^="codewhisperer:toggle"] .lm-Menu-itemIcon {
+    width: 0;
+    padding-right: 3px;
+}
+
+li[data-command^="codewhisperer:toggle"] .p-Menu-itemIcon {
+    width: 0;
+    padding-right: 3px;
+}
+
 li[data-command^="codewhisperer:"] .lm-Menu-itemLabel {
     padding-right: 0;
 }
 
 li[data-command^="codewhisperer:"] .p-Menu-itemLabel {
     padding-right: 0;
 }
@@ -101,7 +111,17 @@
         transform:rotate(135deg);
     }
     100% {
         stroke-dashoffset: 187;
         transform:rotate(450deg);
     }
 }
+
+.cwspr-menu-toggle-button {
+    vertical-align: middle;
+    display: inline-flex;
+    padding-bottom: 2.5px;
+}
+
+.cwspr-menu-toggle-button:hover {
+    background-color: transparent;
+}
```

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/codewhisperer.svg` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/codewhisperer.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/disconnected.svg` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/disconnected.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/log.svg` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/log.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/signout.svg` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/signout.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/style/img/visual-cue-arrow.svg` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/style/img/visual-cue-arrow.svg`

 * *Files identical despite different names*

### Comparing `amazon-codewhisperer-jupyterlab-ext-1.0.3/tsconfig.json` & `amazon-codewhisperer-jupyterlab-ext-1.0.4/tsconfig.json`

 * *Files identical despite different names*

