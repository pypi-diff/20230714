# Comparing `tmp/igittigitt-2.1.3.tar.gz` & `tmp/igittigitt-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igittigitt-2.1.3.tar", last modified: Thu Jul 13 17:51:28 2023, max compression
+gzip compressed data, was "igittigitt-2.1.4.tar", last modified: Fri Jul 14 12:49:14 2023, max compression
```

## Comparing `igittigitt-2.1.3.tar` & `igittigitt-2.1.4.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.505839 igittigitt-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.497839 igittigitt-2.1.3/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.489839 igittigitt-2.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.497839 igittigitt-2.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:50:34.000000 igittigitt-2.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-13 17:50:34.000000 igittigitt-2.1.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 17:50:34.000000 igittigitt-2.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 17:50:34.000000 igittigitt-2.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 17:50:34.000000 igittigitt-2.1.3/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:50:34.000000 igittigitt-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 17:50:34.000000 igittigitt-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 17:50:34.000000 igittigitt-2.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-07-13 17:51:28.505839 igittigitt-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 17:50:34.000000 igittigitt-2.1.3/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-07-13 17:50:34.000000 igittigitt-2.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 17:50:34.000000 igittigitt-2.1.3/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.497839 igittigitt-2.1.3/igittigitt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/igittigitt/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/conf_igittigitt.py
--rw-r--r--   0 runner    (1001) docker     (123)    24984 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/igittigitt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/igittigitt_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.497839 igittigitt-2.1.3/igittigitt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 17:51:28.000000 igittigitt-2.1.3/igittigitt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-13 17:50:34.000000 igittigitt-2.1.3/igittigitt.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-13 17:50:34.000000 igittigitt-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 17:50:34.000000 igittigitt-2.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 17:50:34.000000 igittigitt-2.1.3/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:51:28.505839 igittigitt-2.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.493839 igittigitt-2.1.3/tests/default_pattern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.493839 igittigitt-2.1.3/tests/default_pattern/.config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/default_pattern/.config/git/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/default_pattern/.config/git/ignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/default_pattern/git/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/default_pattern/git/ignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/.test_gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/.test_gitignore_empty
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/.test_venv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/.test_venv/some_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/not_excluded/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/.test_gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/not_excluded/excluded/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/excluded/excluded.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/not_excluded/excluded_not/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/excluded_not/sub_excluded.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/excluded_not.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/not_excluded/not_excluded2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/not_excluded2/sub_excluded.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded/not_excluded2.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/not_excluded.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/test__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/test__pycache__/.test_gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.493839 igittigitt-2.1.3/tests/example/test__pycache__/excluded/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example/test__pycache__/excluded/excluded/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/test__pycache__/excluded/excluded/excluded.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/test__pycache__/some_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example/test__pycache__/test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.493839 igittigitt-2.1.3/tests/example_negation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.493839 igittigitt-2.1.3/tests/example_negation/foo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example_negation/foo/bar/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example_negation/foo/bar/file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.501839 igittigitt-2.1.3/tests/example_negation/foo/other/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/example_negation/foo/other/file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.505839 igittigitt-2.1.3/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/local_testscripts/testing_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.505839 igittigitt-2.1.3/tests/target_expected/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/target_expected/.test_gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:51:28.505839 igittigitt-2.1.3/tests/target_expected/not_excluded/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/target_expected/not_excluded/.test_gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/target_expected/not_excluded/excluded_not.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/target_expected/not_excluded/not_excluded2.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/target_expected/not_excluded.txt
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-07-13 17:50:34.000000 igittigitt-2.1.3/tests/test_pytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.206353 igittigitt-2.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.190352 igittigitt-2.1.4/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.194352 igittigitt-2.1.4/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.182352 igittigitt-2.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.198352 igittigitt-2.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 12:48:24.000000 igittigitt-2.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-14 12:48:24.000000 igittigitt-2.1.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 12:48:24.000000 igittigitt-2.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 12:48:24.000000 igittigitt-2.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 12:48:24.000000 igittigitt-2.1.4/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 12:48:24.000000 igittigitt-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 12:48:24.000000 igittigitt-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 12:48:24.000000 igittigitt-2.1.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21660 2023-07-14 12:49:14.206353 igittigitt-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 12:48:24.000000 igittigitt-2.1.4/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20722 2023-07-14 12:48:24.000000 igittigitt-2.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 12:48:24.000000 igittigitt-2.1.4/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.198352 igittigitt-2.1.4/igittigitt/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-14 12:48:24.000000 igittigitt-2.1.4/igittigitt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-14 12:48:24.000000 igittigitt-2.1.4/igittigitt/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-14 12:48:24.000000 igittigitt-2.1.4/igittigitt/conf_igittigitt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24984 2023-07-14 12:48:24.000000 igittigitt-2.1.4/igittigitt/igittigitt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-14 12:48:24.000000 igittigitt-2.1.4/igittigitt/igittigitt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/igittigitt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.198352 igittigitt-2.1.4/igittigitt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21660 2023-07-14 12:49:14.000000 igittigitt-2.1.4/igittigitt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-14 12:49:14.000000 igittigitt-2.1.4/igittigitt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:49:14.000000 igittigitt-2.1.4/igittigitt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 12:49:14.000000 igittigitt-2.1.4/igittigitt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-14 12:49:14.000000 igittigitt-2.1.4/igittigitt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 12:49:14.000000 igittigitt-2.1.4/igittigitt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-14 12:48:24.000000 igittigitt-2.1.4/igittigitt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-14 12:48:24.000000 igittigitt-2.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 12:48:24.000000 igittigitt-2.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 12:48:24.000000 igittigitt-2.1.4/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:49:14.206353 igittigitt-2.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.182352 igittigitt-2.1.4/tests/default_pattern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.182352 igittigitt-2.1.4/tests/default_pattern/.config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/default_pattern/.config/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/default_pattern/.config/git/ignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/default_pattern/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/default_pattern/git/ignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/.test_gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/.test_gitignore_empty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/example/.test_venv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/.test_venv/some_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/example/not_excluded/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/not_excluded/.test_gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/example/not_excluded/excluded/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/not_excluded/excluded/excluded.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/example/not_excluded/excluded_not/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/not_excluded/excluded_not/sub_excluded.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/not_excluded/excluded_not.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/example/not_excluded/not_excluded2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/not_excluded/not_excluded2/sub_excluded.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/not_excluded/not_excluded2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/not_excluded.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/example/test__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/test__pycache__/.test_gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.186352 igittigitt-2.1.4/tests/example/test__pycache__/excluded/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/example/test__pycache__/excluded/excluded/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/test__pycache__/excluded/excluded/excluded.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/test__pycache__/some_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example/test__pycache__/test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.186352 igittigitt-2.1.4/tests/example_negation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.186352 igittigitt-2.1.4/tests/example_negation/foo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/example_negation/foo/bar/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example_negation/foo/bar/file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.202352 igittigitt-2.1.4/tests/example_negation/foo/other/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/example_negation/foo/other/file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.206353 igittigitt-2.1.4/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/local_testscripts/testing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.206353 igittigitt-2.1.4/tests/target_expected/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/target_expected/.test_gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:49:14.206353 igittigitt-2.1.4/tests/target_expected/not_excluded/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/target_expected/not_excluded/.test_gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/target_expected/not_excluded/excluded_not.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/target_expected/not_excluded/not_excluded2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/target_expected/not_excluded.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-07-14 12:48:24.000000 igittigitt-2.1.4/tests/test_pytest.py
```

### Comparing `igittigitt-2.1.3/.coveragerc` & `igittigitt-2.1.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/.docs/README_template.rst` & `igittigitt-2.1.4/.docs/README_template.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 igittigitt
 ==========
 
 
-Version v2.1.3 as of 2023-07-13 see `Changelog`_
+Version v2.1.4 as of 2023-07-14 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `igittigitt-2.1.3/.docs/badges.rst` & `igittigitt-2.1.4/.docs/badges.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi| 
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/igittigitt/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/igittigitt/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/igittigitt/master?filepath=igittigitt.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
```

### Comparing `igittigitt-2.1.3/.docs/description.rst` & `igittigitt-2.1.4/.docs/description.rst`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/.docs/installation.rst` & `igittigitt-2.1.4/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/.docs/usage.rst` & `igittigitt-2.1.4/.docs/usage.rst`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/.github/workflows/codeql-analysis.yml` & `igittigitt-2.1.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/.github/workflows/python-package.yml` & `igittigitt-2.1.4/.github/workflows/python-package.yml`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         # FLAKE8 tests
         DO_FLAKE8_TESTS: "True"
 
         # MYPY tests
         MYPY_DO_TESTS: "True"
         MYPY_OPTIONS: "--follow-imports=normal --ignore-missing-imports --implicit-reexport --install-types --no-warn-unused-ignores --non-interactive --strict"
-        MYPYPATH: "./igittigitt/3rd_party_stubs"
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

### Comparing `igittigitt-2.1.3/.gitignore` & `igittigitt-2.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/CHANGES.rst` & `igittigitt-2.1.4/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.4
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.3
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `igittigitt-2.1.3/CODE_OF_CONDUCT.md` & `igittigitt-2.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/CONTRIBUTING.md` & `igittigitt-2.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/ISSUE_TEMPLATE.md` & `igittigitt-2.1.4/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/LICENSE` & `igittigitt-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/Makefile` & `igittigitt-2.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/PKG-INFO` & `igittigitt-2.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igittigitt
-Version: 2.1.3
+Version: 2.1.4
 Summary: A spec-compliant gitignore parser for Python
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/igittigitt
 Project-URL: Documentation, https://github.com/bitranox/igittigitt/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/igittigitt.git
 Project-URL: Changelog, https://github.com/bitranox/igittigitt/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 igittigitt
 ==========
 
 
-Version v2.1.3 as of 2023-07-13 see `Changelog`_
+Version v2.1.4 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/igittigitt/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/igittigitt/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/igittigitt/master?filepath=igittigitt.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -203,15 +205,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/igittigitt/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -516,14 +518,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.4
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.3
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `igittigitt-2.1.3/PULL_REQUEST_TEMPLATE.md` & `igittigitt-2.1.4/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/README.rst` & `igittigitt-2.1.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 igittigitt
 ==========
 
 
-Version v2.1.3 as of 2023-07-13 see `Changelog`_
+Version v2.1.4 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/igittigitt/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/igittigitt/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/igittigitt/master?filepath=igittigitt.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -181,15 +183,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/igittigitt/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -494,14 +496,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.4
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.3
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `igittigitt-2.1.3/igittigitt/3rd_party_stubs/readme.txt` & `igittigitt-2.1.4/.3rd_party_stubs/readme.txt`

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

### Comparing `igittigitt-2.1.3/igittigitt/__init__.py` & `igittigitt-2.1.4/igittigitt/__init__.py`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/igittigitt/igittigitt.py` & `igittigitt-2.1.4/igittigitt/igittigitt.py`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/igittigitt/igittigitt_cli.py` & `igittigitt-2.1.4/igittigitt/igittigitt_cli.py`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/igittigitt.egg-info/PKG-INFO` & `igittigitt-2.1.4/igittigitt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igittigitt
-Version: 2.1.3
+Version: 2.1.4
 Summary: A spec-compliant gitignore parser for Python
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/igittigitt
 Project-URL: Documentation, https://github.com/bitranox/igittigitt/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/igittigitt.git
 Project-URL: Changelog, https://github.com/bitranox/igittigitt/blob/master/CHANGES.rst
@@ -20,26 +20,28 @@
 Provides-Extra: test
 License-File: LICENSE
 
 igittigitt
 ==========
 
 
-Version v2.1.3 as of 2023-07-13 see `Changelog`_
+Version v2.1.4 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/igittigitt/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/igittigitt/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/igittigitt/master?filepath=igittigitt.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
@@ -203,15 +205,15 @@
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
 `100% code coverage <https://codeclimate.com/github/bitranox/igittigitt/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/igittigitt/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -516,14 +518,22 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.1.4
+---------
+2023-07-14:
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v2.1.3
 ---------
 2023-07-13:
     - require minimum python 3.8
     - remove python 3.7 tests
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
```

### Comparing `igittigitt-2.1.3/igittigitt.egg-info/SOURCES.txt` & `igittigitt-2.1.4/igittigitt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 PULL_REQUEST_TEMPLATE.md
 README.rst
 conftest.py
 igittigitt.ipynb
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
@@ -39,15 +40,14 @@
 igittigitt/py.typed
 igittigitt.egg-info/PKG-INFO
 igittigitt.egg-info/SOURCES.txt
 igittigitt.egg-info/dependency_links.txt
 igittigitt.egg-info/entry_points.txt
 igittigitt.egg-info/requires.txt
 igittigitt.egg-info/top_level.txt
-igittigitt/3rd_party_stubs/readme.txt
 tests/test_cli.py
 tests/test_pytest.py
 tests/default_pattern/.config/git/ignore
 tests/default_pattern/git/ignore
 tests/example/.test_gitignore
 tests/example/.test_gitignore_empty
 tests/example/not_excluded.txt
```

### Comparing `igittigitt-2.1.3/igittigitt.ipynb` & `igittigitt-2.1.4/igittigitt.ipynb`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/pyproject.toml` & `igittigitt-2.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -28,36 +28,36 @@
 dependencies = [
     "attrs",
     "click",
     "cli_exit_tools",
     "lib_detect_testenv",
     "wcmatch",
 ]
-version = "v2.1.3"
+version = "v2.1.4"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/igittigitt"
 Documentation = "https://github.com/bitranox/igittigitt/blob/master/README.rst"
 Repository = "https://github.com/bitranox/igittigitt.git"
 Changelog = "https://github.com/bitranox/igittigitt/blob/master/CHANGES.rst"
 
 [project.optional-dependencies]
 test = [
-    "black ; platform_python_implementation != 'PyPy'",
-    "black==19.3b0 ; platform_python_implementation == 'PyPy'",
+    "black",
     "codecov",
     "coloredlogs",
     "coverage",
     "flake8",
     "mypy ; platform_python_implementation != 'PyPy'",
     "pytest",
     "pytest-cov",
     "pytest-runner",
+    "readme_renderer",
 ]
 
 [project.scripts]
     igittigitt = "igittigitt.igittigitt_cli:cli_main"
 
 [tool.setuptools.package-data]
 igittigitt = [
```

### Comparing `igittigitt-2.1.3/tests/default_pattern/.config/git/ignore` & `igittigitt-2.1.4/tests/default_pattern/.config/git/ignore`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/tests/default_pattern/git/ignore` & `igittigitt-2.1.4/tests/default_pattern/git/ignore`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/tests/local_testscripts/lib_bash_functions.sh` & `igittigitt-2.1.4/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/tests/local_testscripts/run_pytest.sh` & `igittigitt-2.1.4/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/tests/local_testscripts/run_testloop.sh` & `igittigitt-2.1.4/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `igittigitt-2.1.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/tests/local_testscripts/run_testloop_windows.cmd` & `igittigitt-2.1.4/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/tests/local_testscripts/shellcheck.sh` & `igittigitt-2.1.4/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/tests/local_testscripts/testing_tools.py` & `igittigitt-2.1.4/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/tests/test_cli.py` & `igittigitt-2.1.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `igittigitt-2.1.3/tests/test_pytest.py` & `igittigitt-2.1.4/tests/test_pytest.py`

 * *Files identical despite different names*

