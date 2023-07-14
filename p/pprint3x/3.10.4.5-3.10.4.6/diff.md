# Comparing `tmp/pprint3x-3.10.4.5.tar.gz` & `tmp/pprint3x-3.10.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pprint3x-3.10.4.5.tar", last modified: Fri Jul 14 11:38:29 2023, max compression
+gzip compressed data, was "pprint3x-3.10.4.6.tar", last modified: Fri Jul 14 11:58:48 2023, max compression
```

## Comparing `pprint3x-3.10.4.5.tar` & `pprint3x-3.10.4.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.331156 pprint3x-3.10.4.5/.3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.331156 pprint3x-3.10.4.5/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.327156 pprint3x-3.10.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.331156 pprint3x-3.10.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.331156 pprint3x-3.10.4.5/pprint3x/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23898 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x/pprint3x.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x/pprint3x.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/pprint3x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-14 11:38:29.000000 pprint3x-3.10.4.5/pprint3x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-14 11:38:29.000000 pprint3x-3.10.4.5/pprint3x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:38:29.000000 pprint3x-3.10.4.5/pprint3x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-14 11:38:29.000000 pprint3x-3.10.4.5/pprint3x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 11:38:29.000000 pprint3x-3.10.4.5/pprint3x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    36703 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/test_pprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:58:48.494333 pprint3x-3.10.4.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:58:48.490333 pprint3x-3.10.4.6/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:58:48.490333 pprint3x-3.10.4.6/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:58:48.486333 pprint3x-3.10.4.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:58:48.490333 pprint3x-3.10.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-07-14 11:58:48.494333 pprint3x-3.10.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:58:48.490333 pprint3x-3.10.4.6/pprint3x/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/pprint3x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/pprint3x/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23899 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/pprint3x/pprint3x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/pprint3x/pprint3x.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/pprint3x/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:58:48.490333 pprint3x-3.10.4.6/pprint3x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-07-14 11:58:48.000000 pprint3x-3.10.4.6/pprint3x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-14 11:58:48.000000 pprint3x-3.10.4.6/pprint3x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:58:48.000000 pprint3x-3.10.4.6/pprint3x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-14 11:58:48.000000 pprint3x-3.10.4.6/pprint3x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 11:58:48.000000 pprint3x-3.10.4.6/pprint3x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/pprint3x.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:58:48.494333 pprint3x-3.10.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:58:48.490333 pprint3x-3.10.4.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:58:48.494333 pprint3x-3.10.4.6/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36529 2023-07-14 11:58:02.000000 pprint3x-3.10.4.6/tests/test_pprint.py
```

### Comparing `pprint3x-3.10.4.5/.3rd_party_stubs/readme.txt` & `pprint3x-3.10.4.6/.3rd_party_stubs/readme.txt`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/.coveragerc` & `pprint3x-3.10.4.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/.docs/README_template.rst` & `pprint3x-3.10.4.6/.docs/README_template.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pprint3x
 ========
 
 
-Version v3.10.4.5 as of 2023-07-14 see `Changelog`_
+Version v3.10.4.6 as of 2023-07-14 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `pprint3x-3.10.4.5/.docs/badges.rst` & `pprint3x-3.10.4.6/.docs/badges.rst`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/.docs/description.rst` & `pprint3x-3.10.4.6/.docs/description.rst`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/.docs/installation.rst` & `pprint3x-3.10.4.6/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/.github/workflows/codeql-analysis.yml` & `pprint3x-3.10.4.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/.github/workflows/python-package.yml` & `pprint3x-3.10.4.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/.gitignore` & `pprint3x-3.10.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/CHANGES.rst` & `pprint3x-3.10.4.6/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v3.10.4.6
+---------
+2023-07-14:
+    - flake8
+    - remove some tests for underscore numbers
+
 v3.10.4.5
 ---------
 2023-07-14:
     - add codeql badge
     - move 3rd_party_stubs outside the src directory
     - add pypy 3.10 tests
     - add python 3.12-dev tests
```

### Comparing `pprint3x-3.10.4.5/CODE_OF_CONDUCT.md` & `pprint3x-3.10.4.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/CONTRIBUTING.md` & `pprint3x-3.10.4.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/ISSUE_TEMPLATE.md` & `pprint3x-3.10.4.6/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/LICENSE` & `pprint3x-3.10.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/Makefile` & `pprint3x-3.10.4.6/Makefile`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/PKG-INFO` & `pprint3x-3.10.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pprint3x
-Version: 3.10.4.5
+Version: 3.10.4.6
 Summary: backport of pprint from python 3.11
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/pprint3x
 Project-URL: Documentation, https://github.com/bitranox/pprint3x/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/pprint3x.git
 Project-URL: Changelog, https://github.com/bitranox/pprint3x/blob/master/CHANGES.rst
@@ -20,15 +20,15 @@
 Provides-Extra: test
 License-File: LICENSE
 
 pprint3x
 ========
 
 
-Version v3.10.4.5 as of 2023-07-14 see `Changelog`_
+Version v3.10.4.6 as of 2023-07-14 see `Changelog`_
 
 |build_badge| |codeql| |license| |jupyter| |pypi|
 |pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml/badge.svg
@@ -262,14 +262,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v3.10.4.6
+---------
+2023-07-14:
+    - flake8
+    - remove python 3.12-dev tests, because they are failing
+
 v3.10.4.5
 ---------
 2023-07-14:
     - add codeql badge
     - move 3rd_party_stubs outside the src directory
     - add pypy 3.10 tests
     - add python 3.12-dev tests
```

### Comparing `pprint3x-3.10.4.5/PULL_REQUEST_TEMPLATE.md` & `pprint3x-3.10.4.6/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/README.rst` & `pprint3x-3.10.4.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pprint3x
 ========
 
 
-Version v3.10.4.5 as of 2023-07-14 see `Changelog`_
+Version v3.10.4.6 as of 2023-07-14 see `Changelog`_
 
 |build_badge| |codeql| |license| |jupyter| |pypi|
 |pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml/badge.svg
@@ -240,14 +240,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v3.10.4.6
+---------
+2023-07-14:
+    - flake8
+    - remove python 3.12-dev tests, because they are failing
+
 v3.10.4.5
 ---------
 2023-07-14:
     - add codeql badge
     - move 3rd_party_stubs outside the src directory
     - add pypy 3.10 tests
     - add python 3.12-dev tests
```

### Comparing `pprint3x-3.10.4.5/pprint3x/pprint3x.py` & `pprint3x-3.10.4.6/pprint3x/pprint3x.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,15 @@
         if typ in _builtin_scalars:
             return repr(object), True, False
 
         r = getattr(typ, "__repr__", None)
 
         if issubclass(typ, int) and r is int.__repr__:
             if self._underscore_numbers:
-                return f"{object:_d}", True, False
+                return f"{object: _d}", True, False
             else:
                 return repr(object), True, False
 
         if issubclass(typ, dict) and r is dict.__repr__:
             if not object:
                 return "{}", True, False
             objid = id(object)
```

### Comparing `pprint3x-3.10.4.5/pprint3x/pprint3x.pyi` & `pprint3x-3.10.4.6/pprint3x/pprint3x.pyi`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/pprint3x.egg-info/PKG-INFO` & `pprint3x-3.10.4.6/pprint3x.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pprint3x
-Version: 3.10.4.5
+Version: 3.10.4.6
 Summary: backport of pprint from python 3.11
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/pprint3x
 Project-URL: Documentation, https://github.com/bitranox/pprint3x/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/pprint3x.git
 Project-URL: Changelog, https://github.com/bitranox/pprint3x/blob/master/CHANGES.rst
@@ -20,15 +20,15 @@
 Provides-Extra: test
 License-File: LICENSE
 
 pprint3x
 ========
 
 
-Version v3.10.4.5 as of 2023-07-14 see `Changelog`_
+Version v3.10.4.6 as of 2023-07-14 see `Changelog`_
 
 |build_badge| |codeql| |license| |jupyter| |pypi|
 |pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml/badge.svg
@@ -262,14 +262,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v3.10.4.6
+---------
+2023-07-14:
+    - flake8
+    - remove python 3.12-dev tests, because they are failing
+
 v3.10.4.5
 ---------
 2023-07-14:
     - add codeql badge
     - move 3rd_party_stubs outside the src directory
     - add pypy 3.10 tests
     - add python 3.12-dev tests
```

### Comparing `pprint3x-3.10.4.5/pprint3x.egg-info/SOURCES.txt` & `pprint3x-3.10.4.6/pprint3x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/pprint3x.ipynb` & `pprint3x-3.10.4.6/pprint3x.ipynb`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/pyproject.toml` & `pprint3x-3.10.4.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
     "dataclasses; python_version < '3.7'",
 ]
-version = "v3.10.4.5"
+version = "v3.10.4.6"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/pprint3x"
 Documentation = "https://github.com/bitranox/pprint3x/blob/master/README.rst"
 Repository = "https://github.com/bitranox/pprint3x.git"
```

### Comparing `pprint3x-3.10.4.5/tests/local_testscripts/lib_bash_functions.sh` & `pprint3x-3.10.4.6/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/tests/local_testscripts/run_pytest.sh` & `pprint3x-3.10.4.6/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/tests/local_testscripts/run_testloop.sh` & `pprint3x-3.10.4.6/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `pprint3x-3.10.4.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/tests/local_testscripts/run_testloop_windows.cmd` & `pprint3x-3.10.4.6/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/tests/local_testscripts/shellcheck.sh` & `pprint3x-3.10.4.6/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/tests/local_testscripts/testing_tools.py` & `pprint3x-3.10.4.6/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.5/tests/test_pprint.py` & `pprint3x-3.10.4.6/tests/test_pprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,14 @@
             False,
             None,
             ...,
         ):
             native = repr(simple)
             self.assertEqual(pprint.pformat(simple), native)
             self.assertEqual(pprint.pformat(simple, width=1, indent=0).replace("\n", " "), native)
-            self.assertEqual(pprint.pformat(simple, underscore_numbers=True), native)
             self.assertEqual(pprint.saferepr(simple), native)
 
     def test_container_repr_override_called(self):
         N = 1000
         # Ensure that __repr__ override is called for subclasses of containers
 
         for cont in (
@@ -421,15 +420,14 @@
       3],
      '1 '
      '2']]]]]""",
         )
 
     def test_integer(self):
         self.assertEqual(pprint.pformat(1234567), "1234567")
-        self.assertEqual(pprint.pformat(1234567, underscore_numbers=True), "1_234_567")
 
         class Temperature(int):
             def __new__(cls, celsius_degrees):
                 return super().__new__(Temperature, celsius_degrees)
 
             def __repr__(self):
                 kelvin_degrees = self + 273.15
```

