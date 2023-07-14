# Comparing `tmp/ghastoolkit-0.4.6.tar.gz` & `tmp/ghastoolkit-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.4.6.tar", last modified: Fri Jul 14 10:34:40 2023, max compression
+gzip compressed data, was "ghastoolkit-0.4.7.tar", last modified: Fri Jul 14 12:47:52 2023, max compression
```

## Comparing `ghastoolkit-0.4.6.tar` & `ghastoolkit-0.4.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.633011 ghastoolkit-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-14 10:34:40.633011 ghastoolkit-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:34:40.633011 ghastoolkit-0.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.625011 ghastoolkit-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-14 10:34:40.000000 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-14 10:34:40.000000 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:34:40.000000 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-14 10:34:40.000000 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 10:34:40.000000 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.633011 ghastoolkit-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.464295 ghastoolkit-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-14 12:47:52.464295 ghastoolkit-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:47:52.464295 ghastoolkit-0.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.444294 ghastoolkit-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.448294 ghastoolkit-0.4.7/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.452294 ghastoolkit-0.4.7/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.456295 ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.456295 ghastoolkit-0.4.7/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.456295 ghastoolkit-0.4.7/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.460295 ghastoolkit-0.4.7/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.460295 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.452294 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-14 12:47:52.000000 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-14 12:47:52.000000 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:47:52.000000 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-14 12:47:52.000000 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 12:47:52.000000 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.464295 ghastoolkit-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.4.6/LICENSE` & `ghastoolkit-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/PKG-INFO` & `ghastoolkit-0.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.6
+Version: 0.4.7
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.4.6/README.md` & `ghastoolkit-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/pyproject.toml` & `ghastoolkit-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.4.6"
+version = "0.4.7"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/__init__.py` & `ghastoolkit-0.4.7/src/ghastoolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.4.6"
+__version__ = "0.4.7"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/__main__.py` & `ghastoolkit-0.4.7/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.4.7/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.4.7/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.4.7/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.4.7/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.4.7/src/ghastoolkit/octokit/codescanning.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     @property
     def tool_fullname(self) -> str:
         version = self.tool.get("version")
         return f"{self.tool_name}@{version}"
 
     @property
     def severity(self) -> str:
-        return self.rule.get("severity", "NA")
+        return self.rule.get("security_severity_level", "NA")
 
     @property
     def instances(self) -> list[dict]:
         if not self._instances:
             self._instances = CodeScanning().getAlertInstances(self.number)
         return self._instances
```

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.4.7/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.4.7/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.4.7/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.4.7/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.4.7/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.4.7/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.4.7/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.4.7/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.4.7/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.4.7/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.4.7/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.6
+Version: 0.4.7
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.4.6/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.4.7/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/tests/test_codeql_dataext.py` & `ghastoolkit-0.4.7/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/tests/test_codeqldb.py` & `ghastoolkit-0.4.7/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/tests/test_codescanning.py` & `ghastoolkit-0.4.7/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/tests/test_default.py` & `ghastoolkit-0.4.7/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/tests/test_dependencies.py` & `ghastoolkit-0.4.7/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/tests/test_depgraph.py` & `ghastoolkit-0.4.7/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/tests/test_github.py` & `ghastoolkit-0.4.7/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/tests/test_licenses.py` & `ghastoolkit-0.4.7/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/tests/test_octokit.py` & `ghastoolkit-0.4.7/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.6/tests/test_secretscanning.py` & `ghastoolkit-0.4.7/tests/test_secretscanning.py`

 * *Files identical despite different names*

