# Comparing `tmp/flwr_nightly-1.5.0.dev20230711.tar.gz` & `tmp/flwr_nightly-1.5.0.dev20230712.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.5.0.dev20230711.tar", max compression
+gzip compressed data, was "flwr_nightly-1.5.0.dev20230712.tar", max compression
```

## Comparing `flwr_nightly-1.5.0.dev20230711.tar` & `flwr_nightly-1.5.0.dev20230712.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0    11358 2023-07-11 23:03:35.621309 flwr_nightly-1.5.0.dev20230711/LICENSE
--rw-r--r--   0        0        0    10721 2023-07-11 23:03:35.621309 flwr_nightly-1.5.0.dev20230711/README.md
--rw-r--r--   0        0        0     5221 2023-07-11 23:04:00.681469 flwr_nightly-1.5.0.dev20230711/pyproject.toml
--rw-r--r--   0        0        0      952 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    14126 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     7677 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     7209 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4446 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      745 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     6823 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0      712 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5077 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1685 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5318 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     8448 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1875 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     1113 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0      884 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1791 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1889 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3459 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16315 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7805 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      809 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     4826 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     3906 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     4877 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/driver/driver_client_manager.py
--rw-r--r--   0        0        0     5653 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0      676 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     7295 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     6182 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     7505 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2183 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     8232 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0    10889 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-11 23:03:35.913310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    26333 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6120 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2227 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1054 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      728 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     4467 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
--rw-r--r--   0        0        0     5686 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6408 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4650 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11501 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0     6313 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
--rw-r--r--   0        0        0      751 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     2546 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      724 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2876 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      728 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     3686 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4897 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15958 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6774 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19294 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4833 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1647 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1667 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     6099 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4654 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     6995 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5893 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6740 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7014 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11522 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9991 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8286 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2708 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5428 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7126 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     6026 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     3519 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7079 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6343 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10154 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5478 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4940 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7762 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5471 2023-07-11 23:03:35.917310 flwr_nightly-1.5.0.dev20230711/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    12946 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230711/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-12 23:02:26.569543 flwr_nightly-1.5.0.dev20230712/LICENSE
+-rw-r--r--   0        0        0    10721 2023-07-12 23:02:26.569543 flwr_nightly-1.5.0.dev20230712/README.md
+-rw-r--r--   0        0        0     5221 2023-07-12 23:02:44.681952 flwr_nightly-1.5.0.dev20230712/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    14058 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     7677 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     7209 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4954 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      745 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     7345 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0      712 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6380 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     4693 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5318 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     9050 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1875 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     1113 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1791 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1889 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3459 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16315 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7805 2023-07-12 23:02:26.829545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      809 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     4826 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/driver/app.py
+-rw-r--r--   0        0        0     3906 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0     4877 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/driver/driver_client_manager.py
+-rw-r--r--   0        0        0     5653 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/driver/driver_client_proxy.py
+-rw-r--r--   0        0        0      676 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7295 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     6182 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     7505 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2183 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8232 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0    10889 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    26333 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6120 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2227 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1054 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     4467 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
+-rw-r--r--   0        0        0     5686 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6408 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4650 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11501 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0     6313 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
+-rw-r--r--   0        0        0      751 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     2546 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      724 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     2876 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      728 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     3686 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0     4897 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0    15958 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6774 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19294 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4833 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1647 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1667 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     6099 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4654 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     6995 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5893 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6740 2023-07-12 23:02:26.833545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7014 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11522 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9991 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8286 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2708 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5428 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7126 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     6026 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     3519 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7079 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6343 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10154 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5478 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4940 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7762 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5471 2023-07-12 23:02:26.837545 flwr_nightly-1.5.0.dev20230712/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    12946 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230712/PKG-INFO
```

### Comparing `flwr_nightly-1.5.0.dev20230711/LICENSE` & `flwr_nightly-1.5.0.dev20230712/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/README.md` & `flwr_nightly-1.5.0.dev20230712/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/pyproject.toml` & `flwr_nightly-1.5.0.dev20230712/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.5.0-dev20230711"
+version = "1.5.0-dev20230712"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
@@ -84,26 +84,26 @@
 flake8 = "==3.9.2"
 pytest = "==7.1.2"
 pytest-cov = "==3.0.0"
 pytest-watch = "==4.2.0"
 grpcio-tools = "==1.48.2"
 mypy-protobuf = "==3.2.0"
 jupyterlab = "==3.6.3"
-rope = "==1.8.0"
+rope = "==1.9.0"
 semver = "==2.13.0"
 sphinx = "==5.3.0"
 myst-parser = "==1.0.0"
 sphinx-design = "==0.4.1"
 sphinx-copybutton = "==0.5.2"
 sphinxcontrib-mermaid = "==0.8.1"
 furo = "==2022.12.7"
 sphinx-reredirects = "==0.1.2"
 nbsphinx = "==0.9.2"
 nbstripout = "==0.6.1"
-ruff = "==0.0.272"
+ruff = "==0.0.277"
 sphinx-argparse = "==0.4.0"
 pipreqs = "==0.4.13"
 mdformat-gfm = "==0.3.5"
 mdformat-frontmatter = "==2.0.1"
 mdformat-beautysh = "==0.1.1"
 mdformat-myst = "==0.1.5"
```

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/app.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -194,22 +194,20 @@
             receive, send, create_node, delete_node = conn
 
             # Register node
             if create_node is not None:
                 create_node()  # pylint: disable=not-callable
 
             while True:
-                server_message = receive()
-                if server_message is None:
+                task_ins = receive()
+                if task_ins is None:
                     time.sleep(3)  # Wait for 3s before asking again
                     continue
-                client_message, sleep_duration, keep_going = handle(
-                    client, server_message
-                )
-                send(client_message)
+                task_res, sleep_duration, keep_going = handle(client, task_ins)
+                send(task_res)
                 if not keep_going:
                     break
 
             # Unregister node
             if delete_node is not None:
                 delete_node()  # pylint: disable=not-callable
```

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/client.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/grpc_client/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Contextmanager for a gRPC streaming channel to the Flower server."""
 
 
+import uuid
 from contextlib import contextmanager
 from logging import DEBUG
 from pathlib import Path
 from queue import Queue
 from typing import Callable, Iterator, Optional, Tuple, Union
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH
 from flwr.common.grpc import create_channel
 from flwr.common.logger import log
+from flwr.proto.node_pb2 import Node
+from flwr.proto.task_pb2 import Task, TaskIns, TaskRes
 from flwr.proto.transport_pb2 import ClientMessage, ServerMessage
 from flwr.proto.transport_pb2_grpc import FlowerServiceStub
 
 # The following flags can be uncommented for debugging. Other possible values:
 # https://github.com/grpc/grpc/blob/master/doc/environment_variables.md
 # import os
 # os.environ["GRPC_VERBOSITY"] = "debug"
@@ -42,16 +45,16 @@
 @contextmanager
 def grpc_connection(
     server_address: str,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[Union[bytes, str]] = None,
 ) -> Iterator[
     Tuple[
-        Callable[[], Optional[ServerMessage]],
-        Callable[[ClientMessage], None],
+        Callable[[], Optional[TaskIns]],
+        Callable[[TaskRes], None],
         Optional[Callable[[], None]],
         Optional[Callable[[], None]],
     ]
 ]:
     """Establish a gRPC connection to a gRPC server.
 
     Parameters
@@ -105,18 +108,30 @@
     queue: Queue[ClientMessage] = Queue(  # pylint: disable=unsubscriptable-object
         maxsize=1
     )
     stub = FlowerServiceStub(channel)
 
     server_message_iterator: Iterator[ServerMessage] = stub.Join(iter(queue.get, None))
 
-    def receive() -> ServerMessage:
-        return next(server_message_iterator)
+    def receive() -> TaskIns:
+        server_message = next(server_message_iterator)
+        return TaskIns(
+            task_id=str(uuid.uuid4()),
+            group_id="",
+            workload_id="",
+            task=Task(
+                producer=Node(node_id=0, anonymous=True),
+                consumer=Node(node_id=0, anonymous=True),
+                ancestry=[],
+                legacy_server_message=server_message,
+            ),
+        )
 
-    def send(msg: ClientMessage) -> None:
+    def send(task_res: TaskRes) -> None:
+        msg = task_res.task.legacy_client_message
         return queue.put(msg, block=False)
 
     try:
         # Yield methods
         yield (receive, send, None, None)
     finally:
         # Make sure to have a final
```

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,31 @@
 
 
 from contextlib import contextmanager
 from logging import DEBUG, ERROR, WARN
 from pathlib import Path
 from typing import Callable, Dict, Iterator, Optional, Tuple, Union, cast
 
-from flwr.client.message_handler.task_handler import get_server_message
+from flwr.client.message_handler.task_handler import (
+    get_task_ins,
+    validate_task_ins,
+    validate_task_res,
+)
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH
 from flwr.common.grpc import create_channel
 from flwr.common.logger import log
 from flwr.proto.fleet_pb2 import (
     CreateNodeRequest,
     DeleteNodeRequest,
     PullTaskInsRequest,
     PushTaskResRequest,
 )
 from flwr.proto.fleet_pb2_grpc import FleetStub
 from flwr.proto.node_pb2 import Node
 from flwr.proto.task_pb2 import Task, TaskIns, TaskRes
-from flwr.proto.transport_pb2 import ClientMessage, ServerMessage
 
 KEY_NODE = "node"
 KEY_TASK_INS = "current_task_ins"
 
 
 def on_channel_state_change(channel_connectivity: str) -> None:
     """Log channel connectivity."""
@@ -49,16 +52,16 @@
     server_address: str,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,  # pylint: disable=W0613
     root_certificates: Optional[
         Union[bytes, str]
     ] = None,  # pylint: disable=unused-argument
 ) -> Iterator[
     Tuple[
-        Callable[[], Optional[ServerMessage]],
-        Callable[[ClientMessage], None],
+        Callable[[], Optional[TaskIns]],
+        Callable[[TaskRes], None],
         Optional[Callable[[], None]],
         Optional[Callable[[], None]],
     ]
 ]:
     """Primitives for request/response-based interaction with a server.
 
     One notable difference to the grpc_connection context manager is that
@@ -128,65 +131,80 @@
             log(ERROR, "Node instance missing")
             return
         node: Node = cast(Node, node_store[KEY_NODE])
 
         delete_node_request = DeleteNodeRequest(node=node)
         stub.DeleteNode(request=delete_node_request)
 
-    def receive() -> Optional[ServerMessage]:
+    def receive() -> Optional[TaskIns]:
         """Receive next task from server."""
         # Get Node
         if node_store[KEY_NODE] is None:
             log(ERROR, "Node instance missing")
             return None
         node: Node = cast(Node, node_store[KEY_NODE])
 
         # Request instructions (task) from server
         request = PullTaskInsRequest(node=node)
         response = stub.PullTaskIns(request=request)
 
-        # Remember the current TaskIns
-        task_ins_server_message_tuple = get_server_message(response)
-        if task_ins_server_message_tuple is None:
-            state[KEY_TASK_INS] = None
-            return None
+        # Get the current TaskIns
+        task_ins: Optional[TaskIns] = get_task_ins(response)
 
-        task_ins, server_message = task_ins_server_message_tuple
+        # Discard the current TaskIns if not valid
+        if task_ins is not None and not validate_task_ins(
+            task_ins, discard_reconnect_ins=True
+        ):
+            task_ins = None
 
         # Remember `task_ins` until `task_res` is available
         state[KEY_TASK_INS] = task_ins
 
-        # Return the ServerMessage
-        return server_message
+        # Return the TaskIns if available
+        return task_ins
 
-    def send(client_message_proto: ClientMessage) -> None:
+    def send(task_res: TaskRes) -> None:
         """Send task result back to server."""
         # Get Node
         if node_store[KEY_NODE] is None:
             log(ERROR, "Node instance missing")
             return
         node: Node = cast(Node, node_store[KEY_NODE])
 
         # Get incoming TaskIns
         if state[KEY_TASK_INS] is None:
             log(ERROR, "No current TaskIns")
             return
         task_ins: TaskIns = cast(TaskIns, state[KEY_TASK_INS])
 
-        # Wrap ClientMessage in TaskRes
-        task_res = TaskRes(
-            task_id="",  # This will be generated by the server
-            group_id=task_ins.group_id,
-            workload_id=task_ins.workload_id,
-            task=Task(
+        # Check if fields to be set are not initialized
+        if not validate_task_res(task_res):
+            state[KEY_TASK_INS] = None
+            log(ERROR, "TaskRes has been initialized accidentally")
+
+        # Fill `group_id` and `workload_id` in TaskRes
+        # Note that protobuf API `protobuf.message.MergeFrom(other_msg)`
+        # does NOT always overwrite fields that are set in `other_msg`.
+        # Please refer to:
+        # https://googleapis.dev/python/protobuf/latest/google/protobuf/message.html
+        task_res.MergeFrom(
+            TaskRes(
+                task_id="",  # This will be generated by the server
+                group_id=task_ins.group_id,
+                workload_id=task_ins.workload_id,
+            )
+        )
+
+        # Fill `producer`, `consumer`, and `ancestry` in Task
+        task_res.task.MergeFrom(
+            Task(
                 producer=node,
                 consumer=task_ins.task.producer,
-                legacy_client_message=client_message_proto,
                 ancestry=[task_ins.task_id],
-            ),
+            )
         )
 
         # Serialize ProtoBuf to bytes
         request = PushTaskResRequest(task_res_list=[task_res])
         _ = stub.PushTaskRes(request)
 
         state[KEY_TASK_INS] = None
```

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/message_handler/message_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,23 +20,57 @@
 from flwr.client.client import (
     Client,
     maybe_call_evaluate,
     maybe_call_fit,
     maybe_call_get_parameters,
     maybe_call_get_properties,
 )
+from flwr.client.message_handler.task_handler import (
+    get_server_message_from_task_ins,
+    wrap_client_message_in_task_res,
+)
 from flwr.common import serde
+from flwr.proto.task_pb2 import TaskIns, TaskRes
 from flwr.proto.transport_pb2 import ClientMessage, Reason, ServerMessage
 
 
 class UnknownServerMessage(Exception):
     """Exception indicating that the received message is unknown."""
 
 
-def handle(
+def handle(client: Client, task_ins: TaskIns) -> Tuple[TaskRes, int, bool]:
+    """Handle incoming TaskIns from the server.
+
+    Parameters
+    ----------
+    client : Client
+        The Client instance provided by the user.
+    task_ins: TaskIns
+        The task instruction coming from the server, to be processed by the client.
+
+    Returns
+    -------
+    task_res: TaskRes
+        The task response that should be returned to the server.
+    sleep_duration : int
+        Number of seconds that the client should disconnect from the server.
+    keep_going : bool
+        Flag that indicates whether the client should continue to process the
+        next message from the server (True) or disconnect and optionally
+        reconnect later (False).
+    """
+    server_msg = get_server_message_from_task_ins(task_ins, exclude_reconnect_ins=False)
+    if server_msg is None:
+        raise NotImplementedError()
+    client_msg, sleep_duration, keep_going = handle_legacy_message(client, server_msg)
+    task_res = wrap_client_message_in_task_res(client_msg)
+    return task_res, sleep_duration, keep_going
+
+
+def handle_legacy_message(
     client: Client, server_msg: ServerMessage
 ) -> Tuple[ClientMessage, int, bool]:
     """Handle incoming messages from the server.
 
     Parameters
     ----------
     client : Client
```

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/client/rest_client/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,27 +16,30 @@
 
 
 import sys
 from contextlib import contextmanager
 from logging import ERROR, INFO, WARN
 from typing import Callable, Dict, Iterator, Optional, Tuple, Union, cast
 
-from flwr.client.message_handler.task_handler import get_server_message
+from flwr.client.message_handler.task_handler import (
+    get_task_ins,
+    validate_task_ins,
+    validate_task_res,
+)
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH
 from flwr.common.constant import MISSING_EXTRA_REST
 from flwr.common.logger import log
 from flwr.proto.fleet_pb2 import (
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
 )
 from flwr.proto.node_pb2 import Node
 from flwr.proto.task_pb2 import Task, TaskIns, TaskRes
-from flwr.proto.transport_pb2 import ClientMessage, ServerMessage
 
 try:
     import requests
 except ModuleNotFoundError:
     sys.exit(MISSING_EXTRA_REST)
 
 
@@ -44,24 +47,25 @@
 
 
 PATH_PULL_TASK_INS: str = "api/v0/fleet/pull-task-ins"
 PATH_PUSH_TASK_RES: str = "api/v0/fleet/push-task-res"
 
 
 @contextmanager
+# pylint: disable-next=too-many-statements
 def http_request_response(
     server_address: str,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,  # pylint: disable=W0613
     root_certificates: Optional[
         Union[bytes, str]
     ] = None,  # pylint: disable=unused-argument
 ) -> Iterator[
     Tuple[
-        Callable[[], Optional[ServerMessage]],
-        Callable[[ClientMessage], None],
+        Callable[[], Optional[TaskIns]],
+        Callable[[TaskRes], None],
         Optional[Callable[[], None]],
         Optional[Callable[[], None]],
     ]
 ]:
     """Primitives for request/response-based interaction with a server.
 
     One notable difference to the grpc_connection context manager is that
@@ -111,15 +115,15 @@
     # Necessary state to link TaskRes to TaskIns
     state: Dict[str, Optional[TaskIns]] = {KEY_TASK_INS: None}
 
     ###########################################################################
     # receive/send functions
     ###########################################################################
 
-    def receive() -> Optional[ServerMessage]:
+    def receive() -> Optional[TaskIns]:
         """Receive next task from server."""
         # Serialize ProtoBuf to bytes
         pull_task_ins_req_proto = PullTaskInsRequest(
             node=Node(node_id=0, anonymous=True),
         )
         pull_task_ins_req_bytes: bytes = pull_task_ins_req_proto.SerializeToString()
 
@@ -152,48 +156,64 @@
             )
             return None
 
         # Deserialize ProtoBuf from bytes
         pull_task_ins_response_proto = PullTaskInsResponse()
         pull_task_ins_response_proto.ParseFromString(res.content)
 
-        # Remember the current TaskIns
-        task_ins_server_message_tuple = get_server_message(pull_task_ins_response_proto)
-        if task_ins_server_message_tuple is None:
-            state[KEY_TASK_INS] = None
-            return None
+        # Get the current TaskIns
+        task_ins: Optional[TaskIns] = get_task_ins(pull_task_ins_response_proto)
 
-        task_ins, server_message = task_ins_server_message_tuple
+        # Discard the current TaskIns if not valid
+        if task_ins is not None and not validate_task_ins(
+            task_ins, discard_reconnect_ins=True
+        ):
+            task_ins = None
 
         # Remember `task_ins` until `task_res` is available
         state[KEY_TASK_INS] = task_ins
 
-        # Return the ServerMessage
-        log(INFO, "[Node] POST /%s: success", PATH_PULL_TASK_INS)
-        return server_message
+        # Return the TaskIns if available
+        if task_ins is not None:
+            log(INFO, "[Node] POST /%s: success", PATH_PULL_TASK_INS)
+        return task_ins
 
-    def send(client_message_proto: ClientMessage) -> None:
+    def send(task_res: TaskRes) -> None:
         """Send task result back to server."""
         if state[KEY_TASK_INS] is None:
             log(ERROR, "No current TaskIns")
             return
 
         task_ins: TaskIns = cast(TaskIns, state[KEY_TASK_INS])
 
-        # Wrap ClientMessage in TaskRes
-        task_res = TaskRes(
-            task_id="",  # This will be generated by the server
-            group_id=task_ins.group_id,
-            workload_id=task_ins.workload_id,
-            task=Task(
+        # Check if fields to be set are not initialized
+        if not validate_task_res(task_res):
+            state[KEY_TASK_INS] = None
+            log(ERROR, "TaskRes has been initialized accidentally")
+
+        # Fill `group_id` and `workload_id` in TaskRes
+        # Note that protobuf API `protobuf.message.MergeFrom(other_msg)`
+        # does NOT always overwrite fields that are set in `other_msg`.
+        # Please refer to:
+        # https://googleapis.dev/python/protobuf/latest/google/protobuf/message.html
+        task_res.MergeFrom(
+            TaskRes(
+                task_id="",  # This will be generated by the server
+                group_id=task_ins.group_id,
+                workload_id=task_ins.workload_id,
+            )
+        )
+
+        # Fill `producer`, `consumer`, and `ancestry` in Task
+        task_res.task.MergeFrom(
+            Task(
                 producer=Node(node_id=0, anonymous=True),
                 consumer=task_ins.task.producer,
-                legacy_client_message=client_message_proto,
                 ancestry=[task_ins.task_id],
-            ),
+            )
         )
 
         # Serialize ProtoBuf to bytes
         push_task_res_request_proto = PushTaskResRequest(task_res_list=[task_res])
         push_task_res_request_bytes: bytes = (
             push_task_res_request_proto.SerializeToString()
         )
```

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/address.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/constant.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/date.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/dp.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/grpc.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/logger.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/parameter.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/serde.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/typing.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/common/version.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/driver/app.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/driver/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/driver/driver.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/driver/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/driver/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/driver/driver_client_proxy.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/driver/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/app.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/criterion.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/history.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/server.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/state/state.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/simulation/app.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.5.0.dev20230712/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230711/PKG-INFO` & `flwr_nightly-1.5.0.dev20230712/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.5.0.dev20230711
+Version: 1.5.0.dev20230712
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230711 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230712 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
 License: Apache-2.0 Author: The Flower Authors Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

