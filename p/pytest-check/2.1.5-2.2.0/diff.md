# Comparing `tmp/pytest_check-2.1.5.tar.gz` & `tmp/pytest_check-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_check-2.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_check-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_check-2.1.5.tar` & `pytest_check-2.2.0.tar`

### file list

```diff
@@ -1,65 +1,69 @@
--rw-r--r--   0        0        0     1079 2023-06-06 21:59:29.997499 pytest_check-2.1.5/LICENSE.txt
--rw-r--r--   0        0        0     8651 2023-06-06 21:59:29.997499 pytest_check-2.1.5/README.md
--rw-r--r--   0        0        0     8369 2023-06-06 21:59:29.997499 pytest_check-2.1.5/changelog.md
--rw-r--r--   0        0        0      564 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_alt_names.py
--rw-r--r--   0        0        0      535 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_any_failures.py
--rw-r--r--   0        0        0      187 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_check_and_assert.py
--rw-r--r--   0        0        0      269 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_check_check.py
--rw-r--r--   0        0        0      519 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_check_func_decorator.py
--rw-r--r--   0        0        0      483 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_check_not_in_test.py
--rw-r--r--   0        0        0      724 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_context_functions.py
--rw-r--r--   0        0        0      521 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_context_manager_fail.py
--rw-r--r--   0        0        0      325 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_context_manager_pass.py
--rw-r--r--   0        0        0      331 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_fail_in_fixture.py
--rw-r--r--   0        0        0      448 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_fail_in_thread.py
--rw-r--r--   0        0        0     1536 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_functions_fail.py
--rw-r--r--   0        0        0     1718 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_functions_pass.py
--rw-r--r--   0        0        0      358 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_helpers.py
--rw-r--r--   0        0        0      772 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_httpx.py
--rw-r--r--   0        0        0     1175 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_logging.py
--rw-r--r--   0        0        0      769 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_maxfail.py
--rw-r--r--   0        0        0      185 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_message.py
--rw-r--r--   0        0        0      413 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_mix_checks_and_assertions.py
--rw-r--r--   0        0        0      118 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_multiple_failures.py
--rw-r--r--   0        0        0      384 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_pass_in_thread.py
--rw-r--r--   0        0        0      487 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_raises.py
--rw-r--r--   0        0        0      208 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_simple.py
--rw-r--r--   0        0        0      421 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_speedup_funcs.py
--rw-r--r--   0        0        0      604 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_stop_on_fail.py
--rw-r--r--   0        0        0      358 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_tb_style.py
--rw-r--r--   0        0        0     1101 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_traceback.py
--rw-r--r--   0        0        0      502 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_xfail.py
--rw-r--r--   0        0        0      685 2023-06-06 21:59:30.001499 pytest_check-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     1434 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/__init__.py
--rw-r--r--   0        0        0     5081 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/check_functions.py
--rw-r--r--   0        0        0     1602 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/check_log.py
--rw-r--r--   0        0        0     3831 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/check_raises.py
--rw-r--r--   0        0        0     1551 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/context_manager.py
--rw-r--r--   0        0        0     3363 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/plugin.py
--rw-r--r--   0        0        0     1493 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/pseudo_traceback.py
--rw-r--r--   0        0        0        0 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/conftest.py
--rw-r--r--   0        0        0      600 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_alt_names.py
--rw-r--r--   0        0        0      986 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_any_failures.py
--rw-r--r--   0        0        0      229 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_check_and_assert.py
--rw-r--r--   0        0        0      179 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_check_check.py
--rw-r--r--   0        0        0     1061 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_check_context_manager.py
--rw-r--r--   0        0        0       53 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_check_fixture.py
--rw-r--r--   0        0        0      740 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_check_func_decorator.py
--rw-r--r--   0        0        0      536 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_fail_in_fixture.py
--rw-r--r--   0        0        0      392 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_functions.py
--rw-r--r--   0        0        0     1522 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_helpers.py
--rw-r--r--   0        0        0     1352 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_logging.py
--rw-r--r--   0        0        0     1036 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_maxfail.py
--rw-r--r--   0        0        0      505 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_message.py
--rw-r--r--   0        0        0     1018 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_not_in_test.py
--rw-r--r--   0        0        0     5413 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_raises.py
--rw-r--r--   0        0        0      860 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_red.py
--rw-r--r--   0        0        0     2500 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_speedup_flags.py
--rw-r--r--   0        0        0     2647 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_speedup_functions.py
--rw-r--r--   0        0        0      924 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_stop_on_fail.py
--rw-r--r--   0        0        0      713 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_tb_style.py
--rw-r--r--   0        0        0      508 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_thread.py
--rw-r--r--   0        0        0     1018 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_xfail.py
--rw-r--r--   0        0        0      859 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tox.ini
--rw-r--r--   0        0        0     9018 1970-01-01 00:00:00.000000 pytest_check-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-14 19:48:04.857371 pytest_check-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     8651 2023-07-14 19:48:04.857371 pytest_check-2.2.0/README.md
+-rw-r--r--   0        0        0     8840 2023-07-14 19:48:04.857371 pytest_check-2.2.0/changelog.md
+-rw-r--r--   0        0        0      564 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_alt_names.py
+-rw-r--r--   0        0        0      535 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_any_failures.py
+-rw-r--r--   0        0        0      187 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_check_and_assert.py
+-rw-r--r--   0        0        0      269 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_check_check.py
+-rw-r--r--   0        0        0      519 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_check_func_decorator.py
+-rw-r--r--   0        0        0      483 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_check_not_in_test.py
+-rw-r--r--   0        0        0      724 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_context_functions.py
+-rw-r--r--   0        0        0      521 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_context_manager_fail.py
+-rw-r--r--   0        0        0      325 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_context_manager_pass.py
+-rw-r--r--   0        0        0      331 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_fail_in_fixture.py
+-rw-r--r--   0        0        0      448 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_fail_in_thread.py
+-rw-r--r--   0        0        0     1536 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_functions_fail.py
+-rw-r--r--   0        0        0     1718 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_functions_pass.py
+-rw-r--r--   0        0        0      358 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_helpers.py
+-rw-r--r--   0        0        0      772 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_httpx.py
+-rw-r--r--   0        0        0      241 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_locals.py
+-rw-r--r--   0        0        0     1175 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_logging.py
+-rw-r--r--   0        0        0      769 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_maxfail.py
+-rw-r--r--   0        0        0      185 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_message.py
+-rw-r--r--   0        0        0      413 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_mix_checks_and_assertions.py
+-rw-r--r--   0        0        0      118 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_multiple_failures.py
+-rw-r--r--   0        0        0      384 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_pass_in_thread.py
+-rw-r--r--   0        0        0      487 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_raises.py
+-rw-r--r--   0        0        0      208 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_simple.py
+-rw-r--r--   0        0        0      421 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_speedup_funcs.py
+-rw-r--r--   0        0        0      604 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_stop_on_fail.py
+-rw-r--r--   0        0        0      358 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_tb_style.py
+-rw-r--r--   0        0        0     1102 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_traceback.py
+-rw-r--r--   0        0        0      290 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_tracebackhide.py
+-rw-r--r--   0        0        0      502 2023-07-14 19:48:04.857371 pytest_check-2.2.0/examples/test_example_xfail.py
+-rw-r--r--   0        0        0      685 2023-07-14 19:48:04.857371 pytest_check-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1434 2023-07-14 19:48:04.857371 pytest_check-2.2.0/src/pytest_check/__init__.py
+-rw-r--r--   0        0        0     5081 2023-07-14 19:48:04.857371 pytest_check-2.2.0/src/pytest_check/check_functions.py
+-rw-r--r--   0        0        0     1800 2023-07-14 19:48:04.857371 pytest_check-2.2.0/src/pytest_check/check_log.py
+-rw-r--r--   0        0        0     3831 2023-07-14 19:48:04.857371 pytest_check-2.2.0/src/pytest_check/check_raises.py
+-rw-r--r--   0        0        0     1669 2023-07-14 19:48:04.857371 pytest_check-2.2.0/src/pytest_check/context_manager.py
+-rw-r--r--   0        0        0     3065 2023-07-14 19:48:04.861371 pytest_check-2.2.0/src/pytest_check/plugin.py
+-rw-r--r--   0        0        0     3567 2023-07-14 19:48:04.861371 pytest_check-2.2.0/src/pytest_check/pseudo_traceback.py
+-rw-r--r--   0        0        0        0 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      600 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_alt_names.py
+-rw-r--r--   0        0        0      986 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_any_failures.py
+-rw-r--r--   0        0        0      229 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_check_and_assert.py
+-rw-r--r--   0        0        0      179 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_check_check.py
+-rw-r--r--   0        0        0     1103 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_check_context_manager.py
+-rw-r--r--   0        0        0       53 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_check_fixture.py
+-rw-r--r--   0        0        0      740 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_check_func_decorator.py
+-rw-r--r--   0        0        0      536 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_fail_in_fixture.py
+-rw-r--r--   0        0        0      392 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_functions.py
+-rw-r--r--   0        0        0     1036 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_helpers.py
+-rw-r--r--   0        0        0      639 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_locals.py
+-rw-r--r--   0        0        0     1352 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_logging.py
+-rw-r--r--   0        0        0     1036 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_maxfail.py
+-rw-r--r--   0        0        0      505 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_message.py
+-rw-r--r--   0        0        0      952 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_not_in_test.py
+-rw-r--r--   0        0        0     5413 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_raises.py
+-rw-r--r--   0        0        0      941 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_red.py
+-rw-r--r--   0        0        0     2503 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_speedup_flags.py
+-rw-r--r--   0        0        0     2647 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_speedup_functions.py
+-rw-r--r--   0        0        0      924 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_stop_on_fail.py
+-rw-r--r--   0        0        0      713 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_tb_style.py
+-rw-r--r--   0        0        0      508 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_thread.py
+-rw-r--r--   0        0        0     1343 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_tracebackhide.py
+-rw-r--r--   0        0        0     1018 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tests/test_xfail.py
+-rw-r--r--   0        0        0      888 2023-07-14 19:48:04.861371 pytest_check-2.2.0/tox.ini
+-rw-r--r--   0        0        0     9018 1970-01-01 00:00:00.000000 pytest_check-2.2.0/PKG-INFO
```

### Comparing `pytest_check-2.1.5/LICENSE.txt` & `pytest_check-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/README.md` & `pytest_check-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/changelog.md` & `pytest_check-2.2.0/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,31 @@
 - nothing so far
 
 ### Changed
 
 - nothing so far
 
 -->
+## [2.2.0] - 2023-July-14
+
+### Added
+- 
+- pseudo traceback additions
+- `-l` or `--showlocals` shows locals
+- `__tracebackhide__ = True` is honored.
+- if `assert` or other exception is involved,
+  - the exception is included as part of the traceback.
+
+### Changed
+
+- pseudo traceback changes
+- The red color is used more selectively.
+  - this is intended to help readability
+- Other minor formatting changes.
+  - Please let me know if you have any issues with the changes
 
 ## [2.1.5] - 2023-June-6
 
 ### Fixed
 
 - Fix [127](https://github.com/okken/pytest-check/issues/127) IndexError when running a check in a thread -  Thanks [fperrin](https://github.com/fperrin)
```

### Comparing `pytest_check-2.1.5/examples/test_example_alt_names.py` & `pytest_check-2.2.0/examples/test_example_alt_names.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/examples/test_example_any_failures.py` & `pytest_check-2.2.0/examples/test_example_any_failures.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/examples/test_example_check_func_decorator.py` & `pytest_check-2.2.0/examples/test_example_check_func_decorator.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/examples/test_example_context_functions.py` & `pytest_check-2.2.0/examples/test_example_context_functions.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/examples/test_example_context_manager_fail.py` & `pytest_check-2.2.0/examples/test_example_context_manager_fail.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/examples/test_example_functions_fail.py` & `pytest_check-2.2.0/examples/test_example_functions_fail.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/examples/test_example_functions_pass.py` & `pytest_check-2.2.0/examples/test_example_functions_pass.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/examples/test_example_httpx.py` & `pytest_check-2.2.0/examples/test_example_httpx.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/examples/test_example_logging.py` & `pytest_check-2.2.0/examples/test_example_logging.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/examples/test_example_maxfail.py` & `pytest_check-2.2.0/examples/test_example_maxfail.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/examples/test_example_stop_on_fail.py` & `pytest_check-2.2.0/examples/test_example_stop_on_fail.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/examples/test_example_traceback.py` & `pytest_check-2.2.0/examples/test_example_traceback.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,7 +56,8 @@
 def helper2_assert():
     assert 1 == 2, "assert message"
 
 
 def test_tb_ctx_assert(check):
     with check("check message"):
         helper_assert()
+
```

### Comparing `pytest_check-2.1.5/pyproject.toml` & `pytest_check-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "pytest-check"
 authors = [{name = "Brian Okken"}]
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 description="A pytest plugin that allows multiple failures per test."
-version = "2.1.5"
+version = "2.2.0"
 requires-python = ">3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Framework :: Pytest" ,
 ]
 dependencies = ["pytest"]
```

### Comparing `pytest_check-2.1.5/src/pytest_check/__init__.py` & `pytest_check-2.2.0/src/pytest_check/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/src/pytest_check/check_functions.py` & `pytest_check-2.2.0/src/pytest_check/check_functions.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/src/pytest_check/check_log.py` & `pytest_check-2.2.0/src/pytest_check/check_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 _max_fail = None
 _max_report = None
 _max_tb = None
 _num_failures = 0
 _fail_function = None
 
+_showlocals = False
 
 def clear_failures():
     # get's called at the beginning of each test function
     global _failures, _num_failures
     global _max_fail, _max_report, _max_tb
     _failures = []
     _num_failures = 0
@@ -32,33 +33,35 @@
     return bool(get_failures())
 
 
 def get_failures():
     return _failures
 
 
-def log_failure(msg="", check_str=""):
+def log_failure(msg="", check_str="", tb=None):
     global _num_failures
     __tracebackhide__ = True
     _num_failures += 1
 
     msg = str(msg).strip()
 
     if check_str:
         msg = f"{msg}: {check_str}"
 
     if (_max_report is None) or (_num_failures <= _max_report):
         if _num_failures <= _max_tb:
-            pseudo_trace_str = _build_pseudo_trace_str()
+            pseudo_trace_str = _build_pseudo_trace_str(_showlocals,
+                                                       tb,
+                                                       should_use_color)
             msg = f"{msg}\n{pseudo_trace_str}"
 
         if should_use_color:
-            msg = f"{COLOR_RED}{msg}{COLOR_RESET}"
-
-        msg = f"FAILURE: {msg}"
+            msg = f"{COLOR_RED}FAILURE: {COLOR_RESET}{msg}"
+        else:
+            msg = f"FAILURE: {msg}"
         _failures.append(msg)
         if _fail_function:
             _fail_function(msg)
 
     if _max_fail and (_num_failures >= _max_fail):
         assert_msg = f"pytest-check max fail of {_num_failures} reached"
         assert _num_failures < _max_fail, assert_msg
```

### Comparing `pytest_check-2.1.5/src/pytest_check/check_raises.py` & `pytest_check-2.2.0/src/pytest_check/check_raises.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/src/pytest_check/context_manager.py` & `pytest_check-2.2.0/src/pytest_check/context_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+import traceback
 from . import check_log
 from .check_log import log_failure
 
 _stop_on_fail = False
 
 # This class has grown into much more than just a context manager.
 # it's really the interface into the system.
@@ -20,18 +21,19 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         __tracebackhide__ = True
         if exc_type is not None and issubclass(exc_type, AssertionError):
             if _stop_on_fail:
                 self.msg = None
                 return
             else:
+                fmt_tb = traceback.format_exception(exc_type, exc_val, exc_tb)
                 if self.msg is not None:
-                    log_failure(f"{self.msg}\n{exc_val}")
+                    log_failure(f"{exc_val}, {self.msg}", tb=fmt_tb)
                 else:
-                    log_failure(exc_val)
+                    log_failure(exc_val, tb=fmt_tb)
                 self.msg = None
                 return True
         self.msg = None
 
     def __call__(self, msg=None):
         self.msg = msg
         return self
```

### Comparing `pytest_check-2.1.5/src/pytest_check/plugin.py` & `pytest_check-2.2.0/src/pytest_check/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-import warnings
 
 import pytest
 from _pytest._code.code import ExceptionInfo
 from _pytest.skipping import xfailed_key
 
 from . import check_log, check_raises, context_manager, pseudo_traceback
 
@@ -57,43 +56,33 @@
     context_manager._stop_on_fail = stop_on_fail
     check_raises._stop_on_fail = stop_on_fail
     check_log._stop_on_fail = stop_on_fail
 
     # Allow for --tb=no to turn off check's pseudo tbs
     traceback_style = config.getvalue("tbstyle")
     pseudo_traceback._traceback_style = traceback_style
+    check_log._showlocals = config.getvalue('showlocals')
 
     # grab options
     check_log._default_max_fail = config.getoption("--check-max-fail")
     check_log._default_max_report = config.getoption("--check-max-report")
     check_log._default_max_tb = config.getoption("--check-max-tb")
-    no_tb = config.getoption("--check-no-tb")
-    if no_tb:
-        warnings.warn(
-            "--check-no-tb is deprecated; use --check-max-tb=0", DeprecationWarning
-        )
-        check_log._default_max_tb = 0
 
 
 # Allow for tests to grab "check" via fixture:
 # def test_a(check):
 #    check.equal(a, b)
 @pytest.fixture(name="check")
 def check_fixture():
     return context_manager.check
 
 
 # add some options
 def pytest_addoption(parser):
     parser.addoption(
-        "--check-no-tb",
-        action="store_true",
-        help="turn off pseudo-tracebacks",
-    )
-    parser.addoption(
         "--check-max-report",
         action="store",
         type=int,
         help="max failures to report",
     )
     parser.addoption(
         "--check-max-fail",
```

### Comparing `pytest_check-2.1.5/tests/test_alt_names.py` & `pytest_check-2.2.0/tests/test_alt_names.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/tests/test_any_failures.py` & `pytest_check-2.2.0/tests/test_any_failures.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/tests/test_check_context_manager.py` & `pytest_check-2.2.0/tests/test_check_context_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,13 +20,13 @@
 
 def test_context_manager_fail_with_msg(pytester):
     pytester.copy_example("examples/test_example_context_manager_fail.py")
     result = pytester.runpytest("-k", "test_messages")
     result.assert_outcomes(failed=1, passed=0)
     result.stdout.fnmatch_lines(
         [
-            "*FAILURE: first fail*",
-            "*FAILURE: second fail*",
-            "*FAILURE: third fail*",
+            "*FAILURE: assert 1 == 0, first fail*",
+            "*FAILURE: assert 1 > 2, second fail*",
+            "*FAILURE: assert 5 < 4, third fail*",
             "*Failed Checks: 3*",
         ],
-    )
+    )
```

### Comparing `pytest_check-2.1.5/tests/test_check_func_decorator.py` & `pytest_check-2.2.0/tests/test_check_func_decorator.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/tests/test_fail_in_fixture.py` & `pytest_check-2.2.0/tests/test_fail_in_fixture.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/tests/test_helpers.py` & `pytest_check-2.2.0/tests/test_tracebackhide.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 import sys
-
 import pytest
 
 
-# the output is different in prior versions.
 @pytest.mark.skipif(sys.version_info < (3, 10), reason="requires python3.10 or higher")
-def test_sequence_with_helper_funcs(pytester):
+def test_normal_pseudo_traceback(pytester):
     """
     Should show a sequence of calls
     """
     pytester.copy_example("examples/test_example_helpers.py")
     result = pytester.runpytest("--check-max-tb=2")
     result.assert_outcomes(failed=1, passed=0)
     result.stdout.fnmatch_lines(
         [
-            "*FAILURE: first",
+            "*FAILURE: assert 1 == 0, first",
             "*in test_func() -> helper1()",
             "*in helper1() -> helper2()",
-            '*in helper2() -> with check("first"):',
-            "*FAILURE: second",
+            "*in helper2 -> assert 1 == 0",
+            "*AssertionError: assert 1 == 0",
+
+            "*FAILURE: assert 1 > 2, second",
             "*in test_func() -> helper1()",
             "*in helper1() -> helper2()",
-            '*in helper2() -> with check("second"):',
+            "*in helper2 -> assert 1 > 2",
+            "*AssertionError: assert 1 > 2",
             "*Failed Checks: 2*",
         ],
     )
 
-
-def test_sequence_with_helper_funcs_less_checking(pytester):
+@pytest.mark.skipif(sys.version_info < (3, 10), reason="requires python3.10 or higher")
+def test_tracebackhide(pytester):
     """
-    Should show a sequence of calls
+    Should skip helper1, since it has __tracebackhide__ = True
     """
-    pytester.copy_example("examples/test_example_helpers.py")
+    pytester.copy_example("examples/test_example_tracebackhide.py")
     result = pytester.runpytest("--check-max-tb=2")
     result.assert_outcomes(failed=1, passed=0)
-    result.stdout.fnmatch_lines(
-        [
-            "*FAILURE: first",
-            "*in test_func() -> helper1()",
-            "*in helper1() -> helper2()",
-            "*in helper2()*",
-            "*FAILURE: second",
-            "*in test_func() -> helper1()",
-            "*in helper1() -> helper2()",
-            "*in helper2()*",
-            "*Failed Checks: 2*",
-        ],
-    )
+    result.stdout.no_fnmatch_line("*in helper1() -> helper2()")
+
```

### Comparing `pytest_check-2.1.5/tests/test_logging.py` & `pytest_check-2.2.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/tests/test_maxfail.py` & `pytest_check-2.2.0/tests/test_maxfail.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/tests/test_not_in_test.py` & `pytest_check-2.2.0/tests/test_not_in_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,13 +19,12 @@
     result = pytester.runpytest()
     result.assert_outcomes(errors=1, failed=0, passed=0)
     result.stdout.fnmatch_lines(
         [
             "* ERROR at setup of test_something *",
             "*FAILURE: assert 1 == 0*",
             "*not_in_test.py:* in not_in_a_test() -> helper_func()*",
-            "*not_in_test.py:* in helper_func() -> with check:*",
             "*Failed Checks: 1*",
             "* short test summary info *",
             "*ERROR test_example_check_not_in_test.py::test_something*",
         ],
     )
```

### Comparing `pytest_check-2.1.5/tests/test_raises.py` & `pytest_check-2.2.0/tests/test_raises.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/tests/test_red.py` & `pytest_check-2.2.0/tests/test_red.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,18 @@
     Should have red in failure.
     """
     pytester.copy_example("examples/test_example_simple.py")
     result = pytester.runpytest("--color=yes")
     result.assert_outcomes(failed=1, passed=1)
     result.stdout.fnmatch_lines(
         [
-            "*FAILURE:*[31massert*",  # red before assert
-            "*[0m*",  # reset after
+            "*[31mFAILURE:*[0massert*",
+            "*[31mtest_example_simple.py*[0m:14 in test_fail*",
+            "*[31mAssertionError: assert 1 == 2*",
+            "*[0m*"
         ],
     )
 
 
 def test_no_red(pytester):
     """
     Should NOT have red in failure.
```

### Comparing `pytest_check-2.1.5/tests/test_speedup_flags.py` & `pytest_check-2.2.0/tests/test_speedup_flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             "Failed Checks: 10",
         ],
     )
 
 
 def test_no_tb(pytester):
     pytester.copy_example("examples/test_example_multiple_failures.py")
-    result = pytester.runpytest("--check-no-tb")
+    result = pytester.runpytest("--check-max-tb=0")
     result.assert_outcomes(failed=1)
     result.stdout.fnmatch_lines(
         [
             "*FAILURE: * 7 == 100",
             "*FAILURE: * 8 == 100",
             "*FAILURE: * 9 == 100",
             "Failed Checks: 10",
```

### Comparing `pytest_check-2.1.5/tests/test_speedup_functions.py` & `pytest_check-2.2.0/tests/test_speedup_functions.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/tests/test_stop_on_fail.py` & `pytest_check-2.2.0/tests/test_stop_on_fail.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/tests/test_tb_style.py` & `pytest_check-2.2.0/tests/test_tb_style.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/tests/test_xfail.py` & `pytest_check-2.2.0/tests/test_xfail.py`

 * *Files identical despite different names*

### Comparing `pytest_check-2.1.5/tox.ini` & `pytest_check-2.2.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tox]
-envlist = py37, py38, py39, py310, py311, py312,
-          coverage, lint
+envlist = py37, py38, py39, py310, py311, py312, coverage, lint
 
 skip_missing_interpreters = true
 
 [testenv]
 commands = pytest {posargs}
 description = Run pytest
+package = wheel
+wheel_build_env = .pkg
 
 ; there's a weird thing going on with 3.12b2, pip, and pytest
 [testenv:py312]
 ignore_outcome = true 
 basepython = python3.12
 commands = pytest {posargs}
 description = Run pytest
```

### Comparing `pytest_check-2.1.5/PKG-INFO` & `pytest_check-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-check
-Version: 2.1.5
+Version: 2.2.0
 Summary: A pytest plugin that allows multiple failures per test.
 Author: Brian Okken
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Pytest
 Requires-Dist: pytest
```

