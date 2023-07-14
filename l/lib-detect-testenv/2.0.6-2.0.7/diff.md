# Comparing `tmp/lib_detect_testenv-2.0.6.tar.gz` & `tmp/lib_detect_testenv-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_detect_testenv-2.0.6.tar", last modified: Thu Jul 13 16:44:45 2023, max compression
+gzip compressed data, was "lib_detect_testenv-2.0.7.tar", last modified: Fri Jul 14 11:10:33 2023, max compression
```

## Comparing `lib_detect_testenv-2.0.6.tar` & `lib_detect_testenv-2.0.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.499191 lib_detect_testenv-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.495191 lib_detect_testenv-2.0.6/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.491191 lib_detect_testenv-2.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.495191 lib_detect_testenv-2.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-07-13 16:44:45.499191 lib_detect_testenv-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.495191 lib_detect_testenv-2.0.6/lib_detect_testenv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.495191 lib_detect_testenv-2.0.6/lib_detect_testenv/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/lib_detect_testenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/lib_detect_testenv_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.495191 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 16:44:45.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/lib_detect_testenv.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:44:45.499191 lib_detect_testenv-2.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.499191 lib_detect_testenv-2.0.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:44:45.499191 lib_detect_testenv-2.0.6/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-13 16:43:56.000000 lib_detect_testenv-2.0.6/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:10:33.753031 lib_detect_testenv-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:10:33.753031 lib_detect_testenv-2.0.7/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:10:33.749031 lib_detect_testenv-2.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:10:33.753031 lib_detect_testenv-2.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:10:33.753031 lib_detect_testenv-2.0.7/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-14 11:10:33.753031 lib_detect_testenv-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:10:33.753031 lib_detect_testenv-2.0.7/lib_detect_testenv/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/lib_detect_testenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/lib_detect_testenv/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/lib_detect_testenv/lib_detect_testenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/lib_detect_testenv/lib_detect_testenv_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/lib_detect_testenv/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:10:33.753031 lib_detect_testenv-2.0.7/lib_detect_testenv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-14 11:10:33.000000 lib_detect_testenv-2.0.7/lib_detect_testenv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-14 11:10:33.000000 lib_detect_testenv-2.0.7/lib_detect_testenv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:10:33.000000 lib_detect_testenv-2.0.7/lib_detect_testenv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 11:10:33.000000 lib_detect_testenv-2.0.7/lib_detect_testenv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 11:10:33.000000 lib_detect_testenv-2.0.7/lib_detect_testenv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 11:10:33.000000 lib_detect_testenv-2.0.7/lib_detect_testenv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/lib_detect_testenv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:10:33.757031 lib_detect_testenv-2.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:10:33.753031 lib_detect_testenv-2.0.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:10:33.753031 lib_detect_testenv-2.0.7/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-14 11:09:46.000000 lib_detect_testenv-2.0.7/tests/test_cli.py
```

### Comparing `lib_detect_testenv-2.0.6/.coveragerc` & `lib_detect_testenv-2.0.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/.docs/README_template.rst` & `lib_detect_testenv-2.0.7/.docs/README_template.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_detect_testenv
 ==================
 
 
-Version v2.0.6 as of 2023-07-13 see `Changelog`_
+Version v2.0.7 as of 2023-07-14 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `lib_detect_testenv-2.0.6/.docs/badges.rst` & `lib_detect_testenv-2.0.7/.docs/badges.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi| 
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_detect_testenv/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_detect_testenv/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_detect_testenv/master?filepath=lib_detect_testenv.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
```

### Comparing `lib_detect_testenv-2.0.6/.docs/installation.rst` & `lib_detect_testenv-2.0.7/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/.docs/usage.rst` & `lib_detect_testenv-2.0.7/.docs/usage.rst`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/.github/workflows/codeql-analysis.yml` & `lib_detect_testenv-2.0.7/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/.github/workflows/python-package.yml` & `lib_detect_testenv-2.0.7/.github/workflows/python-package.yml`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         # FLAKE8 tests
         DO_FLAKE8_TESTS: "True"
 
         # MYPY tests
         MYPY_DO_TESTS: "True"
         MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-        MYPYPATH: "./lib_detect_testenv/3rd_party_stubs"
+        MYPYPATH: "./3rd_party_stubs"
 
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

### Comparing `lib_detect_testenv-2.0.6/.gitignore` & `lib_detect_testenv-2.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/CHANGES.rst` & `lib_detect_testenv-2.0.7/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.7
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.6
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.5
```

### Comparing `lib_detect_testenv-2.0.6/CODE_OF_CONDUCT.md` & `lib_detect_testenv-2.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/CONTRIBUTING.md` & `lib_detect_testenv-2.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/ISSUE_TEMPLATE.md` & `lib_detect_testenv-2.0.7/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/LICENSE` & `lib_detect_testenv-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/Makefile` & `lib_detect_testenv-2.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/PKG-INFO` & `lib_detect_testenv-2.0.7/lib_detect_testenv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lib_detect_testenv
-Version: 2.0.6
+Name: lib-detect-testenv
+Version: 2.0.7
 Summary: detects if pytest or doctest or pyrunner on pycharm is running
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_detect_testenv
 Project-URL: Documentation, https://github.com/bitranox/lib_detect_testenv/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_detect_testenv.git
 Project-URL: Changelog, https://github.com/bitranox/lib_detect_testenv/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_detect_testenv
 ==================
 
 
-Version v2.0.6 as of 2023-07-13 see `Changelog`_
+Version v2.0.7 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_detect_testenv/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_detect_testenv/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_detect_testenv/master?filepath=lib_detect_testenv.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -76,15 +78,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_detect_testenv/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -426,14 +428,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.7
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.6
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.5
```

### Comparing `lib_detect_testenv-2.0.6/PULL_REQUEST_TEMPLATE.md` & `lib_detect_testenv-2.0.7/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/README.rst` & `lib_detect_testenv-2.0.7/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 lib_detect_testenv
 ==================
 
 
-Version v2.0.6 as of 2023-07-13 see `Changelog`_
+Version v2.0.7 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_detect_testenv/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_detect_testenv/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_detect_testenv/master?filepath=lib_detect_testenv.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -54,15 +56,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_detect_testenv/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -404,14 +406,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.7
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.6
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.5
```

### Comparing `lib_detect_testenv-2.0.6/lib_detect_testenv/3rd_party_stubs/readme.txt` & `lib_detect_testenv-2.0.7/3rd_party_stubs/readme.txt`

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

### Comparing `lib_detect_testenv-2.0.6/lib_detect_testenv/__init__.py` & `lib_detect_testenv-2.0.7/lib_detect_testenv/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/lib_detect_testenv/__init__conf__.py` & `lib_detect_testenv-2.0.7/lib_detect_testenv/__init__conf__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # CONF
 
 name = 'lib_detect_testenv'
 title = 'detects if pytest or doctest or pyrunner on pycharm is running'
-version = 'v2.0.6'
+version = 'v2.0.7'
 url = 'https://github.com/bitranox/lib_detect_testenv'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'lib_detect_testenv'
 
 
 def print_info() -> None:
     print("""\
 
 Info for lib_detect_testenv:
 
     detects if pytest or doctest or pyrunner on pycharm is running
 
-    Version : v2.0.6
+    Version : v2.0.7
     Url     : https://github.com/bitranox/lib_detect_testenv
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `lib_detect_testenv-2.0.6/lib_detect_testenv/lib_detect_testenv.py` & `lib_detect_testenv-2.0.7/lib_detect_testenv/lib_detect_testenv.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/lib_detect_testenv/lib_detect_testenv_cli.py` & `lib_detect_testenv-2.0.7/lib_detect_testenv/lib_detect_testenv_cli.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/PKG-INFO` & `lib_detect_testenv-2.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lib-detect-testenv
-Version: 2.0.6
+Name: lib_detect_testenv
+Version: 2.0.7
 Summary: detects if pytest or doctest or pyrunner on pycharm is running
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_detect_testenv
 Project-URL: Documentation, https://github.com/bitranox/lib_detect_testenv/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_detect_testenv.git
 Project-URL: Changelog, https://github.com/bitranox/lib_detect_testenv/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_detect_testenv
 ==================
 
 
-Version v2.0.6 as of 2023-07-13 see `Changelog`_
+Version v2.0.7 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_detect_testenv/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_detect_testenv/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_detect_testenv/master?filepath=lib_detect_testenv.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -76,15 +78,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_detect_testenv/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -426,14 +428,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.7
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.6
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.5
```

### Comparing `lib_detect_testenv-2.0.6/lib_detect_testenv.egg-info/SOURCES.txt` & `lib_detect_testenv-2.0.7/lib_detect_testenv.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 .docs/installation_via_pypi.rst
 .docs/licence_mit.rst
 .docs/tested_under.rst
 .docs/try_in_jupyter.rst
 .docs/usage.rst
 .github/workflows/codeql-analysis.yml
 .github/workflows/python-package.yml
+3rd_party_stubs/readme.txt
 lib_detect_testenv/__init__.py
 lib_detect_testenv/__init__conf__.py
 lib_detect_testenv/lib_detect_testenv.py
 lib_detect_testenv/lib_detect_testenv_cli.py
 lib_detect_testenv/py.typed
 lib_detect_testenv.egg-info/PKG-INFO
 lib_detect_testenv.egg-info/SOURCES.txt
 lib_detect_testenv.egg-info/dependency_links.txt
 lib_detect_testenv.egg-info/entry_points.txt
 lib_detect_testenv.egg-info/requires.txt
 lib_detect_testenv.egg-info/top_level.txt
-lib_detect_testenv/3rd_party_stubs/readme.txt
 tests/test_cli.py
 tests/local_testscripts/lib_bash_functions.sh
 tests/local_testscripts/run_clean.sh
 tests/local_testscripts/run_pytest.sh
 tests/local_testscripts/run_testloop.sh
 tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
 tests/local_testscripts/run_testloop_windows.cmd
```

### Comparing `lib_detect_testenv-2.0.6/lib_detect_testenv.ipynb` & `lib_detect_testenv-2.0.7/lib_detect_testenv.ipynb`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/pyproject.toml` & `lib_detect_testenv-2.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
     "click",
     "cli_exit_tools",
 ]
-version = "v2.0.6"
+version = "v2.0.7"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_detect_testenv"
 Documentation = "https://github.com/bitranox/lib_detect_testenv/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_detect_testenv.git"
```

### Comparing `lib_detect_testenv-2.0.6/tests/local_testscripts/lib_bash_functions.sh` & `lib_detect_testenv-2.0.7/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/tests/local_testscripts/run_pytest.sh` & `lib_detect_testenv-2.0.7/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop.sh` & `lib_detect_testenv-2.0.7/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_detect_testenv-2.0.7/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/tests/local_testscripts/run_testloop_windows.cmd` & `lib_detect_testenv-2.0.7/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/tests/local_testscripts/shellcheck.sh` & `lib_detect_testenv-2.0.7/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/tests/local_testscripts/testing_tools.py` & `lib_detect_testenv-2.0.7/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.6/tests/test_cli.py` & `lib_detect_testenv-2.0.7/tests/test_cli.py`

 * *Files identical despite different names*

