# Comparing `tmp/daisyfl-0.4.7.tar.gz` & `tmp/daisyfl-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daisyfl-0.4.7.tar", max compression
+gzip compressed data, was "daisyfl-0.4.8.tar", max compression
```

## Comparing `daisyfl-0.4.7.tar` & `daisyfl-0.4.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    11358 2023-07-12 05:42:59.159463 daisyfl-0.4.7/LICENSE
--rw-r--r--   0        0        0     1158 2023-07-12 05:42:59.159463 daisyfl-0.4.7/README.md
--rw-r--r--   0        0        0     3661 2023-07-12 05:44:16.091264 daisyfl-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     1093 2023-07-12 05:42:59.159463 daisyfl-0.4.7/src/py/daisyfl/__init__.py
--rw-r--r--   0        0        0     1171 2023-07-12 05:42:59.159463 daisyfl-0.4.7/src/py/daisyfl/client/__init__.py
--rw-r--r--   0        0        0     9951 2023-07-12 05:42:59.159463 daisyfl-0.4.7/src/py/daisyfl/client/app.py
--rw-r--r--   0        0        0     3733 2023-07-12 05:42:59.159463 daisyfl-0.4.7/src/py/daisyfl/client/client.py
--rw-r--r--   0        0        0     1363 2023-07-12 05:42:59.159463 daisyfl-0.4.7/src/py/daisyfl/client/client_api_handler.py
--rw-r--r--   0        0        0     3780 2023-07-12 05:42:59.159463 daisyfl-0.4.7/src/py/daisyfl/client/client_operator_manager.py
--rw-r--r--   0        0        0     3367 2023-07-12 05:42:59.159463 daisyfl-0.4.7/src/py/daisyfl/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      714 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/client/grpc_client/__init__.py
--rw-r--r--   0        0        0    10038 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/client/grpc_client/connection.py
--rw-r--r--   0        0        0     6704 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/client/grpc_client/message_handler.py
--rw-r--r--   0        0        0     5084 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/client/numpy_client.py
--rw-r--r--   0        0        0     4998 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/client/trainer.py
--rw-r--r--   0        0        0     1663 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/client/zone_client.py
--rw-r--r--   0        0        0     5644 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/common/__init__.py
--rw-r--r--   0        0        0     1830 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/common/dp.py
--rw-r--r--   0        0        0     3482 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/common/logger.py
--rw-r--r--   0        0        0     1421 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/common/metadata.py
--rw-r--r--   0        0        0     3938 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/common/parameter.py
--rw-r--r--   0        0        0    16903 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/common/serde.py
--rw-r--r--   0        0        0     4044 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/common/typing.py
--rw-r--r--   0        0        0        0 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/base/__init__.py
--rw-r--r--   0        0        0     1162 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/base/client_logic.py
--rw-r--r--   0        0        0     5700 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/base/server_logic.py
--rw-r--r--   0        0        0        0 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/base_async/__init__.py
--rw-r--r--   0        0        0     1162 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/base_async/client_logic.py
--rw-r--r--   0        0        0     5383 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/base_async/server_logic.py
--rw-r--r--   0        0        0     1987 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/msg_demo/client_logic.py
--rw-r--r--   0        0        0      381 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/msg_demo/msg.py
--rw-r--r--   0        0        0     5483 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/msg_demo/server_logic.py
--rw-r--r--   0        0        0      961 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
--rw-r--r--   0        0        0     5848 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
--rw-r--r--   0        0        0    12137 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/sec_agg/client_logic.py
--rw-r--r--   0        0        0     1755 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/sec_agg/common.py
--rw-r--r--   0        0        0    10070 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/sec_agg/primitives.py
--rw-r--r--   0        0        0    22268 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/sec_agg/server_logic.py
--rw-r--r--   0        0        0     1456 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/__init__.py
--rw-r--r--   0        0        0     3016 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/aggregate.py
--rw-r--r--   0        0        0     4538 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     5095 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     6134 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6993 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7245 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedadam.py
--rw-r--r--   0        0        0    13054 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedasync.py
--rw-r--r--   0        0        0    12396 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedavg.py
--rw-r--r--   0        0        0    10915 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedavg_android.py
--rw-r--r--   0        0        0     9115 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedavgm.py
--rw-r--r--   0        0        0     5513 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedopt.py
--rw-r--r--   0        0        0     7263 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedyogi.py
--rw-r--r--   0        0        0    10952 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/qfedavg.py
--rw-r--r--   0        0        0     7867 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/strategy/strategy.py
--rw-r--r--   0        0        0      826 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/utils/__init__.py
--rw-r--r--   0        0        0     6979 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/operator/utils/op_tools.py
--rw-r--r--   0        0        0      676 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/proto/__init__.py
--rw-r--r--   0        0        0    70900 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/proto/transport_pb2.py
--rw-r--r--   0        0        0    25816 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2631 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      781 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0     1064 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/__init__.py
--rw-r--r--   0        0        0     5085 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/app.py
--rw-r--r--   0        0        0     7809 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/client_manager.py
--rw-r--r--   0        0        0     2371 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/client_proxy.py
--rw-r--r--   0        0        0      714 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/grpc_server/__init__.py
--rw-r--r--   0        0        0    12768 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
--rw-r--r--   0        0        0     6827 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/grpc_server/grpc_bridge.py
--rw-r--r--   0        0        0     4459 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
--rw-r--r--   0        0        0    11290 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/grpc_server/grpc_server.py
--rw-r--r--   0        0        0     3626 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/history.py
--rw-r--r--   0        0        0    12168 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/server.py
--rw-r--r--   0        0        0     6432 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/server_api_handler.py
--rw-r--r--   0        0        0     4560 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/server_operator_manager.py
--rw-r--r--   0        0        0    13571 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/server/task_manager.py
--rw-r--r--   0        0        0     1273 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/simulation/__init__.py
--rw-r--r--   0        0        0     7335 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/simulation/app.py
--rw-r--r--   0        0        0      727 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     4661 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0      859 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-07-12 05:42:59.163463 daisyfl-0.4.7/src/py/daisyfl/utils/dynamic_loader.py
--rw-r--r--   0        0        0     2765 2023-07-12 05:44:33.259159 daisyfl-0.4.7/setup.py
--rw-r--r--   0        0        0     3286 2023-07-12 05:44:33.259428 daisyfl-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 13:27:28.582708 daisyfl-0.4.8/LICENSE
+-rw-r--r--   0        0        0     1158 2023-07-14 13:27:28.582708 daisyfl-0.4.8/README.md
+-rw-r--r--   0        0        0     3661 2023-07-14 13:27:55.562673 daisyfl-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1093 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/__init__.py
+-rw-r--r--   0        0        0     1171 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/__init__.py
+-rw-r--r--   0        0        0     9951 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/app.py
+-rw-r--r--   0        0        0     3733 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/client.py
+-rw-r--r--   0        0        0     1363 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/client_api_handler.py
+-rw-r--r--   0        0        0     3780 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/client_operator_manager.py
+-rw-r--r--   0        0        0     3367 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      714 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0    10038 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/connection.py
+-rw-r--r--   0        0        0     6704 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/message_handler.py
+-rw-r--r--   0        0        0     5084 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/numpy_client.py
+-rw-r--r--   0        0        0     4998 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/trainer.py
+-rw-r--r--   0        0        0     1663 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/zone_client.py
+-rw-r--r--   0        0        0     5644 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/common/__init__.py
+-rw-r--r--   0        0        0     1830 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/common/dp.py
+-rw-r--r--   0        0        0     3482 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/common/logger.py
+-rw-r--r--   0        0        0     1421 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/common/metadata.py
+-rw-r--r--   0        0        0     3938 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/common/parameter.py
+-rw-r--r--   0        0        0    16903 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/common/serde.py
+-rw-r--r--   0        0        0     4044 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/common/typing.py
+-rw-r--r--   0        0        0        0 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base/__init__.py
+-rw-r--r--   0        0        0     1162 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base/client_logic.py
+-rw-r--r--   0        0        0     5700 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base/server_logic.py
+-rw-r--r--   0        0        0        0 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base_async/__init__.py
+-rw-r--r--   0        0        0     1162 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base_async/client_logic.py
+-rw-r--r--   0        0        0     5383 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base_async/server_logic.py
+-rw-r--r--   0        0        0     1987 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/client_logic.py
+-rw-r--r--   0        0        0      381 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/msg.py
+-rw-r--r--   0        0        0     5483 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/server_logic.py
+-rw-r--r--   0        0        0      961 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
+-rw-r--r--   0        0        0     5848 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
+-rw-r--r--   0        0        0    12137 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/client_logic.py
+-rw-r--r--   0        0        0     1755 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/common.py
+-rw-r--r--   0        0        0    10070 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/primitives.py
+-rw-r--r--   0        0        0    22268 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/server_logic.py
+-rw-r--r--   0        0        0     1456 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/__init__.py
+-rw-r--r--   0        0        0     3016 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/aggregate.py
+-rw-r--r--   0        0        0     4538 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     5095 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     6134 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6993 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7245 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedadam.py
+-rw-r--r--   0        0        0    13054 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedasync.py
+-rw-r--r--   0        0        0    12396 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavg.py
+-rw-r--r--   0        0        0    10915 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     9115 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavgm.py
+-rw-r--r--   0        0        0     5513 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedopt.py
+-rw-r--r--   0        0        0     7263 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedyogi.py
+-rw-r--r--   0        0        0    10952 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7867 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/strategy.py
+-rw-r--r--   0        0        0      826 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/utils/__init__.py
+-rw-r--r--   0        0        0     6979 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/utils/op_tools.py
+-rw-r--r--   0        0        0      676 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/proto/__init__.py
+-rw-r--r--   0        0        0    70900 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2.py
+-rw-r--r--   0        0        0    25816 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2631 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      781 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1064 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/__init__.py
+-rw-r--r--   0        0        0     5085 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/app.py
+-rw-r--r--   0        0        0     7809 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/client_manager.py
+-rw-r--r--   0        0        0     2371 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/client_proxy.py
+-rw-r--r--   0        0        0      714 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/__init__.py
+-rw-r--r--   0        0        0    12768 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
+-rw-r--r--   0        0        0     6827 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_bridge.py
+-rw-r--r--   0        0        0     4459 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11290 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0     3626 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/history.py
+-rw-r--r--   0        0        0    11871 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/server.py
+-rw-r--r--   0        0        0     7341 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/server_api_handler.py
+-rw-r--r--   0        0        0     4560 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/server_operator_manager.py
+-rw-r--r--   0        0        0    13696 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/task_manager.py
+-rw-r--r--   0        0        0     1273 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/simulation/__init__.py
+-rw-r--r--   0        0        0     7335 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     4661 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0      859 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/utils/dynamic_loader.py
+-rw-r--r--   0        0        0     2765 2023-07-14 13:28:14.933335 daisyfl-0.4.8/setup.py
+-rw-r--r--   0        0        0     3286 2023-07-14 13:28:14.933610 daisyfl-0.4.8/PKG-INFO
```

### Comparing `daisyfl-0.4.7/LICENSE` & `daisyfl-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/README.md` & `daisyfl-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/pyproject.toml` & `daisyfl-0.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "daisyfl"
-version = "0.4.7"
+version = "0.4.8"
 description = "Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing"
 license = "Apache-2.0"
 authors = ["tcfwbper <b05208031@ntu.edu.tw>"]
 readme = "README.md"
 homepage = "https://github.com/Intelligent-Systems-Lab/daisy"
 repository = "https://github.com/Intelligent-Systems-Lab/daisy"
 documentation = "https://github.com/Intelligent-Systems-Lab/daisy/tree/main/doc/daisy"
```

### Comparing `daisyfl-0.4.7/src/py/daisyfl/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/app.py` & `daisyfl-0.4.8/src/py/daisyfl/client/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/client.py` & `daisyfl-0.4.8/src/py/daisyfl/client/client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/client_api_handler.py` & `daisyfl-0.4.8/src/py/daisyfl/client/client_api_handler.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/client_operator_manager.py` & `daisyfl-0.4.8/src/py/daisyfl/client/client_operator_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/dpfedavg_numpy_client.py` & `daisyfl-0.4.8/src/py/daisyfl/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/grpc_client/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/grpc_client/connection.py` & `daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/grpc_client/message_handler.py` & `daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/message_handler.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/numpy_client.py` & `daisyfl-0.4.8/src/py/daisyfl/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/trainer.py` & `daisyfl-0.4.8/src/py/daisyfl/client/trainer.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/client/zone_client.py` & `daisyfl-0.4.8/src/py/daisyfl/client/zone_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/common/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/common/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/common/dp.py` & `daisyfl-0.4.8/src/py/daisyfl/common/dp.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/common/logger.py` & `daisyfl-0.4.8/src/py/daisyfl/common/logger.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/common/metadata.py` & `daisyfl-0.4.8/src/py/daisyfl/common/metadata.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/common/parameter.py` & `daisyfl-0.4.8/src/py/daisyfl/common/parameter.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/common/serde.py` & `daisyfl-0.4.8/src/py/daisyfl/common/serde.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/common/typing.py` & `daisyfl-0.4.8/src/py/daisyfl/common/typing.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/base/client_logic.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/base/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/base/server_logic.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/base/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/base_async/client_logic.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/base_async/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/base_async/server_logic.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/base_async/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/msg_demo/client_logic.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/msg_demo/server_logic.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/msg_demo/zone_client_logic.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/zone_client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/msg_demo/zone_server_logic.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/zone_server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/sec_agg/client_logic.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/sec_agg/common.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/common.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/sec_agg/primitives.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/primitives.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/sec_agg/server_logic.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/aggregate.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedadagrad.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedadam.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedasync.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedasync.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedavg.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedavg_android.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedavgm.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedopt.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/fedyogi.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/qfedavg.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/strategy/strategy.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/utils/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/operator/utils/op_tools.py` & `daisyfl-0.4.8/src/py/daisyfl/operator/utils/op_tools.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/proto/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/proto/transport_pb2.py` & `daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/proto/transport_pb2.pyi` & `daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/proto/transport_pb2_grpc.py` & `daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/proto/transport_pb2_grpc.pyi` & `daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/server/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/app.py` & `daisyfl-0.4.8/src/py/daisyfl/server/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/client_manager.py` & `daisyfl-0.4.8/src/py/daisyfl/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/client_proxy.py` & `daisyfl-0.4.8/src/py/daisyfl/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/grpc_server/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/grpc_server/flower_service_servicer.py` & `daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/grpc_server/grpc_bridge.py` & `daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py` & `daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/grpc_server/grpc_server.py` & `daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_server.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/history.py` & `daisyfl-0.4.8/src/py/daisyfl/server/history.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/server.py` & `daisyfl-0.4.8/src/py/daisyfl/server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,20 +67,19 @@
 # TODO: update CurrentReturns by number of client
 
 class SubtaskManager:
     def __init__(self,) -> None:
         self.subtasks: Dict[int, CurrentReturns] = {}
         self.queues: Dict[int, Queue] = {}
         self.client_previous_subtask: Dict[str, int] = {}
-        self._lock_subtask_id: Lock = Lock()
-        self._lock_previous_subtask: Lock = Lock()
+        self._lock: Lock = Lock()
         self._subtask_num = 0
     
     def subtask_id_generator(self,) -> int:
-        with self._lock_subtask_id:
+        with self._lock:
             tmp = self._subtask_num
             self._subtask_num += 1
         return tmp
     
     def register_subtask(
         self, subtask_id: int, 
         client_instructions: List[Tuple[ClientProxy, FitIns]],
@@ -91,57 +90,54 @@
             selected=len(client_instructions),
             results_num=0,
             failures_num=0,
             cnd=Condition(),
         )
         # queue
         self.queues[subtask_id] = Queue()
-        with self._lock_previous_subtask:
         # update client_previoud_subtask
-            for item in client_instructions:
-                cid = item[0].cid
-                if self.client_previous_subtask.__contains__(cid):
-                    pre_subtask = self.client_previous_subtask[cid]
-                    self.subtasks[pre_subtask].failures_num += 1
-                    del self.client_previous_subtask[cid]
-                    self.subtasks[pre_subtask].cnd.notify_all()
-                self.client_previous_subtask[cid] = subtask_id
+        for item in client_instructions:
+            cid = item[0].cid
+            if self.client_previous_subtask.__contains__(cid):
+                pre_subtask = self.client_previous_subtask[cid]
+                self.subtasks[pre_subtask].failures_num += 1
+                del self.client_previous_subtask[cid]
+                self.subtasks[pre_subtask].cnd.notify_all()
+            self.client_previous_subtask[cid] = subtask_id
         # timeout
         Timer(timeout, self.subtask_timeout, subtask_id)
 
     def unregister_subtask(self, subtask_id: int) -> None:
         del self.subtasks[subtask_id]
         del self.queues[subtask_id]
-        with self._lock_previous_subtask:
-            cid_list = self.client_previous_subtask.keys()
-            for cid in cid_list:
-                if self.client_previous_subtask[cid] == subtask_id:
-                    del self.client_previous_subtask[cid]
+        cid_list = list(self.client_previous_subtask.keys())
+        for cid in cid_list:
+            if self.client_previous_subtask[cid] == subtask_id:
+                del self.client_previous_subtask[cid]
         gc.collect()
         return
 
     def submit_subtask(
         self, result: Tuple[ClientProxy, Union[FitRes, EvaluateRes]],
     ) -> None:
         client_proxy, res = result
-        with self._lock_previous_subtask:
-            if (not self.client_previous_subtask.__contains__(client_proxy.cid)):
-                return
-            subtask_id = self.client_previous_subtask[client_proxy.cid]
-            if (not self.subtasks.__contains__(subtask_id)):
-                return
-            # Check result status code
-            if res.status.code == Code.OK:
-                result[1].config[CID] = result[0].cid
-                self.subtasks[subtask_id].results_num += 1
-                self.queues[subtask_id].put(result)
-            # Not successful, client returned a result where the status code is not OK
-            else:
-                self.subtasks[subtask_id].failures_num += 1
-            del self.client_previous_subtask[client_proxy.cid]
+        if (not self.client_previous_subtask.__contains__(client_proxy.cid)):
+            return
+        subtask_id = self.client_previous_subtask[client_proxy.cid]
+        if (not self.subtasks.__contains__(subtask_id)):
+            return
+        # Check result status code
+        if res.status.code == Code.OK:
+            result[1].config[CID] = result[0].cid
+            self.subtasks[subtask_id].results_num += 1
+            self.queues[subtask_id].put(result)
+        # Not successful, client returned a result where the status code is not OK
+        else:
+            self.subtasks[subtask_id].failures_num += 1
+        del self.client_previous_subtask[client_proxy.cid]
         with self.subtasks[subtask_id].cnd:
             self.subtasks[subtask_id].cnd.notify_all()
         return
         
     def get_current_returns(self, subtask_id: int) -> CurrentReturns:
         return self.subtasks[subtask_id]
```

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/server_api_handler.py` & `daisyfl-0.4.8/src/py/daisyfl/server/server_api_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,14 +106,26 @@
                         res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
                             "client_id", "get_selected_client_ids_for_this_round", "gauge", labels, 87
                         )                        
                         if client_metrics[METRICS].__contains__(ACCURACY):
                             res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
                                 "accuracy_individual", "accuracy_of_the_individual_clients", "gauge", labels, client_metrics[METRICS][ACCURACY]
                             )
+                        if client_metrics[METRICS].__contains__("mloss"):
+                            # yolo
+                            loss_list = client_metrics[METRICS]["mloss"] # [lbox, lobj, lcls]
+                            res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
+                                "loss_box", "loss_box_of_the_individual_clients", "gauge", labels, loss_list[0]
+                            )
+                            res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
+                                "loss_object", "loss_object_of_the_individual_clients", "gauge", labels, loss_list[1]
+                            )
+                            res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
+                                "loss_class", "loss_class_of_the_individual_clients", "gauge", labels, loss_list[2]
+                            )
                         res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
                             "loss_individual", "loss_of_the_individual_clients", "gauge", labels, client_metrics[LOSS]
                         )
             print(res)
             response = make_response(res)
             response.headers["content-type"] = "text/plain"
             return response
```

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/server_operator_manager.py` & `daisyfl-0.4.8/src/py/daisyfl/server/server_operator_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/server/task_manager.py` & `daisyfl-0.4.8/src/py/daisyfl/server/task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,17 @@
             )
         else:
             # fitting task
             subtask_start_time = timeit.default_timer()
             parameters, report = self.server_operator_manager.fit_round(parameters, task)
             meta_task.subtask_returns[SUBTASK_TIMER] = timeit.default_timer() - subtask_start_time
             meta_task.subtask_returns[TIMER_ROUND] = report.config[CURRENT_ROUND]
+            
+            if self.type == Type.MASTER:
+                np.save(task.config[MODEL_PATH], np.array(parameters))
 
         # update subtask returns
         if report.config[METRICS].__contains__(PARTICIPATION):
             meta_task.subtask_returns[CURRENT_ROUND] = task.config[CURRENT_ROUND]
             meta_task.subtask_returns[PARTICIPATION] = report.config[METRICS][PARTICIPATION]
             if self.type == Type.MASTER:
                 del report.config[METRICS][PARTICIPATION]
```

### Comparing `daisyfl-0.4.7/src/py/daisyfl/simulation/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/simulation/app.py` & `daisyfl-0.4.8/src/py/daisyfl/simulation/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/simulation/ray_transport/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py` & `daisyfl-0.4.8/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/src/py/daisyfl/utils/__init__.py` & `daisyfl-0.4.8/src/py/daisyfl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.7/setup.py` & `daisyfl-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4.0.0,<5.0.0'],
  'simulation': ['ray[default]>=2.0.0,<2.1.0']}
 
 setup_kwargs = {
     'name': 'daisyfl',
-    'version': '0.4.7',
+    'version': '0.4.8',
     'description': 'Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing',
     'long_description': "# Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing\n\n\n## dev mode (virtual environment)\n### 1. clone the source code\n```\ngit clone https://github.com/Intelligent-Systems-Lab/daisy\n```\n### 2. build up environment\nprepare and activate your virtual environment (python=3.8^)\n```\ncd daisy\n./dev/bootstrap.sh\n```\n### develop<br>\n### setup examples\ndon't overwrite daisyfl dependency in this step.<br>\n```\ncd <example_path>\npip install <pkgs_for_your_example>\n```\n### 5. run examples\n\n## dev mode (docker)\n### 1. clone the source code\n```\ngit clone https://github.com/Intelligent-Systems-Lab/daisy\n```\n### 2. build up environment\n```\ndocker run -it -v <daisy_source_code>:/root/daisy tcfwbper/daisyfl-dev:<version_tag> /bin/bash\n```\n### 3. develop<br>\n### 4. setup examples<br>\ndon't overwrite daisyfl dependency in this step.<br>\n```\ndocker attach <container_id>\n```\n```\ncd <example_path> && conda activate daisy\npip install <pkgs_for_your_example>\n```\n### 5. run examples\n\n## user mode\n### 1. install daisyfl\n```\npip install <daisyfl_version>\n```\n### 2. setup examples\n```\npip install <pkgs_for_your_example>\n```\n### 3. run examples",
     'author': 'tcfwbper',
     'author_email': 'b05208031@ntu.edu.tw',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Intelligent-Systems-Lab/daisy',
```

### Comparing `daisyfl-0.4.7/PKG-INFO` & `daisyfl-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daisyfl
-Version: 0.4.7
+Version: 0.4.8
 Summary: Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing
 Home-page: https://github.com/Intelligent-Systems-Lab/daisy
 License: Apache-2.0
 Author: tcfwbper
 Author-email: b05208031@ntu.edu.tw
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

