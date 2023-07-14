# Comparing `tmp/taskiq-0.8.2.tar.gz` & `tmp/taskiq-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.8.2.tar", max compression
+gzip compressed data, was "taskiq-0.8.3.tar", max compression
```

## Comparing `taskiq-0.8.2.tar` & `taskiq-0.8.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1075 2023-07-12 10:27:06.760774 taskiq-0.8.2/LICENSE
--rw-r--r--   0        0        0     1875 2023-07-12 10:27:06.760774 taskiq-0.8.2/README.md
--rw-r--r--   0        0        0     3007 2023-07-12 10:27:06.764774 taskiq-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2161 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/__init__.py
--rw-r--r--   0        0        0     2093 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/abc/__init__.py
--rw-r--r--   0        0        0    12957 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/abc/broker.py
--rw-r--r--   0        0        0      323 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      629 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     3562 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1376 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1623 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0      496 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/acks.py
--rw-r--r--   0        0        0       34 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     5679 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2197 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2831 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      197 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     2076 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     3767 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2550 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1517 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     5805 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0      628 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     8307 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     6471 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0     1567 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/compat.py
--rw-r--r--   0        0        0     1251 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/context.py
--rw-r--r--   0        0        0     2930 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/decor.py
--rw-r--r--   0        0        0      511 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/events.py
--rw-r--r--   0        0        0     1010 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      928 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1887 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/funcs.py
--rw-r--r--   0        0        0     5552 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/kicker.py
--rw-r--r--   0        0        0      507 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     4535 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/middlewares/prometheus_middleware.py
--rw-r--r--   0        0        0     2438 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/py.typed
--rw-r--r--   0        0        0      113 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/receiver/__init__.py
--rw-r--r--   0        0        0     2799 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/receiver/params_parser.py
--rw-r--r--   0        0        0    12601 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/receiver/receiver.py
--rw-r--r--   0        0        0      237 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/result/__init__.py
--rw-r--r--   0        0        0     2084 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/result/v1.py
--rw-r--r--   0        0        0     1923 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/result/v2.py
--rw-r--r--   0        0        0       35 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1268 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     2554 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     2404 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0    11916 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/serialization.py
--rw-r--r--   0        0        0     1071 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/state.py
--rw-r--r--   0        0        0     4141 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/task.py
--rw-r--r--   0        0        0      900 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/utils.py
--rw-r--r--   0        0        0      106 2023-07-12 10:27:06.764774 taskiq-0.8.2/taskiq/warnings.py
--rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 taskiq-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-14 08:18:23.007418 taskiq-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1875 2023-07-14 08:18:23.007418 taskiq-0.8.3/README.md
+-rw-r--r--   0        0        0     3007 2023-07-14 08:18:23.011418 taskiq-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2022 2023-07-14 08:18:23.011418 taskiq-0.8.3/taskiq/__init__.py
+-rw-r--r--   0        0        0     2093 2023-07-14 08:18:23.011418 taskiq-0.8.3/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-07-14 08:18:23.011418 taskiq-0.8.3/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0    12959 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      323 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     3562 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1376 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1623 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0      496 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/acks.py
+-rw-r--r--   0        0        0       34 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     5679 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2197 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2831 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     2076 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     3767 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2550 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1517 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     5805 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      628 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     8307 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     6471 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0     1567 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/compat.py
+-rw-r--r--   0        0        0     1251 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/context.py
+-rw-r--r--   0        0        0     2930 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/decor.py
+-rw-r--r--   0        0        0      511 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/events.py
+-rw-r--r--   0        0        0     1010 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      928 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1887 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/funcs.py
+-rw-r--r--   0        0        0     5552 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4056 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2438 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/py.typed
+-rw-r--r--   0        0        0      113 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2799 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0    12601 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0      237 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/result/__init__.py
+-rw-r--r--   0        0        0     2084 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/result/v1.py
+-rw-r--r--   0        0        0     1923 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/result/v2.py
+-rw-r--r--   0        0        0       35 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1268 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     2554 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     2404 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0    11916 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/serialization.py
+-rw-r--r--   0        0        0     1071 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/state.py
+-rw-r--r--   0        0        0     4141 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/task.py
+-rw-r--r--   0        0        0      900 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/utils.py
+-rw-r--r--   0        0        0      106 2023-07-14 08:18:23.015419 taskiq-0.8.3/taskiq/warnings.py
+-rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 taskiq-0.8.3/PKG-INFO
```

### Comparing `taskiq-0.8.2/LICENSE` & `taskiq-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/README.md` & `taskiq-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/pyproject.toml` & `taskiq-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.8.2"
+version = "0.8.3"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
```

### Comparing `taskiq-0.8.2/taskiq/__init__.py` & `taskiq-0.8.3/taskiq/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Distributed task manager."""
+from importlib.metadata import version
+
 from taskiq_dependencies import Depends as TaskiqDepends
 
 from taskiq.abc.broker import AsyncBroker, AsyncTaskiqDecoratedTask
 from taskiq.abc.formatter import TaskiqFormatter
 from taskiq.abc.middleware import TaskiqMiddleware
 from taskiq.abc.result_backend import AsyncResultBackend
 from taskiq.abc.schedule_source import ScheduleSource
@@ -26,21 +28,14 @@
 from taskiq.middlewares.prometheus_middleware import PrometheusMiddleware
 from taskiq.middlewares.retry_middleware import SimpleRetryMiddleware
 from taskiq.result import TaskiqResult
 from taskiq.scheduler import ScheduledTask, TaskiqScheduler
 from taskiq.state import TaskiqState
 from taskiq.task import AsyncTaskiqTask
 
-try:
-    # Python 3.8+
-    from importlib.metadata import version  # noqa: WPS433
-except ImportError:
-    # Python 3.7
-    from importlib_metadata import version  # noqa: WPS433
-
 __version__ = version("taskiq")
 __all__ = [
     "__version__",
     "gather",
     "Context",
     "AsyncBroker",
     "TaskiqError",
```

### Comparing `taskiq-0.8.2/taskiq/__main__.py` & `taskiq-0.8.3/taskiq/__main__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/abc/broker.py` & `taskiq-0.8.3/taskiq/abc/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             event = TaskiqEvents.WORKER_STARTUP
 
         for handler in self.event_handlers[event]:
             await maybe_awaitable(handler(self.state))
 
         for middleware in self.middlewares:
             if middleware.__class__.startup != TaskiqMiddleware.startup:
-                await maybe_awaitable(middleware.startup)
+                await maybe_awaitable(middleware.startup())
 
         await self.result_backend.startup()
 
     async def shutdown(self) -> None:
         """
         Close the broker.
```

### Comparing `taskiq-0.8.2/taskiq/abc/formatter.py` & `taskiq-0.8.3/taskiq/abc/formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/abc/middleware.py` & `taskiq-0.8.3/taskiq/abc/middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/abc/result_backend.py` & `taskiq-0.8.3/taskiq/abc/result_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/abc/schedule_source.py` & `taskiq-0.8.3/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/brokers/inmemory_broker.py` & `taskiq-0.8.3/taskiq/brokers/inmemory_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/brokers/shared_broker.py` & `taskiq-0.8.3/taskiq/brokers/shared_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/brokers/zmq_broker.py` & `taskiq-0.8.3/taskiq/brokers/zmq_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/cli/scheduler/args.py` & `taskiq-0.8.3/taskiq/cli/scheduler/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/cli/scheduler/cmd.py` & `taskiq-0.8.3/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/cli/scheduler/run.py` & `taskiq-0.8.3/taskiq/cli/scheduler/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/cli/utils.py` & `taskiq-0.8.3/taskiq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/cli/watcher.py` & `taskiq-0.8.3/taskiq/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/cli/worker/args.py` & `taskiq-0.8.3/taskiq/cli/worker/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/cli/worker/cmd.py` & `taskiq-0.8.3/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/cli/worker/log_collector.py` & `taskiq-0.8.3/taskiq/cli/worker/log_collector.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/cli/worker/process_manager.py` & `taskiq-0.8.3/taskiq/cli/worker/process_manager.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/cli/worker/run.py` & `taskiq-0.8.3/taskiq/cli/worker/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/compat.py` & `taskiq-0.8.3/taskiq/compat.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/context.py` & `taskiq-0.8.3/taskiq/context.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/decor.py` & `taskiq-0.8.3/taskiq/decor.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/exceptions.py` & `taskiq-0.8.3/taskiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/formatters/json_formatter.py` & `taskiq-0.8.3/taskiq/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/funcs.py` & `taskiq-0.8.3/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/kicker.py` & `taskiq-0.8.3/taskiq/kicker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/middlewares/prometheus_middleware.py` & `taskiq-0.8.3/taskiq/middlewares/prometheus_middleware.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,20 +25,14 @@
         self,
         metrics_path: Optional[Path] = None,
         server_port: int = 9000,
         server_addr: str = "0.0.0.0",  # noqa: S104
     ) -> None:
         super().__init__()
 
-        self.found_errors = None
-        self.received_tasks = None
-        self.success_tasks = None
-        self.saved_results = None
-        self.execution_time = None
-
         metrics_path = metrics_path or Path(gettempdir()) / "taskiq_worker"
 
         if not metrics_path.exists():
             metrics_path.mkdir(parents=True)
 
         logger.debug(f"Setting up multiproc dir to {metrics_path}")
 
@@ -72,15 +66,15 @@
         self.saved_results = Counter(
             "saved_results",
             "Number of saved results in result backend",
             ["task_name"],
         )
         self.execution_time = Histogram(
             "execution_time",
-            "Tome of function execution",
+            "Time of function execution",
             ["task_name"],
         )
         self.server_port = server_port
         self.server_addr = server_addr
 
     def startup(self) -> None:
         """
@@ -106,36 +100,28 @@
 
         This function increments a counter of received tasks,
         when called.
 
         :param message: current message.
         :return: message
         """
-        if self.received_tasks is None:
-            return message
         self.received_tasks.labels(message.task_name).inc()
         return message
 
     def post_execute(
         self,
         message: "TaskiqMessage",
         result: "TaskiqResult[Any]",
     ) -> None:
         """
         This function tracks number of errors and success executions.
 
         :param message: received message.
         :param result: result of the execution.
         """
-        if (  # noqa: WPS337
-            self.success_tasks is None
-            or self.execution_time is None
-            or self.found_errors is None
-        ):
-            return
         if result.is_err:
             self.found_errors.labels(message.task_name).inc()
         else:
             self.success_tasks.labels(message.task_name).inc()
         self.execution_time.labels(message.task_name).observe(result.execution_time)
 
     def post_save(
@@ -145,10 +131,8 @@
     ) -> "None":
         """
         Method to run on save.
 
         :param message: received message.
         :param result: result of execution.
         """
-        if self.saved_results is None:
-            return
         self.saved_results.labels(message.task_name).inc()
```

### Comparing `taskiq-0.8.2/taskiq/middlewares/retry_middleware.py` & `taskiq-0.8.3/taskiq/middlewares/retry_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/receiver/params_parser.py` & `taskiq-0.8.3/taskiq/receiver/params_parser.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/receiver/receiver.py` & `taskiq-0.8.3/taskiq/receiver/receiver.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/result/v1.py` & `taskiq-0.8.3/taskiq/result/v1.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/result/v2.py` & `taskiq-0.8.3/taskiq/result/v2.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/result_backends/dummy.py` & `taskiq-0.8.3/taskiq/result_backends/dummy.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/schedule_sources/label_based.py` & `taskiq-0.8.3/taskiq/schedule_sources/label_based.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/scheduler/merge_functions.py` & `taskiq-0.8.3/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/scheduler/scheduler.py` & `taskiq-0.8.3/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/serialization.py` & `taskiq-0.8.3/taskiq/serialization.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/state.py` & `taskiq-0.8.3/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/task.py` & `taskiq-0.8.3/taskiq/task.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/taskiq/utils.py` & `taskiq-0.8.3/taskiq/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.8.2/PKG-INFO` & `taskiq-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq
-Version: 0.8.2
+Version: 0.8.3
 Summary: Distributed task queue with full async support
 Home-page: https://taskiq-python.github.io/
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Maintainer: Pavel Kirilin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskiq Version: 0.8.2 Summary: Distributed task
+Metadata-Version: 2.1 Name: taskiq Version: 0.8.3 Summary: Distributed task
 queue with full async support Home-page: https://taskiq-python.github.io/
 License: LICENSE Keywords: taskiq,tasks,distributed,async Author: Pavel Kirilin
 Author-email: win10@list.ru Maintainer: Pavel Kirilin Maintainer-email:
 win10@list.ru Requires-Python: >=3.8.1,<4.0.0 Classifier: Development Status ::
 3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 Other/Proprietary License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

