# Comparing `tmp/pprint3x-3.10.4.4.tar.gz` & `tmp/pprint3x-3.10.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pprint3x-3.10.4.4.tar", last modified: Thu Jul 13 17:25:35 2023, max compression
+gzip compressed data, was "pprint3x-3.10.4.5.tar", last modified: Fri Jul 14 11:38:29 2023, max compression
```

## Comparing `pprint3x-3.10.4.4.tar` & `pprint3x-3.10.4.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:25:35.693582 pprint3x-3.10.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:25:35.689582 pprint3x-3.10.4.4/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:25:35.685582 pprint3x-3.10.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:25:35.689582 pprint3x-3.10.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-13 17:25:35.693582 pprint3x-3.10.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-07-13 17:25:23.000000 pprint3x-3.10.4.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:25:35.689582 pprint3x-3.10.4.4/pprint3x/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:25:35.689582 pprint3x-3.10.4.4/pprint3x/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/pprint3x/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/pprint3x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/pprint3x/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23898 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/pprint3x/pprint3x.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/pprint3x/pprint3x.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/pprint3x/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:25:35.689582 pprint3x-3.10.4.4/pprint3x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-13 17:25:35.000000 pprint3x-3.10.4.4/pprint3x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-13 17:25:35.000000 pprint3x-3.10.4.4/pprint3x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:25:35.000000 pprint3x-3.10.4.4/pprint3x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-13 17:25:35.000000 pprint3x-3.10.4.4/pprint3x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 17:25:35.000000 pprint3x-3.10.4.4/pprint3x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/pprint3x.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:25:35.693582 pprint3x-3.10.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:25:35.689582 pprint3x-3.10.4.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:25:35.693582 pprint3x-3.10.4.4/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    36703 2023-07-13 17:24:50.000000 pprint3x-3.10.4.4/tests/test_pprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.331156 pprint3x-3.10.4.5/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.331156 pprint3x-3.10.4.5/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.327156 pprint3x-3.10.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.331156 pprint3x-3.10.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.331156 pprint3x-3.10.4.5/pprint3x/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23898 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x/pprint3x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x/pprint3x.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/pprint3x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-14 11:38:29.000000 pprint3x-3.10.4.5/pprint3x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-14 11:38:29.000000 pprint3x-3.10.4.5/pprint3x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:38:29.000000 pprint3x-3.10.4.5/pprint3x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-14 11:38:29.000000 pprint3x-3.10.4.5/pprint3x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 11:38:29.000000 pprint3x-3.10.4.5/pprint3x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pprint3x.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:38:29.335156 pprint3x-3.10.4.5/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36703 2023-07-14 11:37:42.000000 pprint3x-3.10.4.5/tests/test_pprint.py
```

### Comparing `pprint3x-3.10.4.4/.coveragerc` & `pprint3x-3.10.4.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/.docs/README_template.rst` & `pprint3x-3.10.4.5/.docs/README_template.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pprint3x
 ========
 
 
-Version v3.10.4.4 as of 2023-07-13 see `Changelog`_
+Version v3.10.4.5 as of 2023-07-14 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `pprint3x-3.10.4.4/.docs/badges.rst` & `pprint3x-3.10.4.5/.docs/badges.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi| 
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/pprint3x/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/pprint3x/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/pprint3x/master?filepath=pprint3x.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
```

### Comparing `pprint3x-3.10.4.4/.docs/description.rst` & `pprint3x-3.10.4.5/.docs/description.rst`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/.docs/installation.rst` & `pprint3x-3.10.4.5/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/.github/workflows/codeql-analysis.yml` & `pprint3x-3.10.4.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/.github/workflows/python-package.yml` & `pprint3x-3.10.4.5/.github/workflows/python-package.yml`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         # FLAKE8 tests
         DO_FLAKE8_TESTS: "True"
 
         # MYPY tests
         MYPY_DO_TESTS: "True"
         MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-        MYPYPATH: "./pprint3x/3rd_party_stubs"
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
               DO_CLI_TEST: "False"
 
           - os: ubuntu-latest
+            python-version: "3.12-dev"
+            env:
+              BUILD_DOCS: "True"
+              BUILD: "True"  
+              BUILD_TEST: "True"
+              MYPY_DO_TESTS: "True"
+              DO_SETUP_INSTALL: "True"
+              DO_SETUP_INSTALL_TEST: "True"
+              DO_CLI_TEST: "False"
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
+              DO_CLI_TEST: "False"
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
               DO_CLI_TEST: "False"
 
           - os: macos-latest
             python-version: "3.11"
             env:
               cPREFIX: ""               # prefix before commands - used for wine, there the prefix is "wine"
               cPYTHON: "python3"        # command to launch python interpreter (it's different on macOS, there we need python3)
```

### Comparing `pprint3x-3.10.4.4/.gitignore` & `pprint3x-3.10.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/CHANGES.rst` & `pprint3x-3.10.4.5/CHANGES.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v3.10.4.5
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v3.10.4.4
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v3.10.4.3
```

### Comparing `pprint3x-3.10.4.4/CODE_OF_CONDUCT.md` & `pprint3x-3.10.4.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/CONTRIBUTING.md` & `pprint3x-3.10.4.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/ISSUE_TEMPLATE.md` & `pprint3x-3.10.4.5/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/LICENSE` & `pprint3x-3.10.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/Makefile` & `pprint3x-3.10.4.5/Makefile`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/PKG-INFO` & `pprint3x-3.10.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pprint3x
-Version: 3.10.4.4
+Version: 3.10.4.5
 Summary: backport of pprint from python 3.11
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/pprint3x
 Project-URL: Documentation, https://github.com/bitranox/pprint3x/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/pprint3x.git
 Project-URL: Changelog, https://github.com/bitranox/pprint3x/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 pprint3x
 ========
 
 
-Version v3.10.4.4 as of 2023-07-13 see `Changelog`_
+Version v3.10.4.5 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/pprint3x/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/pprint3x/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/pprint3x/master?filepath=pprint3x.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -90,15 +92,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/pprint3x/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -260,14 +262,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v3.10.4.5
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v3.10.4.4
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v3.10.4.3
```

### Comparing `pprint3x-3.10.4.4/PULL_REQUEST_TEMPLATE.md` & `pprint3x-3.10.4.5/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/README.rst` & `pprint3x-3.10.4.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 pprint3x
 ========
 
 
-Version v3.10.4.4 as of 2023-07-13 see `Changelog`_
+Version v3.10.4.5 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/pprint3x/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/pprint3x/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/pprint3x/master?filepath=pprint3x.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -68,15 +70,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/pprint3x/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -238,14 +240,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v3.10.4.5
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v3.10.4.4
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v3.10.4.3
```

### Comparing `pprint3x-3.10.4.4/pprint3x/3rd_party_stubs/readme.txt` & `pprint3x-3.10.4.5/.3rd_party_stubs/readme.txt`

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

### Comparing `pprint3x-3.10.4.4/pprint3x/pprint3x.py` & `pprint3x-3.10.4.5/pprint3x/pprint3x.py`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/pprint3x/pprint3x.pyi` & `pprint3x-3.10.4.5/pprint3x/pprint3x.pyi`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/pprint3x.egg-info/PKG-INFO` & `pprint3x-3.10.4.5/pprint3x.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pprint3x
-Version: 3.10.4.4
+Version: 3.10.4.5
 Summary: backport of pprint from python 3.11
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/pprint3x
 Project-URL: Documentation, https://github.com/bitranox/pprint3x/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/pprint3x.git
 Project-URL: Changelog, https://github.com/bitranox/pprint3x/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 pprint3x
 ========
 
 
-Version v3.10.4.4 as of 2023-07-13 see `Changelog`_
+Version v3.10.4.5 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/pprint3x/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/pprint3x/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/pprint3x/master?filepath=pprint3x.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -90,15 +92,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/pprint3x/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pprint3x/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -260,14 +262,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v3.10.4.5
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v3.10.4.4
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v3.10.4.3
```

### Comparing `pprint3x-3.10.4.4/pprint3x.egg-info/SOURCES.txt` & `pprint3x-3.10.4.5/pprint3x.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 PULL_REQUEST_TEMPLATE.md
 README.rst
 conftest.py
 pprint3x.ipynb
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
@@ -37,15 +38,14 @@
 pprint3x/pprint3x.pyi
 pprint3x/py.typed
 pprint3x.egg-info/PKG-INFO
 pprint3x.egg-info/SOURCES.txt
 pprint3x.egg-info/dependency_links.txt
 pprint3x.egg-info/requires.txt
 pprint3x.egg-info/top_level.txt
-pprint3x/3rd_party_stubs/readme.txt
 tests/test_pprint.py
 tests/local_testscripts/lib_bash_functions.sh
 tests/local_testscripts/run_clean.sh
 tests/local_testscripts/run_pytest.sh
 tests/local_testscripts/run_testloop.sh
 tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
 tests/local_testscripts/run_testloop_windows.cmd
```

### Comparing `pprint3x-3.10.4.4/pprint3x.ipynb` & `pprint3x-3.10.4.5/pprint3x.ipynb`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/pyproject.toml` & `pprint3x-3.10.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
     "dataclasses; python_version < '3.7'",
 ]
-version = "v3.10.4.4"
+version = "v3.10.4.5"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/pprint3x"
 Documentation = "https://github.com/bitranox/pprint3x/blob/master/README.rst"
 Repository = "https://github.com/bitranox/pprint3x.git"
```

### Comparing `pprint3x-3.10.4.4/tests/local_testscripts/lib_bash_functions.sh` & `pprint3x-3.10.4.5/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/tests/local_testscripts/run_pytest.sh` & `pprint3x-3.10.4.5/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/tests/local_testscripts/run_testloop.sh` & `pprint3x-3.10.4.5/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `pprint3x-3.10.4.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/tests/local_testscripts/run_testloop_windows.cmd` & `pprint3x-3.10.4.5/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/tests/local_testscripts/shellcheck.sh` & `pprint3x-3.10.4.5/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/tests/local_testscripts/testing_tools.py` & `pprint3x-3.10.4.5/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `pprint3x-3.10.4.4/tests/test_pprint.py` & `pprint3x-3.10.4.5/tests/test_pprint.py`

 * *Files identical despite different names*

