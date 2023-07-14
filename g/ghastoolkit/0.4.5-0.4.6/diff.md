# Comparing `tmp/ghastoolkit-0.4.5.tar.gz` & `tmp/ghastoolkit-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.4.5.tar", last modified: Thu Jul 13 17:06:51 2023, max compression
+gzip compressed data, was "ghastoolkit-0.4.6.tar", last modified: Fri Jul 14 10:34:40 2023, max compression
```

## Comparing `ghastoolkit-0.4.5.tar` & `ghastoolkit-0.4.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.137151 ghastoolkit-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 17:06:51.137151 ghastoolkit-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:06:51.137151 ghastoolkit-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.125151 ghastoolkit-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.125151 ghastoolkit-0.4.5/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.129151 ghastoolkit-0.4.5/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.129151 ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.133151 ghastoolkit-0.4.5/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.133151 ghastoolkit-0.4.5/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.133151 ghastoolkit-0.4.5/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.133151 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.129151 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 17:06:51.000000 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-13 17:06:51.000000 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:06:51.000000 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-13 17:06:51.000000 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 17:06:51.000000 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.137151 ghastoolkit-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.633011 ghastoolkit-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-14 10:34:40.633011 ghastoolkit-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:34:40.633011 ghastoolkit-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.625011 ghastoolkit-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/codeql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.629011 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-14 10:34:40.000000 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-14 10:34:40.000000 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:34:40.000000 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-14 10:34:40.000000 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 10:34:40.000000 ghastoolkit-0.4.6/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:34:40.633011 ghastoolkit-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-14 10:34:07.000000 ghastoolkit-0.4.6/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.4.5/LICENSE` & `ghastoolkit-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/PKG-INFO` & `ghastoolkit-0.4.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.5
+Version: 0.4.6
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,46 +12,55 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GHAS Toolkit
-
 <div align="center">
+<h1>GHASToolkit</h1>
+<img src="https://raw.githubusercontent.com/GeekMasher/ghastoolkit/main/docs/static/ghastoolkit.png" />
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/GeekMasher/ghastoolkit)
 [![GitHub Actions](https://img.shields.io/github/actions/workflow/status/geekmasher/ghastoolkit/python-package.yml?style=for-the-badge)](https://github.com/GeekMasher/ghastoolkit/actions/workflows/python-package.yml?query=branch%3Amain)
 [![GitHub Issues](https://img.shields.io/github/issues/geekmasher/ghastoolkit?style=for-the-badge)](https://github.com/GeekMasher/ghastoolkit/issues)
 [![GitHub Stars](https://img.shields.io/github/stars/geekmasher/ghastoolkit?style=for-the-badge)](https://github.com/GeekMasher/ghastoolkit)
 [![Python Versions](https://img.shields.io/pypi/pyversions/ghastoolkit?style=for-the-badge)](https://pypi.org/project/ghastoolkit/)
 [![Licence](https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge)](./LICENSE)
 
 </div>
 
 ## Overview
 
 [GitHub Advanced Security (GHAS)](https://github.com/features/security) Python Toolkit to make the lives of everyone that uses GHAS a little easier.
 
-## Installing 
 
-**Pip:**
+## Installing
+
+To install `ghastoolkit`, you can use `pip` or one of `pypi` family's of tools to install:
 
 ```bash
+# pip 
 pip install ghastoolkit
-```
 
-**Pipenv:**
-
-```bash
+# pipenv
 pipenv install ghastoolkit
+
+# poetry
+poetry add ghastoolkit
 ```
 
-## Usage 
+## Usage
 
-```python
-from ghastoolkit import GitHub
+To see how to use `ghastoolkit`, [take a look at the docs](https://geekmasher.github.io/ghastoolkit).
 
-GitHub.init("GeekMasher/ghastoolkit")
-```
+
+## Licence
+
+This project is licensed under the terms of the MIT open source license.
+Please refer to [MIT](./LICENSE.md) for the full terms.
+
+
+## Support
+
+Support is via [GitHub Issues](https://github.com/GeekMasher/ghastoolkit/issues)
```

### Comparing `ghastoolkit-0.4.5/README.md` & `ghastoolkit-0.4.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,48 @@
-# GHAS Toolkit
-
 <div align="center">
+<h1>GHASToolkit</h1>
+<img src="https://raw.githubusercontent.com/GeekMasher/ghastoolkit/main/docs/static/ghastoolkit.png" />
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/GeekMasher/ghastoolkit)
 [![GitHub Actions](https://img.shields.io/github/actions/workflow/status/geekmasher/ghastoolkit/python-package.yml?style=for-the-badge)](https://github.com/GeekMasher/ghastoolkit/actions/workflows/python-package.yml?query=branch%3Amain)
 [![GitHub Issues](https://img.shields.io/github/issues/geekmasher/ghastoolkit?style=for-the-badge)](https://github.com/GeekMasher/ghastoolkit/issues)
 [![GitHub Stars](https://img.shields.io/github/stars/geekmasher/ghastoolkit?style=for-the-badge)](https://github.com/GeekMasher/ghastoolkit)
 [![Python Versions](https://img.shields.io/pypi/pyversions/ghastoolkit?style=for-the-badge)](https://pypi.org/project/ghastoolkit/)
 [![Licence](https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge)](./LICENSE)
 
 </div>
 
 ## Overview
 
 [GitHub Advanced Security (GHAS)](https://github.com/features/security) Python Toolkit to make the lives of everyone that uses GHAS a little easier.
 
-## Installing 
 
-**Pip:**
+## Installing
+
+To install `ghastoolkit`, you can use `pip` or one of `pypi` family's of tools to install:
 
 ```bash
+# pip 
 pip install ghastoolkit
-```
 
-**Pipenv:**
-
-```bash
+# pipenv
 pipenv install ghastoolkit
+
+# poetry
+poetry add ghastoolkit
 ```
 
-## Usage 
+## Usage
 
-```python
-from ghastoolkit import GitHub
+To see how to use `ghastoolkit`, [take a look at the docs](https://geekmasher.github.io/ghastoolkit).
 
-GitHub.init("GeekMasher/ghastoolkit")
-```
+
+## Licence
+
+This project is licensed under the terms of the MIT open source license.
+Please refer to [MIT](./LICENSE.md) for the full terms.
+
+
+## Support
+
+Support is via [GitHub Issues](https://github.com/GeekMasher/ghastoolkit/issues)
```

### Comparing `ghastoolkit-0.4.5/pyproject.toml` & `ghastoolkit-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.4.5"
+version = "0.4.6"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/__init__.py` & `ghastoolkit-0.4.6/src/ghastoolkit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.4.5"
+__version__ = "0.4.6"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
@@ -37,11 +37,11 @@
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
 from ghastoolkit.supplychain.dependencies import Dependency, Dependencies
 from ghastoolkit.supplychain.licensing import Licenses
 
 # CodeQL
 from ghastoolkit.codeql.databases import CodeQLDatabases, CodeQLDatabase
 from ghastoolkit.codeql.cli import CodeQL
-from ghastoolkit.codeql.results import CodeQLResults
+from ghastoolkit.codeql.results import CodeQLResults, CodeLocation, CodeResult
 
 # CodeQL Data Extensions / Models as Data
 from ghastoolkit.codeql.dataextensions.ext import DataExtensions
```

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/__main__.py` & `ghastoolkit-0.4.6/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.4.6/src/ghastoolkit/codeql/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,95 @@
 import json
 import logging
 import os
 import subprocess
 from sys import stdout
 import tempfile
-from typing import Optional
+from typing import Optional, Union
 
 from ghastoolkit.codeql.databases import CodeQLDatabase
 from ghastoolkit.codeql.results import CodeQLResults
 from ghastoolkit.codeql.utils import findCodeBinary
 
 
 logger = logging.getLogger("ghastoolkit.codeql.cli")
 
 
 class CodeQL:
+    """CodeQL CLI"""
+
     def __init__(self, binary: Optional[str] = None) -> None:
         if binary:
             self.path_binary = [binary]
         else:
             self.path_binary: Optional[list[str]] = findCodeBinary()
 
     def exists(self) -> bool:
+        """
+        Check codeql is present on the system
+        """
         return self.path_binary != None
 
     def runCommand(self, *argvs, display: bool = False) -> Optional[str]:
+        """Run CodeQL command without the binary / path"""
         if not self.path_binary:
             raise Exception("CodeQL binary / path was not found")
         cmd = []
         cmd.extend(self.path_binary)
         cmd.extend(argvs)
+
+        if argvs[0] == "database":
+            cmd.extend(["--threads", "0", "--ram", "0"])
+
         if not display:
             with open(os.devnull, "w") as null:
                 result = subprocess.run(cmd, stdout=null, stderr=null)
         else:
             result = subprocess.check_output(cmd)
             return result.decode().strip()
 
     @property
     def version(self) -> str:
+        """Get CodeQL Version"""
         return self.runCommand("version", "--format", "terse", display=True)
 
     def runQuery(
         self, database: CodeQLDatabase, path: Optional[str] = None
     ) -> CodeQLResults:
+        """Runs Query on a CodeQL Database"""
         if not database.path:
             raise Exception("CodeQL Database path is not set")
 
         path = path or database.default_pack
 
         self.runCommand("database", "run-queries", database.path, path)
         return self.getResults(database, path)
 
-    def runRawQuery(self, path: str, database: CodeQLDatabase) -> list:
+    def runRawQuery(
+        self, path: str, database: CodeQLDatabase, outputtype: str = "bqrs"
+    ) -> Union[dict, list]:
+        """Run raw query"""
         if not database.path:
             raise Exception("CodeQL Database path is not set")
         if not path.endswith(".ql"):
             raise Exception("runRawQuery requires a QL file")
 
         self.runCommand("database", "run-queries", database.path, path)
-        bqrs = os.path.join(
-            database.path, "results", path.replace(":", "/").replace(".ql", ".bqrs")
-        )
-        return self.readBqrs(bqrs).get("#select", {}).get("tuples", [])
+        if outputtype == "bqrs":
+            bqrs = os.path.join(
+                database.path, "results", path.replace(":", "/").replace(".ql", ".bqrs")
+            )
+            return self.readBqrs(bqrs)
+        else:
+            return
 
     def getResults(
         self, database: CodeQLDatabase, path: Optional[str] = None
     ) -> CodeQLResults:
+        """Get interpret results from CodeQL"""
         sarif = os.path.join(tempfile.gettempdir(), "codeql-result.sarif")
         cmd = [
             "database",
             "interpret-results",
             "--format",
             "sarif-latest",
             "--output",
@@ -85,14 +104,15 @@
         with open(sarif, "r") as handle:
             data = json.load(handle)
 
         results = data.get("runs", [])[0].get("results", [])
         return CodeQLResults.loadSarifResults(results)
 
     def readBqrs(self, bqrsfile: str) -> dict:
+        """Read BQRS"""
         output = os.path.join(tempfile.gettempdir(), "codeql-result.bqrs")
 
         self.runCommand(
             "bqrs", "decode", "--format", "json", "--output", output, bqrsfile
         )
 
         with open(output, "r") as handle:
```

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.4.6/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.4.6/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.4.6/src/ghastoolkit/codeql/results.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 from dataclasses import dataclass, field
 from typing import Optional
 
 
 @dataclass
 class CodeLocation:
+    """Code Location Module"""
+
     uri: str
+    """URI to the location where the result occurs"""
 
     start_line: int
+    """Start line of the result"""
     start_column: Optional[int] = None
+    """Start column of the result"""
     end_line: Optional[int] = None
+    """End line of the result"""
     end_column: Optional[int] = None
+    """End line of the result"""
 
     def __str__(self) -> str:
         return f"{self.uri}#{self.start_line}"
 
 
 @dataclass
 class CodeResult:
+    """Code Result"""
+
     rule_id: str
+    """Rule ID"""
     message: str
+    """Message of the result"""
 
     locations: list[CodeLocation] = field(default_factory=list)
+    """Locations of the results"""
 
     def __str__(self) -> str:
         if len(self.locations) == 1:
             return f"CodeResult('{self.rule_id}', '{self.locations[0]}')"
         return f"CodeResult('{self.rule_id}', {len(self.locations)})"
 
     @staticmethod
     def loadSarifLocations(data: list[dict]) -> list["CodeLocation"]:
+        """Load SARIF Locations"""
         locations = []
         for loc in data:
             physical = loc.get("physicalLocation", {})
             region = physical.get("region", {})
             locations.append(
                 CodeLocation(
                     physical.get("artifactLocation", {}).get("uri", ""),
@@ -42,16 +55,19 @@
                     end_column=region.get("endColumn"),
                 )
             )
         return locations
 
 
 class CodeQLResults(list):
+    """CodeQL Results"""
+
     @staticmethod
     def loadSarifResults(results: list[dict]) -> "CodeQLResults":
+        """Load SARIF Results"""
         result = CodeQLResults()
 
         for alert in results:
             result.append(
                 CodeResult(
                     alert.get("ruleId", "NA"),
                     alert.get("message", {}).get("text", "NA"),
```

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.4.6/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.4.6/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.4.6/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.4.6/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.4.6/src/ghastoolkit/octokit/github.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,33 @@
 
 
 logger = logging.getLogger("ghastoolkit.octokit.github")
 
 
 @dataclass
 class Repository:
+    """GitHub Repository"""
+
     owner: str
+    """Owner"""
     repo: str
+    """Repository name"""
 
     reference: Optional[str] = None
+    """Reference (`refs/heads/main`)"""
     branch: Optional[str] = None
+    """Branch / Tab name"""
+
     __prinfo__: Optional[dict] = None
 
     sha: Optional[str] = None
+    """Git SHA"""
 
     clone_path: Optional[str] = None
+    """Clone Path"""
 
     def __post_init__(self) -> None:
         if self.reference and not self.branch:
             if not self.isInPullRequest():
                 _, _, branch = self.reference.split("/", 2)
                 self.branch = branch
         if self.branch and not self.reference:
@@ -86,14 +95,15 @@
             )
             for commit in response:
                 result.append(commit.get("sha"))
         return result
 
     @property
     def clone_url(self) -> str:
+        """Repository clone URL"""
         if GitHub.github_app:
             url = urlparse(GitHub.instance)
             return f"{url.scheme}://x-access-token:{GitHub.token}@{url.netloc}/{self.owner}/{self.repo}.git"
         elif GitHub.token:
             url = urlparse(GitHub.instance)
             return f"{url.scheme}://{GitHub.token}@{url.netloc}/{self.owner}/{self.repo}.git"
         return f"{GitHub.instance}/{self.owner}/{self.repo}.git"
@@ -132,79 +142,96 @@
         cmd = self._cloneCmd(self.clone_path, depth=depth)
         logger.debug(f"Cloning Command :: {cmd}")
 
         with open(os.devnull, "w") as null:
             subprocess.check_call(cmd, stdout=null, stderr=null)
 
     def gitsha(self) -> str:
+        """Get the Git SHA"""
         cmd = ["git", "rev-parse", "HEAD"]
         result = (
             subprocess.check_output(cmd, cwd=self.clone_path).decode("ascii").strip()
         )
         return result
 
     def getFile(self, path: str) -> str:
         """Get a path relative from the base of the cloned repository"""
         if not self.clone_path:
             raise Exception(f"Unknown clone path")
         return os.path.join(self.clone_path, path)
 
-    def display(self):
+    def display(self) -> str:
+        """Display the repository as a string"""
         if self.reference:
             return f"{self.owner}/{self.repo}@{self.reference}"
         return f"{self.owner}/{self.repo}"
 
     @staticmethod
     def parseRepository(name: str) -> "Repository":
+        """Parse the repository name"""
         ref = None
         branch = None
         if "@" in name:
             name, branch = name.split("@", 1)
             ref = f"refs/heads/{branch}"
 
         owner, repo = name.split("/", 1)
         return Repository(owner, repo, reference=ref, branch=branch)
 
 
 class GitHub:
+    """The GitHub class is used to configure the state for all Octokit
+    apis. Its a standard interface across all projects.
+    """
+
     repository: Repository = Repository("GeekMasher", "ghastoolkit")
+    """Repository"""
     token: Optional[str] = None
+    """GitHub Access Token"""
 
     # URLs
     instance: str = "https://github.com"
+    """Instance"""
     api_rest: str = "https://api.github.com"
+    """REST API URL"""
     api_graphql: str = "https://api.github.com/graphql"
+    """GraphQL API URL"""
 
     enterprise: Optional[str] = None
 
     github_app: bool = False
+    """GitHub App setting"""
 
     @staticmethod
     def init(
         repository: Optional[str] = None,
         owner: Optional[str] = None,
         repo: Optional[str] = None,
         reference: Optional[str] = None,
         branch: Optional[str] = None,
-        token: Optional[str] = os.environ.get("GITHUB_TOKEN"),
+        token: Optional[str] = None,
         instance: Optional[str] = None,
         enterprise: Optional[str] = None,
     ) -> None:
+        """Initialise a GitHub class using a number of properties"""
         if repository:
             GitHub.repository = Repository.parseRepository(repository)
         elif owner and repo:
             GitHub.repository = Repository(owner, repo)
 
         if GitHub.repository:
             if reference:
                 GitHub.repository.reference = reference
             if branch:
                 GitHub.repository.branch = branch
 
+        if not token:
+            token = os.environ.get("GITHUB_TOKEN")
         GitHub.token = token
+
         # instance
         if instance:
             GitHub.instance = instance
             GitHub.api_rest, GitHub.api_graphql = GitHub.parseInstance(instance)
 
         GitHub.enterprise = enterprise
 
@@ -222,8 +249,9 @@
         # GitHub Ent Server
         api = url.scheme + "://" + url.netloc + "/api/v3"
 
         return (api, f"{api}/graphql")
 
     @staticmethod
     def display() -> str:
+        """Display the GitHub Settings"""
         return f"GitHub('{GitHub.repository.display()}', '{GitHub.instance}')"
```

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.4.6/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.4.6/src/ghastoolkit/octokit/octokit.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 
                     elif not argv_value and len(defaults) < 0:
                         argv_value = defaults[len(defaults) - args_index]
 
                     params[argv] = argv_value
                     args_index += 1
 
+                # print(f"Request parameters :: '{params}'")
                 result = rest.get(url, parameters=params, authenticated=authenticated)
 
                 if response:
                     return func(self, responce=result, **kwargs)
 
                 # TODO: runtime type checking
```

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.4.6/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.4.6/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.4.6/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.4.6/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.4.6/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.4.6/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.5
+Version: 0.4.6
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,46 +12,55 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GHAS Toolkit
-
 <div align="center">
+<h1>GHASToolkit</h1>
+<img src="https://raw.githubusercontent.com/GeekMasher/ghastoolkit/main/docs/static/ghastoolkit.png" />
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/GeekMasher/ghastoolkit)
 [![GitHub Actions](https://img.shields.io/github/actions/workflow/status/geekmasher/ghastoolkit/python-package.yml?style=for-the-badge)](https://github.com/GeekMasher/ghastoolkit/actions/workflows/python-package.yml?query=branch%3Amain)
 [![GitHub Issues](https://img.shields.io/github/issues/geekmasher/ghastoolkit?style=for-the-badge)](https://github.com/GeekMasher/ghastoolkit/issues)
 [![GitHub Stars](https://img.shields.io/github/stars/geekmasher/ghastoolkit?style=for-the-badge)](https://github.com/GeekMasher/ghastoolkit)
 [![Python Versions](https://img.shields.io/pypi/pyversions/ghastoolkit?style=for-the-badge)](https://pypi.org/project/ghastoolkit/)
 [![Licence](https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge)](./LICENSE)
 
 </div>
 
 ## Overview
 
 [GitHub Advanced Security (GHAS)](https://github.com/features/security) Python Toolkit to make the lives of everyone that uses GHAS a little easier.
 
-## Installing 
 
-**Pip:**
+## Installing
+
+To install `ghastoolkit`, you can use `pip` or one of `pypi` family's of tools to install:
 
 ```bash
+# pip 
 pip install ghastoolkit
-```
 
-**Pipenv:**
-
-```bash
+# pipenv
 pipenv install ghastoolkit
+
+# poetry
+poetry add ghastoolkit
 ```
 
-## Usage 
+## Usage
 
-```python
-from ghastoolkit import GitHub
+To see how to use `ghastoolkit`, [take a look at the docs](https://geekmasher.github.io/ghastoolkit).
 
-GitHub.init("GeekMasher/ghastoolkit")
-```
+
+## Licence
+
+This project is licensed under the terms of the MIT open source license.
+Please refer to [MIT](./LICENSE.md) for the full terms.
+
+
+## Support
+
+Support is via [GitHub Issues](https://github.com/GeekMasher/ghastoolkit/issues)
```

### Comparing `ghastoolkit-0.4.5/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.4.6/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/tests/test_codeql_dataext.py` & `ghastoolkit-0.4.6/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/tests/test_codeqldb.py` & `ghastoolkit-0.4.6/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/tests/test_codescanning.py` & `ghastoolkit-0.4.6/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/tests/test_default.py` & `ghastoolkit-0.4.6/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/tests/test_dependencies.py` & `ghastoolkit-0.4.6/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/tests/test_depgraph.py` & `ghastoolkit-0.4.6/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/tests/test_github.py` & `ghastoolkit-0.4.6/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/tests/test_licenses.py` & `ghastoolkit-0.4.6/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/tests/test_octokit.py` & `ghastoolkit-0.4.6/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.5/tests/test_secretscanning.py` & `ghastoolkit-0.4.6/tests/test_secretscanning.py`

 * *Files identical despite different names*

