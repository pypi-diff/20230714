# Comparing `tmp/taskcluster-taskgraph-5.6.0.tar.gz` & `tmp/taskcluster-taskgraph-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcluster-taskgraph-5.6.0.tar", last modified: Mon Jul 10 16:06:36 2023, max compression
+gzip compressed data, was "dist/taskcluster-taskgraph-5.6.1.tar", last modified: Fri Jul 14 13:44:57 2023, max compression
```

## Comparing `taskcluster-taskgraph-5.6.0.tar` & `taskcluster-taskgraph-5.6.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.589219 taskcluster-taskgraph-5.6.0/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    16725 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/LICENSE
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      175 2023-03-14 14:30:55.000000 taskcluster-taskgraph-5.6.0/MANIFEST.in
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      665 2023-07-10 16:06:36.589219 taskcluster-taskgraph-5.6.0/PKG-INFO
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3659 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/README.rst
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      602 2023-05-15 20:06:30.000000 taskcluster-taskgraph-5.6.0/pyproject.toml
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.577219 taskcluster-taskgraph-5.6.0/requirements/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      177 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/requirements/base.in
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    20339 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/requirements/base.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       22 2023-02-01 03:17:01.000000 taskcluster-taskgraph-5.6.0/requirements/dev.in
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1281 2023-06-05 16:10:05.000000 taskcluster-taskgraph-5.6.0/requirements/dev.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       58 2023-02-01 03:17:01.000000 taskcluster-taskgraph-5.6.0/requirements/test.in
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9241 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/requirements/test.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       38 2023-07-10 16:06:36.589219 taskcluster-taskgraph-5.6.0/setup.cfg
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1555 2023-05-09 14:44:30.000000 taskcluster-taskgraph-5.6.0/setup.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.577219 taskcluster-taskgraph-5.6.0/src/
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.577219 taskcluster-taskgraph-5.6.0/src/taskcluster_taskgraph.egg-info/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      665 2023-07-10 16:06:36.000000 taskcluster-taskgraph-5.6.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3977 2023-07-10 16:06:36.000000 taskcluster-taskgraph-5.6.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        1 2023-07-10 16:06:36.000000 taskcluster-taskgraph-5.6.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       50 2023-07-10 16:06:36.000000 taskcluster-taskgraph-5.6.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      201 2023-07-10 16:06:36.000000 taskcluster-taskgraph-5.6.0/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       10 2023-07-10 16:06:36.000000 taskcluster-taskgraph-5.6.0/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.581220 taskcluster-taskgraph-5.6.0/src/taskgraph/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      729 2023-07-10 16:05:39.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/__init__.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.581220 taskcluster-taskgraph-5.6.0/src/taskgraph/actions/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      416 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/actions/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1836 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/actions/add_new_jobs.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1309 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/actions/cancel.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1941 2023-03-27 14:05:26.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/actions/cancel_all.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1086 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    13113 2023-03-03 20:39:07.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/actions/registry.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9387 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/actions/retrigger.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10661 2023-05-25 14:01:37.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/actions/util.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4822 2023-07-10 15:52:14.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/config.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5184 2023-03-27 14:05:26.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/create.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12882 2023-03-14 14:30:55.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/decision.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7834 2023-02-27 19:27:15.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/docker.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2793 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/files_changed.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      866 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/filter_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15541 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/generator.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4680 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/graph.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.581220 taskcluster-taskgraph-5.6.0/src/taskgraph/loader/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        0 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/loader/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1185 2023-05-25 14:01:37.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/loader/default.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2147 2023-03-28 13:22:32.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/loader/transform.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    26201 2023-06-05 16:10:05.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/main.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9192 2023-05-25 14:01:37.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/morph.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.581220 taskcluster-taskgraph-5.6.0/src/taskgraph/optimize/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      123 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/optimize/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    18341 2023-05-29 20:22:45.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/optimize/base.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2380 2023-02-27 19:27:15.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/optimize/strategies.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    11906 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/parameters.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.581220 taskcluster-taskgraph-5.6.0/src/taskgraph/run-task/
--rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)    29990 2023-05-25 14:01:37.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/run-task/fetch-content
--rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)      896 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/run-task/hgrc
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    30813 2023-07-07 15:10:12.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/run-task/robustcheckout.py
--rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)    45018 2023-07-07 15:10:12.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/run-task/run-task
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3324 2023-02-24 14:13:32.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/target_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3240 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/task.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2434 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/taskgraph.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.581220 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      110 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5146 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/base.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2607 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/cached_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      707 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/code_review.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7606 2023-05-25 14:01:37.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/docker_image.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10479 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/fetch.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6647 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/from_deps.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.585219 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/job/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    17271 2023-05-02 12:56:02.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/job/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5897 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/job/common.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1220 2023-05-25 14:12:26.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/job/index_search.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9814 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/job/run_task.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6015 2023-02-27 19:27:15.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/job/toolchain.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6019 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/notify.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    52086 2023-07-10 15:52:14.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/task.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.585219 taskcluster-taskgraph-5.6.0/src/taskgraph/util/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        0 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2855 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/archive.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2964 2023-06-05 16:10:05.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/attributes.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3406 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/cached_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2433 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/decision.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2592 2023-07-07 15:10:12.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/dependencies.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    11690 2023-04-06 20:04:24.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/docker.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1661 2023-02-01 03:17:01.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/hash.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3419 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/keyed_by.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1331 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/memoize.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3184 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/parameterization.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4466 2023-05-25 14:01:37.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/path.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1576 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/python_path.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      787 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/readonlydict.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8323 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/schema.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1317 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/shell.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12445 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/taskcluster.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1969 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/taskgraph.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1417 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/templates.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3390 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/time.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2687 2023-05-25 14:01:37.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/treeherder.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    18780 2023-07-07 15:10:12.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/vcs.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8947 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/verify.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2498 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/workertypes.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1029 2023-03-03 20:39:07.000000 taskcluster-taskgraph-5.6.0/src/taskgraph/util/yaml.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-10 16:06:36.589219 taskcluster-taskgraph-5.6.0/test/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1584 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_actions_rebuild_cached_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1670 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_actions_registry.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3654 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_create.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7688 2023-03-14 14:30:55.000000 taskcluster-taskgraph-5.6.0/test/test_decision.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3505 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_files_changed.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7588 2023-05-25 14:01:37.000000 taskcluster-taskgraph-5.6.0/test/test_generator.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7063 2023-02-27 19:27:15.000000 taskcluster-taskgraph-5.6.0/test/test_graph.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7940 2023-06-05 16:10:05.000000 taskcluster-taskgraph-5.6.0/test/test_main.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2701 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_morph.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15584 2023-06-05 16:10:05.000000 taskcluster-taskgraph-5.6.0/test/test_optimize.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1727 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_optimize_strategies.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    13921 2023-03-14 14:30:55.000000 taskcluster-taskgraph-5.6.0/test/test_parameters.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2491 2023-05-25 14:01:37.000000 taskcluster-taskgraph-5.6.0/test/test_scripts_fetch_content.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12257 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/test/test_scripts_run_task.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12046 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_target_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3759 2023-02-27 19:27:15.000000 taskcluster-taskgraph-5.6.0/test/test_taskgraph.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1812 2023-05-25 14:01:37.000000 taskcluster-taskgraph-5.6.0/test/test_transform_docker_image.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      874 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_transforms_base.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1527 2023-05-02 13:16:10.000000 taskcluster-taskgraph-5.6.0/test/test_transforms_fetch.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6985 2023-07-07 15:10:12.000000 taskcluster-taskgraph-5.6.0/test/test_transforms_from_deps.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5181 2023-04-13 15:45:37.000000 taskcluster-taskgraph-5.6.0/test/test_transforms_job.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6291 2023-05-25 14:01:37.000000 taskcluster-taskgraph-5.6.0/test/test_transforms_job_run_task.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7131 2023-02-27 19:27:15.000000 taskcluster-taskgraph-5.6.0/test/test_transforms_job_toolchain.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6948 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_transforms_notify.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    25785 2023-07-10 15:52:14.000000 taskcluster-taskgraph-5.6.0/test/test_transforms_task.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3596 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_util_attributes.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1120 2023-06-22 23:33:17.000000 taskcluster-taskgraph-5.6.0/test/test_util_dependencies.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10212 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_util_docker.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2340 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_util_memoize.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7556 2023-02-01 03:17:01.000000 taskcluster-taskgraph-5.6.0/test/test_util_parameterization.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5906 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_util_path.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1045 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_util_python_path.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1234 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_util_readonlydict.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6961 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_util_schema.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10115 2023-02-27 19:27:15.000000 taskcluster-taskgraph-5.6.0/test/test_util_taskcluster.py
--rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)     1677 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_util_templates.py
--rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)     2239 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_util_time.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      913 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_util_treeherder.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15598 2023-07-07 15:10:12.000000 taskcluster-taskgraph-5.6.0/test/test_util_vcs.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4981 2023-01-13 21:44:18.000000 taskcluster-taskgraph-5.6.0/test/test_util_verify.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      942 2023-03-03 20:39:07.000000 taskcluster-taskgraph-5.6.0/test/test_util_workertypes.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1591 2023-03-03 20:39:07.000000 taskcluster-taskgraph-5.6.0/test/test_util_yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.1/LICENSE
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      175 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/MANIFEST.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3659 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.1/README.rst
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      602 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.6.1/pyproject.toml
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/requirements/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      177 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/requirements/base.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    20339 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/requirements/base.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/requirements/dev.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1281 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.6.1/requirements/dev.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       58 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.6.1/requirements/test.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9241 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/requirements/test.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/setup.cfg
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1555 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/setup.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskcluster_taskgraph.egg-info/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3977 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       50 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      201 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       10 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      729 2023-07-14 13:41:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/__init__.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/actions/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      416 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/actions/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1836 2023-06-12 19:54:30.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/actions/add_new_jobs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1309 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/actions/cancel.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1941 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/actions/cancel_all.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1086 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13122 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/actions/registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9387 2023-06-12 19:54:30.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/actions/retrigger.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/actions/util.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4822 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/config.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5184 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12882 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7834 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2793 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      866 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/filter_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15541 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4680 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/graph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/loader/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/loader/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1185 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/loader/default.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2147 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/loader/transform.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    26201 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9192 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/morph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/optimize/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      123 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/optimize/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18341 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/optimize/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2380 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/optimize/strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11906 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/parameters.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/run-task/
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    29990 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/run-task/fetch-content
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)      896 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/run-task/hgrc
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    30813 2023-07-06 14:31:47.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/run-task/robustcheckout.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    45128 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/run-task/run-task
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3324 2023-04-03 20:22:29.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3240 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2434 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/taskgraph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      110 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5146 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2607 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      707 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/code_review.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7606 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10479 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/fetch.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6647 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/from_deps.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/job/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    17271 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/job/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5897 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/job/common.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1220 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/job/index_search.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9814 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/job/run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6015 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/job/toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6019 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    52086 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/task.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2855 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/archive.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2964 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3406 2023-06-02 18:49:13.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2433 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2592 2023-07-06 14:31:47.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/dependencies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11699 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/hash.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3419 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/keyed_by.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1331 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3184 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4466 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1576 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      787 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8323 2023-04-18 14:17:54.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1317 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/shell.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12445 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/taskcluster.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1969 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1417 2022-05-30 14:06:28.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/templates.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3390 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2687 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18780 2023-07-06 14:16:59.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8947 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2498 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      990 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.1/src/taskgraph/util/yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-14 13:44:56.000000 taskcluster-taskgraph-5.6.1/test/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1584 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.6.1/test/test_actions_rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1670 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_actions_registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3654 2023-03-09 21:40:30.000000 taskcluster-taskgraph-5.6.1/test/test_create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7688 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3505 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7588 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7063 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_graph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7940 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.6.1/test/test_main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2701 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_morph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15584 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.6.1/test/test_optimize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1727 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_optimize_strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13921 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_parameters.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2491 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_scripts_fetch_content.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12257 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.6.1/test/test_scripts_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12046 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3759 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1812 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_transform_docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      874 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_transforms_base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1527 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.6.1/test/test_transforms_fetch.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6985 2023-07-06 14:31:47.000000 taskcluster-taskgraph-5.6.1/test/test_transforms_from_deps.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5181 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_transforms_job.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6291 2023-04-19 14:40:27.000000 taskcluster-taskgraph-5.6.1/test/test_transforms_job_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7131 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_transforms_job_toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6948 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_transforms_notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    25785 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.1/test/test_transforms_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3596 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_util_attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1120 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.6.1/test/test_util_dependencies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10212 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_util_docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2340 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_util_memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7556 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_util_parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5906 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_util_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1045 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.6.1/test/test_util_python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1234 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_util_readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6961 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_util_schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10115 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_util_taskcluster.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     1677 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_util_templates.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2239 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_util_time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      913 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_util_treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15598 2023-07-06 14:10:15.000000 taskcluster-taskgraph-5.6.1/test/test_util_vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4981 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.6.1/test/test_util_verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.6.1/test/test_util_workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1005 2023-07-14 13:24:34.000000 taskcluster-taskgraph-5.6.1/test/test_util_yaml.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `taskcluster-taskgraph-5.6.0/LICENSE` & `taskcluster-taskgraph-5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/PKG-INFO` & `taskcluster-taskgraph-5.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.6.0
+Version: 5.6.1
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.6.0/README.rst` & `taskcluster-taskgraph-5.6.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -41,22 +41,22 @@
 and aren't limited to being triggered in response to supported events.
 
 Taskgraph leverages this execution platform to allow CI systems to scale to any
 size or complexity.
 
 1. A *decision task* is created via Taskcluster's normal `.taskcluster.yml`_
    file. This task invokes ``taskgraph``.
-3. Taskgraph evaluates a series of yaml based task definitions (similar to
+2. Taskgraph evaluates a series of yaml based task definitions (similar to
    those other CI offerings provide).
-4. Taskgraph applies transforms on top of these task definitions. Transforms
+3. Taskgraph applies transforms on top of these task definitions. Transforms
    are Python functions that can programmatically alter or even clone a task
    definition.
-5. Taskgraph applies some optional optimization logic to remove unnecessary
+4. Taskgraph applies some optional optimization logic to remove unnecessary
    tasks.
-6. Taskgraph submits the resulting *task graph* to Taskcluster via its API.
+5. Taskgraph submits the resulting *task graph* to Taskcluster via its API.
 
 Taskgraph's combination of declarative task configuration combined with
 programmatic alteration are what allow it to support CI systems of any scale.
 Taskgraph is the library that powers the 30,000+ tasks making up `Firefox's
 CI`_.
 
 .. _Taskcluster CI: https://taskcluster.net/
@@ -64,15 +64,15 @@
 .. _.taskcluster.yml: https://docs.taskcluster.net/docs/reference/integrations/github/taskcluster-yml-v1
 .. _Firefox's CI: https://treeherder.mozilla.org/jobs?repo=mozilla-central
 .. _see the docs: https://taskcluster-taskgraph.readthedocs.io
 
 Installation
 ------------
 
-Taskgraph supports Python 3.6 and up, and can be installed from Pypi:
+Taskgraph supports Python 3.7 and up, and can be installed from Pypi:
 
 .. code-block::
 
   pip install taskcluster-taskgraph
 
 
 Alternatively, the repo can be cloned and installed directly:
```

### Comparing `taskcluster-taskgraph-5.6.0/pyproject.toml` & `taskcluster-taskgraph-5.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/requirements/base.txt` & `taskcluster-taskgraph-5.6.1/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/requirements/dev.txt` & `taskcluster-taskgraph-5.6.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/requirements/test.txt` & `taskcluster-taskgraph-5.6.1/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/setup.py` & `taskcluster-taskgraph-5.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-5.6.1/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.6.0
+Version: 5.6.1
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.6.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-5.6.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/__init__.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "5.6.0"
+__version__ = "5.6.1"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/actions/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     try:
         json.dumps(data)
     except ValueError:
         return False
     return True
 
 
+@memoize
 def read_taskcluster_yml(filename):
     """Load and parse .taskcluster.yml, memoized to save some time"""
     return yaml.load_yaml(filename)
 
 
 @memoize
 def hash_taskcluster_yml(filename):
```

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/config.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/create.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/decision.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/docker.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/files_changed.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/generator.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/graph.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/main.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/morph.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/optimize/strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/parameters.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-5.6.1/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-5.6.1/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-5.6.1/src/taskgraph/run-task/run-task`

 * *Files 0% similar despite different names*

```diff
@@ -1078,14 +1078,18 @@
 
 def main(args):
     os.environ["TASK_WORKDIR"] = os.getcwd()
     print_line(
         b"setup",
         b"run-task started in %s\n" % os.environ["TASK_WORKDIR"].encode("utf-8"),
     )
+    print_line(
+        b"setup",
+        b"Invoked by command: %s\n" % " ".join(args).encode("utf-8"),
+    )
     _display_python_version()
     running_as_root = IS_POSIX and os.getuid() == 0
 
     # Arguments up to '--' are ours. After are for the main task
     # to be executed.
     try:
         i = args.index("--")
```

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/task.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/from_deps.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/job/__init__.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/job/common.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/job/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/job/index_search.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/job/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/job/run_task.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/job/run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/job/toolchain.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/job/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/transforms/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/decision.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/dependencies.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,14 +295,15 @@
     archive_files["Dockerfile"] = io.BytesIO("".join(content).encode("utf-8"))
 
     writer = HashingWriter(out_file)
     create_tar_gz_from_files(writer, archive_files, image_name)
     return writer.hexdigest()
 
 
+@memoize
 def image_paths():
     """Return a map of image name to paths containing their Dockerfile."""
     config = load_yaml("taskcluster", "ci", "docker-image", "kind.yml")
     return {
         k: os.path.join(IMAGE_DIR, v.get("definition", k))
         for k, v in config["tasks"].items()
     }
```

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/memoize.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/path.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/time.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-5.6.1/src/taskgraph/util/yaml.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 import os
 
 from yaml.loader import SafeLoader
 
-from .memoize import memoize
-
 
 class UnicodeLoader(SafeLoader):
     def construct_yaml_str(self, node):
         return self.construct_scalar(node)
 
 
 UnicodeLoader.add_constructor("tag:yaml.org,2002:str", UnicodeLoader.construct_yaml_str)
@@ -26,14 +24,13 @@
     loader = UnicodeLoader(stream)
     try:
         return loader.get_single_data()
     finally:
         loader.dispose()
 
 
-@memoize
 def load_yaml(*parts):
     """Convenience function to load a YAML file in the given path.  This is
     useful for loading kind configuration files from the kind path."""
     filename = os.path.join(*parts)
     with open(filename, "rb") as f:
         return load_stream(f)
```

### Comparing `taskcluster-taskgraph-5.6.0/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.6.1/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_actions_registry.py` & `taskcluster-taskgraph-5.6.1/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_create.py` & `taskcluster-taskgraph-5.6.1/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_decision.py` & `taskcluster-taskgraph-5.6.1/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_files_changed.py` & `taskcluster-taskgraph-5.6.1/test/test_files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_generator.py` & `taskcluster-taskgraph-5.6.1/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_graph.py` & `taskcluster-taskgraph-5.6.1/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_main.py` & `taskcluster-taskgraph-5.6.1/test/test_main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_morph.py` & `taskcluster-taskgraph-5.6.1/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_optimize.py` & `taskcluster-taskgraph-5.6.1/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_optimize_strategies.py` & `taskcluster-taskgraph-5.6.1/test/test_optimize_strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_parameters.py` & `taskcluster-taskgraph-5.6.1/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-5.6.1/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_scripts_run_task.py` & `taskcluster-taskgraph-5.6.1/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_target_tasks.py` & `taskcluster-taskgraph-5.6.1/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_taskgraph.py` & `taskcluster-taskgraph-5.6.1/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_transform_docker_image.py` & `taskcluster-taskgraph-5.6.1/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_transforms_base.py` & `taskcluster-taskgraph-5.6.1/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_transforms_fetch.py` & `taskcluster-taskgraph-5.6.1/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_transforms_from_deps.py` & `taskcluster-taskgraph-5.6.1/test/test_transforms_from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_transforms_job.py` & `taskcluster-taskgraph-5.6.1/test/test_transforms_job.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_transforms_job_run_task.py` & `taskcluster-taskgraph-5.6.1/test/test_transforms_job_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_transforms_job_toolchain.py` & `taskcluster-taskgraph-5.6.1/test/test_transforms_job_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_transforms_notify.py` & `taskcluster-taskgraph-5.6.1/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_transforms_task.py` & `taskcluster-taskgraph-5.6.1/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_attributes.py` & `taskcluster-taskgraph-5.6.1/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_dependencies.py` & `taskcluster-taskgraph-5.6.1/test/test_util_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_docker.py` & `taskcluster-taskgraph-5.6.1/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_memoize.py` & `taskcluster-taskgraph-5.6.1/test/test_util_memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_parameterization.py` & `taskcluster-taskgraph-5.6.1/test/test_util_parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_path.py` & `taskcluster-taskgraph-5.6.1/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_python_path.py` & `taskcluster-taskgraph-5.6.1/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_readonlydict.py` & `taskcluster-taskgraph-5.6.1/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_schema.py` & `taskcluster-taskgraph-5.6.1/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_taskcluster.py` & `taskcluster-taskgraph-5.6.1/test/test_util_taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_templates.py` & `taskcluster-taskgraph-5.6.1/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_time.py` & `taskcluster-taskgraph-5.6.1/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_treeherder.py` & `taskcluster-taskgraph-5.6.1/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_vcs.py` & `taskcluster-taskgraph-5.6.1/test/test_util_vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_verify.py` & `taskcluster-taskgraph-5.6.1/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.6.0/test/test_util_workertypes.py` & `taskcluster-taskgraph-5.6.1/test/test_util_workertypes.py`

 * *Files identical despite different names*

