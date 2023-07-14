# Comparing `tmp/unidist-0.4.0.tar.gz` & `tmp/unidist-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unidist-0.4.0.tar", last modified: Fri Jul  7 15:55:14 2023, max compression
+gzip compressed data, was "unidist-0.4.1.tar", last modified: Fri Jul 14 07:52:17 2023, max compression
```

## Comparing `unidist-0.4.0.tar` & `unidist-0.4.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      687 2023-07-07 15:47:13.000000 unidist-0.4.0/AUTHORS
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    11357 2023-07-07 15:47:13.000000 unidist-0.4.0/LICENSE
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       50 2023-07-07 15:47:13.000000 unidist-0.4.0/MANIFEST.in
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6682 2023-07-07 15:55:14.834100 unidist-0.4.0/PKG-INFO
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6329 2023-07-07 15:47:13.000000 unidist-0.4.0/README.md
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      354 2023-07-07 15:55:14.834100 unidist-0.4.0/setup.cfg
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1185 2023-07-07 15:47:13.000000 unidist-0.4.0/setup.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      559 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      497 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/_version.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6912 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/api.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      916 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/__init__.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/backends/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      172 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/__init__.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/backends/common/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      232 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/common/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2337 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/common/envvars.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/backends/dask/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      323 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/dask/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      758 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/dask/envvars.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/backends/mpi/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      379 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/mpi/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1331 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/mpi/envvars.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/backends/ray/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      434 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/ray/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1131 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/ray/envvars.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6612 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/parameter.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/core/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      107 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/__init__.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       80 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/__init__.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/common/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      122 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/common/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      909 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/common/data_id.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1121 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/common/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/dask/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      115 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/dask/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6692 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/dask/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5526 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/dask/backend.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3460 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/dask/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1078 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/dask/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/mpi/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      114 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5692 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4668 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/backend.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/mpi/core/
--rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)      408 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1965 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/async_operations.py
--rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     9383 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/common.py
--rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)    26560 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/communication.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/mpi/core/controller/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      533 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6091 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    16962 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/api.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     7885 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/common.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5563 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/garbage_collector.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     7918 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/object_store.py
--rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     7224 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/monitor.py
--rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     8921 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/serialization.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/mpi/core/worker/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      142 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/worker/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     9329 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/worker/loop.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6340 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/worker/object_store.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    11488 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/worker/request_store.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    15638 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/worker/task_store.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3153 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      275 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/pymp/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      133 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4336 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4815 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/backend.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/pymp/core/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      305 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/core/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4701 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/core/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4067 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/core/api.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4268 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/core/object_store.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6900 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/core/process_manager.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3004 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      506 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/pyseq/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      128 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4225 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4609 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/backend.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/pyseq/core/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      252 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/core/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3060 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/core/api.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2313 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/core/object_store.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2905 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      382 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/ray/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      114 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/ray/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5544 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/ray/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4616 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/ray/backend.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2742 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/ray/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4778 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/ray/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/base/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      112 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6620 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    10573 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/backend.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1255 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/common.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      384 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/object_ref.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3105 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3330 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/test/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       80 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4174 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/test_actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6039 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/test_async_actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2172 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/test_general.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2668 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/test_task.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2276 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist.egg-info/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6682 2023-07-07 15:55:14.000000 unidist-0.4.0/unidist.egg-info/PKG-INFO
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3428 2023-07-07 15:55:14.000000 unidist-0.4.0/unidist.egg-info/SOURCES.txt
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)        1 2023-07-07 15:55:14.000000 unidist-0.4.0/unidist.egg-info/dependency_links.txt
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      257 2023-07-07 15:55:14.000000 unidist-0.4.0/unidist.egg-info/requires.txt
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)        8 2023-07-07 15:55:14.000000 unidist-0.4.0/unidist.egg-info/top_level.txt
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    80049 2023-07-07 15:47:13.000000 unidist-0.4.0/versioneer.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      687 2023-07-14 07:42:21.000000 unidist-0.4.1/AUTHORS
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    11357 2023-07-14 07:42:21.000000 unidist-0.4.1/LICENSE
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       50 2023-07-14 07:42:21.000000 unidist-0.4.1/MANIFEST.in
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6697 2023-07-14 07:52:17.326372 unidist-0.4.1/PKG-INFO
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6344 2023-07-14 07:42:40.000000 unidist-0.4.1/README.md
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      354 2023-07-14 07:52:17.326372 unidist-0.4.1/setup.cfg
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1185 2023-07-14 07:42:21.000000 unidist-0.4.1/setup.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      559 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      497 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/_version.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6912 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/api.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.316372 unidist-0.4.1/unidist/config/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      916 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/config/__init__.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.316372 unidist-0.4.1/unidist/config/backends/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      172 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/config/backends/__init__.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.316372 unidist-0.4.1/unidist/config/backends/common/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      232 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/config/backends/common/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2337 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/config/backends/common/envvars.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.316372 unidist-0.4.1/unidist/config/backends/dask/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      323 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/config/backends/dask/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      758 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/config/backends/dask/envvars.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.316372 unidist-0.4.1/unidist/config/backends/mpi/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      379 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/config/backends/mpi/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1331 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/config/backends/mpi/envvars.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.316372 unidist-0.4.1/unidist/config/backends/ray/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      434 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/config/backends/ray/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1131 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/config/backends/ray/envvars.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6612 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/config/parameter.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.316372 unidist-0.4.1/unidist/core/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      107 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/__init__.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.316372 unidist-0.4.1/unidist/core/backends/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       80 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/__init__.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.316372 unidist-0.4.1/unidist/core/backends/common/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      122 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/common/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      909 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/common/data_id.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1121 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/common/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/core/backends/dask/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      115 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/dask/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6692 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/dask/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5526 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/dask/backend.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3460 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/dask/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1078 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/dask/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/core/backends/mpi/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      114 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5692 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4668 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/backend.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/core/backends/mpi/core/
+-rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)      408 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1965 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/async_operations.py
+-rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     9383 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/common.py
+-rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)    24758 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/communication.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/core/backends/mpi/core/controller/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      533 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/controller/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6091 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/controller/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    16962 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/controller/api.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     7885 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/controller/common.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5563 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/controller/garbage_collector.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     7918 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/controller/object_store.py
+-rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     7224 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/monitor.py
+-rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     8921 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/serialization.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/core/backends/mpi/core/worker/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      142 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/worker/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     8619 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/worker/loop.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6340 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/worker/object_store.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    11488 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/worker/request_store.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    15638 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/core/worker/task_store.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3153 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      275 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/mpi/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/core/backends/pymp/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      133 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pymp/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4336 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pymp/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4815 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pymp/backend.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/core/backends/pymp/core/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      305 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pymp/core/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4701 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pymp/core/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4067 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pymp/core/api.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4268 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pymp/core/object_store.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6900 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pymp/core/process_manager.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3004 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pymp/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      506 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pymp/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/core/backends/pyseq/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      128 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pyseq/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4225 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pyseq/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4609 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pyseq/backend.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/core/backends/pyseq/core/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      252 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pyseq/core/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3060 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pyseq/core/api.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2313 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pyseq/core/object_store.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2905 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pyseq/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      382 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/pyseq/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/core/backends/ray/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      114 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/ray/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5544 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/ray/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4616 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/ray/backend.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2742 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/ray/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4778 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/backends/ray/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/core/base/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      112 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/base/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6620 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/base/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    10573 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/base/backend.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1255 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/base/common.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      384 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/base/object_ref.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3105 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/base/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3330 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/core/base/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.326372 unidist-0.4.1/unidist/test/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       80 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/test/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4174 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/test/test_actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6039 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/test/test_async_actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2172 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/test/test_general.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2668 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/test/test_task.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2276 2023-07-14 07:42:21.000000 unidist-0.4.1/unidist/test/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-14 07:52:17.316372 unidist-0.4.1/unidist.egg-info/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6697 2023-07-14 07:52:17.000000 unidist-0.4.1/unidist.egg-info/PKG-INFO
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3428 2023-07-14 07:52:17.000000 unidist-0.4.1/unidist.egg-info/SOURCES.txt
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)        1 2023-07-14 07:52:17.000000 unidist-0.4.1/unidist.egg-info/dependency_links.txt
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      257 2023-07-14 07:52:17.000000 unidist-0.4.1/unidist.egg-info/requires.txt
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)        8 2023-07-14 07:52:17.000000 unidist-0.4.1/unidist.egg-info/top_level.txt
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    80049 2023-07-14 07:42:21.000000 unidist-0.4.1/versioneer.py
```

### Comparing `unidist-0.4.0/AUTHORS` & `unidist-0.4.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/LICENSE` & `unidist-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/PKG-INFO` & `unidist-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidist
-Version: 0.4.0
+Version: 0.4.1
 Summary: Unified Distributed Execution
 Home-page: https://github.com/modin-project/unidist
 License: Apache-2.0
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 Provides-Extra: ray
 Provides-Extra: dask
@@ -16,16 +16,16 @@
 <p align="center">
     <a href="https://unidist.readthedocs.io"><img alt="" src="https://github.com/modin-project/unidist/blob/d17f0da551846277c9d56a7f5e7d8f244c09d660/docs/img/unidist-logo-simple-628x128.png?raw=true"></a>
 </p>
 <h2 align="center">Unified Distributed Execution</h2>
 
 <p align="center">
 <a href="https://github.com/modin-project/unidist/actions"><img src="https://github.com/modin-project/unidist/workflows/master/badge.svg" align="center"></a>
-<a href="https://unidist.readthedocs.io/en/latest/?badge=latest"><img alt="" src="https://readthedocs.org/projects/unidist/badge/?version=latest" align="center"></a>
-<a href="https://pypi.org/project/unidist/"><img src="https://badge.fury.io/py/unidist.svg" alt="PyPI version" align="center"></a>
+<a href="https://unidist.readthedocs.io/en/0.4.1/?badge=0.4.1"><img alt="" src="https://readthedocs.org/projects/unidist/badge/?version=0.4.1" align="center"></a>
+<a href="https://pypi.org/project/unidist/0.4.1/"><img src="https://img.shields.io/badge/pypi-0.4.1-blue.svg" alt="PyPI version" align="center"></a>
 </p>
 
 ### What is unidist?
 
 unidist is a framework that is intended to provide the unified API for distributed execution by supporting various performant execution backends. At the moment the following backends are supported under the hood:
 
 * [MPI](https://www.mpi-forum.org/)
```

### Comparing `unidist-0.4.0/README.md` & `unidist-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <p align="center">
     <a href="https://unidist.readthedocs.io"><img alt="" src="https://github.com/modin-project/unidist/blob/d17f0da551846277c9d56a7f5e7d8f244c09d660/docs/img/unidist-logo-simple-628x128.png?raw=true"></a>
 </p>
 <h2 align="center">Unified Distributed Execution</h2>
 
 <p align="center">
 <a href="https://github.com/modin-project/unidist/actions"><img src="https://github.com/modin-project/unidist/workflows/master/badge.svg" align="center"></a>
-<a href="https://unidist.readthedocs.io/en/latest/?badge=latest"><img alt="" src="https://readthedocs.org/projects/unidist/badge/?version=latest" align="center"></a>
-<a href="https://pypi.org/project/unidist/"><img src="https://badge.fury.io/py/unidist.svg" alt="PyPI version" align="center"></a>
+<a href="https://unidist.readthedocs.io/en/0.4.1/?badge=0.4.1"><img alt="" src="https://readthedocs.org/projects/unidist/badge/?version=0.4.1" align="center"></a>
+<a href="https://pypi.org/project/unidist/0.4.1/"><img src="https://img.shields.io/badge/pypi-0.4.1-blue.svg" alt="PyPI version" align="center"></a>
 </p>
 
 ### What is unidist?
 
 unidist is a framework that is intended to provide the unified API for distributed execution by supporting various performant execution backends. At the moment the following backends are supported under the hood:
 
 * [MPI](https://www.mpi-forum.org/)
```

### Comparing `unidist-0.4.0/setup.py` & `unidist-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/__init__.py` & `unidist-0.4.1/unidist/__init__.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/api.py` & `unidist-0.4.1/unidist/api.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/config/__init__.py` & `unidist-0.4.1/unidist/config/__init__.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/config/backends/common/envvars.py` & `unidist-0.4.1/unidist/config/backends/common/envvars.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/config/backends/dask/envvars.py` & `unidist-0.4.1/unidist/config/backends/dask/envvars.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/config/backends/mpi/envvars.py` & `unidist-0.4.1/unidist/config/backends/mpi/envvars.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/config/backends/ray/envvars.py` & `unidist-0.4.1/unidist/config/backends/ray/envvars.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/config/parameter.py` & `unidist-0.4.1/unidist/config/parameter.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/common/data_id.py` & `unidist-0.4.1/unidist/core/backends/common/data_id.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/common/utils.py` & `unidist-0.4.1/unidist/core/backends/common/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/dask/actor.py` & `unidist-0.4.1/unidist/core/backends/dask/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/dask/backend.py` & `unidist-0.4.1/unidist/core/backends/dask/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/dask/remote_function.py` & `unidist-0.4.1/unidist/core/backends/dask/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/dask/utils.py` & `unidist-0.4.1/unidist/core/backends/dask/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/actor.py` & `unidist-0.4.1/unidist/core/backends/mpi/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/backend.py` & `unidist-0.4.1/unidist/core/backends/mpi/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/async_operations.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/async_operations.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/common.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/common.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/communication.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/communication.py`

 * *Files 18% similar despite different names*

```diff
@@ -283,52 +283,36 @@
     source = status.source
     tag = status.tag
     op_type = comm.recv(buf=None, source=source, tag=tag, status=status)
     log_operation(op_type, status)
     return op_type, status.Get_source()
 
 
-def mpi_recv_object(comm, source_rank, cancel_recv=False):
+def mpi_recv_object(comm, source_rank):
     """
     Receive an object of a standard Python data type.
 
     Parameters
     ----------
     comm : object
         MPI communicator object.
     source_rank : int
         Source MPI process to receive data from.
-    cancel_recv : bool, default: False
-        Whether to cancel an incoming message or not.
-        This can happen when a worker is getting to shutdown so
-        there is no need to receive the message.
 
     Returns
     -------
-    object or None
-        Received data object from another MPI process or
-        ``None`` if the message was cancelled.
+    object
+        Received data object from another MPI process.
 
     Notes
     -----
     * De-serialization is a simple pickle.load in this case.
     * The special tag is used for this communication, namely, ``common.MPITag.OBJECT``.
     """
-    backoff = MpiBackoff.get()
-    status = MPI.Status()
-    tag = common.MPITag.OBJECT
-    while not comm.Iprobe(source=source_rank, tag=tag):
-        time.sleep(backoff)
-    request = comm.irecv(source=source_rank, tag=tag)
-    if cancel_recv:
-        request.cancel()
-    data = request.wait(status=status)
-    if status.Is_cancelled():
-        data = None
-    return data
+    return comm.recv(source=source_rank, tag=common.MPITag.OBJECT)
 
 
 def mpi_send_buffer(comm, buffer_size, buffer, dest_rank):
     """
     Send buffer object to another MPI rank in a blocking way.
 
     Parameters
@@ -625,81 +609,51 @@
     handlers.extend(
         _isend_complex_data_impl(comm, s_data, raw_buffers, buffer_count, dest_rank)
     )
 
     return handlers, s_data, raw_buffers, buffer_count
 
 
-def recv_complex_data(comm, source_rank, cancel_recv=False):
+def recv_complex_data(comm, source_rank):
     """
     Receive the data that may consist of different user provided complex types, lambdas and buffers.
 
     The data is de-serialized from received buffer.
 
     Parameters
     ----------
     comm : object
         MPI communicator object.
     source_rank : int
         Source MPI process to receive data from.
-    cancel_recv : bool, default: False
-        Whether to cancel an incoming message or not.
-        This can happen when a worker is getting to shutdown so
-        there is no need to receive the message.
 
     Returns
     -------
     object
-        Received data object from another MPI process or
-        ``None`` if the message was cancelled.
+        Received data object from another MPI process.
 
     Notes
     -----
     * The special tags are used for this communication, namely,
     ``common.MPITag.OBJECT`` and ``common.MPITag.BUFFER``.
     """
-    # Recv main message pack buffer.
-    # First MPI call uses busy wait loop to remove possible contention
-    # in a long running data receive operations.
-    backoff = MpiBackoff.get()
-    status = MPI.Status()
-    info = mpi_busy_wait_recv(comm, source_rank)
+    info = comm.recv(source=source_rank, tag=common.MPITag.OBJECT)
     msgpack_buffer = bytearray(info["s_data_len"])
     buffer_count = info["buffer_count"]
     raw_buffers = list(map(bytearray, info["raw_buffers_len"]))
-    cancelled_requests = []
     with pkl5._bigmpi as bigmpi:
-        while not comm.Iprobe(source=source_rank, tag=common.MPITag.BUFFER):
-            time.sleep(backoff)
-        request = comm.Irecv(
-            bigmpi(msgpack_buffer), source=source_rank, tag=common.MPITag.BUFFER
-        )
-        if cancel_recv:
-            request.Cancel()
-        request.Wait(status=status)
-        cancelled_requests.append(status.Is_cancelled())
+        comm.Recv(bigmpi(msgpack_buffer), source=source_rank, tag=common.MPITag.BUFFER)
         for rbuf in raw_buffers:
-            while not comm.Iprobe(source=source_rank, tag=common.MPITag.BUFFER):
-                time.sleep(backoff)
-            request = comm.Irecv(
-                bigmpi(rbuf), source=source_rank, tag=common.MPITag.BUFFER
-            )
-            if cancel_recv:
-                request.Cancel()
-            request.Wait(status=status)
-            cancelled_requests.append(status.Is_cancelled())
-
-    if any(cancelled for cancelled in cancelled_requests):
-        return None
-    else:
-        # Set the necessary metadata for unpacking
-        deserializer = ComplexDataSerializer(raw_buffers, buffer_count)
+            comm.Recv(bigmpi(rbuf), source=source_rank, tag=common.MPITag.BUFFER)
+
+    # Set the necessary metadata for unpacking
+    deserializer = ComplexDataSerializer(raw_buffers, buffer_count)
 
-        # Start unpacking
-        return deserializer.deserialize(msgpack_buffer)
+    # Start unpacking
+    return deserializer.deserialize(msgpack_buffer)
 
 
 # ---------- #
 # Public API #
 # ---------- #
```

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/controller/__init__.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/controller/actor.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/controller/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/controller/api.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/controller/api.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/controller/common.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/controller/common.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/controller/garbage_collector.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/controller/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/controller/object_store.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/controller/object_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/monitor.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/monitor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/serialization.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/serialization.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/worker/loop.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/worker/loop.py`

 * *Files 20% similar despite different names*

```diff
@@ -96,48 +96,35 @@
         operation_type, source_rank = await async_wrap(
             communication.mpi_recv_operation
         )(mpi_state.comm)
         w_logger.debug("common.Operation processing - {}".format(operation_type))
 
         # Proceed the request
         if operation_type == common.Operation.EXECUTE:
-            request = communication.recv_complex_data(
-                mpi_state.comm,
-                source_rank,
-                cancel_recv=ready_to_shutdown_posted,
-            )
-
-            if request is not None and not ready_to_shutdown_posted:
+            request = communication.recv_complex_data(mpi_state.comm, source_rank)
+            if not ready_to_shutdown_posted:
                 # Execute the task if possible
                 pending_request = task_store.process_task_request(request)
                 if pending_request:
                     task_store.put(pending_request)
                 else:
                     # Check pending requests. Maybe some data became available.
                     task_store.check_pending_tasks()
 
         elif operation_type == common.Operation.GET:
-            request = communication.mpi_recv_object(
-                mpi_state.comm,
-                source_rank,
-                cancel_recv=ready_to_shutdown_posted,
-            )
-            if request is not None and not ready_to_shutdown_posted:
+            request = communication.mpi_recv_object(mpi_state.comm, source_rank)
+            if not ready_to_shutdown_posted:
                 request["id"] = object_store.get_unique_data_id(request["id"])
                 request_store.process_get_request(
                     request["source"], request["id"], request["is_blocking_op"]
                 )
 
         elif operation_type == common.Operation.PUT_DATA:
-            request = communication.recv_complex_data(
-                mpi_state.comm,
-                source_rank,
-                cancel_recv=ready_to_shutdown_posted,
-            )
-            if request is not None and not ready_to_shutdown_posted:
+            request = communication.recv_complex_data(mpi_state.comm, source_rank)
+            if not ready_to_shutdown_posted:
                 w_logger.debug(
                     "PUT (RECV) {} id from {} rank".format(
                         request["id"]._id, source_rank
                     )
                 )
                 request["id"] = object_store.get_unique_data_id(request["id"])
                 object_store.put(request["id"], request["data"])
@@ -147,53 +134,44 @@
 
                 # Check pending requests. Maybe some data became available.
                 task_store.check_pending_tasks()
                 # Check pending actor requests also.
                 task_store.check_pending_actor_tasks()
 
         elif operation_type == common.Operation.PUT_OWNER:
-            request = communication.mpi_recv_object(
-                mpi_state.comm,
-                source_rank,
-                cancel_recv=ready_to_shutdown_posted,
-            )
-            if request is not None and not ready_to_shutdown_posted:
+            request = communication.mpi_recv_object(mpi_state.comm, source_rank)
+            if not ready_to_shutdown_posted:
                 request["id"] = object_store.get_unique_data_id(request["id"])
                 object_store.put_data_owner(request["id"], request["owner"])
 
                 w_logger.debug(
                     "PUT_OWNER {} id is owned by {} rank".format(
                         request["id"]._id, request["owner"]
                     )
                 )
 
         elif operation_type == common.Operation.WAIT:
             request = communication.mpi_recv_object(mpi_state.comm, source_rank)
-            if request is not None and not ready_to_shutdown_posted:
+            if not ready_to_shutdown_posted:
                 w_logger.debug("WAIT for {} id".format(request["id"]._id))
                 request["id"] = object_store.get_unique_data_id(request["id"])
                 request_store.process_wait_request(request["id"])
 
         elif operation_type == common.Operation.ACTOR_CREATE:
-            request = communication.recv_complex_data(
-                mpi_state.comm, source_rank, cancel_recv=ready_to_shutdown_posted
-            )
-            if request is not None and not ready_to_shutdown_posted:
+            request = communication.recv_complex_data(mpi_state.comm, source_rank)
+            if not ready_to_shutdown_posted:
                 cls = request["class"]
                 args = request["args"]
                 kwargs = request["kwargs"]
                 handler = request["handler"]
                 actor_map[handler] = cls(*args, **kwargs)
 
         elif operation_type == common.Operation.ACTOR_EXECUTE:
-            request = communication.recv_complex_data(
-                mpi_state.comm, source_rank, cancel_recv=ready_to_shutdown_posted
-            )
-
-            if request is not None and not ready_to_shutdown_posted:
+            request = communication.recv_complex_data(mpi_state.comm, source_rank)
+            if not ready_to_shutdown_posted:
                 # Prepare the data
                 method_name = request["task"]
                 handler = request["handler"]
                 actor_method = getattr(actor_map[handler], method_name)
                 request["task"] = actor_method
 
                 # Execute the actor task if possible
@@ -211,22 +189,22 @@
             object_store.clear(cleanup_list)
 
         elif operation_type == common.Operation.CANCEL:
             task_store.clear_pending_tasks()
             task_store.clear_pending_actor_tasks()
             request_store.clear_get_requests()
             request_store.clear_wait_requests()
+            async_operations.finish()
             communication.mpi_send_operation(
                 mpi_state.comm,
                 common.Operation.READY_TO_SHUTDOWN,
                 communication.MPIRank.MONITOR,
             )
             ready_to_shutdown_posted = True
         elif operation_type == common.Operation.SHUTDOWN and ready_to_shutdown_posted:
-            async_operations.finish()
             w_logger.debug("Exit worker event loop")
             if not MPI.Is_finalized():
                 MPI.Finalize()
             break  # leave event loop and shutdown worker
         else:
             raise ValueError(f"Unsupported operation: {operation_type}")
```

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/worker/object_store.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/worker/object_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/worker/request_store.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/worker/request_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/core/worker/task_store.py` & `unidist-0.4.1/unidist/core/backends/mpi/core/worker/task_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/mpi/remote_function.py` & `unidist-0.4.1/unidist/core/backends/mpi/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pymp/actor.py` & `unidist-0.4.1/unidist/core/backends/pymp/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pymp/backend.py` & `unidist-0.4.1/unidist/core/backends/pymp/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pymp/core/actor.py` & `unidist-0.4.1/unidist/core/backends/pymp/core/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pymp/core/api.py` & `unidist-0.4.1/unidist/core/backends/pymp/core/api.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pymp/core/object_store.py` & `unidist-0.4.1/unidist/core/backends/pymp/core/object_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pymp/core/process_manager.py` & `unidist-0.4.1/unidist/core/backends/pymp/core/process_manager.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pymp/remote_function.py` & `unidist-0.4.1/unidist/core/backends/pymp/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pyseq/actor.py` & `unidist-0.4.1/unidist/core/backends/pyseq/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pyseq/backend.py` & `unidist-0.4.1/unidist/core/backends/pyseq/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pyseq/core/api.py` & `unidist-0.4.1/unidist/core/backends/pyseq/core/api.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pyseq/core/object_store.py` & `unidist-0.4.1/unidist/core/backends/pyseq/core/object_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/pyseq/remote_function.py` & `unidist-0.4.1/unidist/core/backends/pyseq/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/ray/actor.py` & `unidist-0.4.1/unidist/core/backends/ray/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/ray/backend.py` & `unidist-0.4.1/unidist/core/backends/ray/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/ray/remote_function.py` & `unidist-0.4.1/unidist/core/backends/ray/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/backends/ray/utils.py` & `unidist-0.4.1/unidist/core/backends/ray/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/base/actor.py` & `unidist-0.4.1/unidist/core/base/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/base/backend.py` & `unidist-0.4.1/unidist/core/base/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/base/common.py` & `unidist-0.4.1/unidist/core/base/common.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/base/remote_function.py` & `unidist-0.4.1/unidist/core/base/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/core/base/utils.py` & `unidist-0.4.1/unidist/core/base/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/test/test_actor.py` & `unidist-0.4.1/unidist/test/test_actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/test/test_async_actor.py` & `unidist-0.4.1/unidist/test/test_async_actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/test/test_general.py` & `unidist-0.4.1/unidist/test/test_general.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/test/test_task.py` & `unidist-0.4.1/unidist/test/test_task.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist/test/utils.py` & `unidist-0.4.1/unidist/test/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/unidist.egg-info/PKG-INFO` & `unidist-0.4.1/unidist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidist
-Version: 0.4.0
+Version: 0.4.1
 Summary: Unified Distributed Execution
 Home-page: https://github.com/modin-project/unidist
 License: Apache-2.0
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 Provides-Extra: ray
 Provides-Extra: dask
@@ -16,16 +16,16 @@
 <p align="center">
     <a href="https://unidist.readthedocs.io"><img alt="" src="https://github.com/modin-project/unidist/blob/d17f0da551846277c9d56a7f5e7d8f244c09d660/docs/img/unidist-logo-simple-628x128.png?raw=true"></a>
 </p>
 <h2 align="center">Unified Distributed Execution</h2>
 
 <p align="center">
 <a href="https://github.com/modin-project/unidist/actions"><img src="https://github.com/modin-project/unidist/workflows/master/badge.svg" align="center"></a>
-<a href="https://unidist.readthedocs.io/en/latest/?badge=latest"><img alt="" src="https://readthedocs.org/projects/unidist/badge/?version=latest" align="center"></a>
-<a href="https://pypi.org/project/unidist/"><img src="https://badge.fury.io/py/unidist.svg" alt="PyPI version" align="center"></a>
+<a href="https://unidist.readthedocs.io/en/0.4.1/?badge=0.4.1"><img alt="" src="https://readthedocs.org/projects/unidist/badge/?version=0.4.1" align="center"></a>
+<a href="https://pypi.org/project/unidist/0.4.1/"><img src="https://img.shields.io/badge/pypi-0.4.1-blue.svg" alt="PyPI version" align="center"></a>
 </p>
 
 ### What is unidist?
 
 unidist is a framework that is intended to provide the unified API for distributed execution by supporting various performant execution backends. At the moment the following backends are supported under the hood:
 
 * [MPI](https://www.mpi-forum.org/)
```

### Comparing `unidist-0.4.0/unidist.egg-info/SOURCES.txt` & `unidist-0.4.1/unidist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unidist-0.4.0/versioneer.py` & `unidist-0.4.1/versioneer.py`

 * *Files identical despite different names*

