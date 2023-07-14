# Comparing `tmp/lib_list-1.1.7.tar.gz` & `tmp/lib_list-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_list-1.1.7.tar", last modified: Thu Jul 13 18:40:25 2023, max compression
+gzip compressed data, was "lib_list-1.1.8.tar", last modified: Fri Jul 14 12:38:42 2023, max compression
```

## Comparing `lib_list-1.1.7.tar` & `lib_list-1.1.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.060002 lib_list-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 18:39:34.000000 lib_list-1.1.7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.056002 lib_list-1.1.7/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 18:39:34.000000 lib_list-1.1.7/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 18:39:34.000000 lib_list-1.1.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.052002 lib_list-1.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.056002 lib_list-1.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 18:39:34.000000 lib_list-1.1.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-13 18:39:34.000000 lib_list-1.1.7/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 18:39:34.000000 lib_list-1.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-13 18:39:34.000000 lib_list-1.1.7/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 18:39:34.000000 lib_list-1.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 18:39:34.000000 lib_list-1.1.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 18:39:34.000000 lib_list-1.1.7/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 18:39:34.000000 lib_list-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 18:39:34.000000 lib_list-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 18:39:34.000000 lib_list-1.1.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-13 18:40:25.060002 lib_list-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 18:39:34.000000 lib_list-1.1.7/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-07-13 18:39:34.000000 lib_list-1.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 18:39:34.000000 lib_list-1.1.7/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.056002 lib_list-1.1.7/lib_list/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.060002 lib_list-1.1.7/lib_list/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/lib_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/lib_list_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.060002 lib_list-1.1.7/lib_list.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 18:40:25.000000 lib_list-1.1.7/lib_list.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 18:39:34.000000 lib_list-1.1.7/lib_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-13 18:39:34.000000 lib_list-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 18:39:34.000000 lib_list-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 18:39:34.000000 lib_list-1.1.7/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:40:25.060002 lib_list-1.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.060002 lib_list-1.1.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:40:25.060002 lib_list-1.1.7/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-13 18:39:34.000000 lib_list-1.1.7/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.867275 lib_list-1.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 12:37:55.000000 lib_list-1.1.8/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 12:37:55.000000 lib_list-1.1.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 12:37:55.000000 lib_list-1.1.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.851275 lib_list-1.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 12:37:55.000000 lib_list-1.1.8/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-14 12:37:55.000000 lib_list-1.1.8/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 12:37:55.000000 lib_list-1.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-14 12:37:55.000000 lib_list-1.1.8/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 12:37:55.000000 lib_list-1.1.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 12:37:55.000000 lib_list-1.1.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 12:37:55.000000 lib_list-1.1.8/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 12:37:55.000000 lib_list-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 12:37:55.000000 lib_list-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 12:37:55.000000 lib_list-1.1.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-14 12:38:42.867275 lib_list-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 12:37:55.000000 lib_list-1.1.8/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-07-14 12:37:55.000000 lib_list-1.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 12:37:55.000000 lib_list-1.1.8/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/lib_list/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list/lib_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list/lib_list_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/lib_list.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-14 12:37:55.000000 lib_list-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 12:37:55.000000 lib_list-1.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 12:37:55.000000 lib_list-1.1.8/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:38:42.867275 lib_list-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.867275 lib_list-1.1.8/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/test_cli.py
```

### Comparing `lib_list-1.1.7/.coveragerc` & `lib_list-1.1.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/.docs/README_template.rst` & `lib_list-1.1.8/.docs/README_template.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_list
 ========
 
 
-Version v1.1.7 as of 2023-07-13 see `Changelog`_
+Version v1.1.8 as of 2023-07-14 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `lib_list-1.1.7/.docs/badges.rst` & `lib_list-1.1.8/.docs/badges.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi| 
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_list/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_list/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_list/master?filepath=lib_list.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
```

### Comparing `lib_list-1.1.7/.docs/installation.rst` & `lib_list-1.1.8/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/.github/workflows/codeql-analysis.yml` & `lib_list-1.1.8/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/.github/workflows/python-package.yml` & `lib_list-1.1.8/.github/workflows/python-package.yml`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         # FLAKE8 tests
         DO_FLAKE8_TESTS: "True"
 
         # MYPY tests
         MYPY_DO_TESTS: "True"
         MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-        MYPYPATH: "./lib_list/3rd_party_stubs"
+        MYPYPATH: "./.3rd_party_stubs"
 
         # coverage
         DO_COVERAGE: "True"
         DO_COVERAGE_UPLOAD_CODECOV: "True"
         DO_COVERAGE_UPLOAD_CODE_CLIMATE: "True"
 
         # package name
@@ -129,22 +129,44 @@
               BUILD_TEST: "True"
               MYPY_DO_TESTS: "True"
               DO_SETUP_INSTALL: "True"
               DO_SETUP_INSTALL_TEST: "True"
               DO_CLI_TEST: "True"
 
           - os: ubuntu-latest
+            python-version: "3.12-dev"
+            env:
+              BUILD_DOCS: "True"
+              BUILD: "True"  
+              BUILD_TEST: "True"
+              MYPY_DO_TESTS: "True"
+              DO_SETUP_INSTALL: "True"
+              DO_SETUP_INSTALL_TEST: "True"
+              DO_CLI_TEST: "True"
+
+          - os: ubuntu-latest
             python-version: "pypy-3.9"
             env:
               BUILD_DOCS: "False"
               BUILD: "True"  
               BUILD_TEST: "True"
               MYPY_DO_TESTS: "False"
               DO_SETUP_INSTALL: "True"
               DO_SETUP_INSTALL_TEST: "True"
+              DO_CLI_TEST: "True"
+
+          - os: ubuntu-latest
+            python-version: "pypy-3.10"
+            env:
+              BUILD_DOCS: "False"
+              BUILD: "True"  
+              BUILD_TEST: "True"
+              MYPY_DO_TESTS: "False"
+              DO_SETUP_INSTALL: "True"
+              DO_SETUP_INSTALL_TEST: "True"
               DO_CLI_TEST: "True"
 
           - os: macos-latest
             python-version: "3.11"
             env:
               cPREFIX: ""               # prefix before commands - used for wine, there the prefix is "wine"
               cPYTHON: "python3"        # command to launch python interpreter (it's different on macOS, there we need python3)
```

### Comparing `lib_list-1.1.7/.gitignore` & `lib_list-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/CHANGES.rst` & `lib_list-1.1.8/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.8
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.1.7
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `lib_list-1.1.7/CODE_OF_CONDUCT.md` & `lib_list-1.1.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/CONTRIBUTING.md` & `lib_list-1.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/ISSUE_TEMPLATE.md` & `lib_list-1.1.8/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/LICENSE` & `lib_list-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/Makefile` & `lib_list-1.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/PKG-INFO` & `lib_list-1.1.8/lib_list.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lib_list
-Version: 1.1.7
+Name: lib-list
+Version: 1.1.8
 Summary: some convenience functions for lists
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_list
 Project-URL: Documentation, https://github.com/bitranox/lib_list/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_list.git
 Project-URL: Changelog, https://github.com/bitranox/lib_list/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_list
 ========
 
 
-Version v1.1.7 as of 2023-07-13 see `Changelog`_
+Version v1.1.8 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_list/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_list/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_list/master?filepath=lib_list.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -76,15 +78,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_list/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_list/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -241,14 +243,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.8
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.1.7
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `lib_list-1.1.7/PULL_REQUEST_TEMPLATE.md` & `lib_list-1.1.8/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/README.rst` & `lib_list-1.1.8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 lib_list
 ========
 
 
-Version v1.1.7 as of 2023-07-13 see `Changelog`_
+Version v1.1.8 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_list/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_list/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_list/master?filepath=lib_list.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -54,15 +56,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_list/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_list/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -219,14 +221,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.8
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.1.7
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `lib_list-1.1.7/lib_list/3rd_party_stubs/readme.txt` & `lib_list-1.1.8/.3rd_party_stubs/readme.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 -- projects -- stub_directory -- external_test.pyi
             |
             -- project_A ------- package_a_dir --- 3rd_party_stubs --- external_test.pyi
             |
             -- project_B ------- package_b_dir --- 3rd_party_stubs --- external_test.pyi
 
 
-for travis test of project_A we need to set the MYPYPATH to .../projects/project_A/package_a_dir/3rd_party_stubs
+for travis test of project_A we need to set the MYPYPATH to .../projects/project_A/3rd_party_stubs
 
 for local tests, we need to set the MYPYPATH to .../projects/stub_directory , not to find external_test.pyi twice.
```

### Comparing `lib_list-1.1.7/lib_list/lib_list.py` & `lib_list-1.1.8/lib_list/lib_list.py`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/lib_list/lib_list_cli.py` & `lib_list-1.1.8/lib_list/lib_list_cli.py`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/lib_list.egg-info/PKG-INFO` & `lib_list-1.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lib-list
-Version: 1.1.7
+Name: lib_list
+Version: 1.1.8
 Summary: some convenience functions for lists
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_list
 Project-URL: Documentation, https://github.com/bitranox/lib_list/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_list.git
 Project-URL: Changelog, https://github.com/bitranox/lib_list/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_list
 ========
 
 
-Version v1.1.7 as of 2023-07-13 see `Changelog`_
+Version v1.1.8 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_list/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_list/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_list/master?filepath=lib_list.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -76,15 +78,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_list/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_list/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -241,14 +243,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.8
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.1.7
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `lib_list-1.1.7/lib_list.egg-info/SOURCES.txt` & `lib_list-1.1.8/lib_list.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 PULL_REQUEST_TEMPLATE.md
 README.rst
 conftest.py
 lib_list.ipynb
 pyproject.toml
 requirements.txt
 requirements_test.txt
+.3rd_party_stubs/readme.txt
 .docs/README_template.rst
 .docs/acknowledgment.rst
 .docs/badges.rst
 .docs/commandline_help.rst
 .docs/contribute.rst
 .docs/description.rst
 .docs/index.rst
@@ -38,15 +39,14 @@
 lib_list/py.typed
 lib_list.egg-info/PKG-INFO
 lib_list.egg-info/SOURCES.txt
 lib_list.egg-info/dependency_links.txt
 lib_list.egg-info/entry_points.txt
 lib_list.egg-info/requires.txt
 lib_list.egg-info/top_level.txt
-lib_list/3rd_party_stubs/readme.txt
 tests/test_cli.py
 tests/local_testscripts/lib_bash_functions.sh
 tests/local_testscripts/run_clean.sh
 tests/local_testscripts/run_pytest.sh
 tests/local_testscripts/run_testloop.sh
 tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
 tests/local_testscripts/run_testloop_windows.cmd
```

### Comparing `lib_list-1.1.7/lib_list.ipynb` & `lib_list-1.1.8/lib_list.ipynb`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/pyproject.toml` & `lib_list-1.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
     "click",
     "cli_exit_tools",
 ]
-version = "v1.1.7"
+version = "v1.1.8"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_list"
 Documentation = "https://github.com/bitranox/lib_list/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_list.git"
```

### Comparing `lib_list-1.1.7/tests/local_testscripts/lib_bash_functions.sh` & `lib_list-1.1.8/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/tests/local_testscripts/run_pytest.sh` & `lib_list-1.1.8/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/tests/local_testscripts/run_testloop.sh` & `lib_list-1.1.8/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_list-1.1.8/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/tests/local_testscripts/run_testloop_windows.cmd` & `lib_list-1.1.8/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/tests/local_testscripts/shellcheck.sh` & `lib_list-1.1.8/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/tests/local_testscripts/testing_tools.py` & `lib_list-1.1.8/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.7/tests/test_cli.py` & `lib_list-1.1.8/tests/test_cli.py`

 * *Files identical despite different names*

