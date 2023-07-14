# Comparing `tmp/frinx_python_sdk-0.1.0.tar.gz` & `tmp/frinx_python_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frinx_python_sdk-0.1.0.tar", max compression
+gzip compressed data, was "frinx_python_sdk-0.1.1.tar", max compression
```

## Comparing `frinx_python_sdk-0.1.0.tar` & `frinx_python_sdk-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,59 @@
--rw-r--r--   0        0        0      592 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/client/__init__.py
--rw-r--r--   0        0        0    12317 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/client/conductor.py
--rw-r--r--   0        0        0    10017 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/client/frinx_conductor_wrapper.py
--rw-r--r--   0        0        0        0 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/__init__.py
--rw-r--r--   0        0        0      838 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/conductor_enums.py
--rw-r--r--   0        0        0     2215 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/frinx_rest.py
--rw-r--r--   0        0        0     3742 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/import_workflows.py
--rw-r--r--   0        0        0      115 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/logging/__init__.py
--rw-r--r--   0        0        0      739 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/logging/logging-config.json
--rw-r--r--   0        0        0     3515 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/logging/logging_common.py
--rw-r--r--   0        0        0        0 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/telemetry/__init__.py
--rw-r--r--   0        0        0     5199 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/telemetry/common.py
--rw-r--r--   0        0        0     1993 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/telemetry/enums.py
--rw-r--r--   0        0        0     3574 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/telemetry/metrics.py
--rw-r--r--   0        0        0       89 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/type_aliases.py
--rw-r--r--   0        0        0     1191 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/util.py
--rw-r--r--   0        0        0        0 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/worker/__init__.py
--rw-r--r--   0        0        0      957 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/worker/service.py
--rw-r--r--   0        0        0     2534 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/worker/task.py
--rw-r--r--   0        0        0     3322 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/worker/task_def.py
--rw-r--r--   0        0        0     1011 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/worker/task_result.py
--rw-r--r--   0        0        0     6212 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/worker/worker.py
--rw-r--r--   0        0        0    13289 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/workflow/WORKFLOW_GENERATOR.md
--rw-r--r--   0        0        0        0 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/workflow/__init__.py
--rw-r--r--   0        0        0     2766 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/workflow/service.py
--rw-r--r--   0        0        0    17690 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/workflow/task.py
--rw-r--r--   0        0        0     4949 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/common/workflow/workflow.py
--rw-r--r--   0        0        0        0 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/services/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/services/uniconfig/__init__.py
--rw-r--r--   0        0        0     3290 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/services/uniconfig/cli_network_topology.py
--rw-r--r--   0        0        0     2589 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/services/uniconfig/connection_manager.py
--rw-r--r--   0        0        0     4899 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/services/uniconfig/snapshot_manager.py
--rw-r--r--   0        0        0     7645 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/services/uniconfig/uniconfig_manager.py
--rw-r--r--   0        0        0        0 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/workers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/workers/uniconfig/__init__.py
--rw-r--r--   0        0        0     2657 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/workers/uniconfig/cli_network_topology.py
--rw-r--r--   0        0        0     2343 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/workers/uniconfig/connection_manager.py
--rw-r--r--   0        0        0     3680 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/workers/uniconfig/snapshot_manager.py
--rw-r--r--   0        0        0     5613 2023-05-25 13:14:28.470162 frinx_python_sdk-0.1.0/frinx/workers/uniconfig/uniconfig_manager.py
--rw-r--r--   0        0        0     2475 2023-05-25 13:14:42.138385 frinx_python_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 frinx_python_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1272 2023-07-14 15:17:47.475514 frinx_python_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.475514 frinx_python_sdk-0.1.1/frinx/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.475514 frinx_python_sdk-0.1.1/frinx/client/__init__.py
+-rw-r--r--   0        0        0    12317 2023-07-14 15:17:47.475514 frinx_python_sdk-0.1.1/frinx/client/conductor.py
+-rw-r--r--   0        0        0    10017 2023-07-14 15:17:47.475514 frinx_python_sdk-0.1.1/frinx/client/frinx_conductor_wrapper.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.475514 frinx_python_sdk-0.1.1/frinx/common/__init__.py
+-rw-r--r--   0        0        0      836 2023-07-14 15:17:47.475514 frinx_python_sdk-0.1.1/frinx/common/conductor_enums.py
+-rw-r--r--   0        0        0     2723 2023-07-14 15:17:47.475514 frinx_python_sdk-0.1.1/frinx/common/frinx_rest.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/graphql/__init__.py
+-rw-r--r--   0        0        0     3961 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/graphql/client.py
+-rw-r--r--   0        0        0     8894 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/graphql/graphql_types.py
+-rw-r--r--   0        0        0    19382 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/graphql/schema_converter.py
+-rw-r--r--   0        0        0     3742 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/import_workflows.py
+-rw-r--r--   0        0        0      115 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/logging/__init__.py
+-rw-r--r--   0        0        0      739 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/logging/logging-config.json
+-rw-r--r--   0        0        0     3515 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/logging/logging_common.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/telemetry/__init__.py
+-rw-r--r--   0        0        0     5247 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/telemetry/common.py
+-rw-r--r--   0        0        0     1993 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/telemetry/enums.py
+-rw-r--r--   0        0        0     3574 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/telemetry/metrics.py
+-rw-r--r--   0        0        0      187 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/type_aliases.py
+-rw-r--r--   0        0        0     1365 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/util.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/worker/__init__.py
+-rw-r--r--   0        0        0      957 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/worker/service.py
+-rw-r--r--   0        0        0     2975 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/worker/task.py
+-rw-r--r--   0        0        0     3887 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/worker/task_def.py
+-rw-r--r--   0        0        0     1146 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/worker/task_result.py
+-rw-r--r--   0        0        0     7726 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/worker/worker.py
+-rw-r--r--   0        0        0    13289 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/workflow/WORKFLOW_GENERATOR.md
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/workflow/__init__.py
+-rw-r--r--   0        0        0     2773 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/workflow/service.py
+-rw-r--r--   0        0        0    18191 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/workflow/task.py
+-rw-r--r--   0        0        0     5609 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/common/workflow/workflow.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/services/inventory/__init__.py
+-rw-r--r--   0        0        0      784 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/services/inventory/operations.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/services/schellar/__init__.py
+-rw-r--r--   0        0        0     5316 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/services/schellar/model.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/services/uniconfig/__init__.py
+-rw-r--r--   0        0        0     3066 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/services/uniconfig/cli_network_topology.py
+-rw-r--r--   0        0        0     2365 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/services/uniconfig/connection_manager.py
+-rw-r--r--   0        0        0     4563 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/services/uniconfig/snapshot_manager.py
+-rw-r--r--   0        0        0     7121 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/services/uniconfig/uniconfig_manager.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/workers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/workers/inventory/__init__.py
+-rw-r--r--   0        0        0     1441 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/workers/inventory/operations.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.479514 frinx_python_sdk-0.1.1/frinx/workers/schellar/__init__.py
+-rw-r--r--   0        0        0    11984 2023-07-14 15:17:47.483514 frinx_python_sdk-0.1.1/frinx/workers/schellar/schellar_worker.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.483514 frinx_python_sdk-0.1.1/frinx/workers/test/__init__.py
+-rw-r--r--   0        0        0     5974 2023-07-14 15:17:47.483514 frinx_python_sdk-0.1.1/frinx/workers/test/test_worker.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:17:47.483514 frinx_python_sdk-0.1.1/frinx/workers/uniconfig/__init__.py
+-rw-r--r--   0        0        0     2901 2023-07-14 15:17:47.483514 frinx_python_sdk-0.1.1/frinx/workers/uniconfig/cli_network_topology.py
+-rw-r--r--   0        0        0     2532 2023-07-14 15:17:47.483514 frinx_python_sdk-0.1.1/frinx/workers/uniconfig/connection_manager.py
+-rw-r--r--   0        0        0     3936 2023-07-14 15:17:47.483514 frinx_python_sdk-0.1.1/frinx/workers/uniconfig/snapshot_manager.py
+-rw-r--r--   0        0        0     5954 2023-07-14 15:17:47.483514 frinx_python_sdk-0.1.1/frinx/workers/uniconfig/uniconfig_manager.py
+-rw-r--r--   0        0        0    15559 2023-07-14 15:17:47.483514 frinx_python_sdk-0.1.1/frinx/workflows/schellar/schellar_workflows.py
+-rw-r--r--   0        0        0     5422 2023-07-14 15:17:47.483514 frinx_python_sdk-0.1.1/frinx/workflows/test/test.py
+-rw-r--r--   0        0        0     2667 2023-07-14 15:18:02.339693 frinx_python_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2009 1970-01-01 00:00:00.000000 frinx_python_sdk-0.1.1/PKG-INFO
```

### Comparing `frinx_python_sdk-0.1.0/frinx/client/conductor.py` & `frinx_python_sdk-0.1.1/frinx/client/conductor.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-0.1.0/frinx/client/frinx_conductor_wrapper.py` & `frinx_python_sdk-0.1.1/frinx/client/frinx_conductor_wrapper.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-0.1.0/frinx/common/conductor_enums.py` & `frinx_python_sdk-0.1.1/frinx/common/conductor_enums.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class WorkflowStatus(str, Enum):
     COMPLETED = 'COMPLETED'
     FAILED = 'FAILED'
     PAUSED = 'PAUSED'
     RUNNING = 'RUNNING'
     TERMINATED = 'TERMINATED'
-    TIMEOUT_OUT = 'TIMED_OUT'
+    TIMED_OUT = 'TIMED_OUT'
 
 
 class TimeoutPolicy(str, Enum):
     TIME_OUT_WORKFLOW = 'TIME_OUT_WF'
     ALERT_ONLY = 'ALERT_ONLY'
```

### Comparing `frinx_python_sdk-0.1.0/frinx/common/frinx_rest.py` & `frinx_python_sdk-0.1.1/frinx/common/frinx_rest.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,25 +8,44 @@
 
 # SET SERVICES URL VARIABLES
 UNICONFIG_URL_BASE = os.getenv('UNICONFIG_URL_BASE', 'http://uniconfig:8181/rests')
 CONDUCTOR_URL_BASE = os.getenv('CONDUCTOR_URL_BASE', 'http://workflow-proxy:8088/proxy/api')
 INVENTORY_URL_BASE = os.getenv('INVENTORY_URL_BASE', 'http://inventory:8000/graphql')
 INFLUXDB_URL_BASE = os.getenv('INFLUXDB_URL_BASE', 'http://influxdb:8086')
 RESOURCE_MANAGER_URL_BASE = os.getenv('RESOURCE_MANAGER_URL_BASE', 'http://resource-manager:8884/query')
+SCHELLAR_URL_BASE = os.getenv('SCHELLAR_URL_BASE', 'http://schellar:3000/query')
 
 # URL HEADERS
 UNICONFIG_HEADERS = MappingProxyType({'Content-Type': 'application/json'})
 CONDUCTOR_HEADERS = MappingProxyType(
     {
         'Content-Type': 'application/json',
         'x-tenant-id': X_TENANT_ID,
         'from': X_FROM,
         'x-auth-user-groups': X_AUTH_USER_GROUP
     }
 )
+
+INVENTORY_HEADERS = MappingProxyType(
+    {
+        'Accept-Encoding': 'gzip, deflate, br',
+        'Content-Type': 'application/json',
+        'Accept': 'application/json',
+        'Connection': 'keep-alive',
+        'DNT': '1',
+        'Keep-Alive': 'timeout=5',
+        'x-tenant-id': X_TENANT_ID,
+    }
+)
+
+SCHELLAR_HEADERS = MappingProxyType({
+    'Content-Type': 'application/json',
+    'Accept': 'application/json',
+})
+
 ADDITIONAL_UNICONFIG_REQUEST_PARAMS = MappingProxyType(
     {
         'verify': False,
         'headers': UNICONFIG_HEADERS
     }
 )
```

### Comparing `frinx_python_sdk-0.1.0/frinx/common/import_workflows.py` & `frinx_python_sdk-0.1.1/frinx/common/import_workflows.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-0.1.0/frinx/common/logging/logging-config.json` & `frinx_python_sdk-0.1.1/frinx/common/logging/logging-config.json`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-0.1.0/frinx/common/logging/logging_common.py` & `frinx_python_sdk-0.1.1/frinx/common/logging/logging_common.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-0.1.0/frinx/common/telemetry/common.py` & `frinx_python_sdk-0.1.1/frinx/common/telemetry/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,19 +22,19 @@
     metrics.increment_counter(
         name=MetricName.TASK_EXECUTION_QUEUE_FULL,
         documentation=MetricDocumentation.TASK_EXECUTION_QUEUE_FULL,
         labels={MetricLabel.TASK_TYPE: task_type},
     )
 
 
-def increment_uncaught_exception(metrics: Metrics) -> None:
+def increment_uncaught_exception(metrics: Metrics, task_type: str) -> None:
     metrics.increment_counter(
         name=MetricName.THREAD_UNCAUGHT_EXCEPTION,
         documentation=MetricDocumentation.THREAD_UNCAUGHT_EXCEPTION,
-        labels={},
+        labels={MetricLabel.TASK_TYPE: task_type},
     )
 
 
 def increment_task_poll_error(metrics: Metrics, task_type: str, exception: Exception) -> None:
     metrics.increment_counter(
         name=MetricName.TASK_POLL_ERROR,
         documentation=MetricDocumentation.TASK_POLL_ERROR,
```

### Comparing `frinx_python_sdk-0.1.0/frinx/common/telemetry/enums.py` & `frinx_python_sdk-0.1.1/frinx/common/telemetry/enums.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-0.1.0/frinx/common/telemetry/metrics.py` & `frinx_python_sdk-0.1.1/frinx/common/telemetry/metrics.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-0.1.0/frinx/common/util.py` & `frinx_python_sdk-0.1.1/frinx/common/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 from typing import Any
 
+from frinx.common.type_aliases import DictAny
+
 
 def jsonify_description(
     description: str, labels: list[str] | None = None, rbac: list[str] | None = None
 ) -> str:
     """Returns description in format of stringified JSON.
     >>> jsonify_description("Hello world")
     '{"description": "Hello world"}'
@@ -30,7 +32,11 @@
     words = string.split('_')
     result = words[0].lower() + ''.join(n.capitalize() for n in words[1:])
     return result
 
 
 def normalize_base_url(url: str) -> str:
     return url.removesuffix('/')
+
+
+def remove_empty_elements_from_dict(any_dict: DictAny) -> DictAny:
+    return dict((k, v) for k, v in any_dict.items() if v)
```

### Comparing `frinx_python_sdk-0.1.0/frinx/common/worker/service.py` & `frinx_python_sdk-0.1.1/frinx/common/worker/service.py`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-0.1.0/frinx/common/worker/task.py` & `frinx_python_sdk-0.1.1/frinx/common/worker/task.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from __future__ import annotations
+
 from typing import Any
+from typing import Optional
 from typing import TypeAlias
 
 from pydantic import BaseModel
 from pydantic import Extra
 from pydantic import Field
 
 from frinx.common.type_aliases import DictAny
@@ -13,52 +16,52 @@
 
 
 class Task(BaseModel):
     input_data: DictAny = Field(default={})
     workflow_task: Any = Field(default=None)
     task_definition: Any = Field(default=None)
 
-    task_type: str = Field(default=None)
-    status: str = Field(default=None)
-    reference_task_name: str = Field(default=None)
-    retry_count: int = Field(default=None)
-    seq: int = Field(default=None)
-    correlation_id: str = Field(default=None)
-    poll_count: int = Field(default=None)
-    task_def_name: str = Field(default=None)
-    scheduled_time: int = Field(default=None)
-    start_time: int = Field(default=None)
-    end_time: int = Field(default=None)
-    update_time: int = Field(default=None)
-    start_delay_in_seconds: int = Field(default=None)
-    retried_task_id: str = Field(default=None)
-    retried: bool = Field(default=None)
-    executed: bool = Field(default=None)
-    callback_from_worker: bool = Field(default=None)
-    response_timeout_seconds: int = Field(default=None)
-    workflow_instance_id: str = Field(default=None)
-    workflow_type: str = Field(default=None)
-    task_id: str = Field(default=None)
-    reason_for_incompletion: str = Field(default=None)
-    callback_after_seconds: int = Field(default=None)
-    worker_id: str = Field(default=None)
-    output_data: dict[str, object] = Field(default=None)
-    domain: str = Field(default=None)
-    rate_limit_per_frequency: int = Field(default=None)
-    rate_limit_frequency_in_seconds: int = Field(default=None)
-    external_input_payload_storage_path: str = Field(default=None)
-    external_output_payload_storage_path: str = Field(default=None)
-    workflow_priority: int = Field(default=None)
-    execution_name_space: str = Field(default=None)
-    isolation_group_id: str = Field(default=None)
-    iteration: int = Field(default=None)
-    sub_workflow_id: str = Field(default=None)
-    subworkflow_changed: bool = Field(default=None)
-    loop_over_task: bool = Field(default=None)
-    queue_wait_time: int = Field(default=None)
+    task_type: Optional[str] = Field(default=None)
+    status: Optional[str] = Field(default=None)
+    reference_task_name: Optional[str] = Field(default=None)
+    retry_count: Optional[int] = Field(default=None)
+    seq: Optional[int] = Field(default=None)
+    correlation_id: Optional[str] = Field(default=None)
+    poll_count: Optional[int] = Field(default=None)
+    task_def_name: Optional[str] = Field(default=None)
+    scheduled_time: Optional[int] = Field(default=None)
+    start_time: Optional[int] = Field(default=None)
+    end_time: Optional[int] = Field(default=None)
+    update_time: Optional[int] = Field(default=None)
+    start_delay_in_seconds: Optional[int] = Field(default=None)
+    retried_task_id: Optional[str] = Field(default=None)
+    retried: Optional[bool] = Field(default=None)
+    executed: Optional[bool] = Field(default=None)
+    callback_from_worker: Optional[bool] = Field(default=None)
+    response_timeout_seconds: Optional[int] = Field(default=None)
+    workflow_instance_id: Optional[str] = Field(default=None)
+    workflow_type: Optional[str] = Field(default=None)
+    task_id: Optional[str] = Field(default=None)
+    reason_for_incompletion: Optional[str] = Field(default=None)
+    callback_after_seconds: Optional[int] = Field(default=None)
+    worker_id: Optional[str] = Field(default=None)
+    output_data: Optional[dict[str, Any]] = Field(default=None)
+    domain: Optional[str] = Field(default=None)
+    rate_limit_per_frequency: Optional[int] = Field(default=None)
+    rate_limit_frequency_in_seconds: Optional[int] = Field(default=None)
+    external_input_payload_storage_path: Optional[str] = Field(default=None)
+    external_output_payload_storage_path: Optional[str] = Field(default=None)
+    workflow_priority: Optional[int] = Field(default=None)
+    execution_name_space: Optional[str] = Field(default=None)
+    isolation_group_id: Optional[str] = Field(default=None)
+    iteration: Optional[int] = Field(default=None)
+    sub_workflow_id: Optional[str] = Field(default=None)
+    subworkflow_changed: Optional[bool] = Field(default=None)
+    loop_over_task: Optional[bool] = Field(default=None)
+    queue_wait_time: Optional[int] = Field(default=None)
 
     class Config:
         allow_mutation = True
         extra = Extra.forbid
         validate_assignment = True
         alias_generator = snake_to_camel_case
         allow_population_by_field_name = True
```

### Comparing `frinx_python_sdk-0.1.0/frinx/common/worker/task_result.py` & `frinx_python_sdk-0.1.1/frinx/common/worker/task_result.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,45 @@
-from typing import Any
+from typing import Generic
+from typing import TypeVar
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from frinx.common.conductor_enums import TaskResultStatus
 from frinx.common.util import snake_to_camel_case
+from frinx.common.worker.task_def import TaskOutput
 
+T = TypeVar('T')
 
-class TaskResult(BaseModel):
+
+class Registry(Generic[T]):
+    def __init__(self) -> None:
+        self._store: dict[str, T] = {}
+
+    def set_item(self, k: str, v: T) -> None:
+        self._store[k] = v
+
+    def get_item(self, k: str) -> T:
+        return self._store[k]
+
+
+TO = TypeVar('TO', bound=TaskOutput | None)
+
+
+class TaskResult(BaseModel, Generic[TO]):
     status: TaskResultStatus
-    output: dict[str, Any] = Field(default={})
+    output: TO | None = None
     logs: list[str] | str = Field(default=[])
 
     class Config:
         validate_assignment = True
         alias_generator = snake_to_camel_case
         allow_population_by_field_name = True
 
     @validator('logs', always=True)
     def validate_logs(cls, logs: str | list[str]) -> list[str]: # noqa: 805
         match logs:
             case list():
                 return logs
             case str():
                 return [logs]
-
-    def add_output_data(self, key: str, value: Any) -> None:
-        if self.output is None:
-            self.output = {}
-        self.output[key] = value
-
-    def add_output_data_dict(self, data: dict[str, Any]) -> None:
-        self.output = data
```

### Comparing `frinx_python_sdk-0.1.0/frinx/common/worker/worker.py` & `frinx_python_sdk-0.1.1/frinx/common/worker/worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import logging
 import time
-import typing
 from abc import ABC
 from abc import abstractmethod
+from json import JSONDecodeError
+from json import loads as json_loads
 from typing import Any
 from typing import TypeAlias
 
 from pydantic import ValidationError
 from pydantic.dataclasses import dataclass
 
 from frinx.client.frinx_conductor_wrapper import FrinxConductorWrapper
 from frinx.common.conductor_enums import TaskResultStatus
 from frinx.common.telemetry.common import increment_task_execution_error
 from frinx.common.telemetry.common import increment_task_poll
 from frinx.common.telemetry.common import increment_uncaught_exception
 from frinx.common.telemetry.common import record_task_execute_time
 from frinx.common.telemetry.metrics import Metrics
+from frinx.common.type_aliases import DictAny
 from frinx.common.util import jsonify_description
+from frinx.common.util import remove_empty_elements_from_dict
 from frinx.common.util import snake_to_camel_case
 from frinx.common.worker.task_def import BaseTaskdef
 from frinx.common.worker.task_def import DefaultTaskDefinition
 from frinx.common.worker.task_def import TaskDefinition
+from frinx.common.worker.task_def import TaskExecutionProperties
 from frinx.common.worker.task_def import TaskInput
 from frinx.common.worker.task_def import TaskOutput
 from frinx.common.worker.task_result import TaskResult
 
 logger = logging.getLogger(__name__)
 metrics = Metrics()
 
@@ -39,14 +43,17 @@
 
 
 @dataclass(config=Config)
 class WorkerImpl(ABC):
     task_def: TaskDefinition
     task_def_template: type[BaseTaskdef] | type[DefaultTaskDefinition] | None
 
+    class ExecutionProperties(TaskExecutionProperties):
+        ...
+
     class WorkerDefinition(TaskDefinition):
         ...
 
     class WorkerInput(TaskInput):
         ...
 
     class WorkerOutput(TaskOutput):
@@ -86,69 +93,92 @@
             task_def_template = DefaultTaskDefinition.__fields__.items()  # type: ignore
         else:
             task_def_template = task_def_template.__fields__.items()  # type: ignore
 
         # Transform dict to TaskDefinition object use default values in necessary
         task_def = TaskDefinition(**params)
 
-        for key, value in task_def_template: # type: ignore
+        for key, value in task_def_template:  # type: ignore
             if value.default is not None and task_def.__getattribute__(key) is None:
                 task_def.__setattr__(key, value.default)
 
         return task_def
 
     def register(self, conductor_client: FrinxConductorWrapper) -> None:
         conductor_client.register(
             task_type=self.task_def.name,
             task_definition=self.task_def.dict(by_alias=True, exclude_none=True),
             exec_function=self._execute_wrapper,
         )
 
     @abstractmethod
-    def execute(self, worker_input: typing.Any) -> TaskResult:
+    def execute(self, worker_input: Any) -> TaskResult[Any]:
         # worker_input parameter has to be of type any, otherwise all other subclasses of WorkerImpl would
         # violate Liskov substitution principle.
         # https://mypy.readthedocs.io/en/stable/common_issues.html#incompatible-overrides
         pass
 
     @classmethod
     def _execute_wrapper(cls, task: RawTaskIO) -> Any:
-
         task_type = str(task.get('taskType'))
         increment_task_poll(metrics, task_type)
         try:
             logger.debug('Executing task %s:', task)
             task_result: RawTaskIO = cls._execute_func(task)
             logger.debug('Task result %s:', task_result)
             return task_result
         except Exception as error:
             increment_task_execution_error(metrics, task_type, error)
-            increment_uncaught_exception(metrics)
+            increment_uncaught_exception(metrics, task_type)
             logger.error('Validation error occurred: %s', error)
             return TaskResult(status=TaskResultStatus.FAILED, logs=[TaskExecLog(str(error))]).dict()
 
     @classmethod
     def _execute_func(cls, task: RawTaskIO) -> RawTaskIO:
+
+        input_data: DictAny = task['inputData']
+        execution_properties = cls.ExecutionProperties()
+
+        if execution_properties.exclude_empty_inputs:
+            logger.debug('Worker input data before removing empty elements: %s:', input_data)
+            input_data = remove_empty_elements_from_dict(task['inputData'])
+            logger.debug('Worker input data after removing empty elements: %s:', input_data)
+
+        if execution_properties.transform_string_to_json_valid:
+            logger.debug('Worker input data before json serialization: %s:', input_data)
+            input_data = cls._transform_input_data_to_json(input_data)
+            logger.debug('Worker input data after json serialization: %s:', input_data)
+
         try:
-            cls.WorkerInput.parse_obj(task['inputData'])
+            worker_input = cls.WorkerInput.parse_obj(input_data)
         except ValidationError as error:
             logger.error('Validation error occurred: %s', error)
             raise error
 
-        worker_input = cls.WorkerInput.parse_obj(task['inputData'])
         if not metrics.settings.metrics_enabled:
             return cls.execute(cls, worker_input).dict()  # type: ignore[arg-type]
 
         start_time = time.time()
         task_result: RawTaskIO = cls.execute(cls, worker_input).dict()  # type: ignore[arg-type]
         finish_time = time.time()
         record_task_execute_time(metrics, str(task.get('taskType')), finish_time - start_time)
         return task_result
 
     @classmethod
+    def _transform_input_data_to_json(cls, input_data: DictAny) -> DictAny:
+        for k, v in cls.WorkerInput.__fields__.items():
+            if v.outer_type_ == list[str] or v.outer_type_ == DictAny:
+                if type(input_data.get(k)) == str:
+                    try:
+                        input_data[k] = json_loads(str(input_data.get(k)))
+                    except JSONDecodeError as e:
+                        raise Exception(f'Worker input {k} is invalid JSON, {e}')
+        return input_data
+
+    @classmethod
     def validate(cls) -> None:
         if not issubclass(cls.WorkerInput, TaskInput):
             error_msg = (
                 "Expecting task input model to be a subclass of "
                 f"'{TaskInput.__qualname__}', not '{cls.WorkerInput.__qualname__}'"
             )
             logger.error(error_msg)
```

### Comparing `frinx_python_sdk-0.1.0/frinx/common/workflow/WORKFLOW_GENERATOR.md` & `frinx_python_sdk-0.1.1/frinx/common/workflow/WORKFLOW_GENERATOR.md`

 * *Files identical despite different names*

### Comparing `frinx_python_sdk-0.1.0/frinx/common/workflow/service.py` & `frinx_python_sdk-0.1.1/frinx/common/workflow/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class ServiceWorkflowsImpl:
     service_workflows: list[type[WorkflowImpl]] = []
 
-    def __init__(self, workflows: list[type[WorkflowImpl]] | None, exclude: bool = False) -> None:
+    def __init__(self, workflows: list[type[WorkflowImpl]] | None = None, exclude: bool = False) -> None:
         """
 
         Args:
             workflows: list of Workflows [workflow subclasses]
             exclude: If true, exclude workflows from all workflows. Else install only selected.
         """
         if workflows is None:
```

### Comparing `frinx_python_sdk-0.1.0/frinx/common/workflow/task.py` & `frinx_python_sdk-0.1.1/frinx/common/workflow/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
 from typing import Any
+from typing import Optional
 from typing import TypeAlias
 
 from pydantic import BaseModel
 from pydantic import Extra
 from pydantic import Field
 from pydantic import StrictBool
 from pydantic import root_validator
@@ -57,54 +58,54 @@
     start_delay: int = Field(default=0)
     optional: StrictBool = Field(default=False)
     async_complete: StrictBool = Field(default=False)
     default_case: list[WorkflowTask] | list[Any] = Field(default=[])
     input_parameters: Any | dict[str, Any] = Field(default={})
 
     # OPTIONAL
-    description: str = Field(default=None)
-    dynamic_task_name_param: str = Field(default=None)
-    case_value_param: str = Field(default=None)
-    case_expression: str = Field(default=None)
-    script_expression: str = Field(default=None)
-    decision_cases: dict[str, list[WorkflowTask]] | dict[str, list[Any]] = Field(default=None)
-    dynamic_fork_join_tasks_param: str = Field(default=None)
-    dynamic_fork_tasks_param: str = Field(default=None)
-    dynamic_fork_tasks_input_param_name: str = Field(default=None)
-    fork_tasks: list[list[WorkflowTask]] | list[list[Any]] = Field(default=None)
-    sub_workflow_param: dict[str, Any] | Any = Field(default=None)
-    join_on: list[str] = Field(default=None)
-    sink: str = Field(default=None)
-    task_definition: TaskDef = Field(default=None)
-    rate_limited: StrictBool = Field(default=None)
-    default_exclusive_join_task: list[str] = Field(default=None)
-    loop_condition: str = Field(default=None)
-    loop_over: list[Any] = Field(default=None)
-    retry_count: int = Field(default=None)
-    evaluator_type: str = Field(default=None)
-    expression: str = Field(default=None)
-    workflow_task_type: str = Field(default=None)
+    description: Optional[str] = Field(default=None)
+    dynamic_task_name_param: Optional[str] = Field(default=None)
+    case_value_param: Optional[str] = Field(default=None)
+    case_expression: Optional[str] = Field(default=None)
+    script_expression: Optional[str] = Field(default=None)
+    decision_cases: Optional[dict[str, list[WorkflowTask]] | dict[str, list[Any]]] = Field(default=None)
+    dynamic_fork_join_tasks_param: Optional[str] = Field(default=None)
+    dynamic_fork_tasks_param: Optional[str] = Field(default=None)
+    dynamic_fork_tasks_input_param_name: Optional[str] = Field(default=None)
+    fork_tasks: Optional[list[list[Any]]] = Field(default=None)
+    sub_workflow_param: Optional[Any] = Field(default=None)
+    join_on: Optional[list[str]] = Field(default=None)
+    sink: Optional[str] = Field(default=None)
+    task_definition: Optional[TaskDef] = Field(default=None)
+    rate_limited: Optional[StrictBool] = Field(default=None)
+    default_exclusive_join_task: Optional[list[str]] = Field(default=None)
+    loop_condition: Optional[str] = Field(default=None)
+    loop_over: Optional[list[Any]] = Field(default=None)
+    retry_count: Optional[int] = Field(default=None)
+    evaluator_type: Optional[str] = Field(default=None)
+    expression: Optional[str] = Field(default=None)
+    workflow_task_type: Optional[str] = Field(default=None)
 
     class Config:
         alias_generator = snake_to_camel_case
         allow_population_by_field_name = True
         validate_assignment = True
         validate_all = True
 
     def output_ref(self, path: str | None = None) -> str:
         if not path or path is None:
             return f'${{{self.task_reference_name}.output}}'
         return f'${{{self.task_reference_name}.output.{path}}}'
 
 
 class DoWhileTask(WorkflowTaskImpl):
-    type = TaskType.DO_WHILE
+    type: TaskType = TaskType.DO_WHILE
     loop_condition: str
     loop_over: list[WorkflowTaskImpl]
-    evaluator_type = DoWhileEvaluatorType.JAVASCRIPT
+    evaluator_type: DoWhileEvaluatorType = DoWhileEvaluatorType.JAVASCRIPT
 
 
 class DynamicForkTaskInputParameters(BaseModel):
     dynamic_tasks: str | object
     dynamic_tasks_input: str | object
 
     class Config:
@@ -163,23 +164,23 @@
         validate_assignment = True
         allow_mutation = True
         validate_all = True
 
 
 class DynamicForkTask(WorkflowTaskImpl):
     # TODO why not render in UI?
-    type = TaskType.FORK_JOIN_DYNAMIC
+    type: TaskType = TaskType.FORK_JOIN_DYNAMIC
     dynamic_fork_tasks_param: str = Field(default='dynamicTasks')
     dynamic_fork_tasks_input_param_name: str = Field(default='dynamicTasksInput')
     input_parameters: DynamicForkArraysTaskInputParameters | DynamicForkTaskInputParameters \
                       | DynamicForkArraysTaskFromDefInputParameters | DynamicForkTaskFromDefInputParameters
 
 
 class ForkTask(WorkflowTaskImpl):
-    type = TaskType.FORK_JOIN
+    type: TaskType = TaskType.FORK_JOIN
     fork_tasks: list[list[WorkflowTaskImpl]]
 
 
 class HttpMethod(str, Enum):
     GET = ('GET',)
     PUT = ('PUT',)
     POST = ('POST',)
@@ -188,15 +189,15 @@
     OPTIONS = 'OPTIONS'
 
 
 # TODO HTTP TASK?
 
 
 class HumanTask(WorkflowTaskImpl):
-    type = TaskType.HUMAN
+    type: TaskType = TaskType.HUMAN
 
 
 class InlineTaskInputParameters(BaseModel):
     evaluator_type: str = Field(default='javascript', alias='evaluatorType')
     expression: str
 
     class Config:
@@ -215,15 +216,15 @@
     def expression_in_function(cls, expression: str) -> str:  # noqa: N805
         if not expression.startswith('function'):
             expression = f'function e() {{ {expression} }} e();'
         return expression
 
 
 class InlineTask(WorkflowTaskImpl):
-    type = TaskType.INLINE
+    type: TaskType = TaskType.INLINE
     input_parameters: InlineTaskInputParameters
 
 
 class LambdaTaskInputParameters(BaseModel):
     script_expression: str = Field(alias='scriptExpression')
 
     class Config:
@@ -236,33 +237,33 @@
         data['script_expression'] = script_expression
         if self.__custom_root_type__ and data.keys() != {ROOT_KEY}:
             data = {ROOT_KEY: data}
         super().__init__(**data)
 
 
 class LambdaTask(WorkflowTaskImpl):
-    type = TaskType.LAMBDA
+    type: TaskType = TaskType.LAMBDA
     input_parameters: LambdaTaskInputParameters
 
 
 class WaitDurationTaskInputParameters(BaseModel):
     duration: str
 
 
 class WaitDurationTask(WorkflowTaskImpl):
-    type = TaskType.WAIT
+    type: TaskType = TaskType.WAIT
     input_parameters: WaitDurationTaskInputParameters
 
 
 class WaitUntilTaskInputParameters(BaseModel):
     until: str
 
 
 class WaitUntilTask(WorkflowTaskImpl):
-    type = TaskType.WAIT
+    type: TaskType = TaskType.WAIT
     input_parameters: WaitUntilTaskInputParameters
 
 
 class TerminateTaskInputParameters(BaseModel):
     termination_status: WorkflowStatus
     termination_reason: str | None
     workflow_output: dict[str, Any] | str | None
@@ -273,21 +274,21 @@
         allow_population_by_field_name = True
         validate_assignment = True
         allow_mutation = True
         validate_all = True
 
 
 class TerminateTask(WorkflowTaskImpl):
-    type = TaskType.TERMINATE
+    type: TaskType = TaskType.TERMINATE
     input_parameters: TerminateTaskInputParameters
 
 
 class StartWorkflowTaskPlainInputParameters(BaseModel):
     name: str
-    version: int = Field(default=None)
+    version: Optional[int] = Field(default=None)
     input: dict[str, object] | None = {}
     correlation_id: str | None = Field(alias='correlationId')
 
 
 class StartWorkflowTaskFromDefInputParameters(BaseModel):
     workflow: object
     input: dict[str, object] | None = {}
@@ -322,15 +323,15 @@
         allow_population_by_field_name = True
         validate_assignment = True
         allow_mutation = True
         validate_all = True
 
 
 class StartWorkflowTask(WorkflowTaskImpl):
-    type = TaskType.START_WORKFLOW
+    type: TaskType = TaskType.START_WORKFLOW
     input_parameters: StartWorkflowTaskInputParameters
 
 
 class SwitchTaskInputParameters(BaseModel):
     input_value: str
 
     class Config:
@@ -351,15 +352,15 @@
         allow_population_by_field_name = True
         validate_assignment = True
         allow_mutation = True
         validate_all = True
 
 
 class SwitchTask(WorkflowTaskImpl):
-    type = TaskType.SWITCH
+    type: TaskType = TaskType.SWITCH
     default_case: list[WorkflowTaskImpl] | None = Field(default=[])  # type: ignore[assignment]
     decision_cases: dict[str, list[WorkflowTaskImpl]]
     evaluator_type: SwitchEvaluatorType = Field(default=SwitchEvaluatorType.JAVASCRIPT)
     expression: str
     input_parameters: SwitchTaskInputParameters | SwitchTaskValueParamInputParameters
 
 
@@ -370,30 +371,30 @@
         super().__init__(**data)
 
     class Config:
         extra = Extra.allow
 
 
 class DecisionTask(WorkflowTaskImpl):
-    type = TaskType.DECISION
+    type: TaskType = TaskType.DECISION
     default_case: list[WorkflowTaskImpl] = []
     decision_cases: dict[str, list[WorkflowTaskImpl]]
     case_expression: str
     input_parameters: DecisionTaskInputParameters
 
 
 class DecisionCaseValueTaskInputParameters(BaseModel):
     case_value_param: str
 
 
 class DecisionCaseValueTask(WorkflowTaskImpl):
-    type = TaskType.DECISION
+    type: TaskType = TaskType.DECISION
     default_case: list[WorkflowTaskImpl] = []
     decision_cases: dict[str, list[WorkflowTaskImpl]]
-    case_value_param = 'case_value_param'
+    case_value_param: str = 'case_value_param'
     input_parameters: DecisionCaseValueTaskInputParameters
 
 
 class SubWorkflowInputParameters(BaseModel):
     def __init__(self, **data: Any) -> None:
         if self.__custom_root_type__ and data.keys() != {ROOT_KEY}:
             data = {ROOT_KEY: data}
@@ -402,32 +403,32 @@
     class Config:
         extra = Extra.allow
 
 
 class SubWorkflowParam(BaseModel):
     name: str
     version: int
-    task_to_domain: TaskToDomain = Field(default=None)
-    workflow_definition: WorkflowDef = Field(default=None)
+    task_to_domain: Optional[TaskToDomain] = Field(default=None)
+    workflow_definition: Optional[WorkflowDef] = Field(default=None)
 
 
 class SubWorkflowFromDefParam(BaseModel):
     name: type[Any]
-    task_to_domain: TaskToDomain = Field(default=None)
-    workflow_definition: WorkflowDef = Field(default=None)
+    task_to_domain: Optional[TaskToDomain] = Field(default=None)
+    workflow_definition: Optional[WorkflowDef] = Field(default=None)
 
     class Config:
         alias_generator = snake_to_camel_case
         allow_population_by_field_name = True
         validate_assignment = True
         validate_all = True
 
 
 class SubWorkflowTask(WorkflowTaskImpl):
-    type = TaskType.SUB_WORKFLOW
+    type: TaskType = TaskType.SUB_WORKFLOW
     sub_workflow_param: SubWorkflowParam | SubWorkflowFromDefParam
     input_parameters: SubWorkflowInputParameters
 
     @root_validator(pre=True)
     def check_input_values(cls, values: dict[str, Any]) -> dict[str, Any]:  # noqa: N805
         sub_wf_def = values['sub_workflow_param']
         worker_inputs = values['input_parameters'].dict()
@@ -462,15 +463,15 @@
 
     class Config:
         extra = Extra.allow
 
 
 class SimpleTask(WorkflowTaskImpl):
     name: object | str  # type: ignore[assignment]
-    type = TaskType.SIMPLE
+    type: TaskType = TaskType.SIMPLE
     input_parameters: SimpleTaskInputParameters
 
     @root_validator(pre=True)
     def check_input_values(cls, values: dict[str, Any]) -> dict[str, Any]:  # noqa: N805
         task_def = values['name']
         worker_inputs = values['input_parameters'].dict()
 
@@ -496,37 +497,37 @@
         super().__init__(**data)
 
     class Config:
         extra = Extra.allow
 
 
 class SetVariableTask(WorkflowTaskImpl):
-    type = TaskType.SET_VARIABLE
+    type: TaskType = TaskType.SET_VARIABLE
     input_parameters: SetVariableTaskInputParameters
 
 
 class KafkaPublishTaskInputParameters(BaseModel):
     boot_strap_servers: str
     key: str
     key_serializer: str
     value: str
     request_timeout_ms: str
     max_block_ms: str
-    headers: dict[str, Any] = Field(default=None)
+    headers: Optional[dict[str, Any]] = Field(default=None)
     topic: str
 
     class Config:
         alias_generator = snake_to_camel_case
         allow_population_by_field_name = True
         validate_assignment = True
         allow_mutation = True
 
 
 class KafkaPublishTask(WorkflowTaskImpl):
-    type = TaskType.KAFKA_PUBLISH
+    type: TaskType = TaskType.KAFKA_PUBLISH
     input_parameters: KafkaPublishTaskInputParameters
 
 
 class JsonJqTaskInputParameters(BaseModel):
     query_expression: str = Field(alias='queryExpression')
 
     class Config:
@@ -539,25 +540,25 @@
         data['query_expression'] = query_expression
         if self.__custom_root_type__ and data.keys() != {ROOT_KEY}:
             data = {ROOT_KEY: data}
         super().__init__(**data)
 
 
 class JsonJqTask(WorkflowTaskImpl):
-    type = TaskType.JSON_JQ_TRANSFORM
+    type: TaskType = TaskType.JSON_JQ_TRANSFORM
     input_parameters: JsonJqTaskInputParameters
 
 
 class JoinTask(WorkflowTaskImpl):
-    type = TaskType.JOIN
+    type: TaskType = TaskType.JOIN
     join_on: list[str] = []
 
 
 class ExclusiveJoinTask(WorkflowTaskImpl):
-    type = TaskType.EXCLUSIVE_JOIN
+    type: TaskType = TaskType.EXCLUSIVE_JOIN
     join_on: list[str] = []
 
 
 class EventTask(WorkflowTaskImpl):
-    type = TaskType.EVENT
+    type: TaskType = TaskType.EVENT
     sink: str
     async_complete: bool
```

### Comparing `frinx_python_sdk-0.1.0/frinx/common/workflow/workflow.py` & `frinx_python_sdk-0.1.1/frinx/common/workflow/workflow.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+from __future__ import annotations
+
 import json
 from abc import ABC
 from abc import abstractmethod
 from enum import Enum
 from typing import Any
 from typing import Final
+from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Extra
 from pydantic import Field
 
 from frinx.common.conductor_enums import TimeoutPolicy
 from frinx.common.import_workflows import register_workflow
+from frinx.common.type_aliases import ListAny
 from frinx.common.util import jsonify_description
 from frinx.common.util import snake_to_camel_case
 from frinx.common.workflow.task import WorkflowTaskImpl
 
 
 class FrontendWFInputFieldType(str, Enum):
     TOGGLE = 'toggle'
@@ -30,32 +34,32 @@
 
     def __bool__(self) -> bool:
         return False
 
     def __repr__(self) -> str:
         return '<not-defined>'
 
-    def __copy__(self) -> '_UndefinedType':
+    def __copy__(self) -> _UndefinedType:
         return self
 
-    def __deepcopy__(self, _: Any) -> '_UndefinedType':
+    def __deepcopy__(self, _: Any) -> _UndefinedType:
         return self
 
 
 UNDEFINED: Final[_UndefinedType] = _UndefinedType()
 
 
 class WorkflowInputField(BaseModel):
     name: str
     frontend_default_value: Any = Field(UNDEFINED, alias='value')
     description: str = ''
-    options: list[Any] | None = None
+    options: Optional[ListAny] = None
     type: Any
     frontend_type: FrontendWFInputFieldType | None = None
-    wf_input: str = Field(default=None)
+    wf_input: Optional[str] = Field(default=None)
 
     class Config:
         min_anystr_length = 1
         use_enum_values = True
         allow_population_by_field_name = True
         extra = Extra.forbid
 
@@ -83,70 +87,76 @@
             validate_all = True
 
     name: str
     version: int
 
     # LABELS, RBAC, DESCRIPTION, INPUT VALUES
     description: str
-    labels: list[object] | None = Field(default=None)  # TODO why list[str] return error
-    rbac: list[object] | None = Field(default=None)  # TODO why list[str] return error
+    labels: list[str] | None = Field(default=None)
+    rbac: list[str] | None = Field(default=None)
 
     # PREDEFINED
     restartable: bool = Field(default=False)
     output_parameters: dict[str, object] = Field(default={})
     input_parameters: list[WorkflowInputField | str] = Field(default=[])
     tasks: list[WorkflowTaskImpl] = Field(default=[])
     timeout_policy: TimeoutPolicy = Field(default=TimeoutPolicy.TIME_OUT_WORKFLOW)
     timeout_seconds: int = Field(default=60)
 
-    owner_app: str = Field(default=None)
-    create_time: int = Field(default=None)
-    update_time: int = Field(default=None)
-    created_by: str = Field(default=None)
-    updated_by: str = Field(default=None)
-    failure_workflow: str = Field(default=None)
-    schema_version: int = Field(default=None)
-    workflow_status_listener_enabled: bool = Field(default=None)
-    owner_email: str = Field(default=None)
-    variables: dict[str, object] = Field(default=None)
-    input_template: dict[str, object] = Field(default={})
+    owner_app: Optional[str] = Field(default=None)
+    create_time: Optional[int] = Field(default=None)
+    update_time: Optional[int] = Field(default=None)
+    created_by: Optional[str] = Field(default=None)
+    updated_by: Optional[str] = Field(default=None)
+    failure_workflow: Optional[str] = Field(default=None)
+    schema_version: Optional[int] = Field(default=None)
+    workflow_status_listener_enabled: Optional[bool] = Field(default=None)
+    owner_email: Optional[str] = Field(default=None)
+    variables: Optional[dict[str, Any]] = Field(default=None)
+    input_template: dict[str, Any] = Field(default={})
 
     def __init__(self, **data: Any):
         super().__init__(**data)
         self.description_builder()
         self.workflow_builder(self.input_builder())
 
     def input_builder(self) -> WorkflowInput:
         workflow_inputs = self.WorkflowInput()
         self.input_parameters = []
         for wf_input in workflow_inputs:
             self.input_parameters.append(
                 json.dumps(
                     {
-                        wf_input[0]: {
+                        wf_input[1].name: {
                             'value': wf_input[1].frontend_default_value,
                             'description': wf_input[1].description,
                             'type': wf_input[1].type,
                             'options': wf_input[1].options,
                         }
                     }
                 )
             )
-            self.input_template[wf_input[0]] = wf_input[1].frontend_default_value
+            self.input_template[wf_input[1].name] = wf_input[1].frontend_default_value
         return workflow_inputs
 
     def description_builder(self) -> None:
-        self.description = jsonify_description(self.description, self.labels, self.rbac)   # type: ignore
+        self.description = jsonify_description(self.description, self.labels, self.rbac)
 
     @classmethod
     def register(cls, overwrite: bool = False) -> None:
         register_workflow(cls().json(by_alias=True, exclude_none=True), overwrite)
 
     @abstractmethod
-    def workflow_builder(self, workflow_inputs: WorkflowInput) -> None:
+    def workflow_builder(self, workflow_inputs: Any) -> None:
+        # TODO: workflow_inputs needs to be a reference to WorkflowInput child in it's namespace
+        # error: Argument 1 of "workflow_builder" is incompatible with supertype "WorkflowImpl";
+        # supertype defines the argument type as "WorkflowInput"
+        # NOTE: This violates the Liskov substitution principle
+        # NOTE: See https://mypy.readthedocs.io/en/stable/common_issues.html#incompatible-overrides
+        # https://discuss.python.org/t/a-way-to-typehint-a-return-type-in-parent-based-on-return-type-of-a-child/17020
         pass
 
     class Config:
         alias_generator = snake_to_camel_case
         allow_population_by_field_name = True
         validate_assignment = True
         validate_all = True
```

### Comparing `frinx_python_sdk-0.1.0/frinx/services/uniconfig/cli_network_topology.py` & `frinx_python_sdk-0.1.1/frinx/services/uniconfig/cli_network_topology.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,36 +12,32 @@
 
 def execute_and_read(
     node_id: str,
     command: str,
     transaction_id: str,
     uniconfig_server_id: str | None = None,
     wait_for_output: int = 0,
-    uniconfig_url_base: str | None = None
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Execute command and read output.
     https://docs.frinx.io/frinx-uniconfig/user-guide/network-management-protocols/uniconfig_cli/#rpc-execute-and-read
     Args:
         node_id: Target node.
         command: Command to be executed.
         transaction_id: Transaction ID generated by Uniconfig.
         uniconfig_server_id: Uniconfig server id is used by load balancer to forward request to the correct Uniconfig
          node. It is required when using multi node deployment of Uniconfig.
         wait_for_output: Execute next command after n seconds after previous one.
-        uniconfig_url_base: Override default Uniconfig url.
+        uniconfig_url_base: Uniconfig url.
 
     Returns:
         Http response.
     """
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = normalize_base_url(base_url) + CLI_EXECUTE_AND_READ_URL.format(node_id)
+    url = normalize_base_url(uniconfig_url_base) + CLI_EXECUTE_AND_READ_URL.format(node_id)
     cookies: DictAny = {'UNICONFIGTXID': transaction_id, 'uniconfig_server_id': uniconfig_server_id}
     response = requests.post(
         url,
         data=json.dumps(
             {
                 'input': {
                     'command': command,
@@ -58,35 +54,31 @@
 
 
 def execute(
     node_id: str,
     command: str,
     transaction_id: str,
     uniconfig_server_id: str | None = None,
-    uniconfig_url_base: str | None = None
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Execute command.
     https://docs.frinx.io/frinx-uniconfig/user-guide/network-management-protocols/uniconfig_cli/#rpc-execute
     Args:
         node_id: Target node.
         command: Command to be executed.
         transaction_id: Transaction ID generated by Uniconfig.
         uniconfig_server_id: Uniconfig server id is used by load balancer to forward request to the correct Uniconfig
          node. It is required when using multi node deployment of Uniconfig.
-        uniconfig_url_base: Override default Uniconfig url.
+        uniconfig_url_base: Uniconfig url.
 
     Returns:
         Http response.
     """
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = normalize_base_url(base_url) + CLI_EXECUTE_URL.format(node_id)
+    url = normalize_base_url(uniconfig_url_base) + CLI_EXECUTE_URL.format(node_id)
     cookies: DictAny = {'UNICONFIGTXID': transaction_id, 'uniconfig_server_id': uniconfig_server_id}
     response = requests.post(
         url,
         data=json.dumps(
             {
                 'input': {
                     'command': command
```

### Comparing `frinx_python_sdk-0.1.0/frinx/services/uniconfig/connection_manager.py` & `frinx_python_sdk-0.1.1/frinx/services/uniconfig/connection_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,33 +11,29 @@
 from frinx.common.util import normalize_base_url
 
 
 def install_node(
     node_id: str,
     connection_type: Literal['netconf', 'cli'],
     install_params: DictAny,
-    uniconfig_url_base: str | None = None
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Install node to Uniconfig.
     https://docs.frinx.io/frinx-uniconfig/user-guide/network-management-protocols/uniconfig-installing/
     Args:
         node_id: Unique identifier, which will be assigned to a node after installation.
         connection_type: Connection type. Accepted values are "netconf" and "cli" values.
         install_params: Installation parameters. For more info check the Uniconfig install documentation.
-        uniconfig_url_base: Override default Uniconfig url.
+        uniconfig_url_base: Uniconfig url.
 
     Returns:
         Http response.
     """
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = normalize_base_url(base_url) + INSTALL_NODE_URL
+    url = normalize_base_url(uniconfig_url_base) + INSTALL_NODE_URL
     data: DictAny = {
         'input': {
             'node-id': node_id,
             connection_type: {
                 **install_params
             }
         }
@@ -47,32 +43,28 @@
     response.raise_for_status()
     return response
 
 
 def uninstall_node(
     node_id: str,
     connection_type: Literal['netconf', 'cli'],
-    uniconfig_url_base: str | None = None
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Uninstall node from Uniconfig.
     https://docs.frinx.io/frinx-uniconfig/user-guide/network-management-protocols/uniconfig-installing/#example-request
     Args:
         node_id: Unique identifier of a node to be uninstalled.
         connection_type: Connection type. Accepted values are "netconf" and "cli" values.
-        uniconfig_url_base: Override default Uniconfig url.
+        uniconfig_url_base: Uniconfig url.
 
     Returns:
         Http response.
     """
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = normalize_base_url(base_url) + UNINSTALL_NODE_URL
+    url = normalize_base_url(uniconfig_url_base) + UNINSTALL_NODE_URL
     data = {
         'input': {
             'node-id': node_id,
             'connection-type': connection_type
         }
     }
```

### Comparing `frinx_python_sdk-0.1.0/frinx/services/uniconfig/snapshot_manager.py` & `frinx_python_sdk-0.1.1/frinx/services/uniconfig/snapshot_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,35 +12,31 @@
 
 
 def create_snapshot(
     node_ids: list[str],
     snapshot_name: str,
     transaction_id: str,
     uniconfig_server_id: str | None = None,
-    uniconfig_url_base: str | None = None
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Create Uniconfig snapshot.
     https://docs.frinx.io/frinx-uniconfig/user-guide/uniconfig-operations/snapshot-manager/rpc_create-snapshot/
     Args:
         node_ids: List of node ids to create snapshot from.
         snapshot_name: Name of Uniconfig snapshot.
         transaction_id: Transaction ID generated by Uniconfig.
         uniconfig_server_id: Uniconfig server id is used by load balancer to forward request to the correct Uniconfig
          node. It is required when using multi node deployment of Uniconfig.
-        uniconfig_url_base: Override default Uniconfig url.
+        uniconfig_url_base: Uniconfig url.
 
     Returns:
         Http response.
     """
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = normalize_base_url(base_url) + CREATE_SNAPSHOT_URL
+    url = normalize_base_url(uniconfig_url_base) + CREATE_SNAPSHOT_URL
     cookies: DictAny = {'UNICONFIGTXID': transaction_id, 'uniconfig_server_id': uniconfig_server_id}
     response = requests.post(
         url,
         data=json.dumps(
             {
                 'input': {
                     'name': snapshot_name,
@@ -57,34 +53,30 @@
     return response
 
 
 def delete_snapshot(
     snapshot_name: str,
     transaction_id: str,
     uniconfig_server_id: str | None = None,
-    uniconfig_url_base: str | None = None
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Delete Uniconfig snapshot.
     https://docs.frinx.io/frinx-uniconfig/user-guide/uniconfig-operations/snapshot-manager/rpc_delete-snapshot/
     Args:
         snapshot_name: Name of Uniconfig snapshot.
         transaction_id: Transaction ID generated by Uniconfig.
         uniconfig_server_id: Uniconfig server id is used by load balancer to forward request to the correct Uniconfig
          node. It is required when using multi node deployment of Uniconfig.
-        uniconfig_url_base: Override default Uniconfig url.
+        uniconfig_url_base: Uniconfig url.
 
     Returns:
         Http response.
     """
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = normalize_base_url(base_url) + DELETE_SNAPSHOT_URL
+    url = normalize_base_url(uniconfig_url_base) + DELETE_SNAPSHOT_URL
     cookies: DictAny = {'UNICONFIGTXID': transaction_id, 'uniconfig_server_id': uniconfig_server_id}
     response = requests.post(
         url,
         data=json.dumps(
             {
                 'input': {
                     'name': snapshot_name
@@ -100,35 +92,31 @@
 
 
 def replace_config_with_snapshot(
     snapshot_name: str,
     node_ids: list[str],
     transaction_id: str,
     uniconfig_server_id: str | None = None,
-    uniconfig_url_base: str | None = None
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Replace Uniconfig CONFIG datastore with a snapshot.
     https://docs.frinx.io/frinx-uniconfig/user-guide/uniconfig-operations/snapshot-manager/rpc_replace-config-with-snapshot/
     Args:
         snapshot_name: Name of Uniconfig snapshot.
         node_ids: Target nodes, which will replace nodes in CONFIG datastore.
         transaction_id: Transaction ID generated by Uniconfig.
         uniconfig_server_id: Uniconfig server id is used by load balancer to forward request to the correct Uniconfig
          node. It is required when using multi node deployment of Uniconfig.
-        uniconfig_url_base: Override default Uniconfig url.
+        uniconfig_url_base: Uniconfig url.
 
     Returns:
         Http response.
     """
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = normalize_base_url(base_url) + REPLACE_CONFIG_WITH_SNAPSHOT_URL
+    url = normalize_base_url(uniconfig_url_base) + REPLACE_CONFIG_WITH_SNAPSHOT_URL
     cookies: DictAny = {'UNICONFIGTXID': transaction_id, 'uniconfig_server_id': uniconfig_server_id}
     response = requests.post(
         url,
         data=json.dumps(
             {
                 'input': {
                     'name': snapshot_name,
```

### Comparing `frinx_python_sdk-0.1.0/frinx/services/uniconfig/uniconfig_manager.py` & `frinx_python_sdk-0.1.1/frinx/services/uniconfig/uniconfig_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,67 +12,59 @@
 from frinx.common.type_aliases import DictAny
 from frinx.common.util import normalize_base_url
 
 
 def create_transaction(
     transaction_timeout: int | None = None,
     use_dedicated_session: bool = False,
-    uniconfig_url_base: str | None = None,
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Create Uniconfig transaction.
     https://docs.frinx.io/frinx-uniconfig/user-guide/uniconfig-operations/build-and-commit-model/#creation-of-transaction
     Args:
         transaction_timeout: Transaction timeout in seconds. This parameter overrides global timeout for Uniconfig
          transactions.
         use_dedicated_session: Create dedicated session for this transaction.
-        uniconfig_url_base: Override default Uniconfig url.
+        uniconfig_url_base: Uniconfig url.
 
     Returns:
         Http response.
     """
     params: DictAny = {}
     if transaction_timeout is not None:
         params['timeout'] = transaction_timeout
 
     if use_dedicated_session:
         params['dedicatedDeviceSession'] = 'true'
 
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = base_url + CREATE_TRANSACTION_URL
+    url = normalize_base_url(uniconfig_url_base) + CREATE_TRANSACTION_URL
     response = requests.post(url=url, params=params, headers=UNICONFIG_HEADERS)
     response.raise_for_status()
     return response
 
 
 def close_transaction(
     transaction_id: str,
     uniconfig_server_id: str | None = None,
-    uniconfig_url_base: str | None = None
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Close Uniconfig transaction.
     https://docs.frinx.io/frinx-uniconfig/user-guide/uniconfig-operations/build-and-commit-model/#closing-transaction
     Args:
         transaction_id: Transaction ID generated by Uniconfig.
         uniconfig_server_id: Uniconfig server id is used by load balancer to forward request to the correct Uniconfig
          node. It is required when using multi node deployment of Uniconfig.
-        uniconfig_url_base: Override default Uniconfig url.
+        uniconfig_url_base: Uniconfig url.
 
     Returns:
         Http response.
     """
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = normalize_base_url(base_url) + CLOSE_TRANSACTION_URL
+    url = normalize_base_url(uniconfig_url_base) + CLOSE_TRANSACTION_URL
     cookies: DictAny = {'UNICONFIGTXID': transaction_id, 'uniconfig_server_id': uniconfig_server_id}
     response = requests.post(
         url=url,
         cookies=cookies,
         headers=UNICONFIG_HEADERS
     )
     response.raise_for_status()
@@ -80,35 +72,31 @@
 
 
 def commit_transaction(
     transaction_id: str,
     uniconfig_server_id: str | None = None,
     confirmed_commit: bool = False,
     validate_commit: bool = True,
-    uniconfig_url_base: str | None = None
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Commit Uniconfig transaction.
     https://docs.frinx.io/frinx-uniconfig/user-guide/uniconfig-operations/uniconfig-node-manager/rpc_commit/
     Args:
         transaction_id: Transaction ID generated by Uniconfig.
         uniconfig_server_id: Uniconfig server id is used by load balancer to forward request to the correct Uniconfig
          node. It is required when using multi node deployment of Uniconfig.
         confirmed_commit: Lock configuration of a node, so no other transaction can make changes on the node.
         validate_commit: Validate constraints and consistency of the transaction.
-        uniconfig_url_base: Override default Uniconfig url.
+        uniconfig_url_base: Uniconfig url.
 
     Returns:
         Http response.
     """
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = normalize_base_url(base_url) + COMMIT_TRANSACTION_URL
+    url = normalize_base_url(uniconfig_url_base) + COMMIT_TRANSACTION_URL
     # Input with target nodes will be deprecated in the future, Uniconfig is able to track modified nodes by itself
     data = json.dumps({
             'input': {
                 'do-confirmed-commit': confirmed_commit,
                 'do-validate': validate_commit,
                 'target-nodes': {
                     'node': []
@@ -126,34 +114,30 @@
     return response
 
 
 def replace_config_with_operational(
     node_ids: list[str],
     transaction_id: str,
     uniconfig_server_id: str | None = None,
-    uniconfig_url_base: str | None = None
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Replace Uniconfig CONFIG datastore with OPER datastore.
     https://docs.frinx.io/frinx-uniconfig/user-guide/uniconfig-operations/uniconfig-node-manager/rpc_replace-config-with-oper/
     Args:
         node_ids: Target nodes, which will replace nodes in CONFIG datastore.
         transaction_id: Transaction ID generated by Uniconfig.
         uniconfig_server_id: Uniconfig server id is used by load balancer to forward request to the correct Uniconfig
          node. It is required when using multi node deployment of Uniconfig.
-        uniconfig_url_base: Override default Uniconfig url.
+        uniconfig_url_base: Uniconfig url.
 
     Returns:
         Http response.
     """
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = normalize_base_url(base_url) + REPLACE_CONFIG_WITH_OPERATIONAL_URL
+    url = normalize_base_url(uniconfig_url_base) + REPLACE_CONFIG_WITH_OPERATIONAL_URL
     cookies: DictAny = {'UNICONFIGTXID': transaction_id, 'uniconfig_server_id': uniconfig_server_id}
     response = requests.post(
         url,
         data=json.dumps(
             {
                 'input': {
                     'target-nodes': {
@@ -170,15 +154,15 @@
     return response
 
 
 def sync_from_network(
     node_ids: list[str],
     transaction_id: str,
     uniconfig_server_id: str | None = None,
-    uniconfig_url_base: str | None = None
+    uniconfig_url_base: str = UNICONFIG_URL_BASE
 ) -> requests.Response:
     """
     Synchronize configuration from network nodes to the UniConfig nodes
      in the Operational datastore of UniConfig transaction.
     https://docs.frinx.io/frinx-uniconfig/user-guide/uniconfig-operations/uniconfig-node-manager/rpc_sync-from-network/
     Args:
         node_ids: Target nodes, which will be synced from network.
@@ -186,19 +170,15 @@
          node. It is required when using multi node deployment of Uniconfig.
         transaction_id: Transaction ID generated by Uniconfig.
         uniconfig_url_base: Override default Uniconfig url.
 
     Returns:
         Http response.
     """
-    base_url = UNICONFIG_URL_BASE
-    if uniconfig_url_base is not None:
-        base_url = uniconfig_url_base
-
-    url = normalize_base_url(base_url) + SYNC_FROM_NETWORK_URL
+    url = normalize_base_url(uniconfig_url_base) + SYNC_FROM_NETWORK_URL
     cookies: DictAny = {'UNICONFIGTXID': transaction_id, 'uniconfig_server_id': uniconfig_server_id}
     response = requests.post(
         url,
         data=json.dumps(
             {
                 'input': {
                     'target-nodes': {
```

### Comparing `frinx_python_sdk-0.1.0/frinx/workers/uniconfig/cli_network_topology.py` & `frinx_python_sdk-0.1.1/frinx/workers/uniconfig/cli_network_topology.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 from typing import Any
 
 from frinx.common.conductor_enums import TaskResultStatus
+from frinx.common.frinx_rest import UNICONFIG_URL_BASE
+from frinx.common.type_aliases import ListAny
 from frinx.common.worker.service import ServiceWorkersImpl
 from frinx.common.worker.task_def import TaskDefinition
 from frinx.common.worker.task_def import TaskInput
 from frinx.common.worker.task_def import TaskOutput
 from frinx.common.worker.task_result import TaskResult
 from frinx.common.worker.worker import WorkerImpl
 from frinx.services.uniconfig.cli_network_topology import execute
 from frinx.services.uniconfig.cli_network_topology import execute_and_read
 
 
 class CliNetworkTopology(ServiceWorkersImpl):
     class ExecuteAndRead(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Execute_and_read_RPC'
-            description = 'Run execute and read RPC'
+            name: str = 'UNICONFIG_Execute_and_read_RPC'
+            description: str = 'Run execute and read RPC'
 
         class WorkerInput(TaskInput):
             node_id: str
             command: str
             transaction_id: str
             uniconfig_server_id: str | None = None
             wait_for_output: int = 0
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
         class WorkerOutput(TaskOutput):
             output: dict[str, Any]
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[WorkerOutput]:
             response = execute_and_read(
                 node_id=worker_input.node_id,
                 command=worker_input.command,
                 transaction_id=worker_input.transaction_id,
                 uniconfig_server_id=worker_input.uniconfig_server_id,
                 wait_for_output=worker_input.wait_for_output,
                 uniconfig_url_base=worker_input.uniconfig_url_base
             )
-            return TaskResult(status=TaskResultStatus.COMPLETED, output=response.json())
+            return TaskResult(status=TaskResultStatus.COMPLETED, output=self.WorkerOutput(output=response.json()))
 
     class Execute(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Execute_RPC'
-            description = 'Run execute RPC'
-            labels = ['UNICONFIG']
+            name: str = 'UNICONFIG_Execute_RPC'
+            description: str = 'Run execute RPC'
+            labels: ListAny = ['UNICONFIG']
 
         class WorkerInput(TaskInput):
             node_id: str
             command: str
             transaction_id: str
             uniconfig_server_id: str | None = None
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
         class WorkerOutput(TaskOutput):
             output: dict[str, Any]
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[WorkerOutput]:
             response = execute(
                 node_id=worker_input.node_id,
                 command=worker_input.command,
                 transaction_id=worker_input.transaction_id,
                 uniconfig_server_id=worker_input.uniconfig_server_id,
                 uniconfig_url_base=worker_input.uniconfig_url_base
             )
-            return TaskResult(status=TaskResultStatus.COMPLETED, output=response.json())
+            return TaskResult(status=TaskResultStatus.COMPLETED, output=self.WorkerOutput(output=response.json()))
```

### Comparing `frinx_python_sdk-0.1.0/frinx/workers/uniconfig/connection_manager.py` & `frinx_python_sdk-0.1.1/frinx/workers/uniconfig/connection_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 from typing import Literal
 
 from frinx.common.conductor_enums import TaskResultStatus
+from frinx.common.frinx_rest import UNICONFIG_URL_BASE
 from frinx.common.type_aliases import DictAny
 from frinx.common.worker.service import ServiceWorkersImpl
 from frinx.common.worker.task_def import TaskDefinition
 from frinx.common.worker.task_def import TaskInput
 from frinx.common.worker.task_def import TaskOutput
 from frinx.common.worker.task_result import TaskResult
 from frinx.common.worker.worker import WorkerImpl
 from frinx.services.uniconfig.connection_manager import install_node
 from frinx.services.uniconfig.connection_manager import uninstall_node
 
 
 class ConnectionManager(ServiceWorkersImpl):
     class InstallNode(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Install_node_RPC'
-            description = 'Install node to Uniconfig'
+            name: str = 'UNICONFIG_Install_node_RPC'
+            description: str = 'Install node to Uniconfig'
 
         class WorkerInput(TaskInput):
             node_id: str
             connection_type: Literal['netconf', 'cli']
             install_params: DictAny
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
         class WorkerOutput(TaskOutput):
             output: DictAny
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[WorkerOutput]:
             response = install_node(
                 node_id=worker_input.node_id,
                 connection_type=worker_input.connection_type,
                 install_params=worker_input.install_params,
                 uniconfig_url_base=worker_input.uniconfig_url_base
             )
-            return TaskResult(status=TaskResultStatus.COMPLETED, output=response.json())
+            return TaskResult(status=TaskResultStatus.COMPLETED, output=self.WorkerOutput(output=response.json()))
 
     class UninstallNode(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Uninstall_node_RPC'
-            description = 'Uninstall node from Uniconfig'
+            name: str = 'UNICONFIG_Uninstall_node_RPC'
+            description: str = 'Uninstall node from Uniconfig'
 
         class WorkerInput(TaskInput):
             node_id: str
             connection_type: Literal['netconf', 'cli']
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
         class WorkerOutput(TaskOutput):
             output: DictAny
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[WorkerOutput]:
             response = uninstall_node(
                 node_id=worker_input.node_id,
                 connection_type=worker_input.connection_type,
                 uniconfig_url_base=worker_input.uniconfig_url_base
             )
-            return TaskResult(status=TaskResultStatus.COMPLETED, output=response.json())
+            return TaskResult(status=TaskResultStatus.COMPLETED, output=self.WorkerOutput(output=response.json()))
```

### Comparing `frinx_python_sdk-0.1.0/frinx/workers/uniconfig/snapshot_manager.py` & `frinx_python_sdk-0.1.1/frinx/workers/uniconfig/snapshot_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 from frinx.common.conductor_enums import TaskResultStatus
+from frinx.common.frinx_rest import UNICONFIG_URL_BASE
 from frinx.common.type_aliases import DictAny
 from frinx.common.worker.service import ServiceWorkersImpl
 from frinx.common.worker.task_def import TaskDefinition
 from frinx.common.worker.task_def import TaskInput
 from frinx.common.worker.task_def import TaskOutput
 from frinx.common.worker.task_result import TaskResult
 from frinx.common.worker.worker import WorkerImpl
@@ -11,77 +12,77 @@
 from frinx.services.uniconfig.snapshot_manager import delete_snapshot
 from frinx.services.uniconfig.snapshot_manager import replace_config_with_snapshot
 
 
 class SnapshotManager(ServiceWorkersImpl):
     class CreateSnapshot(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Create_snapshot_RPC'
-            description = 'Create Uniconfig snapshot'
+            name: str = 'UNICONFIG_Create_snapshot_RPC'
+            description: str = 'Create Uniconfig snapshot'
 
         class WorkerInput(TaskInput):
             node_ids: list[str]
             snapshot_name: str
             transaction_id: str
             uniconfig_server_id: str | None = None
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
         class WorkerOutput(TaskOutput):
             output: DictAny
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[WorkerOutput]:
             response = create_snapshot(
                 node_ids=worker_input.node_ids,
                 snapshot_name=worker_input.snapshot_name,
                 transaction_id=worker_input.transaction_id,
                 uniconfig_server_id=worker_input.uniconfig_server_id,
                 uniconfig_url_base=worker_input.uniconfig_url_base
             )
-            return TaskResult(status=TaskResultStatus.COMPLETED, output=response.json())
+            return TaskResult(status=TaskResultStatus.COMPLETED, output=self.WorkerOutput(output=response.json()))
 
     class DeleteSnapshot(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Delete_snapshot_RPC'
-            description = 'Delete Uniconfig snapshot'
+            name: str = 'UNICONFIG_Delete_snapshot_RPC'
+            description: str = 'Delete Uniconfig snapshot'
 
         class WorkerInput(TaskInput):
             snapshot_name: str
             transaction_id: str
             uniconfig_server_id: str | None = None
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
         class WorkerOutput(TaskOutput):
             output: DictAny
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[WorkerOutput]:
             response = delete_snapshot(
                 snapshot_name=worker_input.snapshot_name,
                 transaction_id=worker_input.transaction_id,
                 uniconfig_server_id=worker_input.uniconfig_server_id,
                 uniconfig_url_base=worker_input.uniconfig_url_base
             )
-            return TaskResult(status=TaskResultStatus.COMPLETED, output=response.json())
+            return TaskResult(status=TaskResultStatus.COMPLETED, output=self.WorkerOutput(output=response.json()))
 
     class ReplaceConfigWithSnapshot(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Replace_config_with_snapshot_RPC'
-            description = 'Replace Uniconfig CONFIG datastore with a snapshot'
+            name: str = 'UNICONFIG_Replace_config_with_snapshot_RPC'
+            description: str = 'Replace Uniconfig CONFIG datastore with a snapshot'
 
         class WorkerInput(TaskInput):
             snapshot_name: str
             node_ids: list[str]
             transaction_id: str
             uniconfig_server_id: str | None = None
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
         class WorkerOutput(TaskOutput):
             output: DictAny
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[WorkerOutput]:
             response = replace_config_with_snapshot(
                 snapshot_name=worker_input.snapshot_name,
                 node_ids=worker_input.node_ids,
                 transaction_id=worker_input.transaction_id,
                 uniconfig_server_id=worker_input.uniconfig_server_id,
                 uniconfig_url_base=worker_input.uniconfig_url_base
             )
-            return TaskResult(status=TaskResultStatus.COMPLETED, output=response.json())
+            return TaskResult(status=TaskResultStatus.COMPLETED, output=self.WorkerOutput(output=response.json()))
```

### Comparing `frinx_python_sdk-0.1.0/frinx/workers/uniconfig/uniconfig_manager.py` & `frinx_python_sdk-0.1.1/frinx/workers/uniconfig/uniconfig_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 from frinx.common.conductor_enums import TaskResultStatus
+from frinx.common.frinx_rest import UNICONFIG_URL_BASE
 from frinx.common.type_aliases import DictAny
 from frinx.common.worker.service import ServiceWorkersImpl
 from frinx.common.worker.task_def import TaskDefinition
 from frinx.common.worker.task_def import TaskInput
 from frinx.common.worker.task_def import TaskOutput
 from frinx.common.worker.task_result import TaskResult
 from frinx.common.worker.worker import WorkerImpl
@@ -13,117 +14,117 @@
 from frinx.services.uniconfig.uniconfig_manager import replace_config_with_operational
 from frinx.services.uniconfig.uniconfig_manager import sync_from_network
 
 
 class UniconfigManager(ServiceWorkersImpl):
     class CreateTransaction(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Create_transaction_RPC'
-            description = 'Create Uniconfig transaction'
+            name: str = 'UNICONFIG_Create_transaction_RPC'
+            description: str = 'Create Uniconfig transaction'
 
         class WorkerInput(TaskInput):
             transaction_timeout: int | None = None
             use_dedicated_session: bool = False
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
         class WorkerOutput(TaskOutput):
             transaction_id: str
             uniconfig_server_id: str | None
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[WorkerOutput]:
             response = create_transaction(
                 transaction_timeout=worker_input.transaction_timeout,
                 use_dedicated_session=worker_input.use_dedicated_session,
                 uniconfig_url_base=worker_input.uniconfig_url_base
             )
             cookies: DictAny = response.cookies.get_dict()  # type: ignore
             transaction_id: str = cookies['UNICONFIGTXID']
             uniconfig_server_id: str | None = cookies.get('uniconfig_server_id')
             return TaskResult(
                 status=TaskResultStatus.COMPLETED,
-                output={'transaction_id': transaction_id, 'uniconfig_server_id': uniconfig_server_id}
+                output=self.WorkerOutput(transaction_id=transaction_id, uniconfig_server_id=uniconfig_server_id)
             )
 
     class CloseTransaction(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Close_transaction_RPC'
-            description = 'Close Uniconfig transaction'
+            name: str = 'UNICONFIG_Close_transaction_RPC'
+            description: str = 'Close Uniconfig transaction'
 
         class WorkerInput(TaskInput):
             transaction_id: str
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[None]:
             close_transaction(transaction_id=worker_input.transaction_id)
             return TaskResult(status=TaskResultStatus.COMPLETED)
 
     class CommitTransaction(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Commit_transaction_RPC'
-            description = 'Commit Uniconfig transaction'
+            name: str = 'UNICONFIG_Commit_transaction_RPC'
+            description: str = 'Commit Uniconfig transaction'
 
         class WorkerInput(TaskInput):
             transaction_id: str
             confirmed_commit: bool = False
             validate_commit: bool = True
             uniconfig_server_id: str | None = None
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
         class WorkerOutput(TaskOutput):
             output: DictAny
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[WorkerOutput]:
             response = commit_transaction(
                 transaction_id=worker_input.transaction_id,
                 uniconfig_server_id=worker_input.uniconfig_server_id,
                 confirmed_commit=worker_input.confirmed_commit,
                 validate_commit=worker_input.validate_commit,
                 uniconfig_url_base=worker_input.uniconfig_url_base
             )
 
-            return TaskResult(status=TaskResultStatus.COMPLETED, output=response.json())
+            return TaskResult(status=TaskResultStatus.COMPLETED, output=self.WorkerOutput(output=response.json()))
 
     class ReplaceConfigWithOperational(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Replace_config_with_operational_RPC'
-            description = 'Replace Uniconfig CONFIG datastore with OPER datastore'
+            name: str = 'UNICONFIG_Replace_config_with_operational_RPC'
+            description: str = 'Replace Uniconfig CONFIG datastore with OPER datastore'
 
         class WorkerInput(TaskInput):
             node_ids: list[str]
             transaction_id: str
             uniconfig_server_id: str | None = None
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
         class WorkerOutput(TaskOutput):
             output: DictAny
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[WorkerOutput]:
             response = replace_config_with_operational(
                 node_ids=worker_input.node_ids,
                 transaction_id=worker_input.transaction_id,
                 uniconfig_server_id=worker_input.uniconfig_server_id,
                 uniconfig_url_base=worker_input.uniconfig_url_base
             )
-            return TaskResult(status=TaskResultStatus.COMPLETED, output=response.json())
+            return TaskResult(status=TaskResultStatus.COMPLETED, output=self.WorkerOutput(output=response.json()))
 
     class SyncFromNetwork(WorkerImpl):
         class WorkerDefinition(TaskDefinition):
-            name = 'Sync_from_network_RPC'
-            description = 'Synchronize configuration from network and the UniConfig nodes'
+            name: str = 'UNICONFIG_Sync_from_network_RPC'
+            description: str = 'Synchronize configuration from network and the UniConfig nodes'
 
         class WorkerInput(TaskInput):
             node_ids: list[str]
             transaction_id: str
             uniconfig_server_id: str | None = None
-            uniconfig_url_base: str | None = None
+            uniconfig_url_base: str = UNICONFIG_URL_BASE
 
         class WorkerOutput(TaskOutput):
             output: DictAny
 
-        def execute(self, worker_input: WorkerInput) -> TaskResult:
+        def execute(self, worker_input: WorkerInput) -> TaskResult[WorkerOutput]:
             response = sync_from_network(
                 node_ids=worker_input.node_ids,
                 transaction_id=worker_input.transaction_id,
                 uniconfig_server_id=worker_input.uniconfig_server_id,
                 uniconfig_url_base=worker_input.uniconfig_url_base
             )
-            return TaskResult(status=TaskResultStatus.COMPLETED, output=response.json())
+            return TaskResult(status=TaskResultStatus.COMPLETED, output=self.WorkerOutput(output=response.json()))
```

