# Comparing `tmp/lib_shopware6_api_base-2.1.2.tar.gz` & `tmp/lib_shopware6_api_base-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_shopware6_api_base-2.1.2.tar", last modified: Thu Jul 13 17:35:42 2023, max compression
+gzip compressed data, was "lib_shopware6_api_base-2.1.3.tar", last modified: Fri Jul 14 12:20:04 2023, max compression
```

## Comparing `lib_shopware6_api_base-2.1.2.tar` & `lib_shopware6_api_base-2.1.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.739866 lib_shopware6_api_base-2.1.2/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.735866 lib_shopware6_api_base-2.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.739866 lib_shopware6_api_base-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    74304 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)    73313 2023-07-13 17:35:29.000000 lib_shopware6_api_base-2.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/conf_shopware6_api_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    59849 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    74304 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 17:35:42.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:35:42.743866 lib_shopware6_api_base-2.1.2/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-13 17:34:24.000000 lib_shopware6_api_base-2.1.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:20:04.265468 lib_shopware6_api_base-2.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:20:04.261469 lib_shopware6_api_base-2.1.3/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:20:04.261469 lib_shopware6_api_base-2.1.3/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:20:04.261469 lib_shopware6_api_base-2.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:20:04.265468 lib_shopware6_api_base-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    74756 2023-07-14 12:20:04.265468 lib_shopware6_api_base-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    73765 2023-07-14 12:19:51.000000 lib_shopware6_api_base-2.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:20:04.265468 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/conf_shopware6_api_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59849 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:20:04.265468 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    74756 2023-07-14 12:20:04.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-14 12:20:04.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:20:04.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-14 12:20:04.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-14 12:20:04.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 12:20:04.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/lib_shopware6_api_base.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:20:04.265468 lib_shopware6_api_base-2.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:20:04.265468 lib_shopware6_api_base-2.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:20:04.265468 lib_shopware6_api_base-2.1.3/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-14 12:18:46.000000 lib_shopware6_api_base-2.1.3/tests/test_cli.py
```

### Comparing `lib_shopware6_api_base-2.1.2/.coveragerc` & `lib_shopware6_api_base-2.1.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/.docs/README_template.rst` & `lib_shopware6_api_base-2.1.3/.docs/README_template.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_shopware6_api_base
 ======================
 
 
-Version v2.1.2 as of 2023-07-13 see `Changelog`_
+Version v2.1.3 as of 2023-07-14 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `lib_shopware6_api_base-2.1.2/.docs/badges.rst` & `lib_shopware6_api_base-2.1.3/.docs/badges.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-|build_badge| |license| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |pypi| 
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_shopware6_api_base/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_shopware6_api_base/master?filepath=lib_shopware6_api_base.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
```

### Comparing `lib_shopware6_api_base-2.1.2/.docs/installation.rst` & `lib_shopware6_api_base-2.1.3/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/.docs/usage.rst` & `lib_shopware6_api_base-2.1.3/.docs/usage.rst`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/.github/workflows/codeql-analysis.yml` & `lib_shopware6_api_base-2.1.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/.github/workflows/python-package.yml` & `lib_shopware6_api_base-2.1.3/.github/workflows/python-package.yml`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         # FLAKE8 tests
         DO_FLAKE8_TESTS: "True"
 
         # MYPY tests
         MYPY_DO_TESTS: "True"
         MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-        MYPYPATH: "./lib_shopware6_api_base/3rd_party_stubs"
+        MYPYPATH: "./.3rd_party_stubs"
 
         # coverage
         DO_COVERAGE: "True"
         DO_COVERAGE_UPLOAD_CODECOV: "True"
         DO_COVERAGE_UPLOAD_CODE_CLIMATE: "True"
 
         # package name
@@ -120,22 +120,44 @@
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
 
 
     name: "${{ matrix.os }} Python ${{ matrix.python-version }}"
 
     steps:
     # see : https://github.com/actions/checkout
```

### Comparing `lib_shopware6_api_base-2.1.2/.gitignore` & `lib_shopware6_api_base-2.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/CHANGES.rst` & `lib_shopware6_api_base-2.1.3/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.2
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.1.1
```

### Comparing `lib_shopware6_api_base-2.1.2/CODE_OF_CONDUCT.md` & `lib_shopware6_api_base-2.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/CONTRIBUTING.md` & `lib_shopware6_api_base-2.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/ISSUE_TEMPLATE.md` & `lib_shopware6_api_base-2.1.3/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/LICENSE` & `lib_shopware6_api_base-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/Makefile` & `lib_shopware6_api_base-2.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/PKG-INFO` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lib_shopware6_api_base
-Version: 2.1.2
+Name: lib-shopware6-api-base
+Version: 2.1.3
 Summary: python3 base API client for shopware6
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api_base
 Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api_base/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api_base.git
 Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api_base/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_shopware6_api_base
 ======================
 
 
-Version v2.1.2 as of 2023-07-13 see `Changelog`_
+Version v2.1.3 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_shopware6_api_base/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_shopware6_api_base/master?filepath=lib_shopware6_api_base.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -83,15 +85,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api_base/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Usage`_
 - `Usage from Commandline`_
@@ -1994,14 +1996,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.2
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.1.1
```

### Comparing `lib_shopware6_api_base-2.1.2/PULL_REQUEST_TEMPLATE.md` & `lib_shopware6_api_base-2.1.3/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/README.rst` & `lib_shopware6_api_base-2.1.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 lib_shopware6_api_base
 ======================
 
 
-Version v2.1.2 as of 2023-07-13 see `Changelog`_
+Version v2.1.3 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_shopware6_api_base/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_shopware6_api_base/master?filepath=lib_shopware6_api_base.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -61,15 +63,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api_base/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Usage`_
 - `Usage from Commandline`_
@@ -1972,14 +1974,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.2
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.1.1
```

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/3rd_party_stubs/readme.txt` & `lib_shopware6_api_base-2.1.3/.3rd_party_stubs/readme.txt`

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

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/__init__.py` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/__init__conf__.py` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/__init__conf__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # CONF
 
 name = 'lib_shopware6_api_base'
 title = 'python3 base API client for shopware6'
-version = 'v2.1.2'
+version = 'v2.1.3'
 url = 'https://github.com/bitranox/lib_shopware6_api_base'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'lib_shopware6_api_base'
 
 
 def print_info() -> None:
     print("""\
 
 Info for lib_shopware6_api_base:
 
     python3 base API client for shopware6
 
-    Version : v2.1.2
+    Version : v2.1.3
     Url     : https://github.com/bitranox/lib_shopware6_api_base
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/conf_shopware6_api_base_classes.py` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/conf_shopware6_api_base_classes.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/conf_shopware6_api_base_docker_testcontainer.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base.py` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_cli.py` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base_cli.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base_criteria.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base_criteria_aggregation.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base_criteria_filter.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base/lib_shopware6_api_base_criteria_sorting.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/PKG-INFO` & `lib_shopware6_api_base-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lib-shopware6-api-base
-Version: 2.1.2
+Name: lib_shopware6_api_base
+Version: 2.1.3
 Summary: python3 base API client for shopware6
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api_base
 Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api_base/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api_base.git
 Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api_base/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_shopware6_api_base
 ======================
 
 
-Version v2.1.2 as of 2023-07-13 see `Changelog`_
+Version v2.1.3 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_shopware6_api_base/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_shopware6_api_base/master?filepath=lib_shopware6_api_base.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -83,15 +85,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api_base/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api_base/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Usage`_
 - `Usage from Commandline`_
@@ -1994,14 +1996,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.3
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.2
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.1.1
```

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.egg-info/SOURCES.txt` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 PULL_REQUEST_TEMPLATE.md
 README.rst
 conftest.py
 lib_shopware6_api_base.ipynb
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
@@ -46,15 +47,14 @@
 lib_shopware6_api_base/py.typed
 lib_shopware6_api_base.egg-info/PKG-INFO
 lib_shopware6_api_base.egg-info/SOURCES.txt
 lib_shopware6_api_base.egg-info/dependency_links.txt
 lib_shopware6_api_base.egg-info/entry_points.txt
 lib_shopware6_api_base.egg-info/requires.txt
 lib_shopware6_api_base.egg-info/top_level.txt
-lib_shopware6_api_base/3rd_party_stubs/readme.txt
 tests/test_cli.py
 tests/local_testscripts/lib_bash_functions.sh
 tests/local_testscripts/run_clean.sh
 tests/local_testscripts/run_pytest.sh
 tests/local_testscripts/run_testloop.sh
 tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
 tests/local_testscripts/run_testloop_windows.cmd
```

### Comparing `lib_shopware6_api_base-2.1.2/lib_shopware6_api_base.ipynb` & `lib_shopware6_api_base-2.1.3/lib_shopware6_api_base.ipynb`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/pyproject.toml` & `lib_shopware6_api_base-2.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "cli_exit_tools",
     "lib_detect_testenv",
     "oauthlib",
     "pprint3x",
     "requests",
     "requests_oauthlib",
 ]
-version = "v2.1.2"
+version = "v2.1.3"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_shopware6_api_base"
 Documentation = "https://github.com/bitranox/lib_shopware6_api_base/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_shopware6_api_base.git"
```

### Comparing `lib_shopware6_api_base-2.1.2/tests/local_testscripts/lib_bash_functions.sh` & `lib_shopware6_api_base-2.1.3/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_pytest.sh` & `lib_shopware6_api_base-2.1.3/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop.sh` & `lib_shopware6_api_base-2.1.3/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_shopware6_api_base-2.1.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/tests/local_testscripts/run_testloop_windows.cmd` & `lib_shopware6_api_base-2.1.3/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/tests/local_testscripts/shellcheck.sh` & `lib_shopware6_api_base-2.1.3/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/tests/local_testscripts/testing_tools.py` & `lib_shopware6_api_base-2.1.3/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api_base-2.1.2/tests/test_cli.py` & `lib_shopware6_api_base-2.1.3/tests/test_cli.py`

 * *Files identical despite different names*

