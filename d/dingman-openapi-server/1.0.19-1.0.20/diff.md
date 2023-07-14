# Comparing `tmp/dingman_openapi_server-1.0.19.tar.gz` & `tmp/dingman_openapi_server-1.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dingman_openapi_server-1.0.19.tar", last modified: Fri Jul 14 18:03:32 2023, max compression
+gzip compressed data, was "dist/dingman_openapi_server-1.0.20.tar", last modified: Fri Jul 14 18:10:48 2023, max compression
```

## Comparing `dingman_openapi_server-1.0.19.tar` & `dingman_openapi_server-1.0.20.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:03:32.000961 dingman_openapi_server-1.0.19/
--rw-r--r--   0 jialening   (501) staff       (20)       20 2023-07-11 00:37:52.000000 dingman_openapi_server-1.0.19/MANIFEST.in
--rw-r--r--   0 jialening   (501) staff       (20)      260 2023-07-14 18:03:32.000609 dingman_openapi_server-1.0.19/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)      902 2023-06-15 21:30:55.000000 dingman_openapi_server-1.0.19/README.md
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:03:31.928516 dingman_openapi_server-1.0.19/dingman_openapi_server.egg-info/
--rw-r--r--   0 jialening   (501) staff       (20)      260 2023-07-14 18:03:31.000000 dingman_openapi_server-1.0.19/dingman_openapi_server.egg-info/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)     2948 2023-07-14 18:03:31.000000 dingman_openapi_server-1.0.19/dingman_openapi_server.egg-info/SOURCES.txt
--rw-r--r--   0 jialening   (501) staff       (20)        1 2023-07-14 18:03:31.000000 dingman_openapi_server-1.0.19/dingman_openapi_server.egg-info/dependency_links.txt
--rw-r--r--   0 jialening   (501) staff       (20)       20 2023-07-14 18:03:31.000000 dingman_openapi_server-1.0.19/dingman_openapi_server.egg-info/requires.txt
--rw-r--r--   0 jialening   (501) staff       (20)       15 2023-07-14 18:03:31.000000 dingman_openapi_server-1.0.19/dingman_openapi_server.egg-info/top_level.txt
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:03:31.932808 dingman_openapi_server-1.0.19/openapi_server/
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-10 22:04:36.000000 dingman_openapi_server-1.0.19/openapi_server/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)      393 2023-07-10 22:04:36.000000 dingman_openapi_server-1.0.19/openapi_server/__main__.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:03:31.935221 dingman_openapi_server-1.0.19/openapi_server/controllers/
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-10 22:04:36.000000 dingman_openapi_server-1.0.19/openapi_server/controllers/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     5687 2023-07-10 22:04:36.000000 dingman_openapi_server-1.0.19/openapi_server/controllers/deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      552 2023-07-10 22:04:36.000000 dingman_openapi_server-1.0.19/openapi_server/controllers/security_controller_.py
--rw-r--r--   0 jialening   (501) staff       (20)      608 2023-07-10 22:04:36.000000 dingman_openapi_server-1.0.19/openapi_server/encoder.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:03:31.992876 dingman_openapi_server-1.0.19/openapi_server/models/
--rw-r--r--   0 jialening   (501) staff       (20)     3610 2023-07-10 22:04:36.000000 dingman_openapi_server-1.0.19/openapi_server/models/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     3753 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-07-10 22:04:36.000000 dingman_openapi_server-1.0.19/openapi_server/models/base_model_.py
--rw-r--r--   0 jialening   (501) staff       (20)     4907 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2503 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/config_templates_inner.py
--rw-r--r--   0 jialening   (501) staff       (20)    16535 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/container.py
--rw-r--r--   0 jialening   (501) staff       (20)     2639 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/container_life_cycle.py
--rw-r--r--   0 jialening   (501) staff       (20)     3654 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/container_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     3936 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/container_sec_context.py
--rw-r--r--   0 jialening   (501) staff       (20)     2568 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/container_sec_context_capabilities.py
--rw-r--r--   0 jialening   (501) staff       (20)    10247 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/deploy_platform_resource.py
--rw-r--r--   0 jialening   (501) staff       (20)     7015 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/deploy_resources.py
--rw-r--r--   0 jialening   (501) staff       (20)     3963 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/dingman_error.py
--rw-r--r--   0 jialening   (501) staff       (20)     2425 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/dingman_response.py
--rw-r--r--   0 jialening   (501) staff       (20)    10477 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/endpoint.py
--rw-r--r--   0 jialening   (501) staff       (20)     3192 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/env_from_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     2961 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/env_var.py
--rw-r--r--   0 jialening   (501) staff       (20)     1827 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/env_var_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     4682 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/http_get.py
--rw-r--r--   0 jialening   (501) staff       (20)     4413 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/http_ingress_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     5643 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/ingress.py
--rw-r--r--   0 jialening   (501) staff       (20)     1821 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/ingress_backend.py
--rw-r--r--   0 jialening   (501) staff       (20)     2446 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/ingress_backend_service.py
--rw-r--r--   0 jialening   (501) staff       (20)     3082 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/ingress_rule.py
--rw-r--r--   0 jialening   (501) staff       (20)     3211 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/ingress_tls.py
--rw-r--r--   0 jialening   (501) staff       (20)     3561 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/life_cycle_handler.py
--rw-r--r--   0 jialening   (501) staff       (20)     4613 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/node_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     2047 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/node_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     3199 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/node_selector_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     2827 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/object_field_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     9740 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)     4948 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/pod.py
--rw-r--r--   0 jialening   (501) staff       (20)     4649 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/pod_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     3664 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     4713 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/pod_anti_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     2623 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/preferred_scheduling_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     7480 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/probe.py
--rw-r--r--   0 jialening   (501) staff       (20)     3598 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/ref_volume_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     6245 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/relabel_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2787 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/resource_requirements.py
--rw-r--r--   0 jialening   (501) staff       (20)     8819 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/service.py
--rw-r--r--   0 jialening   (501) staff       (20)     7583 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/service_monitor.py
--rw-r--r--   0 jialening   (501) staff       (20)     3055 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/service_monitor_namespace_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     5386 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/service_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     2413 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/tcp_socket.py
--rw-r--r--   0 jialening   (501) staff       (20)     3521 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/update_strategy.py
--rw-r--r--   0 jialening   (501) staff       (20)     4965 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/update_strategy_rolling_update_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     6189 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/volume.py
--rw-r--r--   0 jialening   (501) staff       (20)     3553 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/volume_device.py
--rw-r--r--   0 jialening   (501) staff       (20)     2767 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/volume_empty_dir.py
--rw-r--r--   0 jialening   (501) staff       (20)     2585 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/volume_host_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     4139 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/volume_mount.py
--rw-r--r--   0 jialening   (501) staff       (20)     2938 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/volume_persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)     2769 2023-07-10 22:04:35.000000 dingman_openapi_server-1.0.19/openapi_server/models/weighted_pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)    11766 2023-07-11 00:37:52.000000 dingman_openapi_server-1.0.19/openapi_server/models/workload.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:03:31.994179 dingman_openapi_server-1.0.19/openapi_server/openapi/
--rw-r--r--   0 jialening   (501) staff       (20)   168189 2023-07-11 00:37:52.000000 dingman_openapi_server-1.0.19/openapi_server/openapi/openapi.yaml
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:03:31.998165 dingman_openapi_server-1.0.19/openapi_server/test/
--rw-r--r--   0 jialening   (501) staff       (20)      437 2023-07-10 22:04:36.000000 dingman_openapi_server-1.0.19/openapi_server/test/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)   126467 2023-07-11 00:37:52.000000 dingman_openapi_server-1.0.19/openapi_server/test/test_deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      809 2023-07-10 22:04:36.000000 dingman_openapi_server-1.0.19/openapi_server/typing_utils.py
--rw-r--r--   0 jialening   (501) staff       (20)     3533 2023-07-10 22:04:36.000000 dingman_openapi_server-1.0.19/openapi_server/util.py
--rw-r--r--   0 jialening   (501) staff       (20)       38 2023-07-14 18:03:32.001102 dingman_openapi_server-1.0.19/setup.cfg
--rw-r--r--   0 jialening   (501) staff       (20)      847 2023-07-14 18:00:33.000000 dingman_openapi_server-1.0.19/setup.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:10:48.454388 dingman_openapi_server-1.0.20/
+-rw-r--r--   0 jialening   (501) staff       (20)       20 2023-07-11 00:37:52.000000 dingman_openapi_server-1.0.20/MANIFEST.in
+-rw-r--r--   0 jialening   (501) staff       (20)      260 2023-07-14 18:10:48.453817 dingman_openapi_server-1.0.20/PKG-INFO
+-rw-r--r--   0 jialening   (501) staff       (20)      902 2023-06-15 21:30:55.000000 dingman_openapi_server-1.0.20/README.md
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:10:48.390707 dingman_openapi_server-1.0.20/dingman_openapi_server.egg-info/
+-rw-r--r--   0 jialening   (501) staff       (20)      260 2023-07-14 18:10:48.000000 dingman_openapi_server-1.0.20/dingman_openapi_server.egg-info/PKG-INFO
+-rw-r--r--   0 jialening   (501) staff       (20)     3004 2023-07-14 18:10:48.000000 dingman_openapi_server-1.0.20/dingman_openapi_server.egg-info/SOURCES.txt
+-rw-r--r--   0 jialening   (501) staff       (20)        1 2023-07-14 18:10:48.000000 dingman_openapi_server-1.0.20/dingman_openapi_server.egg-info/dependency_links.txt
+-rw-r--r--   0 jialening   (501) staff       (20)       20 2023-07-14 18:10:48.000000 dingman_openapi_server-1.0.20/dingman_openapi_server.egg-info/requires.txt
+-rw-r--r--   0 jialening   (501) staff       (20)       15 2023-07-14 18:10:48.000000 dingman_openapi_server-1.0.20/dingman_openapi_server.egg-info/top_level.txt
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:10:48.396031 dingman_openapi_server-1.0.20/openapi_server/
+-rw-r--r--   0 jialening   (501) staff       (20)     6148 2023-07-14 18:09:20.000000 dingman_openapi_server-1.0.20/openapi_server/.DS_Store
+-rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 18:09:17.000000 dingman_openapi_server-1.0.20/openapi_server/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)      393 2023-07-14 18:09:17.000000 dingman_openapi_server-1.0.20/openapi_server/__main__.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:10:48.398159 dingman_openapi_server-1.0.20/openapi_server/controllers/
+-rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 18:09:17.000000 dingman_openapi_server-1.0.20/openapi_server/controllers/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5687 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/controllers/deploy_resources_controller.py
+-rw-r--r--   0 jialening   (501) staff       (20)      552 2023-07-14 18:09:17.000000 dingman_openapi_server-1.0.20/openapi_server/controllers/security_controller_.py
+-rw-r--r--   0 jialening   (501) staff       (20)      608 2023-07-14 18:09:17.000000 dingman_openapi_server-1.0.20/openapi_server/encoder.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:10:48.445973 dingman_openapi_server-1.0.20/openapi_server/models/
+-rw-r--r--   0 jialening   (501) staff       (20)     3610 2023-07-14 18:09:17.000000 dingman_openapi_server-1.0.20/openapi_server/models/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3753 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-07-14 18:09:17.000000 dingman_openapi_server-1.0.20/openapi_server/models/base_model_.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4907 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2503 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/config_templates_inner.py
+-rw-r--r--   0 jialening   (501) staff       (20)    16535 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/container.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2639 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/container_life_cycle.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3654 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/container_port.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3936 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/container_sec_context.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2568 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/container_sec_context_capabilities.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10247 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/deploy_platform_resource.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7015 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/deploy_resources.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3963 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/dingman_error.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2425 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/dingman_response.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10477 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/endpoint.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3192 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/env_from_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2961 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/env_var.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1827 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/env_var_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4682 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/http_get.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4413 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/http_ingress_path.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5643 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/ingress.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1821 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/ingress_backend.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2446 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/ingress_backend_service.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3082 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/ingress_rule.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3211 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/ingress_tls.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3561 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/life_cycle_handler.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4613 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/node_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2047 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/node_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3199 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/node_selector_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2827 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/object_field_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     9740 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/persistent_volume_claim.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4948 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/pod.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4649 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/pod_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3664 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/pod_affinity_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4713 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/pod_anti_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2623 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/preferred_scheduling_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7480 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/probe.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3598 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/ref_volume_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6245 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/relabel_config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2787 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/resource_requirements.py
+-rw-r--r--   0 jialening   (501) staff       (20)     8819 2023-07-14 18:09:15.000000 dingman_openapi_server-1.0.20/openapi_server/models/service.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7583 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/service_monitor.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3055 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/service_monitor_namespace_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5386 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/service_port.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2413 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/tcp_socket.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3521 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/update_strategy.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4965 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/update_strategy_rolling_update_config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6189 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/volume.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3553 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/volume_device.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2767 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/volume_empty_dir.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2585 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/volume_host_path.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4139 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/volume_mount.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2938 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/volume_persistent_volume_claim.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2769 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/weighted_pod_affinity_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)    11858 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/models/workload.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:10:48.446612 dingman_openapi_server-1.0.20/openapi_server/openapi/
+-rw-r--r--   0 jialening   (501) staff       (20)   168240 2023-07-14 18:09:17.000000 dingman_openapi_server-1.0.20/openapi_server/openapi/openapi.yaml
+-rw-r--r--   0 jialening   (501) staff       (20)        7 2023-07-14 18:09:18.000000 dingman_openapi_server-1.0.20/openapi_server/openapi_version
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-14 18:10:48.452585 dingman_openapi_server-1.0.20/openapi_server/test/
+-rw-r--r--   0 jialening   (501) staff       (20)      437 2023-07-14 18:09:17.000000 dingman_openapi_server-1.0.20/openapi_server/test/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)   126467 2023-07-14 18:09:16.000000 dingman_openapi_server-1.0.20/openapi_server/test/test_deploy_resources_controller.py
+-rw-r--r--   0 jialening   (501) staff       (20)      809 2023-07-14 18:09:17.000000 dingman_openapi_server-1.0.20/openapi_server/typing_utils.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3533 2023-07-14 18:09:17.000000 dingman_openapi_server-1.0.20/openapi_server/util.py
+-rw-r--r--   0 jialening   (501) staff       (20)       38 2023-07-14 18:10:48.454696 dingman_openapi_server-1.0.20/setup.cfg
+-rw-r--r--   0 jialening   (501) staff       (20)      847 2023-07-14 18:00:33.000000 dingman_openapi_server-1.0.20/setup.py
```

### Comparing `dingman_openapi_server-1.0.19/README.md` & `dingman_openapi_server-1.0.20/README.md`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/dingman_openapi_server.egg-info/SOURCES.txt` & `dingman_openapi_server-1.0.20/dingman_openapi_server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 README.md
 setup.py
 dingman_openapi_server.egg-info/PKG-INFO
 dingman_openapi_server.egg-info/SOURCES.txt
 dingman_openapi_server.egg-info/dependency_links.txt
 dingman_openapi_server.egg-info/requires.txt
 dingman_openapi_server.egg-info/top_level.txt
+openapi_server/.DS_Store
 openapi_server/__init__.py
 openapi_server/__main__.py
 openapi_server/encoder.py
+openapi_server/openapi_version
 openapi_server/typing_utils.py
 openapi_server/util.py
 openapi_server/controllers/__init__.py
 openapi_server/controllers/deploy_resources_controller.py
 openapi_server/controllers/security_controller_.py
 openapi_server/models/__init__.py
 openapi_server/models/affinity.py
```

### Comparing `dingman_openapi_server-1.0.19/openapi_server/controllers/deploy_resources_controller.py` & `dingman_openapi_server-1.0.20/openapi_server/controllers/deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/controllers/security_controller_.py` & `dingman_openapi_server-1.0.20/openapi_server/controllers/security_controller_.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/encoder.py` & `dingman_openapi_server-1.0.20/openapi_server/encoder.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/__init__.py` & `dingman_openapi_server-1.0.20/openapi_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/affinity.py` & `dingman_openapi_server-1.0.20/openapi_server/models/affinity.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/base_model_.py` & `dingman_openapi_server-1.0.20/openapi_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/config.py` & `dingman_openapi_server-1.0.20/openapi_server/models/config.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/config_templates_inner.py` & `dingman_openapi_server-1.0.20/openapi_server/models/config_templates_inner.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/container.py` & `dingman_openapi_server-1.0.20/openapi_server/models/container.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/container_life_cycle.py` & `dingman_openapi_server-1.0.20/openapi_server/models/container_life_cycle.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/container_port.py` & `dingman_openapi_server-1.0.20/openapi_server/models/container_port.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/container_sec_context.py` & `dingman_openapi_server-1.0.20/openapi_server/models/container_sec_context.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/container_sec_context_capabilities.py` & `dingman_openapi_server-1.0.20/openapi_server/models/container_sec_context_capabilities.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/deploy_platform_resource.py` & `dingman_openapi_server-1.0.20/openapi_server/models/deploy_platform_resource.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/deploy_resources.py` & `dingman_openapi_server-1.0.20/openapi_server/models/deploy_resources.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/dingman_error.py` & `dingman_openapi_server-1.0.20/openapi_server/models/dingman_error.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/dingman_response.py` & `dingman_openapi_server-1.0.20/openapi_server/models/dingman_response.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/endpoint.py` & `dingman_openapi_server-1.0.20/openapi_server/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/env_from_source.py` & `dingman_openapi_server-1.0.20/openapi_server/models/env_from_source.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/env_var.py` & `dingman_openapi_server-1.0.20/openapi_server/models/env_var.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/env_var_source.py` & `dingman_openapi_server-1.0.20/openapi_server/models/env_var_source.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/http_get.py` & `dingman_openapi_server-1.0.20/openapi_server/models/http_get.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/http_ingress_path.py` & `dingman_openapi_server-1.0.20/openapi_server/models/http_ingress_path.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/ingress.py` & `dingman_openapi_server-1.0.20/openapi_server/models/ingress.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/ingress_backend.py` & `dingman_openapi_server-1.0.20/openapi_server/models/ingress_backend.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/ingress_backend_service.py` & `dingman_openapi_server-1.0.20/openapi_server/models/ingress_backend_service.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/ingress_rule.py` & `dingman_openapi_server-1.0.20/openapi_server/models/ingress_rule.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/ingress_tls.py` & `dingman_openapi_server-1.0.20/openapi_server/models/ingress_tls.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/life_cycle_handler.py` & `dingman_openapi_server-1.0.20/openapi_server/models/life_cycle_handler.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/node_affinity.py` & `dingman_openapi_server-1.0.20/openapi_server/models/node_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/node_selector.py` & `dingman_openapi_server-1.0.20/openapi_server/models/node_selector.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/node_selector_term.py` & `dingman_openapi_server-1.0.20/openapi_server/models/node_selector_term.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/object_field_selector.py` & `dingman_openapi_server-1.0.20/openapi_server/models/object_field_selector.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/persistent_volume_claim.py` & `dingman_openapi_server-1.0.20/openapi_server/models/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/pod.py` & `dingman_openapi_server-1.0.20/openapi_server/models/pod.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/pod_affinity.py` & `dingman_openapi_server-1.0.20/openapi_server/models/pod_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/pod_affinity_term.py` & `dingman_openapi_server-1.0.20/openapi_server/models/pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/pod_anti_affinity.py` & `dingman_openapi_server-1.0.20/openapi_server/models/pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/preferred_scheduling_term.py` & `dingman_openapi_server-1.0.20/openapi_server/models/preferred_scheduling_term.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/probe.py` & `dingman_openapi_server-1.0.20/openapi_server/models/probe.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/ref_volume_source.py` & `dingman_openapi_server-1.0.20/openapi_server/models/ref_volume_source.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/relabel_config.py` & `dingman_openapi_server-1.0.20/openapi_server/models/relabel_config.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/resource_requirements.py` & `dingman_openapi_server-1.0.20/openapi_server/models/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/service.py` & `dingman_openapi_server-1.0.20/openapi_server/models/service.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/service_monitor.py` & `dingman_openapi_server-1.0.20/openapi_server/models/service_monitor.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/service_monitor_namespace_selector.py` & `dingman_openapi_server-1.0.20/openapi_server/models/service_monitor_namespace_selector.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/service_port.py` & `dingman_openapi_server-1.0.20/openapi_server/models/service_port.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/tcp_socket.py` & `dingman_openapi_server-1.0.20/openapi_server/models/tcp_socket.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/update_strategy.py` & `dingman_openapi_server-1.0.20/openapi_server/models/update_strategy.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/update_strategy_rolling_update_config.py` & `dingman_openapi_server-1.0.20/openapi_server/models/update_strategy_rolling_update_config.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/volume.py` & `dingman_openapi_server-1.0.20/openapi_server/models/volume.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/volume_device.py` & `dingman_openapi_server-1.0.20/openapi_server/models/volume_device.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/volume_empty_dir.py` & `dingman_openapi_server-1.0.20/openapi_server/models/volume_empty_dir.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/volume_host_path.py` & `dingman_openapi_server-1.0.20/openapi_server/models/volume_host_path.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/volume_mount.py` & `dingman_openapi_server-1.0.20/openapi_server/models/volume_mount.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/volume_persistent_volume_claim.py` & `dingman_openapi_server-1.0.20/openapi_server/models/volume_persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/weighted_pod_affinity_term.py` & `dingman_openapi_server-1.0.20/openapi_server/models/weighted_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/models/workload.py` & `dingman_openapi_server-1.0.20/openapi_server/models/workload.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,25 +328,25 @@
 
         self._service_name = service_name
 
     @property
     def volume_claim_templates(self):
         """Gets the volume_claim_templates of this Workload.
 
-        volumeClaimTemplates is a list of claims that pods are allowed to reference.  # noqa: E501
+        volumeClaimTemplates is a list of claims that pods are allowed to reference, only valid when workload_type is StatefulSet.  # noqa: E501
 
         :return: The volume_claim_templates of this Workload.
         :rtype: List[PersistentVolumeClaim]
         """
         return self._volume_claim_templates
 
     @volume_claim_templates.setter
     def volume_claim_templates(self, volume_claim_templates):
         """Sets the volume_claim_templates of this Workload.
 
-        volumeClaimTemplates is a list of claims that pods are allowed to reference.  # noqa: E501
+        volumeClaimTemplates is a list of claims that pods are allowed to reference, only valid when workload_type is StatefulSet.  # noqa: E501
 
         :param volume_claim_templates: The volume_claim_templates of this Workload.
         :type volume_claim_templates: List[PersistentVolumeClaim]
         """
 
         self._volume_claim_templates = volume_claim_templates
```

### Comparing `dingman_openapi_server-1.0.19/openapi_server/openapi/openapi.yaml` & `dingman_openapi_server-1.0.20/openapi_server/openapi/openapi.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -5339,5174 +5339,5177 @@
 00014da0: 2d61 7070 0a20 2020 2020 2020 2020 2074  -app.          t
 00014db0: 6974 6c65 3a20 7365 7276 6963 655f 6e61  itle: service_na
 00014dc0: 6d65 0a20 2020 2020 2020 2020 2074 7970  me.          typ
 00014dd0: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
 00014de0: 2020 766f 6c75 6d65 5f63 6c61 696d 5f74    volume_claim_t
 00014df0: 656d 706c 6174 6573 3a0a 2020 2020 2020  emplates:.      
 00014e00: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00014e10: 2076 6f6c 756d 6543 6c61 696d 5465 6d70   volumeClaimTemp
-00014e20: 6c61 7465 7320 6973 2061 206c 6973 7420  lates is a list 
-00014e30: 6f66 2063 6c61 696d 7320 7468 6174 2070  of claims that p
-00014e40: 6f64 7320 6172 6520 616c 6c6f 7765 640a  ods are allowed.
-00014e50: 2020 2020 2020 2020 2020 2020 746f 2072              to r
-00014e60: 6566 6572 656e 6365 2e0a 2020 2020 2020  eference..      
-00014e70: 2020 2020 6974 656d 733a 0a20 2020 2020      items:.     
-00014e80: 2020 2020 2020 2024 7265 663a 2027 232f         $ref: '#/
-00014e90: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00014ea0: 6173 2f50 6572 7369 7374 656e 7456 6f6c  as/PersistentVol
-00014eb0: 756d 6543 6c61 696d 270a 2020 2020 2020  umeClaim'.      
-00014ec0: 2020 2020 7469 746c 653a 2076 6f6c 756d      title: volum
-00014ed0: 655f 636c 6169 6d5f 7465 6d70 6c61 7465  e_claim_template
-00014ee0: 730a 2020 2020 2020 2020 2020 7479 7065  s.          type
-00014ef0: 3a20 6172 7261 790a 2020 2020 2020 7265  : array.      re
-00014f00: 7175 6972 6564 3a0a 2020 2020 2020 2d20  quired:.      - 
-00014f10: 6e61 6d65 0a20 2020 2020 2074 6974 6c65  name.      title
-00014f20: 3a20 576f 726b 6c6f 6164 0a20 2020 2020  : Workload.     
-00014f30: 2074 7970 653a 206f 626a 6563 740a 2020   type: object.  
-00014f40: 2020 416e 6e6f 7461 7469 6f6e 733a 0a20    Annotations:. 
-00014f50: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-00014f60: 3a20 416e 2075 6e73 7472 7563 7475 7265  : An unstructure
-00014f70: 6420 6b65 7920 7661 6c75 6520 6d61 7020  d key value map 
-00014f80: 7468 6174 2063 616e 2062 6520 7573 6564  that can be used
-00014f90: 2074 6f20 6174 7461 6368 2061 7262 6974   to attach arbit
-00014fa0: 7261 7279 0a20 2020 2020 2020 206d 6574  rary.        met
-00014fb0: 6164 6174 610a 2020 2020 2020 6578 616d  adata.      exam
-00014fc0: 706c 653a 0a20 2020 2020 202d 2061 6e6e  ple:.      - ann
-00014fd0: 6f74 6174 696f 6e2d 6b65 7931 3a76 616c  otation-key1:val
-00014fe0: 310a 2020 2020 2020 2d20 616e 6e6f 7461  1.      - annota
-00014ff0: 7469 6f6e 2d6b 6579 323a 7661 6c32 0a20  tion-key2:val2. 
-00015000: 2020 2020 2069 7465 6d73 3a0a 2020 2020       items:.    
-00015010: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-00015020: 0a20 2020 2020 2074 6974 6c65 3a20 416e  .      title: An
-00015030: 6e6f 7461 7469 6f6e 730a 2020 2020 2020  notations.      
-00015040: 7479 7065 3a20 6172 7261 790a 2020 2020  type: array.    
-00015050: 4c61 6265 6c73 3a0a 2020 2020 2020 6465  Labels:.      de
-00015060: 7363 7269 7074 696f 6e3a 204d 6170 206f  scription: Map o
-00015070: 6620 7374 7269 6e67 206b 6579 7320 616e  f string keys an
-00015080: 6420 7661 6c75 6573 2074 6861 7420 6361  d values that ca
-00015090: 6e20 6265 2075 7365 6420 746f 206f 7267  n be used to org
-000150a0: 616e 697a 6520 616e 640a 2020 2020 2020  anize and.      
-000150b0: 2020 6361 7465 676f 7269 7a65 2028 7363    categorize (sc
-000150c0: 6f70 6520 616e 6420 7365 6c65 6374 2920  ope and select) 
-000150d0: 6f62 6a65 6374 730a 2020 2020 2020 6578  objects.      ex
-000150e0: 616d 706c 653a 0a20 2020 2020 202d 2061  ample:.      - a
-000150f0: 7070 3a64 656d 6f2d 6170 700a 2020 2020  pp:demo-app.    
-00015100: 2020 2d20 7665 7273 696f 6e3a 7631 2e30    - version:v1.0
-00015110: 2e30 0a20 2020 2020 2069 7465 6d73 3a0a  .0.      items:.
-00015120: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
-00015130: 7269 6e67 0a20 2020 2020 2074 6974 6c65  ring.      title
-00015140: 3a20 4c61 6265 6c73 0a20 2020 2020 2074  : Labels.      t
-00015150: 7970 653a 2061 7272 6179 0a20 2020 204c  ype: array.    L
-00015160: 6162 656c 5365 6c65 6374 6f72 3a0a 2020  abelSelector:.  
-00015170: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00015180: 207c 0a20 2020 2020 2020 2041 6e20 6172   |.        An ar
-00015190: 7261 7920 6f66 206c 6162 656c 2073 656c  ray of label sel
-000151a0: 6563 746f 7220 7275 6c65 2c20 7468 6520  ector rule, the 
-000151b0: 7275 6c65 2063 616e 2065 6974 6865 7220  rule can either 
-000151c0: 6265 2061 206d 6174 6368 206c 6162 656c  be a match label
-000151d0: 206f 7220 6d61 7463 6820 6578 7072 6573   or match expres
-000151e0: 7369 6f6e 2c0a 2020 2020 2020 2020 7265  sion,.        re
-000151f0: 6665 7272 696e 6720 7468 6520 6578 616d  ferring the exam
-00015200: 706c 6520 2866 6972 7374 2069 7320 6120  ple (first is a 
-00015210: 6d61 7463 6820 6c61 6265 6c2c 2073 6563  match label, sec
-00015220: 6f6e 6420 6973 2061 206d 6174 6368 2065  ond is a match e
-00015230: 7870 7265 7373 696f 6e29 0a20 2020 2020  xpression).     
-00015240: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
-00015250: 2d20 6170 703a 6465 6d6f 2d61 7070 0a20  - app:demo-app. 
-00015260: 2020 2020 202d 2022 6b65 793a 7665 7273       - "key:vers
-00015270: 696f 6e2c 206f 7065 7261 746f 723a 496e  ion, operator:In
-00015280: 2c20 7661 6c75 6573 3a5b 7631 2e30 2e30  , values:[v1.0.0
-00015290: 2c20 7631 2e30 2e31 5d22 0a20 2020 2020  , v1.0.1]".     
-000152a0: 2069 7465 6d73 3a0a 2020 2020 2020 2020   items:.        
-000152b0: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
-000152c0: 2020 2074 6974 6c65 3a20 4c61 6265 6c53     title: LabelS
-000152d0: 656c 6563 746f 720a 2020 2020 2020 7479  elector.      ty
-000152e0: 7065 3a20 6172 7261 790a 2020 2020 5570  pe: array.    Up
-000152f0: 6461 7465 5374 7261 7465 6779 3a0a 2020  dateStrategy:.  
-00015300: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
-00015310: 2020 2020 2073 7472 6174 6567 795f 7479       strategy_ty
-00015320: 7065 3a20 526f 6c6c 696e 6755 7064 6174  pe: RollingUpdat
-00015330: 650a 2020 2020 2020 2020 726f 6c6c 696e  e.        rollin
-00015340: 675f 7570 6461 7465 5f63 6f6e 6669 673a  g_update_config:
-00015350: 0a20 2020 2020 2020 2020 2070 6172 7469  .          parti
-00015360: 7469 6f6e 3a20 320a 2020 2020 2020 2020  tion: 2.        
-00015370: 2020 6d61 785f 756e 6176 6169 6c61 626c    max_unavailabl
-00015380: 653a 2031 3025 206f 7220 320a 2020 2020  e: 10% or 2.    
-00015390: 2020 2020 2020 6d61 785f 7375 7267 653a        max_surge:
-000153a0: 2031 3025 206f 7220 320a 2020 2020 2020   10% or 2.      
-000153b0: 7072 6f70 6572 7469 6573 3a0a 2020 2020  properties:.    
-000153c0: 2020 2020 7374 7261 7465 6779 5f74 7970      strategy_typ
-000153d0: 653a 0a20 2020 2020 2020 2020 2064 6573  e:.          des
-000153e0: 6372 6970 7469 6f6e 3a20 5570 6461 7465  cription: Update
-000153f0: 2073 7472 6174 6567 7920 7479 7065 efbc   strategy type..
-00015400: 8c20 7573 6564 2074 6f20 7370 6563 6966  . used to specif
-00015410: 7920 7468 6520 7570 6461 7465 2073 7472  y the update str
-00015420: 6174 6567 7920 666f 720a 2020 2020 2020  ategy for.      
-00015430: 2020 2020 2020 7468 6520 576f 726b 6c6f        the Worklo
-00015440: 6164 2e0a 2020 2020 2020 2020 2020 656e  ad..          en
-00015450: 756d 3a0a 2020 2020 2020 2020 2020 2d20  um:.          - 
-00015460: 5265 6372 6561 7465 0a20 2020 2020 2020  Recreate.       
-00015470: 2020 202d 2052 6f6c 6c69 6e67 5570 6461     - RollingUpda
-00015480: 7465 0a20 2020 2020 2020 2020 202d 204f  te.          - O
-00015490: 6e44 656c 6574 650a 2020 2020 2020 2020  nDelete.        
-000154a0: 2020 6578 616d 706c 653a 2052 6f6c 6c69    example: Rolli
-000154b0: 6e67 5570 6461 7465 0a20 2020 2020 2020  ngUpdate.       
-000154c0: 2020 2074 6974 6c65 3a20 7374 7261 7465     title: strate
-000154d0: 6779 5f74 7970 650a 2020 2020 2020 2020  gy_type.        
-000154e0: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-000154f0: 2020 2020 2020 2072 6f6c 6c69 6e67 5f75         rolling_u
-00015500: 7064 6174 655f 636f 6e66 6967 3a0a 2020  pdate_config:.  
-00015510: 2020 2020 2020 2020 2472 6566 3a20 2723          $ref: '#
-00015520: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00015530: 6d61 732f 5570 6461 7465 5374 7261 7465  mas/UpdateStrate
-00015540: 6779 5f72 6f6c 6c69 6e67 5f75 7064 6174  gy_rolling_updat
-00015550: 655f 636f 6e66 6967 270a 2020 2020 2020  e_config'.      
-00015560: 7469 746c 653a 2055 7064 6174 6553 7472  title: UpdateStr
-00015570: 6174 6567 790a 2020 2020 2020 7479 7065  ategy.      type
-00015580: 3a20 6f62 6a65 6374 0a20 2020 2050 6f64  : object.    Pod
-00015590: 3a0a 2020 2020 2020 6578 616d 706c 653a  :.      example:
-000155a0: 0a20 2020 2020 2020 2076 6f6c 756d 6573  .        volumes
-000155b0: 3a0a 2020 2020 2020 2020 2d20 686f 7374  :.        - host
-000155c0: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
-000155d0: 2020 2070 6174 683a 202f 6461 7461 0a20     path: /data. 
-000155e0: 2020 2020 2020 2020 2020 2070 6174 685f             path_
-000155f0: 7479 7065 3a20 4469 7265 6374 6f72 790a  type: Directory.
-00015600: 2020 2020 2020 2020 2020 6e61 6d65 3a20            name: 
-00015610: 6465 6d6f 2d76 6f6c 0a20 2020 2020 2020  demo-vol.       
-00015620: 2020 2065 6d70 7479 5f64 6972 3a0a 2020     empty_dir:.  
-00015630: 2020 2020 2020 2020 2020 6d65 6469 756d            medium
-00015640: 3a20 4d65 6d6f 7279 0a20 2020 2020 2020  : Memory.       
-00015650: 2020 2020 2073 697a 655f 6c69 6d69 743a       size_limit:
-00015660: 2035 3030 4d69 0a20 2020 2020 2020 2020   500Mi.         
-00015670: 2063 6f6e 6669 675f 6d61 703a 0a20 2020   config_map:.   
-00015680: 2020 2020 2020 2020 206e 616d 653a 2073           name: s
-00015690: 6572 7665 7220 636f 6e66 6967 2f73 6563  erver config/sec
-000156a0: 7265 740a 2020 2020 2020 2020 2020 2020  ret.            
-000156b0: 6f70 7469 6f6e 616c 3a20 6661 6c73 650a  optional: false.
-000156c0: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-000156d0: 756c 745f 6d6f 6465 3a20 3430 300a 2020  ult_mode: 400.  
-000156e0: 2020 2020 2020 2020 7365 6372 6574 3a0a          secret:.
-000156f0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00015700: 3a20 7365 7276 6572 2063 6f6e 6669 672f  : server config/
-00015710: 7365 6372 6574 0a20 2020 2020 2020 2020  secret.         
-00015720: 2020 206f 7074 696f 6e61 6c3a 2066 616c     optional: fal
-00015730: 7365 0a20 2020 2020 2020 2020 2020 2064  se.            d
-00015740: 6566 6175 6c74 5f6d 6f64 653a 2034 3030  efault_mode: 400
-00015750: 0a20 2020 2020 2020 2020 2070 6572 7369  .          persi
-00015760: 7374 656e 745f 766f 6c75 6d65 5f63 6c61  stent_volume_cla
-00015770: 696d 3a0a 2020 2020 2020 2020 2020 2020  im:.            
-00015780: 7265 6164 5f6f 6e6c 793a 2066 616c 7365  read_only: false
-00015790: 0a20 2020 2020 2020 2020 2020 2063 6c61  .            cla
-000157a0: 696d 5f6e 616d 653a 2064 656d 6f2d 7076  im_name: demo-pv
-000157b0: 630a 2020 2020 2020 2020 2d20 686f 7374  c.        - host
-000157c0: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
-000157d0: 2020 2070 6174 683a 202f 6461 7461 0a20     path: /data. 
-000157e0: 2020 2020 2020 2020 2020 2070 6174 685f             path_
-000157f0: 7479 7065 3a20 4469 7265 6374 6f72 790a  type: Directory.
-00015800: 2020 2020 2020 2020 2020 6e61 6d65 3a20            name: 
-00015810: 6465 6d6f 2d76 6f6c 0a20 2020 2020 2020  demo-vol.       
-00015820: 2020 2065 6d70 7479 5f64 6972 3a0a 2020     empty_dir:.  
-00015830: 2020 2020 2020 2020 2020 6d65 6469 756d            medium
-00015840: 3a20 4d65 6d6f 7279 0a20 2020 2020 2020  : Memory.       
-00015850: 2020 2020 2073 697a 655f 6c69 6d69 743a       size_limit:
-00015860: 2035 3030 4d69 0a20 2020 2020 2020 2020   500Mi.         
-00015870: 2063 6f6e 6669 675f 6d61 703a 0a20 2020   config_map:.   
-00015880: 2020 2020 2020 2020 206e 616d 653a 2073           name: s
-00015890: 6572 7665 7220 636f 6e66 6967 2f73 6563  erver config/sec
-000158a0: 7265 740a 2020 2020 2020 2020 2020 2020  ret.            
-000158b0: 6f70 7469 6f6e 616c 3a20 6661 6c73 650a  optional: false.
-000158c0: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-000158d0: 756c 745f 6d6f 6465 3a20 3430 300a 2020  ult_mode: 400.  
-000158e0: 2020 2020 2020 2020 7365 6372 6574 3a0a          secret:.
-000158f0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00015900: 3a20 7365 7276 6572 2063 6f6e 6669 672f  : server config/
-00015910: 7365 6372 6574 0a20 2020 2020 2020 2020  secret.         
-00015920: 2020 206f 7074 696f 6e61 6c3a 2066 616c     optional: fal
-00015930: 7365 0a20 2020 2020 2020 2020 2020 2064  se.            d
-00015940: 6566 6175 6c74 5f6d 6f64 653a 2034 3030  efault_mode: 400
-00015950: 0a20 2020 2020 2020 2020 2070 6572 7369  .          persi
-00015960: 7374 656e 745f 766f 6c75 6d65 5f63 6c61  stent_volume_cla
-00015970: 696d 3a0a 2020 2020 2020 2020 2020 2020  im:.            
-00015980: 7265 6164 5f6f 6e6c 793a 2066 616c 7365  read_only: false
-00015990: 0a20 2020 2020 2020 2020 2020 2063 6c61  .            cla
-000159a0: 696d 5f6e 616d 653a 2064 656d 6f2d 7076  im_name: demo-pv
-000159b0: 630a 2020 2020 2020 2020 616e 6e6f 7461  c.        annota
-000159c0: 7469 6f6e 733a 0a20 2020 2020 2020 202d  tions:.        -
-000159d0: 2061 6e6e 6f74 6174 696f 6e2d 6b65 7931   annotation-key1
-000159e0: 3a76 616c 310a 2020 2020 2020 2020 2d20  :val1.        - 
-000159f0: 616e 6e6f 7461 7469 6f6e 2d6b 6579 323a  annotation-key2:
-00015a00: 7661 6c32 0a20 2020 2020 2020 2063 6f6e  val2.        con
-00015a10: 7461 696e 6572 733a 0a20 2020 2020 2020  tainers:.       
-00015a20: 202d 2069 6d61 6765 3a20 6e67 696e 783a   - image: nginx:
-00015a30: 6c61 7465 7374 0a20 2020 2020 2020 2020  latest.         
-00015a40: 206c 6966 655f 6379 636c 653a 0a20 2020   life_cycle:.   
-00015a50: 2020 2020 2020 2020 2070 7265 5f73 746f           pre_sto
-00015a60: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-00015a70: 2074 6370 5f73 6f63 6b65 743a 0a20 2020   tcp_socket:.   
-00015a80: 2020 2020 2020 2020 2020 2020 2070 6f72               por
-00015a90: 743a 2033 3031 3831 0a20 2020 2020 2020  t: 30181.       
-00015aa0: 2020 2020 2020 2020 2068 6f73 743a 2031           host: 1
-00015ab0: 3237 2e30 2e30 2e31 0a20 2020 2020 2020  27.0.0.1.       
-00015ac0: 2020 2020 2020 2068 7474 705f 6765 743a         http_get:
-00015ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015ae0: 2070 6174 683a 202f 7368 6f77 3f64 6f6d   path: /show?dom
-00015af0: 6169 6e3d 7631 392e 7469 6b74 6f6b 6364  ain=v19.tiktokcd
-00015b00: 6e2e 636f 6d0a 2020 2020 2020 2020 2020  n.com.          
-00015b10: 2020 2020 2020 6874 7470 5f68 6561 6465        http_heade
-00015b20: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-00015b30: 2020 2020 2d20 782d 6465 7673 7265 2d61      - x-devsre-a
-00015b40: 7574 686f 7269 7a61 7469 6f6e 3a42 6561  uthorization:Bea
-00015b50: 7265 7220 6579 4a68 6247 6369 4f69 4a0a  rer eyJhbGciOiJ.
-00015b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b70: 2d20 636f 6e74 656e 742d 7479 7065 3a61  - content-type:a
-00015b80: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e0a  pplication/json.
-00015b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ba0: 7363 6865 6d65 3a20 4854 5450 530a 2020  scheme: HTTPS.  
-00015bb0: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00015bc0: 7274 3a20 3838 3838 0a20 2020 2020 2020  rt: 8888.       
-00015bd0: 2020 2020 2020 2020 2068 6f73 743a 2067           host: g
-00015be0: 7373 2d64 6e73 2d61 6765 6e74 2e65 7861  ss-dns-agent.exa
-00015bf0: 6d70 6c65 2e6f 7267 0a20 2020 2020 2020  mple.org.       
-00015c00: 2020 2020 2020 2065 7865 635f 636f 6d6d         exec_comm
-00015c10: 616e 643a 0a20 2020 2020 2020 2020 2020  and:.           
-00015c20: 2020 202d 202f 6269 6e2f 7368 6f77 646f     - /bin/showdo
-00015c30: 776e 2e73 680a 2020 2020 2020 2020 2020  wn.sh.          
-00015c40: 2020 706f 7374 5f73 7461 7274 3a0a 2020    post_start:.  
-00015c50: 2020 2020 2020 2020 2020 2020 7463 705f              tcp_
-00015c60: 736f 636b 6574 3a0a 2020 2020 2020 2020  socket:.        
-00015c70: 2020 2020 2020 2020 706f 7274 3a20 3330          port: 30
-00015c80: 3138 310a 2020 2020 2020 2020 2020 2020  181.            
-00015c90: 2020 2020 686f 7374 3a20 3132 372e 302e      host: 127.0.
-00015ca0: 302e 310a 2020 2020 2020 2020 2020 2020  0.1.            
-00015cb0: 2020 6874 7470 5f67 6574 3a0a 2020 2020    http_get:.    
-00015cc0: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00015cd0: 3a20 2f73 686f 773f 646f 6d61 696e 3d76  : /show?domain=v
-00015ce0: 3139 2e74 696b 746f 6b63 646e 2e63 6f6d  19.tiktokcdn.com
-00015cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015d00: 2068 7474 705f 6865 6164 6572 733a 0a20   http_headers:. 
-00015d10: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-00015d20: 2078 2d64 6576 7372 652d 6175 7468 6f72   x-devsre-author
-00015d30: 697a 6174 696f 6e3a 4265 6172 6572 2065  ization:Bearer e
-00015d40: 794a 6862 4763 694f 694a 0a20 2020 2020  yJhbGciOiJ.     
-00015d50: 2020 2020 2020 2020 2020 202d 2063 6f6e             - con
-00015d60: 7465 6e74 2d74 7970 653a 6170 706c 6963  tent-type:applic
-00015d70: 6174 696f 6e2f 6a73 6f6e 0a20 2020 2020  ation/json.     
-00015d80: 2020 2020 2020 2020 2020 2073 6368 656d             schem
-00015d90: 653a 2048 5454 5053 0a20 2020 2020 2020  e: HTTPS.       
-00015da0: 2020 2020 2020 2020 2070 6f72 743a 2038           port: 8
-00015db0: 3838 380a 2020 2020 2020 2020 2020 2020  888.            
-00015dc0: 2020 2020 686f 7374 3a20 6773 732d 646e      host: gss-dn
-00015dd0: 732d 6167 656e 742e 6578 616d 706c 652e  s-agent.example.
-00015de0: 6f72 670a 2020 2020 2020 2020 2020 2020  org.            
-00015df0: 2020 6578 6563 5f63 6f6d 6d61 6e64 3a0a    exec_command:.
-00015e00: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00015e10: 2f62 696e 2f73 686f 7764 6f77 6e2e 7368  /bin/showdown.sh
-00015e20: 0a20 2020 2020 2020 2020 2072 6573 6f75  .          resou
-00015e30: 7263 6573 3a0a 2020 2020 2020 2020 2020  rces:.          
-00015e40: 2020 7265 7175 6573 7473 3a0a 2020 2020    requests:.    
-00015e50: 2020 2020 2020 2020 2020 6d65 6d6f 7279            memory
-00015e60: 3a20 3235 364d 690a 2020 2020 2020 2020  : 256Mi.        
-00015e70: 2020 2020 2020 6370 753a 2022 302e 3122        cpu: "0.1"
-00015e80: 0a20 2020 2020 2020 2020 2020 206c 696d  .            lim
-00015e90: 6974 733a 0a20 2020 2020 2020 2020 2020  its:.           
-00015ea0: 2020 206d 656d 6f72 793a 2035 3132 4d69     memory: 512Mi
-00015eb0: 0a20 2020 2020 2020 2020 2020 2020 2063  .              c
-00015ec0: 7075 3a20 2230 2e35 220a 2020 2020 2020  pu: "0.5".      
-00015ed0: 2020 2020 766f 6c75 6d65 5f6d 6f75 6e74      volume_mount
-00015ee0: 733a 0a20 2020 2020 2020 2020 202d 2070  s:.          - p
-00015ef0: 6174 683a 202f 6f70 742f 7365 7276 6572  ath: /opt/server
-00015f00: 2f63 6f6e 660a 2020 2020 2020 2020 2020  /conf.          
-00015f10: 2020 7265 6164 5f6f 6e6c 793a 2074 7275    read_only: tru
-00015f20: 650a 2020 2020 2020 2020 2020 2020 6e61  e.            na
-00015f30: 6d65 3a20 6465 6d6f 2d76 6f6c 0a20 2020  me: demo-vol.   
-00015f40: 2020 2020 2020 2020 2073 7562 5f70 6174           sub_pat
-00015f50: 683a 2073 6572 7665 722e 636f 6e66 0a20  h: server.conf. 
-00015f60: 2020 2020 2020 2020 202d 2070 6174 683a           - path:
-00015f70: 202f 6f70 742f 7365 7276 6572 2f63 6f6e   /opt/server/con
-00015f80: 660a 2020 2020 2020 2020 2020 2020 7265  f.            re
-00015f90: 6164 5f6f 6e6c 793a 2074 7275 650a 2020  ad_only: true.  
-00015fa0: 2020 2020 2020 2020 2020 6e61 6d65 3a20            name: 
-00015fb0: 6465 6d6f 2d76 6f6c 0a20 2020 2020 2020  demo-vol.       
-00015fc0: 2020 2020 2073 7562 5f70 6174 683a 2073       sub_path: s
-00015fd0: 6572 7665 722e 636f 6e66 0a20 2020 2020  erver.conf.     
-00015fe0: 2020 2020 2065 6e76 3a0a 2020 2020 2020       env:.      
-00015ff0: 2020 2020 2020 6e61 6d65 3a20 534d 535f        name: SMS_
-00016000: 4b45 5953 5f50 4154 485f 584d 0a20 2020  KEYS_PATH_XM.   
-00016010: 2020 2020 2020 2020 2076 616c 7565 3a20           value: 
-00016020: 646d 732d 7365 6372 6574 0a20 2020 2020  dms-secret.     
-00016030: 2020 2020 2070 6f72 7473 3a0a 2020 2020       ports:.    
-00016040: 2020 2020 2020 2d20 636f 6e74 6169 6e65        - containe
-00016050: 725f 706f 7274 3a20 3830 0a20 2020 2020  r_port: 80.     
-00016060: 2020 2020 2020 2070 726f 746f 636f 6c3a         protocol:
-00016070: 2054 4350 0a20 2020 2020 2020 2020 2020   TCP.           
-00016080: 206e 616d 653a 2068 7474 700a 2020 2020   name: http.    
-00016090: 2020 2020 2020 2d20 636f 6e74 6169 6e65        - containe
-000160a0: 725f 706f 7274 3a20 3830 0a20 2020 2020  r_port: 80.     
-000160b0: 2020 2020 2020 2070 726f 746f 636f 6c3a         protocol:
-000160c0: 2054 4350 0a20 2020 2020 2020 2020 2020   TCP.           
-000160d0: 206e 616d 653a 2068 7474 700a 2020 2020   name: http.    
-000160e0: 2020 2020 2020 636f 6d6d 616e 643a 0a20        command:. 
-000160f0: 2020 2020 2020 2020 202d 2070 7974 686f           - pytho
-00016100: 6e33 0a20 2020 2020 2020 2020 2061 7267  n3.          arg
-00016110: 733a 0a20 2020 2020 2020 2020 202d 202d  s:.          - -
-00016120: 6d0a 2020 2020 2020 2020 2020 2d20 6f70  m.          - op
-00016130: 656e 6170 695f 7365 7276 6572 0a20 2020  enapi_server.   
-00016140: 2020 2020 2020 2072 6561 6469 6e65 7373         readiness
-00016150: 5f70 726f 6265 3a0a 2020 2020 2020 2020  _probe:.        
-00016160: 2020 2020 7065 7269 6f64 5f73 6563 6f6e      period_secon
-00016170: 6473 3a20 3630 0a20 2020 2020 2020 2020  ds: 60.         
-00016180: 2020 2069 6e69 7469 616c 5f64 656c 6179     initial_delay
-00016190: 5f73 6563 6f6e 6473 3a20 3630 300a 2020  _seconds: 600.  
-000161a0: 2020 2020 2020 2020 2020 7463 705f 736f            tcp_so
-000161b0: 636b 6574 3a0a 2020 2020 2020 2020 2020  cket:.          
-000161c0: 2020 2020 706f 7274 3a20 3330 3138 310a      port: 30181.
-000161d0: 2020 2020 2020 2020 2020 2020 2020 686f                ho
-000161e0: 7374 3a20 3132 372e 302e 302e 310a 2020  st: 127.0.0.1.  
-000161f0: 2020 2020 2020 2020 2020 6661 696c 7572            failur
-00016200: 655f 7468 7265 7368 6f6c 643a 2033 0a20  e_threshold: 3. 
-00016210: 2020 2020 2020 2020 2020 2068 7474 705f             http_
-00016220: 6765 743a 0a20 2020 2020 2020 2020 2020  get:.           
-00016230: 2020 2070 6174 683a 202f 7368 6f77 3f64     path: /show?d
-00016240: 6f6d 6169 6e3d 7631 392e 7469 6b74 6f6b  omain=v19.tiktok
-00016250: 6364 6e2e 636f 6d0a 2020 2020 2020 2020  cdn.com.        
-00016260: 2020 2020 2020 6874 7470 5f68 6561 6465        http_heade
-00016270: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-00016280: 2020 2d20 782d 6465 7673 7265 2d61 7574    - x-devsre-aut
-00016290: 686f 7269 7a61 7469 6f6e 3a42 6561 7265  horization:Beare
-000162a0: 7220 6579 4a68 6247 6369 4f69 4a0a 2020  r eyJhbGciOiJ.  
-000162b0: 2020 2020 2020 2020 2020 2020 2d20 636f              - co
-000162c0: 6e74 656e 742d 7479 7065 3a61 7070 6c69  ntent-type:appli
-000162d0: 6361 7469 6f6e 2f6a 736f 6e0a 2020 2020  cation/json.    
-000162e0: 2020 2020 2020 2020 2020 7363 6865 6d65            scheme
-000162f0: 3a20 4854 5450 530a 2020 2020 2020 2020  : HTTPS.        
-00016300: 2020 2020 2020 706f 7274 3a20 3838 3838        port: 8888
-00016310: 0a20 2020 2020 2020 2020 2020 2020 2068  .              h
-00016320: 6f73 743a 2067 7373 2d64 6e73 2d61 6765  ost: gss-dns-age
-00016330: 6e74 2e65 7861 6d70 6c65 2e6f 7267 0a20  nt.example.org. 
-00016340: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
-00016350: 7574 5f73 6563 6f6e 6473 3a20 3630 0a20  ut_seconds: 60. 
-00016360: 2020 2020 2020 2020 2020 2065 7865 635f             exec_
-00016370: 636f 6d6d 616e 643a 0a20 2020 2020 2020  command:.       
-00016380: 2020 2020 202d 202f 6773 732f 6469 6e67       - /gss/ding
-00016390: 6d61 6e2f 6269 6e2f 6469 6e67 6d61 6e2d  man/bin/dingman-
-000163a0: 636c 6974 0a20 2020 2020 2020 2020 2020  clit.           
-000163b0: 202d 202d 6164 6472 6573 730a 2020 2020   - -address.    
-000163c0: 2020 2020 2020 2020 2d20 3132 372e 302e          - 127.0.
-000163d0: 302e 313a 3330 3530 310a 2020 2020 2020  0.1:30501.      
-000163e0: 2020 2020 2020 2d20 2d63 6f6d 6d61 6e64        - -command
-000163f0: 0a20 2020 2020 2020 2020 2020 202d 2073  .            - s
-00016400: 686f 7720 706f 703a 616c 6c20 7375 6d6d  how pop:all summ
-00016410: 6172 793a 6865 616c 7468 2d73 7461 7475  ary:health-statu
-00016420: 730a 2020 2020 2020 2020 2020 656e 765f  s.          env_
-00016430: 6672 6f6d 3a20 5265 6775 6c61 720a 2020  from: Regular.  
-00016440: 2020 2020 2020 2020 7374 6172 7475 705f          startup_
-00016450: 7072 6f62 653a 0a20 2020 2020 2020 2020  probe:.         
-00016460: 2020 2070 6572 696f 645f 7365 636f 6e64     period_second
-00016470: 733a 2036 300a 2020 2020 2020 2020 2020  s: 60.          
-00016480: 2020 696e 6974 6961 6c5f 6465 6c61 795f    initial_delay_
-00016490: 7365 636f 6e64 733a 2036 3030 0a20 2020  seconds: 600.   
-000164a0: 2020 2020 2020 2020 2074 6370 5f73 6f63           tcp_soc
-000164b0: 6b65 743a 0a20 2020 2020 2020 2020 2020  ket:.           
-000164c0: 2020 2070 6f72 743a 2033 3031 3831 0a20     port: 30181. 
-000164d0: 2020 2020 2020 2020 2020 2020 2068 6f73               hos
-000164e0: 743a 2031 3237 2e30 2e30 2e31 0a20 2020  t: 127.0.0.1.   
-000164f0: 2020 2020 2020 2020 2066 6169 6c75 7265           failure
-00016500: 5f74 6872 6573 686f 6c64 3a20 330a 2020  _threshold: 3.  
-00016510: 2020 2020 2020 2020 2020 6874 7470 5f67            http_g
-00016520: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-00016530: 2020 7061 7468 3a20 2f73 686f 773f 646f    path: /show?do
-00016540: 6d61 696e 3d76 3139 2e74 696b 746f 6b63  main=v19.tiktokc
-00016550: 646e 2e63 6f6d 0a20 2020 2020 2020 2020  dn.com.         
-00016560: 2020 2020 2068 7474 705f 6865 6164 6572       http_header
-00016570: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00016580: 202d 2078 2d64 6576 7372 652d 6175 7468   - x-devsre-auth
-00016590: 6f72 697a 6174 696f 6e3a 4265 6172 6572  orization:Bearer
-000165a0: 2065 794a 6862 4763 694f 694a 0a20 2020   eyJhbGciOiJ.   
-000165b0: 2020 2020 2020 2020 2020 202d 2063 6f6e             - con
-000165c0: 7465 6e74 2d74 7970 653a 6170 706c 6963  tent-type:applic
-000165d0: 6174 696f 6e2f 6a73 6f6e 0a20 2020 2020  ation/json.     
-000165e0: 2020 2020 2020 2020 2073 6368 656d 653a           scheme:
-000165f0: 2048 5454 5053 0a20 2020 2020 2020 2020   HTTPS.         
-00016600: 2020 2020 2070 6f72 743a 2038 3838 380a       port: 8888.
-00016610: 2020 2020 2020 2020 2020 2020 2020 686f                ho
-00016620: 7374 3a20 6773 732d 646e 732d 6167 656e  st: gss-dns-agen
-00016630: 742e 6578 616d 706c 652e 6f72 670a 2020  t.example.org.  
-00016640: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
-00016650: 745f 7365 636f 6e64 733a 2036 300a 2020  t_seconds: 60.  
-00016660: 2020 2020 2020 2020 2020 6578 6563 5f63            exec_c
-00016670: 6f6d 6d61 6e64 3a0a 2020 2020 2020 2020  ommand:.        
-00016680: 2020 2020 2d20 2f67 7373 2f64 696e 676d      - /gss/dingm
-00016690: 616e 2f62 696e 2f64 696e 676d 616e 2d63  an/bin/dingman-c
-000166a0: 6c69 740a 2020 2020 2020 2020 2020 2020  lit.            
-000166b0: 2d20 2d61 6464 7265 7373 0a20 2020 2020  - -address.     
-000166c0: 2020 2020 2020 202d 2031 3237 2e30 2e30         - 127.0.0
-000166d0: 2e31 3a33 3035 3031 0a20 2020 2020 2020  .1:30501.       
-000166e0: 2020 2020 202d 202d 636f 6d6d 616e 640a       - -command.
-000166f0: 2020 2020 2020 2020 2020 2020 2d20 7368              - sh
-00016700: 6f77 2070 6f70 3a61 6c6c 2073 756d 6d61  ow pop:all summa
-00016710: 7279 3a68 6561 6c74 682d 7374 6174 7573  ry:health-status
-00016720: 0a20 2020 2020 2020 2020 2069 6d61 6765  .          image
-00016730: 5f70 756c 6c5f 706f 6c69 6379 3a20 4966  _pull_policy: If
-00016740: 4e6f 7450 7265 7365 6e74 0a20 2020 2020  NotPresent.     
-00016750: 2020 2020 2076 6f6c 756d 655f 6465 7669       volume_devi
-00016760: 6365 733a 0a20 2020 2020 2020 2020 202d  ces:.          -
-00016770: 206e 616d 653a 2064 656d 6f2d 766f 6c0a   name: demo-vol.
-00016780: 2020 2020 2020 2020 2020 2020 6465 7669              devi
-00016790: 6365 5f70 6174 683a 202f 6465 762f 7364  ce_path: /dev/sd
-000167a0: 6131 0a20 2020 2020 2020 2020 2020 2062  a1.            b
-000167b0: 6361 6368 655f 6e75 6d73 3a20 340a 2020  cache_nums: 4.  
-000167c0: 2020 2020 2020 2020 2d20 6e61 6d65 3a20          - name: 
-000167d0: 6465 6d6f 2d76 6f6c 0a20 2020 2020 2020  demo-vol.       
-000167e0: 2020 2020 2064 6576 6963 655f 7061 7468       device_path
-000167f0: 3a20 2f64 6576 2f73 6461 310a 2020 2020  : /dev/sda1.    
-00016800: 2020 2020 2020 2020 6263 6163 6865 5f6e          bcache_n
-00016810: 756d 733a 2034 0a20 2020 2020 2020 2020  ums: 4.         
-00016820: 206e 616d 653a 2068 7474 702d 7365 7276   name: http-serv
-00016830: 6572 0a20 2020 2020 2020 2020 2063 6f6e  er.          con
-00016840: 7461 696e 6572 5f74 7970 653a 2049 6e69  tainer_type: Ini
-00016850: 740a 2020 2020 2020 2020 2020 6c69 7665  t.          live
-00016860: 6e65 7373 5f70 726f 6265 3a0a 2020 2020  ness_probe:.    
-00016870: 2020 2020 2020 2020 7065 7269 6f64 5f73          period_s
-00016880: 6563 6f6e 6473 3a20 3630 0a20 2020 2020  econds: 60.     
-00016890: 2020 2020 2020 2069 6e69 7469 616c 5f64         initial_d
-000168a0: 656c 6179 5f73 6563 6f6e 6473 3a20 3630  elay_seconds: 60
-000168b0: 300a 2020 2020 2020 2020 2020 2020 7463  0.            tc
-000168c0: 705f 736f 636b 6574 3a0a 2020 2020 2020  p_socket:.      
-000168d0: 2020 2020 2020 2020 706f 7274 3a20 3330          port: 30
-000168e0: 3138 310a 2020 2020 2020 2020 2020 2020  181.            
-000168f0: 2020 686f 7374 3a20 3132 372e 302e 302e    host: 127.0.0.
-00016900: 310a 2020 2020 2020 2020 2020 2020 6661  1.            fa
-00016910: 696c 7572 655f 7468 7265 7368 6f6c 643a  ilure_threshold:
-00016920: 2033 0a20 2020 2020 2020 2020 2020 2068   3.            h
-00016930: 7474 705f 6765 743a 0a20 2020 2020 2020  ttp_get:.       
-00016940: 2020 2020 2020 2070 6174 683a 202f 7368         path: /sh
-00016950: 6f77 3f64 6f6d 6169 6e3d 7631 392e 7469  ow?domain=v19.ti
-00016960: 6b74 6f6b 6364 6e2e 636f 6d0a 2020 2020  ktokcdn.com.    
-00016970: 2020 2020 2020 2020 2020 6874 7470 5f68            http_h
-00016980: 6561 6465 7273 3a0a 2020 2020 2020 2020  eaders:.        
-00016990: 2020 2020 2020 2d20 782d 6465 7673 7265        - x-devsre
-000169a0: 2d61 7574 686f 7269 7a61 7469 6f6e 3a42  -authorization:B
-000169b0: 6561 7265 7220 6579 4a68 6247 6369 4f69  earer eyJhbGciOi
-000169c0: 4a0a 2020 2020 2020 2020 2020 2020 2020  J.              
-000169d0: 2d20 636f 6e74 656e 742d 7479 7065 3a61  - content-type:a
-000169e0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e0a  pplication/json.
-000169f0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00016a00: 6865 6d65 3a20 4854 5450 530a 2020 2020  heme: HTTPS.    
-00016a10: 2020 2020 2020 2020 2020 706f 7274 3a20            port: 
-00016a20: 3838 3838 0a20 2020 2020 2020 2020 2020  8888.           
-00016a30: 2020 2068 6f73 743a 2067 7373 2d64 6e73     host: gss-dns
-00016a40: 2d61 6765 6e74 2e65 7861 6d70 6c65 2e6f  -agent.example.o
-00016a50: 7267 0a20 2020 2020 2020 2020 2020 2074  rg.            t
-00016a60: 696d 656f 7574 5f73 6563 6f6e 6473 3a20  imeout_seconds: 
-00016a70: 3630 0a20 2020 2020 2020 2020 2020 2065  60.            e
-00016a80: 7865 635f 636f 6d6d 616e 643a 0a20 2020  xec_command:.   
-00016a90: 2020 2020 2020 2020 202d 202f 6773 732f           - /gss/
-00016aa0: 6469 6e67 6d61 6e2f 6269 6e2f 6469 6e67  dingman/bin/ding
-00016ab0: 6d61 6e2d 636c 6974 0a20 2020 2020 2020  man-clit.       
-00016ac0: 2020 2020 202d 202d 6164 6472 6573 730a       - -address.
-00016ad0: 2020 2020 2020 2020 2020 2020 2d20 3132              - 12
-00016ae0: 372e 302e 302e 313a 3330 3530 310a 2020  7.0.0.1:30501.  
-00016af0: 2020 2020 2020 2020 2020 2d20 2d63 6f6d            - -com
-00016b00: 6d61 6e64 0a20 2020 2020 2020 2020 2020  mand.           
-00016b10: 202d 2073 686f 7720 706f 703a 616c 6c20   - show pop:all 
-00016b20: 7375 6d6d 6172 793a 6865 616c 7468 2d73  summary:health-s
-00016b30: 7461 7475 730a 2020 2020 2020 2020 2020  tatus.          
-00016b40: 7365 6375 7269 7479 5f63 6f6e 7465 7874  security_context
-00016b50: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
-00016b60: 7061 6269 6c69 7469 6573 3a0a 2020 2020  pabilities:.    
-00016b70: 2020 2020 2020 2020 2020 6164 643a 0a20            add:. 
-00016b80: 2020 2020 2020 2020 2020 2020 202d 204e               - N
-00016b90: 4554 5f41 444d 494e 0a20 2020 2020 2020  ET_ADMIN.       
-00016ba0: 2020 2020 2020 202d 2053 5953 5f54 494d         - SYS_TIM
-00016bb0: 450a 2020 2020 2020 2020 2020 2020 2020  E.              
-00016bc0: 6472 6f70 3a0a 2020 2020 2020 2020 2020  drop:.          
-00016bd0: 2020 2020 2d20 4e45 545f 4144 4d49 4e0a      - NET_ADMIN.
-00016be0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00016bf0: 5359 535f 5449 4d45 0a20 2020 2020 2020  SYS_TIME.       
-00016c00: 2020 2020 2072 756e 5f61 735f 6772 6f75       run_as_grou
-00016c10: 703a 2033 3030 300a 2020 2020 2020 2020  p: 3000.        
-00016c20: 2020 2020 7275 6e5f 6173 5f75 7365 723a      run_as_user:
-00016c30: 2031 3030 300a 2020 2020 2020 2020 2d20   1000.        - 
-00016c40: 696d 6167 653a 206e 6769 6e78 3a6c 6174  image: nginx:lat
-00016c50: 6573 740a 2020 2020 2020 2020 2020 6c69  est.          li
-00016c60: 6665 5f63 7963 6c65 3a0a 2020 2020 2020  fe_cycle:.      
-00016c70: 2020 2020 2020 7072 655f 7374 6f70 3a0a        pre_stop:.
-00016c80: 2020 2020 2020 2020 2020 2020 2020 7463                tc
-00016c90: 705f 736f 636b 6574 3a0a 2020 2020 2020  p_socket:.      
-00016ca0: 2020 2020 2020 2020 2020 706f 7274 3a20            port: 
-00016cb0: 3330 3138 310a 2020 2020 2020 2020 2020  30181.          
-00016cc0: 2020 2020 2020 686f 7374 3a20 3132 372e        host: 127.
-00016cd0: 302e 302e 310a 2020 2020 2020 2020 2020  0.0.1.          
-00016ce0: 2020 2020 6874 7470 5f67 6574 3a0a 2020      http_get:.  
-00016cf0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00016d00: 7468 3a20 2f73 686f 773f 646f 6d61 696e  th: /show?domain
-00016d10: 3d76 3139 2e74 696b 746f 6b63 646e 2e63  =v19.tiktokcdn.c
-00016d20: 6f6d 0a20 2020 2020 2020 2020 2020 2020  om.             
-00016d30: 2020 2068 7474 705f 6865 6164 6572 733a     http_headers:
-00016d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016d50: 202d 2078 2d64 6576 7372 652d 6175 7468   - x-devsre-auth
-00016d60: 6f72 697a 6174 696f 6e3a 4265 6172 6572  orization:Bearer
-00016d70: 2065 794a 6862 4763 694f 694a 0a20 2020   eyJhbGciOiJ.   
-00016d80: 2020 2020 2020 2020 2020 2020 202d 2063               - c
-00016d90: 6f6e 7465 6e74 2d74 7970 653a 6170 706c  ontent-type:appl
-00016da0: 6963 6174 696f 6e2f 6a73 6f6e 0a20 2020  ication/json.   
-00016db0: 2020 2020 2020 2020 2020 2020 2073 6368               sch
-00016dc0: 656d 653a 2048 5454 5053 0a20 2020 2020  eme: HTTPS.     
-00016dd0: 2020 2020 2020 2020 2020 2070 6f72 743a             port:
-00016de0: 2038 3838 380a 2020 2020 2020 2020 2020   8888.          
-00016df0: 2020 2020 2020 686f 7374 3a20 6773 732d        host: gss-
-00016e00: 646e 732d 6167 656e 742e 6578 616d 706c  dns-agent.exampl
-00016e10: 652e 6f72 670a 2020 2020 2020 2020 2020  e.org.          
-00016e20: 2020 2020 6578 6563 5f63 6f6d 6d61 6e64      exec_command
-00016e30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016e40: 2d20 2f62 696e 2f73 686f 7764 6f77 6e2e  - /bin/showdown.
-00016e50: 7368 0a20 2020 2020 2020 2020 2020 2070  sh.            p
-00016e60: 6f73 745f 7374 6172 743a 0a20 2020 2020  ost_start:.     
-00016e70: 2020 2020 2020 2020 2074 6370 5f73 6f63           tcp_soc
-00016e80: 6b65 743a 0a20 2020 2020 2020 2020 2020  ket:.           
-00016e90: 2020 2020 2070 6f72 743a 2033 3031 3831       port: 30181
-00016ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016eb0: 2068 6f73 743a 2031 3237 2e30 2e30 2e31   host: 127.0.0.1
-00016ec0: 0a20 2020 2020 2020 2020 2020 2020 2068  .              h
-00016ed0: 7474 705f 6765 743a 0a20 2020 2020 2020  ttp_get:.       
-00016ee0: 2020 2020 2020 2020 2070 6174 683a 202f           path: /
-00016ef0: 7368 6f77 3f64 6f6d 6169 6e3d 7631 392e  show?domain=v19.
-00016f00: 7469 6b74 6f6b 6364 6e2e 636f 6d0a 2020  tiktokcdn.com.  
-00016f10: 2020 2020 2020 2020 2020 2020 2020 6874                ht
-00016f20: 7470 5f68 6561 6465 7273 3a0a 2020 2020  tp_headers:.    
-00016f30: 2020 2020 2020 2020 2020 2020 2d20 782d              - x-
-00016f40: 6465 7673 7265 2d61 7574 686f 7269 7a61  devsre-authoriza
-00016f50: 7469 6f6e 3a42 6561 7265 7220 6579 4a68  tion:Bearer eyJh
-00016f60: 6247 6369 4f69 4a0a 2020 2020 2020 2020  bGciOiJ.        
-00016f70: 2020 2020 2020 2020 2d20 636f 6e74 656e          - conten
-00016f80: 742d 7479 7065 3a61 7070 6c69 6361 7469  t-type:applicati
-00016f90: 6f6e 2f6a 736f 6e0a 2020 2020 2020 2020  on/json.        
-00016fa0: 2020 2020 2020 2020 7363 6865 6d65 3a20          scheme: 
-00016fb0: 4854 5450 530a 2020 2020 2020 2020 2020  HTTPS.          
-00016fc0: 2020 2020 2020 706f 7274 3a20 3838 3838        port: 8888
-00016fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016fe0: 2068 6f73 743a 2067 7373 2d64 6e73 2d61   host: gss-dns-a
-00016ff0: 6765 6e74 2e65 7861 6d70 6c65 2e6f 7267  gent.example.org
-00017000: 0a20 2020 2020 2020 2020 2020 2020 2065  .              e
-00017010: 7865 635f 636f 6d6d 616e 643a 0a20 2020  xec_command:.   
-00017020: 2020 2020 2020 2020 2020 202d 202f 6269             - /bi
-00017030: 6e2f 7368 6f77 646f 776e 2e73 680a 2020  n/showdown.sh.  
-00017040: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-00017050: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-00017060: 6571 7565 7374 733a 0a20 2020 2020 2020  equests:.       
-00017070: 2020 2020 2020 206d 656d 6f72 793a 2032         memory: 2
-00017080: 3536 4d69 0a20 2020 2020 2020 2020 2020  56Mi.           
-00017090: 2020 2063 7075 3a20 2230 2e31 220a 2020     cpu: "0.1".  
-000170a0: 2020 2020 2020 2020 2020 6c69 6d69 7473            limits
-000170b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000170c0: 6d65 6d6f 7279 3a20 3531 324d 690a 2020  memory: 512Mi.  
-000170d0: 2020 2020 2020 2020 2020 2020 6370 753a              cpu:
-000170e0: 2022 302e 3522 0a20 2020 2020 2020 2020   "0.5".         
-000170f0: 2076 6f6c 756d 655f 6d6f 756e 7473 3a0a   volume_mounts:.
-00017100: 2020 2020 2020 2020 2020 2d20 7061 7468            - path
-00017110: 3a20 2f6f 7074 2f73 6572 7665 722f 636f  : /opt/server/co
-00017120: 6e66 0a20 2020 2020 2020 2020 2020 2072  nf.            r
-00017130: 6561 645f 6f6e 6c79 3a20 7472 7565 0a20  ead_only: true. 
-00017140: 2020 2020 2020 2020 2020 206e 616d 653a             name:
-00017150: 2064 656d 6f2d 766f 6c0a 2020 2020 2020   demo-vol.      
-00017160: 2020 2020 2020 7375 625f 7061 7468 3a20        sub_path: 
-00017170: 7365 7276 6572 2e63 6f6e 660a 2020 2020  server.conf.    
-00017180: 2020 2020 2020 2d20 7061 7468 3a20 2f6f        - path: /o
-00017190: 7074 2f73 6572 7665 722f 636f 6e66 0a20  pt/server/conf. 
-000171a0: 2020 2020 2020 2020 2020 2072 6561 645f             read_
-000171b0: 6f6e 6c79 3a20 7472 7565 0a20 2020 2020  only: true.     
-000171c0: 2020 2020 2020 206e 616d 653a 2064 656d         name: dem
-000171d0: 6f2d 766f 6c0a 2020 2020 2020 2020 2020  o-vol.          
-000171e0: 2020 7375 625f 7061 7468 3a20 7365 7276    sub_path: serv
-000171f0: 6572 2e63 6f6e 660a 2020 2020 2020 2020  er.conf.        
-00017200: 2020 656e 763a 0a20 2020 2020 2020 2020    env:.         
-00017210: 2020 206e 616d 653a 2053 4d53 5f4b 4559     name: SMS_KEY
-00017220: 535f 5041 5448 5f58 4d0a 2020 2020 2020  S_PATH_XM.      
-00017230: 2020 2020 2020 7661 6c75 653a 2064 6d73        value: dms
-00017240: 2d73 6563 7265 740a 2020 2020 2020 2020  -secret.        
-00017250: 2020 706f 7274 733a 0a20 2020 2020 2020    ports:.       
-00017260: 2020 202d 2063 6f6e 7461 696e 6572 5f70     - container_p
-00017270: 6f72 743a 2038 300a 2020 2020 2020 2020  ort: 80.        
-00017280: 2020 2020 7072 6f74 6f63 6f6c 3a20 5443      protocol: TC
-00017290: 500a 2020 2020 2020 2020 2020 2020 6e61  P.            na
-000172a0: 6d65 3a20 6874 7470 0a20 2020 2020 2020  me: http.       
-000172b0: 2020 202d 2063 6f6e 7461 696e 6572 5f70     - container_p
-000172c0: 6f72 743a 2038 300a 2020 2020 2020 2020  ort: 80.        
-000172d0: 2020 2020 7072 6f74 6f63 6f6c 3a20 5443      protocol: TC
-000172e0: 500a 2020 2020 2020 2020 2020 2020 6e61  P.            na
-000172f0: 6d65 3a20 6874 7470 0a20 2020 2020 2020  me: http.       
-00017300: 2020 2063 6f6d 6d61 6e64 3a0a 2020 2020     command:.    
-00017310: 2020 2020 2020 2d20 7079 7468 6f6e 330a        - python3.
-00017320: 2020 2020 2020 2020 2020 6172 6773 3a0a            args:.
-00017330: 2020 2020 2020 2020 2020 2d20 2d6d 0a20            - -m. 
-00017340: 2020 2020 2020 2020 202d 206f 7065 6e61           - opena
-00017350: 7069 5f73 6572 7665 720a 2020 2020 2020  pi_server.      
-00017360: 2020 2020 7265 6164 696e 6573 735f 7072      readiness_pr
-00017370: 6f62 653a 0a20 2020 2020 2020 2020 2020  obe:.           
-00017380: 2070 6572 696f 645f 7365 636f 6e64 733a   period_seconds:
-00017390: 2036 300a 2020 2020 2020 2020 2020 2020   60.            
-000173a0: 696e 6974 6961 6c5f 6465 6c61 795f 7365  initial_delay_se
-000173b0: 636f 6e64 733a 2036 3030 0a20 2020 2020  conds: 600.     
-000173c0: 2020 2020 2020 2074 6370 5f73 6f63 6b65         tcp_socke
-000173d0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-000173e0: 2070 6f72 743a 2033 3031 3831 0a20 2020   port: 30181.   
-000173f0: 2020 2020 2020 2020 2020 2068 6f73 743a             host:
-00017400: 2031 3237 2e30 2e30 2e31 0a20 2020 2020   127.0.0.1.     
-00017410: 2020 2020 2020 2066 6169 6c75 7265 5f74         failure_t
-00017420: 6872 6573 686f 6c64 3a20 330a 2020 2020  hreshold: 3.    
-00017430: 2020 2020 2020 2020 6874 7470 5f67 6574          http_get
-00017440: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017450: 7061 7468 3a20 2f73 686f 773f 646f 6d61  path: /show?doma
-00017460: 696e 3d76 3139 2e74 696b 746f 6b63 646e  in=v19.tiktokcdn
-00017470: 2e63 6f6d 0a20 2020 2020 2020 2020 2020  .com.           
-00017480: 2020 2068 7474 705f 6865 6164 6572 733a     http_headers:
-00017490: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
-000174a0: 2078 2d64 6576 7372 652d 6175 7468 6f72   x-devsre-author
-000174b0: 697a 6174 696f 6e3a 4265 6172 6572 2065  ization:Bearer e
-000174c0: 794a 6862 4763 694f 694a 0a20 2020 2020  yJhbGciOiJ.     
-000174d0: 2020 2020 2020 2020 202d 2063 6f6e 7465           - conte
-000174e0: 6e74 2d74 7970 653a 6170 706c 6963 6174  nt-type:applicat
-000174f0: 696f 6e2f 6a73 6f6e 0a20 2020 2020 2020  ion/json.       
-00017500: 2020 2020 2020 2073 6368 656d 653a 2048         scheme: H
-00017510: 5454 5053 0a20 2020 2020 2020 2020 2020  TTPS.           
-00017520: 2020 2070 6f72 743a 2038 3838 380a 2020     port: 8888.  
-00017530: 2020 2020 2020 2020 2020 2020 686f 7374              host
-00017540: 3a20 6773 732d 646e 732d 6167 656e 742e  : gss-dns-agent.
-00017550: 6578 616d 706c 652e 6f72 670a 2020 2020  example.org.    
-00017560: 2020 2020 2020 2020 7469 6d65 6f75 745f          timeout_
-00017570: 7365 636f 6e64 733a 2036 300a 2020 2020  seconds: 60.    
-00017580: 2020 2020 2020 2020 6578 6563 5f63 6f6d          exec_com
-00017590: 6d61 6e64 3a0a 2020 2020 2020 2020 2020  mand:.          
-000175a0: 2020 2d20 2f67 7373 2f64 696e 676d 616e    - /gss/dingman
-000175b0: 2f62 696e 2f64 696e 676d 616e 2d63 6c69  /bin/dingman-cli
-000175c0: 740a 2020 2020 2020 2020 2020 2020 2d20  t.            - 
-000175d0: 2d61 6464 7265 7373 0a20 2020 2020 2020  -address.       
-000175e0: 2020 2020 202d 2031 3237 2e30 2e30 2e31       - 127.0.0.1
-000175f0: 3a33 3035 3031 0a20 2020 2020 2020 2020  :30501.         
-00017600: 2020 202d 202d 636f 6d6d 616e 640a 2020     - -command.  
-00017610: 2020 2020 2020 2020 2020 2d20 7368 6f77            - show
-00017620: 2070 6f70 3a61 6c6c 2073 756d 6d61 7279   pop:all summary
-00017630: 3a68 6561 6c74 682d 7374 6174 7573 0a20  :health-status. 
-00017640: 2020 2020 2020 2020 2065 6e76 5f66 726f           env_fro
-00017650: 6d3a 2052 6567 756c 6172 0a20 2020 2020  m: Regular.     
-00017660: 2020 2020 2073 7461 7274 7570 5f70 726f       startup_pro
-00017670: 6265 3a0a 2020 2020 2020 2020 2020 2020  be:.            
-00017680: 7065 7269 6f64 5f73 6563 6f6e 6473 3a20  period_seconds: 
-00017690: 3630 0a20 2020 2020 2020 2020 2020 2069  60.            i
-000176a0: 6e69 7469 616c 5f64 656c 6179 5f73 6563  nitial_delay_sec
-000176b0: 6f6e 6473 3a20 3630 300a 2020 2020 2020  onds: 600.      
-000176c0: 2020 2020 2020 7463 705f 736f 636b 6574        tcp_socket
-000176d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000176e0: 706f 7274 3a20 3330 3138 310a 2020 2020  port: 30181.    
-000176f0: 2020 2020 2020 2020 2020 686f 7374 3a20            host: 
-00017700: 3132 372e 302e 302e 310a 2020 2020 2020  127.0.0.1.      
-00017710: 2020 2020 2020 6661 696c 7572 655f 7468        failure_th
-00017720: 7265 7368 6f6c 643a 2033 0a20 2020 2020  reshold: 3.     
-00017730: 2020 2020 2020 2068 7474 705f 6765 743a         http_get:
-00017740: 0a20 2020 2020 2020 2020 2020 2020 2070  .              p
-00017750: 6174 683a 202f 7368 6f77 3f64 6f6d 6169  ath: /show?domai
-00017760: 6e3d 7631 392e 7469 6b74 6f6b 6364 6e2e  n=v19.tiktokcdn.
-00017770: 636f 6d0a 2020 2020 2020 2020 2020 2020  com.            
-00017780: 2020 6874 7470 5f68 6561 6465 7273 3a0a    http_headers:.
-00017790: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-000177a0: 782d 6465 7673 7265 2d61 7574 686f 7269  x-devsre-authori
-000177b0: 7a61 7469 6f6e 3a42 6561 7265 7220 6579  zation:Bearer ey
-000177c0: 4a68 6247 6369 4f69 4a0a 2020 2020 2020  JhbGciOiJ.      
-000177d0: 2020 2020 2020 2020 2d20 636f 6e74 656e          - conten
-000177e0: 742d 7479 7065 3a61 7070 6c69 6361 7469  t-type:applicati
-000177f0: 6f6e 2f6a 736f 6e0a 2020 2020 2020 2020  on/json.        
-00017800: 2020 2020 2020 7363 6865 6d65 3a20 4854        scheme: HT
-00017810: 5450 530a 2020 2020 2020 2020 2020 2020  TPS.            
-00017820: 2020 706f 7274 3a20 3838 3838 0a20 2020    port: 8888.   
-00017830: 2020 2020 2020 2020 2020 2068 6f73 743a             host:
-00017840: 2067 7373 2d64 6e73 2d61 6765 6e74 2e65   gss-dns-agent.e
-00017850: 7861 6d70 6c65 2e6f 7267 0a20 2020 2020  xample.org.     
-00017860: 2020 2020 2020 2074 696d 656f 7574 5f73         timeout_s
-00017870: 6563 6f6e 6473 3a20 3630 0a20 2020 2020  econds: 60.     
-00017880: 2020 2020 2020 2065 7865 635f 636f 6d6d         exec_comm
-00017890: 616e 643a 0a20 2020 2020 2020 2020 2020  and:.           
-000178a0: 202d 202f 6773 732f 6469 6e67 6d61 6e2f   - /gss/dingman/
-000178b0: 6269 6e2f 6469 6e67 6d61 6e2d 636c 6974  bin/dingman-clit
-000178c0: 0a20 2020 2020 2020 2020 2020 202d 202d  .            - -
-000178d0: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
-000178e0: 2020 2020 2d20 3132 372e 302e 302e 313a      - 127.0.0.1:
-000178f0: 3330 3530 310a 2020 2020 2020 2020 2020  30501.          
-00017900: 2020 2d20 2d63 6f6d 6d61 6e64 0a20 2020    - -command.   
-00017910: 2020 2020 2020 2020 202d 2073 686f 7720           - show 
-00017920: 706f 703a 616c 6c20 7375 6d6d 6172 793a  pop:all summary:
-00017930: 6865 616c 7468 2d73 7461 7475 730a 2020  health-status.  
-00017940: 2020 2020 2020 2020 696d 6167 655f 7075          image_pu
-00017950: 6c6c 5f70 6f6c 6963 793a 2049 664e 6f74  ll_policy: IfNot
-00017960: 5072 6573 656e 740a 2020 2020 2020 2020  Present.        
-00017970: 2020 766f 6c75 6d65 5f64 6576 6963 6573    volume_devices
-00017980: 3a0a 2020 2020 2020 2020 2020 2d20 6e61  :.          - na
-00017990: 6d65 3a20 6465 6d6f 2d76 6f6c 0a20 2020  me: demo-vol.   
-000179a0: 2020 2020 2020 2020 2064 6576 6963 655f           device_
-000179b0: 7061 7468 3a20 2f64 6576 2f73 6461 310a  path: /dev/sda1.
-000179c0: 2020 2020 2020 2020 2020 2020 6263 6163              bcac
-000179d0: 6865 5f6e 756d 733a 2034 0a20 2020 2020  he_nums: 4.     
-000179e0: 2020 2020 202d 206e 616d 653a 2064 656d       - name: dem
-000179f0: 6f2d 766f 6c0a 2020 2020 2020 2020 2020  o-vol.          
-00017a00: 2020 6465 7669 6365 5f70 6174 683a 202f    device_path: /
-00017a10: 6465 762f 7364 6131 0a20 2020 2020 2020  dev/sda1.       
-00017a20: 2020 2020 2062 6361 6368 655f 6e75 6d73       bcache_nums
-00017a30: 3a20 340a 2020 2020 2020 2020 2020 6e61  : 4.          na
-00017a40: 6d65 3a20 6874 7470 2d73 6572 7665 720a  me: http-server.
-00017a50: 2020 2020 2020 2020 2020 636f 6e74 6169            contai
-00017a60: 6e65 725f 7479 7065 3a20 496e 6974 0a20  ner_type: Init. 
-00017a70: 2020 2020 2020 2020 206c 6976 656e 6573           livenes
-00017a80: 735f 7072 6f62 653a 0a20 2020 2020 2020  s_probe:.       
-00017a90: 2020 2020 2070 6572 696f 645f 7365 636f       period_seco
-00017aa0: 6e64 733a 2036 300a 2020 2020 2020 2020  nds: 60.        
-00017ab0: 2020 2020 696e 6974 6961 6c5f 6465 6c61      initial_dela
-00017ac0: 795f 7365 636f 6e64 733a 2036 3030 0a20  y_seconds: 600. 
-00017ad0: 2020 2020 2020 2020 2020 2074 6370 5f73             tcp_s
-00017ae0: 6f63 6b65 743a 0a20 2020 2020 2020 2020  ocket:.         
-00017af0: 2020 2020 2070 6f72 743a 2033 3031 3831       port: 30181
-00017b00: 0a20 2020 2020 2020 2020 2020 2020 2068  .              h
-00017b10: 6f73 743a 2031 3237 2e30 2e30 2e31 0a20  ost: 127.0.0.1. 
-00017b20: 2020 2020 2020 2020 2020 2066 6169 6c75             failu
-00017b30: 7265 5f74 6872 6573 686f 6c64 3a20 330a  re_threshold: 3.
-00017b40: 2020 2020 2020 2020 2020 2020 6874 7470              http
-00017b50: 5f67 6574 3a0a 2020 2020 2020 2020 2020  _get:.          
-00017b60: 2020 2020 7061 7468 3a20 2f73 686f 773f      path: /show?
-00017b70: 646f 6d61 696e 3d76 3139 2e74 696b 746f  domain=v19.tikto
-00017b80: 6b63 646e 2e63 6f6d 0a20 2020 2020 2020  kcdn.com.       
-00017b90: 2020 2020 2020 2068 7474 705f 6865 6164         http_head
-00017ba0: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
-00017bb0: 2020 202d 2078 2d64 6576 7372 652d 6175     - x-devsre-au
-00017bc0: 7468 6f72 697a 6174 696f 6e3a 4265 6172  thorization:Bear
-00017bd0: 6572 2065 794a 6862 4763 694f 694a 0a20  er eyJhbGciOiJ. 
-00017be0: 2020 2020 2020 2020 2020 2020 202d 2063               - c
-00017bf0: 6f6e 7465 6e74 2d74 7970 653a 6170 706c  ontent-type:appl
-00017c00: 6963 6174 696f 6e2f 6a73 6f6e 0a20 2020  ication/json.   
-00017c10: 2020 2020 2020 2020 2020 2073 6368 656d             schem
-00017c20: 653a 2048 5454 5053 0a20 2020 2020 2020  e: HTTPS.       
-00017c30: 2020 2020 2020 2070 6f72 743a 2038 3838         port: 888
-00017c40: 380a 2020 2020 2020 2020 2020 2020 2020  8.              
-00017c50: 686f 7374 3a20 6773 732d 646e 732d 6167  host: gss-dns-ag
-00017c60: 656e 742e 6578 616d 706c 652e 6f72 670a  ent.example.org.
-00017c70: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00017c80: 6f75 745f 7365 636f 6e64 733a 2036 300a  out_seconds: 60.
-00017c90: 2020 2020 2020 2020 2020 2020 6578 6563              exec
-00017ca0: 5f63 6f6d 6d61 6e64 3a0a 2020 2020 2020  _command:.      
-00017cb0: 2020 2020 2020 2d20 2f67 7373 2f64 696e        - /gss/din
-00017cc0: 676d 616e 2f62 696e 2f64 696e 676d 616e  gman/bin/dingman
-00017cd0: 2d63 6c69 740a 2020 2020 2020 2020 2020  -clit.          
-00017ce0: 2020 2d20 2d61 6464 7265 7373 0a20 2020    - -address.   
-00017cf0: 2020 2020 2020 2020 202d 2031 3237 2e30           - 127.0
-00017d00: 2e30 2e31 3a33 3035 3031 0a20 2020 2020  .0.1:30501.     
-00017d10: 2020 2020 2020 202d 202d 636f 6d6d 616e         - -comman
-00017d20: 640a 2020 2020 2020 2020 2020 2020 2d20  d.            - 
-00017d30: 7368 6f77 2070 6f70 3a61 6c6c 2073 756d  show pop:all sum
-00017d40: 6d61 7279 3a68 6561 6c74 682d 7374 6174  mary:health-stat
-00017d50: 7573 0a20 2020 2020 2020 2020 2073 6563  us.          sec
-00017d60: 7572 6974 795f 636f 6e74 6578 743a 0a20  urity_context:. 
-00017d70: 2020 2020 2020 2020 2020 2063 6170 6162             capab
-00017d80: 696c 6974 6965 733a 0a20 2020 2020 2020  ilities:.       
-00017d90: 2020 2020 2020 2061 6464 3a0a 2020 2020         add:.    
-00017da0: 2020 2020 2020 2020 2020 2d20 4e45 545f            - NET_
-00017db0: 4144 4d49 4e0a 2020 2020 2020 2020 2020  ADMIN.          
-00017dc0: 2020 2020 2d20 5359 535f 5449 4d45 0a20      - SYS_TIME. 
-00017dd0: 2020 2020 2020 2020 2020 2020 2064 726f               dro
-00017de0: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-00017df0: 202d 204e 4554 5f41 444d 494e 0a20 2020   - NET_ADMIN.   
-00017e00: 2020 2020 2020 2020 2020 202d 2053 5953             - SYS
-00017e10: 5f54 494d 450a 2020 2020 2020 2020 2020  _TIME.          
-00017e20: 2020 7275 6e5f 6173 5f67 726f 7570 3a20    run_as_group: 
-00017e30: 3330 3030 0a20 2020 2020 2020 2020 2020  3000.           
-00017e40: 2072 756e 5f61 735f 7573 6572 3a20 3130   run_as_user: 10
-00017e50: 3030 0a20 2020 2020 2020 206c 6162 656c  00.        label
-00017e60: 733a 0a20 2020 2020 2020 202d 2061 7070  s:.        - app
-00017e70: 3a64 656d 6f2d 6170 700a 2020 2020 2020  :demo-app.      
-00017e80: 2020 2d20 7665 7273 696f 6e3a 7631 2e30    - version:v1.0
-00017e90: 2e30 0a20 2020 2020 2020 2061 6666 696e  .0.        affin
-00017ea0: 6974 793a 0a20 2020 2020 2020 2020 2070  ity:.          p
-00017eb0: 6f64 5f61 6e74 695f 6166 6669 6e69 7479  od_anti_affinity
-00017ec0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00017ed0: 6566 6572 7265 645f 6475 7269 6e67 5f73  eferred_during_s
-00017ee0: 6368 6564 756c 696e 675f 6967 6e6f 7265  cheduling_ignore
-00017ef0: 645f 6475 7269 6e67 5f65 7865 6375 7469  d_during_executi
-00017f00: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-00017f10: 2d20 7765 6967 6874 3a20 360a 2020 2020  - weight: 6.    
-00017f20: 2020 2020 2020 2020 2020 706f 645f 6166            pod_af
-00017f30: 6669 6e69 7479 5f74 6572 6d3a 0a20 2020  finity_term:.   
-00017f40: 2020 2020 2020 2020 2020 2020 206c 6162               lab
-00017f50: 656c 5f73 656c 6563 746f 723a 0a20 2020  el_selector:.   
-00017f60: 2020 2020 2020 2020 2020 2020 202d 2061               - a
-00017f70: 7070 3a64 656d 6f2d 6170 700a 2020 2020  pp:demo-app.    
-00017f80: 2020 2020 2020 2020 2020 2020 2d20 226b              - "k
-00017f90: 6579 3a76 6572 7369 6f6e 2c20 6f70 6572  ey:version, oper
-00017fa0: 6174 6f72 3a49 6e2c 2076 616c 7565 733a  ator:In, values:
-00017fb0: 5b76 312e 302e 302c 2076 312e 302e 315d  [v1.0.0, v1.0.1]
-00017fc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00017fd0: 2020 746f 706f 6c6f 6779 5f6b 6579 3a20    topology_key: 
-00017fe0: 746f 706f 6c6f 6779 5f6b 6579 0a20 2020  topology_key.   
-00017ff0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00018000: 6573 7061 6365 733a 0a20 2020 2020 2020  espaces:.       
-00018010: 2020 2020 2020 2020 202d 206e 616d 6573           - names
-00018020: 7061 6365 730a 2020 2020 2020 2020 2020  paces.          
-00018030: 2020 2020 2020 2d20 6e61 6d65 7370 6163        - namespac
-00018040: 6573 0a20 2020 2020 2020 2020 2020 202d  es.            -
-00018050: 2077 6569 6768 743a 2036 0a20 2020 2020   weight: 6.     
-00018060: 2020 2020 2020 2020 2070 6f64 5f61 6666           pod_aff
-00018070: 696e 6974 795f 7465 726d 3a0a 2020 2020  inity_term:.    
-00018080: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00018090: 6c5f 7365 6c65 6374 6f72 3a0a 2020 2020  l_selector:.    
-000180a0: 2020 2020 2020 2020 2020 2020 2d20 6170              - ap
-000180b0: 703a 6465 6d6f 2d61 7070 0a20 2020 2020  p:demo-app.     
-000180c0: 2020 2020 2020 2020 2020 202d 2022 6b65             - "ke
-000180d0: 793a 7665 7273 696f 6e2c 206f 7065 7261  y:version, opera
-000180e0: 746f 723a 496e 2c20 7661 6c75 6573 3a5b  tor:In, values:[
-000180f0: 7631 2e30 2e30 2c20 7631 2e30 2e31 5d22  v1.0.0, v1.0.1]"
-00018100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018110: 2074 6f70 6f6c 6f67 795f 6b65 793a 2074   topology_key: t
-00018120: 6f70 6f6c 6f67 795f 6b65 790a 2020 2020  opology_key.    
-00018130: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00018140: 7370 6163 6573 3a0a 2020 2020 2020 2020  spaces:.        
-00018150: 2020 2020 2020 2020 2d20 6e61 6d65 7370          - namesp
-00018160: 6163 6573 0a20 2020 2020 2020 2020 2020  aces.           
-00018170: 2020 2020 202d 206e 616d 6573 7061 6365       - namespace
-00018180: 730a 2020 2020 2020 2020 2020 2020 7265  s.            re
-00018190: 7175 6972 6564 5f64 7572 696e 675f 7363  quired_during_sc
-000181a0: 6865 6475 6c69 6e67 5f69 676e 6f72 6564  heduling_ignored
-000181b0: 5f64 7572 696e 675f 6578 6563 7574 696f  _during_executio
-000181c0: 6e3a 0a20 2020 2020 2020 2020 2020 202d  n:.            -
-000181d0: 206c 6162 656c 5f73 656c 6563 746f 723a   label_selector:
-000181e0: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
-000181f0: 2061 7070 3a64 656d 6f2d 6170 700a 2020   app:demo-app.  
-00018200: 2020 2020 2020 2020 2020 2020 2d20 226b              - "k
-00018210: 6579 3a76 6572 7369 6f6e 2c20 6f70 6572  ey:version, oper
-00018220: 6174 6f72 3a49 6e2c 2076 616c 7565 733a  ator:In, values:
-00018230: 5b76 312e 302e 302c 2076 312e 302e 315d  [v1.0.0, v1.0.1]
-00018240: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00018250: 746f 706f 6c6f 6779 5f6b 6579 3a20 746f  topology_key: to
-00018260: 706f 6c6f 6779 5f6b 6579 0a20 2020 2020  pology_key.     
-00018270: 2020 2020 2020 2020 206e 616d 6573 7061           namespa
-00018280: 6365 733a 0a20 2020 2020 2020 2020 2020  ces:.           
-00018290: 2020 202d 206e 616d 6573 7061 6365 730a     - namespaces.
-000182a0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-000182b0: 6e61 6d65 7370 6163 6573 0a20 2020 2020  namespaces.     
-000182c0: 2020 2020 2020 202d 206c 6162 656c 5f73         - label_s
-000182d0: 656c 6563 746f 723a 0a20 2020 2020 2020  elector:.       
-000182e0: 2020 2020 2020 202d 2061 7070 3a64 656d         - app:dem
-000182f0: 6f2d 6170 700a 2020 2020 2020 2020 2020  o-app.          
-00018300: 2020 2020 2d20 226b 6579 3a76 6572 7369      - "key:versi
-00018310: 6f6e 2c20 6f70 6572 6174 6f72 3a49 6e2c  on, operator:In,
-00018320: 2076 616c 7565 733a 5b76 312e 302e 302c   values:[v1.0.0,
-00018330: 2076 312e 302e 315d 220a 2020 2020 2020   v1.0.1]".      
-00018340: 2020 2020 2020 2020 746f 706f 6c6f 6779          topology
-00018350: 5f6b 6579 3a20 746f 706f 6c6f 6779 5f6b  _key: topology_k
-00018360: 6579 0a20 2020 2020 2020 2020 2020 2020  ey.             
-00018370: 206e 616d 6573 7061 6365 733a 0a20 2020   namespaces:.   
-00018380: 2020 2020 2020 2020 2020 202d 206e 616d             - nam
-00018390: 6573 7061 6365 730a 2020 2020 2020 2020  espaces.        
-000183a0: 2020 2020 2020 2d20 6e61 6d65 7370 6163        - namespac
-000183b0: 6573 0a20 2020 2020 2020 2020 206e 6f64  es.          nod
-000183c0: 655f 6166 6669 6e69 7479 3a0a 2020 2020  e_affinity:.    
-000183d0: 2020 2020 2020 2020 7072 6566 6572 7265          preferre
-000183e0: 645f 6475 7269 6e67 5f73 6368 6564 756c  d_during_schedul
-000183f0: 696e 675f 6967 6e6f 7265 645f 6475 7269  ing_ignored_duri
-00018400: 6e67 5f65 7865 6375 7469 6f6e 3a0a 2020  ng_execution:.  
-00018410: 2020 2020 2020 2020 2020 2d20 7072 6566            - pref
-00018420: 6572 656e 6365 3a0a 2020 2020 2020 2020  erence:.        
-00018430: 2020 2020 2020 2020 6d61 7463 685f 6578          match_ex
-00018440: 7072 6573 7369 6f6e 733a 0a20 2020 2020  pressions:.     
-00018450: 2020 2020 2020 2020 2020 202d 2022 6b65             - "ke
-00018460: 793a 7665 7273 696f 6e2c 206f 7065 7261  y:version, opera
-00018470: 746f 723a 496e 2c20 7661 6c75 6573 3a5b  tor:In, values:[
-00018480: 7631 2e30 2e30 2c20 7631 2e30 2e31 5d22  v1.0.0, v1.0.1]"
-00018490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000184a0: 206d 6174 6368 5f66 6965 6c64 733a 0a20   match_fields:. 
-000184b0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-000184c0: 2022 6b65 793a 7665 7273 696f 6e2c 206f   "key:version, o
-000184d0: 7065 7261 746f 723a 496e 2c20 7661 6c75  perator:In, valu
-000184e0: 6573 3a5b 7631 2e30 2e30 2c20 7631 2e30  es:[v1.0.0, v1.0
-000184f0: 2e31 5d22 0a20 2020 2020 2020 2020 2020  .1]".           
-00018500: 2020 2077 6569 6768 743a 2030 0a20 2020     weight: 0.   
-00018510: 2020 2020 2020 2020 202d 2070 7265 6665           - prefe
-00018520: 7265 6e63 653a 0a20 2020 2020 2020 2020  rence:.         
-00018530: 2020 2020 2020 206d 6174 6368 5f65 7870         match_exp
-00018540: 7265 7373 696f 6e73 3a0a 2020 2020 2020  ressions:.      
-00018550: 2020 2020 2020 2020 2020 2d20 226b 6579            - "key
-00018560: 3a76 6572 7369 6f6e 2c20 6f70 6572 6174  :version, operat
-00018570: 6f72 3a49 6e2c 2076 616c 7565 733a 5b76  or:In, values:[v
-00018580: 312e 302e 302c 2076 312e 302e 315d 220a  1.0.0, v1.0.1]".
-00018590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185a0: 6d61 7463 685f 6669 656c 6473 3a0a 2020  match_fields:.  
-000185b0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-000185c0: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
-000185d0: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
-000185e0: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
-000185f0: 315d 220a 2020 2020 2020 2020 2020 2020  1]".            
-00018600: 2020 7765 6967 6874 3a20 300a 2020 2020    weight: 0.    
-00018610: 2020 2020 2020 2020 7265 7175 6972 6564          required
-00018620: 5f64 7572 696e 675f 7363 6865 6475 6c69  _during_scheduli
-00018630: 6e67 5f69 676e 6f72 6564 5f64 7572 696e  ng_ignored_durin
-00018640: 675f 6578 6563 7574 696f 6e3a 0a20 2020  g_execution:.   
-00018650: 2020 2020 2020 2020 2020 206e 6f64 655f             node_
-00018660: 7365 6c65 6374 6f72 5f74 6572 6d73 3a0a  selector_terms:.
-00018670: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00018680: 6d61 7463 685f 6578 7072 6573 7369 6f6e  match_expression
-00018690: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000186a0: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
-000186b0: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
-000186c0: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
-000186d0: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
-000186e0: 2020 2020 2020 2020 206d 6174 6368 5f66           match_f
-000186f0: 6965 6c64 733a 0a20 2020 2020 2020 2020  ields:.         
-00018700: 2020 2020 2020 202d 2022 6b65 793a 7665         - "key:ve
-00018710: 7273 696f 6e2c 206f 7065 7261 746f 723a  rsion, operator:
-00018720: 496e 2c20 7661 6c75 6573 3a5b 7631 2e30  In, values:[v1.0
-00018730: 2e30 2c20 7631 2e30 2e31 5d22 0a20 2020  .0, v1.0.1]".   
-00018740: 2020 2020 2020 2020 2020 202d 206d 6174             - mat
-00018750: 6368 5f65 7870 7265 7373 696f 6e73 3a0a  ch_expressions:.
-00018760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018770: 2d20 226b 6579 3a76 6572 7369 6f6e 2c20  - "key:version, 
-00018780: 6f70 6572 6174 6f72 3a49 6e2c 2076 616c  operator:In, val
-00018790: 7565 733a 5b76 312e 302e 302c 2076 312e  ues:[v1.0.0, v1.
-000187a0: 302e 315d 220a 2020 2020 2020 2020 2020  0.1]".          
-000187b0: 2020 2020 2020 6d61 7463 685f 6669 656c        match_fiel
-000187c0: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
-000187d0: 2020 2020 2d20 226b 6579 3a76 6572 7369      - "key:versi
-000187e0: 6f6e 2c20 6f70 6572 6174 6f72 3a49 6e2c  on, operator:In,
-000187f0: 2076 616c 7565 733a 5b76 312e 302e 302c   values:[v1.0.0,
-00018800: 2076 312e 302e 315d 220a 2020 2020 2020   v1.0.1]".      
-00018810: 2020 2020 706f 645f 6166 6669 6e69 7479      pod_affinity
-00018820: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00018830: 6566 6572 7265 645f 6475 7269 6e67 5f73  eferred_during_s
-00018840: 6368 6564 756c 696e 675f 6967 6e6f 7265  cheduling_ignore
-00018850: 645f 6475 7269 6e67 5f65 7865 6375 7469  d_during_executi
-00018860: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-00018870: 2d20 7765 6967 6874 3a20 360a 2020 2020  - weight: 6.    
-00018880: 2020 2020 2020 2020 2020 706f 645f 6166            pod_af
-00018890: 6669 6e69 7479 5f74 6572 6d3a 0a20 2020  finity_term:.   
-000188a0: 2020 2020 2020 2020 2020 2020 206c 6162               lab
-000188b0: 656c 5f73 656c 6563 746f 723a 0a20 2020  el_selector:.   
-000188c0: 2020 2020 2020 2020 2020 2020 202d 2061               - a
-000188d0: 7070 3a64 656d 6f2d 6170 700a 2020 2020  pp:demo-app.    
-000188e0: 2020 2020 2020 2020 2020 2020 2d20 226b              - "k
-000188f0: 6579 3a76 6572 7369 6f6e 2c20 6f70 6572  ey:version, oper
-00018900: 6174 6f72 3a49 6e2c 2076 616c 7565 733a  ator:In, values:
-00018910: 5b76 312e 302e 302c 2076 312e 302e 315d  [v1.0.0, v1.0.1]
-00018920: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00018930: 2020 746f 706f 6c6f 6779 5f6b 6579 3a20    topology_key: 
-00018940: 746f 706f 6c6f 6779 5f6b 6579 0a20 2020  topology_key.   
-00018950: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00018960: 6573 7061 6365 733a 0a20 2020 2020 2020  espaces:.       
-00018970: 2020 2020 2020 2020 202d 206e 616d 6573           - names
-00018980: 7061 6365 730a 2020 2020 2020 2020 2020  paces.          
-00018990: 2020 2020 2020 2d20 6e61 6d65 7370 6163        - namespac
-000189a0: 6573 0a20 2020 2020 2020 2020 2020 202d  es.            -
-000189b0: 2077 6569 6768 743a 2036 0a20 2020 2020   weight: 6.     
-000189c0: 2020 2020 2020 2020 2070 6f64 5f61 6666           pod_aff
-000189d0: 696e 6974 795f 7465 726d 3a0a 2020 2020  inity_term:.    
-000189e0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-000189f0: 6c5f 7365 6c65 6374 6f72 3a0a 2020 2020  l_selector:.    
-00018a00: 2020 2020 2020 2020 2020 2020 2d20 6170              - ap
-00018a10: 703a 6465 6d6f 2d61 7070 0a20 2020 2020  p:demo-app.     
-00018a20: 2020 2020 2020 2020 2020 202d 2022 6b65             - "ke
-00018a30: 793a 7665 7273 696f 6e2c 206f 7065 7261  y:version, opera
-00018a40: 746f 723a 496e 2c20 7661 6c75 6573 3a5b  tor:In, values:[
-00018a50: 7631 2e30 2e30 2c20 7631 2e30 2e31 5d22  v1.0.0, v1.0.1]"
-00018a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018a70: 2074 6f70 6f6c 6f67 795f 6b65 793a 2074   topology_key: t
-00018a80: 6f70 6f6c 6f67 795f 6b65 790a 2020 2020  opology_key.    
-00018a90: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00018aa0: 7370 6163 6573 3a0a 2020 2020 2020 2020  spaces:.        
-00018ab0: 2020 2020 2020 2020 2d20 6e61 6d65 7370          - namesp
-00018ac0: 6163 6573 0a20 2020 2020 2020 2020 2020  aces.           
-00018ad0: 2020 2020 202d 206e 616d 6573 7061 6365       - namespace
-00018ae0: 730a 2020 2020 2020 2020 2020 2020 7265  s.            re
-00018af0: 7175 6972 6564 5f64 7572 696e 675f 7363  quired_during_sc
-00018b00: 6865 6475 6c69 6e67 5f69 676e 6f72 6564  heduling_ignored
-00018b10: 5f64 7572 696e 675f 6578 6563 7574 696f  _during_executio
-00018b20: 6e3a 0a20 2020 2020 2020 2020 2020 202d  n:.            -
-00018b30: 206c 6162 656c 5f73 656c 6563 746f 723a   label_selector:
-00018b40: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
-00018b50: 2061 7070 3a64 656d 6f2d 6170 700a 2020   app:demo-app.  
-00018b60: 2020 2020 2020 2020 2020 2020 2d20 226b              - "k
-00018b70: 6579 3a76 6572 7369 6f6e 2c20 6f70 6572  ey:version, oper
-00018b80: 6174 6f72 3a49 6e2c 2076 616c 7565 733a  ator:In, values:
-00018b90: 5b76 312e 302e 302c 2076 312e 302e 315d  [v1.0.0, v1.0.1]
-00018ba0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00018bb0: 746f 706f 6c6f 6779 5f6b 6579 3a20 746f  topology_key: to
-00018bc0: 706f 6c6f 6779 5f6b 6579 0a20 2020 2020  pology_key.     
-00018bd0: 2020 2020 2020 2020 206e 616d 6573 7061           namespa
-00018be0: 6365 733a 0a20 2020 2020 2020 2020 2020  ces:.           
-00018bf0: 2020 202d 206e 616d 6573 7061 6365 730a     - namespaces.
-00018c00: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00018c10: 6e61 6d65 7370 6163 6573 0a20 2020 2020  namespaces.     
-00018c20: 2020 2020 2020 202d 206c 6162 656c 5f73         - label_s
-00018c30: 656c 6563 746f 723a 0a20 2020 2020 2020  elector:.       
-00018c40: 2020 2020 2020 202d 2061 7070 3a64 656d         - app:dem
-00018c50: 6f2d 6170 700a 2020 2020 2020 2020 2020  o-app.          
-00018c60: 2020 2020 2d20 226b 6579 3a76 6572 7369      - "key:versi
-00018c70: 6f6e 2c20 6f70 6572 6174 6f72 3a49 6e2c  on, operator:In,
-00018c80: 2076 616c 7565 733a 5b76 312e 302e 302c   values:[v1.0.0,
-00018c90: 2076 312e 302e 315d 220a 2020 2020 2020   v1.0.1]".      
-00018ca0: 2020 2020 2020 2020 746f 706f 6c6f 6779          topology
-00018cb0: 5f6b 6579 3a20 746f 706f 6c6f 6779 5f6b  _key: topology_k
-00018cc0: 6579 0a20 2020 2020 2020 2020 2020 2020  ey.             
-00018cd0: 206e 616d 6573 7061 6365 733a 0a20 2020   namespaces:.   
-00018ce0: 2020 2020 2020 2020 2020 202d 206e 616d             - nam
-00018cf0: 6573 7061 6365 730a 2020 2020 2020 2020  espaces.        
-00018d00: 2020 2020 2020 2d20 6e61 6d65 7370 6163        - namespac
-00018d10: 6573 0a20 2020 2020 2070 726f 7065 7274  es.      propert
-00018d20: 6965 733a 0a20 2020 2020 2020 206c 6162  ies:.        lab
-00018d30: 656c 733a 0a20 2020 2020 2020 2020 2064  els:.          d
-00018d40: 6573 6372 6970 7469 6f6e 3a20 4d61 7020  escription: Map 
-00018d50: 6f66 2073 7472 696e 6720 6b65 7973 2061  of string keys a
-00018d60: 6e64 2076 616c 7565 7320 7468 6174 2063  nd values that c
-00018d70: 616e 2062 6520 7573 6564 2074 6f20 6f72  an be used to or
-00018d80: 6761 6e69 7a65 0a20 2020 2020 2020 2020  ganize.         
-00018d90: 2020 2061 6e64 2063 6174 6567 6f72 697a     and categoriz
-00018da0: 6520 2873 636f 7065 2061 6e64 2073 656c  e (scope and sel
-00018db0: 6563 7429 206f 626a 6563 7473 0a20 2020  ect) objects.   
-00018dc0: 2020 2020 2020 2065 7861 6d70 6c65 3a0a         example:.
-00018dd0: 2020 2020 2020 2020 2020 2d20 6170 703a            - app:
-00018de0: 6465 6d6f 2d61 7070 0a20 2020 2020 2020  demo-app.       
-00018df0: 2020 202d 2076 6572 7369 6f6e 3a76 312e     - version:v1.
-00018e00: 302e 300a 2020 2020 2020 2020 2020 6974  0.0.          it
-00018e10: 656d 733a 0a20 2020 2020 2020 2020 2020  ems:.           
-00018e20: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
-00018e30: 2020 2020 2020 2020 7469 746c 653a 204c          title: L
-00018e40: 6162 656c 730a 2020 2020 2020 2020 2020  abels.          
-00018e50: 7479 7065 3a20 6172 7261 790a 2020 2020  type: array.    
-00018e60: 2020 2020 616e 6e6f 7461 7469 6f6e 733a      annotations:
-00018e70: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
-00018e80: 6970 7469 6f6e 3a20 416e 2075 6e73 7472  iption: An unstr
-00018e90: 7563 7475 7265 6420 6b65 7920 7661 6c75  uctured key valu
-00018ea0: 6520 6d61 7020 7468 6174 2063 616e 2062  e map that can b
-00018eb0: 6520 7573 6564 2074 6f20 6174 7461 6368  e used to attach
-00018ec0: 2061 7262 6974 7261 7279 0a20 2020 2020   arbitrary.     
-00018ed0: 2020 2020 2020 206d 6574 6164 6174 610a         metadata.
-00018ee0: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
-00018ef0: 653a 0a20 2020 2020 2020 2020 202d 2061  e:.          - a
-00018f00: 6e6e 6f74 6174 696f 6e2d 6b65 7931 3a76  nnotation-key1:v
-00018f10: 616c 310a 2020 2020 2020 2020 2020 2d20  al1.          - 
-00018f20: 616e 6e6f 7461 7469 6f6e 2d6b 6579 323a  annotation-key2:
-00018f30: 7661 6c32 0a20 2020 2020 2020 2020 2069  val2.          i
-00018f40: 7465 6d73 3a0a 2020 2020 2020 2020 2020  tems:.          
-00018f50: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00018f60: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-00018f70: 416e 6e6f 7461 7469 6f6e 730a 2020 2020  Annotations.    
-00018f80: 2020 2020 2020 7479 7065 3a20 6172 7261        type: arra
-00018f90: 790a 2020 2020 2020 2020 636f 6e74 6169  y.        contai
-00018fa0: 6e65 7273 3a0a 2020 2020 2020 2020 2020  ners:.          
-00018fb0: 6974 656d 733a 0a20 2020 2020 2020 2020  items:.         
-00018fc0: 2020 2024 7265 663a 2027 232f 636f 6d70     $ref: '#/comp
-00018fd0: 6f6e 656e 7473 2f73 6368 656d 6173 2f43  onents/schemas/C
-00018fe0: 6f6e 7461 696e 6572 270a 2020 2020 2020  ontainer'.      
-00018ff0: 2020 2020 7469 746c 653a 2063 6f6e 7461      title: conta
-00019000: 696e 6572 730a 2020 2020 2020 2020 2020  iners.          
-00019010: 7479 7065 3a20 6172 7261 790a 2020 2020  type: array.    
-00019020: 2020 2020 766f 6c75 6d65 733a 0a20 2020      volumes:.   
-00019030: 2020 2020 2020 2069 7465 6d73 3a0a 2020         items:.  
-00019040: 2020 2020 2020 2020 2020 2472 6566 3a20            $ref: 
-00019050: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
-00019060: 6865 6d61 732f 566f 6c75 6d65 270a 2020  hemas/Volume'.  
-00019070: 2020 2020 2020 2020 7469 746c 653a 2076          title: v
-00019080: 6f6c 756d 6573 0a20 2020 2020 2020 2020  olumes.         
-00019090: 2074 7970 653a 2061 7272 6179 0a20 2020   type: array.   
-000190a0: 2020 2020 2061 6666 696e 6974 793a 0a20       affinity:. 
-000190b0: 2020 2020 2020 2020 2024 7265 663a 2027           $ref: '
-000190c0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-000190d0: 656d 6173 2f41 6666 696e 6974 7927 0a20  emas/Affinity'. 
-000190e0: 2020 2020 2074 6974 6c65 3a20 506f 640a       title: Pod.
-000190f0: 2020 2020 2020 7479 7065 3a20 6f62 6a65        type: obje
-00019100: 6374 0a20 2020 2043 6f6e 7461 696e 6572  ct.    Container
-00019110: 3a0a 2020 2020 2020 6578 616d 706c 653a  :.      example:
-00019120: 0a20 2020 2020 2020 2069 6d61 6765 3a20  .        image: 
-00019130: 6e67 696e 783a 6c61 7465 7374 0a20 2020  nginx:latest.   
-00019140: 2020 2020 206c 6966 655f 6379 636c 653a       life_cycle:
-00019150: 0a20 2020 2020 2020 2020 2070 7265 5f73  .          pre_s
-00019160: 746f 703a 0a20 2020 2020 2020 2020 2020  top:.           
-00019170: 2074 6370 5f73 6f63 6b65 743a 0a20 2020   tcp_socket:.   
-00019180: 2020 2020 2020 2020 2020 2070 6f72 743a             port:
-00019190: 2033 3031 3831 0a20 2020 2020 2020 2020   30181.         
-000191a0: 2020 2020 2068 6f73 743a 2031 3237 2e30       host: 127.0
-000191b0: 2e30 2e31 0a20 2020 2020 2020 2020 2020  .0.1.           
-000191c0: 2068 7474 705f 6765 743a 0a20 2020 2020   http_get:.     
-000191d0: 2020 2020 2020 2020 2070 6174 683a 202f           path: /
-000191e0: 7368 6f77 3f64 6f6d 6169 6e3d 7631 392e  show?domain=v19.
-000191f0: 7469 6b74 6f6b 6364 6e2e 636f 6d0a 2020  tiktokcdn.com.  
-00019200: 2020 2020 2020 2020 2020 2020 6874 7470              http
-00019210: 5f68 6561 6465 7273 3a0a 2020 2020 2020  _headers:.      
-00019220: 2020 2020 2020 2020 2d20 782d 6465 7673          - x-devs
-00019230: 7265 2d61 7574 686f 7269 7a61 7469 6f6e  re-authorization
-00019240: 3a42 6561 7265 7220 6579 4a68 6247 6369  :Bearer eyJhbGci
-00019250: 4f69 4a0a 2020 2020 2020 2020 2020 2020  OiJ.            
-00019260: 2020 2d20 636f 6e74 656e 742d 7479 7065    - content-type
-00019270: 3a61 7070 6c69 6361 7469 6f6e 2f6a 736f  :application/jso
-00019280: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00019290: 7363 6865 6d65 3a20 4854 5450 530a 2020  scheme: HTTPS.  
-000192a0: 2020 2020 2020 2020 2020 2020 706f 7274              port
-000192b0: 3a20 3838 3838 0a20 2020 2020 2020 2020  : 8888.         
-000192c0: 2020 2020 2068 6f73 743a 2067 7373 2d64       host: gss-d
-000192d0: 6e73 2d61 6765 6e74 2e65 7861 6d70 6c65  ns-agent.example
-000192e0: 2e6f 7267 0a20 2020 2020 2020 2020 2020  .org.           
-000192f0: 2065 7865 635f 636f 6d6d 616e 643a 0a20   exec_command:. 
-00019300: 2020 2020 2020 2020 2020 202d 202f 6269             - /bi
-00019310: 6e2f 7368 6f77 646f 776e 2e73 680a 2020  n/showdown.sh.  
-00019320: 2020 2020 2020 2020 706f 7374 5f73 7461          post_sta
-00019330: 7274 3a0a 2020 2020 2020 2020 2020 2020  rt:.            
-00019340: 7463 705f 736f 636b 6574 3a0a 2020 2020  tcp_socket:.    
-00019350: 2020 2020 2020 2020 2020 706f 7274 3a20            port: 
-00019360: 3330 3138 310a 2020 2020 2020 2020 2020  30181.          
-00019370: 2020 2020 686f 7374 3a20 3132 372e 302e      host: 127.0.
-00019380: 302e 310a 2020 2020 2020 2020 2020 2020  0.1.            
-00019390: 6874 7470 5f67 6574 3a0a 2020 2020 2020  http_get:.      
-000193a0: 2020 2020 2020 2020 7061 7468 3a20 2f73          path: /s
-000193b0: 686f 773f 646f 6d61 696e 3d76 3139 2e74  how?domain=v19.t
-000193c0: 696b 746f 6b63 646e 2e63 6f6d 0a20 2020  iktokcdn.com.   
-000193d0: 2020 2020 2020 2020 2020 2068 7474 705f             http_
-000193e0: 6865 6164 6572 733a 0a20 2020 2020 2020  headers:.       
-000193f0: 2020 2020 2020 202d 2078 2d64 6576 7372         - x-devsr
-00019400: 652d 6175 7468 6f72 697a 6174 696f 6e3a  e-authorization:
-00019410: 4265 6172 6572 2065 794a 6862 4763 694f  Bearer eyJhbGciO
-00019420: 694a 0a20 2020 2020 2020 2020 2020 2020  iJ.             
-00019430: 202d 2063 6f6e 7465 6e74 2d74 7970 653a   - content-type:
-00019440: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00019450: 0a20 2020 2020 2020 2020 2020 2020 2073  .              s
-00019460: 6368 656d 653a 2048 5454 5053 0a20 2020  cheme: HTTPS.   
-00019470: 2020 2020 2020 2020 2020 2070 6f72 743a             port:
-00019480: 2038 3838 380a 2020 2020 2020 2020 2020   8888.          
-00019490: 2020 2020 686f 7374 3a20 6773 732d 646e      host: gss-dn
-000194a0: 732d 6167 656e 742e 6578 616d 706c 652e  s-agent.example.
-000194b0: 6f72 670a 2020 2020 2020 2020 2020 2020  org.            
-000194c0: 6578 6563 5f63 6f6d 6d61 6e64 3a0a 2020  exec_command:.  
-000194d0: 2020 2020 2020 2020 2020 2d20 2f62 696e            - /bin
-000194e0: 2f73 686f 7764 6f77 6e2e 7368 0a20 2020  /showdown.sh.   
-000194f0: 2020 2020 2072 6573 6f75 7263 6573 3a0a       resources:.
-00019500: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-00019510: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-00019520: 6d65 6d6f 7279 3a20 3235 364d 690a 2020  memory: 256Mi.  
-00019530: 2020 2020 2020 2020 2020 6370 753a 2022            cpu: "
-00019540: 302e 3122 0a20 2020 2020 2020 2020 206c  0.1".          l
-00019550: 696d 6974 733a 0a20 2020 2020 2020 2020  imits:.         
-00019560: 2020 206d 656d 6f72 793a 2035 3132 4d69     memory: 512Mi
-00019570: 0a20 2020 2020 2020 2020 2020 2063 7075  .            cpu
-00019580: 3a20 2230 2e35 220a 2020 2020 2020 2020  : "0.5".        
-00019590: 766f 6c75 6d65 5f6d 6f75 6e74 733a 0a20  volume_mounts:. 
-000195a0: 2020 2020 2020 202d 2070 6174 683a 202f         - path: /
-000195b0: 6f70 742f 7365 7276 6572 2f63 6f6e 660a  opt/server/conf.
-000195c0: 2020 2020 2020 2020 2020 7265 6164 5f6f            read_o
-000195d0: 6e6c 793a 2074 7275 650a 2020 2020 2020  nly: true.      
-000195e0: 2020 2020 6e61 6d65 3a20 6465 6d6f 2d76      name: demo-v
-000195f0: 6f6c 0a20 2020 2020 2020 2020 2073 7562  ol.          sub
-00019600: 5f70 6174 683a 2073 6572 7665 722e 636f  _path: server.co
-00019610: 6e66 0a20 2020 2020 2020 202d 2070 6174  nf.        - pat
-00019620: 683a 202f 6f70 742f 7365 7276 6572 2f63  h: /opt/server/c
-00019630: 6f6e 660a 2020 2020 2020 2020 2020 7265  onf.          re
-00019640: 6164 5f6f 6e6c 793a 2074 7275 650a 2020  ad_only: true.  
-00019650: 2020 2020 2020 2020 6e61 6d65 3a20 6465          name: de
-00019660: 6d6f 2d76 6f6c 0a20 2020 2020 2020 2020  mo-vol.         
-00019670: 2073 7562 5f70 6174 683a 2073 6572 7665   sub_path: serve
-00019680: 722e 636f 6e66 0a20 2020 2020 2020 2065  r.conf.        e
-00019690: 6e76 3a0a 2020 2020 2020 2020 2020 6e61  nv:.          na
-000196a0: 6d65 3a20 534d 535f 4b45 5953 5f50 4154  me: SMS_KEYS_PAT
-000196b0: 485f 584d 0a20 2020 2020 2020 2020 2076  H_XM.          v
-000196c0: 616c 7565 3a20 646d 732d 7365 6372 6574  alue: dms-secret
-000196d0: 0a20 2020 2020 2020 2070 6f72 7473 3a0a  .        ports:.
-000196e0: 2020 2020 2020 2020 2d20 636f 6e74 6169          - contai
-000196f0: 6e65 725f 706f 7274 3a20 3830 0a20 2020  ner_port: 80.   
-00019700: 2020 2020 2020 2070 726f 746f 636f 6c3a         protocol:
-00019710: 2054 4350 0a20 2020 2020 2020 2020 206e   TCP.          n
-00019720: 616d 653a 2068 7474 700a 2020 2020 2020  ame: http.      
-00019730: 2020 2d20 636f 6e74 6169 6e65 725f 706f    - container_po
-00019740: 7274 3a20 3830 0a20 2020 2020 2020 2020  rt: 80.         
-00019750: 2070 726f 746f 636f 6c3a 2054 4350 0a20   protocol: TCP. 
-00019760: 2020 2020 2020 2020 206e 616d 653a 2068           name: h
-00019770: 7474 700a 2020 2020 2020 2020 636f 6d6d  ttp.        comm
-00019780: 616e 643a 0a20 2020 2020 2020 202d 2070  and:.        - p
-00019790: 7974 686f 6e33 0a20 2020 2020 2020 2061  ython3.        a
-000197a0: 7267 733a 0a20 2020 2020 2020 202d 202d  rgs:.        - -
-000197b0: 6d0a 2020 2020 2020 2020 2d20 6f70 656e  m.        - open
-000197c0: 6170 695f 7365 7276 6572 0a20 2020 2020  api_server.     
-000197d0: 2020 2072 6561 6469 6e65 7373 5f70 726f     readiness_pro
-000197e0: 6265 3a0a 2020 2020 2020 2020 2020 7065  be:.          pe
-000197f0: 7269 6f64 5f73 6563 6f6e 6473 3a20 3630  riod_seconds: 60
-00019800: 0a20 2020 2020 2020 2020 2069 6e69 7469  .          initi
-00019810: 616c 5f64 656c 6179 5f73 6563 6f6e 6473  al_delay_seconds
-00019820: 3a20 3630 300a 2020 2020 2020 2020 2020  : 600.          
-00019830: 7463 705f 736f 636b 6574 3a0a 2020 2020  tcp_socket:.    
-00019840: 2020 2020 2020 2020 706f 7274 3a20 3330          port: 30
-00019850: 3138 310a 2020 2020 2020 2020 2020 2020  181.            
-00019860: 686f 7374 3a20 3132 372e 302e 302e 310a  host: 127.0.0.1.
-00019870: 2020 2020 2020 2020 2020 6661 696c 7572            failur
-00019880: 655f 7468 7265 7368 6f6c 643a 2033 0a20  e_threshold: 3. 
-00019890: 2020 2020 2020 2020 2068 7474 705f 6765           http_ge
-000198a0: 743a 0a20 2020 2020 2020 2020 2020 2070  t:.            p
-000198b0: 6174 683a 202f 7368 6f77 3f64 6f6d 6169  ath: /show?domai
-000198c0: 6e3d 7631 392e 7469 6b74 6f6b 6364 6e2e  n=v19.tiktokcdn.
-000198d0: 636f 6d0a 2020 2020 2020 2020 2020 2020  com.            
-000198e0: 6874 7470 5f68 6561 6465 7273 3a0a 2020  http_headers:.  
-000198f0: 2020 2020 2020 2020 2020 2d20 782d 6465            - x-de
-00019900: 7673 7265 2d61 7574 686f 7269 7a61 7469  vsre-authorizati
-00019910: 6f6e 3a42 6561 7265 7220 6579 4a68 6247  on:Bearer eyJhbG
-00019920: 6369 4f69 4a0a 2020 2020 2020 2020 2020  ciOiJ.          
-00019930: 2020 2d20 636f 6e74 656e 742d 7479 7065    - content-type
-00019940: 3a61 7070 6c69 6361 7469 6f6e 2f6a 736f  :application/jso
-00019950: 6e0a 2020 2020 2020 2020 2020 2020 7363  n.            sc
-00019960: 6865 6d65 3a20 4854 5450 530a 2020 2020  heme: HTTPS.    
-00019970: 2020 2020 2020 2020 706f 7274 3a20 3838          port: 88
-00019980: 3838 0a20 2020 2020 2020 2020 2020 2068  88.            h
-00019990: 6f73 743a 2067 7373 2d64 6e73 2d61 6765  ost: gss-dns-age
-000199a0: 6e74 2e65 7861 6d70 6c65 2e6f 7267 0a20  nt.example.org. 
-000199b0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-000199c0: 5f73 6563 6f6e 6473 3a20 3630 0a20 2020  _seconds: 60.   
-000199d0: 2020 2020 2020 2065 7865 635f 636f 6d6d         exec_comm
-000199e0: 616e 643a 0a20 2020 2020 2020 2020 202d  and:.          -
-000199f0: 202f 6773 732f 6469 6e67 6d61 6e2f 6269   /gss/dingman/bi
-00019a00: 6e2f 6469 6e67 6d61 6e2d 636c 6974 0a20  n/dingman-clit. 
-00019a10: 2020 2020 2020 2020 202d 202d 6164 6472           - -addr
-00019a20: 6573 730a 2020 2020 2020 2020 2020 2d20  ess.          - 
-00019a30: 3132 372e 302e 302e 313a 3330 3530 310a  127.0.0.1:30501.
-00019a40: 2020 2020 2020 2020 2020 2d20 2d63 6f6d            - -com
-00019a50: 6d61 6e64 0a20 2020 2020 2020 2020 202d  mand.          -
-00019a60: 2073 686f 7720 706f 703a 616c 6c20 7375   show pop:all su
-00019a70: 6d6d 6172 793a 6865 616c 7468 2d73 7461  mmary:health-sta
-00019a80: 7475 730a 2020 2020 2020 2020 656e 765f  tus.        env_
-00019a90: 6672 6f6d 3a20 5265 6775 6c61 720a 2020  from: Regular.  
-00019aa0: 2020 2020 2020 7374 6172 7475 705f 7072        startup_pr
-00019ab0: 6f62 653a 0a20 2020 2020 2020 2020 2070  obe:.          p
-00019ac0: 6572 696f 645f 7365 636f 6e64 733a 2036  eriod_seconds: 6
-00019ad0: 300a 2020 2020 2020 2020 2020 696e 6974  0.          init
-00019ae0: 6961 6c5f 6465 6c61 795f 7365 636f 6e64  ial_delay_second
-00019af0: 733a 2036 3030 0a20 2020 2020 2020 2020  s: 600.         
-00019b00: 2074 6370 5f73 6f63 6b65 743a 0a20 2020   tcp_socket:.   
-00019b10: 2020 2020 2020 2020 2070 6f72 743a 2033           port: 3
-00019b20: 3031 3831 0a20 2020 2020 2020 2020 2020  0181.           
-00019b30: 2068 6f73 743a 2031 3237 2e30 2e30 2e31   host: 127.0.0.1
-00019b40: 0a20 2020 2020 2020 2020 2066 6169 6c75  .          failu
-00019b50: 7265 5f74 6872 6573 686f 6c64 3a20 330a  re_threshold: 3.
-00019b60: 2020 2020 2020 2020 2020 6874 7470 5f67            http_g
-00019b70: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-00019b80: 7061 7468 3a20 2f73 686f 773f 646f 6d61  path: /show?doma
-00019b90: 696e 3d76 3139 2e74 696b 746f 6b63 646e  in=v19.tiktokcdn
-00019ba0: 2e63 6f6d 0a20 2020 2020 2020 2020 2020  .com.           
-00019bb0: 2068 7474 705f 6865 6164 6572 733a 0a20   http_headers:. 
-00019bc0: 2020 2020 2020 2020 2020 202d 2078 2d64             - x-d
-00019bd0: 6576 7372 652d 6175 7468 6f72 697a 6174  evsre-authorizat
-00019be0: 696f 6e3a 4265 6172 6572 2065 794a 6862  ion:Bearer eyJhb
-00019bf0: 4763 694f 694a 0a20 2020 2020 2020 2020  GciOiJ.         
-00019c00: 2020 202d 2063 6f6e 7465 6e74 2d74 7970     - content-typ
-00019c10: 653a 6170 706c 6963 6174 696f 6e2f 6a73  e:application/js
-00019c20: 6f6e 0a20 2020 2020 2020 2020 2020 2073  on.            s
-00019c30: 6368 656d 653a 2048 5454 5053 0a20 2020  cheme: HTTPS.   
-00019c40: 2020 2020 2020 2020 2070 6f72 743a 2038           port: 8
-00019c50: 3838 380a 2020 2020 2020 2020 2020 2020  888.            
-00019c60: 686f 7374 3a20 6773 732d 646e 732d 6167  host: gss-dns-ag
-00019c70: 656e 742e 6578 616d 706c 652e 6f72 670a  ent.example.org.
-00019c80: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
-00019c90: 745f 7365 636f 6e64 733a 2036 300a 2020  t_seconds: 60.  
-00019ca0: 2020 2020 2020 2020 6578 6563 5f63 6f6d          exec_com
-00019cb0: 6d61 6e64 3a0a 2020 2020 2020 2020 2020  mand:.          
-00019cc0: 2d20 2f67 7373 2f64 696e 676d 616e 2f62  - /gss/dingman/b
-00019cd0: 696e 2f64 696e 676d 616e 2d63 6c69 740a  in/dingman-clit.
-00019ce0: 2020 2020 2020 2020 2020 2d20 2d61 6464            - -add
-00019cf0: 7265 7373 0a20 2020 2020 2020 2020 202d  ress.          -
-00019d00: 2031 3237 2e30 2e30 2e31 3a33 3035 3031   127.0.0.1:30501
-00019d10: 0a20 2020 2020 2020 2020 202d 202d 636f  .          - -co
-00019d20: 6d6d 616e 640a 2020 2020 2020 2020 2020  mmand.          
-00019d30: 2d20 7368 6f77 2070 6f70 3a61 6c6c 2073  - show pop:all s
-00019d40: 756d 6d61 7279 3a68 6561 6c74 682d 7374  ummary:health-st
-00019d50: 6174 7573 0a20 2020 2020 2020 2069 6d61  atus.        ima
-00019d60: 6765 5f70 756c 6c5f 706f 6c69 6379 3a20  ge_pull_policy: 
-00019d70: 4966 4e6f 7450 7265 7365 6e74 0a20 2020  IfNotPresent.   
-00019d80: 2020 2020 2076 6f6c 756d 655f 6465 7669       volume_devi
-00019d90: 6365 733a 0a20 2020 2020 2020 202d 206e  ces:.        - n
-00019da0: 616d 653a 2064 656d 6f2d 766f 6c0a 2020  ame: demo-vol.  
-00019db0: 2020 2020 2020 2020 6465 7669 6365 5f70          device_p
-00019dc0: 6174 683a 202f 6465 762f 7364 6131 0a20  ath: /dev/sda1. 
-00019dd0: 2020 2020 2020 2020 2062 6361 6368 655f           bcache_
-00019de0: 6e75 6d73 3a20 340a 2020 2020 2020 2020  nums: 4.        
-00019df0: 2d20 6e61 6d65 3a20 6465 6d6f 2d76 6f6c  - name: demo-vol
-00019e00: 0a20 2020 2020 2020 2020 2064 6576 6963  .          devic
-00019e10: 655f 7061 7468 3a20 2f64 6576 2f73 6461  e_path: /dev/sda
-00019e20: 310a 2020 2020 2020 2020 2020 6263 6163  1.          bcac
-00019e30: 6865 5f6e 756d 733a 2034 0a20 2020 2020  he_nums: 4.     
-00019e40: 2020 206e 616d 653a 2068 7474 702d 7365     name: http-se
-00019e50: 7276 6572 0a20 2020 2020 2020 2063 6f6e  rver.        con
-00019e60: 7461 696e 6572 5f74 7970 653a 2049 6e69  tainer_type: Ini
-00019e70: 740a 2020 2020 2020 2020 6c69 7665 6e65  t.        livene
-00019e80: 7373 5f70 726f 6265 3a0a 2020 2020 2020  ss_probe:.      
-00019e90: 2020 2020 7065 7269 6f64 5f73 6563 6f6e      period_secon
-00019ea0: 6473 3a20 3630 0a20 2020 2020 2020 2020  ds: 60.         
-00019eb0: 2069 6e69 7469 616c 5f64 656c 6179 5f73   initial_delay_s
-00019ec0: 6563 6f6e 6473 3a20 3630 300a 2020 2020  econds: 600.    
-00019ed0: 2020 2020 2020 7463 705f 736f 636b 6574        tcp_socket
-00019ee0: 3a0a 2020 2020 2020 2020 2020 2020 706f  :.            po
-00019ef0: 7274 3a20 3330 3138 310a 2020 2020 2020  rt: 30181.      
-00019f00: 2020 2020 2020 686f 7374 3a20 3132 372e        host: 127.
-00019f10: 302e 302e 310a 2020 2020 2020 2020 2020  0.0.1.          
-00019f20: 6661 696c 7572 655f 7468 7265 7368 6f6c  failure_threshol
-00019f30: 643a 2033 0a20 2020 2020 2020 2020 2068  d: 3.          h
-00019f40: 7474 705f 6765 743a 0a20 2020 2020 2020  ttp_get:.       
-00019f50: 2020 2020 2070 6174 683a 202f 7368 6f77       path: /show
-00019f60: 3f64 6f6d 6169 6e3d 7631 392e 7469 6b74  ?domain=v19.tikt
-00019f70: 6f6b 6364 6e2e 636f 6d0a 2020 2020 2020  okcdn.com.      
-00019f80: 2020 2020 2020 6874 7470 5f68 6561 6465        http_heade
-00019f90: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-00019fa0: 2d20 782d 6465 7673 7265 2d61 7574 686f  - x-devsre-autho
-00019fb0: 7269 7a61 7469 6f6e 3a42 6561 7265 7220  rization:Bearer 
-00019fc0: 6579 4a68 6247 6369 4f69 4a0a 2020 2020  eyJhbGciOiJ.    
-00019fd0: 2020 2020 2020 2020 2d20 636f 6e74 656e          - conten
-00019fe0: 742d 7479 7065 3a61 7070 6c69 6361 7469  t-type:applicati
-00019ff0: 6f6e 2f6a 736f 6e0a 2020 2020 2020 2020  on/json.        
-0001a000: 2020 2020 7363 6865 6d65 3a20 4854 5450      scheme: HTTP
-0001a010: 530a 2020 2020 2020 2020 2020 2020 706f  S.            po
-0001a020: 7274 3a20 3838 3838 0a20 2020 2020 2020  rt: 8888.       
-0001a030: 2020 2020 2068 6f73 743a 2067 7373 2d64       host: gss-d
-0001a040: 6e73 2d61 6765 6e74 2e65 7861 6d70 6c65  ns-agent.example
-0001a050: 2e6f 7267 0a20 2020 2020 2020 2020 2074  .org.          t
-0001a060: 696d 656f 7574 5f73 6563 6f6e 6473 3a20  imeout_seconds: 
-0001a070: 3630 0a20 2020 2020 2020 2020 2065 7865  60.          exe
-0001a080: 635f 636f 6d6d 616e 643a 0a20 2020 2020  c_command:.     
-0001a090: 2020 2020 202d 202f 6773 732f 6469 6e67       - /gss/ding
-0001a0a0: 6d61 6e2f 6269 6e2f 6469 6e67 6d61 6e2d  man/bin/dingman-
-0001a0b0: 636c 6974 0a20 2020 2020 2020 2020 202d  clit.          -
-0001a0c0: 202d 6164 6472 6573 730a 2020 2020 2020   -address.      
-0001a0d0: 2020 2020 2d20 3132 372e 302e 302e 313a      - 127.0.0.1:
-0001a0e0: 3330 3530 310a 2020 2020 2020 2020 2020  30501.          
-0001a0f0: 2d20 2d63 6f6d 6d61 6e64 0a20 2020 2020  - -command.     
-0001a100: 2020 2020 202d 2073 686f 7720 706f 703a       - show pop:
-0001a110: 616c 6c20 7375 6d6d 6172 793a 6865 616c  all summary:heal
-0001a120: 7468 2d73 7461 7475 730a 2020 2020 2020  th-status.      
-0001a130: 2020 7365 6375 7269 7479 5f63 6f6e 7465    security_conte
-0001a140: 7874 3a0a 2020 2020 2020 2020 2020 6361  xt:.          ca
-0001a150: 7061 6269 6c69 7469 6573 3a0a 2020 2020  pabilities:.    
-0001a160: 2020 2020 2020 2020 6164 643a 0a20 2020          add:.   
-0001a170: 2020 2020 2020 2020 202d 204e 4554 5f41           - NET_A
-0001a180: 444d 494e 0a20 2020 2020 2020 2020 2020  DMIN.           
-0001a190: 202d 2053 5953 5f54 494d 450a 2020 2020   - SYS_TIME.    
-0001a1a0: 2020 2020 2020 2020 6472 6f70 3a0a 2020          drop:.  
-0001a1b0: 2020 2020 2020 2020 2020 2d20 4e45 545f            - NET_
-0001a1c0: 4144 4d49 4e0a 2020 2020 2020 2020 2020  ADMIN.          
-0001a1d0: 2020 2d20 5359 535f 5449 4d45 0a20 2020    - SYS_TIME.   
-0001a1e0: 2020 2020 2020 2072 756e 5f61 735f 6772         run_as_gr
-0001a1f0: 6f75 703a 2033 3030 300a 2020 2020 2020  oup: 3000.      
-0001a200: 2020 2020 7275 6e5f 6173 5f75 7365 723a      run_as_user:
-0001a210: 2031 3030 300a 2020 2020 2020 7072 6f70   1000.      prop
-0001a220: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
-0001a230: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
-0001a240: 6465 7363 7269 7074 696f 6e3a 207c 0a20  description: |. 
-0001a250: 2020 2020 2020 2020 2020 204e 616d 6520             Name 
-0001a260: 6f66 2074 6865 2063 6f6e 7461 696e 6572  of the container
-0001a270: 2073 7065 6369 6669 6564 2061 7320 6120   specified as a 
-0001a280: 444e 535f 4c41 4245 4c2e 2045 6163 6820  DNS_LABEL. Each 
-0001a290: 636f 6e74 6169 6e65 7220 696e 2061 2070  container in a p
-0001a2a0: 6f64 206d 7573 7420 6861 7665 2061 2075  od must have a u
-0001a2b0: 6e69 7175 6520 6e61 6d65 2028 444e 535f  nique name (DNS_
-0001a2c0: 4c41 4245 4c29 2e0a 2020 2020 2020 2020  LABEL)..        
-0001a2d0: 2020 2020 4361 6e6e 6f74 2062 6520 7570      Cannot be up
-0001a2e0: 6461 7465 640a 2020 2020 2020 2020 2020  dated.          
-0001a2f0: 6578 616d 706c 653a 2068 7474 702d 7365  example: http-se
-0001a300: 7276 6572 0a20 2020 2020 2020 2020 2074  rver.          t
-0001a310: 6974 6c65 3a20 6e61 6d65 0a20 2020 2020  itle: name.     
-0001a320: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-0001a330: 670a 2020 2020 2020 2020 636f 6e74 6169  g.        contai
-0001a340: 6e65 725f 7479 7065 3a0a 2020 2020 2020  ner_type:.      
-0001a350: 2020 2020 656e 756d 3a0a 2020 2020 2020      enum:.      
-0001a360: 2020 2020 2d20 496e 6974 0a20 2020 2020      - Init.     
-0001a370: 2020 2020 202d 2052 6567 756c 6172 0a20       - Regular. 
-0001a380: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-0001a390: 636f 6e74 6169 6e65 725f 7479 7065 0a20  container_type. 
-0001a3a0: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-0001a3b0: 7472 696e 670a 2020 2020 2020 2020 656e  tring.        en
-0001a3c0: 763a 0a20 2020 2020 2020 2020 2064 6573  v:.          des
-0001a3d0: 6372 6970 7469 6f6e 3a20 4c69 7374 206f  cription: List o
-0001a3e0: 6620 656e 7669 726f 6e6d 656e 7420 7661  f environment va
-0001a3f0: 7269 6162 6c65 7320 746f 2073 6574 2069  riables to set i
-0001a400: 6e20 7468 6520 636f 6e74 6169 6e65 722e  n the container.
-0001a410: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-0001a420: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-0001a430: 6e61 6d65 3a20 534d 535f 4b45 5953 5f50  name: SMS_KEYS_P
-0001a440: 4154 485f 584d 0a20 2020 2020 2020 2020  ATH_XM.         
-0001a450: 2020 2076 616c 7565 3a20 646d 732d 7365     value: dms-se
-0001a460: 6372 6574 0a20 2020 2020 2020 2020 2069  cret.          i
-0001a470: 7465 6d73 3a0a 2020 2020 2020 2020 2020  tems:.          
-0001a480: 2020 2472 6566 3a20 2723 2f63 6f6d 706f    $ref: '#/compo
-0001a490: 6e65 6e74 732f 7363 6865 6d61 732f 456e  nents/schemas/En
-0001a4a0: 7656 6172 270a 2020 2020 2020 2020 2020  vVar'.          
-0001a4b0: 7469 746c 653a 2065 6e76 0a20 2020 2020  title: env.     
-0001a4c0: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
-0001a4d0: 0a20 2020 2020 2020 2065 6e76 5f66 726f  .        env_fro
-0001a4e0: 6d3a 0a20 2020 2020 2020 2020 2064 6573  m:.          des
-0001a4f0: 6372 6970 7469 6f6e 3a20 4c69 7374 206f  cription: List o
-0001a500: 6620 736f 7572 6365 7320 746f 2070 6f70  f sources to pop
-0001a510: 756c 6174 6520 656e 7669 726f 6e6d 656e  ulate environmen
-0001a520: 7420 7661 7269 6162 6c65 7320 696e 2074  t variables in t
-0001a530: 6865 2063 6f6e 7461 696e 6572 2e0a 2020  he container..  
-0001a540: 2020 2020 2020 2020 6578 616d 706c 653a          example:
-0001a550: 2052 6567 756c 6172 0a20 2020 2020 2020   Regular.       
-0001a560: 2020 2069 7465 6d73 3a0a 2020 2020 2020     items:.      
-0001a570: 2020 2020 2020 2472 6566 3a20 2723 2f63        $ref: '#/c
-0001a580: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-0001a590: 732f 456e 7646 726f 6d53 6f75 7263 6527  s/EnvFromSource'
-0001a5a0: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
-0001a5b0: 3a20 656e 765f 6672 6f6d 0a20 2020 2020  : env_from.     
-0001a5c0: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
-0001a5d0: 0a20 2020 2020 2020 2069 6d61 6765 3a0a  .        image:.
-0001a5e0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-0001a5f0: 7074 696f 6e3a 2044 6f63 6b65 7220 696d  ption: Docker im
-0001a600: 6167 6520 7572 6c0a 2020 2020 2020 2020  age url.        
-0001a610: 2020 6578 616d 706c 653a 206e 6769 6e78    example: nginx
-0001a620: 3a6c 6174 6573 740a 2020 2020 2020 2020  :latest.        
-0001a630: 2020 7469 746c 653a 2069 6d61 6765 0a20    title: image. 
-0001a640: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-0001a650: 7472 696e 670a 2020 2020 2020 2020 696d  tring.        im
-0001a660: 6167 655f 7075 6c6c 5f70 6f6c 6963 793a  age_pull_policy:
-0001a670: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
-0001a680: 6970 7469 6f6e 3a20 4465 6661 756c 7473  iption: Defaults
-0001a690: 2074 6f20 416c 7761 7973 0a20 2020 2020   to Always.     
-0001a6a0: 2020 2020 2065 6e75 6d3a 0a20 2020 2020       enum:.     
-0001a6b0: 2020 2020 202d 2049 664e 6f74 5072 6573       - IfNotPres
-0001a6c0: 656e 740a 2020 2020 2020 2020 2020 2d20  ent.          - 
-0001a6d0: 416c 7761 7973 0a20 2020 2020 2020 2020  Always.         
-0001a6e0: 202d 204e 6576 6572 0a20 2020 2020 2020   - Never.       
-0001a6f0: 2020 2065 7861 6d70 6c65 3a20 4966 4e6f     example: IfNo
-0001a700: 7450 7265 7365 6e74 0a20 2020 2020 2020  tPresent.       
-0001a710: 2020 2074 6974 6c65 3a20 696d 6167 655f     title: image_
-0001a720: 7075 6c6c 5f70 6f6c 6963 790a 2020 2020  pull_policy.    
-0001a730: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
-0001a740: 6e67 0a20 2020 2020 2020 2061 7267 733a  ng.        args:
-0001a750: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
-0001a760: 6970 7469 6f6e 3a20 4172 6775 6d65 6e74  iption: Argument
-0001a770: 7320 746f 2074 6865 2065 6e74 7279 706f  s to the entrypo
-0001a780: 696e 742e 2054 6865 2063 6f6e 7461 696e  int. The contain
-0001a790: 6572 2069 6d61 6765 2773 2043 4d44 2069  er image's CMD i
-0001a7a0: 7320 7573 6564 0a20 2020 2020 2020 2020  s used.         
-0001a7b0: 2020 2069 6620 7468 6973 2069 7320 6e6f     if this is no
-0001a7c0: 7420 7072 6f76 6964 6564 0a20 2020 2020  t provided.     
-0001a7d0: 2020 2020 2065 7861 6d70 6c65 3a0a 2020       example:.  
-0001a7e0: 2020 2020 2020 2020 2d20 2d6d 0a20 2020          - -m.   
-0001a7f0: 2020 2020 2020 202d 206f 7065 6e61 7069         - openapi
-0001a800: 5f73 6572 7665 720a 2020 2020 2020 2020  _server.        
-0001a810: 2020 6974 656d 733a 0a20 2020 2020 2020    items:.       
-0001a820: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-0001a830: 670a 2020 2020 2020 2020 2020 7469 746c  g.          titl
-0001a840: 653a 2061 7267 730a 2020 2020 2020 2020  e: args.        
-0001a850: 2020 7479 7065 3a20 6172 7261 790a 2020    type: array.  
-0001a860: 2020 2020 2020 636f 6d6d 616e 643a 0a20        command:. 
-0001a870: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-0001a880: 7469 6f6e 3a20 7c0a 2020 2020 2020 2020  tion: |.        
-0001a890: 2020 2020 456e 7472 7970 6f69 6e74 2061      Entrypoint a
-0001a8a0: 7272 6179 2e20 4e6f 7420 6578 6563 7574  rray. Not execut
-0001a8b0: 6564 2077 6974 6869 6e20 6120 7368 656c  ed within a shel
-0001a8c0: 6c2e 0a20 2020 2020 2020 2020 2020 2054  l..            T
-0001a8d0: 6865 2063 6f6e 7461 696e 6572 2069 6d61  he container ima
-0001a8e0: 6765 2773 2045 4e54 5259 504f 494e 5420  ge's ENTRYPOINT 
-0001a8f0: 6973 2075 7365 6420 6966 2074 6869 7320  is used if this 
-0001a900: 6973 206e 6f74 2070 726f 7669 6465 642e  is not provided.
-0001a910: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-0001a920: 6c65 3a0a 2020 2020 2020 2020 2020 2d20  le:.          - 
-0001a930: 7079 7468 6f6e 330a 2020 2020 2020 2020  python3.        
-0001a940: 2020 6974 656d 733a 0a20 2020 2020 2020    items:.       
-0001a950: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-0001a960: 670a 2020 2020 2020 2020 2020 7469 746c  g.          titl
-0001a970: 653a 2063 6f6d 6d61 6e64 0a20 2020 2020  e: command.     
-0001a980: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
-0001a990: 0a20 2020 2020 2020 2073 6563 7572 6974  .        securit
-0001a9a0: 795f 636f 6e74 6578 743a 0a20 2020 2020  y_context:.     
-0001a9b0: 2020 2020 2024 7265 663a 2027 232f 636f       $ref: '#/co
-0001a9c0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-0001a9d0: 2f43 6f6e 7461 696e 6572 5365 6343 6f6e  /ContainerSecCon
-0001a9e0: 7465 7874 270a 2020 2020 2020 2020 6c69  text'.        li
-0001a9f0: 6665 5f63 7963 6c65 3a0a 2020 2020 2020  fe_cycle:.      
-0001aa00: 2020 2020 2472 6566 3a20 2723 2f63 6f6d      $ref: '#/com
-0001aa10: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-0001aa20: 436f 6e74 6169 6e65 724c 6966 6543 7963  ContainerLifeCyc
-0001aa30: 6c65 270a 2020 2020 2020 2020 706f 7274  le'.        port
-0001aa40: 733a 0a20 2020 2020 2020 2020 2069 7465  s:.          ite
-0001aa50: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-0001aa60: 2472 6566 3a20 2723 2f63 6f6d 706f 6e65  $ref: '#/compone
-0001aa70: 6e74 732f 7363 6865 6d61 732f 436f 6e74  nts/schemas/Cont
-0001aa80: 6169 6e65 7250 6f72 7427 0a20 2020 2020  ainerPort'.     
-0001aa90: 2020 2020 2074 6974 6c65 3a20 706f 7274       title: port
-0001aaa0: 730a 2020 2020 2020 2020 2020 7479 7065  s.          type
-0001aab0: 3a20 6172 7261 790a 2020 2020 2020 2020  : array.        
-0001aac0: 766f 6c75 6d65 5f6d 6f75 6e74 733a 0a20  volume_mounts:. 
-0001aad0: 2020 2020 2020 2020 2069 7465 6d73 3a0a           items:.
-0001aae0: 2020 2020 2020 2020 2020 2020 2472 6566              $ref
-0001aaf0: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
-0001ab00: 7363 6865 6d61 732f 566f 6c75 6d65 4d6f  schemas/VolumeMo
-0001ab10: 756e 7427 0a20 2020 2020 2020 2020 2074  unt'.          t
-0001ab20: 6974 6c65 3a20 766f 6c75 6d65 5f6d 6f75  itle: volume_mou
-0001ab30: 6e74 730a 2020 2020 2020 2020 2020 7479  nts.          ty
-0001ab40: 7065 3a20 6172 7261 790a 2020 2020 2020  pe: array.      
-0001ab50: 2020 766f 6c75 6d65 5f64 6576 6963 6573    volume_devices
-0001ab60: 3a0a 2020 2020 2020 2020 2020 6974 656d  :.          item
-0001ab70: 733a 0a20 2020 2020 2020 2020 2020 2024  s:.            $
-0001ab80: 7265 663a 2027 232f 636f 6d70 6f6e 656e  ref: '#/componen
-0001ab90: 7473 2f73 6368 656d 6173 2f56 6f6c 756d  ts/schemas/Volum
-0001aba0: 6544 6576 6963 6527 0a20 2020 2020 2020  eDevice'.       
-0001abb0: 2020 2074 6974 6c65 3a20 766f 6c75 6d65     title: volume
-0001abc0: 5f64 6576 6963 6573 0a20 2020 2020 2020  _devices.       
-0001abd0: 2020 2074 7970 653a 2061 7272 6179 0a20     type: array. 
-0001abe0: 2020 2020 2020 2072 6573 6f75 7263 6573         resources
-0001abf0: 3a0a 2020 2020 2020 2020 2020 2472 6566  :.          $ref
-0001ac00: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
-0001ac10: 7363 6865 6d61 732f 5265 736f 7572 6365  schemas/Resource
-0001ac20: 5265 7175 6972 656d 656e 7473 270a 2020  Requirements'.  
-0001ac30: 2020 2020 2020 6c69 7665 6e65 7373 5f70        liveness_p
-0001ac40: 726f 6265 3a0a 2020 2020 2020 2020 2020  robe:.          
-0001ac50: 2472 6566 3a20 2723 2f63 6f6d 706f 6e65  $ref: '#/compone
-0001ac60: 6e74 732f 7363 6865 6d61 732f 5072 6f62  nts/schemas/Prob
-0001ac70: 6527 0a20 2020 2020 2020 2072 6561 6469  e'.        readi
-0001ac80: 6e65 7373 5f70 726f 6265 3a0a 2020 2020  ness_probe:.    
-0001ac90: 2020 2020 2020 2472 6566 3a20 2723 2f63        $ref: '#/c
-0001aca0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-0001acb0: 732f 5072 6f62 6527 0a20 2020 2020 2020  s/Probe'.       
-0001acc0: 2073 7461 7274 7570 5f70 726f 6265 3a0a   startup_probe:.
-0001acd0: 2020 2020 2020 2020 2020 2472 6566 3a20            $ref: 
-0001ace0: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
-0001acf0: 6865 6d61 732f 5072 6f62 6527 0a20 2020  hemas/Probe'.   
-0001ad00: 2020 2072 6571 7569 7265 643a 0a20 2020     required:.   
-0001ad10: 2020 202d 206e 616d 650a 2020 2020 2020     - name.      
-0001ad20: 7469 746c 653a 2043 6f6e 7461 696e 6572  title: Container
-0001ad30: 0a20 2020 2020 2074 7970 653a 206f 626a  .      type: obj
-0001ad40: 6563 740a 2020 2020 456e 7656 6172 3a0a  ect.    EnvVar:.
-0001ad50: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
-0001ad60: 3a0a 2020 2020 2020 2020 6e61 6d65 3a0a  :.        name:.
-0001ad70: 2020 2020 2020 2020 2020 7469 746c 653a            title:
-0001ad80: 206e 616d 650a 2020 2020 2020 2020 2020   name.          
-0001ad90: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
-0001ada0: 2020 2020 2076 616c 7565 3a0a 2020 2020       value:.    
-0001adb0: 2020 2020 2020 7469 746c 653a 2076 616c        title: val
-0001adc0: 7565 0a20 2020 2020 2020 2020 2074 7970  ue.          typ
-0001add0: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-0001ade0: 2020 7661 6c75 655f 6672 6f6d 3a0a 2020    value_from:.  
-0001adf0: 2020 2020 2020 2020 2472 6566 3a20 2723          $ref: '#
-0001ae00: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-0001ae10: 6d61 732f 456e 7656 6172 536f 7572 6365  mas/EnvVarSource
-0001ae20: 270a 2020 2020 2020 7265 7175 6972 6564  '.      required
-0001ae30: 3a0a 2020 2020 2020 2d20 6e61 6d65 0a20  :.      - name. 
-0001ae40: 2020 2020 2074 6974 6c65 3a20 456e 7656       title: EnvV
-0001ae50: 6172 0a20 2020 2020 2074 7970 653a 206f  ar.      type: o
-0001ae60: 626a 6563 740a 2020 2020 456e 7656 6172  bject.    EnvVar
-0001ae70: 536f 7572 6365 3a0a 2020 2020 2020 7072  Source:.      pr
-0001ae80: 6f70 6572 7469 6573 3a0a 2020 2020 2020  operties:.      
-0001ae90: 2020 6669 656c 645f 7265 663a 0a20 2020    field_ref:.   
-0001aea0: 2020 2020 2020 2024 7265 663a 2027 232f         $ref: '#/
-0001aeb0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-0001aec0: 6173 2f4f 626a 6563 7446 6965 6c64 5365  as/ObjectFieldSe
-0001aed0: 6c65 6374 6f72 270a 2020 2020 2020 7469  lector'.      ti
-0001aee0: 746c 653a 2045 6e76 5661 7253 6f75 7263  tle: EnvVarSourc
-0001aef0: 650a 2020 2020 2020 7479 7065 3a20 6f62  e.      type: ob
-0001af00: 6a65 6374 0a20 2020 204f 626a 6563 7446  ject.    ObjectF
-0001af10: 6965 6c64 5365 6c65 6374 6f72 3a0a 2020  ieldSelector:.  
-0001af20: 2020 2020 7072 6f70 6572 7469 6573 3a0a      properties:.
-0001af30: 2020 2020 2020 2020 6170 695f 7665 7273          api_vers
-0001af40: 696f 6e3a 0a20 2020 2020 2020 2020 2064  ion:.          d
-0001af50: 6573 6372 6970 7469 6f6e 3a20 2256 6572  escription: "Ver
-0001af60: 7369 6f6e 206f 6620 7468 6520 7363 6865  sion of the sche
-0001af70: 6d61 2074 6865 2046 6965 6c64 5061 7468  ma the FieldPath
-0001af80: 2069 7320 7772 6974 7465 6e20 696e 2074   is written in t
-0001af90: 6572 6d73 206f 662c 5c0a 2020 2020 2020  erms of,\.      
-0001afa0: 2020 2020 2020 5c20 6465 6661 756c 7473        \ defaults
-0001afb0: 2074 6f20 5c22 7631 5c22 2e22 0a20 2020   to \"v1\".".   
-0001afc0: 2020 2020 2020 2065 7861 6d70 6c65 3a20         example: 
-0001afd0: 7631 0a20 2020 2020 2020 2020 2074 6974  v1.          tit
-0001afe0: 6c65 3a20 6170 695f 7665 7273 696f 6e0a  le: api_version.
-0001aff0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-0001b000: 7374 7269 6e67 0a20 2020 2020 2020 2066  string.        f
-0001b010: 6965 6c64 5f70 6174 683a 0a20 2020 2020  ield_path:.     
-0001b020: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-0001b030: 3a20 5061 7468 206f 6620 7468 6520 6669  : Path of the fi
-0001b040: 656c 6420 746f 2073 656c 6563 7420 696e  eld to select in
-0001b050: 2074 6865 2073 7065 6369 6669 6564 2041   the specified A
-0001b060: 5049 2076 6572 7369 6f6e 2e0a 2020 2020  PI version..    
-0001b070: 2020 2020 2020 6578 616d 706c 653a 206d        example: m
-0001b080: 6574 6164 6174 612e 6e61 6d65 0a20 2020  etadata.name.   
-0001b090: 2020 2020 2020 2074 6974 6c65 3a20 6669         title: fi
-0001b0a0: 656c 645f 7061 7468 0a20 2020 2020 2020  eld_path.       
-0001b0b0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
-0001b0c0: 2020 2020 2020 7469 746c 653a 204f 626a        title: Obj
-0001b0d0: 6563 7446 6965 6c64 5365 6c65 6374 6f72  ectFieldSelector
-0001b0e0: 0a20 2020 2020 2074 7970 653a 206f 626a  .      type: obj
-0001b0f0: 6563 740a 2020 2020 456e 7646 726f 6d53  ect.    EnvFromS
-0001b100: 6f75 7263 653a 0a20 2020 2020 2064 6573  ource:.      des
-0001b110: 6372 6970 7469 6f6e 3a20 456e 7646 726f  cription: EnvFro
-0001b120: 6d53 6f75 7263 6520 7265 7072 6573 656e  mSource represen
-0001b130: 7473 2074 6865 2073 6f75 7263 6520 6f66  ts the source of
-0001b140: 2061 2073 6574 206f 6620 436f 6e66 6967   a set of Config
-0001b150: 4d61 7073 0a20 2020 2020 2065 7861 6d70  Maps.      examp
-0001b160: 6c65 3a0a 2020 2020 2020 2020 6e61 6d65  le:.        name
-0001b170: 3a20 2f61 7069 2f76 312f 706f 6473 2f73  : /api/v1/pods/s
-0001b180: 6f6d 652d 6e61 6d65 0a20 2020 2020 2020  ome-name.       
-0001b190: 206f 7074 696f 6e61 6c3a 2074 7275 650a   optional: true.
-0001b1a0: 2020 2020 2020 2020 736f 7572 6365 5f74          source_t
-0001b1b0: 7970 653a 2043 6f6e 6669 674d 6170 0a20  ype: ConfigMap. 
-0001b1c0: 2020 2020 2070 726f 7065 7274 6965 733a       properties:
-0001b1d0: 0a20 2020 2020 2020 206e 616d 653a 0a20  .        name:. 
-0001b1e0: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-0001b1f0: 7472 696e 670a 2020 2020 2020 2020 6f70  tring.        op
-0001b200: 7469 6f6e 616c 3a0a 2020 2020 2020 2020  tional:.        
-0001b210: 2020 7479 7065 3a20 626f 6f6c 6561 6e0a    type: boolean.
-0001b220: 2020 2020 2020 2020 736f 7572 6365 5f74          source_t
-0001b230: 7970 653a 0a20 2020 2020 2020 2020 2065  ype:.          e
-0001b240: 6e75 6d3a 0a20 2020 2020 2020 2020 202d  num:.          -
-0001b250: 2043 6f6e 6669 674d 6170 0a20 2020 2020   ConfigMap.     
-0001b260: 2020 2020 202d 2053 6563 7265 740a 2020       - Secret.  
-0001b270: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
-0001b280: 7269 6e67 0a20 2020 2020 2074 6974 6c65  ring.      title
-0001b290: 3a20 456e 7646 726f 6d53 6f75 7263 650a  : EnvFromSource.
-0001b2a0: 2020 2020 2020 7479 7065 3a20 6f62 6a65        type: obje
-0001b2b0: 6374 0a20 2020 2043 6f6e 7461 696e 6572  ct.    Container
-0001b2c0: 5365 6343 6f6e 7465 7874 3a0a 2020 2020  SecContext:.    
-0001b2d0: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
-0001b2e0: 6865 2073 6563 7572 6974 7920 636f 6e66  he security conf
-0001b2f0: 6967 7572 6174 696f 6e20 7468 6174 2077  iguration that w
-0001b300: 696c 6c20 6265 2061 7070 6c69 6564 2074  ill be applied t
-0001b310: 6f20 6120 636f 6e74 6169 6e65 722e 0a20  o a container.. 
-0001b320: 2020 2020 2065 7861 6d70 6c65 3a0a 2020       example:.  
-0001b330: 2020 2020 2020 6361 7061 6269 6c69 7469        capabiliti
-0001b340: 6573 3a0a 2020 2020 2020 2020 2020 6164  es:.          ad
-0001b350: 643a 0a20 2020 2020 2020 2020 202d 204e  d:.          - N
-0001b360: 4554 5f41 444d 494e 0a20 2020 2020 2020  ET_ADMIN.       
-0001b370: 2020 202d 2053 5953 5f54 494d 450a 2020     - SYS_TIME.  
-0001b380: 2020 2020 2020 2020 6472 6f70 3a0a 2020          drop:.  
-0001b390: 2020 2020 2020 2020 2d20 4e45 545f 4144          - NET_AD
-0001b3a0: 4d49 4e0a 2020 2020 2020 2020 2020 2d20  MIN.          - 
-0001b3b0: 5359 535f 5449 4d45 0a20 2020 2020 2020  SYS_TIME.       
-0001b3c0: 2072 756e 5f61 735f 6772 6f75 703a 2033   run_as_group: 3
-0001b3d0: 3030 300a 2020 2020 2020 2020 7275 6e5f  000.        run_
-0001b3e0: 6173 5f75 7365 723a 2031 3030 300a 2020  as_user: 1000.  
-0001b3f0: 2020 2020 7072 6f70 6572 7469 6573 3a0a      properties:.
-0001b400: 2020 2020 2020 2020 7275 6e5f 6173 5f75          run_as_u
-0001b410: 7365 723a 0a20 2020 2020 2020 2020 2064  ser:.          d
-0001b420: 6573 6372 6970 7469 6f6e 3a20 5468 6520  escription: The 
-0001b430: 5549 4420 746f 2072 756e 2074 6865 2065  UID to run the e
-0001b440: 6e74 7279 706f 696e 7420 6f66 2074 6865  ntrypoint of the
-0001b450: 2063 6f6e 7461 696e 6572 2070 726f 6365   container proce
-0001b460: 7373 2e0a 2020 2020 2020 2020 2020 6578  ss..          ex
-0001b470: 616d 706c 653a 2031 3030 300a 2020 2020  ample: 1000.    
-0001b480: 2020 2020 2020 7469 746c 653a 2072 756e        title: run
-0001b490: 5f61 735f 7573 6572 0a20 2020 2020 2020  _as_user.       
-0001b4a0: 2020 2074 7970 653a 2069 6e74 6567 6572     type: integer
-0001b4b0: 0a20 2020 2020 2020 2072 756e 5f61 735f  .        run_as_
-0001b4c0: 6772 6f75 703a 0a20 2020 2020 2020 2020  group:.         
-0001b4d0: 2064 6573 6372 6970 7469 6f6e 3a20 5468   description: Th
-0001b4e0: 6520 4749 4420 746f 2072 756e 2074 6865  e GID to run the
-0001b4f0: 2065 6e74 7279 706f 696e 7420 6f66 2074   entrypoint of t
-0001b500: 6865 2063 6f6e 7461 696e 6572 2070 726f  he container pro
-0001b510: 6365 7373 2e0a 2020 2020 2020 2020 2020  cess..          
-0001b520: 6578 616d 706c 653a 2033 3030 300a 2020  example: 3000.  
-0001b530: 2020 2020 2020 2020 7469 746c 653a 2072          title: r
-0001b540: 756e 5f61 735f 6772 6f75 700a 2020 2020  un_as_group.    
-0001b550: 2020 2020 2020 7479 7065 3a20 696e 7465        type: inte
-0001b560: 6765 720a 2020 2020 2020 2020 6361 7061  ger.        capa
-0001b570: 6269 6c69 7469 6573 3a0a 2020 2020 2020  bilities:.      
-0001b580: 2020 2020 2472 6566 3a20 2723 2f63 6f6d      $ref: '#/com
-0001b590: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-0001b5a0: 436f 6e74 6169 6e65 7253 6563 436f 6e74  ContainerSecCont
-0001b5b0: 6578 745f 6361 7061 6269 6c69 7469 6573  ext_capabilities
-0001b5c0: 270a 2020 2020 2020 7469 746c 653a 2043  '.      title: C
-0001b5d0: 6f6e 7461 696e 6572 5365 6343 6f6e 7465  ontainerSecConte
-0001b5e0: 7874 0a20 2020 2020 2074 7970 653a 206f  xt.      type: o
-0001b5f0: 626a 6563 740a 2020 2020 436f 6e74 6169  bject.    Contai
-0001b600: 6e65 724c 6966 6543 7963 6c65 3a0a 2020  nerLifeCycle:.  
-0001b610: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
-0001b620: 2020 2020 2070 7265 5f73 746f 703a 0a20       pre_stop:. 
-0001b630: 2020 2020 2020 2020 2074 6370 5f73 6f63           tcp_soc
-0001b640: 6b65 743a 0a20 2020 2020 2020 2020 2020  ket:.           
-0001b650: 2070 6f72 743a 2033 3031 3831 0a20 2020   port: 30181.   
-0001b660: 2020 2020 2020 2020 2068 6f73 743a 2031           host: 1
-0001b670: 3237 2e30 2e30 2e31 0a20 2020 2020 2020  27.0.0.1.       
-0001b680: 2020 2068 7474 705f 6765 743a 0a20 2020     http_get:.   
-0001b690: 2020 2020 2020 2020 2070 6174 683a 202f           path: /
-0001b6a0: 7368 6f77 3f64 6f6d 6169 6e3d 7631 392e  show?domain=v19.
-0001b6b0: 7469 6b74 6f6b 6364 6e2e 636f 6d0a 2020  tiktokcdn.com.  
-0001b6c0: 2020 2020 2020 2020 2020 6874 7470 5f68            http_h
-0001b6d0: 6561 6465 7273 3a0a 2020 2020 2020 2020  eaders:.        
-0001b6e0: 2020 2020 2d20 782d 6465 7673 7265 2d61      - x-devsre-a
-0001b6f0: 7574 686f 7269 7a61 7469 6f6e 3a42 6561  uthorization:Bea
-0001b700: 7265 7220 6579 4a68 6247 6369 4f69 4a0a  rer eyJhbGciOiJ.
-0001b710: 2020 2020 2020 2020 2020 2020 2d20 636f              - co
-0001b720: 6e74 656e 742d 7479 7065 3a61 7070 6c69  ntent-type:appli
-0001b730: 6361 7469 6f6e 2f6a 736f 6e0a 2020 2020  cation/json.    
-0001b740: 2020 2020 2020 2020 7363 6865 6d65 3a20          scheme: 
-0001b750: 4854 5450 530a 2020 2020 2020 2020 2020  HTTPS.          
-0001b760: 2020 706f 7274 3a20 3838 3838 0a20 2020    port: 8888.   
-0001b770: 2020 2020 2020 2020 2068 6f73 743a 2067           host: g
-0001b780: 7373 2d64 6e73 2d61 6765 6e74 2e65 7861  ss-dns-agent.exa
-0001b790: 6d70 6c65 2e6f 7267 0a20 2020 2020 2020  mple.org.       
-0001b7a0: 2020 2065 7865 635f 636f 6d6d 616e 643a     exec_command:
-0001b7b0: 0a20 2020 2020 2020 2020 202d 202f 6269  .          - /bi
-0001b7c0: 6e2f 7368 6f77 646f 776e 2e73 680a 2020  n/showdown.sh.  
-0001b7d0: 2020 2020 2020 706f 7374 5f73 7461 7274        post_start
-0001b7e0: 3a0a 2020 2020 2020 2020 2020 7463 705f  :.          tcp_
-0001b7f0: 736f 636b 6574 3a0a 2020 2020 2020 2020  socket:.        
-0001b800: 2020 2020 706f 7274 3a20 3330 3138 310a      port: 30181.
-0001b810: 2020 2020 2020 2020 2020 2020 686f 7374              host
-0001b820: 3a20 3132 372e 302e 302e 310a 2020 2020  : 127.0.0.1.    
-0001b830: 2020 2020 2020 6874 7470 5f67 6574 3a0a        http_get:.
-0001b840: 2020 2020 2020 2020 2020 2020 7061 7468              path
-0001b850: 3a20 2f73 686f 773f 646f 6d61 696e 3d76  : /show?domain=v
-0001b860: 3139 2e74 696b 746f 6b63 646e 2e63 6f6d  19.tiktokcdn.com
-0001b870: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
-0001b880: 705f 6865 6164 6572 733a 0a20 2020 2020  p_headers:.     
-0001b890: 2020 2020 2020 202d 2078 2d64 6576 7372         - x-devsr
-0001b8a0: 652d 6175 7468 6f72 697a 6174 696f 6e3a  e-authorization:
-0001b8b0: 4265 6172 6572 2065 794a 6862 4763 694f  Bearer eyJhbGciO
-0001b8c0: 694a 0a20 2020 2020 2020 2020 2020 202d  iJ.            -
-0001b8d0: 2063 6f6e 7465 6e74 2d74 7970 653a 6170   content-type:ap
-0001b8e0: 706c 6963 6174 696f 6e2f 6a73 6f6e 0a20  plication/json. 
-0001b8f0: 2020 2020 2020 2020 2020 2073 6368 656d             schem
-0001b900: 653a 2048 5454 5053 0a20 2020 2020 2020  e: HTTPS.       
-0001b910: 2020 2020 2070 6f72 743a 2038 3838 380a       port: 8888.
-0001b920: 2020 2020 2020 2020 2020 2020 686f 7374              host
-0001b930: 3a20 6773 732d 646e 732d 6167 656e 742e  : gss-dns-agent.
-0001b940: 6578 616d 706c 652e 6f72 670a 2020 2020  example.org.    
-0001b950: 2020 2020 2020 6578 6563 5f63 6f6d 6d61        exec_comma
-0001b960: 6e64 3a0a 2020 2020 2020 2020 2020 2d20  nd:.          - 
-0001b970: 2f62 696e 2f73 686f 7764 6f77 6e2e 7368  /bin/showdown.sh
-0001b980: 0a20 2020 2020 2070 726f 7065 7274 6965  .      propertie
-0001b990: 733a 0a20 2020 2020 2020 2070 6f73 745f  s:.        post_
-0001b9a0: 7374 6172 743a 0a20 2020 2020 2020 2020  start:.         
-0001b9b0: 2024 7265 663a 2027 232f 636f 6d70 6f6e   $ref: '#/compon
-0001b9c0: 656e 7473 2f73 6368 656d 6173 2f4c 6966  ents/schemas/Lif
-0001b9d0: 6543 7963 6c65 4861 6e64 6c65 7227 0a20  eCycleHandler'. 
-0001b9e0: 2020 2020 2020 2070 7265 5f73 746f 703a         pre_stop:
-0001b9f0: 0a20 2020 2020 2020 2020 2024 7265 663a  .          $ref:
-0001ba00: 2027 232f 636f 6d70 6f6e 656e 7473 2f73   '#/components/s
-0001ba10: 6368 656d 6173 2f4c 6966 6543 7963 6c65  chemas/LifeCycle
-0001ba20: 4861 6e64 6c65 7227 0a20 2020 2020 2074  Handler'.      t
-0001ba30: 6974 6c65 3a20 436f 6e74 6169 6e65 724c  itle: ContainerL
-0001ba40: 6966 6543 7963 6c65 0a20 2020 2020 2074  ifeCycle.      t
-0001ba50: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
-0001ba60: 4c69 6665 4379 636c 6548 616e 646c 6572  LifeCycleHandler
-0001ba70: 3a0a 2020 2020 2020 6578 616d 706c 653a  :.      example:
-0001ba80: 0a20 2020 2020 2020 2074 6370 5f73 6f63  .        tcp_soc
-0001ba90: 6b65 743a 0a20 2020 2020 2020 2020 2070  ket:.          p
-0001baa0: 6f72 743a 2033 3031 3831 0a20 2020 2020  ort: 30181.     
-0001bab0: 2020 2020 2068 6f73 743a 2031 3237 2e30       host: 127.0
-0001bac0: 2e30 2e31 0a20 2020 2020 2020 2068 7474  .0.1.        htt
-0001bad0: 705f 6765 743a 0a20 2020 2020 2020 2020  p_get:.         
-0001bae0: 2070 6174 683a 202f 7368 6f77 3f64 6f6d   path: /show?dom
-0001baf0: 6169 6e3d 7631 392e 7469 6b74 6f6b 6364  ain=v19.tiktokcd
-0001bb00: 6e2e 636f 6d0a 2020 2020 2020 2020 2020  n.com.          
-0001bb10: 6874 7470 5f68 6561 6465 7273 3a0a 2020  http_headers:.  
-0001bb20: 2020 2020 2020 2020 2d20 782d 6465 7673          - x-devs
-0001bb30: 7265 2d61 7574 686f 7269 7a61 7469 6f6e  re-authorization
-0001bb40: 3a42 6561 7265 7220 6579 4a68 6247 6369  :Bearer eyJhbGci
-0001bb50: 4f69 4a0a 2020 2020 2020 2020 2020 2d20  OiJ.          - 
-0001bb60: 636f 6e74 656e 742d 7479 7065 3a61 7070  content-type:app
-0001bb70: 6c69 6361 7469 6f6e 2f6a 736f 6e0a 2020  lication/json.  
-0001bb80: 2020 2020 2020 2020 7363 6865 6d65 3a20          scheme: 
-0001bb90: 4854 5450 530a 2020 2020 2020 2020 2020  HTTPS.          
-0001bba0: 706f 7274 3a20 3838 3838 0a20 2020 2020  port: 8888.     
-0001bbb0: 2020 2020 2068 6f73 743a 2067 7373 2d64       host: gss-d
-0001bbc0: 6e73 2d61 6765 6e74 2e65 7861 6d70 6c65  ns-agent.example
-0001bbd0: 2e6f 7267 0a20 2020 2020 2020 2065 7865  .org.        exe
-0001bbe0: 635f 636f 6d6d 616e 643a 0a20 2020 2020  c_command:.     
-0001bbf0: 2020 202d 202f 6269 6e2f 7368 6f77 646f     - /bin/showdo
-0001bc00: 776e 2e73 680a 2020 2020 2020 7072 6f70  wn.sh.      prop
-0001bc10: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
-0001bc20: 6578 6563 5f63 6f6d 6d61 6e64 3a0a 2020  exec_command:.  
-0001bc30: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-0001bc40: 696f 6e3a 2043 6f6d 6d61 6e64 206c 696e  ion: Command lin
-0001bc50: 6520 746f 2065 7865 6375 7465 2069 6e73  e to execute ins
-0001bc60: 6964 6520 7468 6520 636f 6e74 6169 6e65  ide the containe
-0001bc70: 720a 2020 2020 2020 2020 2020 6578 616d  r.          exam
-0001bc80: 706c 653a 0a20 2020 2020 2020 2020 202d  ple:.          -
-0001bc90: 202f 6269 6e2f 7368 6f77 646f 776e 2e73   /bin/showdown.s
-0001bca0: 680a 2020 2020 2020 2020 2020 6974 656d  h.          item
-0001bcb0: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-0001bcc0: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
-0001bcd0: 2020 2020 2020 7469 746c 653a 2065 7865        title: exe
-0001bce0: 635f 636f 6d6d 616e 640a 2020 2020 2020  c_command.      
-0001bcf0: 2020 2020 7479 7065 3a20 6172 7261 790a      type: array.
-0001bd00: 2020 2020 2020 2020 6874 7470 5f67 6574          http_get
-0001bd10: 3a0a 2020 2020 2020 2020 2020 2472 6566  :.          $ref
-0001bd20: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
-0001bd30: 7363 6865 6d61 732f 4874 7470 4765 7427  schemas/HttpGet'
-0001bd40: 0a20 2020 2020 2020 2074 6370 5f73 6f63  .        tcp_soc
-0001bd50: 6b65 743a 0a20 2020 2020 2020 2020 2024  ket:.          $
-0001bd60: 7265 663a 2027 232f 636f 6d70 6f6e 656e  ref: '#/componen
-0001bd70: 7473 2f73 6368 656d 6173 2f54 6370 536f  ts/schemas/TcpSo
-0001bd80: 636b 6574 270a 2020 2020 2020 7469 746c  cket'.      titl
-0001bd90: 653a 204c 6966 6543 7963 6c65 4861 6e64  e: LifeCycleHand
-0001bda0: 6c65 720a 2020 2020 2020 7479 7065 3a20  ler.      type: 
-0001bdb0: 6f62 6a65 6374 0a20 2020 2048 7474 7047  object.    HttpG
-0001bdc0: 6574 3a0a 2020 2020 2020 6578 616d 706c  et:.      exampl
-0001bdd0: 653a 0a20 2020 2020 2020 2070 6174 683a  e:.        path:
-0001bde0: 202f 7368 6f77 3f64 6f6d 6169 6e3d 7631   /show?domain=v1
-0001bdf0: 392e 7469 6b74 6f6b 6364 6e2e 636f 6d0a  9.tiktokcdn.com.
-0001be00: 2020 2020 2020 2020 6874 7470 5f68 6561          http_hea
-0001be10: 6465 7273 3a0a 2020 2020 2020 2020 2d20  ders:.        - 
-0001be20: 782d 6465 7673 7265 2d61 7574 686f 7269  x-devsre-authori
-0001be30: 7a61 7469 6f6e 3a42 6561 7265 7220 6579  zation:Bearer ey
-0001be40: 4a68 6247 6369 4f69 4a0a 2020 2020 2020  JhbGciOiJ.      
-0001be50: 2020 2d20 636f 6e74 656e 742d 7479 7065    - content-type
-0001be60: 3a61 7070 6c69 6361 7469 6f6e 2f6a 736f  :application/jso
-0001be70: 6e0a 2020 2020 2020 2020 7363 6865 6d65  n.        scheme
-0001be80: 3a20 4854 5450 530a 2020 2020 2020 2020  : HTTPS.        
-0001be90: 706f 7274 3a20 3838 3838 0a20 2020 2020  port: 8888.     
-0001bea0: 2020 2068 6f73 743a 2067 7373 2d64 6e73     host: gss-dns
-0001beb0: 2d61 6765 6e74 2e65 7861 6d70 6c65 2e6f  -agent.example.o
-0001bec0: 7267 0a20 2020 2020 2070 726f 7065 7274  rg.      propert
-0001bed0: 6965 733a 0a20 2020 2020 2020 2070 6f72  ies:.        por
-0001bee0: 743a 0a20 2020 2020 2020 2020 2064 6573  t:.          des
-0001bef0: 6372 6970 7469 6f6e 3a20 4e75 6d62 6572  cription: Number
-0001bf00: 206f 6620 7468 6520 706f 7274 2074 6f20   of the port to 
-0001bf10: 6163 6365 7373 206f 6e20 7468 6520 636f  access on the co
-0001bf20: 6e74 6169 6e65 722e 0a20 2020 2020 2020  ntainer..       
-0001bf30: 2020 2065 7861 6d70 6c65 3a20 3838 3838     example: 8888
-0001bf40: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
-0001bf50: 3a20 706f 7274 0a20 2020 2020 2020 2020  : port.         
-0001bf60: 2074 7970 653a 2069 6e74 6567 6572 0a20   type: integer. 
-0001bf70: 2020 2020 2020 2068 6f73 743a 0a20 2020         host:.   
-0001bf80: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-0001bf90: 6f6e 3a20 2248 6f73 7420 6e61 6d65 2074  on: "Host name t
-0001bfa0: 6f20 636f 6e6e 6563 7420 746f 2c20 6465  o connect to, de
-0001bfb0: 6661 756c 7473 2074 6f20 7468 6520 706f  faults to the po
-0001bfc0: 6420 4950 2e22 0a20 2020 2020 2020 2020  d IP.".         
-0001bfd0: 2065 7861 6d70 6c65 3a20 6773 732d 646e   example: gss-dn
-0001bfe0: 732d 6167 656e 742e 6578 616d 706c 652e  s-agent.example.
-0001bff0: 6f72 670a 2020 2020 2020 2020 2020 7469  org.          ti
-0001c000: 746c 653a 2068 6f73 740a 2020 2020 2020  tle: host.      
-0001c010: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-0001c020: 0a20 2020 2020 2020 2068 7474 705f 6865  .        http_he
-0001c030: 6164 6572 733a 0a20 2020 2020 2020 2020  aders:.         
-0001c040: 2064 6573 6372 6970 7469 6f6e 3a20 4375   description: Cu
-0001c050: 7374 6f6d 2068 6561 6465 7273 2074 6f20  stom headers to 
-0001c060: 7365 7420 696e 2074 6865 2072 6571 7565  set in the reque
-0001c070: 7374 2e0a 2020 2020 2020 2020 2020 6578  st..          ex
-0001c080: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
-0001c090: 202d 2078 2d64 6576 7372 652d 6175 7468   - x-devsre-auth
-0001c0a0: 6f72 697a 6174 696f 6e3a 4265 6172 6572  orization:Bearer
-0001c0b0: 2065 794a 6862 4763 694f 694a 0a20 2020   eyJhbGciOiJ.   
-0001c0c0: 2020 2020 2020 202d 2063 6f6e 7465 6e74         - content
-0001c0d0: 2d74 7970 653a 6170 706c 6963 6174 696f  -type:applicatio
-0001c0e0: 6e2f 6a73 6f6e 0a20 2020 2020 2020 2020  n/json.         
-0001c0f0: 2069 7465 6d73 3a0a 2020 2020 2020 2020   items:.        
-0001c100: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-0001c110: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
-0001c120: 3a20 6874 7470 5f68 6561 6465 7273 0a20  : http_headers. 
-0001c130: 2020 2020 2020 2020 2074 7970 653a 2061           type: a
-0001c140: 7272 6179 0a20 2020 2020 2020 2070 6174  rray.        pat
-0001c150: 683a 0a20 2020 2020 2020 2020 2064 6573  h:.          des
-0001c160: 6372 6970 7469 6f6e 3a20 5061 7468 2074  cription: Path t
-0001c170: 6f20 6163 6365 7373 206f 6e20 7468 6520  o access on the 
-0001c180: 4854 5450 2073 6572 7665 722e 0a20 2020  HTTP server..   
-0001c190: 2020 2020 2020 2065 7861 6d70 6c65 3a20         example: 
-0001c1a0: 2f73 686f 773f 646f 6d61 696e 3d76 3139  /show?domain=v19
-0001c1b0: 2e74 696b 746f 6b63 646e 2e63 6f6d 0a20  .tiktokcdn.com. 
-0001c1c0: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-0001c1d0: 7061 7468 0a20 2020 2020 2020 2020 2074  path.          t
-0001c1e0: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
-0001c1f0: 2020 2020 7363 6865 6d65 3a0a 2020 2020      scheme:.    
-0001c200: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-0001c210: 6e3a 2053 6368 656d 6520 746f 2075 7365  n: Scheme to use
-0001c220: 2066 6f72 2063 6f6e 6e65 6374 696e 6720   for connecting 
-0001c230: 746f 2074 6865 2068 6f73 742e 2044 6566  to the host. Def
-0001c240: 6175 6c74 7320 746f 2048 5454 502e 0a20  aults to HTTP.. 
-0001c250: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
-0001c260: 3a20 4854 5450 530a 2020 2020 2020 2020  : HTTPS.        
-0001c270: 2020 7469 746c 653a 2073 6368 656d 650a    title: scheme.
-0001c280: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-0001c290: 7374 7269 6e67 0a20 2020 2020 2072 6571  string.      req
-0001c2a0: 7569 7265 643a 0a20 2020 2020 202d 2070  uired:.      - p
-0001c2b0: 6f72 740a 2020 2020 2020 7469 746c 653a  ort.      title:
-0001c2c0: 2048 7474 7047 6574 0a20 2020 2020 2074   HttpGet.      t
-0001c2d0: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
-0001c2e0: 5463 7053 6f63 6b65 743a 0a20 2020 2020  TcpSocket:.     
-0001c2f0: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
-0001c300: 2020 706f 7274 3a20 3330 3138 310a 2020    port: 30181.  
-0001c310: 2020 2020 2020 686f 7374 3a20 3132 372e        host: 127.
-0001c320: 302e 302e 310a 2020 2020 2020 7072 6f70  0.0.1.      prop
-0001c330: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
-0001c340: 706f 7274 3a0a 2020 2020 2020 2020 2020  port:.          
-0001c350: 6465 7363 7269 7074 696f 6e3a 204e 756d  description: Num
-0001c360: 6265 7220 6f66 2074 6865 2070 6f72 7420  ber of the port 
-0001c370: 746f 2061 6363 6573 7320 6f6e 2074 6865  to access on the
-0001c380: 2063 6f6e 7461 696e 6572 2e0a 2020 2020   container..    
-0001c390: 2020 2020 2020 6578 616d 706c 653a 2033        example: 3
-0001c3a0: 3031 3831 0a20 2020 2020 2020 2020 2074  0181.          t
-0001c3b0: 6974 6c65 3a20 706f 7274 0a20 2020 2020  itle: port.     
-0001c3c0: 2020 2020 2074 7970 653a 2069 6e74 6567       type: integ
-0001c3d0: 6572 0a20 2020 2020 2020 2068 6f73 743a  er.        host:
-0001c3e0: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
-0001c3f0: 6970 7469 6f6e 3a20 2248 6f73 7420 6e61  iption: "Host na
-0001c400: 6d65 2074 6f20 636f 6e6e 6563 7420 746f  me to connect to
-0001c410: 2c20 6465 6661 756c 7473 2074 6f20 7468  , defaults to th
-0001c420: 6520 706f 6420 4950 2e22 0a20 2020 2020  e pod IP.".     
-0001c430: 2020 2020 2065 7861 6d70 6c65 3a20 3132       example: 12
-0001c440: 372e 302e 302e 310a 2020 2020 2020 2020  7.0.0.1.        
-0001c450: 2020 7469 746c 653a 2068 6f73 740a 2020    title: host.  
-0001c460: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
-0001c470: 7269 6e67 0a20 2020 2020 2072 6571 7569  ring.      requi
-0001c480: 7265 643a 0a20 2020 2020 202d 2070 6f72  red:.      - por
-0001c490: 740a 2020 2020 2020 7469 746c 653a 2054  t.      title: T
-0001c4a0: 6370 536f 636b 6574 0a20 2020 2020 2074  cpSocket.      t
-0001c4b0: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
-0001c4c0: 436f 6e74 6169 6e65 7250 6f72 743a 0a20  ContainerPort:. 
-0001c4d0: 2020 2020 2065 7861 6d70 6c65 3a0a 2020       example:.  
-0001c4e0: 2020 2020 2020 636f 6e74 6169 6e65 725f        container_
-0001c4f0: 706f 7274 3a20 3830 0a20 2020 2020 2020  port: 80.       
-0001c500: 2070 726f 746f 636f 6c3a 2054 4350 0a20   protocol: TCP. 
-0001c510: 2020 2020 2020 206e 616d 653a 2068 7474         name: htt
-0001c520: 700a 2020 2020 2020 7072 6f70 6572 7469  p.      properti
-0001c530: 6573 3a0a 2020 2020 2020 2020 6e61 6d65  es:.        name
-0001c540: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
-0001c550: 7269 7074 696f 6e3a 2022 436f 6e74 6169  ription: "Contai
-0001c560: 6e65 7220 706f 7274 206e 616d 652c 2069  ner port name, i
-0001c570: 6620 7370 6563 6966 6965 642c 2074 6869  f specified, thi
-0001c580: 7320 6d75 7374 2062 6520 616e 2049 414e  s must be an IAN
-0001c590: 415f 5356 435f 4e41 4d45 5c0a 2020 2020  A_SVC_NAME\.    
-0001c5a0: 2020 2020 2020 2020 5c20 616e 6420 756e          \ and un
-0001c5b0: 6971 7565 2077 6974 6869 6e20 7468 6520  ique within the 
-0001c5c0: 706f 6422 0a20 2020 2020 2020 2020 2065  pod".          e
-0001c5d0: 7861 6d70 6c65 3a20 6874 7470 0a20 2020  xample: http.   
-0001c5e0: 2020 2020 2020 2074 6974 6c65 3a20 6e61         title: na
-0001c5f0: 6d65 0a20 2020 2020 2020 2020 2074 7970  me.          typ
-0001c600: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-0001c610: 2020 636f 6e74 6169 6e65 725f 706f 7274    container_port
-0001c620: 3a0a 2020 2020 2020 2020 2020 6578 616d  :.          exam
-0001c630: 706c 653a 2038 300a 2020 2020 2020 2020  ple: 80.        
-0001c640: 2020 7469 746c 653a 2063 6f6e 7461 696e    title: contain
-0001c650: 6572 5f70 6f72 740a 2020 2020 2020 2020  er_port.        
-0001c660: 2020 7479 7065 3a20 696e 7465 6765 720a    type: integer.
-0001c670: 2020 2020 2020 2020 7072 6f74 6f63 6f6c          protocol
-0001c680: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
-0001c690: 7269 7074 696f 6e3a 2044 6566 6175 6c74  ription: Default
-0001c6a0: 7320 746f 2054 4350 0a20 2020 2020 2020  s to TCP.       
-0001c6b0: 2020 2065 6e75 6d3a 0a20 2020 2020 2020     enum:.       
-0001c6c0: 2020 202d 2054 4350 0a20 2020 2020 2020     - TCP.       
-0001c6d0: 2020 202d 2055 4450 0a20 2020 2020 2020     - UDP.       
-0001c6e0: 2020 2065 7861 6d70 6c65 3a20 5443 500a     example: TCP.
-0001c6f0: 2020 2020 2020 2020 2020 7469 746c 653a            title:
-0001c700: 2070 726f 746f 636f 6c0a 2020 2020 2020   protocol.      
-0001c710: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-0001c720: 0a20 2020 2020 2072 6571 7569 7265 643a  .      required:
-0001c730: 0a20 2020 2020 202d 206e 616d 650a 2020  .      - name.  
-0001c740: 2020 2020 7469 746c 653a 2043 6f6e 7461      title: Conta
-0001c750: 696e 6572 506f 7274 0a20 2020 2020 2074  inerPort.      t
-0001c760: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
-0001c770: 566f 6c75 6d65 4d6f 756e 743a 0a20 2020  VolumeMount:.   
-0001c780: 2020 2065 7861 6d70 6c65 3a0a 2020 2020     example:.    
-0001c790: 2020 2020 7061 7468 3a20 2f6f 7074 2f73      path: /opt/s
-0001c7a0: 6572 7665 722f 636f 6e66 0a20 2020 2020  erver/conf.     
-0001c7b0: 2020 2072 6561 645f 6f6e 6c79 3a20 7472     read_only: tr
-0001c7c0: 7565 0a20 2020 2020 2020 206e 616d 653a  ue.        name:
-0001c7d0: 2064 656d 6f2d 766f 6c0a 2020 2020 2020   demo-vol.      
-0001c7e0: 2020 7375 625f 7061 7468 3a20 7365 7276    sub_path: serv
-0001c7f0: 6572 2e63 6f6e 660a 2020 2020 2020 7072  er.conf.      pr
-0001c800: 6f70 6572 7469 6573 3a0a 2020 2020 2020  operties:.      
-0001c810: 2020 6e61 6d65 3a0a 2020 2020 2020 2020    name:.        
-0001c820: 2020 6465 7363 7269 7074 696f 6e3a 204d    description: M
-0001c830: 7573 7420 6d61 7463 6820 7468 6520 4e61  ust match the Na
-0001c840: 6d65 206f 6620 6120 566f 6c75 6d65 0a20  me of a Volume. 
-0001c850: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
-0001c860: 3a20 6465 6d6f 2d76 6f6c 0a20 2020 2020  : demo-vol.     
-0001c870: 2020 2020 2074 6974 6c65 3a20 6e61 6d65       title: name
-0001c880: 0a20 2020 2020 2020 2070 6174 683a 0a20  .        path:. 
-0001c890: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-0001c8a0: 7469 6f6e 3a20 5061 7468 2077 6974 6869  tion: Path withi
-0001c8b0: 6e20 7468 6520 636f 6e74 6169 6e65 7220  n the container 
-0001c8c0: 6174 2077 6869 6368 2074 6865 2076 6f6c  at which the vol
-0001c8d0: 756d 6520 7368 6f75 6c64 2062 6520 6d6f  ume should be mo
-0001c8e0: 756e 7465 640a 2020 2020 2020 2020 2020  unted.          
-0001c8f0: 6578 616d 706c 653a 202f 6f70 742f 7365  example: /opt/se
-0001c900: 7276 6572 2f63 6f6e 660a 2020 2020 2020  rver/conf.      
-0001c910: 2020 2020 7469 746c 653a 2070 6174 680a      title: path.
-0001c920: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-0001c930: 7374 7269 6e67 0a20 2020 2020 2020 2073  string.        s
-0001c940: 7562 5f70 6174 683a 0a20 2020 2020 2020  ub_path:.       
-0001c950: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-0001c960: 5061 7468 2077 6974 6869 6e20 7468 6520  Path within the 
-0001c970: 766f 6c75 6d65 2066 726f 6d20 7768 6963  volume from whic
-0001c980: 6820 7468 6520 636f 6e74 6169 6e65 7227  h the container'
-0001c990: 7320 766f 6c75 6d65 2073 686f 756c 640a  s volume should.
-0001c9a0: 2020 2020 2020 2020 2020 2020 6265 206d              be m
-0001c9b0: 6f75 6e74 6564 0a20 2020 2020 2020 2020  ounted.         
-0001c9c0: 2065 7861 6d70 6c65 3a20 7365 7276 6572   example: server
-0001c9d0: 2e63 6f6e 660a 2020 2020 2020 2020 2020  .conf.          
-0001c9e0: 7469 746c 653a 2073 7562 5f70 6174 680a  title: sub_path.
-0001c9f0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-0001ca00: 7374 7269 6e67 0a20 2020 2020 2020 2072  string.        r
-0001ca10: 6561 645f 6f6e 6c79 3a0a 2020 2020 2020  ead_only:.      
-0001ca20: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-0001ca30: 2057 696c 6c20 666f 7263 6520 7468 6520   Will force the 
-0001ca40: 5265 6164 4f6e 6c79 2073 6574 7469 6e67  ReadOnly setting
-0001ca50: 2069 6e20 566f 6c75 6d65 4d6f 756e 7473   in VolumeMounts
-0001ca60: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-0001ca70: 6c65 3a20 7472 7565 0a20 2020 2020 2020  le: true.       
-0001ca80: 2020 2074 6974 6c65 3a20 7265 6164 5f6f     title: read_o
-0001ca90: 6e6c 790a 2020 2020 2020 2020 2020 7479  nly.          ty
-0001caa0: 7065 3a20 626f 6f6c 6561 6e0a 2020 2020  pe: boolean.    
-0001cab0: 2020 7265 7175 6972 6564 3a0a 2020 2020    required:.    
-0001cac0: 2020 2d20 6e61 6d65 0a20 2020 2020 2074    - name.      t
-0001cad0: 6974 6c65 3a20 566f 6c75 6d65 4d6f 756e  itle: VolumeMoun
-0001cae0: 740a 2020 2020 2020 7479 7065 3a20 6f62  t.      type: ob
-0001caf0: 6a65 6374 0a20 2020 2056 6f6c 756d 6544  ject.    VolumeD
-0001cb00: 6576 6963 653a 0a20 2020 2020 2065 7861  evice:.      exa
-0001cb10: 6d70 6c65 3a0a 2020 2020 2020 2020 6e61  mple:.        na
-0001cb20: 6d65 3a20 6465 6d6f 2d76 6f6c 0a20 2020  me: demo-vol.   
-0001cb30: 2020 2020 2064 6576 6963 655f 7061 7468       device_path
-0001cb40: 3a20 2f64 6576 2f73 6461 310a 2020 2020  : /dev/sda1.    
-0001cb50: 2020 2020 6263 6163 6865 5f6e 756d 733a      bcache_nums:
-0001cb60: 2034 0a20 2020 2020 2070 726f 7065 7274   4.      propert
-0001cb70: 6965 733a 0a20 2020 2020 2020 206e 616d  ies:.        nam
-0001cb80: 653a 0a20 2020 2020 2020 2020 2064 6573  e:.          des
-0001cb90: 6372 6970 7469 6f6e 3a20 4d75 7374 206d  cription: Must m
-0001cba0: 6174 6368 2074 6865 204e 616d 6520 6f66  atch the Name of
-0001cbb0: 2061 2056 6f6c 756d 650a 2020 2020 2020   a Volume.      
-0001cbc0: 2020 2020 6578 616d 706c 653a 2064 656d      example: dem
-0001cbd0: 6f2d 766f 6c0a 2020 2020 2020 2020 2020  o-vol.          
-0001cbe0: 7469 746c 653a 206e 616d 650a 2020 2020  title: name.    
-0001cbf0: 2020 2020 6465 7669 6365 5f70 6174 683a      device_path:
-0001cc00: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
-0001cc10: 6970 7469 6f6e 3a20 5061 7468 206f 6620  iption: Path of 
-0001cc20: 7468 6520 6465 7669 6365 2077 6974 6869  the device withi
-0001cc30: 6e20 7468 6520 636f 6e74 6169 6e65 720a  n the container.
-0001cc40: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
-0001cc50: 653a 202f 6465 762f 7364 6131 0a20 2020  e: /dev/sda1.   
-0001cc60: 2020 2020 2020 2074 6974 6c65 3a20 6465         title: de
-0001cc70: 7669 6365 5f70 6174 680a 2020 2020 2020  vice_path.      
-0001cc80: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-0001cc90: 0a20 2020 2020 2020 2062 6361 6368 655f  .        bcache_
-0001cca0: 6e75 6d73 3a0a 2020 2020 2020 2020 2020  nums:.          
-0001ccb0: 6465 7363 7269 7074 696f 6e3a 2055 7365  description: Use
-0001ccc0: 6420 666f 7220 4154 5320 6465 706c 6f79  d for ATS deploy
-0001ccd0: 6d65 6e74 2074 6f20 6175 746f 6d61 7469  ment to automati
-0001cce0: 6361 6c6c 7920 6765 6e65 7261 7465 2062  cally generate b
-0001ccf0: 6361 6368 655f 6e75 6d73 0a20 2020 2020  cache_nums.     
-0001cd00: 2020 2020 2020 2076 6f6c 756d 6520 6465         volume de
-0001cd10: 7669 6365 7320 616e 6420 7265 6c61 7465  vices and relate
-0001cd20: 6420 636f 6e74 656e 7473 2e0a 2020 2020  d contents..    
-0001cd30: 2020 2020 2020 6578 616d 706c 653a 2034        example: 4
-0001cd40: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
-0001cd50: 3a20 6263 6163 6865 5f6e 756d 730a 2020  : bcache_nums.  
-0001cd60: 2020 2020 2020 2020 7479 7065 3a20 696e          type: in
-0001cd70: 7465 6765 720a 2020 2020 2020 7265 7175  teger.      requ
-0001cd80: 6972 6564 3a0a 2020 2020 2020 2d20 6e61  ired:.      - na
-0001cd90: 6d65 0a20 2020 2020 2074 6974 6c65 3a20  me.      title: 
-0001cda0: 566f 6c75 6d65 4465 7669 6365 0a20 2020  VolumeDevice.   
-0001cdb0: 2020 2074 7970 653a 206f 626a 6563 740a     type: object.
-0001cdc0: 2020 2020 5265 736f 7572 6365 5265 7175      ResourceRequ
-0001cdd0: 6972 656d 656e 7473 3a0a 2020 2020 2020  irements:.      
-0001cde0: 6578 616d 706c 653a 0a20 2020 2020 2020  example:.       
-0001cdf0: 2072 6571 7565 7374 733a 0a20 2020 2020   requests:.     
-0001ce00: 2020 2020 206d 656d 6f72 793a 2032 3536       memory: 256
-0001ce10: 4d69 0a20 2020 2020 2020 2020 2063 7075  Mi.          cpu
-0001ce20: 3a20 2230 2e31 220a 2020 2020 2020 2020  : "0.1".        
-0001ce30: 6c69 6d69 7473 3a0a 2020 2020 2020 2020  limits:.        
-0001ce40: 2020 6d65 6d6f 7279 3a20 3531 324d 690a    memory: 512Mi.
-0001ce50: 2020 2020 2020 2020 2020 6370 753a 2022            cpu: "
-0001ce60: 302e 3522 0a20 2020 2020 2070 726f 7065  0.5".      prope
-0001ce70: 7274 6965 733a 0a20 2020 2020 2020 206c  rties:.        l
-0001ce80: 696d 6974 733a 0a20 2020 2020 2020 2020  imits:.         
-0001ce90: 2061 6464 6974 696f 6e61 6c50 726f 7065   additionalPrope
-0001cea0: 7274 6965 733a 0a20 2020 2020 2020 2020  rties:.         
-0001ceb0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
-0001cec0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-0001ced0: 7074 696f 6e3a 2075 7365 6420 746f 2073  ption: used to s
-0001cee0: 7065 6369 6679 2074 6865 206d 6178 696d  pecify the maxim
-0001cef0: 756d 2061 6d6f 756e 7420 6f66 2072 6573  um amount of res
-0001cf00: 6f75 7263 6573 2074 6861 7420 6361 6e20  ources that can 
-0001cf10: 6265 0a20 2020 2020 2020 2020 2020 2063  be.            c
-0001cf20: 6f6e 7375 6d65 642e 0a20 2020 2020 2020  onsumed..       
-0001cf30: 2020 2065 7861 6d70 6c65 3a0a 2020 2020     example:.    
-0001cf40: 2020 2020 2020 2020 6d65 6d6f 7279 3a20          memory: 
-0001cf50: 3531 324d 690a 2020 2020 2020 2020 2020  512Mi.          
-0001cf60: 2020 6370 753a 2022 302e 3522 0a20 2020    cpu: "0.5".   
-0001cf70: 2020 2020 2020 2074 6974 6c65 3a20 6c69         title: li
-0001cf80: 6d69 7473 0a20 2020 2020 2020 2020 2074  mits.          t
-0001cf90: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
-0001cfa0: 2020 2020 7265 7175 6573 7473 3a0a 2020      requests:.  
-0001cfb0: 2020 2020 2020 2020 6164 6469 7469 6f6e          addition
-0001cfc0: 616c 5072 6f70 6572 7469 6573 3a0a 2020  alProperties:.  
-0001cfd0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-0001cfe0: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-0001cff0: 2064 6573 6372 6970 7469 6f6e 3a20 7573   description: us
-0001d000: 6564 2074 6f20 7370 6563 6966 7920 7468  ed to specify th
-0001d010: 6520 6d69 6e69 6d75 6d20 616d 6f75 6e74  e minimum amount
-0001d020: 206f 6620 7265 736f 7572 6365 7320 7468   of resources th
-0001d030: 6174 2073 686f 756c 640a 2020 2020 2020  at should.      
-0001d040: 2020 2020 2020 6265 2063 6f6e 7375 6d65        be consume
-0001d050: 642e 0a20 2020 2020 2020 2020 2065 7861  d..          exa
-0001d060: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
-0001d070: 2020 6d65 6d6f 7279 3a20 3235 364d 690a    memory: 256Mi.
-0001d080: 2020 2020 2020 2020 2020 2020 6370 753a              cpu:
-0001d090: 2022 302e 3122 0a20 2020 2020 2020 2020   "0.1".         
-0001d0a0: 2074 6974 6c65 3a20 7265 7175 6573 7473   title: requests
-0001d0b0: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
-0001d0c0: 206f 626a 6563 740a 2020 2020 2020 7469   object.      ti
-0001d0d0: 746c 653a 2052 6573 6f75 7263 6552 6571  tle: ResourceReq
-0001d0e0: 7569 7265 6d65 6e74 730a 2020 2020 2020  uirements.      
-0001d0f0: 7479 7065 3a20 6f62 6a65 6374 0a20 2020  type: object.   
-0001d100: 2050 726f 6265 3a0a 2020 2020 2020 6578   Probe:.      ex
-0001d110: 616d 706c 653a 0a20 2020 2020 2020 2070  ample:.        p
-0001d120: 6572 696f 645f 7365 636f 6e64 733a 2036  eriod_seconds: 6
-0001d130: 300a 2020 2020 2020 2020 696e 6974 6961  0.        initia
-0001d140: 6c5f 6465 6c61 795f 7365 636f 6e64 733a  l_delay_seconds:
-0001d150: 2036 3030 0a20 2020 2020 2020 2074 6370   600.        tcp
-0001d160: 5f73 6f63 6b65 743a 0a20 2020 2020 2020  _socket:.       
-0001d170: 2020 2070 6f72 743a 2033 3031 3831 0a20     port: 30181. 
-0001d180: 2020 2020 2020 2020 2068 6f73 743a 2031           host: 1
-0001d190: 3237 2e30 2e30 2e31 0a20 2020 2020 2020  27.0.0.1.       
-0001d1a0: 2066 6169 6c75 7265 5f74 6872 6573 686f   failure_thresho
-0001d1b0: 6c64 3a20 330a 2020 2020 2020 2020 6874  ld: 3.        ht
-0001d1c0: 7470 5f67 6574 3a0a 2020 2020 2020 2020  tp_get:.        
-0001d1d0: 2020 7061 7468 3a20 2f73 686f 773f 646f    path: /show?do
-0001d1e0: 6d61 696e 3d76 3139 2e74 696b 746f 6b63  main=v19.tiktokc
-0001d1f0: 646e 2e63 6f6d 0a20 2020 2020 2020 2020  dn.com.         
-0001d200: 2068 7474 705f 6865 6164 6572 733a 0a20   http_headers:. 
-0001d210: 2020 2020 2020 2020 202d 2078 2d64 6576           - x-dev
-0001d220: 7372 652d 6175 7468 6f72 697a 6174 696f  sre-authorizatio
-0001d230: 6e3a 4265 6172 6572 2065 794a 6862 4763  n:Bearer eyJhbGc
-0001d240: 694f 694a 0a20 2020 2020 2020 2020 202d  iOiJ.          -
-0001d250: 2063 6f6e 7465 6e74 2d74 7970 653a 6170   content-type:ap
-0001d260: 706c 6963 6174 696f 6e2f 6a73 6f6e 0a20  plication/json. 
-0001d270: 2020 2020 2020 2020 2073 6368 656d 653a           scheme:
-0001d280: 2048 5454 5053 0a20 2020 2020 2020 2020   HTTPS.         
-0001d290: 2070 6f72 743a 2038 3838 380a 2020 2020   port: 8888.    
-0001d2a0: 2020 2020 2020 686f 7374 3a20 6773 732d        host: gss-
-0001d2b0: 646e 732d 6167 656e 742e 6578 616d 706c  dns-agent.exampl
-0001d2c0: 652e 6f72 670a 2020 2020 2020 2020 7469  e.org.        ti
-0001d2d0: 6d65 6f75 745f 7365 636f 6e64 733a 2036  meout_seconds: 6
-0001d2e0: 300a 2020 2020 2020 2020 6578 6563 5f63  0.        exec_c
-0001d2f0: 6f6d 6d61 6e64 3a0a 2020 2020 2020 2020  ommand:.        
-0001d300: 2d20 2f67 7373 2f64 696e 676d 616e 2f62  - /gss/dingman/b
-0001d310: 696e 2f64 696e 676d 616e 2d63 6c69 740a  in/dingman-clit.
-0001d320: 2020 2020 2020 2020 2d20 2d61 6464 7265          - -addre
-0001d330: 7373 0a20 2020 2020 2020 202d 2031 3237  ss.        - 127
-0001d340: 2e30 2e30 2e31 3a33 3035 3031 0a20 2020  .0.0.1:30501.   
-0001d350: 2020 2020 202d 202d 636f 6d6d 616e 640a       - -command.
-0001d360: 2020 2020 2020 2020 2d20 7368 6f77 2070          - show p
-0001d370: 6f70 3a61 6c6c 2073 756d 6d61 7279 3a68  op:all summary:h
-0001d380: 6561 6c74 682d 7374 6174 7573 0a20 2020  ealth-status.   
-0001d390: 2020 2070 726f 7065 7274 6965 733a 0a20     properties:. 
-0001d3a0: 2020 2020 2020 2065 7865 635f 636f 6d6d         exec_comm
-0001d3b0: 616e 643a 0a20 2020 2020 2020 2020 2064  and:.          d
-0001d3c0: 6573 6372 6970 7469 6f6e 3a20 436f 6d6d  escription: Comm
-0001d3d0: 616e 6420 6c69 6e65 2074 6f20 6578 6563  and line to exec
-0001d3e0: 7574 6520 696e 7369 6465 2074 6865 2063  ute inside the c
-0001d3f0: 6f6e 7461 696e 6572 0a20 2020 2020 2020  ontainer.       
-0001d400: 2020 2065 7861 6d70 6c65 3a0a 2020 2020     example:.    
-0001d410: 2020 2020 2020 2d20 2f67 7373 2f64 696e        - /gss/din
-0001d420: 676d 616e 2f62 696e 2f64 696e 676d 616e  gman/bin/dingman
-0001d430: 2d63 6c69 740a 2020 2020 2020 2020 2020  -clit.          
-0001d440: 2d20 2d61 6464 7265 7373 0a20 2020 2020  - -address.     
-0001d450: 2020 2020 202d 2031 3237 2e30 2e30 2e31       - 127.0.0.1
-0001d460: 3a33 3035 3031 0a20 2020 2020 2020 2020  :30501.         
-0001d470: 202d 202d 636f 6d6d 616e 640a 2020 2020   - -command.    
-0001d480: 2020 2020 2020 2d20 7368 6f77 2070 6f70        - show pop
-0001d490: 3a61 6c6c 2073 756d 6d61 7279 3a68 6561  :all summary:hea
-0001d4a0: 6c74 682d 7374 6174 7573 0a20 2020 2020  lth-status.     
-0001d4b0: 2020 2020 2069 7465 6d73 3a0a 2020 2020       items:.    
-0001d4c0: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
-0001d4d0: 7269 6e67 0a20 2020 2020 2020 2020 2074  ring.          t
-0001d4e0: 6974 6c65 3a20 6578 6563 5f63 6f6d 6d61  itle: exec_comma
-0001d4f0: 6e64 0a20 2020 2020 2020 2020 2074 7970  nd.          typ
-0001d500: 653a 2061 7272 6179 0a20 2020 2020 2020  e: array.       
-0001d510: 2068 7474 705f 6765 743a 0a20 2020 2020   http_get:.     
-0001d520: 2020 2020 2024 7265 663a 2027 232f 636f       $ref: '#/co
-0001d530: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-0001d540: 2f48 7474 7047 6574 270a 2020 2020 2020  /HttpGet'.      
-0001d550: 2020 7463 705f 736f 636b 6574 3a0a 2020    tcp_socket:.  
-0001d560: 2020 2020 2020 2020 2472 6566 3a20 2723          $ref: '#
-0001d570: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-0001d580: 6d61 732f 5463 7053 6f63 6b65 7427 0a20  mas/TcpSocket'. 
-0001d590: 2020 2020 2020 2066 6169 6c75 7265 5f74         failure_t
-0001d5a0: 6872 6573 686f 6c64 3a0a 2020 2020 2020  hreshold:.      
-0001d5b0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-0001d5c0: 204d 696e 696d 756d 2063 6f6e 7365 6375   Minimum consecu
-0001d5d0: 7469 7665 2066 6169 6c75 7265 7320 666f  tive failures fo
-0001d5e0: 7220 7468 6520 7072 6f62 6520 746f 2062  r the probe to b
-0001d5f0: 6520 636f 6e73 6964 6572 6564 0a20 2020  e considered.   
-0001d600: 2020 2020 2020 2020 2066 6169 6c65 6420           failed 
-0001d610: 6166 7465 7220 6861 7669 6e67 2073 7563  after having suc
-0001d620: 6365 6564 6564 2e0a 2020 2020 2020 2020  ceeded..        
-0001d630: 2020 6578 616d 706c 653a 2033 0a20 2020    example: 3.   
-0001d640: 2020 2020 2020 2074 6974 6c65 3a20 6661         title: fa
-0001d650: 696c 7572 655f 7468 7265 7368 6f6c 640a  ilure_threshold.
-0001d660: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-0001d670: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
-0001d680: 7065 7269 6f64 5f73 6563 6f6e 6473 3a0a  period_seconds:.
-0001d690: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-0001d6a0: 7074 696f 6e3a 2048 6f77 206f 6674 656e  ption: How often
-0001d6b0: 2028 696e 2073 6563 6f6e 6473 2920 746f   (in seconds) to
-0001d6c0: 2070 6572 666f 726d 2074 6865 2070 726f   perform the pro
-0001d6d0: 6265 2e20 4465 6661 756c 7420 746f 2031  be. Default to 1
-0001d6e0: 300a 2020 2020 2020 2020 2020 2020 7365  0.            se
-0001d6f0: 636f 6e64 732e 204d 696e 696d 756d 2076  conds. Minimum v
-0001d700: 616c 7565 2069 7320 312e 0a20 2020 2020  alue is 1..     
-0001d710: 2020 2020 2065 7861 6d70 6c65 3a20 3630       example: 60
-0001d720: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
-0001d730: 3a20 7065 7269 6f64 5f73 6563 6f6e 6473  : period_seconds
-0001d740: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
-0001d750: 2069 6e74 6567 6572 0a20 2020 2020 2020   integer.       
-0001d760: 2074 696d 656f 7574 5f73 6563 6f6e 6473   timeout_seconds
-0001d770: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
-0001d780: 7269 7074 696f 6e3a 204e 756d 6265 7220  ription: Number 
-0001d790: 6f66 2073 6563 6f6e 6473 2061 6674 6572  of seconds after
-0001d7a0: 2077 6869 6368 2074 6865 2070 726f 6265   which the probe
-0001d7b0: 2074 696d 6573 206f 7574 2e20 4465 6661   times out. Defa
-0001d7c0: 756c 7473 0a20 2020 2020 2020 2020 2020  ults.           
-0001d7d0: 2074 6f20 3120 7365 636f 6e64 2e0a 2020   to 1 second..  
-0001d7e0: 2020 2020 2020 2020 6578 616d 706c 653a          example:
-0001d7f0: 2036 300a 2020 2020 2020 2020 2020 7469   60.          ti
-0001d800: 746c 653a 2074 696d 656f 7574 5f73 6563  tle: timeout_sec
-0001d810: 6f6e 6473 0a20 2020 2020 2020 2020 2074  onds.          t
-0001d820: 7970 653a 2069 6e74 6567 6572 0a20 2020  ype: integer.   
-0001d830: 2020 2020 2069 6e69 7469 616c 5f64 656c       initial_del
-0001d840: 6179 5f73 6563 6f6e 6473 3a0a 2020 2020  ay_seconds:.    
-0001d850: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-0001d860: 6e3a 204e 756d 6265 7220 6f66 2073 6563  n: Number of sec
-0001d870: 6f6e 6473 2061 6674 6572 2074 6865 2063  onds after the c
-0001d880: 6f6e 7461 696e 6572 2068 6173 2073 7461  ontainer has sta
-0001d890: 7274 6564 2062 6566 6f72 6520 6c69 7665  rted before live
-0001d8a0: 6e65 7373 0a20 2020 2020 2020 2020 2020  ness.           
-0001d8b0: 2070 726f 6265 7320 6172 6520 696e 6974   probes are init
-0001d8c0: 6961 7465 642e 0a20 2020 2020 2020 2020  iated..         
-0001d8d0: 2065 7861 6d70 6c65 3a20 3630 300a 2020   example: 600.  
-0001d8e0: 2020 2020 2020 2020 7469 746c 653a 2069          title: i
-0001d8f0: 6e69 7469 616c 5f64 656c 6179 5f73 6563  nitial_delay_sec
-0001d900: 6f6e 6473 0a20 2020 2020 2020 2020 2074  onds.          t
-0001d910: 7970 653a 2069 6e74 6567 6572 0a20 2020  ype: integer.   
-0001d920: 2020 2074 6974 6c65 3a20 5072 6f62 650a     title: Probe.
-0001d930: 2020 2020 2020 7479 7065 3a20 6f62 6a65        type: obje
-0001d940: 6374 0a20 2020 2056 6f6c 756d 653a 0a20  ct.    Volume:. 
-0001d950: 2020 2020 2065 7861 6d70 6c65 3a0a 2020       example:.  
-0001d960: 2020 2020 2020 686f 7374 5f70 6174 683a        host_path:
-0001d970: 0a20 2020 2020 2020 2020 2070 6174 683a  .          path:
-0001d980: 202f 6461 7461 0a20 2020 2020 2020 2020   /data.         
-0001d990: 2070 6174 685f 7479 7065 3a20 4469 7265   path_type: Dire
-0001d9a0: 6374 6f72 790a 2020 2020 2020 2020 6e61  ctory.        na
-0001d9b0: 6d65 3a20 6465 6d6f 2d76 6f6c 0a20 2020  me: demo-vol.   
-0001d9c0: 2020 2020 2065 6d70 7479 5f64 6972 3a0a       empty_dir:.
-0001d9d0: 2020 2020 2020 2020 2020 6d65 6469 756d            medium
-0001d9e0: 3a20 4d65 6d6f 7279 0a20 2020 2020 2020  : Memory.       
-0001d9f0: 2020 2073 697a 655f 6c69 6d69 743a 2035     size_limit: 5
-0001da00: 3030 4d69 0a20 2020 2020 2020 2063 6f6e  00Mi.        con
-0001da10: 6669 675f 6d61 703a 0a20 2020 2020 2020  fig_map:.       
-0001da20: 2020 206e 616d 653a 2073 6572 7665 7220     name: server 
-0001da30: 636f 6e66 6967 2f73 6563 7265 740a 2020  config/secret.  
-0001da40: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-0001da50: 3a20 6661 6c73 650a 2020 2020 2020 2020  : false.        
-0001da60: 2020 6465 6661 756c 745f 6d6f 6465 3a20    default_mode: 
-0001da70: 3430 300a 2020 2020 2020 2020 7365 6372  400.        secr
-0001da80: 6574 3a0a 2020 2020 2020 2020 2020 6e61  et:.          na
-0001da90: 6d65 3a20 7365 7276 6572 2063 6f6e 6669  me: server confi
-0001daa0: 672f 7365 6372 6574 0a20 2020 2020 2020  g/secret.       
-0001dab0: 2020 206f 7074 696f 6e61 6c3a 2066 616c     optional: fal
-0001dac0: 7365 0a20 2020 2020 2020 2020 2064 6566  se.          def
-0001dad0: 6175 6c74 5f6d 6f64 653a 2034 3030 0a20  ault_mode: 400. 
-0001dae0: 2020 2020 2020 2070 6572 7369 7374 656e         persisten
-0001daf0: 745f 766f 6c75 6d65 5f63 6c61 696d 3a0a  t_volume_claim:.
-0001db00: 2020 2020 2020 2020 2020 7265 6164 5f6f            read_o
-0001db10: 6e6c 793a 2066 616c 7365 0a20 2020 2020  nly: false.     
-0001db20: 2020 2020 2063 6c61 696d 5f6e 616d 653a       claim_name:
-0001db30: 2064 656d 6f2d 7076 630a 2020 2020 2020   demo-pvc.      
-0001db40: 7072 6f70 6572 7469 6573 3a0a 2020 2020  properties:.    
-0001db50: 2020 2020 6e61 6d65 3a0a 2020 2020 2020      name:.      
-0001db60: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-0001db70: 204e 616d 6520 6f66 2074 6865 2076 6f6c   Name of the vol
-0001db80: 756d 652e 204d 7573 7420 6265 2061 2044  ume. Must be a D
-0001db90: 4e53 5f4c 4142 454c 2061 6e64 2075 6e69  NS_LABEL and uni
-0001dba0: 7175 6520 7769 7468 696e 2074 6865 0a20  que within the. 
-0001dbb0: 2020 2020 2020 2020 2020 2070 6f64 0a20             pod. 
-0001dbc0: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
-0001dbd0: 3a20 6465 6d6f 2d76 6f6c 0a20 2020 2020  : demo-vol.     
-0001dbe0: 2020 2020 2074 6974 6c65 3a20 6e61 6d65       title: name
-0001dbf0: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
-0001dc00: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-0001dc10: 636f 6e66 6967 5f6d 6170 3a0a 2020 2020  config_map:.    
-0001dc20: 2020 2020 2020 2472 6566 3a20 2723 2f63        $ref: '#/c
-0001dc30: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-0001dc40: 732f 5265 6656 6f6c 756d 6553 6f75 7263  s/RefVolumeSourc
-0001dc50: 6527 0a20 2020 2020 2020 2073 6563 7265  e'.        secre
-0001dc60: 743a 0a20 2020 2020 2020 2020 2024 7265  t:.          $re
-0001dc70: 663a 2027 232f 636f 6d70 6f6e 656e 7473  f: '#/components
-0001dc80: 2f73 6368 656d 6173 2f52 6566 566f 6c75  /schemas/RefVolu
-0001dc90: 6d65 536f 7572 6365 270a 2020 2020 2020  meSource'.      
-0001dca0: 2020 7065 7273 6973 7465 6e74 5f76 6f6c    persistent_vol
-0001dcb0: 756d 655f 636c 6169 6d3a 0a20 2020 2020  ume_claim:.     
-0001dcc0: 2020 2020 2024 7265 663a 2027 232f 636f       $ref: '#/co
-0001dcd0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-0001dce0: 2f56 6f6c 756d 655f 7065 7273 6973 7465  /Volume_persiste
-0001dcf0: 6e74 5f76 6f6c 756d 655f 636c 6169 6d27  nt_volume_claim'
-0001dd00: 0a20 2020 2020 2020 2065 6d70 7479 5f64  .        empty_d
-0001dd10: 6972 3a0a 2020 2020 2020 2020 2020 2472  ir:.          $r
-0001dd20: 6566 3a20 2723 2f63 6f6d 706f 6e65 6e74  ef: '#/component
-0001dd30: 732f 7363 6865 6d61 732f 566f 6c75 6d65  s/schemas/Volume
-0001dd40: 5f65 6d70 7479 5f64 6972 270a 2020 2020  _empty_dir'.    
-0001dd50: 2020 2020 686f 7374 5f70 6174 683a 0a20      host_path:. 
-0001dd60: 2020 2020 2020 2020 2024 7265 663a 2027           $ref: '
-0001dd70: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-0001dd80: 656d 6173 2f56 6f6c 756d 655f 686f 7374  emas/Volume_host
-0001dd90: 5f70 6174 6827 0a20 2020 2020 2072 6571  _path'.      req
-0001dda0: 7569 7265 643a 0a20 2020 2020 202d 206e  uired:.      - n
-0001ddb0: 616d 650a 2020 2020 2020 7469 746c 653a  ame.      title:
-0001ddc0: 2056 6f6c 756d 650a 2020 2020 2020 7479   Volume.      ty
-0001ddd0: 7065 3a20 6f62 6a65 6374 0a20 2020 2052  pe: object.    R
-0001dde0: 6566 566f 6c75 6d65 536f 7572 6365 3a0a  efVolumeSource:.
-0001ddf0: 2020 2020 2020 6578 616d 706c 653a 0a20        example:. 
-0001de00: 2020 2020 2020 206e 616d 653a 2073 6572         name: ser
-0001de10: 7665 7220 636f 6e66 6967 2f73 6563 7265  ver config/secre
-0001de20: 740a 2020 2020 2020 2020 6f70 7469 6f6e  t.        option
-0001de30: 616c 3a20 6661 6c73 650a 2020 2020 2020  al: false.      
-0001de40: 2020 6465 6661 756c 745f 6d6f 6465 3a20    default_mode: 
-0001de50: 3430 300a 2020 2020 2020 7072 6f70 6572  400.      proper
-0001de60: 7469 6573 3a0a 2020 2020 2020 2020 6e61  ties:.        na
-0001de70: 6d65 3a0a 2020 2020 2020 2020 2020 6465  me:.          de
-0001de80: 7363 7269 7074 696f 6e3a 2076 6f6c 756d  scription: volum
-0001de90: 6520 736f 7572 6365 2028 636f 6e66 6967  e source (config
-0001dea0: 4d61 702f 5365 6372 6574 2920 6e61 6d65  Map/Secret) name
-0001deb0: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-0001dec0: 6c65 3a20 7365 7276 6572 2063 6f6e 6669  le: server confi
-0001ded0: 672f 7365 6372 6574 0a20 2020 2020 2020  g/secret.       
-0001dee0: 2020 2074 6974 6c65 3a20 6e61 6d65 0a20     title: name. 
-0001def0: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-0001df00: 7472 696e 670a 2020 2020 2020 2020 6f70  tring.        op
-0001df10: 7469 6f6e 616c 3a0a 2020 2020 2020 2020  tional:.        
-0001df20: 2020 6465 7363 7269 7074 696f 6e3a 2073    description: s
-0001df30: 7065 6369 6679 2077 6865 7468 6572 2074  pecify whether t
-0001df40: 6865 2076 6f6c 756d 6520 736f 7572 6365  he volume source
-0001df50: 206f 7220 6974 7320 6b65 7973 206d 7573   or its keys mus
-0001df60: 7420 6265 2064 6566 696e 6564 0a20 2020  t be defined.   
-0001df70: 2020 2020 2020 2065 7861 6d70 6c65 3a20         example: 
-0001df80: 6661 6c73 650a 2020 2020 2020 2020 2020  false.          
-0001df90: 7469 746c 653a 206f 7074 696f 6e61 6c0a  title: optional.
-0001dfa0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-0001dfb0: 626f 6f6c 6561 6e0a 2020 2020 2020 2020  boolean.        
-0001dfc0: 6465 6661 756c 745f 6d6f 6465 3a0a 2020  default_mode:.  
-0001dfd0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-0001dfe0: 696f 6e3a 207c 0a20 2020 2020 2020 2020  ion: |.         
-0001dff0: 2020 206d 6f64 6520 6269 7473 2075 7365     mode bits use
-0001e000: 6420 746f 2073 6574 2070 6572 6d69 7373  d to set permiss
-0001e010: 696f 6e73 206f 6e20 6372 6561 7465 6420  ions on created 
-0001e020: 6669 6c65 7320 6279 2064 6566 6175 6c74  files by default
-0001e030: 2e0a 2020 2020 2020 2020 2020 2020 4d75  ..            Mu
-0001e040: 7374 2062 6520 616e 206f 6374 616c 2076  st be an octal v
-0001e050: 616c 7565 2062 6574 7765 656e 2030 3030  alue between 000
-0001e060: 3020 616e 6420 3037 3737 206f 7220 6120  0 and 0777 or a 
-0001e070: 6465 6369 6d61 6c20 7661 6c75 6520 6265  decimal value be
-0001e080: 7477 6565 6e20 3020 616e 6420 3531 310a  tween 0 and 511.
-0001e090: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
-0001e0a0: 653a 2034 3030 0a20 2020 2020 2020 2020  e: 400.         
-0001e0b0: 2074 6974 6c65 3a20 6465 6661 756c 745f   title: default_
-0001e0c0: 6d6f 6465 0a20 2020 2020 2020 2020 2074  mode.          t
-0001e0d0: 7970 653a 2069 6e74 6567 6572 0a20 2020  ype: integer.   
-0001e0e0: 2020 2074 6974 6c65 3a20 5265 6656 6f6c     title: RefVol
-0001e0f0: 756d 6553 6f75 7263 650a 2020 2020 2020  umeSource.      
-0001e100: 7479 7065 3a20 6f62 6a65 6374 0a20 2020  type: object.   
-0001e110: 2041 6666 696e 6974 793a 0a20 2020 2020   Affinity:.     
-0001e120: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
-0001e130: 2020 706f 645f 616e 7469 5f61 6666 696e    pod_anti_affin
-0001e140: 6974 793a 0a20 2020 2020 2020 2020 2070  ity:.          p
-0001e150: 7265 6665 7272 6564 5f64 7572 696e 675f  referred_during_
-0001e160: 7363 6865 6475 6c69 6e67 5f69 676e 6f72  scheduling_ignor
-0001e170: 6564 5f64 7572 696e 675f 6578 6563 7574  ed_during_execut
-0001e180: 696f 6e3a 0a20 2020 2020 2020 2020 202d  ion:.          -
-0001e190: 2077 6569 6768 743a 2036 0a20 2020 2020   weight: 6.     
-0001e1a0: 2020 2020 2020 2070 6f64 5f61 6666 696e         pod_affin
-0001e1b0: 6974 795f 7465 726d 3a0a 2020 2020 2020  ity_term:.      
-0001e1c0: 2020 2020 2020 2020 6c61 6265 6c5f 7365          label_se
-0001e1d0: 6c65 6374 6f72 3a0a 2020 2020 2020 2020  lector:.        
-0001e1e0: 2020 2020 2020 2d20 6170 703a 6465 6d6f        - app:demo
-0001e1f0: 2d61 7070 0a20 2020 2020 2020 2020 2020  -app.           
-0001e200: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
-0001e210: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
-0001e220: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
-0001e230: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
-0001e240: 2020 2020 2020 2074 6f70 6f6c 6f67 795f         topology_
-0001e250: 6b65 793a 2074 6f70 6f6c 6f67 795f 6b65  key: topology_ke
-0001e260: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-0001e270: 6e61 6d65 7370 6163 6573 3a0a 2020 2020  namespaces:.    
-0001e280: 2020 2020 2020 2020 2020 2d20 6e61 6d65            - name
-0001e290: 7370 6163 6573 0a20 2020 2020 2020 2020  spaces.         
-0001e2a0: 2020 2020 202d 206e 616d 6573 7061 6365       - namespace
-0001e2b0: 730a 2020 2020 2020 2020 2020 2d20 7765  s.          - we
-0001e2c0: 6967 6874 3a20 360a 2020 2020 2020 2020  ight: 6.        
-0001e2d0: 2020 2020 706f 645f 6166 6669 6e69 7479      pod_affinity
-0001e2e0: 5f74 6572 6d3a 0a20 2020 2020 2020 2020  _term:.         
-0001e2f0: 2020 2020 206c 6162 656c 5f73 656c 6563       label_selec
-0001e300: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
-0001e310: 2020 202d 2061 7070 3a64 656d 6f2d 6170     - app:demo-ap
-0001e320: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-0001e330: 2d20 226b 6579 3a76 6572 7369 6f6e 2c20  - "key:version, 
-0001e340: 6f70 6572 6174 6f72 3a49 6e2c 2076 616c  operator:In, val
-0001e350: 7565 733a 5b76 312e 302e 302c 2076 312e  ues:[v1.0.0, v1.
-0001e360: 302e 315d 220a 2020 2020 2020 2020 2020  0.1]".          
-0001e370: 2020 2020 746f 706f 6c6f 6779 5f6b 6579      topology_key
-0001e380: 3a20 746f 706f 6c6f 6779 5f6b 6579 0a20  : topology_key. 
-0001e390: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-0001e3a0: 6573 7061 6365 733a 0a20 2020 2020 2020  espaces:.       
-0001e3b0: 2020 2020 2020 202d 206e 616d 6573 7061         - namespa
-0001e3c0: 6365 730a 2020 2020 2020 2020 2020 2020  ces.            
-0001e3d0: 2020 2d20 6e61 6d65 7370 6163 6573 0a20    - namespaces. 
-0001e3e0: 2020 2020 2020 2020 2072 6571 7569 7265           require
-0001e3f0: 645f 6475 7269 6e67 5f73 6368 6564 756c  d_during_schedul
-0001e400: 696e 675f 6967 6e6f 7265 645f 6475 7269  ing_ignored_duri
-0001e410: 6e67 5f65 7865 6375 7469 6f6e 3a0a 2020  ng_execution:.  
-0001e420: 2020 2020 2020 2020 2d20 6c61 6265 6c5f          - label_
-0001e430: 7365 6c65 6374 6f72 3a0a 2020 2020 2020  selector:.      
-0001e440: 2020 2020 2020 2d20 6170 703a 6465 6d6f        - app:demo
-0001e450: 2d61 7070 0a20 2020 2020 2020 2020 2020  -app.           
-0001e460: 202d 2022 6b65 793a 7665 7273 696f 6e2c   - "key:version,
-0001e470: 206f 7065 7261 746f 723a 496e 2c20 7661   operator:In, va
-0001e480: 6c75 6573 3a5b 7631 2e30 2e30 2c20 7631  lues:[v1.0.0, v1
-0001e490: 2e30 2e31 5d22 0a20 2020 2020 2020 2020  .0.1]".         
-0001e4a0: 2020 2074 6f70 6f6c 6f67 795f 6b65 793a     topology_key:
-0001e4b0: 2074 6f70 6f6c 6f67 795f 6b65 790a 2020   topology_key.  
-0001e4c0: 2020 2020 2020 2020 2020 6e61 6d65 7370            namesp
-0001e4d0: 6163 6573 3a0a 2020 2020 2020 2020 2020  aces:.          
-0001e4e0: 2020 2d20 6e61 6d65 7370 6163 6573 0a20    - namespaces. 
-0001e4f0: 2020 2020 2020 2020 2020 202d 206e 616d             - nam
-0001e500: 6573 7061 6365 730a 2020 2020 2020 2020  espaces.        
-0001e510: 2020 2d20 6c61 6265 6c5f 7365 6c65 6374    - label_select
-0001e520: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-0001e530: 2d20 6170 703a 6465 6d6f 2d61 7070 0a20  - app:demo-app. 
-0001e540: 2020 2020 2020 2020 2020 202d 2022 6b65             - "ke
-0001e550: 793a 7665 7273 696f 6e2c 206f 7065 7261  y:version, opera
-0001e560: 746f 723a 496e 2c20 7661 6c75 6573 3a5b  tor:In, values:[
-0001e570: 7631 2e30 2e30 2c20 7631 2e30 2e31 5d22  v1.0.0, v1.0.1]"
-0001e580: 0a20 2020 2020 2020 2020 2020 2074 6f70  .            top
-0001e590: 6f6c 6f67 795f 6b65 793a 2074 6f70 6f6c  ology_key: topol
-0001e5a0: 6f67 795f 6b65 790a 2020 2020 2020 2020  ogy_key.        
-0001e5b0: 2020 2020 6e61 6d65 7370 6163 6573 3a0a      namespaces:.
-0001e5c0: 2020 2020 2020 2020 2020 2020 2d20 6e61              - na
-0001e5d0: 6d65 7370 6163 6573 0a20 2020 2020 2020  mespaces.       
-0001e5e0: 2020 2020 202d 206e 616d 6573 7061 6365       - namespace
-0001e5f0: 730a 2020 2020 2020 2020 6e6f 6465 5f61  s.        node_a
-0001e600: 6666 696e 6974 793a 0a20 2020 2020 2020  ffinity:.       
-0001e610: 2020 2070 7265 6665 7272 6564 5f64 7572     preferred_dur
-0001e620: 696e 675f 7363 6865 6475 6c69 6e67 5f69  ing_scheduling_i
-0001e630: 676e 6f72 6564 5f64 7572 696e 675f 6578  gnored_during_ex
-0001e640: 6563 7574 696f 6e3a 0a20 2020 2020 2020  ecution:.       
-0001e650: 2020 202d 2070 7265 6665 7265 6e63 653a     - preference:
-0001e660: 0a20 2020 2020 2020 2020 2020 2020 206d  .              m
-0001e670: 6174 6368 5f65 7870 7265 7373 696f 6e73  atch_expressions
-0001e680: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001e690: 2d20 226b 6579 3a76 6572 7369 6f6e 2c20  - "key:version, 
-0001e6a0: 6f70 6572 6174 6f72 3a49 6e2c 2076 616c  operator:In, val
-0001e6b0: 7565 733a 5b76 312e 302e 302c 2076 312e  ues:[v1.0.0, v1.
-0001e6c0: 302e 315d 220a 2020 2020 2020 2020 2020  0.1]".          
-0001e6d0: 2020 2020 6d61 7463 685f 6669 656c 6473      match_fields
-0001e6e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001e6f0: 2d20 226b 6579 3a76 6572 7369 6f6e 2c20  - "key:version, 
-0001e700: 6f70 6572 6174 6f72 3a49 6e2c 2076 616c  operator:In, val
-0001e710: 7565 733a 5b76 312e 302e 302c 2076 312e  ues:[v1.0.0, v1.
-0001e720: 302e 315d 220a 2020 2020 2020 2020 2020  0.1]".          
-0001e730: 2020 7765 6967 6874 3a20 300a 2020 2020    weight: 0.    
-0001e740: 2020 2020 2020 2d20 7072 6566 6572 656e        - preferen
-0001e750: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
-0001e760: 2020 6d61 7463 685f 6578 7072 6573 7369    match_expressi
-0001e770: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-0001e780: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
-0001e790: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
-0001e7a0: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
-0001e7b0: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
-0001e7c0: 2020 2020 2020 206d 6174 6368 5f66 6965         match_fie
-0001e7d0: 6c64 733a 0a20 2020 2020 2020 2020 2020  lds:.           
-0001e7e0: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
-0001e7f0: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
-0001e800: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
-0001e810: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
-0001e820: 2020 2020 2077 6569 6768 743a 2030 0a20       weight: 0. 
-0001e830: 2020 2020 2020 2020 2072 6571 7569 7265           require
-0001e840: 645f 6475 7269 6e67 5f73 6368 6564 756c  d_during_schedul
-0001e850: 696e 675f 6967 6e6f 7265 645f 6475 7269  ing_ignored_duri
-0001e860: 6e67 5f65 7865 6375 7469 6f6e 3a0a 2020  ng_execution:.  
-0001e870: 2020 2020 2020 2020 2020 6e6f 6465 5f73            node_s
-0001e880: 656c 6563 746f 725f 7465 726d 733a 0a20  elector_terms:. 
-0001e890: 2020 2020 2020 2020 2020 202d 206d 6174             - mat
-0001e8a0: 6368 5f65 7870 7265 7373 696f 6e73 3a0a  ch_expressions:.
-0001e8b0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-0001e8c0: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
-0001e8d0: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
-0001e8e0: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
-0001e8f0: 315d 220a 2020 2020 2020 2020 2020 2020  1]".            
-0001e900: 2020 6d61 7463 685f 6669 656c 6473 3a0a    match_fields:.
-0001e910: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-0001e920: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
-0001e930: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
-0001e940: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
-0001e950: 315d 220a 2020 2020 2020 2020 2020 2020  1]".            
-0001e960: 2d20 6d61 7463 685f 6578 7072 6573 7369  - match_expressi
-0001e970: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-0001e980: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
-0001e990: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
-0001e9a0: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
-0001e9b0: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
-0001e9c0: 2020 2020 2020 206d 6174 6368 5f66 6965         match_fie
-0001e9d0: 6c64 733a 0a20 2020 2020 2020 2020 2020  lds:.           
-0001e9e0: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
-0001e9f0: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
-0001ea00: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
-0001ea10: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
-0001ea20: 2070 6f64 5f61 6666 696e 6974 793a 0a20   pod_affinity:. 
-0001ea30: 2020 2020 2020 2020 2070 7265 6665 7272           preferr
-0001ea40: 6564 5f64 7572 696e 675f 7363 6865 6475  ed_during_schedu
-0001ea50: 6c69 6e67 5f69 676e 6f72 6564 5f64 7572  ling_ignored_dur
-0001ea60: 696e 675f 6578 6563 7574 696f 6e3a 0a20  ing_execution:. 
-0001ea70: 2020 2020 2020 2020 202d 2077 6569 6768           - weigh
-0001ea80: 743a 2036 0a20 2020 2020 2020 2020 2020  t: 6.           
-0001ea90: 2070 6f64 5f61 6666 696e 6974 795f 7465   pod_affinity_te
-0001eaa0: 726d 3a0a 2020 2020 2020 2020 2020 2020  rm:.            
-0001eab0: 2020 6c61 6265 6c5f 7365 6c65 6374 6f72    label_selector
-0001eac0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001ead0: 2d20 6170 703a 6465 6d6f 2d61 7070 0a20  - app:demo-app. 
-0001eae0: 2020 2020 2020 2020 2020 2020 202d 2022               - "
-0001eaf0: 6b65 793a 7665 7273 696f 6e2c 206f 7065  key:version, ope
-0001eb00: 7261 746f 723a 496e 2c20 7661 6c75 6573  rator:In, values
-0001eb10: 3a5b 7631 2e30 2e30 2c20 7631 2e30 2e31  :[v1.0.0, v1.0.1
-0001eb20: 5d22 0a20 2020 2020 2020 2020 2020 2020  ]".             
-0001eb30: 2074 6f70 6f6c 6f67 795f 6b65 793a 2074   topology_key: t
-0001eb40: 6f70 6f6c 6f67 795f 6b65 790a 2020 2020  opology_key.    
-0001eb50: 2020 2020 2020 2020 2020 6e61 6d65 7370            namesp
-0001eb60: 6163 6573 3a0a 2020 2020 2020 2020 2020  aces:.          
-0001eb70: 2020 2020 2d20 6e61 6d65 7370 6163 6573      - namespaces
-0001eb80: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
-0001eb90: 206e 616d 6573 7061 6365 730a 2020 2020   namespaces.    
-0001eba0: 2020 2020 2020 2d20 7765 6967 6874 3a20        - weight: 
-0001ebb0: 360a 2020 2020 2020 2020 2020 2020 706f  6.            po
-0001ebc0: 645f 6166 6669 6e69 7479 5f74 6572 6d3a  d_affinity_term:
-0001ebd0: 0a20 2020 2020 2020 2020 2020 2020 206c  .              l
-0001ebe0: 6162 656c 5f73 656c 6563 746f 723a 0a20  abel_selector:. 
-0001ebf0: 2020 2020 2020 2020 2020 2020 202d 2061               - a
-0001ec00: 7070 3a64 656d 6f2d 6170 700a 2020 2020  pp:demo-app.    
-0001ec10: 2020 2020 2020 2020 2020 2d20 226b 6579            - "key
-0001ec20: 3a76 6572 7369 6f6e 2c20 6f70 6572 6174  :version, operat
-0001ec30: 6f72 3a49 6e2c 2076 616c 7565 733a 5b76  or:In, values:[v
-0001ec40: 312e 302e 302c 2076 312e 302e 315d 220a  1.0.0, v1.0.1]".
-0001ec50: 2020 2020 2020 2020 2020 2020 2020 746f                to
-0001ec60: 706f 6c6f 6779 5f6b 6579 3a20 746f 706f  pology_key: topo
-0001ec70: 6c6f 6779 5f6b 6579 0a20 2020 2020 2020  logy_key.       
-0001ec80: 2020 2020 2020 206e 616d 6573 7061 6365         namespace
-0001ec90: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0001eca0: 202d 206e 616d 6573 7061 6365 730a 2020   - namespaces.  
-0001ecb0: 2020 2020 2020 2020 2020 2020 2d20 6e61              - na
-0001ecc0: 6d65 7370 6163 6573 0a20 2020 2020 2020  mespaces.       
-0001ecd0: 2020 2072 6571 7569 7265 645f 6475 7269     required_duri
-0001ece0: 6e67 5f73 6368 6564 756c 696e 675f 6967  ng_scheduling_ig
-0001ecf0: 6e6f 7265 645f 6475 7269 6e67 5f65 7865  nored_during_exe
-0001ed00: 6375 7469 6f6e 3a0a 2020 2020 2020 2020  cution:.        
-0001ed10: 2020 2d20 6c61 6265 6c5f 7365 6c65 6374    - label_select
-0001ed20: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-0001ed30: 2d20 6170 703a 6465 6d6f 2d61 7070 0a20  - app:demo-app. 
-0001ed40: 2020 2020 2020 2020 2020 202d 2022 6b65             - "ke
-0001ed50: 793a 7665 7273 696f 6e2c 206f 7065 7261  y:version, opera
-0001ed60: 746f 723a 496e 2c20 7661 6c75 6573 3a5b  tor:In, values:[
-0001ed70: 7631 2e30 2e30 2c20 7631 2e30 2e31 5d22  v1.0.0, v1.0.1]"
-0001ed80: 0a20 2020 2020 2020 2020 2020 2074 6f70  .            top
-0001ed90: 6f6c 6f67 795f 6b65 793a 2074 6f70 6f6c  ology_key: topol
-0001eda0: 6f67 795f 6b65 790a 2020 2020 2020 2020  ogy_key.        
-0001edb0: 2020 2020 6e61 6d65 7370 6163 6573 3a0a      namespaces:.
-0001edc0: 2020 2020 2020 2020 2020 2020 2d20 6e61              - na
-0001edd0: 6d65 7370 6163 6573 0a20 2020 2020 2020  mespaces.       
-0001ede0: 2020 2020 202d 206e 616d 6573 7061 6365       - namespace
-0001edf0: 730a 2020 2020 2020 2020 2020 2d20 6c61  s.          - la
-0001ee00: 6265 6c5f 7365 6c65 6374 6f72 3a0a 2020  bel_selector:.  
-0001ee10: 2020 2020 2020 2020 2020 2d20 6170 703a            - app:
-0001ee20: 6465 6d6f 2d61 7070 0a20 2020 2020 2020  demo-app.       
-0001ee30: 2020 2020 202d 2022 6b65 793a 7665 7273       - "key:vers
-0001ee40: 696f 6e2c 206f 7065 7261 746f 723a 496e  ion, operator:In
-0001ee50: 2c20 7661 6c75 6573 3a5b 7631 2e30 2e30  , values:[v1.0.0
-0001ee60: 2c20 7631 2e30 2e31 5d22 0a20 2020 2020  , v1.0.1]".     
-0001ee70: 2020 2020 2020 2074 6f70 6f6c 6f67 795f         topology_
-0001ee80: 6b65 793a 2074 6f70 6f6c 6f67 795f 6b65  key: topology_ke
-0001ee90: 790a 2020 2020 2020 2020 2020 2020 6e61  y.            na
-0001eea0: 6d65 7370 6163 6573 3a0a 2020 2020 2020  mespaces:.      
-0001eeb0: 2020 2020 2020 2d20 6e61 6d65 7370 6163        - namespac
-0001eec0: 6573 0a20 2020 2020 2020 2020 2020 202d  es.            -
-0001eed0: 206e 616d 6573 7061 6365 730a 2020 2020   namespaces.    
-0001eee0: 2020 7072 6f70 6572 7469 6573 3a0a 2020    properties:.  
-0001eef0: 2020 2020 2020 6e6f 6465 5f61 6666 696e        node_affin
-0001ef00: 6974 793a 0a20 2020 2020 2020 2020 2024  ity:.          $
-0001ef10: 7265 663a 2027 232f 636f 6d70 6f6e 656e  ref: '#/componen
-0001ef20: 7473 2f73 6368 656d 6173 2f4e 6f64 6541  ts/schemas/NodeA
-0001ef30: 6666 696e 6974 7927 0a20 2020 2020 2020  ffinity'.       
-0001ef40: 2070 6f64 5f61 6666 696e 6974 793a 0a20   pod_affinity:. 
-0001ef50: 2020 2020 2020 2020 2024 7265 663a 2027           $ref: '
-0001ef60: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-0001ef70: 656d 6173 2f50 6f64 4166 6669 6e69 7479  emas/PodAffinity
-0001ef80: 270a 2020 2020 2020 2020 706f 645f 616e  '.        pod_an
-0001ef90: 7469 5f61 6666 696e 6974 793a 0a20 2020  ti_affinity:.   
-0001efa0: 2020 2020 2020 2024 7265 663a 2027 232f         $ref: '#/
-0001efb0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-0001efc0: 6173 2f50 6f64 416e 7469 4166 6669 6e69  as/PodAntiAffini
-0001efd0: 7479 270a 2020 2020 2020 7469 746c 653a  ty'.      title:
-0001efe0: 2041 6666 696e 6974 790a 2020 2020 2020   Affinity.      
-0001eff0: 7479 7065 3a20 6f62 6a65 6374 0a20 2020  type: object.   
-0001f000: 204e 6f64 6541 6666 696e 6974 793a 0a20   NodeAffinity:. 
-0001f010: 2020 2020 2065 7861 6d70 6c65 3a0a 2020       example:.  
-0001f020: 2020 2020 2020 7072 6566 6572 7265 645f        preferred_
-0001f030: 6475 7269 6e67 5f73 6368 6564 756c 696e  during_schedulin
-0001f040: 675f 6967 6e6f 7265 645f 6475 7269 6e67  g_ignored_during
-0001f050: 5f65 7865 6375 7469 6f6e 3a0a 2020 2020  _execution:.    
-0001f060: 2020 2020 2d20 7072 6566 6572 656e 6365      - preference
-0001f070: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-0001f080: 7463 685f 6578 7072 6573 7369 6f6e 733a  tch_expressions:
-0001f090: 0a20 2020 2020 2020 2020 2020 202d 2022  .            - "
-0001f0a0: 6b65 793a 7665 7273 696f 6e2c 206f 7065  key:version, ope
-0001f0b0: 7261 746f 723a 496e 2c20 7661 6c75 6573  rator:In, values
-0001f0c0: 3a5b 7631 2e30 2e30 2c20 7631 2e30 2e31  :[v1.0.0, v1.0.1
-0001f0d0: 5d22 0a20 2020 2020 2020 2020 2020 206d  ]".            m
-0001f0e0: 6174 6368 5f66 6965 6c64 733a 0a20 2020  atch_fields:.   
-0001f0f0: 2020 2020 2020 2020 202d 2022 6b65 793a           - "key:
-0001f100: 7665 7273 696f 6e2c 206f 7065 7261 746f  version, operato
-0001f110: 723a 496e 2c20 7661 6c75 6573 3a5b 7631  r:In, values:[v1
-0001f120: 2e30 2e30 2c20 7631 2e30 2e31 5d22 0a20  .0.0, v1.0.1]". 
-0001f130: 2020 2020 2020 2020 2077 6569 6768 743a           weight:
-0001f140: 2030 0a20 2020 2020 2020 202d 2070 7265   0.        - pre
-0001f150: 6665 7265 6e63 653a 0a20 2020 2020 2020  ference:.       
-0001f160: 2020 2020 206d 6174 6368 5f65 7870 7265       match_expre
-0001f170: 7373 696f 6e73 3a0a 2020 2020 2020 2020  ssions:.        
-0001f180: 2020 2020 2d20 226b 6579 3a76 6572 7369      - "key:versi
-0001f190: 6f6e 2c20 6f70 6572 6174 6f72 3a49 6e2c  on, operator:In,
-0001f1a0: 2076 616c 7565 733a 5b76 312e 302e 302c   values:[v1.0.0,
-0001f1b0: 2076 312e 302e 315d 220a 2020 2020 2020   v1.0.1]".      
-0001f1c0: 2020 2020 2020 6d61 7463 685f 6669 656c        match_fiel
-0001f1d0: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
-0001f1e0: 2d20 226b 6579 3a76 6572 7369 6f6e 2c20  - "key:version, 
-0001f1f0: 6f70 6572 6174 6f72 3a49 6e2c 2076 616c  operator:In, val
-0001f200: 7565 733a 5b76 312e 302e 302c 2076 312e  ues:[v1.0.0, v1.
-0001f210: 302e 315d 220a 2020 2020 2020 2020 2020  0.1]".          
-0001f220: 7765 6967 6874 3a20 300a 2020 2020 2020  weight: 0.      
-0001f230: 2020 7265 7175 6972 6564 5f64 7572 696e    required_durin
-0001f240: 675f 7363 6865 6475 6c69 6e67 5f69 676e  g_scheduling_ign
-0001f250: 6f72 6564 5f64 7572 696e 675f 6578 6563  ored_during_exec
-0001f260: 7574 696f 6e3a 0a20 2020 2020 2020 2020  ution:.         
-0001f270: 206e 6f64 655f 7365 6c65 6374 6f72 5f74   node_selector_t
-0001f280: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
-0001f290: 2d20 6d61 7463 685f 6578 7072 6573 7369  - match_expressi
-0001f2a0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-0001f2b0: 202d 2022 6b65 793a 7665 7273 696f 6e2c   - "key:version,
-0001f2c0: 206f 7065 7261 746f 723a 496e 2c20 7661   operator:In, va
-0001f2d0: 6c75 6573 3a5b 7631 2e30 2e30 2c20 7631  lues:[v1.0.0, v1
-0001f2e0: 2e30 2e31 5d22 0a20 2020 2020 2020 2020  .0.1]".         
-0001f2f0: 2020 206d 6174 6368 5f66 6965 6c64 733a     match_fields:
-0001f300: 0a20 2020 2020 2020 2020 2020 202d 2022  .            - "
-0001f310: 6b65 793a 7665 7273 696f 6e2c 206f 7065  key:version, ope
-0001f320: 7261 746f 723a 496e 2c20 7661 6c75 6573  rator:In, values
-0001f330: 3a5b 7631 2e30 2e30 2c20 7631 2e30 2e31  :[v1.0.0, v1.0.1
-0001f340: 5d22 0a20 2020 2020 2020 2020 202d 206d  ]".          - m
-0001f350: 6174 6368 5f65 7870 7265 7373 696f 6e73  atch_expressions
-0001f360: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
-0001f370: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
-0001f380: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
-0001f390: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
-0001f3a0: 315d 220a 2020 2020 2020 2020 2020 2020  1]".            
-0001f3b0: 6d61 7463 685f 6669 656c 6473 3a0a 2020  match_fields:.  
-0001f3c0: 2020 2020 2020 2020 2020 2d20 226b 6579            - "key
-0001f3d0: 3a76 6572 7369 6f6e 2c20 6f70 6572 6174  :version, operat
-0001f3e0: 6f72 3a49 6e2c 2076 616c 7565 733a 5b76  or:In, values:[v
-0001f3f0: 312e 302e 302c 2076 312e 302e 315d 220a  1.0.0, v1.0.1]".
-0001f400: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
-0001f410: 3a0a 2020 2020 2020 2020 7265 7175 6972  :.        requir
-0001f420: 6564 5f64 7572 696e 675f 7363 6865 6475  ed_during_schedu
-0001f430: 6c69 6e67 5f69 676e 6f72 6564 5f64 7572  ling_ignored_dur
-0001f440: 696e 675f 6578 6563 7574 696f 6e3a 0a20  ing_execution:. 
-0001f450: 2020 2020 2020 2020 2024 7265 663a 2027           $ref: '
-0001f460: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-0001f470: 656d 6173 2f4e 6f64 6553 656c 6563 746f  emas/NodeSelecto
-0001f480: 7227 0a20 2020 2020 2020 2070 7265 6665  r'.        prefe
-0001f490: 7272 6564 5f64 7572 696e 675f 7363 6865  rred_during_sche
-0001f4a0: 6475 6c69 6e67 5f69 676e 6f72 6564 5f64  duling_ignored_d
-0001f4b0: 7572 696e 675f 6578 6563 7574 696f 6e3a  uring_execution:
-0001f4c0: 0a20 2020 2020 2020 2020 2069 7465 6d73  .          items
-0001f4d0: 3a0a 2020 2020 2020 2020 2020 2020 2472  :.            $r
-0001f4e0: 6566 3a20 2723 2f63 6f6d 706f 6e65 6e74  ef: '#/component
-0001f4f0: 732f 7363 6865 6d61 732f 5072 6566 6572  s/schemas/Prefer
-0001f500: 7265 6453 6368 6564 756c 696e 6754 6572  redSchedulingTer
-0001f510: 6d27 0a20 2020 2020 2020 2020 2074 6974  m'.          tit
-0001f520: 6c65 3a20 7072 6566 6572 7265 645f 6475  le: preferred_du
-0001f530: 7269 6e67 5f73 6368 6564 756c 696e 675f  ring_scheduling_
-0001f540: 6967 6e6f 7265 645f 6475 7269 6e67 5f65  ignored_during_e
-0001f550: 7865 6375 7469 6f6e 0a20 2020 2020 2020  xecution.       
-0001f560: 2020 2074 7970 653a 2061 7272 6179 0a20     type: array. 
-0001f570: 2020 2020 2074 6974 6c65 3a20 4e6f 6465       title: Node
-0001f580: 4166 6669 6e69 7479 0a20 2020 2020 2074  Affinity.      t
-0001f590: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
-0001f5a0: 4e6f 6465 5365 6c65 6374 6f72 3a0a 2020  NodeSelector:.  
-0001f5b0: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
-0001f5c0: 2020 2020 206e 6f64 655f 7365 6c65 6374       node_select
-0001f5d0: 6f72 5f74 6572 6d73 3a0a 2020 2020 2020  or_terms:.      
-0001f5e0: 2020 2d20 6d61 7463 685f 6578 7072 6573    - match_expres
-0001f5f0: 7369 6f6e 733a 0a20 2020 2020 2020 2020  sions:.         
-0001f600: 202d 2022 6b65 793a 7665 7273 696f 6e2c   - "key:version,
-0001f610: 206f 7065 7261 746f 723a 496e 2c20 7661   operator:In, va
-0001f620: 6c75 6573 3a5b 7631 2e30 2e30 2c20 7631  lues:[v1.0.0, v1
-0001f630: 2e30 2e31 5d22 0a20 2020 2020 2020 2020  .0.1]".         
-0001f640: 206d 6174 6368 5f66 6965 6c64 733a 0a20   match_fields:. 
-0001f650: 2020 2020 2020 2020 202d 2022 6b65 793a           - "key:
-0001f660: 7665 7273 696f 6e2c 206f 7065 7261 746f  version, operato
-0001f670: 723a 496e 2c20 7661 6c75 6573 3a5b 7631  r:In, values:[v1
-0001f680: 2e30 2e30 2c20 7631 2e30 2e31 5d22 0a20  .0.0, v1.0.1]". 
-0001f690: 2020 2020 2020 202d 206d 6174 6368 5f65         - match_e
-0001f6a0: 7870 7265 7373 696f 6e73 3a0a 2020 2020  xpressions:.    
-0001f6b0: 2020 2020 2020 2d20 226b 6579 3a76 6572        - "key:ver
-0001f6c0: 7369 6f6e 2c20 6f70 6572 6174 6f72 3a49  sion, operator:I
-0001f6d0: 6e2c 2076 616c 7565 733a 5b76 312e 302e  n, values:[v1.0.
-0001f6e0: 302c 2076 312e 302e 315d 220a 2020 2020  0, v1.0.1]".    
-0001f6f0: 2020 2020 2020 6d61 7463 685f 6669 656c        match_fiel
-0001f700: 6473 3a0a 2020 2020 2020 2020 2020 2d20  ds:.          - 
-0001f710: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
-0001f720: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
-0001f730: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
-0001f740: 315d 220a 2020 2020 2020 7072 6f70 6572  1]".      proper
-0001f750: 7469 6573 3a0a 2020 2020 2020 2020 6e6f  ties:.        no
-0001f760: 6465 5f73 656c 6563 746f 725f 7465 726d  de_selector_term
-0001f770: 733a 0a20 2020 2020 2020 2020 2069 7465  s:.          ite
-0001f780: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-0001f790: 2472 6566 3a20 2723 2f63 6f6d 706f 6e65  $ref: '#/compone
-0001f7a0: 6e74 732f 7363 6865 6d61 732f 4e6f 6465  nts/schemas/Node
-0001f7b0: 5365 6c65 6374 6f72 5465 726d 270a 2020  SelectorTerm'.  
-0001f7c0: 2020 2020 2020 2020 7469 746c 653a 206e          title: n
-0001f7d0: 6f64 655f 7365 6c65 6374 6f72 5f74 6572  ode_selector_ter
-0001f7e0: 6d73 0a20 2020 2020 2020 2020 2074 7970  ms.          typ
-0001f7f0: 653a 2061 7272 6179 0a20 2020 2020 2074  e: array.      t
-0001f800: 6974 6c65 3a20 4e6f 6465 5365 6c65 6374  itle: NodeSelect
-0001f810: 6f72 0a20 2020 2020 2074 7970 653a 206f  or.      type: o
-0001f820: 626a 6563 740a 2020 2020 4e6f 6465 5365  bject.    NodeSe
-0001f830: 6c65 6374 6f72 5465 726d 3a0a 2020 2020  lectorTerm:.    
-0001f840: 2020 6578 616d 706c 653a 0a20 2020 2020    example:.     
-0001f850: 2020 206d 6174 6368 5f65 7870 7265 7373     match_express
-0001f860: 696f 6e73 3a0a 2020 2020 2020 2020 2d20  ions:.        - 
-0001f870: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
-0001f880: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
-0001f890: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
-0001f8a0: 315d 220a 2020 2020 2020 2020 6d61 7463  1]".        matc
-0001f8b0: 685f 6669 656c 6473 3a0a 2020 2020 2020  h_fields:.      
-0001f8c0: 2020 2d20 226b 6579 3a76 6572 7369 6f6e    - "key:version
-0001f8d0: 2c20 6f70 6572 6174 6f72 3a49 6e2c 2076  , operator:In, v
-0001f8e0: 616c 7565 733a 5b76 312e 302e 302c 2076  alues:[v1.0.0, v
-0001f8f0: 312e 302e 315d 220a 2020 2020 2020 7072  1.0.1]".      pr
-0001f900: 6f70 6572 7469 6573 3a0a 2020 2020 2020  operties:.      
-0001f910: 2020 6d61 7463 685f 6578 7072 6573 7369    match_expressi
-0001f920: 6f6e 733a 0a20 2020 2020 2020 2020 2064  ons:.          d
-0001f930: 6573 6372 6970 7469 6f6e 3a20 7c0a 2020  escription: |.  
-0001f940: 2020 2020 2020 2020 2020 416e 2061 7272            An arr
-0001f950: 6179 206f 6620 6e6f 6465 2073 656c 6563  ay of node selec
-0001f960: 746f 7220 7275 6c65 2c20 7468 6520 7275  tor rule, the ru
-0001f970: 6c65 2063 616e 2062 6520 6120 6d61 7463  le can be a matc
-0001f980: 6820 6578 7072 6573 7369 6f6e 2c0a 2020  h expression,.  
-0001f990: 2020 2020 2020 2020 2020 7265 6665 7272            referr
-0001f9a0: 696e 6720 7468 6520 6578 616d 706c 6520  ing the example 
-0001f9b0: 2849 7420 6973 2061 206d 6174 6368 2065  (It is a match e
-0001f9c0: 7870 7265 7373 696f 6e29 0a20 2020 2020  xpression).     
-0001f9d0: 2020 2020 2065 7861 6d70 6c65 3a0a 2020       example:.  
-0001f9e0: 2020 2020 2020 2020 2d20 226b 6579 3a76          - "key:v
-0001f9f0: 6572 7369 6f6e 2c20 6f70 6572 6174 6f72  ersion, operator
-0001fa00: 3a49 6e2c 2076 616c 7565 733a 5b76 312e  :In, values:[v1.
-0001fa10: 302e 302c 2076 312e 302e 315d 220a 2020  0.0, v1.0.1]".  
-0001fa20: 2020 2020 2020 2020 6974 656d 733a 0a20          items:. 
-0001fa30: 2020 2020 2020 2020 2020 2074 7970 653a             type:
-0001fa40: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-0001fa50: 2020 7469 746c 653a 204e 6f64 6553 656c    title: NodeSel
-0001fa60: 6563 746f 7252 6571 7569 7265 6d65 6e74  ectorRequirement
-0001fa70: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
-0001fa80: 2061 7272 6179 0a20 2020 2020 2020 206d   array.        m
-0001fa90: 6174 6368 5f66 6965 6c64 733a 0a20 2020  atch_fields:.   
-0001faa0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-0001fab0: 6f6e 3a20 7c0a 2020 2020 2020 2020 2020  on: |.          
-0001fac0: 2020 416e 2061 7272 6179 206f 6620 6e6f    An array of no
-0001fad0: 6465 2073 656c 6563 746f 7220 7275 6c65  de selector rule
-0001fae0: 2c20 7468 6520 7275 6c65 2063 616e 2062  , the rule can b
-0001faf0: 6520 6120 6d61 7463 6820 6578 7072 6573  e a match expres
-0001fb00: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
-0001fb10: 2020 7265 6665 7272 696e 6720 7468 6520    referring the 
-0001fb20: 6578 616d 706c 6520 2849 7420 6973 2061  example (It is a
-0001fb30: 206d 6174 6368 2065 7870 7265 7373 696f   match expressio
-0001fb40: 6e29 0a20 2020 2020 2020 2020 2065 7861  n).          exa
-0001fb50: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
-0001fb60: 2d20 226b 6579 3a76 6572 7369 6f6e 2c20  - "key:version, 
-0001fb70: 6f70 6572 6174 6f72 3a49 6e2c 2076 616c  operator:In, val
-0001fb80: 7565 733a 5b76 312e 302e 302c 2076 312e  ues:[v1.0.0, v1.
-0001fb90: 302e 315d 220a 2020 2020 2020 2020 2020  0.1]".          
-0001fba0: 6974 656d 733a 0a20 2020 2020 2020 2020  items:.         
-0001fbb0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
-0001fbc0: 2020 2020 2020 2020 2020 7469 746c 653a            title:
-0001fbd0: 204e 6f64 6553 656c 6563 746f 7252 6571   NodeSelectorReq
-0001fbe0: 7569 7265 6d65 6e74 0a20 2020 2020 2020  uirement.       
-0001fbf0: 2020 2074 7970 653a 2061 7272 6179 0a20     type: array. 
-0001fc00: 2020 2020 2074 6974 6c65 3a20 4e6f 6465       title: Node
-0001fc10: 5365 6c65 6374 6f72 5465 726d 0a20 2020  SelectorTerm.   
-0001fc20: 2020 2074 7970 653a 206f 626a 6563 740a     type: object.
-0001fc30: 2020 2020 4e6f 6465 5365 6c65 6374 6f72      NodeSelector
-0001fc40: 5265 7175 6972 656d 656e 743a 0a20 2020  Requirement:.   
-0001fc50: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-0001fc60: 7c0a 2020 2020 2020 2020 416e 2061 7272  |.        An arr
-0001fc70: 6179 206f 6620 6e6f 6465 2073 656c 6563  ay of node selec
-0001fc80: 746f 7220 7275 6c65 2c20 7468 6520 7275  tor rule, the ru
-0001fc90: 6c65 2063 616e 2062 6520 6120 6d61 7463  le can be a matc
-0001fca0: 6820 6578 7072 6573 7369 6f6e 2c0a 2020  h expression,.  
-0001fcb0: 2020 2020 2020 7265 6665 7272 696e 6720        referring 
-0001fcc0: 7468 6520 6578 616d 706c 6520 2849 7420  the example (It 
-0001fcd0: 6973 2061 206d 6174 6368 2065 7870 7265  is a match expre
-0001fce0: 7373 696f 6e29 0a20 2020 2020 2065 7861  ssion).      exa
-0001fcf0: 6d70 6c65 3a0a 2020 2020 2020 2d20 226b  mple:.      - "k
-0001fd00: 6579 3a76 6572 7369 6f6e 2c20 6f70 6572  ey:version, oper
-0001fd10: 6174 6f72 3a49 6e2c 2076 616c 7565 733a  ator:In, values:
-0001fd20: 5b76 312e 302e 302c 2076 312e 302e 315d  [v1.0.0, v1.0.1]
-0001fd30: 220a 2020 2020 2020 6974 656d 733a 0a20  ".      items:. 
-0001fd40: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-0001fd50: 696e 670a 2020 2020 2020 7469 746c 653a  ing.      title:
-0001fd60: 204e 6f64 6553 656c 6563 746f 7252 6571   NodeSelectorReq
-0001fd70: 7569 7265 6d65 6e74 0a20 2020 2020 2074  uirement.      t
-0001fd80: 7970 653a 2061 7272 6179 0a20 2020 2050  ype: array.    P
-0001fd90: 7265 6665 7272 6564 5363 6865 6475 6c69  referredScheduli
-0001fda0: 6e67 5465 726d 3a0a 2020 2020 2020 6578  ngTerm:.      ex
-0001fdb0: 616d 706c 653a 0a20 2020 2020 2020 2070  ample:.        p
-0001fdc0: 7265 6665 7265 6e63 653a 0a20 2020 2020  reference:.     
-0001fdd0: 2020 2020 206d 6174 6368 5f65 7870 7265       match_expre
-0001fde0: 7373 696f 6e73 3a0a 2020 2020 2020 2020  ssions:.        
-0001fdf0: 2020 2d20 226b 6579 3a76 6572 7369 6f6e    - "key:version
-0001fe00: 2c20 6f70 6572 6174 6f72 3a49 6e2c 2076  , operator:In, v
-0001fe10: 616c 7565 733a 5b76 312e 302e 302c 2076  alues:[v1.0.0, v
-0001fe20: 312e 302e 315d 220a 2020 2020 2020 2020  1.0.1]".        
-0001fe30: 2020 6d61 7463 685f 6669 656c 6473 3a0a    match_fields:.
-0001fe40: 2020 2020 2020 2020 2020 2d20 226b 6579            - "key
-0001fe50: 3a76 6572 7369 6f6e 2c20 6f70 6572 6174  :version, operat
-0001fe60: 6f72 3a49 6e2c 2076 616c 7565 733a 5b76  or:In, values:[v
-0001fe70: 312e 302e 302c 2076 312e 302e 315d 220a  1.0.0, v1.0.1]".
-0001fe80: 2020 2020 2020 2020 7765 6967 6874 3a20          weight: 
-0001fe90: 300a 2020 2020 2020 7072 6f70 6572 7469  0.      properti
-0001fea0: 6573 3a0a 2020 2020 2020 2020 7765 6967  es:.        weig
-0001feb0: 6874 3a0a 2020 2020 2020 2020 2020 7469  ht:.          ti
-0001fec0: 746c 653a 2077 6569 6768 740a 2020 2020  tle: weight.    
-0001fed0: 2020 2020 2020 7479 7065 3a20 696e 7465        type: inte
-0001fee0: 6765 720a 2020 2020 2020 2020 7072 6566  ger.        pref
-0001fef0: 6572 656e 6365 3a0a 2020 2020 2020 2020  erence:.        
-0001ff00: 2020 2472 6566 3a20 2723 2f63 6f6d 706f    $ref: '#/compo
-0001ff10: 6e65 6e74 732f 7363 6865 6d61 732f 4e6f  nents/schemas/No
-0001ff20: 6465 5365 6c65 6374 6f72 5465 726d 270a  deSelectorTerm'.
-0001ff30: 2020 2020 2020 7469 746c 653a 2050 7265        title: Pre
-0001ff40: 6665 7272 6564 5363 6865 6475 6c69 6e67  ferredScheduling
-0001ff50: 5465 726d 0a20 2020 2020 2074 7970 653a  Term.      type:
-0001ff60: 206f 626a 6563 740a 2020 2020 506f 6441   object.    PodA
-0001ff70: 6666 696e 6974 793a 0a20 2020 2020 2065  ffinity:.      e
-0001ff80: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
-0001ff90: 7072 6566 6572 7265 645f 6475 7269 6e67  preferred_during
-0001ffa0: 5f73 6368 6564 756c 696e 675f 6967 6e6f  _scheduling_igno
-0001ffb0: 7265 645f 6475 7269 6e67 5f65 7865 6375  red_during_execu
-0001ffc0: 7469 6f6e 3a0a 2020 2020 2020 2020 2d20  tion:.        - 
-0001ffd0: 7765 6967 6874 3a20 360a 2020 2020 2020  weight: 6.      
-0001ffe0: 2020 2020 706f 645f 6166 6669 6e69 7479      pod_affinity
-0001fff0: 5f74 6572 6d3a 0a20 2020 2020 2020 2020  _term:.         
-00020000: 2020 206c 6162 656c 5f73 656c 6563 746f     label_selecto
-00020010: 723a 0a20 2020 2020 2020 2020 2020 202d  r:.            -
-00020020: 2061 7070 3a64 656d 6f2d 6170 700a 2020   app:demo-app.  
-00020030: 2020 2020 2020 2020 2020 2d20 226b 6579            - "key
-00020040: 3a76 6572 7369 6f6e 2c20 6f70 6572 6174  :version, operat
-00020050: 6f72 3a49 6e2c 2076 616c 7565 733a 5b76  or:In, values:[v
-00020060: 312e 302e 302c 2076 312e 302e 315d 220a  1.0.0, v1.0.1]".
-00020070: 2020 2020 2020 2020 2020 2020 746f 706f              topo
-00020080: 6c6f 6779 5f6b 6579 3a20 746f 706f 6c6f  logy_key: topolo
-00020090: 6779 5f6b 6579 0a20 2020 2020 2020 2020  gy_key.         
-000200a0: 2020 206e 616d 6573 7061 6365 733a 0a20     namespaces:. 
-000200b0: 2020 2020 2020 2020 2020 202d 206e 616d             - nam
-000200c0: 6573 7061 6365 730a 2020 2020 2020 2020  espaces.        
-000200d0: 2020 2020 2d20 6e61 6d65 7370 6163 6573      - namespaces
-000200e0: 0a20 2020 2020 2020 202d 2077 6569 6768  .        - weigh
-000200f0: 743a 2036 0a20 2020 2020 2020 2020 2070  t: 6.          p
-00020100: 6f64 5f61 6666 696e 6974 795f 7465 726d  od_affinity_term
-00020110: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
-00020120: 6265 6c5f 7365 6c65 6374 6f72 3a0a 2020  bel_selector:.  
-00020130: 2020 2020 2020 2020 2020 2d20 6170 703a            - app:
-00020140: 6465 6d6f 2d61 7070 0a20 2020 2020 2020  demo-app.       
-00020150: 2020 2020 202d 2022 6b65 793a 7665 7273       - "key:vers
-00020160: 696f 6e2c 206f 7065 7261 746f 723a 496e  ion, operator:In
-00020170: 2c20 7661 6c75 6573 3a5b 7631 2e30 2e30  , values:[v1.0.0
-00020180: 2c20 7631 2e30 2e31 5d22 0a20 2020 2020  , v1.0.1]".     
-00020190: 2020 2020 2020 2074 6f70 6f6c 6f67 795f         topology_
-000201a0: 6b65 793a 2074 6f70 6f6c 6f67 795f 6b65  key: topology_ke
-000201b0: 790a 2020 2020 2020 2020 2020 2020 6e61  y.            na
-000201c0: 6d65 7370 6163 6573 3a0a 2020 2020 2020  mespaces:.      
-000201d0: 2020 2020 2020 2d20 6e61 6d65 7370 6163        - namespac
-000201e0: 6573 0a20 2020 2020 2020 2020 2020 202d  es.            -
-000201f0: 206e 616d 6573 7061 6365 730a 2020 2020   namespaces.    
-00020200: 2020 2020 7265 7175 6972 6564 5f64 7572      required_dur
-00020210: 696e 675f 7363 6865 6475 6c69 6e67 5f69  ing_scheduling_i
-00020220: 676e 6f72 6564 5f64 7572 696e 675f 6578  gnored_during_ex
-00020230: 6563 7574 696f 6e3a 0a20 2020 2020 2020  ecution:.       
-00020240: 202d 206c 6162 656c 5f73 656c 6563 746f   - label_selecto
-00020250: 723a 0a20 2020 2020 2020 2020 202d 2061  r:.          - a
-00020260: 7070 3a64 656d 6f2d 6170 700a 2020 2020  pp:demo-app.    
-00020270: 2020 2020 2020 2d20 226b 6579 3a76 6572        - "key:ver
-00020280: 7369 6f6e 2c20 6f70 6572 6174 6f72 3a49  sion, operator:I
-00020290: 6e2c 2076 616c 7565 733a 5b76 312e 302e  n, values:[v1.0.
-000202a0: 302c 2076 312e 302e 315d 220a 2020 2020  0, v1.0.1]".    
-000202b0: 2020 2020 2020 746f 706f 6c6f 6779 5f6b        topology_k
-000202c0: 6579 3a20 746f 706f 6c6f 6779 5f6b 6579  ey: topology_key
-000202d0: 0a20 2020 2020 2020 2020 206e 616d 6573  .          names
-000202e0: 7061 6365 733a 0a20 2020 2020 2020 2020  paces:.         
-000202f0: 202d 206e 616d 6573 7061 6365 730a 2020   - namespaces.  
-00020300: 2020 2020 2020 2020 2d20 6e61 6d65 7370          - namesp
-00020310: 6163 6573 0a20 2020 2020 2020 202d 206c  aces.        - l
-00020320: 6162 656c 5f73 656c 6563 746f 723a 0a20  abel_selector:. 
-00020330: 2020 2020 2020 2020 202d 2061 7070 3a64           - app:d
-00020340: 656d 6f2d 6170 700a 2020 2020 2020 2020  emo-app.        
-00020350: 2020 2d20 226b 6579 3a76 6572 7369 6f6e    - "key:version
-00020360: 2c20 6f70 6572 6174 6f72 3a49 6e2c 2076  , operator:In, v
-00020370: 616c 7565 733a 5b76 312e 302e 302c 2076  alues:[v1.0.0, v
-00020380: 312e 302e 315d 220a 2020 2020 2020 2020  1.0.1]".        
-00020390: 2020 746f 706f 6c6f 6779 5f6b 6579 3a20    topology_key: 
-000203a0: 746f 706f 6c6f 6779 5f6b 6579 0a20 2020  topology_key.   
-000203b0: 2020 2020 2020 206e 616d 6573 7061 6365         namespace
-000203c0: 733a 0a20 2020 2020 2020 2020 202d 206e  s:.          - n
-000203d0: 616d 6573 7061 6365 730a 2020 2020 2020  amespaces.      
-000203e0: 2020 2020 2d20 6e61 6d65 7370 6163 6573      - namespaces
-000203f0: 0a20 2020 2020 2070 726f 7065 7274 6965  .      propertie
-00020400: 733a 0a20 2020 2020 2020 2072 6571 7569  s:.        requi
-00020410: 7265 645f 6475 7269 6e67 5f73 6368 6564  red_during_sched
-00020420: 756c 696e 675f 6967 6e6f 7265 645f 6475  uling_ignored_du
-00020430: 7269 6e67 5f65 7865 6375 7469 6f6e 3a0a  ring_execution:.
-00020440: 2020 2020 2020 2020 2020 6974 656d 733a            items:
-00020450: 0a20 2020 2020 2020 2020 2020 2024 7265  .            $re
-00020460: 663a 2027 232f 636f 6d70 6f6e 656e 7473  f: '#/components
-00020470: 2f73 6368 656d 6173 2f50 6f64 4166 6669  /schemas/PodAffi
-00020480: 6e69 7479 5465 726d 270a 2020 2020 2020  nityTerm'.      
-00020490: 2020 2020 7469 746c 653a 2072 6571 7569      title: requi
-000204a0: 7265 645f 6475 7269 6e67 5f73 6368 6564  red_during_sched
-000204b0: 756c 696e 675f 6967 6e6f 7265 645f 6475  uling_ignored_du
-000204c0: 7269 6e67 5f65 7865 6375 7469 6f6e 0a20  ring_execution. 
-000204d0: 2020 2020 2020 2020 2074 7970 653a 2061           type: a
-000204e0: 7272 6179 0a20 2020 2020 2020 2070 7265  rray.        pre
-000204f0: 6665 7272 6564 5f64 7572 696e 675f 7363  ferred_during_sc
-00020500: 6865 6475 6c69 6e67 5f69 676e 6f72 6564  heduling_ignored
-00020510: 5f64 7572 696e 675f 6578 6563 7574 696f  _during_executio
-00020520: 6e3a 0a20 2020 2020 2020 2020 2069 7465  n:.          ite
-00020530: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00020540: 2472 6566 3a20 2723 2f63 6f6d 706f 6e65  $ref: '#/compone
-00020550: 6e74 732f 7363 6865 6d61 732f 5765 6967  nts/schemas/Weig
-00020560: 6874 6564 506f 6441 6666 696e 6974 7954  htedPodAffinityT
-00020570: 6572 6d27 0a20 2020 2020 2020 2020 2074  erm'.          t
-00020580: 6974 6c65 3a20 7072 6566 6572 7265 645f  itle: preferred_
-00020590: 6475 7269 6e67 5f73 6368 6564 756c 696e  during_schedulin
-000205a0: 675f 6967 6e6f 7265 645f 6475 7269 6e67  g_ignored_during
-000205b0: 5f65 7865 6375 7469 6f6e 0a20 2020 2020  _execution.     
-000205c0: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
-000205d0: 0a20 2020 2020 2074 6974 6c65 3a20 506f  .      title: Po
-000205e0: 6441 6666 696e 6974 790a 2020 2020 2020  dAffinity.      
-000205f0: 7479 7065 3a20 6f62 6a65 6374 0a20 2020  type: object.   
-00020600: 2050 6f64 4166 6669 6e69 7479 5465 726d   PodAffinityTerm
-00020610: 3a0a 2020 2020 2020 6578 616d 706c 653a  :.      example:
-00020620: 0a20 2020 2020 2020 206c 6162 656c 5f73  .        label_s
-00020630: 656c 6563 746f 723a 0a20 2020 2020 2020  elector:.       
-00020640: 202d 2061 7070 3a64 656d 6f2d 6170 700a   - app:demo-app.
-00020650: 2020 2020 2020 2020 2d20 226b 6579 3a76          - "key:v
-00020660: 6572 7369 6f6e 2c20 6f70 6572 6174 6f72  ersion, operator
-00020670: 3a49 6e2c 2076 616c 7565 733a 5b76 312e  :In, values:[v1.
-00020680: 302e 302c 2076 312e 302e 315d 220a 2020  0.0, v1.0.1]".  
-00020690: 2020 2020 2020 746f 706f 6c6f 6779 5f6b        topology_k
-000206a0: 6579 3a20 746f 706f 6c6f 6779 5f6b 6579  ey: topology_key
-000206b0: 0a20 2020 2020 2020 206e 616d 6573 7061  .        namespa
-000206c0: 6365 733a 0a20 2020 2020 2020 202d 206e  ces:.        - n
-000206d0: 616d 6573 7061 6365 730a 2020 2020 2020  amespaces.      
-000206e0: 2020 2d20 6e61 6d65 7370 6163 6573 0a20    - namespaces. 
-000206f0: 2020 2020 2070 726f 7065 7274 6965 733a       properties:
-00020700: 0a20 2020 2020 2020 206c 6162 656c 5f73  .        label_s
-00020710: 656c 6563 746f 723a 0a20 2020 2020 2020  elector:.       
-00020720: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-00020730: 7c0a 2020 2020 2020 2020 2020 2020 416e  |.            An
-00020740: 2061 7272 6179 206f 6620 6c61 6265 6c20   array of label 
-00020750: 7365 6c65 6374 6f72 2072 756c 652c 2074  selector rule, t
-00020760: 6865 2072 756c 6520 6361 6e20 6569 7468  he rule can eith
-00020770: 6572 2062 6520 6120 6d61 7463 6820 6c61  er be a match la
-00020780: 6265 6c20 6f72 206d 6174 6368 2065 7870  bel or match exp
-00020790: 7265 7373 696f 6e2c 0a20 2020 2020 2020  ression,.       
-000207a0: 2020 2020 2072 6566 6572 7269 6e67 2074       referring t
-000207b0: 6865 2065 7861 6d70 6c65 2028 6669 7273  he example (firs
-000207c0: 7420 6973 2061 206d 6174 6368 206c 6162  t is a match lab
-000207d0: 656c 2c20 7365 636f 6e64 2069 7320 6120  el, second is a 
-000207e0: 6d61 7463 6820 6578 7072 6573 7369 6f6e  match expression
-000207f0: 290a 2020 2020 2020 2020 2020 6578 616d  ).          exam
-00020800: 706c 653a 0a20 2020 2020 2020 2020 202d  ple:.          -
-00020810: 2061 7070 3a64 656d 6f2d 6170 700a 2020   app:demo-app.  
-00020820: 2020 2020 2020 2020 2d20 226b 6579 3a76          - "key:v
-00020830: 6572 7369 6f6e 2c20 6f70 6572 6174 6f72  ersion, operator
-00020840: 3a49 6e2c 2076 616c 7565 733a 5b76 312e  :In, values:[v1.
-00020850: 302e 302c 2076 312e 302e 315d 220a 2020  0.0, v1.0.1]".  
-00020860: 2020 2020 2020 2020 6974 656d 733a 0a20          items:. 
-00020870: 2020 2020 2020 2020 2020 2074 7970 653a             type:
-00020880: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-00020890: 2020 7469 746c 653a 204c 6162 656c 5365    title: LabelSe
-000208a0: 6c65 6374 6f72 0a20 2020 2020 2020 2020  lector.         
-000208b0: 2074 7970 653a 2061 7272 6179 0a20 2020   type: array.   
-000208c0: 2020 2020 206e 616d 6573 7061 6365 733a       namespaces:
-000208d0: 0a20 2020 2020 2020 2020 2069 7465 6d73  .          items
-000208e0: 3a0a 2020 2020 2020 2020 2020 2020 7479  :.            ty
-000208f0: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
-00020900: 2020 2020 2074 6974 6c65 3a20 6e61 6d65       title: name
-00020910: 7370 6163 6573 0a20 2020 2020 2020 2020  spaces.         
-00020920: 2074 7970 653a 2061 7272 6179 0a20 2020   type: array.   
-00020930: 2020 2020 2074 6f70 6f6c 6f67 795f 6b65       topology_ke
-00020940: 793a 0a20 2020 2020 2020 2020 2074 6974  y:.          tit
-00020950: 6c65 3a20 746f 706f 6c6f 6779 5f6b 6579  le: topology_key
-00020960: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
-00020970: 2073 7472 696e 670a 2020 2020 2020 7469   string.      ti
-00020980: 746c 653a 2050 6f64 4166 6669 6e69 7479  tle: PodAffinity
-00020990: 5465 726d 0a20 2020 2020 2074 7970 653a  Term.      type:
-000209a0: 206f 626a 6563 740a 2020 2020 5765 6967   object.    Weig
-000209b0: 6874 6564 506f 6441 6666 696e 6974 7954  htedPodAffinityT
-000209c0: 6572 6d3a 0a20 2020 2020 2065 7861 6d70  erm:.      examp
-000209d0: 6c65 3a0a 2020 2020 2020 2020 7765 6967  le:.        weig
-000209e0: 6874 3a20 360a 2020 2020 2020 2020 706f  ht: 6.        po
-000209f0: 645f 6166 6669 6e69 7479 5f74 6572 6d3a  d_affinity_term:
-00020a00: 0a20 2020 2020 2020 2020 206c 6162 656c  .          label
-00020a10: 5f73 656c 6563 746f 723a 0a20 2020 2020  _selector:.     
-00020a20: 2020 2020 202d 2061 7070 3a64 656d 6f2d       - app:demo-
-00020a30: 6170 700a 2020 2020 2020 2020 2020 2d20  app.          - 
-00020a40: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
-00020a50: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
-00020a60: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
-00020a70: 315d 220a 2020 2020 2020 2020 2020 746f  1]".          to
-00020a80: 706f 6c6f 6779 5f6b 6579 3a20 746f 706f  pology_key: topo
-00020a90: 6c6f 6779 5f6b 6579 0a20 2020 2020 2020  logy_key.       
-00020aa0: 2020 206e 616d 6573 7061 6365 733a 0a20     namespaces:. 
-00020ab0: 2020 2020 2020 2020 202d 206e 616d 6573           - names
-00020ac0: 7061 6365 730a 2020 2020 2020 2020 2020  paces.          
-00020ad0: 2d20 6e61 6d65 7370 6163 6573 0a20 2020  - namespaces.   
-00020ae0: 2020 2070 726f 7065 7274 6965 733a 0a20     properties:. 
-00020af0: 2020 2020 2020 2077 6569 6768 743a 0a20         weight:. 
-00020b00: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-00020b10: 7765 6967 6874 0a20 2020 2020 2020 2020  weight.         
-00020b20: 2074 7970 653a 2069 6e74 6567 6572 0a20   type: integer. 
-00020b30: 2020 2020 2020 2070 6f64 5f61 6666 696e         pod_affin
-00020b40: 6974 795f 7465 726d 3a0a 2020 2020 2020  ity_term:.      
-00020b50: 2020 2020 2472 6566 3a20 2723 2f63 6f6d      $ref: '#/com
-00020b60: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00020b70: 506f 6441 6666 696e 6974 7954 6572 6d27  PodAffinityTerm'
-00020b80: 0a20 2020 2020 2074 6974 6c65 3a20 5765  .      title: We
-00020b90: 6967 6874 6564 506f 6441 6666 696e 6974  ightedPodAffinit
-00020ba0: 7954 6572 6d0a 2020 2020 2020 7479 7065  yTerm.      type
-00020bb0: 3a20 6f62 6a65 6374 0a20 2020 2050 6f64  : object.    Pod
-00020bc0: 416e 7469 4166 6669 6e69 7479 3a0a 2020  AntiAffinity:.  
-00020bd0: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
-00020be0: 2020 2020 2070 7265 6665 7272 6564 5f64       preferred_d
-00020bf0: 7572 696e 675f 7363 6865 6475 6c69 6e67  uring_scheduling
-00020c00: 5f69 676e 6f72 6564 5f64 7572 696e 675f  _ignored_during_
-00020c10: 6578 6563 7574 696f 6e3a 0a20 2020 2020  execution:.     
-00020c20: 2020 202d 2077 6569 6768 743a 2036 0a20     - weight: 6. 
-00020c30: 2020 2020 2020 2020 2070 6f64 5f61 6666           pod_aff
-00020c40: 696e 6974 795f 7465 726d 3a0a 2020 2020  inity_term:.    
-00020c50: 2020 2020 2020 2020 6c61 6265 6c5f 7365          label_se
-00020c60: 6c65 6374 6f72 3a0a 2020 2020 2020 2020  lector:.        
-00020c70: 2020 2020 2d20 6170 703a 6465 6d6f 2d61      - app:demo-a
-00020c80: 7070 0a20 2020 2020 2020 2020 2020 202d  pp.            -
-00020c90: 2022 6b65 793a 7665 7273 696f 6e2c 206f   "key:version, o
-00020ca0: 7065 7261 746f 723a 496e 2c20 7661 6c75  perator:In, valu
-00020cb0: 6573 3a5b 7631 2e30 2e30 2c20 7631 2e30  es:[v1.0.0, v1.0
-00020cc0: 2e31 5d22 0a20 2020 2020 2020 2020 2020  .1]".           
-00020cd0: 2074 6f70 6f6c 6f67 795f 6b65 793a 2074   topology_key: t
-00020ce0: 6f70 6f6c 6f67 795f 6b65 790a 2020 2020  opology_key.    
-00020cf0: 2020 2020 2020 2020 6e61 6d65 7370 6163          namespac
-00020d00: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00020d10: 2d20 6e61 6d65 7370 6163 6573 0a20 2020  - namespaces.   
-00020d20: 2020 2020 2020 2020 202d 206e 616d 6573           - names
-00020d30: 7061 6365 730a 2020 2020 2020 2020 2d20  paces.        - 
-00020d40: 7765 6967 6874 3a20 360a 2020 2020 2020  weight: 6.      
-00020d50: 2020 2020 706f 645f 6166 6669 6e69 7479      pod_affinity
-00020d60: 5f74 6572 6d3a 0a20 2020 2020 2020 2020  _term:.         
-00020d70: 2020 206c 6162 656c 5f73 656c 6563 746f     label_selecto
-00020d80: 723a 0a20 2020 2020 2020 2020 2020 202d  r:.            -
-00020d90: 2061 7070 3a64 656d 6f2d 6170 700a 2020   app:demo-app.  
-00020da0: 2020 2020 2020 2020 2020 2d20 226b 6579            - "key
-00020db0: 3a76 6572 7369 6f6e 2c20 6f70 6572 6174  :version, operat
-00020dc0: 6f72 3a49 6e2c 2076 616c 7565 733a 5b76  or:In, values:[v
-00020dd0: 312e 302e 302c 2076 312e 302e 315d 220a  1.0.0, v1.0.1]".
-00020de0: 2020 2020 2020 2020 2020 2020 746f 706f              topo
-00020df0: 6c6f 6779 5f6b 6579 3a20 746f 706f 6c6f  logy_key: topolo
-00020e00: 6779 5f6b 6579 0a20 2020 2020 2020 2020  gy_key.         
-00020e10: 2020 206e 616d 6573 7061 6365 733a 0a20     namespaces:. 
-00020e20: 2020 2020 2020 2020 2020 202d 206e 616d             - nam
-00020e30: 6573 7061 6365 730a 2020 2020 2020 2020  espaces.        
-00020e40: 2020 2020 2d20 6e61 6d65 7370 6163 6573      - namespaces
-00020e50: 0a20 2020 2020 2020 2072 6571 7569 7265  .        require
-00020e60: 645f 6475 7269 6e67 5f73 6368 6564 756c  d_during_schedul
-00020e70: 696e 675f 6967 6e6f 7265 645f 6475 7269  ing_ignored_duri
-00020e80: 6e67 5f65 7865 6375 7469 6f6e 3a0a 2020  ng_execution:.  
-00020e90: 2020 2020 2020 2d20 6c61 6265 6c5f 7365        - label_se
-00020ea0: 6c65 6374 6f72 3a0a 2020 2020 2020 2020  lector:.        
-00020eb0: 2020 2d20 6170 703a 6465 6d6f 2d61 7070    - app:demo-app
-00020ec0: 0a20 2020 2020 2020 2020 202d 2022 6b65  .          - "ke
-00020ed0: 793a 7665 7273 696f 6e2c 206f 7065 7261  y:version, opera
-00020ee0: 746f 723a 496e 2c20 7661 6c75 6573 3a5b  tor:In, values:[
-00020ef0: 7631 2e30 2e30 2c20 7631 2e30 2e31 5d22  v1.0.0, v1.0.1]"
-00020f00: 0a20 2020 2020 2020 2020 2074 6f70 6f6c  .          topol
-00020f10: 6f67 795f 6b65 793a 2074 6f70 6f6c 6f67  ogy_key: topolog
-00020f20: 795f 6b65 790a 2020 2020 2020 2020 2020  y_key.          
-00020f30: 6e61 6d65 7370 6163 6573 3a0a 2020 2020  namespaces:.    
-00020f40: 2020 2020 2020 2d20 6e61 6d65 7370 6163        - namespac
-00020f50: 6573 0a20 2020 2020 2020 2020 202d 206e  es.          - n
-00020f60: 616d 6573 7061 6365 730a 2020 2020 2020  amespaces.      
-00020f70: 2020 2d20 6c61 6265 6c5f 7365 6c65 6374    - label_select
-00020f80: 6f72 3a0a 2020 2020 2020 2020 2020 2d20  or:.          - 
-00020f90: 6170 703a 6465 6d6f 2d61 7070 0a20 2020  app:demo-app.   
-00020fa0: 2020 2020 2020 202d 2022 6b65 793a 7665         - "key:ve
-00020fb0: 7273 696f 6e2c 206f 7065 7261 746f 723a  rsion, operator:
-00020fc0: 496e 2c20 7661 6c75 6573 3a5b 7631 2e30  In, values:[v1.0
-00020fd0: 2e30 2c20 7631 2e30 2e31 5d22 0a20 2020  .0, v1.0.1]".   
-00020fe0: 2020 2020 2020 2074 6f70 6f6c 6f67 795f         topology_
-00020ff0: 6b65 793a 2074 6f70 6f6c 6f67 795f 6b65  key: topology_ke
-00021000: 790a 2020 2020 2020 2020 2020 6e61 6d65  y.          name
-00021010: 7370 6163 6573 3a0a 2020 2020 2020 2020  spaces:.        
-00021020: 2020 2d20 6e61 6d65 7370 6163 6573 0a20    - namespaces. 
-00021030: 2020 2020 2020 2020 202d 206e 616d 6573           - names
-00021040: 7061 6365 730a 2020 2020 2020 7072 6f70  paces.      prop
-00021050: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
-00021060: 7265 7175 6972 6564 5f64 7572 696e 675f  required_during_
-00021070: 7363 6865 6475 6c69 6e67 5f69 676e 6f72  scheduling_ignor
-00021080: 6564 5f64 7572 696e 675f 6578 6563 7574  ed_during_execut
-00021090: 696f 6e3a 0a20 2020 2020 2020 2020 2069  ion:.          i
-000210a0: 7465 6d73 3a0a 2020 2020 2020 2020 2020  tems:.          
-000210b0: 2020 2472 6566 3a20 2723 2f63 6f6d 706f    $ref: '#/compo
-000210c0: 6e65 6e74 732f 7363 6865 6d61 732f 506f  nents/schemas/Po
-000210d0: 6441 6666 696e 6974 7954 6572 6d27 0a20  dAffinityTerm'. 
-000210e0: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-000210f0: 7265 7175 6972 6564 5f64 7572 696e 675f  required_during_
-00021100: 7363 6865 6475 6c69 6e67 5f69 676e 6f72  scheduling_ignor
-00021110: 6564 5f64 7572 696e 675f 6578 6563 7574  ed_during_execut
-00021120: 696f 6e0a 2020 2020 2020 2020 2020 7479  ion.          ty
-00021130: 7065 3a20 6172 7261 790a 2020 2020 2020  pe: array.      
-00021140: 2020 7072 6566 6572 7265 645f 6475 7269    preferred_duri
-00021150: 6e67 5f73 6368 6564 756c 696e 675f 6967  ng_scheduling_ig
-00021160: 6e6f 7265 645f 6475 7269 6e67 5f65 7865  nored_during_exe
-00021170: 6375 7469 6f6e 3a0a 2020 2020 2020 2020  cution:.        
-00021180: 2020 6974 656d 733a 0a20 2020 2020 2020    items:.       
-00021190: 2020 2020 2024 7265 663a 2027 232f 636f       $ref: '#/co
-000211a0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-000211b0: 2f57 6569 6768 7465 6450 6f64 4166 6669  /WeightedPodAffi
-000211c0: 6e69 7479 5465 726d 270a 2020 2020 2020  nityTerm'.      
-000211d0: 2020 2020 7469 746c 653a 2070 7265 6665      title: prefe
-000211e0: 7272 6564 5f64 7572 696e 675f 7363 6865  rred_during_sche
-000211f0: 6475 6c69 6e67 5f69 676e 6f72 6564 5f64  duling_ignored_d
-00021200: 7572 696e 675f 6578 6563 7574 696f 6e0a  uring_execution.
-00021210: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-00021220: 6172 7261 790a 2020 2020 2020 7469 746c  array.      titl
-00021230: 653a 2050 6f64 416e 7469 4166 6669 6e69  e: PodAntiAffini
-00021240: 7479 0a20 2020 2020 2074 7970 653a 206f  ty.      type: o
-00021250: 626a 6563 740a 2020 2020 5065 7273 6973  bject.    Persis
-00021260: 7465 6e74 566f 6c75 6d65 436c 6169 6d3a  tentVolumeClaim:
-00021270: 0a20 2020 2020 2065 7861 6d70 6c65 3a0a  .      example:.
-00021280: 2020 2020 2020 2020 766f 6c75 6d65 5f6d          volume_m
-00021290: 6f64 653a 2046 696c 6573 7973 7465 6d0a  ode: Filesystem.
-000212a0: 2020 2020 2020 2020 7265 7175 6573 745f          request_
-000212b0: 7265 736f 7572 6365 733a 0a20 2020 2020  resources:.     
-000212c0: 2020 2020 2072 6571 7565 7374 733a 0a20       requests:. 
-000212d0: 2020 2020 2020 2020 2020 206d 656d 6f72             memor
-000212e0: 793a 2032 3536 4d69 0a20 2020 2020 2020  y: 256Mi.       
-000212f0: 2020 2020 2063 7075 3a20 2230 2e31 220a       cpu: "0.1".
-00021300: 2020 2020 2020 2020 2020 6c69 6d69 7473            limits
-00021310: 3a0a 2020 2020 2020 2020 2020 2020 6d65  :.            me
-00021320: 6d6f 7279 3a20 3531 324d 690a 2020 2020  mory: 512Mi.    
-00021330: 2020 2020 2020 2020 6370 753a 2022 302e          cpu: "0.
-00021340: 3522 0a20 2020 2020 2020 206e 616d 653a  5".        name:
-00021350: 206d 792d 7076 630a 2020 2020 2020 2020   my-pvc.        
-00021360: 6e61 6d65 7370 6163 653a 2067 6974 6f70  namespace: gitop
-00021370: 732d 6364 6e2d 6361 6368 650a 2020 2020  s-cdn-cache.    
-00021380: 2020 2020 616e 6e6f 7461 7469 6f6e 733a      annotations:
-00021390: 0a20 2020 2020 2020 202d 2061 6e6e 6f74  .        - annot
-000213a0: 6174 696f 6e2d 6b65 7931 3a76 616c 310a  ation-key1:val1.
-000213b0: 2020 2020 2020 2020 2d20 616e 6e6f 7461          - annota
-000213c0: 7469 6f6e 2d6b 6579 323a 7661 6c32 0a20  tion-key2:val2. 
-000213d0: 2020 2020 2020 2076 6f6c 756d 655f 6e61         volume_na
-000213e0: 6d65 3a20 6d79 2d70 760a 2020 2020 2020  me: my-pv.      
-000213f0: 2020 7374 6f72 6167 655f 636c 6173 735f    storage_class_
-00021400: 6e61 6d65 3a20 7374 616e 6461 7264 0a20  name: standard. 
-00021410: 2020 2020 2020 2061 6363 6573 735f 6d6f         access_mo
-00021420: 6465 733a 0a20 2020 2020 2020 202d 2052  des:.        - R
-00021430: 6561 6457 7269 7465 4f6e 6365 0a20 2020  eadWriteOnce.   
-00021440: 2020 2020 206c 6162 656c 733a 0a20 2020       labels:.   
-00021450: 2020 2020 202d 2061 7070 3a64 656d 6f2d       - app:demo-
-00021460: 6170 700a 2020 2020 2020 2020 2d20 7665  app.        - ve
-00021470: 7273 696f 6e3a 7631 2e30 2e30 0a20 2020  rsion:v1.0.0.   
-00021480: 2020 2070 726f 7065 7274 6965 733a 0a20     properties:. 
-00021490: 2020 2020 2020 206e 616d 653a 0a20 2020         name:.   
-000214a0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-000214b0: 6f6e 3a20 226e 616d 6520 6f66 2070 6572  on: "name of per
-000214c0: 7369 7374 656e 7420 766f 6c75 6d65 2063  sistent volume c
-000214d0: 6c61 696d 2c20 7573 6564 2069 6e20 6d65  laim, used in me
-000214e0: 7461 6461 7461 2e6e 616d 6522 0a20 2020  tadata.name".   
-000214f0: 2020 2020 2020 2065 7861 6d70 6c65 3a20         example: 
-00021500: 6d79 2d70 7663 0a20 2020 2020 2020 2020  my-pvc.         
-00021510: 2074 6974 6c65 3a20 6e61 6d65 0a20 2020   title: name.   
-00021520: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00021530: 696e 670a 2020 2020 2020 2020 6e61 6d65  ing.        name
-00021540: 7370 6163 653a 0a20 2020 2020 2020 2020  space:.         
-00021550: 2064 6573 6372 6970 7469 6f6e 3a20 6e61   description: na
-00021560: 6d65 7370 6163 6520 666f 7220 7265 736f  mespace for reso
-00021570: 7572 6365 2e0a 2020 2020 2020 2020 2020  urce..          
-00021580: 6578 616d 706c 653a 2067 6974 6f70 732d  example: gitops-
-00021590: 6364 6e2d 6361 6368 650a 2020 2020 2020  cdn-cache.      
-000215a0: 2020 2020 7469 746c 653a 206e 616d 6573      title: names
-000215b0: 7061 6365 0a20 2020 2020 2020 2020 2074  pace.          t
-000215c0: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
-000215d0: 2020 2020 6c61 6265 6c73 3a0a 2020 2020      labels:.    
-000215e0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-000215f0: 6e3a 204d 6170 206f 6620 7374 7269 6e67  n: Map of string
-00021600: 206b 6579 7320 616e 6420 7661 6c75 6573   keys and values
-00021610: 2074 6861 7420 6361 6e20 6265 2075 7365   that can be use
-00021620: 6420 746f 206f 7267 616e 697a 650a 2020  d to organize.  
-00021630: 2020 2020 2020 2020 2020 616e 6420 6361            and ca
-00021640: 7465 676f 7269 7a65 2028 7363 6f70 6520  tegorize (scope 
-00021650: 616e 6420 7365 6c65 6374 2920 6f62 6a65  and select) obje
-00021660: 6374 730a 2020 2020 2020 2020 2020 6578  cts.          ex
-00021670: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
-00021680: 202d 2061 7070 3a64 656d 6f2d 6170 700a   - app:demo-app.
-00021690: 2020 2020 2020 2020 2020 2d20 7665 7273            - vers
-000216a0: 696f 6e3a 7631 2e30 2e30 0a20 2020 2020  ion:v1.0.0.     
-000216b0: 2020 2020 2069 7465 6d73 3a0a 2020 2020       items:.    
-000216c0: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
-000216d0: 7269 6e67 0a20 2020 2020 2020 2020 2074  ring.          t
-000216e0: 6974 6c65 3a20 4c61 6265 6c73 0a20 2020  itle: Labels.   
-000216f0: 2020 2020 2020 2074 7970 653a 2061 7272         type: arr
-00021700: 6179 0a20 2020 2020 2020 2061 6e6e 6f74  ay.        annot
-00021710: 6174 696f 6e73 3a0a 2020 2020 2020 2020  ations:.        
-00021720: 2020 6465 7363 7269 7074 696f 6e3a 2041    description: A
-00021730: 6e20 756e 7374 7275 6374 7572 6564 206b  n unstructured k
-00021740: 6579 2076 616c 7565 206d 6170 2074 6861  ey value map tha
-00021750: 7420 6361 6e20 6265 2075 7365 6420 746f  t can be used to
-00021760: 2061 7474 6163 6820 6172 6269 7472 6172   attach arbitrar
-00021770: 790a 2020 2020 2020 2020 2020 2020 6d65  y.            me
-00021780: 7461 6461 7461 0a20 2020 2020 2020 2020  tadata.         
-00021790: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
-000217a0: 2020 2020 2d20 616e 6e6f 7461 7469 6f6e      - annotation
-000217b0: 2d6b 6579 313a 7661 6c31 0a20 2020 2020  -key1:val1.     
-000217c0: 2020 2020 202d 2061 6e6e 6f74 6174 696f       - annotatio
-000217d0: 6e2d 6b65 7932 3a76 616c 320a 2020 2020  n-key2:val2.    
-000217e0: 2020 2020 2020 6974 656d 733a 0a20 2020        items:.   
-000217f0: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-00021800: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-00021810: 7469 746c 653a 2041 6e6e 6f74 6174 696f  title: Annotatio
-00021820: 6e73 0a20 2020 2020 2020 2020 2074 7970  ns.          typ
-00021830: 653a 2061 7272 6179 0a20 2020 2020 2020  e: array.       
-00021840: 2073 746f 7261 6765 5f63 6c61 7373 5f6e   storage_class_n
-00021850: 616d 653a 0a20 2020 2020 2020 2020 2064  ame:.          d
-00021860: 6573 6372 6970 7469 6f6e 3a20 4e61 6d65  escription: Name
-00021870: 206f 6620 7468 6520 5374 6f72 6167 6543   of the StorageC
-00021880: 6c61 7373 2066 6f72 2074 6865 2050 6572  lass for the Per
-00021890: 7369 7374 656e 7420 566f 6c75 6d65 2043  sistent Volume C
-000218a0: 6c61 696d 0a20 2020 2020 2020 2020 2065  laim.          e
-000218b0: 7861 6d70 6c65 3a20 7374 616e 6461 7264  xample: standard
-000218c0: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
-000218d0: 3a20 7374 6f72 6167 655f 636c 6173 735f  : storage_class_
-000218e0: 6e61 6d65 0a20 2020 2020 2020 2020 2074  name.          t
-000218f0: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
-00021900: 2020 2020 6163 6365 7373 5f6d 6f64 6573      access_modes
-00021910: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
-00021920: 7269 7074 696f 6e3a 2022 4c69 7374 206f  ription: "List o
-00021930: 6620 6163 6365 7373 206d 6f64 6573 2066  f access modes f
-00021940: 6f72 2074 6865 2050 6572 7369 7374 656e  or the Persisten
-00021950: 7420 566f 6c75 6d65 2c20 652e 672e 2052  t Volume, e.g. R
-00021960: 6561 6457 7269 7465 4f6e 6365 2c5c 0a20  eadWriteOnce,\. 
-00021970: 2020 2020 2020 2020 2020 205c 2052 6561             \ Rea
-00021980: 644f 6e6c 794d 616e 792c 2065 7463 2e22  dOnlyMany, etc."
-00021990: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-000219a0: 6c65 3a0a 2020 2020 2020 2020 2020 2d20  le:.          - 
-000219b0: 5265 6164 5772 6974 654f 6e63 650a 2020  ReadWriteOnce.  
-000219c0: 2020 2020 2020 2020 6974 656d 733a 0a20          items:. 
-000219d0: 2020 2020 2020 2020 2020 2074 7970 653a             type:
-000219e0: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-000219f0: 2020 7469 746c 653a 2061 6363 6573 735f    title: access_
-00021a00: 6d6f 6465 730a 2020 2020 2020 2020 2020  modes.          
-00021a10: 7479 7065 3a20 6172 7261 790a 2020 2020  type: array.    
-00021a20: 2020 2020 766f 6c75 6d65 5f6e 616d 653a      volume_name:
-00021a30: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
-00021a40: 6970 7469 6f6e 3a20 4e61 6d65 206f 6620  iption: Name of 
-00021a50: 7468 6520 5065 7273 6973 7465 6e74 2056  the Persistent V
-00021a60: 6f6c 756d 6520 626f 756e 6420 746f 2074  olume bound to t
-00021a70: 6865 2063 6c61 696d 0a20 2020 2020 2020  he claim.       
-00021a80: 2020 2065 7861 6d70 6c65 3a20 6d79 2d70     example: my-p
-00021a90: 760a 2020 2020 2020 2020 2020 7469 746c  v.          titl
-00021aa0: 653a 2076 6f6c 756d 655f 6e61 6d65 0a20  e: volume_name. 
-00021ab0: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-00021ac0: 7472 696e 670a 2020 2020 2020 2020 766f  tring.        vo
-00021ad0: 6c75 6d65 5f6d 6f64 653a 0a20 2020 2020  lume_mode:.     
-00021ae0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-00021af0: 3a20 224d 6f64 6520 6f66 2074 6865 2076  : "Mode of the v
-00021b00: 6f6c 756d 652c 2065 6974 6865 7220 5c22  olume, either \"
-00021b10: 4669 6c65 7379 7374 656d 5c22 206f 7220  Filesystem\" or 
-00021b20: 5c22 426c 6f63 6b5c 2222 0a20 2020 2020  \"Block\"".     
-00021b30: 2020 2020 2065 7861 6d70 6c65 3a20 4669       example: Fi
-00021b40: 6c65 7379 7374 656d 0a20 2020 2020 2020  lesystem.       
-00021b50: 2020 2074 6974 6c65 3a20 766f 6c75 6d65     title: volume
-00021b60: 5f6d 6f64 650a 2020 2020 2020 2020 2020  _mode.          
-00021b70: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
-00021b80: 2020 2020 2072 6571 7565 7374 5f72 6573       request_res
-00021b90: 6f75 7263 6573 3a0a 2020 2020 2020 2020  ources:.        
-00021ba0: 2020 2472 6566 3a20 2723 2f63 6f6d 706f    $ref: '#/compo
-00021bb0: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
-00021bc0: 736f 7572 6365 5265 7175 6972 656d 656e  sourceRequiremen
-00021bd0: 7473 270a 2020 2020 2020 7265 7175 6972  ts'.      requir
-00021be0: 6564 3a0a 2020 2020 2020 2d20 6e61 6d65  ed:.      - name
-00021bf0: 0a20 2020 2020 2074 6974 6c65 3a20 5065  .      title: Pe
-00021c00: 7273 6973 7465 6e74 566f 6c75 6d65 436c  rsistentVolumeCl
-00021c10: 6169 6d0a 2020 2020 2020 7479 7065 3a20  aim.      type: 
-00021c20: 6f62 6a65 6374 0a20 2020 2053 6572 7669  object.    Servi
-00021c30: 6365 3a0a 2020 2020 2020 6578 616d 706c  ce:.      exampl
-00021c40: 653a 0a20 2020 2020 2020 2065 7874 6572  e:.        exter
-00021c50: 6e61 6c5f 6970 733a 0a20 2020 2020 2020  nal_ips:.       
-00021c60: 202d 2031 2e31 2e31 2e31 0a20 2020 2020   - 1.1.1.1.     
-00021c70: 2020 202d 2032 2e32 2e32 2e32 0a20 2020     - 2.2.2.2.   
-00021c80: 2020 2020 2073 6572 7669 6365 5f74 7970       service_typ
-00021c90: 653a 2043 6c75 7374 6572 4950 0a20 2020  e: ClusterIP.   
-00021ca0: 2020 2020 206e 616d 653a 2064 656d 6f2d       name: demo-
-00021cb0: 6170 700a 2020 2020 2020 2020 6e61 6d65  app.        name
-00021cc0: 7370 6163 653a 2067 6974 6f70 732d 6364  space: gitops-cd
-00021cd0: 6e2d 6361 6368 650a 2020 2020 2020 2020  n-cache.        
-00021ce0: 616e 6e6f 7461 7469 6f6e 733a 0a20 2020  annotations:.   
-00021cf0: 2020 2020 202d 2061 6e6e 6f74 6174 696f       - annotatio
-00021d00: 6e2d 6b65 7931 3a76 616c 310a 2020 2020  n-key1:val1.    
-00021d10: 2020 2020 2d20 616e 6e6f 7461 7469 6f6e      - annotation
-00021d20: 2d6b 6579 323a 7661 6c32 0a20 2020 2020  -key2:val2.     
-00021d30: 2020 2073 656c 6563 746f 723a 0a20 2020     selector:.   
-00021d40: 2020 2020 202d 2061 7070 3a64 656d 6f2d       - app:demo-
-00021d50: 6170 700a 2020 2020 2020 2020 2d20 226b  app.        - "k
-00021d60: 6579 3a76 6572 7369 6f6e 2c20 6f70 6572  ey:version, oper
-00021d70: 6174 6f72 3a49 6e2c 2076 616c 7565 733a  ator:In, values:
-00021d80: 5b76 312e 302e 302c 2076 312e 302e 315d  [v1.0.0, v1.0.1]
-00021d90: 220a 2020 2020 2020 2020 706f 7274 733a  ".        ports:
-00021da0: 0a20 2020 2020 2020 202d 2074 6172 6765  .        - targe
-00021db0: 745f 706f 7274 3a20 3830 3830 0a20 2020  t_port: 8080.   
-00021dc0: 2020 2020 2020 2070 726f 746f 636f 6c3a         protocol:
-00021dd0: 2054 4350 0a20 2020 2020 2020 2020 2070   TCP.          p
-00021de0: 6f72 743a 2038 300a 2020 2020 2020 2020  ort: 80.        
-00021df0: 2020 6e61 6d65 3a20 6874 7470 0a20 2020    name: http.   
-00021e00: 2020 2020 2020 206e 6f64 655f 706f 7274         node_port
-00021e10: 3a20 3635 3030 0a20 2020 2020 2020 202d  : 6500.        -
-00021e20: 2074 6172 6765 745f 706f 7274 3a20 3830   target_port: 80
-00021e30: 3830 0a20 2020 2020 2020 2020 2070 726f  80.          pro
-00021e40: 746f 636f 6c3a 2054 4350 0a20 2020 2020  tocol: TCP.     
-00021e50: 2020 2020 2070 6f72 743a 2038 300a 2020       port: 80.  
-00021e60: 2020 2020 2020 2020 6e61 6d65 3a20 6874          name: ht
-00021e70: 7470 0a20 2020 2020 2020 2020 206e 6f64  tp.          nod
-00021e80: 655f 706f 7274 3a20 3635 3030 0a20 2020  e_port: 6500.   
-00021e90: 2020 2020 2063 6c75 7374 6572 5f69 703a       cluster_ip:
-00021ea0: 2063 6c75 7374 6572 5f69 700a 2020 2020   cluster_ip.    
-00021eb0: 2020 2020 6c61 6265 6c73 3a0a 2020 2020      labels:.    
-00021ec0: 2020 2020 2d20 6170 703a 6465 6d6f 2d61      - app:demo-a
-00021ed0: 7070 0a20 2020 2020 2020 202d 2076 6572  pp.        - ver
-00021ee0: 7369 6f6e 3a76 312e 302e 300a 2020 2020  sion:v1.0.0.    
-00021ef0: 2020 7072 6f70 6572 7469 6573 3a0a 2020    properties:.  
-00021f00: 2020 2020 2020 6e61 6d65 3a0a 2020 2020        name:.    
-00021f10: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00021f20: 6e3a 2073 6572 7669 6365 206e 616d 650a  n: service name.
-00021f30: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
-00021f40: 653a 2064 656d 6f2d 6170 700a 2020 2020  e: demo-app.    
-00021f50: 2020 2020 2020 7469 746c 653a 206e 616d        title: nam
-00021f60: 650a 2020 2020 2020 2020 2020 7479 7065  e.          type
-00021f70: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
-00021f80: 206e 616d 6573 7061 6365 3a0a 2020 2020   namespace:.    
-00021f90: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00021fa0: 6e3a 206e 616d 6573 7061 6365 2066 6f72  n: namespace for
-00021fb0: 2072 6573 6f75 7263 652e 0a20 2020 2020   resource..     
-00021fc0: 2020 2020 2065 7861 6d70 6c65 3a20 6769       example: gi
-00021fd0: 746f 7073 2d63 646e 2d63 6163 6865 0a20  tops-cdn-cache. 
-00021fe0: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-00021ff0: 6e61 6d65 7370 6163 650a 2020 2020 2020  namespace.      
-00022000: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-00022010: 0a20 2020 2020 2020 2061 6e6e 6f74 6174  .        annotat
-00022020: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-00022030: 6465 7363 7269 7074 696f 6e3a 2041 6e20  description: An 
-00022040: 756e 7374 7275 6374 7572 6564 206b 6579  unstructured key
-00022050: 2076 616c 7565 206d 6170 2074 6861 7420   value map that 
-00022060: 6361 6e20 6265 2075 7365 6420 746f 2061  can be used to a
-00022070: 7474 6163 6820 6172 6269 7472 6172 790a  ttach arbitrary.
-00022080: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00022090: 6461 7461 0a20 2020 2020 2020 2020 2065  data.          e
-000220a0: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
-000220b0: 2020 2d20 616e 6e6f 7461 7469 6f6e 2d6b    - annotation-k
-000220c0: 6579 313a 7661 6c31 0a20 2020 2020 2020  ey1:val1.       
-000220d0: 2020 202d 2061 6e6e 6f74 6174 696f 6e2d     - annotation-
-000220e0: 6b65 7932 3a76 616c 320a 2020 2020 2020  key2:val2.      
-000220f0: 2020 2020 6974 656d 733a 0a20 2020 2020      items:.     
-00022100: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00022110: 696e 670a 2020 2020 2020 2020 2020 7469  ing.          ti
-00022120: 746c 653a 2041 6e6e 6f74 6174 696f 6e73  tle: Annotations
-00022130: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
-00022140: 2061 7272 6179 0a20 2020 2020 2020 206c   array.        l
-00022150: 6162 656c 733a 0a20 2020 2020 2020 2020  abels:.         
-00022160: 2064 6573 6372 6970 7469 6f6e 3a20 4d61   description: Ma
-00022170: 7020 6f66 2073 7472 696e 6720 6b65 7973  p of string keys
-00022180: 2061 6e64 2076 616c 7565 7320 7468 6174   and values that
-00022190: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-000221a0: 6f72 6761 6e69 7a65 0a20 2020 2020 2020  organize.       
-000221b0: 2020 2020 2061 6e64 2063 6174 6567 6f72       and categor
-000221c0: 697a 6520 2873 636f 7065 2061 6e64 2073  ize (scope and s
-000221d0: 656c 6563 7429 206f 626a 6563 7473 0a20  elect) objects. 
-000221e0: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
-000221f0: 3a0a 2020 2020 2020 2020 2020 2d20 6170  :.          - ap
-00022200: 703a 6465 6d6f 2d61 7070 0a20 2020 2020  p:demo-app.     
-00022210: 2020 2020 202d 2076 6572 7369 6f6e 3a76       - version:v
-00022220: 312e 302e 300a 2020 2020 2020 2020 2020  1.0.0.          
-00022230: 6974 656d 733a 0a20 2020 2020 2020 2020  items:.         
-00022240: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
-00022250: 2020 2020 2020 2020 2020 7469 746c 653a            title:
-00022260: 204c 6162 656c 730a 2020 2020 2020 2020   Labels.        
-00022270: 2020 7479 7065 3a20 6172 7261 790a 2020    type: array.  
-00022280: 2020 2020 2020 7365 6c65 6374 6f72 3a0a        selector:.
-00022290: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-000222a0: 7074 696f 6e3a 207c 0a20 2020 2020 2020  ption: |.       
-000222b0: 2020 2020 2041 6e20 6172 7261 7920 6f66       An array of
-000222c0: 206c 6162 656c 2073 656c 6563 746f 7220   label selector 
-000222d0: 7275 6c65 2c20 7468 6520 7275 6c65 2063  rule, the rule c
-000222e0: 616e 2065 6974 6865 7220 6265 2061 206d  an either be a m
-000222f0: 6174 6368 206c 6162 656c 206f 7220 6d61  atch label or ma
-00022300: 7463 6820 6578 7072 6573 7369 6f6e 2c0a  tch expression,.
-00022310: 2020 2020 2020 2020 2020 2020 7265 6665              refe
-00022320: 7272 696e 6720 7468 6520 6578 616d 706c  rring the exampl
-00022330: 6520 2866 6972 7374 2069 7320 6120 6d61  e (first is a ma
-00022340: 7463 6820 6c61 6265 6c2c 2073 6563 6f6e  tch label, secon
-00022350: 6420 6973 2061 206d 6174 6368 2065 7870  d is a match exp
-00022360: 7265 7373 696f 6e29 0a20 2020 2020 2020  ression).       
-00022370: 2020 2065 7861 6d70 6c65 3a0a 2020 2020     example:.    
-00022380: 2020 2020 2020 2d20 6170 703a 6465 6d6f        - app:demo
-00022390: 2d61 7070 0a20 2020 2020 2020 2020 202d  -app.          -
-000223a0: 2022 6b65 793a 7665 7273 696f 6e2c 206f   "key:version, o
-000223b0: 7065 7261 746f 723a 496e 2c20 7661 6c75  perator:In, valu
-000223c0: 6573 3a5b 7631 2e30 2e30 2c20 7631 2e30  es:[v1.0.0, v1.0
-000223d0: 2e31 5d22 0a20 2020 2020 2020 2020 2069  .1]".          i
-000223e0: 7465 6d73 3a0a 2020 2020 2020 2020 2020  tems:.          
-000223f0: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00022400: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-00022410: 4c61 6265 6c53 656c 6563 746f 720a 2020  LabelSelector.  
-00022420: 2020 2020 2020 2020 7479 7065 3a20 6172          type: ar
-00022430: 7261 790a 2020 2020 2020 2020 7365 7276  ray.        serv
-00022440: 6963 655f 7479 7065 3a0a 2020 2020 2020  ice_type:.      
-00022450: 2020 2020 656e 756d 3a0a 2020 2020 2020      enum:.      
-00022460: 2020 2020 2d20 436c 7573 7465 7249 500a      - ClusterIP.
-00022470: 2020 2020 2020 2020 2020 2d20 4e6f 6465            - Node
-00022480: 506f 7274 0a20 2020 2020 2020 2020 202d  Port.          -
-00022490: 204c 6f61 6442 616c 616e 6365 720a 2020   LoadBalancer.  
-000224a0: 2020 2020 2020 2020 6578 616d 706c 653a          example:
-000224b0: 2043 6c75 7374 6572 4950 0a20 2020 2020   ClusterIP.     
-000224c0: 2020 2020 2074 6974 6c65 3a20 7365 7276       title: serv
-000224d0: 6963 655f 7479 7065 0a20 2020 2020 2020  ice_type.       
-000224e0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
-000224f0: 2020 2020 2020 2020 706f 7274 733a 0a20          ports:. 
-00022500: 2020 2020 2020 2020 2069 7465 6d73 3a0a           items:.
-00022510: 2020 2020 2020 2020 2020 2020 2472 6566              $ref
-00022520: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
-00022530: 7363 6865 6d61 732f 5365 7276 6963 6550  schemas/ServiceP
-00022540: 6f72 7427 0a20 2020 2020 2020 2020 2074  ort'.          t
-00022550: 6974 6c65 3a20 706f 7274 730a 2020 2020  itle: ports.    
-00022560: 2020 2020 2020 7479 7065 3a20 6172 7261        type: arra
-00022570: 790a 2020 2020 2020 2020 636c 7573 7465  y.        cluste
-00022580: 725f 6970 3a0a 2020 2020 2020 2020 2020  r_ip:.          
-00022590: 6465 7363 7269 7074 696f 6e3a 2045 7870  description: Exp
-000225a0: 6f73 6573 2074 6865 2053 6572 7669 6365  oses the Service
-000225b0: 206f 6e20 6120 636c 7573 7465 722d 696e   on a cluster-in
-000225c0: 7465 726e 616c 2049 502e 0a20 2020 2020  ternal IP..     
-000225d0: 2020 2020 2074 6974 6c65 3a20 636c 7573       title: clus
-000225e0: 7465 725f 6970 0a20 2020 2020 2020 2020  ter_ip.         
-000225f0: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
-00022600: 2020 2020 2020 6578 7465 726e 616c 5f69        external_i
-00022610: 7073 3a0a 2020 2020 2020 2020 2020 6465  ps:.          de
-00022620: 7363 7269 7074 696f 6e3a 2041 206c 6973  scription: A lis
-00022630: 7420 6f66 2049 5020 6164 6472 6573 7365  t of IP addresse
-00022640: 7320 666f 7220 7768 6963 6820 6e6f 6465  s for which node
-00022650: 7320 696e 2074 6865 2063 6c75 7374 6572  s in the cluster
-00022660: 2077 696c 6c0a 2020 2020 2020 2020 2020   will.          
-00022670: 2020 616c 736f 2061 6363 6570 7420 7472    also accept tr
-00022680: 6166 6669 6320 666f 7220 7468 6973 2073  affic for this s
-00022690: 6572 7669 6365 0a20 2020 2020 2020 2020  ervice.         
-000226a0: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
-000226b0: 2020 2020 2d20 312e 312e 312e 310a 2020      - 1.1.1.1.  
-000226c0: 2020 2020 2020 2020 2d20 322e 322e 322e          - 2.2.2.
-000226d0: 320a 2020 2020 2020 2020 2020 6974 656d  2.          item
-000226e0: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-000226f0: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
-00022700: 2020 2020 2020 7469 746c 653a 2065 7874        title: ext
-00022710: 6572 6e61 6c5f 6970 730a 2020 2020 2020  ernal_ips.      
-00022720: 2020 2020 7479 7065 3a20 6172 7261 790a      type: array.
-00022730: 2020 2020 2020 7265 7175 6972 6564 3a0a        required:.
-00022740: 2020 2020 2020 2d20 6e61 6d65 0a20 2020        - name.   
-00022750: 2020 2074 6974 6c65 3a20 5365 7276 6963     title: Servic
-00022760: 650a 2020 2020 2020 7479 7065 3a20 6f62  e.      type: ob
-00022770: 6a65 6374 0a20 2020 2053 6572 7669 6365  ject.    Service
-00022780: 506f 7274 3a0a 2020 2020 2020 6578 616d  Port:.      exam
-00022790: 706c 653a 0a20 2020 2020 2020 2074 6172  ple:.        tar
-000227a0: 6765 745f 706f 7274 3a20 3830 3830 0a20  get_port: 8080. 
-000227b0: 2020 2020 2020 2070 726f 746f 636f 6c3a         protocol:
-000227c0: 2054 4350 0a20 2020 2020 2020 2070 6f72   TCP.        por
-000227d0: 743a 2038 300a 2020 2020 2020 2020 6e61  t: 80.        na
-000227e0: 6d65 3a20 6874 7470 0a20 2020 2020 2020  me: http.       
-000227f0: 206e 6f64 655f 706f 7274 3a20 3635 3030   node_port: 6500
-00022800: 0a20 2020 2020 2070 726f 7065 7274 6965  .      propertie
-00022810: 733a 0a20 2020 2020 2020 206e 616d 653a  s:.        name:
-00022820: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
-00022830: 6970 7469 6f6e 3a20 7c0a 2020 2020 2020  iption: |.      
-00022840: 2020 2020 2020 5468 6520 6e61 6d65 206f        The name o
-00022850: 6620 7468 6973 2070 6f72 7420 7769 7468  f this port with
-00022860: 696e 2074 6865 2073 6572 7669 6365 2e20  in the service. 
-00022870: 5468 6973 206d 7573 7420 6265 2061 2044  This must be a D
-00022880: 4e53 5f4c 4142 454c 2e0a 2020 2020 2020  NS_LABEL..      
-00022890: 2020 2020 2020 416c 6c20 706f 7274 7320        All ports 
-000228a0: 7769 7468 696e 2061 2053 6572 7669 6365  within a Service
-000228b0: 5370 6563 206d 7573 7420 6861 7665 2075  Spec must have u
-000228c0: 6e69 7175 6520 6e61 6d65 730a 2020 2020  nique names.    
-000228d0: 2020 2020 2020 6578 616d 706c 653a 2068        example: h
-000228e0: 7474 700a 2020 2020 2020 2020 2020 7469  ttp.          ti
-000228f0: 746c 653a 206e 616d 650a 2020 2020 2020  tle: name.      
-00022900: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-00022910: 0a20 2020 2020 2020 2070 6f72 743a 0a20  .        port:. 
-00022920: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00022930: 7469 6f6e 3a20 5468 6520 706f 7274 2074  tion: The port t
-00022940: 6861 7420 7769 6c6c 2062 6520 6578 706f  hat will be expo
-00022950: 7365 6420 6279 2074 6869 7320 7365 7276  sed by this serv
-00022960: 6963 650a 2020 2020 2020 2020 2020 6578  ice.          ex
-00022970: 616d 706c 653a 2038 300a 2020 2020 2020  ample: 80.      
-00022980: 2020 2020 7469 746c 653a 2070 6f72 740a      title: port.
-00022990: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-000229a0: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
-000229b0: 7461 7267 6574 5f70 6f72 743a 0a20 2020  target_port:.   
-000229c0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-000229d0: 6f6e 3a20 5468 6520 706f 7274 2074 6f20  on: The port to 
-000229e0: 6163 6365 7373 206f 6e20 7468 6520 706f  access on the po
-000229f0: 6473 2074 6172 6765 7465 6420 6279 2074  ds targeted by t
-00022a00: 6865 2073 6572 7669 6365 0a20 2020 2020  he service.     
-00022a10: 2020 2020 2065 7861 6d70 6c65 3a20 3830       example: 80
-00022a20: 3830 0a20 2020 2020 2020 2020 2074 6974  80.          tit
-00022a30: 6c65 3a20 7461 7267 6574 5f70 6f72 740a  le: target_port.
-00022a40: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-00022a50: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
-00022a60: 6e6f 6465 5f70 6f72 743a 0a20 2020 2020  node_port:.     
-00022a70: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-00022a80: 3a20 5468 6520 706f 7274 206f 6e20 6561  : The port on ea
-00022a90: 6368 206e 6f64 6520 6f6e 2077 6869 6368  ch node on which
-00022aa0: 2074 6869 7320 7365 7276 6963 6520 6973   this service is
-00022ab0: 2065 7870 6f73 6564 2077 6865 6e0a 2020   exposed when.  
-00022ac0: 2020 2020 2020 2020 2020 7479 7065 2069            type i
-00022ad0: 7320 4e6f 6465 506f 7274 206f 7220 4c6f  s NodePort or Lo
-00022ae0: 6164 4261 6c61 6e63 6572 0a20 2020 2020  adBalancer.     
-00022af0: 2020 2020 2065 7861 6d70 6c65 3a20 3635       example: 65
-00022b00: 3030 0a20 2020 2020 2020 2020 2074 6974  00.          tit
-00022b10: 6c65 3a20 6e6f 6465 5f70 6f72 740a 2020  le: node_port.  
-00022b20: 2020 2020 2020 2020 7479 7065 3a20 696e          type: in
-00022b30: 7465 6765 720a 2020 2020 2020 2020 7072  teger.        pr
-00022b40: 6f74 6f63 6f6c 3a0a 2020 2020 2020 2020  otocol:.        
-00022b50: 2020 6465 7363 7269 7074 696f 6e3a 2044    description: D
-00022b60: 6566 6175 6c74 7320 746f 2054 4350 0a20  efaults to TCP. 
-00022b70: 2020 2020 2020 2020 2065 6e75 6d3a 0a20           enum:. 
-00022b80: 2020 2020 2020 2020 202d 2054 4350 0a20           - TCP. 
-00022b90: 2020 2020 2020 2020 202d 2055 4450 0a20           - UDP. 
-00022ba0: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
-00022bb0: 3a20 5443 500a 2020 2020 2020 2020 2020  : TCP.          
-00022bc0: 7469 746c 653a 2070 726f 746f 636f 6c0a  title: protocol.
-00022bd0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-00022be0: 7374 7269 6e67 0a20 2020 2020 2072 6571  string.      req
-00022bf0: 7569 7265 643a 0a20 2020 2020 202d 206e  uired:.      - n
-00022c00: 616d 650a 2020 2020 2020 7469 746c 653a  ame.      title:
-00022c10: 2053 6572 7669 6365 506f 7274 0a20 2020   ServicePort.   
-00022c20: 2020 2074 7970 653a 206f 626a 6563 740a     type: object.
-00022c30: 2020 2020 436f 6e66 6967 3a0a 2020 2020      Config:.    
-00022c40: 2020 6578 616d 706c 653a 0a20 2020 2020    example:.     
-00022c50: 2020 2074 656d 706c 6174 6573 3a0a 2020     templates:.  
-00022c60: 2020 2020 2020 2d20 7661 6c75 6573 3a0a        - values:.
-00022c70: 2020 2020 2020 2020 2020 2020 6b65 7931              key1
-00022c80: 3a20 7661 6c75 6531 0a20 2020 2020 2020  : value1.       
-00022c90: 2020 206e 616d 653a 2063 6f6e 662f 7365     name: conf/se
-00022ca0: 7276 6572 2e63 6f6e 660a 2020 2020 2020  rver.conf.      
-00022cb0: 2020 2d20 7661 6c75 6573 3a0a 2020 2020    - values:.    
-00022cc0: 2020 2020 2020 2020 6b65 7931 3a20 7661          key1: va
-00022cd0: 6c75 6531 0a20 2020 2020 2020 2020 206e  lue1.          n
-00022ce0: 616d 653a 2063 6f6e 662f 7365 7276 6572  ame: conf/server
-00022cf0: 2e63 6f6e 660a 2020 2020 2020 2020 6e61  .conf.        na
-00022d00: 6d65 3a20 7365 7276 6572 2d63 6f6e 660a  me: server-conf.
-00022d10: 2020 2020 2020 2020 616e 6e6f 7461 7469          annotati
-00022d20: 6f6e 733a 0a20 2020 2020 2020 202d 2061  ons:.        - a
-00022d30: 6e6e 6f74 6174 696f 6e2d 6b65 7931 3a76  nnotation-key1:v
-00022d40: 616c 310a 2020 2020 2020 2020 2d20 616e  al1.        - an
-00022d50: 6e6f 7461 7469 6f6e 2d6b 6579 323a 7661  notation-key2:va
-00022d60: 6c32 0a20 2020 2020 2020 2066 696c 6573  l2.        files
-00022d70: 3a0a 2020 2020 2020 2020 2d20 636f 6e66  :.        - conf
-00022d80: 2f73 6572 7665 722e 636f 6e66 0a20 2020  /server.conf.   
-00022d90: 2020 2020 206c 6162 656c 733a 0a20 2020       labels:.   
-00022da0: 2020 2020 202d 2061 7070 3a64 656d 6f2d       - app:demo-
-00022db0: 6170 700a 2020 2020 2020 2020 2d20 7665  app.        - ve
-00022dc0: 7273 696f 6e3a 7631 2e30 2e30 0a20 2020  rsion:v1.0.0.   
-00022dd0: 2020 2070 726f 7065 7274 6965 733a 0a20     properties:. 
-00022de0: 2020 2020 2020 206e 616d 653a 0a20 2020         name:.   
-00022df0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00022e00: 6f6e 3a20 5468 6520 636f 6e66 6967 206d  on: The config m
-00022e10: 6170 206e 616d 650a 2020 2020 2020 2020  ap name.        
-00022e20: 2020 6578 616d 706c 653a 2073 6572 7665    example: serve
-00022e30: 722d 636f 6e66 0a20 2020 2020 2020 2020  r-conf.         
-00022e40: 2074 6974 6c65 3a20 6e61 6d65 0a20 2020   title: name.   
-00022e50: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00022e60: 696e 670a 2020 2020 2020 2020 6c61 6265  ing.        labe
-00022e70: 6c73 3a0a 2020 2020 2020 2020 2020 6465  ls:.          de
-00022e80: 7363 7269 7074 696f 6e3a 204d 6170 206f  scription: Map o
-00022e90: 6620 7374 7269 6e67 206b 6579 7320 616e  f string keys an
-00022ea0: 6420 7661 6c75 6573 2074 6861 7420 6361  d values that ca
-00022eb0: 6e20 6265 2075 7365 6420 746f 206f 7267  n be used to org
-00022ec0: 616e 697a 650a 2020 2020 2020 2020 2020  anize.          
-00022ed0: 2020 616e 6420 6361 7465 676f 7269 7a65    and categorize
-00022ee0: 2028 7363 6f70 6520 616e 6420 7365 6c65   (scope and sele
-00022ef0: 6374 2920 6f62 6a65 6374 730a 2020 2020  ct) objects.    
-00022f00: 2020 2020 2020 6578 616d 706c 653a 0a20        example:. 
-00022f10: 2020 2020 2020 2020 202d 2061 7070 3a64           - app:d
-00022f20: 656d 6f2d 6170 700a 2020 2020 2020 2020  emo-app.        
-00022f30: 2020 2d20 7665 7273 696f 6e3a 7631 2e30    - version:v1.0
-00022f40: 2e30 0a20 2020 2020 2020 2020 2069 7465  .0.          ite
-00022f50: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00022f60: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
-00022f70: 2020 2020 2020 2074 6974 6c65 3a20 4c61         title: La
-00022f80: 6265 6c73 0a20 2020 2020 2020 2020 2074  bels.          t
-00022f90: 7970 653a 2061 7272 6179 0a20 2020 2020  ype: array.     
-00022fa0: 2020 2061 6e6e 6f74 6174 696f 6e73 3a0a     annotations:.
-00022fb0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00022fc0: 7074 696f 6e3a 2041 6e20 756e 7374 7275  ption: An unstru
-00022fd0: 6374 7572 6564 206b 6579 2076 616c 7565  ctured key value
-00022fe0: 206d 6170 2074 6861 7420 6361 6e20 6265   map that can be
-00022ff0: 2075 7365 6420 746f 2061 7474 6163 6820   used to attach 
-00023000: 6172 6269 7472 6172 790a 2020 2020 2020  arbitrary.      
-00023010: 2020 2020 2020 6d65 7461 6461 7461 0a20        metadata. 
-00023020: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
-00023030: 3a0a 2020 2020 2020 2020 2020 2d20 616e  :.          - an
-00023040: 6e6f 7461 7469 6f6e 2d6b 6579 313a 7661  notation-key1:va
-00023050: 6c31 0a20 2020 2020 2020 2020 202d 2061  l1.          - a
-00023060: 6e6e 6f74 6174 696f 6e2d 6b65 7932 3a76  nnotation-key2:v
-00023070: 616c 320a 2020 2020 2020 2020 2020 6974  al2.          it
-00023080: 656d 733a 0a20 2020 2020 2020 2020 2020  ems:.           
-00023090: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
-000230a0: 2020 2020 2020 2020 7469 746c 653a 2041          title: A
-000230b0: 6e6e 6f74 6174 696f 6e73 0a20 2020 2020  nnotations.     
-000230c0: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
-000230d0: 0a20 2020 2020 2020 2066 696c 6573 3a0a  .        files:.
-000230e0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-000230f0: 7074 696f 6e3a 2074 6865 206c 6973 7420  ption: the list 
-00023100: 6f66 2063 6f6e 6669 6720 6669 6c65 2070  of config file p
-00023110: 6174 6873 0a20 2020 2020 2020 2020 2065  aths.          e
-00023120: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
-00023130: 2020 2d20 636f 6e66 2f73 6572 7665 722e    - conf/server.
-00023140: 636f 6e66 0a20 2020 2020 2020 2020 2069  conf.          i
-00023150: 7465 6d73 3a0a 2020 2020 2020 2020 2020  tems:.          
-00023160: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00023170: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-00023180: 6669 6c65 730a 2020 2020 2020 2020 2020  files.          
-00023190: 7479 7065 3a20 6172 7261 790a 2020 2020  type: array.    
-000231a0: 2020 2020 7465 6d70 6c61 7465 733a 0a20      templates:. 
-000231b0: 2020 2020 2020 2020 2069 7465 6d73 3a0a           items:.
-000231c0: 2020 2020 2020 2020 2020 2020 2472 6566              $ref
-000231d0: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
-000231e0: 7363 6865 6d61 732f 436f 6e66 6967 5f74  schemas/Config_t
-000231f0: 656d 706c 6174 6573 5f69 6e6e 6572 270a  emplates_inner'.
-00023200: 2020 2020 2020 2020 2020 7469 746c 653a            title:
-00023210: 2074 656d 706c 6174 6573 0a20 2020 2020   templates.     
-00023220: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
-00023230: 0a20 2020 2020 2074 6974 6c65 3a20 436f  .      title: Co
-00023240: 6e66 6967 0a20 2020 2020 2074 7970 653a  nfig.      type:
-00023250: 206f 626a 6563 740a 2020 2020 496e 6772   object.    Ingr
-00023260: 6573 733a 0a20 2020 2020 2065 7861 6d70  ess:.      examp
-00023270: 6c65 3a0a 2020 2020 2020 2020 6e61 6d65  le:.        name
-00023280: 3a20 6465 6d6f 2d61 7070 2d69 6e67 7265  : demo-app-ingre
-00023290: 7373 0a20 2020 2020 2020 206e 616d 6573  ss.        names
-000232a0: 7061 6365 3a20 6769 746f 7073 2d63 646e  pace: gitops-cdn
-000232b0: 2d63 6163 6865 0a20 2020 2020 2020 2061  -cache.        a
-000232c0: 6e6e 6f74 6174 696f 6e73 3a0a 2020 2020  nnotations:.    
-000232d0: 2020 2020 2d20 616e 6e6f 7461 7469 6f6e      - annotation
-000232e0: 2d6b 6579 313a 7661 6c31 0a20 2020 2020  -key1:val1.     
-000232f0: 2020 202d 2061 6e6e 6f74 6174 696f 6e2d     - annotation-
-00023300: 6b65 7932 3a76 616c 320a 2020 2020 2020  key2:val2.      
-00023310: 2020 7275 6c65 733a 0a20 2020 2020 2020    rules:.       
-00023320: 202d 2070 6174 6873 3a0a 2020 2020 2020   - paths:.      
-00023330: 2020 2020 2d20 7061 7468 3a20 2f62 6172      - path: /bar
-00023340: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-00023350: 653a 2069 6e67 7265 7373 2d70 6174 682d  e: ingress-path-
-00023360: 6261 720a 2020 2020 2020 2020 2020 2020  bar.            
-00023370: 7061 7468 5f74 7970 653a 2045 7861 6374  path_type: Exact
-00023380: 0a20 2020 2020 2020 2020 2020 2062 6163  .            bac
-00023390: 6b65 6e64 3a0a 2020 2020 2020 2020 2020  kend:.          
-000233a0: 2020 2020 7365 7276 6963 653a 0a20 2020      service:.   
-000233b0: 2020 2020 2020 2020 2020 2020 2070 6f72               por
-000233c0: 743a 2038 300a 2020 2020 2020 2020 2020  t: 80.          
-000233d0: 2020 2020 2020 6e61 6d65 3a20 6465 6d6f        name: demo
-000233e0: 2d61 7070 2d73 6572 7669 6365 0a20 2020  -app-service.   
-000233f0: 2020 2020 2020 202d 2070 6174 683a 202f         - path: /
-00023400: 6261 720a 2020 2020 2020 2020 2020 2020  bar.            
-00023410: 6e61 6d65 3a20 696e 6772 6573 732d 7061  name: ingress-pa
-00023420: 7468 2d62 6172 0a20 2020 2020 2020 2020  th-bar.         
-00023430: 2020 2070 6174 685f 7479 7065 3a20 4578     path_type: Ex
-00023440: 6163 740a 2020 2020 2020 2020 2020 2020  act.            
-00023450: 6261 636b 656e 643a 0a20 2020 2020 2020  backend:.       
-00023460: 2020 2020 2020 2073 6572 7669 6365 3a0a         service:.
-00023470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023480: 706f 7274 3a20 3830 0a20 2020 2020 2020  port: 80.       
-00023490: 2020 2020 2020 2020 206e 616d 653a 2064           name: d
-000234a0: 656d 6f2d 6170 702d 7365 7276 6963 650a  emo-app-service.
-000234b0: 2020 2020 2020 2020 2020 6e61 6d65 3a20            name: 
-000234c0: 666f 6f2d 696e 6772 6573 732d 7275 6c65  foo-ingress-rule
-000234d0: 0a20 2020 2020 2020 2020 2068 6f73 743a  .          host:
-000234e0: 2077 7777 2e66 6f6f 2e63 6f6d 0a20 2020   www.foo.com.   
-000234f0: 2020 2020 202d 2070 6174 6873 3a0a 2020       - paths:.  
-00023500: 2020 2020 2020 2020 2d20 7061 7468 3a20          - path: 
-00023510: 2f62 6172 0a20 2020 2020 2020 2020 2020  /bar.           
-00023520: 206e 616d 653a 2069 6e67 7265 7373 2d70   name: ingress-p
-00023530: 6174 682d 6261 720a 2020 2020 2020 2020  ath-bar.        
-00023540: 2020 2020 7061 7468 5f74 7970 653a 2045      path_type: E
-00023550: 7861 6374 0a20 2020 2020 2020 2020 2020  xact.           
-00023560: 2062 6163 6b65 6e64 3a0a 2020 2020 2020   backend:.      
-00023570: 2020 2020 2020 2020 7365 7276 6963 653a          service:
-00023580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023590: 2070 6f72 743a 2038 300a 2020 2020 2020   port: 80.      
-000235a0: 2020 2020 2020 2020 2020 6e61 6d65 3a20            name: 
-000235b0: 6465 6d6f 2d61 7070 2d73 6572 7669 6365  demo-app-service
-000235c0: 0a20 2020 2020 2020 2020 202d 2070 6174  .          - pat
-000235d0: 683a 202f 6261 720a 2020 2020 2020 2020  h: /bar.        
-000235e0: 2020 2020 6e61 6d65 3a20 696e 6772 6573      name: ingres
-000235f0: 732d 7061 7468 2d62 6172 0a20 2020 2020  s-path-bar.     
-00023600: 2020 2020 2020 2070 6174 685f 7479 7065         path_type
-00023610: 3a20 4578 6163 740a 2020 2020 2020 2020  : Exact.        
-00023620: 2020 2020 6261 636b 656e 643a 0a20 2020      backend:.   
-00023630: 2020 2020 2020 2020 2020 2073 6572 7669             servi
-00023640: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
-00023650: 2020 2020 706f 7274 3a20 3830 0a20 2020      port: 80.   
-00023660: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00023670: 653a 2064 656d 6f2d 6170 702d 7365 7276  e: demo-app-serv
-00023680: 6963 650a 2020 2020 2020 2020 2020 6e61  ice.          na
-00023690: 6d65 3a20 666f 6f2d 696e 6772 6573 732d  me: foo-ingress-
-000236a0: 7275 6c65 0a20 2020 2020 2020 2020 2068  rule.          h
-000236b0: 6f73 743a 2077 7777 2e66 6f6f 2e63 6f6d  ost: www.foo.com
-000236c0: 0a20 2020 2020 2020 2074 6c73 3a0a 2020  .        tls:.  
-000236d0: 2020 2020 2020 2d20 7365 6372 6574 5f6e        - secret_n
-000236e0: 616d 653a 2061 7070 2d73 6563 7265 740a  ame: app-secret.
-000236f0: 2020 2020 2020 2020 2020 686f 7374 733a            hosts:
-00023700: 0a20 2020 2020 2020 2020 202d 2077 7777  .          - www
-00023710: 2e66 6f6f 2e63 6f6d 0a20 2020 2020 2020  .foo.com.       
-00023720: 2020 202d 2077 7777 2e62 6172 2e63 6f6d     - www.bar.com
-00023730: 0a20 2020 2020 2020 2020 206e 616d 653a  .          name:
-00023740: 2066 6f6f 2d62 6172 2d69 6e67 7265 7373   foo-bar-ingress
-00023750: 0a20 2020 2020 2020 202d 2073 6563 7265  .        - secre
-00023760: 745f 6e61 6d65 3a20 6170 702d 7365 6372  t_name: app-secr
-00023770: 6574 0a20 2020 2020 2020 2020 2068 6f73  et.          hos
-00023780: 7473 3a0a 2020 2020 2020 2020 2020 2d20  ts:.          - 
-00023790: 7777 772e 666f 6f2e 636f 6d0a 2020 2020  www.foo.com.    
-000237a0: 2020 2020 2020 2d20 7777 772e 6261 722e        - www.bar.
-000237b0: 636f 6d0a 2020 2020 2020 2020 2020 6e61  com.          na
-000237c0: 6d65 3a20 666f 6f2d 6261 722d 696e 6772  me: foo-bar-ingr
-000237d0: 6573 730a 2020 2020 2020 2020 6c61 6265  ess.        labe
-000237e0: 6c73 3a0a 2020 2020 2020 2020 2d20 6170  ls:.        - ap
-000237f0: 703a 6465 6d6f 2d61 7070 0a20 2020 2020  p:demo-app.     
-00023800: 2020 202d 2076 6572 7369 6f6e 3a76 312e     - version:v1.
-00023810: 302e 300a 2020 2020 2020 7072 6f70 6572  0.0.      proper
-00023820: 7469 6573 3a0a 2020 2020 2020 2020 6e61  ties:.        na
-00023830: 6d65 3a0a 2020 2020 2020 2020 2020 6465  me:.          de
-00023840: 7363 7269 7074 696f 6e3a 2069 6e67 7265  scription: ingre
-00023850: 7373 206e 616d 652e 0a20 2020 2020 2020  ss name..       
-00023860: 2020 2065 7861 6d70 6c65 3a20 6465 6d6f     example: demo
-00023870: 2d61 7070 2d69 6e67 7265 7373 0a20 2020  -app-ingress.   
-00023880: 2020 2020 2020 2074 6974 6c65 3a20 6e61         title: na
-00023890: 6d65 0a20 2020 2020 2020 2020 2074 7970  me.          typ
-000238a0: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-000238b0: 2020 6e61 6d65 7370 6163 653a 0a20 2020    namespace:.   
-000238c0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-000238d0: 6f6e 3a20 6e61 6d65 7370 6163 6520 666f  on: namespace fo
-000238e0: 7220 7265 736f 7572 6365 2e0a 2020 2020  r resource..    
-000238f0: 2020 2020 2020 6578 616d 706c 653a 2067        example: g
-00023900: 6974 6f70 732d 6364 6e2d 6361 6368 650a  itops-cdn-cache.
-00023910: 2020 2020 2020 2020 2020 7469 746c 653a            title:
-00023920: 206e 616d 6573 7061 6365 0a20 2020 2020   namespace.     
-00023930: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-00023940: 670a 2020 2020 2020 2020 616e 6e6f 7461  g.        annota
-00023950: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
-00023960: 2064 6573 6372 6970 7469 6f6e 3a20 416e   description: An
-00023970: 2075 6e73 7472 7563 7475 7265 6420 6b65   unstructured ke
-00023980: 7920 7661 6c75 6520 6d61 7020 7468 6174  y value map that
-00023990: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-000239a0: 6174 7461 6368 2061 7262 6974 7261 7279  attach arbitrary
-000239b0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-000239c0: 6164 6174 610a 2020 2020 2020 2020 2020  adata.          
-000239d0: 6578 616d 706c 653a 0a20 2020 2020 2020  example:.       
-000239e0: 2020 202d 2061 6e6e 6f74 6174 696f 6e2d     - annotation-
-000239f0: 6b65 7931 3a76 616c 310a 2020 2020 2020  key1:val1.      
-00023a00: 2020 2020 2d20 616e 6e6f 7461 7469 6f6e      - annotation
-00023a10: 2d6b 6579 323a 7661 6c32 0a20 2020 2020  -key2:val2.     
-00023a20: 2020 2020 2069 7465 6d73 3a0a 2020 2020       items:.    
-00023a30: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
-00023a40: 7269 6e67 0a20 2020 2020 2020 2020 2074  ring.          t
-00023a50: 6974 6c65 3a20 416e 6e6f 7461 7469 6f6e  itle: Annotation
-00023a60: 730a 2020 2020 2020 2020 2020 7479 7065  s.          type
-00023a70: 3a20 6172 7261 790a 2020 2020 2020 2020  : array.        
-00023a80: 6c61 6265 6c73 3a0a 2020 2020 2020 2020  labels:.        
-00023a90: 2020 6465 7363 7269 7074 696f 6e3a 204d    description: M
-00023aa0: 6170 206f 6620 7374 7269 6e67 206b 6579  ap of string key
-00023ab0: 7320 616e 6420 7661 6c75 6573 2074 6861  s and values tha
-00023ac0: 7420 6361 6e20 6265 2075 7365 6420 746f  t can be used to
-00023ad0: 206f 7267 616e 697a 650a 2020 2020 2020   organize.      
-00023ae0: 2020 2020 2020 616e 6420 6361 7465 676f        and catego
-00023af0: 7269 7a65 2028 7363 6f70 6520 616e 6420  rize (scope and 
-00023b00: 7365 6c65 6374 2920 6f62 6a65 6374 730a  select) objects.
-00023b10: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
-00023b20: 653a 0a20 2020 2020 2020 2020 202d 2061  e:.          - a
-00023b30: 7070 3a64 656d 6f2d 6170 700a 2020 2020  pp:demo-app.    
-00023b40: 2020 2020 2020 2d20 7665 7273 696f 6e3a        - version:
-00023b50: 7631 2e30 2e30 0a20 2020 2020 2020 2020  v1.0.0.         
-00023b60: 2069 7465 6d73 3a0a 2020 2020 2020 2020   items:.        
-00023b70: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-00023b80: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
-00023b90: 3a20 4c61 6265 6c73 0a20 2020 2020 2020  : Labels.       
-00023ba0: 2020 2074 7970 653a 2061 7272 6179 0a20     type: array. 
-00023bb0: 2020 2020 2020 2072 756c 6573 3a0a 2020         rules:.  
-00023bc0: 2020 2020 2020 2020 6974 656d 733a 0a20          items:. 
-00023bd0: 2020 2020 2020 2020 2020 2024 7265 663a             $ref:
-00023be0: 2027 232f 636f 6d70 6f6e 656e 7473 2f73   '#/components/s
-00023bf0: 6368 656d 6173 2f49 6e67 7265 7373 5275  chemas/IngressRu
-00023c00: 6c65 270a 2020 2020 2020 2020 2020 7469  le'.          ti
-00023c10: 746c 653a 2072 756c 6573 0a20 2020 2020  tle: rules.     
-00023c20: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
-00023c30: 0a20 2020 2020 2020 2074 6c73 3a0a 2020  .        tls:.  
-00023c40: 2020 2020 2020 2020 6974 656d 733a 0a20          items:. 
-00023c50: 2020 2020 2020 2020 2020 2024 7265 663a             $ref:
-00023c60: 2027 232f 636f 6d70 6f6e 656e 7473 2f73   '#/components/s
-00023c70: 6368 656d 6173 2f49 6e67 7265 7373 544c  chemas/IngressTL
-00023c80: 5327 0a20 2020 2020 2020 2020 2074 6974  S'.          tit
-00023c90: 6c65 3a20 746c 730a 2020 2020 2020 2020  le: tls.        
-00023ca0: 2020 7479 7065 3a20 6172 7261 790a 2020    type: array.  
-00023cb0: 2020 2020 7265 7175 6972 6564 3a0a 2020      required:.  
-00023cc0: 2020 2020 2d20 6e61 6d65 0a20 2020 2020      - name.     
-00023cd0: 2074 6974 6c65 3a20 496e 6772 6573 730a   title: Ingress.
-00023ce0: 2020 2020 2020 7479 7065 3a20 6f62 6a65        type: obje
-00023cf0: 6374 0a20 2020 2049 6e67 7265 7373 5275  ct.    IngressRu
-00023d00: 6c65 3a0a 2020 2020 2020 6578 616d 706c  le:.      exampl
-00023d10: 653a 0a20 2020 2020 2020 2070 6174 6873  e:.        paths
-00023d20: 3a0a 2020 2020 2020 2020 2d20 7061 7468  :.        - path
-00023d30: 3a20 2f62 6172 0a20 2020 2020 2020 2020  : /bar.         
-00023d40: 206e 616d 653a 2069 6e67 7265 7373 2d70   name: ingress-p
-00023d50: 6174 682d 6261 720a 2020 2020 2020 2020  ath-bar.        
-00023d60: 2020 7061 7468 5f74 7970 653a 2045 7861    path_type: Exa
-00023d70: 6374 0a20 2020 2020 2020 2020 2062 6163  ct.          bac
-00023d80: 6b65 6e64 3a0a 2020 2020 2020 2020 2020  kend:.          
-00023d90: 2020 7365 7276 6963 653a 0a20 2020 2020    service:.     
-00023da0: 2020 2020 2020 2020 2070 6f72 743a 2038           port: 8
-00023db0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-00023dc0: 6e61 6d65 3a20 6465 6d6f 2d61 7070 2d73  name: demo-app-s
-00023dd0: 6572 7669 6365 0a20 2020 2020 2020 202d  ervice.        -
-00023de0: 2070 6174 683a 202f 6261 720a 2020 2020   path: /bar.    
-00023df0: 2020 2020 2020 6e61 6d65 3a20 696e 6772        name: ingr
-00023e00: 6573 732d 7061 7468 2d62 6172 0a20 2020  ess-path-bar.   
-00023e10: 2020 2020 2020 2070 6174 685f 7479 7065         path_type
-00023e20: 3a20 4578 6163 740a 2020 2020 2020 2020  : Exact.        
-00023e30: 2020 6261 636b 656e 643a 0a20 2020 2020    backend:.     
-00023e40: 2020 2020 2020 2073 6572 7669 6365 3a0a         service:.
-00023e50: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00023e60: 7274 3a20 3830 0a20 2020 2020 2020 2020  rt: 80.         
-00023e70: 2020 2020 206e 616d 653a 2064 656d 6f2d       name: demo-
-00023e80: 6170 702d 7365 7276 6963 650a 2020 2020  app-service.    
-00023e90: 2020 2020 6e61 6d65 3a20 666f 6f2d 696e      name: foo-in
-00023ea0: 6772 6573 732d 7275 6c65 0a20 2020 2020  gress-rule.     
-00023eb0: 2020 2068 6f73 743a 2077 7777 2e66 6f6f     host: www.foo
-00023ec0: 2e63 6f6d 0a20 2020 2020 2070 726f 7065  .com.      prope
-00023ed0: 7274 6965 733a 0a20 2020 2020 2020 206e  rties:.        n
-00023ee0: 616d 653a 0a20 2020 2020 2020 2020 2064  ame:.          d
-00023ef0: 6573 6372 6970 7469 6f6e 3a20 5468 6520  escription: The 
-00023f00: 7275 6c65 206e 616d 652e 0a20 2020 2020  rule name..     
-00023f10: 2020 2020 2065 7861 6d70 6c65 3a20 666f       example: fo
-00023f20: 6f2d 696e 6772 6573 732d 7275 6c65 0a20  o-ingress-rule. 
-00023f30: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-00023f40: 6e61 6d65 0a20 2020 2020 2020 2020 2074  name.          t
-00023f50: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
-00023f60: 2020 2020 686f 7374 3a0a 2020 2020 2020      host:.      
-00023f70: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00023f80: 2041 2066 756c 6c79 2071 7561 6c69 6669   A fully qualifi
-00023f90: 6564 2064 6f6d 6169 6e20 6e61 6d65 206f  ed domain name o
-00023fa0: 6620 6120 6e65 7477 6f72 6b20 686f 7374  f a network host
-00023fb0: 2e0a 2020 2020 2020 2020 2020 6578 616d  ..          exam
-00023fc0: 706c 653a 2077 7777 2e66 6f6f 2e63 6f6d  ple: www.foo.com
-00023fd0: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
-00023fe0: 3a20 686f 7374 0a20 2020 2020 2020 2020  : host.         
-00023ff0: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
-00024000: 2020 2020 2020 7061 7468 733a 0a20 2020        paths:.   
-00024010: 2020 2020 2020 2069 7465 6d73 3a0a 2020         items:.  
-00024020: 2020 2020 2020 2020 2020 2472 6566 3a20            $ref: 
-00024030: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
-00024040: 6865 6d61 732f 4854 5450 496e 6772 6573  hemas/HTTPIngres
-00024050: 7350 6174 6827 0a20 2020 2020 2020 2020  sPath'.         
-00024060: 2074 6974 6c65 3a20 7061 7468 730a 2020   title: paths.  
-00024070: 2020 2020 2020 2020 7479 7065 3a20 6172          type: ar
-00024080: 7261 790a 2020 2020 2020 7469 746c 653a  ray.      title:
-00024090: 2049 6e67 7265 7373 5275 6c65 0a20 2020   IngressRule.   
-000240a0: 2020 2074 7970 653a 206f 626a 6563 740a     type: object.
-000240b0: 2020 2020 4854 5450 496e 6772 6573 7350      HTTPIngressP
-000240c0: 6174 683a 0a20 2020 2020 2065 7861 6d70  ath:.      examp
-000240d0: 6c65 3a0a 2020 2020 2020 2020 7061 7468  le:.        path
-000240e0: 3a20 2f62 6172 0a20 2020 2020 2020 206e  : /bar.        n
-000240f0: 616d 653a 2069 6e67 7265 7373 2d70 6174  ame: ingress-pat
-00024100: 682d 6261 720a 2020 2020 2020 2020 7061  h-bar.        pa
-00024110: 7468 5f74 7970 653a 2045 7861 6374 0a20  th_type: Exact. 
-00024120: 2020 2020 2020 2062 6163 6b65 6e64 3a0a         backend:.
-00024130: 2020 2020 2020 2020 2020 7365 7276 6963            servic
-00024140: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-00024150: 6f72 743a 2038 300a 2020 2020 2020 2020  ort: 80.        
-00024160: 2020 2020 6e61 6d65 3a20 6465 6d6f 2d61      name: demo-a
-00024170: 7070 2d73 6572 7669 6365 0a20 2020 2020  pp-service.     
-00024180: 2070 726f 7065 7274 6965 733a 0a20 2020   properties:.   
-00024190: 2020 2020 206e 616d 653a 0a20 2020 2020       name:.     
-000241a0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-000241b0: 3a20 5468 6520 696e 6772 6573 7320 7061  : The ingress pa
-000241c0: 7468 206e 616d 652e 0a20 2020 2020 2020  th name..       
-000241d0: 2020 2065 7861 6d70 6c65 3a20 696e 6772     example: ingr
-000241e0: 6573 732d 7061 7468 2d62 6172 0a20 2020  ess-path-bar.   
-000241f0: 2020 2020 2020 2074 6974 6c65 3a20 6e61         title: na
-00024200: 6d65 0a20 2020 2020 2020 2020 2074 7970  me.          typ
-00024210: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-00024220: 2020 7061 7468 3a0a 2020 2020 2020 2020    path:.        
-00024230: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
-00024240: 6865 2070 6174 6820 7468 6174 2069 7320  he path that is 
-00024250: 6d61 7463 6865 6420 6167 6169 6e73 7420  matched against 
-00024260: 7468 6520 7061 7468 206f 6620 616e 2069  the path of an i
-00024270: 6e63 6f6d 696e 6720 7265 7175 6573 742e  ncoming request.
-00024280: 0a20 2020 2020 2020 2020 2020 204d 7573  .            Mus
-00024290: 7420 6265 6769 6e20 7769 7468 2061 2027  t begin with a '
-000242a0: 2f27 2e0a 2020 2020 2020 2020 2020 6578  /'..          ex
-000242b0: 616d 706c 653a 202f 6261 720a 2020 2020  ample: /bar.    
-000242c0: 2020 2020 2020 7469 746c 653a 2070 6174        title: pat
-000242d0: 680a 2020 2020 2020 2020 2020 7479 7065  h.          type
-000242e0: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
-000242f0: 2070 6174 685f 7479 7065 3a0a 2020 2020   path_type:.    
-00024300: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00024310: 6e3a 2050 6174 6854 7970 6520 6465 7465  n: PathType dete
-00024320: 726d 696e 6573 2074 6865 2069 6e74 6572  rmines the inter
-00024330: 7072 6574 6174 696f 6e20 6f66 2074 6865  pretation of the
-00024340: 2050 6174 6820 6d61 7463 6869 6e67 2e0a   Path matching..
-00024350: 2020 2020 2020 2020 2020 656e 756d 3a0a            enum:.
-00024360: 2020 2020 2020 2020 2020 2d20 4578 6163            - Exac
-00024370: 740a 2020 2020 2020 2020 2020 2d20 5072  t.          - Pr
-00024380: 6566 6978 0a20 2020 2020 2020 2020 2065  efix.          e
-00024390: 7861 6d70 6c65 3a20 4578 6163 740a 2020  xample: Exact.  
-000243a0: 2020 2020 2020 2020 7469 746c 653a 2070          title: p
-000243b0: 6174 685f 7479 7065 0a20 2020 2020 2020  ath_type.       
-000243c0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
-000243d0: 2020 2020 2020 2020 6261 636b 656e 643a          backend:
-000243e0: 0a20 2020 2020 2020 2020 2024 7265 663a  .          $ref:
-000243f0: 2027 232f 636f 6d70 6f6e 656e 7473 2f73   '#/components/s
-00024400: 6368 656d 6173 2f49 6e67 7265 7373 4261  chemas/IngressBa
-00024410: 636b 656e 6427 0a20 2020 2020 2074 6974  ckend'.      tit
-00024420: 6c65 3a20 4854 5450 496e 6772 6573 7350  le: HTTPIngressP
-00024430: 6174 680a 2020 2020 2020 7479 7065 3a20  ath.      type: 
-00024440: 6f62 6a65 6374 0a20 2020 2049 6e67 7265  object.    Ingre
-00024450: 7373 4261 636b 656e 643a 0a20 2020 2020  ssBackend:.     
-00024460: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
-00024470: 2020 7365 7276 6963 653a 0a20 2020 2020    service:.     
-00024480: 2020 2020 2070 6f72 743a 2038 300a 2020       port: 80.  
-00024490: 2020 2020 2020 2020 6e61 6d65 3a20 6465          name: de
-000244a0: 6d6f 2d61 7070 2d73 6572 7669 6365 0a20  mo-app-service. 
-000244b0: 2020 2020 2070 726f 7065 7274 6965 733a       properties:
-000244c0: 0a20 2020 2020 2020 2073 6572 7669 6365  .        service
-000244d0: 3a0a 2020 2020 2020 2020 2020 2472 6566  :.          $ref
-000244e0: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
-000244f0: 7363 6865 6d61 732f 496e 6772 6573 7342  schemas/IngressB
-00024500: 6163 6b65 6e64 5f73 6572 7669 6365 270a  ackend_service'.
-00024510: 2020 2020 2020 7469 746c 653a 2049 6e67        title: Ing
-00024520: 7265 7373 4261 636b 656e 640a 2020 2020  ressBackend.    
-00024530: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
-00024540: 2020 2049 6e67 7265 7373 544c 533a 0a20     IngressTLS:. 
-00024550: 2020 2020 2065 7861 6d70 6c65 3a0a 2020       example:.  
-00024560: 2020 2020 2020 7365 6372 6574 5f6e 616d        secret_nam
-00024570: 653a 2061 7070 2d73 6563 7265 740a 2020  e: app-secret.  
-00024580: 2020 2020 2020 686f 7374 733a 0a20 2020        hosts:.   
-00024590: 2020 2020 202d 2077 7777 2e66 6f6f 2e63       - www.foo.c
-000245a0: 6f6d 0a20 2020 2020 2020 202d 2077 7777  om.        - www
-000245b0: 2e62 6172 2e63 6f6d 0a20 2020 2020 2020  .bar.com.       
-000245c0: 206e 616d 653a 2066 6f6f 2d62 6172 2d69   name: foo-bar-i
-000245d0: 6e67 7265 7373 0a20 2020 2020 2070 726f  ngress.      pro
-000245e0: 7065 7274 6965 733a 0a20 2020 2020 2020  perties:.       
-000245f0: 206e 616d 653a 0a20 2020 2020 2020 2020   name:.         
-00024600: 2064 6573 6372 6970 7469 6f6e 3a20 4e61   description: Na
-00024610: 6d65 206f 6620 7468 6520 544c 5320 636f  me of the TLS co
-00024620: 6e66 6967 2e0a 2020 2020 2020 2020 2020  nfig..          
-00024630: 6578 616d 706c 653a 2066 6f6f 2d62 6172  example: foo-bar
-00024640: 2d69 6e67 7265 7373 0a20 2020 2020 2020  -ingress.       
-00024650: 2020 2074 6974 6c65 3a20 6e61 6d65 0a20     title: name. 
-00024660: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-00024670: 7472 696e 670a 2020 2020 2020 2020 686f  tring.        ho
-00024680: 7374 733a 0a20 2020 2020 2020 2020 2064  sts:.          d
-00024690: 6573 6372 6970 7469 6f6e 3a20 4120 6c69  escription: A li
-000246a0: 7374 206f 6620 686f 7374 7320 696e 636c  st of hosts incl
-000246b0: 7564 6564 2069 6e20 7468 6520 544c 5320  uded in the TLS 
-000246c0: 6365 7274 6966 6963 6174 652e 0a20 2020  certificate..   
-000246d0: 2020 2020 2020 2065 7861 6d70 6c65 3a0a         example:.
-000246e0: 2020 2020 2020 2020 2020 2d20 7777 772e            - www.
-000246f0: 666f 6f2e 636f 6d0a 2020 2020 2020 2020  foo.com.        
-00024700: 2020 2d20 7777 772e 6261 722e 636f 6d0a    - www.bar.com.
-00024710: 2020 2020 2020 2020 2020 6974 656d 733a            items:
-00024720: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
-00024730: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-00024740: 2020 2020 7469 746c 653a 2068 6f73 7473      title: hosts
-00024750: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
-00024760: 2061 7272 6179 0a20 2020 2020 2020 2073   array.        s
-00024770: 6563 7265 745f 6e61 6d65 3a0a 2020 2020  ecret_name:.    
-00024780: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00024790: 6e3a 2054 6865 206e 616d 6520 6f66 2074  n: The name of t
-000247a0: 6865 2073 6563 7265 7420 7573 6564 2074  he secret used t
-000247b0: 6f20 7465 726d 696e 6174 6520 544c 5320  o terminate TLS 
-000247c0: 7472 6166 6669 6320 6f6e 2070 6f72 740a  traffic on port.
-000247d0: 2020 2020 2020 2020 2020 2020 3434 332e              443.
-000247e0: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-000247f0: 6c65 3a20 6170 702d 7365 6372 6574 0a20  le: app-secret. 
-00024800: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-00024810: 7365 6372 6574 5f6e 616d 650a 2020 2020  secret_name.    
-00024820: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
-00024830: 6e67 0a20 2020 2020 2074 6974 6c65 3a20  ng.      title: 
-00024840: 496e 6772 6573 7354 4c53 0a20 2020 2020  IngressTLS.     
-00024850: 2074 7970 653a 206f 626a 6563 740a 2020   type: object.  
-00024860: 2020 5365 7276 6963 654d 6f6e 6974 6f72    ServiceMonitor
-00024870: 3a0a 2020 2020 2020 6578 616d 706c 653a  :.      example:
-00024880: 0a20 2020 2020 2020 206e 616d 6573 7061  .        namespa
-00024890: 6365 5f73 656c 6563 746f 723a 0a20 2020  ce_selector:.   
-000248a0: 2020 2020 2020 206d 6174 6368 5f6e 616d         match_nam
-000248b0: 6573 3a0a 2020 2020 2020 2020 2020 2d20  es:.          - 
-000248c0: 6465 6661 756c 740a 2020 2020 2020 2020  default.        
-000248d0: 2020 616e 793a 2074 7275 650a 2020 2020    any: true.    
-000248e0: 2020 2020 656e 6470 6f69 6e74 733a 0a20      endpoints:. 
-000248f0: 2020 2020 2020 202d 2068 6f6e 6f72 5f6c         - honor_l
-00024900: 6162 656c 733a 2074 7275 650a 2020 2020  abels: true.    
-00024910: 2020 2020 2020 7061 7468 3a20 2f6d 6574        path: /met
-00024920: 7269 6373 0a20 2020 2020 2020 2020 2074  rics.          t
-00024930: 6172 6765 745f 706f 7274 3a20 3830 3830  arget_port: 8080
-00024940: 0a20 2020 2020 2020 2020 2072 656c 6162  .          relab
-00024950: 656c 696e 6773 3a0a 2020 2020 2020 2020  elings:.        
-00024960: 2020 2d20 7265 6765 783a 2028 2e2a 290a    - regex: (.*).
-00024970: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-00024980: 6365 5f6c 6162 656c 733a 0a20 2020 2020  ce_labels:.     
-00024990: 2020 2020 2020 202d 205f 5f6d 6574 615f         - __meta_
-000249a0: 6b75 6265 726e 6574 6573 5f70 6f64 5f6c  kubernetes_pod_l
-000249b0: 6162 656c 5f61 7070 5f6b 7562 6572 6e65  abel_app_kuberne
-000249c0: 7465 735f 696f 5f6e 616d 650a 2020 2020  tes_io_name.    
-000249d0: 2020 2020 2020 2020 6163 7469 6f6e 3a20          action: 
-000249e0: 7265 706c 6163 650a 2020 2020 2020 2020  replace.        
-000249f0: 2020 2020 7365 7061 7261 746f 723a 203b      separator: ;
-00024a00: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-00024a10: 6c61 6365 6d65 6e74 3a20 2431 0a20 2020  lacement: $1.   
-00024a20: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00024a30: 6c61 6265 6c3a 205f 5f6d 6574 7269 6373  label: __metrics
-00024a40: 5f70 6174 685f 5f0a 2020 2020 2020 2020  _path__.        
-00024a50: 2020 2d20 7265 6765 783a 2028 2e2a 290a    - regex: (.*).
-00024a60: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-00024a70: 6365 5f6c 6162 656c 733a 0a20 2020 2020  ce_labels:.     
-00024a80: 2020 2020 2020 202d 205f 5f6d 6574 615f         - __meta_
-00024a90: 6b75 6265 726e 6574 6573 5f70 6f64 5f6c  kubernetes_pod_l
-00024aa0: 6162 656c 5f61 7070 5f6b 7562 6572 6e65  abel_app_kuberne
-00024ab0: 7465 735f 696f 5f6e 616d 650a 2020 2020  tes_io_name.    
-00024ac0: 2020 2020 2020 2020 6163 7469 6f6e 3a20          action: 
-00024ad0: 7265 706c 6163 650a 2020 2020 2020 2020  replace.        
-00024ae0: 2020 2020 7365 7061 7261 746f 723a 203b      separator: ;
-00024af0: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-00024b00: 6c61 6365 6d65 6e74 3a20 2431 0a20 2020  lacement: $1.   
-00024b10: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00024b20: 6c61 6265 6c3a 205f 5f6d 6574 7269 6373  label: __metrics
-00024b30: 5f70 6174 685f 5f0a 2020 2020 2020 2020  _path__.        
-00024b40: 2020 6d65 7472 6963 5f72 656c 6162 656c    metric_relabel
-00024b50: 696e 6773 3a0a 2020 2020 2020 2020 2020  ings:.          
-00024b60: 2d20 7265 6765 783a 2028 2e2a 290a 2020  - regex: (.*).  
-00024b70: 2020 2020 2020 2020 2020 736f 7572 6365            source
-00024b80: 5f6c 6162 656c 733a 0a20 2020 2020 2020  _labels:.       
-00024b90: 2020 2020 202d 205f 5f6d 6574 615f 6b75       - __meta_ku
-00024ba0: 6265 726e 6574 6573 5f70 6f64 5f6c 6162  bernetes_pod_lab
-00024bb0: 656c 5f61 7070 5f6b 7562 6572 6e65 7465  el_app_kubernete
-00024bc0: 735f 696f 5f6e 616d 650a 2020 2020 2020  s_io_name.      
-00024bd0: 2020 2020 2020 6163 7469 6f6e 3a20 7265        action: re
-00024be0: 706c 6163 650a 2020 2020 2020 2020 2020  place.          
-00024bf0: 2020 7365 7061 7261 746f 723a 203b 0a20    separator: ;. 
-00024c00: 2020 2020 2020 2020 2020 2072 6570 6c61             repla
-00024c10: 6365 6d65 6e74 3a20 2431 0a20 2020 2020  cement: $1.     
-00024c20: 2020 2020 2020 2074 6172 6765 745f 6c61         target_la
-00024c30: 6265 6c3a 205f 5f6d 6574 7269 6373 5f70  bel: __metrics_p
-00024c40: 6174 685f 5f0a 2020 2020 2020 2020 2020  ath__.          
-00024c50: 2d20 7265 6765 783a 2028 2e2a 290a 2020  - regex: (.*).  
-00024c60: 2020 2020 2020 2020 2020 736f 7572 6365            source
-00024c70: 5f6c 6162 656c 733a 0a20 2020 2020 2020  _labels:.       
-00024c80: 2020 2020 202d 205f 5f6d 6574 615f 6b75       - __meta_ku
-00024c90: 6265 726e 6574 6573 5f70 6f64 5f6c 6162  bernetes_pod_lab
-00024ca0: 656c 5f61 7070 5f6b 7562 6572 6e65 7465  el_app_kubernete
-00024cb0: 735f 696f 5f6e 616d 650a 2020 2020 2020  s_io_name.      
-00024cc0: 2020 2020 2020 6163 7469 6f6e 3a20 7265        action: re
-00024cd0: 706c 6163 650a 2020 2020 2020 2020 2020  place.          
-00024ce0: 2020 7365 7061 7261 746f 723a 203b 0a20    separator: ;. 
-00024cf0: 2020 2020 2020 2020 2020 2072 6570 6c61             repla
-00024d00: 6365 6d65 6e74 3a20 2431 0a20 2020 2020  cement: $1.     
-00024d10: 2020 2020 2020 2074 6172 6765 745f 6c61         target_la
-00024d20: 6265 6c3a 205f 5f6d 6574 7269 6373 5f70  bel: __metrics_p
-00024d30: 6174 685f 5f0a 2020 2020 2020 2020 2020  ath__.          
-00024d40: 7363 6865 6d65 3a20 6874 7470 0a20 2020  scheme: http.   
-00024d50: 2020 2020 2020 2070 6f72 743a 2038 3038         port: 808
-00024d60: 300a 2020 2020 2020 2020 2020 686f 6e6f  0.          hono
-00024d70: 725f 7469 6d65 7374 616d 7073 3a20 7472  r_timestamps: tr
-00024d80: 7565 0a20 2020 2020 2020 2020 2073 6372  ue.          scr
-00024d90: 6170 655f 7469 6d65 6f75 743a 2031 3073  ape_timeout: 10s
-00024da0: 0a20 2020 2020 2020 2020 2069 6e74 6572  .          inter
-00024db0: 7661 6c3a 2033 3073 0a20 2020 2020 2020  val: 30s.       
-00024dc0: 2020 2070 6172 616d 733a 0a20 2020 2020     params:.     
-00024dd0: 2020 2020 2020 206d 6f64 756c 653a 0a20         module:. 
-00024de0: 2020 2020 2020 2020 2020 202d 2068 7474             - htt
-00024df0: 705f 3278 780a 2020 2020 2020 2020 2d20  p_2xx.        - 
-00024e00: 686f 6e6f 725f 6c61 6265 6c73 3a20 7472  honor_labels: tr
-00024e10: 7565 0a20 2020 2020 2020 2020 2070 6174  ue.          pat
-00024e20: 683a 202f 6d65 7472 6963 730a 2020 2020  h: /metrics.    
-00024e30: 2020 2020 2020 7461 7267 6574 5f70 6f72        target_por
-00024e40: 743a 2038 3038 300a 2020 2020 2020 2020  t: 8080.        
-00024e50: 2020 7265 6c61 6265 6c69 6e67 733a 0a20    relabelings:. 
-00024e60: 2020 2020 2020 2020 202d 2072 6567 6578           - regex
-00024e70: 3a20 282e 2a29 0a20 2020 2020 2020 2020  : (.*).         
-00024e80: 2020 2073 6f75 7263 655f 6c61 6265 6c73     source_labels
-00024e90: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
-00024ea0: 5f5f 6d65 7461 5f6b 7562 6572 6e65 7465  __meta_kubernete
-00024eb0: 735f 706f 645f 6c61 6265 6c5f 6170 705f  s_pod_label_app_
-00024ec0: 6b75 6265 726e 6574 6573 5f69 6f5f 6e61  kubernetes_io_na
-00024ed0: 6d65 0a20 2020 2020 2020 2020 2020 2061  me.            a
-00024ee0: 6374 696f 6e3a 2072 6570 6c61 6365 0a20  ction: replace. 
-00024ef0: 2020 2020 2020 2020 2020 2073 6570 6172             separ
-00024f00: 6174 6f72 3a20 3b0a 2020 2020 2020 2020  ator: ;.        
-00024f10: 2020 2020 7265 706c 6163 656d 656e 743a      replacement:
-00024f20: 2024 310a 2020 2020 2020 2020 2020 2020   $1.            
-00024f30: 7461 7267 6574 5f6c 6162 656c 3a20 5f5f  target_label: __
-00024f40: 6d65 7472 6963 735f 7061 7468 5f5f 0a20  metrics_path__. 
-00024f50: 2020 2020 2020 2020 202d 2072 6567 6578           - regex
-00024f60: 3a20 282e 2a29 0a20 2020 2020 2020 2020  : (.*).         
-00024f70: 2020 2073 6f75 7263 655f 6c61 6265 6c73     source_labels
-00024f80: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
-00024f90: 5f5f 6d65 7461 5f6b 7562 6572 6e65 7465  __meta_kubernete
-00024fa0: 735f 706f 645f 6c61 6265 6c5f 6170 705f  s_pod_label_app_
-00024fb0: 6b75 6265 726e 6574 6573 5f69 6f5f 6e61  kubernetes_io_na
-00024fc0: 6d65 0a20 2020 2020 2020 2020 2020 2061  me.            a
-00024fd0: 6374 696f 6e3a 2072 6570 6c61 6365 0a20  ction: replace. 
-00024fe0: 2020 2020 2020 2020 2020 2073 6570 6172             separ
-00024ff0: 6174 6f72 3a20 3b0a 2020 2020 2020 2020  ator: ;.        
-00025000: 2020 2020 7265 706c 6163 656d 656e 743a      replacement:
-00025010: 2024 310a 2020 2020 2020 2020 2020 2020   $1.            
-00025020: 7461 7267 6574 5f6c 6162 656c 3a20 5f5f  target_label: __
-00025030: 6d65 7472 6963 735f 7061 7468 5f5f 0a20  metrics_path__. 
-00025040: 2020 2020 2020 2020 206d 6574 7269 635f           metric_
-00025050: 7265 6c61 6265 6c69 6e67 733a 0a20 2020  relabelings:.   
-00025060: 2020 2020 2020 202d 2072 6567 6578 3a20         - regex: 
-00025070: 282e 2a29 0a20 2020 2020 2020 2020 2020  (.*).           
-00025080: 2073 6f75 7263 655f 6c61 6265 6c73 3a0a   source_labels:.
-00025090: 2020 2020 2020 2020 2020 2020 2d20 5f5f              - __
-000250a0: 6d65 7461 5f6b 7562 6572 6e65 7465 735f  meta_kubernetes_
-000250b0: 706f 645f 6c61 6265 6c5f 6170 705f 6b75  pod_label_app_ku
-000250c0: 6265 726e 6574 6573 5f69 6f5f 6e61 6d65  bernetes_io_name
-000250d0: 0a20 2020 2020 2020 2020 2020 2061 6374  .            act
-000250e0: 696f 6e3a 2072 6570 6c61 6365 0a20 2020  ion: replace.   
-000250f0: 2020 2020 2020 2020 2073 6570 6172 6174           separat
-00025100: 6f72 3a20 3b0a 2020 2020 2020 2020 2020  or: ;.          
-00025110: 2020 7265 706c 6163 656d 656e 743a 2024    replacement: $
-00025120: 310a 2020 2020 2020 2020 2020 2020 7461  1.            ta
-00025130: 7267 6574 5f6c 6162 656c 3a20 5f5f 6d65  rget_label: __me
-00025140: 7472 6963 735f 7061 7468 5f5f 0a20 2020  trics_path__.   
-00025150: 2020 2020 2020 202d 2072 6567 6578 3a20         - regex: 
-00025160: 282e 2a29 0a20 2020 2020 2020 2020 2020  (.*).           
-00025170: 2073 6f75 7263 655f 6c61 6265 6c73 3a0a   source_labels:.
-00025180: 2020 2020 2020 2020 2020 2020 2d20 5f5f              - __
-00025190: 6d65 7461 5f6b 7562 6572 6e65 7465 735f  meta_kubernetes_
-000251a0: 706f 645f 6c61 6265 6c5f 6170 705f 6b75  pod_label_app_ku
-000251b0: 6265 726e 6574 6573 5f69 6f5f 6e61 6d65  bernetes_io_name
-000251c0: 0a20 2020 2020 2020 2020 2020 2061 6374  .            act
-000251d0: 696f 6e3a 2072 6570 6c61 6365 0a20 2020  ion: replace.   
-000251e0: 2020 2020 2020 2020 2073 6570 6172 6174           separat
-000251f0: 6f72 3a20 3b0a 2020 2020 2020 2020 2020  or: ;.          
-00025200: 2020 7265 706c 6163 656d 656e 743a 2024    replacement: $
-00025210: 310a 2020 2020 2020 2020 2020 2020 7461  1.            ta
-00025220: 7267 6574 5f6c 6162 656c 3a20 5f5f 6d65  rget_label: __me
-00025230: 7472 6963 735f 7061 7468 5f5f 0a20 2020  trics_path__.   
-00025240: 2020 2020 2020 2073 6368 656d 653a 2068         scheme: h
-00025250: 7474 700a 2020 2020 2020 2020 2020 706f  ttp.          po
-00025260: 7274 3a20 3830 3830 0a20 2020 2020 2020  rt: 8080.       
-00025270: 2020 2068 6f6e 6f72 5f74 696d 6573 7461     honor_timesta
-00025280: 6d70 733a 2074 7275 650a 2020 2020 2020  mps: true.      
-00025290: 2020 2020 7363 7261 7065 5f74 696d 656f      scrape_timeo
-000252a0: 7574 3a20 3130 730a 2020 2020 2020 2020  ut: 10s.        
-000252b0: 2020 696e 7465 7276 616c 3a20 3330 730a    interval: 30s.
-000252c0: 2020 2020 2020 2020 2020 7061 7261 6d73            params
-000252d0: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
-000252e0: 6475 6c65 3a0a 2020 2020 2020 2020 2020  dule:.          
-000252f0: 2020 2d20 6874 7470 5f32 7878 0a20 2020    - http_2xx.   
-00025300: 2020 2020 206e 616d 653a 206d 792d 7365       name: my-se
-00025310: 7276 6963 652d 6d6f 6e69 746f 720a 2020  rvice-monitor.  
-00025320: 2020 2020 2020 6e61 6d65 7370 6163 653a        namespace:
-00025330: 2067 6974 6f70 732d 6364 6e2d 6361 6368   gitops-cdn-cach
-00025340: 650a 2020 2020 2020 2020 616e 6e6f 7461  e.        annota
-00025350: 7469 6f6e 733a 0a20 2020 2020 2020 202d  tions:.        -
-00025360: 2061 6e6e 6f74 6174 696f 6e2d 6b65 7931   annotation-key1
-00025370: 3a76 616c 310a 2020 2020 2020 2020 2d20  :val1.        - 
-00025380: 616e 6e6f 7461 7469 6f6e 2d6b 6579 323a  annotation-key2:
-00025390: 7661 6c32 0a20 2020 2020 2020 2073 656c  val2.        sel
-000253a0: 6563 746f 723a 0a20 2020 2020 2020 202d  ector:.        -
-000253b0: 2061 7070 3a64 656d 6f2d 6170 700a 2020   app:demo-app.  
-000253c0: 2020 2020 2020 2d20 226b 6579 3a76 6572        - "key:ver
-000253d0: 7369 6f6e 2c20 6f70 6572 6174 6f72 3a49  sion, operator:I
-000253e0: 6e2c 2076 616c 7565 733a 5b76 312e 302e  n, values:[v1.0.
-000253f0: 302c 2076 312e 302e 315d 220a 2020 2020  0, v1.0.1]".    
-00025400: 2020 2020 6c61 6265 6c73 3a0a 2020 2020      labels:.    
-00025410: 2020 2020 2d20 6170 703a 6465 6d6f 2d61      - app:demo-a
-00025420: 7070 0a20 2020 2020 2020 202d 2076 6572  pp.        - ver
-00025430: 7369 6f6e 3a76 312e 302e 300a 2020 2020  sion:v1.0.0.    
-00025440: 2020 7072 6f70 6572 7469 6573 3a0a 2020    properties:.  
-00025450: 2020 2020 2020 6e61 6d65 3a0a 2020 2020        name:.    
-00025460: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00025470: 6e3a 2022 6e61 6d65 206f 6620 7365 7276  n: "name of serv
-00025480: 6963 6520 6d6f 6e69 746f 722c 2075 7365  ice monitor, use
-00025490: 6420 696e 206d 6574 6164 6174 612e 6e61  d in metadata.na
-000254a0: 6d65 220a 2020 2020 2020 2020 2020 6578  me".          ex
-000254b0: 616d 706c 653a 206d 792d 7365 7276 6963  ample: my-servic
-000254c0: 652d 6d6f 6e69 746f 720a 2020 2020 2020  e-monitor.      
-000254d0: 2020 2020 7469 746c 653a 206e 616d 650a      title: name.
-000254e0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-000254f0: 7374 7269 6e67 0a20 2020 2020 2020 206e  string.        n
-00025500: 616d 6573 7061 6365 3a0a 2020 2020 2020  amespace:.      
-00025510: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00025520: 206e 616d 6573 7061 6365 2066 6f72 2072   namespace for r
-00025530: 6573 6f75 7263 652e 0a20 2020 2020 2020  esource..       
-00025540: 2020 2065 7861 6d70 6c65 3a20 6769 746f     example: gito
-00025550: 7073 2d63 646e 2d63 6163 6865 0a20 2020  ps-cdn-cache.   
-00025560: 2020 2020 2020 2074 6974 6c65 3a20 6e61         title: na
-00025570: 6d65 7370 6163 650a 2020 2020 2020 2020  mespace.        
-00025580: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00025590: 2020 2020 2020 206c 6162 656c 733a 0a20         labels:. 
-000255a0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-000255b0: 7469 6f6e 3a20 4d61 7020 6f66 2073 7472  tion: Map of str
-000255c0: 696e 6720 6b65 7973 2061 6e64 2076 616c  ing keys and val
-000255d0: 7565 7320 7468 6174 2063 616e 2062 6520  ues that can be 
-000255e0: 7573 6564 2074 6f20 6f72 6761 6e69 7a65  used to organize
-000255f0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-00025600: 2063 6174 6567 6f72 697a 6520 2873 636f   categorize (sco
-00025610: 7065 2061 6e64 2073 656c 6563 7429 206f  pe and select) o
-00025620: 626a 6563 7473 0a20 2020 2020 2020 2020  bjects.         
-00025630: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
-00025640: 2020 2020 2d20 6170 703a 6465 6d6f 2d61      - app:demo-a
-00025650: 7070 0a20 2020 2020 2020 2020 202d 2076  pp.          - v
-00025660: 6572 7369 6f6e 3a76 312e 302e 300a 2020  ersion:v1.0.0.  
-00025670: 2020 2020 2020 2020 6974 656d 733a 0a20          items:. 
-00025680: 2020 2020 2020 2020 2020 2074 7970 653a             type:
-00025690: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-000256a0: 2020 7469 746c 653a 204c 6162 656c 730a    title: Labels.
-000256b0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-000256c0: 6172 7261 790a 2020 2020 2020 2020 616e  array.        an
-000256d0: 6e6f 7461 7469 6f6e 733a 0a20 2020 2020  notations:.     
-000256e0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-000256f0: 3a20 416e 2075 6e73 7472 7563 7475 7265  : An unstructure
-00025700: 6420 6b65 7920 7661 6c75 6520 6d61 7020  d key value map 
-00025710: 7468 6174 2063 616e 2062 6520 7573 6564  that can be used
-00025720: 2074 6f20 6174 7461 6368 2061 7262 6974   to attach arbit
-00025730: 7261 7279 0a20 2020 2020 2020 2020 2020  rary.           
-00025740: 206d 6574 6164 6174 610a 2020 2020 2020   metadata.      
-00025750: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
-00025760: 2020 2020 2020 202d 2061 6e6e 6f74 6174         - annotat
-00025770: 696f 6e2d 6b65 7931 3a76 616c 310a 2020  ion-key1:val1.  
-00025780: 2020 2020 2020 2020 2d20 616e 6e6f 7461          - annota
-00025790: 7469 6f6e 2d6b 6579 323a 7661 6c32 0a20  tion-key2:val2. 
-000257a0: 2020 2020 2020 2020 2069 7465 6d73 3a0a           items:.
-000257b0: 2020 2020 2020 2020 2020 2020 7479 7065              type
-000257c0: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
-000257d0: 2020 2074 6974 6c65 3a20 416e 6e6f 7461     title: Annota
-000257e0: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
-000257f0: 7479 7065 3a20 6172 7261 790a 2020 2020  type: array.    
-00025800: 2020 2020 656e 6470 6f69 6e74 733a 0a20      endpoints:. 
-00025810: 2020 2020 2020 2020 2069 7465 6d73 3a0a           items:.
-00025820: 2020 2020 2020 2020 2020 2020 2472 6566              $ref
-00025830: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
-00025840: 7363 6865 6d61 732f 456e 6470 6f69 6e74  schemas/Endpoint
-00025850: 270a 2020 2020 2020 2020 2020 7469 746c  '.          titl
-00025860: 653a 2065 6e64 706f 696e 7473 0a20 2020  e: endpoints.   
-00025870: 2020 2020 2020 2074 7970 653a 2061 7272         type: arr
-00025880: 6179 0a20 2020 2020 2020 2073 656c 6563  ay.        selec
-00025890: 746f 723a 0a20 2020 2020 2020 2020 2064  tor:.          d
-000258a0: 6573 6372 6970 7469 6f6e 3a20 7c0a 2020  escription: |.  
-000258b0: 2020 2020 2020 2020 2020 416e 2061 7272            An arr
-000258c0: 6179 206f 6620 6c61 6265 6c20 7365 6c65  ay of label sele
-000258d0: 6374 6f72 2072 756c 652c 2074 6865 2072  ctor rule, the r
-000258e0: 756c 6520 6361 6e20 6569 7468 6572 2062  ule can either b
-000258f0: 6520 6120 6d61 7463 6820 6c61 6265 6c20  e a match label 
-00025900: 6f72 206d 6174 6368 2065 7870 7265 7373  or match express
-00025910: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00025920: 2072 6566 6572 7269 6e67 2074 6865 2065   referring the e
-00025930: 7861 6d70 6c65 2028 6669 7273 7420 6973  xample (first is
-00025940: 2061 206d 6174 6368 206c 6162 656c 2c20   a match label, 
-00025950: 7365 636f 6e64 2069 7320 6120 6d61 7463  second is a matc
-00025960: 6820 6578 7072 6573 7369 6f6e 290a 2020  h expression).  
-00025970: 2020 2020 2020 2020 6578 616d 706c 653a          example:
-00025980: 0a20 2020 2020 2020 2020 202d 2061 7070  .          - app
-00025990: 3a64 656d 6f2d 6170 700a 2020 2020 2020  :demo-app.      
-000259a0: 2020 2020 2d20 226b 6579 3a76 6572 7369      - "key:versi
-000259b0: 6f6e 2c20 6f70 6572 6174 6f72 3a49 6e2c  on, operator:In,
-000259c0: 2076 616c 7565 733a 5b76 312e 302e 302c   values:[v1.0.0,
-000259d0: 2076 312e 302e 315d 220a 2020 2020 2020   v1.0.1]".      
-000259e0: 2020 2020 6974 656d 733a 0a20 2020 2020      items:.     
-000259f0: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00025a00: 696e 670a 2020 2020 2020 2020 2020 7469  ing.          ti
-00025a10: 746c 653a 204c 6162 656c 5365 6c65 6374  tle: LabelSelect
-00025a20: 6f72 0a20 2020 2020 2020 2020 2074 7970  or.          typ
-00025a30: 653a 2061 7272 6179 0a20 2020 2020 2020  e: array.       
-00025a40: 206e 616d 6573 7061 6365 5f73 656c 6563   namespace_selec
-00025a50: 746f 723a 0a20 2020 2020 2020 2020 2024  tor:.          $
-00025a60: 7265 663a 2027 232f 636f 6d70 6f6e 656e  ref: '#/componen
-00025a70: 7473 2f73 6368 656d 6173 2f53 6572 7669  ts/schemas/Servi
-00025a80: 6365 4d6f 6e69 746f 725f 6e61 6d65 7370  ceMonitor_namesp
-00025a90: 6163 655f 7365 6c65 6374 6f72 270a 2020  ace_selector'.  
-00025aa0: 2020 2020 7265 7175 6972 6564 3a0a 2020      required:.  
-00025ab0: 2020 2020 2d20 6e61 6d65 0a20 2020 2020      - name.     
-00025ac0: 2074 6974 6c65 3a20 5365 7276 6963 654d   title: ServiceM
-00025ad0: 6f6e 6974 6f72 0a20 2020 2020 2074 7970  onitor.      typ
-00025ae0: 653a 206f 626a 6563 740a 2020 2020 456e  e: object.    En
-00025af0: 6470 6f69 6e74 3a0a 2020 2020 2020 6578  dpoint:.      ex
-00025b00: 616d 706c 653a 0a20 2020 2020 2020 2068  ample:.        h
-00025b10: 6f6e 6f72 5f6c 6162 656c 733a 2074 7275  onor_labels: tru
-00025b20: 650a 2020 2020 2020 2020 7061 7468 3a20  e.        path: 
-00025b30: 2f6d 6574 7269 6373 0a20 2020 2020 2020  /metrics.       
-00025b40: 2074 6172 6765 745f 706f 7274 3a20 3830   target_port: 80
-00025b50: 3830 0a20 2020 2020 2020 2072 656c 6162  80.        relab
-00025b60: 656c 696e 6773 3a0a 2020 2020 2020 2020  elings:.        
-00025b70: 2d20 7265 6765 783a 2028 2e2a 290a 2020  - regex: (.*).  
-00025b80: 2020 2020 2020 2020 736f 7572 6365 5f6c          source_l
-00025b90: 6162 656c 733a 0a20 2020 2020 2020 2020  abels:.         
-00025ba0: 202d 205f 5f6d 6574 615f 6b75 6265 726e   - __meta_kubern
-00025bb0: 6574 6573 5f70 6f64 5f6c 6162 656c 5f61  etes_pod_label_a
-00025bc0: 7070 5f6b 7562 6572 6e65 7465 735f 696f  pp_kubernetes_io
-00025bd0: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
-00025be0: 6163 7469 6f6e 3a20 7265 706c 6163 650a  action: replace.
-00025bf0: 2020 2020 2020 2020 2020 7365 7061 7261            separa
-00025c00: 746f 723a 203b 0a20 2020 2020 2020 2020  tor: ;.         
-00025c10: 2072 6570 6c61 6365 6d65 6e74 3a20 2431   replacement: $1
-00025c20: 0a20 2020 2020 2020 2020 2074 6172 6765  .          targe
-00025c30: 745f 6c61 6265 6c3a 205f 5f6d 6574 7269  t_label: __metri
-00025c40: 6373 5f70 6174 685f 5f0a 2020 2020 2020  cs_path__.      
-00025c50: 2020 2d20 7265 6765 783a 2028 2e2a 290a    - regex: (.*).
-00025c60: 2020 2020 2020 2020 2020 736f 7572 6365            source
-00025c70: 5f6c 6162 656c 733a 0a20 2020 2020 2020  _labels:.       
-00025c80: 2020 202d 205f 5f6d 6574 615f 6b75 6265     - __meta_kube
-00025c90: 726e 6574 6573 5f70 6f64 5f6c 6162 656c  rnetes_pod_label
-00025ca0: 5f61 7070 5f6b 7562 6572 6e65 7465 735f  _app_kubernetes_
-00025cb0: 696f 5f6e 616d 650a 2020 2020 2020 2020  io_name.        
-00025cc0: 2020 6163 7469 6f6e 3a20 7265 706c 6163    action: replac
-00025cd0: 650a 2020 2020 2020 2020 2020 7365 7061  e.          sepa
-00025ce0: 7261 746f 723a 203b 0a20 2020 2020 2020  rator: ;.       
-00025cf0: 2020 2072 6570 6c61 6365 6d65 6e74 3a20     replacement: 
-00025d00: 2431 0a20 2020 2020 2020 2020 2074 6172  $1.          tar
-00025d10: 6765 745f 6c61 6265 6c3a 205f 5f6d 6574  get_label: __met
-00025d20: 7269 6373 5f70 6174 685f 5f0a 2020 2020  rics_path__.    
-00025d30: 2020 2020 6d65 7472 6963 5f72 656c 6162      metric_relab
-00025d40: 656c 696e 6773 3a0a 2020 2020 2020 2020  elings:.        
-00025d50: 2d20 7265 6765 783a 2028 2e2a 290a 2020  - regex: (.*).  
-00025d60: 2020 2020 2020 2020 736f 7572 6365 5f6c          source_l
-00025d70: 6162 656c 733a 0a20 2020 2020 2020 2020  abels:.         
-00025d80: 202d 205f 5f6d 6574 615f 6b75 6265 726e   - __meta_kubern
-00025d90: 6574 6573 5f70 6f64 5f6c 6162 656c 5f61  etes_pod_label_a
-00025da0: 7070 5f6b 7562 6572 6e65 7465 735f 696f  pp_kubernetes_io
-00025db0: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
-00025dc0: 6163 7469 6f6e 3a20 7265 706c 6163 650a  action: replace.
-00025dd0: 2020 2020 2020 2020 2020 7365 7061 7261            separa
-00025de0: 746f 723a 203b 0a20 2020 2020 2020 2020  tor: ;.         
-00025df0: 2072 6570 6c61 6365 6d65 6e74 3a20 2431   replacement: $1
-00025e00: 0a20 2020 2020 2020 2020 2074 6172 6765  .          targe
-00025e10: 745f 6c61 6265 6c3a 205f 5f6d 6574 7269  t_label: __metri
-00025e20: 6373 5f70 6174 685f 5f0a 2020 2020 2020  cs_path__.      
-00025e30: 2020 2d20 7265 6765 783a 2028 2e2a 290a    - regex: (.*).
-00025e40: 2020 2020 2020 2020 2020 736f 7572 6365            source
-00025e50: 5f6c 6162 656c 733a 0a20 2020 2020 2020  _labels:.       
-00025e60: 2020 202d 205f 5f6d 6574 615f 6b75 6265     - __meta_kube
-00025e70: 726e 6574 6573 5f70 6f64 5f6c 6162 656c  rnetes_pod_label
-00025e80: 5f61 7070 5f6b 7562 6572 6e65 7465 735f  _app_kubernetes_
-00025e90: 696f 5f6e 616d 650a 2020 2020 2020 2020  io_name.        
-00025ea0: 2020 6163 7469 6f6e 3a20 7265 706c 6163    action: replac
-00025eb0: 650a 2020 2020 2020 2020 2020 7365 7061  e.          sepa
-00025ec0: 7261 746f 723a 203b 0a20 2020 2020 2020  rator: ;.       
-00025ed0: 2020 2072 6570 6c61 6365 6d65 6e74 3a20     replacement: 
-00025ee0: 2431 0a20 2020 2020 2020 2020 2074 6172  $1.          tar
-00025ef0: 6765 745f 6c61 6265 6c3a 205f 5f6d 6574  get_label: __met
-00025f00: 7269 6373 5f70 6174 685f 5f0a 2020 2020  rics_path__.    
-00025f10: 2020 2020 7363 6865 6d65 3a20 6874 7470      scheme: http
-00025f20: 0a20 2020 2020 2020 2070 6f72 743a 2038  .        port: 8
-00025f30: 3038 300a 2020 2020 2020 2020 686f 6e6f  080.        hono
-00025f40: 725f 7469 6d65 7374 616d 7073 3a20 7472  r_timestamps: tr
-00025f50: 7565 0a20 2020 2020 2020 2073 6372 6170  ue.        scrap
-00025f60: 655f 7469 6d65 6f75 743a 2031 3073 0a20  e_timeout: 10s. 
-00025f70: 2020 2020 2020 2069 6e74 6572 7661 6c3a         interval:
-00025f80: 2033 3073 0a20 2020 2020 2020 2070 6172   30s.        par
-00025f90: 616d 733a 0a20 2020 2020 2020 2020 206d  ams:.          m
-00025fa0: 6f64 756c 653a 0a20 2020 2020 2020 2020  odule:.         
-00025fb0: 202d 2068 7474 705f 3278 780a 2020 2020   - http_2xx.    
-00025fc0: 2020 7072 6f70 6572 7469 6573 3a0a 2020    properties:.  
-00025fd0: 2020 2020 2020 686f 6e6f 725f 6c61 6265        honor_labe
-00025fe0: 6c73 3a0a 2020 2020 2020 2020 2020 6465  ls:.          de
-00025ff0: 7363 7269 7074 696f 6e3a 2068 6f6e 6f72  scription: honor
-00026000: 4c61 6265 6c73 2063 686f 6f73 6573 2074  Labels chooses t
-00026010: 6865 206d 6574 7269 6327 7320 6c61 6265  he metric's labe
-00026020: 6c73 206f 6e20 636f 6c6c 6973 696f 6e73  ls on collisions
-00026030: 2077 6974 680a 2020 2020 2020 2020 2020   with.          
-00026040: 2020 7461 7267 6574 206c 6162 656c 732e    target labels.
-00026050: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-00026060: 6c65 3a20 7472 7565 0a20 2020 2020 2020  le: true.       
-00026070: 2020 2074 6974 6c65 3a20 686f 6e6f 725f     title: honor_
-00026080: 6c61 6265 6c73 0a20 2020 2020 2020 2020  labels.         
-00026090: 2074 7970 653a 2062 6f6f 6c65 616e 0a20   type: boolean. 
-000260a0: 2020 2020 2020 2069 6e74 6572 7661 6c3a         interval:
-000260b0: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
-000260c0: 6970 7469 6f6e 3a20 496e 7465 7276 616c  iption: Interval
-000260d0: 2061 7420 7768 6963 6820 6d65 7472 6963   at which metric
-000260e0: 7320 7368 6f75 6c64 2062 6520 7363 7261  s should be scra
-000260f0: 7065 640a 2020 2020 2020 2020 2020 6578  ped.          ex
-00026100: 616d 706c 653a 2033 3073 0a20 2020 2020  ample: 30s.     
-00026110: 2020 2020 2074 6974 6c65 3a20 696e 7465       title: inte
-00026120: 7276 616c 0a20 2020 2020 2020 2020 2074  rval.          t
-00026130: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
-00026140: 2020 2020 7363 7261 7065 5f74 696d 656f      scrape_timeo
-00026150: 7574 3a0a 2020 2020 2020 2020 2020 6465  ut:.          de
-00026160: 7363 7269 7074 696f 6e3a 2054 696d 656f  scription: Timeo
-00026170: 7574 2061 6674 6572 2077 6869 6368 2074  ut after which t
-00026180: 6865 2073 6372 6170 6520 6973 2065 6e64  he scrape is end
-00026190: 6564 0a20 2020 2020 2020 2020 2065 7861  ed.          exa
-000261a0: 6d70 6c65 3a20 3130 730a 2020 2020 2020  mple: 10s.      
-000261b0: 2020 2020 7469 746c 653a 2073 6372 6170      title: scrap
-000261c0: 655f 7469 6d65 6f75 740a 2020 2020 2020  e_timeout.      
-000261d0: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-000261e0: 0a20 2020 2020 2020 2070 6174 683a 0a20  .        path:. 
-000261f0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00026200: 7469 6f6e 3a20 4854 5450 2070 6174 6820  tion: HTTP path 
-00026210: 746f 2073 6372 6170 6520 666f 7220 6d65  to scrape for me
-00026220: 7472 6963 732e 0a20 2020 2020 2020 2020  trics..         
-00026230: 2065 7861 6d70 6c65 3a20 2f6d 6574 7269   example: /metri
-00026240: 6373 0a20 2020 2020 2020 2020 2074 6974  cs.          tit
-00026250: 6c65 3a20 7061 7468 0a20 2020 2020 2020  le: path.       
-00026260: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
-00026270: 2020 2020 2020 2020 7363 6865 6d65 3a0a          scheme:.
-00026280: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00026290: 7074 696f 6e3a 2048 5454 5020 7363 6865  ption: HTTP sche
-000262a0: 6d65 2074 6f20 7573 6520 666f 7220 7363  me to use for sc
-000262b0: 7261 7069 6e67 2e0a 2020 2020 2020 2020  raping..        
-000262c0: 2020 6578 616d 706c 653a 2068 7474 700a    example: http.
-000262d0: 2020 2020 2020 2020 2020 7469 746c 653a            title:
-000262e0: 2073 6368 656d 650a 2020 2020 2020 2020   scheme.        
-000262f0: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00026300: 2020 2020 2020 2074 6172 6765 745f 706f         target_po
-00026310: 7274 3a0a 2020 2020 2020 2020 2020 6465  rt:.          de
-00026320: 7363 7269 7074 696f 6e3a 2022 4e75 6d62  scription: "Numb
-00026330: 6572 206f 6620 7468 6520 7461 7267 6574  er of the target
-00026340: 2070 6f72 7420 6f66 2074 6865 2050 6f64   port of the Pod
-00026350: 2062 6568 696e 6420 7468 6520 5365 7276   behind the Serv
-00026360: 6963 652c 2074 6865 5c0a 2020 2020 2020  ice, the\.      
-00026370: 2020 2020 2020 5c20 706f 7274 206d 7573        \ port mus
-00026380: 7420 6265 2073 7065 6369 6669 6564 2077  t be specified w
-00026390: 6974 6820 636f 6e74 6169 6e65 7220 706f  ith container po
-000263a0: 7274 2070 726f 7065 7274 792e 204d 7574  rt property. Mut
-000263b0: 7561 6c6c 7920 6578 636c 7573 6976 655c  ually exclusive\
-000263c0: 0a20 2020 2020 2020 2020 2020 205c 2077  .            \ w
-000263d0: 6974 6820 706f 7274 2e22 0a20 2020 2020  ith port.".     
-000263e0: 2020 2020 2065 7861 6d70 6c65 3a20 3830       example: 80
-000263f0: 3830 0a20 2020 2020 2020 2020 2074 6974  80.          tit
-00026400: 6c65 3a20 7461 7267 6574 5f70 6f72 740a  le: target_port.
-00026410: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-00026420: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
-00026430: 7061 7261 6d73 3a0a 2020 2020 2020 2020  params:.        
-00026440: 2020 6164 6469 7469 6f6e 616c 5072 6f70    additionalProp
-00026450: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
-00026460: 2020 2020 6974 656d 733a 0a20 2020 2020      items:.     
-00026470: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-00026480: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-00026490: 2020 7479 7065 3a20 6172 7261 790a 2020    type: array.  
-000264a0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-000264b0: 696f 6e3a 2050 6172 616d 7320 6973 2061  ion: Params is a
-000264c0: 2073 6574 206f 6620 5552 4c20 7061 7261   set of URL para
-000264d0: 6d65 7465 7273 2074 6f20 6265 2061 7070  meters to be app
-000264e0: 656e 6465 6420 746f 2074 6865 2073 6372  ended to the scr
-000264f0: 6170 650a 2020 2020 2020 2020 2020 2020  ape.            
-00026500: 5552 4c20 6265 666f 7265 2073 6372 6170  URL before scrap
-00026510: 696e 672e 0a20 2020 2020 2020 2020 2065  ing..          e
-00026520: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
-00026530: 2020 2020 6d6f 6475 6c65 3a0a 2020 2020      module:.    
-00026540: 2020 2020 2020 2020 2d20 6874 7470 5f32          - http_2
-00026550: 7878 0a20 2020 2020 2020 2020 2074 6974  xx.          tit
-00026560: 6c65 3a20 7061 7261 6d73 0a20 2020 2020  le: params.     
-00026570: 2020 2020 2074 7970 653a 206f 626a 6563       type: objec
-00026580: 740a 2020 2020 2020 2020 7265 6c61 6265  t.        relabe
-00026590: 6c69 6e67 733a 0a20 2020 2020 2020 2020  lings:.         
-000265a0: 2069 7465 6d73 3a0a 2020 2020 2020 2020   items:.        
-000265b0: 2020 2020 2472 6566 3a20 2723 2f63 6f6d      $ref: '#/com
-000265c0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-000265d0: 5265 6c61 6265 6c43 6f6e 6669 6727 0a20  RelabelConfig'. 
-000265e0: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-000265f0: 7265 6c61 6265 6c69 6e67 730a 2020 2020  relabelings.    
-00026600: 2020 2020 2020 7479 7065 3a20 6172 7261        type: arra
-00026610: 790a 2020 2020 2020 2020 706f 7274 3a0a  y.        port:.
-00026620: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00026630: 7074 696f 6e3a 204e 616d 6520 6f66 2074  ption: Name of t
-00026640: 6865 2073 6572 7669 6365 2070 6f72 7420  he service port 
-00026650: 7468 6973 2065 6e64 706f 696e 7420 7265  this endpoint re
-00026660: 6665 7273 2074 6f2e 204d 7574 7561 6c6c  fers to. Mutuall
-00026670: 790a 2020 2020 2020 2020 2020 2020 6578  y.            ex
-00026680: 636c 7573 6976 6520 7769 7468 2074 6172  clusive with tar
-00026690: 6765 7450 6f72 742e 0a20 2020 2020 2020  getPort..       
-000266a0: 2020 2065 7861 6d70 6c65 3a20 3830 3830     example: 8080
-000266b0: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
-000266c0: 3a20 706f 7274 0a20 2020 2020 2020 2020  : port.         
-000266d0: 2074 7970 653a 2069 6e74 6567 6572 0a20   type: integer. 
-000266e0: 2020 2020 2020 2068 6f6e 6f72 5f74 696d         honor_tim
-000266f0: 6573 7461 6d70 733a 0a20 2020 2020 2020  estamps:.       
-00026700: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-00026710: 686f 6e6f 7254 696d 6573 7461 6d70 7320  honorTimestamps 
-00026720: 636f 6e74 726f 6c73 2077 6865 7468 6572  controls whether
-00026730: 2050 726f 6d65 7468 6575 7320 7265 7370   Prometheus resp
-00026740: 6563 7473 2074 6865 2074 696d 6573 7461  ects the timesta
-00026750: 6d70 730a 2020 2020 2020 2020 2020 2020  mps.            
-00026760: 7072 6573 656e 7420 696e 2073 6372 6170  present in scrap
-00026770: 6564 2064 6174 612e 0a20 2020 2020 2020  ed data..       
-00026780: 2020 2065 7861 6d70 6c65 3a20 7472 7565     example: true
-00026790: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
-000267a0: 3a20 686f 6e6f 725f 7469 6d65 7374 616d  : honor_timestam
-000267b0: 7073 0a20 2020 2020 2020 2020 2074 7970  ps.          typ
-000267c0: 653a 2062 6f6f 6c65 616e 0a20 2020 2020  e: boolean.     
-000267d0: 2020 206d 6574 7269 635f 7265 6c61 6265     metric_relabe
-000267e0: 6c69 6e67 733a 0a20 2020 2020 2020 2020  lings:.         
-000267f0: 2069 7465 6d73 3a0a 2020 2020 2020 2020   items:.        
-00026800: 2020 2020 2472 6566 3a20 2723 2f63 6f6d      $ref: '#/com
-00026810: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00026820: 5265 6c61 6265 6c43 6f6e 6669 6727 0a20  RelabelConfig'. 
-00026830: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-00026840: 6d65 7472 6963 5f72 656c 6162 656c 696e  metric_relabelin
-00026850: 6773 0a20 2020 2020 2020 2020 2074 7970  gs.          typ
-00026860: 653a 2061 7272 6179 0a20 2020 2020 2074  e: array.      t
-00026870: 6974 6c65 3a20 456e 6470 6f69 6e74 0a20  itle: Endpoint. 
-00026880: 2020 2020 2074 7970 653a 206f 626a 6563       type: objec
-00026890: 740a 2020 2020 5265 6c61 6265 6c43 6f6e  t.    RelabelCon
-000268a0: 6669 673a 0a20 2020 2020 2065 7861 6d70  fig:.      examp
-000268b0: 6c65 3a0a 2020 2020 2020 2020 7265 6765  le:.        rege
-000268c0: 783a 2028 2e2a 290a 2020 2020 2020 2020  x: (.*).        
-000268d0: 736f 7572 6365 5f6c 6162 656c 733a 0a20  source_labels:. 
-000268e0: 2020 2020 2020 202d 205f 5f6d 6574 615f         - __meta_
-000268f0: 6b75 6265 726e 6574 6573 5f70 6f64 5f6c  kubernetes_pod_l
-00026900: 6162 656c 5f61 7070 5f6b 7562 6572 6e65  abel_app_kuberne
-00026910: 7465 735f 696f 5f6e 616d 650a 2020 2020  tes_io_name.    
-00026920: 2020 2020 6163 7469 6f6e 3a20 7265 706c      action: repl
-00026930: 6163 650a 2020 2020 2020 2020 7365 7061  ace.        sepa
-00026940: 7261 746f 723a 203b 0a20 2020 2020 2020  rator: ;.       
-00026950: 2072 6570 6c61 6365 6d65 6e74 3a20 2431   replacement: $1
-00026960: 0a20 2020 2020 2020 2074 6172 6765 745f  .        target_
-00026970: 6c61 6265 6c3a 205f 5f6d 6574 7269 6373  label: __metrics
-00026980: 5f70 6174 685f 5f0a 2020 2020 2020 7072  _path__.      pr
-00026990: 6f70 6572 7469 6573 3a0a 2020 2020 2020  operties:.      
-000269a0: 2020 736f 7572 6365 5f6c 6162 656c 733a    source_labels:
-000269b0: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
-000269c0: 6970 7469 6f6e 3a20 536f 7572 6365 4c61  iption: SourceLa
-000269d0: 6265 6c73 2073 656c 6563 7473 206c 6162  bels selects lab
-000269e0: 656c 7320 6672 6f6d 2074 6865 2073 6f75  els from the sou
-000269f0: 7263 650a 2020 2020 2020 2020 2020 6578  rce.          ex
-00026a00: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
-00026a10: 202d 205f 5f6d 6574 615f 6b75 6265 726e   - __meta_kubern
-00026a20: 6574 6573 5f70 6f64 5f6c 6162 656c 5f61  etes_pod_label_a
-00026a30: 7070 5f6b 7562 6572 6e65 7465 735f 696f  pp_kubernetes_io
-00026a40: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
-00026a50: 6974 656d 733a 0a20 2020 2020 2020 2020  items:.         
-00026a60: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
-00026a70: 2020 2020 2020 2020 2020 7469 746c 653a            title:
-00026a80: 2073 6f75 7263 655f 6c61 6265 6c73 0a20   source_labels. 
-00026a90: 2020 2020 2020 2020 2074 7970 653a 2061           type: a
-00026aa0: 7272 6179 0a20 2020 2020 2020 2073 6570  rray.        sep
-00026ab0: 6172 6174 6f72 3a0a 2020 2020 2020 2020  arator:.        
-00026ac0: 2020 6465 7363 7269 7074 696f 6e3a 2053    description: S
-00026ad0: 6570 6172 6174 6f72 2070 6c61 6365 6420  eparator placed 
-00026ae0: 6265 7477 6565 6e20 636f 6e63 6174 656e  between concaten
-00026af0: 6174 6564 2073 6f75 7263 6520 6c61 6265  ated source labe
-00026b00: 6c73 2e0a 2020 2020 2020 2020 2020 6578  ls..          ex
-00026b10: 616d 706c 653a 203b 0a20 2020 2020 2020  ample: ;.       
-00026b20: 2020 2074 6974 6c65 3a20 7365 7061 7261     title: separa
-00026b30: 746f 720a 2020 2020 2020 2020 2020 7479  tor.          ty
-00026b40: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
-00026b50: 2020 2072 6567 6578 3a0a 2020 2020 2020     regex:.      
-00026b60: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00026b70: 2052 6567 756c 6172 2065 7870 7265 7373   Regular express
-00026b80: 696f 6e20 6167 6169 6e73 7420 7768 6963  ion against whic
-00026b90: 6820 7468 6520 6578 7472 6163 7465 6420  h the extracted 
-00026ba0: 7661 6c75 6520 6973 206d 6174 6368 6564  value is matched
-00026bb0: 2e0a 2020 2020 2020 2020 2020 2020 4465  ..            De
-00026bc0: 6661 756c 7420 6973 2028 2e2a 290a 2020  fault is (.*).  
-00026bd0: 2020 2020 2020 2020 6578 616d 706c 653a          example:
-00026be0: 2028 2e2a 290a 2020 2020 2020 2020 2020   (.*).          
-00026bf0: 7469 746c 653a 2072 6567 6578 0a20 2020  title: regex.   
-00026c00: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00026c10: 696e 670a 2020 2020 2020 2020 7265 706c  ing.        repl
-00026c20: 6163 656d 656e 743a 0a20 2020 2020 2020  acement:.       
-00026c30: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-00026c40: 5265 706c 6163 656d 656e 7420 7661 6c75  Replacement valu
-00026c50: 6520 6167 6169 6e73 7420 7768 6963 6820  e against which 
-00026c60: 6120 7265 6765 7820 7265 706c 6163 6520  a regex replace 
-00026c70: 6973 2070 6572 666f 726d 6564 0a20 2020  is performed.   
-00026c80: 2020 2020 2020 2020 2069 6620 7468 6520           if the 
-00026c90: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
-00026ca0: 6f6e 206d 6174 6368 6573 2e20 5265 6765  on matches. Rege
-00026cb0: 7820 6361 7074 7572 6520 6772 6f75 7073  x capture groups
-00026cc0: 2061 7265 2061 7661 696c 6162 6c65 2e0a   are available..
-00026cd0: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
-00026ce0: 653a 2024 310a 2020 2020 2020 2020 2020  e: $1.          
-00026cf0: 7469 746c 653a 2072 6570 6c61 6365 6d65  title: replaceme
-00026d00: 6e74 0a20 2020 2020 2020 2020 2074 7970  nt.          typ
-00026d10: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-00026d20: 2020 7461 7267 6574 5f6c 6162 656c 3a0a    target_label:.
-00026d30: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00026d40: 7074 696f 6e3a 204c 6162 656c 2074 6f20  ption: Label to 
-00026d50: 7768 6963 6820 7468 6520 7265 7375 6c74  which the result
-00026d60: 696e 6720 7661 6c75 6520 6973 2077 7269  ing value is wri
-00026d70: 7474 656e 2069 6e20 6120 7265 706c 6163  tten in a replac
-00026d80: 650a 2020 2020 2020 2020 2020 2020 6163  e.            ac
-00026d90: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
-00026da0: 6578 616d 706c 653a 205f 5f6d 6574 7269  example: __metri
-00026db0: 6373 5f70 6174 685f 5f0a 2020 2020 2020  cs_path__.      
-00026dc0: 2020 2020 7469 746c 653a 2074 6172 6765      title: targe
-00026dd0: 745f 6c61 6265 6c0a 2020 2020 2020 2020  t_label.        
-00026de0: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00026df0: 2020 2020 2020 2061 6374 696f 6e3a 0a20         action:. 
-00026e00: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00026e10: 7469 6f6e 3a20 4163 7469 6f6e 2074 6f20  tion: Action to 
-00026e20: 7065 7266 6f72 6d20 6261 7365 6420 6f6e  perform based on
-00026e30: 2072 6567 6578 206d 6174 6368 696e 672e   regex matching.
-00026e40: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-00026e50: 6c65 3a20 7265 706c 6163 650a 2020 2020  le: replace.    
-00026e60: 2020 2020 2020 7469 746c 653a 2061 6374        title: act
-00026e70: 696f 6e0a 2020 2020 2020 2020 2020 7479  ion.          ty
-00026e80: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
-00026e90: 2074 6974 6c65 3a20 5265 6c61 6265 6c43   title: RelabelC
-00026ea0: 6f6e 6669 670a 2020 2020 2020 7479 7065  onfig.      type
-00026eb0: 3a20 6f62 6a65 6374 0a20 2020 2044 6570  : object.    Dep
-00026ec0: 6c6f 7952 6573 6f75 7263 654f 7665 726c  loyResourceOverl
-00026ed0: 6179 733a 0a20 2020 2020 2061 6464 6974  ays:.      addit
-00026ee0: 696f 6e61 6c50 726f 7065 7274 6965 733a  ionalProperties:
-00026ef0: 0a20 2020 2020 2020 2024 7265 663a 2027  .        $ref: '
-00026f00: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-00026f10: 656d 6173 2f44 6570 6c6f 7952 6573 6f75  emas/DeployResou
-00026f20: 7263 6573 270a 2020 2020 2020 7479 7065  rces'.      type
-00026f30: 3a20 6f62 6a65 6374 0a20 2020 2044 6570  : object.    Dep
-00026f40: 6c6f 7950 6c61 7466 6f72 6d52 6573 6f75  loyPlatformResou
-00026f50: 7263 6573 3a0a 2020 2020 2020 6974 656d  rces:.      item
-00026f60: 733a 0a20 2020 2020 2020 2024 7265 663a  s:.        $ref:
-00026f70: 2027 232f 636f 6d70 6f6e 656e 7473 2f73   '#/components/s
-00026f80: 6368 656d 6173 2f44 6570 6c6f 7950 6c61  chemas/DeployPla
-00026f90: 7466 6f72 6d52 6573 6f75 7263 6527 0a20  tformResource'. 
-00026fa0: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
-00026fb0: 0a20 2020 2044 6570 6c6f 7950 6c61 7466  .    DeployPlatf
-00026fc0: 6f72 6d52 6573 6f75 7263 653a 0a20 2020  ormResource:.   
-00026fd0: 2020 2065 7861 6d70 6c65 3a0a 2020 2020     example:.    
-00026fe0: 2020 2020 706f 703a 2061 6d73 310a 2020      pop: ams1.  
-00026ff0: 2020 2020 2020 6370 755f 7265 7175 6573        cpu_reques
-00027000: 7465 643a 2031 3030 300a 2020 2020 2020  ted: 1000.      
-00027010: 2020 6370 755f 7573 6564 3a20 3530 300a    cpu_used: 500.
-00027020: 2020 2020 2020 2020 6370 755f 6c69 6d69          cpu_limi
-00027030: 743a 2032 3030 300a 2020 2020 2020 2020  t: 2000.        
-00027040: 6d65 6d6f 7279 5f75 7365 643a 2035 3030  memory_used: 500
-00027050: 300a 2020 2020 2020 2020 6d65 6d6f 7279  0.        memory
-00027060: 5f72 6571 7565 7374 6564 3a20 3130 3030  _requested: 1000
-00027070: 300a 2020 2020 2020 2020 706c 6174 666f  0.        platfo
-00027080: 726d 3a20 4247 450a 2020 2020 2020 2020  rm: BGE.        
-00027090: 7370 6163 653a 2067 7373 0a20 2020 2020  space: gss.     
-000270a0: 2020 2073 746f 7261 6765 5f72 6571 7565     storage_reque
-000270b0: 7374 6564 3a20 3130 0a20 2020 2020 2020  sted: 10.       
-000270c0: 2073 746f 7261 6765 5f75 7365 643a 2035   storage_used: 5
-000270d0: 0a20 2020 2020 2070 726f 7065 7274 6965  .      propertie
-000270e0: 733a 0a20 2020 2020 2020 2070 6c61 7466  s:.        platf
-000270f0: 6f72 6d3a 0a20 2020 2020 2020 2020 2064  orm:.          d
-00027100: 6573 6372 6970 7469 6f6e 3a20 4e61 6d65  escription: Name
-00027110: 206f 6620 7468 6520 6465 706c 6f79 2070   of the deploy p
-00027120: 6c61 7466 6f72 6d2e 0a20 2020 2020 2020  latform..       
-00027130: 2020 2065 7861 6d70 6c65 3a20 4247 450a     example: BGE.
-00027140: 2020 2020 2020 2020 2020 7469 746c 653a            title:
-00027150: 2070 6c61 7466 6f72 6d0a 2020 2020 2020   platform.      
-00027160: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-00027170: 0a20 2020 2020 2020 2070 6f70 3a0a 2020  .        pop:.  
-00027180: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00027190: 696f 6e3a 204e 616d 6520 6f66 2074 6865  ion: Name of the
-000271a0: 2070 6f70 2e0a 2020 2020 2020 2020 2020   pop..          
-000271b0: 6578 616d 706c 653a 2061 6d73 310a 2020  example: ams1.  
-000271c0: 2020 2020 2020 2020 7469 746c 653a 2070          title: p
-000271d0: 6f70 0a20 2020 2020 2020 2020 2074 7970  op.          typ
-000271e0: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-000271f0: 2020 7370 6163 653a 0a20 2020 2020 2020    space:.       
-00027200: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-00027210: 4e61 6d65 206f 6620 7468 6520 6465 706c  Name of the depl
-00027220: 6f79 2073 7061 6365 2e0a 2020 2020 2020  oy space..      
-00027230: 2020 2020 6578 616d 706c 653a 2067 7373      example: gss
-00027240: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
-00027250: 3a20 7370 6163 650a 2020 2020 2020 2020  : space.        
-00027260: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00027270: 2020 2020 2020 2063 7075 5f72 6571 7565         cpu_reque
-00027280: 7374 6564 3a0a 2020 2020 2020 2020 2020  sted:.          
-00027290: 6465 7363 7269 7074 696f 6e3a 2022 5468  description: "Th
-000272a0: 6520 4350 5520 5175 6f74 6120 7265 7175  e CPU Quota requ
-000272b0: 6573 7465 6420 666f 7220 7468 6520 6465  ested for the de
-000272c0: 706c 6f79 2073 7061 6365 2e20 5468 6520  ploy space. The 
-000272d0: 756e 6974 2069 735c 0a20 2020 2020 2020  unit is\.       
-000272e0: 2020 2020 205c 206d 696c 6963 7075 2c20       \ milicpu, 
-000272f0: 3120 636f 7265 2065 7175 616c 7320 3130  1 core equals 10
-00027300: 3030 2e22 0a20 2020 2020 2020 2020 2065  00.".          e
-00027310: 7861 6d70 6c65 3a20 3130 3030 0a20 2020  xample: 1000.   
-00027320: 2020 2020 2020 2074 6974 6c65 3a20 6370         title: cp
-00027330: 755f 7265 7175 6573 7465 640a 2020 2020  u_requested.    
-00027340: 2020 2020 2020 7479 7065 3a20 696e 7465        type: inte
-00027350: 6765 720a 2020 2020 2020 2020 6370 755f  ger.        cpu_
-00027360: 6c69 6d69 743a 0a20 2020 2020 2020 2020  limit:.         
-00027370: 2064 6573 6372 6970 7469 6f6e 3a20 2254   description: "T
-00027380: 6865 206d 6178 2070 6f73 7369 626c 7920  he max possibly 
-00027390: 4350 5520 7468 6174 2063 616e 2062 6520  CPU that can be 
-000273a0: 7574 696c 697a 6564 2062 7920 7468 6520  utilized by the 
-000273b0: 6465 706c 6f79 2073 7061 6365 2e5c 0a20  deploy space.\. 
-000273c0: 2020 2020 2020 2020 2020 205c 2054 6865             \ The
-000273d0: 2075 6e69 7420 6973 206d 696c 6963 7075   unit is milicpu
-000273e0: 2c20 3120 636f 7265 2065 7175 616c 7320  , 1 core equals 
-000273f0: 3130 3030 2e22 0a20 2020 2020 2020 2020  1000.".         
-00027400: 2065 7861 6d70 6c65 3a20 3230 3030 0a20   example: 2000. 
-00027410: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-00027420: 6370 755f 6c69 6d69 740a 2020 2020 2020  cpu_limit.      
-00027430: 2020 2020 7479 7065 3a20 696e 7465 6765      type: intege
-00027440: 720a 2020 2020 2020 2020 6370 755f 7573  r.        cpu_us
-00027450: 6564 3a0a 2020 2020 2020 2020 2020 6465  ed:.          de
-00027460: 7363 7269 7074 696f 6e3a 2022 5468 6520  scription: "The 
-00027470: 4350 5520 616d 6f75 6e74 2075 7365 6420  CPU amount used 
-00027480: 696e 2074 6865 2064 6570 6c6f 7920 7370  in the deploy sp
-00027490: 6163 652e 2054 6865 2075 6e69 7420 6973  ace. The unit is
-000274a0: 206d 696c 6963 7075 2c5c 0a20 2020 2020   milicpu,\.     
-000274b0: 2020 2020 2020 205c 2031 2063 6f72 6520         \ 1 core 
-000274c0: 6571 7561 6c73 2031 3030 302e 220a 2020  equals 1000.".  
-000274d0: 2020 2020 2020 2020 6578 616d 706c 653a          example:
-000274e0: 2035 3030 0a20 2020 2020 2020 2020 2074   500.          t
-000274f0: 6974 6c65 3a20 6370 755f 7573 6564 0a20  itle: cpu_used. 
-00027500: 2020 2020 2020 2020 2074 7970 653a 2069           type: i
-00027510: 6e74 6567 6572 0a20 2020 2020 2020 206d  nteger.        m
-00027520: 656d 6f72 795f 7265 7175 6573 7465 643a  emory_requested:
-00027530: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
-00027540: 6970 7469 6f6e 3a20 5468 6520 6d65 6d6f  iption: The memo
-00027550: 7279 2051 756f 7461 2072 6571 7565 7374  ry Quota request
-00027560: 6564 2066 6f72 2074 6865 2064 6570 6c6f  ed for the deplo
-00027570: 7920 7370 6163 652e 2054 6865 2075 6e69  y space. The uni
-00027580: 7420 6973 0a20 2020 2020 2020 2020 2020  t is.           
-00027590: 204d 422e 0a20 2020 2020 2020 2020 2065   MB..          e
-000275a0: 7861 6d70 6c65 3a20 3130 3030 300a 2020  xample: 10000.  
-000275b0: 2020 2020 2020 2020 7469 746c 653a 206d          title: m
-000275c0: 656d 6f72 795f 7265 7175 6573 7465 640a  emory_requested.
-000275d0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-000275e0: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
-000275f0: 6d65 6d6f 7279 5f75 7365 643a 0a20 2020  memory_used:.   
-00027600: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00027610: 6f6e 3a20 5468 6520 6d65 6d6f 7279 2061  on: The memory a
-00027620: 6d6f 756e 7420 7573 6564 2069 6e20 7468  mount used in th
-00027630: 6520 6465 706c 6f79 2073 7061 6365 2e20  e deploy space. 
-00027640: 5468 6520 756e 6974 2069 7320 4d42 2e0a  The unit is MB..
-00027650: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
-00027660: 653a 2035 3030 300a 2020 2020 2020 2020  e: 5000.        
-00027670: 2020 7469 746c 653a 206d 656d 6f72 795f    title: memory_
-00027680: 7573 6564 0a20 2020 2020 2020 2020 2074  used.          t
-00027690: 7970 653a 2069 6e74 6567 6572 0a20 2020  ype: integer.   
-000276a0: 2020 2020 2073 746f 7261 6765 5f72 6571       storage_req
-000276b0: 7565 7374 6564 3a0a 2020 2020 2020 2020  uested:.        
-000276c0: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
-000276d0: 6865 2073 746f 7261 6765 2051 756f 7461  he storage Quota
-000276e0: 2072 6571 7565 7374 6564 2066 6f72 2074   requested for t
-000276f0: 6865 2064 6570 6c6f 7920 7370 6163 652e  he deploy space.
-00027700: 2054 6865 2075 6e69 740a 2020 2020 2020   The unit.      
-00027710: 2020 2020 2020 6973 2047 422e 0a20 2020        is GB..   
-00027720: 2020 2020 2020 2065 7861 6d70 6c65 3a20         example: 
-00027730: 3130 0a20 2020 2020 2020 2020 2074 6974  10.          tit
-00027740: 6c65 3a20 7374 6f72 6167 655f 7265 7175  le: storage_requ
-00027750: 6573 7465 640a 2020 2020 2020 2020 2020  ested.          
-00027760: 7479 7065 3a20 696e 7465 6765 720a 2020  type: integer.  
-00027770: 2020 2020 2020 7374 6f72 6167 655f 7573        storage_us
-00027780: 6564 3a0a 2020 2020 2020 2020 2020 6465  ed:.          de
-00027790: 7363 7269 7074 696f 6e3a 2054 6865 2073  scription: The s
-000277a0: 746f 7261 6765 2061 6d6f 756e 7420 7573  torage amount us
-000277b0: 6564 2069 6e20 7468 6520 6465 706c 6f79  ed in the deploy
-000277c0: 2073 7061 6365 2e20 5468 6520 756e 6974   space. The unit
-000277d0: 2069 7320 4d42 2e0a 2020 2020 2020 2020   is MB..        
-000277e0: 2020 6578 616d 706c 653a 2035 0a20 2020    example: 5.   
-000277f0: 2020 2020 2020 2074 6974 6c65 3a20 7374         title: st
-00027800: 6f72 6167 655f 7573 6564 0a20 2020 2020  orage_used.     
-00027810: 2020 2020 2074 7970 653a 2069 6e74 6567       type: integ
-00027820: 6572 0a20 2020 2020 2074 6974 6c65 3a20  er.      title: 
-00027830: 4465 706c 6f79 506c 6174 666f 726d 5265  DeployPlatformRe
-00027840: 736f 7572 6365 0a20 2020 2020 2074 7970  source.      typ
-00027850: 653a 206f 626a 6563 740a 2020 2020 5570  e: object.    Up
-00027860: 6461 7465 5374 7261 7465 6779 5f72 6f6c  dateStrategy_rol
-00027870: 6c69 6e67 5f75 7064 6174 655f 636f 6e66  ling_update_conf
-00027880: 6967 3a0a 2020 2020 2020 6578 616d 706c  ig:.      exampl
-00027890: 653a 0a20 2020 2020 2020 2070 6172 7469  e:.        parti
-000278a0: 7469 6f6e 3a20 320a 2020 2020 2020 2020  tion: 2.        
-000278b0: 6d61 785f 756e 6176 6169 6c61 626c 653a  max_unavailable:
-000278c0: 2031 3025 206f 7220 320a 2020 2020 2020   10% or 2.      
-000278d0: 2020 6d61 785f 7375 7267 653a 2031 3025    max_surge: 10%
-000278e0: 206f 7220 320a 2020 2020 2020 7072 6f70   or 2.      prop
-000278f0: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
-00027900: 6d61 785f 7375 7267 653a 0a20 2020 2020  max_surge:.     
-00027910: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-00027920: 3a20 2275 7365 6420 696e 2044 6570 6c6f  : "used in Deplo
-00027930: 796d 656e 742f 4461 656d 6f6e 5365 743b  yment/DaemonSet;
-00027940: 2054 6865 206d 6178 696d 756d 206e 756d   The maximum num
-00027950: 6265 7220 6f66 2070 6f64 7320 7468 6174  ber of pods that
-00027960: 5c0a 2020 2020 2020 2020 2020 2020 5c20  \.            \ 
-00027970: 6361 6e20 6265 2073 6368 6564 756c 6564  can be scheduled
-00027980: 2061 626f 7665 2074 6865 2064 6573 6972   above the desir
-00027990: 6564 206e 756d 6265 7220 6f66 2070 6f64  ed number of pod
-000279a0: 732e 2056 616c 7565 2063 616e 2062 6520  s. Value can be 
-000279b0: 616e 2061 6273 6f6c 7574 655c 0a20 2020  an absolute\.   
-000279c0: 2020 2020 2020 2020 205c 206e 756d 6265           \ numbe
-000279d0: 7220 2865 783a 2035 2920 6f72 2061 2070  r (ex: 5) or a p
-000279e0: 6572 6365 6e74 6167 6520 6f66 2064 6573  ercentage of des
-000279f0: 6972 6564 2070 6f64 7320 2865 783a 2031  ired pods (ex: 1
-00027a00: 3025 292e 220a 2020 2020 2020 2020 2020  0%).".          
-00027a10: 6578 616d 706c 653a 2031 3025 206f 7220  example: 10% or 
-00027a20: 320a 2020 2020 2020 2020 2020 7469 746c  2.          titl
-00027a30: 653a 206d 6178 5f73 7572 6765 0a20 2020  e: max_surge.   
-00027a40: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00027a50: 696e 670a 2020 2020 2020 2020 6d61 785f  ing.        max_
-00027a60: 756e 6176 6169 6c61 626c 653a 0a20 2020  unavailable:.   
-00027a70: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00027a80: 6f6e 3a20 2275 7365 6420 696e 2044 6570  on: "used in Dep
-00027a90: 6c6f 796d 656e 742f 4461 656d 6f6e 5365  loyment/DaemonSe
-00027aa0: 742f 5374 6174 6566 756c 5365 743b 2054  t/StatefulSet; T
-00027ab0: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
-00027ac0: 725c 0a20 2020 2020 2020 2020 2020 205c  r\.            \
-00027ad0: 206f 6620 706f 6473 2074 6861 7420 6361   of pods that ca
-00027ae0: 6e20 6265 2075 6e61 7661 696c 6162 6c65  n be unavailable
-00027af0: 2064 7572 696e 6720 7468 6520 7570 6461   during the upda
-00027b00: 7465 3b20 5661 6c75 6520 6361 6e20 6265  te; Value can be
-00027b10: 2061 6e20 6162 736f 6c75 7465 5c0a 2020   an absolute\.  
-00027b20: 2020 2020 2020 2020 2020 5c20 6e75 6d62            \ numb
-00027b30: 6572 2028 6578 3a20 3529 206f 7220 6120  er (ex: 5) or a 
-00027b40: 7065 7263 656e 7461 6765 206f 6620 6465  percentage of de
-00027b50: 7369 7265 6420 706f 6473 2028 6578 3a20  sired pods (ex: 
-00027b60: 3130 2529 2e22 0a20 2020 2020 2020 2020  10%).".         
-00027b70: 2065 7861 6d70 6c65 3a20 3130 2520 6f72   example: 10% or
-00027b80: 2032 0a20 2020 2020 2020 2020 2074 6974   2.          tit
-00027b90: 6c65 3a20 6d61 785f 756e 6176 6169 6c61  le: max_unavaila
-00027ba0: 626c 650a 2020 2020 2020 2020 2020 7479  ble.          ty
-00027bb0: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
-00027bc0: 2020 2070 6172 7469 7469 6f6e 3a0a 2020     partition:.  
-00027bd0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00027be0: 696f 6e3a 2022 7573 6564 2069 6e20 5374  ion: "used in St
-00027bf0: 6174 6566 756c 5365 743b 2050 6172 7469  atefulSet; Parti
-00027c00: 7469 6f6e 2069 6e64 6963 6174 6573 2074  tion indicates t
-00027c10: 6865 206f 7264 696e 616c 2061 7420 7768  he ordinal at wh
-00027c20: 6963 685c 0a20 2020 2020 2020 2020 2020  ich\.           
-00027c30: 205c 2074 6865 2057 6f72 6b6c 6f61 6420   \ the Workload 
-00027c40: 7368 6f75 6c64 2062 6520 7061 7274 6974  should be partit
-00027c50: 696f 6e65 6420 666f 7220 7570 6461 7465  ioned for update
-00027c60: 732e 2044 7572 696e 6720 6120 726f 6c6c  s. During a roll
-00027c70: 696e 6720 7570 6461 7465 2c5c 0a20 2020  ing update,\.   
-00027c80: 2020 2020 2020 2020 205c 2061 6c6c 2070           \ all p
-00027c90: 6f64 7320 6672 6f6d 206f 7264 696e 616c  ods from ordinal
-00027ca0: 2050 6172 7469 7469 6f6e 2d31 2074 6f20   Partition-1 to 
-00027cb0: 5265 706c 6963 6120 6172 6520 7570 6461  Replica are upda
-00027cc0: 7465 642e 2041 6c6c 2070 6f64 7320 6672  ted. All pods fr
-00027cd0: 6f6d 5c0a 2020 2020 2020 2020 2020 2020  om\.            
-00027ce0: 5c20 6f72 6469 6e61 6c20 5061 7274 6974  \ ordinal Partit
-00027cf0: 696f 6e2d 3120 746f 2030 2072 656d 6169  ion-1 to 0 remai
-00027d00: 6e20 756e 746f 7563 6865 642e 2022 0a20  n untouched. ". 
-00027d10: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
-00027d20: 3a20 320a 2020 2020 2020 2020 2020 7469  : 2.          ti
-00027d30: 746c 653a 2070 6172 7469 7469 6f6e 0a20  tle: partition. 
-00027d40: 2020 2020 2020 2020 2074 7970 653a 2069           type: i
-00027d50: 6e74 6567 6572 0a20 2020 2020 2074 6974  nteger.      tit
-00027d60: 6c65 3a20 5570 6461 7465 5374 7261 7465  le: UpdateStrate
-00027d70: 6779 5f72 6f6c 6c69 6e67 5f75 7064 6174  gy_rolling_updat
-00027d80: 655f 636f 6e66 6967 0a20 2020 2020 2074  e_config.      t
-00027d90: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
-00027da0: 436f 6e74 6169 6e65 7253 6563 436f 6e74  ContainerSecCont
-00027db0: 6578 745f 6361 7061 6269 6c69 7469 6573  ext_capabilities
-00027dc0: 3a0a 2020 2020 2020 6465 7363 7269 7074  :.      descript
-00027dd0: 696f 6e3a 2054 6865 2050 4f53 4958 2063  ion: The POSIX c
-00027de0: 6170 6162 696c 6974 6965 7320 746f 2061  apabilities to a
-00027df0: 6464 2f64 726f 7020 7768 656e 2072 756e  dd/drop when run
-00027e00: 6e69 6e67 2063 6f6e 7461 696e 6572 732e  ning containers.
-00027e10: 0a20 2020 2020 2065 7861 6d70 6c65 3a0a  .      example:.
-00027e20: 2020 2020 2020 2020 6164 643a 0a20 2020          add:.   
-00027e30: 2020 2020 202d 204e 4554 5f41 444d 494e       - NET_ADMIN
-00027e40: 0a20 2020 2020 2020 202d 2053 5953 5f54  .        - SYS_T
-00027e50: 494d 450a 2020 2020 2020 2020 6472 6f70  IME.        drop
-00027e60: 3a0a 2020 2020 2020 2020 2d20 4e45 545f  :.        - NET_
-00027e70: 4144 4d49 4e0a 2020 2020 2020 2020 2d20  ADMIN.        - 
-00027e80: 5359 535f 5449 4d45 0a20 2020 2020 2070  SYS_TIME.      p
-00027e90: 726f 7065 7274 6965 733a 0a20 2020 2020  roperties:.     
-00027ea0: 2020 2061 6464 3a0a 2020 2020 2020 2020     add:.        
-00027eb0: 2020 6465 7363 7269 7074 696f 6e3a 2041    description: A
-00027ec0: 6464 6564 2063 6170 6162 696c 6974 6965  dded capabilitie
-00027ed0: 732e 0a20 2020 2020 2020 2020 2065 7861  s..          exa
-00027ee0: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
-00027ef0: 2d20 4e45 545f 4144 4d49 4e0a 2020 2020  - NET_ADMIN.    
-00027f00: 2020 2020 2020 2d20 5359 535f 5449 4d45        - SYS_TIME
-00027f10: 0a20 2020 2020 2020 2020 2069 7465 6d73  .          items
-00027f20: 3a0a 2020 2020 2020 2020 2020 2020 7479  :.            ty
-00027f30: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
-00027f40: 2020 2020 2074 6974 6c65 3a20 6164 640a       title: add.
-00027f50: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-00027f60: 6172 7261 790a 2020 2020 2020 2020 6472  array.        dr
-00027f70: 6f70 3a0a 2020 2020 2020 2020 2020 6465  op:.          de
-00027f80: 7363 7269 7074 696f 6e3a 2052 656d 6f76  scription: Remov
-00027f90: 6564 2063 6170 6162 696c 6974 6965 732e  ed capabilities.
-00027fa0: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-00027fb0: 6c65 3a0a 2020 2020 2020 2020 2020 2d20  le:.          - 
-00027fc0: 4e45 545f 4144 4d49 4e0a 2020 2020 2020  NET_ADMIN.      
-00027fd0: 2020 2020 2d20 5359 535f 5449 4d45 0a20      - SYS_TIME. 
-00027fe0: 2020 2020 2020 2020 2069 7465 6d73 3a0a           items:.
-00027ff0: 2020 2020 2020 2020 2020 2020 7479 7065              type
-00028000: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
-00028010: 2020 2074 6974 6c65 3a20 6472 6f70 0a20     title: drop. 
-00028020: 2020 2020 2020 2020 2074 7970 653a 2061           type: a
-00028030: 7272 6179 0a20 2020 2020 2074 6974 6c65  rray.      title
-00028040: 3a20 436f 6e74 6169 6e65 7253 6563 436f  : ContainerSecCo
-00028050: 6e74 6578 745f 6361 7061 6269 6c69 7469  ntext_capabiliti
-00028060: 6573 0a20 2020 2020 2074 7970 653a 206f  es.      type: o
-00028070: 626a 6563 740a 2020 2020 566f 6c75 6d65  bject.    Volume
-00028080: 5f70 6572 7369 7374 656e 745f 766f 6c75  _persistent_volu
-00028090: 6d65 5f63 6c61 696d 3a0a 2020 2020 2020  me_claim:.      
-000280a0: 6465 7363 7269 7074 696f 6e3a 207c 0a20  description: |. 
-000280b0: 2020 2020 2020 2052 6570 7265 7365 6e74         Represent
-000280c0: 7320 6120 7265 6665 7265 6e63 6520 746f  s a reference to
-000280d0: 2061 2050 6572 7369 7374 656e 7456 6f6c   a PersistentVol
-000280e0: 756d 6543 6c61 696d 2069 6e20 7468 6520  umeClaim in the 
-000280f0: 7361 6d65 206e 616d 6573 7061 6365 2e0a  same namespace..
-00028100: 2020 2020 2020 2020 5468 6973 2076 6f6c          This vol
-00028110: 756d 6520 6669 6e64 7320 7468 6520 626f  ume finds the bo
-00028120: 756e 6420 5056 2061 6e64 206d 6f75 6e74  und PV and mount
-00028130: 7320 7468 6174 2076 6f6c 756d 6520 666f  s that volume fo
-00028140: 7220 7468 6520 706f 642e 0a20 2020 2020  r the pod..     
-00028150: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
-00028160: 2020 7265 6164 5f6f 6e6c 793a 2066 616c    read_only: fal
-00028170: 7365 0a20 2020 2020 2020 2063 6c61 696d  se.        claim
-00028180: 5f6e 616d 653a 2064 656d 6f2d 7076 630a  _name: demo-pvc.
-00028190: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
-000281a0: 3a0a 2020 2020 2020 2020 636c 6169 6d5f  :.        claim_
-000281b0: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
-000281c0: 6465 7363 7269 7074 696f 6e3a 2043 6c61  description: Cla
-000281d0: 696d 4e61 6d65 2069 7320 7468 6520 6e61  imName is the na
-000281e0: 6d65 206f 6620 6120 5065 7273 6973 7465  me of a Persiste
-000281f0: 6e74 566f 6c75 6d65 436c 6169 6d20 696e  ntVolumeClaim in
-00028200: 2074 6865 2073 616d 650a 2020 2020 2020   the same.      
-00028210: 2020 2020 2020 6e61 6d65 7370 6163 6520        namespace 
-00028220: 6173 2074 6865 2070 6f64 2075 7369 6e67  as the pod using
-00028230: 2074 6869 7320 766f 6c75 6d65 0a20 2020   this volume.   
-00028240: 2020 2020 2020 2065 7861 6d70 6c65 3a20         example: 
-00028250: 6465 6d6f 2d70 7663 0a20 2020 2020 2020  demo-pvc.       
-00028260: 2020 2074 6974 6c65 3a20 636c 6169 6d5f     title: claim_
-00028270: 6e61 6d65 0a20 2020 2020 2020 2020 2074  name.          t
-00028280: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
-00028290: 2020 2020 7265 6164 5f6f 6e6c 793a 0a20      read_only:. 
-000282a0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-000282b0: 7469 6f6e 3a20 5769 6c6c 2066 6f72 6365  tion: Will force
-000282c0: 2074 6865 2052 6561 644f 6e6c 7920 7365   the ReadOnly se
-000282d0: 7474 696e 6720 696e 2056 6f6c 756d 654d  tting in VolumeM
-000282e0: 6f75 6e74 730a 2020 2020 2020 2020 2020  ounts.          
-000282f0: 6578 616d 706c 653a 2066 616c 7365 0a20  example: false. 
-00028300: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-00028310: 7265 6164 5f6f 6e6c 790a 2020 2020 2020  read_only.      
-00028320: 2020 2020 7479 7065 3a20 626f 6f6c 6561      type: boolea
-00028330: 6e0a 2020 2020 2020 7469 746c 653a 2056  n.      title: V
-00028340: 6f6c 756d 655f 7065 7273 6973 7465 6e74  olume_persistent
-00028350: 5f76 6f6c 756d 655f 636c 6169 6d0a 2020  _volume_claim.  
-00028360: 2020 2020 7479 7065 3a20 6f62 6a65 6374      type: object
-00028370: 0a20 2020 2056 6f6c 756d 655f 656d 7074  .    Volume_empt
-00028380: 795f 6469 723a 0a20 2020 2020 2064 6573  y_dir:.      des
-00028390: 6372 6970 7469 6f6e 3a20 5265 7072 6573  cription: Repres
-000283a0: 656e 7473 2061 2074 656d 706f 7261 7279  ents a temporary
-000283b0: 2064 6972 6563 746f 7279 2074 6861 7420   directory that 
-000283c0: 7368 6172 6573 2061 2070 6f64 2773 206c  shares a pod's l
-000283d0: 6966 6574 696d 650a 2020 2020 2020 6578  ifetime.      ex
-000283e0: 616d 706c 653a 0a20 2020 2020 2020 206d  ample:.        m
-000283f0: 6564 6975 6d3a 204d 656d 6f72 790a 2020  edium: Memory.  
-00028400: 2020 2020 2020 7369 7a65 5f6c 696d 6974        size_limit
-00028410: 3a20 3530 304d 690a 2020 2020 2020 7072  : 500Mi.      pr
-00028420: 6f70 6572 7469 6573 3a0a 2020 2020 2020  operties:.      
-00028430: 2020 6d65 6469 756d 3a0a 2020 2020 2020    medium:.      
-00028440: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00028450: 2052 6570 7265 7365 6e74 7320 7768 6174   Represents what
-00028460: 2074 7970 6520 6f66 2073 746f 7261 6765   type of storage
-00028470: 206d 6564 6975 6d20 7368 6f75 6c64 2062   medium should b
-00028480: 6163 6b20 7468 6973 2064 6972 6563 746f  ack this directo
-00028490: 7279 2e0a 2020 2020 2020 2020 2020 2020  ry..            
-000284a0: 5468 6520 6465 6661 756c 7420 6973 2022  The default is "
-000284b0: 2220 7768 6963 6820 6d65 616e 7320 746f  " which means to
-000284c0: 2075 7365 2074 6865 206e 6f64 6527 7320   use the node's 
-000284d0: 6465 6661 756c 7420 6d65 6469 756d 2e0a  default medium..
-000284e0: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
-000284f0: 653a 204d 656d 6f72 790a 2020 2020 2020  e: Memory.      
-00028500: 2020 2020 7469 746c 653a 206d 6564 6975      title: mediu
-00028510: 6d0a 2020 2020 2020 2020 2020 7479 7065  m.          type
-00028520: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
-00028530: 2073 697a 655f 6c69 6d69 743a 0a20 2020   size_limit:.   
-00028540: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00028550: 6f6e 3a20 5468 6520 746f 7461 6c20 616d  on: The total am
-00028560: 6f75 6e74 206f 6620 6c6f 6361 6c20 7374  ount of local st
-00028570: 6f72 6167 6520 7265 7175 6972 6564 2066  orage required f
-00028580: 6f72 2074 6869 7320 456d 7074 7944 6972  or this EmptyDir
-00028590: 0a20 2020 2020 2020 2020 2020 2076 6f6c  .            vol
-000285a0: 756d 652e 0a20 2020 2020 2020 2020 2065  ume..          e
-000285b0: 7861 6d70 6c65 3a20 3530 304d 690a 2020  xample: 500Mi.  
-000285c0: 2020 2020 2020 2020 7469 746c 653a 2073          title: s
-000285d0: 697a 655f 6c69 6d69 740a 2020 2020 2020  ize_limit.      
-000285e0: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-000285f0: 0a20 2020 2020 2074 6974 6c65 3a20 566f  .      title: Vo
-00028600: 6c75 6d65 5f65 6d70 7479 5f64 6972 0a20  lume_empty_dir. 
-00028610: 2020 2020 2074 7970 653a 206f 626a 6563       type: objec
-00028620: 740a 2020 2020 566f 6c75 6d65 5f68 6f73  t.    Volume_hos
-00028630: 745f 7061 7468 3a0a 2020 2020 2020 6465  t_path:.      de
-00028640: 7363 7269 7074 696f 6e3a 207c 0a20 2020  scription: |.   
-00028650: 2020 2020 2072 6570 7265 7365 6e74 7320       represents 
-00028660: 6120 7072 652d 6578 6973 7469 6e67 2066  a pre-existing f
-00028670: 696c 6520 6f72 2064 6972 6563 746f 7279  ile or directory
-00028680: 206f 6e20 7468 6520 686f 7374 206d 6163   on the host mac
-00028690: 6869 6e65 2074 6861 7420 6973 2064 6972  hine that is dir
-000286a0: 6563 746c 7920 6578 706f 7365 6420 746f  ectly exposed to
-000286b0: 2074 6865 2063 6f6e 7461 696e 6572 2e0a   the container..
-000286c0: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
-000286d0: 6765 6e65 7261 6c6c 7920 7573 6564 2066  generally used f
-000286e0: 6f72 2073 7973 7465 6d20 6167 656e 7473  or system agents
-000286f0: 206f 7220 6f74 6865 7220 7072 6976 696c   or other privil
-00028700: 6567 6564 2074 6869 6e67 7320 7468 6174  eged things that
-00028710: 2061 7265 2061 6c6c 6f77 6564 2074 6f20   are allowed to 
-00028720: 7365 6520 7468 6520 686f 7374 206d 6163  see the host mac
-00028730: 6869 6e65 2e0a 2020 2020 2020 6578 616d  hine..      exam
-00028740: 706c 653a 0a20 2020 2020 2020 2070 6174  ple:.        pat
-00028750: 683a 202f 6461 7461 0a20 2020 2020 2020  h: /data.       
-00028760: 2070 6174 685f 7479 7065 3a20 4469 7265   path_type: Dire
-00028770: 6374 6f72 790a 2020 2020 2020 7072 6f70  ctory.      prop
-00028780: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
-00028790: 7061 7468 3a0a 2020 2020 2020 2020 2020  path:.          
-000287a0: 6465 7363 7269 7074 696f 6e3a 2022 5061  description: "Pa
-000287b0: 7468 206f 6620 7468 6520 6469 7265 6374  th of the direct
-000287c0: 6f72 7920 6f6e 2074 6865 2068 6f73 742e  ory on the host.
-000287d0: 2049 6620 7468 6520 7061 7468 2069 7320   If the path is 
-000287e0: 6120 7379 6d6c 696e 6b2c 5c0a 2020 2020  a symlink,\.    
-000287f0: 2020 2020 2020 2020 5c20 6974 2077 696c          \ it wil
-00028800: 6c20 666f 6c6c 6f77 2074 6865 206c 696e  l follow the lin
-00028810: 6b20 746f 2074 6865 2072 6561 6c20 7061  k to the real pa
-00028820: 7468 220a 2020 2020 2020 2020 2020 6578  th".          ex
-00028830: 616d 706c 653a 202f 6461 7461 0a20 2020  ample: /data.   
-00028840: 2020 2020 2020 2074 6974 6c65 3a20 7061         title: pa
-00028850: 7468 0a20 2020 2020 2020 2020 2074 7970  th.          typ
-00028860: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-00028870: 2020 7061 7468 5f74 7970 653a 0a20 2020    path_type:.   
-00028880: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00028890: 6f6e 3a20 5479 7065 2066 6f72 2048 6f73  on: Type for Hos
-000288a0: 7450 6174 6820 566f 6c75 6d65 2044 6566  tPath Volume Def
-000288b0: 6175 6c74 7320 746f 2022 220a 2020 2020  aults to "".    
-000288c0: 2020 2020 2020 6578 616d 706c 653a 2044        example: D
-000288d0: 6972 6563 746f 7279 0a20 2020 2020 2020  irectory.       
-000288e0: 2020 2074 6974 6c65 3a20 7061 7468 5f74     title: path_t
-000288f0: 7970 650a 2020 2020 2020 2020 2020 7479  ype.          ty
-00028900: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
-00028910: 2074 6974 6c65 3a20 566f 6c75 6d65 5f68   title: Volume_h
-00028920: 6f73 745f 7061 7468 0a20 2020 2020 2074  ost_path.      t
-00028930: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
-00028940: 436f 6e66 6967 5f74 656d 706c 6174 6573  Config_templates
-00028950: 5f69 6e6e 6572 3a0a 2020 2020 2020 6578  _inner:.      ex
-00028960: 616d 706c 653a 0a20 2020 2020 2020 2076  ample:.        v
-00028970: 616c 7565 733a 0a20 2020 2020 2020 2020  alues:.         
-00028980: 206b 6579 313a 2076 616c 7565 310a 2020   key1: value1.  
-00028990: 2020 2020 2020 6e61 6d65 3a20 636f 6e66        name: conf
-000289a0: 2f73 6572 7665 722e 636f 6e66 0a20 2020  /server.conf.   
-000289b0: 2020 2070 726f 7065 7274 6965 733a 0a20     properties:. 
-000289c0: 2020 2020 2020 206e 616d 653a 0a20 2020         name:.   
-000289d0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-000289e0: 6f6e 3a20 7468 6520 636f 6e66 6967 2066  on: the config f
-000289f0: 696c 6520 7061 7468 206e 616d 650a 2020  ile path name.  
-00028a00: 2020 2020 2020 2020 6578 616d 706c 653a          example:
-00028a10: 2063 6f6e 662f 7365 7276 6572 2e63 6f6e   conf/server.con
-00028a20: 660a 2020 2020 2020 2020 2020 7469 746c  f.          titl
-00028a30: 653a 206e 616d 650a 2020 2020 2020 2020  e: name.        
-00028a40: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00028a50: 2020 2020 2020 2076 616c 7565 733a 0a20         values:. 
-00028a60: 2020 2020 2020 2020 2061 6464 6974 696f           additio
-00028a70: 6e61 6c50 726f 7065 7274 6965 733a 0a20  nalProperties:. 
-00028a80: 2020 2020 2020 2020 2020 2074 7970 653a             type:
-00028a90: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-00028aa0: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
-00028ab0: 6865 2063 6f6e 6669 6720 7661 6c75 6573  he config values
-00028ac0: 2066 6f72 2074 6865 2074 656d 706c 6174   for the templat
-00028ad0: 6520 6669 6c65 0a20 2020 2020 2020 2020  e file.         
-00028ae0: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
-00028af0: 2020 2020 2020 6b65 7931 3a20 7661 6c75        key1: valu
-00028b00: 6531 0a20 2020 2020 2020 2020 2074 6974  e1.          tit
-00028b10: 6c65 3a20 7661 6c75 6573 0a20 2020 2020  le: values.     
-00028b20: 2020 2020 2074 7970 653a 206f 626a 6563       type: objec
-00028b30: 740a 2020 2020 2020 7469 746c 653a 2043  t.      title: C
-00028b40: 6f6e 6669 675f 7465 6d70 6c61 7465 735f  onfig_templates_
-00028b50: 696e 6e65 720a 2020 2020 2020 7479 7065  inner.      type
-00028b60: 3a20 6f62 6a65 6374 0a20 2020 2049 6e67  : object.    Ing
-00028b70: 7265 7373 4261 636b 656e 645f 7365 7276  ressBackend_serv
-00028b80: 6963 653a 0a20 2020 2020 2064 6573 6372  ice:.      descr
-00028b90: 6970 7469 6f6e 3a20 5265 6665 7265 6e63  iption: Referenc
-00028ba0: 6573 2061 2053 6572 7669 6365 2061 7320  es a Service as 
-00028bb0: 6120 4261 636b 656e 642e 0a20 2020 2020  a Backend..     
-00028bc0: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
-00028bd0: 2020 706f 7274 3a20 3830 0a20 2020 2020    port: 80.     
-00028be0: 2020 206e 616d 653a 2064 656d 6f2d 6170     name: demo-ap
-00028bf0: 702d 7365 7276 6963 650a 2020 2020 2020  p-service.      
-00028c00: 7072 6f70 6572 7469 6573 3a0a 2020 2020  properties:.    
-00028c10: 2020 2020 6e61 6d65 3a0a 2020 2020 2020      name:.      
-00028c20: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00028c30: 204e 616d 6520 6f66 2074 6865 2072 6566   Name of the ref
-00028c40: 6572 656e 6365 6420 7365 7276 6963 652e  erenced service.
-00028c50: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-00028c60: 6c65 3a20 6465 6d6f 2d61 7070 2d73 6572  le: demo-app-ser
-00028c70: 7669 6365 0a20 2020 2020 2020 2020 2074  vice.          t
-00028c80: 6974 6c65 3a20 6e61 6d65 0a20 2020 2020  itle: name.     
-00028c90: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-00028ca0: 670a 2020 2020 2020 2020 706f 7274 3a0a  g.        port:.
-00028cb0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00028cc0: 7074 696f 6e3a 2054 6865 206e 756d 6572  ption: The numer
-00028cd0: 6963 616c 2070 6f72 7420 6e75 6d62 6572  ical port number
-00028ce0: 206f 6e20 7468 6520 5365 7276 6963 652e   on the Service.
-00028cf0: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-00028d00: 6c65 3a20 3830 0a20 2020 2020 2020 2020  le: 80.         
-00028d10: 2074 6974 6c65 3a20 706f 7274 0a20 2020   title: port.   
-00028d20: 2020 2020 2020 2074 7970 653a 2069 6e74         type: int
-00028d30: 6567 6572 0a20 2020 2020 2074 6974 6c65  eger.      title
-00028d40: 3a20 496e 6772 6573 7342 6163 6b65 6e64  : IngressBackend
-00028d50: 5f73 6572 7669 6365 0a20 2020 2020 2074  _service.      t
-00028d60: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
-00028d70: 5365 7276 6963 654d 6f6e 6974 6f72 5f6e  ServiceMonitor_n
-00028d80: 616d 6573 7061 6365 5f73 656c 6563 746f  amespace_selecto
-00028d90: 723a 0a20 2020 2020 2065 7861 6d70 6c65  r:.      example
-00028da0: 3a0a 2020 2020 2020 2020 6d61 7463 685f  :.        match_
-00028db0: 6e61 6d65 733a 0a20 2020 2020 2020 202d  names:.        -
-00028dc0: 2064 6566 6175 6c74 0a20 2020 2020 2020   default.       
-00028dd0: 2061 6e79 3a20 7472 7565 0a20 2020 2020   any: true.     
-00028de0: 2070 726f 7065 7274 6965 733a 0a20 2020   properties:.   
-00028df0: 2020 2020 206d 6174 6368 5f6e 616d 6573       match_names
-00028e00: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
-00028e10: 7269 7074 696f 6e3a 206d 6174 6368 4e61  ription: matchNa
-00028e20: 6d65 7320 6973 2061 206c 6973 7420 6f66  mes is a list of
-00028e30: 206e 616d 6573 7061 6365 206e 616d 6573   namespace names
-00028e40: 2e20 5468 6520 4e61 6d65 7370 6163 6553  . The NamespaceS
-00028e50: 656c 6563 746f 720a 2020 2020 2020 2020  elector.        
-00028e60: 2020 2020 6d61 7463 6865 7320 6e61 6d65      matches name
-00028e70: 7370 6163 6573 2062 6173 6564 206f 6e20  spaces based on 
-00028e80: 7468 6520 6e61 6d65 7320 7365 6c65 6374  the names select
-00028e90: 6564 2062 7920 7468 6973 206c 6973 742e  ed by this list.
-00028ea0: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
-00028eb0: 6c65 3a0a 2020 2020 2020 2020 2020 2d20  le:.          - 
-00028ec0: 6465 6661 756c 740a 2020 2020 2020 2020  default.        
-00028ed0: 2020 6974 656d 733a 0a20 2020 2020 2020    items:.       
-00028ee0: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-00028ef0: 670a 2020 2020 2020 2020 2020 7469 746c  g.          titl
-00028f00: 653a 206d 6174 6368 5f6e 616d 6573 0a20  e: match_names. 
-00028f10: 2020 2020 2020 2020 2074 7970 653a 2061           type: a
-00028f20: 7272 6179 0a20 2020 2020 2020 2061 6e79  rray.        any
-00028f30: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
-00028f40: 7269 7074 696f 6e3a 2022 616e 7920 6d61  ription: "any ma
-00028f50: 7463 6865 7320 616e 7920 7365 6c65 6374  tches any select
-00028f60: 6564 206e 616d 6573 7061 6365 732e 2049  ed namespaces. I
-00028f70: 6620 7472 7565 2c20 7468 656e 206e 6f6e  f true, then non
-00028f80: 6520 6f66 5c0a 2020 2020 2020 2020 2020  e of\.          
-00028f90: 2020 5c20 7468 6520 6f74 6865 7220 6d61    \ the other ma
-00028fa0: 7463 6820 6669 656c 6473 2063 616e 2062  tch fields can b
-00028fb0: 6520 7365 742e 220a 2020 2020 2020 2020  e set.".        
-00028fc0: 2020 6578 616d 706c 653a 2074 7275 650a    example: true.
-00028fd0: 2020 2020 2020 2020 2020 7469 746c 653a            title:
-00028fe0: 2061 6e79 0a20 2020 2020 2020 2020 2074   any.          t
-00028ff0: 7970 653a 2062 6f6f 6c65 616e 0a20 2020  ype: boolean.   
-00029000: 2020 2074 6974 6c65 3a20 5365 7276 6963     title: Servic
-00029010: 654d 6f6e 6974 6f72 5f6e 616d 6573 7061  eMonitor_namespa
-00029020: 6365 5f73 656c 6563 746f 720a 2020 2020  ce_selector.    
-00029030: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
-00029040: 2073 6563 7572 6974 7953 6368 656d 6573   securitySchemes
-00029050: 3a0a 2020 2020 6265 6172 6572 4175 7468  :.    bearerAuth
-00029060: 3a0a 2020 2020 2020 6265 6172 6572 466f  :.      bearerFo
-00029070: 726d 6174 3a20 4a57 540a 2020 2020 2020  rmat: JWT.      
-00029080: 7363 6865 6d65 3a20 6265 6172 6572 0a20  scheme: bearer. 
-00029090: 2020 2020 2074 7970 653a 2068 7474 700a       type: http.
-000290a0: 2020 2020 2020 782d 6265 6172 6572 496e        x-bearerIn
-000290b0: 666f 4675 6e63 3a20 6f70 656e 6170 695f  foFunc: openapi_
-000290c0: 7365 7276 6572 2e63 6f6e 7472 6f6c 6c65  server.controlle
-000290d0: 7273 2e73 6563 7572 6974 795f 636f 6e74  rs.security_cont
-000290e0: 726f 6c6c 6572 5f2e 696e 666f 5f66 726f  roller_.info_fro
-000290f0: 6d5f 6265 6172 6572 4175 7468 0a         m_bearerAuth.
+00014e10: 2022 766f 6c75 6d65 436c 6169 6d54 656d   "volumeClaimTem
+00014e20: 706c 6174 6573 2069 7320 6120 6c69 7374  plates is a list
+00014e30: 206f 6620 636c 6169 6d73 2074 6861 7420   of claims that 
+00014e40: 706f 6473 2061 7265 2061 6c6c 6f77 6564  pods are allowed
+00014e50: 5c0a 2020 2020 2020 2020 2020 2020 5c20  \.            \ 
+00014e60: 746f 2072 6566 6572 656e 6365 2c20 6f6e  to reference, on
+00014e70: 6c79 2076 616c 6964 2077 6865 6e20 776f  ly valid when wo
+00014e80: 726b 6c6f 6164 5f74 7970 6520 6973 2053  rkload_type is S
+00014e90: 7461 7465 6675 6c53 6574 2e22 0a20 2020  tatefulSet.".   
+00014ea0: 2020 2020 2020 2069 7465 6d73 3a0a 2020         items:.  
+00014eb0: 2020 2020 2020 2020 2020 2472 6566 3a20            $ref: 
+00014ec0: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
+00014ed0: 6865 6d61 732f 5065 7273 6973 7465 6e74  hemas/Persistent
+00014ee0: 566f 6c75 6d65 436c 6169 6d27 0a20 2020  VolumeClaim'.   
+00014ef0: 2020 2020 2020 2074 6974 6c65 3a20 766f         title: vo
+00014f00: 6c75 6d65 5f63 6c61 696d 5f74 656d 706c  lume_claim_templ
+00014f10: 6174 6573 0a20 2020 2020 2020 2020 2074  ates.          t
+00014f20: 7970 653a 2061 7272 6179 0a20 2020 2020  ype: array.     
+00014f30: 2072 6571 7569 7265 643a 0a20 2020 2020   required:.     
+00014f40: 202d 206e 616d 650a 2020 2020 2020 7469   - name.      ti
+00014f50: 746c 653a 2057 6f72 6b6c 6f61 640a 2020  tle: Workload.  
+00014f60: 2020 2020 7479 7065 3a20 6f62 6a65 6374      type: object
+00014f70: 0a20 2020 2041 6e6e 6f74 6174 696f 6e73  .    Annotations
+00014f80: 3a0a 2020 2020 2020 6465 7363 7269 7074  :.      descript
+00014f90: 696f 6e3a 2041 6e20 756e 7374 7275 6374  ion: An unstruct
+00014fa0: 7572 6564 206b 6579 2076 616c 7565 206d  ured key value m
+00014fb0: 6170 2074 6861 7420 6361 6e20 6265 2075  ap that can be u
+00014fc0: 7365 6420 746f 2061 7474 6163 6820 6172  sed to attach ar
+00014fd0: 6269 7472 6172 790a 2020 2020 2020 2020  bitrary.        
+00014fe0: 6d65 7461 6461 7461 0a20 2020 2020 2065  metadata.      e
+00014ff0: 7861 6d70 6c65 3a0a 2020 2020 2020 2d20  xample:.      - 
+00015000: 616e 6e6f 7461 7469 6f6e 2d6b 6579 313a  annotation-key1:
+00015010: 7661 6c31 0a20 2020 2020 202d 2061 6e6e  val1.      - ann
+00015020: 6f74 6174 696f 6e2d 6b65 7932 3a76 616c  otation-key2:val
+00015030: 320a 2020 2020 2020 6974 656d 733a 0a20  2.      items:. 
+00015040: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+00015050: 696e 670a 2020 2020 2020 7469 746c 653a  ing.      title:
+00015060: 2041 6e6e 6f74 6174 696f 6e73 0a20 2020   Annotations.   
+00015070: 2020 2074 7970 653a 2061 7272 6179 0a20     type: array. 
+00015080: 2020 204c 6162 656c 733a 0a20 2020 2020     Labels:.     
+00015090: 2064 6573 6372 6970 7469 6f6e 3a20 4d61   description: Ma
+000150a0: 7020 6f66 2073 7472 696e 6720 6b65 7973  p of string keys
+000150b0: 2061 6e64 2076 616c 7565 7320 7468 6174   and values that
+000150c0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+000150d0: 6f72 6761 6e69 7a65 2061 6e64 0a20 2020  organize and.   
+000150e0: 2020 2020 2063 6174 6567 6f72 697a 6520       categorize 
+000150f0: 2873 636f 7065 2061 6e64 2073 656c 6563  (scope and selec
+00015100: 7429 206f 626a 6563 7473 0a20 2020 2020  t) objects.     
+00015110: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
+00015120: 2d20 6170 703a 6465 6d6f 2d61 7070 0a20  - app:demo-app. 
+00015130: 2020 2020 202d 2076 6572 7369 6f6e 3a76       - version:v
+00015140: 312e 302e 300a 2020 2020 2020 6974 656d  1.0.0.      item
+00015150: 733a 0a20 2020 2020 2020 2074 7970 653a  s:.        type:
+00015160: 2073 7472 696e 670a 2020 2020 2020 7469   string.      ti
+00015170: 746c 653a 204c 6162 656c 730a 2020 2020  tle: Labels.    
+00015180: 2020 7479 7065 3a20 6172 7261 790a 2020    type: array.  
+00015190: 2020 4c61 6265 6c53 656c 6563 746f 723a    LabelSelector:
+000151a0: 0a20 2020 2020 2064 6573 6372 6970 7469  .      descripti
+000151b0: 6f6e 3a20 7c0a 2020 2020 2020 2020 416e  on: |.        An
+000151c0: 2061 7272 6179 206f 6620 6c61 6265 6c20   array of label 
+000151d0: 7365 6c65 6374 6f72 2072 756c 652c 2074  selector rule, t
+000151e0: 6865 2072 756c 6520 6361 6e20 6569 7468  he rule can eith
+000151f0: 6572 2062 6520 6120 6d61 7463 6820 6c61  er be a match la
+00015200: 6265 6c20 6f72 206d 6174 6368 2065 7870  bel or match exp
+00015210: 7265 7373 696f 6e2c 0a20 2020 2020 2020  ression,.       
+00015220: 2072 6566 6572 7269 6e67 2074 6865 2065   referring the e
+00015230: 7861 6d70 6c65 2028 6669 7273 7420 6973  xample (first is
+00015240: 2061 206d 6174 6368 206c 6162 656c 2c20   a match label, 
+00015250: 7365 636f 6e64 2069 7320 6120 6d61 7463  second is a matc
+00015260: 6820 6578 7072 6573 7369 6f6e 290a 2020  h expression).  
+00015270: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
+00015280: 2020 202d 2061 7070 3a64 656d 6f2d 6170     - app:demo-ap
+00015290: 700a 2020 2020 2020 2d20 226b 6579 3a76  p.      - "key:v
+000152a0: 6572 7369 6f6e 2c20 6f70 6572 6174 6f72  ersion, operator
+000152b0: 3a49 6e2c 2076 616c 7565 733a 5b76 312e  :In, values:[v1.
+000152c0: 302e 302c 2076 312e 302e 315d 220a 2020  0.0, v1.0.1]".  
+000152d0: 2020 2020 6974 656d 733a 0a20 2020 2020      items:.     
+000152e0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
+000152f0: 2020 2020 2020 7469 746c 653a 204c 6162        title: Lab
+00015300: 656c 5365 6c65 6374 6f72 0a20 2020 2020  elSelector.     
+00015310: 2074 7970 653a 2061 7272 6179 0a20 2020   type: array.   
+00015320: 2055 7064 6174 6553 7472 6174 6567 793a   UpdateStrategy:
+00015330: 0a20 2020 2020 2065 7861 6d70 6c65 3a0a  .      example:.
+00015340: 2020 2020 2020 2020 7374 7261 7465 6779          strategy
+00015350: 5f74 7970 653a 2052 6f6c 6c69 6e67 5570  _type: RollingUp
+00015360: 6461 7465 0a20 2020 2020 2020 2072 6f6c  date.        rol
+00015370: 6c69 6e67 5f75 7064 6174 655f 636f 6e66  ling_update_conf
+00015380: 6967 3a0a 2020 2020 2020 2020 2020 7061  ig:.          pa
+00015390: 7274 6974 696f 6e3a 2032 0a20 2020 2020  rtition: 2.     
+000153a0: 2020 2020 206d 6178 5f75 6e61 7661 696c       max_unavail
+000153b0: 6162 6c65 3a20 3130 2520 6f72 2032 0a20  able: 10% or 2. 
+000153c0: 2020 2020 2020 2020 206d 6178 5f73 7572           max_sur
+000153d0: 6765 3a20 3130 2520 6f72 2032 0a20 2020  ge: 10% or 2.   
+000153e0: 2020 2070 726f 7065 7274 6965 733a 0a20     properties:. 
+000153f0: 2020 2020 2020 2073 7472 6174 6567 795f         strategy_
+00015400: 7479 7065 3a0a 2020 2020 2020 2020 2020  type:.          
+00015410: 6465 7363 7269 7074 696f 6e3a 2055 7064  description: Upd
+00015420: 6174 6520 7374 7261 7465 6779 2074 7970  ate strategy typ
+00015430: 65ef bc8c 2075 7365 6420 746f 2073 7065  e... used to spe
+00015440: 6369 6679 2074 6865 2075 7064 6174 6520  cify the update 
+00015450: 7374 7261 7465 6779 2066 6f72 0a20 2020  strategy for.   
+00015460: 2020 2020 2020 2020 2074 6865 2057 6f72           the Wor
+00015470: 6b6c 6f61 642e 0a20 2020 2020 2020 2020  kload..         
+00015480: 2065 6e75 6d3a 0a20 2020 2020 2020 2020   enum:.         
+00015490: 202d 2052 6563 7265 6174 650a 2020 2020   - Recreate.    
+000154a0: 2020 2020 2020 2d20 526f 6c6c 696e 6755        - RollingU
+000154b0: 7064 6174 650a 2020 2020 2020 2020 2020  pdate.          
+000154c0: 2d20 4f6e 4465 6c65 7465 0a20 2020 2020  - OnDelete.     
+000154d0: 2020 2020 2065 7861 6d70 6c65 3a20 526f       example: Ro
+000154e0: 6c6c 696e 6755 7064 6174 650a 2020 2020  llingUpdate.    
+000154f0: 2020 2020 2020 7469 746c 653a 2073 7472        title: str
+00015500: 6174 6567 795f 7479 7065 0a20 2020 2020  ategy_type.     
+00015510: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+00015520: 670a 2020 2020 2020 2020 726f 6c6c 696e  g.        rollin
+00015530: 675f 7570 6461 7465 5f63 6f6e 6669 673a  g_update_config:
+00015540: 0a20 2020 2020 2020 2020 2024 7265 663a  .          $ref:
+00015550: 2027 232f 636f 6d70 6f6e 656e 7473 2f73   '#/components/s
+00015560: 6368 656d 6173 2f55 7064 6174 6553 7472  chemas/UpdateStr
+00015570: 6174 6567 795f 726f 6c6c 696e 675f 7570  ategy_rolling_up
+00015580: 6461 7465 5f63 6f6e 6669 6727 0a20 2020  date_config'.   
+00015590: 2020 2074 6974 6c65 3a20 5570 6461 7465     title: Update
+000155a0: 5374 7261 7465 6779 0a20 2020 2020 2074  Strategy.      t
+000155b0: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
+000155c0: 506f 643a 0a20 2020 2020 2065 7861 6d70  Pod:.      examp
+000155d0: 6c65 3a0a 2020 2020 2020 2020 766f 6c75  le:.        volu
+000155e0: 6d65 733a 0a20 2020 2020 2020 202d 2068  mes:.        - h
+000155f0: 6f73 745f 7061 7468 3a0a 2020 2020 2020  ost_path:.      
+00015600: 2020 2020 2020 7061 7468 3a20 2f64 6174        path: /dat
+00015610: 610a 2020 2020 2020 2020 2020 2020 7061  a.            pa
+00015620: 7468 5f74 7970 653a 2044 6972 6563 746f  th_type: Directo
+00015630: 7279 0a20 2020 2020 2020 2020 206e 616d  ry.          nam
+00015640: 653a 2064 656d 6f2d 766f 6c0a 2020 2020  e: demo-vol.    
+00015650: 2020 2020 2020 656d 7074 795f 6469 723a        empty_dir:
+00015660: 0a20 2020 2020 2020 2020 2020 206d 6564  .            med
+00015670: 6975 6d3a 204d 656d 6f72 790a 2020 2020  ium: Memory.    
+00015680: 2020 2020 2020 2020 7369 7a65 5f6c 696d          size_lim
+00015690: 6974 3a20 3530 304d 690a 2020 2020 2020  it: 500Mi.      
+000156a0: 2020 2020 636f 6e66 6967 5f6d 6170 3a0a      config_map:.
+000156b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000156c0: 3a20 7365 7276 6572 2063 6f6e 6669 672f  : server config/
+000156d0: 7365 6372 6574 0a20 2020 2020 2020 2020  secret.         
+000156e0: 2020 206f 7074 696f 6e61 6c3a 2066 616c     optional: fal
+000156f0: 7365 0a20 2020 2020 2020 2020 2020 2064  se.            d
+00015700: 6566 6175 6c74 5f6d 6f64 653a 2034 3030  efault_mode: 400
+00015710: 0a20 2020 2020 2020 2020 2073 6563 7265  .          secre
+00015720: 743a 0a20 2020 2020 2020 2020 2020 206e  t:.            n
+00015730: 616d 653a 2073 6572 7665 7220 636f 6e66  ame: server conf
+00015740: 6967 2f73 6563 7265 740a 2020 2020 2020  ig/secret.      
+00015750: 2020 2020 2020 6f70 7469 6f6e 616c 3a20        optional: 
+00015760: 6661 6c73 650a 2020 2020 2020 2020 2020  false.          
+00015770: 2020 6465 6661 756c 745f 6d6f 6465 3a20    default_mode: 
+00015780: 3430 300a 2020 2020 2020 2020 2020 7065  400.          pe
+00015790: 7273 6973 7465 6e74 5f76 6f6c 756d 655f  rsistent_volume_
+000157a0: 636c 6169 6d3a 0a20 2020 2020 2020 2020  claim:.         
+000157b0: 2020 2072 6561 645f 6f6e 6c79 3a20 6661     read_only: fa
+000157c0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+000157d0: 636c 6169 6d5f 6e61 6d65 3a20 6465 6d6f  claim_name: demo
+000157e0: 2d70 7663 0a20 2020 2020 2020 202d 2068  -pvc.        - h
+000157f0: 6f73 745f 7061 7468 3a0a 2020 2020 2020  ost_path:.      
+00015800: 2020 2020 2020 7061 7468 3a20 2f64 6174        path: /dat
+00015810: 610a 2020 2020 2020 2020 2020 2020 7061  a.            pa
+00015820: 7468 5f74 7970 653a 2044 6972 6563 746f  th_type: Directo
+00015830: 7279 0a20 2020 2020 2020 2020 206e 616d  ry.          nam
+00015840: 653a 2064 656d 6f2d 766f 6c0a 2020 2020  e: demo-vol.    
+00015850: 2020 2020 2020 656d 7074 795f 6469 723a        empty_dir:
+00015860: 0a20 2020 2020 2020 2020 2020 206d 6564  .            med
+00015870: 6975 6d3a 204d 656d 6f72 790a 2020 2020  ium: Memory.    
+00015880: 2020 2020 2020 2020 7369 7a65 5f6c 696d          size_lim
+00015890: 6974 3a20 3530 304d 690a 2020 2020 2020  it: 500Mi.      
+000158a0: 2020 2020 636f 6e66 6967 5f6d 6170 3a0a      config_map:.
+000158b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000158c0: 3a20 7365 7276 6572 2063 6f6e 6669 672f  : server config/
+000158d0: 7365 6372 6574 0a20 2020 2020 2020 2020  secret.         
+000158e0: 2020 206f 7074 696f 6e61 6c3a 2066 616c     optional: fal
+000158f0: 7365 0a20 2020 2020 2020 2020 2020 2064  se.            d
+00015900: 6566 6175 6c74 5f6d 6f64 653a 2034 3030  efault_mode: 400
+00015910: 0a20 2020 2020 2020 2020 2073 6563 7265  .          secre
+00015920: 743a 0a20 2020 2020 2020 2020 2020 206e  t:.            n
+00015930: 616d 653a 2073 6572 7665 7220 636f 6e66  ame: server conf
+00015940: 6967 2f73 6563 7265 740a 2020 2020 2020  ig/secret.      
+00015950: 2020 2020 2020 6f70 7469 6f6e 616c 3a20        optional: 
+00015960: 6661 6c73 650a 2020 2020 2020 2020 2020  false.          
+00015970: 2020 6465 6661 756c 745f 6d6f 6465 3a20    default_mode: 
+00015980: 3430 300a 2020 2020 2020 2020 2020 7065  400.          pe
+00015990: 7273 6973 7465 6e74 5f76 6f6c 756d 655f  rsistent_volume_
+000159a0: 636c 6169 6d3a 0a20 2020 2020 2020 2020  claim:.         
+000159b0: 2020 2072 6561 645f 6f6e 6c79 3a20 6661     read_only: fa
+000159c0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+000159d0: 636c 6169 6d5f 6e61 6d65 3a20 6465 6d6f  claim_name: demo
+000159e0: 2d70 7663 0a20 2020 2020 2020 2061 6e6e  -pvc.        ann
+000159f0: 6f74 6174 696f 6e73 3a0a 2020 2020 2020  otations:.      
+00015a00: 2020 2d20 616e 6e6f 7461 7469 6f6e 2d6b    - annotation-k
+00015a10: 6579 313a 7661 6c31 0a20 2020 2020 2020  ey1:val1.       
+00015a20: 202d 2061 6e6e 6f74 6174 696f 6e2d 6b65   - annotation-ke
+00015a30: 7932 3a76 616c 320a 2020 2020 2020 2020  y2:val2.        
+00015a40: 636f 6e74 6169 6e65 7273 3a0a 2020 2020  containers:.    
+00015a50: 2020 2020 2d20 696d 6167 653a 206e 6769      - image: ngi
+00015a60: 6e78 3a6c 6174 6573 740a 2020 2020 2020  nx:latest.      
+00015a70: 2020 2020 6c69 6665 5f63 7963 6c65 3a0a      life_cycle:.
+00015a80: 2020 2020 2020 2020 2020 2020 7072 655f              pre_
+00015a90: 7374 6f70 3a0a 2020 2020 2020 2020 2020  stop:.          
+00015aa0: 2020 2020 7463 705f 736f 636b 6574 3a0a      tcp_socket:.
+00015ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ac0: 706f 7274 3a20 3330 3138 310a 2020 2020  port: 30181.    
+00015ad0: 2020 2020 2020 2020 2020 2020 686f 7374              host
+00015ae0: 3a20 3132 372e 302e 302e 310a 2020 2020  : 127.0.0.1.    
+00015af0: 2020 2020 2020 2020 2020 6874 7470 5f67            http_g
+00015b00: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
+00015b10: 2020 2020 7061 7468 3a20 2f73 686f 773f      path: /show?
+00015b20: 646f 6d61 696e 3d76 3139 2e74 696b 746f  domain=v19.tikto
+00015b30: 6b63 646e 2e63 6f6d 0a20 2020 2020 2020  kcdn.com.       
+00015b40: 2020 2020 2020 2020 2068 7474 705f 6865           http_he
+00015b50: 6164 6572 733a 0a20 2020 2020 2020 2020  aders:.         
+00015b60: 2020 2020 2020 202d 2078 2d64 6576 7372         - x-devsr
+00015b70: 652d 6175 7468 6f72 697a 6174 696f 6e3a  e-authorization:
+00015b80: 4265 6172 6572 2065 794a 6862 4763 694f  Bearer eyJhbGciO
+00015b90: 694a 0a20 2020 2020 2020 2020 2020 2020  iJ.             
+00015ba0: 2020 202d 2063 6f6e 7465 6e74 2d74 7970     - content-typ
+00015bb0: 653a 6170 706c 6963 6174 696f 6e2f 6a73  e:application/js
+00015bc0: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+00015bd0: 2020 2073 6368 656d 653a 2048 5454 5053     scheme: HTTPS
+00015be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015bf0: 2070 6f72 743a 2038 3838 380a 2020 2020   port: 8888.    
+00015c00: 2020 2020 2020 2020 2020 2020 686f 7374              host
+00015c10: 3a20 6773 732d 646e 732d 6167 656e 742e  : gss-dns-agent.
+00015c20: 6578 616d 706c 652e 6f72 670a 2020 2020  example.org.    
+00015c30: 2020 2020 2020 2020 2020 6578 6563 5f63            exec_c
+00015c40: 6f6d 6d61 6e64 3a0a 2020 2020 2020 2020  ommand:.        
+00015c50: 2020 2020 2020 2d20 2f62 696e 2f73 686f        - /bin/sho
+00015c60: 7764 6f77 6e2e 7368 0a20 2020 2020 2020  wdown.sh.       
+00015c70: 2020 2020 2070 6f73 745f 7374 6172 743a       post_start:
+00015c80: 0a20 2020 2020 2020 2020 2020 2020 2074  .              t
+00015c90: 6370 5f73 6f63 6b65 743a 0a20 2020 2020  cp_socket:.     
+00015ca0: 2020 2020 2020 2020 2020 2070 6f72 743a             port:
+00015cb0: 2033 3031 3831 0a20 2020 2020 2020 2020   30181.         
+00015cc0: 2020 2020 2020 2068 6f73 743a 2031 3237         host: 127
+00015cd0: 2e30 2e30 2e31 0a20 2020 2020 2020 2020  .0.0.1.         
+00015ce0: 2020 2020 2068 7474 705f 6765 743a 0a20       http_get:. 
+00015cf0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00015d00: 6174 683a 202f 7368 6f77 3f64 6f6d 6169  ath: /show?domai
+00015d10: 6e3d 7631 392e 7469 6b74 6f6b 6364 6e2e  n=v19.tiktokcdn.
+00015d20: 636f 6d0a 2020 2020 2020 2020 2020 2020  com.            
+00015d30: 2020 2020 6874 7470 5f68 6561 6465 7273      http_headers
+00015d40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015d50: 2020 2d20 782d 6465 7673 7265 2d61 7574    - x-devsre-aut
+00015d60: 686f 7269 7a61 7469 6f6e 3a42 6561 7265  horization:Beare
+00015d70: 7220 6579 4a68 6247 6369 4f69 4a0a 2020  r eyJhbGciOiJ.  
+00015d80: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00015d90: 636f 6e74 656e 742d 7479 7065 3a61 7070  content-type:app
+00015da0: 6c69 6361 7469 6f6e 2f6a 736f 6e0a 2020  lication/json.  
+00015db0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00015dc0: 6865 6d65 3a20 4854 5450 530a 2020 2020  heme: HTTPS.    
+00015dd0: 2020 2020 2020 2020 2020 2020 706f 7274              port
+00015de0: 3a20 3838 3838 0a20 2020 2020 2020 2020  : 8888.         
+00015df0: 2020 2020 2020 2068 6f73 743a 2067 7373         host: gss
+00015e00: 2d64 6e73 2d61 6765 6e74 2e65 7861 6d70  -dns-agent.examp
+00015e10: 6c65 2e6f 7267 0a20 2020 2020 2020 2020  le.org.         
+00015e20: 2020 2020 2065 7865 635f 636f 6d6d 616e       exec_comman
+00015e30: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
+00015e40: 202d 202f 6269 6e2f 7368 6f77 646f 776e   - /bin/showdown
+00015e50: 2e73 680a 2020 2020 2020 2020 2020 7265  .sh.          re
+00015e60: 736f 7572 6365 733a 0a20 2020 2020 2020  sources:.       
+00015e70: 2020 2020 2072 6571 7565 7374 733a 0a20       requests:. 
+00015e80: 2020 2020 2020 2020 2020 2020 206d 656d               mem
+00015e90: 6f72 793a 2032 3536 4d69 0a20 2020 2020  ory: 256Mi.     
+00015ea0: 2020 2020 2020 2020 2063 7075 3a20 2230           cpu: "0
+00015eb0: 2e31 220a 2020 2020 2020 2020 2020 2020  .1".            
+00015ec0: 6c69 6d69 7473 3a0a 2020 2020 2020 2020  limits:.        
+00015ed0: 2020 2020 2020 6d65 6d6f 7279 3a20 3531        memory: 51
+00015ee0: 324d 690a 2020 2020 2020 2020 2020 2020  2Mi.            
+00015ef0: 2020 6370 753a 2022 302e 3522 0a20 2020    cpu: "0.5".   
+00015f00: 2020 2020 2020 2076 6f6c 756d 655f 6d6f         volume_mo
+00015f10: 756e 7473 3a0a 2020 2020 2020 2020 2020  unts:.          
+00015f20: 2d20 7061 7468 3a20 2f6f 7074 2f73 6572  - path: /opt/ser
+00015f30: 7665 722f 636f 6e66 0a20 2020 2020 2020  ver/conf.       
+00015f40: 2020 2020 2072 6561 645f 6f6e 6c79 3a20       read_only: 
+00015f50: 7472 7565 0a20 2020 2020 2020 2020 2020  true.           
+00015f60: 206e 616d 653a 2064 656d 6f2d 766f 6c0a   name: demo-vol.
+00015f70: 2020 2020 2020 2020 2020 2020 7375 625f              sub_
+00015f80: 7061 7468 3a20 7365 7276 6572 2e63 6f6e  path: server.con
+00015f90: 660a 2020 2020 2020 2020 2020 2d20 7061  f.          - pa
+00015fa0: 7468 3a20 2f6f 7074 2f73 6572 7665 722f  th: /opt/server/
+00015fb0: 636f 6e66 0a20 2020 2020 2020 2020 2020  conf.           
+00015fc0: 2072 6561 645f 6f6e 6c79 3a20 7472 7565   read_only: true
+00015fd0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+00015fe0: 653a 2064 656d 6f2d 766f 6c0a 2020 2020  e: demo-vol.    
+00015ff0: 2020 2020 2020 2020 7375 625f 7061 7468          sub_path
+00016000: 3a20 7365 7276 6572 2e63 6f6e 660a 2020  : server.conf.  
+00016010: 2020 2020 2020 2020 656e 763a 0a20 2020          env:.   
+00016020: 2020 2020 2020 2020 206e 616d 653a 2053           name: S
+00016030: 4d53 5f4b 4559 535f 5041 5448 5f58 4d0a  MS_KEYS_PATH_XM.
+00016040: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00016050: 653a 2064 6d73 2d73 6563 7265 740a 2020  e: dms-secret.  
+00016060: 2020 2020 2020 2020 706f 7274 733a 0a20          ports:. 
+00016070: 2020 2020 2020 2020 202d 2063 6f6e 7461           - conta
+00016080: 696e 6572 5f70 6f72 743a 2038 300a 2020  iner_port: 80.  
+00016090: 2020 2020 2020 2020 2020 7072 6f74 6f63            protoc
+000160a0: 6f6c 3a20 5443 500a 2020 2020 2020 2020  ol: TCP.        
+000160b0: 2020 2020 6e61 6d65 3a20 6874 7470 0a20      name: http. 
+000160c0: 2020 2020 2020 2020 202d 2063 6f6e 7461           - conta
+000160d0: 696e 6572 5f70 6f72 743a 2038 300a 2020  iner_port: 80.  
+000160e0: 2020 2020 2020 2020 2020 7072 6f74 6f63            protoc
+000160f0: 6f6c 3a20 5443 500a 2020 2020 2020 2020  ol: TCP.        
+00016100: 2020 2020 6e61 6d65 3a20 6874 7470 0a20      name: http. 
+00016110: 2020 2020 2020 2020 2063 6f6d 6d61 6e64           command
+00016120: 3a0a 2020 2020 2020 2020 2020 2d20 7079  :.          - py
+00016130: 7468 6f6e 330a 2020 2020 2020 2020 2020  thon3.          
+00016140: 6172 6773 3a0a 2020 2020 2020 2020 2020  args:.          
+00016150: 2d20 2d6d 0a20 2020 2020 2020 2020 202d  - -m.          -
+00016160: 206f 7065 6e61 7069 5f73 6572 7665 720a   openapi_server.
+00016170: 2020 2020 2020 2020 2020 7265 6164 696e            readin
+00016180: 6573 735f 7072 6f62 653a 0a20 2020 2020  ess_probe:.     
+00016190: 2020 2020 2020 2070 6572 696f 645f 7365         period_se
+000161a0: 636f 6e64 733a 2036 300a 2020 2020 2020  conds: 60.      
+000161b0: 2020 2020 2020 696e 6974 6961 6c5f 6465        initial_de
+000161c0: 6c61 795f 7365 636f 6e64 733a 2036 3030  lay_seconds: 600
+000161d0: 0a20 2020 2020 2020 2020 2020 2074 6370  .            tcp
+000161e0: 5f73 6f63 6b65 743a 0a20 2020 2020 2020  _socket:.       
+000161f0: 2020 2020 2020 2070 6f72 743a 2033 3031         port: 301
+00016200: 3831 0a20 2020 2020 2020 2020 2020 2020  81.             
+00016210: 2068 6f73 743a 2031 3237 2e30 2e30 2e31   host: 127.0.0.1
+00016220: 0a20 2020 2020 2020 2020 2020 2066 6169  .            fai
+00016230: 6c75 7265 5f74 6872 6573 686f 6c64 3a20  lure_threshold: 
+00016240: 330a 2020 2020 2020 2020 2020 2020 6874  3.            ht
+00016250: 7470 5f67 6574 3a0a 2020 2020 2020 2020  tp_get:.        
+00016260: 2020 2020 2020 7061 7468 3a20 2f73 686f        path: /sho
+00016270: 773f 646f 6d61 696e 3d76 3139 2e74 696b  w?domain=v19.tik
+00016280: 746f 6b63 646e 2e63 6f6d 0a20 2020 2020  tokcdn.com.     
+00016290: 2020 2020 2020 2020 2068 7474 705f 6865           http_he
+000162a0: 6164 6572 733a 0a20 2020 2020 2020 2020  aders:.         
+000162b0: 2020 2020 202d 2078 2d64 6576 7372 652d       - x-devsre-
+000162c0: 6175 7468 6f72 697a 6174 696f 6e3a 4265  authorization:Be
+000162d0: 6172 6572 2065 794a 6862 4763 694f 694a  arer eyJhbGciOiJ
+000162e0: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
+000162f0: 2063 6f6e 7465 6e74 2d74 7970 653a 6170   content-type:ap
+00016300: 706c 6963 6174 696f 6e2f 6a73 6f6e 0a20  plication/json. 
+00016310: 2020 2020 2020 2020 2020 2020 2073 6368               sch
+00016320: 656d 653a 2048 5454 5053 0a20 2020 2020  eme: HTTPS.     
+00016330: 2020 2020 2020 2020 2070 6f72 743a 2038           port: 8
+00016340: 3838 380a 2020 2020 2020 2020 2020 2020  888.            
+00016350: 2020 686f 7374 3a20 6773 732d 646e 732d    host: gss-dns-
+00016360: 6167 656e 742e 6578 616d 706c 652e 6f72  agent.example.or
+00016370: 670a 2020 2020 2020 2020 2020 2020 7469  g.            ti
+00016380: 6d65 6f75 745f 7365 636f 6e64 733a 2036  meout_seconds: 6
+00016390: 300a 2020 2020 2020 2020 2020 2020 6578  0.            ex
+000163a0: 6563 5f63 6f6d 6d61 6e64 3a0a 2020 2020  ec_command:.    
+000163b0: 2020 2020 2020 2020 2d20 2f67 7373 2f64          - /gss/d
+000163c0: 696e 676d 616e 2f62 696e 2f64 696e 676d  ingman/bin/dingm
+000163d0: 616e 2d63 6c69 740a 2020 2020 2020 2020  an-clit.        
+000163e0: 2020 2020 2d20 2d61 6464 7265 7373 0a20      - -address. 
+000163f0: 2020 2020 2020 2020 2020 202d 2031 3237             - 127
+00016400: 2e30 2e30 2e31 3a33 3035 3031 0a20 2020  .0.0.1:30501.   
+00016410: 2020 2020 2020 2020 202d 202d 636f 6d6d           - -comm
+00016420: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+00016430: 2d20 7368 6f77 2070 6f70 3a61 6c6c 2073  - show pop:all s
+00016440: 756d 6d61 7279 3a68 6561 6c74 682d 7374  ummary:health-st
+00016450: 6174 7573 0a20 2020 2020 2020 2020 2065  atus.          e
+00016460: 6e76 5f66 726f 6d3a 2052 6567 756c 6172  nv_from: Regular
+00016470: 0a20 2020 2020 2020 2020 2073 7461 7274  .          start
+00016480: 7570 5f70 726f 6265 3a0a 2020 2020 2020  up_probe:.      
+00016490: 2020 2020 2020 7065 7269 6f64 5f73 6563        period_sec
+000164a0: 6f6e 6473 3a20 3630 0a20 2020 2020 2020  onds: 60.       
+000164b0: 2020 2020 2069 6e69 7469 616c 5f64 656c       initial_del
+000164c0: 6179 5f73 6563 6f6e 6473 3a20 3630 300a  ay_seconds: 600.
+000164d0: 2020 2020 2020 2020 2020 2020 7463 705f              tcp_
+000164e0: 736f 636b 6574 3a0a 2020 2020 2020 2020  socket:.        
+000164f0: 2020 2020 2020 706f 7274 3a20 3330 3138        port: 3018
+00016500: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00016510: 686f 7374 3a20 3132 372e 302e 302e 310a  host: 127.0.0.1.
+00016520: 2020 2020 2020 2020 2020 2020 6661 696c              fail
+00016530: 7572 655f 7468 7265 7368 6f6c 643a 2033  ure_threshold: 3
+00016540: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
+00016550: 705f 6765 743a 0a20 2020 2020 2020 2020  p_get:.         
+00016560: 2020 2020 2070 6174 683a 202f 7368 6f77       path: /show
+00016570: 3f64 6f6d 6169 6e3d 7631 392e 7469 6b74  ?domain=v19.tikt
+00016580: 6f6b 6364 6e2e 636f 6d0a 2020 2020 2020  okcdn.com.      
+00016590: 2020 2020 2020 2020 6874 7470 5f68 6561          http_hea
+000165a0: 6465 7273 3a0a 2020 2020 2020 2020 2020  ders:.          
+000165b0: 2020 2020 2d20 782d 6465 7673 7265 2d61      - x-devsre-a
+000165c0: 7574 686f 7269 7a61 7469 6f6e 3a42 6561  uthorization:Bea
+000165d0: 7265 7220 6579 4a68 6247 6369 4f69 4a0a  rer eyJhbGciOiJ.
+000165e0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+000165f0: 636f 6e74 656e 742d 7479 7065 3a61 7070  content-type:app
+00016600: 6c69 6361 7469 6f6e 2f6a 736f 6e0a 2020  lication/json.  
+00016610: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+00016620: 6d65 3a20 4854 5450 530a 2020 2020 2020  me: HTTPS.      
+00016630: 2020 2020 2020 2020 706f 7274 3a20 3838          port: 88
+00016640: 3838 0a20 2020 2020 2020 2020 2020 2020  88.             
+00016650: 2068 6f73 743a 2067 7373 2d64 6e73 2d61   host: gss-dns-a
+00016660: 6765 6e74 2e65 7861 6d70 6c65 2e6f 7267  gent.example.org
+00016670: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00016680: 656f 7574 5f73 6563 6f6e 6473 3a20 3630  eout_seconds: 60
+00016690: 0a20 2020 2020 2020 2020 2020 2065 7865  .            exe
+000166a0: 635f 636f 6d6d 616e 643a 0a20 2020 2020  c_command:.     
+000166b0: 2020 2020 2020 202d 202f 6773 732f 6469         - /gss/di
+000166c0: 6e67 6d61 6e2f 6269 6e2f 6469 6e67 6d61  ngman/bin/dingma
+000166d0: 6e2d 636c 6974 0a20 2020 2020 2020 2020  n-clit.         
+000166e0: 2020 202d 202d 6164 6472 6573 730a 2020     - -address.  
+000166f0: 2020 2020 2020 2020 2020 2d20 3132 372e            - 127.
+00016700: 302e 302e 313a 3330 3530 310a 2020 2020  0.0.1:30501.    
+00016710: 2020 2020 2020 2020 2d20 2d63 6f6d 6d61          - -comma
+00016720: 6e64 0a20 2020 2020 2020 2020 2020 202d  nd.            -
+00016730: 2073 686f 7720 706f 703a 616c 6c20 7375   show pop:all su
+00016740: 6d6d 6172 793a 6865 616c 7468 2d73 7461  mmary:health-sta
+00016750: 7475 730a 2020 2020 2020 2020 2020 696d  tus.          im
+00016760: 6167 655f 7075 6c6c 5f70 6f6c 6963 793a  age_pull_policy:
+00016770: 2049 664e 6f74 5072 6573 656e 740a 2020   IfNotPresent.  
+00016780: 2020 2020 2020 2020 766f 6c75 6d65 5f64          volume_d
+00016790: 6576 6963 6573 3a0a 2020 2020 2020 2020  evices:.        
+000167a0: 2020 2d20 6e61 6d65 3a20 6465 6d6f 2d76    - name: demo-v
+000167b0: 6f6c 0a20 2020 2020 2020 2020 2020 2064  ol.            d
+000167c0: 6576 6963 655f 7061 7468 3a20 2f64 6576  evice_path: /dev
+000167d0: 2f73 6461 310a 2020 2020 2020 2020 2020  /sda1.          
+000167e0: 2020 6263 6163 6865 5f6e 756d 733a 2034    bcache_nums: 4
+000167f0: 0a20 2020 2020 2020 2020 202d 206e 616d  .          - nam
+00016800: 653a 2064 656d 6f2d 766f 6c0a 2020 2020  e: demo-vol.    
+00016810: 2020 2020 2020 2020 6465 7669 6365 5f70          device_p
+00016820: 6174 683a 202f 6465 762f 7364 6131 0a20  ath: /dev/sda1. 
+00016830: 2020 2020 2020 2020 2020 2062 6361 6368             bcach
+00016840: 655f 6e75 6d73 3a20 340a 2020 2020 2020  e_nums: 4.      
+00016850: 2020 2020 6e61 6d65 3a20 6874 7470 2d73      name: http-s
+00016860: 6572 7665 720a 2020 2020 2020 2020 2020  erver.          
+00016870: 636f 6e74 6169 6e65 725f 7479 7065 3a20  container_type: 
+00016880: 496e 6974 0a20 2020 2020 2020 2020 206c  Init.          l
+00016890: 6976 656e 6573 735f 7072 6f62 653a 0a20  iveness_probe:. 
+000168a0: 2020 2020 2020 2020 2020 2070 6572 696f             perio
+000168b0: 645f 7365 636f 6e64 733a 2036 300a 2020  d_seconds: 60.  
+000168c0: 2020 2020 2020 2020 2020 696e 6974 6961            initia
+000168d0: 6c5f 6465 6c61 795f 7365 636f 6e64 733a  l_delay_seconds:
+000168e0: 2036 3030 0a20 2020 2020 2020 2020 2020   600.           
+000168f0: 2074 6370 5f73 6f63 6b65 743a 0a20 2020   tcp_socket:.   
+00016900: 2020 2020 2020 2020 2020 2070 6f72 743a             port:
+00016910: 2033 3031 3831 0a20 2020 2020 2020 2020   30181.         
+00016920: 2020 2020 2068 6f73 743a 2031 3237 2e30       host: 127.0
+00016930: 2e30 2e31 0a20 2020 2020 2020 2020 2020  .0.1.           
+00016940: 2066 6169 6c75 7265 5f74 6872 6573 686f   failure_thresho
+00016950: 6c64 3a20 330a 2020 2020 2020 2020 2020  ld: 3.          
+00016960: 2020 6874 7470 5f67 6574 3a0a 2020 2020    http_get:.    
+00016970: 2020 2020 2020 2020 2020 7061 7468 3a20            path: 
+00016980: 2f73 686f 773f 646f 6d61 696e 3d76 3139  /show?domain=v19
+00016990: 2e74 696b 746f 6b63 646e 2e63 6f6d 0a20  .tiktokcdn.com. 
+000169a0: 2020 2020 2020 2020 2020 2020 2068 7474               htt
+000169b0: 705f 6865 6164 6572 733a 0a20 2020 2020  p_headers:.     
+000169c0: 2020 2020 2020 2020 202d 2078 2d64 6576           - x-dev
+000169d0: 7372 652d 6175 7468 6f72 697a 6174 696f  sre-authorizatio
+000169e0: 6e3a 4265 6172 6572 2065 794a 6862 4763  n:Bearer eyJhbGc
+000169f0: 694f 694a 0a20 2020 2020 2020 2020 2020  iOiJ.           
+00016a00: 2020 202d 2063 6f6e 7465 6e74 2d74 7970     - content-typ
+00016a10: 653a 6170 706c 6963 6174 696f 6e2f 6a73  e:application/js
+00016a20: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+00016a30: 2073 6368 656d 653a 2048 5454 5053 0a20   scheme: HTTPS. 
+00016a40: 2020 2020 2020 2020 2020 2020 2070 6f72               por
+00016a50: 743a 2038 3838 380a 2020 2020 2020 2020  t: 8888.        
+00016a60: 2020 2020 2020 686f 7374 3a20 6773 732d        host: gss-
+00016a70: 646e 732d 6167 656e 742e 6578 616d 706c  dns-agent.exampl
+00016a80: 652e 6f72 670a 2020 2020 2020 2020 2020  e.org.          
+00016a90: 2020 7469 6d65 6f75 745f 7365 636f 6e64    timeout_second
+00016aa0: 733a 2036 300a 2020 2020 2020 2020 2020  s: 60.          
+00016ab0: 2020 6578 6563 5f63 6f6d 6d61 6e64 3a0a    exec_command:.
+00016ac0: 2020 2020 2020 2020 2020 2020 2d20 2f67              - /g
+00016ad0: 7373 2f64 696e 676d 616e 2f62 696e 2f64  ss/dingman/bin/d
+00016ae0: 696e 676d 616e 2d63 6c69 740a 2020 2020  ingman-clit.    
+00016af0: 2020 2020 2020 2020 2d20 2d61 6464 7265          - -addre
+00016b00: 7373 0a20 2020 2020 2020 2020 2020 202d  ss.            -
+00016b10: 2031 3237 2e30 2e30 2e31 3a33 3035 3031   127.0.0.1:30501
+00016b20: 0a20 2020 2020 2020 2020 2020 202d 202d  .            - -
+00016b30: 636f 6d6d 616e 640a 2020 2020 2020 2020  command.        
+00016b40: 2020 2020 2d20 7368 6f77 2070 6f70 3a61      - show pop:a
+00016b50: 6c6c 2073 756d 6d61 7279 3a68 6561 6c74  ll summary:healt
+00016b60: 682d 7374 6174 7573 0a20 2020 2020 2020  h-status.       
+00016b70: 2020 2073 6563 7572 6974 795f 636f 6e74     security_cont
+00016b80: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
+00016b90: 2063 6170 6162 696c 6974 6965 733a 0a20   capabilities:. 
+00016ba0: 2020 2020 2020 2020 2020 2020 2061 6464               add
+00016bb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016bc0: 2d20 4e45 545f 4144 4d49 4e0a 2020 2020  - NET_ADMIN.    
+00016bd0: 2020 2020 2020 2020 2020 2d20 5359 535f            - SYS_
+00016be0: 5449 4d45 0a20 2020 2020 2020 2020 2020  TIME.           
+00016bf0: 2020 2064 726f 703a 0a20 2020 2020 2020     drop:.       
+00016c00: 2020 2020 2020 202d 204e 4554 5f41 444d         - NET_ADM
+00016c10: 494e 0a20 2020 2020 2020 2020 2020 2020  IN.             
+00016c20: 202d 2053 5953 5f54 494d 450a 2020 2020   - SYS_TIME.    
+00016c30: 2020 2020 2020 2020 7275 6e5f 6173 5f67          run_as_g
+00016c40: 726f 7570 3a20 3330 3030 0a20 2020 2020  roup: 3000.     
+00016c50: 2020 2020 2020 2072 756e 5f61 735f 7573         run_as_us
+00016c60: 6572 3a20 3130 3030 0a20 2020 2020 2020  er: 1000.       
+00016c70: 202d 2069 6d61 6765 3a20 6e67 696e 783a   - image: nginx:
+00016c80: 6c61 7465 7374 0a20 2020 2020 2020 2020  latest.         
+00016c90: 206c 6966 655f 6379 636c 653a 0a20 2020   life_cycle:.   
+00016ca0: 2020 2020 2020 2020 2070 7265 5f73 746f           pre_sto
+00016cb0: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+00016cc0: 2074 6370 5f73 6f63 6b65 743a 0a20 2020   tcp_socket:.   
+00016cd0: 2020 2020 2020 2020 2020 2020 2070 6f72               por
+00016ce0: 743a 2033 3031 3831 0a20 2020 2020 2020  t: 30181.       
+00016cf0: 2020 2020 2020 2020 2068 6f73 743a 2031           host: 1
+00016d00: 3237 2e30 2e30 2e31 0a20 2020 2020 2020  27.0.0.1.       
+00016d10: 2020 2020 2020 2068 7474 705f 6765 743a         http_get:
+00016d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d30: 2070 6174 683a 202f 7368 6f77 3f64 6f6d   path: /show?dom
+00016d40: 6169 6e3d 7631 392e 7469 6b74 6f6b 6364  ain=v19.tiktokcd
+00016d50: 6e2e 636f 6d0a 2020 2020 2020 2020 2020  n.com.          
+00016d60: 2020 2020 2020 6874 7470 5f68 6561 6465        http_heade
+00016d70: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+00016d80: 2020 2020 2d20 782d 6465 7673 7265 2d61      - x-devsre-a
+00016d90: 7574 686f 7269 7a61 7469 6f6e 3a42 6561  uthorization:Bea
+00016da0: 7265 7220 6579 4a68 6247 6369 4f69 4a0a  rer eyJhbGciOiJ.
+00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016dc0: 2d20 636f 6e74 656e 742d 7479 7065 3a61  - content-type:a
+00016dd0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e0a  pplication/json.
+00016de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016df0: 7363 6865 6d65 3a20 4854 5450 530a 2020  scheme: HTTPS.  
+00016e00: 2020 2020 2020 2020 2020 2020 2020 706f                po
+00016e10: 7274 3a20 3838 3838 0a20 2020 2020 2020  rt: 8888.       
+00016e20: 2020 2020 2020 2020 2068 6f73 743a 2067           host: g
+00016e30: 7373 2d64 6e73 2d61 6765 6e74 2e65 7861  ss-dns-agent.exa
+00016e40: 6d70 6c65 2e6f 7267 0a20 2020 2020 2020  mple.org.       
+00016e50: 2020 2020 2020 2065 7865 635f 636f 6d6d         exec_comm
+00016e60: 616e 643a 0a20 2020 2020 2020 2020 2020  and:.           
+00016e70: 2020 202d 202f 6269 6e2f 7368 6f77 646f     - /bin/showdo
+00016e80: 776e 2e73 680a 2020 2020 2020 2020 2020  wn.sh.          
+00016e90: 2020 706f 7374 5f73 7461 7274 3a0a 2020    post_start:.  
+00016ea0: 2020 2020 2020 2020 2020 2020 7463 705f              tcp_
+00016eb0: 736f 636b 6574 3a0a 2020 2020 2020 2020  socket:.        
+00016ec0: 2020 2020 2020 2020 706f 7274 3a20 3330          port: 30
+00016ed0: 3138 310a 2020 2020 2020 2020 2020 2020  181.            
+00016ee0: 2020 2020 686f 7374 3a20 3132 372e 302e      host: 127.0.
+00016ef0: 302e 310a 2020 2020 2020 2020 2020 2020  0.1.            
+00016f00: 2020 6874 7470 5f67 6574 3a0a 2020 2020    http_get:.    
+00016f10: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00016f20: 3a20 2f73 686f 773f 646f 6d61 696e 3d76  : /show?domain=v
+00016f30: 3139 2e74 696b 746f 6b63 646e 2e63 6f6d  19.tiktokcdn.com
+00016f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016f50: 2068 7474 705f 6865 6164 6572 733a 0a20   http_headers:. 
+00016f60: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+00016f70: 2078 2d64 6576 7372 652d 6175 7468 6f72   x-devsre-author
+00016f80: 697a 6174 696f 6e3a 4265 6172 6572 2065  ization:Bearer e
+00016f90: 794a 6862 4763 694f 694a 0a20 2020 2020  yJhbGciOiJ.     
+00016fa0: 2020 2020 2020 2020 2020 202d 2063 6f6e             - con
+00016fb0: 7465 6e74 2d74 7970 653a 6170 706c 6963  tent-type:applic
+00016fc0: 6174 696f 6e2f 6a73 6f6e 0a20 2020 2020  ation/json.     
+00016fd0: 2020 2020 2020 2020 2020 2073 6368 656d             schem
+00016fe0: 653a 2048 5454 5053 0a20 2020 2020 2020  e: HTTPS.       
+00016ff0: 2020 2020 2020 2020 2070 6f72 743a 2038           port: 8
+00017000: 3838 380a 2020 2020 2020 2020 2020 2020  888.            
+00017010: 2020 2020 686f 7374 3a20 6773 732d 646e      host: gss-dn
+00017020: 732d 6167 656e 742e 6578 616d 706c 652e  s-agent.example.
+00017030: 6f72 670a 2020 2020 2020 2020 2020 2020  org.            
+00017040: 2020 6578 6563 5f63 6f6d 6d61 6e64 3a0a    exec_command:.
+00017050: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00017060: 2f62 696e 2f73 686f 7764 6f77 6e2e 7368  /bin/showdown.sh
+00017070: 0a20 2020 2020 2020 2020 2072 6573 6f75  .          resou
+00017080: 7263 6573 3a0a 2020 2020 2020 2020 2020  rces:.          
+00017090: 2020 7265 7175 6573 7473 3a0a 2020 2020    requests:.    
+000170a0: 2020 2020 2020 2020 2020 6d65 6d6f 7279            memory
+000170b0: 3a20 3235 364d 690a 2020 2020 2020 2020  : 256Mi.        
+000170c0: 2020 2020 2020 6370 753a 2022 302e 3122        cpu: "0.1"
+000170d0: 0a20 2020 2020 2020 2020 2020 206c 696d  .            lim
+000170e0: 6974 733a 0a20 2020 2020 2020 2020 2020  its:.           
+000170f0: 2020 206d 656d 6f72 793a 2035 3132 4d69     memory: 512Mi
+00017100: 0a20 2020 2020 2020 2020 2020 2020 2063  .              c
+00017110: 7075 3a20 2230 2e35 220a 2020 2020 2020  pu: "0.5".      
+00017120: 2020 2020 766f 6c75 6d65 5f6d 6f75 6e74      volume_mount
+00017130: 733a 0a20 2020 2020 2020 2020 202d 2070  s:.          - p
+00017140: 6174 683a 202f 6f70 742f 7365 7276 6572  ath: /opt/server
+00017150: 2f63 6f6e 660a 2020 2020 2020 2020 2020  /conf.          
+00017160: 2020 7265 6164 5f6f 6e6c 793a 2074 7275    read_only: tru
+00017170: 650a 2020 2020 2020 2020 2020 2020 6e61  e.            na
+00017180: 6d65 3a20 6465 6d6f 2d76 6f6c 0a20 2020  me: demo-vol.   
+00017190: 2020 2020 2020 2020 2073 7562 5f70 6174           sub_pat
+000171a0: 683a 2073 6572 7665 722e 636f 6e66 0a20  h: server.conf. 
+000171b0: 2020 2020 2020 2020 202d 2070 6174 683a           - path:
+000171c0: 202f 6f70 742f 7365 7276 6572 2f63 6f6e   /opt/server/con
+000171d0: 660a 2020 2020 2020 2020 2020 2020 7265  f.            re
+000171e0: 6164 5f6f 6e6c 793a 2074 7275 650a 2020  ad_only: true.  
+000171f0: 2020 2020 2020 2020 2020 6e61 6d65 3a20            name: 
+00017200: 6465 6d6f 2d76 6f6c 0a20 2020 2020 2020  demo-vol.       
+00017210: 2020 2020 2073 7562 5f70 6174 683a 2073       sub_path: s
+00017220: 6572 7665 722e 636f 6e66 0a20 2020 2020  erver.conf.     
+00017230: 2020 2020 2065 6e76 3a0a 2020 2020 2020       env:.      
+00017240: 2020 2020 2020 6e61 6d65 3a20 534d 535f        name: SMS_
+00017250: 4b45 5953 5f50 4154 485f 584d 0a20 2020  KEYS_PATH_XM.   
+00017260: 2020 2020 2020 2020 2076 616c 7565 3a20           value: 
+00017270: 646d 732d 7365 6372 6574 0a20 2020 2020  dms-secret.     
+00017280: 2020 2020 2070 6f72 7473 3a0a 2020 2020       ports:.    
+00017290: 2020 2020 2020 2d20 636f 6e74 6169 6e65        - containe
+000172a0: 725f 706f 7274 3a20 3830 0a20 2020 2020  r_port: 80.     
+000172b0: 2020 2020 2020 2070 726f 746f 636f 6c3a         protocol:
+000172c0: 2054 4350 0a20 2020 2020 2020 2020 2020   TCP.           
+000172d0: 206e 616d 653a 2068 7474 700a 2020 2020   name: http.    
+000172e0: 2020 2020 2020 2d20 636f 6e74 6169 6e65        - containe
+000172f0: 725f 706f 7274 3a20 3830 0a20 2020 2020  r_port: 80.     
+00017300: 2020 2020 2020 2070 726f 746f 636f 6c3a         protocol:
+00017310: 2054 4350 0a20 2020 2020 2020 2020 2020   TCP.           
+00017320: 206e 616d 653a 2068 7474 700a 2020 2020   name: http.    
+00017330: 2020 2020 2020 636f 6d6d 616e 643a 0a20        command:. 
+00017340: 2020 2020 2020 2020 202d 2070 7974 686f           - pytho
+00017350: 6e33 0a20 2020 2020 2020 2020 2061 7267  n3.          arg
+00017360: 733a 0a20 2020 2020 2020 2020 202d 202d  s:.          - -
+00017370: 6d0a 2020 2020 2020 2020 2020 2d20 6f70  m.          - op
+00017380: 656e 6170 695f 7365 7276 6572 0a20 2020  enapi_server.   
+00017390: 2020 2020 2020 2072 6561 6469 6e65 7373         readiness
+000173a0: 5f70 726f 6265 3a0a 2020 2020 2020 2020  _probe:.        
+000173b0: 2020 2020 7065 7269 6f64 5f73 6563 6f6e      period_secon
+000173c0: 6473 3a20 3630 0a20 2020 2020 2020 2020  ds: 60.         
+000173d0: 2020 2069 6e69 7469 616c 5f64 656c 6179     initial_delay
+000173e0: 5f73 6563 6f6e 6473 3a20 3630 300a 2020  _seconds: 600.  
+000173f0: 2020 2020 2020 2020 2020 7463 705f 736f            tcp_so
+00017400: 636b 6574 3a0a 2020 2020 2020 2020 2020  cket:.          
+00017410: 2020 2020 706f 7274 3a20 3330 3138 310a      port: 30181.
+00017420: 2020 2020 2020 2020 2020 2020 2020 686f                ho
+00017430: 7374 3a20 3132 372e 302e 302e 310a 2020  st: 127.0.0.1.  
+00017440: 2020 2020 2020 2020 2020 6661 696c 7572            failur
+00017450: 655f 7468 7265 7368 6f6c 643a 2033 0a20  e_threshold: 3. 
+00017460: 2020 2020 2020 2020 2020 2068 7474 705f             http_
+00017470: 6765 743a 0a20 2020 2020 2020 2020 2020  get:.           
+00017480: 2020 2070 6174 683a 202f 7368 6f77 3f64     path: /show?d
+00017490: 6f6d 6169 6e3d 7631 392e 7469 6b74 6f6b  omain=v19.tiktok
+000174a0: 6364 6e2e 636f 6d0a 2020 2020 2020 2020  cdn.com.        
+000174b0: 2020 2020 2020 6874 7470 5f68 6561 6465        http_heade
+000174c0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+000174d0: 2020 2d20 782d 6465 7673 7265 2d61 7574    - x-devsre-aut
+000174e0: 686f 7269 7a61 7469 6f6e 3a42 6561 7265  horization:Beare
+000174f0: 7220 6579 4a68 6247 6369 4f69 4a0a 2020  r eyJhbGciOiJ.  
+00017500: 2020 2020 2020 2020 2020 2020 2d20 636f              - co
+00017510: 6e74 656e 742d 7479 7065 3a61 7070 6c69  ntent-type:appli
+00017520: 6361 7469 6f6e 2f6a 736f 6e0a 2020 2020  cation/json.    
+00017530: 2020 2020 2020 2020 2020 7363 6865 6d65            scheme
+00017540: 3a20 4854 5450 530a 2020 2020 2020 2020  : HTTPS.        
+00017550: 2020 2020 2020 706f 7274 3a20 3838 3838        port: 8888
+00017560: 0a20 2020 2020 2020 2020 2020 2020 2068  .              h
+00017570: 6f73 743a 2067 7373 2d64 6e73 2d61 6765  ost: gss-dns-age
+00017580: 6e74 2e65 7861 6d70 6c65 2e6f 7267 0a20  nt.example.org. 
+00017590: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
+000175a0: 7574 5f73 6563 6f6e 6473 3a20 3630 0a20  ut_seconds: 60. 
+000175b0: 2020 2020 2020 2020 2020 2065 7865 635f             exec_
+000175c0: 636f 6d6d 616e 643a 0a20 2020 2020 2020  command:.       
+000175d0: 2020 2020 202d 202f 6773 732f 6469 6e67       - /gss/ding
+000175e0: 6d61 6e2f 6269 6e2f 6469 6e67 6d61 6e2d  man/bin/dingman-
+000175f0: 636c 6974 0a20 2020 2020 2020 2020 2020  clit.           
+00017600: 202d 202d 6164 6472 6573 730a 2020 2020   - -address.    
+00017610: 2020 2020 2020 2020 2d20 3132 372e 302e          - 127.0.
+00017620: 302e 313a 3330 3530 310a 2020 2020 2020  0.1:30501.      
+00017630: 2020 2020 2020 2d20 2d63 6f6d 6d61 6e64        - -command
+00017640: 0a20 2020 2020 2020 2020 2020 202d 2073  .            - s
+00017650: 686f 7720 706f 703a 616c 6c20 7375 6d6d  how pop:all summ
+00017660: 6172 793a 6865 616c 7468 2d73 7461 7475  ary:health-statu
+00017670: 730a 2020 2020 2020 2020 2020 656e 765f  s.          env_
+00017680: 6672 6f6d 3a20 5265 6775 6c61 720a 2020  from: Regular.  
+00017690: 2020 2020 2020 2020 7374 6172 7475 705f          startup_
+000176a0: 7072 6f62 653a 0a20 2020 2020 2020 2020  probe:.         
+000176b0: 2020 2070 6572 696f 645f 7365 636f 6e64     period_second
+000176c0: 733a 2036 300a 2020 2020 2020 2020 2020  s: 60.          
+000176d0: 2020 696e 6974 6961 6c5f 6465 6c61 795f    initial_delay_
+000176e0: 7365 636f 6e64 733a 2036 3030 0a20 2020  seconds: 600.   
+000176f0: 2020 2020 2020 2020 2074 6370 5f73 6f63           tcp_soc
+00017700: 6b65 743a 0a20 2020 2020 2020 2020 2020  ket:.           
+00017710: 2020 2070 6f72 743a 2033 3031 3831 0a20     port: 30181. 
+00017720: 2020 2020 2020 2020 2020 2020 2068 6f73               hos
+00017730: 743a 2031 3237 2e30 2e30 2e31 0a20 2020  t: 127.0.0.1.   
+00017740: 2020 2020 2020 2020 2066 6169 6c75 7265           failure
+00017750: 5f74 6872 6573 686f 6c64 3a20 330a 2020  _threshold: 3.  
+00017760: 2020 2020 2020 2020 2020 6874 7470 5f67            http_g
+00017770: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
+00017780: 2020 7061 7468 3a20 2f73 686f 773f 646f    path: /show?do
+00017790: 6d61 696e 3d76 3139 2e74 696b 746f 6b63  main=v19.tiktokc
+000177a0: 646e 2e63 6f6d 0a20 2020 2020 2020 2020  dn.com.         
+000177b0: 2020 2020 2068 7474 705f 6865 6164 6572       http_header
+000177c0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000177d0: 202d 2078 2d64 6576 7372 652d 6175 7468   - x-devsre-auth
+000177e0: 6f72 697a 6174 696f 6e3a 4265 6172 6572  orization:Bearer
+000177f0: 2065 794a 6862 4763 694f 694a 0a20 2020   eyJhbGciOiJ.   
+00017800: 2020 2020 2020 2020 2020 202d 2063 6f6e             - con
+00017810: 7465 6e74 2d74 7970 653a 6170 706c 6963  tent-type:applic
+00017820: 6174 696f 6e2f 6a73 6f6e 0a20 2020 2020  ation/json.     
+00017830: 2020 2020 2020 2020 2073 6368 656d 653a           scheme:
+00017840: 2048 5454 5053 0a20 2020 2020 2020 2020   HTTPS.         
+00017850: 2020 2020 2070 6f72 743a 2038 3838 380a       port: 8888.
+00017860: 2020 2020 2020 2020 2020 2020 2020 686f                ho
+00017870: 7374 3a20 6773 732d 646e 732d 6167 656e  st: gss-dns-agen
+00017880: 742e 6578 616d 706c 652e 6f72 670a 2020  t.example.org.  
+00017890: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
+000178a0: 745f 7365 636f 6e64 733a 2036 300a 2020  t_seconds: 60.  
+000178b0: 2020 2020 2020 2020 2020 6578 6563 5f63            exec_c
+000178c0: 6f6d 6d61 6e64 3a0a 2020 2020 2020 2020  ommand:.        
+000178d0: 2020 2020 2d20 2f67 7373 2f64 696e 676d      - /gss/dingm
+000178e0: 616e 2f62 696e 2f64 696e 676d 616e 2d63  an/bin/dingman-c
+000178f0: 6c69 740a 2020 2020 2020 2020 2020 2020  lit.            
+00017900: 2d20 2d61 6464 7265 7373 0a20 2020 2020  - -address.     
+00017910: 2020 2020 2020 202d 2031 3237 2e30 2e30         - 127.0.0
+00017920: 2e31 3a33 3035 3031 0a20 2020 2020 2020  .1:30501.       
+00017930: 2020 2020 202d 202d 636f 6d6d 616e 640a       - -command.
+00017940: 2020 2020 2020 2020 2020 2020 2d20 7368              - sh
+00017950: 6f77 2070 6f70 3a61 6c6c 2073 756d 6d61  ow pop:all summa
+00017960: 7279 3a68 6561 6c74 682d 7374 6174 7573  ry:health-status
+00017970: 0a20 2020 2020 2020 2020 2069 6d61 6765  .          image
+00017980: 5f70 756c 6c5f 706f 6c69 6379 3a20 4966  _pull_policy: If
+00017990: 4e6f 7450 7265 7365 6e74 0a20 2020 2020  NotPresent.     
+000179a0: 2020 2020 2076 6f6c 756d 655f 6465 7669       volume_devi
+000179b0: 6365 733a 0a20 2020 2020 2020 2020 202d  ces:.          -
+000179c0: 206e 616d 653a 2064 656d 6f2d 766f 6c0a   name: demo-vol.
+000179d0: 2020 2020 2020 2020 2020 2020 6465 7669              devi
+000179e0: 6365 5f70 6174 683a 202f 6465 762f 7364  ce_path: /dev/sd
+000179f0: 6131 0a20 2020 2020 2020 2020 2020 2062  a1.            b
+00017a00: 6361 6368 655f 6e75 6d73 3a20 340a 2020  cache_nums: 4.  
+00017a10: 2020 2020 2020 2020 2d20 6e61 6d65 3a20          - name: 
+00017a20: 6465 6d6f 2d76 6f6c 0a20 2020 2020 2020  demo-vol.       
+00017a30: 2020 2020 2064 6576 6963 655f 7061 7468       device_path
+00017a40: 3a20 2f64 6576 2f73 6461 310a 2020 2020  : /dev/sda1.    
+00017a50: 2020 2020 2020 2020 6263 6163 6865 5f6e          bcache_n
+00017a60: 756d 733a 2034 0a20 2020 2020 2020 2020  ums: 4.         
+00017a70: 206e 616d 653a 2068 7474 702d 7365 7276   name: http-serv
+00017a80: 6572 0a20 2020 2020 2020 2020 2063 6f6e  er.          con
+00017a90: 7461 696e 6572 5f74 7970 653a 2049 6e69  tainer_type: Ini
+00017aa0: 740a 2020 2020 2020 2020 2020 6c69 7665  t.          live
+00017ab0: 6e65 7373 5f70 726f 6265 3a0a 2020 2020  ness_probe:.    
+00017ac0: 2020 2020 2020 2020 7065 7269 6f64 5f73          period_s
+00017ad0: 6563 6f6e 6473 3a20 3630 0a20 2020 2020  econds: 60.     
+00017ae0: 2020 2020 2020 2069 6e69 7469 616c 5f64         initial_d
+00017af0: 656c 6179 5f73 6563 6f6e 6473 3a20 3630  elay_seconds: 60
+00017b00: 300a 2020 2020 2020 2020 2020 2020 7463  0.            tc
+00017b10: 705f 736f 636b 6574 3a0a 2020 2020 2020  p_socket:.      
+00017b20: 2020 2020 2020 2020 706f 7274 3a20 3330          port: 30
+00017b30: 3138 310a 2020 2020 2020 2020 2020 2020  181.            
+00017b40: 2020 686f 7374 3a20 3132 372e 302e 302e    host: 127.0.0.
+00017b50: 310a 2020 2020 2020 2020 2020 2020 6661  1.            fa
+00017b60: 696c 7572 655f 7468 7265 7368 6f6c 643a  ilure_threshold:
+00017b70: 2033 0a20 2020 2020 2020 2020 2020 2068   3.            h
+00017b80: 7474 705f 6765 743a 0a20 2020 2020 2020  ttp_get:.       
+00017b90: 2020 2020 2020 2070 6174 683a 202f 7368         path: /sh
+00017ba0: 6f77 3f64 6f6d 6169 6e3d 7631 392e 7469  ow?domain=v19.ti
+00017bb0: 6b74 6f6b 6364 6e2e 636f 6d0a 2020 2020  ktokcdn.com.    
+00017bc0: 2020 2020 2020 2020 2020 6874 7470 5f68            http_h
+00017bd0: 6561 6465 7273 3a0a 2020 2020 2020 2020  eaders:.        
+00017be0: 2020 2020 2020 2d20 782d 6465 7673 7265        - x-devsre
+00017bf0: 2d61 7574 686f 7269 7a61 7469 6f6e 3a42  -authorization:B
+00017c00: 6561 7265 7220 6579 4a68 6247 6369 4f69  earer eyJhbGciOi
+00017c10: 4a0a 2020 2020 2020 2020 2020 2020 2020  J.              
+00017c20: 2d20 636f 6e74 656e 742d 7479 7065 3a61  - content-type:a
+00017c30: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e0a  pplication/json.
+00017c40: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00017c50: 6865 6d65 3a20 4854 5450 530a 2020 2020  heme: HTTPS.    
+00017c60: 2020 2020 2020 2020 2020 706f 7274 3a20            port: 
+00017c70: 3838 3838 0a20 2020 2020 2020 2020 2020  8888.           
+00017c80: 2020 2068 6f73 743a 2067 7373 2d64 6e73     host: gss-dns
+00017c90: 2d61 6765 6e74 2e65 7861 6d70 6c65 2e6f  -agent.example.o
+00017ca0: 7267 0a20 2020 2020 2020 2020 2020 2074  rg.            t
+00017cb0: 696d 656f 7574 5f73 6563 6f6e 6473 3a20  imeout_seconds: 
+00017cc0: 3630 0a20 2020 2020 2020 2020 2020 2065  60.            e
+00017cd0: 7865 635f 636f 6d6d 616e 643a 0a20 2020  xec_command:.   
+00017ce0: 2020 2020 2020 2020 202d 202f 6773 732f           - /gss/
+00017cf0: 6469 6e67 6d61 6e2f 6269 6e2f 6469 6e67  dingman/bin/ding
+00017d00: 6d61 6e2d 636c 6974 0a20 2020 2020 2020  man-clit.       
+00017d10: 2020 2020 202d 202d 6164 6472 6573 730a       - -address.
+00017d20: 2020 2020 2020 2020 2020 2020 2d20 3132              - 12
+00017d30: 372e 302e 302e 313a 3330 3530 310a 2020  7.0.0.1:30501.  
+00017d40: 2020 2020 2020 2020 2020 2d20 2d63 6f6d            - -com
+00017d50: 6d61 6e64 0a20 2020 2020 2020 2020 2020  mand.           
+00017d60: 202d 2073 686f 7720 706f 703a 616c 6c20   - show pop:all 
+00017d70: 7375 6d6d 6172 793a 6865 616c 7468 2d73  summary:health-s
+00017d80: 7461 7475 730a 2020 2020 2020 2020 2020  tatus.          
+00017d90: 7365 6375 7269 7479 5f63 6f6e 7465 7874  security_context
+00017da0: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
+00017db0: 7061 6269 6c69 7469 6573 3a0a 2020 2020  pabilities:.    
+00017dc0: 2020 2020 2020 2020 2020 6164 643a 0a20            add:. 
+00017dd0: 2020 2020 2020 2020 2020 2020 202d 204e               - N
+00017de0: 4554 5f41 444d 494e 0a20 2020 2020 2020  ET_ADMIN.       
+00017df0: 2020 2020 2020 202d 2053 5953 5f54 494d         - SYS_TIM
+00017e00: 450a 2020 2020 2020 2020 2020 2020 2020  E.              
+00017e10: 6472 6f70 3a0a 2020 2020 2020 2020 2020  drop:.          
+00017e20: 2020 2020 2d20 4e45 545f 4144 4d49 4e0a      - NET_ADMIN.
+00017e30: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00017e40: 5359 535f 5449 4d45 0a20 2020 2020 2020  SYS_TIME.       
+00017e50: 2020 2020 2072 756e 5f61 735f 6772 6f75       run_as_grou
+00017e60: 703a 2033 3030 300a 2020 2020 2020 2020  p: 3000.        
+00017e70: 2020 2020 7275 6e5f 6173 5f75 7365 723a      run_as_user:
+00017e80: 2031 3030 300a 2020 2020 2020 2020 6c61   1000.        la
+00017e90: 6265 6c73 3a0a 2020 2020 2020 2020 2d20  bels:.        - 
+00017ea0: 6170 703a 6465 6d6f 2d61 7070 0a20 2020  app:demo-app.   
+00017eb0: 2020 2020 202d 2076 6572 7369 6f6e 3a76       - version:v
+00017ec0: 312e 302e 300a 2020 2020 2020 2020 6166  1.0.0.        af
+00017ed0: 6669 6e69 7479 3a0a 2020 2020 2020 2020  finity:.        
+00017ee0: 2020 706f 645f 616e 7469 5f61 6666 696e    pod_anti_affin
+00017ef0: 6974 793a 0a20 2020 2020 2020 2020 2020  ity:.           
+00017f00: 2070 7265 6665 7272 6564 5f64 7572 696e   preferred_durin
+00017f10: 675f 7363 6865 6475 6c69 6e67 5f69 676e  g_scheduling_ign
+00017f20: 6f72 6564 5f64 7572 696e 675f 6578 6563  ored_during_exec
+00017f30: 7574 696f 6e3a 0a20 2020 2020 2020 2020  ution:.         
+00017f40: 2020 202d 2077 6569 6768 743a 2036 0a20     - weight: 6. 
+00017f50: 2020 2020 2020 2020 2020 2020 2070 6f64               pod
+00017f60: 5f61 6666 696e 6974 795f 7465 726d 3a0a  _affinity_term:.
+00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f80: 6c61 6265 6c5f 7365 6c65 6374 6f72 3a0a  label_selector:.
+00017f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fa0: 2d20 6170 703a 6465 6d6f 2d61 7070 0a20  - app:demo-app. 
+00017fb0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+00017fc0: 2022 6b65 793a 7665 7273 696f 6e2c 206f   "key:version, o
+00017fd0: 7065 7261 746f 723a 496e 2c20 7661 6c75  perator:In, valu
+00017fe0: 6573 3a5b 7631 2e30 2e30 2c20 7631 2e30  es:[v1.0.0, v1.0
+00017ff0: 2e31 5d22 0a20 2020 2020 2020 2020 2020  .1]".           
+00018000: 2020 2020 2074 6f70 6f6c 6f67 795f 6b65       topology_ke
+00018010: 793a 2074 6f70 6f6c 6f67 795f 6b65 790a  y: topology_key.
+00018020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018030: 6e61 6d65 7370 6163 6573 3a0a 2020 2020  namespaces:.    
+00018040: 2020 2020 2020 2020 2020 2020 2d20 6e61              - na
+00018050: 6d65 7370 6163 6573 0a20 2020 2020 2020  mespaces.       
+00018060: 2020 2020 2020 2020 202d 206e 616d 6573           - names
+00018070: 7061 6365 730a 2020 2020 2020 2020 2020  paces.          
+00018080: 2020 2d20 7765 6967 6874 3a20 360a 2020    - weight: 6.  
+00018090: 2020 2020 2020 2020 2020 2020 706f 645f              pod_
+000180a0: 6166 6669 6e69 7479 5f74 6572 6d3a 0a20  affinity_term:. 
+000180b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000180c0: 6162 656c 5f73 656c 6563 746f 723a 0a20  abel_selector:. 
+000180d0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+000180e0: 2061 7070 3a64 656d 6f2d 6170 700a 2020   app:demo-app.  
+000180f0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00018100: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
+00018110: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
+00018120: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
+00018130: 315d 220a 2020 2020 2020 2020 2020 2020  1]".            
+00018140: 2020 2020 746f 706f 6c6f 6779 5f6b 6579      topology_key
+00018150: 3a20 746f 706f 6c6f 6779 5f6b 6579 0a20  : topology_key. 
+00018160: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00018170: 616d 6573 7061 6365 733a 0a20 2020 2020  amespaces:.     
+00018180: 2020 2020 2020 2020 2020 202d 206e 616d             - nam
+00018190: 6573 7061 6365 730a 2020 2020 2020 2020  espaces.        
+000181a0: 2020 2020 2020 2020 2d20 6e61 6d65 7370          - namesp
+000181b0: 6163 6573 0a20 2020 2020 2020 2020 2020  aces.           
+000181c0: 2072 6571 7569 7265 645f 6475 7269 6e67   required_during
+000181d0: 5f73 6368 6564 756c 696e 675f 6967 6e6f  _scheduling_igno
+000181e0: 7265 645f 6475 7269 6e67 5f65 7865 6375  red_during_execu
+000181f0: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+00018200: 2020 2d20 6c61 6265 6c5f 7365 6c65 6374    - label_select
+00018210: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+00018220: 2020 2d20 6170 703a 6465 6d6f 2d61 7070    - app:demo-app
+00018230: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
+00018240: 2022 6b65 793a 7665 7273 696f 6e2c 206f   "key:version, o
+00018250: 7065 7261 746f 723a 496e 2c20 7661 6c75  perator:In, valu
+00018260: 6573 3a5b 7631 2e30 2e30 2c20 7631 2e30  es:[v1.0.0, v1.0
+00018270: 2e31 5d22 0a20 2020 2020 2020 2020 2020  .1]".           
+00018280: 2020 2074 6f70 6f6c 6f67 795f 6b65 793a     topology_key:
+00018290: 2074 6f70 6f6c 6f67 795f 6b65 790a 2020   topology_key.  
+000182a0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000182b0: 7370 6163 6573 3a0a 2020 2020 2020 2020  spaces:.        
+000182c0: 2020 2020 2020 2d20 6e61 6d65 7370 6163        - namespac
+000182d0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+000182e0: 202d 206e 616d 6573 7061 6365 730a 2020   - namespaces.  
+000182f0: 2020 2020 2020 2020 2020 2d20 6c61 6265            - labe
+00018300: 6c5f 7365 6c65 6374 6f72 3a0a 2020 2020  l_selector:.    
+00018310: 2020 2020 2020 2020 2020 2d20 6170 703a            - app:
+00018320: 6465 6d6f 2d61 7070 0a20 2020 2020 2020  demo-app.       
+00018330: 2020 2020 2020 202d 2022 6b65 793a 7665         - "key:ve
+00018340: 7273 696f 6e2c 206f 7065 7261 746f 723a  rsion, operator:
+00018350: 496e 2c20 7661 6c75 6573 3a5b 7631 2e30  In, values:[v1.0
+00018360: 2e30 2c20 7631 2e30 2e31 5d22 0a20 2020  .0, v1.0.1]".   
+00018370: 2020 2020 2020 2020 2020 2074 6f70 6f6c             topol
+00018380: 6f67 795f 6b65 793a 2074 6f70 6f6c 6f67  ogy_key: topolog
+00018390: 795f 6b65 790a 2020 2020 2020 2020 2020  y_key.          
+000183a0: 2020 2020 6e61 6d65 7370 6163 6573 3a0a      namespaces:.
+000183b0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+000183c0: 6e61 6d65 7370 6163 6573 0a20 2020 2020  namespaces.     
+000183d0: 2020 2020 2020 2020 202d 206e 616d 6573           - names
+000183e0: 7061 6365 730a 2020 2020 2020 2020 2020  paces.          
+000183f0: 6e6f 6465 5f61 6666 696e 6974 793a 0a20  node_affinity:. 
+00018400: 2020 2020 2020 2020 2020 2070 7265 6665             prefe
+00018410: 7272 6564 5f64 7572 696e 675f 7363 6865  rred_during_sche
+00018420: 6475 6c69 6e67 5f69 676e 6f72 6564 5f64  duling_ignored_d
+00018430: 7572 696e 675f 6578 6563 7574 696f 6e3a  uring_execution:
+00018440: 0a20 2020 2020 2020 2020 2020 202d 2070  .            - p
+00018450: 7265 6665 7265 6e63 653a 0a20 2020 2020  reference:.     
+00018460: 2020 2020 2020 2020 2020 206d 6174 6368             match
+00018470: 5f65 7870 7265 7373 696f 6e73 3a0a 2020  _expressions:.  
+00018480: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00018490: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
+000184a0: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
+000184b0: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
+000184c0: 315d 220a 2020 2020 2020 2020 2020 2020  1]".            
+000184d0: 2020 2020 6d61 7463 685f 6669 656c 6473      match_fields
+000184e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000184f0: 2020 2d20 226b 6579 3a76 6572 7369 6f6e    - "key:version
+00018500: 2c20 6f70 6572 6174 6f72 3a49 6e2c 2076  , operator:In, v
+00018510: 616c 7565 733a 5b76 312e 302e 302c 2076  alues:[v1.0.0, v
+00018520: 312e 302e 315d 220a 2020 2020 2020 2020  1.0.1]".        
+00018530: 2020 2020 2020 7765 6967 6874 3a20 300a        weight: 0.
+00018540: 2020 2020 2020 2020 2020 2020 2d20 7072              - pr
+00018550: 6566 6572 656e 6365 3a0a 2020 2020 2020  eference:.      
+00018560: 2020 2020 2020 2020 2020 6d61 7463 685f            match_
+00018570: 6578 7072 6573 7369 6f6e 733a 0a20 2020  expressions:.   
+00018580: 2020 2020 2020 2020 2020 2020 202d 2022               - "
+00018590: 6b65 793a 7665 7273 696f 6e2c 206f 7065  key:version, ope
+000185a0: 7261 746f 723a 496e 2c20 7661 6c75 6573  rator:In, values
+000185b0: 3a5b 7631 2e30 2e30 2c20 7631 2e30 2e31  :[v1.0.0, v1.0.1
+000185c0: 5d22 0a20 2020 2020 2020 2020 2020 2020  ]".             
+000185d0: 2020 206d 6174 6368 5f66 6965 6c64 733a     match_fields:
+000185e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000185f0: 202d 2022 6b65 793a 7665 7273 696f 6e2c   - "key:version,
+00018600: 206f 7065 7261 746f 723a 496e 2c20 7661   operator:In, va
+00018610: 6c75 6573 3a5b 7631 2e30 2e30 2c20 7631  lues:[v1.0.0, v1
+00018620: 2e30 2e31 5d22 0a20 2020 2020 2020 2020  .0.1]".         
+00018630: 2020 2020 2077 6569 6768 743a 2030 0a20       weight: 0. 
+00018640: 2020 2020 2020 2020 2020 2072 6571 7569             requi
+00018650: 7265 645f 6475 7269 6e67 5f73 6368 6564  red_during_sched
+00018660: 756c 696e 675f 6967 6e6f 7265 645f 6475  uling_ignored_du
+00018670: 7269 6e67 5f65 7865 6375 7469 6f6e 3a0a  ring_execution:.
+00018680: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00018690: 6465 5f73 656c 6563 746f 725f 7465 726d  de_selector_term
+000186a0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000186b0: 202d 206d 6174 6368 5f65 7870 7265 7373   - match_express
+000186c0: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
+000186d0: 2020 2020 2020 2d20 226b 6579 3a76 6572        - "key:ver
+000186e0: 7369 6f6e 2c20 6f70 6572 6174 6f72 3a49  sion, operator:I
+000186f0: 6e2c 2076 616c 7565 733a 5b76 312e 302e  n, values:[v1.0.
+00018700: 302c 2076 312e 302e 315d 220a 2020 2020  0, v1.0.1]".    
+00018710: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
+00018720: 685f 6669 656c 6473 3a0a 2020 2020 2020  h_fields:.      
+00018730: 2020 2020 2020 2020 2020 2d20 226b 6579            - "key
+00018740: 3a76 6572 7369 6f6e 2c20 6f70 6572 6174  :version, operat
+00018750: 6f72 3a49 6e2c 2076 616c 7565 733a 5b76  or:In, values:[v
+00018760: 312e 302e 302c 2076 312e 302e 315d 220a  1.0.0, v1.0.1]".
+00018770: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00018780: 6d61 7463 685f 6578 7072 6573 7369 6f6e  match_expression
+00018790: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000187a0: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
+000187b0: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
+000187c0: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
+000187d0: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
+000187e0: 2020 2020 2020 2020 206d 6174 6368 5f66           match_f
+000187f0: 6965 6c64 733a 0a20 2020 2020 2020 2020  ields:.         
+00018800: 2020 2020 2020 202d 2022 6b65 793a 7665         - "key:ve
+00018810: 7273 696f 6e2c 206f 7065 7261 746f 723a  rsion, operator:
+00018820: 496e 2c20 7661 6c75 6573 3a5b 7631 2e30  In, values:[v1.0
+00018830: 2e30 2c20 7631 2e30 2e31 5d22 0a20 2020  .0, v1.0.1]".   
+00018840: 2020 2020 2020 2070 6f64 5f61 6666 696e         pod_affin
+00018850: 6974 793a 0a20 2020 2020 2020 2020 2020  ity:.           
+00018860: 2070 7265 6665 7272 6564 5f64 7572 696e   preferred_durin
+00018870: 675f 7363 6865 6475 6c69 6e67 5f69 676e  g_scheduling_ign
+00018880: 6f72 6564 5f64 7572 696e 675f 6578 6563  ored_during_exec
+00018890: 7574 696f 6e3a 0a20 2020 2020 2020 2020  ution:.         
+000188a0: 2020 202d 2077 6569 6768 743a 2036 0a20     - weight: 6. 
+000188b0: 2020 2020 2020 2020 2020 2020 2070 6f64               pod
+000188c0: 5f61 6666 696e 6974 795f 7465 726d 3a0a  _affinity_term:.
+000188d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188e0: 6c61 6265 6c5f 7365 6c65 6374 6f72 3a0a  label_selector:.
+000188f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018900: 2d20 6170 703a 6465 6d6f 2d61 7070 0a20  - app:demo-app. 
+00018910: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+00018920: 2022 6b65 793a 7665 7273 696f 6e2c 206f   "key:version, o
+00018930: 7065 7261 746f 723a 496e 2c20 7661 6c75  perator:In, valu
+00018940: 6573 3a5b 7631 2e30 2e30 2c20 7631 2e30  es:[v1.0.0, v1.0
+00018950: 2e31 5d22 0a20 2020 2020 2020 2020 2020  .1]".           
+00018960: 2020 2020 2074 6f70 6f6c 6f67 795f 6b65       topology_ke
+00018970: 793a 2074 6f70 6f6c 6f67 795f 6b65 790a  y: topology_key.
+00018980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018990: 6e61 6d65 7370 6163 6573 3a0a 2020 2020  namespaces:.    
+000189a0: 2020 2020 2020 2020 2020 2020 2d20 6e61              - na
+000189b0: 6d65 7370 6163 6573 0a20 2020 2020 2020  mespaces.       
+000189c0: 2020 2020 2020 2020 202d 206e 616d 6573           - names
+000189d0: 7061 6365 730a 2020 2020 2020 2020 2020  paces.          
+000189e0: 2020 2d20 7765 6967 6874 3a20 360a 2020    - weight: 6.  
+000189f0: 2020 2020 2020 2020 2020 2020 706f 645f              pod_
+00018a00: 6166 6669 6e69 7479 5f74 6572 6d3a 0a20  affinity_term:. 
+00018a10: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00018a20: 6162 656c 5f73 656c 6563 746f 723a 0a20  abel_selector:. 
+00018a30: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+00018a40: 2061 7070 3a64 656d 6f2d 6170 700a 2020   app:demo-app.  
+00018a50: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00018a60: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
+00018a70: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
+00018a80: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
+00018a90: 315d 220a 2020 2020 2020 2020 2020 2020  1]".            
+00018aa0: 2020 2020 746f 706f 6c6f 6779 5f6b 6579      topology_key
+00018ab0: 3a20 746f 706f 6c6f 6779 5f6b 6579 0a20  : topology_key. 
+00018ac0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00018ad0: 616d 6573 7061 6365 733a 0a20 2020 2020  amespaces:.     
+00018ae0: 2020 2020 2020 2020 2020 202d 206e 616d             - nam
+00018af0: 6573 7061 6365 730a 2020 2020 2020 2020  espaces.        
+00018b00: 2020 2020 2020 2020 2d20 6e61 6d65 7370          - namesp
+00018b10: 6163 6573 0a20 2020 2020 2020 2020 2020  aces.           
+00018b20: 2072 6571 7569 7265 645f 6475 7269 6e67   required_during
+00018b30: 5f73 6368 6564 756c 696e 675f 6967 6e6f  _scheduling_igno
+00018b40: 7265 645f 6475 7269 6e67 5f65 7865 6375  red_during_execu
+00018b50: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+00018b60: 2020 2d20 6c61 6265 6c5f 7365 6c65 6374    - label_select
+00018b70: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+00018b80: 2020 2d20 6170 703a 6465 6d6f 2d61 7070    - app:demo-app
+00018b90: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
+00018ba0: 2022 6b65 793a 7665 7273 696f 6e2c 206f   "key:version, o
+00018bb0: 7065 7261 746f 723a 496e 2c20 7661 6c75  perator:In, valu
+00018bc0: 6573 3a5b 7631 2e30 2e30 2c20 7631 2e30  es:[v1.0.0, v1.0
+00018bd0: 2e31 5d22 0a20 2020 2020 2020 2020 2020  .1]".           
+00018be0: 2020 2074 6f70 6f6c 6f67 795f 6b65 793a     topology_key:
+00018bf0: 2074 6f70 6f6c 6f67 795f 6b65 790a 2020   topology_key.  
+00018c00: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00018c10: 7370 6163 6573 3a0a 2020 2020 2020 2020  spaces:.        
+00018c20: 2020 2020 2020 2d20 6e61 6d65 7370 6163        - namespac
+00018c30: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00018c40: 202d 206e 616d 6573 7061 6365 730a 2020   - namespaces.  
+00018c50: 2020 2020 2020 2020 2020 2d20 6c61 6265            - labe
+00018c60: 6c5f 7365 6c65 6374 6f72 3a0a 2020 2020  l_selector:.    
+00018c70: 2020 2020 2020 2020 2020 2d20 6170 703a            - app:
+00018c80: 6465 6d6f 2d61 7070 0a20 2020 2020 2020  demo-app.       
+00018c90: 2020 2020 2020 202d 2022 6b65 793a 7665         - "key:ve
+00018ca0: 7273 696f 6e2c 206f 7065 7261 746f 723a  rsion, operator:
+00018cb0: 496e 2c20 7661 6c75 6573 3a5b 7631 2e30  In, values:[v1.0
+00018cc0: 2e30 2c20 7631 2e30 2e31 5d22 0a20 2020  .0, v1.0.1]".   
+00018cd0: 2020 2020 2020 2020 2020 2074 6f70 6f6c             topol
+00018ce0: 6f67 795f 6b65 793a 2074 6f70 6f6c 6f67  ogy_key: topolog
+00018cf0: 795f 6b65 790a 2020 2020 2020 2020 2020  y_key.          
+00018d00: 2020 2020 6e61 6d65 7370 6163 6573 3a0a      namespaces:.
+00018d10: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00018d20: 6e61 6d65 7370 6163 6573 0a20 2020 2020  namespaces.     
+00018d30: 2020 2020 2020 2020 202d 206e 616d 6573           - names
+00018d40: 7061 6365 730a 2020 2020 2020 7072 6f70  paces.      prop
+00018d50: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
+00018d60: 6c61 6265 6c73 3a0a 2020 2020 2020 2020  labels:.        
+00018d70: 2020 6465 7363 7269 7074 696f 6e3a 204d    description: M
+00018d80: 6170 206f 6620 7374 7269 6e67 206b 6579  ap of string key
+00018d90: 7320 616e 6420 7661 6c75 6573 2074 6861  s and values tha
+00018da0: 7420 6361 6e20 6265 2075 7365 6420 746f  t can be used to
+00018db0: 206f 7267 616e 697a 650a 2020 2020 2020   organize.      
+00018dc0: 2020 2020 2020 616e 6420 6361 7465 676f        and catego
+00018dd0: 7269 7a65 2028 7363 6f70 6520 616e 6420  rize (scope and 
+00018de0: 7365 6c65 6374 2920 6f62 6a65 6374 730a  select) objects.
+00018df0: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
+00018e00: 653a 0a20 2020 2020 2020 2020 202d 2061  e:.          - a
+00018e10: 7070 3a64 656d 6f2d 6170 700a 2020 2020  pp:demo-app.    
+00018e20: 2020 2020 2020 2d20 7665 7273 696f 6e3a        - version:
+00018e30: 7631 2e30 2e30 0a20 2020 2020 2020 2020  v1.0.0.         
+00018e40: 2069 7465 6d73 3a0a 2020 2020 2020 2020   items:.        
+00018e50: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+00018e60: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
+00018e70: 3a20 4c61 6265 6c73 0a20 2020 2020 2020  : Labels.       
+00018e80: 2020 2074 7970 653a 2061 7272 6179 0a20     type: array. 
+00018e90: 2020 2020 2020 2061 6e6e 6f74 6174 696f         annotatio
+00018ea0: 6e73 3a0a 2020 2020 2020 2020 2020 6465  ns:.          de
+00018eb0: 7363 7269 7074 696f 6e3a 2041 6e20 756e  scription: An un
+00018ec0: 7374 7275 6374 7572 6564 206b 6579 2076  structured key v
+00018ed0: 616c 7565 206d 6170 2074 6861 7420 6361  alue map that ca
+00018ee0: 6e20 6265 2075 7365 6420 746f 2061 7474  n be used to att
+00018ef0: 6163 6820 6172 6269 7472 6172 790a 2020  ach arbitrary.  
+00018f00: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+00018f10: 7461 0a20 2020 2020 2020 2020 2065 7861  ta.          exa
+00018f20: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
+00018f30: 2d20 616e 6e6f 7461 7469 6f6e 2d6b 6579  - annotation-key
+00018f40: 313a 7661 6c31 0a20 2020 2020 2020 2020  1:val1.         
+00018f50: 202d 2061 6e6e 6f74 6174 696f 6e2d 6b65   - annotation-ke
+00018f60: 7932 3a76 616c 320a 2020 2020 2020 2020  y2:val2.        
+00018f70: 2020 6974 656d 733a 0a20 2020 2020 2020    items:.       
+00018f80: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+00018f90: 670a 2020 2020 2020 2020 2020 7469 746c  g.          titl
+00018fa0: 653a 2041 6e6e 6f74 6174 696f 6e73 0a20  e: Annotations. 
+00018fb0: 2020 2020 2020 2020 2074 7970 653a 2061           type: a
+00018fc0: 7272 6179 0a20 2020 2020 2020 2063 6f6e  rray.        con
+00018fd0: 7461 696e 6572 733a 0a20 2020 2020 2020  tainers:.       
+00018fe0: 2020 2069 7465 6d73 3a0a 2020 2020 2020     items:.      
+00018ff0: 2020 2020 2020 2472 6566 3a20 2723 2f63        $ref: '#/c
+00019000: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00019010: 732f 436f 6e74 6169 6e65 7227 0a20 2020  s/Container'.   
+00019020: 2020 2020 2020 2074 6974 6c65 3a20 636f         title: co
+00019030: 6e74 6169 6e65 7273 0a20 2020 2020 2020  ntainers.       
+00019040: 2020 2074 7970 653a 2061 7272 6179 0a20     type: array. 
+00019050: 2020 2020 2020 2076 6f6c 756d 6573 3a0a         volumes:.
+00019060: 2020 2020 2020 2020 2020 6974 656d 733a            items:
+00019070: 0a20 2020 2020 2020 2020 2020 2024 7265  .            $re
+00019080: 663a 2027 232f 636f 6d70 6f6e 656e 7473  f: '#/components
+00019090: 2f73 6368 656d 6173 2f56 6f6c 756d 6527  /schemas/Volume'
+000190a0: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
+000190b0: 3a20 766f 6c75 6d65 730a 2020 2020 2020  : volumes.      
+000190c0: 2020 2020 7479 7065 3a20 6172 7261 790a      type: array.
+000190d0: 2020 2020 2020 2020 6166 6669 6e69 7479          affinity
+000190e0: 3a0a 2020 2020 2020 2020 2020 2472 6566  :.          $ref
+000190f0: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
+00019100: 7363 6865 6d61 732f 4166 6669 6e69 7479  schemas/Affinity
+00019110: 270a 2020 2020 2020 7469 746c 653a 2050  '.      title: P
+00019120: 6f64 0a20 2020 2020 2074 7970 653a 206f  od.      type: o
+00019130: 626a 6563 740a 2020 2020 436f 6e74 6169  bject.    Contai
+00019140: 6e65 723a 0a20 2020 2020 2065 7861 6d70  ner:.      examp
+00019150: 6c65 3a0a 2020 2020 2020 2020 696d 6167  le:.        imag
+00019160: 653a 206e 6769 6e78 3a6c 6174 6573 740a  e: nginx:latest.
+00019170: 2020 2020 2020 2020 6c69 6665 5f63 7963          life_cyc
+00019180: 6c65 3a0a 2020 2020 2020 2020 2020 7072  le:.          pr
+00019190: 655f 7374 6f70 3a0a 2020 2020 2020 2020  e_stop:.        
+000191a0: 2020 2020 7463 705f 736f 636b 6574 3a0a      tcp_socket:.
+000191b0: 2020 2020 2020 2020 2020 2020 2020 706f                po
+000191c0: 7274 3a20 3330 3138 310a 2020 2020 2020  rt: 30181.      
+000191d0: 2020 2020 2020 2020 686f 7374 3a20 3132          host: 12
+000191e0: 372e 302e 302e 310a 2020 2020 2020 2020  7.0.0.1.        
+000191f0: 2020 2020 6874 7470 5f67 6574 3a0a 2020      http_get:.  
+00019200: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00019210: 3a20 2f73 686f 773f 646f 6d61 696e 3d76  : /show?domain=v
+00019220: 3139 2e74 696b 746f 6b63 646e 2e63 6f6d  19.tiktokcdn.com
+00019230: 0a20 2020 2020 2020 2020 2020 2020 2068  .              h
+00019240: 7474 705f 6865 6164 6572 733a 0a20 2020  ttp_headers:.   
+00019250: 2020 2020 2020 2020 2020 202d 2078 2d64             - x-d
+00019260: 6576 7372 652d 6175 7468 6f72 697a 6174  evsre-authorizat
+00019270: 696f 6e3a 4265 6172 6572 2065 794a 6862  ion:Bearer eyJhb
+00019280: 4763 694f 694a 0a20 2020 2020 2020 2020  GciOiJ.         
+00019290: 2020 2020 202d 2063 6f6e 7465 6e74 2d74       - content-t
+000192a0: 7970 653a 6170 706c 6963 6174 696f 6e2f  ype:application/
+000192b0: 6a73 6f6e 0a20 2020 2020 2020 2020 2020  json.           
+000192c0: 2020 2073 6368 656d 653a 2048 5454 5053     scheme: HTTPS
+000192d0: 0a20 2020 2020 2020 2020 2020 2020 2070  .              p
+000192e0: 6f72 743a 2038 3838 380a 2020 2020 2020  ort: 8888.      
+000192f0: 2020 2020 2020 2020 686f 7374 3a20 6773          host: gs
+00019300: 732d 646e 732d 6167 656e 742e 6578 616d  s-dns-agent.exam
+00019310: 706c 652e 6f72 670a 2020 2020 2020 2020  ple.org.        
+00019320: 2020 2020 6578 6563 5f63 6f6d 6d61 6e64      exec_command
+00019330: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
+00019340: 2f62 696e 2f73 686f 7764 6f77 6e2e 7368  /bin/showdown.sh
+00019350: 0a20 2020 2020 2020 2020 2070 6f73 745f  .          post_
+00019360: 7374 6172 743a 0a20 2020 2020 2020 2020  start:.         
+00019370: 2020 2074 6370 5f73 6f63 6b65 743a 0a20     tcp_socket:. 
+00019380: 2020 2020 2020 2020 2020 2020 2070 6f72               por
+00019390: 743a 2033 3031 3831 0a20 2020 2020 2020  t: 30181.       
+000193a0: 2020 2020 2020 2068 6f73 743a 2031 3237         host: 127
+000193b0: 2e30 2e30 2e31 0a20 2020 2020 2020 2020  .0.0.1.         
+000193c0: 2020 2068 7474 705f 6765 743a 0a20 2020     http_get:.   
+000193d0: 2020 2020 2020 2020 2020 2070 6174 683a             path:
+000193e0: 202f 7368 6f77 3f64 6f6d 6169 6e3d 7631   /show?domain=v1
+000193f0: 392e 7469 6b74 6f6b 6364 6e2e 636f 6d0a  9.tiktokcdn.com.
+00019400: 2020 2020 2020 2020 2020 2020 2020 6874                ht
+00019410: 7470 5f68 6561 6465 7273 3a0a 2020 2020  tp_headers:.    
+00019420: 2020 2020 2020 2020 2020 2d20 782d 6465            - x-de
+00019430: 7673 7265 2d61 7574 686f 7269 7a61 7469  vsre-authorizati
+00019440: 6f6e 3a42 6561 7265 7220 6579 4a68 6247  on:Bearer eyJhbG
+00019450: 6369 4f69 4a0a 2020 2020 2020 2020 2020  ciOiJ.          
+00019460: 2020 2020 2d20 636f 6e74 656e 742d 7479      - content-ty
+00019470: 7065 3a61 7070 6c69 6361 7469 6f6e 2f6a  pe:application/j
+00019480: 736f 6e0a 2020 2020 2020 2020 2020 2020  son.            
+00019490: 2020 7363 6865 6d65 3a20 4854 5450 530a    scheme: HTTPS.
+000194a0: 2020 2020 2020 2020 2020 2020 2020 706f                po
+000194b0: 7274 3a20 3838 3838 0a20 2020 2020 2020  rt: 8888.       
+000194c0: 2020 2020 2020 2068 6f73 743a 2067 7373         host: gss
+000194d0: 2d64 6e73 2d61 6765 6e74 2e65 7861 6d70  -dns-agent.examp
+000194e0: 6c65 2e6f 7267 0a20 2020 2020 2020 2020  le.org.         
+000194f0: 2020 2065 7865 635f 636f 6d6d 616e 643a     exec_command:
+00019500: 0a20 2020 2020 2020 2020 2020 202d 202f  .            - /
+00019510: 6269 6e2f 7368 6f77 646f 776e 2e73 680a  bin/showdown.sh.
+00019520: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+00019530: 733a 0a20 2020 2020 2020 2020 2072 6571  s:.          req
+00019540: 7565 7374 733a 0a20 2020 2020 2020 2020  uests:.         
+00019550: 2020 206d 656d 6f72 793a 2032 3536 4d69     memory: 256Mi
+00019560: 0a20 2020 2020 2020 2020 2020 2063 7075  .            cpu
+00019570: 3a20 2230 2e31 220a 2020 2020 2020 2020  : "0.1".        
+00019580: 2020 6c69 6d69 7473 3a0a 2020 2020 2020    limits:.      
+00019590: 2020 2020 2020 6d65 6d6f 7279 3a20 3531        memory: 51
+000195a0: 324d 690a 2020 2020 2020 2020 2020 2020  2Mi.            
+000195b0: 6370 753a 2022 302e 3522 0a20 2020 2020  cpu: "0.5".     
+000195c0: 2020 2076 6f6c 756d 655f 6d6f 756e 7473     volume_mounts
+000195d0: 3a0a 2020 2020 2020 2020 2d20 7061 7468  :.        - path
+000195e0: 3a20 2f6f 7074 2f73 6572 7665 722f 636f  : /opt/server/co
+000195f0: 6e66 0a20 2020 2020 2020 2020 2072 6561  nf.          rea
+00019600: 645f 6f6e 6c79 3a20 7472 7565 0a20 2020  d_only: true.   
+00019610: 2020 2020 2020 206e 616d 653a 2064 656d         name: dem
+00019620: 6f2d 766f 6c0a 2020 2020 2020 2020 2020  o-vol.          
+00019630: 7375 625f 7061 7468 3a20 7365 7276 6572  sub_path: server
+00019640: 2e63 6f6e 660a 2020 2020 2020 2020 2d20  .conf.        - 
+00019650: 7061 7468 3a20 2f6f 7074 2f73 6572 7665  path: /opt/serve
+00019660: 722f 636f 6e66 0a20 2020 2020 2020 2020  r/conf.         
+00019670: 2072 6561 645f 6f6e 6c79 3a20 7472 7565   read_only: true
+00019680: 0a20 2020 2020 2020 2020 206e 616d 653a  .          name:
+00019690: 2064 656d 6f2d 766f 6c0a 2020 2020 2020   demo-vol.      
+000196a0: 2020 2020 7375 625f 7061 7468 3a20 7365      sub_path: se
+000196b0: 7276 6572 2e63 6f6e 660a 2020 2020 2020  rver.conf.      
+000196c0: 2020 656e 763a 0a20 2020 2020 2020 2020    env:.         
+000196d0: 206e 616d 653a 2053 4d53 5f4b 4559 535f   name: SMS_KEYS_
+000196e0: 5041 5448 5f58 4d0a 2020 2020 2020 2020  PATH_XM.        
+000196f0: 2020 7661 6c75 653a 2064 6d73 2d73 6563    value: dms-sec
+00019700: 7265 740a 2020 2020 2020 2020 706f 7274  ret.        port
+00019710: 733a 0a20 2020 2020 2020 202d 2063 6f6e  s:.        - con
+00019720: 7461 696e 6572 5f70 6f72 743a 2038 300a  tainer_port: 80.
+00019730: 2020 2020 2020 2020 2020 7072 6f74 6f63            protoc
+00019740: 6f6c 3a20 5443 500a 2020 2020 2020 2020  ol: TCP.        
+00019750: 2020 6e61 6d65 3a20 6874 7470 0a20 2020    name: http.   
+00019760: 2020 2020 202d 2063 6f6e 7461 696e 6572       - container
+00019770: 5f70 6f72 743a 2038 300a 2020 2020 2020  _port: 80.      
+00019780: 2020 2020 7072 6f74 6f63 6f6c 3a20 5443      protocol: TC
+00019790: 500a 2020 2020 2020 2020 2020 6e61 6d65  P.          name
+000197a0: 3a20 6874 7470 0a20 2020 2020 2020 2063  : http.        c
+000197b0: 6f6d 6d61 6e64 3a0a 2020 2020 2020 2020  ommand:.        
+000197c0: 2d20 7079 7468 6f6e 330a 2020 2020 2020  - python3.      
+000197d0: 2020 6172 6773 3a0a 2020 2020 2020 2020    args:.        
+000197e0: 2d20 2d6d 0a20 2020 2020 2020 202d 206f  - -m.        - o
+000197f0: 7065 6e61 7069 5f73 6572 7665 720a 2020  penapi_server.  
+00019800: 2020 2020 2020 7265 6164 696e 6573 735f        readiness_
+00019810: 7072 6f62 653a 0a20 2020 2020 2020 2020  probe:.         
+00019820: 2070 6572 696f 645f 7365 636f 6e64 733a   period_seconds:
+00019830: 2036 300a 2020 2020 2020 2020 2020 696e   60.          in
+00019840: 6974 6961 6c5f 6465 6c61 795f 7365 636f  itial_delay_seco
+00019850: 6e64 733a 2036 3030 0a20 2020 2020 2020  nds: 600.       
+00019860: 2020 2074 6370 5f73 6f63 6b65 743a 0a20     tcp_socket:. 
+00019870: 2020 2020 2020 2020 2020 2070 6f72 743a             port:
+00019880: 2033 3031 3831 0a20 2020 2020 2020 2020   30181.         
+00019890: 2020 2068 6f73 743a 2031 3237 2e30 2e30     host: 127.0.0
+000198a0: 2e31 0a20 2020 2020 2020 2020 2066 6169  .1.          fai
+000198b0: 6c75 7265 5f74 6872 6573 686f 6c64 3a20  lure_threshold: 
+000198c0: 330a 2020 2020 2020 2020 2020 6874 7470  3.          http
+000198d0: 5f67 6574 3a0a 2020 2020 2020 2020 2020  _get:.          
+000198e0: 2020 7061 7468 3a20 2f73 686f 773f 646f    path: /show?do
+000198f0: 6d61 696e 3d76 3139 2e74 696b 746f 6b63  main=v19.tiktokc
+00019900: 646e 2e63 6f6d 0a20 2020 2020 2020 2020  dn.com.         
+00019910: 2020 2068 7474 705f 6865 6164 6572 733a     http_headers:
+00019920: 0a20 2020 2020 2020 2020 2020 202d 2078  .            - x
+00019930: 2d64 6576 7372 652d 6175 7468 6f72 697a  -devsre-authoriz
+00019940: 6174 696f 6e3a 4265 6172 6572 2065 794a  ation:Bearer eyJ
+00019950: 6862 4763 694f 694a 0a20 2020 2020 2020  hbGciOiJ.       
+00019960: 2020 2020 202d 2063 6f6e 7465 6e74 2d74       - content-t
+00019970: 7970 653a 6170 706c 6963 6174 696f 6e2f  ype:application/
+00019980: 6a73 6f6e 0a20 2020 2020 2020 2020 2020  json.           
+00019990: 2073 6368 656d 653a 2048 5454 5053 0a20   scheme: HTTPS. 
+000199a0: 2020 2020 2020 2020 2020 2070 6f72 743a             port:
+000199b0: 2038 3838 380a 2020 2020 2020 2020 2020   8888.          
+000199c0: 2020 686f 7374 3a20 6773 732d 646e 732d    host: gss-dns-
+000199d0: 6167 656e 742e 6578 616d 706c 652e 6f72  agent.example.or
+000199e0: 670a 2020 2020 2020 2020 2020 7469 6d65  g.          time
+000199f0: 6f75 745f 7365 636f 6e64 733a 2036 300a  out_seconds: 60.
+00019a00: 2020 2020 2020 2020 2020 6578 6563 5f63            exec_c
+00019a10: 6f6d 6d61 6e64 3a0a 2020 2020 2020 2020  ommand:.        
+00019a20: 2020 2d20 2f67 7373 2f64 696e 676d 616e    - /gss/dingman
+00019a30: 2f62 696e 2f64 696e 676d 616e 2d63 6c69  /bin/dingman-cli
+00019a40: 740a 2020 2020 2020 2020 2020 2d20 2d61  t.          - -a
+00019a50: 6464 7265 7373 0a20 2020 2020 2020 2020  ddress.         
+00019a60: 202d 2031 3237 2e30 2e30 2e31 3a33 3035   - 127.0.0.1:305
+00019a70: 3031 0a20 2020 2020 2020 2020 202d 202d  01.          - -
+00019a80: 636f 6d6d 616e 640a 2020 2020 2020 2020  command.        
+00019a90: 2020 2d20 7368 6f77 2070 6f70 3a61 6c6c    - show pop:all
+00019aa0: 2073 756d 6d61 7279 3a68 6561 6c74 682d   summary:health-
+00019ab0: 7374 6174 7573 0a20 2020 2020 2020 2065  status.        e
+00019ac0: 6e76 5f66 726f 6d3a 2052 6567 756c 6172  nv_from: Regular
+00019ad0: 0a20 2020 2020 2020 2073 7461 7274 7570  .        startup
+00019ae0: 5f70 726f 6265 3a0a 2020 2020 2020 2020  _probe:.        
+00019af0: 2020 7065 7269 6f64 5f73 6563 6f6e 6473    period_seconds
+00019b00: 3a20 3630 0a20 2020 2020 2020 2020 2069  : 60.          i
+00019b10: 6e69 7469 616c 5f64 656c 6179 5f73 6563  nitial_delay_sec
+00019b20: 6f6e 6473 3a20 3630 300a 2020 2020 2020  onds: 600.      
+00019b30: 2020 2020 7463 705f 736f 636b 6574 3a0a      tcp_socket:.
+00019b40: 2020 2020 2020 2020 2020 2020 706f 7274              port
+00019b50: 3a20 3330 3138 310a 2020 2020 2020 2020  : 30181.        
+00019b60: 2020 2020 686f 7374 3a20 3132 372e 302e      host: 127.0.
+00019b70: 302e 310a 2020 2020 2020 2020 2020 6661  0.1.          fa
+00019b80: 696c 7572 655f 7468 7265 7368 6f6c 643a  ilure_threshold:
+00019b90: 2033 0a20 2020 2020 2020 2020 2068 7474   3.          htt
+00019ba0: 705f 6765 743a 0a20 2020 2020 2020 2020  p_get:.         
+00019bb0: 2020 2070 6174 683a 202f 7368 6f77 3f64     path: /show?d
+00019bc0: 6f6d 6169 6e3d 7631 392e 7469 6b74 6f6b  omain=v19.tiktok
+00019bd0: 6364 6e2e 636f 6d0a 2020 2020 2020 2020  cdn.com.        
+00019be0: 2020 2020 6874 7470 5f68 6561 6465 7273      http_headers
+00019bf0: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
+00019c00: 782d 6465 7673 7265 2d61 7574 686f 7269  x-devsre-authori
+00019c10: 7a61 7469 6f6e 3a42 6561 7265 7220 6579  zation:Bearer ey
+00019c20: 4a68 6247 6369 4f69 4a0a 2020 2020 2020  JhbGciOiJ.      
+00019c30: 2020 2020 2020 2d20 636f 6e74 656e 742d        - content-
+00019c40: 7479 7065 3a61 7070 6c69 6361 7469 6f6e  type:application
+00019c50: 2f6a 736f 6e0a 2020 2020 2020 2020 2020  /json.          
+00019c60: 2020 7363 6865 6d65 3a20 4854 5450 530a    scheme: HTTPS.
+00019c70: 2020 2020 2020 2020 2020 2020 706f 7274              port
+00019c80: 3a20 3838 3838 0a20 2020 2020 2020 2020  : 8888.         
+00019c90: 2020 2068 6f73 743a 2067 7373 2d64 6e73     host: gss-dns
+00019ca0: 2d61 6765 6e74 2e65 7861 6d70 6c65 2e6f  -agent.example.o
+00019cb0: 7267 0a20 2020 2020 2020 2020 2074 696d  rg.          tim
+00019cc0: 656f 7574 5f73 6563 6f6e 6473 3a20 3630  eout_seconds: 60
+00019cd0: 0a20 2020 2020 2020 2020 2065 7865 635f  .          exec_
+00019ce0: 636f 6d6d 616e 643a 0a20 2020 2020 2020  command:.       
+00019cf0: 2020 202d 202f 6773 732f 6469 6e67 6d61     - /gss/dingma
+00019d00: 6e2f 6269 6e2f 6469 6e67 6d61 6e2d 636c  n/bin/dingman-cl
+00019d10: 6974 0a20 2020 2020 2020 2020 202d 202d  it.          - -
+00019d20: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
+00019d30: 2020 2d20 3132 372e 302e 302e 313a 3330    - 127.0.0.1:30
+00019d40: 3530 310a 2020 2020 2020 2020 2020 2d20  501.          - 
+00019d50: 2d63 6f6d 6d61 6e64 0a20 2020 2020 2020  -command.       
+00019d60: 2020 202d 2073 686f 7720 706f 703a 616c     - show pop:al
+00019d70: 6c20 7375 6d6d 6172 793a 6865 616c 7468  l summary:health
+00019d80: 2d73 7461 7475 730a 2020 2020 2020 2020  -status.        
+00019d90: 696d 6167 655f 7075 6c6c 5f70 6f6c 6963  image_pull_polic
+00019da0: 793a 2049 664e 6f74 5072 6573 656e 740a  y: IfNotPresent.
+00019db0: 2020 2020 2020 2020 766f 6c75 6d65 5f64          volume_d
+00019dc0: 6576 6963 6573 3a0a 2020 2020 2020 2020  evices:.        
+00019dd0: 2d20 6e61 6d65 3a20 6465 6d6f 2d76 6f6c  - name: demo-vol
+00019de0: 0a20 2020 2020 2020 2020 2064 6576 6963  .          devic
+00019df0: 655f 7061 7468 3a20 2f64 6576 2f73 6461  e_path: /dev/sda
+00019e00: 310a 2020 2020 2020 2020 2020 6263 6163  1.          bcac
+00019e10: 6865 5f6e 756d 733a 2034 0a20 2020 2020  he_nums: 4.     
+00019e20: 2020 202d 206e 616d 653a 2064 656d 6f2d     - name: demo-
+00019e30: 766f 6c0a 2020 2020 2020 2020 2020 6465  vol.          de
+00019e40: 7669 6365 5f70 6174 683a 202f 6465 762f  vice_path: /dev/
+00019e50: 7364 6131 0a20 2020 2020 2020 2020 2062  sda1.          b
+00019e60: 6361 6368 655f 6e75 6d73 3a20 340a 2020  cache_nums: 4.  
+00019e70: 2020 2020 2020 6e61 6d65 3a20 6874 7470        name: http
+00019e80: 2d73 6572 7665 720a 2020 2020 2020 2020  -server.        
+00019e90: 636f 6e74 6169 6e65 725f 7479 7065 3a20  container_type: 
+00019ea0: 496e 6974 0a20 2020 2020 2020 206c 6976  Init.        liv
+00019eb0: 656e 6573 735f 7072 6f62 653a 0a20 2020  eness_probe:.   
+00019ec0: 2020 2020 2020 2070 6572 696f 645f 7365         period_se
+00019ed0: 636f 6e64 733a 2036 300a 2020 2020 2020  conds: 60.      
+00019ee0: 2020 2020 696e 6974 6961 6c5f 6465 6c61      initial_dela
+00019ef0: 795f 7365 636f 6e64 733a 2036 3030 0a20  y_seconds: 600. 
+00019f00: 2020 2020 2020 2020 2074 6370 5f73 6f63           tcp_soc
+00019f10: 6b65 743a 0a20 2020 2020 2020 2020 2020  ket:.           
+00019f20: 2070 6f72 743a 2033 3031 3831 0a20 2020   port: 30181.   
+00019f30: 2020 2020 2020 2020 2068 6f73 743a 2031           host: 1
+00019f40: 3237 2e30 2e30 2e31 0a20 2020 2020 2020  27.0.0.1.       
+00019f50: 2020 2066 6169 6c75 7265 5f74 6872 6573     failure_thres
+00019f60: 686f 6c64 3a20 330a 2020 2020 2020 2020  hold: 3.        
+00019f70: 2020 6874 7470 5f67 6574 3a0a 2020 2020    http_get:.    
+00019f80: 2020 2020 2020 2020 7061 7468 3a20 2f73          path: /s
+00019f90: 686f 773f 646f 6d61 696e 3d76 3139 2e74  how?domain=v19.t
+00019fa0: 696b 746f 6b63 646e 2e63 6f6d 0a20 2020  iktokcdn.com.   
+00019fb0: 2020 2020 2020 2020 2068 7474 705f 6865           http_he
+00019fc0: 6164 6572 733a 0a20 2020 2020 2020 2020  aders:.         
+00019fd0: 2020 202d 2078 2d64 6576 7372 652d 6175     - x-devsre-au
+00019fe0: 7468 6f72 697a 6174 696f 6e3a 4265 6172  thorization:Bear
+00019ff0: 6572 2065 794a 6862 4763 694f 694a 0a20  er eyJhbGciOiJ. 
+0001a000: 2020 2020 2020 2020 2020 202d 2063 6f6e             - con
+0001a010: 7465 6e74 2d74 7970 653a 6170 706c 6963  tent-type:applic
+0001a020: 6174 696f 6e2f 6a73 6f6e 0a20 2020 2020  ation/json.     
+0001a030: 2020 2020 2020 2073 6368 656d 653a 2048         scheme: H
+0001a040: 5454 5053 0a20 2020 2020 2020 2020 2020  TTPS.           
+0001a050: 2070 6f72 743a 2038 3838 380a 2020 2020   port: 8888.    
+0001a060: 2020 2020 2020 2020 686f 7374 3a20 6773          host: gs
+0001a070: 732d 646e 732d 6167 656e 742e 6578 616d  s-dns-agent.exam
+0001a080: 706c 652e 6f72 670a 2020 2020 2020 2020  ple.org.        
+0001a090: 2020 7469 6d65 6f75 745f 7365 636f 6e64    timeout_second
+0001a0a0: 733a 2036 300a 2020 2020 2020 2020 2020  s: 60.          
+0001a0b0: 6578 6563 5f63 6f6d 6d61 6e64 3a0a 2020  exec_command:.  
+0001a0c0: 2020 2020 2020 2020 2d20 2f67 7373 2f64          - /gss/d
+0001a0d0: 696e 676d 616e 2f62 696e 2f64 696e 676d  ingman/bin/dingm
+0001a0e0: 616e 2d63 6c69 740a 2020 2020 2020 2020  an-clit.        
+0001a0f0: 2020 2d20 2d61 6464 7265 7373 0a20 2020    - -address.   
+0001a100: 2020 2020 2020 202d 2031 3237 2e30 2e30         - 127.0.0
+0001a110: 2e31 3a33 3035 3031 0a20 2020 2020 2020  .1:30501.       
+0001a120: 2020 202d 202d 636f 6d6d 616e 640a 2020     - -command.  
+0001a130: 2020 2020 2020 2020 2d20 7368 6f77 2070          - show p
+0001a140: 6f70 3a61 6c6c 2073 756d 6d61 7279 3a68  op:all summary:h
+0001a150: 6561 6c74 682d 7374 6174 7573 0a20 2020  ealth-status.   
+0001a160: 2020 2020 2073 6563 7572 6974 795f 636f       security_co
+0001a170: 6e74 6578 743a 0a20 2020 2020 2020 2020  ntext:.         
+0001a180: 2063 6170 6162 696c 6974 6965 733a 0a20   capabilities:. 
+0001a190: 2020 2020 2020 2020 2020 2061 6464 3a0a             add:.
+0001a1a0: 2020 2020 2020 2020 2020 2020 2d20 4e45              - NE
+0001a1b0: 545f 4144 4d49 4e0a 2020 2020 2020 2020  T_ADMIN.        
+0001a1c0: 2020 2020 2d20 5359 535f 5449 4d45 0a20      - SYS_TIME. 
+0001a1d0: 2020 2020 2020 2020 2020 2064 726f 703a             drop:
+0001a1e0: 0a20 2020 2020 2020 2020 2020 202d 204e  .            - N
+0001a1f0: 4554 5f41 444d 494e 0a20 2020 2020 2020  ET_ADMIN.       
+0001a200: 2020 2020 202d 2053 5953 5f54 494d 450a       - SYS_TIME.
+0001a210: 2020 2020 2020 2020 2020 7275 6e5f 6173            run_as
+0001a220: 5f67 726f 7570 3a20 3330 3030 0a20 2020  _group: 3000.   
+0001a230: 2020 2020 2020 2072 756e 5f61 735f 7573         run_as_us
+0001a240: 6572 3a20 3130 3030 0a20 2020 2020 2070  er: 1000.      p
+0001a250: 726f 7065 7274 6965 733a 0a20 2020 2020  roperties:.     
+0001a260: 2020 206e 616d 653a 0a20 2020 2020 2020     name:.       
+0001a270: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+0001a280: 7c0a 2020 2020 2020 2020 2020 2020 4e61  |.            Na
+0001a290: 6d65 206f 6620 7468 6520 636f 6e74 6169  me of the contai
+0001a2a0: 6e65 7220 7370 6563 6966 6965 6420 6173  ner specified as
+0001a2b0: 2061 2044 4e53 5f4c 4142 454c 2e20 4561   a DNS_LABEL. Ea
+0001a2c0: 6368 2063 6f6e 7461 696e 6572 2069 6e20  ch container in 
+0001a2d0: 6120 706f 6420 6d75 7374 2068 6176 6520  a pod must have 
+0001a2e0: 6120 756e 6971 7565 206e 616d 6520 2844  a unique name (D
+0001a2f0: 4e53 5f4c 4142 454c 292e 0a20 2020 2020  NS_LABEL)..     
+0001a300: 2020 2020 2020 2043 616e 6e6f 7420 6265         Cannot be
+0001a310: 2075 7064 6174 6564 0a20 2020 2020 2020   updated.       
+0001a320: 2020 2065 7861 6d70 6c65 3a20 6874 7470     example: http
+0001a330: 2d73 6572 7665 720a 2020 2020 2020 2020  -server.        
+0001a340: 2020 7469 746c 653a 206e 616d 650a 2020    title: name.  
+0001a350: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
+0001a360: 7269 6e67 0a20 2020 2020 2020 2063 6f6e  ring.        con
+0001a370: 7461 696e 6572 5f74 7970 653a 0a20 2020  tainer_type:.   
+0001a380: 2020 2020 2020 2065 6e75 6d3a 0a20 2020         enum:.   
+0001a390: 2020 2020 2020 202d 2049 6e69 740a 2020         - Init.  
+0001a3a0: 2020 2020 2020 2020 2d20 5265 6775 6c61          - Regula
+0001a3b0: 720a 2020 2020 2020 2020 2020 7469 746c  r.          titl
+0001a3c0: 653a 2063 6f6e 7461 696e 6572 5f74 7970  e: container_typ
+0001a3d0: 650a 2020 2020 2020 2020 2020 7479 7065  e.          type
+0001a3e0: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+0001a3f0: 2065 6e76 3a0a 2020 2020 2020 2020 2020   env:.          
+0001a400: 6465 7363 7269 7074 696f 6e3a 204c 6973  description: Lis
+0001a410: 7420 6f66 2065 6e76 6972 6f6e 6d65 6e74  t of environment
+0001a420: 2076 6172 6961 626c 6573 2074 6f20 7365   variables to se
+0001a430: 7420 696e 2074 6865 2063 6f6e 7461 696e  t in the contain
+0001a440: 6572 2e0a 2020 2020 2020 2020 2020 6578  er..          ex
+0001a450: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
+0001a460: 2020 206e 616d 653a 2053 4d53 5f4b 4559     name: SMS_KEY
+0001a470: 535f 5041 5448 5f58 4d0a 2020 2020 2020  S_PATH_XM.      
+0001a480: 2020 2020 2020 7661 6c75 653a 2064 6d73        value: dms
+0001a490: 2d73 6563 7265 740a 2020 2020 2020 2020  -secret.        
+0001a4a0: 2020 6974 656d 733a 0a20 2020 2020 2020    items:.       
+0001a4b0: 2020 2020 2024 7265 663a 2027 232f 636f       $ref: '#/co
+0001a4c0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+0001a4d0: 2f45 6e76 5661 7227 0a20 2020 2020 2020  /EnvVar'.       
+0001a4e0: 2020 2074 6974 6c65 3a20 656e 760a 2020     title: env.  
+0001a4f0: 2020 2020 2020 2020 7479 7065 3a20 6172          type: ar
+0001a500: 7261 790a 2020 2020 2020 2020 656e 765f  ray.        env_
+0001a510: 6672 6f6d 3a0a 2020 2020 2020 2020 2020  from:.          
+0001a520: 6465 7363 7269 7074 696f 6e3a 204c 6973  description: Lis
+0001a530: 7420 6f66 2073 6f75 7263 6573 2074 6f20  t of sources to 
+0001a540: 706f 7075 6c61 7465 2065 6e76 6972 6f6e  populate environ
+0001a550: 6d65 6e74 2076 6172 6961 626c 6573 2069  ment variables i
+0001a560: 6e20 7468 6520 636f 6e74 6169 6e65 722e  n the container.
+0001a570: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
+0001a580: 6c65 3a20 5265 6775 6c61 720a 2020 2020  le: Regular.    
+0001a590: 2020 2020 2020 6974 656d 733a 0a20 2020        items:.   
+0001a5a0: 2020 2020 2020 2020 2024 7265 663a 2027           $ref: '
+0001a5b0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+0001a5c0: 656d 6173 2f45 6e76 4672 6f6d 536f 7572  emas/EnvFromSour
+0001a5d0: 6365 270a 2020 2020 2020 2020 2020 7469  ce'.          ti
+0001a5e0: 746c 653a 2065 6e76 5f66 726f 6d0a 2020  tle: env_from.  
+0001a5f0: 2020 2020 2020 2020 7479 7065 3a20 6172          type: ar
+0001a600: 7261 790a 2020 2020 2020 2020 696d 6167  ray.        imag
+0001a610: 653a 0a20 2020 2020 2020 2020 2064 6573  e:.          des
+0001a620: 6372 6970 7469 6f6e 3a20 446f 636b 6572  cription: Docker
+0001a630: 2069 6d61 6765 2075 726c 0a20 2020 2020   image url.     
+0001a640: 2020 2020 2065 7861 6d70 6c65 3a20 6e67       example: ng
+0001a650: 696e 783a 6c61 7465 7374 0a20 2020 2020  inx:latest.     
+0001a660: 2020 2020 2074 6974 6c65 3a20 696d 6167       title: imag
+0001a670: 650a 2020 2020 2020 2020 2020 7479 7065  e.          type
+0001a680: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+0001a690: 2069 6d61 6765 5f70 756c 6c5f 706f 6c69   image_pull_poli
+0001a6a0: 6379 3a0a 2020 2020 2020 2020 2020 6465  cy:.          de
+0001a6b0: 7363 7269 7074 696f 6e3a 2044 6566 6175  scription: Defau
+0001a6c0: 6c74 7320 746f 2041 6c77 6179 730a 2020  lts to Always.  
+0001a6d0: 2020 2020 2020 2020 656e 756d 3a0a 2020          enum:.  
+0001a6e0: 2020 2020 2020 2020 2d20 4966 4e6f 7450          - IfNotP
+0001a6f0: 7265 7365 6e74 0a20 2020 2020 2020 2020  resent.         
+0001a700: 202d 2041 6c77 6179 730a 2020 2020 2020   - Always.      
+0001a710: 2020 2020 2d20 4e65 7665 720a 2020 2020      - Never.    
+0001a720: 2020 2020 2020 6578 616d 706c 653a 2049        example: I
+0001a730: 664e 6f74 5072 6573 656e 740a 2020 2020  fNotPresent.    
+0001a740: 2020 2020 2020 7469 746c 653a 2069 6d61        title: ima
+0001a750: 6765 5f70 756c 6c5f 706f 6c69 6379 0a20  ge_pull_policy. 
+0001a760: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
+0001a770: 7472 696e 670a 2020 2020 2020 2020 6172  tring.        ar
+0001a780: 6773 3a0a 2020 2020 2020 2020 2020 6465  gs:.          de
+0001a790: 7363 7269 7074 696f 6e3a 2041 7267 756d  scription: Argum
+0001a7a0: 656e 7473 2074 6f20 7468 6520 656e 7472  ents to the entr
+0001a7b0: 7970 6f69 6e74 2e20 5468 6520 636f 6e74  ypoint. The cont
+0001a7c0: 6169 6e65 7220 696d 6167 6527 7320 434d  ainer image's CM
+0001a7d0: 4420 6973 2075 7365 640a 2020 2020 2020  D is used.      
+0001a7e0: 2020 2020 2020 6966 2074 6869 7320 6973        if this is
+0001a7f0: 206e 6f74 2070 726f 7669 6465 640a 2020   not provided.  
+0001a800: 2020 2020 2020 2020 6578 616d 706c 653a          example:
+0001a810: 0a20 2020 2020 2020 2020 202d 202d 6d0a  .          - -m.
+0001a820: 2020 2020 2020 2020 2020 2d20 6f70 656e            - open
+0001a830: 6170 695f 7365 7276 6572 0a20 2020 2020  api_server.     
+0001a840: 2020 2020 2069 7465 6d73 3a0a 2020 2020       items:.    
+0001a850: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
+0001a860: 7269 6e67 0a20 2020 2020 2020 2020 2074  ring.          t
+0001a870: 6974 6c65 3a20 6172 6773 0a20 2020 2020  itle: args.     
+0001a880: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
+0001a890: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
+0001a8a0: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
+0001a8b0: 7269 7074 696f 6e3a 207c 0a20 2020 2020  ription: |.     
+0001a8c0: 2020 2020 2020 2045 6e74 7279 706f 696e         Entrypoin
+0001a8d0: 7420 6172 7261 792e 204e 6f74 2065 7865  t array. Not exe
+0001a8e0: 6375 7465 6420 7769 7468 696e 2061 2073  cuted within a s
+0001a8f0: 6865 6c6c 2e0a 2020 2020 2020 2020 2020  hell..          
+0001a900: 2020 5468 6520 636f 6e74 6169 6e65 7220    The container 
+0001a910: 696d 6167 6527 7320 454e 5452 5950 4f49  image's ENTRYPOI
+0001a920: 4e54 2069 7320 7573 6564 2069 6620 7468  NT is used if th
+0001a930: 6973 2069 7320 6e6f 7420 7072 6f76 6964  is is not provid
+0001a940: 6564 2e0a 2020 2020 2020 2020 2020 6578  ed..          ex
+0001a950: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
+0001a960: 202d 2070 7974 686f 6e33 0a20 2020 2020   - python3.     
+0001a970: 2020 2020 2069 7465 6d73 3a0a 2020 2020       items:.    
+0001a980: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
+0001a990: 7269 6e67 0a20 2020 2020 2020 2020 2074  ring.          t
+0001a9a0: 6974 6c65 3a20 636f 6d6d 616e 640a 2020  itle: command.  
+0001a9b0: 2020 2020 2020 2020 7479 7065 3a20 6172          type: ar
+0001a9c0: 7261 790a 2020 2020 2020 2020 7365 6375  ray.        secu
+0001a9d0: 7269 7479 5f63 6f6e 7465 7874 3a0a 2020  rity_context:.  
+0001a9e0: 2020 2020 2020 2020 2472 6566 3a20 2723          $ref: '#
+0001a9f0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+0001aa00: 6d61 732f 436f 6e74 6169 6e65 7253 6563  mas/ContainerSec
+0001aa10: 436f 6e74 6578 7427 0a20 2020 2020 2020  Context'.       
+0001aa20: 206c 6966 655f 6379 636c 653a 0a20 2020   life_cycle:.   
+0001aa30: 2020 2020 2020 2024 7265 663a 2027 232f         $ref: '#/
+0001aa40: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+0001aa50: 6173 2f43 6f6e 7461 696e 6572 4c69 6665  as/ContainerLife
+0001aa60: 4379 636c 6527 0a20 2020 2020 2020 2070  Cycle'.        p
+0001aa70: 6f72 7473 3a0a 2020 2020 2020 2020 2020  orts:.          
+0001aa80: 6974 656d 733a 0a20 2020 2020 2020 2020  items:.         
+0001aa90: 2020 2024 7265 663a 2027 232f 636f 6d70     $ref: '#/comp
+0001aaa0: 6f6e 656e 7473 2f73 6368 656d 6173 2f43  onents/schemas/C
+0001aab0: 6f6e 7461 696e 6572 506f 7274 270a 2020  ontainerPort'.  
+0001aac0: 2020 2020 2020 2020 7469 746c 653a 2070          title: p
+0001aad0: 6f72 7473 0a20 2020 2020 2020 2020 2074  orts.          t
+0001aae0: 7970 653a 2061 7272 6179 0a20 2020 2020  ype: array.     
+0001aaf0: 2020 2076 6f6c 756d 655f 6d6f 756e 7473     volume_mounts
+0001ab00: 3a0a 2020 2020 2020 2020 2020 6974 656d  :.          item
+0001ab10: 733a 0a20 2020 2020 2020 2020 2020 2024  s:.            $
+0001ab20: 7265 663a 2027 232f 636f 6d70 6f6e 656e  ref: '#/componen
+0001ab30: 7473 2f73 6368 656d 6173 2f56 6f6c 756d  ts/schemas/Volum
+0001ab40: 654d 6f75 6e74 270a 2020 2020 2020 2020  eMount'.        
+0001ab50: 2020 7469 746c 653a 2076 6f6c 756d 655f    title: volume_
+0001ab60: 6d6f 756e 7473 0a20 2020 2020 2020 2020  mounts.         
+0001ab70: 2074 7970 653a 2061 7272 6179 0a20 2020   type: array.   
+0001ab80: 2020 2020 2076 6f6c 756d 655f 6465 7669       volume_devi
+0001ab90: 6365 733a 0a20 2020 2020 2020 2020 2069  ces:.          i
+0001aba0: 7465 6d73 3a0a 2020 2020 2020 2020 2020  tems:.          
+0001abb0: 2020 2472 6566 3a20 2723 2f63 6f6d 706f    $ref: '#/compo
+0001abc0: 6e65 6e74 732f 7363 6865 6d61 732f 566f  nents/schemas/Vo
+0001abd0: 6c75 6d65 4465 7669 6365 270a 2020 2020  lumeDevice'.    
+0001abe0: 2020 2020 2020 7469 746c 653a 2076 6f6c        title: vol
+0001abf0: 756d 655f 6465 7669 6365 730a 2020 2020  ume_devices.    
+0001ac00: 2020 2020 2020 7479 7065 3a20 6172 7261        type: arra
+0001ac10: 790a 2020 2020 2020 2020 7265 736f 7572  y.        resour
+0001ac20: 6365 733a 0a20 2020 2020 2020 2020 2024  ces:.          $
+0001ac30: 7265 663a 2027 232f 636f 6d70 6f6e 656e  ref: '#/componen
+0001ac40: 7473 2f73 6368 656d 6173 2f52 6573 6f75  ts/schemas/Resou
+0001ac50: 7263 6552 6571 7569 7265 6d65 6e74 7327  rceRequirements'
+0001ac60: 0a20 2020 2020 2020 206c 6976 656e 6573  .        livenes
+0001ac70: 735f 7072 6f62 653a 0a20 2020 2020 2020  s_probe:.       
+0001ac80: 2020 2024 7265 663a 2027 232f 636f 6d70     $ref: '#/comp
+0001ac90: 6f6e 656e 7473 2f73 6368 656d 6173 2f50  onents/schemas/P
+0001aca0: 726f 6265 270a 2020 2020 2020 2020 7265  robe'.        re
+0001acb0: 6164 696e 6573 735f 7072 6f62 653a 0a20  adiness_probe:. 
+0001acc0: 2020 2020 2020 2020 2024 7265 663a 2027           $ref: '
+0001acd0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+0001ace0: 656d 6173 2f50 726f 6265 270a 2020 2020  emas/Probe'.    
+0001acf0: 2020 2020 7374 6172 7475 705f 7072 6f62      startup_prob
+0001ad00: 653a 0a20 2020 2020 2020 2020 2024 7265  e:.          $re
+0001ad10: 663a 2027 232f 636f 6d70 6f6e 656e 7473  f: '#/components
+0001ad20: 2f73 6368 656d 6173 2f50 726f 6265 270a  /schemas/Probe'.
+0001ad30: 2020 2020 2020 7265 7175 6972 6564 3a0a        required:.
+0001ad40: 2020 2020 2020 2d20 6e61 6d65 0a20 2020        - name.   
+0001ad50: 2020 2074 6974 6c65 3a20 436f 6e74 6169     title: Contai
+0001ad60: 6e65 720a 2020 2020 2020 7479 7065 3a20  ner.      type: 
+0001ad70: 6f62 6a65 6374 0a20 2020 2045 6e76 5661  object.    EnvVa
+0001ad80: 723a 0a20 2020 2020 2070 726f 7065 7274  r:.      propert
+0001ad90: 6965 733a 0a20 2020 2020 2020 206e 616d  ies:.        nam
+0001ada0: 653a 0a20 2020 2020 2020 2020 2074 6974  e:.          tit
+0001adb0: 6c65 3a20 6e61 6d65 0a20 2020 2020 2020  le: name.       
+0001adc0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
+0001add0: 2020 2020 2020 2020 7661 6c75 653a 0a20          value:. 
+0001ade0: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
+0001adf0: 7661 6c75 650a 2020 2020 2020 2020 2020  value.          
+0001ae00: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+0001ae10: 2020 2020 2076 616c 7565 5f66 726f 6d3a       value_from:
+0001ae20: 0a20 2020 2020 2020 2020 2024 7265 663a  .          $ref:
+0001ae30: 2027 232f 636f 6d70 6f6e 656e 7473 2f73   '#/components/s
+0001ae40: 6368 656d 6173 2f45 6e76 5661 7253 6f75  chemas/EnvVarSou
+0001ae50: 7263 6527 0a20 2020 2020 2072 6571 7569  rce'.      requi
+0001ae60: 7265 643a 0a20 2020 2020 202d 206e 616d  red:.      - nam
+0001ae70: 650a 2020 2020 2020 7469 746c 653a 2045  e.      title: E
+0001ae80: 6e76 5661 720a 2020 2020 2020 7479 7065  nvVar.      type
+0001ae90: 3a20 6f62 6a65 6374 0a20 2020 2045 6e76  : object.    Env
+0001aea0: 5661 7253 6f75 7263 653a 0a20 2020 2020  VarSource:.     
+0001aeb0: 2070 726f 7065 7274 6965 733a 0a20 2020   properties:.   
+0001aec0: 2020 2020 2066 6965 6c64 5f72 6566 3a0a       field_ref:.
+0001aed0: 2020 2020 2020 2020 2020 2472 6566 3a20            $ref: 
+0001aee0: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
+0001aef0: 6865 6d61 732f 4f62 6a65 6374 4669 656c  hemas/ObjectFiel
+0001af00: 6453 656c 6563 746f 7227 0a20 2020 2020  dSelector'.     
+0001af10: 2074 6974 6c65 3a20 456e 7656 6172 536f   title: EnvVarSo
+0001af20: 7572 6365 0a20 2020 2020 2074 7970 653a  urce.      type:
+0001af30: 206f 626a 6563 740a 2020 2020 4f62 6a65   object.    Obje
+0001af40: 6374 4669 656c 6453 656c 6563 746f 723a  ctFieldSelector:
+0001af50: 0a20 2020 2020 2070 726f 7065 7274 6965  .      propertie
+0001af60: 733a 0a20 2020 2020 2020 2061 7069 5f76  s:.        api_v
+0001af70: 6572 7369 6f6e 3a0a 2020 2020 2020 2020  ersion:.        
+0001af80: 2020 6465 7363 7269 7074 696f 6e3a 2022    description: "
+0001af90: 5665 7273 696f 6e20 6f66 2074 6865 2073  Version of the s
+0001afa0: 6368 656d 6120 7468 6520 4669 656c 6450  chema the FieldP
+0001afb0: 6174 6820 6973 2077 7269 7474 656e 2069  ath is written i
+0001afc0: 6e20 7465 726d 7320 6f66 2c5c 0a20 2020  n terms of,\.   
+0001afd0: 2020 2020 2020 2020 205c 2064 6566 6175           \ defau
+0001afe0: 6c74 7320 746f 205c 2276 315c 222e 220a  lts to \"v1\".".
+0001aff0: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
+0001b000: 653a 2076 310a 2020 2020 2020 2020 2020  e: v1.          
+0001b010: 7469 746c 653a 2061 7069 5f76 6572 7369  title: api_versi
+0001b020: 6f6e 0a20 2020 2020 2020 2020 2074 7970  on.          typ
+0001b030: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
+0001b040: 2020 6669 656c 645f 7061 7468 3a0a 2020    field_path:.  
+0001b050: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+0001b060: 696f 6e3a 2050 6174 6820 6f66 2074 6865  ion: Path of the
+0001b070: 2066 6965 6c64 2074 6f20 7365 6c65 6374   field to select
+0001b080: 2069 6e20 7468 6520 7370 6563 6966 6965   in the specifie
+0001b090: 6420 4150 4920 7665 7273 696f 6e2e 0a20  d API version.. 
+0001b0a0: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
+0001b0b0: 3a20 6d65 7461 6461 7461 2e6e 616d 650a  : metadata.name.
+0001b0c0: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+0001b0d0: 2066 6965 6c64 5f70 6174 680a 2020 2020   field_path.    
+0001b0e0: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+0001b0f0: 6e67 0a20 2020 2020 2074 6974 6c65 3a20  ng.      title: 
+0001b100: 4f62 6a65 6374 4669 656c 6453 656c 6563  ObjectFieldSelec
+0001b110: 746f 720a 2020 2020 2020 7479 7065 3a20  tor.      type: 
+0001b120: 6f62 6a65 6374 0a20 2020 2045 6e76 4672  object.    EnvFr
+0001b130: 6f6d 536f 7572 6365 3a0a 2020 2020 2020  omSource:.      
+0001b140: 6465 7363 7269 7074 696f 6e3a 2045 6e76  description: Env
+0001b150: 4672 6f6d 536f 7572 6365 2072 6570 7265  FromSource repre
+0001b160: 7365 6e74 7320 7468 6520 736f 7572 6365  sents the source
+0001b170: 206f 6620 6120 7365 7420 6f66 2043 6f6e   of a set of Con
+0001b180: 6669 674d 6170 730a 2020 2020 2020 6578  figMaps.      ex
+0001b190: 616d 706c 653a 0a20 2020 2020 2020 206e  ample:.        n
+0001b1a0: 616d 653a 202f 6170 692f 7631 2f70 6f64  ame: /api/v1/pod
+0001b1b0: 732f 736f 6d65 2d6e 616d 650a 2020 2020  s/some-name.    
+0001b1c0: 2020 2020 6f70 7469 6f6e 616c 3a20 7472      optional: tr
+0001b1d0: 7565 0a20 2020 2020 2020 2073 6f75 7263  ue.        sourc
+0001b1e0: 655f 7479 7065 3a20 436f 6e66 6967 4d61  e_type: ConfigMa
+0001b1f0: 700a 2020 2020 2020 7072 6f70 6572 7469  p.      properti
+0001b200: 6573 3a0a 2020 2020 2020 2020 6e61 6d65  es:.        name
+0001b210: 3a0a 2020 2020 2020 2020 2020 7479 7065  :.          type
+0001b220: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+0001b230: 206f 7074 696f 6e61 6c3a 0a20 2020 2020   optional:.     
+0001b240: 2020 2020 2074 7970 653a 2062 6f6f 6c65       type: boole
+0001b250: 616e 0a20 2020 2020 2020 2073 6f75 7263  an.        sourc
+0001b260: 655f 7479 7065 3a0a 2020 2020 2020 2020  e_type:.        
+0001b270: 2020 656e 756d 3a0a 2020 2020 2020 2020    enum:.        
+0001b280: 2020 2d20 436f 6e66 6967 4d61 700a 2020    - ConfigMap.  
+0001b290: 2020 2020 2020 2020 2d20 5365 6372 6574          - Secret
+0001b2a0: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
+0001b2b0: 2073 7472 696e 670a 2020 2020 2020 7469   string.      ti
+0001b2c0: 746c 653a 2045 6e76 4672 6f6d 536f 7572  tle: EnvFromSour
+0001b2d0: 6365 0a20 2020 2020 2074 7970 653a 206f  ce.      type: o
+0001b2e0: 626a 6563 740a 2020 2020 436f 6e74 6169  bject.    Contai
+0001b2f0: 6e65 7253 6563 436f 6e74 6578 743a 0a20  nerSecContext:. 
+0001b300: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+0001b310: 3a20 5468 6520 7365 6375 7269 7479 2063  : The security c
+0001b320: 6f6e 6669 6775 7261 7469 6f6e 2074 6861  onfiguration tha
+0001b330: 7420 7769 6c6c 2062 6520 6170 706c 6965  t will be applie
+0001b340: 6420 746f 2061 2063 6f6e 7461 696e 6572  d to a container
+0001b350: 2e0a 2020 2020 2020 6578 616d 706c 653a  ..      example:
+0001b360: 0a20 2020 2020 2020 2063 6170 6162 696c  .        capabil
+0001b370: 6974 6965 733a 0a20 2020 2020 2020 2020  ities:.         
+0001b380: 2061 6464 3a0a 2020 2020 2020 2020 2020   add:.          
+0001b390: 2d20 4e45 545f 4144 4d49 4e0a 2020 2020  - NET_ADMIN.    
+0001b3a0: 2020 2020 2020 2d20 5359 535f 5449 4d45        - SYS_TIME
+0001b3b0: 0a20 2020 2020 2020 2020 2064 726f 703a  .          drop:
+0001b3c0: 0a20 2020 2020 2020 2020 202d 204e 4554  .          - NET
+0001b3d0: 5f41 444d 494e 0a20 2020 2020 2020 2020  _ADMIN.         
+0001b3e0: 202d 2053 5953 5f54 494d 450a 2020 2020   - SYS_TIME.    
+0001b3f0: 2020 2020 7275 6e5f 6173 5f67 726f 7570      run_as_group
+0001b400: 3a20 3330 3030 0a20 2020 2020 2020 2072  : 3000.        r
+0001b410: 756e 5f61 735f 7573 6572 3a20 3130 3030  un_as_user: 1000
+0001b420: 0a20 2020 2020 2070 726f 7065 7274 6965  .      propertie
+0001b430: 733a 0a20 2020 2020 2020 2072 756e 5f61  s:.        run_a
+0001b440: 735f 7573 6572 3a0a 2020 2020 2020 2020  s_user:.        
+0001b450: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
+0001b460: 6865 2055 4944 2074 6f20 7275 6e20 7468  he UID to run th
+0001b470: 6520 656e 7472 7970 6f69 6e74 206f 6620  e entrypoint of 
+0001b480: 7468 6520 636f 6e74 6169 6e65 7220 7072  the container pr
+0001b490: 6f63 6573 732e 0a20 2020 2020 2020 2020  ocess..         
+0001b4a0: 2065 7861 6d70 6c65 3a20 3130 3030 0a20   example: 1000. 
+0001b4b0: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
+0001b4c0: 7275 6e5f 6173 5f75 7365 720a 2020 2020  run_as_user.    
+0001b4d0: 2020 2020 2020 7479 7065 3a20 696e 7465        type: inte
+0001b4e0: 6765 720a 2020 2020 2020 2020 7275 6e5f  ger.        run_
+0001b4f0: 6173 5f67 726f 7570 3a0a 2020 2020 2020  as_group:.      
+0001b500: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+0001b510: 2054 6865 2047 4944 2074 6f20 7275 6e20   The GID to run 
+0001b520: 7468 6520 656e 7472 7970 6f69 6e74 206f  the entrypoint o
+0001b530: 6620 7468 6520 636f 6e74 6169 6e65 7220  f the container 
+0001b540: 7072 6f63 6573 732e 0a20 2020 2020 2020  process..       
+0001b550: 2020 2065 7861 6d70 6c65 3a20 3330 3030     example: 3000
+0001b560: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
+0001b570: 3a20 7275 6e5f 6173 5f67 726f 7570 0a20  : run_as_group. 
+0001b580: 2020 2020 2020 2020 2074 7970 653a 2069           type: i
+0001b590: 6e74 6567 6572 0a20 2020 2020 2020 2063  nteger.        c
+0001b5a0: 6170 6162 696c 6974 6965 733a 0a20 2020  apabilities:.   
+0001b5b0: 2020 2020 2020 2024 7265 663a 2027 232f         $ref: '#/
+0001b5c0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+0001b5d0: 6173 2f43 6f6e 7461 696e 6572 5365 6343  as/ContainerSecC
+0001b5e0: 6f6e 7465 7874 5f63 6170 6162 696c 6974  ontext_capabilit
+0001b5f0: 6965 7327 0a20 2020 2020 2074 6974 6c65  ies'.      title
+0001b600: 3a20 436f 6e74 6169 6e65 7253 6563 436f  : ContainerSecCo
+0001b610: 6e74 6578 740a 2020 2020 2020 7479 7065  ntext.      type
+0001b620: 3a20 6f62 6a65 6374 0a20 2020 2043 6f6e  : object.    Con
+0001b630: 7461 696e 6572 4c69 6665 4379 636c 653a  tainerLifeCycle:
+0001b640: 0a20 2020 2020 2065 7861 6d70 6c65 3a0a  .      example:.
+0001b650: 2020 2020 2020 2020 7072 655f 7374 6f70          pre_stop
+0001b660: 3a0a 2020 2020 2020 2020 2020 7463 705f  :.          tcp_
+0001b670: 736f 636b 6574 3a0a 2020 2020 2020 2020  socket:.        
+0001b680: 2020 2020 706f 7274 3a20 3330 3138 310a      port: 30181.
+0001b690: 2020 2020 2020 2020 2020 2020 686f 7374              host
+0001b6a0: 3a20 3132 372e 302e 302e 310a 2020 2020  : 127.0.0.1.    
+0001b6b0: 2020 2020 2020 6874 7470 5f67 6574 3a0a        http_get:.
+0001b6c0: 2020 2020 2020 2020 2020 2020 7061 7468              path
+0001b6d0: 3a20 2f73 686f 773f 646f 6d61 696e 3d76  : /show?domain=v
+0001b6e0: 3139 2e74 696b 746f 6b63 646e 2e63 6f6d  19.tiktokcdn.com
+0001b6f0: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
+0001b700: 705f 6865 6164 6572 733a 0a20 2020 2020  p_headers:.     
+0001b710: 2020 2020 2020 202d 2078 2d64 6576 7372         - x-devsr
+0001b720: 652d 6175 7468 6f72 697a 6174 696f 6e3a  e-authorization:
+0001b730: 4265 6172 6572 2065 794a 6862 4763 694f  Bearer eyJhbGciO
+0001b740: 694a 0a20 2020 2020 2020 2020 2020 202d  iJ.            -
+0001b750: 2063 6f6e 7465 6e74 2d74 7970 653a 6170   content-type:ap
+0001b760: 706c 6963 6174 696f 6e2f 6a73 6f6e 0a20  plication/json. 
+0001b770: 2020 2020 2020 2020 2020 2073 6368 656d             schem
+0001b780: 653a 2048 5454 5053 0a20 2020 2020 2020  e: HTTPS.       
+0001b790: 2020 2020 2070 6f72 743a 2038 3838 380a       port: 8888.
+0001b7a0: 2020 2020 2020 2020 2020 2020 686f 7374              host
+0001b7b0: 3a20 6773 732d 646e 732d 6167 656e 742e  : gss-dns-agent.
+0001b7c0: 6578 616d 706c 652e 6f72 670a 2020 2020  example.org.    
+0001b7d0: 2020 2020 2020 6578 6563 5f63 6f6d 6d61        exec_comma
+0001b7e0: 6e64 3a0a 2020 2020 2020 2020 2020 2d20  nd:.          - 
+0001b7f0: 2f62 696e 2f73 686f 7764 6f77 6e2e 7368  /bin/showdown.sh
+0001b800: 0a20 2020 2020 2020 2070 6f73 745f 7374  .        post_st
+0001b810: 6172 743a 0a20 2020 2020 2020 2020 2074  art:.          t
+0001b820: 6370 5f73 6f63 6b65 743a 0a20 2020 2020  cp_socket:.     
+0001b830: 2020 2020 2020 2070 6f72 743a 2033 3031         port: 301
+0001b840: 3831 0a20 2020 2020 2020 2020 2020 2068  81.            h
+0001b850: 6f73 743a 2031 3237 2e30 2e30 2e31 0a20  ost: 127.0.0.1. 
+0001b860: 2020 2020 2020 2020 2068 7474 705f 6765           http_ge
+0001b870: 743a 0a20 2020 2020 2020 2020 2020 2070  t:.            p
+0001b880: 6174 683a 202f 7368 6f77 3f64 6f6d 6169  ath: /show?domai
+0001b890: 6e3d 7631 392e 7469 6b74 6f6b 6364 6e2e  n=v19.tiktokcdn.
+0001b8a0: 636f 6d0a 2020 2020 2020 2020 2020 2020  com.            
+0001b8b0: 6874 7470 5f68 6561 6465 7273 3a0a 2020  http_headers:.  
+0001b8c0: 2020 2020 2020 2020 2020 2d20 782d 6465            - x-de
+0001b8d0: 7673 7265 2d61 7574 686f 7269 7a61 7469  vsre-authorizati
+0001b8e0: 6f6e 3a42 6561 7265 7220 6579 4a68 6247  on:Bearer eyJhbG
+0001b8f0: 6369 4f69 4a0a 2020 2020 2020 2020 2020  ciOiJ.          
+0001b900: 2020 2d20 636f 6e74 656e 742d 7479 7065    - content-type
+0001b910: 3a61 7070 6c69 6361 7469 6f6e 2f6a 736f  :application/jso
+0001b920: 6e0a 2020 2020 2020 2020 2020 2020 7363  n.            sc
+0001b930: 6865 6d65 3a20 4854 5450 530a 2020 2020  heme: HTTPS.    
+0001b940: 2020 2020 2020 2020 706f 7274 3a20 3838          port: 88
+0001b950: 3838 0a20 2020 2020 2020 2020 2020 2068  88.            h
+0001b960: 6f73 743a 2067 7373 2d64 6e73 2d61 6765  ost: gss-dns-age
+0001b970: 6e74 2e65 7861 6d70 6c65 2e6f 7267 0a20  nt.example.org. 
+0001b980: 2020 2020 2020 2020 2065 7865 635f 636f           exec_co
+0001b990: 6d6d 616e 643a 0a20 2020 2020 2020 2020  mmand:.         
+0001b9a0: 202d 202f 6269 6e2f 7368 6f77 646f 776e   - /bin/showdown
+0001b9b0: 2e73 680a 2020 2020 2020 7072 6f70 6572  .sh.      proper
+0001b9c0: 7469 6573 3a0a 2020 2020 2020 2020 706f  ties:.        po
+0001b9d0: 7374 5f73 7461 7274 3a0a 2020 2020 2020  st_start:.      
+0001b9e0: 2020 2020 2472 6566 3a20 2723 2f63 6f6d      $ref: '#/com
+0001b9f0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+0001ba00: 4c69 6665 4379 636c 6548 616e 646c 6572  LifeCycleHandler
+0001ba10: 270a 2020 2020 2020 2020 7072 655f 7374  '.        pre_st
+0001ba20: 6f70 3a0a 2020 2020 2020 2020 2020 2472  op:.          $r
+0001ba30: 6566 3a20 2723 2f63 6f6d 706f 6e65 6e74  ef: '#/component
+0001ba40: 732f 7363 6865 6d61 732f 4c69 6665 4379  s/schemas/LifeCy
+0001ba50: 636c 6548 616e 646c 6572 270a 2020 2020  cleHandler'.    
+0001ba60: 2020 7469 746c 653a 2043 6f6e 7461 696e    title: Contain
+0001ba70: 6572 4c69 6665 4379 636c 650a 2020 2020  erLifeCycle.    
+0001ba80: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
+0001ba90: 2020 204c 6966 6543 7963 6c65 4861 6e64     LifeCycleHand
+0001baa0: 6c65 723a 0a20 2020 2020 2065 7861 6d70  ler:.      examp
+0001bab0: 6c65 3a0a 2020 2020 2020 2020 7463 705f  le:.        tcp_
+0001bac0: 736f 636b 6574 3a0a 2020 2020 2020 2020  socket:.        
+0001bad0: 2020 706f 7274 3a20 3330 3138 310a 2020    port: 30181.  
+0001bae0: 2020 2020 2020 2020 686f 7374 3a20 3132          host: 12
+0001baf0: 372e 302e 302e 310a 2020 2020 2020 2020  7.0.0.1.        
+0001bb00: 6874 7470 5f67 6574 3a0a 2020 2020 2020  http_get:.      
+0001bb10: 2020 2020 7061 7468 3a20 2f73 686f 773f      path: /show?
+0001bb20: 646f 6d61 696e 3d76 3139 2e74 696b 746f  domain=v19.tikto
+0001bb30: 6b63 646e 2e63 6f6d 0a20 2020 2020 2020  kcdn.com.       
+0001bb40: 2020 2068 7474 705f 6865 6164 6572 733a     http_headers:
+0001bb50: 0a20 2020 2020 2020 2020 202d 2078 2d64  .          - x-d
+0001bb60: 6576 7372 652d 6175 7468 6f72 697a 6174  evsre-authorizat
+0001bb70: 696f 6e3a 4265 6172 6572 2065 794a 6862  ion:Bearer eyJhb
+0001bb80: 4763 694f 694a 0a20 2020 2020 2020 2020  GciOiJ.         
+0001bb90: 202d 2063 6f6e 7465 6e74 2d74 7970 653a   - content-type:
+0001bba0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+0001bbb0: 0a20 2020 2020 2020 2020 2073 6368 656d  .          schem
+0001bbc0: 653a 2048 5454 5053 0a20 2020 2020 2020  e: HTTPS.       
+0001bbd0: 2020 2070 6f72 743a 2038 3838 380a 2020     port: 8888.  
+0001bbe0: 2020 2020 2020 2020 686f 7374 3a20 6773          host: gs
+0001bbf0: 732d 646e 732d 6167 656e 742e 6578 616d  s-dns-agent.exam
+0001bc00: 706c 652e 6f72 670a 2020 2020 2020 2020  ple.org.        
+0001bc10: 6578 6563 5f63 6f6d 6d61 6e64 3a0a 2020  exec_command:.  
+0001bc20: 2020 2020 2020 2d20 2f62 696e 2f73 686f        - /bin/sho
+0001bc30: 7764 6f77 6e2e 7368 0a20 2020 2020 2070  wdown.sh.      p
+0001bc40: 726f 7065 7274 6965 733a 0a20 2020 2020  roperties:.     
+0001bc50: 2020 2065 7865 635f 636f 6d6d 616e 643a     exec_command:
+0001bc60: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
+0001bc70: 6970 7469 6f6e 3a20 436f 6d6d 616e 6420  iption: Command 
+0001bc80: 6c69 6e65 2074 6f20 6578 6563 7574 6520  line to execute 
+0001bc90: 696e 7369 6465 2074 6865 2063 6f6e 7461  inside the conta
+0001bca0: 696e 6572 0a20 2020 2020 2020 2020 2065  iner.          e
+0001bcb0: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
+0001bcc0: 2020 2d20 2f62 696e 2f73 686f 7764 6f77    - /bin/showdow
+0001bcd0: 6e2e 7368 0a20 2020 2020 2020 2020 2069  n.sh.          i
+0001bce0: 7465 6d73 3a0a 2020 2020 2020 2020 2020  tems:.          
+0001bcf0: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+0001bd00: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
+0001bd10: 6578 6563 5f63 6f6d 6d61 6e64 0a20 2020  exec_command.   
+0001bd20: 2020 2020 2020 2074 7970 653a 2061 7272         type: arr
+0001bd30: 6179 0a20 2020 2020 2020 2068 7474 705f  ay.        http_
+0001bd40: 6765 743a 0a20 2020 2020 2020 2020 2024  get:.          $
+0001bd50: 7265 663a 2027 232f 636f 6d70 6f6e 656e  ref: '#/componen
+0001bd60: 7473 2f73 6368 656d 6173 2f48 7474 7047  ts/schemas/HttpG
+0001bd70: 6574 270a 2020 2020 2020 2020 7463 705f  et'.        tcp_
+0001bd80: 736f 636b 6574 3a0a 2020 2020 2020 2020  socket:.        
+0001bd90: 2020 2472 6566 3a20 2723 2f63 6f6d 706f    $ref: '#/compo
+0001bda0: 6e65 6e74 732f 7363 6865 6d61 732f 5463  nents/schemas/Tc
+0001bdb0: 7053 6f63 6b65 7427 0a20 2020 2020 2074  pSocket'.      t
+0001bdc0: 6974 6c65 3a20 4c69 6665 4379 636c 6548  itle: LifeCycleH
+0001bdd0: 616e 646c 6572 0a20 2020 2020 2074 7970  andler.      typ
+0001bde0: 653a 206f 626a 6563 740a 2020 2020 4874  e: object.    Ht
+0001bdf0: 7470 4765 743a 0a20 2020 2020 2065 7861  tpGet:.      exa
+0001be00: 6d70 6c65 3a0a 2020 2020 2020 2020 7061  mple:.        pa
+0001be10: 7468 3a20 2f73 686f 773f 646f 6d61 696e  th: /show?domain
+0001be20: 3d76 3139 2e74 696b 746f 6b63 646e 2e63  =v19.tiktokcdn.c
+0001be30: 6f6d 0a20 2020 2020 2020 2068 7474 705f  om.        http_
+0001be40: 6865 6164 6572 733a 0a20 2020 2020 2020  headers:.       
+0001be50: 202d 2078 2d64 6576 7372 652d 6175 7468   - x-devsre-auth
+0001be60: 6f72 697a 6174 696f 6e3a 4265 6172 6572  orization:Bearer
+0001be70: 2065 794a 6862 4763 694f 694a 0a20 2020   eyJhbGciOiJ.   
+0001be80: 2020 2020 202d 2063 6f6e 7465 6e74 2d74       - content-t
+0001be90: 7970 653a 6170 706c 6963 6174 696f 6e2f  ype:application/
+0001bea0: 6a73 6f6e 0a20 2020 2020 2020 2073 6368  json.        sch
+0001beb0: 656d 653a 2048 5454 5053 0a20 2020 2020  eme: HTTPS.     
+0001bec0: 2020 2070 6f72 743a 2038 3838 380a 2020     port: 8888.  
+0001bed0: 2020 2020 2020 686f 7374 3a20 6773 732d        host: gss-
+0001bee0: 646e 732d 6167 656e 742e 6578 616d 706c  dns-agent.exampl
+0001bef0: 652e 6f72 670a 2020 2020 2020 7072 6f70  e.org.      prop
+0001bf00: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
+0001bf10: 706f 7274 3a0a 2020 2020 2020 2020 2020  port:.          
+0001bf20: 6465 7363 7269 7074 696f 6e3a 204e 756d  description: Num
+0001bf30: 6265 7220 6f66 2074 6865 2070 6f72 7420  ber of the port 
+0001bf40: 746f 2061 6363 6573 7320 6f6e 2074 6865  to access on the
+0001bf50: 2063 6f6e 7461 696e 6572 2e0a 2020 2020   container..    
+0001bf60: 2020 2020 2020 6578 616d 706c 653a 2038        example: 8
+0001bf70: 3838 380a 2020 2020 2020 2020 2020 7469  888.          ti
+0001bf80: 746c 653a 2070 6f72 740a 2020 2020 2020  tle: port.      
+0001bf90: 2020 2020 7479 7065 3a20 696e 7465 6765      type: intege
+0001bfa0: 720a 2020 2020 2020 2020 686f 7374 3a0a  r.        host:.
+0001bfb0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+0001bfc0: 7074 696f 6e3a 2022 486f 7374 206e 616d  ption: "Host nam
+0001bfd0: 6520 746f 2063 6f6e 6e65 6374 2074 6f2c  e to connect to,
+0001bfe0: 2064 6566 6175 6c74 7320 746f 2074 6865   defaults to the
+0001bff0: 2070 6f64 2049 502e 220a 2020 2020 2020   pod IP.".      
+0001c000: 2020 2020 6578 616d 706c 653a 2067 7373      example: gss
+0001c010: 2d64 6e73 2d61 6765 6e74 2e65 7861 6d70  -dns-agent.examp
+0001c020: 6c65 2e6f 7267 0a20 2020 2020 2020 2020  le.org.         
+0001c030: 2074 6974 6c65 3a20 686f 7374 0a20 2020   title: host.   
+0001c040: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+0001c050: 696e 670a 2020 2020 2020 2020 6874 7470  ing.        http
+0001c060: 5f68 6561 6465 7273 3a0a 2020 2020 2020  _headers:.      
+0001c070: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+0001c080: 2043 7573 746f 6d20 6865 6164 6572 7320   Custom headers 
+0001c090: 746f 2073 6574 2069 6e20 7468 6520 7265  to set in the re
+0001c0a0: 7175 6573 742e 0a20 2020 2020 2020 2020  quest..         
+0001c0b0: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
+0001c0c0: 2020 2020 2d20 782d 6465 7673 7265 2d61      - x-devsre-a
+0001c0d0: 7574 686f 7269 7a61 7469 6f6e 3a42 6561  uthorization:Bea
+0001c0e0: 7265 7220 6579 4a68 6247 6369 4f69 4a0a  rer eyJhbGciOiJ.
+0001c0f0: 2020 2020 2020 2020 2020 2d20 636f 6e74            - cont
+0001c100: 656e 742d 7479 7065 3a61 7070 6c69 6361  ent-type:applica
+0001c110: 7469 6f6e 2f6a 736f 6e0a 2020 2020 2020  tion/json.      
+0001c120: 2020 2020 6974 656d 733a 0a20 2020 2020      items:.     
+0001c130: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+0001c140: 696e 670a 2020 2020 2020 2020 2020 7469  ing.          ti
+0001c150: 746c 653a 2068 7474 705f 6865 6164 6572  tle: http_header
+0001c160: 730a 2020 2020 2020 2020 2020 7479 7065  s.          type
+0001c170: 3a20 6172 7261 790a 2020 2020 2020 2020  : array.        
+0001c180: 7061 7468 3a0a 2020 2020 2020 2020 2020  path:.          
+0001c190: 6465 7363 7269 7074 696f 6e3a 2050 6174  description: Pat
+0001c1a0: 6820 746f 2061 6363 6573 7320 6f6e 2074  h to access on t
+0001c1b0: 6865 2048 5454 5020 7365 7276 6572 2e0a  he HTTP server..
+0001c1c0: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
+0001c1d0: 653a 202f 7368 6f77 3f64 6f6d 6169 6e3d  e: /show?domain=
+0001c1e0: 7631 392e 7469 6b74 6f6b 6364 6e2e 636f  v19.tiktokcdn.co
+0001c1f0: 6d0a 2020 2020 2020 2020 2020 7469 746c  m.          titl
+0001c200: 653a 2070 6174 680a 2020 2020 2020 2020  e: path.        
+0001c210: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+0001c220: 2020 2020 2020 2073 6368 656d 653a 0a20         scheme:. 
+0001c230: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+0001c240: 7469 6f6e 3a20 5363 6865 6d65 2074 6f20  tion: Scheme to 
+0001c250: 7573 6520 666f 7220 636f 6e6e 6563 7469  use for connecti
+0001c260: 6e67 2074 6f20 7468 6520 686f 7374 2e20  ng to the host. 
+0001c270: 4465 6661 756c 7473 2074 6f20 4854 5450  Defaults to HTTP
+0001c280: 2e0a 2020 2020 2020 2020 2020 6578 616d  ..          exam
+0001c290: 706c 653a 2048 5454 5053 0a20 2020 2020  ple: HTTPS.     
+0001c2a0: 2020 2020 2074 6974 6c65 3a20 7363 6865       title: sche
+0001c2b0: 6d65 0a20 2020 2020 2020 2020 2074 7970  me.          typ
+0001c2c0: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
+0001c2d0: 7265 7175 6972 6564 3a0a 2020 2020 2020  required:.      
+0001c2e0: 2d20 706f 7274 0a20 2020 2020 2074 6974  - port.      tit
+0001c2f0: 6c65 3a20 4874 7470 4765 740a 2020 2020  le: HttpGet.    
+0001c300: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
+0001c310: 2020 2054 6370 536f 636b 6574 3a0a 2020     TcpSocket:.  
+0001c320: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
+0001c330: 2020 2020 2070 6f72 743a 2033 3031 3831       port: 30181
+0001c340: 0a20 2020 2020 2020 2068 6f73 743a 2031  .        host: 1
+0001c350: 3237 2e30 2e30 2e31 0a20 2020 2020 2070  27.0.0.1.      p
+0001c360: 726f 7065 7274 6965 733a 0a20 2020 2020  roperties:.     
+0001c370: 2020 2070 6f72 743a 0a20 2020 2020 2020     port:.       
+0001c380: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+0001c390: 4e75 6d62 6572 206f 6620 7468 6520 706f  Number of the po
+0001c3a0: 7274 2074 6f20 6163 6365 7373 206f 6e20  rt to access on 
+0001c3b0: 7468 6520 636f 6e74 6169 6e65 722e 0a20  the container.. 
+0001c3c0: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
+0001c3d0: 3a20 3330 3138 310a 2020 2020 2020 2020  : 30181.        
+0001c3e0: 2020 7469 746c 653a 2070 6f72 740a 2020    title: port.  
+0001c3f0: 2020 2020 2020 2020 7479 7065 3a20 696e          type: in
+0001c400: 7465 6765 720a 2020 2020 2020 2020 686f  teger.        ho
+0001c410: 7374 3a0a 2020 2020 2020 2020 2020 6465  st:.          de
+0001c420: 7363 7269 7074 696f 6e3a 2022 486f 7374  scription: "Host
+0001c430: 206e 616d 6520 746f 2063 6f6e 6e65 6374   name to connect
+0001c440: 2074 6f2c 2064 6566 6175 6c74 7320 746f   to, defaults to
+0001c450: 2074 6865 2070 6f64 2049 502e 220a 2020   the pod IP.".  
+0001c460: 2020 2020 2020 2020 6578 616d 706c 653a          example:
+0001c470: 2031 3237 2e30 2e30 2e31 0a20 2020 2020   127.0.0.1.     
+0001c480: 2020 2020 2074 6974 6c65 3a20 686f 7374       title: host
+0001c490: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
+0001c4a0: 2073 7472 696e 670a 2020 2020 2020 7265   string.      re
+0001c4b0: 7175 6972 6564 3a0a 2020 2020 2020 2d20  quired:.      - 
+0001c4c0: 706f 7274 0a20 2020 2020 2074 6974 6c65  port.      title
+0001c4d0: 3a20 5463 7053 6f63 6b65 740a 2020 2020  : TcpSocket.    
+0001c4e0: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
+0001c4f0: 2020 2043 6f6e 7461 696e 6572 506f 7274     ContainerPort
+0001c500: 3a0a 2020 2020 2020 6578 616d 706c 653a  :.      example:
+0001c510: 0a20 2020 2020 2020 2063 6f6e 7461 696e  .        contain
+0001c520: 6572 5f70 6f72 743a 2038 300a 2020 2020  er_port: 80.    
+0001c530: 2020 2020 7072 6f74 6f63 6f6c 3a20 5443      protocol: TC
+0001c540: 500a 2020 2020 2020 2020 6e61 6d65 3a20  P.        name: 
+0001c550: 6874 7470 0a20 2020 2020 2070 726f 7065  http.      prope
+0001c560: 7274 6965 733a 0a20 2020 2020 2020 206e  rties:.        n
+0001c570: 616d 653a 0a20 2020 2020 2020 2020 2064  ame:.          d
+0001c580: 6573 6372 6970 7469 6f6e 3a20 2243 6f6e  escription: "Con
+0001c590: 7461 696e 6572 2070 6f72 7420 6e61 6d65  tainer port name
+0001c5a0: 2c20 6966 2073 7065 6369 6669 6564 2c20  , if specified, 
+0001c5b0: 7468 6973 206d 7573 7420 6265 2061 6e20  this must be an 
+0001c5c0: 4941 4e41 5f53 5643 5f4e 414d 455c 0a20  IANA_SVC_NAME\. 
+0001c5d0: 2020 2020 2020 2020 2020 205c 2061 6e64             \ and
+0001c5e0: 2075 6e69 7175 6520 7769 7468 696e 2074   unique within t
+0001c5f0: 6865 2070 6f64 220a 2020 2020 2020 2020  he pod".        
+0001c600: 2020 6578 616d 706c 653a 2068 7474 700a    example: http.
+0001c610: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+0001c620: 206e 616d 650a 2020 2020 2020 2020 2020   name.          
+0001c630: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+0001c640: 2020 2020 2063 6f6e 7461 696e 6572 5f70       container_p
+0001c650: 6f72 743a 0a20 2020 2020 2020 2020 2065  ort:.          e
+0001c660: 7861 6d70 6c65 3a20 3830 0a20 2020 2020  xample: 80.     
+0001c670: 2020 2020 2074 6974 6c65 3a20 636f 6e74       title: cont
+0001c680: 6169 6e65 725f 706f 7274 0a20 2020 2020  ainer_port.     
+0001c690: 2020 2020 2074 7970 653a 2069 6e74 6567       type: integ
+0001c6a0: 6572 0a20 2020 2020 2020 2070 726f 746f  er.        proto
+0001c6b0: 636f 6c3a 0a20 2020 2020 2020 2020 2064  col:.          d
+0001c6c0: 6573 6372 6970 7469 6f6e 3a20 4465 6661  escription: Defa
+0001c6d0: 756c 7473 2074 6f20 5443 500a 2020 2020  ults to TCP.    
+0001c6e0: 2020 2020 2020 656e 756d 3a0a 2020 2020        enum:.    
+0001c6f0: 2020 2020 2020 2d20 5443 500a 2020 2020        - TCP.    
+0001c700: 2020 2020 2020 2d20 5544 500a 2020 2020        - UDP.    
+0001c710: 2020 2020 2020 6578 616d 706c 653a 2054        example: T
+0001c720: 4350 0a20 2020 2020 2020 2020 2074 6974  CP.          tit
+0001c730: 6c65 3a20 7072 6f74 6f63 6f6c 0a20 2020  le: protocol.   
+0001c740: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+0001c750: 696e 670a 2020 2020 2020 7265 7175 6972  ing.      requir
+0001c760: 6564 3a0a 2020 2020 2020 2d20 6e61 6d65  ed:.      - name
+0001c770: 0a20 2020 2020 2074 6974 6c65 3a20 436f  .      title: Co
+0001c780: 6e74 6169 6e65 7250 6f72 740a 2020 2020  ntainerPort.    
+0001c790: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
+0001c7a0: 2020 2056 6f6c 756d 654d 6f75 6e74 3a0a     VolumeMount:.
+0001c7b0: 2020 2020 2020 6578 616d 706c 653a 0a20        example:. 
+0001c7c0: 2020 2020 2020 2070 6174 683a 202f 6f70         path: /op
+0001c7d0: 742f 7365 7276 6572 2f63 6f6e 660a 2020  t/server/conf.  
+0001c7e0: 2020 2020 2020 7265 6164 5f6f 6e6c 793a        read_only:
+0001c7f0: 2074 7275 650a 2020 2020 2020 2020 6e61   true.        na
+0001c800: 6d65 3a20 6465 6d6f 2d76 6f6c 0a20 2020  me: demo-vol.   
+0001c810: 2020 2020 2073 7562 5f70 6174 683a 2073       sub_path: s
+0001c820: 6572 7665 722e 636f 6e66 0a20 2020 2020  erver.conf.     
+0001c830: 2070 726f 7065 7274 6965 733a 0a20 2020   properties:.   
+0001c840: 2020 2020 206e 616d 653a 0a20 2020 2020       name:.     
+0001c850: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+0001c860: 3a20 4d75 7374 206d 6174 6368 2074 6865  : Must match the
+0001c870: 204e 616d 6520 6f66 2061 2056 6f6c 756d   Name of a Volum
+0001c880: 650a 2020 2020 2020 2020 2020 6578 616d  e.          exam
+0001c890: 706c 653a 2064 656d 6f2d 766f 6c0a 2020  ple: demo-vol.  
+0001c8a0: 2020 2020 2020 2020 7469 746c 653a 206e          title: n
+0001c8b0: 616d 650a 2020 2020 2020 2020 7061 7468  ame.        path
+0001c8c0: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
+0001c8d0: 7269 7074 696f 6e3a 2050 6174 6820 7769  ription: Path wi
+0001c8e0: 7468 696e 2074 6865 2063 6f6e 7461 696e  thin the contain
+0001c8f0: 6572 2061 7420 7768 6963 6820 7468 6520  er at which the 
+0001c900: 766f 6c75 6d65 2073 686f 756c 6420 6265  volume should be
+0001c910: 206d 6f75 6e74 6564 0a20 2020 2020 2020   mounted.       
+0001c920: 2020 2065 7861 6d70 6c65 3a20 2f6f 7074     example: /opt
+0001c930: 2f73 6572 7665 722f 636f 6e66 0a20 2020  /server/conf.   
+0001c940: 2020 2020 2020 2074 6974 6c65 3a20 7061         title: pa
+0001c950: 7468 0a20 2020 2020 2020 2020 2074 7970  th.          typ
+0001c960: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
+0001c970: 2020 7375 625f 7061 7468 3a0a 2020 2020    sub_path:.    
+0001c980: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+0001c990: 6e3a 2050 6174 6820 7769 7468 696e 2074  n: Path within t
+0001c9a0: 6865 2076 6f6c 756d 6520 6672 6f6d 2077  he volume from w
+0001c9b0: 6869 6368 2074 6865 2063 6f6e 7461 696e  hich the contain
+0001c9c0: 6572 2773 2076 6f6c 756d 6520 7368 6f75  er's volume shou
+0001c9d0: 6c64 0a20 2020 2020 2020 2020 2020 2062  ld.            b
+0001c9e0: 6520 6d6f 756e 7465 640a 2020 2020 2020  e mounted.      
+0001c9f0: 2020 2020 6578 616d 706c 653a 2073 6572      example: ser
+0001ca00: 7665 722e 636f 6e66 0a20 2020 2020 2020  ver.conf.       
+0001ca10: 2020 2074 6974 6c65 3a20 7375 625f 7061     title: sub_pa
+0001ca20: 7468 0a20 2020 2020 2020 2020 2074 7970  th.          typ
+0001ca30: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
+0001ca40: 2020 7265 6164 5f6f 6e6c 793a 0a20 2020    read_only:.   
+0001ca50: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+0001ca60: 6f6e 3a20 5769 6c6c 2066 6f72 6365 2074  on: Will force t
+0001ca70: 6865 2052 6561 644f 6e6c 7920 7365 7474  he ReadOnly sett
+0001ca80: 696e 6720 696e 2056 6f6c 756d 654d 6f75  ing in VolumeMou
+0001ca90: 6e74 730a 2020 2020 2020 2020 2020 6578  nts.          ex
+0001caa0: 616d 706c 653a 2074 7275 650a 2020 2020  ample: true.    
+0001cab0: 2020 2020 2020 7469 746c 653a 2072 6561        title: rea
+0001cac0: 645f 6f6e 6c79 0a20 2020 2020 2020 2020  d_only.         
+0001cad0: 2074 7970 653a 2062 6f6f 6c65 616e 0a20   type: boolean. 
+0001cae0: 2020 2020 2072 6571 7569 7265 643a 0a20       required:. 
+0001caf0: 2020 2020 202d 206e 616d 650a 2020 2020       - name.    
+0001cb00: 2020 7469 746c 653a 2056 6f6c 756d 654d    title: VolumeM
+0001cb10: 6f75 6e74 0a20 2020 2020 2074 7970 653a  ount.      type:
+0001cb20: 206f 626a 6563 740a 2020 2020 566f 6c75   object.    Volu
+0001cb30: 6d65 4465 7669 6365 3a0a 2020 2020 2020  meDevice:.      
+0001cb40: 6578 616d 706c 653a 0a20 2020 2020 2020  example:.       
+0001cb50: 206e 616d 653a 2064 656d 6f2d 766f 6c0a   name: demo-vol.
+0001cb60: 2020 2020 2020 2020 6465 7669 6365 5f70          device_p
+0001cb70: 6174 683a 202f 6465 762f 7364 6131 0a20  ath: /dev/sda1. 
+0001cb80: 2020 2020 2020 2062 6361 6368 655f 6e75         bcache_nu
+0001cb90: 6d73 3a20 340a 2020 2020 2020 7072 6f70  ms: 4.      prop
+0001cba0: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
+0001cbb0: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
+0001cbc0: 6465 7363 7269 7074 696f 6e3a 204d 7573  description: Mus
+0001cbd0: 7420 6d61 7463 6820 7468 6520 4e61 6d65  t match the Name
+0001cbe0: 206f 6620 6120 566f 6c75 6d65 0a20 2020   of a Volume.   
+0001cbf0: 2020 2020 2020 2065 7861 6d70 6c65 3a20         example: 
+0001cc00: 6465 6d6f 2d76 6f6c 0a20 2020 2020 2020  demo-vol.       
+0001cc10: 2020 2074 6974 6c65 3a20 6e61 6d65 0a20     title: name. 
+0001cc20: 2020 2020 2020 2064 6576 6963 655f 7061         device_pa
+0001cc30: 7468 3a0a 2020 2020 2020 2020 2020 6465  th:.          de
+0001cc40: 7363 7269 7074 696f 6e3a 2050 6174 6820  scription: Path 
+0001cc50: 6f66 2074 6865 2064 6576 6963 6520 7769  of the device wi
+0001cc60: 7468 696e 2074 6865 2063 6f6e 7461 696e  thin the contain
+0001cc70: 6572 0a20 2020 2020 2020 2020 2065 7861  er.          exa
+0001cc80: 6d70 6c65 3a20 2f64 6576 2f73 6461 310a  mple: /dev/sda1.
+0001cc90: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+0001cca0: 2064 6576 6963 655f 7061 7468 0a20 2020   device_path.   
+0001ccb0: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+0001ccc0: 696e 670a 2020 2020 2020 2020 6263 6163  ing.        bcac
+0001ccd0: 6865 5f6e 756d 733a 0a20 2020 2020 2020  he_nums:.       
+0001cce0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+0001ccf0: 5573 6564 2066 6f72 2041 5453 2064 6570  Used for ATS dep
+0001cd00: 6c6f 796d 656e 7420 746f 2061 7574 6f6d  loyment to autom
+0001cd10: 6174 6963 616c 6c79 2067 656e 6572 6174  atically generat
+0001cd20: 6520 6263 6163 6865 5f6e 756d 730a 2020  e bcache_nums.  
+0001cd30: 2020 2020 2020 2020 2020 766f 6c75 6d65            volume
+0001cd40: 2064 6576 6963 6573 2061 6e64 2072 656c   devices and rel
+0001cd50: 6174 6564 2063 6f6e 7465 6e74 732e 0a20  ated contents.. 
+0001cd60: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
+0001cd70: 3a20 340a 2020 2020 2020 2020 2020 7469  : 4.          ti
+0001cd80: 746c 653a 2062 6361 6368 655f 6e75 6d73  tle: bcache_nums
+0001cd90: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
+0001cda0: 2069 6e74 6567 6572 0a20 2020 2020 2072   integer.      r
+0001cdb0: 6571 7569 7265 643a 0a20 2020 2020 202d  equired:.      -
+0001cdc0: 206e 616d 650a 2020 2020 2020 7469 746c   name.      titl
+0001cdd0: 653a 2056 6f6c 756d 6544 6576 6963 650a  e: VolumeDevice.
+0001cde0: 2020 2020 2020 7479 7065 3a20 6f62 6a65        type: obje
+0001cdf0: 6374 0a20 2020 2052 6573 6f75 7263 6552  ct.    ResourceR
+0001ce00: 6571 7569 7265 6d65 6e74 733a 0a20 2020  equirements:.   
+0001ce10: 2020 2065 7861 6d70 6c65 3a0a 2020 2020     example:.    
+0001ce20: 2020 2020 7265 7175 6573 7473 3a0a 2020      requests:.  
+0001ce30: 2020 2020 2020 2020 6d65 6d6f 7279 3a20          memory: 
+0001ce40: 3235 364d 690a 2020 2020 2020 2020 2020  256Mi.          
+0001ce50: 6370 753a 2022 302e 3122 0a20 2020 2020  cpu: "0.1".     
+0001ce60: 2020 206c 696d 6974 733a 0a20 2020 2020     limits:.     
+0001ce70: 2020 2020 206d 656d 6f72 793a 2035 3132       memory: 512
+0001ce80: 4d69 0a20 2020 2020 2020 2020 2063 7075  Mi.          cpu
+0001ce90: 3a20 2230 2e35 220a 2020 2020 2020 7072  : "0.5".      pr
+0001cea0: 6f70 6572 7469 6573 3a0a 2020 2020 2020  operties:.      
+0001ceb0: 2020 6c69 6d69 7473 3a0a 2020 2020 2020    limits:.      
+0001cec0: 2020 2020 6164 6469 7469 6f6e 616c 5072      additionalPr
+0001ced0: 6f70 6572 7469 6573 3a0a 2020 2020 2020  operties:.      
+0001cee0: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+0001cef0: 6e67 0a20 2020 2020 2020 2020 2064 6573  ng.          des
+0001cf00: 6372 6970 7469 6f6e 3a20 7573 6564 2074  cription: used t
+0001cf10: 6f20 7370 6563 6966 7920 7468 6520 6d61  o specify the ma
+0001cf20: 7869 6d75 6d20 616d 6f75 6e74 206f 6620  ximum amount of 
+0001cf30: 7265 736f 7572 6365 7320 7468 6174 2063  resources that c
+0001cf40: 616e 2062 650a 2020 2020 2020 2020 2020  an be.          
+0001cf50: 2020 636f 6e73 756d 6564 2e0a 2020 2020    consumed..    
+0001cf60: 2020 2020 2020 6578 616d 706c 653a 0a20        example:. 
+0001cf70: 2020 2020 2020 2020 2020 206d 656d 6f72             memor
+0001cf80: 793a 2035 3132 4d69 0a20 2020 2020 2020  y: 512Mi.       
+0001cf90: 2020 2020 2063 7075 3a20 2230 2e35 220a       cpu: "0.5".
+0001cfa0: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+0001cfb0: 206c 696d 6974 730a 2020 2020 2020 2020   limits.        
+0001cfc0: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
+0001cfd0: 2020 2020 2020 2072 6571 7565 7374 733a         requests:
+0001cfe0: 0a20 2020 2020 2020 2020 2061 6464 6974  .          addit
+0001cff0: 696f 6e61 6c50 726f 7065 7274 6965 733a  ionalProperties:
+0001d000: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
+0001d010: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
+0001d020: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+0001d030: 2075 7365 6420 746f 2073 7065 6369 6679   used to specify
+0001d040: 2074 6865 206d 696e 696d 756d 2061 6d6f   the minimum amo
+0001d050: 756e 7420 6f66 2072 6573 6f75 7263 6573  unt of resources
+0001d060: 2074 6861 7420 7368 6f75 6c64 0a20 2020   that should.   
+0001d070: 2020 2020 2020 2020 2062 6520 636f 6e73           be cons
+0001d080: 756d 6564 2e0a 2020 2020 2020 2020 2020  umed..          
+0001d090: 6578 616d 706c 653a 0a20 2020 2020 2020  example:.       
+0001d0a0: 2020 2020 206d 656d 6f72 793a 2032 3536       memory: 256
+0001d0b0: 4d69 0a20 2020 2020 2020 2020 2020 2063  Mi.            c
+0001d0c0: 7075 3a20 2230 2e31 220a 2020 2020 2020  pu: "0.1".      
+0001d0d0: 2020 2020 7469 746c 653a 2072 6571 7565      title: reque
+0001d0e0: 7374 730a 2020 2020 2020 2020 2020 7479  sts.          ty
+0001d0f0: 7065 3a20 6f62 6a65 6374 0a20 2020 2020  pe: object.     
+0001d100: 2074 6974 6c65 3a20 5265 736f 7572 6365   title: Resource
+0001d110: 5265 7175 6972 656d 656e 7473 0a20 2020  Requirements.   
+0001d120: 2020 2074 7970 653a 206f 626a 6563 740a     type: object.
+0001d130: 2020 2020 5072 6f62 653a 0a20 2020 2020      Probe:.     
+0001d140: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
+0001d150: 2020 7065 7269 6f64 5f73 6563 6f6e 6473    period_seconds
+0001d160: 3a20 3630 0a20 2020 2020 2020 2069 6e69  : 60.        ini
+0001d170: 7469 616c 5f64 656c 6179 5f73 6563 6f6e  tial_delay_secon
+0001d180: 6473 3a20 3630 300a 2020 2020 2020 2020  ds: 600.        
+0001d190: 7463 705f 736f 636b 6574 3a0a 2020 2020  tcp_socket:.    
+0001d1a0: 2020 2020 2020 706f 7274 3a20 3330 3138        port: 3018
+0001d1b0: 310a 2020 2020 2020 2020 2020 686f 7374  1.          host
+0001d1c0: 3a20 3132 372e 302e 302e 310a 2020 2020  : 127.0.0.1.    
+0001d1d0: 2020 2020 6661 696c 7572 655f 7468 7265      failure_thre
+0001d1e0: 7368 6f6c 643a 2033 0a20 2020 2020 2020  shold: 3.       
+0001d1f0: 2068 7474 705f 6765 743a 0a20 2020 2020   http_get:.     
+0001d200: 2020 2020 2070 6174 683a 202f 7368 6f77       path: /show
+0001d210: 3f64 6f6d 6169 6e3d 7631 392e 7469 6b74  ?domain=v19.tikt
+0001d220: 6f6b 6364 6e2e 636f 6d0a 2020 2020 2020  okcdn.com.      
+0001d230: 2020 2020 6874 7470 5f68 6561 6465 7273      http_headers
+0001d240: 3a0a 2020 2020 2020 2020 2020 2d20 782d  :.          - x-
+0001d250: 6465 7673 7265 2d61 7574 686f 7269 7a61  devsre-authoriza
+0001d260: 7469 6f6e 3a42 6561 7265 7220 6579 4a68  tion:Bearer eyJh
+0001d270: 6247 6369 4f69 4a0a 2020 2020 2020 2020  bGciOiJ.        
+0001d280: 2020 2d20 636f 6e74 656e 742d 7479 7065    - content-type
+0001d290: 3a61 7070 6c69 6361 7469 6f6e 2f6a 736f  :application/jso
+0001d2a0: 6e0a 2020 2020 2020 2020 2020 7363 6865  n.          sche
+0001d2b0: 6d65 3a20 4854 5450 530a 2020 2020 2020  me: HTTPS.      
+0001d2c0: 2020 2020 706f 7274 3a20 3838 3838 0a20      port: 8888. 
+0001d2d0: 2020 2020 2020 2020 2068 6f73 743a 2067           host: g
+0001d2e0: 7373 2d64 6e73 2d61 6765 6e74 2e65 7861  ss-dns-agent.exa
+0001d2f0: 6d70 6c65 2e6f 7267 0a20 2020 2020 2020  mple.org.       
+0001d300: 2074 696d 656f 7574 5f73 6563 6f6e 6473   timeout_seconds
+0001d310: 3a20 3630 0a20 2020 2020 2020 2065 7865  : 60.        exe
+0001d320: 635f 636f 6d6d 616e 643a 0a20 2020 2020  c_command:.     
+0001d330: 2020 202d 202f 6773 732f 6469 6e67 6d61     - /gss/dingma
+0001d340: 6e2f 6269 6e2f 6469 6e67 6d61 6e2d 636c  n/bin/dingman-cl
+0001d350: 6974 0a20 2020 2020 2020 202d 202d 6164  it.        - -ad
+0001d360: 6472 6573 730a 2020 2020 2020 2020 2d20  dress.        - 
+0001d370: 3132 372e 302e 302e 313a 3330 3530 310a  127.0.0.1:30501.
+0001d380: 2020 2020 2020 2020 2d20 2d63 6f6d 6d61          - -comma
+0001d390: 6e64 0a20 2020 2020 2020 202d 2073 686f  nd.        - sho
+0001d3a0: 7720 706f 703a 616c 6c20 7375 6d6d 6172  w pop:all summar
+0001d3b0: 793a 6865 616c 7468 2d73 7461 7475 730a  y:health-status.
+0001d3c0: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
+0001d3d0: 3a0a 2020 2020 2020 2020 6578 6563 5f63  :.        exec_c
+0001d3e0: 6f6d 6d61 6e64 3a0a 2020 2020 2020 2020  ommand:.        
+0001d3f0: 2020 6465 7363 7269 7074 696f 6e3a 2043    description: C
+0001d400: 6f6d 6d61 6e64 206c 696e 6520 746f 2065  ommand line to e
+0001d410: 7865 6375 7465 2069 6e73 6964 6520 7468  xecute inside th
+0001d420: 6520 636f 6e74 6169 6e65 720a 2020 2020  e container.    
+0001d430: 2020 2020 2020 6578 616d 706c 653a 0a20        example:. 
+0001d440: 2020 2020 2020 2020 202d 202f 6773 732f           - /gss/
+0001d450: 6469 6e67 6d61 6e2f 6269 6e2f 6469 6e67  dingman/bin/ding
+0001d460: 6d61 6e2d 636c 6974 0a20 2020 2020 2020  man-clit.       
+0001d470: 2020 202d 202d 6164 6472 6573 730a 2020     - -address.  
+0001d480: 2020 2020 2020 2020 2d20 3132 372e 302e          - 127.0.
+0001d490: 302e 313a 3330 3530 310a 2020 2020 2020  0.1:30501.      
+0001d4a0: 2020 2020 2d20 2d63 6f6d 6d61 6e64 0a20      - -command. 
+0001d4b0: 2020 2020 2020 2020 202d 2073 686f 7720           - show 
+0001d4c0: 706f 703a 616c 6c20 7375 6d6d 6172 793a  pop:all summary:
+0001d4d0: 6865 616c 7468 2d73 7461 7475 730a 2020  health-status.  
+0001d4e0: 2020 2020 2020 2020 6974 656d 733a 0a20          items:. 
+0001d4f0: 2020 2020 2020 2020 2020 2074 7970 653a             type:
+0001d500: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+0001d510: 2020 7469 746c 653a 2065 7865 635f 636f    title: exec_co
+0001d520: 6d6d 616e 640a 2020 2020 2020 2020 2020  mmand.          
+0001d530: 7479 7065 3a20 6172 7261 790a 2020 2020  type: array.    
+0001d540: 2020 2020 6874 7470 5f67 6574 3a0a 2020      http_get:.  
+0001d550: 2020 2020 2020 2020 2472 6566 3a20 2723          $ref: '#
+0001d560: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+0001d570: 6d61 732f 4874 7470 4765 7427 0a20 2020  mas/HttpGet'.   
+0001d580: 2020 2020 2074 6370 5f73 6f63 6b65 743a       tcp_socket:
+0001d590: 0a20 2020 2020 2020 2020 2024 7265 663a  .          $ref:
+0001d5a0: 2027 232f 636f 6d70 6f6e 656e 7473 2f73   '#/components/s
+0001d5b0: 6368 656d 6173 2f54 6370 536f 636b 6574  chemas/TcpSocket
+0001d5c0: 270a 2020 2020 2020 2020 6661 696c 7572  '.        failur
+0001d5d0: 655f 7468 7265 7368 6f6c 643a 0a20 2020  e_threshold:.   
+0001d5e0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+0001d5f0: 6f6e 3a20 4d69 6e69 6d75 6d20 636f 6e73  on: Minimum cons
+0001d600: 6563 7574 6976 6520 6661 696c 7572 6573  ecutive failures
+0001d610: 2066 6f72 2074 6865 2070 726f 6265 2074   for the probe t
+0001d620: 6f20 6265 2063 6f6e 7369 6465 7265 640a  o be considered.
+0001d630: 2020 2020 2020 2020 2020 2020 6661 696c              fail
+0001d640: 6564 2061 6674 6572 2068 6176 696e 6720  ed after having 
+0001d650: 7375 6363 6565 6465 642e 0a20 2020 2020  succeeded..     
+0001d660: 2020 2020 2065 7861 6d70 6c65 3a20 330a       example: 3.
+0001d670: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+0001d680: 2066 6169 6c75 7265 5f74 6872 6573 686f   failure_thresho
+0001d690: 6c64 0a20 2020 2020 2020 2020 2074 7970  ld.          typ
+0001d6a0: 653a 2069 6e74 6567 6572 0a20 2020 2020  e: integer.     
+0001d6b0: 2020 2070 6572 696f 645f 7365 636f 6e64     period_second
+0001d6c0: 733a 0a20 2020 2020 2020 2020 2064 6573  s:.          des
+0001d6d0: 6372 6970 7469 6f6e 3a20 486f 7720 6f66  cription: How of
+0001d6e0: 7465 6e20 2869 6e20 7365 636f 6e64 7329  ten (in seconds)
+0001d6f0: 2074 6f20 7065 7266 6f72 6d20 7468 6520   to perform the 
+0001d700: 7072 6f62 652e 2044 6566 6175 6c74 2074  probe. Default t
+0001d710: 6f20 3130 0a20 2020 2020 2020 2020 2020  o 10.           
+0001d720: 2073 6563 6f6e 6473 2e20 4d69 6e69 6d75   seconds. Minimu
+0001d730: 6d20 7661 6c75 6520 6973 2031 2e0a 2020  m value is 1..  
+0001d740: 2020 2020 2020 2020 6578 616d 706c 653a          example:
+0001d750: 2036 300a 2020 2020 2020 2020 2020 7469   60.          ti
+0001d760: 746c 653a 2070 6572 696f 645f 7365 636f  tle: period_seco
+0001d770: 6e64 730a 2020 2020 2020 2020 2020 7479  nds.          ty
+0001d780: 7065 3a20 696e 7465 6765 720a 2020 2020  pe: integer.    
+0001d790: 2020 2020 7469 6d65 6f75 745f 7365 636f      timeout_seco
+0001d7a0: 6e64 733a 0a20 2020 2020 2020 2020 2064  nds:.          d
+0001d7b0: 6573 6372 6970 7469 6f6e 3a20 4e75 6d62  escription: Numb
+0001d7c0: 6572 206f 6620 7365 636f 6e64 7320 6166  er of seconds af
+0001d7d0: 7465 7220 7768 6963 6820 7468 6520 7072  ter which the pr
+0001d7e0: 6f62 6520 7469 6d65 7320 6f75 742e 2044  obe times out. D
+0001d7f0: 6566 6175 6c74 730a 2020 2020 2020 2020  efaults.        
+0001d800: 2020 2020 746f 2031 2073 6563 6f6e 642e      to 1 second.
+0001d810: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
+0001d820: 6c65 3a20 3630 0a20 2020 2020 2020 2020  le: 60.         
+0001d830: 2074 6974 6c65 3a20 7469 6d65 6f75 745f   title: timeout_
+0001d840: 7365 636f 6e64 730a 2020 2020 2020 2020  seconds.        
+0001d850: 2020 7479 7065 3a20 696e 7465 6765 720a    type: integer.
+0001d860: 2020 2020 2020 2020 696e 6974 6961 6c5f          initial_
+0001d870: 6465 6c61 795f 7365 636f 6e64 733a 0a20  delay_seconds:. 
+0001d880: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+0001d890: 7469 6f6e 3a20 4e75 6d62 6572 206f 6620  tion: Number of 
+0001d8a0: 7365 636f 6e64 7320 6166 7465 7220 7468  seconds after th
+0001d8b0: 6520 636f 6e74 6169 6e65 7220 6861 7320  e container has 
+0001d8c0: 7374 6172 7465 6420 6265 666f 7265 206c  started before l
+0001d8d0: 6976 656e 6573 730a 2020 2020 2020 2020  iveness.        
+0001d8e0: 2020 2020 7072 6f62 6573 2061 7265 2069      probes are i
+0001d8f0: 6e69 7469 6174 6564 2e0a 2020 2020 2020  nitiated..      
+0001d900: 2020 2020 6578 616d 706c 653a 2036 3030      example: 600
+0001d910: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
+0001d920: 3a20 696e 6974 6961 6c5f 6465 6c61 795f  : initial_delay_
+0001d930: 7365 636f 6e64 730a 2020 2020 2020 2020  seconds.        
+0001d940: 2020 7479 7065 3a20 696e 7465 6765 720a    type: integer.
+0001d950: 2020 2020 2020 7469 746c 653a 2050 726f        title: Pro
+0001d960: 6265 0a20 2020 2020 2074 7970 653a 206f  be.      type: o
+0001d970: 626a 6563 740a 2020 2020 566f 6c75 6d65  bject.    Volume
+0001d980: 3a0a 2020 2020 2020 6578 616d 706c 653a  :.      example:
+0001d990: 0a20 2020 2020 2020 2068 6f73 745f 7061  .        host_pa
+0001d9a0: 7468 3a0a 2020 2020 2020 2020 2020 7061  th:.          pa
+0001d9b0: 7468 3a20 2f64 6174 610a 2020 2020 2020  th: /data.      
+0001d9c0: 2020 2020 7061 7468 5f74 7970 653a 2044      path_type: D
+0001d9d0: 6972 6563 746f 7279 0a20 2020 2020 2020  irectory.       
+0001d9e0: 206e 616d 653a 2064 656d 6f2d 766f 6c0a   name: demo-vol.
+0001d9f0: 2020 2020 2020 2020 656d 7074 795f 6469          empty_di
+0001da00: 723a 0a20 2020 2020 2020 2020 206d 6564  r:.          med
+0001da10: 6975 6d3a 204d 656d 6f72 790a 2020 2020  ium: Memory.    
+0001da20: 2020 2020 2020 7369 7a65 5f6c 696d 6974        size_limit
+0001da30: 3a20 3530 304d 690a 2020 2020 2020 2020  : 500Mi.        
+0001da40: 636f 6e66 6967 5f6d 6170 3a0a 2020 2020  config_map:.    
+0001da50: 2020 2020 2020 6e61 6d65 3a20 7365 7276        name: serv
+0001da60: 6572 2063 6f6e 6669 672f 7365 6372 6574  er config/secret
+0001da70: 0a20 2020 2020 2020 2020 206f 7074 696f  .          optio
+0001da80: 6e61 6c3a 2066 616c 7365 0a20 2020 2020  nal: false.     
+0001da90: 2020 2020 2064 6566 6175 6c74 5f6d 6f64       default_mod
+0001daa0: 653a 2034 3030 0a20 2020 2020 2020 2073  e: 400.        s
+0001dab0: 6563 7265 743a 0a20 2020 2020 2020 2020  ecret:.         
+0001dac0: 206e 616d 653a 2073 6572 7665 7220 636f   name: server co
+0001dad0: 6e66 6967 2f73 6563 7265 740a 2020 2020  nfig/secret.    
+0001dae0: 2020 2020 2020 6f70 7469 6f6e 616c 3a20        optional: 
+0001daf0: 6661 6c73 650a 2020 2020 2020 2020 2020  false.          
+0001db00: 6465 6661 756c 745f 6d6f 6465 3a20 3430  default_mode: 40
+0001db10: 300a 2020 2020 2020 2020 7065 7273 6973  0.        persis
+0001db20: 7465 6e74 5f76 6f6c 756d 655f 636c 6169  tent_volume_clai
+0001db30: 6d3a 0a20 2020 2020 2020 2020 2072 6561  m:.          rea
+0001db40: 645f 6f6e 6c79 3a20 6661 6c73 650a 2020  d_only: false.  
+0001db50: 2020 2020 2020 2020 636c 6169 6d5f 6e61          claim_na
+0001db60: 6d65 3a20 6465 6d6f 2d70 7663 0a20 2020  me: demo-pvc.   
+0001db70: 2020 2070 726f 7065 7274 6965 733a 0a20     properties:. 
+0001db80: 2020 2020 2020 206e 616d 653a 0a20 2020         name:.   
+0001db90: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+0001dba0: 6f6e 3a20 4e61 6d65 206f 6620 7468 6520  on: Name of the 
+0001dbb0: 766f 6c75 6d65 2e20 4d75 7374 2062 6520  volume. Must be 
+0001dbc0: 6120 444e 535f 4c41 4245 4c20 616e 6420  a DNS_LABEL and 
+0001dbd0: 756e 6971 7565 2077 6974 6869 6e20 7468  unique within th
+0001dbe0: 650a 2020 2020 2020 2020 2020 2020 706f  e.            po
+0001dbf0: 640a 2020 2020 2020 2020 2020 6578 616d  d.          exam
+0001dc00: 706c 653a 2064 656d 6f2d 766f 6c0a 2020  ple: demo-vol.  
+0001dc10: 2020 2020 2020 2020 7469 746c 653a 206e          title: n
+0001dc20: 616d 650a 2020 2020 2020 2020 2020 7479  ame.          ty
+0001dc30: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
+0001dc40: 2020 2063 6f6e 6669 675f 6d61 703a 0a20     config_map:. 
+0001dc50: 2020 2020 2020 2020 2024 7265 663a 2027           $ref: '
+0001dc60: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+0001dc70: 656d 6173 2f52 6566 566f 6c75 6d65 536f  emas/RefVolumeSo
+0001dc80: 7572 6365 270a 2020 2020 2020 2020 7365  urce'.        se
+0001dc90: 6372 6574 3a0a 2020 2020 2020 2020 2020  cret:.          
+0001dca0: 2472 6566 3a20 2723 2f63 6f6d 706f 6e65  $ref: '#/compone
+0001dcb0: 6e74 732f 7363 6865 6d61 732f 5265 6656  nts/schemas/RefV
+0001dcc0: 6f6c 756d 6553 6f75 7263 6527 0a20 2020  olumeSource'.   
+0001dcd0: 2020 2020 2070 6572 7369 7374 656e 745f       persistent_
+0001dce0: 766f 6c75 6d65 5f63 6c61 696d 3a0a 2020  volume_claim:.  
+0001dcf0: 2020 2020 2020 2020 2472 6566 3a20 2723          $ref: '#
+0001dd00: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+0001dd10: 6d61 732f 566f 6c75 6d65 5f70 6572 7369  mas/Volume_persi
+0001dd20: 7374 656e 745f 766f 6c75 6d65 5f63 6c61  stent_volume_cla
+0001dd30: 696d 270a 2020 2020 2020 2020 656d 7074  im'.        empt
+0001dd40: 795f 6469 723a 0a20 2020 2020 2020 2020  y_dir:.         
+0001dd50: 2024 7265 663a 2027 232f 636f 6d70 6f6e   $ref: '#/compon
+0001dd60: 656e 7473 2f73 6368 656d 6173 2f56 6f6c  ents/schemas/Vol
+0001dd70: 756d 655f 656d 7074 795f 6469 7227 0a20  ume_empty_dir'. 
+0001dd80: 2020 2020 2020 2068 6f73 745f 7061 7468         host_path
+0001dd90: 3a0a 2020 2020 2020 2020 2020 2472 6566  :.          $ref
+0001dda0: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
+0001ddb0: 7363 6865 6d61 732f 566f 6c75 6d65 5f68  schemas/Volume_h
+0001ddc0: 6f73 745f 7061 7468 270a 2020 2020 2020  ost_path'.      
+0001ddd0: 7265 7175 6972 6564 3a0a 2020 2020 2020  required:.      
+0001dde0: 2d20 6e61 6d65 0a20 2020 2020 2074 6974  - name.      tit
+0001ddf0: 6c65 3a20 566f 6c75 6d65 0a20 2020 2020  le: Volume.     
+0001de00: 2074 7970 653a 206f 626a 6563 740a 2020   type: object.  
+0001de10: 2020 5265 6656 6f6c 756d 6553 6f75 7263    RefVolumeSourc
+0001de20: 653a 0a20 2020 2020 2065 7861 6d70 6c65  e:.      example
+0001de30: 3a0a 2020 2020 2020 2020 6e61 6d65 3a20  :.        name: 
+0001de40: 7365 7276 6572 2063 6f6e 6669 672f 7365  server config/se
+0001de50: 6372 6574 0a20 2020 2020 2020 206f 7074  cret.        opt
+0001de60: 696f 6e61 6c3a 2066 616c 7365 0a20 2020  ional: false.   
+0001de70: 2020 2020 2064 6566 6175 6c74 5f6d 6f64       default_mod
+0001de80: 653a 2034 3030 0a20 2020 2020 2070 726f  e: 400.      pro
+0001de90: 7065 7274 6965 733a 0a20 2020 2020 2020  perties:.       
+0001dea0: 206e 616d 653a 0a20 2020 2020 2020 2020   name:.         
+0001deb0: 2064 6573 6372 6970 7469 6f6e 3a20 766f   description: vo
+0001dec0: 6c75 6d65 2073 6f75 7263 6520 2863 6f6e  lume source (con
+0001ded0: 6669 674d 6170 2f53 6563 7265 7429 206e  figMap/Secret) n
+0001dee0: 616d 650a 2020 2020 2020 2020 2020 6578  ame.          ex
+0001def0: 616d 706c 653a 2073 6572 7665 7220 636f  ample: server co
+0001df00: 6e66 6967 2f73 6563 7265 740a 2020 2020  nfig/secret.    
+0001df10: 2020 2020 2020 7469 746c 653a 206e 616d        title: nam
+0001df20: 650a 2020 2020 2020 2020 2020 7479 7065  e.          type
+0001df30: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+0001df40: 206f 7074 696f 6e61 6c3a 0a20 2020 2020   optional:.     
+0001df50: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+0001df60: 3a20 7370 6563 6966 7920 7768 6574 6865  : specify whethe
+0001df70: 7220 7468 6520 766f 6c75 6d65 2073 6f75  r the volume sou
+0001df80: 7263 6520 6f72 2069 7473 206b 6579 7320  rce or its keys 
+0001df90: 6d75 7374 2062 6520 6465 6669 6e65 640a  must be defined.
+0001dfa0: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
+0001dfb0: 653a 2066 616c 7365 0a20 2020 2020 2020  e: false.       
+0001dfc0: 2020 2074 6974 6c65 3a20 6f70 7469 6f6e     title: option
+0001dfd0: 616c 0a20 2020 2020 2020 2020 2074 7970  al.          typ
+0001dfe0: 653a 2062 6f6f 6c65 616e 0a20 2020 2020  e: boolean.     
+0001dff0: 2020 2064 6566 6175 6c74 5f6d 6f64 653a     default_mode:
+0001e000: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
+0001e010: 6970 7469 6f6e 3a20 7c0a 2020 2020 2020  iption: |.      
+0001e020: 2020 2020 2020 6d6f 6465 2062 6974 7320        mode bits 
+0001e030: 7573 6564 2074 6f20 7365 7420 7065 726d  used to set perm
+0001e040: 6973 7369 6f6e 7320 6f6e 2063 7265 6174  issions on creat
+0001e050: 6564 2066 696c 6573 2062 7920 6465 6661  ed files by defa
+0001e060: 756c 742e 0a20 2020 2020 2020 2020 2020  ult..           
+0001e070: 204d 7573 7420 6265 2061 6e20 6f63 7461   Must be an octa
+0001e080: 6c20 7661 6c75 6520 6265 7477 6565 6e20  l value between 
+0001e090: 3030 3030 2061 6e64 2030 3737 3720 6f72  0000 and 0777 or
+0001e0a0: 2061 2064 6563 696d 616c 2076 616c 7565   a decimal value
+0001e0b0: 2062 6574 7765 656e 2030 2061 6e64 2035   between 0 and 5
+0001e0c0: 3131 0a20 2020 2020 2020 2020 2065 7861  11.          exa
+0001e0d0: 6d70 6c65 3a20 3430 300a 2020 2020 2020  mple: 400.      
+0001e0e0: 2020 2020 7469 746c 653a 2064 6566 6175      title: defau
+0001e0f0: 6c74 5f6d 6f64 650a 2020 2020 2020 2020  lt_mode.        
+0001e100: 2020 7479 7065 3a20 696e 7465 6765 720a    type: integer.
+0001e110: 2020 2020 2020 7469 746c 653a 2052 6566        title: Ref
+0001e120: 566f 6c75 6d65 536f 7572 6365 0a20 2020  VolumeSource.   
+0001e130: 2020 2074 7970 653a 206f 626a 6563 740a     type: object.
+0001e140: 2020 2020 4166 6669 6e69 7479 3a0a 2020      Affinity:.  
+0001e150: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
+0001e160: 2020 2020 2070 6f64 5f61 6e74 695f 6166       pod_anti_af
+0001e170: 6669 6e69 7479 3a0a 2020 2020 2020 2020  finity:.        
+0001e180: 2020 7072 6566 6572 7265 645f 6475 7269    preferred_duri
+0001e190: 6e67 5f73 6368 6564 756c 696e 675f 6967  ng_scheduling_ig
+0001e1a0: 6e6f 7265 645f 6475 7269 6e67 5f65 7865  nored_during_exe
+0001e1b0: 6375 7469 6f6e 3a0a 2020 2020 2020 2020  cution:.        
+0001e1c0: 2020 2d20 7765 6967 6874 3a20 360a 2020    - weight: 6.  
+0001e1d0: 2020 2020 2020 2020 2020 706f 645f 6166            pod_af
+0001e1e0: 6669 6e69 7479 5f74 6572 6d3a 0a20 2020  finity_term:.   
+0001e1f0: 2020 2020 2020 2020 2020 206c 6162 656c             label
+0001e200: 5f73 656c 6563 746f 723a 0a20 2020 2020  _selector:.     
+0001e210: 2020 2020 2020 2020 202d 2061 7070 3a64           - app:d
+0001e220: 656d 6f2d 6170 700a 2020 2020 2020 2020  emo-app.        
+0001e230: 2020 2020 2020 2d20 226b 6579 3a76 6572        - "key:ver
+0001e240: 7369 6f6e 2c20 6f70 6572 6174 6f72 3a49  sion, operator:I
+0001e250: 6e2c 2076 616c 7565 733a 5b76 312e 302e  n, values:[v1.0.
+0001e260: 302c 2076 312e 302e 315d 220a 2020 2020  0, v1.0.1]".    
+0001e270: 2020 2020 2020 2020 2020 746f 706f 6c6f            topolo
+0001e280: 6779 5f6b 6579 3a20 746f 706f 6c6f 6779  gy_key: topology
+0001e290: 5f6b 6579 0a20 2020 2020 2020 2020 2020  _key.           
+0001e2a0: 2020 206e 616d 6573 7061 6365 733a 0a20     namespaces:. 
+0001e2b0: 2020 2020 2020 2020 2020 2020 202d 206e               - n
+0001e2c0: 616d 6573 7061 6365 730a 2020 2020 2020  amespaces.      
+0001e2d0: 2020 2020 2020 2020 2d20 6e61 6d65 7370          - namesp
+0001e2e0: 6163 6573 0a20 2020 2020 2020 2020 202d  aces.          -
+0001e2f0: 2077 6569 6768 743a 2036 0a20 2020 2020   weight: 6.     
+0001e300: 2020 2020 2020 2070 6f64 5f61 6666 696e         pod_affin
+0001e310: 6974 795f 7465 726d 3a0a 2020 2020 2020  ity_term:.      
+0001e320: 2020 2020 2020 2020 6c61 6265 6c5f 7365          label_se
+0001e330: 6c65 6374 6f72 3a0a 2020 2020 2020 2020  lector:.        
+0001e340: 2020 2020 2020 2d20 6170 703a 6465 6d6f        - app:demo
+0001e350: 2d61 7070 0a20 2020 2020 2020 2020 2020  -app.           
+0001e360: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
+0001e370: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
+0001e380: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
+0001e390: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
+0001e3a0: 2020 2020 2020 2074 6f70 6f6c 6f67 795f         topology_
+0001e3b0: 6b65 793a 2074 6f70 6f6c 6f67 795f 6b65  key: topology_ke
+0001e3c0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+0001e3d0: 6e61 6d65 7370 6163 6573 3a0a 2020 2020  namespaces:.    
+0001e3e0: 2020 2020 2020 2020 2020 2d20 6e61 6d65            - name
+0001e3f0: 7370 6163 6573 0a20 2020 2020 2020 2020  spaces.         
+0001e400: 2020 2020 202d 206e 616d 6573 7061 6365       - namespace
+0001e410: 730a 2020 2020 2020 2020 2020 7265 7175  s.          requ
+0001e420: 6972 6564 5f64 7572 696e 675f 7363 6865  ired_during_sche
+0001e430: 6475 6c69 6e67 5f69 676e 6f72 6564 5f64  duling_ignored_d
+0001e440: 7572 696e 675f 6578 6563 7574 696f 6e3a  uring_execution:
+0001e450: 0a20 2020 2020 2020 2020 202d 206c 6162  .          - lab
+0001e460: 656c 5f73 656c 6563 746f 723a 0a20 2020  el_selector:.   
+0001e470: 2020 2020 2020 2020 202d 2061 7070 3a64           - app:d
+0001e480: 656d 6f2d 6170 700a 2020 2020 2020 2020  emo-app.        
+0001e490: 2020 2020 2d20 226b 6579 3a76 6572 7369      - "key:versi
+0001e4a0: 6f6e 2c20 6f70 6572 6174 6f72 3a49 6e2c  on, operator:In,
+0001e4b0: 2076 616c 7565 733a 5b76 312e 302e 302c   values:[v1.0.0,
+0001e4c0: 2076 312e 302e 315d 220a 2020 2020 2020   v1.0.1]".      
+0001e4d0: 2020 2020 2020 746f 706f 6c6f 6779 5f6b        topology_k
+0001e4e0: 6579 3a20 746f 706f 6c6f 6779 5f6b 6579  ey: topology_key
+0001e4f0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+0001e500: 6573 7061 6365 733a 0a20 2020 2020 2020  espaces:.       
+0001e510: 2020 2020 202d 206e 616d 6573 7061 6365       - namespace
+0001e520: 730a 2020 2020 2020 2020 2020 2020 2d20  s.            - 
+0001e530: 6e61 6d65 7370 6163 6573 0a20 2020 2020  namespaces.     
+0001e540: 2020 2020 202d 206c 6162 656c 5f73 656c       - label_sel
+0001e550: 6563 746f 723a 0a20 2020 2020 2020 2020  ector:.         
+0001e560: 2020 202d 2061 7070 3a64 656d 6f2d 6170     - app:demo-ap
+0001e570: 700a 2020 2020 2020 2020 2020 2020 2d20  p.            - 
+0001e580: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
+0001e590: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
+0001e5a0: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
+0001e5b0: 315d 220a 2020 2020 2020 2020 2020 2020  1]".            
+0001e5c0: 746f 706f 6c6f 6779 5f6b 6579 3a20 746f  topology_key: to
+0001e5d0: 706f 6c6f 6779 5f6b 6579 0a20 2020 2020  pology_key.     
+0001e5e0: 2020 2020 2020 206e 616d 6573 7061 6365         namespace
+0001e5f0: 733a 0a20 2020 2020 2020 2020 2020 202d  s:.            -
+0001e600: 206e 616d 6573 7061 6365 730a 2020 2020   namespaces.    
+0001e610: 2020 2020 2020 2020 2d20 6e61 6d65 7370          - namesp
+0001e620: 6163 6573 0a20 2020 2020 2020 206e 6f64  aces.        nod
+0001e630: 655f 6166 6669 6e69 7479 3a0a 2020 2020  e_affinity:.    
+0001e640: 2020 2020 2020 7072 6566 6572 7265 645f        preferred_
+0001e650: 6475 7269 6e67 5f73 6368 6564 756c 696e  during_schedulin
+0001e660: 675f 6967 6e6f 7265 645f 6475 7269 6e67  g_ignored_during
+0001e670: 5f65 7865 6375 7469 6f6e 3a0a 2020 2020  _execution:.    
+0001e680: 2020 2020 2020 2d20 7072 6566 6572 656e        - preferen
+0001e690: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
+0001e6a0: 2020 6d61 7463 685f 6578 7072 6573 7369    match_expressi
+0001e6b0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+0001e6c0: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
+0001e6d0: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
+0001e6e0: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
+0001e6f0: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
+0001e700: 2020 2020 2020 206d 6174 6368 5f66 6965         match_fie
+0001e710: 6c64 733a 0a20 2020 2020 2020 2020 2020  lds:.           
+0001e720: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
+0001e730: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
+0001e740: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
+0001e750: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
+0001e760: 2020 2020 2077 6569 6768 743a 2030 0a20       weight: 0. 
+0001e770: 2020 2020 2020 2020 202d 2070 7265 6665           - prefe
+0001e780: 7265 6e63 653a 0a20 2020 2020 2020 2020  rence:.         
+0001e790: 2020 2020 206d 6174 6368 5f65 7870 7265       match_expre
+0001e7a0: 7373 696f 6e73 3a0a 2020 2020 2020 2020  ssions:.        
+0001e7b0: 2020 2020 2020 2d20 226b 6579 3a76 6572        - "key:ver
+0001e7c0: 7369 6f6e 2c20 6f70 6572 6174 6f72 3a49  sion, operator:I
+0001e7d0: 6e2c 2076 616c 7565 733a 5b76 312e 302e  n, values:[v1.0.
+0001e7e0: 302c 2076 312e 302e 315d 220a 2020 2020  0, v1.0.1]".    
+0001e7f0: 2020 2020 2020 2020 2020 6d61 7463 685f            match_
+0001e800: 6669 656c 6473 3a0a 2020 2020 2020 2020  fields:.        
+0001e810: 2020 2020 2020 2d20 226b 6579 3a76 6572        - "key:ver
+0001e820: 7369 6f6e 2c20 6f70 6572 6174 6f72 3a49  sion, operator:I
+0001e830: 6e2c 2076 616c 7565 733a 5b76 312e 302e  n, values:[v1.0.
+0001e840: 302c 2076 312e 302e 315d 220a 2020 2020  0, v1.0.1]".    
+0001e850: 2020 2020 2020 2020 7765 6967 6874 3a20          weight: 
+0001e860: 300a 2020 2020 2020 2020 2020 7265 7175  0.          requ
+0001e870: 6972 6564 5f64 7572 696e 675f 7363 6865  ired_during_sche
+0001e880: 6475 6c69 6e67 5f69 676e 6f72 6564 5f64  duling_ignored_d
+0001e890: 7572 696e 675f 6578 6563 7574 696f 6e3a  uring_execution:
+0001e8a0: 0a20 2020 2020 2020 2020 2020 206e 6f64  .            nod
+0001e8b0: 655f 7365 6c65 6374 6f72 5f74 6572 6d73  e_selector_terms
+0001e8c0: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
+0001e8d0: 6d61 7463 685f 6578 7072 6573 7369 6f6e  match_expression
+0001e8e0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0001e8f0: 202d 2022 6b65 793a 7665 7273 696f 6e2c   - "key:version,
+0001e900: 206f 7065 7261 746f 723a 496e 2c20 7661   operator:In, va
+0001e910: 6c75 6573 3a5b 7631 2e30 2e30 2c20 7631  lues:[v1.0.0, v1
+0001e920: 2e30 2e31 5d22 0a20 2020 2020 2020 2020  .0.1]".         
+0001e930: 2020 2020 206d 6174 6368 5f66 6965 6c64       match_field
+0001e940: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0001e950: 202d 2022 6b65 793a 7665 7273 696f 6e2c   - "key:version,
+0001e960: 206f 7065 7261 746f 723a 496e 2c20 7661   operator:In, va
+0001e970: 6c75 6573 3a5b 7631 2e30 2e30 2c20 7631  lues:[v1.0.0, v1
+0001e980: 2e30 2e31 5d22 0a20 2020 2020 2020 2020  .0.1]".         
+0001e990: 2020 202d 206d 6174 6368 5f65 7870 7265     - match_expre
+0001e9a0: 7373 696f 6e73 3a0a 2020 2020 2020 2020  ssions:.        
+0001e9b0: 2020 2020 2020 2d20 226b 6579 3a76 6572        - "key:ver
+0001e9c0: 7369 6f6e 2c20 6f70 6572 6174 6f72 3a49  sion, operator:I
+0001e9d0: 6e2c 2076 616c 7565 733a 5b76 312e 302e  n, values:[v1.0.
+0001e9e0: 302c 2076 312e 302e 315d 220a 2020 2020  0, v1.0.1]".    
+0001e9f0: 2020 2020 2020 2020 2020 6d61 7463 685f            match_
+0001ea00: 6669 656c 6473 3a0a 2020 2020 2020 2020  fields:.        
+0001ea10: 2020 2020 2020 2d20 226b 6579 3a76 6572        - "key:ver
+0001ea20: 7369 6f6e 2c20 6f70 6572 6174 6f72 3a49  sion, operator:I
+0001ea30: 6e2c 2076 616c 7565 733a 5b76 312e 302e  n, values:[v1.0.
+0001ea40: 302c 2076 312e 302e 315d 220a 2020 2020  0, v1.0.1]".    
+0001ea50: 2020 2020 706f 645f 6166 6669 6e69 7479      pod_affinity
+0001ea60: 3a0a 2020 2020 2020 2020 2020 7072 6566  :.          pref
+0001ea70: 6572 7265 645f 6475 7269 6e67 5f73 6368  erred_during_sch
+0001ea80: 6564 756c 696e 675f 6967 6e6f 7265 645f  eduling_ignored_
+0001ea90: 6475 7269 6e67 5f65 7865 6375 7469 6f6e  during_execution
+0001eaa0: 3a0a 2020 2020 2020 2020 2020 2d20 7765  :.          - we
+0001eab0: 6967 6874 3a20 360a 2020 2020 2020 2020  ight: 6.        
+0001eac0: 2020 2020 706f 645f 6166 6669 6e69 7479      pod_affinity
+0001ead0: 5f74 6572 6d3a 0a20 2020 2020 2020 2020  _term:.         
+0001eae0: 2020 2020 206c 6162 656c 5f73 656c 6563       label_selec
+0001eaf0: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
+0001eb00: 2020 202d 2061 7070 3a64 656d 6f2d 6170     - app:demo-ap
+0001eb10: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+0001eb20: 2d20 226b 6579 3a76 6572 7369 6f6e 2c20  - "key:version, 
+0001eb30: 6f70 6572 6174 6f72 3a49 6e2c 2076 616c  operator:In, val
+0001eb40: 7565 733a 5b76 312e 302e 302c 2076 312e  ues:[v1.0.0, v1.
+0001eb50: 302e 315d 220a 2020 2020 2020 2020 2020  0.1]".          
+0001eb60: 2020 2020 746f 706f 6c6f 6779 5f6b 6579      topology_key
+0001eb70: 3a20 746f 706f 6c6f 6779 5f6b 6579 0a20  : topology_key. 
+0001eb80: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+0001eb90: 6573 7061 6365 733a 0a20 2020 2020 2020  espaces:.       
+0001eba0: 2020 2020 2020 202d 206e 616d 6573 7061         - namespa
+0001ebb0: 6365 730a 2020 2020 2020 2020 2020 2020  ces.            
+0001ebc0: 2020 2d20 6e61 6d65 7370 6163 6573 0a20    - namespaces. 
+0001ebd0: 2020 2020 2020 2020 202d 2077 6569 6768           - weigh
+0001ebe0: 743a 2036 0a20 2020 2020 2020 2020 2020  t: 6.           
+0001ebf0: 2070 6f64 5f61 6666 696e 6974 795f 7465   pod_affinity_te
+0001ec00: 726d 3a0a 2020 2020 2020 2020 2020 2020  rm:.            
+0001ec10: 2020 6c61 6265 6c5f 7365 6c65 6374 6f72    label_selector
+0001ec20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001ec30: 2d20 6170 703a 6465 6d6f 2d61 7070 0a20  - app:demo-app. 
+0001ec40: 2020 2020 2020 2020 2020 2020 202d 2022               - "
+0001ec50: 6b65 793a 7665 7273 696f 6e2c 206f 7065  key:version, ope
+0001ec60: 7261 746f 723a 496e 2c20 7661 6c75 6573  rator:In, values
+0001ec70: 3a5b 7631 2e30 2e30 2c20 7631 2e30 2e31  :[v1.0.0, v1.0.1
+0001ec80: 5d22 0a20 2020 2020 2020 2020 2020 2020  ]".             
+0001ec90: 2074 6f70 6f6c 6f67 795f 6b65 793a 2074   topology_key: t
+0001eca0: 6f70 6f6c 6f67 795f 6b65 790a 2020 2020  opology_key.    
+0001ecb0: 2020 2020 2020 2020 2020 6e61 6d65 7370            namesp
+0001ecc0: 6163 6573 3a0a 2020 2020 2020 2020 2020  aces:.          
+0001ecd0: 2020 2020 2d20 6e61 6d65 7370 6163 6573      - namespaces
+0001ece0: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
+0001ecf0: 206e 616d 6573 7061 6365 730a 2020 2020   namespaces.    
+0001ed00: 2020 2020 2020 7265 7175 6972 6564 5f64        required_d
+0001ed10: 7572 696e 675f 7363 6865 6475 6c69 6e67  uring_scheduling
+0001ed20: 5f69 676e 6f72 6564 5f64 7572 696e 675f  _ignored_during_
+0001ed30: 6578 6563 7574 696f 6e3a 0a20 2020 2020  execution:.     
+0001ed40: 2020 2020 202d 206c 6162 656c 5f73 656c       - label_sel
+0001ed50: 6563 746f 723a 0a20 2020 2020 2020 2020  ector:.         
+0001ed60: 2020 202d 2061 7070 3a64 656d 6f2d 6170     - app:demo-ap
+0001ed70: 700a 2020 2020 2020 2020 2020 2020 2d20  p.            - 
+0001ed80: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
+0001ed90: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
+0001eda0: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
+0001edb0: 315d 220a 2020 2020 2020 2020 2020 2020  1]".            
+0001edc0: 746f 706f 6c6f 6779 5f6b 6579 3a20 746f  topology_key: to
+0001edd0: 706f 6c6f 6779 5f6b 6579 0a20 2020 2020  pology_key.     
+0001ede0: 2020 2020 2020 206e 616d 6573 7061 6365         namespace
+0001edf0: 733a 0a20 2020 2020 2020 2020 2020 202d  s:.            -
+0001ee00: 206e 616d 6573 7061 6365 730a 2020 2020   namespaces.    
+0001ee10: 2020 2020 2020 2020 2d20 6e61 6d65 7370          - namesp
+0001ee20: 6163 6573 0a20 2020 2020 2020 2020 202d  aces.          -
+0001ee30: 206c 6162 656c 5f73 656c 6563 746f 723a   label_selector:
+0001ee40: 0a20 2020 2020 2020 2020 2020 202d 2061  .            - a
+0001ee50: 7070 3a64 656d 6f2d 6170 700a 2020 2020  pp:demo-app.    
+0001ee60: 2020 2020 2020 2020 2d20 226b 6579 3a76          - "key:v
+0001ee70: 6572 7369 6f6e 2c20 6f70 6572 6174 6f72  ersion, operator
+0001ee80: 3a49 6e2c 2076 616c 7565 733a 5b76 312e  :In, values:[v1.
+0001ee90: 302e 302c 2076 312e 302e 315d 220a 2020  0.0, v1.0.1]".  
+0001eea0: 2020 2020 2020 2020 2020 746f 706f 6c6f            topolo
+0001eeb0: 6779 5f6b 6579 3a20 746f 706f 6c6f 6779  gy_key: topology
+0001eec0: 5f6b 6579 0a20 2020 2020 2020 2020 2020  _key.           
+0001eed0: 206e 616d 6573 7061 6365 733a 0a20 2020   namespaces:.   
+0001eee0: 2020 2020 2020 2020 202d 206e 616d 6573           - names
+0001eef0: 7061 6365 730a 2020 2020 2020 2020 2020  paces.          
+0001ef00: 2020 2d20 6e61 6d65 7370 6163 6573 0a20    - namespaces. 
+0001ef10: 2020 2020 2070 726f 7065 7274 6965 733a       properties:
+0001ef20: 0a20 2020 2020 2020 206e 6f64 655f 6166  .        node_af
+0001ef30: 6669 6e69 7479 3a0a 2020 2020 2020 2020  finity:.        
+0001ef40: 2020 2472 6566 3a20 2723 2f63 6f6d 706f    $ref: '#/compo
+0001ef50: 6e65 6e74 732f 7363 6865 6d61 732f 4e6f  nents/schemas/No
+0001ef60: 6465 4166 6669 6e69 7479 270a 2020 2020  deAffinity'.    
+0001ef70: 2020 2020 706f 645f 6166 6669 6e69 7479      pod_affinity
+0001ef80: 3a0a 2020 2020 2020 2020 2020 2472 6566  :.          $ref
+0001ef90: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
+0001efa0: 7363 6865 6d61 732f 506f 6441 6666 696e  schemas/PodAffin
+0001efb0: 6974 7927 0a20 2020 2020 2020 2070 6f64  ity'.        pod
+0001efc0: 5f61 6e74 695f 6166 6669 6e69 7479 3a0a  _anti_affinity:.
+0001efd0: 2020 2020 2020 2020 2020 2472 6566 3a20            $ref: 
+0001efe0: 2723 2f63 6f6d 706f 6e65 6e74 732f 7363  '#/components/sc
+0001eff0: 6865 6d61 732f 506f 6441 6e74 6941 6666  hemas/PodAntiAff
+0001f000: 696e 6974 7927 0a20 2020 2020 2074 6974  inity'.      tit
+0001f010: 6c65 3a20 4166 6669 6e69 7479 0a20 2020  le: Affinity.   
+0001f020: 2020 2074 7970 653a 206f 626a 6563 740a     type: object.
+0001f030: 2020 2020 4e6f 6465 4166 6669 6e69 7479      NodeAffinity
+0001f040: 3a0a 2020 2020 2020 6578 616d 706c 653a  :.      example:
+0001f050: 0a20 2020 2020 2020 2070 7265 6665 7272  .        preferr
+0001f060: 6564 5f64 7572 696e 675f 7363 6865 6475  ed_during_schedu
+0001f070: 6c69 6e67 5f69 676e 6f72 6564 5f64 7572  ling_ignored_dur
+0001f080: 696e 675f 6578 6563 7574 696f 6e3a 0a20  ing_execution:. 
+0001f090: 2020 2020 2020 202d 2070 7265 6665 7265         - prefere
+0001f0a0: 6e63 653a 0a20 2020 2020 2020 2020 2020  nce:.           
+0001f0b0: 206d 6174 6368 5f65 7870 7265 7373 696f   match_expressio
+0001f0c0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0001f0d0: 2d20 226b 6579 3a76 6572 7369 6f6e 2c20  - "key:version, 
+0001f0e0: 6f70 6572 6174 6f72 3a49 6e2c 2076 616c  operator:In, val
+0001f0f0: 7565 733a 5b76 312e 302e 302c 2076 312e  ues:[v1.0.0, v1.
+0001f100: 302e 315d 220a 2020 2020 2020 2020 2020  0.1]".          
+0001f110: 2020 6d61 7463 685f 6669 656c 6473 3a0a    match_fields:.
+0001f120: 2020 2020 2020 2020 2020 2020 2d20 226b              - "k
+0001f130: 6579 3a76 6572 7369 6f6e 2c20 6f70 6572  ey:version, oper
+0001f140: 6174 6f72 3a49 6e2c 2076 616c 7565 733a  ator:In, values:
+0001f150: 5b76 312e 302e 302c 2076 312e 302e 315d  [v1.0.0, v1.0.1]
+0001f160: 220a 2020 2020 2020 2020 2020 7765 6967  ".          weig
+0001f170: 6874 3a20 300a 2020 2020 2020 2020 2d20  ht: 0.        - 
+0001f180: 7072 6566 6572 656e 6365 3a0a 2020 2020  preference:.    
+0001f190: 2020 2020 2020 2020 6d61 7463 685f 6578          match_ex
+0001f1a0: 7072 6573 7369 6f6e 733a 0a20 2020 2020  pressions:.     
+0001f1b0: 2020 2020 2020 202d 2022 6b65 793a 7665         - "key:ve
+0001f1c0: 7273 696f 6e2c 206f 7065 7261 746f 723a  rsion, operator:
+0001f1d0: 496e 2c20 7661 6c75 6573 3a5b 7631 2e30  In, values:[v1.0
+0001f1e0: 2e30 2c20 7631 2e30 2e31 5d22 0a20 2020  .0, v1.0.1]".   
+0001f1f0: 2020 2020 2020 2020 206d 6174 6368 5f66           match_f
+0001f200: 6965 6c64 733a 0a20 2020 2020 2020 2020  ields:.         
+0001f210: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
+0001f220: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
+0001f230: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
+0001f240: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
+0001f250: 2020 2077 6569 6768 743a 2030 0a20 2020     weight: 0.   
+0001f260: 2020 2020 2072 6571 7569 7265 645f 6475       required_du
+0001f270: 7269 6e67 5f73 6368 6564 756c 696e 675f  ring_scheduling_
+0001f280: 6967 6e6f 7265 645f 6475 7269 6e67 5f65  ignored_during_e
+0001f290: 7865 6375 7469 6f6e 3a0a 2020 2020 2020  xecution:.      
+0001f2a0: 2020 2020 6e6f 6465 5f73 656c 6563 746f      node_selecto
+0001f2b0: 725f 7465 726d 733a 0a20 2020 2020 2020  r_terms:.       
+0001f2c0: 2020 202d 206d 6174 6368 5f65 7870 7265     - match_expre
+0001f2d0: 7373 696f 6e73 3a0a 2020 2020 2020 2020  ssions:.        
+0001f2e0: 2020 2020 2d20 226b 6579 3a76 6572 7369      - "key:versi
+0001f2f0: 6f6e 2c20 6f70 6572 6174 6f72 3a49 6e2c  on, operator:In,
+0001f300: 2076 616c 7565 733a 5b76 312e 302e 302c   values:[v1.0.0,
+0001f310: 2076 312e 302e 315d 220a 2020 2020 2020   v1.0.1]".      
+0001f320: 2020 2020 2020 6d61 7463 685f 6669 656c        match_fiel
+0001f330: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
+0001f340: 2d20 226b 6579 3a76 6572 7369 6f6e 2c20  - "key:version, 
+0001f350: 6f70 6572 6174 6f72 3a49 6e2c 2076 616c  operator:In, val
+0001f360: 7565 733a 5b76 312e 302e 302c 2076 312e  ues:[v1.0.0, v1.
+0001f370: 302e 315d 220a 2020 2020 2020 2020 2020  0.1]".          
+0001f380: 2d20 6d61 7463 685f 6578 7072 6573 7369  - match_expressi
+0001f390: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+0001f3a0: 202d 2022 6b65 793a 7665 7273 696f 6e2c   - "key:version,
+0001f3b0: 206f 7065 7261 746f 723a 496e 2c20 7661   operator:In, va
+0001f3c0: 6c75 6573 3a5b 7631 2e30 2e30 2c20 7631  lues:[v1.0.0, v1
+0001f3d0: 2e30 2e31 5d22 0a20 2020 2020 2020 2020  .0.1]".         
+0001f3e0: 2020 206d 6174 6368 5f66 6965 6c64 733a     match_fields:
+0001f3f0: 0a20 2020 2020 2020 2020 2020 202d 2022  .            - "
+0001f400: 6b65 793a 7665 7273 696f 6e2c 206f 7065  key:version, ope
+0001f410: 7261 746f 723a 496e 2c20 7661 6c75 6573  rator:In, values
+0001f420: 3a5b 7631 2e30 2e30 2c20 7631 2e30 2e31  :[v1.0.0, v1.0.1
+0001f430: 5d22 0a20 2020 2020 2070 726f 7065 7274  ]".      propert
+0001f440: 6965 733a 0a20 2020 2020 2020 2072 6571  ies:.        req
+0001f450: 7569 7265 645f 6475 7269 6e67 5f73 6368  uired_during_sch
+0001f460: 6564 756c 696e 675f 6967 6e6f 7265 645f  eduling_ignored_
+0001f470: 6475 7269 6e67 5f65 7865 6375 7469 6f6e  during_execution
+0001f480: 3a0a 2020 2020 2020 2020 2020 2472 6566  :.          $ref
+0001f490: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
+0001f4a0: 7363 6865 6d61 732f 4e6f 6465 5365 6c65  schemas/NodeSele
+0001f4b0: 6374 6f72 270a 2020 2020 2020 2020 7072  ctor'.        pr
+0001f4c0: 6566 6572 7265 645f 6475 7269 6e67 5f73  eferred_during_s
+0001f4d0: 6368 6564 756c 696e 675f 6967 6e6f 7265  cheduling_ignore
+0001f4e0: 645f 6475 7269 6e67 5f65 7865 6375 7469  d_during_executi
+0001f4f0: 6f6e 3a0a 2020 2020 2020 2020 2020 6974  on:.          it
+0001f500: 656d 733a 0a20 2020 2020 2020 2020 2020  ems:.           
+0001f510: 2024 7265 663a 2027 232f 636f 6d70 6f6e   $ref: '#/compon
+0001f520: 656e 7473 2f73 6368 656d 6173 2f50 7265  ents/schemas/Pre
+0001f530: 6665 7272 6564 5363 6865 6475 6c69 6e67  ferredScheduling
+0001f540: 5465 726d 270a 2020 2020 2020 2020 2020  Term'.          
+0001f550: 7469 746c 653a 2070 7265 6665 7272 6564  title: preferred
+0001f560: 5f64 7572 696e 675f 7363 6865 6475 6c69  _during_scheduli
+0001f570: 6e67 5f69 676e 6f72 6564 5f64 7572 696e  ng_ignored_durin
+0001f580: 675f 6578 6563 7574 696f 6e0a 2020 2020  g_execution.    
+0001f590: 2020 2020 2020 7479 7065 3a20 6172 7261        type: arra
+0001f5a0: 790a 2020 2020 2020 7469 746c 653a 204e  y.      title: N
+0001f5b0: 6f64 6541 6666 696e 6974 790a 2020 2020  odeAffinity.    
+0001f5c0: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
+0001f5d0: 2020 204e 6f64 6553 656c 6563 746f 723a     NodeSelector:
+0001f5e0: 0a20 2020 2020 2065 7861 6d70 6c65 3a0a  .      example:.
+0001f5f0: 2020 2020 2020 2020 6e6f 6465 5f73 656c          node_sel
+0001f600: 6563 746f 725f 7465 726d 733a 0a20 2020  ector_terms:.   
+0001f610: 2020 2020 202d 206d 6174 6368 5f65 7870       - match_exp
+0001f620: 7265 7373 696f 6e73 3a0a 2020 2020 2020  ressions:.      
+0001f630: 2020 2020 2d20 226b 6579 3a76 6572 7369      - "key:versi
+0001f640: 6f6e 2c20 6f70 6572 6174 6f72 3a49 6e2c  on, operator:In,
+0001f650: 2076 616c 7565 733a 5b76 312e 302e 302c   values:[v1.0.0,
+0001f660: 2076 312e 302e 315d 220a 2020 2020 2020   v1.0.1]".      
+0001f670: 2020 2020 6d61 7463 685f 6669 656c 6473      match_fields
+0001f680: 3a0a 2020 2020 2020 2020 2020 2d20 226b  :.          - "k
+0001f690: 6579 3a76 6572 7369 6f6e 2c20 6f70 6572  ey:version, oper
+0001f6a0: 6174 6f72 3a49 6e2c 2076 616c 7565 733a  ator:In, values:
+0001f6b0: 5b76 312e 302e 302c 2076 312e 302e 315d  [v1.0.0, v1.0.1]
+0001f6c0: 220a 2020 2020 2020 2020 2d20 6d61 7463  ".        - matc
+0001f6d0: 685f 6578 7072 6573 7369 6f6e 733a 0a20  h_expressions:. 
+0001f6e0: 2020 2020 2020 2020 202d 2022 6b65 793a           - "key:
+0001f6f0: 7665 7273 696f 6e2c 206f 7065 7261 746f  version, operato
+0001f700: 723a 496e 2c20 7661 6c75 6573 3a5b 7631  r:In, values:[v1
+0001f710: 2e30 2e30 2c20 7631 2e30 2e31 5d22 0a20  .0.0, v1.0.1]". 
+0001f720: 2020 2020 2020 2020 206d 6174 6368 5f66           match_f
+0001f730: 6965 6c64 733a 0a20 2020 2020 2020 2020  ields:.         
+0001f740: 202d 2022 6b65 793a 7665 7273 696f 6e2c   - "key:version,
+0001f750: 206f 7065 7261 746f 723a 496e 2c20 7661   operator:In, va
+0001f760: 6c75 6573 3a5b 7631 2e30 2e30 2c20 7631  lues:[v1.0.0, v1
+0001f770: 2e30 2e31 5d22 0a20 2020 2020 2070 726f  .0.1]".      pro
+0001f780: 7065 7274 6965 733a 0a20 2020 2020 2020  perties:.       
+0001f790: 206e 6f64 655f 7365 6c65 6374 6f72 5f74   node_selector_t
+0001f7a0: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
+0001f7b0: 6974 656d 733a 0a20 2020 2020 2020 2020  items:.         
+0001f7c0: 2020 2024 7265 663a 2027 232f 636f 6d70     $ref: '#/comp
+0001f7d0: 6f6e 656e 7473 2f73 6368 656d 6173 2f4e  onents/schemas/N
+0001f7e0: 6f64 6553 656c 6563 746f 7254 6572 6d27  odeSelectorTerm'
+0001f7f0: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
+0001f800: 3a20 6e6f 6465 5f73 656c 6563 746f 725f  : node_selector_
+0001f810: 7465 726d 730a 2020 2020 2020 2020 2020  terms.          
+0001f820: 7479 7065 3a20 6172 7261 790a 2020 2020  type: array.    
+0001f830: 2020 7469 746c 653a 204e 6f64 6553 656c    title: NodeSel
+0001f840: 6563 746f 720a 2020 2020 2020 7479 7065  ector.      type
+0001f850: 3a20 6f62 6a65 6374 0a20 2020 204e 6f64  : object.    Nod
+0001f860: 6553 656c 6563 746f 7254 6572 6d3a 0a20  eSelectorTerm:. 
+0001f870: 2020 2020 2065 7861 6d70 6c65 3a0a 2020       example:.  
+0001f880: 2020 2020 2020 6d61 7463 685f 6578 7072        match_expr
+0001f890: 6573 7369 6f6e 733a 0a20 2020 2020 2020  essions:.       
+0001f8a0: 202d 2022 6b65 793a 7665 7273 696f 6e2c   - "key:version,
+0001f8b0: 206f 7065 7261 746f 723a 496e 2c20 7661   operator:In, va
+0001f8c0: 6c75 6573 3a5b 7631 2e30 2e30 2c20 7631  lues:[v1.0.0, v1
+0001f8d0: 2e30 2e31 5d22 0a20 2020 2020 2020 206d  .0.1]".        m
+0001f8e0: 6174 6368 5f66 6965 6c64 733a 0a20 2020  atch_fields:.   
+0001f8f0: 2020 2020 202d 2022 6b65 793a 7665 7273       - "key:vers
+0001f900: 696f 6e2c 206f 7065 7261 746f 723a 496e  ion, operator:In
+0001f910: 2c20 7661 6c75 6573 3a5b 7631 2e30 2e30  , values:[v1.0.0
+0001f920: 2c20 7631 2e30 2e31 5d22 0a20 2020 2020  , v1.0.1]".     
+0001f930: 2070 726f 7065 7274 6965 733a 0a20 2020   properties:.   
+0001f940: 2020 2020 206d 6174 6368 5f65 7870 7265       match_expre
+0001f950: 7373 696f 6e73 3a0a 2020 2020 2020 2020  ssions:.        
+0001f960: 2020 6465 7363 7269 7074 696f 6e3a 207c    description: |
+0001f970: 0a20 2020 2020 2020 2020 2020 2041 6e20  .            An 
+0001f980: 6172 7261 7920 6f66 206e 6f64 6520 7365  array of node se
+0001f990: 6c65 6374 6f72 2072 756c 652c 2074 6865  lector rule, the
+0001f9a0: 2072 756c 6520 6361 6e20 6265 2061 206d   rule can be a m
+0001f9b0: 6174 6368 2065 7870 7265 7373 696f 6e2c  atch expression,
+0001f9c0: 0a20 2020 2020 2020 2020 2020 2072 6566  .            ref
+0001f9d0: 6572 7269 6e67 2074 6865 2065 7861 6d70  erring the examp
+0001f9e0: 6c65 2028 4974 2069 7320 6120 6d61 7463  le (It is a matc
+0001f9f0: 6820 6578 7072 6573 7369 6f6e 290a 2020  h expression).  
+0001fa00: 2020 2020 2020 2020 6578 616d 706c 653a          example:
+0001fa10: 0a20 2020 2020 2020 2020 202d 2022 6b65  .          - "ke
+0001fa20: 793a 7665 7273 696f 6e2c 206f 7065 7261  y:version, opera
+0001fa30: 746f 723a 496e 2c20 7661 6c75 6573 3a5b  tor:In, values:[
+0001fa40: 7631 2e30 2e30 2c20 7631 2e30 2e31 5d22  v1.0.0, v1.0.1]"
+0001fa50: 0a20 2020 2020 2020 2020 2069 7465 6d73  .          items
+0001fa60: 3a0a 2020 2020 2020 2020 2020 2020 7479  :.            ty
+0001fa70: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
+0001fa80: 2020 2020 2074 6974 6c65 3a20 4e6f 6465       title: Node
+0001fa90: 5365 6c65 6374 6f72 5265 7175 6972 656d  SelectorRequirem
+0001faa0: 656e 740a 2020 2020 2020 2020 2020 7479  ent.          ty
+0001fab0: 7065 3a20 6172 7261 790a 2020 2020 2020  pe: array.      
+0001fac0: 2020 6d61 7463 685f 6669 656c 6473 3a0a    match_fields:.
+0001fad0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+0001fae0: 7074 696f 6e3a 207c 0a20 2020 2020 2020  ption: |.       
+0001faf0: 2020 2020 2041 6e20 6172 7261 7920 6f66       An array of
+0001fb00: 206e 6f64 6520 7365 6c65 6374 6f72 2072   node selector r
+0001fb10: 756c 652c 2074 6865 2072 756c 6520 6361  ule, the rule ca
+0001fb20: 6e20 6265 2061 206d 6174 6368 2065 7870  n be a match exp
+0001fb30: 7265 7373 696f 6e2c 0a20 2020 2020 2020  ression,.       
+0001fb40: 2020 2020 2072 6566 6572 7269 6e67 2074       referring t
+0001fb50: 6865 2065 7861 6d70 6c65 2028 4974 2069  he example (It i
+0001fb60: 7320 6120 6d61 7463 6820 6578 7072 6573  s a match expres
+0001fb70: 7369 6f6e 290a 2020 2020 2020 2020 2020  sion).          
+0001fb80: 6578 616d 706c 653a 0a20 2020 2020 2020  example:.       
+0001fb90: 2020 202d 2022 6b65 793a 7665 7273 696f     - "key:versio
+0001fba0: 6e2c 206f 7065 7261 746f 723a 496e 2c20  n, operator:In, 
+0001fbb0: 7661 6c75 6573 3a5b 7631 2e30 2e30 2c20  values:[v1.0.0, 
+0001fbc0: 7631 2e30 2e31 5d22 0a20 2020 2020 2020  v1.0.1]".       
+0001fbd0: 2020 2069 7465 6d73 3a0a 2020 2020 2020     items:.      
+0001fbe0: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+0001fbf0: 6e67 0a20 2020 2020 2020 2020 2074 6974  ng.          tit
+0001fc00: 6c65 3a20 4e6f 6465 5365 6c65 6374 6f72  le: NodeSelector
+0001fc10: 5265 7175 6972 656d 656e 740a 2020 2020  Requirement.    
+0001fc20: 2020 2020 2020 7479 7065 3a20 6172 7261        type: arra
+0001fc30: 790a 2020 2020 2020 7469 746c 653a 204e  y.      title: N
+0001fc40: 6f64 6553 656c 6563 746f 7254 6572 6d0a  odeSelectorTerm.
+0001fc50: 2020 2020 2020 7479 7065 3a20 6f62 6a65        type: obje
+0001fc60: 6374 0a20 2020 204e 6f64 6553 656c 6563  ct.    NodeSelec
+0001fc70: 746f 7252 6571 7569 7265 6d65 6e74 3a0a  torRequirement:.
+0001fc80: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+0001fc90: 6e3a 207c 0a20 2020 2020 2020 2041 6e20  n: |.        An 
+0001fca0: 6172 7261 7920 6f66 206e 6f64 6520 7365  array of node se
+0001fcb0: 6c65 6374 6f72 2072 756c 652c 2074 6865  lector rule, the
+0001fcc0: 2072 756c 6520 6361 6e20 6265 2061 206d   rule can be a m
+0001fcd0: 6174 6368 2065 7870 7265 7373 696f 6e2c  atch expression,
+0001fce0: 0a20 2020 2020 2020 2072 6566 6572 7269  .        referri
+0001fcf0: 6e67 2074 6865 2065 7861 6d70 6c65 2028  ng the example (
+0001fd00: 4974 2069 7320 6120 6d61 7463 6820 6578  It is a match ex
+0001fd10: 7072 6573 7369 6f6e 290a 2020 2020 2020  pression).      
+0001fd20: 6578 616d 706c 653a 0a20 2020 2020 202d  example:.      -
+0001fd30: 2022 6b65 793a 7665 7273 696f 6e2c 206f   "key:version, o
+0001fd40: 7065 7261 746f 723a 496e 2c20 7661 6c75  perator:In, valu
+0001fd50: 6573 3a5b 7631 2e30 2e30 2c20 7631 2e30  es:[v1.0.0, v1.0
+0001fd60: 2e31 5d22 0a20 2020 2020 2069 7465 6d73  .1]".      items
+0001fd70: 3a0a 2020 2020 2020 2020 7479 7065 3a20  :.        type: 
+0001fd80: 7374 7269 6e67 0a20 2020 2020 2074 6974  string.      tit
+0001fd90: 6c65 3a20 4e6f 6465 5365 6c65 6374 6f72  le: NodeSelector
+0001fda0: 5265 7175 6972 656d 656e 740a 2020 2020  Requirement.    
+0001fdb0: 2020 7479 7065 3a20 6172 7261 790a 2020    type: array.  
+0001fdc0: 2020 5072 6566 6572 7265 6453 6368 6564    PreferredSched
+0001fdd0: 756c 696e 6754 6572 6d3a 0a20 2020 2020  ulingTerm:.     
+0001fde0: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
+0001fdf0: 2020 7072 6566 6572 656e 6365 3a0a 2020    preference:.  
+0001fe00: 2020 2020 2020 2020 6d61 7463 685f 6578          match_ex
+0001fe10: 7072 6573 7369 6f6e 733a 0a20 2020 2020  pressions:.     
+0001fe20: 2020 2020 202d 2022 6b65 793a 7665 7273       - "key:vers
+0001fe30: 696f 6e2c 206f 7065 7261 746f 723a 496e  ion, operator:In
+0001fe40: 2c20 7661 6c75 6573 3a5b 7631 2e30 2e30  , values:[v1.0.0
+0001fe50: 2c20 7631 2e30 2e31 5d22 0a20 2020 2020  , v1.0.1]".     
+0001fe60: 2020 2020 206d 6174 6368 5f66 6965 6c64       match_field
+0001fe70: 733a 0a20 2020 2020 2020 2020 202d 2022  s:.          - "
+0001fe80: 6b65 793a 7665 7273 696f 6e2c 206f 7065  key:version, ope
+0001fe90: 7261 746f 723a 496e 2c20 7661 6c75 6573  rator:In, values
+0001fea0: 3a5b 7631 2e30 2e30 2c20 7631 2e30 2e31  :[v1.0.0, v1.0.1
+0001feb0: 5d22 0a20 2020 2020 2020 2077 6569 6768  ]".        weigh
+0001fec0: 743a 2030 0a20 2020 2020 2070 726f 7065  t: 0.      prope
+0001fed0: 7274 6965 733a 0a20 2020 2020 2020 2077  rties:.        w
+0001fee0: 6569 6768 743a 0a20 2020 2020 2020 2020  eight:.         
+0001fef0: 2074 6974 6c65 3a20 7765 6967 6874 0a20   title: weight. 
+0001ff00: 2020 2020 2020 2020 2074 7970 653a 2069           type: i
+0001ff10: 6e74 6567 6572 0a20 2020 2020 2020 2070  nteger.        p
+0001ff20: 7265 6665 7265 6e63 653a 0a20 2020 2020  reference:.     
+0001ff30: 2020 2020 2024 7265 663a 2027 232f 636f       $ref: '#/co
+0001ff40: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+0001ff50: 2f4e 6f64 6553 656c 6563 746f 7254 6572  /NodeSelectorTer
+0001ff60: 6d27 0a20 2020 2020 2074 6974 6c65 3a20  m'.      title: 
+0001ff70: 5072 6566 6572 7265 6453 6368 6564 756c  PreferredSchedul
+0001ff80: 696e 6754 6572 6d0a 2020 2020 2020 7479  ingTerm.      ty
+0001ff90: 7065 3a20 6f62 6a65 6374 0a20 2020 2050  pe: object.    P
+0001ffa0: 6f64 4166 6669 6e69 7479 3a0a 2020 2020  odAffinity:.    
+0001ffb0: 2020 6578 616d 706c 653a 0a20 2020 2020    example:.     
+0001ffc0: 2020 2070 7265 6665 7272 6564 5f64 7572     preferred_dur
+0001ffd0: 696e 675f 7363 6865 6475 6c69 6e67 5f69  ing_scheduling_i
+0001ffe0: 676e 6f72 6564 5f64 7572 696e 675f 6578  gnored_during_ex
+0001fff0: 6563 7574 696f 6e3a 0a20 2020 2020 2020  ecution:.       
+00020000: 202d 2077 6569 6768 743a 2036 0a20 2020   - weight: 6.   
+00020010: 2020 2020 2020 2070 6f64 5f61 6666 696e         pod_affin
+00020020: 6974 795f 7465 726d 3a0a 2020 2020 2020  ity_term:.      
+00020030: 2020 2020 2020 6c61 6265 6c5f 7365 6c65        label_sele
+00020040: 6374 6f72 3a0a 2020 2020 2020 2020 2020  ctor:.          
+00020050: 2020 2d20 6170 703a 6465 6d6f 2d61 7070    - app:demo-app
+00020060: 0a20 2020 2020 2020 2020 2020 202d 2022  .            - "
+00020070: 6b65 793a 7665 7273 696f 6e2c 206f 7065  key:version, ope
+00020080: 7261 746f 723a 496e 2c20 7661 6c75 6573  rator:In, values
+00020090: 3a5b 7631 2e30 2e30 2c20 7631 2e30 2e31  :[v1.0.0, v1.0.1
+000200a0: 5d22 0a20 2020 2020 2020 2020 2020 2074  ]".            t
+000200b0: 6f70 6f6c 6f67 795f 6b65 793a 2074 6f70  opology_key: top
+000200c0: 6f6c 6f67 795f 6b65 790a 2020 2020 2020  ology_key.      
+000200d0: 2020 2020 2020 6e61 6d65 7370 6163 6573        namespaces
+000200e0: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
+000200f0: 6e61 6d65 7370 6163 6573 0a20 2020 2020  namespaces.     
+00020100: 2020 2020 2020 202d 206e 616d 6573 7061         - namespa
+00020110: 6365 730a 2020 2020 2020 2020 2d20 7765  ces.        - we
+00020120: 6967 6874 3a20 360a 2020 2020 2020 2020  ight: 6.        
+00020130: 2020 706f 645f 6166 6669 6e69 7479 5f74    pod_affinity_t
+00020140: 6572 6d3a 0a20 2020 2020 2020 2020 2020  erm:.           
+00020150: 206c 6162 656c 5f73 656c 6563 746f 723a   label_selector:
+00020160: 0a20 2020 2020 2020 2020 2020 202d 2061  .            - a
+00020170: 7070 3a64 656d 6f2d 6170 700a 2020 2020  pp:demo-app.    
+00020180: 2020 2020 2020 2020 2d20 226b 6579 3a76          - "key:v
+00020190: 6572 7369 6f6e 2c20 6f70 6572 6174 6f72  ersion, operator
+000201a0: 3a49 6e2c 2076 616c 7565 733a 5b76 312e  :In, values:[v1.
+000201b0: 302e 302c 2076 312e 302e 315d 220a 2020  0.0, v1.0.1]".  
+000201c0: 2020 2020 2020 2020 2020 746f 706f 6c6f            topolo
+000201d0: 6779 5f6b 6579 3a20 746f 706f 6c6f 6779  gy_key: topology
+000201e0: 5f6b 6579 0a20 2020 2020 2020 2020 2020  _key.           
+000201f0: 206e 616d 6573 7061 6365 733a 0a20 2020   namespaces:.   
+00020200: 2020 2020 2020 2020 202d 206e 616d 6573           - names
+00020210: 7061 6365 730a 2020 2020 2020 2020 2020  paces.          
+00020220: 2020 2d20 6e61 6d65 7370 6163 6573 0a20    - namespaces. 
+00020230: 2020 2020 2020 2072 6571 7569 7265 645f         required_
+00020240: 6475 7269 6e67 5f73 6368 6564 756c 696e  during_schedulin
+00020250: 675f 6967 6e6f 7265 645f 6475 7269 6e67  g_ignored_during
+00020260: 5f65 7865 6375 7469 6f6e 3a0a 2020 2020  _execution:.    
+00020270: 2020 2020 2d20 6c61 6265 6c5f 7365 6c65      - label_sele
+00020280: 6374 6f72 3a0a 2020 2020 2020 2020 2020  ctor:.          
+00020290: 2d20 6170 703a 6465 6d6f 2d61 7070 0a20  - app:demo-app. 
+000202a0: 2020 2020 2020 2020 202d 2022 6b65 793a           - "key:
+000202b0: 7665 7273 696f 6e2c 206f 7065 7261 746f  version, operato
+000202c0: 723a 496e 2c20 7661 6c75 6573 3a5b 7631  r:In, values:[v1
+000202d0: 2e30 2e30 2c20 7631 2e30 2e31 5d22 0a20  .0.0, v1.0.1]". 
+000202e0: 2020 2020 2020 2020 2074 6f70 6f6c 6f67           topolog
+000202f0: 795f 6b65 793a 2074 6f70 6f6c 6f67 795f  y_key: topology_
+00020300: 6b65 790a 2020 2020 2020 2020 2020 6e61  key.          na
+00020310: 6d65 7370 6163 6573 3a0a 2020 2020 2020  mespaces:.      
+00020320: 2020 2020 2d20 6e61 6d65 7370 6163 6573      - namespaces
+00020330: 0a20 2020 2020 2020 2020 202d 206e 616d  .          - nam
+00020340: 6573 7061 6365 730a 2020 2020 2020 2020  espaces.        
+00020350: 2d20 6c61 6265 6c5f 7365 6c65 6374 6f72  - label_selector
+00020360: 3a0a 2020 2020 2020 2020 2020 2d20 6170  :.          - ap
+00020370: 703a 6465 6d6f 2d61 7070 0a20 2020 2020  p:demo-app.     
+00020380: 2020 2020 202d 2022 6b65 793a 7665 7273       - "key:vers
+00020390: 696f 6e2c 206f 7065 7261 746f 723a 496e  ion, operator:In
+000203a0: 2c20 7661 6c75 6573 3a5b 7631 2e30 2e30  , values:[v1.0.0
+000203b0: 2c20 7631 2e30 2e31 5d22 0a20 2020 2020  , v1.0.1]".     
+000203c0: 2020 2020 2074 6f70 6f6c 6f67 795f 6b65       topology_ke
+000203d0: 793a 2074 6f70 6f6c 6f67 795f 6b65 790a  y: topology_key.
+000203e0: 2020 2020 2020 2020 2020 6e61 6d65 7370            namesp
+000203f0: 6163 6573 3a0a 2020 2020 2020 2020 2020  aces:.          
+00020400: 2d20 6e61 6d65 7370 6163 6573 0a20 2020  - namespaces.   
+00020410: 2020 2020 2020 202d 206e 616d 6573 7061         - namespa
+00020420: 6365 730a 2020 2020 2020 7072 6f70 6572  ces.      proper
+00020430: 7469 6573 3a0a 2020 2020 2020 2020 7265  ties:.        re
+00020440: 7175 6972 6564 5f64 7572 696e 675f 7363  quired_during_sc
+00020450: 6865 6475 6c69 6e67 5f69 676e 6f72 6564  heduling_ignored
+00020460: 5f64 7572 696e 675f 6578 6563 7574 696f  _during_executio
+00020470: 6e3a 0a20 2020 2020 2020 2020 2069 7465  n:.          ite
+00020480: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
+00020490: 2472 6566 3a20 2723 2f63 6f6d 706f 6e65  $ref: '#/compone
+000204a0: 6e74 732f 7363 6865 6d61 732f 506f 6441  nts/schemas/PodA
+000204b0: 6666 696e 6974 7954 6572 6d27 0a20 2020  ffinityTerm'.   
+000204c0: 2020 2020 2020 2074 6974 6c65 3a20 7265         title: re
+000204d0: 7175 6972 6564 5f64 7572 696e 675f 7363  quired_during_sc
+000204e0: 6865 6475 6c69 6e67 5f69 676e 6f72 6564  heduling_ignored
+000204f0: 5f64 7572 696e 675f 6578 6563 7574 696f  _during_executio
+00020500: 6e0a 2020 2020 2020 2020 2020 7479 7065  n.          type
+00020510: 3a20 6172 7261 790a 2020 2020 2020 2020  : array.        
+00020520: 7072 6566 6572 7265 645f 6475 7269 6e67  preferred_during
+00020530: 5f73 6368 6564 756c 696e 675f 6967 6e6f  _scheduling_igno
+00020540: 7265 645f 6475 7269 6e67 5f65 7865 6375  red_during_execu
+00020550: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+00020560: 6974 656d 733a 0a20 2020 2020 2020 2020  items:.         
+00020570: 2020 2024 7265 663a 2027 232f 636f 6d70     $ref: '#/comp
+00020580: 6f6e 656e 7473 2f73 6368 656d 6173 2f57  onents/schemas/W
+00020590: 6569 6768 7465 6450 6f64 4166 6669 6e69  eightedPodAffini
+000205a0: 7479 5465 726d 270a 2020 2020 2020 2020  tyTerm'.        
+000205b0: 2020 7469 746c 653a 2070 7265 6665 7272    title: preferr
+000205c0: 6564 5f64 7572 696e 675f 7363 6865 6475  ed_during_schedu
+000205d0: 6c69 6e67 5f69 676e 6f72 6564 5f64 7572  ling_ignored_dur
+000205e0: 696e 675f 6578 6563 7574 696f 6e0a 2020  ing_execution.  
+000205f0: 2020 2020 2020 2020 7479 7065 3a20 6172          type: ar
+00020600: 7261 790a 2020 2020 2020 7469 746c 653a  ray.      title:
+00020610: 2050 6f64 4166 6669 6e69 7479 0a20 2020   PodAffinity.   
+00020620: 2020 2074 7970 653a 206f 626a 6563 740a     type: object.
+00020630: 2020 2020 506f 6441 6666 696e 6974 7954      PodAffinityT
+00020640: 6572 6d3a 0a20 2020 2020 2065 7861 6d70  erm:.      examp
+00020650: 6c65 3a0a 2020 2020 2020 2020 6c61 6265  le:.        labe
+00020660: 6c5f 7365 6c65 6374 6f72 3a0a 2020 2020  l_selector:.    
+00020670: 2020 2020 2d20 6170 703a 6465 6d6f 2d61      - app:demo-a
+00020680: 7070 0a20 2020 2020 2020 202d 2022 6b65  pp.        - "ke
+00020690: 793a 7665 7273 696f 6e2c 206f 7065 7261  y:version, opera
+000206a0: 746f 723a 496e 2c20 7661 6c75 6573 3a5b  tor:In, values:[
+000206b0: 7631 2e30 2e30 2c20 7631 2e30 2e31 5d22  v1.0.0, v1.0.1]"
+000206c0: 0a20 2020 2020 2020 2074 6f70 6f6c 6f67  .        topolog
+000206d0: 795f 6b65 793a 2074 6f70 6f6c 6f67 795f  y_key: topology_
+000206e0: 6b65 790a 2020 2020 2020 2020 6e61 6d65  key.        name
+000206f0: 7370 6163 6573 3a0a 2020 2020 2020 2020  spaces:.        
+00020700: 2d20 6e61 6d65 7370 6163 6573 0a20 2020  - namespaces.   
+00020710: 2020 2020 202d 206e 616d 6573 7061 6365       - namespace
+00020720: 730a 2020 2020 2020 7072 6f70 6572 7469  s.      properti
+00020730: 6573 3a0a 2020 2020 2020 2020 6c61 6265  es:.        labe
+00020740: 6c5f 7365 6c65 6374 6f72 3a0a 2020 2020  l_selector:.    
+00020750: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00020760: 6e3a 207c 0a20 2020 2020 2020 2020 2020  n: |.           
+00020770: 2041 6e20 6172 7261 7920 6f66 206c 6162   An array of lab
+00020780: 656c 2073 656c 6563 746f 7220 7275 6c65  el selector rule
+00020790: 2c20 7468 6520 7275 6c65 2063 616e 2065  , the rule can e
+000207a0: 6974 6865 7220 6265 2061 206d 6174 6368  ither be a match
+000207b0: 206c 6162 656c 206f 7220 6d61 7463 6820   label or match 
+000207c0: 6578 7072 6573 7369 6f6e 2c0a 2020 2020  expression,.    
+000207d0: 2020 2020 2020 2020 7265 6665 7272 696e          referrin
+000207e0: 6720 7468 6520 6578 616d 706c 6520 2866  g the example (f
+000207f0: 6972 7374 2069 7320 6120 6d61 7463 6820  irst is a match 
+00020800: 6c61 6265 6c2c 2073 6563 6f6e 6420 6973  label, second is
+00020810: 2061 206d 6174 6368 2065 7870 7265 7373   a match express
+00020820: 696f 6e29 0a20 2020 2020 2020 2020 2065  ion).          e
+00020830: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
+00020840: 2020 2d20 6170 703a 6465 6d6f 2d61 7070    - app:demo-app
+00020850: 0a20 2020 2020 2020 2020 202d 2022 6b65  .          - "ke
+00020860: 793a 7665 7273 696f 6e2c 206f 7065 7261  y:version, opera
+00020870: 746f 723a 496e 2c20 7661 6c75 6573 3a5b  tor:In, values:[
+00020880: 7631 2e30 2e30 2c20 7631 2e30 2e31 5d22  v1.0.0, v1.0.1]"
+00020890: 0a20 2020 2020 2020 2020 2069 7465 6d73  .          items
+000208a0: 3a0a 2020 2020 2020 2020 2020 2020 7479  :.            ty
+000208b0: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
+000208c0: 2020 2020 2074 6974 6c65 3a20 4c61 6265       title: Labe
+000208d0: 6c53 656c 6563 746f 720a 2020 2020 2020  lSelector.      
+000208e0: 2020 2020 7479 7065 3a20 6172 7261 790a      type: array.
+000208f0: 2020 2020 2020 2020 6e61 6d65 7370 6163          namespac
+00020900: 6573 3a0a 2020 2020 2020 2020 2020 6974  es:.          it
+00020910: 656d 733a 0a20 2020 2020 2020 2020 2020  ems:.           
+00020920: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
+00020930: 2020 2020 2020 2020 7469 746c 653a 206e          title: n
+00020940: 616d 6573 7061 6365 730a 2020 2020 2020  amespaces.      
+00020950: 2020 2020 7479 7065 3a20 6172 7261 790a      type: array.
+00020960: 2020 2020 2020 2020 746f 706f 6c6f 6779          topology
+00020970: 5f6b 6579 3a0a 2020 2020 2020 2020 2020  _key:.          
+00020980: 7469 746c 653a 2074 6f70 6f6c 6f67 795f  title: topology_
+00020990: 6b65 790a 2020 2020 2020 2020 2020 7479  key.          ty
+000209a0: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
+000209b0: 2074 6974 6c65 3a20 506f 6441 6666 696e   title: PodAffin
+000209c0: 6974 7954 6572 6d0a 2020 2020 2020 7479  ityTerm.      ty
+000209d0: 7065 3a20 6f62 6a65 6374 0a20 2020 2057  pe: object.    W
+000209e0: 6569 6768 7465 6450 6f64 4166 6669 6e69  eightedPodAffini
+000209f0: 7479 5465 726d 3a0a 2020 2020 2020 6578  tyTerm:.      ex
+00020a00: 616d 706c 653a 0a20 2020 2020 2020 2077  ample:.        w
+00020a10: 6569 6768 743a 2036 0a20 2020 2020 2020  eight: 6.       
+00020a20: 2070 6f64 5f61 6666 696e 6974 795f 7465   pod_affinity_te
+00020a30: 726d 3a0a 2020 2020 2020 2020 2020 6c61  rm:.          la
+00020a40: 6265 6c5f 7365 6c65 6374 6f72 3a0a 2020  bel_selector:.  
+00020a50: 2020 2020 2020 2020 2d20 6170 703a 6465          - app:de
+00020a60: 6d6f 2d61 7070 0a20 2020 2020 2020 2020  mo-app.         
+00020a70: 202d 2022 6b65 793a 7665 7273 696f 6e2c   - "key:version,
+00020a80: 206f 7065 7261 746f 723a 496e 2c20 7661   operator:In, va
+00020a90: 6c75 6573 3a5b 7631 2e30 2e30 2c20 7631  lues:[v1.0.0, v1
+00020aa0: 2e30 2e31 5d22 0a20 2020 2020 2020 2020  .0.1]".         
+00020ab0: 2074 6f70 6f6c 6f67 795f 6b65 793a 2074   topology_key: t
+00020ac0: 6f70 6f6c 6f67 795f 6b65 790a 2020 2020  opology_key.    
+00020ad0: 2020 2020 2020 6e61 6d65 7370 6163 6573        namespaces
+00020ae0: 3a0a 2020 2020 2020 2020 2020 2d20 6e61  :.          - na
+00020af0: 6d65 7370 6163 6573 0a20 2020 2020 2020  mespaces.       
+00020b00: 2020 202d 206e 616d 6573 7061 6365 730a     - namespaces.
+00020b10: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
+00020b20: 3a0a 2020 2020 2020 2020 7765 6967 6874  :.        weight
+00020b30: 3a0a 2020 2020 2020 2020 2020 7469 746c  :.          titl
+00020b40: 653a 2077 6569 6768 740a 2020 2020 2020  e: weight.      
+00020b50: 2020 2020 7479 7065 3a20 696e 7465 6765      type: intege
+00020b60: 720a 2020 2020 2020 2020 706f 645f 6166  r.        pod_af
+00020b70: 6669 6e69 7479 5f74 6572 6d3a 0a20 2020  finity_term:.   
+00020b80: 2020 2020 2020 2024 7265 663a 2027 232f         $ref: '#/
+00020b90: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00020ba0: 6173 2f50 6f64 4166 6669 6e69 7479 5465  as/PodAffinityTe
+00020bb0: 726d 270a 2020 2020 2020 7469 746c 653a  rm'.      title:
+00020bc0: 2057 6569 6768 7465 6450 6f64 4166 6669   WeightedPodAffi
+00020bd0: 6e69 7479 5465 726d 0a20 2020 2020 2074  nityTerm.      t
+00020be0: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
+00020bf0: 506f 6441 6e74 6941 6666 696e 6974 793a  PodAntiAffinity:
+00020c00: 0a20 2020 2020 2065 7861 6d70 6c65 3a0a  .      example:.
+00020c10: 2020 2020 2020 2020 7072 6566 6572 7265          preferre
+00020c20: 645f 6475 7269 6e67 5f73 6368 6564 756c  d_during_schedul
+00020c30: 696e 675f 6967 6e6f 7265 645f 6475 7269  ing_ignored_duri
+00020c40: 6e67 5f65 7865 6375 7469 6f6e 3a0a 2020  ng_execution:.  
+00020c50: 2020 2020 2020 2d20 7765 6967 6874 3a20        - weight: 
+00020c60: 360a 2020 2020 2020 2020 2020 706f 645f  6.          pod_
+00020c70: 6166 6669 6e69 7479 5f74 6572 6d3a 0a20  affinity_term:. 
+00020c80: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00020c90: 5f73 656c 6563 746f 723a 0a20 2020 2020  _selector:.     
+00020ca0: 2020 2020 2020 202d 2061 7070 3a64 656d         - app:dem
+00020cb0: 6f2d 6170 700a 2020 2020 2020 2020 2020  o-app.          
+00020cc0: 2020 2d20 226b 6579 3a76 6572 7369 6f6e    - "key:version
+00020cd0: 2c20 6f70 6572 6174 6f72 3a49 6e2c 2076  , operator:In, v
+00020ce0: 616c 7565 733a 5b76 312e 302e 302c 2076  alues:[v1.0.0, v
+00020cf0: 312e 302e 315d 220a 2020 2020 2020 2020  1.0.1]".        
+00020d00: 2020 2020 746f 706f 6c6f 6779 5f6b 6579      topology_key
+00020d10: 3a20 746f 706f 6c6f 6779 5f6b 6579 0a20  : topology_key. 
+00020d20: 2020 2020 2020 2020 2020 206e 616d 6573             names
+00020d30: 7061 6365 733a 0a20 2020 2020 2020 2020  paces:.         
+00020d40: 2020 202d 206e 616d 6573 7061 6365 730a     - namespaces.
+00020d50: 2020 2020 2020 2020 2020 2020 2d20 6e61              - na
+00020d60: 6d65 7370 6163 6573 0a20 2020 2020 2020  mespaces.       
+00020d70: 202d 2077 6569 6768 743a 2036 0a20 2020   - weight: 6.   
+00020d80: 2020 2020 2020 2070 6f64 5f61 6666 696e         pod_affin
+00020d90: 6974 795f 7465 726d 3a0a 2020 2020 2020  ity_term:.      
+00020da0: 2020 2020 2020 6c61 6265 6c5f 7365 6c65        label_sele
+00020db0: 6374 6f72 3a0a 2020 2020 2020 2020 2020  ctor:.          
+00020dc0: 2020 2d20 6170 703a 6465 6d6f 2d61 7070    - app:demo-app
+00020dd0: 0a20 2020 2020 2020 2020 2020 202d 2022  .            - "
+00020de0: 6b65 793a 7665 7273 696f 6e2c 206f 7065  key:version, ope
+00020df0: 7261 746f 723a 496e 2c20 7661 6c75 6573  rator:In, values
+00020e00: 3a5b 7631 2e30 2e30 2c20 7631 2e30 2e31  :[v1.0.0, v1.0.1
+00020e10: 5d22 0a20 2020 2020 2020 2020 2020 2074  ]".            t
+00020e20: 6f70 6f6c 6f67 795f 6b65 793a 2074 6f70  opology_key: top
+00020e30: 6f6c 6f67 795f 6b65 790a 2020 2020 2020  ology_key.      
+00020e40: 2020 2020 2020 6e61 6d65 7370 6163 6573        namespaces
+00020e50: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
+00020e60: 6e61 6d65 7370 6163 6573 0a20 2020 2020  namespaces.     
+00020e70: 2020 2020 2020 202d 206e 616d 6573 7061         - namespa
+00020e80: 6365 730a 2020 2020 2020 2020 7265 7175  ces.        requ
+00020e90: 6972 6564 5f64 7572 696e 675f 7363 6865  ired_during_sche
+00020ea0: 6475 6c69 6e67 5f69 676e 6f72 6564 5f64  duling_ignored_d
+00020eb0: 7572 696e 675f 6578 6563 7574 696f 6e3a  uring_execution:
+00020ec0: 0a20 2020 2020 2020 202d 206c 6162 656c  .        - label
+00020ed0: 5f73 656c 6563 746f 723a 0a20 2020 2020  _selector:.     
+00020ee0: 2020 2020 202d 2061 7070 3a64 656d 6f2d       - app:demo-
+00020ef0: 6170 700a 2020 2020 2020 2020 2020 2d20  app.          - 
+00020f00: 226b 6579 3a76 6572 7369 6f6e 2c20 6f70  "key:version, op
+00020f10: 6572 6174 6f72 3a49 6e2c 2076 616c 7565  erator:In, value
+00020f20: 733a 5b76 312e 302e 302c 2076 312e 302e  s:[v1.0.0, v1.0.
+00020f30: 315d 220a 2020 2020 2020 2020 2020 746f  1]".          to
+00020f40: 706f 6c6f 6779 5f6b 6579 3a20 746f 706f  pology_key: topo
+00020f50: 6c6f 6779 5f6b 6579 0a20 2020 2020 2020  logy_key.       
+00020f60: 2020 206e 616d 6573 7061 6365 733a 0a20     namespaces:. 
+00020f70: 2020 2020 2020 2020 202d 206e 616d 6573           - names
+00020f80: 7061 6365 730a 2020 2020 2020 2020 2020  paces.          
+00020f90: 2d20 6e61 6d65 7370 6163 6573 0a20 2020  - namespaces.   
+00020fa0: 2020 2020 202d 206c 6162 656c 5f73 656c       - label_sel
+00020fb0: 6563 746f 723a 0a20 2020 2020 2020 2020  ector:.         
+00020fc0: 202d 2061 7070 3a64 656d 6f2d 6170 700a   - app:demo-app.
+00020fd0: 2020 2020 2020 2020 2020 2d20 226b 6579            - "key
+00020fe0: 3a76 6572 7369 6f6e 2c20 6f70 6572 6174  :version, operat
+00020ff0: 6f72 3a49 6e2c 2076 616c 7565 733a 5b76  or:In, values:[v
+00021000: 312e 302e 302c 2076 312e 302e 315d 220a  1.0.0, v1.0.1]".
+00021010: 2020 2020 2020 2020 2020 746f 706f 6c6f            topolo
+00021020: 6779 5f6b 6579 3a20 746f 706f 6c6f 6779  gy_key: topology
+00021030: 5f6b 6579 0a20 2020 2020 2020 2020 206e  _key.          n
+00021040: 616d 6573 7061 6365 733a 0a20 2020 2020  amespaces:.     
+00021050: 2020 2020 202d 206e 616d 6573 7061 6365       - namespace
+00021060: 730a 2020 2020 2020 2020 2020 2d20 6e61  s.          - na
+00021070: 6d65 7370 6163 6573 0a20 2020 2020 2070  mespaces.      p
+00021080: 726f 7065 7274 6965 733a 0a20 2020 2020  roperties:.     
+00021090: 2020 2072 6571 7569 7265 645f 6475 7269     required_duri
+000210a0: 6e67 5f73 6368 6564 756c 696e 675f 6967  ng_scheduling_ig
+000210b0: 6e6f 7265 645f 6475 7269 6e67 5f65 7865  nored_during_exe
+000210c0: 6375 7469 6f6e 3a0a 2020 2020 2020 2020  cution:.        
+000210d0: 2020 6974 656d 733a 0a20 2020 2020 2020    items:.       
+000210e0: 2020 2020 2024 7265 663a 2027 232f 636f       $ref: '#/co
+000210f0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00021100: 2f50 6f64 4166 6669 6e69 7479 5465 726d  /PodAffinityTerm
+00021110: 270a 2020 2020 2020 2020 2020 7469 746c  '.          titl
+00021120: 653a 2072 6571 7569 7265 645f 6475 7269  e: required_duri
+00021130: 6e67 5f73 6368 6564 756c 696e 675f 6967  ng_scheduling_ig
+00021140: 6e6f 7265 645f 6475 7269 6e67 5f65 7865  nored_during_exe
+00021150: 6375 7469 6f6e 0a20 2020 2020 2020 2020  cution.         
+00021160: 2074 7970 653a 2061 7272 6179 0a20 2020   type: array.   
+00021170: 2020 2020 2070 7265 6665 7272 6564 5f64       preferred_d
+00021180: 7572 696e 675f 7363 6865 6475 6c69 6e67  uring_scheduling
+00021190: 5f69 676e 6f72 6564 5f64 7572 696e 675f  _ignored_during_
+000211a0: 6578 6563 7574 696f 6e3a 0a20 2020 2020  execution:.     
+000211b0: 2020 2020 2069 7465 6d73 3a0a 2020 2020       items:.    
+000211c0: 2020 2020 2020 2020 2472 6566 3a20 2723          $ref: '#
+000211d0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+000211e0: 6d61 732f 5765 6967 6874 6564 506f 6441  mas/WeightedPodA
+000211f0: 6666 696e 6974 7954 6572 6d27 0a20 2020  ffinityTerm'.   
+00021200: 2020 2020 2020 2074 6974 6c65 3a20 7072         title: pr
+00021210: 6566 6572 7265 645f 6475 7269 6e67 5f73  eferred_during_s
+00021220: 6368 6564 756c 696e 675f 6967 6e6f 7265  cheduling_ignore
+00021230: 645f 6475 7269 6e67 5f65 7865 6375 7469  d_during_executi
+00021240: 6f6e 0a20 2020 2020 2020 2020 2074 7970  on.          typ
+00021250: 653a 2061 7272 6179 0a20 2020 2020 2074  e: array.      t
+00021260: 6974 6c65 3a20 506f 6441 6e74 6941 6666  itle: PodAntiAff
+00021270: 696e 6974 790a 2020 2020 2020 7479 7065  inity.      type
+00021280: 3a20 6f62 6a65 6374 0a20 2020 2050 6572  : object.    Per
+00021290: 7369 7374 656e 7456 6f6c 756d 6543 6c61  sistentVolumeCla
+000212a0: 696d 3a0a 2020 2020 2020 6578 616d 706c  im:.      exampl
+000212b0: 653a 0a20 2020 2020 2020 2076 6f6c 756d  e:.        volum
+000212c0: 655f 6d6f 6465 3a20 4669 6c65 7379 7374  e_mode: Filesyst
+000212d0: 656d 0a20 2020 2020 2020 2072 6571 7565  em.        reque
+000212e0: 7374 5f72 6573 6f75 7263 6573 3a0a 2020  st_resources:.  
+000212f0: 2020 2020 2020 2020 7265 7175 6573 7473          requests
+00021300: 3a0a 2020 2020 2020 2020 2020 2020 6d65  :.            me
+00021310: 6d6f 7279 3a20 3235 364d 690a 2020 2020  mory: 256Mi.    
+00021320: 2020 2020 2020 2020 6370 753a 2022 302e          cpu: "0.
+00021330: 3122 0a20 2020 2020 2020 2020 206c 696d  1".          lim
+00021340: 6974 733a 0a20 2020 2020 2020 2020 2020  its:.           
+00021350: 206d 656d 6f72 793a 2035 3132 4d69 0a20   memory: 512Mi. 
+00021360: 2020 2020 2020 2020 2020 2063 7075 3a20             cpu: 
+00021370: 2230 2e35 220a 2020 2020 2020 2020 6e61  "0.5".        na
+00021380: 6d65 3a20 6d79 2d70 7663 0a20 2020 2020  me: my-pvc.     
+00021390: 2020 206e 616d 6573 7061 6365 3a20 6769     namespace: gi
+000213a0: 746f 7073 2d63 646e 2d63 6163 6865 0a20  tops-cdn-cache. 
+000213b0: 2020 2020 2020 2061 6e6e 6f74 6174 696f         annotatio
+000213c0: 6e73 3a0a 2020 2020 2020 2020 2d20 616e  ns:.        - an
+000213d0: 6e6f 7461 7469 6f6e 2d6b 6579 313a 7661  notation-key1:va
+000213e0: 6c31 0a20 2020 2020 2020 202d 2061 6e6e  l1.        - ann
+000213f0: 6f74 6174 696f 6e2d 6b65 7932 3a76 616c  otation-key2:val
+00021400: 320a 2020 2020 2020 2020 766f 6c75 6d65  2.        volume
+00021410: 5f6e 616d 653a 206d 792d 7076 0a20 2020  _name: my-pv.   
+00021420: 2020 2020 2073 746f 7261 6765 5f63 6c61       storage_cla
+00021430: 7373 5f6e 616d 653a 2073 7461 6e64 6172  ss_name: standar
+00021440: 640a 2020 2020 2020 2020 6163 6365 7373  d.        access
+00021450: 5f6d 6f64 6573 3a0a 2020 2020 2020 2020  _modes:.        
+00021460: 2d20 5265 6164 5772 6974 654f 6e63 650a  - ReadWriteOnce.
+00021470: 2020 2020 2020 2020 6c61 6265 6c73 3a0a          labels:.
+00021480: 2020 2020 2020 2020 2d20 6170 703a 6465          - app:de
+00021490: 6d6f 2d61 7070 0a20 2020 2020 2020 202d  mo-app.        -
+000214a0: 2076 6572 7369 6f6e 3a76 312e 302e 300a   version:v1.0.0.
+000214b0: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
+000214c0: 3a0a 2020 2020 2020 2020 6e61 6d65 3a0a  :.        name:.
+000214d0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+000214e0: 7074 696f 6e3a 2022 6e61 6d65 206f 6620  ption: "name of 
+000214f0: 7065 7273 6973 7465 6e74 2076 6f6c 756d  persistent volum
+00021500: 6520 636c 6169 6d2c 2075 7365 6420 696e  e claim, used in
+00021510: 206d 6574 6164 6174 612e 6e61 6d65 220a   metadata.name".
+00021520: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
+00021530: 653a 206d 792d 7076 630a 2020 2020 2020  e: my-pvc.      
+00021540: 2020 2020 7469 746c 653a 206e 616d 650a      title: name.
+00021550: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
+00021560: 7374 7269 6e67 0a20 2020 2020 2020 206e  string.        n
+00021570: 616d 6573 7061 6365 3a0a 2020 2020 2020  amespace:.      
+00021580: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00021590: 206e 616d 6573 7061 6365 2066 6f72 2072   namespace for r
+000215a0: 6573 6f75 7263 652e 0a20 2020 2020 2020  esource..       
+000215b0: 2020 2065 7861 6d70 6c65 3a20 6769 746f     example: gito
+000215c0: 7073 2d63 646e 2d63 6163 6865 0a20 2020  ps-cdn-cache.   
+000215d0: 2020 2020 2020 2074 6974 6c65 3a20 6e61         title: na
+000215e0: 6d65 7370 6163 650a 2020 2020 2020 2020  mespace.        
+000215f0: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+00021600: 2020 2020 2020 206c 6162 656c 733a 0a20         labels:. 
+00021610: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00021620: 7469 6f6e 3a20 4d61 7020 6f66 2073 7472  tion: Map of str
+00021630: 696e 6720 6b65 7973 2061 6e64 2076 616c  ing keys and val
+00021640: 7565 7320 7468 6174 2063 616e 2062 6520  ues that can be 
+00021650: 7573 6564 2074 6f20 6f72 6761 6e69 7a65  used to organize
+00021660: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+00021670: 2063 6174 6567 6f72 697a 6520 2873 636f   categorize (sco
+00021680: 7065 2061 6e64 2073 656c 6563 7429 206f  pe and select) o
+00021690: 626a 6563 7473 0a20 2020 2020 2020 2020  bjects.         
+000216a0: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
+000216b0: 2020 2020 2d20 6170 703a 6465 6d6f 2d61      - app:demo-a
+000216c0: 7070 0a20 2020 2020 2020 2020 202d 2076  pp.          - v
+000216d0: 6572 7369 6f6e 3a76 312e 302e 300a 2020  ersion:v1.0.0.  
+000216e0: 2020 2020 2020 2020 6974 656d 733a 0a20          items:. 
+000216f0: 2020 2020 2020 2020 2020 2074 7970 653a             type:
+00021700: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00021710: 2020 7469 746c 653a 204c 6162 656c 730a    title: Labels.
+00021720: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
+00021730: 6172 7261 790a 2020 2020 2020 2020 616e  array.        an
+00021740: 6e6f 7461 7469 6f6e 733a 0a20 2020 2020  notations:.     
+00021750: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00021760: 3a20 416e 2075 6e73 7472 7563 7475 7265  : An unstructure
+00021770: 6420 6b65 7920 7661 6c75 6520 6d61 7020  d key value map 
+00021780: 7468 6174 2063 616e 2062 6520 7573 6564  that can be used
+00021790: 2074 6f20 6174 7461 6368 2061 7262 6974   to attach arbit
+000217a0: 7261 7279 0a20 2020 2020 2020 2020 2020  rary.           
+000217b0: 206d 6574 6164 6174 610a 2020 2020 2020   metadata.      
+000217c0: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
+000217d0: 2020 2020 2020 202d 2061 6e6e 6f74 6174         - annotat
+000217e0: 696f 6e2d 6b65 7931 3a76 616c 310a 2020  ion-key1:val1.  
+000217f0: 2020 2020 2020 2020 2d20 616e 6e6f 7461          - annota
+00021800: 7469 6f6e 2d6b 6579 323a 7661 6c32 0a20  tion-key2:val2. 
+00021810: 2020 2020 2020 2020 2069 7465 6d73 3a0a           items:.
+00021820: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00021830: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+00021840: 2020 2074 6974 6c65 3a20 416e 6e6f 7461     title: Annota
+00021850: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+00021860: 7479 7065 3a20 6172 7261 790a 2020 2020  type: array.    
+00021870: 2020 2020 7374 6f72 6167 655f 636c 6173      storage_clas
+00021880: 735f 6e61 6d65 3a0a 2020 2020 2020 2020  s_name:.        
+00021890: 2020 6465 7363 7269 7074 696f 6e3a 204e    description: N
+000218a0: 616d 6520 6f66 2074 6865 2053 746f 7261  ame of the Stora
+000218b0: 6765 436c 6173 7320 666f 7220 7468 6520  geClass for the 
+000218c0: 5065 7273 6973 7465 6e74 2056 6f6c 756d  Persistent Volum
+000218d0: 6520 436c 6169 6d0a 2020 2020 2020 2020  e Claim.        
+000218e0: 2020 6578 616d 706c 653a 2073 7461 6e64    example: stand
+000218f0: 6172 640a 2020 2020 2020 2020 2020 7469  ard.          ti
+00021900: 746c 653a 2073 746f 7261 6765 5f63 6c61  tle: storage_cla
+00021910: 7373 5f6e 616d 650a 2020 2020 2020 2020  ss_name.        
+00021920: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+00021930: 2020 2020 2020 2061 6363 6573 735f 6d6f         access_mo
+00021940: 6465 733a 0a20 2020 2020 2020 2020 2064  des:.          d
+00021950: 6573 6372 6970 7469 6f6e 3a20 224c 6973  escription: "Lis
+00021960: 7420 6f66 2061 6363 6573 7320 6d6f 6465  t of access mode
+00021970: 7320 666f 7220 7468 6520 5065 7273 6973  s for the Persis
+00021980: 7465 6e74 2056 6f6c 756d 652c 2065 2e67  tent Volume, e.g
+00021990: 2e20 5265 6164 5772 6974 654f 6e63 652c  . ReadWriteOnce,
+000219a0: 5c0a 2020 2020 2020 2020 2020 2020 5c20  \.            \ 
+000219b0: 5265 6164 4f6e 6c79 4d61 6e79 2c20 6574  ReadOnlyMany, et
+000219c0: 632e 220a 2020 2020 2020 2020 2020 6578  c.".          ex
+000219d0: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
+000219e0: 202d 2052 6561 6457 7269 7465 4f6e 6365   - ReadWriteOnce
+000219f0: 0a20 2020 2020 2020 2020 2069 7465 6d73  .          items
+00021a00: 3a0a 2020 2020 2020 2020 2020 2020 7479  :.            ty
+00021a10: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
+00021a20: 2020 2020 2074 6974 6c65 3a20 6163 6365       title: acce
+00021a30: 7373 5f6d 6f64 6573 0a20 2020 2020 2020  ss_modes.       
+00021a40: 2020 2074 7970 653a 2061 7272 6179 0a20     type: array. 
+00021a50: 2020 2020 2020 2076 6f6c 756d 655f 6e61         volume_na
+00021a60: 6d65 3a0a 2020 2020 2020 2020 2020 6465  me:.          de
+00021a70: 7363 7269 7074 696f 6e3a 204e 616d 6520  scription: Name 
+00021a80: 6f66 2074 6865 2050 6572 7369 7374 656e  of the Persisten
+00021a90: 7420 566f 6c75 6d65 2062 6f75 6e64 2074  t Volume bound t
+00021aa0: 6f20 7468 6520 636c 6169 6d0a 2020 2020  o the claim.    
+00021ab0: 2020 2020 2020 6578 616d 706c 653a 206d        example: m
+00021ac0: 792d 7076 0a20 2020 2020 2020 2020 2074  y-pv.          t
+00021ad0: 6974 6c65 3a20 766f 6c75 6d65 5f6e 616d  itle: volume_nam
+00021ae0: 650a 2020 2020 2020 2020 2020 7479 7065  e.          type
+00021af0: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+00021b00: 2076 6f6c 756d 655f 6d6f 6465 3a0a 2020   volume_mode:.  
+00021b10: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00021b20: 696f 6e3a 2022 4d6f 6465 206f 6620 7468  ion: "Mode of th
+00021b30: 6520 766f 6c75 6d65 2c20 6569 7468 6572  e volume, either
+00021b40: 205c 2246 696c 6573 7973 7465 6d5c 2220   \"Filesystem\" 
+00021b50: 6f72 205c 2242 6c6f 636b 5c22 220a 2020  or \"Block\"".  
+00021b60: 2020 2020 2020 2020 6578 616d 706c 653a          example:
+00021b70: 2046 696c 6573 7973 7465 6d0a 2020 2020   Filesystem.    
+00021b80: 2020 2020 2020 7469 746c 653a 2076 6f6c        title: vol
+00021b90: 756d 655f 6d6f 6465 0a20 2020 2020 2020  ume_mode.       
+00021ba0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
+00021bb0: 2020 2020 2020 2020 7265 7175 6573 745f          request_
+00021bc0: 7265 736f 7572 6365 733a 0a20 2020 2020  resources:.     
+00021bd0: 2020 2020 2024 7265 663a 2027 232f 636f       $ref: '#/co
+00021be0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00021bf0: 2f52 6573 6f75 7263 6552 6571 7569 7265  /ResourceRequire
+00021c00: 6d65 6e74 7327 0a20 2020 2020 2072 6571  ments'.      req
+00021c10: 7569 7265 643a 0a20 2020 2020 202d 206e  uired:.      - n
+00021c20: 616d 650a 2020 2020 2020 7469 746c 653a  ame.      title:
+00021c30: 2050 6572 7369 7374 656e 7456 6f6c 756d   PersistentVolum
+00021c40: 6543 6c61 696d 0a20 2020 2020 2074 7970  eClaim.      typ
+00021c50: 653a 206f 626a 6563 740a 2020 2020 5365  e: object.    Se
+00021c60: 7276 6963 653a 0a20 2020 2020 2065 7861  rvice:.      exa
+00021c70: 6d70 6c65 3a0a 2020 2020 2020 2020 6578  mple:.        ex
+00021c80: 7465 726e 616c 5f69 7073 3a0a 2020 2020  ternal_ips:.    
+00021c90: 2020 2020 2d20 312e 312e 312e 310a 2020      - 1.1.1.1.  
+00021ca0: 2020 2020 2020 2d20 322e 322e 322e 320a        - 2.2.2.2.
+00021cb0: 2020 2020 2020 2020 7365 7276 6963 655f          service_
+00021cc0: 7479 7065 3a20 436c 7573 7465 7249 500a  type: ClusterIP.
+00021cd0: 2020 2020 2020 2020 6e61 6d65 3a20 6465          name: de
+00021ce0: 6d6f 2d61 7070 0a20 2020 2020 2020 206e  mo-app.        n
+00021cf0: 616d 6573 7061 6365 3a20 6769 746f 7073  amespace: gitops
+00021d00: 2d63 646e 2d63 6163 6865 0a20 2020 2020  -cdn-cache.     
+00021d10: 2020 2061 6e6e 6f74 6174 696f 6e73 3a0a     annotations:.
+00021d20: 2020 2020 2020 2020 2d20 616e 6e6f 7461          - annota
+00021d30: 7469 6f6e 2d6b 6579 313a 7661 6c31 0a20  tion-key1:val1. 
+00021d40: 2020 2020 2020 202d 2061 6e6e 6f74 6174         - annotat
+00021d50: 696f 6e2d 6b65 7932 3a76 616c 320a 2020  ion-key2:val2.  
+00021d60: 2020 2020 2020 7365 6c65 6374 6f72 3a0a        selector:.
+00021d70: 2020 2020 2020 2020 2d20 6170 703a 6465          - app:de
+00021d80: 6d6f 2d61 7070 0a20 2020 2020 2020 202d  mo-app.        -
+00021d90: 2022 6b65 793a 7665 7273 696f 6e2c 206f   "key:version, o
+00021da0: 7065 7261 746f 723a 496e 2c20 7661 6c75  perator:In, valu
+00021db0: 6573 3a5b 7631 2e30 2e30 2c20 7631 2e30  es:[v1.0.0, v1.0
+00021dc0: 2e31 5d22 0a20 2020 2020 2020 2070 6f72  .1]".        por
+00021dd0: 7473 3a0a 2020 2020 2020 2020 2d20 7461  ts:.        - ta
+00021de0: 7267 6574 5f70 6f72 743a 2038 3038 300a  rget_port: 8080.
+00021df0: 2020 2020 2020 2020 2020 7072 6f74 6f63            protoc
+00021e00: 6f6c 3a20 5443 500a 2020 2020 2020 2020  ol: TCP.        
+00021e10: 2020 706f 7274 3a20 3830 0a20 2020 2020    port: 80.     
+00021e20: 2020 2020 206e 616d 653a 2068 7474 700a       name: http.
+00021e30: 2020 2020 2020 2020 2020 6e6f 6465 5f70            node_p
+00021e40: 6f72 743a 2036 3530 300a 2020 2020 2020  ort: 6500.      
+00021e50: 2020 2d20 7461 7267 6574 5f70 6f72 743a    - target_port:
+00021e60: 2038 3038 300a 2020 2020 2020 2020 2020   8080.          
+00021e70: 7072 6f74 6f63 6f6c 3a20 5443 500a 2020  protocol: TCP.  
+00021e80: 2020 2020 2020 2020 706f 7274 3a20 3830          port: 80
+00021e90: 0a20 2020 2020 2020 2020 206e 616d 653a  .          name:
+00021ea0: 2068 7474 700a 2020 2020 2020 2020 2020   http.          
+00021eb0: 6e6f 6465 5f70 6f72 743a 2036 3530 300a  node_port: 6500.
+00021ec0: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
+00021ed0: 6970 3a20 636c 7573 7465 725f 6970 0a20  ip: cluster_ip. 
+00021ee0: 2020 2020 2020 206c 6162 656c 733a 0a20         labels:. 
+00021ef0: 2020 2020 2020 202d 2061 7070 3a64 656d         - app:dem
+00021f00: 6f2d 6170 700a 2020 2020 2020 2020 2d20  o-app.        - 
+00021f10: 7665 7273 696f 6e3a 7631 2e30 2e30 0a20  version:v1.0.0. 
+00021f20: 2020 2020 2070 726f 7065 7274 6965 733a       properties:
+00021f30: 0a20 2020 2020 2020 206e 616d 653a 0a20  .        name:. 
+00021f40: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00021f50: 7469 6f6e 3a20 7365 7276 6963 6520 6e61  tion: service na
+00021f60: 6d65 0a20 2020 2020 2020 2020 2065 7861  me.          exa
+00021f70: 6d70 6c65 3a20 6465 6d6f 2d61 7070 0a20  mple: demo-app. 
+00021f80: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
+00021f90: 6e61 6d65 0a20 2020 2020 2020 2020 2074  name.          t
+00021fa0: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
+00021fb0: 2020 2020 6e61 6d65 7370 6163 653a 0a20      namespace:. 
+00021fc0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00021fd0: 7469 6f6e 3a20 6e61 6d65 7370 6163 6520  tion: namespace 
+00021fe0: 666f 7220 7265 736f 7572 6365 2e0a 2020  for resource..  
+00021ff0: 2020 2020 2020 2020 6578 616d 706c 653a          example:
+00022000: 2067 6974 6f70 732d 6364 6e2d 6361 6368   gitops-cdn-cach
+00022010: 650a 2020 2020 2020 2020 2020 7469 746c  e.          titl
+00022020: 653a 206e 616d 6573 7061 6365 0a20 2020  e: namespace.   
+00022030: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+00022040: 696e 670a 2020 2020 2020 2020 616e 6e6f  ing.        anno
+00022050: 7461 7469 6f6e 733a 0a20 2020 2020 2020  tations:.       
+00022060: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+00022070: 416e 2075 6e73 7472 7563 7475 7265 6420  An unstructured 
+00022080: 6b65 7920 7661 6c75 6520 6d61 7020 7468  key value map th
+00022090: 6174 2063 616e 2062 6520 7573 6564 2074  at can be used t
+000220a0: 6f20 6174 7461 6368 2061 7262 6974 7261  o attach arbitra
+000220b0: 7279 0a20 2020 2020 2020 2020 2020 206d  ry.            m
+000220c0: 6574 6164 6174 610a 2020 2020 2020 2020  etadata.        
+000220d0: 2020 6578 616d 706c 653a 0a20 2020 2020    example:.     
+000220e0: 2020 2020 202d 2061 6e6e 6f74 6174 696f       - annotatio
+000220f0: 6e2d 6b65 7931 3a76 616c 310a 2020 2020  n-key1:val1.    
+00022100: 2020 2020 2020 2d20 616e 6e6f 7461 7469        - annotati
+00022110: 6f6e 2d6b 6579 323a 7661 6c32 0a20 2020  on-key2:val2.   
+00022120: 2020 2020 2020 2069 7465 6d73 3a0a 2020         items:.  
+00022130: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
+00022140: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
+00022150: 2074 6974 6c65 3a20 416e 6e6f 7461 7469   title: Annotati
+00022160: 6f6e 730a 2020 2020 2020 2020 2020 7479  ons.          ty
+00022170: 7065 3a20 6172 7261 790a 2020 2020 2020  pe: array.      
+00022180: 2020 6c61 6265 6c73 3a0a 2020 2020 2020    labels:.      
+00022190: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+000221a0: 204d 6170 206f 6620 7374 7269 6e67 206b   Map of string k
+000221b0: 6579 7320 616e 6420 7661 6c75 6573 2074  eys and values t
+000221c0: 6861 7420 6361 6e20 6265 2075 7365 6420  hat can be used 
+000221d0: 746f 206f 7267 616e 697a 650a 2020 2020  to organize.    
+000221e0: 2020 2020 2020 2020 616e 6420 6361 7465          and cate
+000221f0: 676f 7269 7a65 2028 7363 6f70 6520 616e  gorize (scope an
+00022200: 6420 7365 6c65 6374 2920 6f62 6a65 6374  d select) object
+00022210: 730a 2020 2020 2020 2020 2020 6578 616d  s.          exam
+00022220: 706c 653a 0a20 2020 2020 2020 2020 202d  ple:.          -
+00022230: 2061 7070 3a64 656d 6f2d 6170 700a 2020   app:demo-app.  
+00022240: 2020 2020 2020 2020 2d20 7665 7273 696f          - versio
+00022250: 6e3a 7631 2e30 2e30 0a20 2020 2020 2020  n:v1.0.0.       
+00022260: 2020 2069 7465 6d73 3a0a 2020 2020 2020     items:.      
+00022270: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+00022280: 6e67 0a20 2020 2020 2020 2020 2074 6974  ng.          tit
+00022290: 6c65 3a20 4c61 6265 6c73 0a20 2020 2020  le: Labels.     
+000222a0: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
+000222b0: 0a20 2020 2020 2020 2073 656c 6563 746f  .        selecto
+000222c0: 723a 0a20 2020 2020 2020 2020 2064 6573  r:.          des
+000222d0: 6372 6970 7469 6f6e 3a20 7c0a 2020 2020  cription: |.    
+000222e0: 2020 2020 2020 2020 416e 2061 7272 6179          An array
+000222f0: 206f 6620 6c61 6265 6c20 7365 6c65 6374   of label select
+00022300: 6f72 2072 756c 652c 2074 6865 2072 756c  or rule, the rul
+00022310: 6520 6361 6e20 6569 7468 6572 2062 6520  e can either be 
+00022320: 6120 6d61 7463 6820 6c61 6265 6c20 6f72  a match label or
+00022330: 206d 6174 6368 2065 7870 7265 7373 696f   match expressio
+00022340: 6e2c 0a20 2020 2020 2020 2020 2020 2072  n,.            r
+00022350: 6566 6572 7269 6e67 2074 6865 2065 7861  eferring the exa
+00022360: 6d70 6c65 2028 6669 7273 7420 6973 2061  mple (first is a
+00022370: 206d 6174 6368 206c 6162 656c 2c20 7365   match label, se
+00022380: 636f 6e64 2069 7320 6120 6d61 7463 6820  cond is a match 
+00022390: 6578 7072 6573 7369 6f6e 290a 2020 2020  expression).    
+000223a0: 2020 2020 2020 6578 616d 706c 653a 0a20        example:. 
+000223b0: 2020 2020 2020 2020 202d 2061 7070 3a64           - app:d
+000223c0: 656d 6f2d 6170 700a 2020 2020 2020 2020  emo-app.        
+000223d0: 2020 2d20 226b 6579 3a76 6572 7369 6f6e    - "key:version
+000223e0: 2c20 6f70 6572 6174 6f72 3a49 6e2c 2076  , operator:In, v
+000223f0: 616c 7565 733a 5b76 312e 302e 302c 2076  alues:[v1.0.0, v
+00022400: 312e 302e 315d 220a 2020 2020 2020 2020  1.0.1]".        
+00022410: 2020 6974 656d 733a 0a20 2020 2020 2020    items:.       
+00022420: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+00022430: 670a 2020 2020 2020 2020 2020 7469 746c  g.          titl
+00022440: 653a 204c 6162 656c 5365 6c65 6374 6f72  e: LabelSelector
+00022450: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
+00022460: 2061 7272 6179 0a20 2020 2020 2020 2073   array.        s
+00022470: 6572 7669 6365 5f74 7970 653a 0a20 2020  ervice_type:.   
+00022480: 2020 2020 2020 2065 6e75 6d3a 0a20 2020         enum:.   
+00022490: 2020 2020 2020 202d 2043 6c75 7374 6572         - Cluster
+000224a0: 4950 0a20 2020 2020 2020 2020 202d 204e  IP.          - N
+000224b0: 6f64 6550 6f72 740a 2020 2020 2020 2020  odePort.        
+000224c0: 2020 2d20 4c6f 6164 4261 6c61 6e63 6572    - LoadBalancer
+000224d0: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
+000224e0: 6c65 3a20 436c 7573 7465 7249 500a 2020  le: ClusterIP.  
+000224f0: 2020 2020 2020 2020 7469 746c 653a 2073          title: s
+00022500: 6572 7669 6365 5f74 7970 650a 2020 2020  ervice_type.    
+00022510: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+00022520: 6e67 0a20 2020 2020 2020 2070 6f72 7473  ng.        ports
+00022530: 3a0a 2020 2020 2020 2020 2020 6974 656d  :.          item
+00022540: 733a 0a20 2020 2020 2020 2020 2020 2024  s:.            $
+00022550: 7265 663a 2027 232f 636f 6d70 6f6e 656e  ref: '#/componen
+00022560: 7473 2f73 6368 656d 6173 2f53 6572 7669  ts/schemas/Servi
+00022570: 6365 506f 7274 270a 2020 2020 2020 2020  cePort'.        
+00022580: 2020 7469 746c 653a 2070 6f72 7473 0a20    title: ports. 
+00022590: 2020 2020 2020 2020 2074 7970 653a 2061           type: a
+000225a0: 7272 6179 0a20 2020 2020 2020 2063 6c75  rray.        clu
+000225b0: 7374 6572 5f69 703a 0a20 2020 2020 2020  ster_ip:.       
+000225c0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+000225d0: 4578 706f 7365 7320 7468 6520 5365 7276  Exposes the Serv
+000225e0: 6963 6520 6f6e 2061 2063 6c75 7374 6572  ice on a cluster
+000225f0: 2d69 6e74 6572 6e61 6c20 4950 2e0a 2020  -internal IP..  
+00022600: 2020 2020 2020 2020 7469 746c 653a 2063          title: c
+00022610: 6c75 7374 6572 5f69 700a 2020 2020 2020  luster_ip.      
+00022620: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+00022630: 0a20 2020 2020 2020 2065 7874 6572 6e61  .        externa
+00022640: 6c5f 6970 733a 0a20 2020 2020 2020 2020  l_ips:.         
+00022650: 2064 6573 6372 6970 7469 6f6e 3a20 4120   description: A 
+00022660: 6c69 7374 206f 6620 4950 2061 6464 7265  list of IP addre
+00022670: 7373 6573 2066 6f72 2077 6869 6368 206e  sses for which n
+00022680: 6f64 6573 2069 6e20 7468 6520 636c 7573  odes in the clus
+00022690: 7465 7220 7769 6c6c 0a20 2020 2020 2020  ter will.       
+000226a0: 2020 2020 2061 6c73 6f20 6163 6365 7074       also accept
+000226b0: 2074 7261 6666 6963 2066 6f72 2074 6869   traffic for thi
+000226c0: 7320 7365 7276 6963 650a 2020 2020 2020  s service.      
+000226d0: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
+000226e0: 2020 2020 2020 202d 2031 2e31 2e31 2e31         - 1.1.1.1
+000226f0: 0a20 2020 2020 2020 2020 202d 2032 2e32  .          - 2.2
+00022700: 2e32 2e32 0a20 2020 2020 2020 2020 2069  .2.2.          i
+00022710: 7465 6d73 3a0a 2020 2020 2020 2020 2020  tems:.          
+00022720: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+00022730: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
+00022740: 6578 7465 726e 616c 5f69 7073 0a20 2020  external_ips.   
+00022750: 2020 2020 2020 2074 7970 653a 2061 7272         type: arr
+00022760: 6179 0a20 2020 2020 2072 6571 7569 7265  ay.      require
+00022770: 643a 0a20 2020 2020 202d 206e 616d 650a  d:.      - name.
+00022780: 2020 2020 2020 7469 746c 653a 2053 6572        title: Ser
+00022790: 7669 6365 0a20 2020 2020 2074 7970 653a  vice.      type:
+000227a0: 206f 626a 6563 740a 2020 2020 5365 7276   object.    Serv
+000227b0: 6963 6550 6f72 743a 0a20 2020 2020 2065  icePort:.      e
+000227c0: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
+000227d0: 7461 7267 6574 5f70 6f72 743a 2038 3038  target_port: 808
+000227e0: 300a 2020 2020 2020 2020 7072 6f74 6f63  0.        protoc
+000227f0: 6f6c 3a20 5443 500a 2020 2020 2020 2020  ol: TCP.        
+00022800: 706f 7274 3a20 3830 0a20 2020 2020 2020  port: 80.       
+00022810: 206e 616d 653a 2068 7474 700a 2020 2020   name: http.    
+00022820: 2020 2020 6e6f 6465 5f70 6f72 743a 2036      node_port: 6
+00022830: 3530 300a 2020 2020 2020 7072 6f70 6572  500.      proper
+00022840: 7469 6573 3a0a 2020 2020 2020 2020 6e61  ties:.        na
+00022850: 6d65 3a0a 2020 2020 2020 2020 2020 6465  me:.          de
+00022860: 7363 7269 7074 696f 6e3a 207c 0a20 2020  scription: |.   
+00022870: 2020 2020 2020 2020 2054 6865 206e 616d           The nam
+00022880: 6520 6f66 2074 6869 7320 706f 7274 2077  e of this port w
+00022890: 6974 6869 6e20 7468 6520 7365 7276 6963  ithin the servic
+000228a0: 652e 2054 6869 7320 6d75 7374 2062 6520  e. This must be 
+000228b0: 6120 444e 535f 4c41 4245 4c2e 0a20 2020  a DNS_LABEL..   
+000228c0: 2020 2020 2020 2020 2041 6c6c 2070 6f72           All por
+000228d0: 7473 2077 6974 6869 6e20 6120 5365 7276  ts within a Serv
+000228e0: 6963 6553 7065 6320 6d75 7374 2068 6176  iceSpec must hav
+000228f0: 6520 756e 6971 7565 206e 616d 6573 0a20  e unique names. 
+00022900: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
+00022910: 3a20 6874 7470 0a20 2020 2020 2020 2020  : http.         
+00022920: 2074 6974 6c65 3a20 6e61 6d65 0a20 2020   title: name.   
+00022930: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+00022940: 696e 670a 2020 2020 2020 2020 706f 7274  ing.        port
+00022950: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
+00022960: 7269 7074 696f 6e3a 2054 6865 2070 6f72  ription: The por
+00022970: 7420 7468 6174 2077 696c 6c20 6265 2065  t that will be e
+00022980: 7870 6f73 6564 2062 7920 7468 6973 2073  xposed by this s
+00022990: 6572 7669 6365 0a20 2020 2020 2020 2020  ervice.         
+000229a0: 2065 7861 6d70 6c65 3a20 3830 0a20 2020   example: 80.   
+000229b0: 2020 2020 2020 2074 6974 6c65 3a20 706f         title: po
+000229c0: 7274 0a20 2020 2020 2020 2020 2074 7970  rt.          typ
+000229d0: 653a 2069 6e74 6567 6572 0a20 2020 2020  e: integer.     
+000229e0: 2020 2074 6172 6765 745f 706f 7274 3a0a     target_port:.
+000229f0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00022a00: 7074 696f 6e3a 2054 6865 2070 6f72 7420  ption: The port 
+00022a10: 746f 2061 6363 6573 7320 6f6e 2074 6865  to access on the
+00022a20: 2070 6f64 7320 7461 7267 6574 6564 2062   pods targeted b
+00022a30: 7920 7468 6520 7365 7276 6963 650a 2020  y the service.  
+00022a40: 2020 2020 2020 2020 6578 616d 706c 653a          example:
+00022a50: 2038 3038 300a 2020 2020 2020 2020 2020   8080.          
+00022a60: 7469 746c 653a 2074 6172 6765 745f 706f  title: target_po
+00022a70: 7274 0a20 2020 2020 2020 2020 2074 7970  rt.          typ
+00022a80: 653a 2069 6e74 6567 6572 0a20 2020 2020  e: integer.     
+00022a90: 2020 206e 6f64 655f 706f 7274 3a0a 2020     node_port:.  
+00022aa0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00022ab0: 696f 6e3a 2054 6865 2070 6f72 7420 6f6e  ion: The port on
+00022ac0: 2065 6163 6820 6e6f 6465 206f 6e20 7768   each node on wh
+00022ad0: 6963 6820 7468 6973 2073 6572 7669 6365  ich this service
+00022ae0: 2069 7320 6578 706f 7365 6420 7768 656e   is exposed when
+00022af0: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
+00022b00: 6520 6973 204e 6f64 6550 6f72 7420 6f72  e is NodePort or
+00022b10: 204c 6f61 6442 616c 616e 6365 720a 2020   LoadBalancer.  
+00022b20: 2020 2020 2020 2020 6578 616d 706c 653a          example:
+00022b30: 2036 3530 300a 2020 2020 2020 2020 2020   6500.          
+00022b40: 7469 746c 653a 206e 6f64 655f 706f 7274  title: node_port
+00022b50: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
+00022b60: 2069 6e74 6567 6572 0a20 2020 2020 2020   integer.       
+00022b70: 2070 726f 746f 636f 6c3a 0a20 2020 2020   protocol:.     
+00022b80: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00022b90: 3a20 4465 6661 756c 7473 2074 6f20 5443  : Defaults to TC
+00022ba0: 500a 2020 2020 2020 2020 2020 656e 756d  P.          enum
+00022bb0: 3a0a 2020 2020 2020 2020 2020 2d20 5443  :.          - TC
+00022bc0: 500a 2020 2020 2020 2020 2020 2d20 5544  P.          - UD
+00022bd0: 500a 2020 2020 2020 2020 2020 6578 616d  P.          exam
+00022be0: 706c 653a 2054 4350 0a20 2020 2020 2020  ple: TCP.       
+00022bf0: 2020 2074 6974 6c65 3a20 7072 6f74 6f63     title: protoc
+00022c00: 6f6c 0a20 2020 2020 2020 2020 2074 7970  ol.          typ
+00022c10: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
+00022c20: 7265 7175 6972 6564 3a0a 2020 2020 2020  required:.      
+00022c30: 2d20 6e61 6d65 0a20 2020 2020 2074 6974  - name.      tit
+00022c40: 6c65 3a20 5365 7276 6963 6550 6f72 740a  le: ServicePort.
+00022c50: 2020 2020 2020 7479 7065 3a20 6f62 6a65        type: obje
+00022c60: 6374 0a20 2020 2043 6f6e 6669 673a 0a20  ct.    Config:. 
+00022c70: 2020 2020 2065 7861 6d70 6c65 3a0a 2020       example:.  
+00022c80: 2020 2020 2020 7465 6d70 6c61 7465 733a        templates:
+00022c90: 0a20 2020 2020 2020 202d 2076 616c 7565  .        - value
+00022ca0: 733a 0a20 2020 2020 2020 2020 2020 206b  s:.            k
+00022cb0: 6579 313a 2076 616c 7565 310a 2020 2020  ey1: value1.    
+00022cc0: 2020 2020 2020 6e61 6d65 3a20 636f 6e66        name: conf
+00022cd0: 2f73 6572 7665 722e 636f 6e66 0a20 2020  /server.conf.   
+00022ce0: 2020 2020 202d 2076 616c 7565 733a 0a20       - values:. 
+00022cf0: 2020 2020 2020 2020 2020 206b 6579 313a             key1:
+00022d00: 2076 616c 7565 310a 2020 2020 2020 2020   value1.        
+00022d10: 2020 6e61 6d65 3a20 636f 6e66 2f73 6572    name: conf/ser
+00022d20: 7665 722e 636f 6e66 0a20 2020 2020 2020  ver.conf.       
+00022d30: 206e 616d 653a 2073 6572 7665 722d 636f   name: server-co
+00022d40: 6e66 0a20 2020 2020 2020 2061 6e6e 6f74  nf.        annot
+00022d50: 6174 696f 6e73 3a0a 2020 2020 2020 2020  ations:.        
+00022d60: 2d20 616e 6e6f 7461 7469 6f6e 2d6b 6579  - annotation-key
+00022d70: 313a 7661 6c31 0a20 2020 2020 2020 202d  1:val1.        -
+00022d80: 2061 6e6e 6f74 6174 696f 6e2d 6b65 7932   annotation-key2
+00022d90: 3a76 616c 320a 2020 2020 2020 2020 6669  :val2.        fi
+00022da0: 6c65 733a 0a20 2020 2020 2020 202d 2063  les:.        - c
+00022db0: 6f6e 662f 7365 7276 6572 2e63 6f6e 660a  onf/server.conf.
+00022dc0: 2020 2020 2020 2020 6c61 6265 6c73 3a0a          labels:.
+00022dd0: 2020 2020 2020 2020 2d20 6170 703a 6465          - app:de
+00022de0: 6d6f 2d61 7070 0a20 2020 2020 2020 202d  mo-app.        -
+00022df0: 2076 6572 7369 6f6e 3a76 312e 302e 300a   version:v1.0.0.
+00022e00: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
+00022e10: 3a0a 2020 2020 2020 2020 6e61 6d65 3a0a  :.        name:.
+00022e20: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00022e30: 7074 696f 6e3a 2054 6865 2063 6f6e 6669  ption: The confi
+00022e40: 6720 6d61 7020 6e61 6d65 0a20 2020 2020  g map name.     
+00022e50: 2020 2020 2065 7861 6d70 6c65 3a20 7365       example: se
+00022e60: 7276 6572 2d63 6f6e 660a 2020 2020 2020  rver-conf.      
+00022e70: 2020 2020 7469 746c 653a 206e 616d 650a      title: name.
+00022e80: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
+00022e90: 7374 7269 6e67 0a20 2020 2020 2020 206c  string.        l
+00022ea0: 6162 656c 733a 0a20 2020 2020 2020 2020  abels:.         
+00022eb0: 2064 6573 6372 6970 7469 6f6e 3a20 4d61   description: Ma
+00022ec0: 7020 6f66 2073 7472 696e 6720 6b65 7973  p of string keys
+00022ed0: 2061 6e64 2076 616c 7565 7320 7468 6174   and values that
+00022ee0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+00022ef0: 6f72 6761 6e69 7a65 0a20 2020 2020 2020  organize.       
+00022f00: 2020 2020 2061 6e64 2063 6174 6567 6f72       and categor
+00022f10: 697a 6520 2873 636f 7065 2061 6e64 2073  ize (scope and s
+00022f20: 656c 6563 7429 206f 626a 6563 7473 0a20  elect) objects. 
+00022f30: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
+00022f40: 3a0a 2020 2020 2020 2020 2020 2d20 6170  :.          - ap
+00022f50: 703a 6465 6d6f 2d61 7070 0a20 2020 2020  p:demo-app.     
+00022f60: 2020 2020 202d 2076 6572 7369 6f6e 3a76       - version:v
+00022f70: 312e 302e 300a 2020 2020 2020 2020 2020  1.0.0.          
+00022f80: 6974 656d 733a 0a20 2020 2020 2020 2020  items:.         
+00022f90: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
+00022fa0: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+00022fb0: 204c 6162 656c 730a 2020 2020 2020 2020   Labels.        
+00022fc0: 2020 7479 7065 3a20 6172 7261 790a 2020    type: array.  
+00022fd0: 2020 2020 2020 616e 6e6f 7461 7469 6f6e        annotation
+00022fe0: 733a 0a20 2020 2020 2020 2020 2064 6573  s:.          des
+00022ff0: 6372 6970 7469 6f6e 3a20 416e 2075 6e73  cription: An uns
+00023000: 7472 7563 7475 7265 6420 6b65 7920 7661  tructured key va
+00023010: 6c75 6520 6d61 7020 7468 6174 2063 616e  lue map that can
+00023020: 2062 6520 7573 6564 2074 6f20 6174 7461   be used to atta
+00023030: 6368 2061 7262 6974 7261 7279 0a20 2020  ch arbitrary.   
+00023040: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+00023050: 610a 2020 2020 2020 2020 2020 6578 616d  a.          exam
+00023060: 706c 653a 0a20 2020 2020 2020 2020 202d  ple:.          -
+00023070: 2061 6e6e 6f74 6174 696f 6e2d 6b65 7931   annotation-key1
+00023080: 3a76 616c 310a 2020 2020 2020 2020 2020  :val1.          
+00023090: 2d20 616e 6e6f 7461 7469 6f6e 2d6b 6579  - annotation-key
+000230a0: 323a 7661 6c32 0a20 2020 2020 2020 2020  2:val2.         
+000230b0: 2069 7465 6d73 3a0a 2020 2020 2020 2020   items:.        
+000230c0: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+000230d0: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
+000230e0: 3a20 416e 6e6f 7461 7469 6f6e 730a 2020  : Annotations.  
+000230f0: 2020 2020 2020 2020 7479 7065 3a20 6172          type: ar
+00023100: 7261 790a 2020 2020 2020 2020 6669 6c65  ray.        file
+00023110: 733a 0a20 2020 2020 2020 2020 2064 6573  s:.          des
+00023120: 6372 6970 7469 6f6e 3a20 7468 6520 6c69  cription: the li
+00023130: 7374 206f 6620 636f 6e66 6967 2066 696c  st of config fil
+00023140: 6520 7061 7468 730a 2020 2020 2020 2020  e paths.        
+00023150: 2020 6578 616d 706c 653a 0a20 2020 2020    example:.     
+00023160: 2020 2020 202d 2063 6f6e 662f 7365 7276       - conf/serv
+00023170: 6572 2e63 6f6e 660a 2020 2020 2020 2020  er.conf.        
+00023180: 2020 6974 656d 733a 0a20 2020 2020 2020    items:.       
+00023190: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+000231a0: 670a 2020 2020 2020 2020 2020 7469 746c  g.          titl
+000231b0: 653a 2066 696c 6573 0a20 2020 2020 2020  e: files.       
+000231c0: 2020 2074 7970 653a 2061 7272 6179 0a20     type: array. 
+000231d0: 2020 2020 2020 2074 656d 706c 6174 6573         templates
+000231e0: 3a0a 2020 2020 2020 2020 2020 6974 656d  :.          item
+000231f0: 733a 0a20 2020 2020 2020 2020 2020 2024  s:.            $
+00023200: 7265 663a 2027 232f 636f 6d70 6f6e 656e  ref: '#/componen
+00023210: 7473 2f73 6368 656d 6173 2f43 6f6e 6669  ts/schemas/Confi
+00023220: 675f 7465 6d70 6c61 7465 735f 696e 6e65  g_templates_inne
+00023230: 7227 0a20 2020 2020 2020 2020 2074 6974  r'.          tit
+00023240: 6c65 3a20 7465 6d70 6c61 7465 730a 2020  le: templates.  
+00023250: 2020 2020 2020 2020 7479 7065 3a20 6172          type: ar
+00023260: 7261 790a 2020 2020 2020 7469 746c 653a  ray.      title:
+00023270: 2043 6f6e 6669 670a 2020 2020 2020 7479   Config.      ty
+00023280: 7065 3a20 6f62 6a65 6374 0a20 2020 2049  pe: object.    I
+00023290: 6e67 7265 7373 3a0a 2020 2020 2020 6578  ngress:.      ex
+000232a0: 616d 706c 653a 0a20 2020 2020 2020 206e  ample:.        n
+000232b0: 616d 653a 2064 656d 6f2d 6170 702d 696e  ame: demo-app-in
+000232c0: 6772 6573 730a 2020 2020 2020 2020 6e61  gress.        na
+000232d0: 6d65 7370 6163 653a 2067 6974 6f70 732d  mespace: gitops-
+000232e0: 6364 6e2d 6361 6368 650a 2020 2020 2020  cdn-cache.      
+000232f0: 2020 616e 6e6f 7461 7469 6f6e 733a 0a20    annotations:. 
+00023300: 2020 2020 2020 202d 2061 6e6e 6f74 6174         - annotat
+00023310: 696f 6e2d 6b65 7931 3a76 616c 310a 2020  ion-key1:val1.  
+00023320: 2020 2020 2020 2d20 616e 6e6f 7461 7469        - annotati
+00023330: 6f6e 2d6b 6579 323a 7661 6c32 0a20 2020  on-key2:val2.   
+00023340: 2020 2020 2072 756c 6573 3a0a 2020 2020       rules:.    
+00023350: 2020 2020 2d20 7061 7468 733a 0a20 2020      - paths:.   
+00023360: 2020 2020 2020 202d 2070 6174 683a 202f         - path: /
+00023370: 6261 720a 2020 2020 2020 2020 2020 2020  bar.            
+00023380: 6e61 6d65 3a20 696e 6772 6573 732d 7061  name: ingress-pa
+00023390: 7468 2d62 6172 0a20 2020 2020 2020 2020  th-bar.         
+000233a0: 2020 2070 6174 685f 7479 7065 3a20 4578     path_type: Ex
+000233b0: 6163 740a 2020 2020 2020 2020 2020 2020  act.            
+000233c0: 6261 636b 656e 643a 0a20 2020 2020 2020  backend:.       
+000233d0: 2020 2020 2020 2073 6572 7669 6365 3a0a         service:.
+000233e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000233f0: 706f 7274 3a20 3830 0a20 2020 2020 2020  port: 80.       
+00023400: 2020 2020 2020 2020 206e 616d 653a 2064           name: d
+00023410: 656d 6f2d 6170 702d 7365 7276 6963 650a  emo-app-service.
+00023420: 2020 2020 2020 2020 2020 2d20 7061 7468            - path
+00023430: 3a20 2f62 6172 0a20 2020 2020 2020 2020  : /bar.         
+00023440: 2020 206e 616d 653a 2069 6e67 7265 7373     name: ingress
+00023450: 2d70 6174 682d 6261 720a 2020 2020 2020  -path-bar.      
+00023460: 2020 2020 2020 7061 7468 5f74 7970 653a        path_type:
+00023470: 2045 7861 6374 0a20 2020 2020 2020 2020   Exact.         
+00023480: 2020 2062 6163 6b65 6e64 3a0a 2020 2020     backend:.    
+00023490: 2020 2020 2020 2020 2020 7365 7276 6963            servic
+000234a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000234b0: 2020 2070 6f72 743a 2038 300a 2020 2020     port: 80.    
+000234c0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000234d0: 3a20 6465 6d6f 2d61 7070 2d73 6572 7669  : demo-app-servi
+000234e0: 6365 0a20 2020 2020 2020 2020 206e 616d  ce.          nam
+000234f0: 653a 2066 6f6f 2d69 6e67 7265 7373 2d72  e: foo-ingress-r
+00023500: 756c 650a 2020 2020 2020 2020 2020 686f  ule.          ho
+00023510: 7374 3a20 7777 772e 666f 6f2e 636f 6d0a  st: www.foo.com.
+00023520: 2020 2020 2020 2020 2d20 7061 7468 733a          - paths:
+00023530: 0a20 2020 2020 2020 2020 202d 2070 6174  .          - pat
+00023540: 683a 202f 6261 720a 2020 2020 2020 2020  h: /bar.        
+00023550: 2020 2020 6e61 6d65 3a20 696e 6772 6573      name: ingres
+00023560: 732d 7061 7468 2d62 6172 0a20 2020 2020  s-path-bar.     
+00023570: 2020 2020 2020 2070 6174 685f 7479 7065         path_type
+00023580: 3a20 4578 6163 740a 2020 2020 2020 2020  : Exact.        
+00023590: 2020 2020 6261 636b 656e 643a 0a20 2020      backend:.   
+000235a0: 2020 2020 2020 2020 2020 2073 6572 7669             servi
+000235b0: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
+000235c0: 2020 2020 706f 7274 3a20 3830 0a20 2020      port: 80.   
+000235d0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+000235e0: 653a 2064 656d 6f2d 6170 702d 7365 7276  e: demo-app-serv
+000235f0: 6963 650a 2020 2020 2020 2020 2020 2d20  ice.          - 
+00023600: 7061 7468 3a20 2f62 6172 0a20 2020 2020  path: /bar.     
+00023610: 2020 2020 2020 206e 616d 653a 2069 6e67         name: ing
+00023620: 7265 7373 2d70 6174 682d 6261 720a 2020  ress-path-bar.  
+00023630: 2020 2020 2020 2020 2020 7061 7468 5f74            path_t
+00023640: 7970 653a 2045 7861 6374 0a20 2020 2020  ype: Exact.     
+00023650: 2020 2020 2020 2062 6163 6b65 6e64 3a0a         backend:.
+00023660: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00023670: 7276 6963 653a 0a20 2020 2020 2020 2020  rvice:.         
+00023680: 2020 2020 2020 2070 6f72 743a 2038 300a         port: 80.
+00023690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000236a0: 6e61 6d65 3a20 6465 6d6f 2d61 7070 2d73  name: demo-app-s
+000236b0: 6572 7669 6365 0a20 2020 2020 2020 2020  ervice.         
+000236c0: 206e 616d 653a 2066 6f6f 2d69 6e67 7265   name: foo-ingre
+000236d0: 7373 2d72 756c 650a 2020 2020 2020 2020  ss-rule.        
+000236e0: 2020 686f 7374 3a20 7777 772e 666f 6f2e    host: www.foo.
+000236f0: 636f 6d0a 2020 2020 2020 2020 746c 733a  com.        tls:
+00023700: 0a20 2020 2020 2020 202d 2073 6563 7265  .        - secre
+00023710: 745f 6e61 6d65 3a20 6170 702d 7365 6372  t_name: app-secr
+00023720: 6574 0a20 2020 2020 2020 2020 2068 6f73  et.          hos
+00023730: 7473 3a0a 2020 2020 2020 2020 2020 2d20  ts:.          - 
+00023740: 7777 772e 666f 6f2e 636f 6d0a 2020 2020  www.foo.com.    
+00023750: 2020 2020 2020 2d20 7777 772e 6261 722e        - www.bar.
+00023760: 636f 6d0a 2020 2020 2020 2020 2020 6e61  com.          na
+00023770: 6d65 3a20 666f 6f2d 6261 722d 696e 6772  me: foo-bar-ingr
+00023780: 6573 730a 2020 2020 2020 2020 2d20 7365  ess.        - se
+00023790: 6372 6574 5f6e 616d 653a 2061 7070 2d73  cret_name: app-s
+000237a0: 6563 7265 740a 2020 2020 2020 2020 2020  ecret.          
+000237b0: 686f 7374 733a 0a20 2020 2020 2020 2020  hosts:.         
+000237c0: 202d 2077 7777 2e66 6f6f 2e63 6f6d 0a20   - www.foo.com. 
+000237d0: 2020 2020 2020 2020 202d 2077 7777 2e62           - www.b
+000237e0: 6172 2e63 6f6d 0a20 2020 2020 2020 2020  ar.com.         
+000237f0: 206e 616d 653a 2066 6f6f 2d62 6172 2d69   name: foo-bar-i
+00023800: 6e67 7265 7373 0a20 2020 2020 2020 206c  ngress.        l
+00023810: 6162 656c 733a 0a20 2020 2020 2020 202d  abels:.        -
+00023820: 2061 7070 3a64 656d 6f2d 6170 700a 2020   app:demo-app.  
+00023830: 2020 2020 2020 2d20 7665 7273 696f 6e3a        - version:
+00023840: 7631 2e30 2e30 0a20 2020 2020 2070 726f  v1.0.0.      pro
+00023850: 7065 7274 6965 733a 0a20 2020 2020 2020  perties:.       
+00023860: 206e 616d 653a 0a20 2020 2020 2020 2020   name:.         
+00023870: 2064 6573 6372 6970 7469 6f6e 3a20 696e   description: in
+00023880: 6772 6573 7320 6e61 6d65 2e0a 2020 2020  gress name..    
+00023890: 2020 2020 2020 6578 616d 706c 653a 2064        example: d
+000238a0: 656d 6f2d 6170 702d 696e 6772 6573 730a  emo-app-ingress.
+000238b0: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+000238c0: 206e 616d 650a 2020 2020 2020 2020 2020   name.          
+000238d0: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+000238e0: 2020 2020 206e 616d 6573 7061 6365 3a0a       namespace:.
+000238f0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00023900: 7074 696f 6e3a 206e 616d 6573 7061 6365  ption: namespace
+00023910: 2066 6f72 2072 6573 6f75 7263 652e 0a20   for resource.. 
+00023920: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
+00023930: 3a20 6769 746f 7073 2d63 646e 2d63 6163  : gitops-cdn-cac
+00023940: 6865 0a20 2020 2020 2020 2020 2074 6974  he.          tit
+00023950: 6c65 3a20 6e61 6d65 7370 6163 650a 2020  le: namespace.  
+00023960: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
+00023970: 7269 6e67 0a20 2020 2020 2020 2061 6e6e  ring.        ann
+00023980: 6f74 6174 696f 6e73 3a0a 2020 2020 2020  otations:.      
+00023990: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+000239a0: 2041 6e20 756e 7374 7275 6374 7572 6564   An unstructured
+000239b0: 206b 6579 2076 616c 7565 206d 6170 2074   key value map t
+000239c0: 6861 7420 6361 6e20 6265 2075 7365 6420  hat can be used 
+000239d0: 746f 2061 7474 6163 6820 6172 6269 7472  to attach arbitr
+000239e0: 6172 790a 2020 2020 2020 2020 2020 2020  ary.            
+000239f0: 6d65 7461 6461 7461 0a20 2020 2020 2020  metadata.       
+00023a00: 2020 2065 7861 6d70 6c65 3a0a 2020 2020     example:.    
+00023a10: 2020 2020 2020 2d20 616e 6e6f 7461 7469        - annotati
+00023a20: 6f6e 2d6b 6579 313a 7661 6c31 0a20 2020  on-key1:val1.   
+00023a30: 2020 2020 2020 202d 2061 6e6e 6f74 6174         - annotat
+00023a40: 696f 6e2d 6b65 7932 3a76 616c 320a 2020  ion-key2:val2.  
+00023a50: 2020 2020 2020 2020 6974 656d 733a 0a20          items:. 
+00023a60: 2020 2020 2020 2020 2020 2074 7970 653a             type:
+00023a70: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00023a80: 2020 7469 746c 653a 2041 6e6e 6f74 6174    title: Annotat
+00023a90: 696f 6e73 0a20 2020 2020 2020 2020 2074  ions.          t
+00023aa0: 7970 653a 2061 7272 6179 0a20 2020 2020  ype: array.     
+00023ab0: 2020 206c 6162 656c 733a 0a20 2020 2020     labels:.     
+00023ac0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00023ad0: 3a20 4d61 7020 6f66 2073 7472 696e 6720  : Map of string 
+00023ae0: 6b65 7973 2061 6e64 2076 616c 7565 7320  keys and values 
+00023af0: 7468 6174 2063 616e 2062 6520 7573 6564  that can be used
+00023b00: 2074 6f20 6f72 6761 6e69 7a65 0a20 2020   to organize.   
+00023b10: 2020 2020 2020 2020 2061 6e64 2063 6174           and cat
+00023b20: 6567 6f72 697a 6520 2873 636f 7065 2061  egorize (scope a
+00023b30: 6e64 2073 656c 6563 7429 206f 626a 6563  nd select) objec
+00023b40: 7473 0a20 2020 2020 2020 2020 2065 7861  ts.          exa
+00023b50: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
+00023b60: 2d20 6170 703a 6465 6d6f 2d61 7070 0a20  - app:demo-app. 
+00023b70: 2020 2020 2020 2020 202d 2076 6572 7369           - versi
+00023b80: 6f6e 3a76 312e 302e 300a 2020 2020 2020  on:v1.0.0.      
+00023b90: 2020 2020 6974 656d 733a 0a20 2020 2020      items:.     
+00023ba0: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+00023bb0: 696e 670a 2020 2020 2020 2020 2020 7469  ing.          ti
+00023bc0: 746c 653a 204c 6162 656c 730a 2020 2020  tle: Labels.    
+00023bd0: 2020 2020 2020 7479 7065 3a20 6172 7261        type: arra
+00023be0: 790a 2020 2020 2020 2020 7275 6c65 733a  y.        rules:
+00023bf0: 0a20 2020 2020 2020 2020 2069 7465 6d73  .          items
+00023c00: 3a0a 2020 2020 2020 2020 2020 2020 2472  :.            $r
+00023c10: 6566 3a20 2723 2f63 6f6d 706f 6e65 6e74  ef: '#/component
+00023c20: 732f 7363 6865 6d61 732f 496e 6772 6573  s/schemas/Ingres
+00023c30: 7352 756c 6527 0a20 2020 2020 2020 2020  sRule'.         
+00023c40: 2074 6974 6c65 3a20 7275 6c65 730a 2020   title: rules.  
+00023c50: 2020 2020 2020 2020 7479 7065 3a20 6172          type: ar
+00023c60: 7261 790a 2020 2020 2020 2020 746c 733a  ray.        tls:
+00023c70: 0a20 2020 2020 2020 2020 2069 7465 6d73  .          items
+00023c80: 3a0a 2020 2020 2020 2020 2020 2020 2472  :.            $r
+00023c90: 6566 3a20 2723 2f63 6f6d 706f 6e65 6e74  ef: '#/component
+00023ca0: 732f 7363 6865 6d61 732f 496e 6772 6573  s/schemas/Ingres
+00023cb0: 7354 4c53 270a 2020 2020 2020 2020 2020  sTLS'.          
+00023cc0: 7469 746c 653a 2074 6c73 0a20 2020 2020  title: tls.     
+00023cd0: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
+00023ce0: 0a20 2020 2020 2072 6571 7569 7265 643a  .      required:
+00023cf0: 0a20 2020 2020 202d 206e 616d 650a 2020  .      - name.  
+00023d00: 2020 2020 7469 746c 653a 2049 6e67 7265      title: Ingre
+00023d10: 7373 0a20 2020 2020 2074 7970 653a 206f  ss.      type: o
+00023d20: 626a 6563 740a 2020 2020 496e 6772 6573  bject.    Ingres
+00023d30: 7352 756c 653a 0a20 2020 2020 2065 7861  sRule:.      exa
+00023d40: 6d70 6c65 3a0a 2020 2020 2020 2020 7061  mple:.        pa
+00023d50: 7468 733a 0a20 2020 2020 2020 202d 2070  ths:.        - p
+00023d60: 6174 683a 202f 6261 720a 2020 2020 2020  ath: /bar.      
+00023d70: 2020 2020 6e61 6d65 3a20 696e 6772 6573      name: ingres
+00023d80: 732d 7061 7468 2d62 6172 0a20 2020 2020  s-path-bar.     
+00023d90: 2020 2020 2070 6174 685f 7479 7065 3a20       path_type: 
+00023da0: 4578 6163 740a 2020 2020 2020 2020 2020  Exact.          
+00023db0: 6261 636b 656e 643a 0a20 2020 2020 2020  backend:.       
+00023dc0: 2020 2020 2073 6572 7669 6365 3a0a 2020       service:.  
+00023dd0: 2020 2020 2020 2020 2020 2020 706f 7274              port
+00023de0: 3a20 3830 0a20 2020 2020 2020 2020 2020  : 80.           
+00023df0: 2020 206e 616d 653a 2064 656d 6f2d 6170     name: demo-ap
+00023e00: 702d 7365 7276 6963 650a 2020 2020 2020  p-service.      
+00023e10: 2020 2d20 7061 7468 3a20 2f62 6172 0a20    - path: /bar. 
+00023e20: 2020 2020 2020 2020 206e 616d 653a 2069           name: i
+00023e30: 6e67 7265 7373 2d70 6174 682d 6261 720a  ngress-path-bar.
+00023e40: 2020 2020 2020 2020 2020 7061 7468 5f74            path_t
+00023e50: 7970 653a 2045 7861 6374 0a20 2020 2020  ype: Exact.     
+00023e60: 2020 2020 2062 6163 6b65 6e64 3a0a 2020       backend:.  
+00023e70: 2020 2020 2020 2020 2020 7365 7276 6963            servic
+00023e80: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00023e90: 2070 6f72 743a 2038 300a 2020 2020 2020   port: 80.      
+00023ea0: 2020 2020 2020 2020 6e61 6d65 3a20 6465          name: de
+00023eb0: 6d6f 2d61 7070 2d73 6572 7669 6365 0a20  mo-app-service. 
+00023ec0: 2020 2020 2020 206e 616d 653a 2066 6f6f         name: foo
+00023ed0: 2d69 6e67 7265 7373 2d72 756c 650a 2020  -ingress-rule.  
+00023ee0: 2020 2020 2020 686f 7374 3a20 7777 772e        host: www.
+00023ef0: 666f 6f2e 636f 6d0a 2020 2020 2020 7072  foo.com.      pr
+00023f00: 6f70 6572 7469 6573 3a0a 2020 2020 2020  operties:.      
+00023f10: 2020 6e61 6d65 3a0a 2020 2020 2020 2020    name:.        
+00023f20: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
+00023f30: 6865 2072 756c 6520 6e61 6d65 2e0a 2020  he rule name..  
+00023f40: 2020 2020 2020 2020 6578 616d 706c 653a          example:
+00023f50: 2066 6f6f 2d69 6e67 7265 7373 2d72 756c   foo-ingress-rul
+00023f60: 650a 2020 2020 2020 2020 2020 7469 746c  e.          titl
+00023f70: 653a 206e 616d 650a 2020 2020 2020 2020  e: name.        
+00023f80: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+00023f90: 2020 2020 2020 2068 6f73 743a 0a20 2020         host:.   
+00023fa0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00023fb0: 6f6e 3a20 4120 6675 6c6c 7920 7175 616c  on: A fully qual
+00023fc0: 6966 6965 6420 646f 6d61 696e 206e 616d  ified domain nam
+00023fd0: 6520 6f66 2061 206e 6574 776f 726b 2068  e of a network h
+00023fe0: 6f73 742e 0a20 2020 2020 2020 2020 2065  ost..          e
+00023ff0: 7861 6d70 6c65 3a20 7777 772e 666f 6f2e  xample: www.foo.
+00024000: 636f 6d0a 2020 2020 2020 2020 2020 7469  com.          ti
+00024010: 746c 653a 2068 6f73 740a 2020 2020 2020  tle: host.      
+00024020: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+00024030: 0a20 2020 2020 2020 2070 6174 6873 3a0a  .        paths:.
+00024040: 2020 2020 2020 2020 2020 6974 656d 733a            items:
+00024050: 0a20 2020 2020 2020 2020 2020 2024 7265  .            $re
+00024060: 663a 2027 232f 636f 6d70 6f6e 656e 7473  f: '#/components
+00024070: 2f73 6368 656d 6173 2f48 5454 5049 6e67  /schemas/HTTPIng
+00024080: 7265 7373 5061 7468 270a 2020 2020 2020  ressPath'.      
+00024090: 2020 2020 7469 746c 653a 2070 6174 6873      title: paths
+000240a0: 0a20 2020 2020 2020 2020 2074 7970 653a  .          type:
+000240b0: 2061 7272 6179 0a20 2020 2020 2074 6974   array.      tit
+000240c0: 6c65 3a20 496e 6772 6573 7352 756c 650a  le: IngressRule.
+000240d0: 2020 2020 2020 7479 7065 3a20 6f62 6a65        type: obje
+000240e0: 6374 0a20 2020 2048 5454 5049 6e67 7265  ct.    HTTPIngre
+000240f0: 7373 5061 7468 3a0a 2020 2020 2020 6578  ssPath:.      ex
+00024100: 616d 706c 653a 0a20 2020 2020 2020 2070  ample:.        p
+00024110: 6174 683a 202f 6261 720a 2020 2020 2020  ath: /bar.      
+00024120: 2020 6e61 6d65 3a20 696e 6772 6573 732d    name: ingress-
+00024130: 7061 7468 2d62 6172 0a20 2020 2020 2020  path-bar.       
+00024140: 2070 6174 685f 7479 7065 3a20 4578 6163   path_type: Exac
+00024150: 740a 2020 2020 2020 2020 6261 636b 656e  t.        backen
+00024160: 643a 0a20 2020 2020 2020 2020 2073 6572  d:.          ser
+00024170: 7669 6365 3a0a 2020 2020 2020 2020 2020  vice:.          
+00024180: 2020 706f 7274 3a20 3830 0a20 2020 2020    port: 80.     
+00024190: 2020 2020 2020 206e 616d 653a 2064 656d         name: dem
+000241a0: 6f2d 6170 702d 7365 7276 6963 650a 2020  o-app-service.  
+000241b0: 2020 2020 7072 6f70 6572 7469 6573 3a0a      properties:.
+000241c0: 2020 2020 2020 2020 6e61 6d65 3a0a 2020          name:.  
+000241d0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+000241e0: 696f 6e3a 2054 6865 2069 6e67 7265 7373  ion: The ingress
+000241f0: 2070 6174 6820 6e61 6d65 2e0a 2020 2020   path name..    
+00024200: 2020 2020 2020 6578 616d 706c 653a 2069        example: i
+00024210: 6e67 7265 7373 2d70 6174 682d 6261 720a  ngress-path-bar.
+00024220: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+00024230: 206e 616d 650a 2020 2020 2020 2020 2020   name.          
+00024240: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+00024250: 2020 2020 2070 6174 683a 0a20 2020 2020       path:.     
+00024260: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00024270: 3a20 5468 6520 7061 7468 2074 6861 7420  : The path that 
+00024280: 6973 206d 6174 6368 6564 2061 6761 696e  is matched again
+00024290: 7374 2074 6865 2070 6174 6820 6f66 2061  st the path of a
+000242a0: 6e20 696e 636f 6d69 6e67 2072 6571 7565  n incoming reque
+000242b0: 7374 2e0a 2020 2020 2020 2020 2020 2020  st..            
+000242c0: 4d75 7374 2062 6567 696e 2077 6974 6820  Must begin with 
+000242d0: 6120 272f 272e 0a20 2020 2020 2020 2020  a '/'..         
+000242e0: 2065 7861 6d70 6c65 3a20 2f62 6172 0a20   example: /bar. 
+000242f0: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
+00024300: 7061 7468 0a20 2020 2020 2020 2020 2074  path.          t
+00024310: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
+00024320: 2020 2020 7061 7468 5f74 7970 653a 0a20      path_type:. 
+00024330: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00024340: 7469 6f6e 3a20 5061 7468 5479 7065 2064  tion: PathType d
+00024350: 6574 6572 6d69 6e65 7320 7468 6520 696e  etermines the in
+00024360: 7465 7270 7265 7461 7469 6f6e 206f 6620  terpretation of 
+00024370: 7468 6520 5061 7468 206d 6174 6368 696e  the Path matchin
+00024380: 672e 0a20 2020 2020 2020 2020 2065 6e75  g..          enu
+00024390: 6d3a 0a20 2020 2020 2020 2020 202d 2045  m:.          - E
+000243a0: 7861 6374 0a20 2020 2020 2020 2020 202d  xact.          -
+000243b0: 2050 7265 6669 780a 2020 2020 2020 2020   Prefix.        
+000243c0: 2020 6578 616d 706c 653a 2045 7861 6374    example: Exact
+000243d0: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
+000243e0: 3a20 7061 7468 5f74 7970 650a 2020 2020  : path_type.    
+000243f0: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+00024400: 6e67 0a20 2020 2020 2020 2062 6163 6b65  ng.        backe
+00024410: 6e64 3a0a 2020 2020 2020 2020 2020 2472  nd:.          $r
+00024420: 6566 3a20 2723 2f63 6f6d 706f 6e65 6e74  ef: '#/component
+00024430: 732f 7363 6865 6d61 732f 496e 6772 6573  s/schemas/Ingres
+00024440: 7342 6163 6b65 6e64 270a 2020 2020 2020  sBackend'.      
+00024450: 7469 746c 653a 2048 5454 5049 6e67 7265  title: HTTPIngre
+00024460: 7373 5061 7468 0a20 2020 2020 2074 7970  ssPath.      typ
+00024470: 653a 206f 626a 6563 740a 2020 2020 496e  e: object.    In
+00024480: 6772 6573 7342 6163 6b65 6e64 3a0a 2020  gressBackend:.  
+00024490: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
+000244a0: 2020 2020 2073 6572 7669 6365 3a0a 2020       service:.  
+000244b0: 2020 2020 2020 2020 706f 7274 3a20 3830          port: 80
+000244c0: 0a20 2020 2020 2020 2020 206e 616d 653a  .          name:
+000244d0: 2064 656d 6f2d 6170 702d 7365 7276 6963   demo-app-servic
+000244e0: 650a 2020 2020 2020 7072 6f70 6572 7469  e.      properti
+000244f0: 6573 3a0a 2020 2020 2020 2020 7365 7276  es:.        serv
+00024500: 6963 653a 0a20 2020 2020 2020 2020 2024  ice:.          $
+00024510: 7265 663a 2027 232f 636f 6d70 6f6e 656e  ref: '#/componen
+00024520: 7473 2f73 6368 656d 6173 2f49 6e67 7265  ts/schemas/Ingre
+00024530: 7373 4261 636b 656e 645f 7365 7276 6963  ssBackend_servic
+00024540: 6527 0a20 2020 2020 2074 6974 6c65 3a20  e'.      title: 
+00024550: 496e 6772 6573 7342 6163 6b65 6e64 0a20  IngressBackend. 
+00024560: 2020 2020 2074 7970 653a 206f 626a 6563       type: objec
+00024570: 740a 2020 2020 496e 6772 6573 7354 4c53  t.    IngressTLS
+00024580: 3a0a 2020 2020 2020 6578 616d 706c 653a  :.      example:
+00024590: 0a20 2020 2020 2020 2073 6563 7265 745f  .        secret_
+000245a0: 6e61 6d65 3a20 6170 702d 7365 6372 6574  name: app-secret
+000245b0: 0a20 2020 2020 2020 2068 6f73 7473 3a0a  .        hosts:.
+000245c0: 2020 2020 2020 2020 2d20 7777 772e 666f          - www.fo
+000245d0: 6f2e 636f 6d0a 2020 2020 2020 2020 2d20  o.com.        - 
+000245e0: 7777 772e 6261 722e 636f 6d0a 2020 2020  www.bar.com.    
+000245f0: 2020 2020 6e61 6d65 3a20 666f 6f2d 6261      name: foo-ba
+00024600: 722d 696e 6772 6573 730a 2020 2020 2020  r-ingress.      
+00024610: 7072 6f70 6572 7469 6573 3a0a 2020 2020  properties:.    
+00024620: 2020 2020 6e61 6d65 3a0a 2020 2020 2020      name:.      
+00024630: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00024640: 204e 616d 6520 6f66 2074 6865 2054 4c53   Name of the TLS
+00024650: 2063 6f6e 6669 672e 0a20 2020 2020 2020   config..       
+00024660: 2020 2065 7861 6d70 6c65 3a20 666f 6f2d     example: foo-
+00024670: 6261 722d 696e 6772 6573 730a 2020 2020  bar-ingress.    
+00024680: 2020 2020 2020 7469 746c 653a 206e 616d        title: nam
+00024690: 650a 2020 2020 2020 2020 2020 7479 7065  e.          type
+000246a0: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+000246b0: 2068 6f73 7473 3a0a 2020 2020 2020 2020   hosts:.        
+000246c0: 2020 6465 7363 7269 7074 696f 6e3a 2041    description: A
+000246d0: 206c 6973 7420 6f66 2068 6f73 7473 2069   list of hosts i
+000246e0: 6e63 6c75 6465 6420 696e 2074 6865 2054  ncluded in the T
+000246f0: 4c53 2063 6572 7469 6669 6361 7465 2e0a  LS certificate..
+00024700: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
+00024710: 653a 0a20 2020 2020 2020 2020 202d 2077  e:.          - w
+00024720: 7777 2e66 6f6f 2e63 6f6d 0a20 2020 2020  ww.foo.com.     
+00024730: 2020 2020 202d 2077 7777 2e62 6172 2e63       - www.bar.c
+00024740: 6f6d 0a20 2020 2020 2020 2020 2069 7465  om.          ite
+00024750: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
+00024760: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+00024770: 2020 2020 2020 2074 6974 6c65 3a20 686f         title: ho
+00024780: 7374 730a 2020 2020 2020 2020 2020 7479  sts.          ty
+00024790: 7065 3a20 6172 7261 790a 2020 2020 2020  pe: array.      
+000247a0: 2020 7365 6372 6574 5f6e 616d 653a 0a20    secret_name:. 
+000247b0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+000247c0: 7469 6f6e 3a20 5468 6520 6e61 6d65 206f  tion: The name o
+000247d0: 6620 7468 6520 7365 6372 6574 2075 7365  f the secret use
+000247e0: 6420 746f 2074 6572 6d69 6e61 7465 2054  d to terminate T
+000247f0: 4c53 2074 7261 6666 6963 206f 6e20 706f  LS traffic on po
+00024800: 7274 0a20 2020 2020 2020 2020 2020 2034  rt.            4
+00024810: 3433 2e0a 2020 2020 2020 2020 2020 6578  43..          ex
+00024820: 616d 706c 653a 2061 7070 2d73 6563 7265  ample: app-secre
+00024830: 740a 2020 2020 2020 2020 2020 7469 746c  t.          titl
+00024840: 653a 2073 6563 7265 745f 6e61 6d65 0a20  e: secret_name. 
+00024850: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
+00024860: 7472 696e 670a 2020 2020 2020 7469 746c  tring.      titl
+00024870: 653a 2049 6e67 7265 7373 544c 530a 2020  e: IngressTLS.  
+00024880: 2020 2020 7479 7065 3a20 6f62 6a65 6374      type: object
+00024890: 0a20 2020 2053 6572 7669 6365 4d6f 6e69  .    ServiceMoni
+000248a0: 746f 723a 0a20 2020 2020 2065 7861 6d70  tor:.      examp
+000248b0: 6c65 3a0a 2020 2020 2020 2020 6e61 6d65  le:.        name
+000248c0: 7370 6163 655f 7365 6c65 6374 6f72 3a0a  space_selector:.
+000248d0: 2020 2020 2020 2020 2020 6d61 7463 685f            match_
+000248e0: 6e61 6d65 733a 0a20 2020 2020 2020 2020  names:.         
+000248f0: 202d 2064 6566 6175 6c74 0a20 2020 2020   - default.     
+00024900: 2020 2020 2061 6e79 3a20 7472 7565 0a20       any: true. 
+00024910: 2020 2020 2020 2065 6e64 706f 696e 7473         endpoints
+00024920: 3a0a 2020 2020 2020 2020 2d20 686f 6e6f  :.        - hono
+00024930: 725f 6c61 6265 6c73 3a20 7472 7565 0a20  r_labels: true. 
+00024940: 2020 2020 2020 2020 2070 6174 683a 202f           path: /
+00024950: 6d65 7472 6963 730a 2020 2020 2020 2020  metrics.        
+00024960: 2020 7461 7267 6574 5f70 6f72 743a 2038    target_port: 8
+00024970: 3038 300a 2020 2020 2020 2020 2020 7265  080.          re
+00024980: 6c61 6265 6c69 6e67 733a 0a20 2020 2020  labelings:.     
+00024990: 2020 2020 202d 2072 6567 6578 3a20 282e       - regex: (.
+000249a0: 2a29 0a20 2020 2020 2020 2020 2020 2073  *).            s
+000249b0: 6f75 7263 655f 6c61 6265 6c73 3a0a 2020  ource_labels:.  
+000249c0: 2020 2020 2020 2020 2020 2d20 5f5f 6d65            - __me
+000249d0: 7461 5f6b 7562 6572 6e65 7465 735f 706f  ta_kubernetes_po
+000249e0: 645f 6c61 6265 6c5f 6170 705f 6b75 6265  d_label_app_kube
+000249f0: 726e 6574 6573 5f69 6f5f 6e61 6d65 0a20  rnetes_io_name. 
+00024a00: 2020 2020 2020 2020 2020 2061 6374 696f             actio
+00024a10: 6e3a 2072 6570 6c61 6365 0a20 2020 2020  n: replace.     
+00024a20: 2020 2020 2020 2073 6570 6172 6174 6f72         separator
+00024a30: 3a20 3b0a 2020 2020 2020 2020 2020 2020  : ;.            
+00024a40: 7265 706c 6163 656d 656e 743a 2024 310a  replacement: $1.
+00024a50: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00024a60: 6574 5f6c 6162 656c 3a20 5f5f 6d65 7472  et_label: __metr
+00024a70: 6963 735f 7061 7468 5f5f 0a20 2020 2020  ics_path__.     
+00024a80: 2020 2020 202d 2072 6567 6578 3a20 282e       - regex: (.
+00024a90: 2a29 0a20 2020 2020 2020 2020 2020 2073  *).            s
+00024aa0: 6f75 7263 655f 6c61 6265 6c73 3a0a 2020  ource_labels:.  
+00024ab0: 2020 2020 2020 2020 2020 2d20 5f5f 6d65            - __me
+00024ac0: 7461 5f6b 7562 6572 6e65 7465 735f 706f  ta_kubernetes_po
+00024ad0: 645f 6c61 6265 6c5f 6170 705f 6b75 6265  d_label_app_kube
+00024ae0: 726e 6574 6573 5f69 6f5f 6e61 6d65 0a20  rnetes_io_name. 
+00024af0: 2020 2020 2020 2020 2020 2061 6374 696f             actio
+00024b00: 6e3a 2072 6570 6c61 6365 0a20 2020 2020  n: replace.     
+00024b10: 2020 2020 2020 2073 6570 6172 6174 6f72         separator
+00024b20: 3a20 3b0a 2020 2020 2020 2020 2020 2020  : ;.            
+00024b30: 7265 706c 6163 656d 656e 743a 2024 310a  replacement: $1.
+00024b40: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00024b50: 6574 5f6c 6162 656c 3a20 5f5f 6d65 7472  et_label: __metr
+00024b60: 6963 735f 7061 7468 5f5f 0a20 2020 2020  ics_path__.     
+00024b70: 2020 2020 206d 6574 7269 635f 7265 6c61       metric_rela
+00024b80: 6265 6c69 6e67 733a 0a20 2020 2020 2020  belings:.       
+00024b90: 2020 202d 2072 6567 6578 3a20 282e 2a29     - regex: (.*)
+00024ba0: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
+00024bb0: 7263 655f 6c61 6265 6c73 3a0a 2020 2020  rce_labels:.    
+00024bc0: 2020 2020 2020 2020 2d20 5f5f 6d65 7461          - __meta
+00024bd0: 5f6b 7562 6572 6e65 7465 735f 706f 645f  _kubernetes_pod_
+00024be0: 6c61 6265 6c5f 6170 705f 6b75 6265 726e  label_app_kubern
+00024bf0: 6574 6573 5f69 6f5f 6e61 6d65 0a20 2020  etes_io_name.   
+00024c00: 2020 2020 2020 2020 2061 6374 696f 6e3a           action:
+00024c10: 2072 6570 6c61 6365 0a20 2020 2020 2020   replace.       
+00024c20: 2020 2020 2073 6570 6172 6174 6f72 3a20       separator: 
+00024c30: 3b0a 2020 2020 2020 2020 2020 2020 7265  ;.            re
+00024c40: 706c 6163 656d 656e 743a 2024 310a 2020  placement: $1.  
+00024c50: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00024c60: 5f6c 6162 656c 3a20 5f5f 6d65 7472 6963  _label: __metric
+00024c70: 735f 7061 7468 5f5f 0a20 2020 2020 2020  s_path__.       
+00024c80: 2020 202d 2072 6567 6578 3a20 282e 2a29     - regex: (.*)
+00024c90: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
+00024ca0: 7263 655f 6c61 6265 6c73 3a0a 2020 2020  rce_labels:.    
+00024cb0: 2020 2020 2020 2020 2d20 5f5f 6d65 7461          - __meta
+00024cc0: 5f6b 7562 6572 6e65 7465 735f 706f 645f  _kubernetes_pod_
+00024cd0: 6c61 6265 6c5f 6170 705f 6b75 6265 726e  label_app_kubern
+00024ce0: 6574 6573 5f69 6f5f 6e61 6d65 0a20 2020  etes_io_name.   
+00024cf0: 2020 2020 2020 2020 2061 6374 696f 6e3a           action:
+00024d00: 2072 6570 6c61 6365 0a20 2020 2020 2020   replace.       
+00024d10: 2020 2020 2073 6570 6172 6174 6f72 3a20       separator: 
+00024d20: 3b0a 2020 2020 2020 2020 2020 2020 7265  ;.            re
+00024d30: 706c 6163 656d 656e 743a 2024 310a 2020  placement: $1.  
+00024d40: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00024d50: 5f6c 6162 656c 3a20 5f5f 6d65 7472 6963  _label: __metric
+00024d60: 735f 7061 7468 5f5f 0a20 2020 2020 2020  s_path__.       
+00024d70: 2020 2073 6368 656d 653a 2068 7474 700a     scheme: http.
+00024d80: 2020 2020 2020 2020 2020 706f 7274 3a20            port: 
+00024d90: 3830 3830 0a20 2020 2020 2020 2020 2068  8080.          h
+00024da0: 6f6e 6f72 5f74 696d 6573 7461 6d70 733a  onor_timestamps:
+00024db0: 2074 7275 650a 2020 2020 2020 2020 2020   true.          
+00024dc0: 7363 7261 7065 5f74 696d 656f 7574 3a20  scrape_timeout: 
+00024dd0: 3130 730a 2020 2020 2020 2020 2020 696e  10s.          in
+00024de0: 7465 7276 616c 3a20 3330 730a 2020 2020  terval: 30s.    
+00024df0: 2020 2020 2020 7061 7261 6d73 3a0a 2020        params:.  
+00024e00: 2020 2020 2020 2020 2020 6d6f 6475 6c65            module
+00024e10: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
+00024e20: 6874 7470 5f32 7878 0a20 2020 2020 2020  http_2xx.       
+00024e30: 202d 2068 6f6e 6f72 5f6c 6162 656c 733a   - honor_labels:
+00024e40: 2074 7275 650a 2020 2020 2020 2020 2020   true.          
+00024e50: 7061 7468 3a20 2f6d 6574 7269 6373 0a20  path: /metrics. 
+00024e60: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+00024e70: 706f 7274 3a20 3830 3830 0a20 2020 2020  port: 8080.     
+00024e80: 2020 2020 2072 656c 6162 656c 696e 6773       relabelings
+00024e90: 3a0a 2020 2020 2020 2020 2020 2d20 7265  :.          - re
+00024ea0: 6765 783a 2028 2e2a 290a 2020 2020 2020  gex: (.*).      
+00024eb0: 2020 2020 2020 736f 7572 6365 5f6c 6162        source_lab
+00024ec0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+00024ed0: 202d 205f 5f6d 6574 615f 6b75 6265 726e   - __meta_kubern
+00024ee0: 6574 6573 5f70 6f64 5f6c 6162 656c 5f61  etes_pod_label_a
+00024ef0: 7070 5f6b 7562 6572 6e65 7465 735f 696f  pp_kubernetes_io
+00024f00: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
+00024f10: 2020 6163 7469 6f6e 3a20 7265 706c 6163    action: replac
+00024f20: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+00024f30: 7061 7261 746f 723a 203b 0a20 2020 2020  parator: ;.     
+00024f40: 2020 2020 2020 2072 6570 6c61 6365 6d65         replaceme
+00024f50: 6e74 3a20 2431 0a20 2020 2020 2020 2020  nt: $1.         
+00024f60: 2020 2074 6172 6765 745f 6c61 6265 6c3a     target_label:
+00024f70: 205f 5f6d 6574 7269 6373 5f70 6174 685f   __metrics_path_
+00024f80: 5f0a 2020 2020 2020 2020 2020 2d20 7265  _.          - re
+00024f90: 6765 783a 2028 2e2a 290a 2020 2020 2020  gex: (.*).      
+00024fa0: 2020 2020 2020 736f 7572 6365 5f6c 6162        source_lab
+00024fb0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+00024fc0: 202d 205f 5f6d 6574 615f 6b75 6265 726e   - __meta_kubern
+00024fd0: 6574 6573 5f70 6f64 5f6c 6162 656c 5f61  etes_pod_label_a
+00024fe0: 7070 5f6b 7562 6572 6e65 7465 735f 696f  pp_kubernetes_io
+00024ff0: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
+00025000: 2020 6163 7469 6f6e 3a20 7265 706c 6163    action: replac
+00025010: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+00025020: 7061 7261 746f 723a 203b 0a20 2020 2020  parator: ;.     
+00025030: 2020 2020 2020 2072 6570 6c61 6365 6d65         replaceme
+00025040: 6e74 3a20 2431 0a20 2020 2020 2020 2020  nt: $1.         
+00025050: 2020 2074 6172 6765 745f 6c61 6265 6c3a     target_label:
+00025060: 205f 5f6d 6574 7269 6373 5f70 6174 685f   __metrics_path_
+00025070: 5f0a 2020 2020 2020 2020 2020 6d65 7472  _.          metr
+00025080: 6963 5f72 656c 6162 656c 696e 6773 3a0a  ic_relabelings:.
+00025090: 2020 2020 2020 2020 2020 2d20 7265 6765            - rege
+000250a0: 783a 2028 2e2a 290a 2020 2020 2020 2020  x: (.*).        
+000250b0: 2020 2020 736f 7572 6365 5f6c 6162 656c      source_label
+000250c0: 733a 0a20 2020 2020 2020 2020 2020 202d  s:.            -
+000250d0: 205f 5f6d 6574 615f 6b75 6265 726e 6574   __meta_kubernet
+000250e0: 6573 5f70 6f64 5f6c 6162 656c 5f61 7070  es_pod_label_app
+000250f0: 5f6b 7562 6572 6e65 7465 735f 696f 5f6e  _kubernetes_io_n
+00025100: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+00025110: 6163 7469 6f6e 3a20 7265 706c 6163 650a  action: replace.
+00025120: 2020 2020 2020 2020 2020 2020 7365 7061              sepa
+00025130: 7261 746f 723a 203b 0a20 2020 2020 2020  rator: ;.       
+00025140: 2020 2020 2072 6570 6c61 6365 6d65 6e74       replacement
+00025150: 3a20 2431 0a20 2020 2020 2020 2020 2020  : $1.           
+00025160: 2074 6172 6765 745f 6c61 6265 6c3a 205f   target_label: _
+00025170: 5f6d 6574 7269 6373 5f70 6174 685f 5f0a  _metrics_path__.
+00025180: 2020 2020 2020 2020 2020 2d20 7265 6765            - rege
+00025190: 783a 2028 2e2a 290a 2020 2020 2020 2020  x: (.*).        
+000251a0: 2020 2020 736f 7572 6365 5f6c 6162 656c      source_label
+000251b0: 733a 0a20 2020 2020 2020 2020 2020 202d  s:.            -
+000251c0: 205f 5f6d 6574 615f 6b75 6265 726e 6574   __meta_kubernet
+000251d0: 6573 5f70 6f64 5f6c 6162 656c 5f61 7070  es_pod_label_app
+000251e0: 5f6b 7562 6572 6e65 7465 735f 696f 5f6e  _kubernetes_io_n
+000251f0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+00025200: 6163 7469 6f6e 3a20 7265 706c 6163 650a  action: replace.
+00025210: 2020 2020 2020 2020 2020 2020 7365 7061              sepa
+00025220: 7261 746f 723a 203b 0a20 2020 2020 2020  rator: ;.       
+00025230: 2020 2020 2072 6570 6c61 6365 6d65 6e74       replacement
+00025240: 3a20 2431 0a20 2020 2020 2020 2020 2020  : $1.           
+00025250: 2074 6172 6765 745f 6c61 6265 6c3a 205f   target_label: _
+00025260: 5f6d 6574 7269 6373 5f70 6174 685f 5f0a  _metrics_path__.
+00025270: 2020 2020 2020 2020 2020 7363 6865 6d65            scheme
+00025280: 3a20 6874 7470 0a20 2020 2020 2020 2020  : http.         
+00025290: 2070 6f72 743a 2038 3038 300a 2020 2020   port: 8080.    
+000252a0: 2020 2020 2020 686f 6e6f 725f 7469 6d65        honor_time
+000252b0: 7374 616d 7073 3a20 7472 7565 0a20 2020  stamps: true.   
+000252c0: 2020 2020 2020 2073 6372 6170 655f 7469         scrape_ti
+000252d0: 6d65 6f75 743a 2031 3073 0a20 2020 2020  meout: 10s.     
+000252e0: 2020 2020 2069 6e74 6572 7661 6c3a 2033       interval: 3
+000252f0: 3073 0a20 2020 2020 2020 2020 2070 6172  0s.          par
+00025300: 616d 733a 0a20 2020 2020 2020 2020 2020  ams:.           
+00025310: 206d 6f64 756c 653a 0a20 2020 2020 2020   module:.       
+00025320: 2020 2020 202d 2068 7474 705f 3278 780a       - http_2xx.
+00025330: 2020 2020 2020 2020 6e61 6d65 3a20 6d79          name: my
+00025340: 2d73 6572 7669 6365 2d6d 6f6e 6974 6f72  -service-monitor
+00025350: 0a20 2020 2020 2020 206e 616d 6573 7061  .        namespa
+00025360: 6365 3a20 6769 746f 7073 2d63 646e 2d63  ce: gitops-cdn-c
+00025370: 6163 6865 0a20 2020 2020 2020 2061 6e6e  ache.        ann
+00025380: 6f74 6174 696f 6e73 3a0a 2020 2020 2020  otations:.      
+00025390: 2020 2d20 616e 6e6f 7461 7469 6f6e 2d6b    - annotation-k
+000253a0: 6579 313a 7661 6c31 0a20 2020 2020 2020  ey1:val1.       
+000253b0: 202d 2061 6e6e 6f74 6174 696f 6e2d 6b65   - annotation-ke
+000253c0: 7932 3a76 616c 320a 2020 2020 2020 2020  y2:val2.        
+000253d0: 7365 6c65 6374 6f72 3a0a 2020 2020 2020  selector:.      
+000253e0: 2020 2d20 6170 703a 6465 6d6f 2d61 7070    - app:demo-app
+000253f0: 0a20 2020 2020 2020 202d 2022 6b65 793a  .        - "key:
+00025400: 7665 7273 696f 6e2c 206f 7065 7261 746f  version, operato
+00025410: 723a 496e 2c20 7661 6c75 6573 3a5b 7631  r:In, values:[v1
+00025420: 2e30 2e30 2c20 7631 2e30 2e31 5d22 0a20  .0.0, v1.0.1]". 
+00025430: 2020 2020 2020 206c 6162 656c 733a 0a20         labels:. 
+00025440: 2020 2020 2020 202d 2061 7070 3a64 656d         - app:dem
+00025450: 6f2d 6170 700a 2020 2020 2020 2020 2d20  o-app.        - 
+00025460: 7665 7273 696f 6e3a 7631 2e30 2e30 0a20  version:v1.0.0. 
+00025470: 2020 2020 2070 726f 7065 7274 6965 733a       properties:
+00025480: 0a20 2020 2020 2020 206e 616d 653a 0a20  .        name:. 
+00025490: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+000254a0: 7469 6f6e 3a20 226e 616d 6520 6f66 2073  tion: "name of s
+000254b0: 6572 7669 6365 206d 6f6e 6974 6f72 2c20  ervice monitor, 
+000254c0: 7573 6564 2069 6e20 6d65 7461 6461 7461  used in metadata
+000254d0: 2e6e 616d 6522 0a20 2020 2020 2020 2020  .name".         
+000254e0: 2065 7861 6d70 6c65 3a20 6d79 2d73 6572   example: my-ser
+000254f0: 7669 6365 2d6d 6f6e 6974 6f72 0a20 2020  vice-monitor.   
+00025500: 2020 2020 2020 2074 6974 6c65 3a20 6e61         title: na
+00025510: 6d65 0a20 2020 2020 2020 2020 2074 7970  me.          typ
+00025520: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
+00025530: 2020 6e61 6d65 7370 6163 653a 0a20 2020    namespace:.   
+00025540: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00025550: 6f6e 3a20 6e61 6d65 7370 6163 6520 666f  on: namespace fo
+00025560: 7220 7265 736f 7572 6365 2e0a 2020 2020  r resource..    
+00025570: 2020 2020 2020 6578 616d 706c 653a 2067        example: g
+00025580: 6974 6f70 732d 6364 6e2d 6361 6368 650a  itops-cdn-cache.
+00025590: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+000255a0: 206e 616d 6573 7061 6365 0a20 2020 2020   namespace.     
+000255b0: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+000255c0: 670a 2020 2020 2020 2020 6c61 6265 6c73  g.        labels
+000255d0: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
+000255e0: 7269 7074 696f 6e3a 204d 6170 206f 6620  ription: Map of 
+000255f0: 7374 7269 6e67 206b 6579 7320 616e 6420  string keys and 
+00025600: 7661 6c75 6573 2074 6861 7420 6361 6e20  values that can 
+00025610: 6265 2075 7365 6420 746f 206f 7267 616e  be used to organ
+00025620: 697a 650a 2020 2020 2020 2020 2020 2020  ize.            
+00025630: 616e 6420 6361 7465 676f 7269 7a65 2028  and categorize (
+00025640: 7363 6f70 6520 616e 6420 7365 6c65 6374  scope and select
+00025650: 2920 6f62 6a65 6374 730a 2020 2020 2020  ) objects.      
+00025660: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
+00025670: 2020 2020 2020 202d 2061 7070 3a64 656d         - app:dem
+00025680: 6f2d 6170 700a 2020 2020 2020 2020 2020  o-app.          
+00025690: 2d20 7665 7273 696f 6e3a 7631 2e30 2e30  - version:v1.0.0
+000256a0: 0a20 2020 2020 2020 2020 2069 7465 6d73  .          items
+000256b0: 3a0a 2020 2020 2020 2020 2020 2020 7479  :.            ty
+000256c0: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
+000256d0: 2020 2020 2074 6974 6c65 3a20 4c61 6265       title: Labe
+000256e0: 6c73 0a20 2020 2020 2020 2020 2074 7970  ls.          typ
+000256f0: 653a 2061 7272 6179 0a20 2020 2020 2020  e: array.       
+00025700: 2061 6e6e 6f74 6174 696f 6e73 3a0a 2020   annotations:.  
+00025710: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00025720: 696f 6e3a 2041 6e20 756e 7374 7275 6374  ion: An unstruct
+00025730: 7572 6564 206b 6579 2076 616c 7565 206d  ured key value m
+00025740: 6170 2074 6861 7420 6361 6e20 6265 2075  ap that can be u
+00025750: 7365 6420 746f 2061 7474 6163 6820 6172  sed to attach ar
+00025760: 6269 7472 6172 790a 2020 2020 2020 2020  bitrary.        
+00025770: 2020 2020 6d65 7461 6461 7461 0a20 2020      metadata.   
+00025780: 2020 2020 2020 2065 7861 6d70 6c65 3a0a         example:.
+00025790: 2020 2020 2020 2020 2020 2d20 616e 6e6f            - anno
+000257a0: 7461 7469 6f6e 2d6b 6579 313a 7661 6c31  tation-key1:val1
+000257b0: 0a20 2020 2020 2020 2020 202d 2061 6e6e  .          - ann
+000257c0: 6f74 6174 696f 6e2d 6b65 7932 3a76 616c  otation-key2:val
+000257d0: 320a 2020 2020 2020 2020 2020 6974 656d  2.          item
+000257e0: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
+000257f0: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
+00025800: 2020 2020 2020 7469 746c 653a 2041 6e6e        title: Ann
+00025810: 6f74 6174 696f 6e73 0a20 2020 2020 2020  otations.       
+00025820: 2020 2074 7970 653a 2061 7272 6179 0a20     type: array. 
+00025830: 2020 2020 2020 2065 6e64 706f 696e 7473         endpoints
+00025840: 3a0a 2020 2020 2020 2020 2020 6974 656d  :.          item
+00025850: 733a 0a20 2020 2020 2020 2020 2020 2024  s:.            $
+00025860: 7265 663a 2027 232f 636f 6d70 6f6e 656e  ref: '#/componen
+00025870: 7473 2f73 6368 656d 6173 2f45 6e64 706f  ts/schemas/Endpo
+00025880: 696e 7427 0a20 2020 2020 2020 2020 2074  int'.          t
+00025890: 6974 6c65 3a20 656e 6470 6f69 6e74 730a  itle: endpoints.
+000258a0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
+000258b0: 6172 7261 790a 2020 2020 2020 2020 7365  array.        se
+000258c0: 6c65 6374 6f72 3a0a 2020 2020 2020 2020  lector:.        
+000258d0: 2020 6465 7363 7269 7074 696f 6e3a 207c    description: |
+000258e0: 0a20 2020 2020 2020 2020 2020 2041 6e20  .            An 
+000258f0: 6172 7261 7920 6f66 206c 6162 656c 2073  array of label s
+00025900: 656c 6563 746f 7220 7275 6c65 2c20 7468  elector rule, th
+00025910: 6520 7275 6c65 2063 616e 2065 6974 6865  e rule can eithe
+00025920: 7220 6265 2061 206d 6174 6368 206c 6162  r be a match lab
+00025930: 656c 206f 7220 6d61 7463 6820 6578 7072  el or match expr
+00025940: 6573 7369 6f6e 2c0a 2020 2020 2020 2020  ession,.        
+00025950: 2020 2020 7265 6665 7272 696e 6720 7468      referring th
+00025960: 6520 6578 616d 706c 6520 2866 6972 7374  e example (first
+00025970: 2069 7320 6120 6d61 7463 6820 6c61 6265   is a match labe
+00025980: 6c2c 2073 6563 6f6e 6420 6973 2061 206d  l, second is a m
+00025990: 6174 6368 2065 7870 7265 7373 696f 6e29  atch expression)
+000259a0: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
+000259b0: 6c65 3a0a 2020 2020 2020 2020 2020 2d20  le:.          - 
+000259c0: 6170 703a 6465 6d6f 2d61 7070 0a20 2020  app:demo-app.   
+000259d0: 2020 2020 2020 202d 2022 6b65 793a 7665         - "key:ve
+000259e0: 7273 696f 6e2c 206f 7065 7261 746f 723a  rsion, operator:
+000259f0: 496e 2c20 7661 6c75 6573 3a5b 7631 2e30  In, values:[v1.0
+00025a00: 2e30 2c20 7631 2e30 2e31 5d22 0a20 2020  .0, v1.0.1]".   
+00025a10: 2020 2020 2020 2069 7465 6d73 3a0a 2020         items:.  
+00025a20: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
+00025a30: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
+00025a40: 2074 6974 6c65 3a20 4c61 6265 6c53 656c   title: LabelSel
+00025a50: 6563 746f 720a 2020 2020 2020 2020 2020  ector.          
+00025a60: 7479 7065 3a20 6172 7261 790a 2020 2020  type: array.    
+00025a70: 2020 2020 6e61 6d65 7370 6163 655f 7365      namespace_se
+00025a80: 6c65 6374 6f72 3a0a 2020 2020 2020 2020  lector:.        
+00025a90: 2020 2472 6566 3a20 2723 2f63 6f6d 706f    $ref: '#/compo
+00025aa0: 6e65 6e74 732f 7363 6865 6d61 732f 5365  nents/schemas/Se
+00025ab0: 7276 6963 654d 6f6e 6974 6f72 5f6e 616d  rviceMonitor_nam
+00025ac0: 6573 7061 6365 5f73 656c 6563 746f 7227  espace_selector'
+00025ad0: 0a20 2020 2020 2072 6571 7569 7265 643a  .      required:
+00025ae0: 0a20 2020 2020 202d 206e 616d 650a 2020  .      - name.  
+00025af0: 2020 2020 7469 746c 653a 2053 6572 7669      title: Servi
+00025b00: 6365 4d6f 6e69 746f 720a 2020 2020 2020  ceMonitor.      
+00025b10: 7479 7065 3a20 6f62 6a65 6374 0a20 2020  type: object.   
+00025b20: 2045 6e64 706f 696e 743a 0a20 2020 2020   Endpoint:.     
+00025b30: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
+00025b40: 2020 686f 6e6f 725f 6c61 6265 6c73 3a20    honor_labels: 
+00025b50: 7472 7565 0a20 2020 2020 2020 2070 6174  true.        pat
+00025b60: 683a 202f 6d65 7472 6963 730a 2020 2020  h: /metrics.    
+00025b70: 2020 2020 7461 7267 6574 5f70 6f72 743a      target_port:
+00025b80: 2038 3038 300a 2020 2020 2020 2020 7265   8080.        re
+00025b90: 6c61 6265 6c69 6e67 733a 0a20 2020 2020  labelings:.     
+00025ba0: 2020 202d 2072 6567 6578 3a20 282e 2a29     - regex: (.*)
+00025bb0: 0a20 2020 2020 2020 2020 2073 6f75 7263  .          sourc
+00025bc0: 655f 6c61 6265 6c73 3a0a 2020 2020 2020  e_labels:.      
+00025bd0: 2020 2020 2d20 5f5f 6d65 7461 5f6b 7562      - __meta_kub
+00025be0: 6572 6e65 7465 735f 706f 645f 6c61 6265  ernetes_pod_labe
+00025bf0: 6c5f 6170 705f 6b75 6265 726e 6574 6573  l_app_kubernetes
+00025c00: 5f69 6f5f 6e61 6d65 0a20 2020 2020 2020  _io_name.       
+00025c10: 2020 2061 6374 696f 6e3a 2072 6570 6c61     action: repla
+00025c20: 6365 0a20 2020 2020 2020 2020 2073 6570  ce.          sep
+00025c30: 6172 6174 6f72 3a20 3b0a 2020 2020 2020  arator: ;.      
+00025c40: 2020 2020 7265 706c 6163 656d 656e 743a      replacement:
+00025c50: 2024 310a 2020 2020 2020 2020 2020 7461   $1.          ta
+00025c60: 7267 6574 5f6c 6162 656c 3a20 5f5f 6d65  rget_label: __me
+00025c70: 7472 6963 735f 7061 7468 5f5f 0a20 2020  trics_path__.   
+00025c80: 2020 2020 202d 2072 6567 6578 3a20 282e       - regex: (.
+00025c90: 2a29 0a20 2020 2020 2020 2020 2073 6f75  *).          sou
+00025ca0: 7263 655f 6c61 6265 6c73 3a0a 2020 2020  rce_labels:.    
+00025cb0: 2020 2020 2020 2d20 5f5f 6d65 7461 5f6b        - __meta_k
+00025cc0: 7562 6572 6e65 7465 735f 706f 645f 6c61  ubernetes_pod_la
+00025cd0: 6265 6c5f 6170 705f 6b75 6265 726e 6574  bel_app_kubernet
+00025ce0: 6573 5f69 6f5f 6e61 6d65 0a20 2020 2020  es_io_name.     
+00025cf0: 2020 2020 2061 6374 696f 6e3a 2072 6570       action: rep
+00025d00: 6c61 6365 0a20 2020 2020 2020 2020 2073  lace.          s
+00025d10: 6570 6172 6174 6f72 3a20 3b0a 2020 2020  eparator: ;.    
+00025d20: 2020 2020 2020 7265 706c 6163 656d 656e        replacemen
+00025d30: 743a 2024 310a 2020 2020 2020 2020 2020  t: $1.          
+00025d40: 7461 7267 6574 5f6c 6162 656c 3a20 5f5f  target_label: __
+00025d50: 6d65 7472 6963 735f 7061 7468 5f5f 0a20  metrics_path__. 
+00025d60: 2020 2020 2020 206d 6574 7269 635f 7265         metric_re
+00025d70: 6c61 6265 6c69 6e67 733a 0a20 2020 2020  labelings:.     
+00025d80: 2020 202d 2072 6567 6578 3a20 282e 2a29     - regex: (.*)
+00025d90: 0a20 2020 2020 2020 2020 2073 6f75 7263  .          sourc
+00025da0: 655f 6c61 6265 6c73 3a0a 2020 2020 2020  e_labels:.      
+00025db0: 2020 2020 2d20 5f5f 6d65 7461 5f6b 7562      - __meta_kub
+00025dc0: 6572 6e65 7465 735f 706f 645f 6c61 6265  ernetes_pod_labe
+00025dd0: 6c5f 6170 705f 6b75 6265 726e 6574 6573  l_app_kubernetes
+00025de0: 5f69 6f5f 6e61 6d65 0a20 2020 2020 2020  _io_name.       
+00025df0: 2020 2061 6374 696f 6e3a 2072 6570 6c61     action: repla
+00025e00: 6365 0a20 2020 2020 2020 2020 2073 6570  ce.          sep
+00025e10: 6172 6174 6f72 3a20 3b0a 2020 2020 2020  arator: ;.      
+00025e20: 2020 2020 7265 706c 6163 656d 656e 743a      replacement:
+00025e30: 2024 310a 2020 2020 2020 2020 2020 7461   $1.          ta
+00025e40: 7267 6574 5f6c 6162 656c 3a20 5f5f 6d65  rget_label: __me
+00025e50: 7472 6963 735f 7061 7468 5f5f 0a20 2020  trics_path__.   
+00025e60: 2020 2020 202d 2072 6567 6578 3a20 282e       - regex: (.
+00025e70: 2a29 0a20 2020 2020 2020 2020 2073 6f75  *).          sou
+00025e80: 7263 655f 6c61 6265 6c73 3a0a 2020 2020  rce_labels:.    
+00025e90: 2020 2020 2020 2d20 5f5f 6d65 7461 5f6b        - __meta_k
+00025ea0: 7562 6572 6e65 7465 735f 706f 645f 6c61  ubernetes_pod_la
+00025eb0: 6265 6c5f 6170 705f 6b75 6265 726e 6574  bel_app_kubernet
+00025ec0: 6573 5f69 6f5f 6e61 6d65 0a20 2020 2020  es_io_name.     
+00025ed0: 2020 2020 2061 6374 696f 6e3a 2072 6570       action: rep
+00025ee0: 6c61 6365 0a20 2020 2020 2020 2020 2073  lace.          s
+00025ef0: 6570 6172 6174 6f72 3a20 3b0a 2020 2020  eparator: ;.    
+00025f00: 2020 2020 2020 7265 706c 6163 656d 656e        replacemen
+00025f10: 743a 2024 310a 2020 2020 2020 2020 2020  t: $1.          
+00025f20: 7461 7267 6574 5f6c 6162 656c 3a20 5f5f  target_label: __
+00025f30: 6d65 7472 6963 735f 7061 7468 5f5f 0a20  metrics_path__. 
+00025f40: 2020 2020 2020 2073 6368 656d 653a 2068         scheme: h
+00025f50: 7474 700a 2020 2020 2020 2020 706f 7274  ttp.        port
+00025f60: 3a20 3830 3830 0a20 2020 2020 2020 2068  : 8080.        h
+00025f70: 6f6e 6f72 5f74 696d 6573 7461 6d70 733a  onor_timestamps:
+00025f80: 2074 7275 650a 2020 2020 2020 2020 7363   true.        sc
+00025f90: 7261 7065 5f74 696d 656f 7574 3a20 3130  rape_timeout: 10
+00025fa0: 730a 2020 2020 2020 2020 696e 7465 7276  s.        interv
+00025fb0: 616c 3a20 3330 730a 2020 2020 2020 2020  al: 30s.        
+00025fc0: 7061 7261 6d73 3a0a 2020 2020 2020 2020  params:.        
+00025fd0: 2020 6d6f 6475 6c65 3a0a 2020 2020 2020    module:.      
+00025fe0: 2020 2020 2d20 6874 7470 5f32 7878 0a20      - http_2xx. 
+00025ff0: 2020 2020 2070 726f 7065 7274 6965 733a       properties:
+00026000: 0a20 2020 2020 2020 2068 6f6e 6f72 5f6c  .        honor_l
+00026010: 6162 656c 733a 0a20 2020 2020 2020 2020  abels:.         
+00026020: 2064 6573 6372 6970 7469 6f6e 3a20 686f   description: ho
+00026030: 6e6f 724c 6162 656c 7320 6368 6f6f 7365  norLabels choose
+00026040: 7320 7468 6520 6d65 7472 6963 2773 206c  s the metric's l
+00026050: 6162 656c 7320 6f6e 2063 6f6c 6c69 7369  abels on collisi
+00026060: 6f6e 7320 7769 7468 0a20 2020 2020 2020  ons with.       
+00026070: 2020 2020 2074 6172 6765 7420 6c61 6265       target labe
+00026080: 6c73 2e0a 2020 2020 2020 2020 2020 6578  ls..          ex
+00026090: 616d 706c 653a 2074 7275 650a 2020 2020  ample: true.    
+000260a0: 2020 2020 2020 7469 746c 653a 2068 6f6e        title: hon
+000260b0: 6f72 5f6c 6162 656c 730a 2020 2020 2020  or_labels.      
+000260c0: 2020 2020 7479 7065 3a20 626f 6f6c 6561      type: boolea
+000260d0: 6e0a 2020 2020 2020 2020 696e 7465 7276  n.        interv
+000260e0: 616c 3a0a 2020 2020 2020 2020 2020 6465  al:.          de
+000260f0: 7363 7269 7074 696f 6e3a 2049 6e74 6572  scription: Inter
+00026100: 7661 6c20 6174 2077 6869 6368 206d 6574  val at which met
+00026110: 7269 6373 2073 686f 756c 6420 6265 2073  rics should be s
+00026120: 6372 6170 6564 0a20 2020 2020 2020 2020  craped.         
+00026130: 2065 7861 6d70 6c65 3a20 3330 730a 2020   example: 30s.  
+00026140: 2020 2020 2020 2020 7469 746c 653a 2069          title: i
+00026150: 6e74 6572 7661 6c0a 2020 2020 2020 2020  nterval.        
+00026160: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+00026170: 2020 2020 2020 2073 6372 6170 655f 7469         scrape_ti
+00026180: 6d65 6f75 743a 0a20 2020 2020 2020 2020  meout:.         
+00026190: 2064 6573 6372 6970 7469 6f6e 3a20 5469   description: Ti
+000261a0: 6d65 6f75 7420 6166 7465 7220 7768 6963  meout after whic
+000261b0: 6820 7468 6520 7363 7261 7065 2069 7320  h the scrape is 
+000261c0: 656e 6465 640a 2020 2020 2020 2020 2020  ended.          
+000261d0: 6578 616d 706c 653a 2031 3073 0a20 2020  example: 10s.   
+000261e0: 2020 2020 2020 2074 6974 6c65 3a20 7363         title: sc
+000261f0: 7261 7065 5f74 696d 656f 7574 0a20 2020  rape_timeout.   
+00026200: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+00026210: 696e 670a 2020 2020 2020 2020 7061 7468  ing.        path
+00026220: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
+00026230: 7269 7074 696f 6e3a 2048 5454 5020 7061  ription: HTTP pa
+00026240: 7468 2074 6f20 7363 7261 7065 2066 6f72  th to scrape for
+00026250: 206d 6574 7269 6373 2e0a 2020 2020 2020   metrics..      
+00026260: 2020 2020 6578 616d 706c 653a 202f 6d65      example: /me
+00026270: 7472 6963 730a 2020 2020 2020 2020 2020  trics.          
+00026280: 7469 746c 653a 2070 6174 680a 2020 2020  title: path.    
+00026290: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+000262a0: 6e67 0a20 2020 2020 2020 2073 6368 656d  ng.        schem
+000262b0: 653a 0a20 2020 2020 2020 2020 2064 6573  e:.          des
+000262c0: 6372 6970 7469 6f6e 3a20 4854 5450 2073  cription: HTTP s
+000262d0: 6368 656d 6520 746f 2075 7365 2066 6f72  cheme to use for
+000262e0: 2073 6372 6170 696e 672e 0a20 2020 2020   scraping..     
+000262f0: 2020 2020 2065 7861 6d70 6c65 3a20 6874       example: ht
+00026300: 7470 0a20 2020 2020 2020 2020 2074 6974  tp.          tit
+00026310: 6c65 3a20 7363 6865 6d65 0a20 2020 2020  le: scheme.     
+00026320: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+00026330: 670a 2020 2020 2020 2020 7461 7267 6574  g.        target
+00026340: 5f70 6f72 743a 0a20 2020 2020 2020 2020  _port:.         
+00026350: 2064 6573 6372 6970 7469 6f6e 3a20 224e   description: "N
+00026360: 756d 6265 7220 6f66 2074 6865 2074 6172  umber of the tar
+00026370: 6765 7420 706f 7274 206f 6620 7468 6520  get port of the 
+00026380: 506f 6420 6265 6869 6e64 2074 6865 2053  Pod behind the S
+00026390: 6572 7669 6365 2c20 7468 655c 0a20 2020  ervice, the\.   
+000263a0: 2020 2020 2020 2020 205c 2070 6f72 7420           \ port 
+000263b0: 6d75 7374 2062 6520 7370 6563 6966 6965  must be specifie
+000263c0: 6420 7769 7468 2063 6f6e 7461 696e 6572  d with container
+000263d0: 2070 6f72 7420 7072 6f70 6572 7479 2e20   port property. 
+000263e0: 4d75 7475 616c 6c79 2065 7863 6c75 7369  Mutually exclusi
+000263f0: 7665 5c0a 2020 2020 2020 2020 2020 2020  ve\.            
+00026400: 5c20 7769 7468 2070 6f72 742e 220a 2020  \ with port.".  
+00026410: 2020 2020 2020 2020 6578 616d 706c 653a          example:
+00026420: 2038 3038 300a 2020 2020 2020 2020 2020   8080.          
+00026430: 7469 746c 653a 2074 6172 6765 745f 706f  title: target_po
+00026440: 7274 0a20 2020 2020 2020 2020 2074 7970  rt.          typ
+00026450: 653a 2069 6e74 6567 6572 0a20 2020 2020  e: integer.     
+00026460: 2020 2070 6172 616d 733a 0a20 2020 2020     params:.     
+00026470: 2020 2020 2061 6464 6974 696f 6e61 6c50       additionalP
+00026480: 726f 7065 7274 6965 733a 0a20 2020 2020  roperties:.     
+00026490: 2020 2020 2020 2069 7465 6d73 3a0a 2020         items:.  
+000264a0: 2020 2020 2020 2020 2020 2020 7479 7065              type
+000264b0: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+000264c0: 2020 2020 2074 7970 653a 2061 7272 6179       type: array
+000264d0: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
+000264e0: 6970 7469 6f6e 3a20 5061 7261 6d73 2069  iption: Params i
+000264f0: 7320 6120 7365 7420 6f66 2055 524c 2070  s a set of URL p
+00026500: 6172 616d 6574 6572 7320 746f 2062 6520  arameters to be 
+00026510: 6170 7065 6e64 6564 2074 6f20 7468 6520  appended to the 
+00026520: 7363 7261 7065 0a20 2020 2020 2020 2020  scrape.         
+00026530: 2020 2055 524c 2062 6566 6f72 6520 7363     URL before sc
+00026540: 7261 7069 6e67 2e0a 2020 2020 2020 2020  raping..        
+00026550: 2020 6578 616d 706c 653a 0a20 2020 2020    example:.     
+00026560: 2020 2020 2020 206d 6f64 756c 653a 0a20         module:. 
+00026570: 2020 2020 2020 2020 2020 202d 2068 7474             - htt
+00026580: 705f 3278 780a 2020 2020 2020 2020 2020  p_2xx.          
+00026590: 7469 746c 653a 2070 6172 616d 730a 2020  title: params.  
+000265a0: 2020 2020 2020 2020 7479 7065 3a20 6f62          type: ob
+000265b0: 6a65 6374 0a20 2020 2020 2020 2072 656c  ject.        rel
+000265c0: 6162 656c 696e 6773 3a0a 2020 2020 2020  abelings:.      
+000265d0: 2020 2020 6974 656d 733a 0a20 2020 2020      items:.     
+000265e0: 2020 2020 2020 2024 7265 663a 2027 232f         $ref: '#/
+000265f0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00026600: 6173 2f52 656c 6162 656c 436f 6e66 6967  as/RelabelConfig
+00026610: 270a 2020 2020 2020 2020 2020 7469 746c  '.          titl
+00026620: 653a 2072 656c 6162 656c 696e 6773 0a20  e: relabelings. 
+00026630: 2020 2020 2020 2020 2074 7970 653a 2061           type: a
+00026640: 7272 6179 0a20 2020 2020 2020 2070 6f72  rray.        por
+00026650: 743a 0a20 2020 2020 2020 2020 2064 6573  t:.          des
+00026660: 6372 6970 7469 6f6e 3a20 4e61 6d65 206f  cription: Name o
+00026670: 6620 7468 6520 7365 7276 6963 6520 706f  f the service po
+00026680: 7274 2074 6869 7320 656e 6470 6f69 6e74  rt this endpoint
+00026690: 2072 6566 6572 7320 746f 2e20 4d75 7475   refers to. Mutu
+000266a0: 616c 6c79 0a20 2020 2020 2020 2020 2020  ally.           
+000266b0: 2065 7863 6c75 7369 7665 2077 6974 6820   exclusive with 
+000266c0: 7461 7267 6574 506f 7274 2e0a 2020 2020  targetPort..    
+000266d0: 2020 2020 2020 6578 616d 706c 653a 2038        example: 8
+000266e0: 3038 300a 2020 2020 2020 2020 2020 7469  080.          ti
+000266f0: 746c 653a 2070 6f72 740a 2020 2020 2020  tle: port.      
+00026700: 2020 2020 7479 7065 3a20 696e 7465 6765      type: intege
+00026710: 720a 2020 2020 2020 2020 686f 6e6f 725f  r.        honor_
+00026720: 7469 6d65 7374 616d 7073 3a0a 2020 2020  timestamps:.    
+00026730: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00026740: 6e3a 2068 6f6e 6f72 5469 6d65 7374 616d  n: honorTimestam
+00026750: 7073 2063 6f6e 7472 6f6c 7320 7768 6574  ps controls whet
+00026760: 6865 7220 5072 6f6d 6574 6865 7573 2072  her Prometheus r
+00026770: 6573 7065 6374 7320 7468 6520 7469 6d65  espects the time
+00026780: 7374 616d 7073 0a20 2020 2020 2020 2020  stamps.         
+00026790: 2020 2070 7265 7365 6e74 2069 6e20 7363     present in sc
+000267a0: 7261 7065 6420 6461 7461 2e0a 2020 2020  raped data..    
+000267b0: 2020 2020 2020 6578 616d 706c 653a 2074        example: t
+000267c0: 7275 650a 2020 2020 2020 2020 2020 7469  rue.          ti
+000267d0: 746c 653a 2068 6f6e 6f72 5f74 696d 6573  tle: honor_times
+000267e0: 7461 6d70 730a 2020 2020 2020 2020 2020  tamps.          
+000267f0: 7479 7065 3a20 626f 6f6c 6561 6e0a 2020  type: boolean.  
+00026800: 2020 2020 2020 6d65 7472 6963 5f72 656c        metric_rel
+00026810: 6162 656c 696e 6773 3a0a 2020 2020 2020  abelings:.      
+00026820: 2020 2020 6974 656d 733a 0a20 2020 2020      items:.     
+00026830: 2020 2020 2020 2024 7265 663a 2027 232f         $ref: '#/
+00026840: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00026850: 6173 2f52 656c 6162 656c 436f 6e66 6967  as/RelabelConfig
+00026860: 270a 2020 2020 2020 2020 2020 7469 746c  '.          titl
+00026870: 653a 206d 6574 7269 635f 7265 6c61 6265  e: metric_relabe
+00026880: 6c69 6e67 730a 2020 2020 2020 2020 2020  lings.          
+00026890: 7479 7065 3a20 6172 7261 790a 2020 2020  type: array.    
+000268a0: 2020 7469 746c 653a 2045 6e64 706f 696e    title: Endpoin
+000268b0: 740a 2020 2020 2020 7479 7065 3a20 6f62  t.      type: ob
+000268c0: 6a65 6374 0a20 2020 2052 656c 6162 656c  ject.    Relabel
+000268d0: 436f 6e66 6967 3a0a 2020 2020 2020 6578  Config:.      ex
+000268e0: 616d 706c 653a 0a20 2020 2020 2020 2072  ample:.        r
+000268f0: 6567 6578 3a20 282e 2a29 0a20 2020 2020  egex: (.*).     
+00026900: 2020 2073 6f75 7263 655f 6c61 6265 6c73     source_labels
+00026910: 3a0a 2020 2020 2020 2020 2d20 5f5f 6d65  :.        - __me
+00026920: 7461 5f6b 7562 6572 6e65 7465 735f 706f  ta_kubernetes_po
+00026930: 645f 6c61 6265 6c5f 6170 705f 6b75 6265  d_label_app_kube
+00026940: 726e 6574 6573 5f69 6f5f 6e61 6d65 0a20  rnetes_io_name. 
+00026950: 2020 2020 2020 2061 6374 696f 6e3a 2072         action: r
+00026960: 6570 6c61 6365 0a20 2020 2020 2020 2073  eplace.        s
+00026970: 6570 6172 6174 6f72 3a20 3b0a 2020 2020  eparator: ;.    
+00026980: 2020 2020 7265 706c 6163 656d 656e 743a      replacement:
+00026990: 2024 310a 2020 2020 2020 2020 7461 7267   $1.        targ
+000269a0: 6574 5f6c 6162 656c 3a20 5f5f 6d65 7472  et_label: __metr
+000269b0: 6963 735f 7061 7468 5f5f 0a20 2020 2020  ics_path__.     
+000269c0: 2070 726f 7065 7274 6965 733a 0a20 2020   properties:.   
+000269d0: 2020 2020 2073 6f75 7263 655f 6c61 6265       source_labe
+000269e0: 6c73 3a0a 2020 2020 2020 2020 2020 6465  ls:.          de
+000269f0: 7363 7269 7074 696f 6e3a 2053 6f75 7263  scription: Sourc
+00026a00: 654c 6162 656c 7320 7365 6c65 6374 7320  eLabels selects 
+00026a10: 6c61 6265 6c73 2066 726f 6d20 7468 6520  labels from the 
+00026a20: 736f 7572 6365 0a20 2020 2020 2020 2020  source.         
+00026a30: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
+00026a40: 2020 2020 2d20 5f5f 6d65 7461 5f6b 7562      - __meta_kub
+00026a50: 6572 6e65 7465 735f 706f 645f 6c61 6265  ernetes_pod_labe
+00026a60: 6c5f 6170 705f 6b75 6265 726e 6574 6573  l_app_kubernetes
+00026a70: 5f69 6f5f 6e61 6d65 0a20 2020 2020 2020  _io_name.       
+00026a80: 2020 2069 7465 6d73 3a0a 2020 2020 2020     items:.      
+00026a90: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+00026aa0: 6e67 0a20 2020 2020 2020 2020 2074 6974  ng.          tit
+00026ab0: 6c65 3a20 736f 7572 6365 5f6c 6162 656c  le: source_label
+00026ac0: 730a 2020 2020 2020 2020 2020 7479 7065  s.          type
+00026ad0: 3a20 6172 7261 790a 2020 2020 2020 2020  : array.        
+00026ae0: 7365 7061 7261 746f 723a 0a20 2020 2020  separator:.     
+00026af0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00026b00: 3a20 5365 7061 7261 746f 7220 706c 6163  : Separator plac
+00026b10: 6564 2062 6574 7765 656e 2063 6f6e 6361  ed between conca
+00026b20: 7465 6e61 7465 6420 736f 7572 6365 206c  tenated source l
+00026b30: 6162 656c 732e 0a20 2020 2020 2020 2020  abels..         
+00026b40: 2065 7861 6d70 6c65 3a20 3b0a 2020 2020   example: ;.    
+00026b50: 2020 2020 2020 7469 746c 653a 2073 6570        title: sep
+00026b60: 6172 6174 6f72 0a20 2020 2020 2020 2020  arator.         
+00026b70: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
+00026b80: 2020 2020 2020 7265 6765 783a 0a20 2020        regex:.   
+00026b90: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00026ba0: 6f6e 3a20 5265 6775 6c61 7220 6578 7072  on: Regular expr
+00026bb0: 6573 7369 6f6e 2061 6761 696e 7374 2077  ession against w
+00026bc0: 6869 6368 2074 6865 2065 7874 7261 6374  hich the extract
+00026bd0: 6564 2076 616c 7565 2069 7320 6d61 7463  ed value is matc
+00026be0: 6865 642e 0a20 2020 2020 2020 2020 2020  hed..           
+00026bf0: 2044 6566 6175 6c74 2069 7320 282e 2a29   Default is (.*)
+00026c00: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
+00026c10: 6c65 3a20 282e 2a29 0a20 2020 2020 2020  le: (.*).       
+00026c20: 2020 2074 6974 6c65 3a20 7265 6765 780a     title: regex.
+00026c30: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
+00026c40: 7374 7269 6e67 0a20 2020 2020 2020 2072  string.        r
+00026c50: 6570 6c61 6365 6d65 6e74 3a0a 2020 2020  eplacement:.    
+00026c60: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00026c70: 6e3a 2052 6570 6c61 6365 6d65 6e74 2076  n: Replacement v
+00026c80: 616c 7565 2061 6761 696e 7374 2077 6869  alue against whi
+00026c90: 6368 2061 2072 6567 6578 2072 6570 6c61  ch a regex repla
+00026ca0: 6365 2069 7320 7065 7266 6f72 6d65 640a  ce is performed.
+00026cb0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00026cc0: 6865 2072 6567 756c 6172 2065 7870 7265  he regular expre
+00026cd0: 7373 696f 6e20 6d61 7463 6865 732e 2052  ssion matches. R
+00026ce0: 6567 6578 2063 6170 7475 7265 2067 726f  egex capture gro
+00026cf0: 7570 7320 6172 6520 6176 6169 6c61 626c  ups are availabl
+00026d00: 652e 0a20 2020 2020 2020 2020 2065 7861  e..          exa
+00026d10: 6d70 6c65 3a20 2431 0a20 2020 2020 2020  mple: $1.       
+00026d20: 2020 2074 6974 6c65 3a20 7265 706c 6163     title: replac
+00026d30: 656d 656e 740a 2020 2020 2020 2020 2020  ement.          
+00026d40: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+00026d50: 2020 2020 2074 6172 6765 745f 6c61 6265       target_labe
+00026d60: 6c3a 0a20 2020 2020 2020 2020 2064 6573  l:.          des
+00026d70: 6372 6970 7469 6f6e 3a20 4c61 6265 6c20  cription: Label 
+00026d80: 746f 2077 6869 6368 2074 6865 2072 6573  to which the res
+00026d90: 756c 7469 6e67 2076 616c 7565 2069 7320  ulting value is 
+00026da0: 7772 6974 7465 6e20 696e 2061 2072 6570  written in a rep
+00026db0: 6c61 6365 0a20 2020 2020 2020 2020 2020  lace.           
+00026dc0: 2061 6374 696f 6e2e 0a20 2020 2020 2020   action..       
+00026dd0: 2020 2065 7861 6d70 6c65 3a20 5f5f 6d65     example: __me
+00026de0: 7472 6963 735f 7061 7468 5f5f 0a20 2020  trics_path__.   
+00026df0: 2020 2020 2020 2074 6974 6c65 3a20 7461         title: ta
+00026e00: 7267 6574 5f6c 6162 656c 0a20 2020 2020  rget_label.     
+00026e10: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+00026e20: 670a 2020 2020 2020 2020 6163 7469 6f6e  g.        action
+00026e30: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
+00026e40: 7269 7074 696f 6e3a 2041 6374 696f 6e20  ription: Action 
+00026e50: 746f 2070 6572 666f 726d 2062 6173 6564  to perform based
+00026e60: 206f 6e20 7265 6765 7820 6d61 7463 6869   on regex matchi
+00026e70: 6e67 2e0a 2020 2020 2020 2020 2020 6578  ng..          ex
+00026e80: 616d 706c 653a 2072 6570 6c61 6365 0a20  ample: replace. 
+00026e90: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
+00026ea0: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
+00026eb0: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
+00026ec0: 2020 2020 7469 746c 653a 2052 656c 6162      title: Relab
+00026ed0: 656c 436f 6e66 6967 0a20 2020 2020 2074  elConfig.      t
+00026ee0: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
+00026ef0: 4465 706c 6f79 5265 736f 7572 6365 4f76  DeployResourceOv
+00026f00: 6572 6c61 7973 3a0a 2020 2020 2020 6164  erlays:.      ad
+00026f10: 6469 7469 6f6e 616c 5072 6f70 6572 7469  ditionalProperti
+00026f20: 6573 3a0a 2020 2020 2020 2020 2472 6566  es:.        $ref
+00026f30: 3a20 2723 2f63 6f6d 706f 6e65 6e74 732f  : '#/components/
+00026f40: 7363 6865 6d61 732f 4465 706c 6f79 5265  schemas/DeployRe
+00026f50: 736f 7572 6365 7327 0a20 2020 2020 2074  sources'.      t
+00026f60: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
+00026f70: 4465 706c 6f79 506c 6174 666f 726d 5265  DeployPlatformRe
+00026f80: 736f 7572 6365 733a 0a20 2020 2020 2069  sources:.      i
+00026f90: 7465 6d73 3a0a 2020 2020 2020 2020 2472  tems:.        $r
+00026fa0: 6566 3a20 2723 2f63 6f6d 706f 6e65 6e74  ef: '#/component
+00026fb0: 732f 7363 6865 6d61 732f 4465 706c 6f79  s/schemas/Deploy
+00026fc0: 506c 6174 666f 726d 5265 736f 7572 6365  PlatformResource
+00026fd0: 270a 2020 2020 2020 7479 7065 3a20 6172  '.      type: ar
+00026fe0: 7261 790a 2020 2020 4465 706c 6f79 506c  ray.    DeployPl
+00026ff0: 6174 666f 726d 5265 736f 7572 6365 3a0a  atformResource:.
+00027000: 2020 2020 2020 6578 616d 706c 653a 0a20        example:. 
+00027010: 2020 2020 2020 2070 6f70 3a20 616d 7331         pop: ams1
+00027020: 0a20 2020 2020 2020 2063 7075 5f72 6571  .        cpu_req
+00027030: 7565 7374 6564 3a20 3130 3030 0a20 2020  uested: 1000.   
+00027040: 2020 2020 2063 7075 5f75 7365 643a 2035       cpu_used: 5
+00027050: 3030 0a20 2020 2020 2020 2063 7075 5f6c  00.        cpu_l
+00027060: 696d 6974 3a20 3230 3030 0a20 2020 2020  imit: 2000.     
+00027070: 2020 206d 656d 6f72 795f 7573 6564 3a20     memory_used: 
+00027080: 3530 3030 0a20 2020 2020 2020 206d 656d  5000.        mem
+00027090: 6f72 795f 7265 7175 6573 7465 643a 2031  ory_requested: 1
+000270a0: 3030 3030 0a20 2020 2020 2020 2070 6c61  0000.        pla
+000270b0: 7466 6f72 6d3a 2042 4745 0a20 2020 2020  tform: BGE.     
+000270c0: 2020 2073 7061 6365 3a20 6773 730a 2020     space: gss.  
+000270d0: 2020 2020 2020 7374 6f72 6167 655f 7265        storage_re
+000270e0: 7175 6573 7465 643a 2031 300a 2020 2020  quested: 10.    
+000270f0: 2020 2020 7374 6f72 6167 655f 7573 6564      storage_used
+00027100: 3a20 350a 2020 2020 2020 7072 6f70 6572  : 5.      proper
+00027110: 7469 6573 3a0a 2020 2020 2020 2020 706c  ties:.        pl
+00027120: 6174 666f 726d 3a0a 2020 2020 2020 2020  atform:.        
+00027130: 2020 6465 7363 7269 7074 696f 6e3a 204e    description: N
+00027140: 616d 6520 6f66 2074 6865 2064 6570 6c6f  ame of the deplo
+00027150: 7920 706c 6174 666f 726d 2e0a 2020 2020  y platform..    
+00027160: 2020 2020 2020 6578 616d 706c 653a 2042        example: B
+00027170: 4745 0a20 2020 2020 2020 2020 2074 6974  GE.          tit
+00027180: 6c65 3a20 706c 6174 666f 726d 0a20 2020  le: platform.   
+00027190: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+000271a0: 696e 670a 2020 2020 2020 2020 706f 703a  ing.        pop:
+000271b0: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
+000271c0: 6970 7469 6f6e 3a20 4e61 6d65 206f 6620  iption: Name of 
+000271d0: 7468 6520 706f 702e 0a20 2020 2020 2020  the pop..       
+000271e0: 2020 2065 7861 6d70 6c65 3a20 616d 7331     example: ams1
+000271f0: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
+00027200: 3a20 706f 700a 2020 2020 2020 2020 2020  : pop.          
+00027210: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+00027220: 2020 2020 2073 7061 6365 3a0a 2020 2020       space:.    
+00027230: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00027240: 6e3a 204e 616d 6520 6f66 2074 6865 2064  n: Name of the d
+00027250: 6570 6c6f 7920 7370 6163 652e 0a20 2020  eploy space..   
+00027260: 2020 2020 2020 2065 7861 6d70 6c65 3a20         example: 
+00027270: 6773 730a 2020 2020 2020 2020 2020 7469  gss.          ti
+00027280: 746c 653a 2073 7061 6365 0a20 2020 2020  tle: space.     
+00027290: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+000272a0: 670a 2020 2020 2020 2020 6370 755f 7265  g.        cpu_re
+000272b0: 7175 6573 7465 643a 0a20 2020 2020 2020  quested:.       
+000272c0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+000272d0: 2254 6865 2043 5055 2051 756f 7461 2072  "The CPU Quota r
+000272e0: 6571 7565 7374 6564 2066 6f72 2074 6865  equested for the
+000272f0: 2064 6570 6c6f 7920 7370 6163 652e 2054   deploy space. T
+00027300: 6865 2075 6e69 7420 6973 5c0a 2020 2020  he unit is\.    
+00027310: 2020 2020 2020 2020 5c20 6d69 6c69 6370          \ milicp
+00027320: 752c 2031 2063 6f72 6520 6571 7561 6c73  u, 1 core equals
+00027330: 2031 3030 302e 220a 2020 2020 2020 2020   1000.".        
+00027340: 2020 6578 616d 706c 653a 2031 3030 300a    example: 1000.
+00027350: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+00027360: 2063 7075 5f72 6571 7565 7374 6564 0a20   cpu_requested. 
+00027370: 2020 2020 2020 2020 2074 7970 653a 2069           type: i
+00027380: 6e74 6567 6572 0a20 2020 2020 2020 2063  nteger.        c
+00027390: 7075 5f6c 696d 6974 3a0a 2020 2020 2020  pu_limit:.      
+000273a0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+000273b0: 2022 5468 6520 6d61 7820 706f 7373 6962   "The max possib
+000273c0: 6c79 2043 5055 2074 6861 7420 6361 6e20  ly CPU that can 
+000273d0: 6265 2075 7469 6c69 7a65 6420 6279 2074  be utilized by t
+000273e0: 6865 2064 6570 6c6f 7920 7370 6163 652e  he deploy space.
+000273f0: 5c0a 2020 2020 2020 2020 2020 2020 5c20  \.            \ 
+00027400: 5468 6520 756e 6974 2069 7320 6d69 6c69  The unit is mili
+00027410: 6370 752c 2031 2063 6f72 6520 6571 7561  cpu, 1 core equa
+00027420: 6c73 2031 3030 302e 220a 2020 2020 2020  ls 1000.".      
+00027430: 2020 2020 6578 616d 706c 653a 2032 3030      example: 200
+00027440: 300a 2020 2020 2020 2020 2020 7469 746c  0.          titl
+00027450: 653a 2063 7075 5f6c 696d 6974 0a20 2020  e: cpu_limit.   
+00027460: 2020 2020 2020 2074 7970 653a 2069 6e74         type: int
+00027470: 6567 6572 0a20 2020 2020 2020 2063 7075  eger.        cpu
+00027480: 5f75 7365 643a 0a20 2020 2020 2020 2020  _used:.         
+00027490: 2064 6573 6372 6970 7469 6f6e 3a20 2254   description: "T
+000274a0: 6865 2043 5055 2061 6d6f 756e 7420 7573  he CPU amount us
+000274b0: 6564 2069 6e20 7468 6520 6465 706c 6f79  ed in the deploy
+000274c0: 2073 7061 6365 2e20 5468 6520 756e 6974   space. The unit
+000274d0: 2069 7320 6d69 6c69 6370 752c 5c0a 2020   is milicpu,\.  
+000274e0: 2020 2020 2020 2020 2020 5c20 3120 636f            \ 1 co
+000274f0: 7265 2065 7175 616c 7320 3130 3030 2e22  re equals 1000."
+00027500: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
+00027510: 6c65 3a20 3530 300a 2020 2020 2020 2020  le: 500.        
+00027520: 2020 7469 746c 653a 2063 7075 5f75 7365    title: cpu_use
+00027530: 640a 2020 2020 2020 2020 2020 7479 7065  d.          type
+00027540: 3a20 696e 7465 6765 720a 2020 2020 2020  : integer.      
+00027550: 2020 6d65 6d6f 7279 5f72 6571 7565 7374    memory_request
+00027560: 6564 3a0a 2020 2020 2020 2020 2020 6465  ed:.          de
+00027570: 7363 7269 7074 696f 6e3a 2054 6865 206d  scription: The m
+00027580: 656d 6f72 7920 5175 6f74 6120 7265 7175  emory Quota requ
+00027590: 6573 7465 6420 666f 7220 7468 6520 6465  ested for the de
+000275a0: 706c 6f79 2073 7061 6365 2e20 5468 6520  ploy space. The 
+000275b0: 756e 6974 2069 730a 2020 2020 2020 2020  unit is.        
+000275c0: 2020 2020 4d42 2e0a 2020 2020 2020 2020      MB..        
+000275d0: 2020 6578 616d 706c 653a 2031 3030 3030    example: 10000
+000275e0: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
+000275f0: 3a20 6d65 6d6f 7279 5f72 6571 7565 7374  : memory_request
+00027600: 6564 0a20 2020 2020 2020 2020 2074 7970  ed.          typ
+00027610: 653a 2069 6e74 6567 6572 0a20 2020 2020  e: integer.     
+00027620: 2020 206d 656d 6f72 795f 7573 6564 3a0a     memory_used:.
+00027630: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00027640: 7074 696f 6e3a 2054 6865 206d 656d 6f72  ption: The memor
+00027650: 7920 616d 6f75 6e74 2075 7365 6420 696e  y amount used in
+00027660: 2074 6865 2064 6570 6c6f 7920 7370 6163   the deploy spac
+00027670: 652e 2054 6865 2075 6e69 7420 6973 204d  e. The unit is M
+00027680: 422e 0a20 2020 2020 2020 2020 2065 7861  B..          exa
+00027690: 6d70 6c65 3a20 3530 3030 0a20 2020 2020  mple: 5000.     
+000276a0: 2020 2020 2074 6974 6c65 3a20 6d65 6d6f       title: memo
+000276b0: 7279 5f75 7365 640a 2020 2020 2020 2020  ry_used.        
+000276c0: 2020 7479 7065 3a20 696e 7465 6765 720a    type: integer.
+000276d0: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
+000276e0: 7265 7175 6573 7465 643a 0a20 2020 2020  requested:.     
+000276f0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00027700: 3a20 5468 6520 7374 6f72 6167 6520 5175  : The storage Qu
+00027710: 6f74 6120 7265 7175 6573 7465 6420 666f  ota requested fo
+00027720: 7220 7468 6520 6465 706c 6f79 2073 7061  r the deploy spa
+00027730: 6365 2e20 5468 6520 756e 6974 0a20 2020  ce. The unit.   
+00027740: 2020 2020 2020 2020 2069 7320 4742 2e0a           is GB..
+00027750: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
+00027760: 653a 2031 300a 2020 2020 2020 2020 2020  e: 10.          
+00027770: 7469 746c 653a 2073 746f 7261 6765 5f72  title: storage_r
+00027780: 6571 7565 7374 6564 0a20 2020 2020 2020  equested.       
+00027790: 2020 2074 7970 653a 2069 6e74 6567 6572     type: integer
+000277a0: 0a20 2020 2020 2020 2073 746f 7261 6765  .        storage
+000277b0: 5f75 7365 643a 0a20 2020 2020 2020 2020  _used:.         
+000277c0: 2064 6573 6372 6970 7469 6f6e 3a20 5468   description: Th
+000277d0: 6520 7374 6f72 6167 6520 616d 6f75 6e74  e storage amount
+000277e0: 2075 7365 6420 696e 2074 6865 2064 6570   used in the dep
+000277f0: 6c6f 7920 7370 6163 652e 2054 6865 2075  loy space. The u
+00027800: 6e69 7420 6973 204d 422e 0a20 2020 2020  nit is MB..     
+00027810: 2020 2020 2065 7861 6d70 6c65 3a20 350a       example: 5.
+00027820: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+00027830: 2073 746f 7261 6765 5f75 7365 640a 2020   storage_used.  
+00027840: 2020 2020 2020 2020 7479 7065 3a20 696e          type: in
+00027850: 7465 6765 720a 2020 2020 2020 7469 746c  teger.      titl
+00027860: 653a 2044 6570 6c6f 7950 6c61 7466 6f72  e: DeployPlatfor
+00027870: 6d52 6573 6f75 7263 650a 2020 2020 2020  mResource.      
+00027880: 7479 7065 3a20 6f62 6a65 6374 0a20 2020  type: object.   
+00027890: 2055 7064 6174 6553 7472 6174 6567 795f   UpdateStrategy_
+000278a0: 726f 6c6c 696e 675f 7570 6461 7465 5f63  rolling_update_c
+000278b0: 6f6e 6669 673a 0a20 2020 2020 2065 7861  onfig:.      exa
+000278c0: 6d70 6c65 3a0a 2020 2020 2020 2020 7061  mple:.        pa
+000278d0: 7274 6974 696f 6e3a 2032 0a20 2020 2020  rtition: 2.     
+000278e0: 2020 206d 6178 5f75 6e61 7661 696c 6162     max_unavailab
+000278f0: 6c65 3a20 3130 2520 6f72 2032 0a20 2020  le: 10% or 2.   
+00027900: 2020 2020 206d 6178 5f73 7572 6765 3a20       max_surge: 
+00027910: 3130 2520 6f72 2032 0a20 2020 2020 2070  10% or 2.      p
+00027920: 726f 7065 7274 6965 733a 0a20 2020 2020  roperties:.     
+00027930: 2020 206d 6178 5f73 7572 6765 3a0a 2020     max_surge:.  
+00027940: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00027950: 696f 6e3a 2022 7573 6564 2069 6e20 4465  ion: "used in De
+00027960: 706c 6f79 6d65 6e74 2f44 6165 6d6f 6e53  ployment/DaemonS
+00027970: 6574 3b20 5468 6520 6d61 7869 6d75 6d20  et; The maximum 
+00027980: 6e75 6d62 6572 206f 6620 706f 6473 2074  number of pods t
+00027990: 6861 745c 0a20 2020 2020 2020 2020 2020  hat\.           
+000279a0: 205c 2063 616e 2062 6520 7363 6865 6475   \ can be schedu
+000279b0: 6c65 6420 6162 6f76 6520 7468 6520 6465  led above the de
+000279c0: 7369 7265 6420 6e75 6d62 6572 206f 6620  sired number of 
+000279d0: 706f 6473 2e20 5661 6c75 6520 6361 6e20  pods. Value can 
+000279e0: 6265 2061 6e20 6162 736f 6c75 7465 5c0a  be an absolute\.
+000279f0: 2020 2020 2020 2020 2020 2020 5c20 6e75              \ nu
+00027a00: 6d62 6572 2028 6578 3a20 3529 206f 7220  mber (ex: 5) or 
+00027a10: 6120 7065 7263 656e 7461 6765 206f 6620  a percentage of 
+00027a20: 6465 7369 7265 6420 706f 6473 2028 6578  desired pods (ex
+00027a30: 3a20 3130 2529 2e22 0a20 2020 2020 2020  : 10%).".       
+00027a40: 2020 2065 7861 6d70 6c65 3a20 3130 2520     example: 10% 
+00027a50: 6f72 2032 0a20 2020 2020 2020 2020 2074  or 2.          t
+00027a60: 6974 6c65 3a20 6d61 785f 7375 7267 650a  itle: max_surge.
+00027a70: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
+00027a80: 7374 7269 6e67 0a20 2020 2020 2020 206d  string.        m
+00027a90: 6178 5f75 6e61 7661 696c 6162 6c65 3a0a  ax_unavailable:.
+00027aa0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00027ab0: 7074 696f 6e3a 2022 7573 6564 2069 6e20  ption: "used in 
+00027ac0: 4465 706c 6f79 6d65 6e74 2f44 6165 6d6f  Deployment/Daemo
+00027ad0: 6e53 6574 2f53 7461 7465 6675 6c53 6574  nSet/StatefulSet
+00027ae0: 3b20 5468 6520 6d61 7869 6d75 6d20 6e75  ; The maximum nu
+00027af0: 6d62 6572 5c0a 2020 2020 2020 2020 2020  mber\.          
+00027b00: 2020 5c20 6f66 2070 6f64 7320 7468 6174    \ of pods that
+00027b10: 2063 616e 2062 6520 756e 6176 6169 6c61   can be unavaila
+00027b20: 626c 6520 6475 7269 6e67 2074 6865 2075  ble during the u
+00027b30: 7064 6174 653b 2056 616c 7565 2063 616e  pdate; Value can
+00027b40: 2062 6520 616e 2061 6273 6f6c 7574 655c   be an absolute\
+00027b50: 0a20 2020 2020 2020 2020 2020 205c 206e  .            \ n
+00027b60: 756d 6265 7220 2865 783a 2035 2920 6f72  umber (ex: 5) or
+00027b70: 2061 2070 6572 6365 6e74 6167 6520 6f66   a percentage of
+00027b80: 2064 6573 6972 6564 2070 6f64 7320 2865   desired pods (e
+00027b90: 783a 2031 3025 292e 220a 2020 2020 2020  x: 10%).".      
+00027ba0: 2020 2020 6578 616d 706c 653a 2031 3025      example: 10%
+00027bb0: 206f 7220 320a 2020 2020 2020 2020 2020   or 2.          
+00027bc0: 7469 746c 653a 206d 6178 5f75 6e61 7661  title: max_unava
+00027bd0: 696c 6162 6c65 0a20 2020 2020 2020 2020  ilable.         
+00027be0: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
+00027bf0: 2020 2020 2020 7061 7274 6974 696f 6e3a        partition:
+00027c00: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
+00027c10: 6970 7469 6f6e 3a20 2275 7365 6420 696e  iption: "used in
+00027c20: 2053 7461 7465 6675 6c53 6574 3b20 5061   StatefulSet; Pa
+00027c30: 7274 6974 696f 6e20 696e 6469 6361 7465  rtition indicate
+00027c40: 7320 7468 6520 6f72 6469 6e61 6c20 6174  s the ordinal at
+00027c50: 2077 6869 6368 5c0a 2020 2020 2020 2020   which\.        
+00027c60: 2020 2020 5c20 7468 6520 576f 726b 6c6f      \ the Worklo
+00027c70: 6164 2073 686f 756c 6420 6265 2070 6172  ad should be par
+00027c80: 7469 7469 6f6e 6564 2066 6f72 2075 7064  titioned for upd
+00027c90: 6174 6573 2e20 4475 7269 6e67 2061 2072  ates. During a r
+00027ca0: 6f6c 6c69 6e67 2075 7064 6174 652c 5c0a  olling update,\.
+00027cb0: 2020 2020 2020 2020 2020 2020 5c20 616c              \ al
+00027cc0: 6c20 706f 6473 2066 726f 6d20 6f72 6469  l pods from ordi
+00027cd0: 6e61 6c20 5061 7274 6974 696f 6e2d 3120  nal Partition-1 
+00027ce0: 746f 2052 6570 6c69 6361 2061 7265 2075  to Replica are u
+00027cf0: 7064 6174 6564 2e20 416c 6c20 706f 6473  pdated. All pods
+00027d00: 2066 726f 6d5c 0a20 2020 2020 2020 2020   from\.         
+00027d10: 2020 205c 206f 7264 696e 616c 2050 6172     \ ordinal Par
+00027d20: 7469 7469 6f6e 2d31 2074 6f20 3020 7265  tition-1 to 0 re
+00027d30: 6d61 696e 2075 6e74 6f75 6368 6564 2e20  main untouched. 
+00027d40: 220a 2020 2020 2020 2020 2020 6578 616d  ".          exam
+00027d50: 706c 653a 2032 0a20 2020 2020 2020 2020  ple: 2.         
+00027d60: 2074 6974 6c65 3a20 7061 7274 6974 696f   title: partitio
+00027d70: 6e0a 2020 2020 2020 2020 2020 7479 7065  n.          type
+00027d80: 3a20 696e 7465 6765 720a 2020 2020 2020  : integer.      
+00027d90: 7469 746c 653a 2055 7064 6174 6553 7472  title: UpdateStr
+00027da0: 6174 6567 795f 726f 6c6c 696e 675f 7570  ategy_rolling_up
+00027db0: 6461 7465 5f63 6f6e 6669 670a 2020 2020  date_config.    
+00027dc0: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
+00027dd0: 2020 2043 6f6e 7461 696e 6572 5365 6343     ContainerSecC
+00027de0: 6f6e 7465 7874 5f63 6170 6162 696c 6974  ontext_capabilit
+00027df0: 6965 733a 0a20 2020 2020 2064 6573 6372  ies:.      descr
+00027e00: 6970 7469 6f6e 3a20 5468 6520 504f 5349  iption: The POSI
+00027e10: 5820 6361 7061 6269 6c69 7469 6573 2074  X capabilities t
+00027e20: 6f20 6164 642f 6472 6f70 2077 6865 6e20  o add/drop when 
+00027e30: 7275 6e6e 696e 6720 636f 6e74 6169 6e65  running containe
+00027e40: 7273 2e0a 2020 2020 2020 6578 616d 706c  rs..      exampl
+00027e50: 653a 0a20 2020 2020 2020 2061 6464 3a0a  e:.        add:.
+00027e60: 2020 2020 2020 2020 2d20 4e45 545f 4144          - NET_AD
+00027e70: 4d49 4e0a 2020 2020 2020 2020 2d20 5359  MIN.        - SY
+00027e80: 535f 5449 4d45 0a20 2020 2020 2020 2064  S_TIME.        d
+00027e90: 726f 703a 0a20 2020 2020 2020 202d 204e  rop:.        - N
+00027ea0: 4554 5f41 444d 494e 0a20 2020 2020 2020  ET_ADMIN.       
+00027eb0: 202d 2053 5953 5f54 494d 450a 2020 2020   - SYS_TIME.    
+00027ec0: 2020 7072 6f70 6572 7469 6573 3a0a 2020    properties:.  
+00027ed0: 2020 2020 2020 6164 643a 0a20 2020 2020        add:.     
+00027ee0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00027ef0: 3a20 4164 6465 6420 6361 7061 6269 6c69  : Added capabili
+00027f00: 7469 6573 2e0a 2020 2020 2020 2020 2020  ties..          
+00027f10: 6578 616d 706c 653a 0a20 2020 2020 2020  example:.       
+00027f20: 2020 202d 204e 4554 5f41 444d 494e 0a20     - NET_ADMIN. 
+00027f30: 2020 2020 2020 2020 202d 2053 5953 5f54           - SYS_T
+00027f40: 494d 450a 2020 2020 2020 2020 2020 6974  IME.          it
+00027f50: 656d 733a 0a20 2020 2020 2020 2020 2020  ems:.           
+00027f60: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
+00027f70: 2020 2020 2020 2020 7469 746c 653a 2061          title: a
+00027f80: 6464 0a20 2020 2020 2020 2020 2074 7970  dd.          typ
+00027f90: 653a 2061 7272 6179 0a20 2020 2020 2020  e: array.       
+00027fa0: 2064 726f 703a 0a20 2020 2020 2020 2020   drop:.         
+00027fb0: 2064 6573 6372 6970 7469 6f6e 3a20 5265   description: Re
+00027fc0: 6d6f 7665 6420 6361 7061 6269 6c69 7469  moved capabiliti
+00027fd0: 6573 2e0a 2020 2020 2020 2020 2020 6578  es..          ex
+00027fe0: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
+00027ff0: 202d 204e 4554 5f41 444d 494e 0a20 2020   - NET_ADMIN.   
+00028000: 2020 2020 2020 202d 2053 5953 5f54 494d         - SYS_TIM
+00028010: 450a 2020 2020 2020 2020 2020 6974 656d  E.          item
+00028020: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
+00028030: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
+00028040: 2020 2020 2020 7469 746c 653a 2064 726f        title: dro
+00028050: 700a 2020 2020 2020 2020 2020 7479 7065  p.          type
+00028060: 3a20 6172 7261 790a 2020 2020 2020 7469  : array.      ti
+00028070: 746c 653a 2043 6f6e 7461 696e 6572 5365  tle: ContainerSe
+00028080: 6343 6f6e 7465 7874 5f63 6170 6162 696c  cContext_capabil
+00028090: 6974 6965 730a 2020 2020 2020 7479 7065  ities.      type
+000280a0: 3a20 6f62 6a65 6374 0a20 2020 2056 6f6c  : object.    Vol
+000280b0: 756d 655f 7065 7273 6973 7465 6e74 5f76  ume_persistent_v
+000280c0: 6f6c 756d 655f 636c 6169 6d3a 0a20 2020  olume_claim:.   
+000280d0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+000280e0: 7c0a 2020 2020 2020 2020 5265 7072 6573  |.        Repres
+000280f0: 656e 7473 2061 2072 6566 6572 656e 6365  ents a reference
+00028100: 2074 6f20 6120 5065 7273 6973 7465 6e74   to a Persistent
+00028110: 566f 6c75 6d65 436c 6169 6d20 696e 2074  VolumeClaim in t
+00028120: 6865 2073 616d 6520 6e61 6d65 7370 6163  he same namespac
+00028130: 652e 0a20 2020 2020 2020 2054 6869 7320  e..        This 
+00028140: 766f 6c75 6d65 2066 696e 6473 2074 6865  volume finds the
+00028150: 2062 6f75 6e64 2050 5620 616e 6420 6d6f   bound PV and mo
+00028160: 756e 7473 2074 6861 7420 766f 6c75 6d65  unts that volume
+00028170: 2066 6f72 2074 6865 2070 6f64 2e0a 2020   for the pod..  
+00028180: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
+00028190: 2020 2020 2072 6561 645f 6f6e 6c79 3a20       read_only: 
+000281a0: 6661 6c73 650a 2020 2020 2020 2020 636c  false.        cl
+000281b0: 6169 6d5f 6e61 6d65 3a20 6465 6d6f 2d70  aim_name: demo-p
+000281c0: 7663 0a20 2020 2020 2070 726f 7065 7274  vc.      propert
+000281d0: 6965 733a 0a20 2020 2020 2020 2063 6c61  ies:.        cla
+000281e0: 696d 5f6e 616d 653a 0a20 2020 2020 2020  im_name:.       
+000281f0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+00028200: 436c 6169 6d4e 616d 6520 6973 2074 6865  ClaimName is the
+00028210: 206e 616d 6520 6f66 2061 2050 6572 7369   name of a Persi
+00028220: 7374 656e 7456 6f6c 756d 6543 6c61 696d  stentVolumeClaim
+00028230: 2069 6e20 7468 6520 7361 6d65 0a20 2020   in the same.   
+00028240: 2020 2020 2020 2020 206e 616d 6573 7061           namespa
+00028250: 6365 2061 7320 7468 6520 706f 6420 7573  ce as the pod us
+00028260: 696e 6720 7468 6973 2076 6f6c 756d 650a  ing this volume.
+00028270: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
+00028280: 653a 2064 656d 6f2d 7076 630a 2020 2020  e: demo-pvc.    
+00028290: 2020 2020 2020 7469 746c 653a 2063 6c61        title: cla
+000282a0: 696d 5f6e 616d 650a 2020 2020 2020 2020  im_name.        
+000282b0: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+000282c0: 2020 2020 2020 2072 6561 645f 6f6e 6c79         read_only
+000282d0: 3a0a 2020 2020 2020 2020 2020 6465 7363  :.          desc
+000282e0: 7269 7074 696f 6e3a 2057 696c 6c20 666f  ription: Will fo
+000282f0: 7263 6520 7468 6520 5265 6164 4f6e 6c79  rce the ReadOnly
+00028300: 2073 6574 7469 6e67 2069 6e20 566f 6c75   setting in Volu
+00028310: 6d65 4d6f 756e 7473 0a20 2020 2020 2020  meMounts.       
+00028320: 2020 2065 7861 6d70 6c65 3a20 6661 6c73     example: fals
+00028330: 650a 2020 2020 2020 2020 2020 7469 746c  e.          titl
+00028340: 653a 2072 6561 645f 6f6e 6c79 0a20 2020  e: read_only.   
+00028350: 2020 2020 2020 2074 7970 653a 2062 6f6f         type: boo
+00028360: 6c65 616e 0a20 2020 2020 2074 6974 6c65  lean.      title
+00028370: 3a20 566f 6c75 6d65 5f70 6572 7369 7374  : Volume_persist
+00028380: 656e 745f 766f 6c75 6d65 5f63 6c61 696d  ent_volume_claim
+00028390: 0a20 2020 2020 2074 7970 653a 206f 626a  .      type: obj
+000283a0: 6563 740a 2020 2020 566f 6c75 6d65 5f65  ect.    Volume_e
+000283b0: 6d70 7479 5f64 6972 3a0a 2020 2020 2020  mpty_dir:.      
+000283c0: 6465 7363 7269 7074 696f 6e3a 2052 6570  description: Rep
+000283d0: 7265 7365 6e74 7320 6120 7465 6d70 6f72  resents a tempor
+000283e0: 6172 7920 6469 7265 6374 6f72 7920 7468  ary directory th
+000283f0: 6174 2073 6861 7265 7320 6120 706f 6427  at shares a pod'
+00028400: 7320 6c69 6665 7469 6d65 0a20 2020 2020  s lifetime.     
+00028410: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
+00028420: 2020 6d65 6469 756d 3a20 4d65 6d6f 7279    medium: Memory
+00028430: 0a20 2020 2020 2020 2073 697a 655f 6c69  .        size_li
+00028440: 6d69 743a 2035 3030 4d69 0a20 2020 2020  mit: 500Mi.     
+00028450: 2070 726f 7065 7274 6965 733a 0a20 2020   properties:.   
+00028460: 2020 2020 206d 6564 6975 6d3a 0a20 2020       medium:.   
+00028470: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00028480: 6f6e 3a20 5265 7072 6573 656e 7473 2077  on: Represents w
+00028490: 6861 7420 7479 7065 206f 6620 7374 6f72  hat type of stor
+000284a0: 6167 6520 6d65 6469 756d 2073 686f 756c  age medium shoul
+000284b0: 6420 6261 636b 2074 6869 7320 6469 7265  d back this dire
+000284c0: 6374 6f72 792e 0a20 2020 2020 2020 2020  ctory..         
+000284d0: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
+000284e0: 7320 2222 2077 6869 6368 206d 6561 6e73  s "" which means
+000284f0: 2074 6f20 7573 6520 7468 6520 6e6f 6465   to use the node
+00028500: 2773 2064 6566 6175 6c74 206d 6564 6975  's default mediu
+00028510: 6d2e 0a20 2020 2020 2020 2020 2065 7861  m..          exa
+00028520: 6d70 6c65 3a20 4d65 6d6f 7279 0a20 2020  mple: Memory.   
+00028530: 2020 2020 2020 2074 6974 6c65 3a20 6d65         title: me
+00028540: 6469 756d 0a20 2020 2020 2020 2020 2074  dium.          t
+00028550: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
+00028560: 2020 2020 7369 7a65 5f6c 696d 6974 3a0a      size_limit:.
+00028570: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00028580: 7074 696f 6e3a 2054 6865 2074 6f74 616c  ption: The total
+00028590: 2061 6d6f 756e 7420 6f66 206c 6f63 616c   amount of local
+000285a0: 2073 746f 7261 6765 2072 6571 7569 7265   storage require
+000285b0: 6420 666f 7220 7468 6973 2045 6d70 7479  d for this Empty
+000285c0: 4469 720a 2020 2020 2020 2020 2020 2020  Dir.            
+000285d0: 766f 6c75 6d65 2e0a 2020 2020 2020 2020  volume..        
+000285e0: 2020 6578 616d 706c 653a 2035 3030 4d69    example: 500Mi
+000285f0: 0a20 2020 2020 2020 2020 2074 6974 6c65  .          title
+00028600: 3a20 7369 7a65 5f6c 696d 6974 0a20 2020  : size_limit.   
+00028610: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+00028620: 696e 670a 2020 2020 2020 7469 746c 653a  ing.      title:
+00028630: 2056 6f6c 756d 655f 656d 7074 795f 6469   Volume_empty_di
+00028640: 720a 2020 2020 2020 7479 7065 3a20 6f62  r.      type: ob
+00028650: 6a65 6374 0a20 2020 2056 6f6c 756d 655f  ject.    Volume_
+00028660: 686f 7374 5f70 6174 683a 0a20 2020 2020  host_path:.     
+00028670: 2064 6573 6372 6970 7469 6f6e 3a20 7c0a   description: |.
+00028680: 2020 2020 2020 2020 7265 7072 6573 656e          represen
+00028690: 7473 2061 2070 7265 2d65 7869 7374 696e  ts a pre-existin
+000286a0: 6720 6669 6c65 206f 7220 6469 7265 6374  g file or direct
+000286b0: 6f72 7920 6f6e 2074 6865 2068 6f73 7420  ory on the host 
+000286c0: 6d61 6368 696e 6520 7468 6174 2069 7320  machine that is 
+000286d0: 6469 7265 6374 6c79 2065 7870 6f73 6564  directly exposed
+000286e0: 2074 6f20 7468 6520 636f 6e74 6169 6e65   to the containe
+000286f0: 722e 0a20 2020 2020 2020 2054 6869 7320  r..        This 
+00028700: 6973 2067 656e 6572 616c 6c79 2075 7365  is generally use
+00028710: 6420 666f 7220 7379 7374 656d 2061 6765  d for system age
+00028720: 6e74 7320 6f72 206f 7468 6572 2070 7269  nts or other pri
+00028730: 7669 6c65 6765 6420 7468 696e 6773 2074  vileged things t
+00028740: 6861 7420 6172 6520 616c 6c6f 7765 6420  hat are allowed 
+00028750: 746f 2073 6565 2074 6865 2068 6f73 7420  to see the host 
+00028760: 6d61 6368 696e 652e 0a20 2020 2020 2065  machine..      e
+00028770: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
+00028780: 7061 7468 3a20 2f64 6174 610a 2020 2020  path: /data.    
+00028790: 2020 2020 7061 7468 5f74 7970 653a 2044      path_type: D
+000287a0: 6972 6563 746f 7279 0a20 2020 2020 2070  irectory.      p
+000287b0: 726f 7065 7274 6965 733a 0a20 2020 2020  roperties:.     
+000287c0: 2020 2070 6174 683a 0a20 2020 2020 2020     path:.       
+000287d0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+000287e0: 2250 6174 6820 6f66 2074 6865 2064 6972  "Path of the dir
+000287f0: 6563 746f 7279 206f 6e20 7468 6520 686f  ectory on the ho
+00028800: 7374 2e20 4966 2074 6865 2070 6174 6820  st. If the path 
+00028810: 6973 2061 2073 796d 6c69 6e6b 2c5c 0a20  is a symlink,\. 
+00028820: 2020 2020 2020 2020 2020 205c 2069 7420             \ it 
+00028830: 7769 6c6c 2066 6f6c 6c6f 7720 7468 6520  will follow the 
+00028840: 6c69 6e6b 2074 6f20 7468 6520 7265 616c  link to the real
+00028850: 2070 6174 6822 0a20 2020 2020 2020 2020   path".         
+00028860: 2065 7861 6d70 6c65 3a20 2f64 6174 610a   example: /data.
+00028870: 2020 2020 2020 2020 2020 7469 746c 653a            title:
+00028880: 2070 6174 680a 2020 2020 2020 2020 2020   path.          
+00028890: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+000288a0: 2020 2020 2070 6174 685f 7479 7065 3a0a       path_type:.
+000288b0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+000288c0: 7074 696f 6e3a 2054 7970 6520 666f 7220  ption: Type for 
+000288d0: 486f 7374 5061 7468 2056 6f6c 756d 6520  HostPath Volume 
+000288e0: 4465 6661 756c 7473 2074 6f20 2222 0a20  Defaults to "". 
+000288f0: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
+00028900: 3a20 4469 7265 6374 6f72 790a 2020 2020  : Directory.    
+00028910: 2020 2020 2020 7469 746c 653a 2070 6174        title: pat
+00028920: 685f 7479 7065 0a20 2020 2020 2020 2020  h_type.         
+00028930: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
+00028940: 2020 2020 7469 746c 653a 2056 6f6c 756d      title: Volum
+00028950: 655f 686f 7374 5f70 6174 680a 2020 2020  e_host_path.    
+00028960: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
+00028970: 2020 2043 6f6e 6669 675f 7465 6d70 6c61     Config_templa
+00028980: 7465 735f 696e 6e65 723a 0a20 2020 2020  tes_inner:.     
+00028990: 2065 7861 6d70 6c65 3a0a 2020 2020 2020   example:.      
+000289a0: 2020 7661 6c75 6573 3a0a 2020 2020 2020    values:.      
+000289b0: 2020 2020 6b65 7931 3a20 7661 6c75 6531      key1: value1
+000289c0: 0a20 2020 2020 2020 206e 616d 653a 2063  .        name: c
+000289d0: 6f6e 662f 7365 7276 6572 2e63 6f6e 660a  onf/server.conf.
+000289e0: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
+000289f0: 3a0a 2020 2020 2020 2020 6e61 6d65 3a0a  :.        name:.
+00028a00: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00028a10: 7074 696f 6e3a 2074 6865 2063 6f6e 6669  ption: the confi
+00028a20: 6720 6669 6c65 2070 6174 6820 6e61 6d65  g file path name
+00028a30: 0a20 2020 2020 2020 2020 2065 7861 6d70  .          examp
+00028a40: 6c65 3a20 636f 6e66 2f73 6572 7665 722e  le: conf/server.
+00028a50: 636f 6e66 0a20 2020 2020 2020 2020 2074  conf.          t
+00028a60: 6974 6c65 3a20 6e61 6d65 0a20 2020 2020  itle: name.     
+00028a70: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+00028a80: 670a 2020 2020 2020 2020 7661 6c75 6573  g.        values
+00028a90: 3a0a 2020 2020 2020 2020 2020 6164 6469  :.          addi
+00028aa0: 7469 6f6e 616c 5072 6f70 6572 7469 6573  tionalProperties
+00028ab0: 3a0a 2020 2020 2020 2020 2020 2020 7479  :.            ty
+00028ac0: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
+00028ad0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00028ae0: 3a20 5468 6520 636f 6e66 6967 2076 616c  : The config val
+00028af0: 7565 7320 666f 7220 7468 6520 7465 6d70  ues for the temp
+00028b00: 6c61 7465 2066 696c 650a 2020 2020 2020  late file.      
+00028b10: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
+00028b20: 2020 2020 2020 2020 206b 6579 313a 2076           key1: v
+00028b30: 616c 7565 310a 2020 2020 2020 2020 2020  alue1.          
+00028b40: 7469 746c 653a 2076 616c 7565 730a 2020  title: values.  
+00028b50: 2020 2020 2020 2020 7479 7065 3a20 6f62          type: ob
+00028b60: 6a65 6374 0a20 2020 2020 2074 6974 6c65  ject.      title
+00028b70: 3a20 436f 6e66 6967 5f74 656d 706c 6174  : Config_templat
+00028b80: 6573 5f69 6e6e 6572 0a20 2020 2020 2074  es_inner.      t
+00028b90: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
+00028ba0: 496e 6772 6573 7342 6163 6b65 6e64 5f73  IngressBackend_s
+00028bb0: 6572 7669 6365 3a0a 2020 2020 2020 6465  ervice:.      de
+00028bc0: 7363 7269 7074 696f 6e3a 2052 6566 6572  scription: Refer
+00028bd0: 656e 6365 7320 6120 5365 7276 6963 6520  ences a Service 
+00028be0: 6173 2061 2042 6163 6b65 6e64 2e0a 2020  as a Backend..  
+00028bf0: 2020 2020 6578 616d 706c 653a 0a20 2020      example:.   
+00028c00: 2020 2020 2070 6f72 743a 2038 300a 2020       port: 80.  
+00028c10: 2020 2020 2020 6e61 6d65 3a20 6465 6d6f        name: demo
+00028c20: 2d61 7070 2d73 6572 7669 6365 0a20 2020  -app-service.   
+00028c30: 2020 2070 726f 7065 7274 6965 733a 0a20     properties:. 
+00028c40: 2020 2020 2020 206e 616d 653a 0a20 2020         name:.   
+00028c50: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00028c60: 6f6e 3a20 4e61 6d65 206f 6620 7468 6520  on: Name of the 
+00028c70: 7265 6665 7265 6e63 6564 2073 6572 7669  referenced servi
+00028c80: 6365 2e0a 2020 2020 2020 2020 2020 6578  ce..          ex
+00028c90: 616d 706c 653a 2064 656d 6f2d 6170 702d  ample: demo-app-
+00028ca0: 7365 7276 6963 650a 2020 2020 2020 2020  service.        
+00028cb0: 2020 7469 746c 653a 206e 616d 650a 2020    title: name.  
+00028cc0: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
+00028cd0: 7269 6e67 0a20 2020 2020 2020 2070 6f72  ring.        por
+00028ce0: 743a 0a20 2020 2020 2020 2020 2064 6573  t:.          des
+00028cf0: 6372 6970 7469 6f6e 3a20 5468 6520 6e75  cription: The nu
+00028d00: 6d65 7269 6361 6c20 706f 7274 206e 756d  merical port num
+00028d10: 6265 7220 6f6e 2074 6865 2053 6572 7669  ber on the Servi
+00028d20: 6365 2e0a 2020 2020 2020 2020 2020 6578  ce..          ex
+00028d30: 616d 706c 653a 2038 300a 2020 2020 2020  ample: 80.      
+00028d40: 2020 2020 7469 746c 653a 2070 6f72 740a      title: port.
+00028d50: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
+00028d60: 696e 7465 6765 720a 2020 2020 2020 7469  integer.      ti
+00028d70: 746c 653a 2049 6e67 7265 7373 4261 636b  tle: IngressBack
+00028d80: 656e 645f 7365 7276 6963 650a 2020 2020  end_service.    
+00028d90: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
+00028da0: 2020 2053 6572 7669 6365 4d6f 6e69 746f     ServiceMonito
+00028db0: 725f 6e61 6d65 7370 6163 655f 7365 6c65  r_namespace_sele
+00028dc0: 6374 6f72 3a0a 2020 2020 2020 6578 616d  ctor:.      exam
+00028dd0: 706c 653a 0a20 2020 2020 2020 206d 6174  ple:.        mat
+00028de0: 6368 5f6e 616d 6573 3a0a 2020 2020 2020  ch_names:.      
+00028df0: 2020 2d20 6465 6661 756c 740a 2020 2020    - default.    
+00028e00: 2020 2020 616e 793a 2074 7275 650a 2020      any: true.  
+00028e10: 2020 2020 7072 6f70 6572 7469 6573 3a0a      properties:.
+00028e20: 2020 2020 2020 2020 6d61 7463 685f 6e61          match_na
+00028e30: 6d65 733a 0a20 2020 2020 2020 2020 2064  mes:.          d
+00028e40: 6573 6372 6970 7469 6f6e 3a20 6d61 7463  escription: matc
+00028e50: 684e 616d 6573 2069 7320 6120 6c69 7374  hNames is a list
+00028e60: 206f 6620 6e61 6d65 7370 6163 6520 6e61   of namespace na
+00028e70: 6d65 732e 2054 6865 204e 616d 6573 7061  mes. The Namespa
+00028e80: 6365 5365 6c65 6374 6f72 0a20 2020 2020  ceSelector.     
+00028e90: 2020 2020 2020 206d 6174 6368 6573 206e         matches n
+00028ea0: 616d 6573 7061 6365 7320 6261 7365 6420  amespaces based 
+00028eb0: 6f6e 2074 6865 206e 616d 6573 2073 656c  on the names sel
+00028ec0: 6563 7465 6420 6279 2074 6869 7320 6c69  ected by this li
+00028ed0: 7374 2e0a 2020 2020 2020 2020 2020 6578  st..          ex
+00028ee0: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
+00028ef0: 202d 2064 6566 6175 6c74 0a20 2020 2020   - default.     
+00028f00: 2020 2020 2069 7465 6d73 3a0a 2020 2020       items:.    
+00028f10: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
+00028f20: 7269 6e67 0a20 2020 2020 2020 2020 2074  ring.          t
+00028f30: 6974 6c65 3a20 6d61 7463 685f 6e61 6d65  itle: match_name
+00028f40: 730a 2020 2020 2020 2020 2020 7479 7065  s.          type
+00028f50: 3a20 6172 7261 790a 2020 2020 2020 2020  : array.        
+00028f60: 616e 793a 0a20 2020 2020 2020 2020 2064  any:.          d
+00028f70: 6573 6372 6970 7469 6f6e 3a20 2261 6e79  escription: "any
+00028f80: 206d 6174 6368 6573 2061 6e79 2073 656c   matches any sel
+00028f90: 6563 7465 6420 6e61 6d65 7370 6163 6573  ected namespaces
+00028fa0: 2e20 4966 2074 7275 652c 2074 6865 6e20  . If true, then 
+00028fb0: 6e6f 6e65 206f 665c 0a20 2020 2020 2020  none of\.       
+00028fc0: 2020 2020 205c 2074 6865 206f 7468 6572       \ the other
+00028fd0: 206d 6174 6368 2066 6965 6c64 7320 6361   match fields ca
+00028fe0: 6e20 6265 2073 6574 2e22 0a20 2020 2020  n be set.".     
+00028ff0: 2020 2020 2065 7861 6d70 6c65 3a20 7472       example: tr
+00029000: 7565 0a20 2020 2020 2020 2020 2074 6974  ue.          tit
+00029010: 6c65 3a20 616e 790a 2020 2020 2020 2020  le: any.        
+00029020: 2020 7479 7065 3a20 626f 6f6c 6561 6e0a    type: boolean.
+00029030: 2020 2020 2020 7469 746c 653a 2053 6572        title: Ser
+00029040: 7669 6365 4d6f 6e69 746f 725f 6e61 6d65  viceMonitor_name
+00029050: 7370 6163 655f 7365 6c65 6374 6f72 0a20  space_selector. 
+00029060: 2020 2020 2074 7970 653a 206f 626a 6563       type: objec
+00029070: 740a 2020 7365 6375 7269 7479 5363 6865  t.  securitySche
+00029080: 6d65 733a 0a20 2020 2062 6561 7265 7241  mes:.    bearerA
+00029090: 7574 683a 0a20 2020 2020 2062 6561 7265  uth:.      beare
+000290a0: 7246 6f72 6d61 743a 204a 5754 0a20 2020  rFormat: JWT.   
+000290b0: 2020 2073 6368 656d 653a 2062 6561 7265     scheme: beare
+000290c0: 720a 2020 2020 2020 7479 7065 3a20 6874  r.      type: ht
+000290d0: 7470 0a20 2020 2020 2078 2d62 6561 7265  tp.      x-beare
+000290e0: 7249 6e66 6f46 756e 633a 206f 7065 6e61  rInfoFunc: opena
+000290f0: 7069 5f73 6572 7665 722e 636f 6e74 726f  pi_server.contro
+00029100: 6c6c 6572 732e 7365 6375 7269 7479 5f63  llers.security_c
+00029110: 6f6e 7472 6f6c 6c65 725f 2e69 6e66 6f5f  ontroller_.info_
+00029120: 6672 6f6d 5f62 6561 7265 7241 7574 680a  from_bearerAuth.
```

### Comparing `dingman_openapi_server-1.0.19/openapi_server/test/test_deploy_resources_controller.py` & `dingman_openapi_server-1.0.20/openapi_server/test/test_deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/typing_utils.py` & `dingman_openapi_server-1.0.20/openapi_server/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/openapi_server/util.py` & `dingman_openapi_server-1.0.20/openapi_server/util.py`

 * *Files identical despite different names*

### Comparing `dingman_openapi_server-1.0.19/setup.py` & `dingman_openapi_server-1.0.20/setup.py`

 * *Files identical despite different names*

