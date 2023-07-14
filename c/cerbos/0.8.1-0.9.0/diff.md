# Comparing `tmp/cerbos-0.8.1.tar.gz` & `tmp/cerbos-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbos-0.8.1.tar", last modified: Tue Jul 11 14:52:08 2023, max compression
+gzip compressed data, was "cerbos-0.9.0.tar", last modified: Fri Jul 14 10:10:51 2023, max compression
```

## Comparing `cerbos-0.8.1.tar` & `cerbos-0.9.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
--rw-r--r--   0        0        0    11357 2023-07-11 14:51:34.962167 cerbos-0.8.1/LICENSE
--rw-r--r--   0        0        0     6175 2023-07-11 14:51:34.962167 cerbos-0.8.1/README.md
--rw-r--r--   0        0        0      167 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/__init__.py
--rw-r--r--   0        0        0     5052 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/audit/v1/audit_pb2.py
--rw-r--r--   0        0        0     5463 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/audit/v1/audit_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/audit/v1/audit_pb2_grpc.py
--rw-r--r--   0        0        0     1537 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/effect/v1/effect_pb2.py
--rw-r--r--   0        0        0      541 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/effect/v1/effect_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/effect/v1/effect_pb2_grpc.py
--rw-r--r--   0        0        0    24465 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/engine/v1/engine_pb2.py
--rw-r--r--   0        0        0    18348 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/engine/v1/engine_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/engine/v1/engine_pb2_grpc.py
--rw-r--r--   0        0        0    33169 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/policy/v1/policy_pb2.py
--rw-r--r--   0        0        0    29198 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/policy/v1/policy_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/policy/v1/policy_pb2_grpc.py
--rw-r--r--   0        0        0    40721 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/request/v1/request_pb2.py
--rw-r--r--   0        0        0    14880 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/request/v1/request_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/request/v1/request_pb2_grpc.py
--rw-r--r--   0        0        0    40197 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/response/v1/response_pb2.py
--rw-r--r--   0        0        0    20863 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/response/v1/response_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/response/v1/response_pb2_grpc.py
--rw-r--r--   0        0        0     3055 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/schema/v1/schema_pb2.py
--rw-r--r--   0        0        0     1614 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/schema/v1/schema_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/schema/v1/schema_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/_async/__init__.py
--rw-r--r--   0        0        0    24037 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/_async/_grpc.py
--rw-r--r--   0        0        0    12739 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/_async/_http.py
--rw-r--r--   0        0        0        0 2023-07-11 14:52:05.371922 cerbos-0.8.1/cerbos/sdk/_sync/__init__.py
--rw-r--r--   0        0        0    23695 2023-07-11 14:52:06.371980 cerbos-0.8.1/cerbos/sdk/_sync/_grpc.py
--rw-r--r--   0        0        0    12551 2023-07-11 14:52:05.371922 cerbos-0.8.1/cerbos/sdk/_sync/_http.py
--rw-r--r--   0        0        0      481 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/client.py
--rw-r--r--   0        0        0      881 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/container.py
--rw-r--r--   0        0        0      491 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/grpc/client.py
--rw-r--r--   0        0        0      702 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/grpc/utils.py
--rw-r--r--   0        0        0      106 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/http/client.py
--rw-r--r--   0        0        0     6501 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/model.py
--rw-r--r--   0        0        0    14057 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/svc/v1/svc_pb2.py
--rw-r--r--   0        0        0      449 2023-07-11 14:51:34.966168 cerbos-0.8.1/cerbos/svc/v1/svc_pb2.pyi
--rw-r--r--   0        0        0    38288 2023-07-11 14:51:34.966168 cerbos-0.8.1/cerbos/svc/v1/svc_pb2_grpc.py
--rw-r--r--   0        0        0     9422 2023-07-11 14:51:34.966168 cerbos-0.8.1/cerbos/telemetry/v1/telemetry_pb2.py
--rw-r--r--   0        0        0    10796 2023-07-11 14:51:34.966168 cerbos-0.8.1/cerbos/telemetry/v1/telemetry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-11 14:51:34.966168 cerbos-0.8.1/cerbos/telemetry/v1/telemetry_pb2_grpc.py
--rw-r--r--   0        0        0     2695 2023-07-11 14:52:08.268090 cerbos-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0     1303 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/check.py
--rw-r--r--   0        0        0     4868 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/conftest.py
--rw-r--r--   0        0        0     6496 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/grpc/test_grpc_admin_client.py
--rw-r--r--   0        0        0    15671 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/grpc/test_grpc_client.py
--rw-r--r--   0        0        0    20088 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/http/test_http_client.py
--rw-r--r--   0        0        0     2061 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/http/test_http_plan_response.py
--rw-r--r--   0        0        0      758 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/conf.yaml
--rw-r--r--   0        0        0      578 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/_schemas/leave_request.json
--rw-r--r--   0        0        0     1030 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/_schemas/principal.json
--rw-r--r--   0        0        0      402 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/_schemas/purchase_order.json
--rw-r--r--   0        0        0      387 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/_schemas/salary_record.json
--rw-r--r--   0        0        0      451 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/derived_roles/common_roles.yaml
--rw-r--r--   0        0        0      323 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/derived_roles/derived_roles_01.yaml
--rw-r--r--   0        0        0      492 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/derived_roles/derived_roles_02.yaml
--rw-r--r--   0        0        0      599 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/derived_roles/derived_roles_03.yaml
--rw-r--r--   0        0        0      577 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/principal_policies/policy_01.yaml
--rw-r--r--   0        0        0      300 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/principal_policies/policy_02.yaml
--rw-r--r--   0        0        0      226 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/principal_policies/policy_02_acme.hr.yaml
--rw-r--r--   0        0        0      499 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/principal_policies/policy_02_acme.yaml
--rw-r--r--   0        0        0     2090 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_01.yaml
--rw-r--r--   0        0        0      624 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_02.yaml
--rw-r--r--   0        0        0      526 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_03.yaml
--rw-r--r--   0        0        0      689 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_04.yaml
--rw-r--r--   0        0        0      377 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_05.yaml
--rw-r--r--   0        0        0      704 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.hr.uk.yaml
--rw-r--r--   0        0        0     1138 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.hr.yaml
--rw-r--r--   0        0        0      535 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.yaml
--rw-r--r--   0        0        0      450 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/tests/policy_04_test.yaml
--rw-r--r--   0        0        0     6987 1970-01-01 00:00:00.000000 cerbos-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-14 10:10:11.024972 cerbos-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6175 2023-07-14 10:10:11.024972 cerbos-0.9.0/README.md
+-rw-r--r--   0        0        0      167 2023-07-14 10:10:11.024972 cerbos-0.9.0/cerbos/__init__.py
+-rw-r--r--   0        0        0     5052 2023-07-14 10:10:11.024972 cerbos-0.9.0/cerbos/audit/v1/audit_pb2.py
+-rw-r--r--   0        0        0     5463 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/audit/v1/audit_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/audit/v1/audit_pb2_grpc.py
+-rw-r--r--   0        0        0     1537 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/effect/v1/effect_pb2.py
+-rw-r--r--   0        0        0      541 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/effect/v1/effect_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/effect/v1/effect_pb2_grpc.py
+-rw-r--r--   0        0        0    24465 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/engine/v1/engine_pb2.py
+-rw-r--r--   0        0        0    18348 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/engine/v1/engine_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/engine/v1/engine_pb2_grpc.py
+-rw-r--r--   0        0        0    35452 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/policy/v1/policy_pb2.py
+-rw-r--r--   0        0        0    30998 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/policy/v1/policy_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/policy/v1/policy_pb2_grpc.py
+-rw-r--r--   0        0        0    40721 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/request/v1/request_pb2.py
+-rw-r--r--   0        0        0    14880 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/request/v1/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/request/v1/request_pb2_grpc.py
+-rw-r--r--   0        0        0    40197 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/response/v1/response_pb2.py
+-rw-r--r--   0        0        0    20863 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/response/v1/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/response/v1/response_pb2_grpc.py
+-rw-r--r--   0        0        0     3055 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/schema/v1/schema_pb2.py
+-rw-r--r--   0        0        0     1614 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/schema/v1/schema_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/schema/v1/schema_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/_async/__init__.py
+-rw-r--r--   0        0        0    24037 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/_async/_grpc.py
+-rw-r--r--   0        0        0    12739 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/_async/_http.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:10:47.565674 cerbos-0.9.0/cerbos/sdk/_sync/__init__.py
+-rw-r--r--   0        0        0    23695 2023-07-14 10:10:48.865700 cerbos-0.9.0/cerbos/sdk/_sync/_grpc.py
+-rw-r--r--   0        0        0    12551 2023-07-14 10:10:47.565674 cerbos-0.9.0/cerbos/sdk/_sync/_http.py
+-rw-r--r--   0        0        0      481 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/client.py
+-rw-r--r--   0        0        0      881 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/container.py
+-rw-r--r--   0        0        0      491 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/grpc/client.py
+-rw-r--r--   0        0        0      702 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/grpc/utils.py
+-rw-r--r--   0        0        0      106 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/http/client.py
+-rw-r--r--   0        0        0     6501 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/sdk/model.py
+-rw-r--r--   0        0        0    14057 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/svc/v1/svc_pb2.py
+-rw-r--r--   0        0        0      449 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/svc/v1/svc_pb2.pyi
+-rw-r--r--   0        0        0    38288 2023-07-14 10:10:11.028972 cerbos-0.9.0/cerbos/svc/v1/svc_pb2_grpc.py
+-rw-r--r--   0        0        0     9422 2023-07-14 10:10:11.032972 cerbos-0.9.0/cerbos/telemetry/v1/telemetry_pb2.py
+-rw-r--r--   0        0        0    10796 2023-07-14 10:10:11.032972 cerbos-0.9.0/cerbos/telemetry/v1/telemetry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-14 10:10:11.032972 cerbos-0.9.0/cerbos/telemetry/v1/telemetry_pb2_grpc.py
+-rw-r--r--   0        0        0     2695 2023-07-14 10:10:51.013743 cerbos-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 10:10:11.032972 cerbos-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     1303 2023-07-14 10:10:11.032972 cerbos-0.9.0/tests/check.py
+-rw-r--r--   0        0        0     4868 2023-07-14 10:10:11.032972 cerbos-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     6496 2023-07-14 10:10:11.032972 cerbos-0.9.0/tests/grpc/test_grpc_admin_client.py
+-rw-r--r--   0        0        0    16279 2023-07-14 10:10:11.032972 cerbos-0.9.0/tests/grpc/test_grpc_client.py
+-rw-r--r--   0        0        0    20088 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/http/test_http_client.py
+-rw-r--r--   0        0        0     2061 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/http/test_http_plan_response.py
+-rw-r--r--   0        0        0      758 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/conf.yaml
+-rw-r--r--   0        0        0      578 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/_schemas/leave_request.json
+-rw-r--r--   0        0        0     1030 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/_schemas/principal.json
+-rw-r--r--   0        0        0      402 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/_schemas/purchase_order.json
+-rw-r--r--   0        0        0      387 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/_schemas/salary_record.json
+-rw-r--r--   0        0        0      451 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/derived_roles/common_roles.yaml
+-rw-r--r--   0        0        0      323 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/derived_roles/derived_roles_01.yaml
+-rw-r--r--   0        0        0      492 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/derived_roles/derived_roles_02.yaml
+-rw-r--r--   0        0        0      599 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/derived_roles/derived_roles_03.yaml
+-rw-r--r--   0        0        0      118 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/export_variables/policy_01.yaml
+-rw-r--r--   0        0        0      577 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/principal_policies/policy_01.yaml
+-rw-r--r--   0        0        0      300 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/principal_policies/policy_02.yaml
+-rw-r--r--   0        0        0      226 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/principal_policies/policy_02_acme.hr.yaml
+-rw-r--r--   0        0        0      499 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/principal_policies/policy_02_acme.yaml
+-rw-r--r--   0        0        0     2090 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_01.yaml
+-rw-r--r--   0        0        0      624 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_02.yaml
+-rw-r--r--   0        0        0      526 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_03.yaml
+-rw-r--r--   0        0        0      710 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_04.yaml
+-rw-r--r--   0        0        0      377 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_05.yaml
+-rw-r--r--   0        0        0      704 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.hr.uk.yaml
+-rw-r--r--   0        0        0     1138 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.hr.yaml
+-rw-r--r--   0        0        0      535 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.yaml
+-rw-r--r--   0        0        0      450 2023-07-14 10:10:11.036972 cerbos-0.9.0/tests/store/policies/tests/policy_04_test.yaml
+-rw-r--r--   0        0        0     6987 1970-01-01 00:00:00.000000 cerbos-0.9.0/PKG-INFO
```

### Comparing `cerbos-0.8.1/LICENSE` & `cerbos-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/README.md` & `cerbos-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/audit/v1/audit_pb2.py` & `cerbos-0.9.0/cerbos/audit/v1/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/audit/v1/audit_pb2.pyi` & `cerbos-0.9.0/cerbos/audit/v1/audit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/effect/v1/effect_pb2.py` & `cerbos-0.9.0/cerbos/effect/v1/effect_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/effect/v1/effect_pb2.pyi` & `cerbos-0.9.0/cerbos/effect/v1/effect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/engine/v1/engine_pb2.py` & `cerbos-0.9.0/cerbos/engine/v1/engine_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/engine/v1/engine_pb2.pyi` & `cerbos-0.9.0/cerbos/engine/v1/engine_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/policy/v1/policy_pb2.py` & `cerbos-0.9.0/cerbos/policy/v1/policy_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,31 @@
 from cerbos.engine.v1 import engine_pb2 as cerbos_dot_engine_dot_v1_dot_engine__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x63\x65rbos/policy/v1/policy.proto\x12\x10\x63\x65rbos.policy.v1\x1a\x1d\x63\x65rbos/effect/v1/effect.proto\x1a\x1d\x63\x65rbos/engine/v1/engine.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x17validate/validate.proto\"\xd4\x04\n\x06Policy\x12\x39\n\x0b\x61pi_version\x18\x01 \x01(\tB\x18\xfa\x42\x15r\x13\n\x11\x61pi.cerbos.dev/v1R\napiVersion\x12\x1a\n\x08\x64isabled\x18\x02 \x01(\x08R\x08\x64isabled\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x36\n\x08metadata\x18\x04 \x01(\x0b\x32\x1a.cerbos.policy.v1.MetadataR\x08metadata\x12K\n\x0fresource_policy\x18\x05 \x01(\x0b\x32 .cerbos.policy.v1.ResourcePolicyH\x00R\x0eresourcePolicy\x12N\n\x10principal_policy\x18\x06 \x01(\x0b\x32!.cerbos.policy.v1.PrincipalPolicyH\x00R\x0fprincipalPolicy\x12\x45\n\rderived_roles\x18\x07 \x01(\x0b\x32\x1e.cerbos.policy.v1.DerivedRolesH\x00R\x0c\x64\x65rivedRoles\x12\x45\n\tvariables\x18\x08 \x03(\x0b\x32\'.cerbos.policy.v1.Policy.VariablesEntryR\tvariables\x12\x1c\n\x0bjson_schema\x18\t \x01(\tR\x07$schema\x1a<\n\x0eVariablesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x12\n\x0bpolicy_type\x12\x03\xf8\x42\x01\"\xc4\x02\n\x08Metadata\x12\x1f\n\x0bsource_file\x18\x01 \x01(\tR\nsourceFile\x12M\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32+.cerbos.policy.v1.Metadata.AnnotationsEntryR\x0b\x61nnotations\x12\x30\n\x04hash\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt64ValueR\x04hash\x12+\n\x0fstore_identifer\x18\x04 \x01(\tB\x02\x18\x01R\x0estoreIdentifer\x12)\n\x10store_identifier\x18\x05 \x01(\tR\x0fstoreIdentifier\x1a>\n\x10\x41nnotationsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xb4\x03\n\x0eResourcePolicy\x12\x66\n\x08resource\x18\x01 \x01(\tBJ\xfa\x42GrE\x10\x01\x32\x41^[[:alpha:]][[:word:]\\@\\.\\-/]*(\\:[[:alpha:]][[:word:]\\@\\.\\-/]*)*$R\x08resource\x12.\n\x07version\x18\x02 \x01(\tB\x14\xfa\x42\x11r\x0f\x32\r^[[:word:]]+$R\x07version\x12Q\n\x14import_derived_roles\x18\x03 \x03(\tB\x1f\xfa\x42\x1c\x92\x01\x19\x18\x01\"\x15r\x13\x32\x11^[[:word:]\\-\\.]+$R\x12importDerivedRoles\x12\x34\n\x05rules\x18\x04 \x03(\x0b\x32\x1e.cerbos.policy.v1.ResourceRuleR\x05rules\x12L\n\x05scope\x18\x05 \x01(\tB6\xfa\x42\x33r12/^([[:alnum:]][[:word:]\\-]*(\\.[[:word:]\\-]*)*)*$R\x05scope\x12\x33\n\x07schemas\x18\x06 \x01(\x0b\x32\x19.cerbos.policy.v1.SchemasR\x07schemas\"\xa5\x03\n\x0cResourceRule\x12*\n\x07\x61\x63tions\x18\x01 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x08\x01\x18\x01\"\x04r\x02\x10\x01R\x07\x61\x63tions\x12\x44\n\rderived_roles\x18\x02 \x03(\tB\x1f\xfa\x42\x1c\x92\x01\x19\x18\x01\"\x15r\x13\x32\x11^[[:word:]\\-\\.]+$R\x0c\x64\x65rivedRoles\x12:\n\x05roles\x18\x03 \x03(\tB$\xfa\x42!\x92\x01\x1e\x18\x01\"\x1ar\x18\x32\x16^([[:word:]\\-\\.]+|\\*)$R\x05roles\x12\x39\n\tcondition\x18\x04 \x01(\x0b\x32\x1b.cerbos.policy.v1.ConditionR\tcondition\x12<\n\x06\x65\x66\x66\x65\x63t\x18\x05 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectB\n\xfa\x42\x07\x82\x01\x04\x18\x01\x18\x02R\x06\x65\x66\x66\x65\x63t\x12<\n\x04name\x18\x06 \x01(\tB(\xfa\x42%r#2!^([[:alpha:]][[:word:]\\@\\.\\-]*)*$R\x04name\x12\x30\n\x06output\x18\x07 \x01(\x0b\x32\x18.cerbos.policy.v1.OutputR\x06output\"\xae\x02\n\x0fPrincipalPolicy\x12\x66\n\tprincipal\x18\x01 \x01(\tBH\xfa\x42\x45rC\x10\x01\x32?^[[:alpha:]][[:word:]\\@\\.\\-]*(\\:[[:alpha:]][[:word:]\\@\\.\\-]*)*$R\tprincipal\x12.\n\x07version\x18\x02 \x01(\tB\x14\xfa\x42\x11r\x0f\x32\r^[[:word:]]+$R\x07version\x12\x35\n\x05rules\x18\x03 \x03(\x0b\x32\x1f.cerbos.policy.v1.PrincipalRuleR\x05rules\x12L\n\x05scope\x18\x04 \x01(\tB6\xfa\x42\x33r12/^([[:alnum:]][[:word:]\\-]*(\\.[[:word:]\\-]*)*)*$R\x05scope\"\x95\x03\n\rPrincipalRule\x12#\n\x08resource\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08resource\x12J\n\x07\x61\x63tions\x18\x02 \x03(\x0b\x32&.cerbos.policy.v1.PrincipalRule.ActionB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x07\x61\x63tions\x1a\x92\x02\n\x06\x41\x63tion\x12\x1f\n\x06\x61\x63tion\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x06\x61\x63tion\x12\x39\n\tcondition\x18\x02 \x01(\x0b\x32\x1b.cerbos.policy.v1.ConditionR\tcondition\x12<\n\x06\x65\x66\x66\x65\x63t\x18\x03 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectB\n\xfa\x42\x07\x82\x01\x04\x18\x01\x18\x02R\x06\x65\x66\x66\x65\x63t\x12<\n\x04name\x18\x04 \x01(\tB(\xfa\x42%r#2!^([[:alpha:]][[:word:]\\@\\.\\-]*)*$R\x04name\x12\x30\n\x06output\x18\x05 \x01(\x0b\x32\x18.cerbos.policy.v1.OutputR\x06output\"\x85\x01\n\x0c\x44\x65rivedRoles\x12.\n\x04name\x18\x01 \x01(\tB\x1a\xfa\x42\x17r\x15\x10\x01\x32\x11^[[:word:]\\-\\.]+$R\x04name\x12\x45\n\x0b\x64\x65\x66initions\x18\x02 \x03(\x0b\x32\x19.cerbos.policy.v1.RoleDefB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x0b\x64\x65\x66initions\"\xbd\x01\n\x07RoleDef\x12,\n\x04name\x18\x01 \x01(\tB\x18\xfa\x42\x15r\x13\x32\x11^[[:word:]\\-\\.]+$R\x04name\x12I\n\x0cparent_roles\x18\x02 \x03(\tB&\xfa\x42#\x92\x01 \x08\x01\x18\x01\"\x1ar\x18\x32\x16^([[:word:]\\-\\.]+|\\*)$R\x0bparentRoles\x12\x39\n\tcondition\x18\x03 \x01(\x0b\x32\x1b.cerbos.policy.v1.ConditionR\tcondition\"h\n\tCondition\x12/\n\x05match\x18\x01 \x01(\x0b\x32\x17.cerbos.policy.v1.MatchH\x00R\x05match\x12\x18\n\x06script\x18\x02 \x01(\tH\x00R\x06scriptB\x10\n\tcondition\x12\x03\xf8\x42\x01\"\x8b\x02\n\x05Match\x12\x34\n\x03\x61ll\x18\x01 \x01(\x0b\x32 .cerbos.policy.v1.Match.ExprListH\x00R\x03\x61ll\x12\x34\n\x03\x61ny\x18\x02 \x01(\x0b\x32 .cerbos.policy.v1.Match.ExprListH\x00R\x03\x61ny\x12\x36\n\x04none\x18\x03 \x01(\x0b\x32 .cerbos.policy.v1.Match.ExprListH\x00R\x04none\x12\x14\n\x04\x65xpr\x18\x04 \x01(\tH\x00R\x04\x65xpr\x1a=\n\x08\x45xprList\x12\x31\n\x02of\x18\x01 \x03(\x0b\x32\x17.cerbos.policy.v1.MatchB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x02ofB\t\n\x02op\x12\x03\xf8\x42\x01\"\x1c\n\x06Output\x12\x12\n\x04\x65xpr\x18\x01 \x01(\tR\x04\x65xpr\"\xc7\x02\n\x07Schemas\x12K\n\x10principal_schema\x18\x01 \x01(\x0b\x32 .cerbos.policy.v1.Schemas.SchemaR\x0fprincipalSchema\x12I\n\x0fresource_schema\x18\x02 \x01(\x0b\x32 .cerbos.policy.v1.Schemas.SchemaR\x0eresourceSchema\x1a\x38\n\nIgnoreWhen\x12*\n\x07\x61\x63tions\x18\x01 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x08\x01\x18\x01\"\x04r\x02\x10\x01R\x07\x61\x63tions\x1aj\n\x06Schema\x12\x19\n\x03ref\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x03ref\x12\x45\n\x0bignore_when\x18\x02 \x01(\x0b\x32$.cerbos.policy.v1.Schemas.IgnoreWhenR\nignoreWhen\"\x9c\x05\n\x0bTestFixture\x1a\xe0\x01\n\nPrincipals\x12X\n\nprincipals\x18\x01 \x03(\x0b\x32\x38.cerbos.policy.v1.TestFixture.Principals.PrincipalsEntryR\nprincipals\x12\x1c\n\x0bjson_schema\x18\x02 \x01(\tR\x07$schema\x1aZ\n\x0fPrincipalsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.cerbos.engine.v1.PrincipalR\x05value:\x02\x38\x01\x1a\xd9\x01\n\tResources\x12T\n\tresources\x18\x01 \x03(\x0b\x32\x36.cerbos.policy.v1.TestFixture.Resources.ResourcesEntryR\tresources\x12\x1c\n\x0bjson_schema\x18\x02 \x01(\tR\x07$schema\x1aX\n\x0eResourcesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32\x1a.cerbos.engine.v1.ResourceR\x05value:\x02\x38\x01\x1a\xcd\x01\n\x07\x41uxData\x12M\n\x08\x61ux_data\x18\x01 \x03(\x0b\x32\x32.cerbos.policy.v1.TestFixture.AuxData.AuxDataEntryR\x07\x61uxData\x12\x1c\n\x0bjson_schema\x18\x02 \x01(\tR\x07$schema\x1aU\n\x0c\x41uxDataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12/\n\x05value\x18\x02 \x01(\x0b\x32\x19.cerbos.engine.v1.AuxDataR\x05value:\x02\x38\x01\";\n\x0bTestOptions\x12,\n\x03now\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x03now\"\xfc\x05\n\tTestSuite\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x12\n\x04skip\x18\x03 \x01(\x08R\x04skip\x12\x1f\n\x0bskip_reason\x18\x04 \x01(\tR\nskipReason\x12;\n\x05tests\x18\x05 \x03(\x0b\x32\x1b.cerbos.policy.v1.TestTableB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x05tests\x12K\n\nprincipals\x18\x06 \x03(\x0b\x32+.cerbos.policy.v1.TestSuite.PrincipalsEntryR\nprincipals\x12H\n\tresources\x18\x07 \x03(\x0b\x32*.cerbos.policy.v1.TestSuite.ResourcesEntryR\tresources\x12\x43\n\x08\x61ux_data\x18\x08 \x03(\x0b\x32(.cerbos.policy.v1.TestSuite.AuxDataEntryR\x07\x61uxData\x12\x37\n\x07options\x18\t \x01(\x0b\x32\x1d.cerbos.policy.v1.TestOptionsR\x07options\x12\x1c\n\x0bjson_schema\x18\n \x01(\tR\x07$schema\x1aZ\n\x0fPrincipalsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.cerbos.engine.v1.PrincipalR\x05value:\x02\x38\x01\x1aX\n\x0eResourcesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32\x1a.cerbos.engine.v1.ResourceR\x05value:\x02\x38\x01\x1aU\n\x0c\x41uxDataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12/\n\x05value\x18\x02 \x01(\x0b\x32\x19.cerbos.engine.v1.AuxDataR\x05value:\x02\x38\x01\"\xd5\x07\n\tTestTable\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x12\n\x04skip\x18\x03 \x01(\x08R\x04skip\x12\x1f\n\x0bskip_reason\x18\x04 \x01(\tR\nskipReason\x12\x41\n\x05input\x18\x05 \x01(\x0b\x32!.cerbos.policy.v1.TestTable.InputB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x05input\x12M\n\x08\x65xpected\x18\x06 \x03(\x0b\x32\'.cerbos.policy.v1.TestTable.ExpectationB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x08\x65xpected\x12\x37\n\x07options\x18\x07 \x01(\x0b\x32\x1d.cerbos.policy.v1.TestOptionsR\x07options\x1a\xb0\x01\n\x05Input\x12\x30\n\nprincipals\x18\x01 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x08\x01\x18\x01\"\x04r\x02\x10\x01R\nprincipals\x12.\n\tresources\x18\x02 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x08\x01\x18\x01\"\x04r\x02\x10\x01R\tresources\x12*\n\x07\x61\x63tions\x18\x03 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x08\x01\x18\x01\"\x04r\x02\x10\x01R\x07\x61\x63tions\x12\x19\n\x08\x61ux_data\x18\x04 \x01(\tR\x07\x61uxData\x1az\n\x12OutputExpectations\x12\x1f\n\x06\x61\x63tion\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x06\x61\x63tion\x12\x43\n\x08\x65xpected\x18\x02 \x03(\x0b\x32\x1d.cerbos.engine.v1.OutputEntryB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x08\x65xpected\x1a\xd9\x02\n\x0b\x45xpectation\x12%\n\tprincipal\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\tprincipal\x12#\n\x08resource\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08resource\x12^\n\x07\x61\x63tions\x18\x03 \x03(\x0b\x32\x34.cerbos.policy.v1.TestTable.Expectation.ActionsEntryB\x0e\xfa\x42\x0b\x9a\x01\x08\x08\x01\"\x04r\x02\x10\x01R\x07\x61\x63tions\x12H\n\x07outputs\x18\x04 \x03(\x0b\x32..cerbos.policy.v1.TestTable.OutputExpectationsR\x07outputs\x1aT\n\x0c\x41\x63tionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12.\n\x05value\x18\x02 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectR\x05value:\x02\x38\x01\"\xc9\x07\n\x04Test\x12=\n\x04name\x18\x01 \x01(\x0b\x32\x1f.cerbos.policy.v1.Test.TestNameB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x12\n\x04skip\x18\x03 \x01(\x08R\x04skip\x12\x1f\n\x0bskip_reason\x18\x04 \x01(\tR\nskipReason\x12<\n\x05input\x18\x05 \x01(\x0b\x32\x1c.cerbos.engine.v1.CheckInputB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x05input\x12P\n\x08\x65xpected\x18\x06 \x03(\x0b\x32$.cerbos.policy.v1.Test.ExpectedEntryB\x0e\xfa\x42\x0b\x9a\x01\x08\x08\x01\"\x04r\x02\x10\x01R\x08\x65xpected\x12\x37\n\x07options\x18\x07 \x01(\x0b\x32\x1d.cerbos.policy.v1.TestOptionsR\x07options\x12V\n\x10\x65xpected_outputs\x18\x08 \x03(\x0b\x32+.cerbos.policy.v1.Test.ExpectedOutputsEntryR\x0f\x65xpectedOutputs\x1a\x95\x01\n\x08TestName\x12/\n\x0ftest_table_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\rtestTableName\x12,\n\rprincipal_key\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0cprincipalKey\x12*\n\x0cresource_key\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0bresourceKey\x1a\xb0\x01\n\rOutputEntries\x12K\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x31.cerbos.policy.v1.Test.OutputEntries.EntriesEntryR\x07\x65ntries\x1aR\n\x0c\x45ntriesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01\x1aU\n\rExpectedEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12.\n\x05value\x18\x02 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectR\x05value:\x02\x38\x01\x1ah\n\x14\x45xpectedOutputsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12:\n\x05value\x18\x02 \x01(\x0b\x32$.cerbos.policy.v1.Test.OutputEntriesR\x05value:\x02\x38\x01\"\xb0\x10\n\x0bTestResults\x12;\n\x06suites\x18\x01 \x03(\x0b\x32#.cerbos.policy.v1.TestResults.SuiteR\x06suites\x12?\n\x07summary\x18\x02 \x01(\x0b\x32%.cerbos.policy.v1.TestResults.SummaryR\x07summary\x1a[\n\x05Tally\x12<\n\x06result\x18\x01 \x01(\x0e\x32$.cerbos.policy.v1.TestResults.ResultR\x06result\x12\x14\n\x05\x63ount\x18\x02 \x01(\rR\x05\x63ount\x1a\xc1\x01\n\x07Summary\x12K\n\x0eoverall_result\x18\x01 \x01(\x0e\x32$.cerbos.policy.v1.TestResults.ResultR\roverallResult\x12\x1f\n\x0btests_count\x18\x02 \x01(\rR\ntestsCount\x12H\n\rresult_counts\x18\x03 \x03(\x0b\x32#.cerbos.policy.v1.TestResults.TallyR\x0cresultCounts\x1a\xbc\x02\n\x05Suite\x12\x12\n\x04\x66ile\x18\x01 \x01(\tR\x04\x66ile\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12K\n\nprincipals\x18\x03 \x03(\x0b\x32\'.cerbos.policy.v1.TestResults.PrincipalB\x02\x18\x01R\nprincipals\x12?\n\x07summary\x18\x04 \x01(\x0b\x32%.cerbos.policy.v1.TestResults.SummaryR\x07summary\x12\x14\n\x05\x65rror\x18\x05 \x01(\tR\x05\x65rror\x12\x45\n\ntest_cases\x18\x06 \x03(\x0b\x32&.cerbos.policy.v1.TestResults.TestCaseR\ttestCases\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x1ag\n\x08TestCase\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12G\n\nprincipals\x18\x02 \x03(\x0b\x32\'.cerbos.policy.v1.TestResults.PrincipalR\nprincipals\x1a\x65\n\tPrincipal\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x44\n\tresources\x18\x02 \x03(\x0b\x32&.cerbos.policy.v1.TestResults.ResourceR\tresources\x1a^\n\x08Resource\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x07\x61\x63tions\x18\x02 \x03(\x0b\x32$.cerbos.policy.v1.TestResults.ActionR\x07\x61\x63tions\x1a]\n\x06\x41\x63tion\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x07\x64\x65tails\x18\x02 \x01(\x0b\x32%.cerbos.policy.v1.TestResults.DetailsR\x07\x64\x65tails\x1a\xe9\x01\n\x07\x44\x65tails\x12<\n\x06result\x18\x01 \x01(\x0e\x32$.cerbos.policy.v1.TestResults.ResultR\x06result\x12\x41\n\x07\x66\x61ilure\x18\x02 \x01(\x0b\x32%.cerbos.policy.v1.TestResults.FailureH\x00R\x07\x66\x61ilure\x12\x16\n\x05\x65rror\x18\x03 \x01(\tH\x00R\x05\x65rror\x12:\n\x0c\x65ngine_trace\x18\x04 \x03(\x0b\x32\x17.cerbos.engine.v1.TraceR\x0b\x65ngineTraceB\t\n\x07outcome\x1a\x9c\x03\n\rOutputFailure\x12\x10\n\x03src\x18\x01 \x01(\tR\x03src\x12]\n\nmismatched\x18\x02 \x01(\x0b\x32;.cerbos.policy.v1.TestResults.OutputFailure.MismatchedValueH\x00R\nmismatched\x12T\n\x07missing\x18\x03 \x01(\x0b\x32\x38.cerbos.policy.v1.TestResults.OutputFailure.MissingValueH\x00R\x07missing\x1au\n\x0fMismatchedValue\x12\x32\n\x08\x65xpected\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x08\x65xpected\x12.\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x06\x61\x63tual\x1a\x42\n\x0cMissingValue\x12\x32\n\x08\x65xpected\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x08\x65xpectedB\t\n\x07outcome\x1a\xb8\x01\n\x07\x46\x61ilure\x12\x34\n\x08\x65xpected\x18\x01 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectR\x08\x65xpected\x12\x30\n\x06\x61\x63tual\x18\x02 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectR\x06\x61\x63tual\x12\x45\n\x07outputs\x18\x03 \x03(\x0b\x32+.cerbos.policy.v1.TestResults.OutputFailureR\x07outputs\"n\n\x06Result\x12\x16\n\x12RESULT_UNSPECIFIED\x10\x00\x12\x12\n\x0eRESULT_SKIPPED\x10\x01\x12\x11\n\rRESULT_PASSED\x10\x02\x12\x11\n\rRESULT_FAILED\x10\x03\x12\x12\n\x0eRESULT_ERRORED\x10\x04\x42o\n\x18\x64\x65v.cerbos.api.v1.policyZ<github.com/cerbos/cerbos/api/genpb/cerbos/policy/v1;policyv1\xaa\x02\x14\x43\x65rbos.Api.V1.Policyb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x63\x65rbos/policy/v1/policy.proto\x12\x10\x63\x65rbos.policy.v1\x1a\x1d\x63\x65rbos/effect/v1/effect.proto\x1a\x1d\x63\x65rbos/engine/v1/engine.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x17validate/validate.proto\"\xa8\x05\n\x06Policy\x12\x39\n\x0b\x61pi_version\x18\x01 \x01(\tB\x18\xfa\x42\x15r\x13\n\x11\x61pi.cerbos.dev/v1R\napiVersion\x12\x1a\n\x08\x64isabled\x18\x02 \x01(\x08R\x08\x64isabled\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x36\n\x08metadata\x18\x04 \x01(\x0b\x32\x1a.cerbos.policy.v1.MetadataR\x08metadata\x12K\n\x0fresource_policy\x18\x05 \x01(\x0b\x32 .cerbos.policy.v1.ResourcePolicyH\x00R\x0eresourcePolicy\x12N\n\x10principal_policy\x18\x06 \x01(\x0b\x32!.cerbos.policy.v1.PrincipalPolicyH\x00R\x0fprincipalPolicy\x12\x45\n\rderived_roles\x18\x07 \x01(\x0b\x32\x1e.cerbos.policy.v1.DerivedRolesH\x00R\x0c\x64\x65rivedRoles\x12N\n\x10\x65xport_variables\x18\n \x01(\x0b\x32!.cerbos.policy.v1.ExportVariablesH\x00R\x0f\x65xportVariables\x12I\n\tvariables\x18\x08 \x03(\x0b\x32\'.cerbos.policy.v1.Policy.VariablesEntryB\x02\x18\x01R\tvariables\x12\x1c\n\x0bjson_schema\x18\t \x01(\tR\x07$schema\x1a<\n\x0eVariablesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x12\n\x0bpolicy_type\x12\x03\xf8\x42\x01\"\xc4\x02\n\x08Metadata\x12\x1f\n\x0bsource_file\x18\x01 \x01(\tR\nsourceFile\x12M\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32+.cerbos.policy.v1.Metadata.AnnotationsEntryR\x0b\x61nnotations\x12\x30\n\x04hash\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt64ValueR\x04hash\x12+\n\x0fstore_identifer\x18\x04 \x01(\tB\x02\x18\x01R\x0estoreIdentifer\x12)\n\x10store_identifier\x18\x05 \x01(\tR\x0fstoreIdentifier\x1a>\n\x10\x41nnotationsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xef\x03\n\x0eResourcePolicy\x12\x66\n\x08resource\x18\x01 \x01(\tBJ\xfa\x42GrE\x10\x01\x32\x41^[[:alpha:]][[:word:]\\@\\.\\-/]*(\\:[[:alpha:]][[:word:]\\@\\.\\-/]*)*$R\x08resource\x12.\n\x07version\x18\x02 \x01(\tB\x14\xfa\x42\x11r\x0f\x32\r^[[:word:]]+$R\x07version\x12Q\n\x14import_derived_roles\x18\x03 \x03(\tB\x1f\xfa\x42\x1c\x92\x01\x19\x18\x01\"\x15r\x13\x32\x11^[[:word:]\\-\\.]+$R\x12importDerivedRoles\x12\x34\n\x05rules\x18\x04 \x03(\x0b\x32\x1e.cerbos.policy.v1.ResourceRuleR\x05rules\x12L\n\x05scope\x18\x05 \x01(\tB6\xfa\x42\x33r12/^([[:alnum:]][[:word:]\\-]*(\\.[[:word:]\\-]*)*)*$R\x05scope\x12\x33\n\x07schemas\x18\x06 \x01(\x0b\x32\x19.cerbos.policy.v1.SchemasR\x07schemas\x12\x39\n\tvariables\x18\x07 \x01(\x0b\x32\x1b.cerbos.policy.v1.VariablesR\tvariables\"\xa5\x03\n\x0cResourceRule\x12*\n\x07\x61\x63tions\x18\x01 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x08\x01\x18\x01\"\x04r\x02\x10\x01R\x07\x61\x63tions\x12\x44\n\rderived_roles\x18\x02 \x03(\tB\x1f\xfa\x42\x1c\x92\x01\x19\x18\x01\"\x15r\x13\x32\x11^[[:word:]\\-\\.]+$R\x0c\x64\x65rivedRoles\x12:\n\x05roles\x18\x03 \x03(\tB$\xfa\x42!\x92\x01\x1e\x18\x01\"\x1ar\x18\x32\x16^([[:word:]\\-\\.]+|\\*)$R\x05roles\x12\x39\n\tcondition\x18\x04 \x01(\x0b\x32\x1b.cerbos.policy.v1.ConditionR\tcondition\x12<\n\x06\x65\x66\x66\x65\x63t\x18\x05 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectB\n\xfa\x42\x07\x82\x01\x04\x18\x01\x18\x02R\x06\x65\x66\x66\x65\x63t\x12<\n\x04name\x18\x06 \x01(\tB(\xfa\x42%r#2!^([[:alpha:]][[:word:]\\@\\.\\-]*)*$R\x04name\x12\x30\n\x06output\x18\x07 \x01(\x0b\x32\x18.cerbos.policy.v1.OutputR\x06output\"\xe9\x02\n\x0fPrincipalPolicy\x12\x66\n\tprincipal\x18\x01 \x01(\tBH\xfa\x42\x45rC\x10\x01\x32?^[[:alpha:]][[:word:]\\@\\.\\-]*(\\:[[:alpha:]][[:word:]\\@\\.\\-]*)*$R\tprincipal\x12.\n\x07version\x18\x02 \x01(\tB\x14\xfa\x42\x11r\x0f\x32\r^[[:word:]]+$R\x07version\x12\x35\n\x05rules\x18\x03 \x03(\x0b\x32\x1f.cerbos.policy.v1.PrincipalRuleR\x05rules\x12L\n\x05scope\x18\x04 \x01(\tB6\xfa\x42\x33r12/^([[:alnum:]][[:word:]\\-]*(\\.[[:word:]\\-]*)*)*$R\x05scope\x12\x39\n\tvariables\x18\x05 \x01(\x0b\x32\x1b.cerbos.policy.v1.VariablesR\tvariables\"\x95\x03\n\rPrincipalRule\x12#\n\x08resource\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08resource\x12J\n\x07\x61\x63tions\x18\x02 \x03(\x0b\x32&.cerbos.policy.v1.PrincipalRule.ActionB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x07\x61\x63tions\x1a\x92\x02\n\x06\x41\x63tion\x12\x1f\n\x06\x61\x63tion\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x06\x61\x63tion\x12\x39\n\tcondition\x18\x02 \x01(\x0b\x32\x1b.cerbos.policy.v1.ConditionR\tcondition\x12<\n\x06\x65\x66\x66\x65\x63t\x18\x03 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectB\n\xfa\x42\x07\x82\x01\x04\x18\x01\x18\x02R\x06\x65\x66\x66\x65\x63t\x12<\n\x04name\x18\x04 \x01(\tB(\xfa\x42%r#2!^([[:alpha:]][[:word:]\\@\\.\\-]*)*$R\x04name\x12\x30\n\x06output\x18\x05 \x01(\x0b\x32\x18.cerbos.policy.v1.OutputR\x06output\"\xc0\x01\n\x0c\x44\x65rivedRoles\x12.\n\x04name\x18\x01 \x01(\tB\x1a\xfa\x42\x17r\x15\x10\x01\x32\x11^[[:word:]\\-\\.]+$R\x04name\x12\x45\n\x0b\x64\x65\x66initions\x18\x02 \x03(\x0b\x32\x19.cerbos.policy.v1.RoleDefB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x0b\x64\x65\x66initions\x12\x39\n\tvariables\x18\x03 \x01(\x0b\x32\x1b.cerbos.policy.v1.VariablesR\tvariables\"\xbd\x01\n\x07RoleDef\x12,\n\x04name\x18\x01 \x01(\tB\x18\xfa\x42\x15r\x13\x32\x11^[[:word:]\\-\\.]+$R\x04name\x12I\n\x0cparent_roles\x18\x02 \x03(\tB&\xfa\x42#\x92\x01 \x08\x01\x18\x01\"\x1ar\x18\x32\x16^([[:word:]\\-\\.]+|\\*)$R\x0bparentRoles\x12\x39\n\tcondition\x18\x03 \x01(\x0b\x32\x1b.cerbos.policy.v1.ConditionR\tcondition\"\xd7\x01\n\x0f\x45xportVariables\x12.\n\x04name\x18\x01 \x01(\tB\x1a\xfa\x42\x17r\x15\x10\x01\x32\x11^[[:word:]\\-\\.]+$R\x04name\x12T\n\x0b\x64\x65\x66initions\x18\x02 \x03(\x0b\x32\x32.cerbos.policy.v1.ExportVariables.DefinitionsEntryR\x0b\x64\x65\x66initions\x1a>\n\x10\x44\x65\x66initionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xbc\x01\n\tVariables\x12\x37\n\x06import\x18\x01 \x03(\tB\x1f\xfa\x42\x1c\x92\x01\x19\x18\x01\"\x15r\x13\x32\x11^[[:word:]\\-\\.]+$R\x06import\x12<\n\x05local\x18\x02 \x03(\x0b\x32&.cerbos.policy.v1.Variables.LocalEntryR\x05local\x1a\x38\n\nLocalEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"h\n\tCondition\x12/\n\x05match\x18\x01 \x01(\x0b\x32\x17.cerbos.policy.v1.MatchH\x00R\x05match\x12\x18\n\x06script\x18\x02 \x01(\tH\x00R\x06scriptB\x10\n\tcondition\x12\x03\xf8\x42\x01\"\x8b\x02\n\x05Match\x12\x34\n\x03\x61ll\x18\x01 \x01(\x0b\x32 .cerbos.policy.v1.Match.ExprListH\x00R\x03\x61ll\x12\x34\n\x03\x61ny\x18\x02 \x01(\x0b\x32 .cerbos.policy.v1.Match.ExprListH\x00R\x03\x61ny\x12\x36\n\x04none\x18\x03 \x01(\x0b\x32 .cerbos.policy.v1.Match.ExprListH\x00R\x04none\x12\x14\n\x04\x65xpr\x18\x04 \x01(\tH\x00R\x04\x65xpr\x1a=\n\x08\x45xprList\x12\x31\n\x02of\x18\x01 \x03(\x0b\x32\x17.cerbos.policy.v1.MatchB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x02ofB\t\n\x02op\x12\x03\xf8\x42\x01\"\x1c\n\x06Output\x12\x12\n\x04\x65xpr\x18\x01 \x01(\tR\x04\x65xpr\"\xc7\x02\n\x07Schemas\x12K\n\x10principal_schema\x18\x01 \x01(\x0b\x32 .cerbos.policy.v1.Schemas.SchemaR\x0fprincipalSchema\x12I\n\x0fresource_schema\x18\x02 \x01(\x0b\x32 .cerbos.policy.v1.Schemas.SchemaR\x0eresourceSchema\x1a\x38\n\nIgnoreWhen\x12*\n\x07\x61\x63tions\x18\x01 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x08\x01\x18\x01\"\x04r\x02\x10\x01R\x07\x61\x63tions\x1aj\n\x06Schema\x12\x19\n\x03ref\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x03ref\x12\x45\n\x0bignore_when\x18\x02 \x01(\x0b\x32$.cerbos.policy.v1.Schemas.IgnoreWhenR\nignoreWhen\"\x9c\x05\n\x0bTestFixture\x1a\xe0\x01\n\nPrincipals\x12X\n\nprincipals\x18\x01 \x03(\x0b\x32\x38.cerbos.policy.v1.TestFixture.Principals.PrincipalsEntryR\nprincipals\x12\x1c\n\x0bjson_schema\x18\x02 \x01(\tR\x07$schema\x1aZ\n\x0fPrincipalsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.cerbos.engine.v1.PrincipalR\x05value:\x02\x38\x01\x1a\xd9\x01\n\tResources\x12T\n\tresources\x18\x01 \x03(\x0b\x32\x36.cerbos.policy.v1.TestFixture.Resources.ResourcesEntryR\tresources\x12\x1c\n\x0bjson_schema\x18\x02 \x01(\tR\x07$schema\x1aX\n\x0eResourcesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32\x1a.cerbos.engine.v1.ResourceR\x05value:\x02\x38\x01\x1a\xcd\x01\n\x07\x41uxData\x12M\n\x08\x61ux_data\x18\x01 \x03(\x0b\x32\x32.cerbos.policy.v1.TestFixture.AuxData.AuxDataEntryR\x07\x61uxData\x12\x1c\n\x0bjson_schema\x18\x02 \x01(\tR\x07$schema\x1aU\n\x0c\x41uxDataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12/\n\x05value\x18\x02 \x01(\x0b\x32\x19.cerbos.engine.v1.AuxDataR\x05value:\x02\x38\x01\";\n\x0bTestOptions\x12,\n\x03now\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x03now\"\xfc\x05\n\tTestSuite\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x12\n\x04skip\x18\x03 \x01(\x08R\x04skip\x12\x1f\n\x0bskip_reason\x18\x04 \x01(\tR\nskipReason\x12;\n\x05tests\x18\x05 \x03(\x0b\x32\x1b.cerbos.policy.v1.TestTableB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x05tests\x12K\n\nprincipals\x18\x06 \x03(\x0b\x32+.cerbos.policy.v1.TestSuite.PrincipalsEntryR\nprincipals\x12H\n\tresources\x18\x07 \x03(\x0b\x32*.cerbos.policy.v1.TestSuite.ResourcesEntryR\tresources\x12\x43\n\x08\x61ux_data\x18\x08 \x03(\x0b\x32(.cerbos.policy.v1.TestSuite.AuxDataEntryR\x07\x61uxData\x12\x37\n\x07options\x18\t \x01(\x0b\x32\x1d.cerbos.policy.v1.TestOptionsR\x07options\x12\x1c\n\x0bjson_schema\x18\n \x01(\tR\x07$schema\x1aZ\n\x0fPrincipalsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.cerbos.engine.v1.PrincipalR\x05value:\x02\x38\x01\x1aX\n\x0eResourcesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32\x1a.cerbos.engine.v1.ResourceR\x05value:\x02\x38\x01\x1aU\n\x0c\x41uxDataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12/\n\x05value\x18\x02 \x01(\x0b\x32\x19.cerbos.engine.v1.AuxDataR\x05value:\x02\x38\x01\"\xd5\x07\n\tTestTable\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x12\n\x04skip\x18\x03 \x01(\x08R\x04skip\x12\x1f\n\x0bskip_reason\x18\x04 \x01(\tR\nskipReason\x12\x41\n\x05input\x18\x05 \x01(\x0b\x32!.cerbos.policy.v1.TestTable.InputB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x05input\x12M\n\x08\x65xpected\x18\x06 \x03(\x0b\x32\'.cerbos.policy.v1.TestTable.ExpectationB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x08\x65xpected\x12\x37\n\x07options\x18\x07 \x01(\x0b\x32\x1d.cerbos.policy.v1.TestOptionsR\x07options\x1a\xb0\x01\n\x05Input\x12\x30\n\nprincipals\x18\x01 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x08\x01\x18\x01\"\x04r\x02\x10\x01R\nprincipals\x12.\n\tresources\x18\x02 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x08\x01\x18\x01\"\x04r\x02\x10\x01R\tresources\x12*\n\x07\x61\x63tions\x18\x03 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x08\x01\x18\x01\"\x04r\x02\x10\x01R\x07\x61\x63tions\x12\x19\n\x08\x61ux_data\x18\x04 \x01(\tR\x07\x61uxData\x1az\n\x12OutputExpectations\x12\x1f\n\x06\x61\x63tion\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x06\x61\x63tion\x12\x43\n\x08\x65xpected\x18\x02 \x03(\x0b\x32\x1d.cerbos.engine.v1.OutputEntryB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x08\x65xpected\x1a\xd9\x02\n\x0b\x45xpectation\x12%\n\tprincipal\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\tprincipal\x12#\n\x08resource\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08resource\x12^\n\x07\x61\x63tions\x18\x03 \x03(\x0b\x32\x34.cerbos.policy.v1.TestTable.Expectation.ActionsEntryB\x0e\xfa\x42\x0b\x9a\x01\x08\x08\x01\"\x04r\x02\x10\x01R\x07\x61\x63tions\x12H\n\x07outputs\x18\x04 \x03(\x0b\x32..cerbos.policy.v1.TestTable.OutputExpectationsR\x07outputs\x1aT\n\x0c\x41\x63tionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12.\n\x05value\x18\x02 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectR\x05value:\x02\x38\x01\"\xc9\x07\n\x04Test\x12=\n\x04name\x18\x01 \x01(\x0b\x32\x1f.cerbos.policy.v1.Test.TestNameB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x12\n\x04skip\x18\x03 \x01(\x08R\x04skip\x12\x1f\n\x0bskip_reason\x18\x04 \x01(\tR\nskipReason\x12<\n\x05input\x18\x05 \x01(\x0b\x32\x1c.cerbos.engine.v1.CheckInputB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x05input\x12P\n\x08\x65xpected\x18\x06 \x03(\x0b\x32$.cerbos.policy.v1.Test.ExpectedEntryB\x0e\xfa\x42\x0b\x9a\x01\x08\x08\x01\"\x04r\x02\x10\x01R\x08\x65xpected\x12\x37\n\x07options\x18\x07 \x01(\x0b\x32\x1d.cerbos.policy.v1.TestOptionsR\x07options\x12V\n\x10\x65xpected_outputs\x18\x08 \x03(\x0b\x32+.cerbos.policy.v1.Test.ExpectedOutputsEntryR\x0f\x65xpectedOutputs\x1a\x95\x01\n\x08TestName\x12/\n\x0ftest_table_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\rtestTableName\x12,\n\rprincipal_key\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0cprincipalKey\x12*\n\x0cresource_key\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0bresourceKey\x1a\xb0\x01\n\rOutputEntries\x12K\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x31.cerbos.policy.v1.Test.OutputEntries.EntriesEntryR\x07\x65ntries\x1aR\n\x0c\x45ntriesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01\x1aU\n\rExpectedEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12.\n\x05value\x18\x02 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectR\x05value:\x02\x38\x01\x1ah\n\x14\x45xpectedOutputsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12:\n\x05value\x18\x02 \x01(\x0b\x32$.cerbos.policy.v1.Test.OutputEntriesR\x05value:\x02\x38\x01\"\xb0\x10\n\x0bTestResults\x12;\n\x06suites\x18\x01 \x03(\x0b\x32#.cerbos.policy.v1.TestResults.SuiteR\x06suites\x12?\n\x07summary\x18\x02 \x01(\x0b\x32%.cerbos.policy.v1.TestResults.SummaryR\x07summary\x1a[\n\x05Tally\x12<\n\x06result\x18\x01 \x01(\x0e\x32$.cerbos.policy.v1.TestResults.ResultR\x06result\x12\x14\n\x05\x63ount\x18\x02 \x01(\rR\x05\x63ount\x1a\xc1\x01\n\x07Summary\x12K\n\x0eoverall_result\x18\x01 \x01(\x0e\x32$.cerbos.policy.v1.TestResults.ResultR\roverallResult\x12\x1f\n\x0btests_count\x18\x02 \x01(\rR\ntestsCount\x12H\n\rresult_counts\x18\x03 \x03(\x0b\x32#.cerbos.policy.v1.TestResults.TallyR\x0cresultCounts\x1a\xbc\x02\n\x05Suite\x12\x12\n\x04\x66ile\x18\x01 \x01(\tR\x04\x66ile\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12K\n\nprincipals\x18\x03 \x03(\x0b\x32\'.cerbos.policy.v1.TestResults.PrincipalB\x02\x18\x01R\nprincipals\x12?\n\x07summary\x18\x04 \x01(\x0b\x32%.cerbos.policy.v1.TestResults.SummaryR\x07summary\x12\x14\n\x05\x65rror\x18\x05 \x01(\tR\x05\x65rror\x12\x45\n\ntest_cases\x18\x06 \x03(\x0b\x32&.cerbos.policy.v1.TestResults.TestCaseR\ttestCases\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x1ag\n\x08TestCase\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12G\n\nprincipals\x18\x02 \x03(\x0b\x32\'.cerbos.policy.v1.TestResults.PrincipalR\nprincipals\x1a\x65\n\tPrincipal\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x44\n\tresources\x18\x02 \x03(\x0b\x32&.cerbos.policy.v1.TestResults.ResourceR\tresources\x1a^\n\x08Resource\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x07\x61\x63tions\x18\x02 \x03(\x0b\x32$.cerbos.policy.v1.TestResults.ActionR\x07\x61\x63tions\x1a]\n\x06\x41\x63tion\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x07\x64\x65tails\x18\x02 \x01(\x0b\x32%.cerbos.policy.v1.TestResults.DetailsR\x07\x64\x65tails\x1a\xe9\x01\n\x07\x44\x65tails\x12<\n\x06result\x18\x01 \x01(\x0e\x32$.cerbos.policy.v1.TestResults.ResultR\x06result\x12\x41\n\x07\x66\x61ilure\x18\x02 \x01(\x0b\x32%.cerbos.policy.v1.TestResults.FailureH\x00R\x07\x66\x61ilure\x12\x16\n\x05\x65rror\x18\x03 \x01(\tH\x00R\x05\x65rror\x12:\n\x0c\x65ngine_trace\x18\x04 \x03(\x0b\x32\x17.cerbos.engine.v1.TraceR\x0b\x65ngineTraceB\t\n\x07outcome\x1a\x9c\x03\n\rOutputFailure\x12\x10\n\x03src\x18\x01 \x01(\tR\x03src\x12]\n\nmismatched\x18\x02 \x01(\x0b\x32;.cerbos.policy.v1.TestResults.OutputFailure.MismatchedValueH\x00R\nmismatched\x12T\n\x07missing\x18\x03 \x01(\x0b\x32\x38.cerbos.policy.v1.TestResults.OutputFailure.MissingValueH\x00R\x07missing\x1au\n\x0fMismatchedValue\x12\x32\n\x08\x65xpected\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x08\x65xpected\x12.\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x06\x61\x63tual\x1a\x42\n\x0cMissingValue\x12\x32\n\x08\x65xpected\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x08\x65xpectedB\t\n\x07outcome\x1a\xb8\x01\n\x07\x46\x61ilure\x12\x34\n\x08\x65xpected\x18\x01 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectR\x08\x65xpected\x12\x30\n\x06\x61\x63tual\x18\x02 \x01(\x0e\x32\x18.cerbos.effect.v1.EffectR\x06\x61\x63tual\x12\x45\n\x07outputs\x18\x03 \x03(\x0b\x32+.cerbos.policy.v1.TestResults.OutputFailureR\x07outputs\"n\n\x06Result\x12\x16\n\x12RESULT_UNSPECIFIED\x10\x00\x12\x12\n\x0eRESULT_SKIPPED\x10\x01\x12\x11\n\rRESULT_PASSED\x10\x02\x12\x11\n\rRESULT_FAILED\x10\x03\x12\x12\n\x0eRESULT_ERRORED\x10\x04\x42o\n\x18\x64\x65v.cerbos.api.v1.policyZ<github.com/cerbos/cerbos/api/genpb/cerbos/policy/v1;policyv1\xaa\x02\x14\x43\x65rbos.Api.V1.Policyb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'cerbos.policy.v1.policy_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\030dev.cerbos.api.v1.policyZ<github.com/cerbos/cerbos/api/genpb/cerbos/policy/v1;policyv1\252\002\024Cerbos.Api.V1.Policy'
   _POLICY_VARIABLESENTRY._options = None
   _POLICY_VARIABLESENTRY._serialized_options = b'8\001'
   _POLICY.oneofs_by_name['policy_type']._options = None
   _POLICY.oneofs_by_name['policy_type']._serialized_options = b'\370B\001'
   _POLICY.fields_by_name['api_version']._options = None
   _POLICY.fields_by_name['api_version']._serialized_options = b'\372B\025r\023\n\021api.cerbos.dev/v1'
+  _POLICY.fields_by_name['variables']._options = None
+  _POLICY.fields_by_name['variables']._serialized_options = b'\030\001'
   _METADATA_ANNOTATIONSENTRY._options = None
   _METADATA_ANNOTATIONSENTRY._serialized_options = b'8\001'
   _METADATA.fields_by_name['store_identifer']._options = None
   _METADATA.fields_by_name['store_identifer']._serialized_options = b'\030\001'
   _RESOURCEPOLICY.fields_by_name['resource']._options = None
   _RESOURCEPOLICY.fields_by_name['resource']._serialized_options = b'\372BGrE\020\0012A^[[:alpha:]][[:word:]\\@\\.\\-/]*(\\:[[:alpha:]][[:word:]\\@\\.\\-/]*)*$'
   _RESOURCEPOLICY.fields_by_name['version']._options = None
@@ -76,14 +78,22 @@
   _DERIVEDROLES.fields_by_name['name']._serialized_options = b'\372B\027r\025\020\0012\021^[[:word:]\\-\\.]+$'
   _DERIVEDROLES.fields_by_name['definitions']._options = None
   _DERIVEDROLES.fields_by_name['definitions']._serialized_options = b'\372B\005\222\001\002\010\001'
   _ROLEDEF.fields_by_name['name']._options = None
   _ROLEDEF.fields_by_name['name']._serialized_options = b'\372B\025r\0232\021^[[:word:]\\-\\.]+$'
   _ROLEDEF.fields_by_name['parent_roles']._options = None
   _ROLEDEF.fields_by_name['parent_roles']._serialized_options = b'\372B#\222\001 \010\001\030\001\"\032r\0302\026^([[:word:]\\-\\.]+|\\*)$'
+  _EXPORTVARIABLES_DEFINITIONSENTRY._options = None
+  _EXPORTVARIABLES_DEFINITIONSENTRY._serialized_options = b'8\001'
+  _EXPORTVARIABLES.fields_by_name['name']._options = None
+  _EXPORTVARIABLES.fields_by_name['name']._serialized_options = b'\372B\027r\025\020\0012\021^[[:word:]\\-\\.]+$'
+  _VARIABLES_LOCALENTRY._options = None
+  _VARIABLES_LOCALENTRY._serialized_options = b'8\001'
+  _VARIABLES.fields_by_name['import']._options = None
+  _VARIABLES.fields_by_name['import']._serialized_options = b'\372B\034\222\001\031\030\001\"\025r\0232\021^[[:word:]\\-\\.]+$'
   _CONDITION.oneofs_by_name['condition']._options = None
   _CONDITION.oneofs_by_name['condition']._serialized_options = b'\370B\001'
   _MATCH_EXPRLIST.fields_by_name['of']._options = None
   _MATCH_EXPRLIST.fields_by_name['of']._serialized_options = b'\372B\005\222\001\002\010\001'
   _MATCH.oneofs_by_name['op']._options = None
   _MATCH.oneofs_by_name['op']._serialized_options = b'\370B\001'
   _SCHEMAS_IGNOREWHEN.fields_by_name['actions']._options = None
@@ -147,117 +157,125 @@
   _TEST.fields_by_name['input']._options = None
   _TEST.fields_by_name['input']._serialized_options = b'\372B\005\212\001\002\020\001'
   _TEST.fields_by_name['expected']._options = None
   _TEST.fields_by_name['expected']._serialized_options = b'\372B\013\232\001\010\010\001\"\004r\002\020\001'
   _TESTRESULTS_SUITE.fields_by_name['principals']._options = None
   _TESTRESULTS_SUITE.fields_by_name['principals']._serialized_options = b'\030\001'
   _globals['_POLICY']._serialized_start=234
-  _globals['_POLICY']._serialized_end=830
-  _globals['_POLICY_VARIABLESENTRY']._serialized_start=750
-  _globals['_POLICY_VARIABLESENTRY']._serialized_end=810
-  _globals['_METADATA']._serialized_start=833
-  _globals['_METADATA']._serialized_end=1157
-  _globals['_METADATA_ANNOTATIONSENTRY']._serialized_start=1095
-  _globals['_METADATA_ANNOTATIONSENTRY']._serialized_end=1157
-  _globals['_RESOURCEPOLICY']._serialized_start=1160
-  _globals['_RESOURCEPOLICY']._serialized_end=1596
-  _globals['_RESOURCERULE']._serialized_start=1599
-  _globals['_RESOURCERULE']._serialized_end=2020
-  _globals['_PRINCIPALPOLICY']._serialized_start=2023
-  _globals['_PRINCIPALPOLICY']._serialized_end=2325
-  _globals['_PRINCIPALRULE']._serialized_start=2328
-  _globals['_PRINCIPALRULE']._serialized_end=2733
-  _globals['_PRINCIPALRULE_ACTION']._serialized_start=2459
-  _globals['_PRINCIPALRULE_ACTION']._serialized_end=2733
-  _globals['_DERIVEDROLES']._serialized_start=2736
-  _globals['_DERIVEDROLES']._serialized_end=2869
-  _globals['_ROLEDEF']._serialized_start=2872
-  _globals['_ROLEDEF']._serialized_end=3061
-  _globals['_CONDITION']._serialized_start=3063
-  _globals['_CONDITION']._serialized_end=3167
-  _globals['_MATCH']._serialized_start=3170
-  _globals['_MATCH']._serialized_end=3437
-  _globals['_MATCH_EXPRLIST']._serialized_start=3365
-  _globals['_MATCH_EXPRLIST']._serialized_end=3426
-  _globals['_OUTPUT']._serialized_start=3439
-  _globals['_OUTPUT']._serialized_end=3467
-  _globals['_SCHEMAS']._serialized_start=3470
-  _globals['_SCHEMAS']._serialized_end=3797
-  _globals['_SCHEMAS_IGNOREWHEN']._serialized_start=3633
-  _globals['_SCHEMAS_IGNOREWHEN']._serialized_end=3689
-  _globals['_SCHEMAS_SCHEMA']._serialized_start=3691
-  _globals['_SCHEMAS_SCHEMA']._serialized_end=3797
-  _globals['_TESTFIXTURE']._serialized_start=3800
-  _globals['_TESTFIXTURE']._serialized_end=4468
-  _globals['_TESTFIXTURE_PRINCIPALS']._serialized_start=3816
-  _globals['_TESTFIXTURE_PRINCIPALS']._serialized_end=4040
-  _globals['_TESTFIXTURE_PRINCIPALS_PRINCIPALSENTRY']._serialized_start=3950
-  _globals['_TESTFIXTURE_PRINCIPALS_PRINCIPALSENTRY']._serialized_end=4040
-  _globals['_TESTFIXTURE_RESOURCES']._serialized_start=4043
-  _globals['_TESTFIXTURE_RESOURCES']._serialized_end=4260
-  _globals['_TESTFIXTURE_RESOURCES_RESOURCESENTRY']._serialized_start=4172
-  _globals['_TESTFIXTURE_RESOURCES_RESOURCESENTRY']._serialized_end=4260
-  _globals['_TESTFIXTURE_AUXDATA']._serialized_start=4263
-  _globals['_TESTFIXTURE_AUXDATA']._serialized_end=4468
-  _globals['_TESTFIXTURE_AUXDATA_AUXDATAENTRY']._serialized_start=4383
-  _globals['_TESTFIXTURE_AUXDATA_AUXDATAENTRY']._serialized_end=4468
-  _globals['_TESTOPTIONS']._serialized_start=4470
-  _globals['_TESTOPTIONS']._serialized_end=4529
-  _globals['_TESTSUITE']._serialized_start=4532
-  _globals['_TESTSUITE']._serialized_end=5296
-  _globals['_TESTSUITE_PRINCIPALSENTRY']._serialized_start=3950
-  _globals['_TESTSUITE_PRINCIPALSENTRY']._serialized_end=4040
-  _globals['_TESTSUITE_RESOURCESENTRY']._serialized_start=4172
-  _globals['_TESTSUITE_RESOURCESENTRY']._serialized_end=4260
-  _globals['_TESTSUITE_AUXDATAENTRY']._serialized_start=4383
-  _globals['_TESTSUITE_AUXDATAENTRY']._serialized_end=4468
-  _globals['_TESTTABLE']._serialized_start=5299
-  _globals['_TESTTABLE']._serialized_end=6280
-  _globals['_TESTTABLE_INPUT']._serialized_start=5632
-  _globals['_TESTTABLE_INPUT']._serialized_end=5808
-  _globals['_TESTTABLE_OUTPUTEXPECTATIONS']._serialized_start=5810
-  _globals['_TESTTABLE_OUTPUTEXPECTATIONS']._serialized_end=5932
-  _globals['_TESTTABLE_EXPECTATION']._serialized_start=5935
-  _globals['_TESTTABLE_EXPECTATION']._serialized_end=6280
-  _globals['_TESTTABLE_EXPECTATION_ACTIONSENTRY']._serialized_start=6196
-  _globals['_TESTTABLE_EXPECTATION_ACTIONSENTRY']._serialized_end=6280
-  _globals['_TEST']._serialized_start=6283
-  _globals['_TEST']._serialized_end=7252
-  _globals['_TEST_TESTNAME']._serialized_start=6731
-  _globals['_TEST_TESTNAME']._serialized_end=6880
-  _globals['_TEST_OUTPUTENTRIES']._serialized_start=6883
-  _globals['_TEST_OUTPUTENTRIES']._serialized_end=7059
-  _globals['_TEST_OUTPUTENTRIES_ENTRIESENTRY']._serialized_start=6977
-  _globals['_TEST_OUTPUTENTRIES_ENTRIESENTRY']._serialized_end=7059
-  _globals['_TEST_EXPECTEDENTRY']._serialized_start=7061
-  _globals['_TEST_EXPECTEDENTRY']._serialized_end=7146
-  _globals['_TEST_EXPECTEDOUTPUTSENTRY']._serialized_start=7148
-  _globals['_TEST_EXPECTEDOUTPUTSENTRY']._serialized_end=7252
-  _globals['_TESTRESULTS']._serialized_start=7255
-  _globals['_TESTRESULTS']._serialized_end=9351
-  _globals['_TESTRESULTS_TALLY']._serialized_start=7396
-  _globals['_TESTRESULTS_TALLY']._serialized_end=7487
-  _globals['_TESTRESULTS_SUMMARY']._serialized_start=7490
-  _globals['_TESTRESULTS_SUMMARY']._serialized_end=7683
-  _globals['_TESTRESULTS_SUITE']._serialized_start=7686
-  _globals['_TESTRESULTS_SUITE']._serialized_end=8002
-  _globals['_TESTRESULTS_TESTCASE']._serialized_start=8004
-  _globals['_TESTRESULTS_TESTCASE']._serialized_end=8107
-  _globals['_TESTRESULTS_PRINCIPAL']._serialized_start=8109
-  _globals['_TESTRESULTS_PRINCIPAL']._serialized_end=8210
-  _globals['_TESTRESULTS_RESOURCE']._serialized_start=8212
-  _globals['_TESTRESULTS_RESOURCE']._serialized_end=8306
-  _globals['_TESTRESULTS_ACTION']._serialized_start=8308
-  _globals['_TESTRESULTS_ACTION']._serialized_end=8401
-  _globals['_TESTRESULTS_DETAILS']._serialized_start=8404
-  _globals['_TESTRESULTS_DETAILS']._serialized_end=8637
-  _globals['_TESTRESULTS_OUTPUTFAILURE']._serialized_start=8640
-  _globals['_TESTRESULTS_OUTPUTFAILURE']._serialized_end=9052
-  _globals['_TESTRESULTS_OUTPUTFAILURE_MISMATCHEDVALUE']._serialized_start=8856
-  _globals['_TESTRESULTS_OUTPUTFAILURE_MISMATCHEDVALUE']._serialized_end=8973
-  _globals['_TESTRESULTS_OUTPUTFAILURE_MISSINGVALUE']._serialized_start=8975
-  _globals['_TESTRESULTS_OUTPUTFAILURE_MISSINGVALUE']._serialized_end=9041
-  _globals['_TESTRESULTS_FAILURE']._serialized_start=9055
-  _globals['_TESTRESULTS_FAILURE']._serialized_end=9239
-  _globals['_TESTRESULTS_RESULT']._serialized_start=9241
-  _globals['_TESTRESULTS_RESULT']._serialized_end=9351
+  _globals['_POLICY']._serialized_end=914
+  _globals['_POLICY_VARIABLESENTRY']._serialized_start=834
+  _globals['_POLICY_VARIABLESENTRY']._serialized_end=894
+  _globals['_METADATA']._serialized_start=917
+  _globals['_METADATA']._serialized_end=1241
+  _globals['_METADATA_ANNOTATIONSENTRY']._serialized_start=1179
+  _globals['_METADATA_ANNOTATIONSENTRY']._serialized_end=1241
+  _globals['_RESOURCEPOLICY']._serialized_start=1244
+  _globals['_RESOURCEPOLICY']._serialized_end=1739
+  _globals['_RESOURCERULE']._serialized_start=1742
+  _globals['_RESOURCERULE']._serialized_end=2163
+  _globals['_PRINCIPALPOLICY']._serialized_start=2166
+  _globals['_PRINCIPALPOLICY']._serialized_end=2527
+  _globals['_PRINCIPALRULE']._serialized_start=2530
+  _globals['_PRINCIPALRULE']._serialized_end=2935
+  _globals['_PRINCIPALRULE_ACTION']._serialized_start=2661
+  _globals['_PRINCIPALRULE_ACTION']._serialized_end=2935
+  _globals['_DERIVEDROLES']._serialized_start=2938
+  _globals['_DERIVEDROLES']._serialized_end=3130
+  _globals['_ROLEDEF']._serialized_start=3133
+  _globals['_ROLEDEF']._serialized_end=3322
+  _globals['_EXPORTVARIABLES']._serialized_start=3325
+  _globals['_EXPORTVARIABLES']._serialized_end=3540
+  _globals['_EXPORTVARIABLES_DEFINITIONSENTRY']._serialized_start=3478
+  _globals['_EXPORTVARIABLES_DEFINITIONSENTRY']._serialized_end=3540
+  _globals['_VARIABLES']._serialized_start=3543
+  _globals['_VARIABLES']._serialized_end=3731
+  _globals['_VARIABLES_LOCALENTRY']._serialized_start=3675
+  _globals['_VARIABLES_LOCALENTRY']._serialized_end=3731
+  _globals['_CONDITION']._serialized_start=3733
+  _globals['_CONDITION']._serialized_end=3837
+  _globals['_MATCH']._serialized_start=3840
+  _globals['_MATCH']._serialized_end=4107
+  _globals['_MATCH_EXPRLIST']._serialized_start=4035
+  _globals['_MATCH_EXPRLIST']._serialized_end=4096
+  _globals['_OUTPUT']._serialized_start=4109
+  _globals['_OUTPUT']._serialized_end=4137
+  _globals['_SCHEMAS']._serialized_start=4140
+  _globals['_SCHEMAS']._serialized_end=4467
+  _globals['_SCHEMAS_IGNOREWHEN']._serialized_start=4303
+  _globals['_SCHEMAS_IGNOREWHEN']._serialized_end=4359
+  _globals['_SCHEMAS_SCHEMA']._serialized_start=4361
+  _globals['_SCHEMAS_SCHEMA']._serialized_end=4467
+  _globals['_TESTFIXTURE']._serialized_start=4470
+  _globals['_TESTFIXTURE']._serialized_end=5138
+  _globals['_TESTFIXTURE_PRINCIPALS']._serialized_start=4486
+  _globals['_TESTFIXTURE_PRINCIPALS']._serialized_end=4710
+  _globals['_TESTFIXTURE_PRINCIPALS_PRINCIPALSENTRY']._serialized_start=4620
+  _globals['_TESTFIXTURE_PRINCIPALS_PRINCIPALSENTRY']._serialized_end=4710
+  _globals['_TESTFIXTURE_RESOURCES']._serialized_start=4713
+  _globals['_TESTFIXTURE_RESOURCES']._serialized_end=4930
+  _globals['_TESTFIXTURE_RESOURCES_RESOURCESENTRY']._serialized_start=4842
+  _globals['_TESTFIXTURE_RESOURCES_RESOURCESENTRY']._serialized_end=4930
+  _globals['_TESTFIXTURE_AUXDATA']._serialized_start=4933
+  _globals['_TESTFIXTURE_AUXDATA']._serialized_end=5138
+  _globals['_TESTFIXTURE_AUXDATA_AUXDATAENTRY']._serialized_start=5053
+  _globals['_TESTFIXTURE_AUXDATA_AUXDATAENTRY']._serialized_end=5138
+  _globals['_TESTOPTIONS']._serialized_start=5140
+  _globals['_TESTOPTIONS']._serialized_end=5199
+  _globals['_TESTSUITE']._serialized_start=5202
+  _globals['_TESTSUITE']._serialized_end=5966
+  _globals['_TESTSUITE_PRINCIPALSENTRY']._serialized_start=4620
+  _globals['_TESTSUITE_PRINCIPALSENTRY']._serialized_end=4710
+  _globals['_TESTSUITE_RESOURCESENTRY']._serialized_start=4842
+  _globals['_TESTSUITE_RESOURCESENTRY']._serialized_end=4930
+  _globals['_TESTSUITE_AUXDATAENTRY']._serialized_start=5053
+  _globals['_TESTSUITE_AUXDATAENTRY']._serialized_end=5138
+  _globals['_TESTTABLE']._serialized_start=5969
+  _globals['_TESTTABLE']._serialized_end=6950
+  _globals['_TESTTABLE_INPUT']._serialized_start=6302
+  _globals['_TESTTABLE_INPUT']._serialized_end=6478
+  _globals['_TESTTABLE_OUTPUTEXPECTATIONS']._serialized_start=6480
+  _globals['_TESTTABLE_OUTPUTEXPECTATIONS']._serialized_end=6602
+  _globals['_TESTTABLE_EXPECTATION']._serialized_start=6605
+  _globals['_TESTTABLE_EXPECTATION']._serialized_end=6950
+  _globals['_TESTTABLE_EXPECTATION_ACTIONSENTRY']._serialized_start=6866
+  _globals['_TESTTABLE_EXPECTATION_ACTIONSENTRY']._serialized_end=6950
+  _globals['_TEST']._serialized_start=6953
+  _globals['_TEST']._serialized_end=7922
+  _globals['_TEST_TESTNAME']._serialized_start=7401
+  _globals['_TEST_TESTNAME']._serialized_end=7550
+  _globals['_TEST_OUTPUTENTRIES']._serialized_start=7553
+  _globals['_TEST_OUTPUTENTRIES']._serialized_end=7729
+  _globals['_TEST_OUTPUTENTRIES_ENTRIESENTRY']._serialized_start=7647
+  _globals['_TEST_OUTPUTENTRIES_ENTRIESENTRY']._serialized_end=7729
+  _globals['_TEST_EXPECTEDENTRY']._serialized_start=7731
+  _globals['_TEST_EXPECTEDENTRY']._serialized_end=7816
+  _globals['_TEST_EXPECTEDOUTPUTSENTRY']._serialized_start=7818
+  _globals['_TEST_EXPECTEDOUTPUTSENTRY']._serialized_end=7922
+  _globals['_TESTRESULTS']._serialized_start=7925
+  _globals['_TESTRESULTS']._serialized_end=10021
+  _globals['_TESTRESULTS_TALLY']._serialized_start=8066
+  _globals['_TESTRESULTS_TALLY']._serialized_end=8157
+  _globals['_TESTRESULTS_SUMMARY']._serialized_start=8160
+  _globals['_TESTRESULTS_SUMMARY']._serialized_end=8353
+  _globals['_TESTRESULTS_SUITE']._serialized_start=8356
+  _globals['_TESTRESULTS_SUITE']._serialized_end=8672
+  _globals['_TESTRESULTS_TESTCASE']._serialized_start=8674
+  _globals['_TESTRESULTS_TESTCASE']._serialized_end=8777
+  _globals['_TESTRESULTS_PRINCIPAL']._serialized_start=8779
+  _globals['_TESTRESULTS_PRINCIPAL']._serialized_end=8880
+  _globals['_TESTRESULTS_RESOURCE']._serialized_start=8882
+  _globals['_TESTRESULTS_RESOURCE']._serialized_end=8976
+  _globals['_TESTRESULTS_ACTION']._serialized_start=8978
+  _globals['_TESTRESULTS_ACTION']._serialized_end=9071
+  _globals['_TESTRESULTS_DETAILS']._serialized_start=9074
+  _globals['_TESTRESULTS_DETAILS']._serialized_end=9307
+  _globals['_TESTRESULTS_OUTPUTFAILURE']._serialized_start=9310
+  _globals['_TESTRESULTS_OUTPUTFAILURE']._serialized_end=9722
+  _globals['_TESTRESULTS_OUTPUTFAILURE_MISMATCHEDVALUE']._serialized_start=9526
+  _globals['_TESTRESULTS_OUTPUTFAILURE_MISMATCHEDVALUE']._serialized_end=9643
+  _globals['_TESTRESULTS_OUTPUTFAILURE_MISSINGVALUE']._serialized_start=9645
+  _globals['_TESTRESULTS_OUTPUTFAILURE_MISSINGVALUE']._serialized_end=9711
+  _globals['_TESTRESULTS_FAILURE']._serialized_start=9725
+  _globals['_TESTRESULTS_FAILURE']._serialized_end=9909
+  _globals['_TESTRESULTS_RESULT']._serialized_start=9911
+  _globals['_TESTRESULTS_RESULT']._serialized_end=10021
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cerbos-0.8.1/cerbos/policy/v1/policy_pb2.pyi` & `cerbos-0.9.0/cerbos/policy/v1/policy_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,41 +9,43 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Policy(_message.Message):
-    __slots__ = ["api_version", "disabled", "description", "metadata", "resource_policy", "principal_policy", "derived_roles", "variables", "json_schema"]
+    __slots__ = ["api_version", "disabled", "description", "metadata", "resource_policy", "principal_policy", "derived_roles", "export_variables", "variables", "json_schema"]
     class VariablesEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     API_VERSION_FIELD_NUMBER: _ClassVar[int]
     DISABLED_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     RESOURCE_POLICY_FIELD_NUMBER: _ClassVar[int]
     PRINCIPAL_POLICY_FIELD_NUMBER: _ClassVar[int]
     DERIVED_ROLES_FIELD_NUMBER: _ClassVar[int]
+    EXPORT_VARIABLES_FIELD_NUMBER: _ClassVar[int]
     VARIABLES_FIELD_NUMBER: _ClassVar[int]
     JSON_SCHEMA_FIELD_NUMBER: _ClassVar[int]
     api_version: str
     disabled: bool
     description: str
     metadata: Metadata
     resource_policy: ResourcePolicy
     principal_policy: PrincipalPolicy
     derived_roles: DerivedRoles
+    export_variables: ExportVariables
     variables: _containers.ScalarMap[str, str]
     json_schema: str
-    def __init__(self, api_version: _Optional[str] = ..., disabled: bool = ..., description: _Optional[str] = ..., metadata: _Optional[_Union[Metadata, _Mapping]] = ..., resource_policy: _Optional[_Union[ResourcePolicy, _Mapping]] = ..., principal_policy: _Optional[_Union[PrincipalPolicy, _Mapping]] = ..., derived_roles: _Optional[_Union[DerivedRoles, _Mapping]] = ..., variables: _Optional[_Mapping[str, str]] = ..., json_schema: _Optional[str] = ...) -> None: ...
+    def __init__(self, api_version: _Optional[str] = ..., disabled: bool = ..., description: _Optional[str] = ..., metadata: _Optional[_Union[Metadata, _Mapping]] = ..., resource_policy: _Optional[_Union[ResourcePolicy, _Mapping]] = ..., principal_policy: _Optional[_Union[PrincipalPolicy, _Mapping]] = ..., derived_roles: _Optional[_Union[DerivedRoles, _Mapping]] = ..., export_variables: _Optional[_Union[ExportVariables, _Mapping]] = ..., variables: _Optional[_Mapping[str, str]] = ..., json_schema: _Optional[str] = ...) -> None: ...
 
 class Metadata(_message.Message):
     __slots__ = ["source_file", "annotations", "hash", "store_identifer", "store_identifier"]
     class AnnotationsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
@@ -59,28 +61,30 @@
     annotations: _containers.ScalarMap[str, str]
     hash: _wrappers_pb2.UInt64Value
     store_identifer: str
     store_identifier: str
     def __init__(self, source_file: _Optional[str] = ..., annotations: _Optional[_Mapping[str, str]] = ..., hash: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., store_identifer: _Optional[str] = ..., store_identifier: _Optional[str] = ...) -> None: ...
 
 class ResourcePolicy(_message.Message):
-    __slots__ = ["resource", "version", "import_derived_roles", "rules", "scope", "schemas"]
+    __slots__ = ["resource", "version", "import_derived_roles", "rules", "scope", "schemas", "variables"]
     RESOURCE_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     IMPORT_DERIVED_ROLES_FIELD_NUMBER: _ClassVar[int]
     RULES_FIELD_NUMBER: _ClassVar[int]
     SCOPE_FIELD_NUMBER: _ClassVar[int]
     SCHEMAS_FIELD_NUMBER: _ClassVar[int]
+    VARIABLES_FIELD_NUMBER: _ClassVar[int]
     resource: str
     version: str
     import_derived_roles: _containers.RepeatedScalarFieldContainer[str]
     rules: _containers.RepeatedCompositeFieldContainer[ResourceRule]
     scope: str
     schemas: Schemas
-    def __init__(self, resource: _Optional[str] = ..., version: _Optional[str] = ..., import_derived_roles: _Optional[_Iterable[str]] = ..., rules: _Optional[_Iterable[_Union[ResourceRule, _Mapping]]] = ..., scope: _Optional[str] = ..., schemas: _Optional[_Union[Schemas, _Mapping]] = ...) -> None: ...
+    variables: Variables
+    def __init__(self, resource: _Optional[str] = ..., version: _Optional[str] = ..., import_derived_roles: _Optional[_Iterable[str]] = ..., rules: _Optional[_Iterable[_Union[ResourceRule, _Mapping]]] = ..., scope: _Optional[str] = ..., schemas: _Optional[_Union[Schemas, _Mapping]] = ..., variables: _Optional[_Union[Variables, _Mapping]] = ...) -> None: ...
 
 class ResourceRule(_message.Message):
     __slots__ = ["actions", "derived_roles", "roles", "condition", "effect", "name", "output"]
     ACTIONS_FIELD_NUMBER: _ClassVar[int]
     DERIVED_ROLES_FIELD_NUMBER: _ClassVar[int]
     ROLES_FIELD_NUMBER: _ClassVar[int]
     CONDITION_FIELD_NUMBER: _ClassVar[int]
@@ -93,24 +97,26 @@
     condition: Condition
     effect: _effect_pb2.Effect
     name: str
     output: Output
     def __init__(self, actions: _Optional[_Iterable[str]] = ..., derived_roles: _Optional[_Iterable[str]] = ..., roles: _Optional[_Iterable[str]] = ..., condition: _Optional[_Union[Condition, _Mapping]] = ..., effect: _Optional[_Union[_effect_pb2.Effect, str]] = ..., name: _Optional[str] = ..., output: _Optional[_Union[Output, _Mapping]] = ...) -> None: ...
 
 class PrincipalPolicy(_message.Message):
-    __slots__ = ["principal", "version", "rules", "scope"]
+    __slots__ = ["principal", "version", "rules", "scope", "variables"]
     PRINCIPAL_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     RULES_FIELD_NUMBER: _ClassVar[int]
     SCOPE_FIELD_NUMBER: _ClassVar[int]
+    VARIABLES_FIELD_NUMBER: _ClassVar[int]
     principal: str
     version: str
     rules: _containers.RepeatedCompositeFieldContainer[PrincipalRule]
     scope: str
-    def __init__(self, principal: _Optional[str] = ..., version: _Optional[str] = ..., rules: _Optional[_Iterable[_Union[PrincipalRule, _Mapping]]] = ..., scope: _Optional[str] = ...) -> None: ...
+    variables: Variables
+    def __init__(self, principal: _Optional[str] = ..., version: _Optional[str] = ..., rules: _Optional[_Iterable[_Union[PrincipalRule, _Mapping]]] = ..., scope: _Optional[str] = ..., variables: _Optional[_Union[Variables, _Mapping]] = ...) -> None: ...
 
 class PrincipalRule(_message.Message):
     __slots__ = ["resource", "actions"]
     class Action(_message.Message):
         __slots__ = ["action", "condition", "effect", "name", "output"]
         ACTION_FIELD_NUMBER: _ClassVar[int]
         CONDITION_FIELD_NUMBER: _ClassVar[int]
@@ -126,31 +132,62 @@
     RESOURCE_FIELD_NUMBER: _ClassVar[int]
     ACTIONS_FIELD_NUMBER: _ClassVar[int]
     resource: str
     actions: _containers.RepeatedCompositeFieldContainer[PrincipalRule.Action]
     def __init__(self, resource: _Optional[str] = ..., actions: _Optional[_Iterable[_Union[PrincipalRule.Action, _Mapping]]] = ...) -> None: ...
 
 class DerivedRoles(_message.Message):
-    __slots__ = ["name", "definitions"]
+    __slots__ = ["name", "definitions", "variables"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     DEFINITIONS_FIELD_NUMBER: _ClassVar[int]
+    VARIABLES_FIELD_NUMBER: _ClassVar[int]
     name: str
     definitions: _containers.RepeatedCompositeFieldContainer[RoleDef]
-    def __init__(self, name: _Optional[str] = ..., definitions: _Optional[_Iterable[_Union[RoleDef, _Mapping]]] = ...) -> None: ...
+    variables: Variables
+    def __init__(self, name: _Optional[str] = ..., definitions: _Optional[_Iterable[_Union[RoleDef, _Mapping]]] = ..., variables: _Optional[_Union[Variables, _Mapping]] = ...) -> None: ...
 
 class RoleDef(_message.Message):
     __slots__ = ["name", "parent_roles", "condition"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     PARENT_ROLES_FIELD_NUMBER: _ClassVar[int]
     CONDITION_FIELD_NUMBER: _ClassVar[int]
     name: str
     parent_roles: _containers.RepeatedScalarFieldContainer[str]
     condition: Condition
     def __init__(self, name: _Optional[str] = ..., parent_roles: _Optional[_Iterable[str]] = ..., condition: _Optional[_Union[Condition, _Mapping]] = ...) -> None: ...
 
+class ExportVariables(_message.Message):
+    __slots__ = ["name", "definitions"]
+    class DefinitionsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    DEFINITIONS_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    definitions: _containers.ScalarMap[str, str]
+    def __init__(self, name: _Optional[str] = ..., definitions: _Optional[_Mapping[str, str]] = ...) -> None: ...
+
+class Variables(_message.Message):
+    __slots__ = ["local"]
+    class LocalEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    IMPORT_FIELD_NUMBER: _ClassVar[int]
+    LOCAL_FIELD_NUMBER: _ClassVar[int]
+    local: _containers.ScalarMap[str, str]
+    def __init__(self, local: _Optional[_Mapping[str, str]] = ..., **kwargs) -> None: ...
+
 class Condition(_message.Message):
     __slots__ = ["match", "script"]
     MATCH_FIELD_NUMBER: _ClassVar[int]
     SCRIPT_FIELD_NUMBER: _ClassVar[int]
     match: Match
     script: str
     def __init__(self, match: _Optional[_Union[Match, _Mapping]] = ..., script: _Optional[str] = ...) -> None: ...
```

### Comparing `cerbos-0.8.1/cerbos/request/v1/request_pb2.py` & `cerbos-0.9.0/cerbos/request/v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/request/v1/request_pb2.pyi` & `cerbos-0.9.0/cerbos/request/v1/request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/response/v1/response_pb2.py` & `cerbos-0.9.0/cerbos/response/v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/response/v1/response_pb2.pyi` & `cerbos-0.9.0/cerbos/response/v1/response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/schema/v1/schema_pb2.py` & `cerbos-0.9.0/cerbos/schema/v1/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/schema/v1/schema_pb2.pyi` & `cerbos-0.9.0/cerbos/schema/v1/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/sdk/_async/_grpc.py` & `cerbos-0.9.0/cerbos/sdk/_async/_grpc.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/sdk/_async/_http.py` & `cerbos-0.9.0/cerbos/sdk/_async/_http.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/sdk/_sync/_grpc.py` & `cerbos-0.9.0/cerbos/sdk/_sync/_grpc.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/sdk/_sync/_http.py` & `cerbos-0.9.0/cerbos/sdk/_sync/_http.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/sdk/container.py` & `cerbos-0.9.0/cerbos/sdk/container.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/sdk/grpc/utils.py` & `cerbos-0.9.0/cerbos/sdk/grpc/utils.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/sdk/model.py` & `cerbos-0.9.0/cerbos/sdk/model.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/svc/v1/svc_pb2.py` & `cerbos-0.9.0/cerbos/svc/v1/svc_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/svc/v1/svc_pb2_grpc.py` & `cerbos-0.9.0/cerbos/svc/v1/svc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/telemetry/v1/telemetry_pb2.py` & `cerbos-0.9.0/cerbos/telemetry/v1/telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/cerbos/telemetry/v1/telemetry_pb2.pyi` & `cerbos-0.9.0/cerbos/telemetry/v1/telemetry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/pyproject.toml` & `cerbos-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "httpx[http2]>=0.22.0",
     "anyio>=3.6.1",
     "tenacity>=8.1.0",
     "grpcio-tools>=1.54.2",
 ]
 requires-python = ">=3.8"
 dynamic = []
-version = "0.8.1"
+version = "0.9.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Homepage = "https://cerbos.dev"
```

### Comparing `cerbos-0.8.1/tests/check.py` & `cerbos-0.9.0/tests/check.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/conftest.py` & `cerbos-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/grpc/test_grpc_admin_client.py` & `cerbos-0.9.0/tests/grpc/test_grpc_admin_client.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/grpc/test_grpc_client.py` & `cerbos-0.9.0/tests/grpc/test_grpc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,38 @@
         cerbos_grpc_client: CerbosClient,
         principal_john: engine_pb2.Principal,
         resource_list: List[request_pb2.CheckResourcesRequest.ResourceEntry],
     ):
         have = cerbos_grpc_client.check_resources(principal_john, resource_list)
         _assert_check_resources_with_output(have)
 
+    def test_is_allowed_with_export_variables(
+        self,
+        cerbos_grpc_client: CerbosClient,
+    ):
+        p = engine_pb2.Principal(
+            id="daffy",
+            roles={"user"},
+            policy_version="default",
+            attr={
+                "vip": struct_pb2.Value(bool_value=True),
+            },
+        )
+        r = engine_pb2.Resource(
+            id="XX325",
+            kind="album:object",
+            policy_version="default",
+        )
+        have = cerbos_grpc_client.is_allowed(
+            "view-as-vip",
+            p,
+            r,
+        )
+        assert have
+
 
 class TestPrincipalContext:
     def test_is_allowed(
         self,
         principal_ctx: PrincipalContext,
         resource_john_leave_req: engine_pb2.Resource,
     ):
```

### Comparing `cerbos-0.8.1/tests/http/test_http_client.py` & `cerbos-0.9.0/tests/http/test_http_client.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/http/test_http_plan_response.py` & `cerbos-0.9.0/tests/http/test_http_plan_response.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/store/conf.yaml` & `cerbos-0.9.0/tests/store/conf.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/store/policies/_schemas/leave_request.json` & `cerbos-0.9.0/tests/store/policies/_schemas/leave_request.json`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/store/policies/_schemas/principal.json` & `cerbos-0.9.0/tests/store/policies/_schemas/principal.json`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/store/policies/derived_roles/derived_roles_03.yaml` & `cerbos-0.9.0/tests/store/policies/derived_roles/derived_roles_03.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/store/policies/principal_policies/policy_01.yaml` & `cerbos-0.9.0/tests/store/policies/principal_policies/policy_01.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/store/policies/resource_policies/policy_01.yaml` & `cerbos-0.9.0/tests/store/policies/resource_policies/policy_01.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/store/policies/resource_policies/policy_02.yaml` & `cerbos-0.9.0/tests/store/policies/resource_policies/policy_02.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/store/policies/resource_policies/policy_03.yaml` & `cerbos-0.9.0/tests/store/policies/resource_policies/policy_03.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/store/policies/resource_policies/policy_04.yaml` & `cerbos-0.9.0/tests/store/policies/resource_policies/policy_04.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 ---
 apiVersion: api.cerbos.dev/v1
 resourcePolicy:
   version: "default"
+  variables:
+    import:
+      - vip_variables
   importDerivedRoles:
     - apatr_common_roles
   resource: "album:object"
   rules:
     - actions: ['*']
       effect: EFFECT_ALLOW
       derivedRoles:
@@ -26,8 +29,8 @@
 
     - actions: ['view-as-vip']
       effect: EFFECT_ALLOW
       roles:
         - user
       condition:
         match:
-          expr: request.principal.attr.vip == true
+          expr: V.is_vip
```

### Comparing `cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.hr.uk.yaml` & `cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.hr.uk.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.hr.yaml` & `cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.hr.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.yaml` & `cerbos-0.9.0/tests/store/policies/resource_policies/policy_05_acme.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.8.1/PKG-INFO` & `cerbos-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbos
-Version: 0.8.1
+Version: 0.9.0
 Summary: SDK for working with Cerbos: an open core, language-agnostic, scalable authorization solution
 Author-Email: Cerbos Developers <sdk+python@cerbos.dev>
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
```

