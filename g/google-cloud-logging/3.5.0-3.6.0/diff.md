# Comparing `tmp/google-cloud-logging-3.5.0.tar.gz` & `tmp/google-cloud-logging-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-logging-3.5.0.tar", last modified: Tue Jan 24 23:49:49 2023, max compression
+gzip compressed data, was "google-cloud-logging-3.6.0.tar", last modified: Fri Jul 14 17:27:20 2023, max compression
```

## Comparing `google-cloud-logging-3.5.0.tar` & `google-cloud-logging-3.6.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.069625 google-cloud-logging-3.5.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4164 2023-01-24 23:49:49.069625 google-cloud-logging-3.5.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3249 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.049624 google-cloud-logging-3.5.0/google/
--rw-rw-r--   0 root         (0)     1003      747 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.049624 google-cloud-logging-3.5.0/google/cloud/
--rw-rw-r--   0 root         (0)     1003      747 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.049624 google-cloud-logging-3.5.0/google/cloud/logging/
--rw-rw-r--   0 root         (0)     1003     1700 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.049624 google-cloud-logging-3.5.0/google/cloud/logging/handlers/
--rw-rw-r--   0 root         (0)     1003     1264 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging/handlers/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.049624 google-cloud-logging-3.5.0/google/cloud/logging/handlers/middleware/
--rw-rw-r--   0 root         (0)     1003      711 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging/handlers/middleware/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.053624 google-cloud-logging-3.5.0/google/cloud/logging/handlers/transports/
--rw-rw-r--   0 root         (0)     1003     1191 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging/handlers/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003       81 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.053624 google-cloud-logging-3.5.0/google/cloud/logging_v2/
--rw-rw-r--   0 root         (0)     1003     1946 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    24318 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/_gapic.py
--rw-rw-r--   0 root         (0)     1003     4739 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/_helpers.py
--rw-rw-r--   0 root         (0)     1003    20518 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/_http.py
--rw-rw-r--   0 root         (0)     1003     3315 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/_instrumentation.py
--rw-rw-r--   0 root         (0)     1003    16819 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/client.py
--rw-rw-r--   0 root         (0)     1003    11633 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/entries.py
--rw-rw-r--   0 root         (0)     1003    10136 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.053624 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/
--rw-rw-r--   0 root         (0)     1003     1264 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/__init__.py
--rw-rw-r--   0 root         (0)     1003     7592 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/_helpers.py
--rw-rw-r--   0 root         (0)     1003     6696 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/_monitored_resources.py
--rw-rw-r--   0 root         (0)     1003     4772 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/app_engine.py
--rw-rw-r--   0 root         (0)     1003     2233 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/container_engine.py
--rw-rw-r--   0 root         (0)     1003    11769 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/handlers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.057624 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/middleware/
--rw-rw-r--   0 root         (0)     1003      711 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/middleware/__init__.py
--rw-rw-r--   0 root         (0)     1003     1447 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/middleware/request.py
--rw-rw-r--   0 root         (0)     1003     5428 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/structured_log.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.057624 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/transports/
--rw-rw-r--   0 root         (0)     1003     1192 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11085 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/transports/background_thread.py
--rw-rw-r--   0 root         (0)     1003     1937 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/transports/base.py
--rw-rw-r--   0 root         (0)     1003     2289 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/transports/sync.py
--rw-rw-r--   0 root         (0)     1003    19363 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/logger.py
--rw-rw-r--   0 root         (0)     1003     6316 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/metric.py
--rw-rw-r--   0 root         (0)     1003       81 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/py.typed
--rw-rw-r--   0 root         (0)     1003     1699 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/resource.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.057624 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.057624 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/
--rw-rw-r--   0 root         (0)     1003      773 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   124920 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/async_client.py
--rw-rw-r--   0 root         (0)     1003   137102 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/client.py
--rw-rw-r--   0 root         (0)     1003    20535 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.057624 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/transports/
--rw-rw-r--   0 root         (0)     1003     1203 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20588 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/transports/base.py
--rw-rw-r--   0 root         (0)     1003    44347 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    45399 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.057624 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/
--rw-rw-r--   0 root         (0)     1003      777 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    43918 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/async_client.py
--rw-rw-r--   0 root         (0)     1003    50665 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/client.py
--rw-rw-r--   0 root         (0)     1003    16170 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.061625 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/transports/
--rw-rw-r--   0 root         (0)     1003     1212 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11438 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18610 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18984 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.061625 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/
--rw-rw-r--   0 root         (0)     1003      777 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    34748 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/async_client.py
--rw-rw-r--   0 root         (0)     1003    42619 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/client.py
--rw-rw-r--   0 root         (0)     1003     5822 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.061625 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/transports/
--rw-rw-r--   0 root         (0)     1003     1212 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9993 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16262 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16608 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003     8334 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/sink.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.061625 google-cloud-logging-3.5.0/google/cloud/logging_v2/types/
--rw-rw-r--   0 root         (0)     1003     3990 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    14834 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/types/log_entry.py
--rw-rw-r--   0 root         (0)     1003    23098 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/types/logging.py
--rw-rw-r--   0 root         (0)     1003    63397 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/types/logging_config.py
--rw-rw-r--   0 root         (0)     1003    13539 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/google/cloud/logging_v2/types/logging_metrics.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.065625 google-cloud-logging-3.5.0/google_cloud_logging.egg-info/
--rw-r--r--   0 root         (0)     1003     4164 2023-01-24 23:49:48.000000 google-cloud-logging-3.5.0/google_cloud_logging.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4979 2023-01-24 23:49:49.000000 google-cloud-logging-3.5.0/google_cloud_logging.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-24 23:49:48.000000 google-cloud-logging-3.5.0/google_cloud_logging.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-24 23:49:48.000000 google-cloud-logging-3.5.0/google_cloud_logging.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-24 23:49:48.000000 google-cloud-logging-3.5.0/google_cloud_logging.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      450 2023-01-24 23:49:48.000000 google-cloud-logging-3.5.0/google_cloud_logging.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-24 23:49:48.000000 google-cloud-logging-3.5.0/google_cloud_logging.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-24 23:49:49.073626 google-cloud-logging-3.5.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3146 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.065625 google-cloud-logging-3.5.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.065625 google-cloud-logging-3.5.0/tests/performance/
--rw-rw-r--   0 root         (0)     1003     5732 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/performance/noxfile.py
--rw-rw-r--   0 root         (0)     1003    12836 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/performance/test_performance.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.065625 google-cloud-logging-3.5.0/tests/system/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.049624 google-cloud-logging-3.5.0/tests/system/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.065625 google-cloud-logging-3.5.0/tests/system/gapic/v2/
--rw-rw-r--   0 root         (0)     1003     1188 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/system/gapic/v2/test_system_logging_service_v2_v2.py
--rw-rw-r--   0 root         (0)     1003    36153 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/system/test_system.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.065625 google-cloud-logging-3.5.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.065625 google-cloud-logging-3.5.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.069625 google-cloud-logging-3.5.0/tests/unit/gapic/logging_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/gapic/logging_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   273972 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/gapic/logging_v2/test_config_service_v2.py
--rw-rw-r--   0 root         (0)     1003   109799 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/gapic/logging_v2/test_logging_service_v2.py
--rw-rw-r--   0 root         (0)     1003   105898 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/gapic/logging_v2/test_metrics_service_v2.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.069625 google-cloud-logging-3.5.0/tests/unit/handlers/
--rw-rw-r--   0 root         (0)     1003      574 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.069625 google-cloud-logging-3.5.0/tests/unit/handlers/middleware/
--rw-rw-r--   0 root         (0)     1003     3189 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/middleware/test_request.py
--rw-rw-r--   0 root         (0)     1003    17592 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/test__helpers.py
--rw-rw-r--   0 root         (0)     1003    10014 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/test__monitored_resources.py
--rw-rw-r--   0 root         (0)     1003     8715 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/test_app_engine.py
--rw-rw-r--   0 root         (0)     1003     1832 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/test_container_engine.py
--rw-rw-r--   0 root         (0)     1003    33348 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/test_handlers.py
--rw-rw-r--   0 root         (0)     1003    22138 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/test_structured_log.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-24 23:49:49.069625 google-cloud-logging-3.5.0/tests/unit/handlers/transports/
--rw-rw-r--   0 root         (0)     1003      574 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    18697 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/transports/test_background_thread.py
--rw-rw-r--   0 root         (0)     1003     1324 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/transports/test_base.py
--rw-rw-r--   0 root         (0)     1003     3952 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/handlers/transports/test_sync.py
--rw-rw-r--   0 root         (0)     1003    27360 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/test__gapic.py
--rw-rw-r--   0 root         (0)     1003     7978 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/test__helpers.py
--rw-rw-r--   0 root         (0)     1003    30841 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/test__http.py
--rw-rw-r--   0 root         (0)     1003     2913 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/test__instrumentation.py
--rw-rw-r--   0 root         (0)     1003    33086 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/test_client.py
--rw-rw-r--   0 root         (0)     1003    29785 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/test_entries.py
--rw-rw-r--   0 root         (0)     1003    66978 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/test_logger.py
--rw-rw-r--   0 root         (0)     1003     2605 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/test_logging_shim.py
--rw-rw-r--   0 root         (0)     1003     9521 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/test_metric.py
--rw-rw-r--   0 root         (0)     1003    12732 2023-01-24 23:46:24.000000 google-cloud-logging-3.5.0/tests/unit/test_sink.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.395452 google-cloud-logging-3.6.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4164 2023-07-14 17:27:20.395452 google-cloud-logging-3.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3249 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.375451 google-cloud-logging-3.6.0/google/
+-rw-rw-r--   0 root         (0)     1003      747 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.375451 google-cloud-logging-3.6.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      747 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.375451 google-cloud-logging-3.6.0/google/cloud/logging/
+-rw-rw-r--   0 root         (0)     1003     1700 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.375451 google-cloud-logging-3.6.0/google/cloud/logging/handlers/
+-rw-rw-r--   0 root         (0)     1003     1264 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging/handlers/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.375451 google-cloud-logging-3.6.0/google/cloud/logging/handlers/middleware/
+-rw-rw-r--   0 root         (0)     1003      711 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging/handlers/middleware/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.375451 google-cloud-logging-3.6.0/google/cloud/logging/handlers/transports/
+-rw-rw-r--   0 root         (0)     1003     1191 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging/handlers/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.379451 google-cloud-logging-3.6.0/google/cloud/logging_v2/
+-rw-rw-r--   0 root         (0)     1003     1946 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24318 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/_gapic.py
+-rw-rw-r--   0 root         (0)     1003     4739 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/_helpers.py
+-rw-rw-r--   0 root         (0)     1003    20518 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/_http.py
+-rw-rw-r--   0 root         (0)     1003     3315 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/_instrumentation.py
+-rw-rw-r--   0 root         (0)     1003    16819 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/client.py
+-rw-rw-r--   0 root         (0)     1003    11759 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/entries.py
+-rw-rw-r--   0 root         (0)     1003    10136 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.379451 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/
+-rw-rw-r--   0 root         (0)     1003     1264 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7592 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     6835 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/_monitored_resources.py
+-rw-rw-r--   0 root         (0)     1003     4772 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/app_engine.py
+-rw-rw-r--   0 root         (0)     1003     2233 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/container_engine.py
+-rw-rw-r--   0 root         (0)     1003    11769 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/handlers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.379451 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/middleware/
+-rw-rw-r--   0 root         (0)     1003      711 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/middleware/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1447 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/middleware/request.py
+-rw-rw-r--   0 root         (0)     1003     5428 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/structured_log.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.379451 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/transports/
+-rw-rw-r--   0 root         (0)     1003     1192 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11085 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/transports/background_thread.py
+-rw-rw-r--   0 root         (0)     1003     1937 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/transports/base.py
+-rw-rw-r--   0 root         (0)     1003     2289 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/transports/sync.py
+-rw-rw-r--   0 root         (0)     1003    19336 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/logger.py
+-rw-rw-r--   0 root         (0)     1003     6316 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/metric.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/py.typed
+-rw-rw-r--   0 root         (0)     1003     1699 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/resource.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.379451 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.383451 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   124978 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/async_client.py
+-rw-rw-r--   0 root         (0)     1003   137160 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/client.py
+-rw-rw-r--   0 root         (0)     1003    20535 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.383451 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/transports/
+-rw-rw-r--   0 root         (0)     1003     1203 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20588 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    44347 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    45399 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.383451 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    43922 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/async_client.py
+-rw-rw-r--   0 root         (0)     1003    50669 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/client.py
+-rw-rw-r--   0 root         (0)     1003    16170 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.383451 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/transports/
+-rw-rw-r--   0 root         (0)     1003     1212 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11438 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18610 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18984 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.387452 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    34748 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/async_client.py
+-rw-rw-r--   0 root         (0)     1003    42619 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/client.py
+-rw-rw-r--   0 root         (0)     1003     5822 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.387452 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/transports/
+-rw-rw-r--   0 root         (0)     1003     1212 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9993 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16262 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16608 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003     8334 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/sink.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.387452 google-cloud-logging-3.6.0/google/cloud/logging_v2/types/
+-rw-rw-r--   0 root         (0)     1003     3990 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14870 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/types/log_entry.py
+-rw-rw-r--   0 root         (0)     1003    23134 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/types/logging.py
+-rw-rw-r--   0 root         (0)     1003    63433 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/types/logging_config.py
+-rw-rw-r--   0 root         (0)     1003    13575 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/google/cloud/logging_v2/types/logging_metrics.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.387452 google-cloud-logging-3.6.0/google_cloud_logging.egg-info/
+-rw-r--r--   0 root         (0)     1003     4164 2023-07-14 17:27:20.000000 google-cloud-logging-3.6.0/google_cloud_logging.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4979 2023-07-14 17:27:20.000000 google-cloud-logging-3.6.0/google_cloud_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-14 17:27:20.000000 google-cloud-logging-3.6.0/google_cloud_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-14 17:27:20.000000 google-cloud-logging-3.6.0/google_cloud_logging.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-14 17:27:20.000000 google-cloud-logging-3.6.0/google_cloud_logging.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      450 2023-07-14 17:27:20.000000 google-cloud-logging-3.6.0/google_cloud_logging.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-14 17:27:20.000000 google-cloud-logging-3.6.0/google_cloud_logging.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-14 17:27:20.395452 google-cloud-logging-3.6.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3146 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.387452 google-cloud-logging-3.6.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.387452 google-cloud-logging-3.6.0/tests/performance/
+-rw-rw-r--   0 root         (0)     1003     5732 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/performance/noxfile.py
+-rw-rw-r--   0 root         (0)     1003    12836 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/performance/test_performance.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.387452 google-cloud-logging-3.6.0/tests/system/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.371451 google-cloud-logging-3.6.0/tests/system/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.391452 google-cloud-logging-3.6.0/tests/system/gapic/v2/
+-rw-rw-r--   0 root         (0)     1003     1188 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/system/gapic/v2/test_system_logging_service_v2_v2.py
+-rw-rw-r--   0 root         (0)     1003    36153 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/system/test_system.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.391452 google-cloud-logging-3.6.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.391452 google-cloud-logging-3.6.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.391452 google-cloud-logging-3.6.0/tests/unit/gapic/logging_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/gapic/logging_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   273972 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/gapic/logging_v2/test_config_service_v2.py
+-rw-rw-r--   0 root         (0)     1003   109799 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/gapic/logging_v2/test_logging_service_v2.py
+-rw-rw-r--   0 root         (0)     1003   105898 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/gapic/logging_v2/test_metrics_service_v2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.395452 google-cloud-logging-3.6.0/tests/unit/handlers/
+-rw-rw-r--   0 root         (0)     1003      574 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.395452 google-cloud-logging-3.6.0/tests/unit/handlers/middleware/
+-rw-rw-r--   0 root         (0)     1003     3189 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/middleware/test_request.py
+-rw-rw-r--   0 root         (0)     1003    17592 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003    13053 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/test__monitored_resources.py
+-rw-rw-r--   0 root         (0)     1003     8715 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/test_app_engine.py
+-rw-rw-r--   0 root         (0)     1003     1832 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/test_container_engine.py
+-rw-rw-r--   0 root         (0)     1003    33348 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/test_handlers.py
+-rw-rw-r--   0 root         (0)     1003    22138 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/test_structured_log.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-14 17:27:20.395452 google-cloud-logging-3.6.0/tests/unit/handlers/transports/
+-rw-rw-r--   0 root         (0)     1003      574 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18697 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/transports/test_background_thread.py
+-rw-rw-r--   0 root         (0)     1003     1324 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/transports/test_base.py
+-rw-rw-r--   0 root         (0)     1003     3952 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/handlers/transports/test_sync.py
+-rw-rw-r--   0 root         (0)     1003    27360 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/test__gapic.py
+-rw-rw-r--   0 root         (0)     1003     7978 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003    30841 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/test__http.py
+-rw-rw-r--   0 root         (0)     1003     2913 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/test__instrumentation.py
+-rw-rw-r--   0 root         (0)     1003    33086 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/test_client.py
+-rw-rw-r--   0 root         (0)     1003    29785 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/test_entries.py
+-rw-rw-r--   0 root         (0)     1003    67250 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/test_logger.py
+-rw-rw-r--   0 root         (0)     1003     2605 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/test_logging_shim.py
+-rw-rw-r--   0 root         (0)     1003     9521 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/test_metric.py
+-rw-rw-r--   0 root         (0)     1003    12732 2023-07-14 17:24:40.000000 google-cloud-logging-3.6.0/tests/unit/test_sink.py
```

### Comparing `google-cloud-logging-3.5.0/LICENSE` & `google-cloud-logging-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/MANIFEST.in` & `google-cloud-logging-3.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/PKG-INFO` & `google-cloud-logging-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-logging
-Version: 3.5.0
+Version: 3.6.0
 Summary: Stackdriver Logging API client library
 Home-page: https://github.com/googleapis/python-logging
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-logging-3.5.0/README.rst` & `google-cloud-logging-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/__init__.py` & `google-cloud-logging-3.6.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging/gapic_version.py` & `google-cloud-logging-3.6.0/google/cloud/logging/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.5.0"  # {x-release-please-version}
+__version__ = "3.6.0"  # {x-release-please-version}
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging/handlers/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging/handlers/middleware/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging/handlers/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging/handlers/transports/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging/handlers/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/_gapic.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/_gapic.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/_helpers.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/_http.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/_http.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/_instrumentation.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/_instrumentation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/client.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/entries.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/entries.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,18 @@
         if self.resource is not None:
             info["resource"] = self.resource._to_dict()
         if self.labels is not None:
             info["labels"] = self.labels
         if self.insert_id is not None:
             info["insertId"] = self.insert_id
         if self.severity is not None:
-            info["severity"] = self.severity
+            if isinstance(self.severity, str):
+                info["severity"] = self.severity.upper()
+            else:
+                info["severity"] = self.severity
         if self.http_request is not None:
             info["httpRequest"] = self.http_request
         if self.timestamp is not None:
             info["timestamp"] = _datetime_to_rfc3339(self.timestamp)
         if self.trace is not None:
             info["trace"] = self.trace
         if self.span_id is not None:
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/gapic_metadata.json` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/gapic_version.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.5.0"  # {x-release-please-version}
+__version__ = "3.6.0"  # {x-release-please-version}
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/_helpers.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/_monitored_resources.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/_monitored_resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,16 +67,16 @@
     elif _CLOUD_RUN_SERVICE_ID in os.environ:
         function_name = os.environ.get(_CLOUD_RUN_SERVICE_ID)
     else:
         function_name = ""
     resource = Resource(
         type="cloud_function",
         labels={
-            "project_id": project,
-            "function_name": function_name,
+            "project_id": project if project else "",
+            "function_name": function_name if function_name else "",
             "region": region.split("/")[-1] if region else "",
         },
     )
     return resource
 
 
 def _create_kubernetes_resource():
@@ -87,15 +87,15 @@
     zone = retrieve_metadata_server(_ZONE_ID)
     cluster_name = retrieve_metadata_server(_GKE_CLUSTER_NAME)
     project = retrieve_metadata_server(_PROJECT_NAME)
 
     resource = Resource(
         type="k8s_container",
         labels={
-            "project_id": project,
+            "project_id": project if project else "",
             "location": zone if zone else "",
             "cluster_name": cluster_name if cluster_name else "",
         },
     )
     return resource
 
 
@@ -106,15 +106,15 @@
     """
     instance = retrieve_metadata_server(_GCE_INSTANCE_ID)
     zone = retrieve_metadata_server(_ZONE_ID)
     project = retrieve_metadata_server(_PROJECT_NAME)
     resource = Resource(
         type="gce_instance",
         labels={
-            "project_id": project,
+            "project_id": project if project else "",
             "instance_id": instance if instance else "",
             "zone": zone if zone else "",
         },
     )
     return resource
 
 
@@ -124,15 +124,15 @@
         google.cloud.logging.Resource
     """
     region = retrieve_metadata_server(_REGION_ID)
     project = retrieve_metadata_server(_PROJECT_NAME)
     resource = Resource(
         type="cloud_run_revision",
         labels={
-            "project_id": project,
+            "project_id": project if project else "",
             "service_name": os.environ.get(_CLOUD_RUN_SERVICE_ID, ""),
             "revision_name": os.environ.get(_CLOUD_RUN_REVISION_ID, ""),
             "location": region.split("/")[-1] if region else "",
             "configuration_name": os.environ.get(_CLOUD_RUN_CONFIGURATION_ID, ""),
         },
     )
     return resource
@@ -144,15 +144,15 @@
         google.cloud.logging.Resource
     """
     zone = retrieve_metadata_server(_ZONE_ID)
     project = retrieve_metadata_server(_PROJECT_NAME)
     resource = Resource(
         type="gae_app",
         labels={
-            "project_id": project,
+            "project_id": project if project else "",
             "module_id": os.environ.get(_GAE_SERVICE_ENV, ""),
             "version_id": os.environ.get(_GAE_VERSION_ENV, ""),
             "zone": zone if zone else "",
         },
     )
     return resource
 
@@ -160,15 +160,15 @@
 def _create_global_resource(project):
     """Create a global resource.
     Args:
         project (str): The project ID to pass on to the resource
     Returns:
         google.cloud.logging.Resource
     """
-    return Resource(type="global", labels={"project_id": project})
+    return Resource(type="global", labels={"project_id": project if project else ""})
 
 
 def detect_resource(project=""):
     """Return the default monitored resource based on the local environment.
     If GCP resource not found, defaults to `global`.
 
     Args:
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/app_engine.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/app_engine.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/container_engine.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/container_engine.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/handlers.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/middleware/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/middleware/request.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/middleware/request.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/structured_log.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/structured_log.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/transports/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/transports/background_thread.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/transports/background_thread.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/transports/base.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/handlers/transports/sync.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/handlers/transports/sync.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/logger.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
         # Apply defaults
         kw["log_name"] = kw.pop("log_name", self.full_name)
         kw["labels"] = kw.pop("labels", self.labels)
         kw["resource"] = kw.pop("resource", self.default_resource)
 
         severity = kw.get("severity", None)
-        if isinstance(severity, str) and not severity.isupper():
+        if isinstance(severity, str):
             # convert severity to upper case, as expected by enum definition
             kw["severity"] = severity.upper()
 
         if isinstance(kw["resource"], collections.abc.Mapping):
             # if resource was passed as a dict, attempt to parse it into a
             # Resource object
             try:
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/metric.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/metric.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/resource.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/resource.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/async_client.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.ListBucketsRequest, dict]]):
-                The request object. The parameters to `ListBuckets`.
+                The request object. The parameters to ``ListBuckets``.
             parent (:class:`str`):
                 Required. The parent resource whose buckets are to be
                 listed:
 
                 ::
 
                     "projects/[PROJECT_ID]/locations/[LOCATION_ID]"
@@ -389,15 +389,15 @@
                 response = await client.get_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.GetBucketRequest, dict]]):
-                The request object. The parameters to `GetBucket`.
+                The request object. The parameters to ``GetBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -471,15 +471,15 @@
                 response = await client.create_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.CreateBucketRequest, dict]]):
-                The request object. The parameters to `CreateBucket`.
+                The request object. The parameters to ``CreateBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -561,15 +561,15 @@
                 response = await client.update_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UpdateBucketRequest, dict]]):
-                The request object. The parameters to `UpdateBucket`.
+                The request object. The parameters to ``UpdateBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -642,15 +642,15 @@
                 )
 
                 # Make the request
                 await client.delete_bucket(request=request)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.DeleteBucketRequest, dict]]):
-                The request object. The parameters to `DeleteBucket`.
+                The request object. The parameters to ``DeleteBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -711,15 +711,15 @@
                 )
 
                 # Make the request
                 await client.undelete_bucket(request=request)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UndeleteBucketRequest, dict]]):
-                The request object. The parameters to `UndeleteBucket`.
+                The request object. The parameters to ``UndeleteBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -783,15 +783,15 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.ListViewsRequest, dict]]):
-                The request object. The parameters to `ListViews`.
+                The request object. The parameters to ``ListViews``.
             parent (:class:`str`):
                 Required. The bucket whose views are to be listed:
 
                 ::
 
                     "projects/[PROJECT_ID]/locations/[LOCATION_ID]/buckets/[BUCKET_ID]"
 
@@ -897,15 +897,15 @@
                 response = await client.get_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.GetViewRequest, dict]]):
-                The request object. The parameters to `GetView`.
+                The request object. The parameters to ``GetView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -978,15 +978,15 @@
                 response = await client.create_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.CreateViewRequest, dict]]):
-                The request object. The parameters to `CreateView`.
+                The request object. The parameters to ``CreateView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -1061,15 +1061,15 @@
                 response = await client.update_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UpdateViewRequest, dict]]):
-                The request object. The parameters to `UpdateView`.
+                The request object. The parameters to ``UpdateView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -1140,15 +1140,15 @@
                 )
 
                 # Make the request
                 await client.delete_view(request=request)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.DeleteViewRequest, dict]]):
-                The request object. The parameters to `DeleteView`.
+                The request object. The parameters to ``DeleteView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -1212,15 +1212,15 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.ListSinksRequest, dict]]):
-                The request object. The parameters to `ListSinks`.
+                The request object. The parameters to ``ListSinks``.
             parent (:class:`str`):
                 Required. The parent resource whose sinks are to be
                 listed:
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -1342,15 +1342,15 @@
                 response = await client.get_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.GetSinkRequest, dict]]):
-                The request object. The parameters to `GetSink`.
+                The request object. The parameters to ``GetSink``.
             sink_name (:class:`str`):
                 Required. The resource name of the sink:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
                     "organizations/[ORGANIZATION_ID]/sinks/[SINK_ID]"
@@ -1483,15 +1483,15 @@
                 response = await client.create_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.CreateSinkRequest, dict]]):
-                The request object. The parameters to `CreateSink`.
+                The request object. The parameters to ``CreateSink``.
             parent (:class:`str`):
                 Required. The resource in which to create the sink:
 
                 ::
 
                     "projects/[PROJECT_ID]"
                     "organizations/[ORGANIZATION_ID]"
@@ -1622,15 +1622,15 @@
                 response = await client.update_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UpdateSinkRequest, dict]]):
-                The request object. The parameters to `UpdateSink`.
+                The request object. The parameters to ``UpdateSink``.
             sink_name (:class:`str`):
                 Required. The full resource name of the sink to update,
                 including the parent resource and the sink identifier:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
@@ -1785,15 +1785,15 @@
                 )
 
                 # Make the request
                 await client.delete_sink(request=request)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.DeleteSinkRequest, dict]]):
-                The request object. The parameters to `DeleteSink`.
+                The request object. The parameters to ``DeleteSink``.
             sink_name (:class:`str`):
                 Required. The full resource name of the sink to delete,
                 including the parent resource and the sink identifier:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
@@ -1903,15 +1903,15 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.ListExclusionsRequest, dict]]):
-                The request object. The parameters to `ListExclusions`.
+                The request object. The parameters to ``ListExclusions``.
             parent (:class:`str`):
                 Required. The parent resource whose exclusions are to be
                 listed.
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -2033,15 +2033,15 @@
                 response = await client.get_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.GetExclusionRequest, dict]]):
-                The request object. The parameters to `GetExclusion`.
+                The request object. The parameters to ``GetExclusion``.
             name (:class:`str`):
                 Required. The resource name of an existing exclusion:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
                     "organizations/[ORGANIZATION_ID]/exclusions/[EXCLUSION_ID]"
@@ -2168,15 +2168,15 @@
                 response = await client.create_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.CreateExclusionRequest, dict]]):
-                The request object. The parameters to `CreateExclusion`.
+                The request object. The parameters to ``CreateExclusion``.
             parent (:class:`str`):
                 Required. The parent resource in which to create the
                 exclusion:
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -2304,15 +2304,15 @@
                 response = await client.update_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UpdateExclusionRequest, dict]]):
-                The request object. The parameters to `UpdateExclusion`.
+                The request object. The parameters to ``UpdateExclusion``.
             name (:class:`str`):
                 Required. The resource name of the exclusion to update:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
                     "organizations/[ORGANIZATION_ID]/exclusions/[EXCLUSION_ID]"
@@ -2443,15 +2443,15 @@
                 )
 
                 # Make the request
                 await client.delete_exclusion(request=request)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.DeleteExclusionRequest, dict]]):
-                The request object. The parameters to `DeleteExclusion`.
+                The request object. The parameters to ``DeleteExclusion``.
             name (:class:`str`):
                 Required. The resource name of an existing exclusion to
                 delete:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
@@ -2567,16 +2567,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.GetCmekSettingsRequest, dict]]):
                 The request object. The parameters to
                 [GetCmekSettings][google.logging.v2.ConfigServiceV2.GetCmekSettings].
-                See [Enabling CMEK for Log
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Log
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -2674,16 +2675,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UpdateCmekSettingsRequest, dict]]):
                 The request object. The parameters to
                 [UpdateCmekSettings][google.logging.v2.ConfigServiceV2.UpdateCmekSettings].
-                See [Enabling CMEK for Log
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Log
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -2778,16 +2780,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.GetSettingsRequest, dict]]):
                 The request object. The parameters to
                 [GetSettings][google.logging.v2.ConfigServiceV2.GetSettings].
-                See [Enabling CMEK for Log
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Log
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             name (:class:`str`):
                 Required. The resource for which to retrieve settings.
 
                 ::
 
                     "projects/[PROJECT_ID]/settings"
@@ -2919,16 +2922,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UpdateSettingsRequest, dict]]):
                 The request object. The parameters to
                 [UpdateSettings][google.logging.v2.ConfigServiceV2.UpdateSettings].
-                See [Enabling CMEK for Log
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Log
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             settings (:class:`google.cloud.logging_v2.types.Settings`):
                 Required. The settings to update.
 
                 See `Enabling CMEK for Log
                 Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/client.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,15 +568,15 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.ListBucketsRequest, dict]):
-                The request object. The parameters to `ListBuckets`.
+                The request object. The parameters to ``ListBuckets``.
             parent (str):
                 Required. The parent resource whose buckets are to be
                 listed:
 
                 ::
 
                     "projects/[PROJECT_ID]/locations/[LOCATION_ID]"
@@ -690,15 +690,15 @@
                 response = client.get_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.GetBucketRequest, dict]):
-                The request object. The parameters to `GetBucket`.
+                The request object. The parameters to ``GetBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -773,15 +773,15 @@
                 response = client.create_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.CreateBucketRequest, dict]):
-                The request object. The parameters to `CreateBucket`.
+                The request object. The parameters to ``CreateBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -864,15 +864,15 @@
                 response = client.update_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UpdateBucketRequest, dict]):
-                The request object. The parameters to `UpdateBucket`.
+                The request object. The parameters to ``UpdateBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -946,15 +946,15 @@
                 )
 
                 # Make the request
                 client.delete_bucket(request=request)
 
         Args:
             request (Union[google.cloud.logging_v2.types.DeleteBucketRequest, dict]):
-                The request object. The parameters to `DeleteBucket`.
+                The request object. The parameters to ``DeleteBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -1016,15 +1016,15 @@
                 )
 
                 # Make the request
                 client.undelete_bucket(request=request)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UndeleteBucketRequest, dict]):
-                The request object. The parameters to `UndeleteBucket`.
+                The request object. The parameters to ``UndeleteBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -1089,15 +1089,15 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.ListViewsRequest, dict]):
-                The request object. The parameters to `ListViews`.
+                The request object. The parameters to ``ListViews``.
             parent (str):
                 Required. The bucket whose views are to be listed:
 
                 ::
 
                     "projects/[PROJECT_ID]/locations/[LOCATION_ID]/buckets/[BUCKET_ID]"
 
@@ -1203,15 +1203,15 @@
                 response = client.get_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.GetViewRequest, dict]):
-                The request object. The parameters to `GetView`.
+                The request object. The parameters to ``GetView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -1285,15 +1285,15 @@
                 response = client.create_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.CreateViewRequest, dict]):
-                The request object. The parameters to `CreateView`.
+                The request object. The parameters to ``CreateView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -1369,15 +1369,15 @@
                 response = client.update_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UpdateViewRequest, dict]):
-                The request object. The parameters to `UpdateView`.
+                The request object. The parameters to ``UpdateView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -1449,15 +1449,15 @@
                 )
 
                 # Make the request
                 client.delete_view(request=request)
 
         Args:
             request (Union[google.cloud.logging_v2.types.DeleteViewRequest, dict]):
-                The request object. The parameters to `DeleteView`.
+                The request object. The parameters to ``DeleteView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -1522,15 +1522,15 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.ListSinksRequest, dict]):
-                The request object. The parameters to `ListSinks`.
+                The request object. The parameters to ``ListSinks``.
             parent (str):
                 Required. The parent resource whose sinks are to be
                 listed:
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -1641,15 +1641,15 @@
                 response = client.get_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.GetSinkRequest, dict]):
-                The request object. The parameters to `GetSink`.
+                The request object. The parameters to ``GetSink``.
             sink_name (str):
                 Required. The resource name of the sink:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
                     "organizations/[ORGANIZATION_ID]/sinks/[SINK_ID]"
@@ -1771,15 +1771,15 @@
                 response = client.create_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.CreateSinkRequest, dict]):
-                The request object. The parameters to `CreateSink`.
+                The request object. The parameters to ``CreateSink``.
             parent (str):
                 Required. The resource in which to create the sink:
 
                 ::
 
                     "projects/[PROJECT_ID]"
                     "organizations/[ORGANIZATION_ID]"
@@ -1910,15 +1910,15 @@
                 response = client.update_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UpdateSinkRequest, dict]):
-                The request object. The parameters to `UpdateSink`.
+                The request object. The parameters to ``UpdateSink``.
             sink_name (str):
                 Required. The full resource name of the sink to update,
                 including the parent resource and the sink identifier:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
@@ -2062,15 +2062,15 @@
                 )
 
                 # Make the request
                 client.delete_sink(request=request)
 
         Args:
             request (Union[google.cloud.logging_v2.types.DeleteSinkRequest, dict]):
-                The request object. The parameters to `DeleteSink`.
+                The request object. The parameters to ``DeleteSink``.
             sink_name (str):
                 Required. The full resource name of the sink to delete,
                 including the parent resource and the sink identifier:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
@@ -2169,15 +2169,15 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.ListExclusionsRequest, dict]):
-                The request object. The parameters to `ListExclusions`.
+                The request object. The parameters to ``ListExclusions``.
             parent (str):
                 Required. The parent resource whose exclusions are to be
                 listed.
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -2288,15 +2288,15 @@
                 response = client.get_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.GetExclusionRequest, dict]):
-                The request object. The parameters to `GetExclusion`.
+                The request object. The parameters to ``GetExclusion``.
             name (str):
                 Required. The resource name of an existing exclusion:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
                     "organizations/[ORGANIZATION_ID]/exclusions/[EXCLUSION_ID]"
@@ -2412,15 +2412,15 @@
                 response = client.create_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.CreateExclusionRequest, dict]):
-                The request object. The parameters to `CreateExclusion`.
+                The request object. The parameters to ``CreateExclusion``.
             parent (str):
                 Required. The parent resource in which to create the
                 exclusion:
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -2548,15 +2548,15 @@
                 response = client.update_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UpdateExclusionRequest, dict]):
-                The request object. The parameters to `UpdateExclusion`.
+                The request object. The parameters to ``UpdateExclusion``.
             name (str):
                 Required. The resource name of the exclusion to update:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
                     "organizations/[ORGANIZATION_ID]/exclusions/[EXCLUSION_ID]"
@@ -2687,15 +2687,15 @@
                 )
 
                 # Make the request
                 client.delete_exclusion(request=request)
 
         Args:
             request (Union[google.cloud.logging_v2.types.DeleteExclusionRequest, dict]):
-                The request object. The parameters to `DeleteExclusion`.
+                The request object. The parameters to ``DeleteExclusion``.
             name (str):
                 Required. The resource name of an existing exclusion to
                 delete:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
@@ -2800,16 +2800,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.GetCmekSettingsRequest, dict]):
                 The request object. The parameters to
                 [GetCmekSettings][google.logging.v2.ConfigServiceV2.GetCmekSettings].
-                See [Enabling CMEK for Log
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Log
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -2908,16 +2909,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UpdateCmekSettingsRequest, dict]):
                 The request object. The parameters to
                 [UpdateCmekSettings][google.logging.v2.ConfigServiceV2.UpdateCmekSettings].
-                See [Enabling CMEK for Log
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Log
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -3013,16 +3015,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.GetSettingsRequest, dict]):
                 The request object. The parameters to
                 [GetSettings][google.logging.v2.ConfigServiceV2.GetSettings].
-                See [Enabling CMEK for Log
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Log
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             name (str):
                 Required. The resource for which to retrieve settings.
 
                 ::
 
                     "projects/[PROJECT_ID]/settings"
@@ -3154,16 +3157,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UpdateSettingsRequest, dict]):
                 The request object. The parameters to
                 [UpdateSettings][google.logging.v2.ConfigServiceV2.UpdateSettings].
-                See [Enabling CMEK for Log
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Log
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             settings (google.cloud.logging_v2.types.Settings):
                 Required. The settings to update.
 
                 See `Enabling CMEK for Log
                 Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/pagers.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/transports/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/transports/base.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/transports/grpc.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/config_service_v2/transports/grpc_asyncio.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/config_service_v2/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/async_client.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,15 +576,15 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.ListLogEntriesRequest, dict]]):
-                The request object. The parameters to `ListLogEntries`.
+                The request object. The parameters to ``ListLogEntries``.
             resource_names (:class:`MutableSequence[str]`):
                 Required. Names of one or more parent resources from
                 which to retrieve log entries:
 
                 -  ``projects/[PROJECT_ID]``
                 -  ``organizations/[ORGANIZATION_ID]``
                 -  ``billingAccounts/[BILLING_ACCOUNT_ID]``
@@ -981,15 +981,15 @@
 
                 # Handle the response
                 async for response in stream:
                     print(response)
 
         Args:
             requests (AsyncIterator[`google.cloud.logging_v2.types.TailLogEntriesRequest`]):
-                The request object AsyncIterator. The parameters to `TailLogEntries`.
+                The request object AsyncIterator. The parameters to ``TailLogEntries``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/client.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -774,15 +774,15 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.ListLogEntriesRequest, dict]):
-                The request object. The parameters to `ListLogEntries`.
+                The request object. The parameters to ``ListLogEntries``.
             resource_names (MutableSequence[str]):
                 Required. Names of one or more parent resources from
                 which to retrieve log entries:
 
                 -  ``projects/[PROJECT_ID]``
                 -  ``organizations/[ORGANIZATION_ID]``
                 -  ``billingAccounts/[BILLING_ACCOUNT_ID]``
@@ -1149,15 +1149,15 @@
 
                 # Handle the response
                 for response in stream:
                     print(response)
 
         Args:
             requests (Iterator[google.cloud.logging_v2.types.TailLogEntriesRequest]):
-                The request object iterator. The parameters to `TailLogEntries`.
+                The request object iterator. The parameters to ``TailLogEntries``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/pagers.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/transports/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/transports/base.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/transports/grpc.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/logging_service_v2/transports/grpc_asyncio.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/logging_service_v2/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/async_client.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/client.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/pagers.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/transports/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/transports/base.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc_asyncio.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/sink.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/sink.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/types/__init__.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/types/log_entry.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/types/log_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 from google.api import monitored_resource_pb2  # type: ignore
 from google.logging.type import http_request_pb2  # type: ignore
 from google.logging.type import log_severity_pb2  # type: ignore
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/types/logging.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/types/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 from google.api import monitored_resource_pb2  # type: ignore
 from google.cloud.logging_v2.types import log_entry
 from google.protobuf import duration_pb2  # type: ignore
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/types/logging_config.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/types/logging_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
```

### Comparing `google-cloud-logging-3.5.0/google/cloud/logging_v2/types/logging_metrics.py` & `google-cloud-logging-3.6.0/google/cloud/logging_v2/types/logging_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 from google.api import distribution_pb2  # type: ignore
 from google.api import metric_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
```

### Comparing `google-cloud-logging-3.5.0/google_cloud_logging.egg-info/PKG-INFO` & `google-cloud-logging-3.6.0/google_cloud_logging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-logging
-Version: 3.5.0
+Version: 3.6.0
 Summary: Stackdriver Logging API client library
 Home-page: https://github.com/googleapis/python-logging
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-logging-3.5.0/google_cloud_logging.egg-info/SOURCES.txt` & `google-cloud-logging-3.6.0/google_cloud_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/setup.py` & `google-cloud-logging-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/__init__.py` & `google-cloud-logging-3.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/performance/noxfile.py` & `google-cloud-logging-3.6.0/tests/performance/noxfile.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/performance/test_performance.py` & `google-cloud-logging-3.6.0/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/system/gapic/v2/test_system_logging_service_v2_v2.py` & `google-cloud-logging-3.6.0/tests/system/gapic/v2/test_system_logging_service_v2_v2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/system/test_system.py` & `google-cloud-logging-3.6.0/tests/system/test_system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/__init__.py` & `google-cloud-logging-3.6.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/gapic/__init__.py` & `google-cloud-logging-3.6.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/gapic/logging_v2/__init__.py` & `google-cloud-logging-3.6.0/tests/unit/gapic/logging_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/gapic/logging_v2/test_config_service_v2.py` & `google-cloud-logging-3.6.0/tests/unit/gapic/logging_v2/test_config_service_v2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/gapic/logging_v2/test_logging_service_v2.py` & `google-cloud-logging-3.6.0/tests/unit/gapic/logging_v2/test_logging_service_v2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/gapic/logging_v2/test_metrics_service_v2.py` & `google-cloud-logging-3.6.0/tests/unit/gapic/logging_v2/test_metrics_service_v2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/__init__.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/middleware/test_request.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/middleware/test_request.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/test__helpers.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/test__helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/test__monitored_resources.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/test__monitored_resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
 import mock
 import os
-
+import functools
 
 from google.cloud.logging_v2.handlers._monitored_resources import (
     _create_functions_resource,
 )
 from google.cloud.logging_v2.handlers._monitored_resources import (
     _create_app_engine_resource,
 )
@@ -62,14 +62,28 @@
         ):
             return self.NAME
         elif endpoint == _monitored_resources._PROJECT_NAME:
             return self.PROJECT
         else:
             return None
 
+    def _mock_metadata_no_project(self, endpoint):
+        if (
+            endpoint == _monitored_resources._ZONE_ID
+            or endpoint == _monitored_resources._REGION_ID
+        ):
+            return self.LOCATION
+        elif (
+            endpoint == _monitored_resources._GKE_CLUSTER_NAME
+            or endpoint == _monitored_resources._GCE_INSTANCE_ID
+        ):
+            return self.NAME
+        else:
+            return None
+
     def setUp(self):
         os.environ.clear()
 
     def test_create_legacy_functions_resource(self):
         patch = mock.patch(
             "google.cloud.logging_v2.handlers._monitored_resources.retrieve_metadata_server",
             wraps=self._mock_metadata,
@@ -96,14 +110,31 @@
 
             self.assertIsInstance(func_resource, Resource)
             self.assertEqual(func_resource.type, "cloud_function")
             self.assertEqual(func_resource.labels["project_id"], self.PROJECT)
             self.assertEqual(func_resource.labels["function_name"], self.NAME)
             self.assertEqual(func_resource.labels["region"], self.LOCATION)
 
+    def test_functions_resource_no_name(self):
+        """
+        Simulate functions environment with function name returned as None
+        https://github.com/googleapis/python-logging/pull/718
+        """
+        patch = mock.patch(
+            "google.cloud.logging_v2.handlers._monitored_resources.retrieve_metadata_server",
+            wraps=self._mock_metadata_no_project,
+        )
+        with patch:
+            func_resource = _create_functions_resource()
+
+            self.assertIsInstance(func_resource, Resource)
+            self.assertEqual(func_resource.type, "cloud_function")
+            self.assertEqual(func_resource.labels["project_id"], "")
+            self.assertEqual(func_resource.labels["function_name"], "")
+
     def test_create_kubernetes_resource(self):
 
         patch = mock.patch(
             "google.cloud.logging_v2.handlers._monitored_resources.retrieve_metadata_server",
             wraps=self._mock_metadata,
         )
         with patch:
@@ -165,14 +196,37 @@
 
     def test_global_resource(self):
         resource = _create_global_resource(self.PROJECT)
         self.assertIsInstance(resource, Resource)
         self.assertEqual(resource.type, "global")
         self.assertEqual(resource.labels["project_id"], self.PROJECT)
 
+    def test_with_no_project_from_server(self):
+        """
+        Ensure project_id uses an empty string if not known
+        https://github.com/googleapis/python-logging/issues/710
+        """
+        patch = mock.patch(
+            "google.cloud.logging_v2.handlers._monitored_resources.retrieve_metadata_server",
+            wraps=self._mock_metadata_no_project,
+        )
+        with patch:
+            _global_resource_patched = functools.partial(_create_global_resource, None)
+            resource_fns = [
+                _global_resource_patched,
+                _create_app_engine_resource,
+                _create_cloud_run_resource,
+                _create_compute_resource,
+                _create_kubernetes_resource,
+                _create_functions_resource,
+            ]
+            for fn in resource_fns:
+                resource = fn()
+                self.assertEqual(resource.labels["project_id"], "")
+
 
 class Test_Resource_Detection(unittest.TestCase):
 
     PROJECT = "test-project"
 
     def _mock_k8s_metadata(self, endpoint):
         if (
@@ -185,14 +239,22 @@
 
     def _mock_gce_metadata(self, endpoint):
         if endpoint == _monitored_resources._GCE_INSTANCE_ID:
             return "TRUE"
         else:
             return None
 
+    def _mock_partial_metadata(self, endpoint):
+        if endpoint == _monitored_resources._ZONE_ID:
+            return "ZONE"
+        elif endpoint == _monitored_resources._GCE_INSTANCE_ID:
+            return "instance"
+        else:
+            return None
+
     def setUp(self):
         os.environ.clear()
 
     def test_detect_appengine(self):
         for env in _monitored_resources._GAE_ENV_VARS:
             os.environ[env] = "TRUE"
         resource = detect_resource(self.PROJECT)
@@ -245,7 +307,23 @@
             "google.cloud.logging_v2.handlers._monitored_resources.retrieve_metadata_server",
             return_value=None,
         )
         with patch:
             resource = detect_resource(self.PROJECT)
             self.assertIsInstance(resource, Resource)
             self.assertEqual(resource.type, "global")
+
+    def test_detect_partial_data(self):
+        """
+        Test case where the metadata server returns partial data
+        """
+        patch = mock.patch(
+            "google.cloud.logging_v2.handlers._monitored_resources.retrieve_metadata_server",
+            wraps=self._mock_partial_metadata,
+        )
+        with patch:
+            resource = detect_resource(self.PROJECT)
+            self.assertIsInstance(resource, Resource)
+            self.assertEqual(resource.type, "gce_instance")
+            # project id not returned from metadata serve
+            # should be empty string
+            self.assertEqual(resource.labels["project_id"], "")
```

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/test_app_engine.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/test_app_engine.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/test_container_engine.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/test_container_engine.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/test_handlers.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/test_handlers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/test_structured_log.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/test_structured_log.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/transports/__init__.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/transports/test_background_thread.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/transports/test_background_thread.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/transports/test_base.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/transports/test_base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/handlers/transports/test_sync.py` & `google-cloud-logging-3.6.0/tests/unit/handlers/transports/test_sync.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/test__gapic.py` & `google-cloud-logging-3.6.0/tests/unit/test__gapic.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/test__helpers.py` & `google-cloud-logging-3.6.0/tests/unit/test__helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/test__http.py` & `google-cloud-logging-3.6.0/tests/unit/test__http.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/test__instrumentation.py` & `google-cloud-logging-3.6.0/tests/unit/test__instrumentation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/test_client.py` & `google-cloud-logging-3.6.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/test_entries.py` & `google-cloud-logging-3.6.0/tests/unit/test_entries.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/test_logger.py` & `google-cloud-logging-3.6.0/tests/unit/test_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from copy import deepcopy
-from datetime import datetime
-from datetime import timedelta
-from datetime import timezone
 import sys
-
 import unittest
-import pytest
+from copy import deepcopy
+from datetime import datetime, timedelta, timezone
 
 import mock
+import pytest
 
 
 def _make_credentials():
     import google.auth.credentials
 
     return mock.Mock(spec=google.auth.credentials.Credentials)
 
@@ -127,14 +124,15 @@
 
         self.assertEqual(
             api._write_entries_called_with, (ENTRIES, None, None, None, True)
         )
 
     def test_log_empty_w_explicit(self):
         import datetime
+
         from google.cloud.logging import Resource
 
         ALT_LOG_NAME = "projects/foo/logs/alt.log.name"
         DEFAULT_LABELS = {"foo": "spam"}
         LABELS = {"foo": "bar", "baz": "qux"}
         IID = "IID"
         SEVERITY = "CRITICAL"
@@ -233,14 +231,15 @@
 
         self.assertEqual(
             api._write_entries_called_with, (ENTRIES, None, None, None, True)
         )
 
     def test_log_text_explicit(self):
         import datetime
+
         from google.cloud.logging import Resource
 
         ALT_LOG_NAME = "projects/foo/logs/alt.log.name"
         TEXT = "TEXT"
         DEFAULT_LABELS = {"foo": "spam"}
         LABELS = {"foo": "bar", "baz": "qux"}
         IID = "IID"
@@ -366,14 +365,15 @@
 
         self.assertEqual(
             api._write_entries_called_with, (ENTRIES, None, None, None, True)
         )
 
     def test_log_struct_w_explicit(self):
         import datetime
+
         from google.cloud.logging import Resource
 
         ALT_LOG_NAME = "projects/foo/logs/alt.log.name"
         STRUCT = {"message": "MESSAGE", "weather": "cloudy"}
         DEFAULT_LABELS = {"foo": "spam"}
         LABELS = {"foo": "bar", "baz": "qux"}
         IID = "IID"
@@ -529,18 +529,19 @@
             logger.log(MESSAGE, severity=lower_severity)
 
             self.assertEqual(
                 api._write_entries_called_with, (ENTRIES, None, None, None, True)
             )
 
     def test_log_proto_defaults(self):
+        import json
+
         from google.cloud.logging_v2.handlers._monitored_resources import (
             detect_resource,
         )
-        import json
         from google.protobuf.json_format import MessageToJson
         from google.protobuf.struct_pb2 import Struct, Value
 
         message = Struct(fields={"foo": Value(bool_value=True)})
         ENTRIES = [
             {
                 "logName": "projects/%s/logs/%s" % (self.PROJECT, self.LOGGER_NAME),
@@ -555,18 +556,19 @@
         logger.log_proto(message)
 
         self.assertEqual(
             api._write_entries_called_with, (ENTRIES, None, None, None, True)
         )
 
     def test_log_proto_w_default_labels(self):
+        import json
+
         from google.cloud.logging_v2.handlers._monitored_resources import (
             detect_resource,
         )
-        import json
         from google.protobuf.json_format import MessageToJson
         from google.protobuf.struct_pb2 import Struct, Value
 
         message = Struct(fields={"foo": Value(bool_value=True)})
         DEFAULT_LABELS = {"foo": "spam"}
         ENTRIES = [
             {
@@ -583,20 +585,20 @@
         logger.log_proto(message)
 
         self.assertEqual(
             api._write_entries_called_with, (ENTRIES, None, None, None, True)
         )
 
     def test_log_proto_w_explicit(self):
-        import json
         import datetime
-        from google.protobuf.json_format import MessageToJson
-        from google.protobuf.struct_pb2 import Struct
-        from google.protobuf.struct_pb2 import Value
+        import json
+
         from google.cloud.logging import Resource
+        from google.protobuf.json_format import MessageToJson
+        from google.protobuf.struct_pb2 import Struct, Value
 
         message = Struct(fields={"foo": Value(bool_value=True)})
         ALT_LOG_NAME = "projects/foo/logs/alt.log.name"
         DEFAULT_LABELS = {"foo": "spam"}
         LABELS = {"foo": "bar", "baz": "qux"}
         IID = "IID"
         SEVERITY = "CRITICAL"
@@ -716,19 +718,20 @@
 
         self.assertEqual(
             api._write_entries_called_with, (ENTRIES, None, None, None, True)
         )
 
     def test_log_inference_proto(self):
         import json
-        from google.protobuf.json_format import MessageToJson
-        from google.protobuf.struct_pb2 import Struct, Value
+
         from google.cloud.logging_v2.handlers._monitored_resources import (
             detect_resource,
         )
+        from google.protobuf.json_format import MessageToJson
+        from google.protobuf.struct_pb2 import Struct, Value
 
         message = Struct(fields={"foo": Value(bool_value=True)})
         ENTRIES = [
             {
                 "logName": "projects/%s/logs/%s" % (self.PROJECT, self.LOGGER_NAME),
                 "protoPayload": json.loads(MessageToJson(message)),
                 "resource": detect_resource(self.PROJECT)._to_dict(),
@@ -805,16 +808,15 @@
             client._connection._called_with["data"]["filter"],
             LOG_FILTER + " AND timestamp>=" + self.TIME_FORMAT,
         )
         yesterday = datetime.now(timezone.utc) - timedelta(days=1)
         self.assertLess(yesterday - timestamp, timedelta(minutes=1))
 
     def test_list_entries_explicit(self):
-        from google.cloud.logging import DESCENDING
-        from google.cloud.logging import Client
+        from google.cloud.logging import DESCENDING, Client
 
         PROJECT1 = "PROJECT1"
         PROJECT2 = "PROJECT2"
         INPUT_FILTER = "resource.type:global"
         TOKEN = "TOKEN"
         PAGE_SIZE = 42
         client = Client(
@@ -866,16 +868,15 @@
         timestamp = datetime.strptime(
             client._connection._called_with["data"]["filter"], combined_filter
         )
         yesterday = datetime.now(timezone.utc) - timedelta(days=1)
         self.assertLess(yesterday - timestamp, timedelta(minutes=1))
 
     def test_list_entries_explicit_timestamp(self):
-        from google.cloud.logging import DESCENDING
-        from google.cloud.logging import Client
+        from google.cloud.logging import DESCENDING, Client
 
         PROJECT1 = "PROJECT1"
         PROJECT2 = "PROJECT2"
         INPUT_FILTER = 'resource.type:global AND timestamp="2020-10-13T21"'
         TOKEN = "TOKEN"
         PAGE_SIZE = 42
         client = Client(
@@ -912,19 +913,21 @@
                     "pageToken": TOKEN,
                     "resourceNames": [f"projects/{PROJECT1}", f"projects/{PROJECT2}"],
                 },
             },
         )
 
     def test_list_entries_limit(self):
-        from google.cloud.logging import DESCENDING
-        from google.cloud.logging import ProtobufEntry
-        from google.cloud.logging import StructEntry
-        from google.cloud.logging import Logger
-        from google.cloud.logging import Client
+        from google.cloud.logging import (
+            DESCENDING,
+            Client,
+            Logger,
+            ProtobufEntry,
+            StructEntry,
+        )
 
         PROJECT1 = "PROJECT1"
         PROJECT2 = "PROJECT2"
         INPUT_FILTER = "logName:LOGNAME"
         IID1 = "IID1"
         IID2 = "IID2"
         PAYLOAD = {"message": "MESSAGE", "weather": "partly cloudy"}
@@ -1006,16 +1009,15 @@
                     "pageToken": TOKEN,
                     "resourceNames": [f"projects/{PROJECT1}", f"projects/{PROJECT2}"],
                 },
             },
         )
 
     def test_list_entries_folder(self):
-        from google.cloud.logging import TextEntry
-        from google.cloud.logging import Client
+        from google.cloud.logging import Client, TextEntry
 
         client = Client(
             project=self.PROJECT, credentials=_make_credentials(), _use_grpc=False
         )
         FOLDER_ID = "123"
         LOG_NAME = f"folders/{FOLDER_ID}/logs/cloudaudit.googleapis.com%2Fdata_access"
 
@@ -1038,19 +1040,19 @@
         self.assertEqual(len(entries), 1)
         entry = entries[0]
         self.assertIsInstance(entry, TextEntry)
         self.assertIsNone(entry.logger)
         self.assertEqual(entry.log_name, LOG_NAME)
 
     def test_first_log_emits_instrumentation(self):
+        import google.cloud.logging_v2
+        from google.cloud.logging_v2._instrumentation import _create_diagnostic_entry
         from google.cloud.logging_v2.handlers._monitored_resources import (
             detect_resource,
         )
-        from google.cloud.logging_v2._instrumentation import _create_diagnostic_entry
-        import google.cloud.logging_v2
 
         google.cloud.logging_v2._instrumentation_emitted = False
         DEFAULT_LABELS = {"foo": "spam"}
         resource = detect_resource(self.PROJECT)
         instrumentation_entry = _create_diagnostic_entry(
             resource=resource,
             labels=DEFAULT_LABELS,
@@ -1112,16 +1114,16 @@
         logger = _Logger()
         batch = self._make_one(logger, client=client)
         batch.log_empty()
         self.assertEqual(batch.entries, [ENTRY])
 
     def test_log_empty_explicit(self):
         import datetime
-        from google.cloud.logging import Resource
-        from google.cloud.logging import LogEntry
+
+        from google.cloud.logging import LogEntry, Resource
 
         LABELS = {"foo": "bar", "baz": "qux"}
         IID = "IID"
         SEVERITY = "CRITICAL"
         METHOD = "POST"
         URI = "https://api.example.com/endpoint"
         STATUS = "500"
@@ -1157,29 +1159,29 @@
             trace=TRACE,
             span_id=SPANID,
             trace_sampled=True,
         )
         self.assertEqual(batch.entries, [ENTRY])
 
     def test_log_text_defaults(self):
-        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
         from google.cloud.logging import TextEntry
+        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
 
         TEXT = "This is the entry text"
         ENTRY = TextEntry(payload=TEXT, resource=_GLOBAL_RESOURCE)
         client = _Client(project=self.PROJECT, connection=_make_credentials())
         logger = _Logger()
         batch = self._make_one(logger, client=client)
         batch.log_text(TEXT)
         self.assertEqual(batch.entries, [ENTRY])
 
     def test_log_text_explicit(self):
         import datetime
-        from google.cloud.logging import Resource
-        from google.cloud.logging import TextEntry
+
+        from google.cloud.logging import Resource, TextEntry
 
         TEXT = "This is the entry text"
         LABELS = {"foo": "bar", "baz": "qux"}
         IID = "IID"
         SEVERITY = "CRITICAL"
         METHOD = "POST"
         URI = "https://api.example.com/endpoint"
@@ -1218,29 +1220,29 @@
             trace=TRACE,
             span_id=SPANID,
             trace_sampled=True,
         )
         self.assertEqual(batch.entries, [ENTRY])
 
     def test_log_struct_defaults(self):
-        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
         from google.cloud.logging import StructEntry
+        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
 
         STRUCT = {"message": "Message text", "weather": "partly cloudy"}
         ENTRY = StructEntry(payload=STRUCT, resource=_GLOBAL_RESOURCE)
         client = _Client(project=self.PROJECT, connection=_make_credentials())
         logger = _Logger()
         batch = self._make_one(logger, client=client)
         batch.log_struct(STRUCT)
         self.assertEqual(batch.entries, [ENTRY])
 
     def test_log_struct_explicit(self):
         import datetime
-        from google.cloud.logging import Resource
-        from google.cloud.logging import StructEntry
+
+        from google.cloud.logging import Resource, StructEntry
 
         STRUCT = {"message": "Message text", "weather": "partly cloudy"}
         LABELS = {"foo": "bar", "baz": "qux"}
         IID = "IID"
         SEVERITY = "CRITICAL"
         METHOD = "POST"
         URI = "https://api.example.com/endpoint"
@@ -1279,33 +1281,31 @@
             trace=TRACE,
             span_id=SPANID,
             trace_sampled=True,
         )
         self.assertEqual(batch.entries, [ENTRY])
 
     def test_log_proto_defaults(self):
-        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
         from google.cloud.logging import ProtobufEntry
-        from google.protobuf.struct_pb2 import Struct
-        from google.protobuf.struct_pb2 import Value
+        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
+        from google.protobuf.struct_pb2 import Struct, Value
 
         message = Struct(fields={"foo": Value(bool_value=True)})
         ENTRY = ProtobufEntry(payload=message, resource=_GLOBAL_RESOURCE)
         client = _Client(project=self.PROJECT, connection=_make_credentials())
         logger = _Logger()
         batch = self._make_one(logger, client=client)
         batch.log_proto(message)
         self.assertEqual(batch.entries, [ENTRY])
 
     def test_log_proto_explicit(self):
         import datetime
-        from google.cloud.logging import Resource
-        from google.cloud.logging import ProtobufEntry
-        from google.protobuf.struct_pb2 import Struct
-        from google.protobuf.struct_pb2 import Value
+
+        from google.cloud.logging import ProtobufEntry, Resource
+        from google.protobuf.struct_pb2 import Struct, Value
 
         message = Struct(fields={"foo": Value(bool_value=True)})
         LABELS = {"foo": "bar", "baz": "qux"}
         IID = "IID"
         SEVERITY = "CRITICAL"
         METHOD = "POST"
         URI = "https://api.example.com/endpoint"
@@ -1361,50 +1361,49 @@
         self.assertEqual(batch.entries, [ENTRY])
 
     def test_log_inference_text(self):
         """
         When calling batch.log with text input, it should
         call batch.log_text
         """
-        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
         from google.cloud.logging import TextEntry
+        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
 
         TEXT = "This is the entry text"
         ENTRY = TextEntry(payload=TEXT, resource=_GLOBAL_RESOURCE)
         client = _Client(project=self.PROJECT, connection=_make_credentials())
         logger = _Logger()
         batch = self._make_one(logger, client=client)
         batch.log(TEXT)
         self.assertEqual(batch.entries, [ENTRY])
 
     def test_log_inference_struct(self):
         """
         When calling batch.struct with text input, it should
         call batch.log_struct
         """
-        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
         from google.cloud.logging import StructEntry
+        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
 
         STRUCT = {"message": "Message text", "weather": "partly cloudy"}
         ENTRY = StructEntry(payload=STRUCT, resource=_GLOBAL_RESOURCE)
         client = _Client(project=self.PROJECT, connection=_make_credentials())
         logger = _Logger()
         batch = self._make_one(logger, client=client)
         batch.log(STRUCT)
         self.assertEqual(batch.entries, [ENTRY])
 
     def test_log_inference_proto(self):
         """
         When calling batch.log with proto input, it should
         call batch.log_proto
         """
-        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
         from google.cloud.logging import ProtobufEntry
-        from google.protobuf.struct_pb2 import Struct
-        from google.protobuf.struct_pb2 import Value
+        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
+        from google.protobuf.struct_pb2 import Struct, Value
 
         message = Struct(fields={"foo": Value(bool_value=True)})
         ENTRY = ProtobufEntry(payload=message, resource=_GLOBAL_RESOURCE)
         client = _Client(project=self.PROJECT, connection=_make_credentials())
         logger = _Logger()
         batch = self._make_one(logger, client=client)
         batch.log(message)
@@ -1412,16 +1411,16 @@
 
     def test_log_inference_struct_explicit(self):
         """
         When calling batch.log with struct input, it should
         call batch.log_struct, along with input arguments
         """
         import datetime
-        from google.cloud.logging import Resource
-        from google.cloud.logging import StructEntry
+
+        from google.cloud.logging import Resource, StructEntry
 
         STRUCT = {"message": "Message text", "weather": "partly cloudy"}
         LABELS = {"foo": "bar", "baz": "qux"}
         IID = "IID"
         SEVERITY = "CRITICAL"
         METHOD = "POST"
         URI = "https://api.example.com/endpoint"
@@ -1460,35 +1459,61 @@
             trace=TRACE,
             span_id=SPANID,
             trace_sampled=True,
         )
         self.assertEqual(batch.entries, [ENTRY])
 
     def test_commit_w_unknown_entry_type(self):
-        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
         from google.cloud.logging import LogEntry
+        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
 
         logger = _Logger()
         client = _Client(project=self.PROJECT, connection=_make_credentials())
         api = client.logging_api = _DummyLoggingAPI()
         batch = self._make_one(logger, client)
         batch.entries.append(LogEntry(severity="blah"))
-        ENTRY = {"severity": "blah", "resource": _GLOBAL_RESOURCE._to_dict()}
+        ENTRY = {"severity": "BLAH", "resource": _GLOBAL_RESOURCE._to_dict()}
 
         batch.commit()
 
         self.assertEqual(list(batch.entries), [])
         self.assertEqual(
             api._write_entries_called_with,
             ([ENTRY], logger.full_name, None, None, True),
         )
 
-    def test_commit_w_resource_specified(self):
+    def test_commit_w_lowercase_severity_type(self):
+        from google.cloud.logging import LogEntry
         from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
+
+        logger = _Logger()
+        client = _Client(project=self.PROJECT, connection=_make_credentials())
+        api = client.logging_api = _DummyLoggingAPI()
+        batch = self._make_one(logger, client)
+        batch.entries.append(LogEntry(severity="info"))
+        batch.entries.append(LogEntry(severity="warn"))
+        batch.entries.append(LogEntry(severity="error"))
+        batch.entries.append(LogEntry(severity="fatal"))
+        ENTRIES = [
+            {"severity": "INFO", "resource": _GLOBAL_RESOURCE._to_dict()},
+            {"severity": "WARN", "resource": _GLOBAL_RESOURCE._to_dict()},
+            {"severity": "ERROR", "resource": _GLOBAL_RESOURCE._to_dict()},
+            {"severity": "FATAL", "resource": _GLOBAL_RESOURCE._to_dict()},
+        ]
+
+        batch.commit()
+        self.assertEqual(list(batch.entries), [])
+        self.assertEqual(
+            api._write_entries_called_with,
+            (ENTRIES, logger.full_name, None, None, True),
+        )
+
+    def test_commit_w_resource_specified(self):
         from google.cloud.logging import Resource
+        from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
 
         logger = _Logger()
         client = _Client(project=self.PROJECT, connection=_make_credentials())
         api = client.logging_api = _DummyLoggingAPI()
         RESOURCE = Resource(
             type="gae_app", labels={"module_id": "default", "version_id": "test"}
         )
@@ -1504,21 +1529,21 @@
         batch.commit()
         self.assertEqual(
             api._write_entries_called_with,
             (ENTRIES, logger.full_name, RESOURCE._to_dict(), None, True),
         )
 
     def test_commit_w_bound_client(self):
-        import json
         import datetime
-        from google.protobuf.json_format import MessageToJson
-        from google.protobuf.struct_pb2 import Struct
-        from google.protobuf.struct_pb2 import Value
+        import json
+
         from google.cloud._helpers import _datetime_to_rfc3339
         from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
+        from google.protobuf.json_format import MessageToJson
+        from google.protobuf.struct_pb2 import Struct, Value
 
         TEXT = "This is the entry text"
         STRUCT = {"message": TEXT, "weather": "partly cloudy"}
         message = Struct(fields={"foo": Value(bool_value=True)})
         IID1 = "IID1"
         IID2 = "IID2"
         IID3 = "IID3"
@@ -1595,19 +1620,19 @@
         self.assertEqual(
             api._write_entries_called_with,
             (ENTRIES, logger.full_name, None, None, True),
         )
 
     def test_commit_w_alternate_client(self):
         import json
-        from google.protobuf.json_format import MessageToJson
-        from google.protobuf.struct_pb2 import Struct
-        from google.protobuf.struct_pb2 import Value
+
         from google.cloud.logging import Logger
         from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
+        from google.protobuf.json_format import MessageToJson
+        from google.protobuf.struct_pb2 import Struct, Value
 
         TEXT = "This is the entry text"
         STRUCT = {"message": TEXT, "weather": "partly cloudy"}
         message = Struct(fields={"foo": Value(bool_value=True)})
         DEFAULT_LABELS = {"foo": "spam"}
         LABELS = {"foo": "bar", "baz": "qux"}
         SEVERITY = "CRITICAL"
@@ -1647,19 +1672,19 @@
         self.assertEqual(
             api._write_entries_called_with,
             (ENTRIES, logger.full_name, None, DEFAULT_LABELS, False),
         )
 
     def test_context_mgr_success(self):
         import json
-        from google.protobuf.json_format import MessageToJson
-        from google.protobuf.struct_pb2 import Struct
-        from google.protobuf.struct_pb2 import Value
+
         from google.cloud.logging import Logger
         from google.cloud.logging_v2.entries import _GLOBAL_RESOURCE
+        from google.protobuf.json_format import MessageToJson
+        from google.protobuf.struct_pb2 import Struct, Value
 
         TEXT = "This is the entry text"
         STRUCT = {"message": TEXT, "weather": "partly cloudy"}
         message = Struct(fields={"foo": Value(bool_value=True)})
         DEFAULT_LABELS = {"foo": "spam"}
         LABELS = {"foo": "bar", "baz": "qux"}
         SEVERITY = "CRITICAL"
@@ -1698,19 +1723,17 @@
         self.assertEqual(
             api._write_entries_called_with,
             (ENTRIES, logger.full_name, None, DEFAULT_LABELS, True),
         )
 
     def test_context_mgr_failure(self):
         import datetime
-        from google.protobuf.struct_pb2 import Struct
-        from google.protobuf.struct_pb2 import Value
-        from google.cloud.logging import TextEntry
-        from google.cloud.logging import StructEntry
-        from google.cloud.logging import ProtobufEntry
+
+        from google.cloud.logging import ProtobufEntry, StructEntry, TextEntry
+        from google.protobuf.struct_pb2 import Struct, Value
 
         TEXT = "This is the entry text"
         STRUCT = {"message": TEXT, "weather": "partly cloudy"}
         LABELS = {"foo": "bar", "baz": "qux"}
         IID = "IID"
         SEVERITY = "CRITICAL"
         METHOD = "POST"
@@ -1748,16 +1771,16 @@
     def test_append_context_to_error(self):
         """
         If an InvalidArgument exception contains info on the log that threw it,
         we should be able to add it to the exceptiom message. If not, the
         exception should be unchanged
         """
         from google.api_core.exceptions import InvalidArgument
-        from google.rpc.error_details_pb2 import DebugInfo
         from google.cloud.logging import TextEntry
+        from google.rpc.error_details_pb2 import DebugInfo
 
         logger = _Logger()
         client = _Client(project=self.PROJECT)
         batch = self._make_one(logger, client=client)
         test_entries = [TextEntry(payload=str(i)) for i in range(11)]
         batch.entries = test_entries
         starting_message = "test"
@@ -1799,16 +1822,16 @@
     )
     def test_batch_error_gets_context(self):
         """
         Simulate an InvalidArgument sent as part of a batch commit, to ensure
         _append_context_to_error is thrown
         """
         from google.api_core.exceptions import InvalidArgument
-        from google.rpc.error_details_pb2 import DebugInfo
         from google.cloud.logging import TextEntry
+        from google.rpc.error_details_pb2 import DebugInfo
 
         logger = _Logger()
         client = _Client(project=self.PROJECT)
         starting_message = "hello"
         exception = InvalidArgument(
             starting_message, details=[DebugInfo(detail="key: 1")]
         )
```

### Comparing `google-cloud-logging-3.5.0/tests/unit/test_logging_shim.py` & `google-cloud-logging-3.6.0/tests/unit/test_logging_shim.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/test_metric.py` & `google-cloud-logging-3.6.0/tests/unit/test_metric.py`

 * *Files identical despite different names*

### Comparing `google-cloud-logging-3.5.0/tests/unit/test_sink.py` & `google-cloud-logging-3.6.0/tests/unit/test_sink.py`

 * *Files identical despite different names*

