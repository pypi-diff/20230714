# Comparing `tmp/python-arango-7.5.8.tar.gz` & `tmp/python-arango-7.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-arango-7.5.8.tar", last modified: Fri Jun  2 15:44:35 2023, max compression
+gzip compressed data, was "python-arango-7.5.9.tar", last modified: Fri Jul 14 09:18:45 2023, max compression
```

## Comparing `python-arango-7.5.8.tar` & `python-arango-7.5.9.tar`

### file list

```diff
@@ -1,94 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.190516 python-arango-7.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.182516 python-arango-7.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.182516 python-arango-7.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-02 15:44:21.000000 python-arango-7.5.8/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-02 15:44:21.000000 python-arango-7.5.8/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-02 15:44:21.000000 python-arango-7.5.8/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-02 15:44:21.000000 python-arango-7.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-02 15:44:21.000000 python-arango-7.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-02 15:44:21.000000 python-arango-7.5.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-02 15:44:21.000000 python-arango-7.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 15:44:21.000000 python-arango-7.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-06-02 15:44:35.190516 python-arango-7.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-02 15:44:21.000000 python-arango-7.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.186516 python-arango-7.5.8/arango/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26767 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/aql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   122524 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)    99686 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    34373 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/errno.py
--rw-r--r--   0 runner    (1001) docker     (123)    22468 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    39554 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32737 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/foxx.py
--rw-r--r--   0 runner    (1001) docker     (123)    35862 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/pregel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33852 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 15:44:34.000000 python-arango-7.5.8/arango/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-06-02 15:44:21.000000 python-arango-7.5.8/arango/wal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.186516 python-arango-7.5.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/admin.rst
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/analyzer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/aql.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/async.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/backup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/batch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/certificates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/cluster.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/collection.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/cursor.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/document.rst
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/errno.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/foxx.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/graph.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/http.rst
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/indexes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/pregel.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/replication.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/serializer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/simple.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/specs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.190516 python-arango-7.5.8/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/task.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/threading.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/transaction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/user.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/view.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-02 15:44:21.000000 python-arango-7.5.8/docs/wal.rst
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-02 15:44:21.000000 python-arango-7.5.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:44:35.190516 python-arango-7.5.8/python_arango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-06-02 15:44:35.000000 python-arango-7.5.8/python_arango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-02 15:44:35.000000 python-arango-7.5.8/python_arango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:44:35.000000 python-arango-7.5.8/python_arango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-02 15:44:35.000000 python-arango-7.5.8/python_arango.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 15:44:35.000000 python-arango-7.5.8/python_arango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-02 15:44:35.190516 python-arango-7.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-02 15:44:21.000000 python-arango-7.5.8/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4068 2023-06-02 15:44:21.000000 python-arango-7.5.8/tester.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:45.003551 python-arango-7.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:44.995550 python-arango-7.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:44.999551 python-arango-7.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-14 09:18:33.000000 python-arango-7.5.9/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-14 09:18:33.000000 python-arango-7.5.9/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-14 09:18:33.000000 python-arango-7.5.9/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-14 09:18:33.000000 python-arango-7.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-14 09:18:33.000000 python-arango-7.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-14 09:18:33.000000 python-arango-7.5.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-14 09:18:33.000000 python-arango-7.5.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 09:18:33.000000 python-arango-7.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-14 09:18:33.000000 python-arango-7.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-14 09:18:45.003551 python-arango-7.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-14 09:18:33.000000 python-arango-7.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:44.999551 python-arango-7.5.9/arango/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27539 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/aql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123588 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102581 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34373 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/errno.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41559 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32737 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/foxx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35862 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/pregel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33852 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 09:18:44.000000 python-arango-7.5.9/arango/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/wal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:45.003551 python-arango-7.5.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/admin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/analyzer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/aql.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/async.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/backup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/batch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/certificates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/cluster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/collection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/cursor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/document.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/errno.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/foxx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/graph.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/http.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/indexes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/overload.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/pregel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/replication.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/serializer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/simple.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/specs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:45.003551 python-arango-7.5.9/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/task.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/threading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/view.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/wal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-14 09:18:33.000000 python-arango-7.5.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:45.003551 python-arango-7.5.9/python_arango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-14 09:18:44.000000 python-arango-7.5.9/python_arango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-14 09:18:44.000000 python-arango-7.5.9/python_arango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:18:44.000000 python-arango-7.5.9/python_arango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-14 09:18:44.000000 python-arango-7.5.9/python_arango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 09:18:44.000000 python-arango-7.5.9/python_arango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 09:18:45.015551 python-arango-7.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-14 09:18:33.000000 python-arango-7.5.9/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4095 2023-07-14 09:18:33.000000 python-arango-7.5.9/tester.sh
```

### Comparing `python-arango-7.5.8/.github/workflows/build.yaml` & `python-arango-7.5.9/.github/workflows/build.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
       - name: Fetch all tags and branches
         run: git fetch --prune --unshallow
 
       - name: Create ArangoDB Docker container
         run: >
           docker create --name arango -p 8529:8529 -e ARANGO_ROOT_PASSWORD=passwd -v "$(pwd)/tests/static/":/tests/static
-          arangodb/arangodb:3.10.6 --server.jwt-secret-keyfile=/tests/static/keyfile
+          arangodb/arangodb:3.10.9 --server.jwt-secret-keyfile=/tests/static/keyfile
 
       - name: Start ArangoDB Docker container
         run: docker start arango
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
```

### Comparing `python-arango-7.5.8/.github/workflows/pypi.yaml` & `python-arango-7.5.9/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/.gitignore` & `python-arango-7.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/.pre-commit-config.yaml` & `python-arango-7.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/CONTRIBUTING.md` & `python-arango-7.5.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/LICENSE` & `python-arango-7.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/PKG-INFO` & `python-arango-7.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-arango
-Version: 7.5.8
+Version: 7.5.9
 Summary: Python Driver for ArangoDB
 Home-page: https://github.com/ArangoDB-Community/python-arango
 Author: Joohwan Oh
 Author-email: joohwan.oh@outlook.com
 License: MIT
 Keywords: arangodb,python,driver
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,15 @@
 # Python-Arango
 
 Python driver for [ArangoDB](https://www.arangodb.com), a scalable multi-model
 database natively supporting documents, graphs and search.
 
 ## Requirements
 
-- ArangoDB version 3.7+
+- ArangoDB version 3.9+
 - Python version 3.8+
 
 ## Installation
 
 ```shell
 pip install python-arango --upgrade
 ```
```

### Comparing `python-arango-7.5.8/README.md` & `python-arango-7.5.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Python-Arango
 
 Python driver for [ArangoDB](https://www.arangodb.com), a scalable multi-model
 database natively supporting documents, graphs and search.
 
 ## Requirements
 
-- ArangoDB version 3.7+
+- ArangoDB version 3.9+
 - Python version 3.8+
 
 ## Installation
 
 ```shell
 pip install python-arango --upgrade
 ```
```

### Comparing `python-arango-7.5.8/arango/api.py` & `python-arango-7.5.9/arango/api.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/aql.py` & `python-arango-7.5.9/arango/aql.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,19 +209,27 @@
             data=data,
         )
 
         def response_handler(resp: Response) -> Union[Json, Jsons]:
             if not resp.is_success:
                 raise AQLQueryExplainError(resp, request)
             if "plan" in resp.body:
-                plan: Json = resp.body["plan"]
-                return plan
+                result: Json = resp.body["plan"]
+                if "stats" in resp.body:
+                    result["stats"] = resp.body["stats"]
+                return result
             else:
-                plans: Jsons = resp.body["plans"]
-                return plans
+                results: Jsons = resp.body["plans"]
+                if "stats" in resp.body:
+                    # Although "plans" contains an array, "stats" is a single object.
+                    # We need to duplicate "stats" for each plan in order to preserve
+                    # the original structure.
+                    for plan in results:
+                        plan["stats"] = resp.body["stats"]
+                return results
 
         return self._execute(request, response_handler)
 
     def validate(self, query: str) -> Result[Json]:
         """Parse and validate the query without executing it.
 
         :param query: Query to validate.
@@ -263,14 +271,15 @@
         intermediate_commit_size: Optional[int] = None,
         satellite_sync_wait: Optional[int] = None,
         stream: Optional[bool] = None,
         skip_inaccessible_cols: Optional[bool] = None,
         max_runtime: Optional[Number] = None,
         fill_block_cache: Optional[bool] = None,
         allow_dirty_read: bool = False,
+        allow_retry: bool = False,
     ) -> Result[Cursor]:
         """Execute the query and return the result cursor.
 
         :param query: Query to execute.
         :type query: str
         :param count: If set to True, the total document count is included in
             the result cursor.
@@ -300,15 +309,15 @@
             "resource limit exceeded". Value 0 indicates no limit.
         :type memory_limit: int
         :param fail_on_warning: If set to True, the query throws an exception
             instead of producing a warning. This parameter can be used during
             development to catch issues early. If set to False, warnings are
             returned with the query result. There is a server configuration
             option "--query.fail-on-warning" for setting the default value for
-            this behaviour so it does not need to be set per-query.
+            this behaviour, so it does not need to be set per-query.
         :type fail_on_warning: bool
         :param profile: Return additional profiling details in the cursor,
             unless the query cache is used.
         :type profile: bool
         :param max_transaction_size: Transaction size limit in bytes.
         :type max_transaction_size: int
         :param max_warning_count: Max number of warnings returned.
@@ -357,14 +366,17 @@
             cache, or for queries that read data which are known to be outside
             of the hot set. By setting the option to false, data read by the
             query will not make it into the RocksDB block cache if not already
             in there, thus leaving more room for the actual hot set.
         :type fill_block_cache: bool
         :param allow_dirty_read: Allow reads from followers in a cluster.
         :type allow_dirty_read: bool | None
+        :param allow_retry: Make it possible to retry fetching the latest batch
+            from a cursor.
+        :type allow_retry: bool
         :return: Result cursor.
         :rtype: arango.cursor.Cursor
         :raise arango.exceptions.AQLQueryExecuteError: If execute fails.
         """
         data: Json = {"query": query, "count": count}
         if batch_size is not None:
             data["batchSize"] = batch_size
@@ -403,29 +415,33 @@
         if stream is not None:
             options["stream"] = stream
         if skip_inaccessible_cols is not None:
             options["skipInaccessibleCollections"] = skip_inaccessible_cols
         if max_runtime is not None:
             options["maxRuntime"] = max_runtime
 
+        # New in 3.11
+        if allow_retry is not None:
+            options["allowRetry"] = allow_retry
+
         if options:
             data["options"] = options
         data.update(options)
 
         request = Request(
             method="post",
             endpoint="/_api/cursor",
             data=data,
             headers={"x-arango-allow-dirty-read": "true"} if allow_dirty_read else None,
         )
 
         def response_handler(resp: Response) -> Cursor:
             if not resp.is_success:
                 raise AQLQueryExecuteError(resp, request)
-            return Cursor(self._conn, resp.body)
+            return Cursor(self._conn, resp.body, allow_retry=allow_retry)
 
         return self._execute(request, response_handler)
 
     def kill(self, query_id: str) -> Result[bool]:
         """Kill a running query.
 
         :param query_id: Query ID.
```

### Comparing `python-arango-7.5.8/arango/backup.py` & `python-arango-7.5.9/arango/backup.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/client.py` & `python-arango-7.5.9/arango/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     BasicConnection,
     Connection,
     JwtConnection,
     JwtSuperuserConnection,
 )
 from arango.database import StandardDatabase
 from arango.exceptions import ServerConnectionError
-from arango.http import DefaultHTTPClient, HTTPClient
+from arango.http import DEFAULT_REQUEST_TIMEOUT, DefaultHTTPClient, HTTPClient
 from arango.resolver import (
     HostResolver,
     RandomHostResolver,
     RoundRobinHostResolver,
     SingleHostResolver,
 )
 
@@ -51,30 +51,30 @@
        None: Do not change the verification behavior of the underlying HTTP client.
        True: Verify TLS certificate using the system CA certificates.
        False: Do not verify TLS certificate.
        str: Path to a custom CA bundle file or directory.
     :type verify_override: Union[bool, str, None]
     :param request_timeout: This is the default request timeout (in seconds)
        for http requests issued by the client if the parameter http_client is
-       not secified. The default value is 60.
+       not specified. The default value is 60.
        None: No timeout.
        int: Timeout value in seconds.
-    :type request_timeout: Any
+    :type request_timeout: int | float
     """
 
     def __init__(
         self,
         hosts: Union[str, Sequence[str]] = "http://127.0.0.1:8529",
         host_resolver: str = "roundrobin",
         resolver_max_tries: Optional[int] = None,
         http_client: Optional[HTTPClient] = None,
         serializer: Callable[..., str] = lambda x: dumps(x),
         deserializer: Callable[[str], Any] = lambda x: loads(x),
         verify_override: Union[bool, str, None] = None,
-        request_timeout: Any = 60,
+        request_timeout: Union[int, float] = DEFAULT_REQUEST_TIMEOUT,
     ) -> None:
         if isinstance(hosts, str):
             self._hosts = [host.strip("/") for host in hosts.split(",")]
         else:
             self._hosts = [host.strip("/") for host in hosts]
 
         host_count = len(self._hosts)
@@ -84,19 +84,15 @@
             self._host_resolver = SingleHostResolver(1, resolver_max_tries)
         elif host_resolver == "random":
             self._host_resolver = RandomHostResolver(host_count, resolver_max_tries)
         else:
             self._host_resolver = RoundRobinHostResolver(host_count, resolver_max_tries)
 
         # Initializes the http client
-        self._http = http_client or DefaultHTTPClient()
-        # Sets the request timeout.
-        # This call can only happen AFTER initializing the http client.
-        if http_client is None:
-            self.request_timeout = request_timeout
+        self._http = http_client or DefaultHTTPClient(request_timeout=request_timeout)
 
         self._serializer = serializer
         self._deserializer = deserializer
         self._sessions = [self._http.create_session(h) for h in self._hosts]
 
         # override SSL/TLS certificate verification if provided
         if verify_override is not None:
@@ -133,20 +129,20 @@
     @property
     def request_timeout(self) -> Any:
         """Return the request timeout of the http client.
 
         :return: Request timeout.
         :rtype: Any
         """
-        return self._http.REQUEST_TIMEOUT  # type: ignore
+        return self._http.request_timeout  # type: ignore
 
     # Setter for request_timeout
     @request_timeout.setter
     def request_timeout(self, value: Any) -> None:
-        self._http.REQUEST_TIMEOUT = value  # type: ignore
+        self._http.request_timeout = value  # type: ignore
 
     def db(
         self,
         name: str = "_system",
         username: str = "root",
         password: str = "",
         verify: bool = False,
```

### Comparing `python-arango-7.5.8/arango/cluster.py` & `python-arango-7.5.9/arango/cluster.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/collection.py` & `python-arango-7.5.9/arango/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1338,39 +1338,50 @@
         primarySort: Optional[Json] = None,
         storedValues: Optional[Sequence[Json]] = None,
         analyzer: Optional[str] = None,
         features: Optional[Sequence[str]] = None,
         includeAllFields: Optional[bool] = None,
         trackListPositions: Optional[bool] = None,
         searchField: Optional[bool] = None,
+        primaryKeyCache: Optional[bool] = None,
+        cache: Optional[bool] = None,
     ) -> Result[Json]:
         """Create a new inverted index, introduced in version 3.10.
 
         :param fields: Document fields to index.
         :type fields: Json
         :param name: Optional name for the index.
         :type name: str | None
         :param inBackground: Do not hold the collection lock.
         :type inBackground: bool | None
-        :param parallelism:
+        :param parallelism: The number of threads to use for indexing the fields.
         :type parallelism: int | None
-        :param primarySort:
-        :type primarySort: Json | None
-        :param storedValues:
+        :param primarySort: Primary sort order to enable an AQL optimization.
+        :type primarySort: Optional[Json]
+        :param storedValues: An array of objects with paths to additional
+            attributes to store in the index.
         :type storedValues: Sequence[Json] | None
-        :param analyzer:
-        :type analyzer: str | None
-        :param features:
+        :param analyzer: Analyzer to use by default.
+        :type analyzer: Optional[str]
+        :param features: List of Analyzer features.
         :type features: Sequence[str] | None
-        :param includeAllFields:
+        :param includeAllFields: This option only applies if you use the
+            inverted index in search-alias views.
         :type includeAllFields: bool | None
-        :param trackListPositions:
+        :param trackListPositions: This option only applies if you use the
+            inverted index in search-alias views, and searchField is true.
         :type trackListPositions: bool | None
-        :param searchField:
+        :param searchField: This option only applies if you use the inverted
+            index in search-alias views
         :type searchField: bool | None
+        :param primaryKeyCache: Always cache the primary key column in memory.
+        :type primaryKeyCache: bool | None
+        :param cache: Always cache the field normalization values in memory
+            for all fields by default.
+        :type cache: bool | None
         :return: New index details.
         :rtype: dict
         :raise arango.exceptions.IndexCreateError: If create fails.
         """
         data: Json = {"type": "inverted", "fields": fields}
 
         if name is not None:
@@ -1391,14 +1402,18 @@
             data["includeAllFields"] = includeAllFields
         if trackListPositions is not None:
             data["trackListPositions"] = trackListPositions
         if searchField is not None:
             data["searchField"] = searchField
         if fields is not None:
             data["fields"] = fields
+        if primaryKeyCache is not None:
+            data["primaryKeyCache"] = primaryKeyCache
+        if cache is not None:
+            data["cache"] = cache
 
         return self._add_index(data)
 
     def delete_index(self, index_id: str, ignore_missing: bool = False) -> Result[bool]:
         """Delete an index.
 
         :param index_id: Index ID.
```

### Comparing `python-arango-7.5.8/arango/connection.py` & `python-arango-7.5.9/arango/connection.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/cursor.py` & `python-arango-7.5.9/arango/cursor.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,44 +23,53 @@
     shared across threads without proper locking mechanism.
 
     :param connection: HTTP connection.
     :param init_data: Cursor initialization data.
     :type init_data: dict
     :param cursor_type: Cursor type ("cursor" or "export").
     :type cursor_type: str
+    :param allow_retry: If set to True, the cursor will always attempt to fetch
+            the latest batch from server even if the previous attempt failed.
+            This option is only available for server versions 3.11 and above.
+    :type allow_retry: bool
     """
 
     __slots__ = [
         "_conn",
         "_type",
         "_id",
         "_count",
         "_cached",
         "_stats",
         "_profile",
         "_warnings",
         "_has_more",
         "_batch",
+        "_next_batch_id",
+        "_allow_retry",
     ]
 
     def __init__(
         self,
         connection: BaseConnection,
         init_data: Json,
         cursor_type: str = "cursor",
+        allow_retry: bool = False,
     ) -> None:
         self._conn = connection
         self._type = cursor_type
+        self._allow_retry = allow_retry
         self._batch: Deque[Any] = deque()
         self._id = None
         self._count: Optional[int] = None
         self._cached = None
         self._stats = None
         self._profile = None
         self._warnings = None
+        self._next_batch_id: Optional[str] = None
         self._update(init_data)
 
     def __iter__(self) -> "Cursor":
         return self
 
     def __next__(self) -> Any:  # pragma: no cover
         return self.next()
@@ -95,14 +104,21 @@
         if "count" in data:
             self._count = data["count"]
             result["count"] = data["count"]
         if "cached" in data:
             self._cached = data["cached"]
             result["cached"] = data["cached"]
 
+        # New in 3.11
+        if "nextBatchId" in data:
+            # This is only available for server versions 3.11 and above.
+            # Currently, we are testing against 3.10.9
+            self._next_batch_id = data["nextBatchId"]  # pragma: no cover
+            result["next_batch_id"] = data["nextBatchId"]  # pragma: no cover
+
         self._has_more = bool(data["hasMore"])
         result["has_more"] = data["hasMore"]
 
         self._batch.extend(data["result"])
         result["batch"] = data["result"]
 
         if "extra" in data:
@@ -134,14 +150,19 @@
                     stats["cursorsCreated"] = stats.pop("cursorsCreated")
                 if "cursorsRearmed" in stats:
                     stats["cursorsRearmed"] = stats.pop("cursorsRearmed")
                 if "cacheHits" in stats:
                     stats["cacheHits"] = stats.pop("cacheHits")
                 if "cacheMisses" in stats:
                     stats["cacheMisses"] = stats.pop("cacheMisses")
+
+                # New in 3.11
+                if "peakMemoryUsage" in stats:
+                    stats["peak_memory_usage"] = stats.pop("peakMemoryUsage")
+
                 self._stats = stats
                 result["statistics"] = stats
 
         return result
 
     @property
     def id(self) -> Optional[str]:
@@ -264,15 +285,20 @@
         :return: New batch details.
         :rtype: dict
         :raise arango.exceptions.CursorNextError: If batch retrieval fails.
         :raise arango.exceptions.CursorStateError: If cursor ID is not set.
         """
         if self._id is None:
             raise CursorStateError("cursor ID not set")
-        request = Request(method="put", endpoint=f"/_api/{self._type}/{self._id}")
+
+        endpoint = f"/_api/{self._type}/{self._id}"
+        if self._allow_retry and self._next_batch_id is not None:
+            endpoint += f"/{self._next_batch_id}"  # pragma: no cover
+
+        request = Request(method="post", endpoint=endpoint)
         resp = self._conn.send_request(request)
 
         if not resp.is_success:
             raise CursorNextError(resp, request)
 
         return self._update(resp.body)
```

### Comparing `python-arango-7.5.8/arango/database.py` & `python-arango-7.5.9/arango/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-__all__ = ["StandardDatabase", "AsyncDatabase", "BatchDatabase", "TransactionDatabase"]
+__all__ = [
+    "StandardDatabase",
+    "AsyncDatabase",
+    "BatchDatabase",
+    "OverloadControlDatabase",
+    "TransactionDatabase",
+]
 
 from datetime import datetime
 from numbers import Number
 from typing import Any, List, Optional, Sequence, Union
 
 from arango.api import ApiGroup
 from arango.aql import AQL
@@ -71,14 +77,15 @@
     ViewReplaceError,
     ViewUpdateError,
 )
 from arango.executor import (
     AsyncApiExecutor,
     BatchApiExecutor,
     DefaultApiExecutor,
+    OverloadControlApiExecutor,
     TransactionApiExecutor,
 )
 from arango.formatter import (
     format_body,
     format_database,
     format_server_status,
     format_tls,
@@ -296,29 +303,33 @@
             if not resp.is_success:
                 raise TransactionExecuteError(resp, request)
 
             return resp.body.get("result")
 
         return self._execute(request, response_handler)
 
-    def version(self) -> Result[str]:
+    def version(self, details: bool = False) -> Result[Any]:
         """Return ArangoDB server version.
-
+        :param details: Return more detailed version output
+        :type details: bool | None
         :return: Server version.
         :rtype: str
         :raise arango.exceptions.ServerVersionError: If retrieval fails.
         """
         request = Request(
-            method="get", endpoint="/_api/version", params={"details": False}
+            method="get", endpoint="/_api/version", params={"details": details}
         )
 
-        def response_handler(resp: Response) -> str:
+        def response_handler(resp: Response) -> Any:
             if not resp.is_success:
                 raise ServerVersionError(resp, request)
-            return str(resp.body["version"])
+            if not details:
+                return str(resp.body["version"])
+            else:
+                return resp.body
 
         return self._execute(request, response_handler)
 
     def details(self) -> Result[Json]:
         """Return ArangoDB server details.
 
         :return: Server details.
@@ -2510,14 +2521,27 @@
             exclusive=exclusive,
             sync=sync,
             allow_implicit=allow_implicit,
             lock_timeout=lock_timeout,
             max_size=max_size,
         )
 
+    def begin_controlled_execution(
+        self, max_queue_time_seconds: Optional[float] = None
+    ) -> "OverloadControlDatabase":
+        """Begin a controlled connection, with options to handle server-side overload.
+
+        :param max_queue_time_seconds: Maximum time in seconds a request can be queued
+            on the server-side. If set to 0 or None, the server ignores this setting.
+        :type max_queue_time_seconds: Optional[float]
+        :return: Database API wrapper object specifically for queue bounded execution.
+        :rtype: arango.database.OverloadControlDatabase
+        """
+        return OverloadControlDatabase(self._conn, max_queue_time_seconds)
+
 
 class AsyncDatabase(Database):
     """Database API wrapper tailored specifically for async execution.
 
     See :func:`arango.database.StandardDatabase.begin_async_execution`.
 
     :param connection: HTTP connection.
@@ -2680,7 +2704,59 @@
         """Abort the transaction.
 
         :return: True if the abort operation was successful.
         :rtype: bool
         :raise arango.exceptions.TransactionAbortError: If abort fails.
         """
         return self._executor.abort()
+
+
+class OverloadControlDatabase(Database):
+    """Database API wrapper tailored to gracefully handle server overload scenarios.
+
+    See :func:`arango.database.StandardDatabase.begin_controlled_execution`.
+
+    :param connection: HTTP connection.
+    :param max_queue_time_seconds: Maximum server-side queuing time in seconds.
+        If the server-side queuing time exceeds the client's specified limit,
+        the request will be rejected.
+    :type max_queue_time_seconds: Optional[float]
+    """
+
+    def __init__(
+        self, connection: Connection, max_queue_time_seconds: Optional[float] = None
+    ) -> None:
+        self._executor: OverloadControlApiExecutor
+        super().__init__(
+            connection=connection,
+            executor=OverloadControlApiExecutor(connection, max_queue_time_seconds),
+        )
+
+    def __repr__(self) -> str:  # pragma: no cover
+        return f"<OverloadControlDatabase {self.name}>"
+
+    @property
+    def last_queue_time(self) -> float:
+        """Return the most recently recorded server-side queuing time in seconds.
+
+        :return: Server-side queuing time in seconds.
+        :rtype: float
+        """
+        return self._executor.queue_time_seconds
+
+    @property
+    def max_queue_time(self) -> Optional[float]:
+        """Return the maximum server-side queuing time in seconds.
+
+        :return: Maximum server-side queuing time in seconds.
+        :rtype: Optional[float]
+        """
+        return self._executor.max_queue_time_seconds
+
+    def adjust_max_queue_time(self, max_queue_time_seconds: Optional[float]) -> None:
+        """Adjust the maximum server-side queuing time in seconds.
+
+        :param max_queue_time_seconds: New maximum server-side queuing time
+            in seconds. Setting it to None disables the limit.
+        :type max_queue_time_seconds: Optional[float]
+        """
+        self._executor.max_queue_time_seconds = max_queue_time_seconds
```

### Comparing `python-arango-7.5.8/arango/errno.py` & `python-arango-7.5.9/arango/errno.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/exceptions.py` & `python-arango-7.5.9/arango/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,23 @@
     """Failed to retrieve batch job result."""
 
 
 class BatchExecuteError(ArangoServerError):
     """Failed to execute batch API request."""
 
 
+#########################################
+# Overload Control Execution Exceptions #
+#########################################
+
+
+class OverloadControlExecutorError(ArangoServerError):
+    """Failed to execute overload controlled API request."""
+
+
 #########################
 # Collection Exceptions #
 #########################
 
 
 class CollectionListError(ArangoServerError):
     """Failed to retrieve collections."""
```

### Comparing `python-arango-7.5.8/arango/executor.py` & `python-arango-7.5.9/arango/executor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 __all__ = [
     "ApiExecutor",
     "DefaultApiExecutor",
     "AsyncApiExecutor",
     "BatchApiExecutor",
     "TransactionApiExecutor",
+    "OverloadControlApiExecutor",
 ]
 
 from collections import OrderedDict
 from typing import Any, Callable, Optional, Sequence, Tuple, TypeVar, Union
 from urllib.parse import urlencode
 from uuid import uuid4
 
 from arango.connection import Connection
 from arango.exceptions import (
     AsyncExecuteError,
     BatchExecuteError,
     BatchStateError,
+    OverloadControlExecutorError,
     TransactionAbortError,
     TransactionCommitError,
     TransactionInitError,
     TransactionStatusError,
 )
 from arango.job import AsyncJob, BatchJob
 from arango.request import Request
@@ -28,14 +30,15 @@
 from arango.utils import suppress_warning
 
 ApiExecutor = Union[
     "DefaultApiExecutor",
     "AsyncApiExecutor",
     "BatchApiExecutor",
     "TransactionApiExecutor",
+    "OverloadControlApiExecutor",
 ]
 
 T = TypeVar("T")
 
 
 class DefaultApiExecutor:
     """Default API executor.
@@ -424,7 +427,88 @@
             endpoint=f"/_api/transaction/{self._id}",
         )
         resp = self._conn.send_request(request)
 
         if resp.is_success:
             return True
         raise TransactionAbortError(resp, request)
+
+
+class OverloadControlApiExecutor:
+    """Allows setting the maximum acceptable server-side queuing time
+        for client requests.
+
+    :param connection: HTTP connection.
+    :type connection: arango.connection.BasicConnection |
+        arango.connection.JwtConnection | arango.connection.JwtSuperuserConnection
+    :param max_queue_time_seconds: Maximum server-side queuing time in seconds.
+    :type max_queue_time_seconds: float
+    """
+
+    def __init__(
+        self, connection: Connection, max_queue_time_seconds: Optional[float] = None
+    ) -> None:
+        self._conn = connection
+        self._max_queue_time_seconds = max_queue_time_seconds
+        self._queue_time_seconds = 0.0
+
+    @property
+    def context(self) -> str:  # pragma: no cover
+        return "overload-control"
+
+    @property
+    def queue_time_seconds(self) -> float:
+        """Return the most recent request queuing/de-queuing time.
+            Defaults to 0 if no request has been sent.
+
+        :return: Server-side queuing time in seconds.
+        :rtype: float
+        """
+        return self._queue_time_seconds
+
+    @property
+    def max_queue_time_seconds(self) -> Optional[float]:
+        """Return the maximum server-side queuing time.
+
+        :return: Maximum server-side queuing time in seconds.
+        :rtype: Optional[float]
+        """
+        return self._max_queue_time_seconds
+
+    @max_queue_time_seconds.setter
+    def max_queue_time_seconds(self, value: Optional[float]) -> None:
+        """Set the maximum server-side queuing time.
+            Setting it to None disables the feature.
+
+        :param value: Maximum server-side queuing time in seconds.
+        :type value: Optional[float]
+        """
+        self._max_queue_time_seconds = value
+
+    def execute(
+        self,
+        request: Request,
+        response_handler: Callable[[Response], T],
+    ) -> T:
+        """Execute an API request and return the result.
+
+        :param request: HTTP request.
+        :type request: arango.request.Request
+        :param response_handler: HTTP response handler.
+        :type response_handler: callable
+        :return: API execution result.
+        """
+        if self._max_queue_time_seconds is not None:
+            request.headers["x-arango-queue-time-seconds"] = str(
+                self._max_queue_time_seconds
+            )
+        resp = self._conn.send_request(request)
+
+        if not resp.is_success:
+            raise OverloadControlExecutorError(resp, request)
+
+        if "X-Arango-Queue-Time-Seconds" in resp.headers:
+            self._queue_time_seconds = float(
+                resp.headers["X-Arango-Queue-Time-Seconds"]
+            )
+
+        return response_handler(resp)
```

### Comparing `python-arango-7.5.8/arango/formatter.py` & `python-arango-7.5.9/arango/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,48 @@
         result["storedValues"] = body["storedValues"]
     if "cacheEnabled" in body:
         result["cacheEnabled"] = body["cacheEnabled"]
     if "legacyPolygons" in body:
         result["legacyPolygons"] = body["legacyPolygons"]
     if "estimates" in body:
         result["estimates"] = body["estimates"]
+    if "analyzer" in body:
+        result["analyzer"] = body["analyzer"]
+    if "cleanupIntervalStep" in body:
+        result["cleanup_interval_step"] = body["cleanupIntervalStep"]
+        if "commitIntervalMsec" in body:
+            result["commit_interval_msec"] = body["commitIntervalMsec"]
+    if "consolidationIntervalMsec" in body:
+        result["consolidation_interval_msec"] = body["consolidationIntervalMsec"]
+    if "consolidationPolicy" in body:
+        result["consolidation_policy"] = format_view_consolidation_policy(
+            body["consolidationPolicy"]
+        )
+    if "features" in body:
+        result["features"] = body["features"]
+    if "includeAllFields" in body:
+        result["include_all_fields"] = body["includeAllFields"]
+    if "primarySort" in body:
+        result["primary_sort"] = body["primarySort"]
+    if "searchField" in body:
+        result["search_field"] = body["searchField"]
+    if "trackListPositions" in body:
+        result["track_list_positions"] = body["trackListPositions"]
+    if "version" in body:
+        result["version"] = body["version"]
+    if "cache" in body:
+        result["cache"] = body["cache"]
+    if "primaryKeyCache" in body:
+        result["primaryKeyCache"] = body["primaryKeyCache"]
+    if "writebufferIdle" in body:
+        result["writebuffer_idle"] = body["writebufferIdle"]
+    if "writebufferActive" in body:
+        result["writebuffer_active"] = body["writebufferActive"]
+    if "writebufferSizeMax" in body:
+        result["writebuffer_max_size"] = body["writebufferSizeMax"]
 
     return verify_format(body, result)
 
 
 def format_key_options(body: Json) -> Json:
     """Format collection key options data.
 
@@ -318,14 +352,18 @@
         result["started"] = body["started"]
     if "state" in body:
         result["state"] = body["state"]
     if "stream" in body:
         result["stream"] = body["stream"]
     if "user" in body:
         result["user"] = body["user"]
+
+    # New in 3.11
+    if "peakMemoryUsage" in body:
+        result["peak_memory_usage"] = body["peakMemoryUsage"]
     return verify_format(body, result)
 
 
 def format_aql_tracking(body: Json) -> Json:
     """Format AQL tracking data.
 
     :param body: Input body.
@@ -894,14 +932,24 @@
     if "writebufferSizeMax" in body:
         result["writebuffer_max_size"] = body["writebufferSizeMax"]
     if "links" in body:
         result["links"] = body["links"]
     if "indexes" in body:
         result["indexes"] = body["indexes"]
 
+    # Introduced in 3.9.6 EE
+    if "primaryKeyCache" in body:
+        result["primaryKeyCache"] = body["primaryKeyCache"]
+    if "primarySortCache" in body:
+        result["primarySortCache"] = body["primarySortCache"]
+
+    # Introduced in 3.12 EE
+    if "optimizeTopK" in body:
+        result["optimizeTopK"] = body["optimizeTopK"]
+
     return verify_format(body, result)
 
 
 def format_vertex(body: Json) -> Json:
     """Format vertex data.
 
     :param body: Input body.
```

### Comparing `python-arango-7.5.8/arango/foxx.py` & `python-arango-7.5.9/arango/foxx.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/graph.py` & `python-arango-7.5.9/arango/graph.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/job.py` & `python-arango-7.5.9/arango/job.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/pregel.py` & `python-arango-7.5.9/arango/pregel.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/replication.py` & `python-arango-7.5.9/arango/replication.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/request.py` & `python-arango-7.5.9/arango/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def normalize_headers(
     headers: Optional[Headers], driver_flags: Optional[DriverFlags] = None
 ) -> Headers:
     flags = ""
     if driver_flags is not None:
         for flag in driver_flags:
             flags = flags + flag + ";"
-    driver_version = "7.5.3"
+    driver_version = "7.5.8"
     driver_header = "python-arango/" + driver_version + " (" + flags + ")"
     normalized_headers: Headers = {
         "charset": "utf-8",
         "content-type": "application/json",
         "x-arango-driver": driver_header,
     }
     if headers is not None:
```

### Comparing `python-arango-7.5.8/arango/resolver.py` & `python-arango-7.5.9/arango/resolver.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/response.py` & `python-arango-7.5.9/arango/response.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/utils.py` & `python-arango-7.5.9/arango/utils.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/arango/wal.py` & `python-arango-7.5.9/arango/wal.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/Makefile` & `python-arango-7.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/admin.rst` & `python-arango-7.5.9/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/analyzer.rst` & `python-arango-7.5.9/docs/analyzer.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/aql.rst` & `python-arango-7.5.9/docs/aql.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/async.rst` & `python-arango-7.5.9/docs/async.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/auth.rst` & `python-arango-7.5.9/docs/auth.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/backup.rst` & `python-arango-7.5.9/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/batch.rst` & `python-arango-7.5.9/docs/batch.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/certificates.rst` & `python-arango-7.5.9/docs/certificates.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/cluster.rst` & `python-arango-7.5.9/docs/cluster.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/collection.rst` & `python-arango-7.5.9/docs/collection.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/conf.py` & `python-arango-7.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/contributing.rst` & `python-arango-7.5.9/docs/contributing.rst`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 =====
 
 To ensure PEP8_ compliance, run flake8_:
 
 .. code-block:: bash
 
     ~$ pip install flake8
-    ~$ git clone https://github.com/joowani/python-arango.git
+    ~$ git clone https://github.com/ArangoDB-Community/python-arango.git
     ~$ cd python-arango
     ~$ flake8
 
 If there is a good reason to ignore a warning, see here_ on how to exclude it.
 
 Testing
 =======
@@ -53,24 +53,24 @@
 **python-arango**. It uses pytest_ and requires an actual ArangoDB instance.
 
 To run the test suite (use your own host, port and root password):
 
 .. code-block:: bash
 
     ~$ pip install pytest
-    ~$ git clone https://github.com/joowani/python-arango.git
+    ~$ git clone https://github.com/ArangoDB-Community/python-arango.git
     ~$ cd python-arango
     ~$ py.test --complete --host=127.0.0.1 --port=8529 --passwd=passwd
 
 To run the test suite with coverage report:
 
 .. code-block:: bash
 
     ~$ pip install coverage pytest pytest-cov
-    ~$ git clone https://github.com/joowani/python-arango.git
+    ~$ git clone https://github.com/ArangoDB-Community/python-arango.git
     ~$ cd python-arango
     ~$ py.test --complete --host=127.0.0.1 --port=8529 --passwd=passwd --cov=kq
 
 As the test suite creates real databases and jobs, it should only be run in
 development environments.
 
 Documentation
@@ -78,17 +78,17 @@
 
 The documentation including the README is written in reStructuredText_ and uses
 Sphinx_. To build an HTML version on your local machine:
 
 .. code-block:: bash
 
     ~$ pip install sphinx sphinx_rtd_theme
-    ~$ git clone https://github.com/joowani/python-arango.git
-    ~$ cd python-arango/docs
-    ~$ sphinx-build . build  # Open build/index.html in a browser
+    ~$ git clone https://github.com/ArangoDB-Community/python-arango.git
+    ~$ cd python-arango
+    ~$ python -m sphinx -b html -W docs docs/_build/  # Open build/index.html in a browser
 
 As always, thank you for your contribution!
 
 .. _dev: https://github.com/joowani/python-arango/tree/dev
 .. _GitHub: https://github.com/joowani/python-arango
 .. _PEP8: https://www.python.org/dev/peps/pep-0008/
 .. _coverage: https://coveralls.io/github/joowani/python-arango
```

### Comparing `python-arango-7.5.8/docs/cursor.rst` & `python-arango-7.5.9/docs/cursor.rst`

 * *Files 25% similar despite different names*

```diff
@@ -112,7 +112,58 @@
 
     # Alternatively, you can manually fetch and pop for finer control.
     cursor = db.aql.execute('FOR doc IN students RETURN doc', batch_size=1)
     while cursor.has_more(): # Fetch until nothing is left on the server.
         cursor.fetch()
     while not cursor.empty(): # Pop until nothing is left on the cursor.
         cursor.pop()
+
+With ArangoDB 3.11.0 or higher, you can also use the `allow_retry`
+parameter of :func:`arango.aql.AQL.execute` to automatically retry
+the request if the cursor encountered any issues during the previous
+fetch operation. Note that this feature causes the server to cache the
+last batch. To allow re-fetching of the very last batch of the query,
+the server cannot automatically delete the cursor. Once you have successfully
+received the last batch, you should call :func:`arango.cursor.Cursor.close`.
+
+**Example:**
+
+.. code-block:: python
+
+    from arango import ArangoClient
+
+    # Initialize the ArangoDB client.
+    client = ArangoClient()
+
+    # Connect to "test" database as root user.
+    db = client.db('test', username='root', password='passwd')
+
+    # Set up some test data to query against.
+    db.collection('students').insert_many([
+        {'_key': 'Abby', 'age': 22},
+        {'_key': 'John', 'age': 18},
+        {'_key': 'Mary', 'age': 21},
+        {'_key': 'Suzy', 'age': 23},
+        {'_key': 'Dave', 'age': 20}
+    ])
+
+    # Execute an AQL query which returns a cursor object.
+    cursor = db.aql.execute(
+        'FOR doc IN students FILTER doc.age > @val RETURN doc',
+        bind_vars={'val': 17},
+        batch_size=2,
+        count=True,
+        allow_retry=True
+    )
+
+    while cursor.has_more():
+        try:
+            cursor.fetch()
+        except ConnectionError:
+            # Retry the request.
+            continue
+
+    while not cursor.empty():
+        cursor.pop()
+
+    # Delete the cursor from the server.
+    cursor.close()
```

### Comparing `python-arango-7.5.8/docs/database.rst` & `python-arango-7.5.9/docs/database.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/document.rst` & `python-arango-7.5.9/docs/document.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/errors.rst` & `python-arango-7.5.9/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/foxx.rst` & `python-arango-7.5.9/docs/foxx.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/graph.rst` & `python-arango-7.5.9/docs/graph.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/http.rst` & `python-arango-7.5.9/docs/http.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/index.rst` & `python-arango-7.5.9/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 -------------
 
 Welcome to the documentation for **python-arango**, a Python driver for ArangoDB_.
 
 Requirements
 =============
 
-- ArangoDB version 3.7+
+- ArangoDB version 3.9+
 - Python version 3.8+
 
 Installation
 ============
 
 .. code-block:: bash
 
@@ -34,14 +34,15 @@
     indexes
     graph
     aql
     simple
     cursor
     async
     batch
+    overload
     transaction
     admin
     user
     task
     wal
     pregel
     foxx
```

### Comparing `python-arango-7.5.8/docs/indexes.rst` & `python-arango-7.5.9/docs/indexes.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/logging.rst` & `python-arango-7.5.9/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/make.bat` & `python-arango-7.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/overview.rst` & `python-arango-7.5.9/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/pregel.rst` & `python-arango-7.5.9/docs/pregel.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/replication.rst` & `python-arango-7.5.9/docs/replication.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/schema.rst` & `python-arango-7.5.9/docs/schema.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/serializer.rst` & `python-arango-7.5.9/docs/serializer.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/simple.rst` & `python-arango-7.5.9/docs/simple.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/specs.rst` & `python-arango-7.5.9/docs/specs.rst`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,23 @@
 
 HTTPClient
 ==========
 
 .. autoclass:: arango.http.HTTPClient
     :members:
 
+.. _OverloadControlDatabase:
+
+OverloadControlDatabase
+=======================
+
+.. autoclass:: arango.database.OverloadControlDatabase
+    :inherited-members:
+    :members:
+
 .. _Pregel:
 
 Pregel
 ======
 
 .. autoclass:: arango.pregel.Pregel
     :members:
```

### Comparing `python-arango-7.5.8/docs/static/logo.png` & `python-arango-7.5.9/docs/static/logo.png`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/task.rst` & `python-arango-7.5.9/docs/task.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/threading.rst` & `python-arango-7.5.9/docs/threading.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/transaction.rst` & `python-arango-7.5.9/docs/transaction.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/user.rst` & `python-arango-7.5.9/docs/user.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/view.rst` & `python-arango-7.5.9/docs/view.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/docs/wal.rst` & `python-arango-7.5.9/docs/wal.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/pyproject.toml` & `python-arango-7.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.8/python_arango.egg-info/PKG-INFO` & `python-arango-7.5.9/python_arango.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-arango
-Version: 7.5.8
+Version: 7.5.9
 Summary: Python Driver for ArangoDB
 Home-page: https://github.com/ArangoDB-Community/python-arango
 Author: Joohwan Oh
 Author-email: joohwan.oh@outlook.com
 License: MIT
 Keywords: arangodb,python,driver
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,15 @@
 # Python-Arango
 
 Python driver for [ArangoDB](https://www.arangodb.com), a scalable multi-model
 database natively supporting documents, graphs and search.
 
 ## Requirements
 
-- ArangoDB version 3.7+
+- ArangoDB version 3.9+
 - Python version 3.8+
 
 ## Installation
 
 ```shell
 pip install python-arango --upgrade
 ```
```

### Comparing `python-arango-7.5.8/python_arango.egg-info/SOURCES.txt` & `python-arango-7.5.9/python_arango.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .pre-commit-config.yaml
+CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
@@ -61,14 +62,15 @@
 docs/foxx.rst
 docs/graph.rst
 docs/http.rst
 docs/index.rst
 docs/indexes.rst
 docs/logging.rst
 docs/make.bat
+docs/overload.rst
 docs/overview.rst
 docs/pregel.rst
 docs/replication.rst
 docs/schema.rst
 docs/serializer.rst
 docs/simple.rst
 docs/specs.rst
```

### Comparing `python-arango-7.5.8/setup.py` & `python-arango-7.5.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     install_requires=[
         "urllib3>=1.26.0",
         "requests",
         "requests_toolbelt",
         "PyJWT",
         "setuptools>=42",
         "importlib_metadata>=4.7.1",
+        "packaging>=23.1",
     ],
     extras_require={
         "dev": [
             "black>=22.3.0",
             "flake8>=4.0.1",
             "isort>=5.10.1",
             "mypy>=0.942",
```

### Comparing `python-arango-7.5.8/tester.sh` & `python-arango-7.5.9/tester.sh`

 * *Files 5% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 # Tests python-arango driver against a local ArangoDB single server or cluster setup.
 # 1. Starts a local ArangoDB server or cluster (community).
 # 2. Runs the python-arango tests for the community edition.
 # 3. Starts a local ArangoDB server or cluster (enterprise).
 # 4. Runs all python-arango tests, including enterprise tests.
 
 # Usage:
-#   ./start.sh [all|single|cluster] [all|community|enterprise] [version] ["notest"]
+#   ./tester.sh [all|single|cluster] [all|community|enterprise] [version] ["notest"]
 
 setup="${1:-all}"
 if [[ "$setup" != "all" && "$setup" != "single" && "$setup" != "cluster" ]]; then
     echo "Invalid argument. Please provide either 'all', 'single' or 'cluster'."
     exit 1
 fi
 
 tests="${2:-all}"
 if [[ "$tests" != "all" && "$tests" != "community" && "$tests" != "enterprise" ]]; then
     echo "Invalid argument. Please provide either 'all', 'community', or 'enterprise'."
     exit 1
 fi
 
-version="${3:-3.10.6}"
+# 3.11.1
+# 3.10.9
+# 3.9.9
+version="${3:-3.11.1}"
 
 if [[ -n "$4" && "$4" != "notest" ]]; then
     echo "Invalid argument. Use 'notest' to only start the docker container, without running the tests."
     exit 1
 fi
 mode="${4:-test}"
```

