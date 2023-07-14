# Comparing `tmp/bullmq-1.6.1.tar.gz` & `tmp/bullmq-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-1.6.1.tar", last modified: Mon Jul 10 23:38:04 2023, max compression
+gzip compressed data, was "bullmq-1.7.0.tar", last modified: Fri Jul 14 17:30:11 2023, max compression
```

## Comparing `bullmq-1.6.1.tar` & `bullmq-1.7.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.380847 bullmq-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-10 23:38:04.376846 bullmq-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-10 23:36:30.000000 bullmq-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.368847 bullmq-1.6.1/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-10 23:38:01.000000 bullmq-1.6.1/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.376846 bullmq-1.6.1/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/addJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/changePriority-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveToActive-10.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveToFinished-13.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/pause-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/promote-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/retryJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-10 23:37:27.000000 bullmq-1.6.1/bullmq/commands/updateProgress-2.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.376846 bullmq-1.6.1/bullmq/custom_errors/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/custom_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/custom_errors/waiting_children_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.376846 bullmq-1.6.1/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-10 23:36:30.000000 bullmq-1.6.1/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:04.368847 bullmq-1.6.1/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-10 23:38:04.000000 bullmq-1.6.1/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-10 23:38:04.000000 bullmq-1.6.1/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 23:38:04.000000 bullmq-1.6.1/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 23:38:04.000000 bullmq-1.6.1/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 23:38:04.000000 bullmq-1.6.1/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-10 23:38:01.000000 bullmq-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:38:04.380847 bullmq-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-10 23:36:30.000000 bullmq-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.935833 bullmq-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-14 17:30:11.935833 bullmq-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-14 17:28:40.000000 bullmq-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.931832 bullmq-1.7.0/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-14 17:30:08.000000 bullmq-1.7.0/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.935833 bullmq-1.7.0/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/addJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/changePriority-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveToActive-10.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveToFinished-13.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/pause-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/promote-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/retryJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/updateProgress-2.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.935833 bullmq-1.7.0/bullmq/custom_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/custom_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/custom_errors/waiting_children_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.935833 bullmq-1.7.0/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.931832 bullmq-1.7.0/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-14 17:30:11.000000 bullmq-1.7.0/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-14 17:30:11.000000 bullmq-1.7.0/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:30:11.000000 bullmq-1.7.0/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 17:30:11.000000 bullmq-1.7.0/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 17:30:11.000000 bullmq-1.7.0/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-14 17:30:08.000000 bullmq-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:30:11.935833 bullmq-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-14 17:28:40.000000 bullmq-1.7.0/setup.py
```

### Comparing `bullmq-1.6.1/PKG-INFO` & `bullmq-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.6.1
+Version: 1.7.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.6.1/README.md` & `bullmq-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/backoffs.py` & `bullmq-1.7.0/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/addJob-9.lua` & `bullmq-1.7.0/bullmq/commands/addJob-9.lua`

 * *Files 2% similar despite different names*

```diff
@@ -137,23 +137,26 @@
     local priority = tonumber(jobAttributes[1]) or 0
     local delay = tonumber(jobAttributes[2]) or 0
     if delay > 0 then
       local delayedTimestamp = tonumber(timestamp) + delay 
       local score = delayedTimestamp * 0x1000
       local parentDelayedKey = parentQueueKey .. ":delayed" 
       rcall("ZADD", parentDelayedKey, score, parentId)
+      rcall("XADD", parentQueueKey .. ":events", "*", "event", "delayed", "jobId", parentId,
+        "delay", delayedTimestamp)
       addDelayMarkerIfNeeded(parentTarget, parentDelayedKey)
-    -- Standard or priority add
-    elseif priority == 0 then
-      rcall("RPUSH", parentTarget, parentId)
     else
-      addJobWithPriority(parentWaitKey, parentQueueKey .. ":prioritized", priority, paused,
-        parentId, parentQueueKey .. ":pc")
+      if priority == 0 then
+        rcall("RPUSH", parentTarget, parentId)
+      else
+        addJobWithPriority(parentWaitKey, parentQueueKey .. ":prioritized", priority, paused,
+          parentId, parentQueueKey .. ":pc")
+      end
+      rcall("XADD", parentQueueKey .. ":events", "*", "event", "waiting", "jobId", parentId, "prev", "waiting-children")
     end
-    rcall("XADD", parentQueueKey .. ":events", "*", "event", "waiting", "jobId", parentId, "prev", "waiting-children")
   end
 end
 if parentKey ~= nil then
   if rcall("EXISTS", parentKey) ~= 1 then
     return -5
   end
   parentData = cjson.encode(parent)
```

### Comparing `bullmq-1.6.1/bullmq/commands/changeDelay-3.lua` & `bullmq-1.7.0/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/changePriority-5.lua` & `bullmq-1.7.0/bullmq/commands/changePriority-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-1.7.0/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/drain-4.lua` & `bullmq-1.7.0/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/getCounts-1.lua` & `bullmq-1.7.0/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/getRanges-1.lua` & `bullmq-1.7.0/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/getState-8.lua` & `bullmq-1.7.0/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/getStateV2-8.lua` & `bullmq-1.7.0/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/isFinished-3.lua` & `bullmq-1.7.0/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-1.7.0/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-1.7.0/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/moveToActive-10.lua` & `bullmq-1.7.0/bullmq/commands/moveToActive-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/moveToDelayed-8.lua` & `bullmq-1.7.0/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/moveToFinished-13.lua` & `bullmq-1.7.0/bullmq/commands/moveToFinished-13.lua`

 * *Files 1% similar despite different names*

```diff
@@ -431,23 +431,26 @@
     local priority = tonumber(jobAttributes[1]) or 0
     local delay = tonumber(jobAttributes[2]) or 0
     if delay > 0 then
       local delayedTimestamp = tonumber(timestamp) + delay 
       local score = delayedTimestamp * 0x1000
       local parentDelayedKey = parentQueueKey .. ":delayed" 
       rcall("ZADD", parentDelayedKey, score, parentId)
+      rcall("XADD", parentQueueKey .. ":events", "*", "event", "delayed", "jobId", parentId,
+        "delay", delayedTimestamp)
       addDelayMarkerIfNeeded(parentTarget, parentDelayedKey)
-    -- Standard or priority add
-    elseif priority == 0 then
-      rcall("RPUSH", parentTarget, parentId)
     else
-      addJobWithPriority(parentWaitKey, parentQueueKey .. ":prioritized", priority, paused,
-        parentId, parentQueueKey .. ":pc")
+      if priority == 0 then
+        rcall("RPUSH", parentTarget, parentId)
+      else
+        addJobWithPriority(parentWaitKey, parentQueueKey .. ":prioritized", priority, paused,
+          parentId, parentQueueKey .. ":pc")
+      end
+      rcall("XADD", parentQueueKey .. ":events", "*", "event", "waiting", "jobId", parentId, "prev", "waiting-children")
     end
-    rcall("XADD", parentQueueKey .. ":events", "*", "event", "waiting", "jobId", parentId, "prev", "waiting-children")
   end
 end
 local function getRateLimitTTL(maxJobs, rateLimiterKey)
   if maxJobs then
     local pttl = rcall("PTTL", rateLimiterKey)
     if pttl == 0 then
       rcall("DEL", rateLimiterKey)
```

### Comparing `bullmq-1.6.1/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-1.7.0/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/obliterate-2.lua` & `bullmq-1.7.0/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/pause-5.lua` & `bullmq-1.7.0/bullmq/commands/pause-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/promote-7.lua` & `bullmq-1.7.0/bullmq/commands/promote-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/removeJob-1.lua` & `bullmq-1.7.0/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/removeRepeatable-2.lua` & `bullmq-1.7.0/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/reprocessJob-6.lua` & `bullmq-1.7.0/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/retryJob-9.lua` & `bullmq-1.7.0/bullmq/commands/retryJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/commands/retryJobs-6.lua` & `bullmq-1.7.0/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/event_emitter.py` & `bullmq-1.7.0/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/job.py` & `bullmq-1.7.0/bullmq/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         self.removeOnComplete = opts.get("removeOnComplete", True)
         self.removeOnFail = opts.get("removeOnFail", False)
         self.processedOn = 0
         self.finishedOn = 0
         self.returnvalue = None
         self.failedReason = None
         self.repeatJobKey = None
+        self.token: str = None
         parent = opts.get("parent")
         self.parentKey = get_parent_key(parent)
         self.parent = {"id": parent.get("id"), "queueKey": parent.get("queue")} if parent else None
         self.stacktrace: List[str] = []
         self.scripts = Scripts(queue.prefix, queue.name, queue.redisConnection)
 
     def updateData(self, data):
@@ -200,15 +201,16 @@
 
         return job
 
     @staticmethod
     async def fromId(queue: Queue, jobId: str):
         key = f"{queue.prefix}:{queue.name}:{jobId}"
         raw_data = await queue.client.hgetall(key)
-        return Job.fromJSON(queue, raw_data, jobId)
+        if len(raw_data):
+            return Job.fromJSON(queue, raw_data, jobId)
 
 
 def optsFromJSON(rawOpts: dict) -> dict:
     # opts = json.loads(rawOpts)
     opts = rawOpts
 
     option_entries = opts.items()
```

### Comparing `bullmq-1.6.1/bullmq/queue.py` & `bullmq-1.7.0/bullmq/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,7 +212,10 @@
         ]
 
     def close(self):
         """
         Close the queue instance.
         """
         return self.redisConnection.close()
+
+    def remove(self, job_id: str):
+        return self.scripts.remove(job_id)
```

### Comparing `bullmq-1.6.1/bullmq/redis_connection.py` & `bullmq-1.7.0/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/scripts.py` & `bullmq-1.7.0/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/timer.py` & `bullmq-1.7.0/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/types/job_options.py` & `bullmq-1.7.0/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/types/worker_options.py` & `bullmq-1.7.0/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/utils.py` & `bullmq-1.7.0/bullmq/utils.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/bullmq/worker.py` & `bullmq-1.7.0/bullmq/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         self.scripts = Scripts(opts.get("prefix", "bull"), name, self.redisConnection)
         self.closing = False
         self.forceClosing = False
         self.closed = False
         self.running = False
         self.processing = set()
         self.jobs = set()
+        self.id = uuid4().hex
 
         if opts.get("autorun", True):
             asyncio.ensure_future(self.run())
 
     async def run(self):
         if self.running:
             raise Exception("Worker is already running")
@@ -51,23 +52,25 @@
         self.timer = Timer(
             (self.opts.get("lockDuration") / 2) / 1000, self.extendLocks)
         self.stalledCheckTimer = Timer(self.opts.get(
             "stalledInterval") / 1000, self.runStalledJobsCheck)
         self.running = True
         jobs = []
 
-        token = uuid4().hex
+        token_postfix = 0
 
         while not self.closed:
             if len(jobs) == 0 and len(self.processing) < self.opts.get("concurrency") and not self.closing:
+                token_postfix+=1
+                token = f'{self.id}:{token_postfix}'
                 waiting_job = asyncio.ensure_future(self.getNextJob(token))
                 self.processing.add(waiting_job)
 
             if len(jobs) > 0:
-                jobs_to_process = [self.processJob(job, token) for job in jobs]
+                jobs_to_process = [self.processJob(job, job.token) for job in jobs]
                 processing_jobs = [asyncio.ensure_future(
                     j) for j in jobs_to_process]
                 self.processing.update(processing_jobs)
 
             try:
                 jobs, pending = await getCompleted(self.processing)
 
@@ -113,15 +116,17 @@
             timeout = int(math.ceil(timeout)) if isRedisVersionLowerThan(redis_version, '6.0.0') else timeout
 
             job_id = await self.bclient.brpoplpush(self.scripts.keys["wait"], self.scripts.keys["active"], timeout)
             if job_id:
                 job, job_id, limit_until, delay_until = await self.scripts.moveToActive(token, self.opts, job_id)
 
         if job and job_id:
-            return Job.fromJSON(self, job, job_id)
+            job_instance = Job.fromJSON(self, job, job_id)
+            job_instance.token = token
+            return job_instance
 
     async def processJob(self, job: Job, token: str):
         try:
             self.jobs.add((job, token))
             result = await self.processor(job, token)
             if not self.forceClosing:
                 await self.scripts.moveToCompleted(job, result, job.opts.get("removeOnComplete", False), token, self.opts, fetchNext=not self.closing)
```

### Comparing `bullmq-1.6.1/bullmq.egg-info/PKG-INFO` & `bullmq-1.7.0/bullmq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.6.1
+Version: 1.7.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.6.1/bullmq.egg-info/SOURCES.txt` & `bullmq-1.7.0/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-1.6.1/pyproject.toml` & `bullmq-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bullmq"
-version = "1.6.1"
+version = "1.7.0"
 description='BullMQ for Python'
 readme="README.md"
 authors = [
     {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
 ]
 requires-python = ">=3.10.0"
 classifiers=[
@@ -23,15 +23,15 @@
     "redis >= 4.5.0, < 5",
     "msgpack >= 1.0.0, < 2",
     "semver >= 2.13.0, < 3"
 ]
 
 [project.optional-dependencies]
 dev = [
-    "setuptools==63.1.0",
+    "setuptools==63.4.3",
     "pre-commit==3.3.3",
     "build==0.8.0",
     "python-semantic-release==7.28.1",
     "types-redis==4.6.0.2"
 ]
 
 [project.urls]
```

