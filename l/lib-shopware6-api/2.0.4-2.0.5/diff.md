# Comparing `tmp/lib_shopware6_api-2.0.4.tar.gz` & `tmp/lib_shopware6_api-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_shopware6_api-2.0.4.tar", last modified: Thu Jul 13 17:40:05 2023, max compression
+gzip compressed data, was "lib_shopware6_api-2.0.5.tar", last modified: Fri Jul 14 12:35:51 2023, max compression
```

## Comparing `lib_shopware6_api-2.0.4.tar` & `lib_shopware6_api-2.0.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.545062 lib_shopware6_api-2.0.4/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.541062 lib_shopware6_api-2.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.545062 lib_shopware6_api-2.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    80805 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)    79854 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.545062 lib_shopware6_api-2.0.4/lib_shopware6_api/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/lib_shopware6_api/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/lib_shopware6_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/lib_shopware6_api_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_delivery_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    57284 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_media.py
--rw-r--r--   0 runner    (1001) docker     (123)    26121 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api/sub_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    80805 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 17:40:05.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/lib_shopware6_api.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:40:05.549062 lib_shopware6_api-2.0.4/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-13 17:37:21.000000 lib_shopware6_api-2.0.4/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:35:51.605785 lib_shopware6_api-2.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:35:51.597785 lib_shopware6_api-2.0.5/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:35:51.601785 lib_shopware6_api-2.0.5/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:35:51.593785 lib_shopware6_api-2.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:35:51.601785 lib_shopware6_api-2.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    81247 2023-07-14 12:35:51.601785 lib_shopware6_api-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    80296 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:35:51.601785 lib_shopware6_api-2.0.5/lib_shopware6_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/lib_shopware6_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/lib_shopware6_api_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/sub_currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/sub_delivery_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57284 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/sub_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26121 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/sub_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/sub_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api/sub_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:35:51.601785 lib_shopware6_api-2.0.5/lib_shopware6_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    81247 2023-07-14 12:35:51.000000 lib_shopware6_api-2.0.5/lib_shopware6_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-14 12:35:51.000000 lib_shopware6_api-2.0.5/lib_shopware6_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:35:51.000000 lib_shopware6_api-2.0.5/lib_shopware6_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-14 12:35:51.000000 lib_shopware6_api-2.0.5/lib_shopware6_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-14 12:35:51.000000 lib_shopware6_api-2.0.5/lib_shopware6_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 12:35:51.000000 lib_shopware6_api-2.0.5/lib_shopware6_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/lib_shopware6_api.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:35:51.605785 lib_shopware6_api-2.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:35:51.601785 lib_shopware6_api-2.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:35:51.601785 lib_shopware6_api-2.0.5/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-14 12:33:04.000000 lib_shopware6_api-2.0.5/tests/test_cli.py
```

### Comparing `lib_shopware6_api-2.0.4/.coveragerc` & `lib_shopware6_api-2.0.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/.docs/README_template.rst` & `lib_shopware6_api-2.0.5/.docs/README_template.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_shopware6_api
 =================
 
 
-Version v2.0.4 as of 2023-07-13 see `Changelog`_
+Version v2.0.5 as of 2023-07-14 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `lib_shopware6_api-2.0.4/.docs/badges.rst` & `lib_shopware6_api-2.0.5/.docs/badges.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi| 
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_shopware6_api/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_shopware6_api/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_shopware6_api/master?filepath=lib_shopware6_api.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
```

### Comparing `lib_shopware6_api-2.0.4/.docs/installation.rst` & `lib_shopware6_api-2.0.5/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/.docs/usage.rst` & `lib_shopware6_api-2.0.5/.docs/usage.rst`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/.github/workflows/codeql-analysis.yml` & `lib_shopware6_api-2.0.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/.github/workflows/python-package.yml` & `lib_shopware6_api-2.0.5/.github/workflows/python-package.yml`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         # FLAKE8 tests
         DO_FLAKE8_TESTS: "True"
 
         # MYPY tests
         MYPY_DO_TESTS: "True"
         MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-        MYPYPATH: "./lib_shopware6_api/3rd_party_stubs"
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

### Comparing `lib_shopware6_api-2.0.4/.gitignore` & `lib_shopware6_api-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/CHANGES.rst` & `lib_shopware6_api-2.0.5/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.5
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.4
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.3
```

### Comparing `lib_shopware6_api-2.0.4/CODE_OF_CONDUCT.md` & `lib_shopware6_api-2.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/CONTRIBUTING.md` & `lib_shopware6_api-2.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/ISSUE_TEMPLATE.md` & `lib_shopware6_api-2.0.5/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/LICENSE` & `lib_shopware6_api-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/Makefile` & `lib_shopware6_api-2.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/PKG-INFO` & `lib_shopware6_api-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib_shopware6_api
-Version: 2.0.4
+Version: 2.0.5
 Summary: use the shopware 6 api
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api
 Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api.git
 Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_shopware6_api
 =================
 
 
-Version v2.0.4 as of 2023-07-13 see `Changelog`_
+Version v2.0.5 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_shopware6_api/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_shopware6_api/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_shopware6_api/master?filepath=lib_shopware6_api.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -78,15 +80,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -1957,14 +1959,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.5
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.4
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.3
```

### Comparing `lib_shopware6_api-2.0.4/PULL_REQUEST_TEMPLATE.md` & `lib_shopware6_api-2.0.5/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/README.rst` & `lib_shopware6_api-2.0.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 lib_shopware6_api
 =================
 
 
-Version v2.0.4 as of 2023-07-13 see `Changelog`_
+Version v2.0.5 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_shopware6_api/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_shopware6_api/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_shopware6_api/master?filepath=lib_shopware6_api.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -56,15 +58,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -1935,14 +1937,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.5
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.4
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.3
```

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api/3rd_party_stubs/readme.txt` & `lib_shopware6_api-2.0.5/.3rd_party_stubs/readme.txt`

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

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api/__init__.py` & `lib_shopware6_api-2.0.5/lib_shopware6_api/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api/lib_shopware6_api.py` & `lib_shopware6_api-2.0.5/lib_shopware6_api/lib_shopware6_api.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api/lib_shopware6_api_cli.py` & `lib_shopware6_api-2.0.5/lib_shopware6_api/lib_shopware6_api_cli.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_currency.py` & `lib_shopware6_api-2.0.5/lib_shopware6_api/sub_currency.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_delivery_time.py` & `lib_shopware6_api-2.0.5/lib_shopware6_api/sub_delivery_time.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_media.py` & `lib_shopware6_api-2.0.5/lib_shopware6_api/sub_media.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_product.py` & `lib_shopware6_api-2.0.5/lib_shopware6_api/sub_product.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_tax.py` & `lib_shopware6_api-2.0.5/lib_shopware6_api/sub_tax.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api/sub_unit.py` & `lib_shopware6_api-2.0.5/lib_shopware6_api/sub_unit.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/PKG-INFO` & `lib_shopware6_api-2.0.5/lib_shopware6_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-shopware6-api
-Version: 2.0.4
+Version: 2.0.5
 Summary: use the shopware 6 api
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_shopware6_api
 Project-URL: Documentation, https://github.com/bitranox/lib_shopware6_api/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_shopware6_api.git
 Project-URL: Changelog, https://github.com/bitranox/lib_shopware6_api/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_shopware6_api
 =================
 
 
-Version v2.0.4 as of 2023-07-13 see `Changelog`_
+Version v2.0.5 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/lib_shopware6_api/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/lib_shopware6_api/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/lib_shopware6_api/master?filepath=lib_shopware6_api.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -78,15 +80,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/lib_shopware6_api/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux <https://github.com/bitranox/lib_shopware6_api/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -1957,14 +1959,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.5
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.0.4
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
 
 v2.0.3
```

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api.egg-info/SOURCES.txt` & `lib_shopware6_api-2.0.5/lib_shopware6_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 PULL_REQUEST_TEMPLATE.md
 README.rst
 conftest.py
 lib_shopware6_api.ipynb
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
@@ -45,15 +46,14 @@
 lib_shopware6_api/sub_unit.py
 lib_shopware6_api.egg-info/PKG-INFO
 lib_shopware6_api.egg-info/SOURCES.txt
 lib_shopware6_api.egg-info/dependency_links.txt
 lib_shopware6_api.egg-info/entry_points.txt
 lib_shopware6_api.egg-info/requires.txt
 lib_shopware6_api.egg-info/top_level.txt
-lib_shopware6_api/3rd_party_stubs/readme.txt
 tests/test_cli.py
 tests/local_testscripts/lib_bash_functions.sh
 tests/local_testscripts/run_clean.sh
 tests/local_testscripts/run_pytest.sh
 tests/local_testscripts/run_testloop.sh
 tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
 tests/local_testscripts/run_testloop_windows.cmd
```

### Comparing `lib_shopware6_api-2.0.4/lib_shopware6_api.ipynb` & `lib_shopware6_api-2.0.5/lib_shopware6_api.ipynb`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/pyproject.toml` & `lib_shopware6_api-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 dependencies = [
     "attrs>=21.3.0",
     "click",
     "cli_exit_tools",
     "lib_detect_testenv",
     "lib_shopware6_api_base",
 ]
-version = "v2.0.4"
+version = "v2.0.5"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_shopware6_api"
 Documentation = "https://github.com/bitranox/lib_shopware6_api/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_shopware6_api.git"
```

### Comparing `lib_shopware6_api-2.0.4/tests/local_testscripts/lib_bash_functions.sh` & `lib_shopware6_api-2.0.5/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/tests/local_testscripts/run_pytest.sh` & `lib_shopware6_api-2.0.5/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop.sh` & `lib_shopware6_api-2.0.5/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_shopware6_api-2.0.5/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/tests/local_testscripts/run_testloop_windows.cmd` & `lib_shopware6_api-2.0.5/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/tests/local_testscripts/shellcheck.sh` & `lib_shopware6_api-2.0.5/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/tests/local_testscripts/testing_tools.py` & `lib_shopware6_api-2.0.5/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `lib_shopware6_api-2.0.4/tests/test_cli.py` & `lib_shopware6_api-2.0.5/tests/test_cli.py`

 * *Files identical despite different names*

