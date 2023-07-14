# Comparing `tmp/autumn8-2.0.0rc1.tar.gz` & `tmp/autumn8-2.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-2.0.0rc1.tar", last modified: Thu Jun 22 11:01:51 2023, max compression
+gzip compressed data, was "autumn8-2.0.1rc1.tar", last modified: Fri Jul 14 17:25:23 2023, max compression
```

## Comparing `autumn8-2.0.0rc1.tar` & `autumn8-2.0.1rc1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.427145 autumn8-2.0.0rc1/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-06-22 11:01:51.417145 autumn8-2.0.0rc1/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.407145 autumn8-2.0.0rc1/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-2.0.0rc1/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.407145 autumn8-2.0.0rc1/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-2.0.0rc1/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-2.0.0rc1/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     8030 2023-06-21 15:47:37.000000 autumn8-2.0.0rc1/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.407145 autumn8-2.0.0rc1/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12773 2023-06-21 15:47:37.000000 autumn8-2.0.0rc1/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17489 2023-06-21 15:47:37.000000 autumn8-2.0.0rc1/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-2.0.0rc1/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5170 2023-06-12 13:36:42.000000 autumn8-2.0.0rc1/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.417145 autumn8-2.0.0rc1/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-06-22 11:00:55.000000 autumn8-2.0.0rc1/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.417145 autumn8-2.0.0rc1/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7161 2023-06-13 13:38:00.000000 autumn8-2.0.0rc1/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-2.0.0rc1/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-24 15:09:02.000000 autumn8-2.0.0rc1/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.417145 autumn8-2.0.0rc1/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-2.0.0rc1/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-2.0.0rc1/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-2.0.0rc1/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-2.0.0rc1/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-2.0.0rc1/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.417145 autumn8-2.0.0rc1/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-2.0.0rc1/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-2.0.0rc1/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/autumn8/examples/tensorflow_custom_layers.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      108 2023-06-12 13:36:42.000000 autumn8-2.0.0rc1/autumn8/exceptions.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       71 2023-06-21 15:47:37.000000 autumn8-2.0.0rc1/autumn8/i18n.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.417145 autumn8-2.0.0rc1/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.417145 autumn8-2.0.0rc1/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4067 2023-06-12 13:36:42.000000 autumn8-2.0.0rc1/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12004 2023-06-12 13:36:42.000000 autumn8-2.0.0rc1/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/autumn8/lib/api/user.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1595 2023-06-12 13:36:42.000000 autumn8-2.0.0rc1/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-2.0.0rc1/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3537 2023-06-22 11:00:44.000000 autumn8-2.0.0rc1/autumn8/lib/service.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       69 2023-06-13 13:38:00.000000 autumn8-2.0.0rc1/autumn8/libenv.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.417145 autumn8-2.0.0rc1/autumn8/types/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1924 2023-06-21 13:43:24.000000 autumn8-2.0.0rc1/autumn8/types/deployment.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      502 2023-06-21 15:47:37.000000 autumn8-2.0.0rc1/autumn8/types/router.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.407145 autumn8-2.0.0rc1/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-06-22 11:01:51.000000 autumn8-2.0.0rc1/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1544 2023-06-22 11:01:51.000000 autumn8-2.0.0rc1/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-06-22 11:01:51.000000 autumn8-2.0.0rc1/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-06-22 11:01:51.000000 autumn8-2.0.0rc1/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-06-22 11:01:51.000000 autumn8-2.0.0rc1/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-06-22 11:01:51.000000 autumn8-2.0.0rc1/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-06-22 11:01:51.427145 autumn8-2.0.0rc1/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-22 11:01:51.417145 autumn8-2.0.0rc1/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-06-06 16:39:42.000000 autumn8-2.0.0rc1/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-2.0.0rc1/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.449715 autumn8-2.0.1rc1/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-07-14 17:25:23.449715 autumn8-2.0.1rc1/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.429714 autumn8-2.0.1rc1/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-2.0.1rc1/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.439715 autumn8-2.0.1rc1/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-2.0.1rc1/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-2.0.1rc1/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     8030 2023-07-13 18:40:03.000000 autumn8-2.0.1rc1/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.439715 autumn8-2.0.1rc1/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12773 2023-07-13 18:40:03.000000 autumn8-2.0.1rc1/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17489 2023-07-13 18:40:03.000000 autumn8-2.0.1rc1/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5170 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.439715 autumn8-2.0.1rc1/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-07-14 17:24:37.000000 autumn8-2.0.1rc1/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.439715 autumn8-2.0.1rc1/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7161 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.439715 autumn8-2.0.1rc1/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-2.0.1rc1/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-2.0.1rc1/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-2.0.1rc1/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-2.0.1rc1/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-2.0.1rc1/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.449715 autumn8-2.0.1rc1/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-2.0.1rc1/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/examples/tensorflow_custom_layers.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      108 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/exceptions.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       71 2023-07-13 18:40:03.000000 autumn8-2.0.1rc1/autumn8/i18n.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.449715 autumn8-2.0.1rc1/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.449715 autumn8-2.0.1rc1/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4067 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12022 2023-07-14 17:13:43.000000 autumn8-2.0.1rc1/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/lib/api/user.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1595 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3537 2023-07-14 16:30:50.000000 autumn8-2.0.1rc1/autumn8/lib/service.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       69 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/autumn8/libenv.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.449715 autumn8-2.0.1rc1/autumn8/types/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1995 2023-07-14 16:30:50.000000 autumn8-2.0.1rc1/autumn8/types/deployment.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      502 2023-07-13 18:40:03.000000 autumn8-2.0.1rc1/autumn8/types/router.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.439715 autumn8-2.0.1rc1/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-07-14 17:25:23.000000 autumn8-2.0.1rc1/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1544 2023-07-14 17:25:23.000000 autumn8-2.0.1rc1/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-07-14 17:25:23.000000 autumn8-2.0.1rc1/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-07-14 17:25:23.000000 autumn8-2.0.1rc1/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-07-14 17:25:23.000000 autumn8-2.0.1rc1/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-07-14 17:25:23.000000 autumn8-2.0.1rc1/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-07-14 17:25:23.449715 autumn8-2.0.1rc1/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-07-14 17:25:23.449715 autumn8-2.0.1rc1/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-07-05 15:39:16.000000 autumn8-2.0.1rc1/tests/test_settings.py
```

### Comparing `autumn8-2.0.0rc1/PKG-INFO` & `autumn8-2.0.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 2.0.0rc1
+Version: 2.0.1rc1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-2.0.0rc1/README.md` & `autumn8-2.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/cli/analyze.py` & `autumn8-2.0.1rc1/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/cli/cli_environment.py` & `autumn8-2.0.1rc1/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/cli/commands/cloud.py` & `autumn8-2.0.1rc1/autumn8/cli/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/cli/commands/models.py` & `autumn8-2.0.1rc1/autumn8/cli/commands/models.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/cli/examples.py` & `autumn8-2.0.1rc1/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/cli/interactive.py` & `autumn8-2.0.1rc1/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/cli/main.py` & `autumn8-2.0.1rc1/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/cli/options.py` & `autumn8-2.0.1rc1/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/cli/pending_uploads.py` & `autumn8-2.0.1rc1/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/cli/validation.py` & `autumn8-2.0.1rc1/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/common/config/cloud_info.py` & `autumn8-2.0.1rc1/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/common/config/settings.py` & `autumn8-2.0.1rc1/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/common/config/supported_instances.py` & `autumn8-2.0.1rc1/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/common/types.py` & `autumn8-2.0.1rc1/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/env/__init__.py` & `autumn8-2.0.1rc1/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/examples/mnist.py` & `autumn8-2.0.1rc1/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/examples/model.py` & `autumn8-2.0.1rc1/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/examples/sbert-alpha.py` & `autumn8-2.0.1rc1/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-2.0.1rc1/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/lib/__init__.py` & `autumn8-2.0.1rc1/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/lib/api/cloud.py` & `autumn8-2.0.1rc1/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/lib/api/lab.py` & `autumn8-2.0.1rc1/autumn8/lib/api/lab.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 
 import appdirs
 import boto3
 import httpx
 import requests
 from mypy_boto3_s3 import S3Client, S3ServiceResource
-from mypy_boto3_s3.type_defs import PartTypeDef
+from mypy_boto3_s3.type_defs import PartOutputTypeDef
 from mypy_boto3_sts.type_defs import CredentialsTypeDef
 from requests.auth import HTTPBasicAuth
 from tqdm.contrib.concurrent import thread_map
 
 from autumn8.cli import pending_uploads
 from autumn8.cli.analyze import is_model_file_link_external, s3path_join
 from autumn8.cli.cli_environment import CliEnvironment
@@ -209,15 +209,15 @@
         file
     )
     return object_key
 
 
 def get_uploaded_parts(
     s3_client: S3Client, s3_bucket_name, s3_file_url, upload_id
-) -> List[PartTypeDef]:
+) -> List[PartOutputTypeDef]:
     res = s3_client.list_parts(
         Bucket=s3_bucket_name, Key=s3_file_url, UploadId=upload_id
     )
     return list(res["Parts"]) if "Parts" in res else []
 
 
 def upload_part(
@@ -225,15 +225,15 @@
     s3_client: S3Client,
     s3_bucket_name,
     s3_file_url,
     file,
     part_size_in_bytes,
     total_bytes,
     mpu_id,
-    parts_already_uploaded: Dict[int, PartTypeDef],
+    parts_already_uploaded: Dict[int, PartOutputTypeDef],
     lock,
 ):
     with lock:
         file.seek((part_number - 1) * part_size_in_bytes)
         data = file.read(part_size_in_bytes)
 
     if not len(data):
```

### Comparing `autumn8-2.0.0rc1/autumn8/lib/api/user.py` & `autumn8-2.0.1rc1/autumn8/lib/api/user.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/lib/api_creds.py` & `autumn8-2.0.1rc1/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/lib/asyncio.py` & `autumn8-2.0.1rc1/autumn8/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/lib/http.py` & `autumn8-2.0.1rc1/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/lib/logging.py` & `autumn8-2.0.1rc1/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/lib/logging.yaml` & `autumn8-2.0.1rc1/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/lib/package_resolver.py` & `autumn8-2.0.1rc1/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/lib/service.py` & `autumn8-2.0.1rc1/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/autumn8/types/deployment.py` & `autumn8-2.0.1rc1/autumn8/types/deployment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import dataclasses
 import enum
 import json
-from typing import Optional, Union
 from dataclasses import dataclass
+from typing import Optional, Union
+
 from pydantic import BaseModel
 
 
 class DeploymentStatus(str, enum.Enum):
     STARTING = "STARTING"
     READY = "READY"
     INVALID = "INVALID"
     CRASHED = "CRASHED"
     SLEEPING = "SLEEPING"
+    TERMINATING = "TERMINATING"
     TERMINATED = "TERMINATED"
 
 
 class ServerType(str, enum.Enum):
     MULTIMODEL_SERVER = "MULTIMODEL_SERVER"
     CUSTOM_PYTORCH_INFERER = "PYTORCH"  # for CLI imported models
     TORCHSERVE = "TORCHSERVE"
@@ -47,18 +49,20 @@
     version: str
     """The version of the manifest"""
 
     uri: str
     """S3 Object key, or HTTP url, under which the model file is available"""
 
     memory: int
+    model_name: str
     model_id: int
     """AutoDL ID of the model"""
 
-    model_name: str
+    optimized: Optional[bool] = None
+
     deployment_id: Optional[
         str
     ] = None  # idk why, but for some time we passed this only for deployments with external s3 bucket models
     model_bucket: Optional[str] = None
     """An external public S3 bucket containing the model file"""
 
     @classmethod
```

### Comparing `autumn8-2.0.0rc1/autumn8.egg-info/PKG-INFO` & `autumn8-2.0.1rc1/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 2.0.0rc1
+Version: 2.0.1rc1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-2.0.0rc1/autumn8.egg-info/SOURCES.txt` & `autumn8-2.0.1rc1/autumn8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/pyproject.toml` & `autumn8-2.0.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/tests/test_io_bottleneck_detection.py` & `autumn8-2.0.1rc1/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-2.0.0rc1/tests/test_settings.py` & `autumn8-2.0.1rc1/tests/test_settings.py`

 * *Files identical despite different names*

