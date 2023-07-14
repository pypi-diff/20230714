# Comparing `tmp/cli_exit_tools-1.2.5.tar.gz` & `tmp/cli_exit_tools-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_exit_tools-1.2.5.tar", last modified: Thu Jul 13 17:11:56 2023, max compression
+gzip compressed data, was "cli_exit_tools-1.2.6.tar", last modified: Fri Jul 14 11:33:41 2023, max compression
```

## Comparing `cli_exit_tools-1.2.5.tar` & `cli_exit_tools-1.2.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.740480 cli_exit_tools-1.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-07-13 17:11:43.000000 cli_exit_tools-1.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/cli_exit_tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/cli_exit_tools/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/cli_exit_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/cli_exit_tools_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 17:11:56.000000 cli_exit_tools-1.2.5/cli_exit_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/cli_exit_tools.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:56.744480 cli_exit_tools-1.2.5/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-13 17:11:10.000000 cli_exit_tools-1.2.5/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:33:41.011610 cli_exit_tools-1.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:33:41.007610 cli_exit_tools-1.2.6/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:33:41.007610 cli_exit_tools-1.2.6/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:33:41.003610 cli_exit_tools-1.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:33:41.007610 cli_exit_tools-1.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-07-14 11:33:41.011610 cli_exit_tools-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-14 11:33:28.000000 cli_exit_tools-1.2.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:33:41.007610 cli_exit_tools-1.2.6/cli_exit_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/cli_exit_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/cli_exit_tools/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/cli_exit_tools/cli_exit_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/cli_exit_tools/cli_exit_tools_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/cli_exit_tools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:33:41.011610 cli_exit_tools-1.2.6/cli_exit_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-07-14 11:33:40.000000 cli_exit_tools-1.2.6/cli_exit_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-14 11:33:40.000000 cli_exit_tools-1.2.6/cli_exit_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:33:40.000000 cli_exit_tools-1.2.6/cli_exit_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 11:33:40.000000 cli_exit_tools-1.2.6/cli_exit_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-14 11:33:40.000000 cli_exit_tools-1.2.6/cli_exit_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 11:33:40.000000 cli_exit_tools-1.2.6/cli_exit_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/cli_exit_tools.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:33:41.011610 cli_exit_tools-1.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:33:41.011610 cli_exit_tools-1.2.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:33:41.011610 cli_exit_tools-1.2.6/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-14 11:32:56.000000 cli_exit_tools-1.2.6/tests/test_cli.py
```

### Comparing `cli_exit_tools-1.2.5/.coveragerc` & `cli_exit_tools-1.2.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/.docs/README_template.rst` & `cli_exit_tools-1.2.6/.docs/README_template.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cli_exit_tools
 ==============
 
 
-Version v1.2.5 as of 2023-07-13 see `Changelog`_
+Version v1.2.6 as of 2023-07-14 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `cli_exit_tools-1.2.5/.docs/badges.rst` & `cli_exit_tools-1.2.6/.docs/badges.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi| 
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/cli_exit_tools/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/cli_exit_tools/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/cli_exit_tools/master?filepath=cli_exit_tools.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
```

### Comparing `cli_exit_tools-1.2.5/.docs/installation.rst` & `cli_exit_tools-1.2.6/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/.docs/usage.rst` & `cli_exit_tools-1.2.6/.docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/.github/workflows/codeql-analysis.yml` & `cli_exit_tools-1.2.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/.github/workflows/python-package.yml` & `cli_exit_tools-1.2.6/.github/workflows/python-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         # FLAKE8 tests
         DO_FLAKE8_TESTS: "True"
 
         # MYPY tests
         MYPY_DO_TESTS: "True"
         MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-        MYPYPATH: "./cli_exit_tools/3rd_party_stubs"
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

### Comparing `cli_exit_tools-1.2.5/.gitignore` & `cli_exit_tools-1.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/CHANGES.rst` & `cli_exit_tools-1.2.6/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+
+v1.2.6
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.2.5
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v1.2.4
```

### Comparing `cli_exit_tools-1.2.5/CODE_OF_CONDUCT.md` & `cli_exit_tools-1.2.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/CONTRIBUTING.md` & `cli_exit_tools-1.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/ISSUE_TEMPLATE.md` & `cli_exit_tools-1.2.6/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/LICENSE` & `cli_exit_tools-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/Makefile` & `cli_exit_tools-1.2.6/Makefile`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/PKG-INFO` & `cli_exit_tools-1.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_exit_tools
-Version: 1.2.5
+Version: 1.2.6
 Summary: functions to exit an cli application properly
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/cli_exit_tools
 Project-URL: Documentation, https://github.com/bitranox/cli_exit_tools/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/cli_exit_tools.git
 Project-URL: Changelog, https://github.com/bitranox/cli_exit_tools/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 cli_exit_tools
 ==============
 
 
-Version v1.2.5 as of 2023-07-13 see `Changelog`_
+Version v1.2.6 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/cli_exit_tools/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/cli_exit_tools/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/cli_exit_tools/master?filepath=cli_exit_tools.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -81,15 +83,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -409,14 +411,23 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+
+v1.2.6
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.2.5
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v1.2.4
```

### Comparing `cli_exit_tools-1.2.5/PULL_REQUEST_TEMPLATE.md` & `cli_exit_tools-1.2.6/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/README.rst` & `cli_exit_tools-1.2.6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 cli_exit_tools
 ==============
 
 
-Version v1.2.5 as of 2023-07-13 see `Changelog`_
+Version v1.2.6 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/cli_exit_tools/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/cli_exit_tools/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/cli_exit_tools/master?filepath=cli_exit_tools.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -59,15 +61,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -387,14 +389,23 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+
+v1.2.6
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.2.5
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v1.2.4
```

### Comparing `cli_exit_tools-1.2.5/cli_exit_tools/3rd_party_stubs/readme.txt` & `cli_exit_tools-1.2.6/.3rd_party_stubs/readme.txt`

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

### Comparing `cli_exit_tools-1.2.5/cli_exit_tools/__init__.py` & `cli_exit_tools-1.2.6/cli_exit_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/cli_exit_tools/__init__conf__.py` & `cli_exit_tools-1.2.6/cli_exit_tools/__init__conf__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # CONF
 
 name = 'cli_exit_tools'
 title = 'functions to exit an cli application properly'
-version = 'v1.2.5'
+version = 'v1.2.6'
 url = 'https://github.com/bitranox/cli_exit_tools'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'cli_exit_tools'
 
 
 def print_info() -> None:
     print("""\
 
 Info for cli_exit_tools:
 
     functions to exit an cli application properly
 
-    Version : v1.2.5
+    Version : v1.2.6
     Url     : https://github.com/bitranox/cli_exit_tools
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `cli_exit_tools-1.2.5/cli_exit_tools/cli_exit_tools.py` & `cli_exit_tools-1.2.6/cli_exit_tools/cli_exit_tools.py`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/cli_exit_tools/cli_exit_tools_cli.py` & `cli_exit_tools-1.2.6/cli_exit_tools/cli_exit_tools_cli.py`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/cli_exit_tools.egg-info/PKG-INFO` & `cli_exit_tools-1.2.6/cli_exit_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-exit-tools
-Version: 1.2.5
+Version: 1.2.6
 Summary: functions to exit an cli application properly
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/cli_exit_tools
 Project-URL: Documentation, https://github.com/bitranox/cli_exit_tools/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/cli_exit_tools.git
 Project-URL: Changelog, https://github.com/bitranox/cli_exit_tools/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 cli_exit_tools
 ==============
 
 
-Version v1.2.5 as of 2023-07-13 see `Changelog`_
+Version v1.2.6 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/cli_exit_tools/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/cli_exit_tools/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/cli_exit_tools/master?filepath=cli_exit_tools.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -81,15 +83,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -409,14 +411,23 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+
+v1.2.6
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.2.5
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v1.2.4
```

### Comparing `cli_exit_tools-1.2.5/cli_exit_tools.egg-info/SOURCES.txt` & `cli_exit_tools-1.2.6/cli_exit_tools.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 PULL_REQUEST_TEMPLATE.md
 README.rst
 cli_exit_tools.ipynb
 conftest.py
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
 cli_exit_tools/py.typed
 cli_exit_tools.egg-info/PKG-INFO
 cli_exit_tools.egg-info/SOURCES.txt
 cli_exit_tools.egg-info/dependency_links.txt
 cli_exit_tools.egg-info/entry_points.txt
 cli_exit_tools.egg-info/requires.txt
 cli_exit_tools.egg-info/top_level.txt
-cli_exit_tools/3rd_party_stubs/readme.txt
 tests/test_cli.py
 tests/local_testscripts/lib_bash_functions.sh
 tests/local_testscripts/run_clean.sh
 tests/local_testscripts/run_pytest.sh
 tests/local_testscripts/run_testloop.sh
 tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
 tests/local_testscripts/run_testloop_windows.cmd
```

### Comparing `cli_exit_tools-1.2.5/cli_exit_tools.ipynb` & `cli_exit_tools-1.2.6/cli_exit_tools.ipynb`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/pyproject.toml` & `cli_exit_tools-1.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
     "click",
     "lib_detect_testenv",
 ]
-version = "v1.2.5"
+version = "v1.2.6"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/cli_exit_tools"
 Documentation = "https://github.com/bitranox/cli_exit_tools/blob/master/README.rst"
 Repository = "https://github.com/bitranox/cli_exit_tools.git"
```

### Comparing `cli_exit_tools-1.2.5/tests/local_testscripts/lib_bash_functions.sh` & `cli_exit_tools-1.2.6/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/tests/local_testscripts/run_pytest.sh` & `cli_exit_tools-1.2.6/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop.sh` & `cli_exit_tools-1.2.6/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `cli_exit_tools-1.2.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/tests/local_testscripts/run_testloop_windows.cmd` & `cli_exit_tools-1.2.6/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/tests/local_testscripts/shellcheck.sh` & `cli_exit_tools-1.2.6/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/tests/local_testscripts/testing_tools.py` & `cli_exit_tools-1.2.6/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.5/tests/test_cli.py` & `cli_exit_tools-1.2.6/tests/test_cli.py`

 * *Files identical despite different names*

