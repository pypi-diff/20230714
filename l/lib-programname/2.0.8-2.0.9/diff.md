# Comparing `tmp/lib_programname-2.0.8.tar.gz` & `tmp/lib_programname-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_programname-2.0.8.tar", last modified: Thu Jul 13 17:14:47 2023, max compression
+gzip compressed data, was "lib_programname-2.0.9.tar", last modified: Fri Jul 14 13:07:08 2023, max compression
```

## Comparing `lib_programname-2.0.8.tar` & `lib_programname-2.0.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.346317 lib_programname-2.0.8/
--rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/.docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1009 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/README_template.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/acknowledgment.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2097 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/badges.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1551 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/badges_project.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/commandline_help.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      169 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/contribute.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1842 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/description.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/installation_via_makefile.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      294 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/installation_via_pypi.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/licence_mit.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      395 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/tested_under.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/try_in_jupyter.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.docs/usage.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      204 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.334316 lib_programname-2.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2457 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.github/workflows/codeql-analysis.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     8780 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.github/workflows/python-package.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-07-13 17:13:47.000000 lib_programname-2.0.8/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-07-13 17:13:47.000000 lib_programname-2.0.8/CHANGES.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3164 2023-07-13 17:13:47.000000 lib_programname-2.0.8/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-07-13 17:13:47.000000 lib_programname-2.0.8/CONTRIBUTING.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-07-13 17:13:47.000000 lib_programname-2.0.8/ISSUE_TEMPLATE.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-07-13 17:13:47.000000 lib_programname-2.0.8/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-07-13 17:13:47.000000 lib_programname-2.0.8/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1227 2023-07-13 17:13:47.000000 lib_programname-2.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-13 17:14:47.346317 lib_programname-2.0.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-07-13 17:13:47.000000 lib_programname-2.0.8/PULL_REQUEST_TEMPLATE.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    10369 2023-07-13 17:13:47.000000 lib_programname-2.0.8/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-07-13 17:13:47.000000 lib_programname-2.0.8/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/lib_programname/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/lib_programname/3rd_party_stubs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/3rd_party_stubs/readme.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/__init__conf__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7510 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/lib_programname.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1551 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/lib_programname_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/lib_programname.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 17:14:47.000000 lib_programname-2.0.8/lib_programname.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1544 2023-07-13 17:13:47.000000 lib_programname-2.0.8/lib_programname.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)     2541 2023-07-13 17:13:47.000000 lib_programname-2.0.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-07-13 17:13:47.000000 lib_programname-2.0.8/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-07-13 17:13:47.000000 lib_programname-2.0.8/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:14:47.346317 lib_programname-2.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:14:47.342317 lib_programname-2.0.8/tests/local_testscripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9587 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/lib_bash_functions.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/run_clean.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/run_pytest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1842 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/run_testloop.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1806 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      878 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/run_testloop_windows.cmd
--rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/shellcheck.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     5620 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/local_testscripts/testing_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-07-13 17:13:47.000000 lib_programname-2.0.8/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:08.086636 lib_programname-2.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:08.078636 lib_programname-2.0.9/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.3rd_party_stubs/readme.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:08.082635 lib_programname-2.0.9/.docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1009 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/README_template.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/acknowledgment.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2325 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/badges.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1551 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/badges_project.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/commandline_help.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      169 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/contribute.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1842 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/description.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/installation_via_makefile.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      294 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/installation_via_pypi.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/licence_mit.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/tested_under.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/try_in_jupyter.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.docs/usage.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      204 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:08.078636 lib_programname-2.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:08.082635 lib_programname-2.0.9/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2457 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.github/workflows/codeql-analysis.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9440 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.github/workflows/python-package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-07-14 13:06:24.000000 lib_programname-2.0.9/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2067 2023-07-14 13:06:24.000000 lib_programname-2.0.9/CHANGES.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3164 2023-07-14 13:06:24.000000 lib_programname-2.0.9/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-07-14 13:06:24.000000 lib_programname-2.0.9/CONTRIBUTING.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-07-14 13:06:24.000000 lib_programname-2.0.9/ISSUE_TEMPLATE.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-07-14 13:06:24.000000 lib_programname-2.0.9/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-07-14 13:06:24.000000 lib_programname-2.0.9/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1227 2023-07-14 13:06:24.000000 lib_programname-2.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-07-14 13:07:08.086636 lib_programname-2.0.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-07-14 13:06:24.000000 lib_programname-2.0.9/PULL_REQUEST_TEMPLATE.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10807 2023-07-14 13:06:56.000000 lib_programname-2.0.9/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-07-14 13:06:24.000000 lib_programname-2.0.9/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:08.082635 lib_programname-2.0.9/lib_programname/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-07-14 13:06:24.000000 lib_programname-2.0.9/lib_programname/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-14 13:06:24.000000 lib_programname-2.0.9/lib_programname/__init__conf__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7510 2023-07-14 13:06:24.000000 lib_programname-2.0.9/lib_programname/lib_programname.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1551 2023-07-14 13:06:24.000000 lib_programname-2.0.9/lib_programname/lib_programname_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:06:24.000000 lib_programname-2.0.9/lib_programname/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:08.082635 lib_programname-2.0.9/lib_programname.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-07-14 13:07:08.000000 lib_programname-2.0.9/lib_programname.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-14 13:07:08.000000 lib_programname-2.0.9/lib_programname.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:07:08.000000 lib_programname-2.0.9/lib_programname.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-14 13:07:08.000000 lib_programname-2.0.9/lib_programname.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-14 13:07:08.000000 lib_programname-2.0.9/lib_programname.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 13:07:08.000000 lib_programname-2.0.9/lib_programname.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1544 2023-07-14 13:06:24.000000 lib_programname-2.0.9/lib_programname.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2541 2023-07-14 13:06:24.000000 lib_programname-2.0.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-07-14 13:06:24.000000 lib_programname-2.0.9/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-07-14 13:06:24.000000 lib_programname-2.0.9/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:07:08.086636 lib_programname-2.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:08.082635 lib_programname-2.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:08.086636 lib_programname-2.0.9/tests/local_testscripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9587 2023-07-14 13:06:24.000000 lib_programname-2.0.9/tests/local_testscripts/lib_bash_functions.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-14 13:06:24.000000 lib_programname-2.0.9/tests/local_testscripts/run_clean.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-07-14 13:06:24.000000 lib_programname-2.0.9/tests/local_testscripts/run_pytest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1842 2023-07-14 13:06:24.000000 lib_programname-2.0.9/tests/local_testscripts/run_testloop.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1806 2023-07-14 13:06:24.000000 lib_programname-2.0.9/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      878 2023-07-14 13:06:24.000000 lib_programname-2.0.9/tests/local_testscripts/run_testloop_windows.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-07-14 13:06:24.000000 lib_programname-2.0.9/tests/local_testscripts/shellcheck.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5620 2023-07-14 13:06:24.000000 lib_programname-2.0.9/tests/local_testscripts/testing_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-07-14 13:06:24.000000 lib_programname-2.0.9/tests/test_cli.py
```

### Comparing `lib_programname-2.0.8/.coveragerc` & `lib_programname-2.0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/.docs/README_template.rst` & `lib_programname-2.0.9/.docs/README_template.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_programname
 ===============
 
 
-Version v2.0.8 as of 2023-07-13 see `Changelog`_
+Version v2.0.9 as of 2023-07-14 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `lib_programname-2.0.8/.docs/badges.rst` & `lib_programname-2.0.9/.docs/badges.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi| 
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_programname/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_programname/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_programname/master?filepath=lib_programname.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
```

### Comparing `lib_programname-2.0.8/.docs/badges_project.rst` & `lib_programname-2.0.9/.docs/badges_project.rst`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/.docs/description.rst` & `lib_programname-2.0.9/.docs/description.rst`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/.docs/installation.rst` & `lib_programname-2.0.9/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/.github/workflows/codeql-analysis.yml` & `lib_programname-2.0.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/.github/workflows/python-package.yml` & `lib_programname-2.0.9/.github/workflows/python-package.yml`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         # FLAKE8 tests
         DO_FLAKE8_TESTS: "True"
 
         # MYPY tests
         MYPY_DO_TESTS: "True"
         MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-        MYPYPATH: "./lib_programname/3rd_party_stubs"
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

### Comparing `lib_programname-2.0.8/.gitignore` & `lib_programname-2.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/CHANGES.rst` & `lib_programname-2.0.9/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.9
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.8
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.7
```

### Comparing `lib_programname-2.0.8/CODE_OF_CONDUCT.md` & `lib_programname-2.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/CONTRIBUTING.md` & `lib_programname-2.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/ISSUE_TEMPLATE.md` & `lib_programname-2.0.9/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/LICENSE` & `lib_programname-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/Makefile` & `lib_programname-2.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/PKG-INFO` & `lib_programname-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib_programname
-Version: 2.0.8
+Version: 2.0.9
 Summary: get reliably the name of the executed script
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_programname
 Project-URL: Documentation, https://github.com/bitranox/lib_programname/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_programname.git
 Project-URL: Changelog, https://github.com/bitranox/lib_programname/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_programname
 ===============
 
 
-Version v2.0.8 as of 2023-07-13 see `Changelog`_
+Version v2.0.9 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_programname/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_programname/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_programname/master?filepath=lib_programname.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -130,15 +132,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_programname/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -297,14 +299,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.9
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.8
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.7
```

### Comparing `lib_programname-2.0.8/PULL_REQUEST_TEMPLATE.md` & `lib_programname-2.0.9/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/README.rst` & `lib_programname-2.0.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 lib_programname
 ===============
 
 
-Version v2.0.8 as of 2023-07-13 see `Changelog`_
+Version v2.0.9 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_programname/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_programname/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_programname/master?filepath=lib_programname.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -108,15 +110,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_programname/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -275,14 +277,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.9
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.8
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.7
```

### Comparing `lib_programname-2.0.8/lib_programname/3rd_party_stubs/readme.txt` & `lib_programname-2.0.9/.3rd_party_stubs/readme.txt`

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

### Comparing `lib_programname-2.0.8/lib_programname/__init__.py` & `lib_programname-2.0.9/lib_programname/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/lib_programname/__init__conf__.py` & `lib_programname-2.0.9/lib_programname/__init__conf__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # CONF
 
 name = 'lib_programname'
 title = 'get reliably the name of the executed script'
-version = 'v2.0.8'
+version = 'v2.0.9'
 url = 'https://github.com/bitranox/lib_programname'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'lib_programname'
 
 
 def print_info() -> None:
     print("""\
 
 Info for lib_programname:
 
     get reliably the name of the executed script
 
-    Version : v2.0.8
+    Version : v2.0.9
     Url     : https://github.com/bitranox/lib_programname
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `lib_programname-2.0.8/lib_programname/lib_programname.py` & `lib_programname-2.0.9/lib_programname/lib_programname.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/lib_programname/lib_programname_cli.py` & `lib_programname-2.0.9/lib_programname/lib_programname_cli.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/lib_programname.egg-info/PKG-INFO` & `lib_programname-2.0.9/lib_programname.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-programname
-Version: 2.0.8
+Version: 2.0.9
 Summary: get reliably the name of the executed script
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_programname
 Project-URL: Documentation, https://github.com/bitranox/lib_programname/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_programname.git
 Project-URL: Changelog, https://github.com/bitranox/lib_programname/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_programname
 ===============
 
 
-Version v2.0.8 as of 2023-07-13 see `Changelog`_
+Version v2.0.9 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_programname/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_programname/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_programname/master?filepath=lib_programname.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -130,15 +132,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_programname/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -297,14 +299,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.9
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.8
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.7
```

### Comparing `lib_programname-2.0.8/lib_programname.egg-info/SOURCES.txt` & `lib_programname-2.0.9/lib_programname.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 PULL_REQUEST_TEMPLATE.md
 README.rst
 conftest.py
 lib_programname.ipynb
 pyproject.toml
 requirements.txt
 requirements_test.txt
+.3rd_party_stubs/readme.txt
 .docs/README_template.rst
 .docs/acknowledgment.rst
 .docs/badges.rst
 .docs/badges_project.rst
 .docs/commandline_help.rst
 .docs/contribute.rst
 .docs/description.rst
@@ -39,15 +40,14 @@
 lib_programname/py.typed
 lib_programname.egg-info/PKG-INFO
 lib_programname.egg-info/SOURCES.txt
 lib_programname.egg-info/dependency_links.txt
 lib_programname.egg-info/entry_points.txt
 lib_programname.egg-info/requires.txt
 lib_programname.egg-info/top_level.txt
-lib_programname/3rd_party_stubs/readme.txt
 tests/test_cli.py
 tests/local_testscripts/lib_bash_functions.sh
 tests/local_testscripts/run_clean.sh
 tests/local_testscripts/run_pytest.sh
 tests/local_testscripts/run_testloop.sh
 tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
 tests/local_testscripts/run_testloop_windows.cmd
```

### Comparing `lib_programname-2.0.8/lib_programname.ipynb` & `lib_programname-2.0.9/lib_programname.ipynb`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/pyproject.toml` & `lib_programname-2.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
     "click",
     "cli_exit_tools",
     "lib_detect_testenv",
 ]
-version = "v2.0.8"
+version = "v2.0.9"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_programname"
 Documentation = "https://github.com/bitranox/lib_programname/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_programname.git"
```

### Comparing `lib_programname-2.0.8/tests/local_testscripts/lib_bash_functions.sh` & `lib_programname-2.0.9/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/tests/local_testscripts/run_pytest.sh` & `lib_programname-2.0.9/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/tests/local_testscripts/run_testloop.sh` & `lib_programname-2.0.9/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_programname-2.0.9/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/tests/local_testscripts/run_testloop_windows.cmd` & `lib_programname-2.0.9/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/tests/local_testscripts/shellcheck.sh` & `lib_programname-2.0.9/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/tests/local_testscripts/testing_tools.py` & `lib_programname-2.0.9/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.8/tests/test_cli.py` & `lib_programname-2.0.9/tests/test_cli.py`

 * *Files identical despite different names*

