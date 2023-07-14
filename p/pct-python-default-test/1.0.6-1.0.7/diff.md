# Comparing `tmp/pct_python_default_test-1.0.6.tar.gz` & `tmp/pct_python_default_test-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pct_python_default_test-1.0.6.tar", last modified: Thu Jul 13 17:09:37 2023, max compression
+gzip compressed data, was "pct_python_default_test-1.0.7.tar", last modified: Fri Jul 14 10:27:48 2023, max compression
```

## Comparing `pct_python_default_test-1.0.6.tar` & `pct_python_default_test-1.0.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.991490 pct_python_default_test-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.979489 pct_python_default_test-1.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-07-13 17:09:37.991490 pct_python_default_test-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/pct_python_default_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/pct_python_default_test/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/pct_python_default_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/pct_python_default_test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 17:09:37.000000 pct_python_default_test-1.0.6/pct_python_default_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pct_python_default_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:09:37.991490 pct_python_default_test-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:09:37.987490 pct_python_default_test-1.0.6/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-13 17:08:46.000000 pct_python_default_test-1.0.6/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:27:48.587550 pct_python_default_test-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:27:48.583550 pct_python_default_test-1.0.7/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:27:48.567550 pct_python_default_test-1.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:27:48.583550 pct_python_default_test-1.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:27:48.583550 pct_python_default_test-1.0.7/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-07-14 10:27:48.587550 pct_python_default_test-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:27:48.583550 pct_python_default_test-1.0.7/pct_python_default_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/pct_python_default_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/pct_python_default_test/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/pct_python_default_test/pct_python_default_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/pct_python_default_test/pct_python_default_test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/pct_python_default_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:27:48.583550 pct_python_default_test-1.0.7/pct_python_default_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-07-14 10:27:48.000000 pct_python_default_test-1.0.7/pct_python_default_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-14 10:27:48.000000 pct_python_default_test-1.0.7/pct_python_default_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:27:48.000000 pct_python_default_test-1.0.7/pct_python_default_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 10:27:48.000000 pct_python_default_test-1.0.7/pct_python_default_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 10:27:48.000000 pct_python_default_test-1.0.7/pct_python_default_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 10:27:48.000000 pct_python_default_test-1.0.7/pct_python_default_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/pct_python_default_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:27:48.587550 pct_python_default_test-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:27:48.583550 pct_python_default_test-1.0.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:27:48.583550 pct_python_default_test-1.0.7/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-14 10:27:01.000000 pct_python_default_test-1.0.7/tests/test_cli.py
```

### Comparing `pct_python_default_test-1.0.6/.coveragerc` & `pct_python_default_test-1.0.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/.docs/README_template.rst` & `pct_python_default_test-1.0.7/.docs/README_template.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pct_python_default_test
 =======================
 
 
-Version v1.0.6 as of 2023-07-13 see `Changelog`_
+Version v1.0.7 as of 2023-07-14 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `pct_python_default_test-1.0.6/.docs/badges.rst` & `pct_python_default_test-1.0.7/.docs/badges.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-|build_badge| |license| |jupyter| |black|
+|build_badge| |codeql| |license| |jupyter| 
+|black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/pct_python_default_test/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/pct_python_default_test/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/pct_python_default_test/master?filepath=pct_python_default_test.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
```

### Comparing `pct_python_default_test-1.0.6/.docs/description.rst` & `pct_python_default_test-1.0.7/.docs/description.rst`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/.docs/installation.rst` & `pct_python_default_test-1.0.7/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/.github/workflows/codeql-analysis.yml` & `pct_python_default_test-1.0.7/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/.github/workflows/python-package.yml` & `pct_python_default_test-1.0.7/.github/workflows/python-package.yml`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         # FLAKE8 tests
         DO_FLAKE8_TESTS: "True"
 
         # MYPY tests
         MYPY_DO_TESTS: "True"
         MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-        MYPYPATH: "./pct_python_default_test/3rd_party_stubs"
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

### Comparing `pct_python_default_test-1.0.6/.gitignore` & `pct_python_default_test-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/CHANGES.rst` & `pct_python_default_test-1.0.7/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Changelog
 ---------
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.0.7
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.0.6
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v1.0.5
```

### Comparing `pct_python_default_test-1.0.6/CODE_OF_CONDUCT.md` & `pct_python_default_test-1.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/CONTRIBUTING.md` & `pct_python_default_test-1.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/ISSUE_TEMPLATE.md` & `pct_python_default_test-1.0.7/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/LICENSE` & `pct_python_default_test-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/Makefile` & `pct_python_default_test-1.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/PKG-INFO` & `pct_python_default_test-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pct_python_default_test
-Version: 1.0.6
+Version: 1.0.7
 Summary: a pizzacutter default test project, crated with PizzaCutter and the PizzaCutter default python template
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/pct_python_default_test
 Project-URL: Documentation, https://github.com/bitranox/pct_python_default_test/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/pct_python_default_test.git
 Project-URL: Changelog, https://github.com/bitranox/pct_python_default_test/blob/master/CHANGES.rst
@@ -20,26 +20,30 @@
 Provides-Extra: test
 License-File: LICENSE
 
 pct_python_default_test
 =======================
 
 
-Version v1.0.6 as of 2023-07-13 see `Changelog`_
+Version v1.0.7 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |black|
+|build_badge| |codeql| |license| |jupyter|
+|black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/pct_python_default_test/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/pct_python_default_test/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/pct_python_default_test/master?filepath=pct_python_default_test.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -86,15 +90,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/pct_python_default_test/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -267,14 +271,22 @@
 Changelog
 ---------
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.0.7
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.0.6
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v1.0.5
```

### Comparing `pct_python_default_test-1.0.6/PULL_REQUEST_TEMPLATE.md` & `pct_python_default_test-1.0.7/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/README.rst` & `pct_python_default_test-1.0.7/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 pct_python_default_test
 =======================
 
 
-Version v1.0.6 as of 2023-07-13 see `Changelog`_
+Version v1.0.7 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |black|
+|build_badge| |codeql| |license| |jupyter|
+|black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/pct_python_default_test/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/pct_python_default_test/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/pct_python_default_test/master?filepath=pct_python_default_test.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -64,15 +68,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/pct_python_default_test/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -245,14 +249,22 @@
 Changelog
 ---------
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.0.7
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.0.6
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v1.0.5
```

### Comparing `pct_python_default_test-1.0.6/pct_python_default_test/3rd_party_stubs/readme.txt` & `pct_python_default_test-1.0.7/3rd_party_stubs/readme.txt`

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

### Comparing `pct_python_default_test-1.0.6/pct_python_default_test/__init__conf__.py` & `pct_python_default_test-1.0.7/pct_python_default_test/__init__conf__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # CONF
 
 name = 'pct_python_default_test'
 title = 'a pizzacutter default test project, crated with PizzaCutter and the PizzaCutter default python template'
-version = 'v1.0.6'
+version = 'v1.0.7'
 url = 'https://github.com/bitranox/pct_python_default_test'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'pct_python_default_test'
 
 
 def print_info() -> None:
     print("""\
 
 Info for pct_python_default_test:
 
     a pizzacutter default test project, crated with PizzaCutter and the PizzaCutter default python template
 
-    Version : v1.0.6
+    Version : v1.0.7
     Url     : https://github.com/bitranox/pct_python_default_test
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `pct_python_default_test-1.0.6/pct_python_default_test/pct_python_default_test.py` & `pct_python_default_test-1.0.7/pct_python_default_test/pct_python_default_test.py`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/pct_python_default_test/pct_python_default_test_cli.py` & `pct_python_default_test-1.0.7/pct_python_default_test/pct_python_default_test_cli.py`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/pct_python_default_test.egg-info/PKG-INFO` & `pct_python_default_test-1.0.7/pct_python_default_test.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pct-python-default-test
-Version: 1.0.6
+Version: 1.0.7
 Summary: a pizzacutter default test project, crated with PizzaCutter and the PizzaCutter default python template
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/pct_python_default_test
 Project-URL: Documentation, https://github.com/bitranox/pct_python_default_test/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/pct_python_default_test.git
 Project-URL: Changelog, https://github.com/bitranox/pct_python_default_test/blob/master/CHANGES.rst
@@ -20,26 +20,30 @@
 Provides-Extra: test
 License-File: LICENSE
 
 pct_python_default_test
 =======================
 
 
-Version v1.0.6 as of 2023-07-13 see `Changelog`_
+Version v1.0.7 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |black|
+|build_badge| |codeql| |license| |jupyter|
+|black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/pct_python_default_test/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/pct_python_default_test/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/pct_python_default_test/master?filepath=pct_python_default_test.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -86,15 +90,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/pct_python_default_test/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -267,14 +271,22 @@
 Changelog
 ---------
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.0.7
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.0.6
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v1.0.5
```

### Comparing `pct_python_default_test-1.0.6/pct_python_default_test.egg-info/SOURCES.txt` & `pct_python_default_test-1.0.7/pct_python_default_test.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

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
 pct_python_default_test/__init__.py
 pct_python_default_test/__init__conf__.py
 pct_python_default_test/pct_python_default_test.py
 pct_python_default_test/pct_python_default_test_cli.py
 pct_python_default_test/py.typed
 pct_python_default_test.egg-info/PKG-INFO
 pct_python_default_test.egg-info/SOURCES.txt
 pct_python_default_test.egg-info/dependency_links.txt
 pct_python_default_test.egg-info/entry_points.txt
 pct_python_default_test.egg-info/requires.txt
 pct_python_default_test.egg-info/top_level.txt
-pct_python_default_test/3rd_party_stubs/readme.txt
 tests/test_cli.py
 tests/local_testscripts/lib_bash_functions.sh
 tests/local_testscripts/run_clean.sh
 tests/local_testscripts/run_pytest.sh
 tests/local_testscripts/run_testloop.sh
 tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
 tests/local_testscripts/run_testloop_windows.cmd
```

### Comparing `pct_python_default_test-1.0.6/pct_python_default_test.ipynb` & `pct_python_default_test-1.0.7/pct_python_default_test.ipynb`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/pyproject.toml` & `pct_python_default_test-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
     "click",
     "cli_exit_tools",
 ]
-version = "v1.0.6"
+version = "v1.0.7"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/pct_python_default_test"
 Documentation = "https://github.com/bitranox/pct_python_default_test/blob/master/README.rst"
 Repository = "https://github.com/bitranox/pct_python_default_test.git"
```

### Comparing `pct_python_default_test-1.0.6/tests/local_testscripts/lib_bash_functions.sh` & `pct_python_default_test-1.0.7/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/tests/local_testscripts/run_pytest.sh` & `pct_python_default_test-1.0.7/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop.sh` & `pct_python_default_test-1.0.7/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `pct_python_default_test-1.0.7/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/tests/local_testscripts/run_testloop_windows.cmd` & `pct_python_default_test-1.0.7/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/tests/local_testscripts/shellcheck.sh` & `pct_python_default_test-1.0.7/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/tests/local_testscripts/testing_tools.py` & `pct_python_default_test-1.0.7/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.6/tests/test_cli.py` & `pct_python_default_test-1.0.7/tests/test_cli.py`

 * *Files identical despite different names*

