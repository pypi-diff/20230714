# Comparing `tmp/resotolib-3.6.0.tar.gz` & `tmp/resotolib-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotolib-3.6.0.tar", last modified: Fri Jun 30 19:22:55 2023, max compression
+gzip compressed data, was "resotolib-3.6.1.tar", last modified: Fri Jul 14 17:03:52 2023, max compression
```

## Comparing `resotolib-3.6.0.tar` & `resotolib-3.6.1.tar`

### file list

```diff
@@ -1,89 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:55.256366 resotolib-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 19:16:54.000000 resotolib-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-30 19:22:55.256366 resotolib-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-30 19:16:54.000000 resotolib-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-30 19:16:54.000000 resotolib-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:55.240366 resotolib-3.6.0/resotolib/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:55.244366 resotolib-3.6.0/resotolib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/asynchronous/periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/asynchronous/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:55.244366 resotolib-3.6.0/resotolib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/asynchronous/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    40114 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:55.244366 resotolib-3.6.0/resotolib/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/durations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:55.244366 resotolib-3.6.0/resotolib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)    26663 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:55.244366 resotolib-3.6.0/resotolib/log/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    23264 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:55.248366 resotolib-3.6.0/resotolib/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:55.252366 resotolib-3.6.0/resotolib/web/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-06-30 19:16:54.000000 resotolib-3.6.0/resotolib/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:55.244366 resotolib-3.6.0/resotolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-30 19:22:55.000000 resotolib-3.6.0/resotolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-30 19:22:55.000000 resotolib-3.6.0/resotolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:22:55.000000 resotolib-3.6.0/resotolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:18:08.000000 resotolib-3.6.0/resotolib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-30 19:22:55.000000 resotolib-3.6.0/resotolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 19:22:55.000000 resotolib-3.6.0/resotolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 19:22:55.256366 resotolib-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:55.256366 resotolib-3.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-30 19:16:54.000000 resotolib-3.6.0/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:52.501672 resotolib-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 16:57:37.000000 resotolib-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-14 17:03:52.501672 resotolib-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-14 16:57:37.000000 resotolib-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-14 16:57:37.000000 resotolib-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:52.489672 resotolib-3.6.1/resotolib/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:52.489672 resotolib-3.6.1/resotolib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/asynchronous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:52.489672 resotolib-3.6.1/resotolib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/asynchronous/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40237 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:52.489672 resotolib-3.6.1/resotolib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:52.493672 resotolib-3.6.1/resotolib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    27774 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:52.493672 resotolib-3.6.1/resotolib/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:52.493672 resotolib-3.6.1/resotolib/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:52.497672 resotolib-3.6.1/resotolib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-14 16:57:37.000000 resotolib-3.6.1/resotolib/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:52.489672 resotolib-3.6.1/resotolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-14 17:03:52.000000 resotolib-3.6.1/resotolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-14 17:03:52.000000 resotolib-3.6.1/resotolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:03:52.000000 resotolib-3.6.1/resotolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:58:52.000000 resotolib-3.6.1/resotolib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-14 17:03:52.000000 resotolib-3.6.1/resotolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 17:03:52.000000 resotolib-3.6.1/resotolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 17:03:52.501672 resotolib-3.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:52.501672 resotolib-3.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16198 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-14 16:57:37.000000 resotolib-3.6.1/test/test_x509.py
```

### Comparing `resotolib-3.6.0/PKG-INFO` & `resotolib-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto common library.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotolib
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotolib-3.6.0/README.md` & `resotolib-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/pyproject.toml` & `resotolib-3.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotolib"
-version = "3.6.0"
+version = "3.6.1"
 authors = [{name="Some Engineering Inc."}]
 description = "Resoto common library."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -32,14 +32,15 @@
     "Pint",
     "PyJWT",
     "PyYAML",
     "aiohttp[speedups]",
     "attrs",
     "cattrs",
     "cryptography",
+    "frozendict",
     "jsons",
     "networkx",
     "parsy",
     "prometheus-client",
     "psutil",
     "python-dateutil",
     "requests",
```

### Comparing `resotolib-3.6.0/resotolib/args.py` & `resotolib-3.6.1/resotolib/args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/asynchronous/utils.py` & `resotolib-3.6.1/resotolib/asynchronous/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/asynchronous/web/auth.py` & `resotolib-3.6.1/resotolib/asynchronous/web/auth.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/asynchronous/web/runner.py` & `resotolib-3.6.1/resotolib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/asynchronous/web/ws_handler.py` & `resotolib-3.6.1/resotolib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/baseplugin.py` & `resotolib-3.6.1/resotolib/baseplugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import time
 from abc import ABC, abstractmethod
 from enum import Enum, auto
 from threading import Thread, current_thread
-from typing import Dict, Optional, Set, Any
+from typing import Dict, Optional, Any
+from queue import Queue
 
 from prometheus_client import Counter
 
 import resotolib.config
 import resotolib.proc
 from resotolib.args import ArgumentParser
 from resotolib.baseresources import BaseResource, Cloud
 from resotolib.config import Config
 from resotolib.core import resotocore
 from resotolib.core.actions import CoreActions
 from resotolib.core.ca import TLSData
-from resotolib.graph import Graph
+from resotolib.graph import Graph, GraphMergeKind
 from resotolib.logger import log
 from resotolib.types import Json
 
-# from multiprocessing import Process
 
 metrics_unhandled_plugin_exceptions = Counter(
     "resoto_unhandled_plugin_exceptions_total",
     "Unhandled plugin exceptions",
     ["plugin"],
 )
 
@@ -35,15 +35,14 @@
     PERSISTENT is a persistent plugin that gets instantiated once upon startup
     """
 
     COLLECTOR = auto()
     ACTION = auto()
     PERSISTENT = auto()
     CLI = auto()
-    POST_COLLECT = auto()
 
 
 class BasePlugin(ABC, Thread):
     """A resoto Plugin is a thread that does some work.
 
     If the plugin_type is PluginType.COLLECTOR the Plugin gets instantiated each
     collect run.
@@ -199,20 +198,28 @@
     When the collect() method finishes, the Collector will retrieve the
     Plugins Graph and append it to the global Graph.
     """
 
     plugin_type = PluginType.COLLECTOR  # Type of the Plugin
     cloud: str = NotImplemented  # Name of the cloud this plugin implements
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+        graph_queue: Optional[Queue[Optional[Graph]]] = None,
+        graph_merge_kind: GraphMergeKind = GraphMergeKind.cloud,
+        task_data: Optional[Json] = None,
+    ) -> None:
         super().__init__()
         self.name = str(self.cloud)
         cloud = Cloud(id=self.cloud)
         self.root = cloud
-        self.graph = Graph(root=self.root)
+        self._graph_queue: Optional[Queue[Optional[Graph]]] = graph_queue
+        self.graph_merge_kind: GraphMergeKind = graph_merge_kind
+        self.graph = self.new_graph()
+        self.task_data = task_data
 
     @abstractmethod
     def collect(self) -> None:
         """Collects all the Cloud Resources"""
         pass
 
     @staticmethod
@@ -236,39 +243,40 @@
 
     @staticmethod
     def cleanup(config: Config, resource: BaseResource, graph: Graph) -> bool:
         return resource.cleanup(graph)
 
     def go(self) -> None:
         self.collect()
+        if self.graph_merge_kind == GraphMergeKind.cloud or len(self.graph) > 1:
+            if self.graph_merge_kind == GraphMergeKind.account:
+                log.debug("Using backwards compatibility mode")
+            assert isinstance(self.graph.root, BaseResource)
+            log.debug(f"Sending graph of {self.graph.root.kdname} to queue")
+            self.send_graph(self.graph)
+
+    def new_graph(self) -> Graph:
+        return Graph(root=self.root)
+
+    def send_account_graph(self, graph: Graph) -> None:
+        if not isinstance(graph, Graph):
+            log.error(f"Expected Graph, got {type(graph)}")
+            return
+
+        if self.graph_merge_kind == GraphMergeKind.account:
+            assert isinstance(graph.root, BaseResource)
+            kdname = graph.root.kdname
+            cloud_graph = self.new_graph()
+            cloud_graph.merge(graph, skip_deferred_edges=True)
+            log.debug(f"Sending graph of {kdname} to queue")
+            self.send_graph(cloud_graph)
+        elif self.graph_merge_kind == GraphMergeKind.cloud:
+            self.graph.merge(graph, skip_deferred_edges=True)
+        else:
+            raise ValueError(f"Unknown graph merge kind {self.graph_merge_kind}")
 
-
-class BasePostCollectPlugin(ABC):
-    """A resoto Post Collect plugin is a thread that runs after collection is done.
-
-    Whenever the thread is started the post_collect() method is run. The post_collect() method
-    is expected take the graph and perform operations on it, e.g. add the external edges or
-    enritch the graph in some other way.
-    """
-
-    plugin_type = PluginType.POST_COLLECT  # Type of the Plugin
-    name: str = NotImplemented  # Name of the cloud this plugin implements
-    activate_with: Set[str]  # List of clouds this plugin should be activated on
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.name = self.name
-
-    @abstractmethod
-    def post_collect(self, graph: Graph) -> None:
-        """Process the collected graph"""
-        pass
-
-    @staticmethod
-    def add_args(arg_parser: ArgumentParser) -> None:
-        """Adds Plugin specific arguments to the global arg parser"""
-        pass
-
-    @staticmethod
-    def add_config(config: Config) -> None:
-        """Adds Plugin specific config options"""
-        pass
+    def send_graph(self, graph: Graph) -> None:
+        if self._graph_queue is None:
+            raise RuntimeError("Unable to send graph - no graph queue set")
+        if not isinstance(graph, Graph):
+            raise TypeError(f"Unable to send graph - expected type Graph, got {type(graph)}")
+        self._graph_queue.put(graph)
```

### Comparing `resotolib-3.6.0/resotolib/baseresources.py` & `resotolib-3.6.1/resotolib/baseresources.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import weakref
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from datetime import datetime, timezone, timedelta
 from enum import Enum, unique
 from functools import wraps, cached_property
 from typing import Dict, Iterator, List, ClassVar, Optional, TypedDict, Any, TypeVar, Type, Callable, Set, Tuple
+from collections import defaultdict
 
 from attr import resolve_types
 from attrs import define, field, Factory
 from prometheus_client import Counter, Summary
 
 from resotolib.json import from_json as _from_json, to_json as _to_json
 from resotolib.logger import log
@@ -109,14 +110,18 @@
         if len(self.node.event_log) > 0:
             if "metadata" not in changes:
                 changes[section] = {}
             changes["metadata"]["event_log"] = self.node.str_event_log
         return changes
 
 
+MetricName = str
+StatName = str
+
+
 @define(eq=False, slots=False, kw_only=True)
 class BaseResource(ABC):
     """A BaseResource is any node we're connecting to the Graph()
 
     BaseResources have an id, name and tags. The id is a unique id used to search for
     the resource within the Graph. The name is used for display purposes. Tags are
     key/value pairs that get exported in the GRAPHML view.
@@ -147,15 +152,15 @@
     _resotocore_id: Optional[str] = field(default=None, repr=False)
     _resotocore_revision: Optional[str] = field(default=None, repr=False)
     _resotocore_query_tag: Optional[str] = field(default=None, repr=False)
     _clean: bool = False
     _cleaned: bool = False
     _protected: bool = False
     _deferred_connections: List[Dict[str, Any]] = field(factory=list)
-    _metrics: Dict[str, Any] = field(factory=dict)
+    _resource_usage: Dict[MetricName, Dict[StatName, float]] = field(factory=lambda: defaultdict(dict))
 
     ctime: Optional[datetime] = field(
         default=None,
         metadata={"synthetic": {"age": "trafo.duration_to_datetime"}},
     )
     mtime: Optional[datetime] = field(
         default=None,
```

### Comparing `resotolib-3.6.0/resotolib/config.py` & `resotolib-3.6.1/resotolib/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/core/__init__.py` & `resotolib-3.6.1/resotolib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/core/actions.py` & `resotolib-3.6.1/resotolib/core/actions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/core/ca.py` & `resotolib-3.6.1/resotolib/core/ca.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/core/config.py` & `resotolib-3.6.1/resotolib/core/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/core/custom_command.py` & `resotolib-3.6.1/resotolib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/core/events.py` & `resotolib-3.6.1/resotolib/core/events.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/core/model_check.py` & `resotolib-3.6.1/resotolib/core/model_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
-from attrs import define
 from typing import List, Dict, Tuple, Type, Optional, Any
 
+from attrs import define
+
 from resotolib.baseresources import BaseResource
-from resotolib.core.model_export import dataclasses_to_resotocore_model
+from resotolib.graph import resource_classes_to_resotocore_model
 from resotolib.json import from_json
 from resotolib.types import Json
 
 
 @define
 class CheckProp:
     name: str
@@ -132,8 +133,8 @@
         *dynamic_import("resoto_plugin_random.resources.RandomResource"),
         *dynamic_import("resoto_plugin_scarf.resources.ScarfResource"),
         *dynamic_import("resoto_plugin_slack.resources.SlackResource"),
         *dynamic_import("resoto_plugin_vsphere.resources.VSphereResource"),
         *base,
     }
     # check overlap for all plugin classes
-    check_overlap_for(dataclasses_to_resotocore_model(model_classes, aggregate_root=BaseResource))
+    check_overlap_for(resource_classes_to_resotocore_model(model_classes, aggregate_root=BaseResource))
```

### Comparing `resotolib-3.6.0/resotolib/core/model_export.py` & `resotolib-3.6.1/resotolib/core/model_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,25 +272,29 @@
         else:
             raise AttributeError(f"Don't know how to handle: {cls}")
     return model
 
 
 # Use this model exporter, if a dynamic object is exported
 # with given name and properties.
-def dynamic_object_to_resotocore_model(name: str, properties: Dict[str, type]) -> List[Json]:
-    dependant = dataclasses_to_resotocore_model(set(properties.values()))
+def dynamic_object_to_resotocore_model(
+    name: str, properties: Dict[str, type], aggregate_root: bool = True, traverse_dependant: bool = True
+) -> List[Json]:
+    dependant = dataclasses_to_resotocore_model(set(properties.values())) if traverse_dependant else []
     # append definition for top level object
     dependant.append(
         {
             "fqn": name,
             "bases": [],
+            "aggregate_root": aggregate_root,
             "properties": [
                 {"name": prop_name, "kind": model_name(prop_type), "required": False}
                 for prop_name, prop_type in properties.items()
             ],
+            "metadata": {"dynamic": True},
         }
     )
     return dependant
 
 
 def get_node_attributes(node: BaseResource) -> Json:
     if not hasattr(node, "to_json"):
@@ -310,15 +314,15 @@
                 "reported": get_node_attributes(node),
                 "metadata": {
                     "python_type": type_str(node),
                     "cleaned": node.cleaned,
                     "phantom": node.phantom,
                     "protected": node.protected,
                 },
-                "metrics": node._metrics,
+                "usage": node._resource_usage,
             }
         )
         if node.clean:
             node_dict.update(
                 {
                     "desired": {
                         "clean": node.clean,
```

### Comparing `resotolib-3.6.0/resotolib/core/progress.py` & `resotolib-3.6.1/resotolib/core/progress.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/core/search.py` & `resotolib-3.6.1/resotolib/core/search.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/core/tasks.py` & `resotolib-3.6.1/resotolib/core/tasks.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/durations.py` & `resotolib-3.6.1/resotolib/durations.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,12 +81,12 @@
             if seconds >= factor:
                 found = True
                 num = int(seconds / factor)
                 seconds = seconds - (num * factor)
                 result += f"{num}{unit}"
             if found:
                 count += 1
-            if precision and count >= precision or unit == down_to_unit:
+            if (precision and count >= precision) or unit == down_to_unit or (down_to_unit is None and seconds < 1):
                 break
 
     # in case the duration is less than one second
     return result if result else ("0s" if down_to_unit is None else f"0{down_to_unit}")
```

### Comparing `resotolib-3.6.0/resotolib/event.py` & `resotolib-3.6.1/resotolib/event.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/graph/__init__.py` & `resotolib-3.6.1/resotolib/graph/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tempfile
 import threading
 from collections import defaultdict, namedtuple, deque
 from datetime import datetime
 from enum import Enum
 from functools import lru_cache
 from time import time
-from typing import Dict, Iterator, List, Tuple, Optional, Union, Any, Type, TypeVar
+from typing import Dict, Iterator, List, Tuple, Optional, Union, Any, Type, TypeVar, Set
 
 import networkx
 from attr import resolve_types
 from attrs import define, fields
 from networkx.algorithms.dag import is_directed_acyclic_graph
 from prometheus_client import Summary
 from typeguard import check_type
@@ -21,18 +21,23 @@
 from resotolib.baseresources import (
     BaseCloud,
     BaseAccount,
     GraphRoot,
     Cloud,
     BaseResource,
     EdgeType,
+    BaseRegion,
+    BaseZone,
+    MetricName,
+    StatName,
 )
 from resotolib.core.model_export import (
-    dataclasses_to_resotocore_model,
     node_to_dict,
+    dataclasses_to_resotocore_model,
+    dynamic_object_to_resotocore_model,
 )
 from resotolib.json import to_json_str
 from resotolib.logger import log
 from resotolib.types import Json
 from resotolib.utils import get_resource_attributes, unset_cached_properties, utc_str
 
 T = TypeVar("T")
@@ -352,37 +357,61 @@
     def resolve_deferred_connections(self) -> None:
         log.debug("Resolving deferred graph connections")
         for node in self.nodes:
             if isinstance(node, BaseResource):
                 node.resolve_deferred_connections(self)
 
     def export_model(self, **kwargs: Any) -> List[Json]:
-        """Return the graph node dataclass model in resotocore format"""
-        classes = set()
-        for node in self.nodes:
-            classes.add(type(node))
-        model = dataclasses_to_resotocore_model(classes, aggregate_root=BaseResource, **kwargs)
-
-        # fixme: workaround to report kind
-        for resource_model in model:
-            if resource_model.get("fqn") == "resource":
-                resource_model.get("properties", []).append(
-                    {
-                        "name": "kind",
-                        "kind": "string",
-                        "required": True,
-                        "description": "",
-                    }
-                )
-        return model
+        return export_model(graph=self, **kwargs)
 
     def export_iterator(self) -> GraphExportIterator:
         return GraphExportIterator(self)
 
 
+def resource_classes_to_resotocore_model(classes: Set[Type[Any]], **kwargs: Any) -> List[Json]:
+    model = {c["fqn"]: c for c in dataclasses_to_resotocore_model(classes, **kwargs)}
+    # create a phantom resource which defines default property paths
+    dynamic_types: Dict[str, Dict[str, Type[Any]]] = {
+        "resource_short_property_access": {
+            "cloud": Union[Cloud, str],  # type: ignore
+            "account": Union[BaseAccount, str],  # type: ignore
+            "region": Union[BaseRegion, str],  # type: ignore
+            "zone": Union[BaseZone, str],  # type: ignore
+            "usage": Dict[MetricName, Dict[StatName, float]],
+        }
+    }
+    for name, dynamic in dynamic_types.items():
+        for dyn in dynamic_object_to_resotocore_model(name, dynamic, aggregate_root=True, traverse_dependant=False):
+            model[dyn["fqn"]] = dyn
+    return list(model.values())
+
+
+def export_model(graph: Optional[Graph] = None, **kwargs: Any) -> List[Json]:
+    """Return the graph node dataclass model in resotocore format"""
+    classes = set()
+    if graph is None:
+        classes.add(BaseResource)
+    else:
+        for node in graph.nodes:
+            classes.add(type(node))
+
+    model = resource_classes_to_resotocore_model(classes, aggregate_root=BaseResource, **kwargs)
+    for resource_model in model:
+        if resource_model.get("fqn") == "resource":
+            resource_model.get("properties", []).append(
+                {
+                    "name": "kind",
+                    "kind": "string",
+                    "required": True,
+                    "description": "",
+                }
+            )
+    return model
+
+
 @lru_cache(maxsize=4096)  # Only resolve types once per type
 def resolve_type(clazz: Type[Any]) -> None:
     resolve_types(clazz)  # type: ignore
 
 
 def validate_dataclass(node: BaseResource) -> None:
     resolve_type(type(node))  # make sure all type annotations are resolved
```

### Comparing `resotolib-3.6.0/resotolib/graph/graph_extensions.py` & `resotolib-3.6.1/resotolib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/json.py` & `resotolib-3.6.1/resotolib/json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/json_bender.py` & `resotolib-3.6.1/resotolib/json_bender.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/jwt.py` & `resotolib-3.6.1/resotolib/jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/lock.py` & `resotolib-3.6.1/resotolib/lock.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/logger.py` & `resotolib-3.6.1/resotolib/logger.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/parse_util.py` & `resotolib-3.6.1/resotolib/parse_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
+from datetime import datetime, timezone
 from typing import Callable
 
 import parsy
 from parsy import Parser, generate, regex, string
+from dateutil.parser import parse as parse_iso_8601
 
 
 def make_direct_parser(fn: Callable[[str, int], parsy.Result]) -> Parser:
     """
     Make typed parser (required for mypy).
     """
     return Parser(fn)
@@ -69,14 +71,36 @@
 optional_slash = slash.at_most(1).concat()
 variable_dp = optional_slash + variable_dp_array_part + (dot_dp + variable_dp_array_part).many().map("".join)
 variable_no_array_dp = optional_slash + (variable_dp_part + variable_dp_part_plain).at_least(1).map("".join)
 
 
 unquoted_allowed_characters = re.compile("[A-Za-z0-9_\\-:/.]")
 unquoted_end_of_unquoted_str = re.compile("[,\\[\\])(}{\\s]")
+iso_date_re = re.compile("[0-9]{4}-?[0-9]{2}-?[0-9]{2}T?[0-9]{2}:?[0-9]{2}:?[0-9]{2}\\.?[0-9]*(Z|[+-]\\d{2}:?\\d{2})?")
+
+
+@make_direct_parser
+def iso_date_time_utc_parser(stream: str, index: int) -> parsy.Result:
+    try:
+        if match := iso_date_re.match(stream, index):
+            ds = match.group()
+            try:
+                dt = datetime.fromisoformat(ds)
+            except Exception:
+                dt = parse_iso_8601(ds)
+            if dt.tzinfo is None:
+                dt = dt.replace(tzinfo=timezone.utc)
+            else:
+                offset = dt.tzinfo.utcoffset(None)
+                if offset is not None and offset.total_seconds() > 0:
+                    dt = dt.astimezone(timezone.utc)
+            return parsy.Result.success(index + len(ds), dt)
+    except Exception:
+        pass
+    return parsy.Result.failure(index, "No valid ISO 8601 date time")
 
 
 def unquoted_string_parser(*stop_words: str) -> Parser:
     @make_direct_parser
     def unquoted_string_direct_parser(stream: str, index: int) -> parsy.Result:
         # read from index until -> end_of_unquoted_str
         # all characters in between have to be allowed characters
```

### Comparing `resotolib-3.6.0/resotolib/proc.py` & `resotolib-3.6.1/resotolib/proc.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,22 @@
 
 
 def initializer() -> None:
     signal(SIGINT, handler)
     signal(SIGTERM, handler)
 
 
+def collector_initializer(nice_level: int = 5) -> None:
+    initializer()
+    try:
+        os.nice(nice_level)
+    except Exception:
+        pass
+
+
 def set_thread_name(thread_name: str = "resoto") -> None:
     threading.current_thread().name = thread_name
 
 
 def emergency_shutdown(reason: str = "") -> None:
     log.fatal(f"EMERGENCY SHUTDOWN: {reason}")
     for p in psutil.Process().children(recursive=True):
```

### Comparing `resotolib-3.6.0/resotolib/tree.py` & `resotolib-3.6.1/resotolib/tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/utils.py` & `resotolib-3.6.1/resotolib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,31 @@
 import time
 from argparse import ArgumentParser
 from contextlib import closing
 from copy import deepcopy
 from datetime import date, datetime, timezone, timedelta
 from functools import wraps, cached_property
 from tarfile import TarFile, TarInfo
-from typing import Dict, List, Tuple, Optional, NoReturn, Any, Mapping, Union, Callable, cast, Iterator, TypeVar
+from typing import (
+    Dict,
+    List,
+    Tuple,
+    Optional,
+    NoReturn,
+    Any,
+    Mapping,
+    Union,
+    Callable,
+    cast,
+    Iterator,
+    TypeVar,
+    Sequence,
+)
 from zoneinfo import ZoneInfo
+from frozendict import frozendict
 
 import pkg_resources
 import requests
 from tzlocal import get_localzone_name
 
 from resotolib.logger import log
 from resotolib.types import DecoratedFn, JsonElement
@@ -624,7 +639,24 @@
         return tcp.getsockname()[1]  # type: ignore
 
 
 def stdin_generator() -> Iterator[str]:
     if select.select([sys.stdin], [], [], 0.0)[0]:
         for line in iter(sys.stdin.readline, ""):
             yield line.rstrip("\r\n")
+
+
+# makes things hashable
+def freeze(elem: JsonElement) -> Any:
+    # check if can be hashed first
+    try:
+        hash(elem)
+        return elem
+    except TypeError:
+        pass
+
+    if isinstance(elem, Sequence):
+        return tuple([freeze(v) for v in elem])
+    elif isinstance(elem, Mapping):
+        return frozendict({k: freeze(v) for k, v in elem.items()})
+    else:
+        return elem
```

### Comparing `resotolib-3.6.0/resotolib/web/__init__.py` & `resotolib-3.6.1/resotolib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/web/metrics.py` & `resotolib-3.6.1/resotolib/web/metrics.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/web/static/android-chrome-192x192.png` & `resotolib-3.6.1/resotolib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/web/static/android-chrome-512x512.png` & `resotolib-3.6.1/resotolib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/web/static/apple-touch-icon.png` & `resotolib-3.6.1/resotolib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/web/static/favicon-16x16.png` & `resotolib-3.6.1/resotolib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/web/static/favicon-32x32.png` & `resotolib-3.6.1/resotolib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/web/static/index.html` & `resotolib-3.6.1/resotolib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/web/static/mstile-150x150.png` & `resotolib-3.6.1/resotolib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/web/static/picnic.min.css` & `resotolib-3.6.1/resotolib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib/x509.py` & `resotolib-3.6.1/resotolib/x509.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/resotolib.egg-info/PKG-INFO` & `resotolib-3.6.1/resotolib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto common library.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotolib
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotolib-3.6.0/resotolib.egg-info/SOURCES.txt` & `resotolib-3.6.1/resotolib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 resotolib.egg-info/PKG-INFO
 resotolib.egg-info/SOURCES.txt
 resotolib.egg-info/dependency_links.txt
 resotolib.egg-info/not-zip-safe
 resotolib.egg-info/requires.txt
 resotolib.egg-info/top_level.txt
 resotolib/asynchronous/__init__.py
-resotolib/asynchronous/periodic.py
 resotolib/asynchronous/utils.py
 resotolib/asynchronous/web/__init__.py
 resotolib/asynchronous/web/auth.py
 resotolib/asynchronous/web/runner.py
 resotolib/asynchronous/web/ws_handler.py
 resotolib/core/__init__.py
 resotolib/core/actions.py
```

### Comparing `resotolib-3.6.0/test/test_args.py` & `resotolib-3.6.1/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/test/test_baseresources.py` & `resotolib-3.6.1/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/test/test_config.py` & `resotolib-3.6.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/test/test_graph.py` & `resotolib-3.6.1/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/test/test_graph_extensions.py` & `resotolib-3.6.1/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/test/test_json.py` & `resotolib-3.6.1/test/test_json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/test/test_jwt.py` & `resotolib-3.6.1/test/test_jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/test/test_plugin.py` & `resotolib-3.6.1/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/test/test_tree.py` & `resotolib-3.6.1/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/test/test_utils.py` & `resotolib-3.6.1/test/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,23 +15,25 @@
     sha256sum,
     rrdata_as_dict,
     get_local_tzinfo,
     utc_str,
     replace_env_vars,
     merge_json_elements,
     drop_deleted_attributes,
+    freeze,
 )
 from resotolib.baseresources import BaseResource
 from resotolib.utils import stdin_generator
 from attrs import define
 from typing import ClassVar
 import pytest
 import sys
 import tempfile
 from contextlib import contextmanager
+from frozendict import frozendict
 
 
 class Writer(threading.Thread):
     def __init__(self, buffer_, rw_lock, init_sleep_time, sleep_time, to_write):
         """
         @param buffer_: common buffer_ shared by the readers and writers
         @type buffer_: list
@@ -458,7 +460,21 @@
         ("", []),
     ],
 )
 def test_sync_stdin_generator(input_data, expected_output):
     with replace_stdin(input_data):
         output = list(stdin_generator())
     assert output == expected_output
+
+
+def test_freeze():
+    tpl = (1, 2, 3)
+    # hashable things are not touched
+    assert id(tpl) == id(freeze(tpl))
+    # dict to frozendict
+    flat_dict = {"foo": "bar"}
+    assert freeze(flat_dict) == frozendict(flat_dict)
+    # nested too
+    nested_dict = {"foo": flat_dict}
+    assert freeze(nested_dict) == frozendict({"foo": frozendict(flat_dict)})
+    # and a list to tupple
+    assert freeze([1, 2]) == (1, 2)
```

### Comparing `resotolib-3.6.0/test/test_web.py` & `resotolib-3.6.1/test/test_web.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.0/test/test_x509.py` & `resotolib-3.6.1/test/test_x509.py`

 * *Files identical despite different names*

