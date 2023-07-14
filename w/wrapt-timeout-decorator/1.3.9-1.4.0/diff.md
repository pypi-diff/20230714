# Comparing `tmp/wrapt_timeout_decorator-1.3.9.tar.gz` & `tmp/wrapt_timeout_decorator-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapt_timeout_decorator-1.3.9.tar", last modified: Tue Apr 26 08:55:42 2022, max compression
+gzip compressed data, was "wrapt_timeout_decorator-1.4.0.tar", last modified: Fri Jul 14 17:41:12 2023, max compression
```

## Comparing `wrapt_timeout_decorator-1.3.9.tar` & `wrapt_timeout_decorator-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 08:55:42.593802 wrapt_timeout_decorator-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    35813 2022-04-26 08:55:42.593802 wrapt_timeout_decorator-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    35114 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-04-26 08:55:42.593802 wrapt_timeout_decorator-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4183 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 08:55:42.593802 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator/
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3783 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator/wrap_function_multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     7235 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator/wrap_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7440 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator/wrapt_timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-04-26 08:54:41.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator/wrapt_timeout_decorator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 08:55:42.593802 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    35813 2022-04-26 08:55:42.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-04-26 08:55:42.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-26 08:55:42.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-04-26 08:55:42.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-26 08:55:40.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-04-26 08:55:42.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-04-26 08:55:42.000000 wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:12.547037 wrapt_timeout_decorator-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:12.539037 wrapt_timeout_decorator-1.4.0/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.3rd_party_stubs/wrapt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:12.539037 wrapt_timeout_decorator-1.4.0/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/badges_project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/commandline_help.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/licence_mit.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:12.543037 wrapt_timeout_decorator-1.4.0/.docs/parts/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/alternative_exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/caveats_using_no_signals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/caveats_using_signals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/detect_pickle_errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/general_recommendations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/hard_timeout.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/multithreading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/nested_timeouts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/override_parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/use_as_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/use_eval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/parts/use_with_windows.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:12.535036 wrapt_timeout_decorator-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:12.543037 wrapt_timeout_decorator-1.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.github/ISSUE_TEMPLATE/issue_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:12.543037 wrapt_timeout_decorator-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    39929 2023-07-14 17:41:12.547037 wrapt_timeout_decorator-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    38943 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:41:12.547037 wrapt_timeout_decorator-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:12.543037 wrapt_timeout_decorator-1.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:12.543037 wrapt_timeout_decorator-1.4.0/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/test_subprocess_alive_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/test_wrapt_timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/tests/wrapt_timeout_test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:12.547037 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator/wrap_function_multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator/wrap_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator/wrapt_timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator/wrapt_timeout_decorator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:12.547037 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    39929 2023-07-14 17:41:12.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-14 17:41:12.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:41:12.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 17:41:12.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-14 17:41:12.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 17:41:12.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    37612 2023-07-14 17:40:08.000000 wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator.ipynb
```

### Comparing `wrapt_timeout_decorator-1.3.9/LICENSE` & `wrapt_timeout_decorator-1.4.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 1990-2022 Robert Nowotny
+Copyright (c) 1990-2023 Robert Nowotny
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `wrapt_timeout_decorator-1.3.9/PKG-INFO` & `wrapt_timeout_decorator-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,110 +1,126 @@
 Metadata-Version: 2.1
 Name: wrapt_timeout_decorator
-Version: 1.3.9
+Version: 1.4.0
 Summary: The better timout decorator
-Home-page: https://github.com/bitranox/wrapt_timeout_decorator
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/wrapt_timeout_decorator
+Project-URL: Documentation, https://github.com/bitranox/wrapt_timeout_decorator/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/wrapt_timeout_decorator.git
+Project-URL: Changelog, https://github.com/bitranox/wrapt_timeout_decorator/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 wrapt_timeout_decorator
 =======================
 
 
-Version v1.3.9 as of 2022-04-26 see `Changelog`_
+Version v1.4.0 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/wrapt_timeout_decorator/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/wrapt_timeout_decorator/master?filepath=wrapt_timeout_decorator.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/wrapt-timeout-decorator?label=PyPI%20Package
    :target: https://badge.fury.io/py/wrapt_timeout_decorator
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/wrapt_timeout_decorator
    :target: https://codecov.io/gh/bitranox/wrapt_timeout_decorator
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/wrapt_timeout_decorator?branch=master
-   :target: https://bettercodehub.com/results/bitranox/wrapt_timeout_decorator
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/wrapt_timeout_decorator?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/wrapt_timeout_decorator?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/wrapt_timeout_decorator?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/wrapt_timeout_decorator
+.. |snyk| image:: https://snyk.io/test/github/bitranox/wrapt_timeout_decorator/badge.svg
    :target: https://snyk.io/test/github/bitranox/wrapt_timeout_decorator
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/wrapt-timeout-decorator
    :target: https://pypi.org/project/wrapt-timeout-decorator/
    :alt: PyPI - Downloads
 
-there are many timeout decorators out there - that one focuses on correctness when using with Classes, methods,
-class methods, static methods and so on, preserving also the traceback information for Pycharm debugging.
+There are several timeout decorators available, but the one mentioned here
+focuses on ensuring correctness when used with classes, methods, class methods,
+static methods, etc. It also preserves traceback information for PyCharm debugging.
+
+Additionally, there is a powerful eval function that allows reading
+the desired timeout value even from class attributes.
+
+Two timeout strategies have been implemented:
+one using "Signals" and the other using "Multiprocessing".
+
+Signals
+-------
+
+The "Signals" strategy (for POSIX Systems) is elegant and efficient,
+but it has some important caveats which should be reviewed
+in the `Caveats using Signals`_ section.
+
 
-There is also a powerful eval function, it allows to read the desired timeout value even from Class attributes.
+Multiprocessing
+---------------
 
-It is very flexible and can be used with python >= 3.6, pypy3 and probably other dialects.
+The default strategy is to use Multiprocessing
 
-There are two timeout strategies implemented, the ubiquitous method using "Signals" and the second using Multiprocessing.
-Using "Signals" is slick and lean, but there are nasty caveats, please check section `Caveats using Signals`_
+- on Windows, due to the lack of signals, this is only available choice, which is enforced automatically
+- signals (on POSIX) can not be used in a subthread, therefore multiprocessing is enforced in such cases
 
-The default strategy is therefore using Multiprocessing, but You can also use Signals, You have been warned !
+When using a subprocess many types from multiprocessing need to be pickable so that child processes can use them.
+Therefore we use "dill" instead of "pickle" and "multiprocess" instead of "multiprocessing".
 
-Due to the lack of signals on Windows, or for threaded functions (in a subthread) where signals cant be used, Your only choice is Multiprocessing,
-this is set automatically.
+dill extends python’s pickle module for serializing and de-serializing python objects to the majority of the built-in python types
 
-Under Windows the decorated function and results needs to be pickable.
-For that purpose we use "multiprocess" and "dill" instead of "multiprocessing" and "pickle", in order to be able to use this decorator on more sophisticated objects.
-Communication to the subprocess is done via "multiprocess.pipe" instead of "queue", which is faster and might also work on Amazon AWS.
+Communication with the subprocess is done via "multiprocess.pipe" instead of "queue",
+which offers improved speed and may also work on Amazon AWS.
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10.0, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/wrapt_timeout_decorator>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -143,20 +159,28 @@
             print('{} seconds have passed'.format(i))
 
     if __name__ == '__main__':
         mytest('starting')
 
 General Recommendations
 -----------------------
-dont sprincle Your code with timeouts. Just use it were absolutely necessary, for instance when reading or writing a file. And do that on the lowest
-abstraction level possible to avoid unwanted side effects (Exceptions caught by some other code, non pickable functions or arguments, and so on, but not TOO
-low. Remember that forking the program takes some time (when use multiprocessing).
+Minimize the excessive use of timeouts in your code and reserve their usage for essential cases.
+
+Implement timeouts at the lowest possible abstraction level to prevent unintended
+consequences such as exceptions being caught by unrelated code or non-pickable
+functions and arguments.
+
+Avoid incorporating the Timeout Decorator within a loop that iterates multiple times,
+as this can result in considerable time overhead,
+especially on Windows systems, when utilizing multiprocessing.
+
+Whenever feasible, leverage the existing built-in timeouts already provided by the functions
+and libraries you utilize. These built-in timeouts can handle most situations effectively.
+Only resort to use this Timeout Decorator as a last resort when all other alternatives have been exhausted.
 
-Most functions and libraries You call, they HAVE already some timeouts. use those. This Timeout Decorator should be only the last ressort, if everything else
-fails.
 
     BAD EXAMPLE (Pseudocode) - lets assume the write to the database fails sometimes for unknown reasons, and "hangs"
 
     .. code-block:: py
 
         # module file_analyzer
         import time
@@ -593,14 +617,74 @@
 .. warning::
     Make sure that in case of multiprocessing strategy for timeout, your function does not return objects which cannot
     be pickled, otherwise it will fail at marshalling it between master and child processes. To cover more cases,
     we use multiprocess and dill instead of multiprocessing and pickle.
 
     Since Signals will not work on Windows, it is disabled by default, whatever You set.
 
+
+Subprocess Monitoring
+---------------------
+
+when using multiprocessing, the subprocess is monitored if it is still alive.
+if the subprocess was terminated or killed (for instance by OOMKiller),
+``multiprocessing.context.ProcessError`` will be raised.
+By default the subprocess is monitored every 5 seconds, but can be set with parameter
+``dec_poll_subprocess``. polling can be turned off by setting to 0.0 seconds
+
+.. code-block:: python
+
+    from wrapt_timeout_decorator import timeout
+
+
+    @timeout(10, use_signals=False, timeout_exception=TimeoutError, dec_poll_subprocess=1)
+    def slow_process() -> None:
+        # should have enough time to finish
+        # but instead it gets terminated, and the
+        # poll the subprocess every second
+        logger.error(f"Slow process started at {get_str_time()}")
+        time.sleep(5)
+        logger.error(f"Slow process done at {get_str_time()}")
+
+
+    def fake_oom_killer() -> None:
+        logger.error(f"Fake OOMKiller started at {get_str_time()}")
+        time.sleep(2)
+        # kill sibling slow_process
+        # hacky way to find it
+        target = psutil.Process().parent().children(recursive=True)[-1]
+        target.kill()
+        logger.error(f"Killed {target.pid} at {get_str_time()}")
+
+
+    def start_processes() -> None:
+        """
+        starts the 'fake_oom_killer' and 'slow_process' process -
+        and kill 'slow_process' after two seconds
+
+        >>> start_processes()
+        Traceback (most recent call last):
+            ...
+        multiprocessing.context.ProcessError: Function slow_process was terminated or killed after ... seconds
+        """
+        process_oom_killer = multiprocessing.Process(target=fake_oom_killer, args=())
+        process_oom_killer.start()
+        slow_process()
+        process_oom_killer.join()
+
+
+    def get_str_time() -> str:
+        t = time.localtime()
+        current_time = time.strftime("%H:%M:%S", t)
+        return current_time
+
+
+    if __name__ == '__main__':
+        start_processes()
+
 use as function not as decorator
 --------------------------------
 
 You can use the timout also as function, without using as decorator:
 
 .. code-block:: py
 
@@ -776,14 +860,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade wrapt_timeout_decorator
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade wrapt_timeout_decorator[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/wrapt_timeout_decorator.git
 
@@ -799,22 +890,22 @@
     # for the latest development version :
     wrapt_timeout_decorator @ git+https://github.com/bitranox/wrapt_timeout_decorator.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/wrapt_timeout_decorator.git
     $ cd wrapt_timeout_decorator
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -839,16 +930,20 @@
 following modules will be automatically installed :
 
 .. code-block:: bash
 
     ## Project Requirements
     cli_exit_tools
     lib_detect_testenv
-    dill
+
+    # class decorators are failing on windows with dill 0.3.5, 0.3.5.1
+    dill>0.3.0,!=0.3.5,!=0.3.5.1;sys_platform=="win32"
+    dill;sys_platform!="win32"
     multiprocess
+    psutil
     wrapt
 
 Acknowledgements
 ----------------
 
 - special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"
 
@@ -864,14 +959,54 @@
 This software is licensed under the `MIT license <http://en.wikipedia.org/wiki/MIT_License>`_
 
 ---
 
 Changelog
 =========
 
+v1.4.0
+---------
+2023-07-13:
+    - check for killed child processes (for instance by OOMKiller)
+    - change dill requirements for windows
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
+v1.3.12.2
+---------
+2022-06-01: update to github actions checkout@v3 and setup-python@v3
+
+v1.3.12
+--------
+2022-05-23: update requirements.txt
+
+v1.3.11
+--------
+2022-05-23:
+    - set dill version < 0.3.5 on windows, because decorating class methods fails with dill 0.3.5 upwards
+    - update tests to the latest python versions
+
+v1.3.10
+--------
+2022-04-26: add tests for thread lock
+
 v1.3.9
 --------
 2022-04-26: preserve Signature of the decorator
 
 v1.3.8
 --------
 2022-03-29: remedy mypy Untyped decorator makes function "cli_info" untyped
@@ -954,9 +1089,7 @@
 -------
 2017-11-30: using dill and multiprocess to enhance windows functionality
 
 v1.0.0
 -------
 2017-11-10: Initial public release
 
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wrapt_timeout_decorator-1.3.9/README.rst` & `wrapt_timeout_decorator-1.4.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,90 +1,104 @@
 wrapt_timeout_decorator
 =======================
 
 
-Version v1.3.9 as of 2022-04-26 see `Changelog`_
+Version v1.4.0 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/wrapt_timeout_decorator/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/wrapt_timeout_decorator/master?filepath=wrapt_timeout_decorator.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/wrapt-timeout-decorator?label=PyPI%20Package
    :target: https://badge.fury.io/py/wrapt_timeout_decorator
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/wrapt_timeout_decorator
    :target: https://codecov.io/gh/bitranox/wrapt_timeout_decorator
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/wrapt_timeout_decorator?branch=master
-   :target: https://bettercodehub.com/results/bitranox/wrapt_timeout_decorator
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/wrapt_timeout_decorator?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/wrapt_timeout_decorator?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/wrapt_timeout_decorator?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/wrapt_timeout_decorator
+.. |snyk| image:: https://snyk.io/test/github/bitranox/wrapt_timeout_decorator/badge.svg
    :target: https://snyk.io/test/github/bitranox/wrapt_timeout_decorator
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/wrapt-timeout-decorator
    :target: https://pypi.org/project/wrapt-timeout-decorator/
    :alt: PyPI - Downloads
 
-there are many timeout decorators out there - that one focuses on correctness when using with Classes, methods,
-class methods, static methods and so on, preserving also the traceback information for Pycharm debugging.
+There are several timeout decorators available, but the one mentioned here
+focuses on ensuring correctness when used with classes, methods, class methods,
+static methods, etc. It also preserves traceback information for PyCharm debugging.
+
+Additionally, there is a powerful eval function that allows reading
+the desired timeout value even from class attributes.
+
+Two timeout strategies have been implemented:
+one using "Signals" and the other using "Multiprocessing".
+
+Signals
+-------
+
+The "Signals" strategy (for POSIX Systems) is elegant and efficient,
+but it has some important caveats which should be reviewed
+in the `Caveats using Signals`_ section.
+
 
-There is also a powerful eval function, it allows to read the desired timeout value even from Class attributes.
+Multiprocessing
+---------------
 
-It is very flexible and can be used with python >= 3.6, pypy3 and probably other dialects.
+The default strategy is to use Multiprocessing
 
-There are two timeout strategies implemented, the ubiquitous method using "Signals" and the second using Multiprocessing.
-Using "Signals" is slick and lean, but there are nasty caveats, please check section `Caveats using Signals`_
+- on Windows, due to the lack of signals, this is only available choice, which is enforced automatically
+- signals (on POSIX) can not be used in a subthread, therefore multiprocessing is enforced in such cases
 
-The default strategy is therefore using Multiprocessing, but You can also use Signals, You have been warned !
+When using a subprocess many types from multiprocessing need to be pickable so that child processes can use them.
+Therefore we use "dill" instead of "pickle" and "multiprocess" instead of "multiprocessing".
 
-Due to the lack of signals on Windows, or for threaded functions (in a subthread) where signals cant be used, Your only choice is Multiprocessing,
-this is set automatically.
+dill extends python’s pickle module for serializing and de-serializing python objects to the majority of the built-in python types
 
-Under Windows the decorated function and results needs to be pickable.
-For that purpose we use "multiprocess" and "dill" instead of "multiprocessing" and "pickle", in order to be able to use this decorator on more sophisticated objects.
-Communication to the subprocess is done via "multiprocess.pipe" instead of "queue", which is faster and might also work on Amazon AWS.
+Communication with the subprocess is done via "multiprocess.pipe" instead of "queue",
+which offers improved speed and may also work on Amazon AWS.
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10.0, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/wrapt_timeout_decorator>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -123,20 +137,28 @@
             print('{} seconds have passed'.format(i))
 
     if __name__ == '__main__':
         mytest('starting')
 
 General Recommendations
 -----------------------
-dont sprincle Your code with timeouts. Just use it were absolutely necessary, for instance when reading or writing a file. And do that on the lowest
-abstraction level possible to avoid unwanted side effects (Exceptions caught by some other code, non pickable functions or arguments, and so on, but not TOO
-low. Remember that forking the program takes some time (when use multiprocessing).
+Minimize the excessive use of timeouts in your code and reserve their usage for essential cases.
+
+Implement timeouts at the lowest possible abstraction level to prevent unintended
+consequences such as exceptions being caught by unrelated code or non-pickable
+functions and arguments.
+
+Avoid incorporating the Timeout Decorator within a loop that iterates multiple times,
+as this can result in considerable time overhead,
+especially on Windows systems, when utilizing multiprocessing.
+
+Whenever feasible, leverage the existing built-in timeouts already provided by the functions
+and libraries you utilize. These built-in timeouts can handle most situations effectively.
+Only resort to use this Timeout Decorator as a last resort when all other alternatives have been exhausted.
 
-Most functions and libraries You call, they HAVE already some timeouts. use those. This Timeout Decorator should be only the last ressort, if everything else
-fails.
 
     BAD EXAMPLE (Pseudocode) - lets assume the write to the database fails sometimes for unknown reasons, and "hangs"
 
     .. code-block:: py
 
         # module file_analyzer
         import time
@@ -573,14 +595,74 @@
 .. warning::
     Make sure that in case of multiprocessing strategy for timeout, your function does not return objects which cannot
     be pickled, otherwise it will fail at marshalling it between master and child processes. To cover more cases,
     we use multiprocess and dill instead of multiprocessing and pickle.
 
     Since Signals will not work on Windows, it is disabled by default, whatever You set.
 
+
+Subprocess Monitoring
+---------------------
+
+when using multiprocessing, the subprocess is monitored if it is still alive.
+if the subprocess was terminated or killed (for instance by OOMKiller),
+``multiprocessing.context.ProcessError`` will be raised.
+By default the subprocess is monitored every 5 seconds, but can be set with parameter
+``dec_poll_subprocess``. polling can be turned off by setting to 0.0 seconds
+
+.. code-block:: python
+
+    from wrapt_timeout_decorator import timeout
+
+
+    @timeout(10, use_signals=False, timeout_exception=TimeoutError, dec_poll_subprocess=1)
+    def slow_process() -> None:
+        # should have enough time to finish
+        # but instead it gets terminated, and the
+        # poll the subprocess every second
+        logger.error(f"Slow process started at {get_str_time()}")
+        time.sleep(5)
+        logger.error(f"Slow process done at {get_str_time()}")
+
+
+    def fake_oom_killer() -> None:
+        logger.error(f"Fake OOMKiller started at {get_str_time()}")
+        time.sleep(2)
+        # kill sibling slow_process
+        # hacky way to find it
+        target = psutil.Process().parent().children(recursive=True)[-1]
+        target.kill()
+        logger.error(f"Killed {target.pid} at {get_str_time()}")
+
+
+    def start_processes() -> None:
+        """
+        starts the 'fake_oom_killer' and 'slow_process' process -
+        and kill 'slow_process' after two seconds
+
+        >>> start_processes()
+        Traceback (most recent call last):
+            ...
+        multiprocessing.context.ProcessError: Function slow_process was terminated or killed after ... seconds
+        """
+        process_oom_killer = multiprocessing.Process(target=fake_oom_killer, args=())
+        process_oom_killer.start()
+        slow_process()
+        process_oom_killer.join()
+
+
+    def get_str_time() -> str:
+        t = time.localtime()
+        current_time = time.strftime("%H:%M:%S", t)
+        return current_time
+
+
+    if __name__ == '__main__':
+        start_processes()
+
 use as function not as decorator
 --------------------------------
 
 You can use the timout also as function, without using as decorator:
 
 .. code-block:: py
 
@@ -756,14 +838,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade wrapt_timeout_decorator
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade wrapt_timeout_decorator[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/wrapt_timeout_decorator.git
 
@@ -779,22 +868,22 @@
     # for the latest development version :
     wrapt_timeout_decorator @ git+https://github.com/bitranox/wrapt_timeout_decorator.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/wrapt_timeout_decorator.git
     $ cd wrapt_timeout_decorator
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -819,16 +908,20 @@
 following modules will be automatically installed :
 
 .. code-block:: bash
 
     ## Project Requirements
     cli_exit_tools
     lib_detect_testenv
-    dill
+
+    # class decorators are failing on windows with dill 0.3.5, 0.3.5.1
+    dill>0.3.0,!=0.3.5,!=0.3.5.1;sys_platform=="win32"
+    dill;sys_platform!="win32"
     multiprocess
+    psutil
     wrapt
 
 Acknowledgements
 ----------------
 
 - special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"
 
@@ -844,14 +937,54 @@
 This software is licensed under the `MIT license <http://en.wikipedia.org/wiki/MIT_License>`_
 
 ---
 
 Changelog
 =========
 
+v1.4.0
+---------
+2023-07-13:
+    - check for killed child processes (for instance by OOMKiller)
+    - change dill requirements for windows
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
+v1.3.12.2
+---------
+2022-06-01: update to github actions checkout@v3 and setup-python@v3
+
+v1.3.12
+--------
+2022-05-23: update requirements.txt
+
+v1.3.11
+--------
+2022-05-23:
+    - set dill version < 0.3.5 on windows, because decorating class methods fails with dill 0.3.5 upwards
+    - update tests to the latest python versions
+
+v1.3.10
+--------
+2022-04-26: add tests for thread lock
+
 v1.3.9
 --------
 2022-04-26: preserve Signature of the decorator
 
 v1.3.8
 --------
 2022-03-29: remedy mypy Untyped decorator makes function "cli_info" untyped
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator/wrap_helper.py` & `wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator/wrap_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import signal
 import sys
 import threading
 from types import FrameType
 from typing import Any, Callable, Dict, List, Type, Union, Optional
 
 # EXT
-import dill  # type: ignore
-import multiprocess  # type: ignore
+import dill
+import multiprocess
 
 # Types
 AlarmHandler = Union[Callable[[int, Optional[FrameType]], Any], int, signal.Handlers, None]
 
 logger = logging.getLogger("pickle_analyzer")
 
 
@@ -22,67 +22,77 @@
         self,
         dec_timeout: Union[None, float, str],
         use_signals: bool,
         timeout_exception: Type[BaseException],
         exception_message: str,
         dec_allow_eval: bool,
         dec_hard_timeout: bool,
+        dec_poll_subprocess: float,
         wrapped: Callable[..., Any],
         instance: object,
         args: Any,
         kwargs: Any,
     ) -> None:
         self.dec_timeout = dec_timeout
         self.use_signals = use_signals
         self.timeout_exception = timeout_exception
         self.exception_message = exception_message
         self.dec_allow_eval = dec_allow_eval
         self.dec_hard_timeout = dec_hard_timeout
+        self.dec_poll_subprocess = dec_poll_subprocess
         self.wrapped = wrapped
         self.instance = instance
         self.args = args
         self.kwargs = kwargs
 
-        self.dec_timeout_float = 0.0  # type: float
+        self.dec_timeout_float: float = 0.0
         self.old_alarm_handler: AlarmHandler = None
         self.child_conn: "multiprocess.Pipe" = None
 
         self.pop_kwargs()
         self.set_signals_to_false_if_not_possible()
         self.eval_if_required()
         self.convert_timeout_given_to_float()
-        self.format_exception_message()
+        self.format_timeout_exception_message()
 
     def convert_timeout_given_to_float(self) -> None:
         if self.dec_timeout is None:
             self.dec_timeout_float = 0.0
         else:
             try:
                 self.dec_timeout_float = float(self.dec_timeout)
             except ValueError:
                 raise ValueError(f'the given or evaluated value for the timeout can not be converted to float : "{self.dec_timeout}"')
 
     def pop_kwargs(self) -> None:
-        self.dec_allow_eval = self.kwargs.pop("dec_allow_eval", self.dec_allow_eval)
+        """ this is to override the decorator settings with parameters given to the decorated function itself """
         self.dec_timeout = self.kwargs.pop("dec_timeout", self.dec_timeout)
         self.use_signals = self.kwargs.pop("use_signals", self.use_signals)
+        self.dec_allow_eval = self.kwargs.pop("dec_allow_eval", self.dec_allow_eval)
         self.dec_hard_timeout = self.kwargs.pop("dec_hard_timeout", self.dec_hard_timeout)
+        self.dec_poll_subprocess = self.kwargs.pop("dec_poll_subprocess", self.dec_poll_subprocess)
 
     @property
     def should_eval(self) -> bool:
         if self.dec_allow_eval and isinstance(self.dec_timeout, str):
             return True
         else:
             return False
 
-    def format_exception_message(self) -> None:
+    def format_timeout_exception_message(self) -> None:
+        # todo : make time human readable lib_cast
         function_name = self.wrapped.__name__ or "(unknown name)"
         if not self.exception_message:
             self.exception_message = f"Function {function_name} timed out after {self.dec_timeout_float} seconds"
 
+    def format_subprocess_exception_message(self, subprocess_run_time: float) -> None:
+        # todo : make time human readable lib_cast
+        function_name = self.wrapped.__name__ or "(unknown name)"
+        self.exception_message = f"Function {function_name} was terminated or killed after {subprocess_run_time} seconds"
+
     def new_alarm_handler(self, signum: signal.Signals, frame: FrameType) -> None:
         raise_exception(self.timeout_exception, self.exception_message)
 
     def save_old_and_set_new_alarm_handler(self) -> None:
         self.old_alarm_handler = signal.signal(signal.SIGALRM, self.new_alarm_handler)  # type: ignore
         signal.setitimer(signal.ITIMER_REAL, self.dec_timeout_float)  # type: ignore  # on windows we dont have signals
 
@@ -116,15 +126,15 @@
     )
     raise dill.PicklingError(s_err)
 
 
 def detect_unpickable_objects(object_to_pickle: Any, dill_trace: bool = True, log_warning: bool = True) -> Dict[str, Union[str, List[Any]]]:
     if log_warning:
         logger.warning('always remember that the "object_to_pickle" should not be defined within the main context')
-    dict_result = dict()  # type: Dict[str, Union[str, List[Any]]]
+    dict_result: Dict[str, Union[str, List[Any]]] = dict()
     dict_result["object_name"] = ""
     dict_result["bad_items"] = list()
     dict_result["bad_objects"] = list()
     dict_result["bad_types"] = list()
     safe_status_of_dill_trace = dill.detect.trace
     # noinspection PyBroadException
     try:
@@ -146,26 +156,26 @@
     if hasattr(object_to_pickle, "__name__"):
         if object_to_pickle.__name__:  # type: ignore
             object_name = object_to_pickle.__name__  # type: ignore
     return object_name
 
 
 def get_bad_pickling_types(object_to_pickle: object) -> List[Any]:
-    bad_types = list()  # type: List[Any]
+    bad_types: List[Any] = list()
     # noinspection PyBroadException
     try:
         bad_types = dill.detect.badtypes(object_to_pickle)
     except Exception:
         bad_types = [sys.exc_info()[1]]
     finally:
         return bad_types
 
 
 def get_bad_pickling_objects(object_to_pickle: Any) -> Any:
-    bad_objects = list()  # type: List[object]
+    bad_objects: List[object] = list()
     # noinspection PyBroadException
     try:
         bad_objects = dill.detect.badobjects(object_to_pickle)
     except Exception:
         bad_objects = [sys.exc_info()[1]]
     finally:
         return bad_objects
```

### Comparing `wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator/wrapt_timeout_decorator.py` & `wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator/wrapt_timeout_decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 """
 
 # STDLIB
 import sys
 from typing import Any, Callable, Type, TypeVar, Union
 
 # EXT
-from dill import PicklingError  # type: ignore
+from dill import PicklingError
 import wrapt
 
 # OWN
 try:
     from .wrap_helper import WrapHelper, detect_unpickable_objects_and_reraise
     from .wrap_function_multiprocess import Timeout
-except ImportError:  # pragma: no cover
+except (ImportError, ModuleNotFoundError):  # pragma: no cover
     # import for local doctest
     from wrap_helper import WrapHelper, detect_unpickable_objects_and_reraise  # type: ignore   # pragma: no cover
     from wrap_function_multiprocess import Timeout  # type: ignore  # pragma: no cover
 
 # to preserve Signature of the decorator
 F = TypeVar("F", bound=Callable[..., Any])
 
@@ -28,14 +28,15 @@
 def timeout(
     dec_timeout: Union[None, float, str] = None,
     use_signals: bool = True,
     timeout_exception: Type[BaseException] = TimeoutError,
     exception_message: str = "",
     dec_allow_eval: bool = False,
     dec_hard_timeout: bool = False,
+    dec_poll_subprocess: float = 5.0,
 ) -> Any:
 
     """Add a timeout parameter to a function and return it.
 
     ToDo :   not clear how to type a decorator factory,
              tried:   ->  Callable[..., Any]
                 ...
@@ -115,27 +116,33 @@
                                 if dec_hard_timeout = False, the decorator will timeout after the process is allowed to
                                 run for dec_timeout seconds, that means the time to set up the new process is not considered.
                                 If You set up a small timeout value like 0.1 seconds, in windows that function might now
                                 take something like 0.6 seconds to timeout - 0.5 seconds to set up the process, and
                                 allowing the function in the process to run for 0.1 seconds.
                                 Since You can not know how long the spawn() will take under Windows, this is the default setting.
 
+    :param dec_poll_subprocess: when using multiprocessing, monitor the subprocess if it is still alive.
+                                if the subprocess was terminated or killed (for instance by OOMKiller),
+                                multiprocessing.context.ProcessError will be raised.
+                                the default is 5.0 seconds, polling can be turned off by setting to 0.0 seconds
+
     * all parameters starting with dec_ can be overridden via kwargs passed to the wrapped function.
 
     :raises:                    TimeoutError if time limit is reached
     :returns:                   the Result of the wrapped function
 
     It is illegal to pass anything other than a function as the first parameter.
     The function is wrapped and returned to the caller.
     """
 
     @wrapt.decorator
     def wrapper(wrapped: F, instance: object, args: Any, kwargs: Any) -> Any:
         wrap_helper = WrapHelper(
-            dec_timeout, use_signals, timeout_exception, exception_message, dec_allow_eval, dec_hard_timeout, wrapped, instance, args, kwargs
+            dec_timeout, use_signals, timeout_exception, exception_message, dec_allow_eval, dec_hard_timeout, dec_poll_subprocess, wrapped, instance, args,
+            kwargs
         )
         if not wrap_helper.dec_timeout_float:
             return wrapped(*wrap_helper.args, **wrap_helper.kwargs)
         else:
             return wrapped_with_timeout(wrap_helper)
 
     return wrapper
```

### Comparing `wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator/wrapt_timeout_decorator_cli.py` & `wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator/wrapt_timeout_decorator_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,32 +26,32 @@
     >>> info()
     Info for ...
 
     """
     __init__conf__.print_info()
 
 
-@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)    # type: ignore
 @click.version_option(
     version=__init__conf__.version, prog_name=__init__conf__.shell_command, message=f"{__init__conf__.shell_command} version {__init__conf__.version}"
 )
 @click.option("--traceback/--no-traceback", is_flag=True, type=bool, default=None, help="return traceback information on cli")
 def cli_main(traceback: Optional[bool] = None) -> None:
     if traceback is not None:
         cli_exit_tools.config.traceback = traceback
 
 
-@cli_main.command("info", context_settings=CLICK_CONTEXT_SETTINGS)
+@cli_main.command("info", context_settings=CLICK_CONTEXT_SETTINGS)  # type: ignore
 def cli_info() -> None:
     """get program informations"""
     info()
 
 
 # entry point if main
 if __name__ == "__main__":
     try:
-        cli_main()
+        cli_main()  # type: ignore
     except Exception as exc:
         cli_exit_tools.print_exception_message()
         sys.exit(cli_exit_tools.get_system_exit_code(exc))
     finally:
         cli_exit_tools.flush_streams()
```

### Comparing `wrapt_timeout_decorator-1.3.9/wrapt_timeout_decorator.egg-info/PKG-INFO` & `wrapt_timeout_decorator-1.4.0/wrapt_timeout_decorator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,110 +1,126 @@
 Metadata-Version: 2.1
 Name: wrapt-timeout-decorator
-Version: 1.3.9
+Version: 1.4.0
 Summary: The better timout decorator
-Home-page: https://github.com/bitranox/wrapt_timeout_decorator
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/wrapt_timeout_decorator
+Project-URL: Documentation, https://github.com/bitranox/wrapt_timeout_decorator/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/wrapt_timeout_decorator.git
+Project-URL: Changelog, https://github.com/bitranox/wrapt_timeout_decorator/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 wrapt_timeout_decorator
 =======================
 
 
-Version v1.3.9 as of 2022-04-26 see `Changelog`_
+Version v1.4.0 as of 2023-07-14 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/wrapt_timeout_decorator/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/wrapt_timeout_decorator/master?filepath=wrapt_timeout_decorator.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/wrapt-timeout-decorator?label=PyPI%20Package
    :target: https://badge.fury.io/py/wrapt_timeout_decorator
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/wrapt_timeout_decorator
    :target: https://codecov.io/gh/bitranox/wrapt_timeout_decorator
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/wrapt_timeout_decorator?branch=master
-   :target: https://bettercodehub.com/results/bitranox/wrapt_timeout_decorator
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/wrapt_timeout_decorator?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/wrapt_timeout_decorator?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/wrapt_timeout_decorator?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/wrapt_timeout_decorator
+.. |snyk| image:: https://snyk.io/test/github/bitranox/wrapt_timeout_decorator/badge.svg
    :target: https://snyk.io/test/github/bitranox/wrapt_timeout_decorator
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/wrapt-timeout-decorator
    :target: https://pypi.org/project/wrapt-timeout-decorator/
    :alt: PyPI - Downloads
 
-there are many timeout decorators out there - that one focuses on correctness when using with Classes, methods,
-class methods, static methods and so on, preserving also the traceback information for Pycharm debugging.
+There are several timeout decorators available, but the one mentioned here
+focuses on ensuring correctness when used with classes, methods, class methods,
+static methods, etc. It also preserves traceback information for PyCharm debugging.
+
+Additionally, there is a powerful eval function that allows reading
+the desired timeout value even from class attributes.
+
+Two timeout strategies have been implemented:
+one using "Signals" and the other using "Multiprocessing".
+
+Signals
+-------
+
+The "Signals" strategy (for POSIX Systems) is elegant and efficient,
+but it has some important caveats which should be reviewed
+in the `Caveats using Signals`_ section.
+
 
-There is also a powerful eval function, it allows to read the desired timeout value even from Class attributes.
+Multiprocessing
+---------------
 
-It is very flexible and can be used with python >= 3.6, pypy3 and probably other dialects.
+The default strategy is to use Multiprocessing
 
-There are two timeout strategies implemented, the ubiquitous method using "Signals" and the second using Multiprocessing.
-Using "Signals" is slick and lean, but there are nasty caveats, please check section `Caveats using Signals`_
+- on Windows, due to the lack of signals, this is only available choice, which is enforced automatically
+- signals (on POSIX) can not be used in a subthread, therefore multiprocessing is enforced in such cases
 
-The default strategy is therefore using Multiprocessing, but You can also use Signals, You have been warned !
+When using a subprocess many types from multiprocessing need to be pickable so that child processes can use them.
+Therefore we use "dill" instead of "pickle" and "multiprocess" instead of "multiprocessing".
 
-Due to the lack of signals on Windows, or for threaded functions (in a subthread) where signals cant be used, Your only choice is Multiprocessing,
-this is set automatically.
+dill extends python’s pickle module for serializing and de-serializing python objects to the majority of the built-in python types
 
-Under Windows the decorated function and results needs to be pickable.
-For that purpose we use "multiprocess" and "dill" instead of "multiprocessing" and "pickle", in order to be able to use this decorator on more sophisticated objects.
-Communication to the subprocess is done via "multiprocess.pipe" instead of "queue", which is faster and might also work on Amazon AWS.
+Communication with the subprocess is done via "multiprocess.pipe" instead of "queue",
+which offers improved speed and may also work on Amazon AWS.
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10.0, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/wrapt_timeout_decorator>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/wrapt_timeout_decorator/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/wrapt_timeout_decorator/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -143,20 +159,28 @@
             print('{} seconds have passed'.format(i))
 
     if __name__ == '__main__':
         mytest('starting')
 
 General Recommendations
 -----------------------
-dont sprincle Your code with timeouts. Just use it were absolutely necessary, for instance when reading or writing a file. And do that on the lowest
-abstraction level possible to avoid unwanted side effects (Exceptions caught by some other code, non pickable functions or arguments, and so on, but not TOO
-low. Remember that forking the program takes some time (when use multiprocessing).
+Minimize the excessive use of timeouts in your code and reserve their usage for essential cases.
+
+Implement timeouts at the lowest possible abstraction level to prevent unintended
+consequences such as exceptions being caught by unrelated code or non-pickable
+functions and arguments.
+
+Avoid incorporating the Timeout Decorator within a loop that iterates multiple times,
+as this can result in considerable time overhead,
+especially on Windows systems, when utilizing multiprocessing.
+
+Whenever feasible, leverage the existing built-in timeouts already provided by the functions
+and libraries you utilize. These built-in timeouts can handle most situations effectively.
+Only resort to use this Timeout Decorator as a last resort when all other alternatives have been exhausted.
 
-Most functions and libraries You call, they HAVE already some timeouts. use those. This Timeout Decorator should be only the last ressort, if everything else
-fails.
 
     BAD EXAMPLE (Pseudocode) - lets assume the write to the database fails sometimes for unknown reasons, and "hangs"
 
     .. code-block:: py
 
         # module file_analyzer
         import time
@@ -593,14 +617,74 @@
 .. warning::
     Make sure that in case of multiprocessing strategy for timeout, your function does not return objects which cannot
     be pickled, otherwise it will fail at marshalling it between master and child processes. To cover more cases,
     we use multiprocess and dill instead of multiprocessing and pickle.
 
     Since Signals will not work on Windows, it is disabled by default, whatever You set.
 
+
+Subprocess Monitoring
+---------------------
+
+when using multiprocessing, the subprocess is monitored if it is still alive.
+if the subprocess was terminated or killed (for instance by OOMKiller),
+``multiprocessing.context.ProcessError`` will be raised.
+By default the subprocess is monitored every 5 seconds, but can be set with parameter
+``dec_poll_subprocess``. polling can be turned off by setting to 0.0 seconds
+
+.. code-block:: python
+
+    from wrapt_timeout_decorator import timeout
+
+
+    @timeout(10, use_signals=False, timeout_exception=TimeoutError, dec_poll_subprocess=1)
+    def slow_process() -> None:
+        # should have enough time to finish
+        # but instead it gets terminated, and the
+        # poll the subprocess every second
+        logger.error(f"Slow process started at {get_str_time()}")
+        time.sleep(5)
+        logger.error(f"Slow process done at {get_str_time()}")
+
+
+    def fake_oom_killer() -> None:
+        logger.error(f"Fake OOMKiller started at {get_str_time()}")
+        time.sleep(2)
+        # kill sibling slow_process
+        # hacky way to find it
+        target = psutil.Process().parent().children(recursive=True)[-1]
+        target.kill()
+        logger.error(f"Killed {target.pid} at {get_str_time()}")
+
+
+    def start_processes() -> None:
+        """
+        starts the 'fake_oom_killer' and 'slow_process' process -
+        and kill 'slow_process' after two seconds
+
+        >>> start_processes()
+        Traceback (most recent call last):
+            ...
+        multiprocessing.context.ProcessError: Function slow_process was terminated or killed after ... seconds
+        """
+        process_oom_killer = multiprocessing.Process(target=fake_oom_killer, args=())
+        process_oom_killer.start()
+        slow_process()
+        process_oom_killer.join()
+
+
+    def get_str_time() -> str:
+        t = time.localtime()
+        current_time = time.strftime("%H:%M:%S", t)
+        return current_time
+
+
+    if __name__ == '__main__':
+        start_processes()
+
 use as function not as decorator
 --------------------------------
 
 You can use the timout also as function, without using as decorator:
 
 .. code-block:: py
 
@@ -776,14 +860,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade wrapt_timeout_decorator
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade wrapt_timeout_decorator[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/wrapt_timeout_decorator.git
 
@@ -799,22 +890,22 @@
     # for the latest development version :
     wrapt_timeout_decorator @ git+https://github.com/bitranox/wrapt_timeout_decorator.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/wrapt_timeout_decorator.git
     $ cd wrapt_timeout_decorator
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -839,16 +930,20 @@
 following modules will be automatically installed :
 
 .. code-block:: bash
 
     ## Project Requirements
     cli_exit_tools
     lib_detect_testenv
-    dill
+
+    # class decorators are failing on windows with dill 0.3.5, 0.3.5.1
+    dill>0.3.0,!=0.3.5,!=0.3.5.1;sys_platform=="win32"
+    dill;sys_platform!="win32"
     multiprocess
+    psutil
     wrapt
 
 Acknowledgements
 ----------------
 
 - special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"
 
@@ -864,14 +959,54 @@
 This software is licensed under the `MIT license <http://en.wikipedia.org/wiki/MIT_License>`_
 
 ---
 
 Changelog
 =========
 
+v1.4.0
+---------
+2023-07-13:
+    - check for killed child processes (for instance by OOMKiller)
+    - change dill requirements for windows
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
+v1.3.12.2
+---------
+2022-06-01: update to github actions checkout@v3 and setup-python@v3
+
+v1.3.12
+--------
+2022-05-23: update requirements.txt
+
+v1.3.11
+--------
+2022-05-23:
+    - set dill version < 0.3.5 on windows, because decorating class methods fails with dill 0.3.5 upwards
+    - update tests to the latest python versions
+
+v1.3.10
+--------
+2022-04-26: add tests for thread lock
+
 v1.3.9
 --------
 2022-04-26: preserve Signature of the decorator
 
 v1.3.8
 --------
 2022-03-29: remedy mypy Untyped decorator makes function "cli_info" untyped
@@ -954,9 +1089,7 @@
 -------
 2017-11-30: using dill and multiprocess to enhance windows functionality
 
 v1.0.0
 -------
 2017-11-10: Initial public release
 
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

