# Comparing `tmp/zerobug-2.0.8.tar.gz` & `tmp/zerobug-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zerobug-2.0.8.tar", last modified: Tue May 30 10:38:41 2023, max compression
+gzip compressed data, was "dist/zerobug-2.0.9.tar", last modified: Fri Jul 14 05:26:50 2023, max compression
```

## Comparing `zerobug-2.0.8.tar` & `zerobug-2.0.9.tar`

### file list

```diff
@@ -1,59 +1,73 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/__main__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    23977 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/z0testrc
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug/dummy/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      121 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/dummy/dummylib.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)       47 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/dummy/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2877 2023-05-30 10:36:16.000000 zerobug-2.0.8/zerobug/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/scripts/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug/_travis/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1852 2023-04-14 14:02:41.000000 zerobug-2.0.8/zerobug/_travis/travis_after_tests_success
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17892 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/_travis/travis_run_pypi_tests
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug/_travis/cfg/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_pr.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      534 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1126 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/coveragerc
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      716 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      122 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_shellcheck.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      703 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      690 2023-01-30 07:04:22.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      132 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_shellcheck_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      629 2023-01-30 06:58:04.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      152 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_shellcheck_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      533 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      704 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_beta.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    24224 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/_travis/travis_install_env
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1361 2023-01-27 07:10:19.000000 zerobug-2.0.8/zerobug/_travis/build_cmd
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/_travis/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    60073 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/z0testlib.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      574 2023-05-30 10:36:08.000000 zerobug-2.0.8/zerobug/zerobug.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      157 2022-12-09 05:08:44.000000 zerobug-2.0.8/zerobug/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        8 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-09 06:43:26.000000 zerobug-2.0.8/zerobug.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       91 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1946 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       70 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15072 2023-05-30 10:38:41.000000 zerobug-2.0.8/zerobug.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-30 10:38:41.000000 zerobug-2.0.8/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2877 2023-05-30 10:36:08.000000 zerobug-2.0.8/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15072 2023-05-30 10:38:41.000000 zerobug-2.0.8/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    10940 2023-05-30 10:38:35.000000 zerobug-2.0.8/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 05:26:50.000000 zerobug-2.0.9/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2023-06-22 02:31:29.000000 zerobug-2.0.9/zerobug/__main__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2378 2023-07-12 13:37:46.000000 zerobug-2.0.9/zerobug/py2_template.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    23977 2023-06-27 17:52:42.000000 zerobug-2.0.9/zerobug/z0testrc
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug/dummy/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      121 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/dummy/dummylib.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)       47 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/dummy/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug/tests/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1220 2023-06-27 17:52:42.000000 zerobug-2.0.9/zerobug/tests/test_03_internal_sanity_check.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8156 2023-07-09 19:50:20.000000 zerobug-2.0.9/zerobug/tests/test_07_odoo.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1824 2023-06-27 17:52:42.000000 zerobug-2.0.9/zerobug/tests/test_05_os_tree.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      883 2023-07-11 17:04:23.000000 zerobug-2.0.9/zerobug/tests/test_01_internal_version.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1535 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/tests/conftest.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      262 2023-06-22 02:31:04.000000 zerobug-2.0.9/zerobug/tests/dummy_01.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      763 2023-06-27 17:52:42.000000 zerobug-2.0.9/zerobug/tests/__pytest_sample.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1216 2023-07-11 14:40:37.000000 zerobug-2.0.9/zerobug/tests/test_01_internal_version_old.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       49 2023-07-12 13:37:46.000000 zerobug-2.0.9/zerobug/tests/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2055 2023-07-12 13:37:46.000000 zerobug-2.0.9/zerobug/py3_template.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2956 2023-07-14 05:08:46.000000 zerobug-2.0.9/zerobug/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6814 2023-06-27 17:52:42.000000 zerobug-2.0.9/zerobug/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/scripts/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug/_travis/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1876 2023-06-24 06:17:11.000000 zerobug-2.0.9/zerobug/_travis/travis_after_tests_success
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17892 2023-06-27 17:52:42.000000 zerobug-2.0.9/zerobug/_travis/travis_run_pypi_tests
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      144 2023-07-11 17:18:45.000000 zerobug-2.0.9/zerobug/_travis/__init__.pyc
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug/_travis/cfg/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_pr.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      534 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1148 2023-06-24 06:17:11.000000 zerobug-2.0.9/zerobug/_travis/cfg/coveragerc
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      716 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      122 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_shellcheck.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      703 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      690 2023-01-30 07:04:22.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8__init__AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      132 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_shellcheck_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      629 2023-01-30 06:58:04.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8__init__.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      152 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_shellcheck_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      533 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      704 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8__init__NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_beta.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    24224 2023-06-27 17:52:42.000000 zerobug-2.0.9/zerobug/_travis/travis_install_env
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1361 2023-07-09 06:55:30.000000 zerobug-2.0.9/zerobug/_travis/build_cmd
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        0 2023-06-24 06:17:11.000000 zerobug-2.0.9/zerobug/_travis/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    65304 2023-07-13 19:26:06.000000 zerobug-2.0.9/zerobug/z0testlib.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      574 2023-06-27 17:52:42.000000 zerobug-2.0.9/zerobug/zerobug.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      157 2022-12-09 05:08:44.000000 zerobug-2.0.9/zerobug/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2692 2023-07-12 13:37:46.000000 zerobug-2.0.9/zerobug/py23_template.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        8 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-09 06:43:26.000000 zerobug-2.0.9/zerobug.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       91 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2357 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       70 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    19958 2023-07-14 05:26:50.000000 zerobug-2.0.9/zerobug.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-07-14 05:26:50.000000 zerobug-2.0.9/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2956 2023-07-14 05:07:08.000000 zerobug-2.0.9/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    19958 2023-07-14 05:26:50.000000 zerobug-2.0.9/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14770 2023-07-14 05:26:26.000000 zerobug-2.0.9/README.rst
```

### Comparing `zerobug-2.0.8/zerobug/z0testrc` & `zerobug-2.0.9/zerobug/z0testrc`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 # WLOGCMD:        oveerride opt_echo; may be None, 'echo', 'echo-1' or 'echo-0'
 #
 # This free software is released under GNU Affero GPL3
 # author: Antonio M. Vigliotti - antoniomaria.vigliotti@gmail.com
 # (C) 2015-2023 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
 #
 
-__version__=2.0.8
+__version__=2.0.9
 
 export opt_dry_run
 export ctr
 export opt_verbose
 export max_test
 export min_test
 export opt_noctr
```

### Comparing `zerobug-2.0.8/zerobug/scripts/setup.info` & `zerobug-2.0.9/zerobug/scripts/setup.info`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# -*- coding: utf-8 -*-
+import os.path as pth
 import sys
 
 from setuptools import find_packages, setup
 
 author = "Antonio Maria Vigliotti"
 author_email = "<info@shs-av.com>"
 source_url = "https://github.com/zeroincombenze/tools/tree/master/zerobug"
@@ -33,18 +35,18 @@
             'os0',
             'z0lib',
         ],
     )
 
 setup(
     name='zerobug',
-    version='2.0.8',
+    version='2.0.9',
     description='Zeroincombenze continuous testing framework'
     ' and tools for python and bash programs',
-    long_description=open("README.rst").read(),
+    long_description=open(pth.join(pth.dirname(__file__), "README.rst")).read(),
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `zerobug-2.0.8/zerobug/scripts/main.py` & `zerobug-2.0.9/zerobug/scripts/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
@@ -58,16 +58,17 @@
     local_venv = "/devel/venv/"
     pkgpath = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
     bin_path = lib_path = ""
     path = pkgpath
     while not bin_path and path != "/" and path != os.environ["HOME"]:
         path = os.path.dirname(path)
         if os.path.isdir(path) and os.path.basename(path) in ("bin", "lib"):
-            if (os.path.isdir(os.path.join(os.path.dirname(path), "bin")) and
-                    os.path.isdir(os.path.join(os.path.dirname(path), "lib"))):
+            if os.path.isdir(
+                os.path.join(os.path.dirname(path), "bin")
+            ) and os.path.isdir(os.path.join(os.path.dirname(path), "lib")):
                 bin_path = os.path.join(os.path.dirname(path), "bin")
                 lib_path = os.path.join(os.path.dirname(path), "lib")
     if not bin_path and local_venv:
         for path in sys.path:
             if local_venv in path:
                 bin_path = os.path.join(
                     path[: path.find(local_venv)],
```

### Comparing `zerobug-2.0.8/zerobug/_travis/travis_after_tests_success` & `zerobug-2.0.9/zerobug/_travis/travis_after_tests_success`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python
+# -*- coding: utf-8 -*-
 
 from __future__ import print_function
 
 import os
 import sys
 
 from coverage.cmdline import main as coverage_main
```

### Comparing `zerobug-2.0.8/zerobug/_travis/travis_run_pypi_tests` & `zerobug-2.0.9/zerobug/_travis/travis_run_pypi_tests`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.8
+__version__=2.0.9
 
 
 travis_test_bash() {
     echo "======== Testing test_bash   ========"
     local s sts
     sts=0
     if [ ${opt_dry_run:-0} -eq 0 ]; then
```

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_pr.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_pr.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_70.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_70.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/coveragerc` & `zerobug-2.0.9/zerobug/_travis/cfg/coveragerc`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     */site-packages/*
     */lib/python*/*
     */lib64/python*/*
     */venv_odoo/*
     */__init__.py
     */__openerp__.py
     */__manifest__.py
+    */_check4deps_.py
 # Regexes for lines to exclude from consideration
 exclude_lines =
     # Have to re-enable the standard pragma
     pragma: no cover
 
     # Don't complain about null context checking
     if context is None:
```

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8__init__.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8__init__.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_61.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_61.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_pylint_beta.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_pylint_beta.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg` & `zerobug-2.0.9/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/_travis/travis_install_env` & `zerobug-2.0.9/zerobug/_travis/travis_install_env`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.8
+__version__=2.0.9
 
 
 run_traced() {
   [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x
   [[ -z ${Z0_STACK:+_} ]] && export Z0_STACK=0
   ((Z0_STACK=Z0_STACK+2))
   local xcmd="$1" lm="                    "
```

### Comparing `zerobug-2.0.8/zerobug/_travis/build_cmd` & `zerobug-2.0.9/zerobug/_travis/build_cmd`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.8/zerobug/z0testlib.py` & `zerobug-2.0.9/zerobug/z0testlib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2015-2023 SHS-AV s.r.l. (<http://www.zeroincombenze.org>)
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 from __future__ import print_function, unicode_literals
+from builtins import str as text
+from io import open
 
 import argparse
 import glob
 import os
 import shutil
 import stat
 import subprocess
+
 # import os.path
 import sys
 from string import Template
 from subprocess import PIPE, Popen
 
+import unittest
+
 import magic
 
 from os0 import os0
 from python_plus import _c
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 # return code
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 if os.name == "posix":
     RED = "\033[1;31m"
     GREEN = "\033[1;32m"
@@ -143,14 +148,131 @@
     if False:
 
     # Ignore unit test failure
     return TEST_FAILED
 """
 
 
+class PypiTest(unittest.TestCase):
+
+    def setUp(self):
+        self.assert_counter = 0
+
+    def tearDown(self):
+        # print("🏆🥇 %d tests SUCCESSFULLY completed" % self.assert_counter)
+        print("%d tests SUCCESSFULLY completed" % self.assert_counter)
+
+    def version(self):
+        return __version__
+
+    # ----------------------------------
+    # --  Counted assertion functions --
+    # ----------------------------------
+
+    def assertFalse(self, expr, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertFalse(expr, msg=msg)
+
+    def assertTrue(self, expr, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertTrue(expr, msg=msg)
+
+    def assertRaises(self, expected_exception, *args, **kwargs):     # pragma: no cover
+        self.assert_counter += 1
+        return super(PypiTest, self).assertRaises(expected_exception, *args, **kwargs)
+
+    def assertEqual(self, first, second, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertEqual(first, second, msg=msg)
+
+    def assertNotEqual(self, first, second, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertNotEqual(first, second, msg=msg)
+
+    def assertIn(self, member, container, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertIn(member, container, msg=msg)
+
+    def assertNotIn(self, member, container, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertNotIn(member, container, msg=msg)
+
+    def assertIs(self, expr1, expr2, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertIs(expr1, expr2, msg=msg)
+
+    def assertIsNot(self, expr1, expr2, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertIsNot(expr1, expr2, msg=msg)
+
+    def assertLess(self, a, b, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertLess(a, b, msg=msg)
+
+    def assertLessEqual(self, a, b, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertLessEqual(a, b, msg=msg)
+
+    def assertGreater(self, a, b, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertGreater(a, b, msg=msg)
+
+    def assertGreaterEqual(self, a, b, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertGreaterEqual(a, b, msg=msg)
+
+    def assertIsNone(self, obj, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertIsNone(obj, msg=msg)
+
+    def assertIsNotNone(self, obj, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertIsNotNone(obj, msg=msg)
+
+    def assertIsInstance(self, obj, cls, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertIsInstance(obj, cls, msg=msg)
+
+    def assertNotIsInstance(self, obj, cls, msg=None, msg_info=None):
+        self.assert_counter += 1
+        if msg_info:
+            print(("%d. " % self.assert_counter) + msg_info)
+        return super(PypiTest, self).assertNotIsInstance(obj, cls, msg=msg)
+
+
 class Macro(Template):
     delimiter = '${'
     idpattern = r'[^}]+?}'
 
     def substitute(self, **kwargs):
         nk = {}
         for k, v in kwargs.items():
@@ -383,21 +505,24 @@
                 this_fqn = sys.argv[0]
             else:
                 argv = []
         else:
             self.autorun = True
         this_fqn = os.path.abspath(this_fqn or self._get_this_fqn())
         this = os.path.splitext(os.path.basename(this_fqn))[0]
-        this_dir = os.getcwd()
-        if not os.path.basename(this_dir) == 'tests' and not os.path.isdir('./tests'):
+        this_dir = os.path.abspath(os.getcwd())
+        if (
+                not os.path.basename(this_dir) == 'tests'
+                and not os.path.isdir(os.path.join(this_dir, 'tests'))
+        ):
             this_dir = os.path.dirname(this_fqn)
         self.this_dir = this_dir
         if os.path.basename(this_dir) == 'tests':
             self.testdir = self.this_dir
-            self.rundir = os.path.abspath(os.path.join(self.this_dir, '..'))
+            self.rundir = os.path.dirname(self.this_dir)
         else:  # pragma: no cover
             if os.path.isdir('./tests'):
                 self.testdir = os.path.join(self.this_dir, 'tests')
             else:
                 self.testdir = self.this_dir
             self.rundir = self.this_dir
         # Testing package dir must be the 1.st one in sys.path
@@ -406,18 +531,15 @@
             ix = sys.path.index(this_pkg_dir)
             del sys.path[ix]
         sys.path.insert(0, this_pkg_dir)
 
         if not id:
             if this.startswith('test_'):
                 id = this[5:]
-            elif (
-                this.startswith('zerobug')
-                or this == '__main__'
-            ):
+            elif this.startswith('zerobug') or this == '__main__':
                 id = os.path.basename(self.rundir)
             else:
                 id = this
             if id[-3:] >= '_00' and id[-3:] <= '_99':
                 id = id[0:-3]
             if id[-5:] == '_test':
                 id = id[0:-5]
@@ -1031,14 +1153,19 @@
             elif TestCls and hasattr(TestCls, testname):
                 sts = getattr(T, testname)(ctx)
             elif os.path.splitext(basetn)[0] != ctx['this']:
                 mime = magic.Magic(mime=True).from_file(os.path.realpath(testname))
                 if os.path.dirname(testname) == "":
                     testname = os.path.join(self.testdir, testname)
                 if mime == 'text/x-python':
+                    with open(os.path.realpath(testname), "r", encoding="utf-8") as fd:
+                        content = fd.read()
+                    if "\nimport unittest\n" in content:
+                        opt4childs = []
+                        del content
                     if os.environ.get('TRAVIS_PDB') == 'true':
                         if ctx.get('python3', False):
                             test_w_args = [
                                 'python3',
                                 '-m',
                                 'pdb',
                                 testname,
@@ -1094,16 +1221,19 @@
             T.teardown(ctx)
         return sts
 
     def main_local(self, ctx, Test, UT1=None, UT=None):
         """Default main program for local tests"""
         # self.dbgmsg(ctx, '>>> main_local(%s)' % Test)
         test_list = sorted(
-            [meth for meth in dir(Test)
-             if meth.startswith("test_") and callable(getattr(Test, meth))]
+            [
+                meth
+                for meth in dir(Test)
+                if meth.startswith("test_") and callable(getattr(Test, meth))
+            ]
         )
         if not ctx.get('opt_noctr', False):
             self._exec_tests_4_count(test_list, ctx, Test)
         if ctx.get('dry_run', False):
             if not ctx.get('_run_autotest', False):
                 print(ctx['max_test'])
             sts = TEST_SUCCESS
@@ -1146,26 +1276,31 @@
             # Discover test files
             test_list = []
             for pattern in (
                 ctx['opt_pattern'] and ctx['opt_pattern'].split(',') or self.pattern
             ):
                 t_list = glob.glob(os.path.abspath(os.path.join(self.testdir, pattern)))
                 if not pattern.endswith(".py") and not pattern.endswith(".sh"):
-                    t_list += glob.glob(os.path.abspath(os.path.join(self.testdir,
-                                                                     pattern + ".py")))
-                    t_list += glob.glob(os.path.abspath(os.path.join(self.testdir,
-                                                                     pattern + ".sh")))
+                    t_list += glob.glob(
+                        os.path.abspath(os.path.join(self.testdir, pattern + ".py"))
+                    )
+                    t_list += glob.glob(
+                        os.path.abspath(os.path.join(self.testdir, pattern + ".sh"))
+                    )
                 for fn in sorted(t_list):
                     mime = magic.Magic(mime=True).from_file(os.path.realpath(fn))
                     if mime in ('text/x-python', 'text/x-shellscript'):
                         test_list.append(fn)
         if len(test_list) == 0 and Test is not None:
             test_list = sorted(
-                [meth for meth in dir(Test)
-                 if meth.startswith("test_") and callable(getattr(Test, meth))]
+                [
+                    meth
+                    for meth in dir(Test)
+                    if meth.startswith("test_") and callable(getattr(Test, meth))
+                ]
             )
         if not ctx.get('opt_noctr', False):
             self._exec_tests_4_count(test_list, ctx, Test)
         if ctx.get('dry_run', False):
             if not ctx.get('_run_autotest', False):
                 print(ctx['ctr'])
             sts = TEST_SUCCESS
@@ -1314,15 +1449,14 @@
             else:
                 self.testdir = self.this_dir
             self.rundir = self.this_dir
 
     def simulate_install_pypi(self, cmd):
         """Simulate pip post installation for"""
         PYCODE = r"""#!%(exec)s
-# -*- coding: utf-8 -*-
 import re
 import sys
 if sys.version_info[0] == 2:
     from %(pypi)s.scripts.%(cmd)s import main
 else:
     from .%(pypi)s.scripts.%(cmd)s import main
 if __name__ == '__main__':
@@ -1389,28 +1523,26 @@
     def build_odoo_env(self, ctx, version, hierarchy=None, name=None, retodoodir=None):
         """Build a simplified Odoo directory tree
         version: 16.0, 15.0, 14.0, 13.0, ..., 7.0, 6.1
         name: name of odoo dir (default equal to version)
         hierarchy: flat,tree,server (def=flat)
         """
         name = name or version
-        if version in ('10.0', '11.0', '12.0', '13.0', '14.0', '15.0', '16.0'):
-            if hierarchy == 'tree':
-                odoo_home = os.path.join(name, 'odoo', 'odoo')
-            else:
-                odoo_home = os.path.join(name, 'odoo')
-            script = 'odoo-bin'
-        elif version in ('6.1', '7.0', '8.0', '9.0'):
+        if int(version.split(".")[0]) < 10:
             if hierarchy == 'server':
                 odoo_home = os.path.join(name, 'server', 'openerp')
             else:
                 odoo_home = os.path.join(name, 'openerp')
             script = 'openerp-server'
         else:
-            raise KeyError('Invalid Odoo version')
+            if hierarchy == 'tree':
+                odoo_home = os.path.join(name, 'odoo', 'odoo')
+            else:
+                odoo_home = os.path.join(name, 'odoo')
+            script = 'odoo-bin'
         os_tree = [
             name,
             os.path.join(name, 'addons'),
             odoo_home,
             os.path.join(odoo_home, 'addons'),
             os.path.join(odoo_home, 'osv'),
             os.path.join(odoo_home, 'service'),
@@ -1441,23 +1573,29 @@
             versions = version.split('.')
             fd.write(RELEASE_PY % (versions[0], versions[1]))
         for fn in ("osv", "service", "tools"):
             with open(os.path.join(odoo_home, fn, "__init__.py"), 'w') as fd:
                 fd.write('print("Fake Odoo")\n')
         init_py = ""
         for fn in (script, "models.py", "fields.py", "api.py"):
-            if fn == "apy.py" and (version.startswith("6") or version.startswith("7")):
+            if fn == "api.py" and (version.startswith("6") or version.startswith("7")):
                 continue
             if fn == script:
+                ffn = os.path.join(os.path.dirname(odoo_home), fn)
                 for fn2 in ("release", "osv", "service", "tools"):
                     init_py += "import %s\n" % fn2
             else:
+                ffn = os.path.join(odoo_home, fn)
                 init_py += "import %s\n" % fn[:-3]
-            with open(os.path.join(odoo_root, fn), 'w') as fd:
+            with open(ffn, 'w') as fd:
                 fd.write('print("Fake Odoo")\n')
+                if fn == script:
+                    mode = os.fstat(fd.fileno()).st_mode
+                    mode |= stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH
+                    os.fchmod(fd.fileno(), stat.S_IMODE(mode))
         with open(os.path.join(odoo_home, "__init__.py"), 'w') as fd:
             fd.write(init_py)
         with open(os.path.join(odoo_root, '.travis.yml'), 'w') as fd:
             fd.write('\n')
         with open(os.path.join(odoo_root, 'README.rst'), 'w') as fd:
             fd.write('This directory is a fake, just for test!\n')
         if retodoodir:
@@ -1500,17 +1638,17 @@
         majver = int(version.split('.')[0])
         if majver < 10:
             ffn = os.path.join(moduledir, '__openerp__.py')
             ffn_del = os.path.join(moduledir, '__manifest__.py')
         else:
             ffn = os.path.join(moduledir, '__manifest__.py')
             ffn_del = os.path.join(moduledir, '__openerp__.py')
-        with open(ffn, 'w') as fd:
+        with open(ffn, 'w', encoding="utf-8") as fd:
             fd.write(
-                str(
+                text(
                     {
                         'name': name,
                         'version': version,
                         'summary': 'This module is a fake, just for test!',
                         'depends': dependencies if dependencies else [],
                     }
                 )
```

### Comparing `zerobug-2.0.8/zerobug/zerobug.py` & `zerobug-2.0.9/zerobug/zerobug.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 """
     Zeroincombenze® unit test library for python programs Regression Test Suite
 """
 import sys
 from . import z0test
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 def version():
     return __version__
 
 
 def main(cli_args=None):
```

### Comparing `zerobug-2.0.8/zerobug.egg-info/SOURCES.txt` & `zerobug-2.0.9/zerobug.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 README.rst
 setup.py
 zerobug/__init__.py
 zerobug/__main__.py
+zerobug/py23_template.py
+zerobug/py2_template.py
+zerobug/py3_template.py
 zerobug/z0testlib.py
 zerobug/z0testrc
 zerobug/zerobug.py
 zerobug.egg-info/PKG-INFO
 zerobug.egg-info/SOURCES.txt
 zerobug.egg-info/dependency_links.txt
 zerobug.egg-info/entry_points.txt
 zerobug.egg-info/not-zip-safe
 zerobug.egg-info/requires.txt
 zerobug.egg-info/top_level.txt
 zerobug/_travis/__init__.py
+zerobug/_travis/__init__.pyc
 zerobug/_travis/build_cmd
 zerobug/_travis/travis_after_tests_success
 zerobug/_travis/travis_install_env
 zerobug/_travis/travis_run_pypi_tests
 zerobug/_travis/cfg/coveragerc
 zerobug/_travis/cfg/travis_run_flake8.cfg
 zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg
@@ -43,8 +47,17 @@
 zerobug/_travis/cfg/travis_run_shellcheck.cfg
 zerobug/_travis/cfg/travis_run_shellcheck_MINIMAL.cfg
 zerobug/_travis/cfg/travis_run_shellcheck_REDUCED.cfg
 zerobug/dummy/__init__.py
 zerobug/dummy/dummylib.py
 zerobug/scripts/__init__.py
 zerobug/scripts/main.py
-zerobug/scripts/setup.info
+zerobug/scripts/setup.info
+zerobug/tests/__init__.py
+zerobug/tests/__pytest_sample.py
+zerobug/tests/conftest.py
+zerobug/tests/dummy_01.py
+zerobug/tests/test_01_internal_version.py
+zerobug/tests/test_01_internal_version_old.py
+zerobug/tests/test_03_internal_sanity_check.py
+zerobug/tests/test_05_os_tree.py
+zerobug/tests/test_07_odoo.py
```

### Comparing `zerobug-2.0.8/zerobug.egg-info/PKG-INFO` & `zerobug-2.0.9/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,392 +1,498 @@
-Metadata-Version: 1.2
-Name: zerobug
-Version: 2.0.8
-Summary: Zeroincombenze continuous testing framework and tools for python and bash programs
-Home-page: https://github.com/zeroincombenze/tools
-Author: Antonio Maria Vigliotti
-Author-email: <info@shs-av.com>
-License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools/tree/master/zerobug
-Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io/en/latest/zerobug
-Project-URL: Changelog, https://github.com/zeroincombenze/tools/blob/master/zerobug/egg-info/CHANGELOG.rst
-Description: 
-        =============
-        zerobug 2.0.7
-        =============
-        
-        
-        
-        |Maturity| |Build Status| |Coverage Status| |license gpl|
-        
-        
-        
-        
-        Overview
-        ========
-        
-        
-        
-        
-        
-        
-        
-        
-        |
-        
-        Features
-        --------
-        
-        * Test execution log
-        * Autodiscovery test modules and functions
-        * Python 2.7+ and 3.5+
-        * coverage integration
-        * travis integration
-        
-        
-        |
-        
-        Usage
-        =====
-        
-        
-        
-        Code example
-        ------------
-        
-        *zerobug* makes avaiable following functions to test:
-        
-        |
-        
-        `Z0BUG.setup(ctx)` (python)
-        
-        `Z0BUG_setup` (bash)
-        
-        Setup for test. It is called before all tests.
-        
-        |
-        
-        `Z0BUG.teardown(ctx)` (python)
-        
-        `Z0BUG_teardown` (bash)
-        
-        Setup for test. It is called after all tests.
-        
-        |
-        
-        `Z0BUG.build_os_tree(ctx, list_of_paths)` (python)
-        
-        `Z0BUG_build_os_tree list_of_paths` (bash)
-        
-        Build a full os tree from supplied list.
-        If python, list of paths is a list of strings.
-        If bash, list is one string of paths separated by spaces.
-        Function reads list of paths and then create all directories.
-        If directory is an absolute path, it is created with the supplied path.
-        If directory is a relative path, the directory is created under "tests/res" directory.
-        
-        Warning!
-        To check is made is parent dir does not exit. Please, supply path from parent
-        to children, if you want to build a nested tree.
-        
-        ::
-        
-            # (python)
-            from zerobug import Z0BUG
-            class RegressionTest():
-        
-                def __init__(self, Z0BUG):
-                    self.Z0BUG = Z0BUG
-        
-                def test_01(self, ctx):
-                    os_tree = ['10.0',
-                               '10.0/addons',
-                               '10.0/odoo',]
-                    root = self.Z0BUG.build_os_tree(ctx, os_tree)
-        
-        ::
-        
-            # (bash)
-            Z0BUG_setup() {
-                Z0BUG_build_os_tree "10.0 10.0/addons 10.0/odoo"
-            }
-        
-        |
-        
-        `Z0BUG.remove_os_tree(ctx, list_of_paths)` (python)
-        
-        `Z0BUG_remove_os_tree list_of_paths` (bash)
-        
-        Remove a full os tree created by `build_os_tree`
-        If python, list of paths is a list of strings.
-        If bash, list is a string of paths separated by spaces.
-        Function reads list of paths and remove all directories.
-        If directory is an absolute path, the supplied path is dropped.
-        If directory is a relative path, the directory is dropped from tests/res directory.
-        
-        Warning!
-        This function remove directory and all sub-directories without any control.
-        
-        ::
-        
-            # (python)
-            from zerobug import Z0BUG
-            class RegressionTest():
-        
-                def __init__(self, Z0BUG):
-                    self.Z0BUG = Z0BUG
-        
-                def test_01(self, ctx):
-                    os_tree = ['10.0',
-                               '10.0/addons',
-                               '10.0/odoo',]
-                    root = self.Z0BUG.remove_os_tree(ctx, os_tree)
-        
-        |
-        
-        `Z0BUG.build_odoo_env(ctx, version)` (python)
-        
-        Like build_os_tree but create a specific odoo os tree.
-        
-        ::
-        
-            # (python)
-            from zerobug import Z0BUG
-            from zerobug import Z0testOdoo
-            class RegressionTest():
-        
-                def __init__(self, Z0BUG):
-                    self.Z0BUG = Z0BUG
-        
-                def test_01(self, ctx):
-                    root = Z0testOdoo.build_odoo_env(ctx, '10.0')
-        
-        |
-        
-        `Z0BUG.git_clone(remote, reponame, branch, odoo_path, force=None)` (python)
-        
-        Execute git clone of `remote:reponame:branch` into local directory `odoo_path`.
-        In local travis emulation, if repository uses local repository, if exists.
-        Return odoo root directory
-        
-        ::
-        
-            # (python)
-            from zerobug import Z0BUG
-            from zerobug import Z0testOdoo
-        
-            from zerobug import Z0BUG
-            class RegressionTest():
-        
-                def __init__(self, Z0BUG):
-                    self.Z0BUG = Z0BUG
-        
-                def test_01(self, ctx):
-                    remote = 'OCA'
-                    reponame = 'OCB'
-                    branch = '10.0'
-                    odoo_path = '/opt/odoo/10.0'
-                    Z0testOdoo.git_clone(remote, reponame, branch, odoo_path)
-        
-        
-        
-        
-        Unit test can run in package directory or in ./tests directory of package.
-        
-        Every test can inquire internal context.
-        
-        ::
-        
-            this_fqn      parent caller full qualified name (i.e. /opt/odoo/z0bug.pyc)
-            this          parent name, w/o extension (i.e. z0bug)
-            ctr           test counter [both bash and python tests]
-            dry_run       dry-run (do nothing) [opt_dry_run in bash test]          "-n"
-            esanity       True if required sanity check with echo                  "-X"
-            max_test      # of tests to execute [both bash and python tests]       "-z"
-            min_test      # of test executed before this one                       "-r"
-            on_error      behavior after error, 'continue' or 'raise' (default)
-            opt_echo      True if echo test result onto std output                 "-e"
-            opt_new       new log file [both bash and python tests]                "-N"
-            opt_noctr     do not count # tests [both bash and python tests]        "-0"
-            opt_verbose   show messages during execution                           "-v"
-            logfn         real trace log file name from switch                     "-l"
-            qsanity       True if required sanity check w/o echo                   "-x"
-            run4cover     Run tests for coverage (use coverage run rather python)  "-C"
-            python3       Execute test in python3                                  "-3"
-            run_daemon    True if execution w/o tty as stdio
-            run_on_top    Top test (not parent)
-            run_tty       Opposite of run_daemon
-            tlog          default tracelog file name
-            _run_autotest True if running auto-test
-            _parser       cmd line parser
-            _opt_obj      parser obj, to acquire optional switches
-            WLOGCMD       override opt_echo; may be None, 'echo', 'echo-1', 'echo-0'
-            Z0            this library object
-        
-        Environment read:
-        
-        DEV_ENVIRONMENT Name of package; if set test is under travis emulator control
-        
-        COVERAGE_PROCESS_START
-                        Name of coverage conf file; if set test is running for coverage
-        
-        
-        
-        |
-        |
-        
-        Getting started
-        ===============
-        
-        
-        Installation
-        ------------
-        
-        Zeroincombenze tools require:
-        
-        * Linux Centos 7/8 or Debian 9/10 or Ubuntu 18/20/22
-        * python 2.7+, some tools require python 3.6+
-        * bash 5.0+
-        
-        Stable version via Python Package
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            pip install zerobug
-        
-        |
-        
-        Current version via Git
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            cd $HOME
-            git clone https://github.com/zeroincombenze/tools.git
-            cd ./tools
-            ./install_tools.sh -p
-            source $HOME/devel/activate_tools
-        
-        
-        Upgrade
-        -------
-        
-        Stable version via Python Package
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            pip install zerobug -U
-        
-        |
-        
-        Current version via Git
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            cd $HOME
-            ./install_tools.sh -U
-            source $HOME/devel/activate_tools
-        
-        
-        |
-        |
-        
-        Credits
-        =======
-        
-        Copyright
-        ---------
-        
-        SHS-AV s.r.l. <https://www.shs-av.com/>
-        
-        
-        Contributors
-        ------------
-        
-        * Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
-        
-        
-        
-        |
-        
-        This module is part of tools project.
-        
-        Last Update / Ultimo aggiornamento: 2023-05-21
-        
-        .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
-            :target: https://odoo-community.org/page/development-status
-            :alt: 
-        .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
-            :target: https://travis-ci.com/zeroincombenze/tools
-            :alt: github.com
-        .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
-            :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
-            :alt: License: AGPL-3
-        .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
-            :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
-            :alt: License: OPL
-        .. |Coverage Status| image:: https://coveralls.io/repos/github/zeroincombenze/tools/badge.svg?branch=master
-            :target: https://coveralls.io/github/zeroincombenze/tools?branch=2.0
-            :alt: Coverage
-        .. |Codecov Status| image:: https://codecov.io/gh/zeroincombenze/tools/branch/2.0/graph/badge.svg
-            :target: https://codecov.io/gh/zeroincombenze/tools/branch/2.0
-            :alt: Codecov
-        .. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
-            :target: https://wiki.zeroincombenze.org/en/Odoo/2.0/dev
-            :alt: Technical Documentation
-        .. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
-            :target: https://wiki.zeroincombenze.org/it/Odoo/2.0/man
-            :alt: Technical Documentation
-        .. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
-            :target: https://erp2.zeroincombenze.it
-            :alt: Try Me
-        .. |OCA Codecov| image:: https://codecov.io/gh/OCA/tools/branch/2.0/graph/badge.svg
-            :target: https://codecov.io/gh/OCA/tools/branch/2.0
-            :alt: Codecov
-        .. |Odoo Italia Associazione| image:: https://www.odoo-italia.org/images/Immagini/Odoo%20Italia%20-%20126x56.png
-           :target: https://odoo-italia.org
-           :alt: Odoo Italia Associazione
-        .. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
-           :target: https://www.zeroincombenze.it/
-           :alt: Zeroincombenze
-        .. |en| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/en_US.png
-           :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
-        .. |it| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/it_IT.png
-           :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
-        .. |check| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/check.png
-        .. |no_check| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/no_check.png
-        .. |menu| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/menu.png
-        .. |right_do| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/right_do.png
-        .. |exclamation| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/exclamation.png
-        .. |warning| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/warning.png
-        .. |same| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/same.png
-        .. |late| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/late.png
-        .. |halt| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/halt.png
-        .. |info| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/info.png
-        .. |xml_schema| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/iso/icons/xml-schema.png
-           :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/iso/scope/xml-schema.md
-        .. |DesktopTelematico| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/DesktopTelematico.png
-           :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/Desktoptelematico.md
-        .. |FatturaPA| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/fatturapa.png
-           :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/fatturapa.md
-        .. |chat_with_us| image:: https://www.shs-av.com/wp-content/chat_with_us.gif
-           :target: https://t.me/Assitenza_clienti_powERP
-        
-        
-        
-Keywords: bash,optargs
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: System :: System Shells
+
+======
+ 2.0.9
+======
+
+
+
+|Maturity| |license gpl|
+
+
+
+
+Overview
+========
+
+Zeroincombenze® continuous testing framework for python and bash programs
+-------------------------------------------------------------------------
+
+This library can run unit test of target package software.
+Supported languages are *python* (through z0testlib.py) and *bash* (through z0testrc)
+
+*zerobug* supports test automation, aggregation of tests into collections
+and independence of the tests from the reporting framework.
+The *zerobug* module provides all code that make it easy to support testing
+both for python programs both for bash scripts.
+*zerobug* shows execution test with a message like "n/tot message"
+where *n* is current unit test and *tot* is the total unit test to execute,
+that is a sort of advancing test progress.
+
+You can use z0bug_odoo that is the odoo integration to test Odoo modules.
+
+*zerobug* is built on follow concepts:
+
+* test main - it is a main program to executes all test runners
+* test runner - it is a program to executes one or more test suites
+* test suite - it is a collection of test cases
+* test case - it is a smallest unit test
+
+The main file is the command **zerobug** of this package; it searches for test runner files
+named `[id_]test_` where 'id' is the shor name of testing package.
+
+Test suite is a collection of test case named `test_[0-9]+` inside the runner file,
+executed in sorted order.
+
+Every suit can contains one or more test case, the smallest unit test;
+every unit test terminates with success or with failure.
+
+Because **zerobug** can show total number of unit test to execute, it runs tests
+in 2 passes. In the first pass it counts the number of test, in second pass executes really
+it. This behavior can be overridden by -0 switch.
+
+
+
+
+
+
+
+|
+
+Features
+--------
+
+* Test execution log
+* Autodiscovery test modules and functions
+* Python 2.7+ and 3.5+
+* coverage integration
+* travis integration
+
+
+|
+
+Usage
+=====
+
+::
+
+    usage: zerobug [-h] [-B] [-C] [-e] [-J] [-k] [-l file] [-N] [-n] [-O]
+                   [-p file_list] [-q] [-r number] [-s number] [-V] [-v] [-x] [-X]
+                   [-z number] [-0] [-1] [-3]
+
+    Regression test on z0bug_odoo
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      -B, --debug           trace msgs in zerobug.tracehis
+      -C, --no-coverage     run tests without coverage
+      -e, --echo            enable echoing even if not interactive tty
+      -J                    load travisrc
+      -k, --keep            keep current logfile
+      -l file, --logname file
+                            set logfile name
+      -N, --new             create new logfile
+      -n, --dry-run         count and display # unit tests
+      -O                    load odoorc
+      -p file_list, --search-pattern file_list
+                            test file pattern
+      -q, --quiet           run tests without output (quiet mode)
+      -r number, --restart number
+                            set to counted tests, 1st one next to this
+      -s number, --start number
+                            deprecated
+      -V, --version         show program's version number and exit
+      -v, --verbose         verbose mode
+      -x, --qsanity         like -X but run silently
+      -X, --esanity         execute test library sanity check and exit
+      -z number, --end number
+                            display total # tests when execute them
+      -0, --no-count        no count # unit tests
+      -1, --coverage        run tests for coverage (obsolete)
+      -3, --python3         use python3
+
+
+Code example
+------------
+
+*zerobug* makes avaiable following functions to test:
+
+|
+
+`Z0BUG.setup(ctx)` (python)
+
+`Z0BUG_setup` (bash)
+
+Setup for test. It is called before all tests.
+
+|
+
+`Z0BUG.teardown(ctx)` (python)
+
+`Z0BUG_teardown` (bash)
+
+Setup for test. It is called after all tests.
+
+|
+
+`Z0BUG.build_os_tree(ctx, list_of_paths)` (python)
+
+`Z0BUG_build_os_tree list_of_paths` (bash)
+
+Build a full os tree from supplied list.
+If python, list of paths is a list of strings.
+If bash, list is one string of paths separated by spaces.
+Function reads list of paths and then create all directories.
+If directory is an absolute path, it is created with the supplied path.
+If directory is a relative path, the directory is created under "tests/res" directory.
+
+Warning!
+To check is made is parent dir does not exit. Please, supply path from parent
+to children, if you want to build a nested tree.
+
+::
+
+    # (python)
+    from zerobug import Z0BUG
+    class RegressionTest():
+
+        def __init__(self, Z0BUG):
+            self.Z0BUG = Z0BUG
+
+        def test_01(self, ctx):
+            os_tree = ['10.0',
+                       '10.0/addons',
+                       '10.0/odoo',]
+            root = self.Z0BUG.build_os_tree(ctx, os_tree)
+
+::
+
+    # (bash)
+    Z0BUG_setup() {
+        Z0BUG_build_os_tree "10.0 10.0/addons 10.0/odoo"
+    }
+
+|
+
+`Z0BUG.remove_os_tree(ctx, list_of_paths)` (python)
+
+`Z0BUG_remove_os_tree list_of_paths` (bash)
+
+Remove a full os tree created by `build_os_tree`
+If python, list of paths is a list of strings.
+If bash, list is a string of paths separated by spaces.
+Function reads list of paths and remove all directories.
+If directory is an absolute path, the supplied path is dropped.
+If directory is a relative path, the directory is dropped from tests/res directory.
+
+Warning!
+This function remove directory and all sub-directories without any control.
+
+::
+
+    # (python)
+    from zerobug import Z0BUG
+    class RegressionTest():
+
+        def __init__(self, Z0BUG):
+            self.Z0BUG = Z0BUG
+
+        def test_01(self, ctx):
+            os_tree = ['10.0',
+                       '10.0/addons',
+                       '10.0/odoo',]
+            root = self.Z0BUG.remove_os_tree(ctx, os_tree)
+
+|
+
+`Z0BUG.build_odoo_env(ctx, version)` (python)
+
+Like build_os_tree but create a specific odoo os tree.
+
+::
+
+    # (python)
+    from zerobug import Z0BUG
+    from zerobug import Z0testOdoo
+    class RegressionTest():
+
+        def __init__(self, Z0BUG):
+            self.Z0BUG = Z0BUG
+
+        def test_01(self, ctx):
+            root = Z0testOdoo.build_odoo_env(ctx, '10.0')
+
+|
+
+`Z0BUG.git_clone(remote, reponame, branch, odoo_path, force=None)` (python)
+
+Execute git clone of `remote:reponame:branch` into local directory `odoo_path`.
+In local travis emulation, if repository uses local repository, if exists.
+Return odoo root directory
+
+::
+
+    # (python)
+    from zerobug import Z0BUG
+    from zerobug import Z0testOdoo
+
+    from zerobug import Z0BUG
+    class RegressionTest():
+
+        def __init__(self, Z0BUG):
+            self.Z0BUG = Z0BUG
+
+        def test_01(self, ctx):
+            remote = 'OCA'
+            reponame = 'OCB'
+            branch = '10.0'
+            odoo_path = '/opt/odoo/10.0'
+            Z0testOdoo.git_clone(remote, reponame, branch, odoo_path)
+
+
+
+
+Unit test can run in package directory or in ./tests directory of package.
+
+Every test can inquire internal context.
+
+::
+
+    this_fqn      parent caller full qualified name (i.e. /opt/odoo/z0bug.pyc)
+    this          parent name, w/o extension (i.e. z0bug)
+    ctr           test counter [both bash and python tests]
+    dry_run       dry-run (do nothing) [opt_dry_run in bash test]          "-n"
+    esanity       True if required sanity check with echo                  "-X"
+    max_test      # of tests to execute [both bash and python tests]       "-z"
+    min_test      # of test executed before this one                       "-r"
+    on_error      behavior after error, 'continue' or 'raise' (default)
+    opt_echo      True if echo test result onto std output                 "-e"
+    opt_new       new log file [both bash and python tests]                "-N"
+    opt_noctr     do not count # tests [both bash and python tests]        "-0"
+    opt_verbose   show messages during execution                           "-v"
+    logfn         real trace log file name from switch                     "-l"
+    qsanity       True if required sanity check w/o echo                   "-x"
+    run4cover     Run tests for coverage (use coverage run rather python)  "-C"
+    python3       Execute test in python3                                  "-3"
+    run_daemon    True if execution w/o tty as stdio
+    run_on_top    Top test (not parent)
+    run_tty       Opposite of run_daemon
+    tlog          default tracelog file name
+    _run_autotest True if running auto-test
+    _parser       cmd line parser
+    _opt_obj      parser obj, to acquire optional switches
+    WLOGCMD       override opt_echo; may be None, 'echo', 'echo-1', 'echo-0'
+    Z0            this library object
+
+Environment read:
+
+DEV_ENVIRONMENT Name of package; if set test is under travis emulator control
+
+COVERAGE_PROCESS_START
+                Name of coverage conf file; if set test is running for coverage
+
+
+
+|
+|
+
+Getting started
+===============
+
+
+Installation
+------------
+
+Zeroincombenze tools require:
+
+* Linux Centos 7/8 or Debian 9/10 or Ubuntu 18/20/22
+* python 2.7+, some tools require python 3.6+
+* bash 5.0+
+
+Stable version via Python Package
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    pip install 
+
+|
+
+Current version via Git
+~~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    cd $HOME
+    git clone https://github.com/zeroincombenze/tools.git
+    cd ./tools
+    ./install_tools.sh -p
+    source $HOME/devel/activate_tools
+
+
+Upgrade
+-------
+
+Stable version via Python Package
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    pip install  -U
+
+|
+
+Current version via Git
+~~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    cd $HOME
+    ./install_tools.sh -U
+    source $HOME/devel/activate_tools
+
+
+History
+-------
+
+2.0.9 (2023-07-12)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] zerobug implementation with unittest
+* [FIX] z0testlib.py: build_odoo_env, odoo-bin / openerp-server are executable
+* [FIX] z0testlib.py: minor fixes
+
+2.0.7 (2023-05-14)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] travis_run_pypi_tests: new switch -p PATTERN
+
+2.0.6 (2023-05-08)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] Now all_tests is ignored
+* [IMP] Build Odoo environment for Odoo 16.0
+
+2.0.5 (2023-03-24)
+~~~~~~~~~~~~~~~~~~
+
+* [FIX] travis_install_env: ensure list_requirements is executable
+* [IMP] flake8 configuration
+* [IMP] coveralls and codecov are not more dependencies
+* [IMP] Test for Odoo 16.0
+
+2.0.4 (2022-12-08)
+~~~~~~~~~~~~~~~~~~
+
+* [FIX] run_pypi_test: best recognition of python version
+* [FIX] build_cmd: best recognition of python version
+* [FIX] travis_install_env: ensure coverage version
+* [IMP] odoo environment to test more precise
+
+2.0.3 (2022-11-08)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] npm management
+
+2.0.2.1 (2022-10-31)
+~~~~~~~~~~~~~~~~~~~~
+
+* [FIX] Odoo 11.0+
+* [FIX] Ensure coverage 5.0+
+
+2.0.2 (2022-10-20)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] Stable version
+
+2.0.1.1 (2022-10-12)
+~~~~~~~~~~~~~~~~~~~~
+
+* [IMP] minor improvements
+
+2.0.1 (2022-10-12)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] stable version
+
+2.0.0.2 (2022-10-05)
+~~~~~~~~~~~~~~~~~~~~
+
+* [IMP] travis_install_env: python2 tests
+
+2.0.0.1 (2022-09-06)
+~~~~~~~~~~~~~~~~~~~~
+
+* [FIX] travis_install_env: minor fixes
+* [IMP] z0testlib: show coverage result
+
+
+
+
+|
+|
+
+Credits
+=======
+
+Copyright
+---------
+
+SHS-AV s.r.l. <https://www.shs-av.com/>
+
+
+Contributors
+------------
+
+* Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
+
+
+|
+
+This module is part of  project.
+
+Last Update / Ultimo aggiornamento: 
+
+.. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
+    :target: https://odoo-community.org/page/development-status
+    :alt: 
+.. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
+    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+    :alt: License: AGPL-3
+.. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
+    :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
+    :alt: License: OPL
+.. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
+    :target: https://wiki.zeroincombenze.org/en/Odoo/2.0/dev
+    :alt: Technical Documentation
+.. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
+    :target: https://wiki.zeroincombenze.org/it/Odoo/2.0/man
+    :alt: Technical Documentation
+.. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
+    :target: https://erp2.zeroincombenze.it
+    :alt: Try Me
+.. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
+   :target: https://www.zeroincombenze.it/
+   :alt: Zeroincombenze
+.. |en| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/en_US.png
+   :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
+.. |it| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/it_IT.png
+   :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
+.. |check| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/check.png
+.. |no_check| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/no_check.png
+.. |menu| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/menu.png
+.. |right_do| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/right_do.png
+.. |exclamation| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/exclamation.png
+.. |warning| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/warning.png
+.. |same| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/same.png
+.. |late| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/late.png
+.. |halt| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/halt.png
+.. |info| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/info.png
+.. |xml_schema| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/iso/icons/xml-schema.png
+   :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/iso/scope/xml-schema.md
+.. |DesktopTelematico| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/DesktopTelematico.png
+   :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/Desktoptelematico.md
+.. |FatturaPA| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/fatturapa.png
+   :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/fatturapa.md
+.. |chat_with_us| image:: https://www.shs-av.com/wp-content/chat_with_us.gif
+   :target: https://t.me/Assitenza_clienti_powERP
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zerobug-2.0.8/setup.py` & `zerobug-2.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# -*- coding: utf-8 -*-
+import os.path as pth
 import sys
 
 from setuptools import find_packages, setup
 
 author = "Antonio Maria Vigliotti"
 author_email = "<info@shs-av.com>"
 source_url = "https://github.com/zeroincombenze/tools/tree/master/zerobug"
@@ -33,18 +35,18 @@
             'os0',
             'z0lib',
         ],
     )
 
 setup(
     name='zerobug',
-    version='2.0.8',
+    version='2.0.9',
     description='Zeroincombenze continuous testing framework'
     ' and tools for python and bash programs',
-    long_description=open("README.rst").read(),
+    long_description=open(pth.join(pth.dirname(__file__), "README.rst")).read(),
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

