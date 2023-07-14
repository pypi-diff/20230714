# Comparing `tmp/syft-0.8.2b3.tar.gz` & `tmp/syft-0.8.2b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.2b3.tar", last modified: Fri Jul  7 10:25:30 2023, max compression
+gzip compressed data, was "syft-0.8.2b4.tar", last modified: Fri Jul 14 05:28:24 2023, max compression
```

## Comparing `syft-0.8.2b3.tar` & `syft-0.8.2b4.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.959880 syft-0.8.2b3/
--rw-r--r--   0 om        (1001) users      (100)    11843 2023-07-07 10:23:23.000000 syft-0.8.2b3/LICENSE
--rw-r--r--   0 om        (1001) users      (100)       98 2023-07-07 10:23:23.000000 syft-0.8.2b3/MANIFEST.in
--rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-07 10:25:30.959880 syft-0.8.2b3/PKG-INFO
--rw-r--r--   0 om        (1001) users      (100)    16170 2023-07-07 10:23:22.000000 syft-0.8.2b3/README.md
--rw-r--r--   0 om        (1001) users      (100)      272 2023-07-07 10:23:23.000000 syft-0.8.2b3/pyproject.toml
--rw-r--r--   0 om        (1001) users      (100)     3210 2023-07-07 10:25:30.959880 syft-0.8.2b3/setup.cfg
--rw-r--r--   0 om        (1001) users      (100)      107 2023-07-07 10:23:23.000000 syft-0.8.2b3/setup.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.939880 syft-0.8.2b3/src/
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.943880 syft-0.8.2b3/src/syft/
--rw-r--r--   0 om        (1001) users      (100)      580 2023-07-07 10:23:29.000000 syft-0.8.2b3/src/syft/VERSION
--rw-r--r--   0 om        (1001) users      (100)     5576 2023-07-07 10:23:29.000000 syft-0.8.2b3/src/syft/__init__.py
--rw-r--r--   0 om        (1001) users      (100)       93 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/__main__.py
--rw-r--r--   0 om        (1001) users      (100)      542 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/abstract_node.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.943880 syft-0.8.2b3/src/syft/capnp/
--rw-r--r--   0 om        (1001) users      (100)      270 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/capnp/__init__.py
--rw-r--r--   0 om        (1001) users      (100)       75 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/capnp/iterable.capnp
--rw-r--r--   0 om        (1001) users      (100)      102 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 om        (1001) users      (100)      186 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.943880 syft-0.8.2b3/src/syft/client/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    25448 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/api.py
--rw-r--r--   0 om        (1001) users      (100)    27509 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/client.py
--rw-r--r--   0 om        (1001) users      (100)      568 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/connection.py
--rw-r--r--   0 om        (1001) users      (100)      650 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/deploy.py
--rw-r--r--   0 om        (1001) users      (100)     7468 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/domain_client.py
--rw-r--r--   0 om        (1001) users      (100)     2598 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/enclave_client.py
--rw-r--r--   0 om        (1001) users      (100)     1116 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/gateway_client.py
--rw-r--r--   0 om        (1001) users      (100)    15257 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/registry.py
--rw-r--r--   0 om        (1001) users      (100)     2623 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/search.py
--rw-r--r--   0 om        (1001) users      (100)      549 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/user_settings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.943880 syft-0.8.2b3/src/syft/external/
--rw-r--r--   0 om        (1001) users      (100)     1735 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/__init__.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.947880 syft-0.8.2b3/src/syft/external/oblv/
--rw-r--r--   0 om        (1001) users      (100)      860 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      284 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/auth.py
--rw-r--r--   0 om        (1001) users      (100)      212 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/constants.py
--rw-r--r--   0 om        (1001) users      (100)     4835 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/deployment.py
--rw-r--r--   0 om        (1001) users      (100)    12233 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 om        (1001) users      (100)     1800 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 om        (1001) users      (100)      489 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 om        (1001) users      (100)     2280 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 om        (1001) users      (100)     7462 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 om        (1001) users      (100)    13948 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 om        (1001) users      (100)     1146 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/gevent_patch.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.947880 syft-0.8.2b3/src/syft/img/
--rw-r--r--   0 om        (1001) users      (100)      297 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/img/base64.py
--rw-r--r--   0 om        (1001) users      (100)    25535 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/img/logo.png
--rw-r--r--   0 om        (1001) users      (100)    41764 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.947880 syft-0.8.2b3/src/syft/node/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     2631 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/credentials.py
--rw-r--r--   0 om        (1001) users      (100)      152 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/domain.py
--rw-r--r--   0 om        (1001) users      (100)      259 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/enclave.py
--rw-r--r--   0 om        (1001) users      (100)      728 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/gateway.py
--rw-r--r--   0 om        (1001) users      (100)    31549 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/node.py
--rw-r--r--   0 om        (1001) users      (100)     6979 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/routes.py
--rw-r--r--   0 om        (1001) users      (100)     2064 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/run.py
--rw-r--r--   0 om        (1001) users      (100)     6992 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/server.py
--rw-r--r--   0 om        (1001) users      (100)      127 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/worker.py
--rw-r--r--   0 om        (1001) users      (100)     1100 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/worker_settings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.947880 syft-0.8.2b3/src/syft/serde/
--rw-r--r--   0 om        (1001) users      (100)      159 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     3597 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/array.py
--rw-r--r--   0 om        (1001) users      (100)     4099 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/arrow.py
--rw-r--r--   0 om        (1001) users      (100)      298 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/capnp.py
--rw-r--r--   0 om        (1001) users      (100)      722 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/deserialize.py
--rw-r--r--   0 om        (1001) users      (100)     1230 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/lib_permissions.py
--rw-r--r--   0 om        (1001) users      (100)    11663 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 om        (1001) users      (100)      875 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/mock.py
--rw-r--r--   0 om        (1001) users      (100)    11639 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/recursive.py
--rw-r--r--   0 om        (1001) users      (100)    10253 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 om        (1001) users      (100)     1822 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/serializable.py
--rw-r--r--   0 om        (1001) users      (100)      369 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/serialize.py
--rw-r--r--   0 om        (1001) users      (100)     4959 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/signature.py
--rw-r--r--   0 om        (1001) users      (100)     4885 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/third_party.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.947880 syft-0.8.2b3/src/syft/service/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/__init__.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/action/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      703 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 om        (1001) users      (100)    16706 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_graph.py
--rw-r--r--   0 om        (1001) users      (100)     6874 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 om        (1001) users      (100)    48723 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_object.py
--rw-r--r--   0 om        (1001) users      (100)     2416 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_permissions.py
--rw-r--r--   0 om        (1001) users      (100)    26998 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_service.py
--rw-r--r--   0 om        (1001) users      (100)    10264 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_store.py
--rw-r--r--   0 om        (1001) users      (100)     1165 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_types.py
--rw-r--r--   0 om        (1001) users      (100)     3889 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/numpy.py
--rw-r--r--   0 om        (1001) users      (100)     2233 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/pandas.py
--rw-r--r--   0 om        (1001) users      (100)     2920 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/plan.py
--rw-r--r--   0 om        (1001) users      (100)     4951 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/verification.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/code/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      236 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/code_parse.py
--rw-r--r--   0 om        (1001) users      (100)      102 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/unparse.py
--rw-r--r--   0 om        (1001) users      (100)    24908 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/user_code.py
--rw-r--r--   0 om        (1001) users      (100)     1756 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 om        (1001) users      (100)    10109 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/user_code_service.py
--rw-r--r--   0 om        (1001) users      (100)     1446 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 om        (1001) users      (100)     1782 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/context.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/data_subject/
--rw-r--r--   0 om        (1001) users      (100)       69 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     4076 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 om        (1001) users      (100)      870 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 om        (1001) users      (100)     3215 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 om        (1001) users      (100)     5006 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/dataset/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/dataset/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    23367 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/dataset/dataset.py
--rw-r--r--   0 om        (1001) users      (100)     6382 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 om        (1001) users      (100)     1911 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/enclave/
--rw-r--r--   0 om        (1001) users      (100)     6038 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/metadata/
--rw-r--r--   0 om        (1001) users      (100)     3481 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/network/
--rw-r--r--   0 om        (1001) users      (100)    16636 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/network/network_service.py
--rw-r--r--   0 om        (1001) users      (100)     2976 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/network/node_peer.py
--rw-r--r--   0 om        (1001) users      (100)     4593 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/network/routes.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/notification/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/notification/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     7961 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/notification/notification_service.py
--rw-r--r--   0 om        (1001) users      (100)     4566 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 om        (1001) users      (100)     3259 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/policy/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/policy/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    22437 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/policy/policy.py
--rw-r--r--   0 om        (1001) users      (100)     2081 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/policy/policy_service.py
--rw-r--r--   0 om        (1001) users      (100)     1077 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/project/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/project/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    48080 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/project/project.py
--rw-r--r--   0 om        (1001) users      (100)    15374 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/project/project_service.py
--rw-r--r--   0 om        (1001) users      (100)     1908 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/queue/
--rw-r--r--   0 om        (1001) users      (100)     2044 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/queue/base_queue.py
--rw-r--r--   0 om        (1001) users      (100)     3008 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/queue/queue.py
--rw-r--r--   0 om        (1001) users      (100)     4845 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 om        (1001) users      (100)     7929 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/service/request/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/request/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    26514 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/request/request.py
--rw-r--r--   0 om        (1001) users      (100)    10112 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/request/request_service.py
--rw-r--r--   0 om        (1001) users      (100)     1410 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/request/request_stash.py
--rw-r--r--   0 om        (1001) users      (100)     2850 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/response.py
--rw-r--r--   0 om        (1001) users      (100)    13653 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/service/settings/
--rw-r--r--   0 om        (1001) users      (100)      882 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/settings/settings.py
--rw-r--r--   0 om        (1001) users      (100)     3486 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/settings/settings_service.py
--rw-r--r--   0 om        (1001) users      (100)     1711 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/service/user/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      201 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/roles.py
--rw-r--r--   0 om        (1001) users      (100)     6115 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/user.py
--rw-r--r--   0 om        (1001) users      (100)     3427 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/user_roles.py
--rw-r--r--   0 om        (1001) users      (100)    14978 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/user_service.py
--rw-r--r--   0 om        (1001) users      (100)     4363 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/service/vpn/
--rw-r--r--   0 om        (1001) users      (100)     1809 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/vpn/headscale_client.py
--rw-r--r--   0 om        (1001) users      (100)     6789 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/vpn/tailscale_client.py
--rw-r--r--   0 om        (1001) users      (100)     5414 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/vpn/vpn.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/store/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     3235 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/dict_document_store.py
--rw-r--r--   0 om        (1001) users      (100)    22993 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/document_store.py
--rw-r--r--   0 om        (1001) users      (100)    21837 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/kv_document_store.py
--rw-r--r--   0 om        (1001) users      (100)     4326 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/linked_obj.py
--rw-r--r--   0 om        (1001) users      (100)    11840 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/locks.py
--rw-r--r--   0 om        (1001) users      (100)     8768 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/mongo_client.py
--rw-r--r--   0 om        (1001) users      (100)      846 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/mongo_codecs.py
--rw-r--r--   0 om        (1001) users      (100)    13836 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/mongo_document_store.py
--rw-r--r--   0 om        (1001) users      (100)    13136 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/types/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      136 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/base.py
--rw-r--r--   0 om        (1001) users      (100)     1091 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/datetime.py
--rw-r--r--   0 om        (1001) users      (100)     5167 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/grid_url.py
--rw-r--r--   0 om        (1001) users      (100)     4807 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/syft_metaclass.py
--rw-r--r--   0 om        (1001) users      (100)    25848 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/syft_object.py
--rw-r--r--   0 om        (1001) users      (100)     8113 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/transforms.py
--rw-r--r--   0 om        (1001) users      (100)     2098 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/twin_object.py
--rw-r--r--   0 om        (1001) users      (100)     8038 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/uid.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.959880 syft-0.8.2b3/src/syft/util/
--rw-r--r--   0 om        (1001) users      (100)       67 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      852 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/autoreload.py
--rw-r--r--   0 om        (1001) users      (100)      271 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/colors.py
--rw-r--r--   0 om        (1001) users      (100)       34 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/constants.py
--rw-r--r--   0 om        (1001) users      (100)     1514 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/decorators.py
--rw-r--r--   0 om        (1001) users      (100)     1607 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/experimental_flags.py
--rw-r--r--   0 om        (1001) users      (100)     1327 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/filterwarnings.py
--rw-r--r--   0 om        (1001) users      (100)     2940 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/fonts.py
--rw-r--r--   0 om        (1001) users      (100)      153 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/jax_settings.py
--rw-r--r--   0 om        (1001) users      (100)     3779 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/logger.py
--rw-r--r--   0 om        (1001) users      (100)      752 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/markdown.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.959880 syft-0.8.2b3/src/syft/util/notebook_ui/
--rw-r--r--   0 om        (1001) users      (100)    27090 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 om        (1001) users      (100)       42 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/options.py
--rw-r--r--   0 om        (1001) users      (100)     5297 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/schema.py
--rw-r--r--   0 om        (1001) users      (100)     2771 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/telemetry.py
--rw-r--r--   0 om        (1001) users      (100)     6728 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/trace_decorator.py
--rw-r--r--   0 om        (1001) users      (100)    22738 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/util.py
--rw-r--r--   0 om        (1001) users      (100)     3123 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/version_compare.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.943880 syft-0.8.2b3/src/syft.egg-info/
--rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 om        (1001) users      (100)     5879 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 om        (1001) users      (100)        1 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 om        (1001) users      (100)       43 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 om        (1001) users      (100)        1 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 om        (1001) users      (100)     1555 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/requires.txt
--rw-r--r--   0 om        (1001) users      (100)        5 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.845855 syft-0.8.2b4/
+-rw-r--r--   0 om        (1001) users      (100)    11843 2023-07-14 05:26:20.000000 syft-0.8.2b4/LICENSE
+-rw-r--r--   0 om        (1001) users      (100)       98 2023-07-14 05:26:20.000000 syft-0.8.2b4/MANIFEST.in
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-14 05:28:24.845855 syft-0.8.2b4/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)    16170 2023-07-14 05:26:20.000000 syft-0.8.2b4/README.md
+-rw-r--r--   0 om        (1001) users      (100)      272 2023-07-14 05:26:20.000000 syft-0.8.2b4/pyproject.toml
+-rw-r--r--   0 om        (1001) users      (100)     3210 2023-07-14 05:28:24.845855 syft-0.8.2b4/setup.cfg
+-rw-r--r--   0 om        (1001) users      (100)      107 2023-07-14 05:26:20.000000 syft-0.8.2b4/setup.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.829855 syft-0.8.2b4/src/
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.829855 syft-0.8.2b4/src/syft/
+-rw-r--r--   0 om        (1001) users      (100)      580 2023-07-14 05:26:27.000000 syft-0.8.2b4/src/syft/VERSION
+-rw-r--r--   0 om        (1001) users      (100)     5626 2023-07-14 05:26:27.000000 syft-0.8.2b4/src/syft/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       93 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/__main__.py
+-rw-r--r--   0 om        (1001) users      (100)      654 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/abstract_node.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft/capnp/
+-rw-r--r--   0 om        (1001) users      (100)      270 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/capnp/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       75 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      186 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft/client/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    25732 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/api.py
+-rw-r--r--   0 om        (1001) users      (100)    28029 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/client.py
+-rw-r--r--   0 om        (1001) users      (100)      568 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/connection.py
+-rw-r--r--   0 om        (1001) users      (100)      650 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/deploy.py
+-rw-r--r--   0 om        (1001) users      (100)     8798 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/domain_client.py
+-rw-r--r--   0 om        (1001) users      (100)     4434 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/enclave_client.py
+-rw-r--r--   0 om        (1001) users      (100)     2372 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/gateway_client.py
+-rw-r--r--   0 om        (1001) users      (100)    15257 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/registry.py
+-rw-r--r--   0 om        (1001) users      (100)     2623 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/search.py
+-rw-r--r--   0 om        (1001) users      (100)      549 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/user_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft/external/
+-rw-r--r--   0 om        (1001) users      (100)     1735 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft/external/oblv/
+-rw-r--r--   0 om        (1001) users      (100)      860 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      284 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/auth.py
+-rw-r--r--   0 om        (1001) users      (100)      212 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     4835 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 om        (1001) users      (100)    12380 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 om        (1001) users      (100)     1800 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 om        (1001) users      (100)      489 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 om        (1001) users      (100)     2280 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7462 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 om        (1001) users      (100)    13948 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1146 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/gevent_patch.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft/img/
+-rw-r--r--   0 om        (1001) users      (100)      297 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/img/base64.py
+-rw-r--r--   0 om        (1001) users      (100)    25535 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/img/logo.png
+-rw-r--r--   0 om        (1001) users      (100)    41764 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/node/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     2631 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/credentials.py
+-rw-r--r--   0 om        (1001) users      (100)      152 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/domain.py
+-rw-r--r--   0 om        (1001) users      (100)      259 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/enclave.py
+-rw-r--r--   0 om        (1001) users      (100)      728 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/gateway.py
+-rw-r--r--   0 om        (1001) users      (100)    31684 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/node.py
+-rw-r--r--   0 om        (1001) users      (100)     6960 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/routes.py
+-rw-r--r--   0 om        (1001) users      (100)     2064 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/run.py
+-rw-r--r--   0 om        (1001) users      (100)     6992 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/server.py
+-rw-r--r--   0 om        (1001) users      (100)      127 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/worker.py
+-rw-r--r--   0 om        (1001) users      (100)     1100 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/worker_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/serde/
+-rw-r--r--   0 om        (1001) users      (100)      159 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3597 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/array.py
+-rw-r--r--   0 om        (1001) users      (100)     4099 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/arrow.py
+-rw-r--r--   0 om        (1001) users      (100)      298 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/capnp.py
+-rw-r--r--   0 om        (1001) users      (100)      722 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/deserialize.py
+-rw-r--r--   0 om        (1001) users      (100)     1230 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    11663 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 om        (1001) users      (100)      875 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/mock.py
+-rw-r--r--   0 om        (1001) users      (100)    11639 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/recursive.py
+-rw-r--r--   0 om        (1001) users      (100)    10253 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 om        (1001) users      (100)     1822 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/serializable.py
+-rw-r--r--   0 om        (1001) users      (100)      369 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/serialize.py
+-rw-r--r--   0 om        (1001) users      (100)     4959 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/signature.py
+-rw-r--r--   0 om        (1001) users      (100)     4885 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/third_party.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/service/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/service/action/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      703 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 om        (1001) users      (100)    16706 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_graph.py
+-rw-r--r--   0 om        (1001) users      (100)     6874 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 om        (1001) users      (100)    48803 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_object.py
+-rw-r--r--   0 om        (1001) users      (100)     2502 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    26998 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_service.py
+-rw-r--r--   0 om        (1001) users      (100)    10264 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_store.py
+-rw-r--r--   0 om        (1001) users      (100)     1165 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_types.py
+-rw-r--r--   0 om        (1001) users      (100)     3889 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/numpy.py
+-rw-r--r--   0 om        (1001) users      (100)     2233 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/pandas.py
+-rw-r--r--   0 om        (1001) users      (100)     2920 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/plan.py
+-rw-r--r--   0 om        (1001) users      (100)     4951 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/verification.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/service/code/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      236 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/unparse.py
+-rw-r--r--   0 om        (1001) users      (100)    27413 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/user_code.py
+-rw-r--r--   0 om        (1001) users      (100)     1756 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)    10340 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1446 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     1782 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/context.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/service/data_subject/
+-rw-r--r--   0 om        (1001) users      (100)       69 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     4076 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 om        (1001) users      (100)      870 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 om        (1001) users      (100)     3215 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 om        (1001) users      (100)     5006 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/dataset/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    23590 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 om        (1001) users      (100)     6382 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1911 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/enclave/
+-rw-r--r--   0 om        (1001) users      (100)     6038 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/metadata/
+-rw-r--r--   0 om        (1001) users      (100)     3605 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/network/
+-rw-r--r--   0 om        (1001) users      (100)    18133 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/network/network_service.py
+-rw-r--r--   0 om        (1001) users      (100)     3064 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/network/node_peer.py
+-rw-r--r--   0 om        (1001) users      (100)     4593 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/network/routes.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/notification/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/notification/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     7961 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4566 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     3259 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/policy/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/policy/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    22437 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/policy/policy.py
+-rw-r--r--   0 om        (1001) users      (100)     2081 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1077 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/project/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/project/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    48433 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/project/project.py
+-rw-r--r--   0 om        (1001) users      (100)    15374 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/project/project_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1908 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/queue/
+-rw-r--r--   0 om        (1001) users      (100)     2044 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 om        (1001) users      (100)     3008 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/queue/queue.py
+-rw-r--r--   0 om        (1001) users      (100)     4845 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7929 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/request/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/request/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    26923 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/request/request.py
+-rw-r--r--   0 om        (1001) users      (100)    10112 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/request/request_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1410 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/request/request_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     2850 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/response.py
+-rw-r--r--   0 om        (1001) users      (100)    13653 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/settings/
+-rw-r--r--   0 om        (1001) users      (100)      881 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/settings/settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3486 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1711 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/user/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      201 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/roles.py
+-rw-r--r--   0 om        (1001) users      (100)     6115 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/user.py
+-rw-r--r--   0 om        (1001) users      (100)     3427 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/user_roles.py
+-rw-r--r--   0 om        (1001) users      (100)    15957 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/user_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4363 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/vpn/
+-rw-r--r--   0 om        (1001) users      (100)     1809 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     6789 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     5414 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/vpn/vpn.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.845855 syft-0.8.2b4/src/syft/store/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3235 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/dict_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    22993 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    22010 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/kv_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)     4326 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/linked_obj.py
+-rw-r--r--   0 om        (1001) users      (100)    11840 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/locks.py
+-rw-r--r--   0 om        (1001) users      (100)     8768 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/mongo_client.py
+-rw-r--r--   0 om        (1001) users      (100)      846 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 om        (1001) users      (100)    13836 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    13136 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.845855 syft-0.8.2b4/src/syft/types/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      136 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/base.py
+-rw-r--r--   0 om        (1001) users      (100)     1091 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/datetime.py
+-rw-r--r--   0 om        (1001) users      (100)     5167 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/grid_url.py
+-rw-r--r--   0 om        (1001) users      (100)     4807 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 om        (1001) users      (100)    25848 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/syft_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8113 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/transforms.py
+-rw-r--r--   0 om        (1001) users      (100)     2098 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/twin_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8038 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/uid.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.845855 syft-0.8.2b4/src/syft/util/
+-rw-r--r--   0 om        (1001) users      (100)       67 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      852 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/autoreload.py
+-rw-r--r--   0 om        (1001) users      (100)      271 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/colors.py
+-rw-r--r--   0 om        (1001) users      (100)       34 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     1514 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/decorators.py
+-rw-r--r--   0 om        (1001) users      (100)     1607 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/experimental_flags.py
+-rw-r--r--   0 om        (1001) users      (100)     1327 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/filterwarnings.py
+-rw-r--r--   0 om        (1001) users      (100)     2940 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/fonts.py
+-rw-r--r--   0 om        (1001) users      (100)      153 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/jax_settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3779 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/logger.py
+-rw-r--r--   0 om        (1001) users      (100)      752 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/markdown.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.845855 syft-0.8.2b4/src/syft/util/notebook_ui/
+-rw-r--r--   0 om        (1001) users      (100)    27090 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 om        (1001) users      (100)       42 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/options.py
+-rw-r--r--   0 om        (1001) users      (100)     5297 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/schema.py
+-rw-r--r--   0 om        (1001) users      (100)     2771 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/telemetry.py
+-rw-r--r--   0 om        (1001) users      (100)     6728 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/trace_decorator.py
+-rw-r--r--   0 om        (1001) users      (100)    22738 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/util.py
+-rw-r--r--   0 om        (1001) users      (100)     3123 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/version_compare.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft.egg-info/
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)     5879 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 om        (1001) users      (100)       43 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 om        (1001) users      (100)     1555 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/requires.txt
+-rw-r--r--   0 om        (1001) users      (100)        5 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.2b3/LICENSE` & `syft-0.8.2b4/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/PKG-INFO` & `syft-0.8.2b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b3
+Version: 0.8.2b4
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b3 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b4 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b3/README.md` & `syft-0.8.2b4/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/setup.cfg` & `syft-0.8.2b4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.2-beta.3"
+version = attr: "0.8.2-beta.4"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
```

### Comparing `syft-0.8.2b3/src/syft/VERSION` & `syft-0.8.2b4/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.2-beta.3"
+__version__ = "0.8.2-beta.4"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.2b3/src/syft/__init__.py` & `syft-0.8.2b4/src/syft/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-__version__ = "0.8.2-beta.3"
+__version__ = "0.8.2-beta.4"
 
 # stdlib
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
 
 # relative
 from . import gevent_patch  # noqa: F401
+from .abstract_node import NodeType  # noqa: F401
 from .client.client import connect  # noqa: F401
 from .client.client import login  # noqa: F401
 from .client.client import register  # noqa: F401
 from .client.deploy import Orchestra  # noqa: F401
 from .client.registry import DomainRegistry  # noqa: F401
 from .client.registry import EnclaveRegistry  # noqa: F401
 from .client.registry import NetworkRegistry  # noqa: F401
```

### Comparing `syft-0.8.2b3/src/syft/client/api.py` & `syft-0.8.2b4/src/syft/client/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # future
 from __future__ import annotations
 
 # stdlib
+from collections import OrderedDict
 import inspect
 from inspect import signature
 import types
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
@@ -47,15 +48,15 @@
 from ..types.uid import UID
 from ..util.autoreload import autoreload_enabled
 from ..util.telemetry import instrument
 from .connection import NodeConnection
 
 
 class APIRegistry:
-    __api_registry__: Dict[Tuple, SyftAPI] = {}
+    __api_registry__: Dict[Tuple, SyftAPI] = OrderedDict()
 
     @classmethod
     def set_api_for(
         cls,
         node_uid: Union[UID, str],
         user_verify_key: Union[SyftVerifyKey, str],
         api: SyftAPI,
@@ -75,14 +76,21 @@
         key = (node_uid, user_verify_key)
         return cls.__api_registry__.get(key, None)
 
     @classmethod
     def get_all_api(cls) -> List[SyftAPI]:
         return list(cls.__api_registry__.values())
 
+    @classmethod
+    def get_by_recent_node_uid(cls, node_uid: UID) -> Optional[SyftAPI]:
+        for key, api in reversed(cls.__api_registry__.items()):
+            if key[0] == node_uid:
+                return api
+        return None
+
 
 @serializable()
 class APIEndpoint(SyftBaseObject):
     service_path: str
     module_path: str
     name: str
     description: str
```

### Comparing `syft-0.8.2b3/src/syft/client/client.py` & `syft-0.8.2b4/src/syft/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 # stdlib
 from enum import Enum
 import hashlib
 import json
 from typing import Any
 from typing import Callable
 from typing import Dict
+from typing import List
 from typing import Optional
+from typing import TYPE_CHECKING
 from typing import Tuple
 from typing import Type
 from typing import Union
 from typing import cast
 
 # third party
 import pydantic
@@ -22,14 +24,15 @@
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from typing_extensions import Self
 
 # relative
 from .. import __version__
 from ..abstract_node import AbstractNode
+from ..abstract_node import NodeType
 from ..node.credentials import SyftSigningKey
 from ..node.credentials import SyftVerifyKey
 from ..node.credentials import UserLoginCredentials
 from ..serde.deserialize import _deserialize
 from ..serde.serializable import serializable
 from ..serde.serialize import _serialize
 from ..service.context import NodeServiceContext
@@ -52,14 +55,18 @@
 from .api import APIRegistry
 from .api import SignedSyftAPICall
 from .api import SyftAPI
 from .api import SyftAPICall
 from .api import debox_signed_syftapicall_response
 from .connection import NodeConnection
 
+if TYPE_CHECKING:
+    # relative
+    from ..service.network.node_peer import NodePeer
+
 # use to enable mitm proxy
 # from syft.grid.connections.http_connection import HTTPConnection
 # HTTPConnection.proxies = {"http": "http://127.0.0.1:8080"}
 
 
 def upgrade_tls(url: GridURL, response: Response) -> GridURL:
     try:
@@ -229,17 +236,16 @@
                 proxy_target_uid=self.proxy_target_uid,
                 path="login",
                 kwargs=credentials,
             )
         else:
             response = self._make_post(self.routes.ROUTE_LOGIN.value, credentials)
             obj = _deserialize(response, from_bytes=True)
-        if isinstance(obj, UserPrivateKey):
-            return obj
-        return None
+
+        return obj
 
     def register(self, new_user: UserCreate) -> SyftSigningKey:
         data = _serialize(new_user, to_bytes=True)
         if self.proxy_target_uid:
             response = forward_message_to_proxy(
                 self.make_call,
                 proxy_target_uid=self.proxy_target_uid,
@@ -281,19 +287,19 @@
         # in the gateway fixes PR
         # relative
         from .domain_client import DomainClient
         from .enclave_client import EnclaveClient
         from .gateway_client import GatewayClient
 
         metadata = self.get_node_metadata(credentials=SyftSigningKey.generate())
-        if metadata.node_type == "domain":
+        if metadata.node_type == NodeType.DOMAIN.value:
             return DomainClient
-        elif metadata.node_type == "gateway":
+        elif metadata.node_type == NodeType.GATEWAY.value:
             return GatewayClient
-        elif metadata.node_type == "enclave":
+        elif metadata.node_type == NodeType.ENCLAVE.value:
             return EnclaveClient
         else:
             return SyftError(message=f"Unknown node type {metadata.node_type}")
 
 
 @serializable()
 class PythonConnection(NodeConnection):
@@ -362,17 +368,15 @@
                 proxy_target_uid=self.proxy_target_uid,
                 path="login",
                 kwargs={"email": email, "password": password},
             )
 
         else:
             obj = self.exchange_credentials(email=email, password=password)
-        if isinstance(obj, UserPrivateKey):
-            return obj
-        return None
+        return obj
 
     def register(self, new_user: UserCreate) -> Optional[SyftSigningKey]:
         if self.proxy_target_uid:
             response = forward_message_to_proxy(
                 self.make_call,
                 proxy_target_uid=self.proxy_target_uid,
                 path="register",
@@ -399,19 +403,19 @@
         # in the gateway fixes PR
         # relative
         from .domain_client import DomainClient
         from .enclave_client import EnclaveClient
         from .gateway_client import GatewayClient
 
         metadata = self.get_node_metadata(credentials=SyftSigningKey.generate())
-        if metadata.node_type == "domain":
+        if metadata.node_type == NodeType.DOMAIN.value:
             return DomainClient
-        elif metadata.node_type == "gateway":
+        elif metadata.node_type == NodeType.GATEWAY.value:
             return GatewayClient
-        elif metadata.node_type == "enclave":
+        elif metadata.node_type == NodeType.ENCLAVE.value:
             return EnclaveClient
         else:
             return SyftError(message=f"Unknown node type {metadata.node_type}")
 
 
 @instrument
 @serializable()
@@ -436,14 +440,30 @@
 
         self.post_init()
 
     def post_init(self) -> None:
         if self.metadata is None:
             self._fetch_node_metadata(self.credentials)
 
+    def create_project(
+        self, name: str, description: str, user_email_address: str
+    ) -> Any:
+        # relative
+        from ..service.project.project import ProjectSubmit
+
+        project_create = ProjectSubmit(
+            name=name,
+            description=description,
+            shareholders=[self],
+            user_email_address=user_email_address,
+            members=[self],
+        )
+        project = project_create.start()
+        return project
+
     @property
     def authed(self) -> bool:
         return bool(self.credentials)
 
     @property
     def logged_in_user(self) -> Optional[str]:
         return self.__logged_in_user
@@ -517,50 +537,48 @@
             remote_node_verify_key=client.metadata.to(NodeMetadata).verify_key,
         )
 
         return result
 
     @property
     def users(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("user"):
+        if self.api.has_service("user"):
             return self.api.services.user
         return None
 
     @property
     def settings(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("user"):
+        if self.api.has_service("user"):
             return self.api.services.settings
         return None
 
     @property
     def notifications(self) -> Optional[APIModule]:
         print(
             "WARNING: Notifications is currently is in a beta state, so use carefully!"
         )
         print("If possible try using client.requests/client.projects")
-        if self.api is not None and self.api.has_service("notifications"):
+        if self.api.has_service("notifications"):
             return self.api.services.notifications
         return None
 
     @property
-    def domains(self) -> Optional[APIModule]:
-        return self.peers
-
-    @property
-    def peers(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("network"):
+    def peers(self) -> Optional[Union[List[NodePeer], SyftError]]:
+        if self.api.has_service("network"):
             return self.api.services.network.get_all_peers()
         return None
 
     def login(
         self, email: str, password: str, cache: bool = True, register=False, **kwargs
     ) -> Self:
         if register:
             self.register(email=email, password=password, **kwargs)
         user_private_key = self.connection.login(email=email, password=password)
+        if isinstance(user_private_key, SyftError):
+            return user_private_key
         signing_key = None
         if user_private_key is not None:
             signing_key = user_private_key.signing_key
             self.__user_role = user_private_key.role
         if signing_key is not None:
             self.credentials = signing_key
             self.__logged_in_user = email
```

### Comparing `syft-0.8.2b3/src/syft/client/connection.py` & `syft-0.8.2b4/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/client/deploy.py` & `syft-0.8.2b4/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/client/domain_client.py` & `syft-0.8.2b4/src/syft/client/domain_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,43 +4,72 @@
 # stdlib
 from typing import Optional
 from typing import TYPE_CHECKING
 from typing import Union
 
 # third party
 from tqdm import tqdm
-from typing_extensions import Self
 
 # relative
 from ..img.base64 import base64read
 from ..serde.serializable import serializable
+from ..service.dataset.dataset import Contributor
+from ..service.dataset.dataset import CreateAsset
 from ..service.dataset.dataset import CreateDataset
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
+from ..service.user.roles import Roles
 from ..service.user.user_roles import ServiceRole
 from ..types.uid import UID
 from ..util.fonts import fonts_css
 from ..util.util import get_mb_size
 from .api import APIModule
 from .client import SyftClient
+from .client import login
 
 if TYPE_CHECKING:
     # relative
     from ..service.project.project import Project
 
 
+def add_default_uploader(
+    user, obj: Union[CreateDataset, CreateAsset]
+) -> Union[CreateDataset, CreateAsset]:
+    uploader = None
+    for contributor in obj.contributors:
+        if contributor.role == str(Roles.UPLOADER):
+            uploader = contributor
+            break
+
+    if uploader is None:
+        uploader = Contributor(
+            role=str(Roles.UPLOADER),
+            name=user.name,
+            email=user.email,
+        )
+        obj.contributors.append(uploader)
+    obj.uploader = uploader
+    return obj
+
+
 @serializable()
 class DomainClient(SyftClient):
     def __repr__(self) -> str:
         return f"<DomainClient: {self.name}>"
 
     def upload_dataset(self, dataset: CreateDataset) -> Union[SyftSuccess, SyftError]:
         # relative
         from ..types.twin_object import TwinObject
 
+        user = self.users.get_current_user()
+        dataset = add_default_uploader(user, dataset)
+        for i in range(len(dataset.assets)):
+            asset = dataset.assets[i]
+            dataset.assets[i] = add_default_uploader(user, asset)
+
         dataset._check_asset_must_contain_mock()
         dataset_size = 0
 
         for asset in tqdm(dataset.asset_list):
             print(f"Uploading: {asset.name}")
             try:
                 twin = TwinObject(private_obj=asset.data, mock_obj=asset.mock)
@@ -58,42 +87,59 @@
         if valid.ok():
             return self.api.services.dataset.add(dataset=dataset)
         else:
             if len(valid.err()) > 0:
                 return tuple(valid.err())
             return valid.err()
 
-    def apply_to_gateway(self, client: Self) -> None:
+    def connect_to_gateway(
+        self,
+        via_client: Optional[SyftClient] = None,
+        url: Optional[str] = None,
+        port: Optional[int] = None,
+        handle: Optional["NodeHandle"] = None,  # noqa: F821
+        **kwargs,
+    ) -> None:
+        if via_client is not None:
+            client = via_client
+        elif handle is not None:
+            client = handle.client
+        else:
+            client = login(url=url, port=port, **kwargs)
+            if isinstance(client, SyftError):
+                return client
+
         res = self.exchange_route(client)
         if isinstance(res, SyftSuccess):
             return SyftSuccess(
-                message=f"Connected {self.metadata.node_type} to gateway"
+                message=f"Connected {self.metadata.node_type} to {client.name} gateway"
             )
         return res
 
     @property
     def data_subject_registry(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("data_subject"):
+        if self.api.has_service("data_subject"):
             return self.api.services.data_subject
         return None
 
     @property
     def code(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("code"):
+        if self.api.has_service("code"):
             return self.api.services.code
+        return None
 
     @property
     def requests(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("request"):
+        if self.api.has_service("request"):
             return self.api.services.request
         return None
 
     @property
     def datasets(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("dataset"):
+        if self.api.has_service("dataset"):
             return self.api.services.dataset
         return None
 
     @property
     def projects(self) -> Optional[APIModule]:
         if self.api.has_service("project"):
             return self.api.services.project
```

### Comparing `syft-0.8.2b3/src/syft/client/registry.py` & `syft-0.8.2b4/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/client/search.py` & `syft-0.8.2b4/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/client/user_settings.py` & `syft-0.8.2b4/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/external/__init__.py` & `syft-0.8.2b4/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/external/oblv/__init__.py` & `syft-0.8.2b4/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/external/oblv/deployment.py` & `syft-0.8.2b4/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/external/oblv/deployment_client.py` & `syft-0.8.2b4/src/syft/external/oblv/deployment_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -301,16 +301,18 @@
 
         code_id = UID()
         code.id = code_id
         code.enclave_metadata = enclave_metadata
 
         for domain_client in self.domain_clients:
             domain_client.code.request_code_execution(code=code)
+            print(f"Sent code execution request to {domain_client.name}")
 
         res = self.api.services.code.request_code_execution(code=code)
+        print(f"Execution will be done on {self.__enclave_client.name}")
 
         return res
 
     @property
     def api(self) -> SyftAPI:
         if not self.__enclave_client:
             raise Exception("Kindly login or register with the enclave")
```

### Comparing `syft-0.8.2b3/src/syft/external/oblv/exceptions.py` & `syft-0.8.2b4/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.2b4/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.2b4/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/external/oblv/oblv_service.py` & `syft-0.8.2b4/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/gevent_patch.py` & `syft-0.8.2b4/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/img/logo.png` & `syft-0.8.2b4/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.2b4/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/node/credentials.py` & `syft-0.8.2b4/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/node/gateway.py` & `syft-0.8.2b4/src/syft/node/gateway.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/node/node.py` & `syft-0.8.2b4/src/syft/node/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 def gipc_decoder(obj_bytes):
     return _deserialize(obj_bytes, from_bytes=True)
 
 
 NODE_PRIVATE_KEY = "NODE_PRIVATE_KEY"
 NODE_UID = "NODE_UID"
 NODE_TYPE = "NODE_TYPE"
+NODE_NAME = "NODE_NAME"
 
 DEFAULT_ROOT_EMAIL = "DEFAULT_ROOT_EMAIL"
 DEFAULT_ROOT_PASSWORD = "DEFAULT_ROOT_PASSWORD"  # nosec
 
 
 def get_env(key: str, default: Optional[Any] = None) -> Optional[str]:
     return os.environ.get(key, default)
@@ -122,14 +123,18 @@
     return get_env(NODE_PRIVATE_KEY)
 
 
 def get_node_type() -> Optional[str]:
     return get_env(NODE_TYPE, "domain")
 
 
+def get_node_name() -> Optional[str]:
+    return get_env(NODE_NAME, None)
+
+
 def get_node_uid_env() -> Optional[str]:
     return get_env(NODE_UID)
 
 
 def get_default_root_email() -> Optional[str]:
     return get_env(DEFAULT_ROOT_EMAIL, "info@openmined.org")
 
@@ -192,15 +197,15 @@
             self.signing_key = signing_key
 
         if self.signing_key is None:
             self.signing_key = SyftSigningKey.generate()
 
         self.processes = processes
         self.is_subprocess = is_subprocess
-        self.name = name
+        self.name = random_name() if name is None else name
         services = (
             [
                 UserService,
                 SettingsService,
                 ActionService,
                 DatasetService,
                 UserCodeService,
```

### Comparing `syft-0.8.2b3/src/syft/node/routes.py` & `syft-0.8.2b4/src/syft/node/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
         method = node.get_service_method(UserService.exchange_credentials)
         context = UnauthedServiceContext(node=node, login_credentials=login_credentials)
         result = method(context=context)
 
         if isinstance(result, SyftError):
             logger.bind(payload={"email": email}).error(result.message)
-            response = {"Error": result.message}
+            response = result
         else:
             user_private_key = result
             if not isinstance(user_private_key, UserPrivateKey):
                 raise Exception(f"Incorrect return type: {type(user_private_key)}")
             response = user_private_key
 
         return Response(
```

### Comparing `syft-0.8.2b3/src/syft/node/run.py` & `syft-0.8.2b4/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/node/server.py` & `syft-0.8.2b4/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/node/worker_settings.py` & `syft-0.8.2b4/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/serde/array.py` & `syft-0.8.2b4/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/serde/arrow.py` & `syft-0.8.2b4/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/serde/deserialize.py` & `syft-0.8.2b4/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/serde/lib_permissions.py` & `syft-0.8.2b4/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/serde/lib_service_registry.py` & `syft-0.8.2b4/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/serde/mock.py` & `syft-0.8.2b4/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/serde/recursive.py` & `syft-0.8.2b4/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/serde/recursive_primitives.py` & `syft-0.8.2b4/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/serde/serializable.py` & `syft-0.8.2b4/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/serde/signature.py` & `syft-0.8.2b4/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/serde/third_party.py` & `syft-0.8.2b4/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/action/action_data_empty.py` & `syft-0.8.2b4/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/action/action_graph.py` & `syft-0.8.2b4/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/action/action_graph_service.py` & `syft-0.8.2b4/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/action/action_object.py` & `syft-0.8.2b4/src/syft/service/action/action_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from result import Result
 from typing_extensions import Self
 
 # relative
 from ...client.api import SyftAPI
 from ...client.client import SyftClient
 from ...serde.serializable import serializable
+from ...service.response import SyftError
 from ...store.linked_obj import LinkedObject
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftBaseObject
 from ...types.syft_object import SyftObject
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ...util.logger import debug
@@ -724,15 +725,15 @@
         res.syft_client_verify_key = client.verify_key
         return res
 
     def get_from(self, client: SyftClient) -> Any:
         """Get the object from a Syft Client"""
         res = client.api.services.action.get(self.id)
         if not isinstance(res, ActionObject):
-            return Err(res)
+            return SyftError(message=f"{res}")
         else:
             return res.syft_action_data
 
     def get(self) -> Any:
         """Get the object from a Syft Client"""
         # relative
         from ...client.api import APIRegistry
@@ -740,15 +741,15 @@
         api = APIRegistry.api_for(
             node_uid=self.syft_node_location,
             user_verify_key=self.syft_client_verify_key,
         )
         res = api.services.action.get(self.id)
 
         if not isinstance(res, ActionObject):
-            return Err(res)
+            return SyftError(message=f"{res}")
         else:
             return res.syft_action_data
 
     def as_empty(self):
         id = self.id
         # TODO: fix
         if isinstance(id, LineageID):
```

### Comparing `syft-0.8.2b3/src/syft/service/action/action_permissions.py` & `syft-0.8.2b4/src/syft/service/action/action_permissions.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,17 +48,18 @@
         if self.permission in COMPOUND_ACTION_PERMISSION:
             return f"{self.permission.name}"
         else:
             return f"{self.credentials.verify}_{self.permission.name}"
 
     def __repr__(self) -> str:
         if self.credentials is not None:
-            return f"<{self.permission.name}: {self.uid} as {self.credentials.verify}>"
+            return f"[{self.permission.name}: {self.uid} as {self.credentials.verify}]"
         else:
-            # TODO: somehow, __repr__ is only triggered in this case
+            # TODO: somehow, __repr__ is only triggered in this case.
+            # Maybe fixed by change from <> brackets to [] so it now prints in htlm?
             return self.permission_string
 
 
 class ActionObjectOWNER(ActionObjectPermission):
     def __init__(self, uid: UID, credentials: SyftVerifyKey):
         self.uid = uid
         self.credentials = credentials
```

### Comparing `syft-0.8.2b3/src/syft/service/action/action_service.py` & `syft-0.8.2b4/src/syft/service/action/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/action/action_store.py` & `syft-0.8.2b4/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/action/action_types.py` & `syft-0.8.2b4/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/action/numpy.py` & `syft-0.8.2b4/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/action/pandas.py` & `syft-0.8.2b4/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/action/plan.py` & `syft-0.8.2b4/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/action/verification.py` & `syft-0.8.2b4/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/code/user_code.py` & `syft-0.8.2b4/src/syft/service/code/user_code.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 from ...types.syft_object import SyftHashableObject
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import add_node_uid_for_key
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.uid import UID
+from ...util import options
+from ...util.colors import SURFACE
 from ...util.markdown import CodeMarkdown
 from ...util.markdown import as_markdown_code
 from ..context import AuthedServiceContext
 from ..dataset.dataset import Asset
 from ..policy.policy import CustomInputPolicy
 from ..policy.policy import CustomOutputPolicy
 from ..policy.policy import ExactMatch
@@ -104,14 +106,37 @@
 
     def __init__(self, base_dict: Dict):
         self.base_dict = base_dict
 
     def __repr__(self):
         return str(self.base_dict)
 
+    def _repr_html_(self):
+        string = f"""
+            <style>
+                .syft-user_code {{color: {SURFACE[options.color_theme]};}}
+                </style>
+                <div class='syft-user_code'>
+                    <h3 style="line-height: 25%; margin-top: 25px;">User Code Status</h3>
+                    <p style="margin-left: 3px;">
+            """
+        for node_view, status in self.base_dict.items():
+            node_name_str = f"{node_view.node_name}"
+            uid_str = f"{node_view.node_id}"
+            status_str = f"{status.value}"
+
+            string += f"""
+                    &#x2022; <strong>UID: </strong>{uid_str}&nbsp;
+                    <strong>Node name: </strong>{node_name_str}&nbsp;
+                    <strong>Status: </strong>{status_str}
+                    <br>
+                """
+        string += "</p></div>"
+        return string
+
     def __repr_syft_nested__(self):
         string = ""
         for node_view, status in self.base_dict.items():
             string += f"{node_view.node_name}: {status}<br>"
         return string
 
     @property
@@ -190,15 +215,15 @@
     signature: inspect.Signature
     status: UserCodeStatusContext
     input_kwargs: List[str]
     enclave_metadata: Optional[EnclaveMetadata] = None
 
     __attr_searchable__ = ["user_verify_key", "status", "service_func_name"]
     __attr_unique__ = ["code_hash", "user_unique_func_name"]
-    __repr_attrs__ = ["status.approved", "service_func_name"]
+    __repr_attrs__ = ["status.approved", "service_func_name", "shareholders"]
 
     def __setattr__(self, key: str, value: Any) -> None:
         attr = getattr(type(self), key, None)
         if inspect.isdatadescriptor(attr):
             attr.fset(self, value)
         else:
             return super().__setattr__(key, value)
@@ -220,14 +245,22 @@
                 "value": str(self.user_verify_key),
                 "type": "clipboard",
             },
             "Status": status_badge,
         }
 
     @property
+    def shareholders(self) -> List[str]:
+        node_names_list = []
+        nodes = self.input_policy_init_kwargs.keys()
+        for node_view in nodes:
+            node_names_list.append(str(node_view.node_name))
+        return node_names_list
+
+    @property
     def input_policy(self) -> Optional[InputPolicy]:
         if not self.status.approved:
             return None
 
         if len(self.input_policy_state) == 0:
             input_policy = None
             if isinstance(self.input_policy_type, type) and issubclass(
@@ -351,17 +384,25 @@
     def unsafe_function(self) -> Optional[Callable]:
         print("WARNING: This code was submitted by a User and could be UNSAFE.")
 
         # 🟡 TODO: re-use the same infrastructure as the execute_byte_code function
         def wrapper(*args: Any, **kwargs: Any) -> Callable:
             try:
                 filtered_kwargs = {}
+                on_private_data, on_mock_data = False, False
                 for k, v in kwargs.items():
-                    filtered_kwargs[k] = debox_asset(v)
-                # third party
+                    filtered_kwargs[k], arg_type = debox_asset(v)
+                    on_private_data = (
+                        on_private_data or arg_type == ArgumentType.PRIVATE
+                    )
+                    on_mock_data = on_mock_data or arg_type == ArgumentType.MOCK
+                if on_private_data:
+                    print("Warning: The result you see is computed on PRIVATE data.")
+                elif on_mock_data:
+                    print("Warning: The result you see is computed on MOCK data.")
 
                 # remove the decorator
                 inner_function = ast.parse(self.raw_code).body[0]
                 inner_function.decorator_list = []
                 # compile the function
                 raw_byte_code = compile_byte_code(unparse(inner_function))
                 # load it
@@ -374,24 +415,25 @@
             except Exception as e:
                 print(f"Failed to run unsafe_function. {e}")
 
         return wrapper
 
     def _repr_markdown_(self):
         md = f"""class UserCode
-    id: str = {self.id}
-    status.approved: str = {self.status.approved}
+    id: UID = {self.id}
+    status.approved: bool = {self.status.approved}
     service_func_name: str = {self.service_func_name}
+    shareholders: list = {self.shareholders}
     code:
 
 {self.raw_code}"""
         return as_markdown_code(md)
 
     @property
-    def code(self) -> CodeMarkdown:
+    def show_code(self) -> CodeMarkdown:
         return CodeMarkdown(self.raw_code)
 
     def show_code_cell(self):
         warning_message = """# WARNING: \n# Before you submit
 # change the name of the function \n# for no duplicates\n\n"""
 
         # third party
@@ -428,33 +470,45 @@
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         # only run this on the client side
         if self.local_function:
             # filtered_args = []
             filtered_kwargs = {}
             # for arg in args:
             #     filtered_args.append(debox_asset(arg))
+            on_private_data, on_mock_data = False, False
             for k, v in kwargs.items():
-                filtered_kwargs[k] = debox_asset(v)
-
+                filtered_kwargs[k], arg_type = debox_asset(v)
+                on_private_data = on_private_data or arg_type == ArgumentType.PRIVATE
+                on_mock_data = on_mock_data or arg_type == ArgumentType.MOCK
+            if on_private_data:
+                print("Warning: The result you see is computed on PRIVATE data.")
+            elif on_mock_data:
+                print("Warning: The result you see is computed on MOCK data.")
             return self.local_function(**filtered_kwargs)
         else:
             raise NotImplementedError
 
 
+class ArgumentType(Enum):
+    REAL = 1
+    MOCK = 2
+    PRIVATE = 4
+
+
 def debox_asset(arg: Any) -> Any:
     deboxed_arg = arg
     if isinstance(deboxed_arg, Asset):
         asset = deboxed_arg
         if asset.has_data_permission():
-            return asset.data
+            return asset.data, ArgumentType.PRIVATE
         else:
-            return asset.mock
+            return asset.mock, ArgumentType.MOCK
     if hasattr(deboxed_arg, "syft_action_data"):
         deboxed_arg = deboxed_arg.syft_action_data
-    return deboxed_arg
+    return deboxed_arg, ArgumentType.REAL
 
 
 def syft_function_single_use(*args: Any, **kwargs: Any):
     return syft_function(
         input_policy=ExactMatch(*args, **kwargs),
         output_policy=SingleExecutionExactOutput(),
     )
@@ -639,20 +693,23 @@
     input_keys = list(context.output["input_policy_init_kwargs"].keys())
     if context.node.node_type == NodeType.DOMAIN:
         node_view = NodeView(
             node_name=context.node.name,
             node_id=context.node.id,
             verify_key=context.node.signing_key.verify_key,
         )
-        if node_view in input_keys or len(input_keys) == 0:
-            context.output["status"] = UserCodeStatusContext(
-                base_dict={node_view: UserCodeStatus.SUBMITTED}
-            )
-        else:
-            raise ValueError(f"Invalid input keys: {input_keys} for {node_view}")
+        context.output["status"] = UserCodeStatusContext(
+            base_dict={node_view: UserCodeStatus.SUBMITTED}
+        )
+        # if node_view in input_keys or len(input_keys) == 0:
+        #     context.output["status"] = UserCodeStatusContext(
+        #         base_dict={node_view: UserCodeStatus.SUBMITTED}
+        #     )
+        # else:
+        #     raise ValueError(f"Invalid input keys: {input_keys} for {node_view}")
     elif context.node.node_type == NodeType.ENCLAVE:
         base_dict = {key: UserCodeStatus.SUBMITTED for key in input_keys}
         context.output["status"] = UserCodeStatusContext(base_dict=base_dict)
     else:
         raise NotImplementedError(
             f"Invalid node type:{context.node.node_type} for code submission"
         )
```

### Comparing `syft-0.8.2b3/src/syft/service/code/user_code_parse.py` & `syft-0.8.2b4/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/code/user_code_service.py` & `syft-0.8.2b4/src/syft/service/code/user_code_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,34 +154,37 @@
             filtered_kwargs = filter_kwargs(kwargs)
             result = self.stash.get_by_uid(context.credentials, uid=uid)
             if not result.is_ok():
                 return SyftError(message=result.err())
 
             # Unroll variables
             code_item = result.ok()
-            status = code_item.status
+            code_status = code_item.status
 
             # Check if the user has permission to execute the code
             # They can execute if they are root user or if they are the user who submitted the code
             if not (
                 context.credentials == context.node.verify_key
                 or context.credentials == code_item.user_verify_key
             ):
                 return SyftError(
                     message=f"Code Execution Permission: {context.credentials} denied"
                 )
 
             # Check if the code is approved
-            if status.for_context(context) != UserCodeStatus.EXECUTE:
-                if status.for_context(context) == UserCodeStatus.SUBMITTED:
+            if code_status.for_context(context) != UserCodeStatus.EXECUTE:
+                if code_status.for_context(context) == UserCodeStatus.SUBMITTED:
+                    string = ""
+                    for node_view, status in code_status.base_dict.items():
+                        string += f"Code status on node '{node_view.node_name}' is '{status.value}'. "
                     return SyftNotReady(
-                        message=f"{type(code_item)} Your code is waiting for approval: {status}"
+                        message=f"{type(code_item)} Your code is waiting for approval. {string}"
                     )
                 return SyftError(
-                    message=f"{type(code_item)} Your code cannot be run: {status.for_context(context)}"
+                    message=f"{type(code_item)} Your code cannot be run: {code_status.for_context(context)}"
                 )
 
             output_policy = code_item.output_policy
             if output_policy is None:
                 raise Exception("Output policy not approved", code_item)
 
             # Check if the OutputPolicy is valid
```

### Comparing `syft-0.8.2b3/src/syft/service/code/user_code_stash.py` & `syft-0.8.2b4/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/context.py` & `syft-0.8.2b4/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/data_subject/data_subject.py` & `syft-0.8.2b4/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.2b4/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.2b4/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.2b4/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/dataset/dataset.py` & `syft-0.8.2b4/src/syft/service/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     name: str
     description: Optional[str]
     contributors: List[Contributor] = []
     data_subjects: List[DataSubject] = []
     mock_is_real: bool = False
     shape: Optional[Tuple]
     created_at: DateTime = DateTime.now()
+    uploader: Contributor
 
     __repr_attrs__ = ["name", "shape"]
 
     def _repr_html_(self) -> Any:
         itables_css = f"""
         .itables table {{
             margin: 0 auto;
@@ -118,15 +119,15 @@
 
         # relative
         from ...service.action.action_object import ActionObject
 
         uploaded_by_line = "n/a"
         if len(self.contributors) > 0:
             uploaded_by_line = (
-                f"<p><strong>Uploaded by: </strong>{self.contributors[0].name}</p>"
+                f"<p><strong>Uploaded by: </strong>{self.uploader.name}</p>"
             )
         if isinstance(self.data, ActionObject):
             data_table_line = itables.to_html_datatable(
                 df=self.data.syft_action_data, css=itables_css
             )
         elif isinstance(self.data, pd.DataFrame):
             data_table_line = itables.to_html_datatable(df=self.data, css=itables_css)
@@ -246,14 +247,15 @@
     node_uid: Optional[UID]
     action_id: Optional[UID]
     data: Optional[Any]
     mock: Optional[Any]
     shape: Optional[Tuple]
     mock_is_real: bool = False
     created_at: Optional[DateTime]
+    uploader: Optional[Contributor]
 
     __repr_attrs__ = ["name"]
 
     class Config:
         validate_assignment = True
 
     @root_validator()
@@ -375,14 +377,15 @@
     citation: Optional[str]
     url: Optional[str]
     description: Optional[str]
     updated_at: Optional[str]
     requests: Optional[int] = 0
     mb_size: Optional[int]
     created_at: DateTime = DateTime.now()
+    uploader: Contributor
 
     __attr_searchable__ = ["name", "citation", "url", "description", "action_ids"]
     __attr_unique__ = ["name"]
     __repr_attrs__ = ["name", "url", "created_at"]
 
     @property
     def icon(self):
@@ -398,15 +401,15 @@
         }
 
     def _repr_html_(self) -> Any:
         uploaded_by_line = "n/a"
         if len(self.contributors) > 0:
             uploaded_by_line = (
                 "<p class='paragraph-sm'><strong>"
-                + f"<span class='pr-8'>Uploaded by:</span></strong>{self.contributors[0].name}</p>"
+                + f"<span class='pr-8'>Uploaded by:</span></strong>{self.uploader.name}</p>"
             )
         return f"""
             <style>
             {fonts_css}
             .syft-dataset {{color: {SURFACE[options.color_theme]};}}
             .syft-dataset h3,
             .syft-dataset p
@@ -525,14 +528,15 @@
     __version__ = SYFT_OBJECT_VERSION_1
     asset_list: List[CreateAsset] = []
 
     __repr_attrs__ = ["name", "url"]
 
     id: Optional[UID] = None
     created_at: Optional[DateTime]
+    uploader: Optional[Contributor]
 
     class Config:
         validate_assignment = True
 
     def _check_asset_must_contain_mock(self) -> None:
         _check_asset_must_contain_mock(self.asset_list)
 
@@ -593,14 +597,17 @@
 
         self.asset_list.append(asset)
 
         return SyftSuccess(
             message=f"Asset '{asset.name}' added to '{self.name}' Dataset."
         )
 
+    def replace_asset(self, asset: CreateAsset):
+        return self.add_asset(asset=asset, force_replace=True)
+
     def remove_asset(self, name: str) -> None:
         asset_to_remove = None
         for asset in self.asset_list:
             if asset.name == name:
                 asset_to_remove = asset
                 break
```

### Comparing `syft-0.8.2b3/src/syft/service/dataset/dataset_service.py` & `syft-0.8.2b4/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.2b4/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/enclave/enclave_service.py` & `syft-0.8.2b4/src/syft/service/enclave/enclave_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/metadata/node_metadata.py` & `syft-0.8.2b4/src/syft/service/metadata/node_metadata.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Optional
 
 # third party
 from packaging import version
 from pydantic import BaseModel
 
 # relative
+from ...abstract_node import NodeType
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import StorableObjectType
 from ...types.syft_object import SyftObject
 from ...types.transforms import convert_types
 from ...types.transforms import drop
@@ -64,22 +65,22 @@
 
     name: str
     id: UID
     verify_key: SyftVerifyKey
     highest_object_version: int
     lowest_object_version: int
     syft_version: str
-    node_type: str = "domain"
+    node_type: NodeType = NodeType.DOMAIN
     deployed_on: str = "Date"
     organization: str = "OpenMined"
     on_board: bool = False
     description: str = "Text"
     signup_enabled: bool
 
-    def check_version(self, client_version: str) -> None:
+    def check_version(self, client_version: str) -> bool:
         return check_version(
             client_version=client_version,
             server_version=self.syft_version,
             server_name=self.name,
         )
 
 
@@ -88,15 +89,15 @@
     metadata_version: int
     name: str
     id: str
     verify_key: str
     highest_object_version: int
     lowest_object_version: int
     syft_version: str
-    node_type: str = "domain"
+    node_type: str = NodeType.DOMAIN.value
     deployed_on: str = "Date"
     organization: str = "OpenMined"
     on_board: bool = False
     description: str = "My cool domain"
     signup_enabled: bool
 
     def check_version(self, client_version: str) -> bool:
@@ -108,17 +109,18 @@
 
 
 @transform(NodeMetadata, NodeMetadataJSON)
 def metadata_to_json() -> List[Callable]:
     return [
         drop(["__canonical_name__"]),
         rename("__version__", "metadata_version"),
-        convert_types(["id", "verify_key"], str),
+        convert_types(["id", "verify_key", "node_type"], str),
     ]
 
 
 @transform(NodeMetadataJSON, NodeMetadata)
 def json_to_metadata() -> List[Callable]:
     return [
         drop(["metadata_version"]),
         convert_types(["id", "verify_key"], [UID, SyftVerifyKey]),
+        convert_types(["node_type"], NodeType),
     ]
```

### Comparing `syft-0.8.2b3/src/syft/service/network/network_service.py` & `syft-0.8.2b4/src/syft/service/network/network_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Optional
 from typing import Union
 
 # third party
 from result import Result
 
 # relative
+from ...abstract_node import NodeType
 from ...client.client import HTTPConnection
 from ...client.client import PythonConnection
 from ...client.client import SyftClient
 from ...node.credentials import SyftVerifyKey
 from ...node.worker_settings import WorkerSettings
 from ...serde.serializable import serializable
 from ...store.document_store import BaseUIDStoreStash
@@ -45,14 +46,15 @@
 from ..vpn.tailscale_client import get_vpn_client
 from .node_peer import NodePeer
 from .routes import HTTPNodeRoute
 from .routes import NodeRoute
 from .routes import PythonNodeRoute
 
 VerifyKeyPartitionKey = PartitionKey(key="verify_key", type_=SyftVerifyKey)
+NodeTypePartitionKey = PartitionKey(key="node_type", type_=NodeType)
 
 
 @instrument
 @serializable()
 class NetworkStash(BaseUIDStoreStash):
     object_type = NodePeer
     settings: PartitionSettings = PartitionSettings(
@@ -94,14 +96,20 @@
 
     def get_for_verify_key(
         self, credentials: SyftVerifyKey, verify_key: SyftVerifyKey
     ) -> Result[NodePeer, SyftError]:
         qks = QueryKeys(qks=[VerifyKeyPartitionKey.with_obj(verify_key)])
         return self.query_one(credentials, qks)
 
+    def get_by_node_type(
+        self, credentials: SyftVerifyKey, node_type: NodeType
+    ) -> Result[List[NodePeer], SyftError]:
+        qks = QueryKeys(qks=[NodeTypePartitionKey.with_obj(node_type)])
+        return self.query_all(credentials=credentials, qks=qks)
+
 
 @instrument
 @serializable()
 class NetworkService(AbstractService):
     store: DocumentStore
     stash: NetworkStash
 
@@ -276,14 +284,48 @@
         """Get all Peers"""
         result = self.stash.get_all(credentials=context.node.verify_key)
         if result.is_ok():
             peers = result.ok()
             return peers
         return SyftError(message=result.err())
 
+    @service_method(
+        path="network.get_peer_by_name", name="get_peer_by_name", roles=GUEST_ROLE_LEVEL
+    )
+    def get_peer_by_name(
+        self, context: AuthedServiceContext, name: str
+    ) -> Union[Optional[NodePeer], SyftError]:
+        """Get Peer by Name"""
+        result = self.stash.get_by_name(
+            credentials=context.node.verify_key,
+            name=name,
+        )
+        if result.is_ok():
+            peer = result.ok()
+            return peer
+        return SyftError(message=str(result.err()))
+
+    @service_method(
+        path="network.get_peers_by_type",
+        name="get_peers_by_type",
+        roles=GUEST_ROLE_LEVEL,
+    )
+    def get_peers_by_type(
+        self, context: AuthedServiceContext, node_type: NodeType
+    ) -> Union[List[NodePeer], SyftError]:
+        result = self.stash.get_by_node_type(
+            credentials=context.node.verify_key, node_type=node_type
+        )
+
+        if result.is_err():
+            return SyftError(message=str(result.err()))
+
+        # Return peers or an empty list when result is None
+        return result.ok() or []
+
     @service_method(path="network.join_vpn", name="join_vpn")
     def join_vpn(
         self,
         context: AuthedServiceContext,
         peer: Optional[NodePeer] = None,
         client: Optional[SyftClient] = None,
     ) -> Union[SyftSuccess, SyftError]:
@@ -484,9 +526,9 @@
     ).as_container_host()
     return HTTPConnection(url=url, proxy_target_uid=obj.proxy_target_uid)
 
 
 @transform(NodeMetadata, NodePeer)
 def metadata_to_peer() -> List[Callable]:
     return [
-        keep(["id", "name", "verify_key"]),
+        keep(["id", "name", "verify_key", "node_type"]),
     ]
```

### Comparing `syft-0.8.2b3/src/syft/service/network/node_peer.py` & `syft-0.8.2b4/src/syft/service/network/node_peer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List
 from typing import Optional
 
 # third party
 from typing_extensions import Self
 
 # relative
+from ...abstract_node import NodeType
 from ...client.client import SyftClient
 from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...service.response import SyftError
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
@@ -24,24 +25,25 @@
 
 @serializable()
 class NodePeer(SyftObject):
     # version
     __canonical_name__ = "NodePeer"
     __version__ = SYFT_OBJECT_VERSION_1
 
+    __attr_searchable__ = ["name", "node_type"]
+    __attr_unique__ = ["verify_key"]
+    __repr_attrs__ = ["name", "node_type"]
+
     id: Optional[UID]
     name: str
     verify_key: SyftVerifyKey
     is_vpn: bool = False
     vpn_auth_key: Optional[str] = None
     node_routes: List[NodeRouteType] = []
-
-    __attr_searchable__ = ["name"]
-    __attr_unique__ = ["verify_key"]
-    __repr_attrs__ = ["name"]
+    node_type: NodeType
 
     def update_routes(self, new_routes: List[NodeRoute]) -> None:
         add_routes = []
         existing_routes = set(self.node_routes)
         for new_route in new_routes:
             if new_route not in existing_routes:
                 add_routes.append(new_route)
```

### Comparing `syft-0.8.2b3/src/syft/service/network/routes.py` & `syft-0.8.2b4/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/notification/notification_service.py` & `syft-0.8.2b4/src/syft/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/notification/notification_stash.py` & `syft-0.8.2b4/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/notification/notifications.py` & `syft-0.8.2b4/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/policy/policy.py` & `syft-0.8.2b4/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/policy/policy_service.py` & `syft-0.8.2b4/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.2b4/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/project/project.py` & `syft-0.8.2b4/src/syft/service/project/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -936,16 +936,28 @@
                 id_check = True
 
             if type_check and parent_check and id_check:
                 results.append(event)
         return results
 
     def create_code_request(
-        self, obj: SubmitUserCode, client: SyftClient, reason: Optional[str] = None
+        self,
+        obj: SubmitUserCode,
+        client: Optional[SyftClient] = None,
+        reason: Optional[str] = None,
     ):
+        if client is None:
+            leader_client = self.get_leader_client(self.user_signing_key)
+            res = add_code_request_to_project(
+                project=self,
+                code=obj,
+                client=leader_client,
+                reason=reason,
+            )
+            return res
         return add_code_request_to_project(
             project=self,
             code=obj,
             client=client,
             reason=reason,
         )
 
@@ -1398,15 +1410,15 @@
         ]
     )
 
 
 def create_project_event_hash(project_event: ProjectEvent) -> Tuple[bytes, str]:
     # Creating a custom hash for the project
     # as the recursive hash is yet to be revamped
-    # for primitives python types
+    # for primitives python types.
 
     # hashing is calculated based on the following attributes,
     # attrs = ["id", "project_id", "seq no",
     # "prev_event_uid", "prev_event_hash", "creator_verify_key"]
 
     return hash_object(
         [
```

### Comparing `syft-0.8.2b3/src/syft/service/project/project_service.py` & `syft-0.8.2b4/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/project/project_stash.py` & `syft-0.8.2b4/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/queue/base_queue.py` & `syft-0.8.2b4/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/queue/queue.py` & `syft-0.8.2b4/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/queue/queue_stash.py` & `syft-0.8.2b4/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/queue/zmq_queue.py` & `syft-0.8.2b4/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/request/request.py` & `syft-0.8.2b4/src/syft/service/request/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,25 +181,31 @@
                 change.__repr_syft_nested__()
                 if hasattr(change, "__repr_syft_nested__")
                 else type(change)
             )
             str_change = f"{str_change}. "
             str_changes.append(str_change)
         str_changes = "\n".join(str_changes)
+        api = APIRegistry.api_for(
+            self.node_uid,
+            self.syft_client_verify_key,
+        )
+
         return f"""
             <style>
             .syft-request {{color: {SURFACE[options.color_theme]};}}
             </style>
             <div class='syft-request'>
                 <h3>Request</h3>
                 <p><strong>Id: </strong>{self.id}</p>
                 <p><strong>Request time: </strong>{self.request_time}</p>
                 {updated_at_line}
                 <p><strong>Changes: </strong> {str_changes}</p>
                 <p><strong>Status: </strong>{self.status}</p>
+                <p><strong>Sent to Domain </strong>{api.node_name}</p>
             </div>
             """
 
     def _coll_repr_(self):
         if self.status == RequestStatus.APPROVED:
             badge_color = "badge-green"
         elif self.status == RequestStatus.PENDING:
@@ -258,14 +264,15 @@
         return request_status
 
     def approve(self):
         api = APIRegistry.api_for(
             self.node_uid,
             self.syft_client_verify_key,
         )
+        print(f"Request approved for domain {api.node_name}")
         return api.services.request.apply(self.id)
 
     def deny(self, reason: str):
         """Denies the particular request.
 
         Args:
             reason (str): Reason for which the request has been denied.
@@ -273,23 +280,26 @@
         api = APIRegistry.api_for(
             self.node_uid,
             self.syft_client_verify_key,
         )
         return api.services.request.undo(uid=self.id, reason=reason)
 
     def approve_with_client(self, client):
+        print(f"Request approved for domain {client.name}")
         return client.api.services.request.apply(self.id)
 
     def apply(self, context: AuthedServiceContext) -> Result[SyftSuccess, SyftError]:
         change_context = ChangeContext.from_service(context)
         change_context.requesting_user_credentials = self.requesting_user_verify_key
         for change in self.changes:
             # by default change status is not applied
             change_status = ChangeStatus(change_id=change.id, applied=False)
             result = change.apply(context=change_context)
+            if isinstance(result, SyftError):
+                return result
             if result.is_err():
                 # add to history and save history to request
                 self.history.append(change_status)
                 self.save(context=context)
                 return result
 
             # If no error, then change successfully applied.
@@ -722,15 +732,15 @@
             if obj.is_err():
                 return SyftError(message=obj.err())
             obj = obj.ok()
             if apply:
                 res = self.mutate(obj, context, undo=False)
 
                 if isinstance(res, SyftError):
-                    return res
+                    return Err(res.message)
 
                 # relative
                 from ..enclave.enclave_service import propagate_inputs_to_enclave
 
                 user_code = res
                 if self.is_enclave_request(user_code.enclave_metadata):
                     enclave_res = propagate_inputs_to_enclave(
@@ -738,15 +748,15 @@
                     )
                     if isinstance(enclave_res, SyftError):
                         return enclave_res
                 self.linked_obj.update_with_context(context, user_code)
             else:
                 res = self.mutate(obj, context, undo=True)
                 if isinstance(res, SyftError):
-                    return res
+                    return Err(res.message)
 
                 # TODO: Handle Enclave approval.
                 self.linked_obj.update_with_context(context, res)
             return Ok(SyftSuccess(message=f"{type(self)} Success"))
         except Exception as e:
             print(f"failed to apply {type(self)}. {e}")
             return Err(SyftError(message=str(e)))
```

### Comparing `syft-0.8.2b3/src/syft/service/request/request_service.py` & `syft-0.8.2b4/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/request/request_stash.py` & `syft-0.8.2b4/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/response.py` & `syft-0.8.2b4/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/service.py` & `syft-0.8.2b4/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/settings/settings.py` & `syft-0.8.2b4/src/syft/service/settings/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     __canonical_name__ = "NodeSettings"
     __version__ = SYFT_OBJECT_VERSION_1
     __repr_attrs__ = ["name", "organization", "deployed_on", "signup_enabled"]
 
     name: str = "Node"
     deployed_on: str
     organization: str = "OpenMined"
-    on_board: bool = False
+    on_board: bool = True
     description: str = "Text"
     signup_enabled: bool
```

### Comparing `syft-0.8.2b3/src/syft/service/settings/settings_service.py` & `syft-0.8.2b4/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/settings/settings_stash.py` & `syft-0.8.2b4/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/user/user.py` & `syft-0.8.2b4/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/user/user_roles.py` & `syft-0.8.2b4/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/user/user_service.py` & `syft-0.8.2b4/src/syft/service/user/user_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # stdlib
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 # relative
+from ...abstract_node import NodeType
 from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...node.credentials import UserLoginCredentials
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...types.syft_metaclass import Empty
 from ...types.uid import UID
@@ -110,15 +111,14 @@
                 results = [
                     results[i : i + page_size]
                     for i in range(0, len(results), page_size)
                 ]
                 # Return the proper slice using chunk_index
                 results = results[page_index]
                 results = UserViewPage(users=results, total=total)
-
             return results
 
         # 🟡 TODO: No user exists will happen when result.ok() is empty list
         return SyftError(message="No users exists")
 
     def get_role_for_credentials(
         self, credentials: Union[SyftVerifyKey, SyftSigningKey]
@@ -171,14 +171,28 @@
             ]
             # Return the proper slice using page_index
             results = results[page_index]
             results = UserViewPage(users=results, total=total)
 
         return results
 
+    @service_method(
+        path="user.get_current_user", name="get_current_user", roles=GUEST_ROLE_LEVEL
+    )
+    def get_current_user(self, context: AuthedServiceContext) -> UserView:
+        result = self.stash.get_by_verify_key(
+            credentials=context.credentials, verify_key=context.credentials
+        )
+        if result.is_ok():
+            # this seems weird that we get back None as Ok(None)
+            user = result.ok()
+            if user:
+                return user
+        return SyftError(message=str(result.err()))
+
     @service_method(path="user.update", name="update", roles=GUEST_ROLE_LEVEL)
     def update(
         self, context: AuthedServiceContext, uid: UID, user_update: UserUpdate
     ) -> Union[UserView, SyftError]:
         updates_role = user_update.role is not Empty
 
         if (
@@ -310,14 +324,22 @@
         )
         if result.is_ok():
             user = result.ok()
             if user is not None and check_pwd(
                 context.login_credentials.password,
                 user.hashed_password,
             ):
+                if (
+                    context.node.node_type == NodeType.ENCLAVE
+                    and user.role == ServiceRole.ADMIN
+                ):
+                    return SyftError(
+                        message="Admins are not allowed to login to Enclaves."
+                        "\n Kindly register a new data scientist account by your_client.register."
+                    )
                 return user.to(UserPrivateKey)
 
             return SyftError(
                 message="No user exists with "
                 f"{context.login_credentials.email} and supplied password."
             )
```

### Comparing `syft-0.8.2b3/src/syft/service/user/user_stash.py` & `syft-0.8.2b4/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/vpn/headscale_client.py` & `syft-0.8.2b4/src/syft/service/vpn/headscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/vpn/tailscale_client.py` & `syft-0.8.2b4/src/syft/service/vpn/tailscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/service/vpn/vpn.py` & `syft-0.8.2b4/src/syft/service/vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/store/dict_document_store.py` & `syft-0.8.2b4/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/store/document_store.py` & `syft-0.8.2b4/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/store/kv_document_store.py` & `syft-0.8.2b4/src/syft/store/kv_document_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,17 +182,21 @@
             ck_check = self._check_partition_keys_unique(
                 unique_query_keys=unique_query_keys
             )
 
             if not store_key_exists and ck_check == UniqueKeyCheck.EMPTY:
                 # attempt to claim it for writing
                 ownership_result = self.take_ownership(uid=uid, credentials=credentials)
-                can_write = True if ownership_result.is_ok() else False
+                can_write = ownership_result.is_ok()
             elif not ignore_duplicates:
-                return Err(f"Duplication Key Error: {obj}")
+                keys = ", ".join(f"`{key.key}`" for key in unique_query_keys.all)
+                return Err(
+                    f"Duplication Key Error for {obj}.\n"
+                    f"The fields that should be unique are {keys}."
+                )
             else:
                 # we are not throwing an error, because we are ignoring duplicates
                 # we are also not writing though
                 return Ok(obj)
 
             if can_write:
                 self._set_data_and_keys(
@@ -205,15 +209,15 @@
                 if uid not in self.permissions:
                     # create default permissions
                     self.permissions[uid] = set()
                 permission = f"{credentials.verify}_READ"
                 permissions = self.permissions[uid]
                 permissions.add(permission)
                 if add_permissions is not None:
-                    permissions.update([x.permission_string for x in add_permissions])
+                    permissions.update(x.permission_string for x in add_permissions)
                 self.permissions[uid] = permissions
                 return Ok(obj)
             else:
                 return Err(f"Permission: {write_permission} denied")
         except Exception as e:
             return Err(f"Failed to write obj {obj}. {e}")
```

### Comparing `syft-0.8.2b3/src/syft/store/linked_obj.py` & `syft-0.8.2b4/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/store/locks.py` & `syft-0.8.2b4/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/store/mongo_client.py` & `syft-0.8.2b4/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/store/mongo_codecs.py` & `syft-0.8.2b4/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/store/mongo_document_store.py` & `syft-0.8.2b4/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/store/sqlite_document_store.py` & `syft-0.8.2b4/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/types/datetime.py` & `syft-0.8.2b4/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/types/grid_url.py` & `syft-0.8.2b4/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/types/syft_metaclass.py` & `syft-0.8.2b4/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/types/syft_object.py` & `syft-0.8.2b4/src/syft/types/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/types/transforms.py` & `syft-0.8.2b4/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/types/twin_object.py` & `syft-0.8.2b4/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/types/uid.py` & `syft-0.8.2b4/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/autoreload.py` & `syft-0.8.2b4/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/decorators.py` & `syft-0.8.2b4/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/experimental_flags.py` & `syft-0.8.2b4/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/filterwarnings.py` & `syft-0.8.2b4/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/fonts.py` & `syft-0.8.2b4/src/syft/util/fonts.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/logger.py` & `syft-0.8.2b4/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/markdown.py` & `syft-0.8.2b4/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.2b4/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/schema.py` & `syft-0.8.2b4/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/telemetry.py` & `syft-0.8.2b4/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/trace_decorator.py` & `syft-0.8.2b4/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/util.py` & `syft-0.8.2b4/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft/util/version_compare.py` & `syft-0.8.2b4/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft.egg-info/PKG-INFO` & `syft-0.8.2b4/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b3
+Version: 0.8.2b4
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b3 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b4 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b3/src/syft.egg-info/SOURCES.txt` & `syft-0.8.2b4/src/syft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b3/src/syft.egg-info/requires.txt` & `syft-0.8.2b4/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*

