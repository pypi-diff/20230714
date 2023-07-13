# Comparing `tmp/momento-1.6.1.tar.gz` & `tmp/momento-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momento-1.6.1.tar", max compression
+gzip compressed data, was "momento-1.7.0.tar", max compression
```

## Comparing `momento-1.6.1.tar` & `momento-1.7.0.tar`

### file list

```diff
@@ -1,106 +1,116 @@
--rw-r--r--   0        0        0    11357 2023-06-27 19:56:11.222096 momento-1.6.1/LICENSE
--rw-r--r--   0        0        0     4282 2023-06-27 19:56:11.222096 momento-1.6.1/README.md
--rw-r--r--   0        0        0     3805 2023-06-27 19:56:31.462333 momento-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      619 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/__init__.py
--rw-r--r--   0        0        0       86 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/auth/__init__.py
--rw-r--r--   0        0        0     2868 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/auth/credential_provider.py
--rw-r--r--   0        0        0     2003 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/auth/momento_endpoint_resolver.py
--rw-r--r--   0        0        0    43798 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/cache_client.py
--rw-r--r--   0        0        0    44449 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/cache_client_async.py
--rw-r--r--   0        0        0      176 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/__init__.py
--rw-r--r--   0        0        0     3250 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/configuration.py
--rw-r--r--   0        0        0     4290 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/configurations.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/transport/__init__.py
--rw-r--r--   0        0        0      314 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/transport/grpc_configuration.py
--rw-r--r--   0        0        0     2358 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/transport/transport_strategy.py
--rw-r--r--   0        0        0     1503 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/errors/__init__.py
--rw-r--r--   0        0        0     3991 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/errors/error_converter.py
--rw-r--r--   0        0        0     2329 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/errors/error_details.py
--rw-r--r--   0        0        0     8799 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/errors/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/__init__.py
--rw-r--r--   0        0        0      406 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/_utilities/__init__.py
--rw-r--r--   0        0        0     4735 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/_utilities/_data_validation.py
--rw-r--r--   0        0        0      531 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/_utilities/_momento_version.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/__init__.py
--rw-r--r--   0        0        0     4377 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1856 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_retry_interceptor.py
--rw-r--r--   0        0        0     5794 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_scs_control_client.py
--rw-r--r--   0        0        0    47792 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_scs_data_client.py
--rw-r--r--   0        0        0     3206 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_scs_grpc_manager.py
--rw-r--r--   0        0        0      123 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_utilities.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/synchronous/__init__.py
--rw-r--r--   0        0        0     3714 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1829 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_retry_interceptor.py
--rw-r--r--   0        0        0     5700 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_scs_control_client.py
--rw-r--r--   0        0        0    47412 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_scs_data_client.py
--rw-r--r--   0        0        0     2436 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_scs_grpc_manager.py
--rw-r--r--   0        0        0      159 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_utilities.py
--rw-r--r--   0        0        0     2790 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/logs.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/py.typed
--rw-r--r--   0        0        0      154 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/requests/__init__.py
--rw-r--r--   0        0        0     3800 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/requests/collection_ttl.py
--rw-r--r--   0        0        0       91 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/requests/sort_order.py
--rw-r--r--   0        0        0     6841 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/cache/__init__.py
--rw-r--r--   0        0        0     1758 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/cache/create.py
--rw-r--r--   0        0        0     1405 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/cache/delete.py
--rw-r--r--   0        0        0      849 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/cache/flush.py
--rw-r--r--   0        0        0     2275 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/cache/list.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/signing_key/__init__.py
--rw-r--r--   0        0        0     1764 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/signing_key/create.py
--rw-r--r--   0        0        0     2479 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/signing_key/list.py
--rw-r--r--   0        0        0      979 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/signing_key/revoke.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/__init__.py
--rw-r--r--   0        0        0     2047 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/fetch.py
--rw-r--r--   0        0        0     1678 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/get_field.py
--rw-r--r--   0        0        0     3320 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/get_fields.py
--rw-r--r--   0        0        0     1050 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/increment.py
--rw-r--r--   0        0        0      945 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/remove_field.py
--rw-r--r--   0        0        0      953 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/remove_fields.py
--rw-r--r--   0        0        0      921 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/set_field.py
--rw-r--r--   0        0        0      929 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/set_fields.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/__init__.py
--rw-r--r--   0        0        0     1052 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/concatenate_back.py
--rw-r--r--   0        0        0     1060 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/concatenate_front.py
--rw-r--r--   0        0        0     1402 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/fetch.py
--rw-r--r--   0        0        0     1070 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/length.py
--rw-r--r--   0        0        0     1189 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/pop_back.py
--rw-r--r--   0        0        0     1199 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/pop_front.py
--rw-r--r--   0        0        0      977 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/push_back.py
--rw-r--r--   0        0        0      985 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/push_front.py
--rw-r--r--   0        0        0      874 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/remove_value.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/__init__.py
--rw-r--r--   0        0        0      823 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/delete.py
--rw-r--r--   0        0        0     1155 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/get.py
--rw-r--r--   0        0        0     1141 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/increment.py
--rw-r--r--   0        0        0      799 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/set.py
--rw-r--r--   0        0        0     1056 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/set_if_not_exists.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/__init__.py
--rw-r--r--   0        0        0      870 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/add_element.py
--rw-r--r--   0        0        0      880 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/add_elements.py
--rw-r--r--   0        0        0     1452 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/fetch.py
--rw-r--r--   0        0        0      896 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/remove_element.py
--rw-r--r--   0        0        0      906 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/remove_elements.py
--rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/fetch.py
--rw-r--r--   0        0        0     1205 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/get_rank.py
--rw-r--r--   0        0        0     1581 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/get_score.py
--rw-r--r--   0        0        0     2323 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/get_scores.py
--rw-r--r--   0        0        0     1087 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/increment_score.py
--rw-r--r--   0        0        0      944 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/put_element.py
--rw-r--r--   0        0        0      952 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/put_elements.py
--rw-r--r--   0        0        0      971 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/remove_element.py
--rw-r--r--   0        0        0      979 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/remove_elements.py
--rw-r--r--   0        0        0     1460 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/mixins.py
--rw-r--r--   0        0        0     4724 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/response.py
--rw-r--r--   0        0        0      423 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/default_eligibility_strategy.py
--rw-r--r--   0        0        0      216 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/eligibility_strategy.py
--rw-r--r--   0        0        0     2181 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/fixed_count_retry_strategy.py
--rw-r--r--   0        0        0      251 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/retry_strategy.py
--rw-r--r--   0        0        0      291 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/retryable_props.py
--rw-r--r--   0        0        0     1722 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/typing.py
--rw-r--r--   0        0        0     5792 1970-01-01 00:00:00.000000 momento-1.6.1/setup.py
--rw-r--r--   0        0        0     5580 1970-01-01 00:00:00.000000 momento-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-13 23:14:39.004979 momento-1.7.0/LICENSE
+-rw-r--r--   0        0        0     4243 2023-07-13 23:14:39.004979 momento-1.7.0/README.md
+-rw-r--r--   0        0        0     3805 2023-07-13 23:14:57.769164 momento-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      816 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/__init__.py
+-rw-r--r--   0        0        0       86 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/auth/__init__.py
+-rw-r--r--   0        0        0     2868 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/auth/credential_provider.py
+-rw-r--r--   0        0        0     2003 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/auth/momento_endpoint_resolver.py
+-rw-r--r--   0        0        0    43798 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/cache_client.py
+-rw-r--r--   0        0        0    44449 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/cache_client_async.py
+-rw-r--r--   0        0        0      327 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/config/__init__.py
+-rw-r--r--   0        0        0     3250 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/config/configuration.py
+-rw-r--r--   0        0        0     4290 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/config/configurations.py
+-rw-r--r--   0        0        0     1211 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/config/topic_configuration.py
+-rw-r--r--   0        0        0      895 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/config/topic_configurations.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/config/transport/__init__.py
+-rw-r--r--   0        0        0      314 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/config/transport/grpc_configuration.py
+-rw-r--r--   0        0        0     2358 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/config/transport/transport_strategy.py
+-rw-r--r--   0        0        0     1503 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/errors/__init__.py
+-rw-r--r--   0        0        0     3991 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/errors/error_converter.py
+-rw-r--r--   0        0        0     2329 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/errors/error_details.py
+-rw-r--r--   0        0        0     8799 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/errors/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/__init__.py
+-rw-r--r--   0        0        0      432 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/_utilities/__init__.py
+-rw-r--r--   0        0        0     4833 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/_utilities/_data_validation.py
+-rw-r--r--   0        0        0      531 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/_utilities/_momento_version.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/aio/__init__.py
+-rw-r--r--   0        0        0     5842 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/aio/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1856 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/aio/_retry_interceptor.py
+-rw-r--r--   0        0        0     5794 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/aio/_scs_control_client.py
+-rw-r--r--   0        0        0    47792 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/aio/_scs_data_client.py
+-rw-r--r--   0        0        0     5184 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/aio/_scs_grpc_manager.py
+-rw-r--r--   0        0        0     4800 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/aio/_scs_pubsub_client.py
+-rw-r--r--   0        0        0      123 2023-07-13 23:14:39.004979 momento-1.7.0/src/momento/internal/aio/_utilities.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/internal/synchronous/__init__.py
+-rw-r--r--   0        0        0     5046 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/internal/synchronous/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1829 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/internal/synchronous/_retry_interceptor.py
+-rw-r--r--   0        0        0     5700 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/internal/synchronous/_scs_control_client.py
+-rw-r--r--   0        0        0    47412 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/internal/synchronous/_scs_data_client.py
+-rw-r--r--   0        0        0     4524 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/internal/synchronous/_scs_grpc_manager.py
+-rw-r--r--   0        0        0     4727 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/internal/synchronous/_scs_pubsub_client.py
+-rw-r--r--   0        0        0      159 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/internal/synchronous/_utilities.py
+-rw-r--r--   0        0        0     2790 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/logs.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/py.typed
+-rw-r--r--   0        0        0      154 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/requests/__init__.py
+-rw-r--r--   0        0        0     3800 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/requests/collection_ttl.py
+-rw-r--r--   0        0        0       91 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/requests/sort_order.py
+-rw-r--r--   0        0        0     7281 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/control/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/control/cache/__init__.py
+-rw-r--r--   0        0        0     1758 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/control/cache/create.py
+-rw-r--r--   0        0        0     1405 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/control/cache/delete.py
+-rw-r--r--   0        0        0      849 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/control/cache/flush.py
+-rw-r--r--   0        0        0     2275 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/control/cache/list.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/control/signing_key/__init__.py
+-rw-r--r--   0        0        0     1764 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/control/signing_key/create.py
+-rw-r--r--   0        0        0     2479 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/control/signing_key/list.py
+-rw-r--r--   0        0        0      979 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/control/signing_key/revoke.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/dictionary/__init__.py
+-rw-r--r--   0        0        0     2047 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/dictionary/fetch.py
+-rw-r--r--   0        0        0     1678 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/dictionary/get_field.py
+-rw-r--r--   0        0        0     3320 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/dictionary/get_fields.py
+-rw-r--r--   0        0        0     1050 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/dictionary/increment.py
+-rw-r--r--   0        0        0      945 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/dictionary/remove_field.py
+-rw-r--r--   0        0        0      953 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/dictionary/remove_fields.py
+-rw-r--r--   0        0        0      921 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/dictionary/set_field.py
+-rw-r--r--   0        0        0      929 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/dictionary/set_fields.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/list/__init__.py
+-rw-r--r--   0        0        0     1052 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/list/concatenate_back.py
+-rw-r--r--   0        0        0     1060 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/list/concatenate_front.py
+-rw-r--r--   0        0        0     1402 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/list/fetch.py
+-rw-r--r--   0        0        0     1070 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/list/length.py
+-rw-r--r--   0        0        0     1189 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/list/pop_back.py
+-rw-r--r--   0        0        0     1199 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/list/pop_front.py
+-rw-r--r--   0        0        0      977 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/list/push_back.py
+-rw-r--r--   0        0        0      985 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/list/push_front.py
+-rw-r--r--   0        0        0      874 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/list/remove_value.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/scalar/__init__.py
+-rw-r--r--   0        0        0      823 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/scalar/delete.py
+-rw-r--r--   0        0        0     1155 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/scalar/get.py
+-rw-r--r--   0        0        0     1141 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/scalar/increment.py
+-rw-r--r--   0        0        0      799 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/scalar/set.py
+-rw-r--r--   0        0        0     1056 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/scalar/set_if_not_exists.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/set/__init__.py
+-rw-r--r--   0        0        0      870 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/set/add_element.py
+-rw-r--r--   0        0        0      880 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/set/add_elements.py
+-rw-r--r--   0        0        0     1452 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/set/fetch.py
+-rw-r--r--   0        0        0      896 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/set/remove_element.py
+-rw-r--r--   0        0        0      906 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/set/remove_elements.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/sorted_set/__init__.py
+-rw-r--r--   0        0        0     1616 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/sorted_set/fetch.py
+-rw-r--r--   0        0        0     1205 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/sorted_set/get_rank.py
+-rw-r--r--   0        0        0     1581 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/sorted_set/get_score.py
+-rw-r--r--   0        0        0     2323 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/sorted_set/get_scores.py
+-rw-r--r--   0        0        0     1087 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/sorted_set/increment_score.py
+-rw-r--r--   0        0        0      944 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/sorted_set/put_element.py
+-rw-r--r--   0        0        0      952 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/sorted_set/put_elements.py
+-rw-r--r--   0        0        0      971 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/sorted_set/remove_element.py
+-rw-r--r--   0        0        0      979 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/data/sorted_set/remove_elements.py
+-rw-r--r--   0        0        0     1460 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/pubsub/__init__.py
+-rw-r--r--   0        0        0      775 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/pubsub/publish.py
+-rw-r--r--   0        0        0     7829 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/pubsub/subscribe.py
+-rw-r--r--   0        0        0     1116 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/pubsub/subscription_item.py
+-rw-r--r--   0        0        0     4766 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/responses/response.py
+-rw-r--r--   0        0        0      423 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/retry/__init__.py
+-rw-r--r--   0        0        0     2900 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/retry/default_eligibility_strategy.py
+-rw-r--r--   0        0        0      216 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/retry/eligibility_strategy.py
+-rw-r--r--   0        0        0     2181 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/retry/fixed_count_retry_strategy.py
+-rw-r--r--   0        0        0      251 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/retry/retry_strategy.py
+-rw-r--r--   0        0        0      291 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/retry/retryable_props.py
+-rw-r--r--   0        0        0     3570 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/topic_client.py
+-rw-r--r--   0        0        0     3661 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/topic_client_async.py
+-rw-r--r--   0        0        0     1739 2023-07-13 23:14:39.008979 momento-1.7.0/src/momento/typing.py
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 momento-1.7.0/setup.py
+-rw-r--r--   0        0        0     5541 1970-01-01 00:00:00.000000 momento-1.7.0/PKG-INFO
```

### Comparing `momento-1.6.1/LICENSE` & `momento-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/README.md` & `momento-1.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,17 @@
 
 cache_client = CacheClient(
     Configurations.Laptop.v1(),
     CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),
     timedelta(seconds=60)
 )
 
-create_cache_response = cache_client.create_cache("cache")
-set_response = cache_client.set("cache", "my-key", "my-value")
-get_response = cache_client.get(_CACHE_NAME, _KEY)
+cache_client.create_cache("cache")
+cache_client.set("cache", "my-key", "my-value")
+get_response = cache_client.get("cache", "my-key")
 match get_response:
     case CacheGet.Hit() as hit:
         print(f"Got value: {hit.value_string}")
     case _:
         print(f"Response was not a hit: {get_response}")
 
 ```
```

### Comparing `momento-1.6.1/pyproject.toml` & `momento-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "momento"
-version = "1.6.1"
+version = "1.7.0"
 
 authors = ["Momento <hello@momentohq.com>"]
 description = "SDK for Momento"
 
 license = "Apache-2.0"
 
 documentation = "https://docs.momentohq.com/"
@@ -26,15 +26,15 @@
 ]
 
 exclude = ["src/momento/internal/codegen.py"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
-momento-wire-types = "^0.64"
+momento-wire-types = "^0.67"
 grpcio = "^1.46.0"
 # note if you bump this presigned url test need be updated
 pyjwt = "^2.4.0"
 # Need a lower bound of 4 to be compatible with python 3.7 flake8
 importlib-metadata = { version=">=4", python="<3.8" }
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `momento-1.6.1/src/momento/auth/credential_provider.py` & `momento-1.7.0/src/momento/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/auth/momento_endpoint_resolver.py` & `momento-1.7.0/src/momento/auth/momento_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/cache_client.py` & `momento-1.7.0/src/momento/cache_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/cache_client_async.py` & `momento-1.7.0/src/momento/cache_client_async.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/config/configuration.py` & `momento-1.7.0/src/momento/config/configuration.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/config/configurations.py` & `momento-1.7.0/src/momento/config/configurations.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/config/transport/transport_strategy.py` & `momento-1.7.0/src/momento/config/transport/transport_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/errors/__init__.py` & `momento-1.7.0/src/momento/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/errors/error_converter.py` & `momento-1.7.0/src/momento/errors/error_converter.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/errors/error_details.py` & `momento-1.7.0/src/momento/errors/error_details.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/errors/exceptions.py` & `momento-1.7.0/src/momento/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/internal/_utilities/_data_validation.py` & `momento-1.7.0/src/momento/internal/_utilities/_data_validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,18 @@
     _validate_name(set_name, "Set name")
 
 
 def _validate_sorted_set_name(sorted_set_name: str) -> None:
     _validate_name(sorted_set_name, "Sorted set name")
 
 
+def _validate_topic_name(topic_name: str) -> None:
+    _validate_name(topic_name, "Topic name")
+
+
 def _validate_sorted_set_score(score: float) -> float:
     if isinstance(score, float):
         return score
     raise InvalidArgumentException(f"score must be a float. Given type: {type(score)}")
 
 
 def _as_bytes(
```

### Comparing `momento-1.6.1/src/momento/internal/_utilities/_momento_version.py` & `momento-1.7.0/src/momento/internal/_utilities/_momento_version.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/internal/aio/_add_header_client_interceptor.py` & `momento-1.7.0/src/momento/internal/aio/_add_header_client_interceptor.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,48 @@
     once_only_headers = ["agent"]
 
     def __init__(self, name: str, value: str):
         self.name = name
         self.value = value
 
 
+class AddHeaderStreamingClientInterceptor(grpc.aio.UnaryStreamClientInterceptor):
+    are_only_once_headers_sent = False
+
+    def __init__(self, headers: list[Header]):
+        self._headers_to_add_once: list[Header] = list(
+            filter(lambda header: header.name in header.once_only_headers, headers)
+        )
+        self.headers_to_add_every_time = list(
+            filter(lambda header: header.name not in header.once_only_headers, headers)
+        )
+
+    async def intercept_unary_stream(
+        self,
+        continuation: Callable[
+            [grpc.aio._interceptor.ClientCallDetails, grpc.aio._typing.RequestType],
+            grpc.aio._call.UnaryStreamCall,
+        ],
+        client_call_details: grpc.aio._interceptor.ClientCallDetails,
+        request: grpc.aio._typing.RequestType,
+    ) -> grpc.aio._call.UnaryStreamCall | grpc.aio._typing.ResponseType:
+
+        new_client_call_details = sanitize_client_call_details(client_call_details)
+
+        for header in self.headers_to_add_every_time:
+            new_client_call_details.metadata.add(header.name, header.value)
+
+        if not AddHeaderStreamingClientInterceptor.are_only_once_headers_sent:
+            for header in self._headers_to_add_once:
+                new_client_call_details.metadata.add(header.name, header.value)
+                AddHeaderStreamingClientInterceptor.are_only_once_headers_sent = True
+
+        return await continuation(new_client_call_details, request)
+
+
 class AddHeaderClientInterceptor(grpc.aio.UnaryUnaryClientInterceptor):
     are_only_once_headers_sent = False
 
     def __init__(self, headers: list[Header]):
         self._headers_to_add_once: list[Header] = list(
             filter(lambda header: header.name in header.once_only_headers, headers)
         )
```

### Comparing `momento-1.6.1/src/momento/internal/aio/_retry_interceptor.py` & `momento-1.7.0/src/momento/internal/aio/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/internal/aio/_scs_control_client.py` & `momento-1.7.0/src/momento/internal/aio/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/internal/aio/_scs_data_client.py` & `momento-1.7.0/src/momento/internal/aio/_scs_data_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/internal/aio/_scs_grpc_manager.py` & `momento-1.7.0/src/momento/internal/aio/_scs_grpc_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from __future__ import annotations
 
+from typing import Optional
+
 import grpc
 from momento_wire_types import cacheclient_pb2_grpc as cache_client
+from momento_wire_types import cachepubsub_pb2_grpc as pubsub_client
 from momento_wire_types import controlclient_pb2_grpc as control_client
 
 from momento.auth import CredentialProvider
-from momento.config import Configuration
+from momento.config import Configuration, TopicConfiguration
 from momento.internal._utilities import momento_version
 from momento.retry import RetryStrategy
 
-from ._add_header_client_interceptor import AddHeaderClientInterceptor, Header
+from ._add_header_client_interceptor import (
+    AddHeaderClientInterceptor,
+    AddHeaderStreamingClientInterceptor,
+    Header,
+)
 from ._retry_interceptor import RetryInterceptor
 
 
 class _ControlGrpcManager:
-    """Internal gRPC control mananger."""
+    """Internal gRPC control manager."""
 
     version = momento_version
 
     def __init__(self, configuration: Configuration, credential_provider: CredentialProvider):
         self._secure_channel = grpc.aio.secure_channel(
             target=credential_provider.control_endpoint,
             credentials=grpc.ssl_channel_credentials(),
@@ -29,15 +36,15 @@
         await self._secure_channel.close()
 
     def async_stub(self) -> control_client.ScsControlStub:
         return control_client.ScsControlStub(self._secure_channel)  # type: ignore[no-untyped-call]
 
 
 class _DataGrpcManager:
-    """Internal gRPC data mananger."""
+    """Internal gRPC data manager."""
 
     version = momento_version
 
     def __init__(self, configuration: Configuration, credential_provider: CredentialProvider):
         self._secure_channel = grpc.aio.secure_channel(
             target=credential_provider.cache_endpoint,
             credentials=grpc.ssl_channel_credentials(),
@@ -61,16 +68,67 @@
     async def close(self) -> None:
         await self._secure_channel.close()
 
     def async_stub(self) -> cache_client.ScsStub:
         return cache_client.ScsStub(self._secure_channel)  # type: ignore[no-untyped-call]
 
 
-def _interceptors(auth_token: str, retry_strategy: RetryStrategy) -> list[grpc.aio.ClientInterceptor]:
+class _PubsubGrpcManager:
+    """Internal gRPC pubsub manager."""
+
+    version = momento_version
+
+    def __init__(self, configuration: TopicConfiguration, credential_provider: CredentialProvider):
+        self._secure_channel = grpc.aio.secure_channel(
+            target=credential_provider.cache_endpoint,
+            credentials=grpc.ssl_channel_credentials(),
+            interceptors=_interceptors(credential_provider.auth_token, None),
+        )
+
+    async def close(self) -> None:
+        await self._secure_channel.close()
+
+    def async_stub(self) -> pubsub_client.PubsubStub:
+        return pubsub_client.PubsubStub(self._secure_channel)  # type: ignore[no-untyped-call]
+
+
+class _PubsubGrpcStreamManager:
+    """Internal gRPC pubsub stream manager."""
+
+    version = momento_version
+
+    def __init__(self, configuration: TopicConfiguration, credential_provider: CredentialProvider):
+        self._secure_channel = grpc.aio.secure_channel(
+            target=credential_provider.cache_endpoint,
+            credentials=grpc.ssl_channel_credentials(),
+            interceptors=_stream_interceptors(credential_provider.auth_token),
+        )
+
+    async def close(self) -> None:
+        await self._secure_channel.close()
+
+    def async_stub(self) -> pubsub_client.PubsubStub:
+        return pubsub_client.PubsubStub(self._secure_channel)  # type: ignore[no-untyped-call]
+
+
+def _interceptors(auth_token: str, retry_strategy: Optional[RetryStrategy] = None) -> list[grpc.aio.ClientInterceptor]:
     headers = [
         Header("authorization", auth_token),
         Header("agent", f"python:{_ControlGrpcManager.version}"),
     ]
-    return [
-        AddHeaderClientInterceptor(headers),
-        RetryInterceptor(retry_strategy),
+    return list(
+        filter(
+            None,
+            [
+                AddHeaderClientInterceptor(headers),
+                RetryInterceptor(retry_strategy) if retry_strategy else None,
+            ],
+        )
+    )
+
+
+def _stream_interceptors(auth_token: str) -> list[grpc.aio.UnaryStreamClientInterceptor]:
+    headers = [
+        Header("authorization", auth_token),
+        Header("agent", f"python:{_PubsubGrpcStreamManager.version}"),
     ]
+    return [AddHeaderStreamingClientInterceptor(headers)]
```

### Comparing `momento-1.6.1/src/momento/internal/synchronous/_add_header_client_interceptor.py` & `momento-1.7.0/src/momento/internal/synchronous/_add_header_client_interceptor.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,48 @@
 class _ClientCallDetails(
     collections.namedtuple("_ClientCallDetails", ("method", "timeout", "metadata", "credentials")),
     grpc.ClientCallDetails,
 ):
     pass
 
 
+class AddHeaderStreamingClientInterceptor(grpc.UnaryStreamClientInterceptor):
+    are_only_once_headers_sent = False
+
+    def __init__(self, headers: list[Header]):
+        self._headers_to_add_once: list[Header] = list(
+            filter(lambda header: header.name in header.once_only_headers, headers)
+        )
+        self.headers_to_add_every_time = list(
+            filter(lambda header: header.name not in header.once_only_headers, headers)
+        )
+
+    def intercept_unary_stream(
+        self,
+        continuation: Callable[
+            [grpc.ClientCallDetails, RequestType],
+            grpc.Call,
+        ],
+        client_call_details: grpc.ClientCallDetails,
+        request: RequestType,
+    ) -> grpc.Call | ResponseType:
+
+        new_client_call_details = sanitize_client_call_details(client_call_details)
+
+        for header in self.headers_to_add_every_time:
+            new_client_call_details.metadata.append((header.name, header.value))
+
+        if not AddHeaderStreamingClientInterceptor.are_only_once_headers_sent:
+            for header in self._headers_to_add_once:
+                new_client_call_details.metadata.append((header.name, header.value))
+                AddHeaderStreamingClientInterceptor.are_only_once_headers_sent = True
+
+        return continuation(new_client_call_details, request)
+
+
 class AddHeaderClientInterceptor(grpc.UnaryUnaryClientInterceptor):
     are_only_once_headers_sent = False
 
     @staticmethod
     def is_only_once_header(header: Header) -> bool:
         return header.name in header.once_only_headers
```

### Comparing `momento-1.6.1/src/momento/internal/synchronous/_retry_interceptor.py` & `momento-1.7.0/src/momento/internal/synchronous/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/internal/synchronous/_scs_control_client.py` & `momento-1.7.0/src/momento/internal/synchronous/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/internal/synchronous/_scs_data_client.py` & `momento-1.7.0/src/momento/internal/synchronous/_scs_data_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/internal/synchronous/_scs_grpc_manager.py` & `momento-1.7.0/src/momento/internal/synchronous/_scs_grpc_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from __future__ import annotations
 
+from typing import Optional
+
 import grpc
 from momento_wire_types import cacheclient_pb2_grpc as cache_client
+from momento_wire_types import cachepubsub_pb2_grpc as pubsub_client
 from momento_wire_types import controlclient_pb2_grpc as control_client
 
 from momento.auth import CredentialProvider
-from momento.config import Configuration
+from momento.config import Configuration, TopicConfiguration
 from momento.internal._utilities import momento_version
 from momento.internal.synchronous._add_header_client_interceptor import (
     AddHeaderClientInterceptor,
+    AddHeaderStreamingClientInterceptor,
     Header,
 )
 from momento.internal.synchronous._retry_interceptor import RetryInterceptor
 from momento.retry import RetryStrategy
 
 
 class _ControlGrpcManager:
@@ -54,10 +58,68 @@
     def close(self) -> None:
         self._secure_channel.close()
 
     def stub(self) -> cache_client.ScsStub:
         return self._stub
 
 
-def _interceptors(auth_token: str, retry_strategy: RetryStrategy) -> list[grpc.UnaryUnaryClientInterceptor]:
+class _PubsubGrpcManager:
+    """Internal gRPC pubsub manager."""
+
+    version = momento_version
+
+    def __init__(self, configuration: TopicConfiguration, credential_provider: CredentialProvider):
+        self._secure_channel = grpc.secure_channel(
+            target=credential_provider.cache_endpoint,
+            credentials=grpc.ssl_channel_credentials(),
+        )
+        intercept_channel = grpc.intercept_channel(
+            self._secure_channel, *_interceptors(credential_provider.auth_token, None)
+        )
+        self._stub = pubsub_client.PubsubStub(intercept_channel)  # type: ignore[no-untyped-call]
+
+    def close(self) -> None:
+        self._secure_channel.close()
+
+    def stub(self) -> pubsub_client.PubsubStub:
+        return self._stub
+
+
+class _PubsubGrpcStreamManager:
+    """Internal gRPC pubsub stream manager."""
+
+    version = momento_version
+
+    def __init__(self, configuration: TopicConfiguration, credential_provider: CredentialProvider):
+        self._secure_channel = grpc.secure_channel(
+            target=credential_provider.cache_endpoint,
+            credentials=grpc.ssl_channel_credentials(),
+        )
+        intercept_channel = grpc.intercept_channel(
+            self._secure_channel, *_stream_interceptors(credential_provider.auth_token)
+        )
+        self._stub = pubsub_client.PubsubStub(intercept_channel)  # type: ignore[no-untyped-call]
+
+    def close(self) -> None:
+        self._secure_channel.close()
+
+    def stub(self) -> pubsub_client.PubsubStub:
+        return self._stub
+
+
+def _interceptors(
+    auth_token: str, retry_strategy: Optional[RetryStrategy] = None
+) -> list[grpc.UnaryUnaryClientInterceptor]:
     headers = [Header("authorization", auth_token), Header("agent", f"python:{_ControlGrpcManager.version}")]
-    return [AddHeaderClientInterceptor(headers), RetryInterceptor(retry_strategy)]
+    return list(
+        filter(
+            None, [AddHeaderClientInterceptor(headers), RetryInterceptor(retry_strategy) if retry_strategy else None]
+        )
+    )
+
+
+def _stream_interceptors(auth_token: str) -> list[grpc.UnaryStreamClientInterceptor]:
+    headers = [
+        Header("authorization", auth_token),
+        Header("agent", f"python:{_PubsubGrpcStreamManager.version}"),
+    ]
+    return [AddHeaderStreamingClientInterceptor(headers)]
```

### Comparing `momento-1.6.1/src/momento/logs.py` & `momento-1.7.0/src/momento/logs.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/requests/collection_ttl.py` & `momento-1.7.0/src/momento/requests/collection_ttl.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/__init__.py` & `momento-1.7.0/src/momento/responses/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -103,15 +103,21 @@
     CacheSortedSetPutElement,
     CacheSortedSetPutElementResponse,
 )
 from .data.sorted_set.put_elements import (
     CacheSortedSetPutElements,
     CacheSortedSetPutElementsResponse,
 )
-from .response import CacheResponse, ControlResponse
+from .pubsub.publish import TopicPublish, TopicPublishResponse
+from .pubsub.subscribe import TopicSubscribe, TopicSubscribeResponse
+from .pubsub.subscription_item import (
+    TopicSubscriptionItem,
+    TopicSubscriptionItemResponse,
+)
+from .response import CacheResponse, ControlResponse, PubsubResponse
 
 __all__ = [
     "CreateCache",
     "CreateCacheResponse",
     "DeleteCache",
     "DeleteCacheResponse",
     "ListCaches",
@@ -187,10 +193,17 @@
     "CacheSortedSetGetScores",
     "CacheSortedSetGetScoresResponse",
     "CacheSortedSetPutElementResponse",
     "CacheSortedSetPutElements",
     "CacheSortedSetPutElementsResponse",
     "CacheSortedSetFetch",
     "CacheSortedSetFetchResponse",
+    "TopicPublish",
+    "TopicPublishResponse",
+    "TopicSubscribe",
+    "TopicSubscribeResponse",
+    "TopicSubscriptionItem",
+    "TopicSubscriptionItemResponse",
     "CacheResponse",
     "ControlResponse",
+    "PubsubResponse",
 ]
```

### Comparing `momento-1.6.1/src/momento/responses/control/cache/create.py` & `momento-1.7.0/src/momento/responses/control/cache/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/control/cache/delete.py` & `momento-1.7.0/src/momento/responses/control/cache/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/control/cache/flush.py` & `momento-1.7.0/src/momento/responses/control/cache/flush.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/control/cache/list.py` & `momento-1.7.0/src/momento/responses/control/cache/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/control/signing_key/create.py` & `momento-1.7.0/src/momento/responses/control/signing_key/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/control/signing_key/list.py` & `momento-1.7.0/src/momento/responses/control/signing_key/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/control/signing_key/revoke.py` & `momento-1.7.0/src/momento/responses/control/signing_key/revoke.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/dictionary/fetch.py` & `momento-1.7.0/src/momento/responses/data/dictionary/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/dictionary/get_field.py` & `momento-1.7.0/src/momento/responses/data/dictionary/get_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/dictionary/get_fields.py` & `momento-1.7.0/src/momento/responses/data/dictionary/get_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/dictionary/increment.py` & `momento-1.7.0/src/momento/responses/data/dictionary/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/dictionary/remove_field.py` & `momento-1.7.0/src/momento/responses/data/dictionary/remove_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/dictionary/remove_fields.py` & `momento-1.7.0/src/momento/responses/data/dictionary/remove_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/dictionary/set_field.py` & `momento-1.7.0/src/momento/responses/data/dictionary/set_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/dictionary/set_fields.py` & `momento-1.7.0/src/momento/responses/data/dictionary/set_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/list/concatenate_back.py` & `momento-1.7.0/src/momento/responses/data/list/concatenate_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/list/concatenate_front.py` & `momento-1.7.0/src/momento/responses/data/list/concatenate_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/list/fetch.py` & `momento-1.7.0/src/momento/responses/data/list/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/list/length.py` & `momento-1.7.0/src/momento/responses/data/list/length.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/list/pop_back.py` & `momento-1.7.0/src/momento/responses/data/list/pop_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/list/pop_front.py` & `momento-1.7.0/src/momento/responses/data/list/pop_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/list/push_back.py` & `momento-1.7.0/src/momento/responses/data/list/push_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/list/push_front.py` & `momento-1.7.0/src/momento/responses/data/list/push_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/list/remove_value.py` & `momento-1.7.0/src/momento/responses/data/list/remove_value.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/scalar/delete.py` & `momento-1.7.0/src/momento/responses/data/scalar/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/scalar/get.py` & `momento-1.7.0/src/momento/responses/data/scalar/get.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/scalar/increment.py` & `momento-1.7.0/src/momento/responses/data/scalar/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/scalar/set.py` & `momento-1.7.0/src/momento/responses/data/scalar/set.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/scalar/set_if_not_exists.py` & `momento-1.7.0/src/momento/responses/data/scalar/set_if_not_exists.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/set/add_element.py` & `momento-1.7.0/src/momento/responses/data/set/add_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/set/add_elements.py` & `momento-1.7.0/src/momento/responses/data/set/add_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/set/fetch.py` & `momento-1.7.0/src/momento/responses/data/set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/set/remove_element.py` & `momento-1.7.0/src/momento/responses/data/set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/set/remove_elements.py` & `momento-1.7.0/src/momento/responses/data/set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/sorted_set/fetch.py` & `momento-1.7.0/src/momento/responses/data/sorted_set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/sorted_set/get_rank.py` & `momento-1.7.0/src/momento/responses/data/sorted_set/get_rank.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/sorted_set/get_score.py` & `momento-1.7.0/src/momento/responses/data/sorted_set/get_score.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/sorted_set/get_scores.py` & `momento-1.7.0/src/momento/responses/data/sorted_set/get_scores.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/sorted_set/increment_score.py` & `momento-1.7.0/src/momento/responses/data/sorted_set/increment_score.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/sorted_set/put_element.py` & `momento-1.7.0/src/momento/responses/data/sorted_set/put_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/sorted_set/put_elements.py` & `momento-1.7.0/src/momento/responses/data/sorted_set/put_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/sorted_set/remove_element.py` & `momento-1.7.0/src/momento/responses/data/sorted_set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/data/sorted_set/remove_elements.py` & `momento-1.7.0/src/momento/responses/data/sorted_set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/mixins.py` & `momento-1.7.0/src/momento/responses/mixins.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/responses/response.py` & `momento-1.7.0/src/momento/responses/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,7 +122,11 @@
 
 class CacheResponse(Response):
     ...
 
 
 class ControlResponse(Response):
     ...
+
+
+class PubsubResponse(Response):
+    ...
```

### Comparing `momento-1.6.1/src/momento/retry/default_eligibility_strategy.py` & `momento-1.7.0/src/momento/retry/default_eligibility_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/retry/fixed_count_retry_strategy.py` & `momento-1.7.0/src/momento/retry/fixed_count_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.1/src/momento/typing.py` & `momento-1.7.0/src/momento/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import Iterable, List, Mapping, Set, Union
 
 TCacheName = str
+TTopicName = str
 
 TMomentoValue = Union[str, bytes]
 
 # Scalar Types
 TScalarKey = Union[str, bytes]
 TScalarValue = TMomentoValue
```

### Comparing `momento-1.6.1/setup.py` & `momento-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,32 +21,33 @@
  'momento.responses.control.signing_key',
  'momento.responses.data',
  'momento.responses.data.dictionary',
  'momento.responses.data.list',
  'momento.responses.data.scalar',
  'momento.responses.data.set',
  'momento.responses.data.sorted_set',
+ 'momento.responses.pubsub',
  'momento.retry']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['grpcio>=1.46.0,<2.0.0',
- 'momento-wire-types>=0.64,<0.65',
+ 'momento-wire-types>=0.67,<0.68',
  'pyjwt>=2.4.0,<3.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4']}
 
 setup_kwargs = {
     'name': 'momento',
-    'version': '1.6.1',
+    'version': '1.7.0',
     'description': 'SDK for Momento',
-    'long_description': '<head>\n  <meta name="Momento Python Client Library Documentation" content="Python client software development kit for Momento Cache">\n</head>\n<img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>\n\n[![project status](https://momentohq.github.io/standards-and-practices/badges/project-status-official.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n[![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n\n# Momento Python Client Library\n\nMomento Cache is a fast, simple, pay-as-you-go caching solution without any of the operational overhead\nrequired by traditional caching solutions.  This repo contains the source code for the Momento Python client library.\n\nTo get started with Momento you will need a Momento Auth Token. You can get one from the [Momento Console](https://console.gomomento.com).\n\n* Website: [https://www.gomomento.com/](https://www.gomomento.com/)\n* Momento Documentation: [https://docs.momentohq.com/](https://docs.momentohq.com/)\n* Getting Started: [https://docs.momentohq.com/getting-started](https://docs.momentohq.com/getting-started)\n* Python SDK Documentation: [https://docs.momentohq.com/develop/sdks/python](https://docs.momentohq.com/develop/sdks/python)\n* Discuss: [Momento Discord](https://discord.gg/3HkAKjUZGq)\n\n## Packages\n\nThe Momento Python SDK package is available on pypi: [momento](https://pypi.org/project/momento/).\n\n## Usage\n\nThe examples below require an environment variable named MOMENTO_AUTH_TOKEN which must\nbe set to a valid [Momento authentication token](https://docs.momentohq.com/docs/getting-started#obtain-an-auth-token).\n\nPython 3.10 introduced the `match` statement, which allows for [structural pattern matching on objects](https://peps.python.org/pep-0636/#adding-a-ui-matching-objects).\nIf you are running python 3.10 or greater, here is a quickstart you can use in your own project:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache, ListCaches\n\ncache_client = CacheClient(\n    Configurations.Laptop.v1(),\n    CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),\n    timedelta(seconds=60)\n)\n\ncreate_cache_response = cache_client.create_cache("cache")\nset_response = cache_client.set("cache", "my-key", "my-value")\nget_response = cache_client.get(_CACHE_NAME, _KEY)\nmatch get_response:\n    case CacheGet.Hit() as hit:\n        print(f"Got value: {hit.value_string}")\n    case _:\n        print(f"Response was not a hit: {get_response}")\n\n```\n\nThe above code uses [structural pattern matching](https://peps.python.org/pep-0636/), a feature introduced in Python 3.10.\nUsing a Python version less than 3.10? No problem. Here is the same example compatible across all versions of Python:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\ncache_client = CacheClient(\n    configuration=Configurations.Laptop.v1(),\n    credential_provider=CredentialProvider.from_environment_variable(\'MOMENTO_AUTH_TOKEN\'),\n    default_ttl=timedelta(seconds=60)\n)\ncache_client.create_cache("cache")\ncache_client.set("cache", "myKey", "myValue")\nget_response = cache_client.get("cache", "myKey")\nif isinstance(get_response, CacheGet.Hit):\n    print(f"Got value: {get_response.value_string}")\n\n```\n\n## Getting Started and Documentation\n\nDocumentation is available on the [Momento Docs website](https://docs.momentohq.com).\n\n## Examples\n\nWorking example projects, with all required build configuration files, are available for both Python 3.10 and up\nand Python versions before 3.10:\n\n* [Python 3.10+ examples](./examples/py310)\n* [Pre-3.10 Python examples](./examples/prepy310)\n\n## Developing\n\nIf you are interested in contributing to the SDK, please see the [CONTRIBUTING](./CONTRIBUTING.md) docs.\n\n----------------------------------------------------------------------------------------\nFor more info, visit our website at [https://gomomento.com](https://gomomento.com)!\n',
+    'long_description': '<head>\n  <meta name="Momento Python Client Library Documentation" content="Python client software development kit for Momento Cache">\n</head>\n<img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>\n\n[![project status](https://momentohq.github.io/standards-and-practices/badges/project-status-official.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n[![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n\n# Momento Python Client Library\n\nMomento Cache is a fast, simple, pay-as-you-go caching solution without any of the operational overhead\nrequired by traditional caching solutions.  This repo contains the source code for the Momento Python client library.\n\nTo get started with Momento you will need a Momento Auth Token. You can get one from the [Momento Console](https://console.gomomento.com).\n\n* Website: [https://www.gomomento.com/](https://www.gomomento.com/)\n* Momento Documentation: [https://docs.momentohq.com/](https://docs.momentohq.com/)\n* Getting Started: [https://docs.momentohq.com/getting-started](https://docs.momentohq.com/getting-started)\n* Python SDK Documentation: [https://docs.momentohq.com/develop/sdks/python](https://docs.momentohq.com/develop/sdks/python)\n* Discuss: [Momento Discord](https://discord.gg/3HkAKjUZGq)\n\n## Packages\n\nThe Momento Python SDK package is available on pypi: [momento](https://pypi.org/project/momento/).\n\n## Usage\n\nThe examples below require an environment variable named MOMENTO_AUTH_TOKEN which must\nbe set to a valid [Momento authentication token](https://docs.momentohq.com/docs/getting-started#obtain-an-auth-token).\n\nPython 3.10 introduced the `match` statement, which allows for [structural pattern matching on objects](https://peps.python.org/pep-0636/#adding-a-ui-matching-objects).\nIf you are running python 3.10 or greater, here is a quickstart you can use in your own project:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache, ListCaches\n\ncache_client = CacheClient(\n    Configurations.Laptop.v1(),\n    CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),\n    timedelta(seconds=60)\n)\n\ncache_client.create_cache("cache")\ncache_client.set("cache", "my-key", "my-value")\nget_response = cache_client.get("cache", "my-key")\nmatch get_response:\n    case CacheGet.Hit() as hit:\n        print(f"Got value: {hit.value_string}")\n    case _:\n        print(f"Response was not a hit: {get_response}")\n\n```\n\nThe above code uses [structural pattern matching](https://peps.python.org/pep-0636/), a feature introduced in Python 3.10.\nUsing a Python version less than 3.10? No problem. Here is the same example compatible across all versions of Python:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\ncache_client = CacheClient(\n    configuration=Configurations.Laptop.v1(),\n    credential_provider=CredentialProvider.from_environment_variable(\'MOMENTO_AUTH_TOKEN\'),\n    default_ttl=timedelta(seconds=60)\n)\ncache_client.create_cache("cache")\ncache_client.set("cache", "myKey", "myValue")\nget_response = cache_client.get("cache", "myKey")\nif isinstance(get_response, CacheGet.Hit):\n    print(f"Got value: {get_response.value_string}")\n\n```\n\n## Getting Started and Documentation\n\nDocumentation is available on the [Momento Docs website](https://docs.momentohq.com).\n\n## Examples\n\nWorking example projects, with all required build configuration files, are available for both Python 3.10 and up\nand Python versions before 3.10:\n\n* [Python 3.10+ examples](./examples/py310)\n* [Pre-3.10 Python examples](./examples/prepy310)\n\n## Developing\n\nIf you are interested in contributing to the SDK, please see the [CONTRIBUTING](./CONTRIBUTING.md) docs.\n\n----------------------------------------------------------------------------------------\nFor more info, visit our website at [https://gomomento.com](https://gomomento.com)!\n',
     'author': 'Momento',
     'author_email': 'hello@momentohq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gomomento.com',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `momento-1.6.1/PKG-INFO` & `momento-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momento
-Version: 1.6.1
+Version: 1.7.0
 Summary: SDK for Momento
 Home-page: https://gomomento.com
 License: Apache-2.0
 Keywords: Momento,caching,key-value store,serverless
 Author: Momento
 Author-email: hello@momentohq.com
 Requires-Python: >=3.7,<4.0
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Typing :: Typed
 Requires-Dist: grpcio (>=1.46.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4) ; python_version < "3.8"
-Requires-Dist: momento-wire-types (>=0.64,<0.65)
+Requires-Dist: momento-wire-types (>=0.67,<0.68)
 Requires-Dist: pyjwt (>=2.4.0,<3.0.0)
 Project-URL: Documentation, https://docs.momentohq.com/
 Project-URL: Repository, https://github.com/momentohq/client-sdk-python
 Description-Content-Type: text/markdown
 
 <head>
   <meta name="Momento Python Client Library Documentation" content="Python client software development kit for Momento Cache">
@@ -72,17 +72,17 @@
 
 cache_client = CacheClient(
     Configurations.Laptop.v1(),
     CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),
     timedelta(seconds=60)
 )
 
-create_cache_response = cache_client.create_cache("cache")
-set_response = cache_client.set("cache", "my-key", "my-value")
-get_response = cache_client.get(_CACHE_NAME, _KEY)
+cache_client.create_cache("cache")
+cache_client.set("cache", "my-key", "my-value")
+get_response = cache_client.get("cache", "my-key")
 match get_response:
     case CacheGet.Hit() as hit:
         print(f"Got value: {hit.value_string}")
     case _:
         print(f"Response was not a hit: {get_response}")
 
 ```
```

