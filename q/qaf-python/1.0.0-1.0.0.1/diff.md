# Comparing `tmp/qaf-python-1.0.0.tar.gz` & `tmp/qaf-python-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaf-python-1.0.0.tar", last modified: Fri Apr 22 05:59:41 2022, max compression
+gzip compressed data, was "qaf-python-1.0.0.1.tar", last modified: Fri Jul 14 15:13:00 2023, max compression
```

## Comparing `qaf-python-1.0.0.tar` & `qaf-python-1.0.0.1.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.351393 qaf-python-1.0.0/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1066 2022-04-22 05:47:36.000000 qaf-python-1.0.0/LICENSE
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1066 2022-04-22 05:54:03.000000 qaf-python-1.0.0/LICENSE.txt
--rw-r--r--   0 nishith.shah   (502) staff       (20)     5291 2022-04-22 05:59:41.352125 qaf-python-1.0.0/PKG-INFO
--rw-r--r--   0 nishith.shah   (502) staff       (20)     4386 2022-04-22 05:47:36.000000 qaf-python-1.0.0/README.md
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.235502 qaf-python-1.0.0/qaf/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1962 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/__init__.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.236812 qaf-python-1.0.0/qaf/automation/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/__init__.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.238967 qaf-python-1.0.0/qaf/automation/config/
--rw-r--r--   0 nishith.shah   (502) staff       (20)      401 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/config/logging_config.ini
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.252610 qaf-python-1.0.0/qaf/automation/core/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/core/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     6594 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/core/base_environment.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     4894 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/core/configurations_manager.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1563 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/core/load_class.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1442 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/core/message_type.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     2054 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/core/project_environment.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     4018 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/core/qaf_exceptions.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     3995 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/core/reporter.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     5414 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/core/resources_manager.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1695 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/core/singleton.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.254205 qaf-python-1.0.0/qaf/automation/formatter/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/__init__.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.260446 qaf-python-1.0.0/qaf/automation/formatter/py_test_report/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/py_test_report/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1938 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/py_test_report/behave_step_decorators.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.264651 qaf-python-1.0.0/qaf/automation/formatter/py_test_report/meta_info/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/py_test_report/meta_info/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     4175 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/py_test_report/meta_info/pytest_component.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1898 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/py_test_report/pystep_decorators.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     5693 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/py_test_report/pytest_fixture.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1933 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/py_test_report/pytest_utils.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.270175 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     2333 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/behave_before_all.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     4972 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/execution_meta_info.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.272738 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/feature/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/feature/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     4580 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/feature/feature_overview.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.277397 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/scenario/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/scenario/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     3413 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/scenario/command_log.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     2955 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/scenario/scenario.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     5972 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/scenario/scenario_meta_info.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.284020 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/step/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/step/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     2733 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/step/checkpoint.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     3371 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/step/step.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1718 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/step/sub_check_points.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     2540 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/test_results_meta_info.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.287583 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/util/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/util/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     2169 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/formatter/qaf_report/util/utils.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.289653 qaf-python-1.0.0/qaf/automation/integration/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/integration/__init__.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.292904 qaf-python-1.0.0/qaf/automation/keys/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1158 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/keys/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     2492 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/keys/application_properties.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.298934 qaf-python-1.0.0/qaf/automation/step_def/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/step_def/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)    14815 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/step_def/common_steps.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     8454 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/step_def/ws_common_steps.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.301900 qaf-python-1.0.0/qaf/automation/ui/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1916 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/js_toolkit.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.304568 qaf-python-1.0.0/qaf/automation/ui/util/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1162 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/util/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)    10100 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/util/qaf_wd_expected_conditions.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.317399 qaf-python-1.0.0/qaf/automation/ui/webdriver/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/webdriver/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1913 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/webdriver/abstract_listener.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1370 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/webdriver/base_test_page.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     3583 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/webdriver/command_tracker.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     2997 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/webdriver/desired_capabilities.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     2236 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/webdriver/qaf_find_by.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     5621 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/webdriver/qaf_test_base.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     7072 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/webdriver/qaf_web_driver.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)    31561 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/webdriver/qaf_web_element.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     3112 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ui/webdriver/qaf_webdriver_listener.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.330982 qaf-python-1.0.0/qaf/automation/util/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/util/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1320 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/util/datetime_util.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1330 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/util/directory_util.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1598 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/util/json_parser.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)    21215 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/util/string_util.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     2660 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/util/validator.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.334604 qaf-python-1.0.0/qaf/automation/ws/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ws/__init__.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.338907 qaf-python-1.0.0/qaf/automation/ws/rest/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     1122 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ws/rest/__init__.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     2674 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ws/rest/ws_listener.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     4560 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ws/rest/ws_request.py
--rw-r--r--   0 nishith.shah   (502) staff       (20)     6166 2022-04-22 05:47:36.000000 qaf-python-1.0.0/qaf/automation/ws/ws_request_bean.py
-drwxr-xr-x   0 nishith.shah   (502) staff       (20)        0 2022-04-22 05:59:41.349166 qaf-python-1.0.0/qaf_python.egg-info/
--rw-r--r--   0 nishith.shah   (502) staff       (20)     5291 2022-04-22 05:59:40.000000 qaf-python-1.0.0/qaf_python.egg-info/PKG-INFO
--rw-r--r--   0 nishith.shah   (502) staff       (20)     3321 2022-04-22 05:59:41.000000 qaf-python-1.0.0/qaf_python.egg-info/SOURCES.txt
--rw-r--r--   0 nishith.shah   (502) staff       (20)        1 2022-04-22 05:59:40.000000 qaf-python-1.0.0/qaf_python.egg-info/dependency_links.txt
--rw-r--r--   0 nishith.shah   (502) staff       (20)        1 2022-04-22 05:49:33.000000 qaf-python-1.0.0/qaf_python.egg-info/not-zip-safe
--rw-r--r--   0 nishith.shah   (502) staff       (20)      134 2022-04-22 05:59:41.000000 qaf-python-1.0.0/qaf_python.egg-info/requires.txt
--rw-r--r--   0 nishith.shah   (502) staff       (20)        4 2022-04-22 05:59:41.000000 qaf-python-1.0.0/qaf_python.egg-info/top_level.txt
--rw-r--r--   0 nishith.shah   (502) staff       (20)       79 2022-04-22 05:59:41.353770 qaf-python-1.0.0/setup.cfg
--rw-r--r--   0 nishith.shah   (502) staff       (20)     3028 2022-04-22 05:59:38.000000 qaf-python-1.0.0/setup.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.828309 qaf-python-1.0.0.1/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1066 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/LICENSE
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1066 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/LICENSE.txt
+-rw-r--r--   0 nishithshah   (502) staff       (20)    14144 2023-07-14 15:13:00.830000 qaf-python-1.0.0.1/PKG-INFO
+-rw-r--r--   0 nishithshah   (502) staff       (20)    13240 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/README.md
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.559459 qaf-python-1.0.0.1/qaf/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1381 2023-07-14 12:41:56.000000 qaf-python-1.0.0.1/qaf/__init__.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.562821 qaf-python-1.0.0.1/qaf/automation/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1123 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/__init__.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.575824 qaf-python-1.0.0.1/qaf/automation/bdd2/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1318 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/bdd2/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)      471 2023-07-13 13:37:57.000000 qaf-python-1.0.0.1/qaf/automation/bdd2/bdd_keywords.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2915 2023-07-13 20:33:55.000000 qaf-python-1.0.0.1/qaf/automation/bdd2/bddstep_executor.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     4477 2023-07-13 19:33:56.000000 qaf-python-1.0.0.1/qaf/automation/bdd2/factory.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     4055 2023-07-14 12:44:20.000000 qaf-python-1.0.0.1/qaf/automation/bdd2/model.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     8977 2023-07-14 12:44:20.000000 qaf-python-1.0.0.1/qaf/automation/bdd2/parser.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     8189 2023-07-14 12:48:49.000000 qaf-python-1.0.0.1/qaf/automation/bdd2/qaf_teststep.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     4941 2023-07-13 20:19:20.000000 qaf-python-1.0.0.1/qaf/automation/bdd2/step_registry.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.579196 qaf-python-1.0.0.1/qaf/automation/config/
+-rw-r--r--   0 nishithshah   (502) staff       (20)      401 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/config/logging_config.ini
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.595643 qaf-python-1.0.0.1/qaf/automation/core/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1286 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/core/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     3136 2023-06-06 15:28:25.000000 qaf-python-1.0.0.1/qaf/automation/core/checkpoint_bean.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     3095 2023-07-14 12:44:20.000000 qaf-python-1.0.0.1/qaf/automation/core/command_log_bean.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     5746 2023-07-13 19:38:29.000000 qaf-python-1.0.0.1/qaf/automation/core/configurations_manager.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1563 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/core/load_class.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1442 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/core/message_type.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     5037 2023-07-13 14:27:01.000000 qaf-python-1.0.0.1/qaf/automation/core/qaf_exceptions.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     3961 2023-06-06 15:28:25.000000 qaf-python-1.0.0.1/qaf/automation/core/reporter.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1695 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/core/singleton.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     9333 2023-07-13 14:28:33.000000 qaf-python-1.0.0.1/qaf/automation/core/test_base.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.604260 qaf-python-1.0.0.1/qaf/automation/integration/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1121 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/integration/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2995 2023-07-13 14:33:15.000000 qaf-python-1.0.0.1/qaf/automation/integration/result_updator.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1695 2023-07-13 14:33:15.000000 qaf-python-1.0.0.1/qaf/automation/integration/testcase_result_updator.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1644 2023-07-13 14:33:15.000000 qaf-python-1.0.0.1/qaf/automation/integration/testcase_run_result.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.609032 qaf-python-1.0.0.1/qaf/automation/keys/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1121 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/keys/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2702 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/keys/application_properties.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.615329 qaf-python-1.0.0.1/qaf/automation/report/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1122 2023-06-06 15:28:25.000000 qaf-python-1.0.0.1/qaf/automation/report/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)    11333 2023-07-13 14:36:13.000000 qaf-python-1.0.0.1/qaf/automation/report/json_reporter.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2259 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/report/status_counter.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2169 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/report/utils.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.620784 qaf-python-1.0.0.1/qaf/automation/step_def/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1122 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/step_def/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)    12968 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/step_def/common_steps.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     7998 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/step_def/ws_common_steps.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.625836 qaf-python-1.0.0.1/qaf/automation/ui/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1122 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/ui/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1916 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/ui/js_toolkit.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.641638 qaf-python-1.0.0.1/qaf/automation/ui/util/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1162 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/ui/util/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     4977 2023-06-06 15:28:25.000000 qaf-python-1.0.0.1/qaf/automation/ui/util/dynamic_wait.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     3720 2023-07-13 14:39:29.000000 qaf-python-1.0.0.1/qaf/automation/ui/util/locator_util.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     6340 2023-06-06 15:28:25.000000 qaf-python-1.0.0.1/qaf/automation/ui/util/qaf_element_expected_conditions.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1952 2023-06-06 15:28:25.000000 qaf-python-1.0.0.1/qaf/automation/ui/util/qaf_wd_expected_conditions.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.662645 qaf-python-1.0.0.1/qaf/automation/ui/webdriver/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1122 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/ui/webdriver/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1913 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/ui/webdriver/abstract_listener.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1344 2023-06-06 15:28:25.000000 qaf-python-1.0.0.1/qaf/automation/ui/webdriver/base_test_page.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     3577 2023-07-13 19:42:19.000000 qaf-python-1.0.0.1/qaf/automation/ui/webdriver/command_tracker.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     7087 2023-07-13 14:51:35.000000 qaf-python-1.0.0.1/qaf/automation/ui/webdriver/driver_factory.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)      781 2023-07-13 20:12:37.000000 qaf-python-1.0.0.1/qaf/automation/ui/webdriver/options.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     9413 2023-07-13 14:58:05.000000 qaf-python-1.0.0.1/qaf/automation/ui/webdriver/qaf_web_driver.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)    33850 2023-07-14 12:42:22.000000 qaf-python-1.0.0.1/qaf/automation/ui/webdriver/qaf_web_element.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     3919 2023-07-14 12:42:22.000000 qaf-python-1.0.0.1/qaf/automation/ui/webdriver/qaf_webdriver_listener.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.723075 qaf-python-1.0.0.1/qaf/automation/util/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1122 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/util/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2100 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/util/csv_util.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2855 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/automation/util/dataprovider_util.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1320 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/util/datetime_util.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1330 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/util/directory_util.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1598 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/util/json_parser.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     9430 2023-07-13 19:38:29.000000 qaf-python-1.0.0.1/qaf/automation/util/property_util.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)    21476 2023-06-06 15:28:25.000000 qaf-python-1.0.0.1/qaf/automation/util/string_util.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2660 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/util/validator.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.727274 qaf-python-1.0.0.1/qaf/automation/ws/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1122 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/ws/__init__.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.733214 qaf-python-1.0.0.1/qaf/automation/ws/rest/
+-rw-r--r--   0 nishithshah   (502) staff       (20)     1122 2022-06-28 15:46:28.000000 qaf-python-1.0.0.1/qaf/automation/ws/rest/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     3202 2023-06-06 15:28:25.000000 qaf-python-1.0.0.1/qaf/automation/ws/rest/ws_listener.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     5627 2023-06-06 15:28:25.000000 qaf-python-1.0.0.1/qaf/automation/ws/rest/ws_request.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     7935 2023-06-06 15:28:25.000000 qaf-python-1.0.0.1/qaf/automation/ws/ws_request_bean.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.738601 qaf-python-1.0.0.1/qaf/behave/
+-rw-r--r--   0 nishithshah   (502) staff       (20)      843 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/behave/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     5362 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/behave/base_environment.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     5124 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/behave/qaf_behave_plugin.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2125 2023-07-14 12:42:17.000000 qaf-python-1.0.0.1/qaf/listeners.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.756675 qaf-python-1.0.0.1/qaf/pytest/
+-rw-r--r--   0 nishithshah   (502) staff       (20)      139 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/pytest/__init__.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     4606 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/pytest/hooks.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2615 2023-07-13 13:37:02.000000 qaf-python-1.0.0.1/qaf/pytest/pytest_utils.py
+-rw-r--r--   0 nishithshah   (502) staff       (20)     4752 2023-07-14 12:42:22.000000 qaf-python-1.0.0.1/qaf/pytest/qaf_pytest_plugin.py
+drwxr-xr-x   0 nishithshah   (502) staff       (20)        0 2023-07-14 15:13:00.822638 qaf-python-1.0.0.1/qaf_python.egg-info/
+-rw-r--r--   0 nishithshah   (502) staff       (20)    14144 2023-07-14 15:13:00.000000 qaf-python-1.0.0.1/qaf_python.egg-info/PKG-INFO
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2936 2023-07-14 15:13:00.000000 qaf-python-1.0.0.1/qaf_python.egg-info/SOURCES.txt
+-rw-r--r--   0 nishithshah   (502) staff       (20)        1 2023-07-14 15:13:00.000000 qaf-python-1.0.0.1/qaf_python.egg-info/dependency_links.txt
+-rw-r--r--   0 nishithshah   (502) staff       (20)       46 2023-07-14 15:13:00.000000 qaf-python-1.0.0.1/qaf_python.egg-info/entry_points.txt
+-rw-r--r--   0 nishithshah   (502) staff       (20)        1 2023-07-14 15:13:00.000000 qaf-python-1.0.0.1/qaf_python.egg-info/not-zip-safe
+-rw-r--r--   0 nishithshah   (502) staff       (20)      168 2023-07-14 15:13:00.000000 qaf-python-1.0.0.1/qaf_python.egg-info/requires.txt
+-rw-r--r--   0 nishithshah   (502) staff       (20)        4 2023-07-14 15:13:00.000000 qaf-python-1.0.0.1/qaf_python.egg-info/top_level.txt
+-rw-r--r--   0 nishithshah   (502) staff       (20)       79 2023-07-14 15:13:00.836968 qaf-python-1.0.0.1/setup.cfg
+-rw-r--r--   0 nishithshah   (502) staff       (20)     2831 2023-07-14 15:11:34.000000 qaf-python-1.0.0.1/setup.py
```

### Comparing `qaf-python-1.0.0/LICENSE` & `qaf-python-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/LICENSE.txt` & `qaf-python-1.0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/bdd2/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-__version__ = "1.2.1"
-
 #  Copyright (c) 2022 Infostretch Corporation
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -15,29 +13,12 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
-
-from qaf.automation.core.qaf_exceptions import KeyNotFoundError
-
-from qaf.automation.core.configurations_manager import ConfigurationsManager as CM
-from qaf.automation.keys.application_properties import ApplicationProperties as AP
-from qaf.automation.core.resources_manager import ResourcesManager
-
-
-ResourcesManager().set_up()
-
-if not CM().contains_key(key=AP.TESTING_APPROACH):
-    raise KeyNotFoundError(message=AP.TESTING_APPROACH + ' e.g. behave, pytest')
-
-if CM().get_str_for_key(key=AP.TESTING_APPROACH).lower() == 'behave':
-    from behave.runner_util import load_step_modules
-    import os
-
-    import qaf.automation.step_def as step_def_path
-    step_def_path = str(os.path.abspath(step_def_path.__file__)).replace('/__init__.py', '')
-
-    SUBSTEP_DIRS = [step_def_path]
-    load_step_modules(SUBSTEP_DIRS)
+from qaf.automation.bdd2.step_registry import *  # pylint: disable=wildcard-import
+__all__ = [
+    "given", "when", "then", "step", "and", "but",
+    "Given", "When", "Then", "Step", "And", "But"
+]
```

### Comparing `qaf-python-1.0.0/qaf/automation/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/report/__init__.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/core/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/step_def/__init__.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/core/base_environment.py` & `qaf-python-1.0.0.1/qaf/behave/base_environment.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,132 +14,109 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
-from behave.contrib.scenario_autoretry import patch_scenario_with_autoretry as autoretry
-from behave.model_core import Status
 import os
-import six
 import re
-from qaf.automation.core.message_type import MessageType
-from qaf.automation.ui.webdriver.qaf_test_base import QAFTestBase
 
-from qaf.automation.core.project_environment import ProjectEnvironment
-from qaf.automation.formatter.qaf_report.behave_before_all import before_all
-from qaf.automation.formatter.qaf_report.scenario.scenario_meta_info import ScenarioMetaInfo, MetaData
-from qaf.automation.formatter.qaf_report.scenario.scenario import Scenario
-from qaf.automation.formatter.qaf_report.feature.feature_overview import FeatureOverView
-from qaf.automation.formatter.qaf_report.execution_meta_info import ExecutionMetaInfo
-from qaf.automation.formatter.qaf_report.scenario.command_log import CommandLogStack
-from qaf.automation.formatter.qaf_report.step.step import Step
-from qaf.automation.util.datetime_util import date_time, current_timestamp
-from qaf.automation.util.directory_util import create_directory
+import six
+from behave.contrib.scenario_autoretry import patch_scenario_with_autoretry as autoretry
+from behave.model_core import Status
 
-OUTPUT_TEST_RESULTS_DIR = 'test-results'
+from qaf.automation.core.test_base import tear_down, start_step, end_step, get_command_logs, get_checkpoint_results, \
+    is_verification_failed, clear_assertions_log, get_bundle
+from qaf.automation.integration.result_updator import update_result
+from qaf.automation.integration.testcase_run_result import TestCaseRunResult
+from qaf.automation.keys.application_properties import ApplicationProperties
+from qaf.automation.report.utils import step_status
+from qaf.automation.util.datetime_util import current_timestamp
 
 
 class BaseEnvironment:
-    def __init__(self):
-        self.current_feature = None
-        self.current_scenario = None
-        self.current_step = None
-        self.obj_scenario_meta_info = None
 
     def before_all(self, context):
-        ProjectEnvironment.set_up()
-
-        root_directory = os.path.join(OUTPUT_TEST_RESULTS_DIR, date_time())
-        create_directory(root_directory)
-        os.environ['REPORT_DIR'] = root_directory
+        get_bundle().set_property(ApplicationProperties.TESTING_APPROACH, "behave")
 
-        before_all()
+        from behave.runner_util import load_step_modules
+        import qaf.automation.step_def as step_def_path
+        step_def_path = str(os.path.abspath(step_def_path.__file__)).replace('/__init__.py', '')
+
+        QAF_STEPS = [step_def_path]
+        load_step_modules(QAF_STEPS)
+        step_provider_pkgs = get_bundle().get_string(ApplicationProperties.STEP_PROVIDER_PKG)
+        if step_provider_pkgs:
+            step_provider_pkg_list = step_provider_pkgs.replace('.', '/').split(";")
+            load_step_modules(step_provider_pkg_list)
 
     def after_all(self, context):
-        ExecutionMetaInfo().endTime = current_timestamp()
-        QAFTestBase().stop_driver()
+        tear_down()
 
     def before_feature(self, context, feature):
-
         for scenario in feature.scenarios:
             if "autoretry" in scenario.effective_tags:
                 autoretry(scenario, max_attempts=2)
 
-        current_feature_directory = os.path.join(os.getenv('REPORT_DIR'), 'json', re.sub('[^A-Za-z0-9]+', ' - ',
-                                                                                         re.sub('.feature', '',
-                                                                                                feature.filename)))
-        create_directory(current_feature_directory)
-        os.environ['CURRENT_FEATURE_DIR'] = current_feature_directory
-
-        ExecutionMetaInfo().add_test(re.sub('[^A-Za-z0-9]+', ' - ', re.sub('.feature', '', feature.filename)))
-
-        FeatureOverView().startTime = current_timestamp()
-        FeatureOverView().add_class(feature.name)
-
     def after_feature(self, context, feature):
-        FeatureOverView().endTime = current_timestamp()
+        pass
 
     def before_scenario(self, context, scenario):
         self.current_scenario = scenario
-        current_scenario_directory = os.path.join(os.getenv('CURRENT_FEATURE_DIR'), scenario.feature.name)
-        create_directory(current_scenario_directory)
-        os.environ['CURRENT_SCENARIO_DIR'] = current_scenario_directory
-
-        self.obj_scenario_meta_info = ScenarioMetaInfo()
-        self.obj_scenario_meta_info.startTime = current_timestamp()
+        self.startTime = current_timestamp()
+        clear_assertions_log()
+        get_bundle().set_property(ApplicationProperties.CURRENT_TEST_NAME, scenario.name)
 
     def after_scenario(self, context, scenario):
+
         status_name = scenario.status.name
 
-        if scenario.status == Status.failed:
+        testcase_run_result = TestCaseRunResult()
+        testcase_run_result.className = scenario.feature.name
+        testcase_run_result.commandLogs = get_command_logs().copy()
+        testcase_run_result.starttime = self.startTime
+        testcase_run_result.endtime = current_timestamp()  # self.startTime + (scenario.duration * 1000)
+        testcase_run_result.metaData = {
+            "name": scenario.name,
+            "resultFileName": scenario.name,
+            "referece": six.text_type(scenario.location),
+            "groups": scenario.effective_tags
+        }
+        testcase_run_result.executionInfo = {
+            "testName": "Behave Test",
+            "suiteName": "Behave Suite",
+            "driverCapabilities": {
+                "browser-desired-capabilities":get_bundle().get("driver.desiredCapabilities", {}),
+                "browser-actual-capabilities": get_bundle().get("driverCapabilities",{})
+            }
+        }
+        if scenario.description:
+            testcase_run_result.metaData["description"] = scenario.description
+
+        if scenario.status != Status.passed:
             steps = scenario.steps
             for step in steps:
                 if step.status == Status.failed:
                     error_message = step.error_message
                     error_message = error_message.splitlines()
-
-                    Scenario(file_name=scenario.name).errorTrace = error_message
+                    testcase_run_result.throwable = error_message
                 elif step.status == Status.skipped or step.status == Status.untested:
-                    obj_step = Step()
-                    obj_step.start_behave_step(step)
-                    obj_step.stop_behave_step(step)
-                    Scenario(file_name=self.current_scenario.name).add_checkPoints(obj_step.obj_check_point)
-                    del obj_step
+                    start_step(step.name, step.keyword + ' ' + step.name)
+                    end_step(None)
         else:
-            checkPoints = Scenario(file_name=self.current_scenario.name).checkPoints
-            for checkPoint in checkPoints:
-                if checkPoint['type'] == MessageType.TestStepFail:
-                    status_name = 'failed'
-                    break
-
-        ExecutionMetaInfo().update_status(status_name)
-        FeatureOverView().update_status(status_name)
-
-        self.obj_scenario_meta_info.duration = scenario.duration * 1000
-        self.obj_scenario_meta_info.result = status_name
-
-        obj_meta_data = MetaData()
-        obj_meta_data.name = scenario.name
-        obj_meta_data.resultFileName = scenario.name
-        if scenario.description:
-            obj_meta_data.description = scenario.description
-        obj_meta_data.referece = six.text_type(scenario.location)
-        obj_meta_data.groups = scenario.effective_tags
-
-        self.obj_scenario_meta_info.metaData = obj_meta_data.to_json_dict()
-        self.obj_scenario_meta_info.close()
-
-        del self.obj_scenario_meta_info
-        self.obj_scenario_meta_info = None
-        Scenario(file_name=scenario.name).seleniumLog = CommandLogStack().get_all_command_log()
+            if is_verification_failed():
+                status_name = 'failed'
+
+        testcase_run_result.checkPoints = get_checkpoint_results().copy()
+        testcase_run_result.status = status_name
+
+        update_result(testcase_run_result)
+        tear_down()
 
     def before_step(self, context, step):
-        self.current_step = step
+        start_step(step.name, step.keyword + ' ' + step.name)
 
     def after_step(self, context, step):
-        obj_step = Step()
-        obj_step.start_behave_step(step)
-        obj_step.stop_behave_step(step)
-        Scenario(file_name=self.current_scenario.name).add_checkPoints(obj_step.obj_check_point)
-        del obj_step
+        status = step_status(step)
+        b_status = bool(re.search('(?i)pass', status)) if bool(re.search('(?i)fail|pass', status)) else None
+        end_step(b_status)
```

### Comparing `qaf-python-1.0.0/qaf/automation/core/configurations_manager.py` & `qaf-python-1.0.0.1/qaf/automation/core/configurations_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,107 +15,118 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 import json
-
-from qaf.automation.core.singleton import Singleton
-from qaf.automation.util.string_util import to_boolean
+import os
 from typing import (
     Optional,
 )
 
+from qaf.automation.core.singleton import Singleton
+from qaf.automation.keys.application_properties import ApplicationProperties as AP
+from qaf.automation.util.property_util import PropertyUtil
+
+__all__ = [
+    "expression", "get_bundle", "ConfigurationsManager"
+]
+
 
 class ConfigurationsManager(metaclass=Singleton):
     """
     This class will store the values of all property files.
     """
 
     def __init__(self):
-        self.__dict = {}
+        self.__dict = PropertyUtil()
+        application_properties_path = os.path.join('resources', 'application.properties')
+        if os.path.exists(application_properties_path):
+            self.__dict.load(application_properties_path)
+        self.__dict.load(self.__dict.get_string(AP.RESOURCES))
 
     def contains_key(self, key: str) -> bool:
         """
         Check that configurations manager contains key.
 
         Args:
             key (str): Key name to verify key is exist or not.
 
         Returns:
             bool: Returns True If dict contains key else returns False
 
         """
-        return True if key in self.__dict else False
+        return self.__dict.__contains__(key)
 
     def set_object_for_key(self, key: str, value=object) -> None:
         """
         Set object for key into the dict
 
         Args:
             key (str): Key name to store value
             value (str): Value which needs to be store
 
         Returns:
             None
         """
-        self.__dict[key] = value
+        self.__dict.set_property(key, value)
 
     def get_object_for_key(self, key: str, default_value: Optional[object] = None) -> object:
         """
         Returns object for key.
 
         Args:
             key (str): Key name to store value
             default_value (Optional(object)): This will default value for key
 
         Returns:
             Optional(object): Stored value for key
         """
-        return self.__dict[key] if self.contains_key(key) else default_value
+        return self.__dict.get(key, default_value)
 
     def get_str_for_key(self, key: str, default_value=None) -> str:
         """
         Returns object for key.
 
         Args:
             key (str): Key name to store value
             default_value (Optional(str)): This will default value for key
 
         Returns:
             Optional(str): Stored value for key
         """
-        return str(self.__dict[key]) if self.contains_key(key) else default_value
+        # return str(self.__dict[key]) if self.contains_key(key) else default_value
+        return self.__dict.get_string(key, default_value)
 
     def get_int_for_key(self, key: str, default_value=None) -> int:
         """
         Returns object for key.
 
         Args:
             key (str): Key name to store value
             default_value (Optional(int)): This will default value for key
 
         Returns:
             Optional(int): Stored value for key
         """
-        return int(self.__dict[key]) if self.contains_key(key) else default_value
+        return self.__dict.get_int(key, default_value)
 
     def get_bool_for_key(self, key: str, default_value=False) -> bool:
         """
         Returns object for key.
 
         Args:
             key (str): Key name to store value
             default_value (Optional(bool)): This will default value for key
 
         Returns:
             Optional(bool): Stored value for key
         """
-        return to_boolean(self.__dict[key]) if self.contains_key(key) else default_value
+        return self.__dict.get_boolean(key, default_value)
 
     def get_list_for_key(self, key: str, default_value=None) -> list:
         """
         Returns object for key.
 
         Args:
             key (str): Key name to store value
@@ -140,9 +151,23 @@
 
         Returns:
             Optional(dict): Stored value for key
         """
         if default_value is None:
             default_value = {}
         if self.contains_key(key) and isinstance(self.__dict[key], str):
-            return json.loads(self.__dict[key])
+            return json.loads(self.__dict.get_string(key))
         return default_value
+
+    @staticmethod
+    def get_bundle():
+        return ConfigurationsManager().__dict
+
+    @staticmethod
+    def expression(func):
+        """ mark for function allowed in expression while resolving properties"""
+        ConfigurationsManager.get_bundle().evaluator.functions[func.__name__] = func
+        return func
+
+
+get_bundle = ConfigurationsManager.get_bundle
+expression = ConfigurationsManager.expression
```

### Comparing `qaf-python-1.0.0/qaf/automation/core/load_class.py` & `qaf-python-1.0.0.1/qaf/automation/core/load_class.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/core/message_type.py` & `qaf-python-1.0.0.1/qaf/automation/core/message_type.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/core/project_environment.py` & `qaf-python-1.0.0.1/qaf/automation/util/json_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,36 +14,23 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
-import os
+class JsonParser(dict):
+    __getattr__ = dict.__getitem__
 
-from qaf.automation.core.configurations_manager import ConfigurationsManager as CM
-from qaf.automation.core.resources_manager import ResourcesManager
-from qaf.automation.keys.application_properties import ApplicationProperties as AP
-
-
-class ProjectEnvironment:
-    """
-    This class will set up application properties, locators, etc.
-    """
-
-    @staticmethod
-    def set_up() -> None:
-        """
-        This method will initialise the application properties and locators storage file.
-
-        Returns:
-            None
-        """
-        ResourcesManager().set_up()
-        ProjectEnvironment.set_executable_path()
-
-    @staticmethod
-    def set_executable_path():
-        executable_path = CM().get_str_for_key(AP.EXECUTABLE_PATH)
-        all_executable_path = executable_path.split(";")
-        for each_executable_path in all_executable_path:
-            os.environ["PATH"] += os.pathsep + each_executable_path
+    def __init__(self, *args, **kwargs):
+        super(JsonParser, self).__init__(*args, **kwargs)
+        self.update(**dict((k, self.parse(v))
+                           for k, v in dict.items(self)))
+
+    @classmethod
+    def parse(cls, v):
+        if isinstance(v, dict):
+            return cls(v)
+        elif isinstance(v, list):
+            return [cls.parse(i) for i in v]
+        else:
+            return v
```

### Comparing `qaf-python-1.0.0/qaf/automation/core/reporter.py` & `qaf-python-1.0.0.1/qaf/automation/core/reporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,114 +14,114 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
-import uuid
-from qaf.automation.formatter.qaf_report.step.checkpoint import CheckPoint
-import os
-from qaf.automation.formatter.qaf_report.step.sub_check_points import SubCheckPoints
-from qaf.automation.ui.webdriver import qaf_test_base
-from qaf.automation.core.message_type import MessageType
 from typing import (
     Optional,
 )
 
+from qaf.automation.core.checkpoint_bean import CheckPointBean
+from qaf.automation.core.message_type import MessageType
+from qaf.automation.core.test_base import add_checkpoint, take_screenshot
+
 
 class Reporter:
     """
     This class will handle log event
     """
 
-    def add_check_point(self, message: str, message_type: MessageType, screen_shot: Optional[str] = '') -> None:
-        check_point = CheckPoint()
-        check_point.message = message
+    @staticmethod
+    def add_check_point(message: str, message_type: MessageType, screen_shot: Optional[str] = '') -> None:
+        check_point = CheckPointBean()
+        check_point.message = str(message)
         check_point.type = message_type
         check_point.screenshot = screen_shot
-        SubCheckPoints().add_check_point(check_point)
+        #SubCheckPoints().add_check_point(check_point)
+        add_checkpoint(check_point)
 
     @staticmethod
     def log(message: str, message_type: Optional[MessageType] = MessageType.Info) -> None:
         """
         Log message into log file.
 
         Args:
             message (str): Message needs to be log
             message_type (int): Message type
 
         Returns:
             None
         """
-        Reporter().add_check_point(message, message_type)
+        Reporter.add_check_point(message, message_type)
 
     @staticmethod
     def info(message: str) -> None:
         """
         Log message into log file.
 
         Args:
             message (str): Message needs to be log
 
         Returns:
             None
         """
-        Reporter().add_check_point(message, MessageType.Info)
+        Reporter.add_check_point(message, MessageType.Info)
 
     @staticmethod
     def debug(message: str) -> None:
         """
         Log message into log file.
 
         Args:
             message (str): Message needs to be log
 
         Returns:
             None
         """
-        Reporter().add_check_point(message, MessageType.Info)
+        Reporter.add_check_point(message, MessageType.Info)
 
     @staticmethod
     def error(message: str) -> None:
         """
         Log message into log file.
 
         Args:
             message (str): Message needs to be log
 
         Returns:
             None
         """
-        Reporter().add_check_point(message, MessageType.Fail)
+        Reporter.add_check_point(message, MessageType.Fail)
 
     @staticmethod
     def critical(message: str) -> None:
         """
         Log message into log file.
 
         Args:
             message (str): Message needs to be log
 
         Returns:
             None
         """
-        Reporter().add_check_point(message, MessageType.Warn)
+        Reporter.add_check_point(message, MessageType.Warn)
 
     @staticmethod
     def warn(message: str) -> None:
         """
         Log message into log file.
 
         Args:
             message (str): Message needs to be log
 
         Returns:
             None
         """
-        Reporter().add_check_point(message, MessageType.Warn)
+        Reporter.add_check_point(message, MessageType.Warn)
 
     @staticmethod
     def log_with_screenshot(message: str, message_type: Optional[MessageType] = MessageType.Info) -> None:
-        filename = os.path.join(os.getenv('REPORT_DIR'), 'img', str(uuid.uuid4()) + '.png')
-        qaf_test_base.QAFTestBase().get_driver().save_screenshot(filename=filename)
-        Reporter().add_check_point(message, message_type, screen_shot=filename)
+        filename = take_screenshot() #os.path.join(os.getenv('REPORT_DIR'), 'img', str(uuid.uuid4()) + '.png')
+        #qaf_test_base.QAFTestBase().get_driver().save_screenshot(filename=filename)
+        Reporter.add_check_point(message, message_type, screen_shot=filename)
```

### Comparing `qaf-python-1.0.0/qaf/automation/core/singleton.py` & `qaf-python-1.0.0.1/qaf/automation/core/singleton.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/py_test_report/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/ui/webdriver/__init__.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/py_test_report/behave_step_decorators.py` & `qaf-python-1.0.0.1/qaf/automation/integration/testcase_run_result.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,31 +13,29 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
+class TestCaseRunResult:
+    """
+    @author: Chirag Jayswal
+    """
+
+    def __init__(self):
+        self.checkPoints = []
+        self.commandLogs = []
+        self.status = ""
+        self.metaData = {}
+        self.testData = []
+        self.steps = []
+        self.starttime = 0
+        self.endtime = 0
+        self.isTest = True
+        self.executionInfo = {}
+        self.className = ""
+        self.willRetry = False
+        self.throwable = None
 
-from qaf.automation.formatter.py_test_report.meta_info import pytest_component
-from qaf.automation.formatter.py_test_report.pytest_utils import PyTestStatus
-
-
-class step(object):
-
-    def __init__(self, name=None, keyword="CommonStep:"):
-        self.keyword = keyword
-        self.name = name
-
-    def before_step(self, step=None):
-        pytest_component.PyTestStep._before_step(name=self.name, keyword=self.keyword, step=step)
-
-    def after_step(self, status, exception=None):
-        pytest_component.PyTestStep._after_step(status=status, exception=exception)
-
-    def __call__(self, step):
-        def wrapped_step(context, *args, **kwargs):
-            self.before_step(step)
-            step(context, *args, **kwargs)
-            self.after_step(status=PyTestStatus.passed.name)
-
-        return wrapped_step
+    def get_name(self):
+        return self.metaData.get("name")
```

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/py_test_report/meta_info/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/util/__init__.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/py_test_report/pystep_decorators.py` & `qaf-python-1.0.0.1/qaf/automation/ui/util/qaf_wd_expected_conditions.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,30 +14,35 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
-from qaf.automation.formatter.py_test_report.meta_info import pytest_component
-from qaf.automation.formatter.py_test_report.pytest_utils import PyTestStatus
+from selenium.common.exceptions import NoSuchElementException
 
 
-class pystep(object):
-
-    def __init__(self, keyword="[Func]", name=None):
-        self.keyword = keyword
-        self.name = name
-
-    def before_step(self, step=None):
-        pytest_component.PyTestStep._before_step(name=self.name, keyword=self.keyword, step=step)
-
-    def after_step(self, status, exception=None):
-        pytest_component.PyTestStep._after_step(status=status, exception=exception)
-
-    def __call__(self, step):
-        def wrapped_step(*args):
-            self.before_step(step)
-            step(*args)
-            self.after_step(status=PyTestStatus.passed.name)
-
-        return wrapped_step
+class WaitForAjax(object):
+    def __init__(self, snippet: str) -> None:
+        self.snippet = snippet
+
+    def __call__(self, driver) -> bool:
+        try:
+            value = driver.execute_script(self.snippet)
+            return bool(value)
+        except:
+            return False
+
+
+class WaitForAnyPresent(object):
+    def __init__(self, locators: [str]) -> None:
+        self.locators = locators
+
+    def __call__(self, driver) -> bool:
+        try:
+            from qaf.automation.ui.webdriver.qaf_web_element import QAFWebElement
+            for locator in self.locators:
+                if QAFWebElement(locator=locator).is_present():
+                    return True
+            return False
+        except NoSuchElementException:
+            return False
```

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/py_test_report/pytest_utils.py` & `qaf-python-1.0.0.1/qaf/automation/util/datetime_util.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,38 +14,17 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
-from enum import Enum
-import six
-import inspect
+import time
+from time import strftime
 
 
-def del_all_attr(obj):
-    for name in inspect.getmembers(obj):
-        if not name[0].startswith('_') and not inspect.ismethod(name[1]):
-            delattr(obj, name[0])
+def current_timestamp():
+    return int(round(time.time() * 1000))
 
 
-class PyTestStatus(Enum):
-    untested = 0
-    skipped = 1
-    passed = 2
-    failed = 3
-    undefined = 4
-    executing = 5
-
-    def __eq__(self, other):
-        if isinstance(other, six.string_types):
-            return self.name == other
-        return super(PyTestStatus, self).__eq__(other)
-
-    @classmethod
-    def from_name(cls, name):
-        enum_value = cls.__members__.get(name, None)
-        if enum_value is None:
-            known_names = ", ".join(cls.__members__.keys())
-            raise LookupError("%s (expected: %s)" % (name, known_names))
-        return enum_value
+def date_time(format='%d-%m-%Y_%H_%M_%S'):
+    return strftime(format, time.localtime())
```

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/qaf_report/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/qaf_report/feature/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/ws/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/qaf_report/scenario/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/integration/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,7 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
-
```

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/qaf_report/scenario/command_log.py` & `qaf-python-1.0.0.1/qaf/automation/core/command_log_bean.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
+from dataclasses import dataclass
 
-from collections import deque
 
-from qaf.automation.core.singleton import Singleton
+@dataclass
+class CommandLogBean:
+    """
+    @author: Chirag Jayswal
+    """
 
-
-class CommandLog:
     def __init__(self) -> None:
         self.commandName = ''
-        self.args = {}
+        self.args = []
         self.result = ''
         self.__subLogs = []
         self.duration = 0
 
     @property
     def commandName(self) -> str:
         return self.__commandName
@@ -55,53 +57,43 @@
     def result(self, value: str) -> None:
         self.__result = value
 
     @property
     def subLogs(self) -> list:
         return self.__subLogs
 
-    def add_subLogs(self, sub_log: str) -> None:
+    @subLogs.setter
+    def subLogs(self, value: list):
+        self.__subLogs = value
+
+    def add_subLogs(self, sub_log: "CommandLogBean") -> None:
         self.__subLogs.append(sub_log)
 
     @property
     def duration(self) -> int:
         return self.__duration
 
     @duration.setter
     def duration(self, value: int) -> None:
         self.__duration = value
 
     def to_json_dict(self) -> dict:
-        args_array = []
-        for key, value in self.args.items():
-            args_array.append(str(key) + ':' + str(value))
+        # args_array = []
+        # if self.args:
+        #     for key, value in self.args.items():
+        #         args_array.append(str(key) + ':' + str(value))
 
         _dict = {
             "commandName": self.commandName,
-            "args": args_array,
+            "args": list(map(str, self.args)),
             "result": self.result,
             "subLogs": self.subLogs,
             "duration": self.duration,
         }
         return _dict
 
     def to_string(self) -> str:
-        string = 'Command: ' + self.commandName
-        for key, value in self.args.items():
-            string = string + ' ' + str(key) + ':' + str(value)
-        string = string + str(self.result)
+        string = f'Command: {self.commandName} {self.args} {self.result}'
+        # for key, value in self.args.items():
+        #     string = string + ' ' + str(key) + ':' + str(value)
+        # string = string + str(self.result)
         return string
-
-
-class CommandLogStack(metaclass=Singleton):
-    def __init__(self) -> None:
-        self.__command_log_stack = deque()
-
-    def add_command_log(self, selenium_log: CommandLog) -> None:
-        self.__command_log_stack.append(selenium_log.to_json_dict())
-
-    def get_all_command_log(self) -> list:
-        arr_selenium_log = []
-        while self.__command_log_stack:
-            selenium_log = self.__command_log_stack.popleft()
-            arr_selenium_log.append(selenium_log)
-        return arr_selenium_log
```

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/qaf_report/step/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/keys/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,7 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
-
```

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/qaf_report/step/checkpoint.py` & `qaf-python-1.0.0.1/qaf/automation/core/checkpoint_bean.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,16 +13,22 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
+from dataclasses import dataclass
 
-class CheckPoint:
+
+@dataclass
+class CheckPointBean:
+    """
+        @author: Chirag Jayswal
+    """
     def __init__(self) -> None:
         self.message = ''
         self.type = ''
         self.duration = 0
         self.threshold = 0
         self.screenshot = ''
         self.subCheckPoints = []
@@ -72,16 +78,27 @@
         return self.__subCheckPoints
 
     @subCheckPoints.setter
     def subCheckPoints(self, value: list):
         self.__subCheckPoints = value
 
     def to_json_dict(self) -> dict:
+
         _dict = {
             "message": self.message,
             "type": self.type,
             "duration": self.duration,
             "threshold": self.threshold,
             "screenshot": self.screenshot,
             "subCheckPoints": self.subCheckPoints,
         }
         return _dict
+
+    def is_success(self) -> bool:
+        if "pass" in self.type.lower():
+            return True
+        if "fail" in self.type.lower():
+            return False
+        for checkPoint in self.subCheckPoints:
+            if not checkPoint.is_success():
+                return False
+        return True
```

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/qaf_report/util/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,7 +14,8 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
+
```

### Comparing `qaf-python-1.0.0/qaf/automation/formatter/qaf_report/util/utils.py` & `qaf-python-1.0.0.1/qaf/automation/report/utils.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/integration/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/ui/util/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,7 +14,8 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
+from . import qaf_wd_expected_conditions
```

### Comparing `qaf-python-1.0.0/qaf/automation/keys/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/core/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,8 +14,13 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
-from . import application_properties
+from qaf.automation.core.configurations_manager import get_bundle, expression
+
+# pylint: disable=undefined-all-variable
+__all__ = [
+    "get_bundle", "expression"
+]
```

### Comparing `qaf-python-1.0.0/qaf/automation/keys/application_properties.py` & `qaf-python-1.0.0.1/qaf/automation/keys/application_properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,24 +33,30 @@
 
     # selenium
     SELENIUM_WAIT_TIMEOUT = "selenium.wait.timeout"
     REMOTE_SERVER = "remote.server"
     REMOTE_PORT = "remote.port"
 
     DRIVER_NAME = "driver.name"
+    DRIVER_CLASS = "driver.class"
 
     DRIVER_CAPABILITY_PREFIX = "driver.capabilities"
     DRIVER_ADDITIONAL_CAPABILITIES = "driver.additional.capabilities"
     DRIVER_ADDITIONAL_CAPABILITIES_FORMAT = "{0}.additional.capabilities"
     DRIVER_CAPABILITY_PREFIX_FORMAT = "{0}.capabilities"
+    DRIVER_RESOURCES_FORMAT = "{0}.resources"
 
     SELENIUM_BASE_URL = "env.baseurl"
     RESOURCES = "env.resources"
 
     # listeners
     WEBDRIVER_COMMAND_LISTENERS = "wd.command.listeners"
     WEBELEMENT_COMMAND_LISTENERS = "we.command.listeners"
     WEBSERVICE_COMMAND_LISTENERS = "ws.command.listeners"
+    RESULT_UPDATERS = "result.updator"
 
     ENV_DEFAULT_LANGUAGE = "env.default.locale"
     EXECUTABLE_PATH = 'executable.path'
     TESTING_APPROACH = 'testing.approach'
+    STEP_PROVIDER_PKG = 'step.provider.pkg'
+
+    SELENIUM_SINGLETON = 'selenium.singleton'
```

### Comparing `qaf-python-1.0.0/qaf/automation/step_def/__init__.py` & `qaf-python-1.0.0.1/qaf/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,7 +14,13 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
+from qaf.listeners import pluginmagager, QAFWebDriverListener, QAFElementListener, StepListener
+
+pluginmagager.add_hookspecs(QAFWebDriverListener)
+pluginmagager.add_hookspecs(QAFElementListener)
+pluginmagager.add_hookspecs(StepListener)
+__version__ = "1.0.0"
```

### Comparing `qaf-python-1.0.0/qaf/automation/step_def/ws_common_steps.py` & `qaf-python-1.0.0.1/qaf/automation/step_def/ws_common_steps.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,174 +14,173 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
-from behave import *
+from http.client import responses
+
+import jmespath
 from hamcrest import *
 
+from qaf.automation.bdd2.step_registry import step
 from qaf.automation.core.configurations_manager import ConfigurationsManager as CM
 from qaf.automation.util.validator import Validator
 from qaf.automation.ws.rest.ws_request import WsRequest
 from qaf.automation.ws.ws_request_bean import WsRequestBean
-from http.client import responses
-import jmespath
 
-use_step_matcher("re")
 
-
-@step(u"user requests '(?P<api_key>[\S\s]+)' with data '(?P<data>[\S\s]+)'")
+@step(u"user requests '{api_key}' with data '{data}'")
 def user_requests_with_data(context, api_key, data):
     ws_request_bean = WsRequestBean().fill_from_config(api_key)
-    ws_request_bean.resolve_parameters(data)
-    WsRequest().request(ws_request_bean)
+    WsRequest().request(ws_request_bean, data)
 
 
-@step(u"user requests '(?P<api_key>[\S\s]+)'")
+@step(u"user requests '{api_key}'")
 def user_requests(context, api_key):
-    WsRequest().request(WsRequestBean().fill_from_config(api_key))
+    ws_request_bean = WsRequestBean().fill_from_config(api_key)
+    WsRequest().request(ws_request_bean)
 
 
 ############################
 # Status Code Verification #
 ############################
 
-@step(u"response should have status code '(?P<status_code>[\S\s]+)'")
+@step(u"response should have status code '{status_code}'")
 def response_should_have_status_code(context, status_code):
     Validator.assert_that(WsRequest.response.status_code, equal_to(int(status_code)), reason="Response Status")
 
 
-@step(u"response should have status '(?P<status>[\S\s]+)'")
+@step(u"response should have status '{status}'")
 def response_should_have_status(context, status):
     Validator.assert_that(responses[WsRequest.response.status_code], equal_to(status), reason="Response Status")
 
 
 #######################
 # Header Verification #
 #######################
 
-@step(u"response should have header '(?P<header>[\S\s]+)' with value '(?P<value>[\S\s]+)'")
+@step(u"response should have header '{header}' with value '{value}'")
 def verify_should_have_header_with_value(context, header, value):
     Validator.assert_that(WsRequest.response.headers, has_entry(key_match=header, value_match=value),
                           reason="Response Header")
 
 
-@step(u"response should have header '(?P<header>[\S\s]+)'")
+@step(u"response should have header '{header}'")
 def verify_should_have_header(context, header):
     Validator.assert_that(WsRequest.response.headers, has_key(header), reason="Response Header")
 
 
-@step(u"store response header '(?P<header>[\S\s]+)' into '(?P<variable>[\S\s]+)'")
+@step(u"store response header '{header}' into '{variable}'")
 def store_response_body_to(context, header, variable):
     CM().set_object_for_key(variable, str(WsRequest.response.headers[header]))
 
 
 #####################
 # Body Verification #
 #####################
 
-@step(u"store response body '(?P<path>[\S\s]+)' into '(?P<variable>[\S\s]+)'")
+@step(u"store response body '{path}' into '{variable}'")
 def store_response_body_to(context, path, variable):
     value = value_at_json_path(WsRequest.response.json(), path)
     CM().set_object_for_key(variable, str(value))
 
 
-@step(u"response should have '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should have '{value}' at '{path}'")
 def response_should_have_value_at_jsonpath(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(str(actual_value), equal_to(value))
 
 
-@step(u"response should have '(?P<path>[\S\s]+)'")
+@step(u"response should have '{path}'")
 def response_should_have_jsonpath(context, path):
     Validator.assert_that(has_json_path(WsRequest.response.json(), path), equal_to(True),
                           reason="Response Body has " + path)
 
 
-@step(u"response should not have '(?P<path>[\S\s]+)'")
+@step(u"response should not have '{path}'")
 def response_should_have_jsonpath(context, path):
     Validator.assert_that(has_json_path(WsRequest.response.json(), path), equal_to(False),
                           reason="Response Body has " + path)
 
 
-@step(u"response should have value contains '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should have value contains '{value}' at '{path}'")
 def response_should_have_value_at_jsonpath(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(str(actual_value), contains_string(value))
 
 
-@step(u"response should have value ignoring case '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should have value ignoring case '{value}' at '{path}'")
 def response_should_have_value_at_jsonpath(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(str(actual_value), equal_to_ignoring_case(value))
 
 
-@step(u"response should have value ignoring whitespace '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should have value ignoring whitespace '{value}' at '{path}'")
 def response_should_have_value_at_jsonpath(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(str(actual_value), equal_to_ignoring_whitespace(value))
 
 
-@step(u"response should have value contains ignoring case '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should have value contains ignoring case '{value}' at '{path}'")
 def response_should_have_value_at_jsonpath(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(str(actual_value).upper(), contains_string(value.upper()))
 
 
-@step(u"response should have value end with '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should have value end with '{value}' at '{path}'")
 def response_should_have_value_at_jsonpath(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(str(actual_value), ends_with(value))
 
 
-@step(u"response should have value start with '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should have value start with '{value}' at '{path}'")
 def response_should_have_value_at_jsonpath(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(str(actual_value), starts_with(value))
 
 
-@step(u"response should have value matches with '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should have value matches with '{value}' at '{path}'")
 def response_should_have_value_at_jsonpath(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(str(actual_value), matches_regexp(value))
 
 
-@step(u"response should start with '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should start with '{value}' at '{path}'")
 def response_should_have_value_at_jsonpath(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(str(actual_value), starts_with(value))
 
 
-@step(u"response should be less than '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should be less than '{value}' at '{path}'")
 def response_should_less_than(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(int(actual_value), less_than(value))
 
 
-@step(u"response should be less than or equals to '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should be less than or equals to '{value}' at '{path}'")
 def response_should_less_than_or_equals_to(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(int(actual_value), less_than_or_equal_to(value))
 
 
-@step(u"response should be greater than '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should be greater than '{value}' at '{path}'")
 def response_should_greater_than(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(int(actual_value), greater_than(value))
 
 
-@step(u"response should be greater than or equals to '(?P<value>[\S\s]+)' at '(?P<path>[\S\s]+)'")
+@step(u"response should be greater than or equals to '{value}' at '{path}'")
 def response_should_greater_than_or_equals_to(context, value, path):
     actual_value = value_at_json_path(WsRequest.response.json(), path)
     Validator.assert_that(int(actual_value), greater_than_or_equal_to(value))
 
 
-@step(u"download file as '(?P<file_name>[\S\s]+)' from '(?P<response>[\S\s]+)'")
+@step(u"download file as '{file_name}' from '{response}'")
 def download_file_from_response(context, file_name, response):
     raise NotImplemented
 
 
 def has_json_path(json, path):
     expression = jmespath.compile(path)
     value = expression.search(json)
```

### Comparing `qaf-python-1.0.0/qaf/automation/ui/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/ui/webdriver/base_test_page.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,15 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
+from qaf.automation.core.test_base import get_driver
+from qaf.automation.ui.webdriver.qaf_web_driver import QAFWebDriver
 
+
+class BaseTestPage:
+    @property
+    def driver(self) -> QAFWebDriver:
+        return get_driver()
```

### Comparing `qaf-python-1.0.0/qaf/automation/ui/js_toolkit.py` & `qaf-python-1.0.0.1/qaf/automation/ui/js_toolkit.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/ui/util/__init__.py` & `qaf-python-1.0.0.1/qaf/automation/integration/testcase_result_updator.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,8 +14,32 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
-from . import qaf_wd_expected_conditions
+from abc import ABC, abstractmethod
+
+from qaf.automation.integration.testcase_run_result import TestCaseRunResult
+
+"""
+    Extend this class to add custom result updator.
+    Register custom updator class using `result.updator` property
+    @author: Chirag Jayswal
+    """
+
+
+class TestCaseResultUpdator(ABC):
+    @abstractmethod
+    def update_result(self, result: TestCaseRunResult) -> bool:
+        pass
+
+    @abstractmethod
+    def get_tool_name(self) -> str:
+        pass
+
+    def before_shutdown(self):
+        pass
+
+    def enabled(self) -> bool:
+        return True
```

### Comparing `qaf-python-1.0.0/qaf/automation/ui/webdriver/abstract_listener.py` & `qaf-python-1.0.0.1/qaf/automation/ui/webdriver/abstract_listener.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/ui/webdriver/base_test_page.py` & `qaf-python-1.0.0.1/qaf/automation/util/directory_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
-from qaf.automation.ui.webdriver.qaf_test_base import QAFTestBase
-from qaf.automation.ui.webdriver.qaf_web_driver import QAFWebDriver
+import os
 
 
-class BaseTestPage:
-    @property
-    def driver(self):
-        return QAFWebDriver(QAFTestBase().get_driver())
+def create_directory(directory):
+    try:
+        if not os.path.exists(directory):
+            os.makedirs(directory)
+    except OSError:
+        print('Error: Creating directory. ' + directory)
```

### Comparing `qaf-python-1.0.0/qaf/automation/ui/webdriver/command_tracker.py` & `qaf-python-1.0.0.1/qaf/automation/ui/webdriver/command_tracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
 
 class CommandTracker:
     def __init__(self, command: str, parameters: dict) -> None:
         self.exception = None
         self.stage = -1
         self.retry = False
-        self.start_time = None
-        self.end_time = None
+        self.start_time = 0
+        self.end_time = 0
         self.response = None
         self.command = command
         self.__parameters = {}
         self.parameters = parameters
 
     @property
     def exception(self) -> Exception:
@@ -69,27 +69,27 @@
         return self.__retry
 
     @retry.setter
     def retry(self, value: bool) -> None:
         self.__retry = value
 
     @property
-    def start_time(self) -> str:
+    def start_time(self) -> int:
         return self.__start_time
 
     @start_time.setter
-    def start_time(self, value: str) -> None:
+    def start_time(self, value: int) -> None:
         self.__start_time = value
 
     @property
-    def end_time(self) -> str:
+    def end_time(self) -> int:
         return self.__end_time
 
     @end_time.setter
-    def end_time(self, value: str) -> None:
+    def end_time(self, value: int) -> None:
         self.__end_time = value
 
     @property
     def response(self) -> dict:
         return self.__response
 
     @response.setter
```

### Comparing `qaf-python-1.0.0/qaf/automation/ui/webdriver/qaf_web_driver.py` & `qaf-python-1.0.0.1/qaf/automation/ui/webdriver/qaf_web_driver.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,124 +13,157 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
-
+import time
 from typing import Optional
 
-from selenium.webdriver.support.wait import WebDriverWait
-
-from qaf.automation.ui import js_toolkit
-from qaf.automation.ui.util.qaf_wd_expected_conditions import WaitForAjax
-from qaf.automation.ui.webdriver.qaf_find_by import get_find_by
+from appium.webdriver import Remote as AppiumDriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver as RemoteWebDriver
-from appium.webdriver.webdriver import WebDriver as AppiumRemoteWebDriver
+from selenium.webdriver.support.expected_conditions import presence_of_element_located
+from selenium.webdriver.support.wait import WebDriverWait
 
 from qaf.automation.core.configurations_manager import ConfigurationsManager as CM
 from qaf.automation.core.load_class import load_class
 from qaf.automation.keys.application_properties import ApplicationProperties as AP
+from qaf.automation.ui import js_toolkit
+from qaf.automation.ui.util.dynamic_wait import DynamicWait
+from qaf.automation.ui.util.locator_util import parse_locator
+from qaf.automation.ui.util.qaf_wd_expected_conditions import WaitForAjax, WaitForAnyPresent
+from qaf.automation.ui.webdriver import qaf_web_element as qafwebelement
 from qaf.automation.ui.webdriver.command_tracker import CommandTracker
-from qaf.automation.ui.webdriver import qaf_web_element as qafwebelement, qaf_test_base
 from qaf.automation.ui.webdriver.qaf_webdriver_listener import QAFWebDriverListener
 
 
 class QAFWebDriver(RemoteWebDriver):
 
-    def __init__(self, driver, browser_profile=None, proxy=None,
+    def __init__(self, under_laying_driver, browser_profile=None, proxy=None,
                  keep_alive=False, file_detector=None, options=None):
-        self.__driver = driver
+        self.__under_laying_driver = under_laying_driver
         self.w3c = False
 
         self.__listeners = []
         self.__listeners.append(QAFWebDriverListener())
 
-        RemoteWebDriver.__init__(self, command_executor=driver.command_executor,
-                                 desired_capabilities=driver.desired_capabilities,
+        RemoteWebDriver.__init__(self, command_executor=under_laying_driver.command_executor,
                                  browser_profile=browser_profile,
                                  proxy=proxy,
-                                 keep_alive=keep_alive, file_detector=file_detector, options=options)
+                                 file_detector=file_detector, options=options)
 
         if CM().contains_key(AP.WEBDRIVER_COMMAND_LISTENERS):
             class_name = CM().get_str_for_key(AP.WEBDRIVER_COMMAND_LISTENERS)
             self.__listeners.append(load_class(class_name)())
 
-    def start_session(self, capabilities: dict, browser_profile=None) -> None:
-        self.command_executor = self.__driver.command_executor
-        self.capabilities = self.__driver.capabilities
-        if hasattr(self.command_executor, 'w3c') and self.command_executor.w3c:
-            self.w3c = self.command_executor.w3c is None
-        self.session_id = self.__driver.session_id
+    def start_client(self):
+        pass
+
+    def stop_client(self):
+        pass
 
-    def find_element(self, by=By.ID, value=None, key=None) -> qafwebelement.QAFWebElement:
+    def start_session(self, capabilities: dict, browser_profile=None) -> None:
+        self.command_executor = self.__under_laying_driver.command_executor
+        try:
+            self.capabilities = self.__under_laying_driver.capabilities
+            self.w3c = self.command_executor.w3c
+        except:
+            self.caps = self.__under_laying_driver.capabilities
+            self.w3c = True
+        self.session_id = self.__under_laying_driver.session_id
+
+    def find_element(self, by: Optional[str] = By.ID, value: Optional[str] = None,
+                     key: Optional[str] = None) -> qafwebelement.QAFWebElement:
+        description = value
+        metadata = {}
         if key is not None and len(key) > 0:
             value = CM().get_str_for_key(key, default_value=key)
-            by, value = get_find_by(value)
+            by, value, description, metadata = parse_locator(value, w3c=self.w3c)
 
         web_element = super(QAFWebDriver, self).find_element(by=by, value=value)
         qaf_web_element = qafwebelement.QAFWebElement.create_instance_using_webelement(web_element)
         qaf_web_element._parent = self
+        qaf_web_element._id = web_element.id
         qaf_web_element.by = by
         qaf_web_element.locator = value
-        qaf_web_element.description = value
+        qaf_web_element.description = description
+        qaf_web_element.metadata = metadata
         return qaf_web_element
 
-    def find_elements(self, by: Optional[str] = By.ID, value: Optional[str] = None, key: Optional[str] = None) -> [
-        qafwebelement.QAFWebElement]:
+    def find_elements(self, by: Optional[str] = By.ID, value: Optional[str] = None, key: Optional[str] = None) -> \
+            [qafwebelement.QAFWebElement]:
+        description = value
+        metadata = {}
         if key is not None and len(key) > 0:
             value = CM().get_str_for_key(key, default_value=key)
-            by, value = get_find_by(value)
+            by, value, description, metadata = parse_locator(value, w3c=self.w3c)
 
         web_elements = super(QAFWebDriver, self).find_elements(by=by, value=value)
         qaf_web_elements = []
         for web_element in web_elements:
             qaf_web_element = qafwebelement.QAFWebElement.create_instance_using_webelement(web_element)
             qaf_web_element._parent = self
+            qaf_web_element._id = web_element.id
             qaf_web_element.by = by
             qaf_web_element.locator = value
-            qaf_web_element.description = value
+            qaf_web_element.description = description
+            qaf_web_element.metadata = metadata
+            qaf_web_element.cacheable = True  # list element needs to be cacheable
             qaf_web_elements.append(qaf_web_element)
         return qaf_web_elements
 
     def wait_for_ajax(self, jstoolkit: Optional[str] = js_toolkit.GLOBAL_WAIT_CONDITION, wait_time: Optional[int] = 0):
-        wait_time_out = CM().get_int_for_key(AP.SELENIUM_WAIT_TIMEOUT) \
-            if wait_time == 0 else wait_time
         message = 'Wait time out for ajax to complete'
-        return WebDriverWait(qaf_test_base.QAFTestBase().get_driver(), wait_time_out).until(
-            WaitForAjax(jstoolkit), message
+        return qaf_webdriver_wait(self, wait_time).until(WaitForAjax(jstoolkit), message)
+
+    def wait_for_any_present(self, locators: [str], wait_time: Optional[int] = 0) -> bool:
+        message = "Wait time out for any of elements [%s] to be present".format(','.join(map(str, locators)))
+        return qaf_webdriver_wait(self, wait_time).until(
+            WaitForAnyPresent(locators), message
         )
 
     def execute(self, driver_command: str, params: dict = None) -> dict:
         command_tracker = CommandTracker(driver_command, params)
         self.before_command(command_tracker)
 
         try:
             if command_tracker.response is None:
+                command_tracker.start_time = round(time.time() * 1000)
                 response = super(QAFWebDriver, self).execute(command_tracker.command,
                                                              command_tracker.parameters)
                 command_tracker.response = response
+                command_tracker.end_time = round(time.time() * 1000)
+                self.after_command(command_tracker)
+
         except Exception as e:
-            self.on_exception(command_tracker)
+            self.after_command(command_tracker)
             command_tracker.exception = e
+            self.on_exception(command_tracker)
 
+        command_tracker.end_time = round(time.time() * 1000)
         if command_tracker.has_exception():
             if command_tracker.retry:
                 response = super(QAFWebDriver, self).execute(command_tracker.command,
                                                              command_tracker.parameters)
                 command_tracker.response = response
                 command_tracker.exception = None
             else:
                 raise command_tracker.exception
 
-        self.after_command(command_tracker)
         return command_tracker.response
 
+    def load(self, element: qafwebelement.QAFWebElement):
+        wait_time_out = CM().get_int_for_key(AP.SELENIUM_WAIT_TIMEOUT)
+        web_element = WebDriverWait(self, wait_time_out).until(
+            presence_of_element_located((element.by, element.locator)))
+        qafwebelement.QAFWebElement.create_instance_using_webelement(web_element)
+        return web_element.id
+
     # Listener methods
     def before_command(self, command_tracker: CommandTracker) -> None:
         if self.__listeners is not None:
             for listener in self.__listeners:
                 listener.before_command(self, command_tracker)
 
     def after_command(self, command_tracker: CommandTracker) -> None:
@@ -139,10 +172,31 @@
                 listener.after_command(self, command_tracker)
 
     def on_exception(self, command_tracker: CommandTracker) -> None:
         if self.__listeners is not None:
             for listener in self.__listeners:
                 listener.on_exception(self, command_tracker)
 
-
-class QAFAppiumWebDriver(AppiumRemoteWebDriver, QAFWebDriver):
-    pass
+    @property
+    def under_laying_driver(self):
+        return self if self.__under_laying_driver is None else self.__under_laying_driver
+
+    @property
+    def to_selenium_webdriver(self) -> RemoteWebDriver:
+        return self if self.__under_laying_driver is None else self.__under_laying_driver
+
+    @property
+    def to_appium_webdriver(self) -> AppiumDriver:
+        return self if self.__under_laying_driver is None else self.__under_laying_driver
+
+    @property
+    def capabilities(self):
+        return self._capabilities
+
+    @capabilities.setter
+    def capabilities(self, value):
+        self._capabilities = value
+
+
+def qaf_webdriver_wait(driver: QAFWebDriver, timeout,
+                       ignored_exceptions=None) -> DynamicWait[QAFWebDriver]:
+    return DynamicWait[QAFWebDriver](driver, timeout, ignored_exceptions=ignored_exceptions)
```

### Comparing `qaf-python-1.0.0/qaf/automation/ui/webdriver/qaf_webdriver_listener.py` & `qaf-python-1.0.0.1/qaf/automation/ui/webdriver/qaf_webdriver_listener.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,49 +14,63 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
+import logging
 import sys
 
-from qaf.automation.ui.webdriver.command_tracker import CommandTracker
-
-from qaf.automation.formatter.qaf_report.scenario.command_log import CommandLog, CommandLogStack
+from qaf.automation.core.command_log_bean import CommandLogBean
+from qaf.automation.core.test_base import add_command
+# from qaf.automation.formatter.qaf_report.scenario.command_log import CommandLog, CommandLogStack
 from qaf.automation.ui.webdriver.abstract_listener import DriverListener
-import logging
+from qaf.automation.ui.webdriver.command_tracker import CommandTracker
 
 
 class QAFWebDriverListener(DriverListener):
     __streaming_handler = logging.StreamHandler(sys.stdout)
     __logger = logging.getLogger()
     __logger.setLevel(logging.INFO)
     __logger.addHandler(__streaming_handler)
 
     def on_exception(self, driver, command_tracker: CommandTracker):
-        selenium_log = CommandLog()
+        from qaf import pluginmagager
+        pluginmagager.hook.on_driver_command_failure(driver=driver, command_tracker=command_tracker)
+        selenium_log = CommandLogBean()
         selenium_log.commandName = command_tracker.command
         selenium_log.result = command_tracker.message
-        selenium_log.args = command_tracker.parameters
-        CommandLogStack().add_command_log(selenium_log)
+        selenium_log.args = [str(command_tracker.parameters)]
+        selenium_log.duration = command_tracker.end_time - command_tracker.start_time
+        # CommandLogStack().add_command_log(selenium_log)
+        add_command(selenium_log)
         self.__logger.info(selenium_log.to_string())
 
     def after_command(self, driver, command_tracker: CommandTracker):
+        from qaf import pluginmagager
+        pluginmagager.hook.after_driver_command(driver=driver, command_tracker=command_tracker)
+
         if not is_command_excluded_from_logging(command_tracker.command):
-            selenium_log = CommandLog()
+            selenium_log = CommandLogBean()
             selenium_log.commandName = command_tracker.command
             selenium_log.result = 'OK' if (
-                        command_tracker.response is None or 'status' not in command_tracker.response) else \
-            command_tracker.response['status']
-            selenium_log.args = command_tracker.parameters
-            CommandLogStack().add_command_log(selenium_log)
+                    command_tracker.response is None or 'value' not in command_tracker.response) else \
+                str(command_tracker.response['value'])
+            selenium_log.args = [str(command_tracker.parameters)]
+            selenium_log.duration = command_tracker.end_time - command_tracker.start_time
+            # CommandLogStack().add_command_log(selenium_log)
+            add_command(selenium_log)
             self.__logger.info(selenium_log.to_string())
 
     def before_command(self, driver, command_tracker: CommandTracker):
+        from qaf import pluginmagager
+
+        pluginmagager.hook.before_driver_command(driver=driver, command_tracker=command_tracker)
+
         self.__logger.info('Executing ' + command_tracker.command +
                            ' Parameters: ' + str(command_tracker.parameters))
 
 
 excludeCommandsFromLogging = ['getHtmlSource', 'captureEntirePageScreenshotToString', 'executeScript', 'screenshot']
```

### Comparing `qaf-python-1.0.0/qaf/automation/util/string_util.py` & `qaf-python-1.0.0.1/qaf/automation/util/string_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-
 #  Copyright (c) 2022 Infostretch Corporation
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -50,14 +49,16 @@
     'reverse',
     'uuid',
     'shuffle',
     'strip_html',
     'prettify',
     'slugify',
     'to_boolean',
+    'decode_base64',
+    'encode_base64',
 ]
 
 # compiled regex
 URL_RE = re.compile(
     r'^'
     r'([a-z-]+://)'  # scheme
     r'([a-z_\d-]+:[a-z_\d-]+@)?'  # user:password
@@ -644,8 +645,18 @@
     # translate non-ascii signs
     s = unicodedata.normalize('NFD', s).encode('ascii', 'ignore').decode('utf-8')
 
     return s
 
 
 def to_boolean(string):
-    return string.lower() in ("yes", "true", "t", "1", "yes")
+    return string.lower() in ("yes", "true", "t", "1", "y")
+
+
+def decode_base64(string: str) -> str:
+    import base64
+    return base64.b64decode(string).decode('utf-8')
+
+
+def encode_base64(string: str) -> str:
+    import base64
+    return base64.b64encode(string.encode('utf-8'))
```

### Comparing `qaf-python-1.0.0/qaf/automation/util/validator.py` & `qaf-python-1.0.0.1/qaf/automation/util/validator.py`

 * *Files identical despite different names*

### Comparing `qaf-python-1.0.0/qaf/automation/ws/rest/ws_listener.py` & `qaf-python-1.0.0.1/qaf/automation/ws/rest/ws_listener.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,38 +17,46 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 import logging
 import sys
 
-from qaf.automation.ui.webdriver.command_tracker import CommandTracker
-
-from qaf.automation.formatter.qaf_report.scenario.command_log import CommandLog, CommandLogStack
+from qaf.automation.core.command_log_bean import CommandLogBean
+from qaf.automation.core.test_base import add_command
+# from qaf.automation.formatter.qaf_report.scenario.command_log import CommandLog, CommandLogStack
 from qaf.automation.ui.webdriver.abstract_listener import DriverListener
+from qaf.automation.ui.webdriver.command_tracker import CommandTracker
 
 
 class WsListener(DriverListener):
     __streaming_handler = logging.StreamHandler(sys.stdout)
     __logger = logging.getLogger()
     __logger.setLevel(logging.INFO)
     __logger.addHandler(__streaming_handler)
 
     def before_command(self, driver, command_tracker: CommandTracker) -> None:
-        commandlog = CommandLog()
-        commandlog.commandName = command_tracker.command
-        commandlog.result = command_tracker.message
-        commandlog.args = command_tracker.parameters
-        CommandLogStack().add_command_log(commandlog)
-        self.__logger.info(commandlog.to_string())
+        self.__logger.info('Executing ' + command_tracker.command +
+                           ' Parameters: ' + str(command_tracker.parameters))
 
     def after_command(self, driver, command_tracker: CommandTracker) -> None:
-        commandlog = CommandLog()
+        commandlog = CommandLogBean()
         commandlog.commandName = command_tracker.command
-        commandlog.result = command_tracker.response if command_tracker.response is not None else command_tracker.response['status_code']
-        commandlog.args = command_tracker.parameters
-        CommandLogStack().add_command_log(commandlog)
+        commandlog.result = command_tracker.response.text if command_tracker.response is not None else command_tracker.response['status_code']
+        commandlog.args = [str(command_tracker.parameters)]
+        commandlog.duration = command_tracker.end_time - command_tracker.start_time
+
+        #CommandLogStack().add_command_log(commandlog)
+        add_command(commandlog)
         self.__logger.info(commandlog.to_string())
 
     def on_exception(self, driver, command_tracker: CommandTracker) -> None:
-        self.__logger.info('Executing ' + command_tracker.command +
+        self.__logger.info('exception ' + command_tracker.command +
                            ' Parameters: ' + str(command_tracker.parameters))
+        commandlog = CommandLogBean()
+        commandlog.commandName = command_tracker.command
+        commandlog.result = command_tracker.message
+        commandlog.args = [str(command_tracker.parameters)]
+        commandlog.duration = command_tracker.end_time - command_tracker.start_time
+        # CommandLogStack().add_command_log(commandlog)
+        add_command(commandlog)
+        self.__logger.info(commandlog.to_string())
```

### Comparing `qaf-python-1.0.0/qaf/automation/ws/rest/ws_request.py` & `qaf-python-1.0.0.1/qaf/automation/ws/rest/ws_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
+import time
 
 import requests
 from requests import PreparedRequest
 
 from qaf.automation.core.configurations_manager import ConfigurationsManager as CM
 from qaf.automation.core.load_class import load_class
 from qaf.automation.keys.application_properties import ApplicationProperties as AP
@@ -36,48 +37,58 @@
         self.__listeners = []
         self.__listeners.append(WsListener())
 
         if CM().contains_key(AP.WEBSERVICE_COMMAND_LISTENERS):
             class_name = CM().get_str_for_key(AP.WEBSERVICE_COMMAND_LISTENERS)
             self.__listeners.append(load_class(class_name)())
 
-    def request(self, request_bean: WsRequestBean) -> dict:
-        command_tracker = CommandTracker(request_bean.endPoint, request_bean.to_string)
+    def request(self, request_bean: WsRequestBean, params="{}") -> dict:
+        request_bean.resolve_parameters(params)
+        command_tracker = CommandTracker(f'{request_bean.method} {request_bean.url}', request_bean.to_dict())
         s, prep, send_kwargs = self.prepare_request(request_bean)
         self.before_command(command_tracker)
-
+        command_tracker.start_time = round(time.time() * 1000)
         try:
-            WsRequest.response = s.send(prep, **send_kwargs).json()
+            WsRequest.response = s.send(prep, **send_kwargs)
+            request = WsRequest.response.request.prepare() if isinstance(WsRequest.response.request, requests.Request) else WsRequest.response.request
+            headers = '\r\n'.join(f'{k}: {v}' for k, v in request.headers.items())
+            body = '' if request.body is None else request.body.decode() if isinstance(request.body,
+                                                                                       bytes) else request.body
+            #command_tracker = CommandTracker(f'{request.method} {request.url}{request.path_url}', {"headers":headers,"body":body })
+            command_tracker.command=f'{request.method} {request.url}{request.path_url}'
+            command_tracker.parameters= {"headers":headers,"body":body }
             command_tracker.response = WsRequest.response
+            command_tracker.end_time = round(time.time() * 1000)
+            self.after_command(command_tracker)
 
         except Exception as e:
-            self.on_exception(command_tracker)
+            command_tracker.end_time = round(time.time() * 1000)
             command_tracker.exception = e
+            self.on_exception(command_tracker)
 
         if command_tracker.has_exception():
             if command_tracker.retry:
                 WsRequest.response = s.send(prep, **send_kwargs)
                 command_tracker.response = WsRequest.response
                 command_tracker.exception = None
             else:
                 raise command_tracker.exception
-        self.after_command(command_tracker)
         return command_tracker.response
 
     def prepare_request(self, request_bean: WsRequestBean) -> (requests.Session, PreparedRequest, dict):
         s = requests.Session()
 
         req = requests.Request(
             method=request_bean.method.upper(),
             url=request_bean.url,
             headers=request_bean.headers,
             files=request_bean.files,
-            data=request_bean.data or {},
-            json=request_bean.json,
-            params=request_bean.params or {},
+            data=request_bean.body or request_bean.formParameters or {},
+            # json=request_bean.json,
+            params=request_bean.queryParameters or {},
             auth=request_bean.auth,
             cookies=request_bean.cookies,
             hooks=request_bean.hooks,
         )
 
         prep = s.prepare_request(req)
```

### Comparing `qaf-python-1.0.0/setup.py` & `qaf-python-1.0.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,58 +23,49 @@
 try:
     with open('README.md') as f:
         readme = f.read()
 except FileNotFoundError:
     readme = ""
 
 setup(name='qaf-python',
-      version='1.0.0',
+      version='1.0.0.1',
       description='This is Automation framework for Python developed by Infostretch',
-      author='Nishith Shah',
+      author='Nishith Shah, Chirag Jayswal',
       author_email='nishith.shah@infostretch.com',
       license='MIT',
 
       # The project's main homepage.
       url='https://github.com/qmetry/qaf-python',
 
       long_description=readme,
       long_description_content_type="text/markdown",
       maintainer_email='nishith.shah@infostretch.com',
-
-      # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
+      entry_points={"pytest11": ["qaf = qaf.pytest.qaf_pytest_plugin"]},
       classifiers=[
-
-          # How mature is this project? Common values are
-          #   3 - Alpha
-          #   4 - Beta
-          #   5 - Production/Stable
           'Development Status :: 4 - Beta',
-
-          # Indicate who your project is intended for
           'Intended Audience :: Developers',
-
           'Natural Language :: English',
           'Operating System :: OS Independent',
-
           'License :: OSI Approved :: MIT License',
-          # Specify the Python versions you support here. In particular, ensure
           'Programming Language :: Python :: 3',
           'Topic :: Software Development :: Quality Assurance',
           'Topic :: Software Development :: Testing',
       ],
 
       keywords='qaf, bdd, automation, python-selenium, python-automation, appium, python-appium',
       packages=find_packages(),
       python_requires=">=3.6",
       package_data={
           'qaf.automation': ['config/*.ini']
       },
       install_requires=[
-          'selenium==3.14.1',
-          'Appium-Python-Client==0.48',
-          'behave==1.2.6',
-          'PyHamcrest==1.9.0',
-          'requests==2.20.0',
-          'jmespath==1.0.0',
-          'webdriver-manager==3.5.4'
+          'selenium~=4.9.1',
+          'Appium-Python-Client~=2.10.1',
+          'behave~=1.2.6',
+          'PyHamcrest~=1.9.0',
+          'requests~=2.31.0',
+          'jmespath~=1.0.0',
+          'webdriver-manager~=3.8.6',
+          'simpleeval==0.9.13',
+          'pytest~=7.3.1'
       ],
       zip_safe=False)
```

