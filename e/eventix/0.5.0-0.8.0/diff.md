# Comparing `tmp/eventix-0.5.0.tar.gz` & `tmp/eventix-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventix-0.5.0.tar", max compression
+gzip compressed data, was "eventix-0.8.0.tar", max compression
```

## Comparing `eventix-0.5.0.tar` & `eventix-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,55 @@
--rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/__init__.py
--rw-r--r--   0        0        0     1117 2023-07-04 15:24:17.141091 eventix-0.5.0/eventix/contexts/__init__.py
--rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.5.0/eventix/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/functions/__init__.py
--rw-r--r--   0        0        0     3500 2023-07-04 15:24:17.133091 eventix-0.5.0/eventix/functions/core.py
--rw-r--r--   0        0        0      709 2023-07-03 12:35:26.910564 eventix-0.5.0/eventix/functions/errors.py
--rw-r--r--   0        0        0      801 2023-07-04 06:52:56.282299 eventix-0.5.0/eventix/functions/eventix_client.py
--rw-r--r--   0        0        0     2815 2023-07-04 08:25:54.140139 eventix-0.5.0/eventix/functions/fastapi.py
--rw-r--r--   0        0        0     5982 2023-07-04 21:08:43.049808 eventix-0.5.0/eventix/functions/task.py
--rw-r--r--   0        0        0     1155 2023-07-04 15:24:17.145091 eventix-0.5.0/eventix/functions/task_scheduler.py
--rw-r--r--   0        0        0     5469 2023-07-04 15:24:17.137091 eventix-0.5.0/eventix/functions/task_worker.py
--rw-r--r--   0        0        0      322 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/functions/tools.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/pydantic/__init__.py
--rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/pydantic/event.py
--rw-r--r--   0        0        0     1987 2023-07-04 12:48:48.055369 eventix-0.5.0/eventix/pydantic/task.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/router/__init__.py
--rw-r--r--   0        0        0      517 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/router/event.py
--rw-r--r--   0        0        0      236 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/router/metrics.py
--rw-r--r--   0        0        0     1201 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/router/task.py
--rw-r--r--   0        0        0        0 2023-07-04 19:28:16.696215 eventix-0.5.0/eventix/tasks/__init__.py
--rw-r--r--   0        0        0      219 2023-07-04 21:10:00.620848 eventix-0.5.0/eventix/tasks/cleanup.py
--rw-r--r--   0        0        0      974 2023-07-04 21:15:38.476803 eventix-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 eventix-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.0/eventix/__init__.py
+-rw-r--r--   0        0        0     1577 2023-07-06 06:33:36.740790 eventix-0.8.0/eventix/contexts/__init__.py
+-rw-r--r--   0        0        0     2796 2023-07-06 07:02:50.296411 eventix-0.8.0/eventix/contexts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/depends/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.8.0/eventix/exceptions/__init__.py
+-rw-r--r--   0        0        0     2396 2023-07-03 12:34:47.194805 eventix-0.8.0/eventix/exceptions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.0/eventix/functions/__init__.py
+-rw-r--r--   0        0        0      176 2023-07-03 12:30:27.428538 eventix-0.8.0/eventix/functions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6492 2023-07-06 14:41:10.892197 eventix-0.8.0/eventix/functions/__pycache__/core.cpython-311.pyc
+-rw-r--r--   0        0        0     1833 2023-07-13 10:40:02.600612 eventix-0.8.0/eventix/functions/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0     2546 2023-07-07 07:11:23.559241 eventix-0.8.0/eventix/functions/__pycache__/eventix_client.cpython-311.pyc
+-rw-r--r--   0        0        0     5466 2023-07-04 08:25:54.680135 eventix-0.8.0/eventix/functions/__pycache__/fastapi.cpython-311.pyc
+-rw-r--r--   0        0        0     2013 2023-07-12 07:19:14.246636 eventix-0.8.0/eventix/functions/__pycache__/metrics.cpython-311.pyc
+-rw-r--r--   0        0        0      942 2023-07-06 14:41:10.948196 eventix-0.8.0/eventix/functions/__pycache__/schedule.cpython-311.pyc
+-rw-r--r--   0        0        0     8220 2023-07-13 11:00:24.001119 eventix-0.8.0/eventix/functions/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     3107 2023-07-04 20:37:50.771263 eventix-0.8.0/eventix/functions/__pycache__/task_scheduler.cpython-311.pyc
+-rw-r--r--   0        0        0    15277 2023-07-12 07:19:14.218636 eventix-0.8.0/eventix/functions/__pycache__/task_worker.cpython-311.pyc
+-rw-r--r--   0        0        0     2089 2023-07-12 07:19:14.222636 eventix-0.8.0/eventix/functions/__pycache__/tools.cpython-311.pyc
+-rw-r--r--   0        0        0     4036 2023-07-06 14:36:57.587160 eventix-0.8.0/eventix/functions/core.py
+-rw-r--r--   0        0        0      950 2023-07-13 10:39:48.044793 eventix-0.8.0/eventix/functions/errors.py
+-rw-r--r--   0        0        0     1676 2023-07-07 07:11:22.071252 eventix-0.8.0/eventix/functions/eventix_client.py
+-rw-r--r--   0        0        0     2815 2023-07-04 08:25:54.140139 eventix-0.8.0/eventix/functions/fastapi.py
+-rw-r--r--   0        0        0      858 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/functions/metrics.py
+-rw-r--r--   0        0        0      426 2023-07-06 14:36:57.671160 eventix-0.8.0/eventix/functions/schedule.py
+-rw-r--r--   0        0        0     7507 2023-07-13 11:00:20.373143 eventix-0.8.0/eventix/functions/task.py
+-rw-r--r--   0        0        0     1155 2023-07-04 15:24:17.145091 eventix-0.8.0/eventix/functions/task_scheduler.py
+-rw-r--r--   0        0        0     7605 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/functions/task_worker.py
+-rw-r--r--   0        0        0      790 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/functions/tools.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.0/eventix/pydantic/__init__.py
+-rw-r--r--   0        0        0      175 2023-07-03 12:30:27.464538 eventix-0.8.0/eventix/pydantic/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1024 2023-07-03 12:35:27.342561 eventix-0.8.0/eventix/pydantic/__pycache__/event.cpython-311.pyc
+-rw-r--r--   0        0        0     1670 2023-07-12 07:19:14.222636 eventix-0.8.0/eventix/pydantic/__pycache__/pagination.cpython-311.pyc
+-rw-r--r--   0        0        0     1666 2023-07-06 19:19:55.403553 eventix-0.8.0/eventix/pydantic/__pycache__/schedule.cpython-311.pyc
+-rw-r--r--   0        0        0     3075 2023-07-13 11:01:55.584489 eventix-0.8.0/eventix/pydantic/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.8.0/eventix/pydantic/event.py
+-rw-r--r--   0        0        0      615 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/pydantic/pagination.py
+-rw-r--r--   0        0        0      634 2023-07-06 19:19:42.803712 eventix-0.8.0/eventix/pydantic/schedule.py
+-rw-r--r--   0        0        0     2063 2023-07-13 11:01:52.956508 eventix-0.8.0/eventix/pydantic/task.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.0/eventix/router/__init__.py
+-rw-r--r--   0        0        0      173 2023-07-03 12:35:27.342561 eventix-0.8.0/eventix/router/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      989 2023-07-12 07:19:14.258636 eventix-0.8.0/eventix/router/__pycache__/default.cpython-311.pyc
+-rw-r--r--   0        0        0      748 2023-07-12 07:19:14.246636 eventix-0.8.0/eventix/router/__pycache__/metrics.cpython-311.pyc
+-rw-r--r--   0        0        0     2068 2023-07-12 07:19:14.250636 eventix-0.8.0/eventix/router/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     2577 2023-07-12 07:19:14.258636 eventix-0.8.0/eventix/router/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0        0        0      340 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/router/default.py
+-rw-r--r--   0        0        0      243 2023-07-12 07:18:50.102891 eventix-0.8.0/eventix/router/metrics.py
+-rw-r--r--   0        0        0      913 2023-07-12 07:18:50.102891 eventix-0.8.0/eventix/router/task.py
+-rw-r--r--   0        0        0     1386 2023-07-12 07:18:50.102891 eventix-0.8.0/eventix/router/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:28:16.696215 eventix-0.8.0/eventix/tasks/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-04 20:38:18.799048 eventix-0.8.0/eventix/tasks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1107 2023-07-06 20:58:27.178748 eventix-0.8.0/eventix/tasks/__pycache__/cleanup.cpython-311.pyc
+-rw-r--r--   0        0        0      396 2023-07-06 20:57:49.171190 eventix-0.8.0/eventix/tasks/cleanup.py
+-rw-r--r--   0        0        0     1025 2023-07-14 10:59:43.151255 eventix-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 eventix-0.8.0/PKG-INFO
```

### Comparing `eventix-0.5.0/eventix/contexts/__init__.py` & `eventix-0.8.0/eventix/contexts/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,32 @@
     # noinspection PyTypeChecker
     namespace = namespace_context_var.get()
     if namespace is None:
         namespace = os.environ.get("EVENTIX_NAMESPACE", "default")
     yield namespace
 
 
+delay_tasks_context_var = contextvars.ContextVar('delay_tasks_context_var', default=True)
+
+
+@contextlib.contextmanager
+def delay_tasks(delay_tasks: bool = True):
+    # noinspection PyTypeChecker
+    token = delay_tasks_context_var.set(delay_tasks)
+    yield
+    delay_tasks_context_var.reset(token)
+
+
+@contextlib.contextmanager
+def delay_tasks_context():
+    # noinspection PyTypeChecker
+    delay_tasks = delay_tasks_context_var.get()
+    yield delay_tasks
+
+
 worker_id_context_var = contextvars.ContextVar('worker_id_context_var', default=None)
 
 
 @contextlib.contextmanager
 def worker_id_provider(worker_id: str):
     # noinspection PyTypeChecker
     token = worker_id_context_var.set(worker_id)
```

### Comparing `eventix-0.5.0/eventix/exceptions/__init__.py` & `eventix-0.8.0/eventix/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `eventix-0.5.0/eventix/functions/core.py` & `eventix-0.8.0/eventix/functions/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 import functools
 import logging
 from inspect import signature
 from typing import Callable, Dict, Any
 
 from pydantic import BaseModel
 
-from eventix.contexts import namespace_context
+from eventix.contexts import namespace_context, delay_tasks_context
 from eventix.functions.task_scheduler import TaskScheduler
 from eventix.pydantic.task import TaskModel
 
 log = logging.getLogger(__name__)
 
 
 class EventixTaskBase(object):
     pass
 
 
-
-def task(store_result: bool = True, unique_key_generator: Callable = None):
+def task(store_result: bool = True, unique_key_generator: Callable = None, retry: bool = True, max_retries: int | None = None, error_expires: int | None = None, result_expires: int | None = 604800):
     # parameters suggested:
     #
     # store_result: bool , wether to store or not to store results
     # unique_uid: ....  having a unique id, which leads to update the task if it is rescheduled.
 
     # retry: bool, wether to retry failed tasks
     # max_retry: int, maximum retries default 5 ... each retry doubles the time to wait, starting with 30 sec
@@ -53,19 +52,24 @@
                         cls = self.arg_spec_kwargs[kw]
                         if issubclass(cls, BaseModel):
                             arg = cls.parse_obj(arg)
                     new_kwargs[kw] = arg
                 return new_args, new_kwargs
 
             @functools.wraps(f)
-            def delay(self, *args, _priority: int | None = 0, **kwargs):
+            def delay(self, *args, _priority: int | None = 0, **kwargs) -> TaskModel:
                 # priority has to be negated, needed for fixing ascending sort order
                 tm = self.make_task_model(args, kwargs, priority=_priority * -1)
-                # log.debug(f"scheduling {self.func.__name__} info: {tm.json()}")
-                tm = TaskScheduler.schedule(tm)
+                with delay_tasks_context() as delay:
+                    if delay:
+                        tm = TaskScheduler.schedule(tm)
+                    else:
+                        self.run(*args, **kwargs)
+
+                # IDEA: It could be possible to run worker execute with generated task during tests
                 return tm
 
             @functools.wraps(f)
             def run(self, *args, **kwargs):
                 args, kwargs = self.restore_pydantic_instances(args, kwargs)
                 return self.func(*args, **kwargs)
 
@@ -73,14 +77,18 @@
                 with namespace_context() as namespace:
                     params = dict(
                         task=self.func_name,
                         args=args,
                         kwargs=kwargs,
                         priority=priority,
                         store_result=store_result,
+                        retry=retry,
+                        max_retries=max_retries,
+                        error_expires=error_expires,
+                        result_expires=result_expires,
                         namespace=kwargs['namespace'] if "namespace" in kwargs else namespace
                     )
 
                     if is_unique:
                         unique_key = unique_key_generator(*args, **kwargs)
                         params |= dict(unique_key=unique_key)
```

### Comparing `eventix-0.5.0/eventix/functions/errors.py` & `eventix-0.8.0/eventix/functions/errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import contextlib
 from typing import List, Type
 
 import pydash
 from fastapi import HTTPException
 
+import logging
+
+log = logging.getLogger(__name__)
 
 @contextlib.contextmanager
 def raise_errors(r, exceptions: List[Type[Exception]]):
     exceptions_by_class = {e.__name__: e for e in exceptions}
-    if r.status_code == 200:
+    if r.status_code < 399:
         yield r
     else:
-        json = r.json()
-        detail = pydash.get(json, 'detail', json)
-        error_class = pydash.get(detail, 'error_class')
-        payload = pydash.get(detail, 'error_payload', {})
-        if error_class in exceptions_by_class:
-            e = exceptions_by_class[error_class](**payload)
-            raise e
-        # backend errors
-        raise HTTPException(status_code=r.status_code, detail=detail)
+        try:
+            json = r.json()
+            detail = pydash.get(json, 'detail', json)
+            error_class = pydash.get(detail, 'error_class')
+            payload = pydash.get(detail, 'error_payload', {})
+
+            if error_class in exceptions_by_class:
+                e = exceptions_by_class[error_class](**payload)
+                raise e
+            # backend errors
+            raise HTTPException(status_code=r.status_code, detail=detail)
+
+        except Exception as e:
+            log.error(r.content)
+            raise HTTPException(status_code=r.status_code, detail=r.content)
```

### Comparing `eventix-0.5.0/eventix/functions/fastapi.py` & `eventix-0.8.0/eventix/functions/fastapi.py`

 * *Files identical despite different names*

### Comparing `eventix-0.5.0/eventix/functions/task.py` & `eventix-0.8.0/eventix/functions/task.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 from traceback import format_tb
-from typing import List, Any
+from typing import List, Any, Tuple
 
 from webexception.webexception import WebException
 
-from eventix.pydantic.task import TaskModel
+from eventix.pydantic.pagination import PaginationParametersModel
+from eventix.pydantic.task import TaskModel, task_model_status
 from pydantic_db_backend.backend import Backend
 from pydantic_db_backend.exceptions import RevisionConflict
 
 # post
 # already exists
 # still scheduled -> update
 
@@ -106,18 +107,49 @@
             Backend.put_instance(existing_task)
             log.info(f"Released task {existing_task.uid}")
             # noinspection PyTypeChecker
         except RevisionConflict as e:
             continue
 
 
+def task_clean_expired_tasks():
+    params = dict(
+        model=TaskModel,
+        skip=0,
+        limit=100,
+        query_filter=dict(
+            expires={
+                "$and": [
+                    {"$ne": None},
+                    {"$lt": utcnow()},
+                ]
+            }  # task expired
+        ),
+        # sort=[
+        #     {"priority": "asc"},
+        #     {"eta": "asc"}
+        # ]
+    )
+
+    while True:
+        # noinspection PyTypeChecker
+        existing_uids = Backend.get_uids(**params)
+
+        # repeat until we were able to take something or nothing is left.
+        if len(existing_uids) == 0:
+            break
+
+        for uid in existing_uids:
+            Backend.delete_uid(TaskModel, uid)
+            log.info(f"Removed expired task {uid}")
+
+
 def task_next_scheduled(worker_id: str, namespace: str, expires: int = 300) -> TaskModel | None:
     log.debug(f"[{worker_id}] Worker getting next scheduled task...")
 
-
     # looking up possible tasks in right order
     # take first one
     # try to set worker_id and expiration
 
     eta = utcnow().isoformat()  # eta has to be now or in the past
 
     query_filter = dict(
@@ -182,21 +214,40 @@
         task.worker_id = None
 
     else:
         task.status = "error"
         if task.error_expires is not None:
             task.expires = utcnow() + datetime.timedelta(seconds=task.error_expires)
 
-    task.worker_expires = None  # remove worker_expires for prevent cleanup
+    task.worker_expires = None  # removes worker_expires for cleanup prevention
 
 
 def task_set_result(task: TaskModel, result: Any):
     task.status = "done"
     if task.store_result:
         task.result = result
         if task.result_expires is not None:
             task.expires = utcnow() + datetime.timedelta(seconds=task.result_expires)
     else:
         task.expires = utcnow()
 
-    task.worker_expires = None  # remove worker_expires for prevent cleanup
+    task.worker_expires = None  # removes worker_expires for cleanup prevention
+
 
+def tasks_by_status(
+    status: task_model_status | None = None,
+    namespace: str | None = None,
+    pagination: PaginationParametersModel | None = None
+) -> Tuple[List[TaskModel], int]:
+    query_filter = {}
+    if status is not None:
+        query_filter["status"] = {"$eq": status}
+    if namespace is not None:
+        query_filter["namespace"] = {"$eq": namespace}
+    params = {
+        "query_filter": query_filter,
+        **pagination.dict(),
+    }
+    # noinspection PyTypeChecker
+    tasks, max_results = Backend.get_instances(TaskModel, **params, max_results=True)
+    tasks: List[TaskModel]
+    return tasks, max_results
```

### Comparing `eventix-0.5.0/eventix/functions/task_scheduler.py` & `eventix-0.8.0/eventix/functions/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `eventix-0.5.0/eventix/functions/task_worker.py` & `eventix-0.8.0/eventix/functions/task_worker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,94 @@
 from __future__ import annotations
 
 import importlib
 import logging
 import os
 import sys
 import time
-from typing import List
+from typing import List, Dict
 
 import dotenv
+import requests.exceptions
 from pydantic_db_backend.utils import utcnow
 
 from eventix.contexts import worker_id_context, namespace_provider
 from eventix.exceptions import TaskNotRegistered, backend_exceptions
 from eventix.functions.core import EventixTaskBase, namespace_context
 from eventix.functions.errors import raise_errors
 from eventix.functions.eventix_client import EventixClient
+from eventix.functions.schedule import schedule_set_next_schedule
 from eventix.functions.task import task_set_error, task_set_result
+from eventix.functions.tools import setup_logging
+from eventix.pydantic.schedule import Schedule
 from eventix.pydantic.task import TaskModel
 
 log = logging.getLogger(__name__)
 
 
 class TaskWorker(EventixClient):
     _wait_interval = 10
     _tasks = {}
-    namespace: str = None
+    _schedule: Dict[str, Schedule] = {}
 
-    @classmethod
-    def setup_logging(cls, without_time: bool = False, level: int = logging.INFO):
-        if without_time:
-            f = "[%(levelname)8s] %(message)s"
-        else:
-            f = "%(asctime)s [%(levelname)s] %(message)s"
-        logging.basicConfig(
-            level=level,
-            format=f,
-            handlers=[
-                logging.StreamHandler()
-            ]
-        )
+    namespace: str = None
+    schedule_enabled: bool = False
+    log_level: str = None
 
     @classmethod
     def config(cls, config: dict):
 
         base_url = os.environ.get("EVENTIX_URL", "")
         if base_url == "":
             log.error("No EVENTIX_URL set.")
             sys.exit()
 
         cls.set_base_url(base_url)
 
-        if "register_tasks" in config:
-            cls.register_tasks(config['register_tasks'])
+        cls.config_register_tasks(config)
 
         if "namespace" in config:
             cls.namespace = config['namespace']
 
         namespace = os.environ.get("EVENTIX_NAMESPACE", "")
         if namespace != "":
             cls.namespace = namespace
 
+        schedule_enabled = os.environ.get("EVENTIX_SCHEDULE_ENABLED", "false")
+        cls.schedule_enabled = schedule_enabled.lower() == "true"
+
+        cls.config_schedule(config)
+
+    @classmethod
+    def config_register_tasks(cls, config):
+        if "register_tasks" in config:
+            cls.register_tasks(config['register_tasks'])
+
+    @classmethod
+    def config_schedule(cls, config):
+        if "schedule" in config:
+            for entry in config['schedule']:
+                s = Schedule.parse_obj(entry)
+                if s.task not in cls._tasks:
+                    raise TaskNotRegistered(s.task)
+
+                schedule_set_next_schedule(s)
+                cls._schedule[s.uid] = s
+                log.info(f"Scheduled '{s.name}' on '{s.schedule}'")
+
+    @classmethod
+    def check_scheduled_tasks(cls):
+        log.debug(f"Check scheduled tasks...")
+        for s in cls._schedule.values():
+            if s.next_schedule <= utcnow():
+                # trigger task
+                # update schedule
+                log.debug(f"triggering scheduled task '{s.name}'")
+                cls._tasks[s.task].delay(*s.args, _priority=s.priority, **s.kwargs)
+                schedule_set_next_schedule(s)
 
     @classmethod
     def register_tasks(cls, paths=List[str]):
         log.info("registering tasks...")
         # noinspection PyTypeChecker
         for path in paths:
             try:
@@ -73,45 +98,57 @@
                     [getattr(imported_module, x) for x in dir(imported_module)]
                 ):
                     log.info(f"registered '{f.func_name}' from {path}")
                     cls._tasks[f.func_name] = f
             except ImportError as e:
                 print(e)
 
+    # with raise_errors(r):
+    #     return TaskModel.parse_raw(r.content)
+
     @classmethod
     def task_next_scheduled(cls) -> TaskModel | None:
         with namespace_context() as namespace:
             with worker_id_context() as worker_id:
                 params = dict(
                     worker_id=worker_id,
                     namespace=namespace
                 )
-                r = cls.interface.get(f'/task/next_scheduled', params=params)
-                if r.status_code == 200:
-                    tm = TaskModel.parse_raw(r.content)
-                    return tm
-                else:
+                r = cls.interface.get(f'/tasks/next_scheduled', params=params)
+                try:
+                    with raise_errors(r, backend_exceptions):
+                        if r.status_code == 200:
+                            tm = TaskModel.parse_raw(r.content)
+                            return tm
+                        if r.status_code == 204:
+                            return None
+                except Exception as e:
+                    log.error("Upstream server error:")
+                    log.exception(str(e))
                     return None
-
-    # with raise_errors(r):
-    #     return TaskModel.parse_raw(r.content)
-
     @classmethod
-    def listen(cls, endless=True):
+    def listen(cls, endless=True, schedule_enabled: bool = False):
+        log.info(f"Schedule {'enabled' if schedule_enabled else 'disabled'}")
         log.info("Start listening...")
         while True:
-            log.info("Looking for tasks...")
-            t = cls.task_next_scheduled()
-            if t is not None:
-                cls.execute_task(t)
-            else:
-                log.info(f"Nothing to do... waiting {cls._wait_interval}s")
-                if not endless:
-                    return
-                time.sleep(cls._wait_interval)
+            try:
+                if schedule_enabled:
+                    cls.check_scheduled_tasks()
+                log.debug("Looking for tasks...")
+                t = cls.task_next_scheduled()
+                if t is not None:
+                    cls.execute_task(t)
+                else:
+                    log.info(f"Nothing to do... waiting {cls._wait_interval}s")
+                    if not endless:
+                        return
+                    time.sleep(cls._wait_interval)
+            except requests.exceptions.ConnectionError as e:
+                log.error(f"Upstream Eventix server {cls.interface.base_url} not reachable.")
+                time.sleep(5)
 
     @classmethod
     def execute_task(cls, task: TaskModel):
         try:
             log.info(f"Executing task: {task.task} uid: {task.uid} ...")
 
             if task.task not in cls._tasks:
@@ -161,15 +198,21 @@
         return None
 
     @classmethod
     def load_env(cls):
         dotenv.load_dotenv(".env.local")
 
     def __init__(self, config: dict) -> None:
-        self.setup_logging()
         self.load_env()
+        self.init_logging()
         self.config(config)
 
-    def start(self, endless: bool = True):
+    def init_logging(self):
+        self.log_level = os.environ.get("EVENTIX_WORKER_LOG_LEVEL", "INFO")
+        urllib3_logger = logging.getLogger("urllib3.connectionpool")
+        urllib3_logger.setLevel(logging.INFO)
+        setup_logging(level=self.log_level.upper(), module=False, prefix="[WORKER]")
+
+    def start(self, endless: bool | None = True):
         log.info(f"Using namespace: {self.namespace}")
         with namespace_provider(self.namespace):
-            self.listen(endless)
+            self.listen(endless, self.schedule_enabled)
```

### Comparing `eventix-0.5.0/eventix/pydantic/task.py` & `eventix-0.8.0/eventix/pydantic/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import datetime
-from typing import Any, Dict, Tuple, Self, Type, Literal
+from typing import Any, Dict, Self, Literal
 
 from pydantic import Field
-from webexception.webexception import WebException
 
 from pydantic_db_backend.backend import BackendModel
-from pydantic_db_backend.utils import utcnow, _uid
+from pydantic_db_backend.indexes import SortingIndex, AggregationIndex
+from pydantic_db_backend.utils import utcnow
 
 task_model_status = Literal["scheduled", "processing", "done", "error", "retry"]
 
 
 class TaskModel(BackendModel):
     unique_key: str | None = None
     eta: datetime.datetime | None = Field(default_factory=utcnow)
@@ -46,15 +46,16 @@
 
     def unique_update_from(self, task: Self):
         self.eta = min([task.eta, self.eta])
         self.priority = min([task.priority, self.priority])
 
     class Config:
         backend_indexes = [
-            ("priority_eta", [{"priority": "asc"}, {"eta": "asc"}]),
+            SortingIndex("priority_eta", [{"priority": "asc"}, {"eta": "asc"}]),
+            AggregationIndex("status_sum", {"status": "_sum"})
         ]
 
     # sort order
     # priority-, eta-
 
     # 9    0
     # 9    1
```

### Comparing `eventix-0.5.0/pyproject.toml` & `eventix-0.8.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 [tool.poetry]
 name = "eventix"
-version = "0.5.0"
+version = "0.8.0"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.99.1"
-uvicorn = "^0.22.0"
+uvicorn = "^0.21.0"
 python-dotenv = "^0.15.0"
 pydash = "*"
-pydantic-db-backend = {version = "^0.4.3", extras = ["couchdb"]}
+pydantic-db-backend = {version = "^0.6.0", extras = ["couchdb"]}
 psutil = "^5.9.5"
 requests = "^2.31.0"
 toml = "^0.10.2"
 webexception = "^1.0.2"
 croniter = "^1.4.1"
+supervisor = "^4.2.5"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 httpx = "^0.24.1"
 freezegun = "^1.2.2"
 coverage = "^7.2.7"
 pytest-mock = "^3.11.1"
+semantic-version = "^2.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q -s -v"
 testpaths = [
     "tests",
 ]
 log_cli = true
 log_cli_level = "DEBUG"
 #log_cli_level = "INFO"
-#log_cli_format = "[%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
-log_cli_format = "[%(name)s][%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
+log_cli_format = "[%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
+#log_cli_format = "[%(name)s][%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
```

### Comparing `eventix-0.5.0/PKG-INFO` & `eventix-0.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: eventix
-Version: 0.5.0
+Version: 0.8.0
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: croniter (>=1.4.1,<2.0.0)
 Requires-Dist: fastapi (>=0.99.1,<0.100.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
-Requires-Dist: pydantic-db-backend[couchdb] (>=0.4.3,<0.5.0)
+Requires-Dist: pydantic-db-backend[couchdb] (>=0.6.0,<0.7.0)
 Requires-Dist: pydash
 Requires-Dist: python-dotenv (>=0.15.0,<0.16.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: supervisor (>=4.2.5,<5.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
+Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
 Requires-Dist: webexception (>=1.0.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Eventix
 
 ## Database
```

