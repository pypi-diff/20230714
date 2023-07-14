# Comparing `tmp/cs_util-0.0.3.tar.gz` & `tmp/cs_util-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cs_util-0.0.3.tar", last modified: Thu Feb 16 15:45:12 2023, max compression
+gzip compressed data, was "/home/mkilbing/astro/repositories/github/cs_util/dist/.tmp-no9cbwk0/cs_util-0.0.4.tar", last modified: Fri Jul 14 14:01:59 2023, max compression
```

## Comparing `cs_util-0.0.3.tar` & `cs_util-0.0.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-02-16 15:45:12.850528 cs_util-0.0.3/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       73 2022-09-28 15:28:14.000000 cs_util-0.0.3/.coveragerc
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-02-16 15:45:12.794528 cs_util-0.0.3/.github/
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-02-16 15:45:12.811528 cs_util-0.0.3/.github/workflows/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2195 2022-09-28 15:31:29.000000 cs_util-0.0.3/.github/workflows/cd-build.yml
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2945 2022-09-28 15:31:29.000000 cs_util-0.0.3/.github/workflows/ci-build.yml
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2237 2022-10-19 08:52:59.000000 cs_util-0.0.3/.gitignore
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       41 2022-09-28 15:28:14.000000 cs_util-0.0.3/.pylintrc
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      245 2022-09-28 15:28:14.000000 cs_util-0.0.3/.pyup.yml
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3219 2022-09-28 15:28:14.000000 cs_util-0.0.3/CODE_OF_CONDUCT.md
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      115 2022-09-28 15:28:14.000000 cs_util-0.0.3/CONTRIBUTING.md
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1073 2022-09-28 15:31:29.000000 cs_util-0.0.3/LICENCE.txt
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      113 2022-09-28 15:28:14.000000 cs_util-0.0.3/MANIFEST.in
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2985 2023-02-16 15:45:12.850528 cs_util-0.0.3/PKG-INFO
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2231 2022-10-11 12:54:32.000000 cs_util-0.0.3/README.md
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-02-16 15:45:12.818528 cs_util-0.0.3/cs_util/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1140 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/__init__.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1397 2022-10-08 12:05:07.000000 cs_util-0.0.3/cs_util/calc.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3208 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/canfar.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     4329 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/cat.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2307 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/cfis.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     5765 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/cosmo.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1507 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/logging.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     6755 2023-02-15 13:50:35.000000 cs_util-0.0.3/cs_util/plots.py
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-02-16 15:45:12.830528 cs_util-0.0.3/cs_util/tests/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       61 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/tests/__init__.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1512 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/tests/test_calc.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1036 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/tests/test_canfar.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2380 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/tests/test_cat.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3756 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/tests/test_cfis.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     7125 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/tests/test_cosmo.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2707 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/tests/test_logging.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2356 2023-02-16 15:20:29.000000 cs_util-0.0.3/cs_util/tests/test_plots.py
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-02-16 15:45:12.822528 cs_util-0.0.3/cs_util.egg-info/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2985 2023-02-16 15:45:12.000000 cs_util-0.0.3/cs_util.egg-info/PKG-INFO
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1267 2023-02-16 15:45:12.000000 cs_util-0.0.3/cs_util.egg-info/SOURCES.txt
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)        1 2023-02-16 15:45:12.000000 cs_util-0.0.3/cs_util.egg-info/dependency_links.txt
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      263 2023-02-16 15:45:12.000000 cs_util-0.0.3/cs_util.egg-info/requires.txt
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       16 2023-02-16 15:45:12.000000 cs_util-0.0.3/cs_util.egg-info/top_level.txt
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       70 2022-10-16 16:28:42.000000 cs_util-0.0.3/develop.txt
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-02-16 15:45:12.831528 cs_util-0.0.3/docs/
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-02-16 15:45:12.834528 cs_util-0.0.3/docs/_script_templates/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      174 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/_script_templates/module.rst_t
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1070 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/_script_templates/package.rst_t
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      128 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/_script_templates/toc.rst_t
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-02-16 15:45:12.837528 cs_util-0.0.3/docs/_templates/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      174 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/_templates/module.rst_t
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1060 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/_templates/package.rst_t
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      128 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/_templates/toc.rst_t
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      138 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/requirements.txt
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-02-16 15:45:12.847528 cs_util-0.0.3/docs/source/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      119 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/source/about.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      318 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/source/citing.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     7015 2023-02-16 15:20:29.000000 cs_util-0.0.3/docs/source/conf.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      422 2022-09-28 15:31:29.000000 cs_util-0.0.3/docs/source/contributing.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      811 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/source/index.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      680 2022-09-28 15:31:29.000000 cs_util-0.0.3/docs/source/installation.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      120 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/source/my_ref.bib
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      262 2022-09-28 15:31:29.000000 cs_util-0.0.3/docs/source/quickstart.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2743 2023-02-16 15:20:29.000000 cs_util-0.0.3/docs/source/refs.bib
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      395 2022-10-16 16:56:43.000000 cs_util-0.0.3/docs/source/toc.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       67 2022-09-28 15:28:14.000000 cs_util-0.0.3/docs/source/z_ref.rst
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      117 2022-10-16 17:46:09.000000 cs_util-0.0.3/environment.yml
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       44 2023-02-16 15:20:29.000000 cs_util-0.0.3/requirements.txt
-drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-02-16 15:45:12.849528 cs_util-0.0.3/scripts/
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      628 2022-09-28 15:28:14.000000 cs_util-0.0.3/scripts/__init__.py
--rwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)     2327 2022-09-28 15:31:29.000000 cs_util-0.0.3/scripts/example_script.py
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      403 2023-02-16 15:45:12.851528 cs_util-0.0.3/setup.cfg
--rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2304 2023-02-16 15:45:05.000000 cs_util-0.0.3/setup.py
+drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-07-14 14:01:58.998960 cs_util-0.0.4/
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       73 2022-09-28 15:28:14.000000 cs_util-0.0.4/.coveragerc
+drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-07-14 14:01:58.944960 cs_util-0.0.4/.github/
+drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-07-14 14:01:58.960960 cs_util-0.0.4/.github/workflows/
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2195 2022-09-28 15:31:29.000000 cs_util-0.0.4/.github/workflows/cd-build.yml
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2945 2022-09-28 15:31:29.000000 cs_util-0.0.4/.github/workflows/ci-build.yml
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2237 2022-10-19 08:52:59.000000 cs_util-0.0.4/.gitignore
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       41 2022-09-28 15:28:14.000000 cs_util-0.0.4/.pylintrc
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      245 2022-09-28 15:28:14.000000 cs_util-0.0.4/.pyup.yml
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3219 2022-09-28 15:28:14.000000 cs_util-0.0.4/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      115 2022-09-28 15:28:14.000000 cs_util-0.0.4/CONTRIBUTING.md
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1073 2022-09-28 15:31:29.000000 cs_util-0.0.4/LICENCE.txt
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      113 2022-09-28 15:28:14.000000 cs_util-0.0.4/MANIFEST.in
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3503 2023-07-14 14:01:58.997960 cs_util-0.0.4/PKG-INFO
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2467 2023-06-21 12:32:56.000000 cs_util-0.0.4/README.md
+drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-07-14 14:01:58.967960 cs_util-0.0.4/cs_util/
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      869 2023-06-27 09:27:52.000000 cs_util-0.0.4/cs_util/__init__.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1020 2023-06-21 12:37:12.000000 cs_util-0.0.4/cs_util/calc.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3176 2023-06-27 09:27:52.000000 cs_util-0.0.4/cs_util/canfar.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     5102 2023-06-27 09:27:52.000000 cs_util-0.0.4/cs_util/cat.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2306 2023-06-27 09:27:52.000000 cs_util-0.0.4/cs_util/cfis.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     5821 2023-06-27 09:27:52.000000 cs_util-0.0.4/cs_util/cosmo.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1504 2023-06-21 12:32:56.000000 cs_util-0.0.4/cs_util/logging.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     6982 2023-06-27 09:27:52.000000 cs_util-0.0.4/cs_util/plots.py
+drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-07-14 14:01:58.978960 cs_util-0.0.4/cs_util/tests/
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       61 2023-06-21 12:32:56.000000 cs_util-0.0.4/cs_util/tests/__init__.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1522 2023-06-27 09:27:52.000000 cs_util-0.0.4/cs_util/tests/test_calc.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1032 2023-06-21 12:37:12.000000 cs_util-0.0.4/cs_util/tests/test_canfar.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2647 2023-06-27 09:27:52.000000 cs_util-0.0.4/cs_util/tests/test_cat.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3731 2023-06-27 09:27:52.000000 cs_util-0.0.4/cs_util/tests/test_cfis.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     7051 2023-06-27 09:27:52.000000 cs_util-0.0.4/cs_util/tests/test_cosmo.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3142 2023-06-27 09:27:52.000000 cs_util-0.0.4/cs_util/tests/test_logging.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2314 2023-06-21 12:32:56.000000 cs_util-0.0.4/cs_util/tests/test_plots.py
+drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-07-14 14:01:58.971960 cs_util-0.0.4/cs_util.egg-info/
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     3503 2023-07-14 14:01:58.000000 cs_util-0.0.4/cs_util.egg-info/PKG-INFO
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1263 2023-07-14 14:01:58.000000 cs_util-0.0.4/cs_util.egg-info/SOURCES.txt
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)        1 2023-07-14 14:01:58.000000 cs_util-0.0.4/cs_util.egg-info/dependency_links.txt
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      210 2023-07-14 14:01:58.000000 cs_util-0.0.4/cs_util.egg-info/requires.txt
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)        8 2023-07-14 14:01:58.000000 cs_util-0.0.4/cs_util.egg-info/top_level.txt
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       70 2022-10-16 16:28:42.000000 cs_util-0.0.4/develop.txt
+drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-07-14 14:01:58.979960 cs_util-0.0.4/docs/
+drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-07-14 14:01:58.982960 cs_util-0.0.4/docs/_script_templates/
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      174 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/_script_templates/module.rst_t
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1070 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/_script_templates/package.rst_t
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      128 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/_script_templates/toc.rst_t
+drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-07-14 14:01:58.985960 cs_util-0.0.4/docs/_templates/
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      174 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/_templates/module.rst_t
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1060 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/_templates/package.rst_t
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      128 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/_templates/toc.rst_t
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      138 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/requirements.txt
+drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-07-14 14:01:58.995960 cs_util-0.0.4/docs/source/
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      119 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/source/about.rst
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      318 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/source/citing.rst
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     7060 2023-06-27 09:09:58.000000 cs_util-0.0.4/docs/source/conf.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      422 2022-09-28 15:31:29.000000 cs_util-0.0.4/docs/source/contributing.rst
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      811 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/source/index.rst
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      680 2022-09-28 15:31:29.000000 cs_util-0.0.4/docs/source/installation.rst
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      120 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/source/my_ref.bib
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      262 2022-09-28 15:31:29.000000 cs_util-0.0.4/docs/source/quickstart.rst
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     2743 2023-06-21 12:32:56.000000 cs_util-0.0.4/docs/source/refs.bib
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      395 2022-10-16 16:56:43.000000 cs_util-0.0.4/docs/source/toc.rst
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       67 2022-09-28 15:28:14.000000 cs_util-0.0.4/docs/source/z_ref.rst
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      117 2022-10-16 17:46:09.000000 cs_util-0.0.4/environment.yml
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)     1763 2023-07-14 07:30:57.000000 cs_util-0.0.4/pyproject.toml
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       44 2023-06-21 12:32:56.000000 cs_util-0.0.4/requirements.txt
+drwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)        0 2023-07-14 14:01:58.997960 cs_util-0.0.4/scripts/
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)      628 2022-09-28 15:28:14.000000 cs_util-0.0.4/scripts/__init__.py
+-rwxrwxr-x   0 mkilbing  (1016) mkilbing  (1016)     2359 2023-06-21 12:32:56.000000 cs_util-0.0.4/scripts/example_script.py
+-rw-rw-r--   0 mkilbing  (1016) mkilbing  (1016)       38 2023-07-14 14:01:58.998960 cs_util-0.0.4/setup.cfg
```

### Comparing `cs_util-0.0.3/.github/workflows/cd-build.yml` & `cs_util-0.0.4/.github/workflows/cd-build.yml`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.3/.github/workflows/ci-build.yml` & `cs_util-0.0.4/.github/workflows/ci-build.yml`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.3/.gitignore` & `cs_util-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.3/CODE_OF_CONDUCT.md` & `cs_util-0.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.3/LICENCE.txt` & `cs_util-0.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.3/PKG-INFO` & `cs_util-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: cs_util
-Version: 0.0.3
-Summary: Utility library for CosmoStat
-Home-page: https://github.com/martinkilbinger/cs_util
-Author: Martin Kilbinger
-Author-email: martin.kilbinger@cea.fr
-License: MIT
+Version: 0.0.4
+Author: The CosmoStat Lab
+Maintainer-email: Martin Kilbinger <martin.kilbinger@cea.fr>
+Project-URL: Source, https://github.com/CosmoStat/cs_util
+Project-URL: Documentation, https://github.com/CosmoStat/cs_util
+Project-URL: Tracker, https://github.com/CosmoStat/cs_util/issues
+Keywords: CosmoStat,cosmology,weak gravitational lensing
+Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.6
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: develop
+Provides-Extra: lint
+Provides-Extra: release
+Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENCE.txt
 
 # cs_util package
 
 Utility library for CosmoStat
 
 | Usage | Development | Release |
@@ -40,8 +45,14 @@
 
 
 
 ## Contents
 
 ### Library
 
-### Scripts
+- Galaxy catalogue handling
+- Weak-lensing related cosmological quantities (e.g. surface mass density)
+- VOS (Virtual Observatory Software)
+- Command line logging
+- Plotting
+- Basic statistic calculations
+- UNIONS/CFIS weak-lensing survey handling
```

#### html2text {}

```diff
@@ -1,38 +1,45 @@
-Metadata-Version: 2.1 Name: cs_util Version: 0.0.3 Summary: Utility library for
-CosmoStat Home-page: https://github.com/martinkilbinger/cs_util Author: Martin
-Kilbinger Author-email: martin.kilbinger@cea.fr License: MIT Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: develop License-File: LICENCE.txt #
-cs_util package Utility library for CosmoStat | Usage | Development | Release |
-| ----- | ----------- | ------- | | [![docs](https://img.shields.io/badge/docs-
-Sphinx-blue)](https://martinkilbinger.github.io/cs_util/) | [![build](https://
-github.com/martinkilbinger/cs_util/workflows/CI/badge.svg)](https://github.com/
-martinkilbinger/cs_util/actions?query=workflow%3ACI) | [![release](https://
-img.shields.io/github/v/release/martinkilbinger/cs_util)](https://github.com/
-martinkilbinger/cs_util/releases/latest) | | [![license](https://
-img.shields.io/github/license/martinkilbinger/cs_util)](https://github.com/
-martinkilbinger/cs_util/blob/master/LICENCE.txt) | [![deploy](https://
-github.com/martinkilbinger/cs_util/workflows/CD/badge.svg)](https://github.com/
-martinkilbinger/cs_util/actions?query=workflow%3ACD) | [![pypi](https://
-img.shields.io/pypi/v/cs_util)](https://pypi.org/project/cs_util/) | | [!
-[wemake-python-styleguide](https://img.shields.io/badge/style-wemake-
-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide) | [!
-[codecov](https://codecov.io/gh/martinkilbinger/cs_util/branch/master/graph/
-badge.svg?token=XHJIQXV7AX)](https://codecov.io/gh/martinkilbinger/cs_util) |
-[![python](https://img.shields.io/pypi/pyversions/cs_util)](https://
-www.python.org/downloads/source/) | | [![contribute](https://img.shields.io/
-badge/contribute-read-lightgrey)](https://github.com/martinkilbinger/cs_util/
-blob/master/CONTRIBUTING.md) | [![CodeFactor](https://www.codefactor.io/
-repository/github/martinkilbinger/cs_util/badge)](https://www.codefactor.io/
-repository/github/martinkilbinger/cs_util) | | | [![coc](https://
-img.shields.io/badge/conduct-read-lightgrey)](https://github.com/
-martinkilbinger/cs_util/blob/master/CODE_OF_CONDUCT.md) | [![Updates](https://
-pyup.io/repos/github/martinkilbinger/cs_util/shield.svg)](https://pyup.io/
-repos/github/martinkilbinger/cs_util/) | | --- > Author: Martin_Kilbinger >
-Email: martin.kilbinger@cea.fr > Year: 2022 --- ## Contents ### Library ###
-Scripts
+Metadata-Version: 2.1 Name: cs_util Version: 0.0.4 Author: The CosmoStat Lab
+Maintainer-email: Martin Kilbinger
+kilbinger@cea.fr> Project-URL: Source, https://github.com/CosmoStat/cs_util
+Project-URL: Documentation, https://github.com/CosmoStat/cs_util Project-URL:
+Tracker, https://github.com/CosmoStat/cs_util/issues Keywords:
+CosmoStat,cosmology,weak gravitational lensing Classifier: Development Status
+:: 1 - Planning Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Operating System :: POSIX :: Linux Classifier:
+Operating System :: MacOS Classifier: Topic :: Scientific/Engineering Requires-
+Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: lint
+Provides-Extra: release Provides-Extra: test Provides-Extra: dev License-File:
+LICENCE.txt # cs_util package Utility library for CosmoStat | Usage |
+Development | Release | | ----- | ----------- | ------- | | [![docs](https://
+img.shields.io/badge/docs-Sphinx-blue)](https://martinkilbinger.github.io/
+cs_util/) | [![build](https://github.com/martinkilbinger/cs_util/workflows/CI/
+badge.svg)](https://github.com/martinkilbinger/cs_util/
+actions?query=workflow%3ACI) | [![release](https://img.shields.io/github/v/
+release/martinkilbinger/cs_util)](https://github.com/martinkilbinger/cs_util/
+releases/latest) | | [![license](https://img.shields.io/github/license/
+martinkilbinger/cs_util)](https://github.com/martinkilbinger/cs_util/blob/
+master/LICENCE.txt) | [![deploy](https://github.com/martinkilbinger/cs_util/
+workflows/CD/badge.svg)](https://github.com/martinkilbinger/cs_util/
+actions?query=workflow%3ACD) | [![pypi](https://img.shields.io/pypi/v/cs_util)]
+(https://pypi.org/project/cs_util/) | | [![wemake-python-styleguide](https://
+img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-
+services/wemake-python-styleguide) | [![codecov](https://codecov.io/gh/
+martinkilbinger/cs_util/branch/master/graph/badge.svg?token=XHJIQXV7AX)](https:
+//codecov.io/gh/martinkilbinger/cs_util) | [![python](https://img.shields.io/
+pypi/pyversions/cs_util)](https://www.python.org/downloads/source/) | | [!
+[contribute](https://img.shields.io/badge/contribute-read-lightgrey)](https://
+github.com/martinkilbinger/cs_util/blob/master/CONTRIBUTING.md) | [!
+[CodeFactor](https://www.codefactor.io/repository/github/martinkilbinger/
+cs_util/badge)](https://www.codefactor.io/repository/github/martinkilbinger/
+cs_util) | | | [![coc](https://img.shields.io/badge/conduct-read-lightgrey)]
+(https://github.com/martinkilbinger/cs_util/blob/master/CODE_OF_CONDUCT.md) |
+[![Updates](https://pyup.io/repos/github/martinkilbinger/cs_util/shield.svg)]
+(https://pyup.io/repos/github/martinkilbinger/cs_util/) | | --- > Author:
+Martin_Kilbinger > Email: martin.kilbinger@cea.fr > Year: 2022 --- ## Contents
+### Library - Galaxy catalogue handling - Weak-lensing related cosmological
+quantities (e.g. surface mass density) - VOS (Virtual Observatory Software) -
+Command line logging - Plotting - Basic statistic calculations - UNIONS/CFIS
+weak-lensing survey handling
```

### Comparing `cs_util-0.0.3/README.md` & `cs_util-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,8 +18,14 @@
 
 
 
 ## Contents
 
 ### Library
 
-### Scripts
+- Galaxy catalogue handling
+- Weak-lensing related cosmological quantities (e.g. surface mass density)
+- VOS (Virtual Observatory Software)
+- Command line logging
+- Plotting
+- Basic statistic calculations
+- UNIONS/CFIS weak-lensing survey handling
```

#### html2text {}

```diff
@@ -20,9 +20,12 @@
 blob/master/CONTRIBUTING.md) | [![CodeFactor](https://www.codefactor.io/
 repository/github/martinkilbinger/cs_util/badge)](https://www.codefactor.io/
 repository/github/martinkilbinger/cs_util) | | | [![coc](https://
 img.shields.io/badge/conduct-read-lightgrey)](https://github.com/
 martinkilbinger/cs_util/blob/master/CODE_OF_CONDUCT.md) | [![Updates](https://
 pyup.io/repos/github/martinkilbinger/cs_util/shield.svg)](https://pyup.io/
 repos/github/martinkilbinger/cs_util/) | | --- > Author: Martin_Kilbinger >
-Email: martin.kilbinger@cea.fr > Year: 2022 --- ## Contents ### Library ###
-Scripts
+Email: martin.kilbinger@cea.fr > Year: 2022 --- ## Contents ### Library -
+Galaxy catalogue handling - Weak-lensing related cosmological quantities (e.g.
+surface mass density) - VOS (Virtual Observatory Software) - Command line
+logging - Plotting - Basic statistic calculations - UNIONS/CFIS weak-lensing
+survey handling
```

### Comparing `cs_util-0.0.3/cs_util/__init__.py` & `cs_util-0.0.4/cs_util/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """cs_util PACKAGE.
 
-Provide a basic description of what your package contains.
+CosmoStat utilities for weak lensing and cosmology.
 
 References
 ----------
 This package makes use of the following third-party packages:
 
 - `Matplotlib <https://matplotlib.org/>`_ :cite:`Hunter:2007`
 - `Numpy <https://numpy.org/>`_ :cite:`Harris:2020`
@@ -19,18 +19,8 @@
     supressed in this module to allow the defintion of a package
     ``__version__``, which is standard for most Python packages.
 
 """
 
 from warnings import warn
 
-from importlib_metadata import version
-
-try:
-    _version = version('cs_util')
-except Exception:  # pragma: no cover
-    _version = 'Unkown'
-    warn(
-        'Could not extract package metadata. Make sure the package is '
-        + 'correctly installed.',
-    )
-__version__ = _version
+__version__ = "0.0.4"
```

### Comparing `cs_util-0.0.3/cs_util/calc.py` & `cs_util-0.0.4/cs_util/calc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""CALC.                                                                       
-                                                                                
-:Name: calc.py                                                                 
-                                                                                
+"""CALC.
+
+:Name: calc.py
+
 :Description: This file contains methods for general calculations
               and statistics.
-                                                                                
+
 :Author: Martin Kilbinger <martin.kilbinger@cea.fr>
 
 """
 
 import numpy as np
 
 
@@ -32,14 +32,14 @@
     tuple :
         weighted average and weighted standard deviation
 
     """
     average = np.average(values, weights=weights)
 
     # Fast and numerically precise:
-    variance = np.average((values-average)**2, weights=weights)
-    
+    variance = np.average((values - average) ** 2, weights=weights)
+
     if corrected:
         n = len(values)
-        variance  = variance * n / (n - 1)
+        variance = variance * n / (n - 1)
 
     return average, np.sqrt(variance)
```

### Comparing `cs_util-0.0.3/cs_util/canfar.py` & `cs_util-0.0.4/cs_util/canfar.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     ----------
     command : str
         VOS command name
 
     """
 
     def __init__(self, command):
-
         self._avail_commands = tuple(vosc.__all__)
         self.command = command
 
     @property
     def command(self):
         """Set Command.
 
@@ -54,18 +53,17 @@
             if value is not valid vos command
 
         """
         return self._command
 
     @command.setter
     def command(self, value):
-
         if value not in self._avail_commands:
             raise ValueError(
-                f'vos command must be one of {self._avail_commands}'
+                f"vos command must be one of {self._avail_commands}"
             )
 
         self._command = getattr(vosc, value)
 
     def __call__(self, *args, **kwargs):
         """Call Method.
 
@@ -77,17 +75,15 @@
             if error in vos command occurs
 
         """
         try:
             self._command()
 
         except Exception:
-            raise vosError(
-                f'Error in VOs command: {self._command.__name__}'
-            )
+            raise vosError(f"Error in VOs command: {self._command.__name__}")
 
 
 def download(source, target, verbose=False):
     """Download.
 
     Download file from vos.
 
@@ -102,28 +98,28 @@
 
     Returns
     -------
     status : bool
         status, True/False or success/failure
 
     """
-    cmd = 'vcp'
+    cmd = "vcp"
 
     if not os.path.exists(target):
         sys.argv = [cmd, source, target]
         if verbose:
-            print(f'Downloading file {source} to {target}...')
+            print(f"Downloading file {source} to {target}...")
         vcp = vosHandler(cmd)
 
         vcp()
         if verbose:
-            print('Download finished.')
+            print("Download finished.")
     else:
         if verbose:
-            print(f'Target file {target} exists, skipping download.')
+            print(f"Target file {target} exists, skipping download.")
 
 
 def dir_list(path, verbose=False):
     """Set Directory List.
 
     List content of path on vos.
 
@@ -141,26 +137,26 @@
 
     Returns
     -------
     list
         file or directory at path, type is str
 
     """
-    cmd = 'vls'
+    cmd = "vls"
     sys.argv = [cmd, path]
     vls = vosHandler(cmd)
 
     if verbose:
-        print('Getting vos directory content from vls...')
+        print("Getting vos directory content from vls...")
 
     f = StringIO()
 
     try:
         with redirect_stdout(f):
             vls()
     except Exception:
-        print('Error during vls command')
+        print("Error during vls command")
         raise
 
     vls_out = f.getvalue()
 
-    return vls_out.split('\n')
+    return vls_out.split("\n")
```

### Comparing `cs_util-0.0.3/cs_util/cat.py` & `cs_util-0.0.4/cs_util/cat.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 :Description: This script contains methods to read and write galaxy catalogues.
 
 :Author: Martin Kilbinger <martin.kilbinger@cea.fr>
 
 """
 
 import os
-from datetime import datetime                                                   
+from datetime import datetime
 from astropy.io import fits
+from astropy.io import ascii
 
 
-def write_header_info_sp(primary_header, name='unknown', version='unknown'):
+def write_header_info_sp(primary_header, name="unknown", version="unknown"):
     """Write Header Info sp_validation.
 
     Write information about software and run to FITS header
 
     Parameters
     ----------
     primary_header : dict
@@ -29,24 +30,24 @@
 
     Returns
     -------
     dict
         updated FITS header information
 
     """
-    if 'USER' in os.environ:
-        author = os.environ['USER']
+    if "USER" in os.environ:
+        author = os.environ["USER"]
     else:
-        author = 'unknown'
-    primary_header['AUTHOR'] = (author, 'Who ran the software')
-    primary_header['SOFTNAME'] = (name, 'Name of the software')
-    primary_header['SOFTVERS'] = (version, 'Version of the software')
-    primary_header['DATE'] = (
-        datetime.now().strftime('%Y-%m-%d_%H-%M-%S'),
-        'When it was started',
+        author = "unknown"
+    primary_header["AUTHOR"] = (author, "Who ran the software")
+    primary_header["SOFTNAME"] = (name, "Name of the software")
+    primary_header["SOFTVERS"] = (version, "Version of the software")
+    primary_header["DATE"] = (
+        datetime.now().strftime("%Y-%m-%d_%H-%M-%S"),
+        "When it was started",
     )
 
     return primary_header
 
 
 def add_shear_bias_to_header(primary_header, R, R_shear, R_select, c):
     """Add Shear Bias To Header.
@@ -64,64 +65,49 @@
         shear response matrix
     R_select : 2x2-matrix
         selection response matrix
     c : 2-tuple
         additive bias
 
     """
-    primary_header['R'] = (
-        r'<R>',
-        r'Mean full response <R_shear> + <R_select>'
-    )
-    primary_header['R_11'] = (R[0, 0], 'Full response matrix comp 1 1')
-    primary_header['R_12'] = (R[0, 1], 'Full response matrix comp 1 2')
-    primary_header['R_21'] = (R[1, 0], 'Full response matrix comp 2 1')
-    primary_header['R_22'] = (R[1, 1], 'Full response matrix comp 2 2')
-
-    primary_header['R_g'] = (r'<R_g>', r'Mean shear response matrix <R_shear>')
-    primary_header['R_g11'] = (
-        R_shear[0, 0],
-        'Mean shear resp matrix comp 1 1'
-    )
-    primary_header['R_g12'] = (
-        R_shear[0, 1],
-        'Mean shear resp matrix comp 1 2'
-    )
-    primary_header['R_g21'] = (
-        R_shear[1, 0],
-        'Mean shear resp matrix comp 2 1'
-    )
-    primary_header['R_g22'] = (
-        R_shear[1, 1],
-        'Mean shear resp matrix comp 2 2'
-    )
-
-    primary_header['R_S'] = (
-        r'<R_S>',
-        r'Global selection response matrix <R_select>'
+    primary_header["R"] = (r"<R>", r"Mean full response <R_shear> + <R_select>")
+    primary_header["R_11"] = (R[0, 0], "Full response matrix comp 1 1")
+    primary_header["R_12"] = (R[0, 1], "Full response matrix comp 1 2")
+    primary_header["R_21"] = (R[1, 0], "Full response matrix comp 2 1")
+    primary_header["R_22"] = (R[1, 1], "Full response matrix comp 2 2")
+
+    primary_header["R_g"] = (r"<R_g>", r"Mean shear response matrix <R_shear>")
+    primary_header["R_g11"] = (R_shear[0, 0], "Mean shear resp matrix comp 1 1")
+    primary_header["R_g12"] = (R_shear[0, 1], "Mean shear resp matrix comp 1 2")
+    primary_header["R_g21"] = (R_shear[1, 0], "Mean shear resp matrix comp 2 1")
+    primary_header["R_g22"] = (R_shear[1, 1], "Mean shear resp matrix comp 2 2")
+
+    primary_header["R_S"] = (
+        r"<R_S>",
+        r"Global selection response matrix <R_select>",
     )
-    primary_header['R_S11'] = (
+    primary_header["R_S11"] = (
         R_select[0, 0],
-        'Global selection resp matrix comp 1 1'
+        "Global selection resp matrix comp 1 1",
     )
-    primary_header['R_S12'] = (
+    primary_header["R_S12"] = (
         R_select[0, 1],
-        'Global selection resp matrix comp 1 2'
+        "Global selection resp matrix comp 1 2",
     )
-    primary_header['R_S21'] = (
+    primary_header["R_S21"] = (
         R_select[1, 0],
-        'Global selection resp matrix comp 2 1'
+        "Global selection resp matrix comp 2 1",
     )
-    primary_header['R_S22'] = (
+    primary_header["R_S22"] = (
         R_select[1, 1],
-        'Global selection resp matrix comp 2 2'
+        "Global selection resp matrix comp 2 2",
     )
 
-    primary_header['c_1'] = (c[0], 'Additive bias 1st comp')
-    primary_header['c_2'] = (c[1], 'Additive bias 2nd comp')
+    primary_header["c_1"] = (c[0], "Additive bias 1st comp")
+    primary_header["c_2"] = (c[1], "Additive bias 2nd comp")
 
 
 def write_fits_BinTable_file(
     cols,
     output_path,
     R=None,
     R_shear=None,
@@ -155,7 +141,58 @@
     primary_header = write_header_info_sp(primary_header)
     if R is not None:
         add_shear_bias_to_header(primary_header, R, R_shear, R_select, c)
     primary_hdu = fits.PrimaryHDU(header=primary_header)
 
     hdu_list = fits.HDUList([primary_hdu, table_hdu])
     hdu_list.writeto(output_path, overwrite=True)
+
+
+def bin_edges2centers(bin_edges):
+    """Bin Edges To Centers.
+
+    Transform bin edge values to central values.
+
+    Parameters
+    ----------
+    bin_edges : list
+        bin edge values
+
+    Returns
+    -------
+    list
+        bin central values
+
+    """
+    bin_means = 0.5 * (bin_edges[1:] + bin_edges[:-1])
+
+    return bin_means
+
+
+def read_dndz(file_path):
+    """Read Dndz.
+
+    Read redshift histogram from file.
+
+    Parameters
+    ----------
+    file_path : str
+        input file path
+
+    Returns
+    -------
+    list :
+        redshift bin centers
+    list :
+        number densities
+    list :
+        redshift bin edges
+
+    """
+    dat = ascii.read(file_path, format="commented_header")
+
+    # Remove last n(z) value which is zero, to match bin centers
+    nz = dat["dn_dz"][:-1]
+    z_edges = dat["z"]
+    z_centers = bin_edges2centers(z_edges)
+
+    return z_centers, nz, z_edges
```

### Comparing `cs_util-0.0.3/cs_util/cfis.py` & `cs_util-0.0.4/cs_util/cfis.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 import re
 import numpy as np
 from astropy import units
 from astropy import coordinates as coords
 
 
 class Cfis(object):
-    """Cfis
+    """Cfis.
 
     Class for CFIS image properties.
 
     """
-    size = {'tile' : 0.5 * units.deg}
+
+    size = {"tile": 0.5 * units.deg}
 
 
 def get_tile_number(tile_name):
     """Get Tile Number.
 
     Return tile number of given image tile name.
 
@@ -41,18 +42,18 @@
 
     Returns
     -------
     tuple
         tile number for x and tile number for y
 
     """
-    m = re.search(r'(\d{3})[\.-](\d{3})', tile_name)
+    m = re.search(r"(\d{3})[\.-](\d{3})", tile_name)
     if m is None or len(m.groups()) != 2:
         raise ValueError(
-            f'Image name \'{tile_name}\' does not match tile name syntax'
+            f"Image name '{tile_name}' does not match tile name syntax"
         )
 
     nix = m.groups()[0]
     niy = m.groups()[1]
 
     return nix, niy
 
@@ -65,48 +66,48 @@
     Parameters
     ----------
     nix : str or list
         tile number(s) for x coordinate(s);
     niy : str or list
         tile number(s) for y coordinate(s)
 
-    See also
+    See Also
     --------
     get_tile_number_from_coord
 
     Returns
     -------
     tuple
         right ascension and declination
 
     """
-    number_pattern = re.compile(r'\d{3}')
+    number_pattern = re.compile(r"\d{3}")
 
     # Transform from str to int
     if not np.isscalar(nix):
         # Check input numbers
         if not all(
             [bool(number_pattern.fullmatch(number)) for number in nix + niy]
         ):
-            raise ValueError('Input needs to be three-digit numbers')
+            raise ValueError("Input needs to be three-digit numbers")
 
         # Transform to list
         xi = np.array(nix).astype(int)
         yi = np.array(niy).astype(int)
     else:
         if not all(
             [bool(number_pattern.fullmatch(number)) for number in [nix, niy]]
         ):
-            raise ValueError('Input needs to be three-digit numbers')
+            raise ValueError("Input needs to be three-digit numbers")
 
         xi = int(nix)
         yi = int(niy)
 
     # Declination
     d = yi / 2 - 90
-    dec = coords.Angle(d, unit='deg')
+    dec = coords.Angle(d, unit="deg")
 
     # Right ascension
     r = xi / 2 / np.cos(dec.radian)
-    ra = coords.Angle(r, unit='deg')
+    ra = coords.Angle(r, unit="deg")
 
     return ra, dec
```

### Comparing `cs_util-0.0.3/cs_util/cosmo.py` & `cs_util-0.0.4/cs_util/cosmo.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
 import numpy as np
 
 from astropy import constants
 from astropy import units
 
 
-
 def sigma_crit(z_lens, z_source, cosmo, d_lens=None, d_source=None):
-    """Critical surface mass density.
+    """Sigma Crit.
+
+    Critical surface mass density.
 
     Parameters
     ----------
     z_lens : float
         lens redshift
     z_source : float
         source redshift
@@ -49,36 +50,37 @@
     a_lens = 1 / (1 + z_lens)
     a_source = 1 / (1 + z_source)
     if not d_lens:
         d_lens = cosmo.angular_diameter_distance(a_lens) * units.Mpc
     if not d_source:
         d_source = cosmo.angular_diameter_distance(a_source) * units.Mpc
 
-    d_lens_source = cosmo.angular_diameter_distance(
-        a_lens,
-        a_source
-    ) * units.Mpc
+    d_lens_source = (
+        cosmo.angular_diameter_distance(a_lens, a_source) * units.Mpc
+    )
 
     frac = d_source / (d_lens_source * d_lens)
     pref = constants.c**2 / (4 * np.pi * constants.G)
 
-    sigma_cr =  (pref * frac).to(unit_return)
+    sigma_cr = (pref * frac).to(unit_return)
 
     return sigma_cr
 
 
 def sigma_crit_eff(
     z_lens,
     z_source_arr,
     nz_source_arr,
     cosmo,
     d_lens=None,
     d_source_arr=None,
 ):
-    """Effective critical surface mass density, which
+    """Sigma Crit Eff.
+
+    Effective critical surface mass density, which
     is sigma_crit(z_lens, z_source) weighted by nz_source.
 
     Parameters
     ----------
     z_lens : float
         lens redshift
     z_source_arr : list
@@ -110,25 +112,25 @@
     n_source = len(z_source_arr)
 
     if d_source_arr is None:
         d_source_arr = [None] * n_source
 
     if (len(nz_source_arr) != n_source) or (len(d_source_arr) != n_source):
         raise IndexError(
-            'Lists for source z, n(z), and/or d_ang have different lenghts'
+            "Lists for source z, n(z), and/or d_ang have different lenghts"
         )
 
     sigma_cr_arr = []
     for idx in range(n_source):
         sigma_cr = sigma_crit(
             z_lens,
             z_source_arr[idx],
             cosmo,
             d_lens=d_lens,
-            d_source=d_source_arr[idx]
+            d_source=d_source_arr[idx],
         )
 
         # Get unit
         if len(sigma_cr_arr) == 0:
             unit = sigma_cr.unit
 
         sigma_cr_arr.append(sigma_cr.value)
@@ -144,15 +146,17 @@
     z_lens,
     z_source_arr,
     nz_source_arr,
     cosmo,
     d_lens=None,
     d_source_arr=None,
 ):
-    """Effective inverse critical surface mass density, which
+    """Sigma Crit M1 Eff.
+
+    Effective inverse critical surface mass density, which
     is sigma_crit^{-1}(z_lens, z_source) weighted by nz_source.
     See Eq. (17) in :cite:`2004AJ....127.2544S`.
 
     Parameters
     ----------
     z_lens : float
         lens redshift
@@ -186,27 +190,27 @@
     n_source = len(z_source_arr)
 
     if d_source_arr is None:
         d_source_arr = [None] * n_source
 
     if (len(nz_source_arr) != n_source) or (len(d_source_arr) != n_source):
         raise IndexError(
-            'Lists for source z, n(z), and/or d_ang have different lenghts'
+            "Lists for source z, n(z), and/or d_ang have different lenghts"
         )
 
     sigma_cr_m1_arr = []
     weights = []
 
     for idx in range(n_source):
         sigma_cr = sigma_crit(
             z_lens,
             z_source_arr[idx],
             cosmo,
             d_lens=d_lens,
-            d_source=d_source_arr[idx]
+            d_source=d_source_arr[idx],
         )
 
         # Get unit
         if len(sigma_cr_m1_arr) == 0:
             unit = 1 / sigma_cr.unit
 
         # If lens behind source: continue
```

### Comparing `cs_util-0.0.3/cs_util/logging.py` & `cs_util-0.0.4/cs_util/logging.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,36 +33,35 @@
     Returns
     -------
     filehandler
         log file handler (if close_no_return is False)
 
     """
     # Set log file path
-    if name == 'sys.stdout':
+    if name == "sys.stdout":
         f = sys.stdout
-    elif name == 'sys.stderr':
+    elif name == "sys.stderr":
         f = sys.stderr
     else:
         if name is None:
-            name = 'log_' + os.path.basename(argv[0])
-        f = open(name, 'w')
+            name = "log_" + os.path.basename(argv[0])
+        f = open(name, "w")
 
     # Loop over arguments
-    log = ''
+    log = ""
     for a in argv:
-
         # Quote argument if special characters
-        if '[' in a or ']' in a:
-            a = f'\"{a}\"'
+        if "[" in a or "]" in a:
+            a = f'"{a}"'
 
-        log = f'{log}{a} '
+        log = f"{log}{a} "
 
     # Write to file except last character (space)
     print(log[:-1], file=f)
 
     # Return file handle if required
     if not close_no_return:
         return f
 
     # Close if proper file
-    if not name in ('sys.stdout', 'sys.stderr'):
+    if not name in ("sys.stdout", "sys.stderr"):
         f.close()
```

### Comparing `cs_util-0.0.3/cs_util/plots.py` & `cs_util-0.0.4/cs_util/plots.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,32 +25,35 @@
 
     Returns
     -------
     matplotlib.figure.Figure
         figure object
 
     """
-    fig = plt.figure(figsize=figsize, facecolor='none')
+    fig = plt.figure(figsize=figsize, facecolor="none")
 
     return fig
 
 
-def savefig(fname):
+def savefig(fname, close_fig=True):
     """Save Figure.
 
     Save figure to file.
 
     Parameters
     ----------
     fname : str
         output file name
+    close_fig : bool, optional
+        closes figure if True (default)
 
     """
-    plt.savefig(fname, facecolor='w', bbox_inches='tight')
-    plt.close()
+    plt.savefig(fname, facecolor="w", bbox_inches="tight")
+    if close_fig:
+        plt.close()
 
 
 def plot_histograms(
     xs,
     labels,
     title,
     x_label,
@@ -101,55 +104,51 @@
     list
         values, bins for each histogram call
 
     """
     if weights is None:
         weights = [np.ones_like(x) for x in xs]
     if colors is None:
-        prop_cycle = plt.rcParams['axes.prop_cycle']
-        colors = prop_cycle.by_key()['color']
+        prop_cycle = plt.rcParams["axes.prop_cycle"]
+        colors = prop_cycle.by_key()["color"]
     if linestyles is None:
-        linestyles = ['-'] * len(labels)
+        linestyles = ["-"] * len(labels)
 
     figure(figsize=(15, 10))
 
     # Return lists
     n_arr = []
     bins_arr = []
 
     # Histograms
     for x, w, label, color, linestyle in zip(
-            xs, weights, labels, colors, linestyles
+        xs, weights, labels, colors, linestyles
     ):
         n, bins, _ = plt.hist(
             x,
             n_bin,
             weights=w,
             range=x_range,
-            histtype='step',
+            histtype="step",
             color=color,
             linestyle=linestyle,
             linewidth=1,
             density=density,
-            label=label
+            label=label,
         )
         n_arr.append(n)
         bins_arr.append(bins)
 
     # Horizontal lines
     if vline_x:
         ylim = plt.ylim()
         for x, lab in zip(vline_x, vline_lab):
-            print('MKDEBUG', x, lab)
+            print("MKDEBUG", x, lab)
             plt.vlines(
-                x=x,
-                ymax=ylim[1],
-                ymin=ylim[0],
-                linestyles='--',
-                colors='k'
+                x=x, ymax=ylim[1], ymin=ylim[0], linestyles="--", colors="k"
             )
             plt.text(x * 1.5, ylim[1] * 0.95, lab)
         plt.ylim(ylim)
 
     plt.title(title)
     plt.xlabel(x_label)
     plt.ylabel(y_label)
@@ -163,71 +162,77 @@
     x,
     y,
     yerr,
     title,
     xlabel,
     ylabel,
     out_path=None,
+    create_figure=True,
     xlog=False,
     ylog=False,
     log=False,
     labels=None,
     colors=None,
     linestyles=None,
     eb_linestyles=None,
     linewidths=None,
     xlim=None,
-    ylim=None
+    ylim=None,
+    close_fig=True,
 ):
     """Plot Data 1D.
 
     Plot one-dimensional data points with errorbars.
 
     Parameters
     ----------
     x, y, yerr : array of array of float
         data
     title, xlabel, ylabel : string
         title and labels
     out_path : string, optional
         output file path, default is ``None``
+    create_figure : bool, optional
+        create figure if ``True`` (default)
     xlog, ylog : bool, optional, default is ``False``
         logscale on x, y if True
     labels : list, optional, default is ``None``
         plot labels, no labels if None
     color : list, optional, default is ``None``
         line colors, matplotlib default colors if ``None``
     linestyle : list, optional, default is ``None``
         linestyle indicators, '-' if ``None``
     linewidths : list
         line widths, default is `2`
-    eb_linestyle : array of string, optional, default is ``None``
+    eb_linestyles : array of string, optional, default is ``None``
         errorbar linestyle indicators, '-' if ``None``
     xlim : array(float, 2), optional, default=None
         x-axis limits, automatic if ``None``
     ylim : array(float, 2), optional, default is ``None``
         y-axis limits, automatic if ``None``
+    close_fig : bool, optional
+        closes figure if True (default)
 
     """
     if labels is None:
-        labels = [''] * len(x)
+        labels = [""] * len(x)
         do_legend = False
     else:
         do_legend = True
     if colors is None:
-        prop_cycle = plt.rcParams['axes.prop_cycle']
-        colors = prop_cycle.by_key()['color']
+        prop_cycle = plt.rcParams["axes.prop_cycle"]
+        colors = prop_cycle.by_key()["color"]
     if linestyles is None:
-        linestyles = ['-'] * len(x)
+        linestyles = ["-"] * len(x)
     if eb_linestyles is None:
-        eb_linestyles = ['-'] * len(x)
+        eb_linestyles = ["-"] * len(x)
     if linewidths is None:
         linewidths = [2] * len(x)
 
-    if out_path:
+    if create_figure:
         figure(figsize=(15, 10))
 
     for i in range(len(x)):
         if np.isnan(yerr[i]).all():
             eb = plt.plot(
                 x[i],
                 y[i],
@@ -239,62 +244,57 @@
             eb = plt.errorbar(
                 x[i],
                 y[i],
                 yerr=yerr[i],
                 label=labels[i],
                 color=colors[i],
                 linestyle=linestyles[i],
-                marker='o',
-                markerfacecolor='none',
+                marker="o",
+                markerfacecolor="none",
                 capsize=4,
             )
             eb[-1][0].set_linestyle(eb_linestyles[i])
 
     plt.hlines(
         y=0,
         xmin=plt.xlim()[0],
         xmax=plt.xlim()[1],
-        linestyles='dashed',
+        linestyles="dashed",
     )
 
     if xlog:
-        plt.xscale('log')
+        plt.xscale("log")
         plt.xticks(
             [0.1, 0.2, 0.5, 1, 2, 5, 10, 20, 50, 100, 200, 500],
             labels=[
-                '0.1',
-                '0.2',
-                '0.5',
-                '1',
-                '2',
-                '5',
-                '10',
-                '20',
-                '50',
-                '100',
-                '200',
-                '500',
-            ]
+                "0.1",
+                "0.2",
+                "0.5",
+                "1",
+                "2",
+                "5",
+                "10",
+                "20",
+                "50",
+                "100",
+                "200",
+                "500",
+            ],
         )
     if ylog:
-        plt.yscale('log')
+        plt.yscale("log")
 
     if xlim:
         plt.xlim(xlim)
     if ylim:
         plt.ylim(ylim)
 
-    plt.hlines(
-        y=0,
-        xmin=plt.xlim()[0],
-        xmax=plt.xlim()[1],
-        linestyles='dashed'
-    )
+    plt.hlines(y=0, xmin=plt.xlim()[0], xmax=plt.xlim()[1], linestyles="dashed")
 
     plt.title(title)
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
     if do_legend:
         plt.legend()
 
     if out_path:
-        savefig(out_path)
+        savefig(out_path, close_fig=close_fig)
```

### Comparing `cs_util-0.0.3/cs_util/tests/test_calc.py` & `cs_util-0.0.4/cs_util/tests/test_calc.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,29 +27,29 @@
 
     def tearDown(self):
         """Unset test parameter values."""
         self._x = None
         self._w = None
 
     def test_weighted_avg_and_std(self):
-        """Test ``cs_util.calc.weighted_avg_and_std`` method.
-
-        """
+        """Test ``cs_util.calc.weighted_avg_and_std`` method."""
         mean_w, std_w_uncor = calc.weighted_avg_and_std(self._x, self._w)
-        npt.assert_almost_equal(mean_w, self._mean_w, err_msg='weighted means differ')
+        npt.assert_almost_equal(
+            mean_w, self._mean_w, err_msg="weighted means differ"
+        )
         npt.assert_almost_equal(
             std_w_uncor,
             self._std_w_uncor,
-            err_msg='uncorrected weighted std differ',
+            err_msg="uncorrected weighted std differ",
         )
 
         mean_w, std_w_cor = calc.weighted_avg_and_std(
-            self._x,
-            self._w,
-            corrected=True
+            self._x, self._w, corrected=True
+        )
+        npt.assert_almost_equal(
+            mean_w, self._mean_w, err_msg="weighted means differ"
         )
-        npt.assert_almost_equal(mean_w, self._mean_w, err_msg='weighted means differ')
         npt.assert_almost_equal(
             std_w_cor,
             self._std_w_cor,
-            err_msg='corrected weighted std differ',
+            err_msg="corrected weighted std differ",
         )
```

### Comparing `cs_util-0.0.3/cs_util/tests/test_cat.py` & `cs_util-0.0.4/cs_util/tests/test_plots.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,82 @@
-"""UNIT TESTS FOR CAT SUBPACKAGE.
+"""UNIT TESTS FOR PLOTS SUBPACKAGE.
 
-This module contains unit tests for the cat subpackage.
+This module contains unit tests for the plots subpackage.
 
 """
 
 import os
 
 import numpy as np
+from matplotlib.figure import Figure
 from numpy import testing as npt
 
 from unittest import TestCase
 
-from cs_util import cat
+from cs_util import plots
 
 
-class CatTestCase(TestCase):
-    """Test case for the ``cat`` module."""
+class PlotsTestCase(TestCase):
+    """Test case for the ``plots`` module."""
 
     def setUp(self):
         """Set test parameter values."""
-        self._primary_header = {}
-        self._keys = ['AUTHOR', 'SOFTNAME', 'SOFTVERS', 'DATE']
-
-        self._keys_matrix = ['R_', 'R_g', 'R_S']
-        self._keys_c = ['c']
-        self._R = np.array([[0.5, 0.7], [-0.2, 1.2]])
-        self._R_shear = np.array([[0.4, 0.6], [-0.1, 1.1]])
-        self._R_select = np.array([[0.1, 0.2], [0.0, -0.15]])
-        self._c = np.array([-0.001, 2.1e-5])
+        self._fig_size = [13, 7]
 
+        self._x = [1, 1.5, 2, 2, 3, 5]
+        self._n_bin = 4
+        self._x_range = [1, 5]
+        self._img_path = "test.png"
+        self._n_arr = np.array([2.0, 2.0, 1.0, 1.0])
+        self._bins = np.array([1.0, 2.0, 3.0, 4.0, 5.0])
 
     def tearDown(self):
         """Unset test parameter values."""
-        self._primary_header = None
-        self._keys_matrix = None
-        self._keys_c = None
-        self._R = None
-        self._R_shear = None
-        self._R_select = None
-        self._c = None
-
-        self._out_path = None
-
-    def test_write_header_info_sp(self):
-        """Test ``cs_util.write_header_info_sp`` method.
-
-        """
-        primary_header = cat.write_header_info_sp(self._primary_header)
-        for key in self._keys:
-            self.assertTrue(key in primary_header, msg=key)
-
-    def test_add_shear_bias_to_header(self):
-        """Test ``cs_util.add_shear_bias_to_header`` method.
-
-        """
-        primary_header = self._primary_header
-        cat.add_shear_bias_to_header(
-            primary_header,
-            self._R,
-            self._R_shear,
-            self._R_select,
-            self._c
-        )
-
-        for key_base in self._keys_matrix:
-            if key_base == 'R_':
-                key = 'R'
-            else:
-                key = key_base
-            self.assertTrue(key in primary_header, msg=key)
-            for idx in (1, 2):
-                for jdx in (1, 2):
-                    key = f'{key_base}{idx}{jdx}'
-                    self.assertTrue(key in primary_header, msg=key)
-
-            for idx in (1, 2):
-                for jdx in (1, 2):
-                    key = f'R_{idx}{jdx}'
-                    npt.assert_equal(
-                        self._R[idx-1, jdx-1],
-                        primary_header[key][0],
-                        f'Incorrect value for {key}'
-                    )
+        self._fig_size = None
+        self._x = None
+        self._n_bin = None
+        self._x_range = None
+
+        if os.path.exists(self._img_path):
+            os.remove(self._img_path)
+        self._img_path = None
+
+        self._n_arr = None
+        self._bins = None
+
+    def test_figure(self):
+        """Test ``cs_util.weighted_avg_and_std`` method."""
+        fig = plots.figure(figsize=(self._fig_size[0], self._fig_size[1]))
+
+        # Check for return value
+        self.assertIsNotNone(fig, msg="Incorrect return type")
+
+        # Check image size
+        size = fig.get_size_inches()
+        for idx in (0, 1):
+            npt.assert_almost_equal(size[idx], self._fig_size[idx])
+
+    def test_plot_histograms(self):
+        """Test ``cs_util.plot_histograms`` method."""
+        vline_x_arr = [None, [1.2]]
+        vline_lab_arr = [None, ["vlab"]]
+        for vline_x, vline_lab in zip(vline_x_arr, vline_lab_arr):
+            n_arr, bins = plots.plot_histograms(
+                [self._x],
+                ["hist 1"],
+                "title",
+                "$x$",
+                "freq",
+                self._x_range,
+                self._n_bin,
+                self._img_path,
+                density=False,
+                vline_x=vline_x,
+                vline_lab=vline_lab,
+            )
+
+            # Check return histogram data
+            npt.assert_almost_equal(n_arr[0], self._n_arr)
+            npt.assert_almost_equal(bins[0], self._bins)
+
+            # Check output plot file
+            self.assertTrue(os.path.exists(self._img_path))
```

### Comparing `cs_util-0.0.3/cs_util/tests/test_cfis.py` & `cs_util-0.0.4/cs_util/tests/test_cfis.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,53 +19,51 @@
     """Test case for the ``cfis`` module."""
 
     def setUp(self):
         """Set test parameter values."""
 
         self._size_tile = 0.5 * units.deg
 
-        self._tile_number_ok = ['270.283', '188-308']
-        self._nix = ['270', '188']
-        self._niy = ['283', '308']
+        self._tile_number_ok = ["270.283", "188-308"]
+        self._nix = ["270", "188"]
+        self._niy = ["283", "308"]
         self._dec = [51.5, 64]
         self._ra = [216.86237, 214.43017]
         self._unit = units.deg
 
-        self._nix_nok = ['23x', '1234']
-        self._tile_number_nok = '12x.456'
+        self._nix_nok = ["23x", "1234"]
+        self._tile_number_nok = "12x.456"
 
     def tearDown(self):
         """Unset test parameter values."""
         self._tile_number_ok = None
         self._nix = None
         self._niy = None
         self._dec = None
         self._ra = None
         self._unit = None
         self._tile_number_nok = None
 
     def test_Cfis(self):
         """Test ``cs_util.Cfis`` class."""
-        self.assertTrue(self._size_tile == cfis.Cfis().size['tile'])
+        self.assertTrue(self._size_tile == cfis.Cfis().size["tile"])
 
     def test_get_tile_number(self):
         """Test ``cs_util.get_tile_number`` method."""
 
         # Test return values for valid input tile numbers
         for idx, tile_number_ok in enumerate(self._tile_number_ok):
             nix, niy = cfis.get_tile_number(tile_number_ok)
             self.assertTrue(
                 (nix == self._nix[idx]) and (niy == self._niy[idx]),
-                msg=f'{nix}!={self._nix[idx]} or {niy}!={self._niy[idx]}',
+                msg=f"{nix}!={self._nix[idx]} or {niy}!={self._niy[idx]}",
             )
 
         self.assertRaises(
-            ValueError,
-            cfis.get_tile_number,
-            self._tile_number_nok
+            ValueError, cfis.get_tile_number, self._tile_number_nok
         )
 
     def test_get_tile_coord_from_nixy(self):
         """Test ``cs_util.get_tile_coord_from_nixy`` method."""
 
         # Call with scalar arguments
         for idx in range(len(self._nix)):
@@ -74,42 +72,41 @@
                 self._niy[idx],
             )
 
             # Test values
             npt.assert_almost_equal(
                 ra.value,
                 self._ra[idx],
-                err_msg=f'{ra}!={self._ra[idx]}',
+                err_msg=f"{ra}!={self._ra[idx]}",
                 decimal=5,
             )
             npt.assert_almost_equal(
                 dec.value,
                 self._dec[idx],
-                err_msg=f'{dec}!={self._dec[idx]}',
+                err_msg=f"{dec}!={self._dec[idx]}",
             )
 
             # Test units
             self.assertTrue(ra.unit == self._unit)
             self.assertTrue(dec.unit == self._unit)
 
         # Call with list arguments
         ra, dec = cfis.get_tile_coord_from_nixy(self._nix, self._niy)
         for idx in range(len(self._nix)):
-
             # Test values
             npt.assert_almost_equal(
                 ra[idx].value,
                 self._ra[idx],
-                err_msg=f'{ra[idx]}!={self._ra[idx]}',
+                err_msg=f"{ra[idx]}!={self._ra[idx]}",
                 decimal=5,
             )
             npt.assert_almost_equal(
                 dec[idx].value,
                 self._dec[idx],
-                err_msg=f'{dec[idx]}!={self._dec[idx]}',
+                err_msg=f"{dec[idx]}!={self._dec[idx]}",
             )
             # Test units
             self.assertTrue(ra[idx].unit == self._unit)
             self.assertTrue(dec[idx].unit == self._unit)
 
         # Test exception for invalid input
         self.assertRaises(
```

### Comparing `cs_util-0.0.3/cs_util/tests/test_cosmo.py` & `cs_util-0.0.4/cs_util/tests/test_cosmo.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,32 +38,30 @@
         self._d_source = 1617.9195 * units.Mpc
         self._d_lens = 1315.3937 * units.Mpc
 
         self._d_source_arr = [
             1157.82363726,
             1440.63922894,
             1617.91952285,
-            1678.82870081
+            1678.82870081,
         ] * units.Mpc
 
     def tearDown(self):
         """Unset test parameter values."""
         self._z_source = None
         self._z_lens = None
         self._cosmo = None
         self._sigma_crit_value = None
         self._sigma_crit_unit = None
         self._d_source = None
         self._d_lens = None
         self._ds_cosmo = None
 
     def test_sigma_crit(self):
-        """Test ``cs_util.cosmo.sigma_crit`` method.
-
-        """
+        """Test ``cs_util.cosmo.sigma_crit`` method."""
         sigma_crit = cosmo.sigma_crit(
             self._z_lens,
             self._z_source,
             self._cosmo,
         )
         # Test return value
         npt.assert_almost_equal(
@@ -72,17 +70,15 @@
             decimal=4,
         )
         # Test return unit
         npt.assert_equal(sigma_crit.unit, self._sigma_crit_unit)
 
         # Test with lens behind source
         sigma_crit = cosmo.sigma_crit(
-            self._z_lens,
-            self._z_lens / 2,
-            self._cosmo
+            self._z_lens, self._z_lens / 2, self._cosmo
         )
         npt.assert_equal(sigma_crit, 0 * self._sigma_crit_unit)
 
         # Test changing default arguments
         sigma_crit = cosmo.sigma_crit(
             self._z_lens,
             self._z_source,
@@ -117,17 +113,15 @@
         npt.assert_almost_equal(
             sigma_crit.value,
             self._sigma_crit_value,
             decimal=2,
         )
 
     def test_sigma_crit_eff(self):
-        """Test ``cs_util.cosmo.sigma_crit_eff`` method.
-
-        """
+        """Test ``cs_util.cosmo.sigma_crit_eff`` method."""
         sigma_crit_eff = cosmo.sigma_crit_eff(
             self._z_lens,
             self._z_source_arr,
             self._nz_source_arr,
             self._cosmo,
         )
         # Test return value
@@ -145,15 +139,15 @@
             IndexError,
             cosmo.sigma_crit_eff,
             self._z_lens,
             self._z_source_arr[:-1],
             self._nz_source_arr,
             self._cosmo,
         )
-        
+
         # Test changing default arguments
         sigma_crit_eff = cosmo.sigma_crit_eff(
             self._z_lens,
             self._z_source_arr,
             self._nz_source_arr,
             self._cosmo,
             d_source_arr=self._d_source_arr,
@@ -185,35 +179,31 @@
         )
         npt.assert_almost_equal(
             sigma_crit_eff.value,
             self._sigma_crit_value_eff,
             decimal=3,
         )
 
-
     def test_sigma_crit_m1_eff(self):
-        """Test ``cs_util.cosmo.sigma_crit_m1_eff`` method.
-
-        """
+        """Test ``cs_util.cosmo.sigma_crit_m1_eff`` method."""
         sigma_crit_m1_eff = cosmo.sigma_crit_m1_eff(
             self._z_lens,
             self._z_source_arr,
             self._nz_source_arr,
             self._cosmo,
         )
         # Test return value
         npt.assert_almost_equal(
             sigma_crit_m1_eff.value,
             self._sigma_crit_value_eff_m1,
             decimal=4,
         )
         # Test return unit
         npt.assert_equal(
-            sigma_crit_m1_eff.unit,
-            (1 / self._sigma_crit_unit).unit
+            sigma_crit_m1_eff.unit, (1 / self._sigma_crit_unit).unit
         )
 
         # Test exception when redshift array lengths inconsistent
         self.assertRaises(
             IndexError,
             cosmo.sigma_crit_m1_eff,
             self._z_lens,
```

### Comparing `cs_util-0.0.3/cs_util/tests/test_logging.py` & `cs_util-0.0.4/cs_util/tests/test_logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,89 +15,95 @@
 
 class LoggingTestCase(TestCase):
     """Test case for the ``logging`` module."""
 
     def setUp(self):
         """Set test parameter values."""
         self._argv = [
-            'test_cmd arg',
-             '-s',
-             'opt_short',
-             '--long',
-             'opt_long',
-             '-l',
-             '"opt 1 2 list"',
-             '-c',
-             'opt_special_char[x]',
+            "test_cmd arg",
+            "-s",
+            "opt_short",
+            "--long",
+            "opt_long",
+            "-l",
+            '"opt 1 2 list"',
+            "-c",
+            "opt_special_char[x]",
         ]
-        self._log_file_path = 'log_test'
-
+        self._log_file_path = "log_test"
+        self._log_file_path_default = "log_test_cmd arg"
 
     def tearDown(self):
         """Unset test parameter values."""
         self._argv = None
         os.remove(self._log_file_path)
         self._log_file_path = None
 
     def test_log_command(self):
         """Test ``cs_util.logging.log_command`` method with
-            argument string.
+        argument string.
 
         """
         # Test log file content
 
-        # Create log command file with no return
-        fh_none = logging.log_command(
-            self._argv,
-            name=self._log_file_path,
-            close_no_return=True,
-        )
+        names_output = [self._log_file_path, None]
+        names_input = [self._log_file_path, self._log_file_path_default]
 
-        # Read log command file
-        with open(self._log_file_path, 'r') as file:
-            log_str = file.read().replace('\n', '')
-
-        # Mask special characters
-        argv_list = []
-        for a in self._argv:
-            if '[' in a or ']' in a:
-                a = f'\"{a}\"'
-            argv_list.append(a)
-
-        # Transform argv list to str
-        argv_str = ' '.join(argv_list)
-
-        # Test for equality with input
-        npt.assert_equal(
-            argv_str,
-            log_str,
-            'Incorrect log file output'
-        )
+        for name_out, name_in in zip(names_output, names_input):
+            # Create log command file with no return
+            fh_none = logging.log_command(
+                self._argv,
+                name=name_out,
+                close_no_return=True,
+            )
+
+            # Read log command file
+            with open(name_in, "r") as file:
+                log_str = file.read().replace("\n", "")
+            os.unlink(name_in)
+
+            # Mask special characters
+            argv_list = []
+            for a in self._argv:
+                if "[" in a or "]" in a:
+                    a = f'"{a}"'
+                argv_list.append(a)
+
+            # Transform argv list to str
+            argv_str = " ".join(argv_list)
 
-        # Test return type ``None``
-        npt.assert_equal(fh_none, None, 'Incorrect return type')
+            # Test for equality with input
+            npt.assert_equal(argv_str, log_str, "Incorrect log file output")
+
+            # Test return type ``None``
+            npt.assert_equal(fh_none, None, "Incorrect return type")
 
         # Test return type is file handler: read and test type string
         # Create log command file with no return
         fh_open = logging.log_command(
             self._argv,
             name=self._log_file_path,
             close_no_return=False,
         )
-        self.assertIsNotNone(fh_open, msg='Incorrect return object')
+        self.assertIsNotNone(fh_open, msg="Incorrect return object")
 
         # Test return object is stdout
         fh_stdout = logging.log_command(
             self._argv,
-            name='sys.stdout',
+            name="sys.stdout",
             close_no_return=False,
         )
-        npt.assert_equal(fh_stdout, sys.stdout, 'Incorrect return object')
+        npt.assert_equal(fh_stdout, sys.stdout, "Incorrect return object")
 
         # Test return object is stderr
         fh_stderr = logging.log_command(
             self._argv,
-            name='sys.stderr',
+            name="sys.stderr",
             close_no_return=False,
         )
-        npt.assert_equal(fh_stderr, sys.stderr, 'Incorrect return object')
+        npt.assert_equal(fh_stderr, sys.stderr, "Incorrect return object")
 
+        # Test logging with default log file name
+        fh_none = logging.log_command(
+            self._argv,
+            close_no_return=True,
+        )
```

### Comparing `cs_util-0.0.3/cs_util.egg-info/PKG-INFO` & `cs_util-0.0.4/cs_util.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: cs-util
-Version: 0.0.3
-Summary: Utility library for CosmoStat
-Home-page: https://github.com/martinkilbinger/cs_util
-Author: Martin Kilbinger
-Author-email: martin.kilbinger@cea.fr
-License: MIT
+Version: 0.0.4
+Author: The CosmoStat Lab
+Maintainer-email: Martin Kilbinger <martin.kilbinger@cea.fr>
+Project-URL: Source, https://github.com/CosmoStat/cs_util
+Project-URL: Documentation, https://github.com/CosmoStat/cs_util
+Project-URL: Tracker, https://github.com/CosmoStat/cs_util/issues
+Keywords: CosmoStat,cosmology,weak gravitational lensing
+Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.6
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: develop
+Provides-Extra: lint
+Provides-Extra: release
+Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENCE.txt
 
 # cs_util package
 
 Utility library for CosmoStat
 
 | Usage | Development | Release |
@@ -40,8 +45,14 @@
 
 
 
 ## Contents
 
 ### Library
 
-### Scripts
+- Galaxy catalogue handling
+- Weak-lensing related cosmological quantities (e.g. surface mass density)
+- VOS (Virtual Observatory Software)
+- Command line logging
+- Plotting
+- Basic statistic calculations
+- UNIONS/CFIS weak-lensing survey handling
```

#### html2text {}

```diff
@@ -1,38 +1,45 @@
-Metadata-Version: 2.1 Name: cs-util Version: 0.0.3 Summary: Utility library for
-CosmoStat Home-page: https://github.com/martinkilbinger/cs_util Author: Martin
-Kilbinger Author-email: martin.kilbinger@cea.fr License: MIT Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: develop License-File: LICENCE.txt #
-cs_util package Utility library for CosmoStat | Usage | Development | Release |
-| ----- | ----------- | ------- | | [![docs](https://img.shields.io/badge/docs-
-Sphinx-blue)](https://martinkilbinger.github.io/cs_util/) | [![build](https://
-github.com/martinkilbinger/cs_util/workflows/CI/badge.svg)](https://github.com/
-martinkilbinger/cs_util/actions?query=workflow%3ACI) | [![release](https://
-img.shields.io/github/v/release/martinkilbinger/cs_util)](https://github.com/
-martinkilbinger/cs_util/releases/latest) | | [![license](https://
-img.shields.io/github/license/martinkilbinger/cs_util)](https://github.com/
-martinkilbinger/cs_util/blob/master/LICENCE.txt) | [![deploy](https://
-github.com/martinkilbinger/cs_util/workflows/CD/badge.svg)](https://github.com/
-martinkilbinger/cs_util/actions?query=workflow%3ACD) | [![pypi](https://
-img.shields.io/pypi/v/cs_util)](https://pypi.org/project/cs_util/) | | [!
-[wemake-python-styleguide](https://img.shields.io/badge/style-wemake-
-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide) | [!
-[codecov](https://codecov.io/gh/martinkilbinger/cs_util/branch/master/graph/
-badge.svg?token=XHJIQXV7AX)](https://codecov.io/gh/martinkilbinger/cs_util) |
-[![python](https://img.shields.io/pypi/pyversions/cs_util)](https://
-www.python.org/downloads/source/) | | [![contribute](https://img.shields.io/
-badge/contribute-read-lightgrey)](https://github.com/martinkilbinger/cs_util/
-blob/master/CONTRIBUTING.md) | [![CodeFactor](https://www.codefactor.io/
-repository/github/martinkilbinger/cs_util/badge)](https://www.codefactor.io/
-repository/github/martinkilbinger/cs_util) | | | [![coc](https://
-img.shields.io/badge/conduct-read-lightgrey)](https://github.com/
-martinkilbinger/cs_util/blob/master/CODE_OF_CONDUCT.md) | [![Updates](https://
-pyup.io/repos/github/martinkilbinger/cs_util/shield.svg)](https://pyup.io/
-repos/github/martinkilbinger/cs_util/) | | --- > Author: Martin_Kilbinger >
-Email: martin.kilbinger@cea.fr > Year: 2022 --- ## Contents ### Library ###
-Scripts
+Metadata-Version: 2.1 Name: cs-util Version: 0.0.4 Author: The CosmoStat Lab
+Maintainer-email: Martin Kilbinger
+kilbinger@cea.fr> Project-URL: Source, https://github.com/CosmoStat/cs_util
+Project-URL: Documentation, https://github.com/CosmoStat/cs_util Project-URL:
+Tracker, https://github.com/CosmoStat/cs_util/issues Keywords:
+CosmoStat,cosmology,weak gravitational lensing Classifier: Development Status
+:: 1 - Planning Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Operating System :: POSIX :: Linux Classifier:
+Operating System :: MacOS Classifier: Topic :: Scientific/Engineering Requires-
+Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: lint
+Provides-Extra: release Provides-Extra: test Provides-Extra: dev License-File:
+LICENCE.txt # cs_util package Utility library for CosmoStat | Usage |
+Development | Release | | ----- | ----------- | ------- | | [![docs](https://
+img.shields.io/badge/docs-Sphinx-blue)](https://martinkilbinger.github.io/
+cs_util/) | [![build](https://github.com/martinkilbinger/cs_util/workflows/CI/
+badge.svg)](https://github.com/martinkilbinger/cs_util/
+actions?query=workflow%3ACI) | [![release](https://img.shields.io/github/v/
+release/martinkilbinger/cs_util)](https://github.com/martinkilbinger/cs_util/
+releases/latest) | | [![license](https://img.shields.io/github/license/
+martinkilbinger/cs_util)](https://github.com/martinkilbinger/cs_util/blob/
+master/LICENCE.txt) | [![deploy](https://github.com/martinkilbinger/cs_util/
+workflows/CD/badge.svg)](https://github.com/martinkilbinger/cs_util/
+actions?query=workflow%3ACD) | [![pypi](https://img.shields.io/pypi/v/cs_util)]
+(https://pypi.org/project/cs_util/) | | [![wemake-python-styleguide](https://
+img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-
+services/wemake-python-styleguide) | [![codecov](https://codecov.io/gh/
+martinkilbinger/cs_util/branch/master/graph/badge.svg?token=XHJIQXV7AX)](https:
+//codecov.io/gh/martinkilbinger/cs_util) | [![python](https://img.shields.io/
+pypi/pyversions/cs_util)](https://www.python.org/downloads/source/) | | [!
+[contribute](https://img.shields.io/badge/contribute-read-lightgrey)](https://
+github.com/martinkilbinger/cs_util/blob/master/CONTRIBUTING.md) | [!
+[CodeFactor](https://www.codefactor.io/repository/github/martinkilbinger/
+cs_util/badge)](https://www.codefactor.io/repository/github/martinkilbinger/
+cs_util) | | | [![coc](https://img.shields.io/badge/conduct-read-lightgrey)]
+(https://github.com/martinkilbinger/cs_util/blob/master/CODE_OF_CONDUCT.md) |
+[![Updates](https://pyup.io/repos/github/martinkilbinger/cs_util/shield.svg)]
+(https://pyup.io/repos/github/martinkilbinger/cs_util/) | | --- > Author:
+Martin_Kilbinger > Email: martin.kilbinger@cea.fr > Year: 2022 --- ## Contents
+### Library - Galaxy catalogue handling - Weak-lensing related cosmological
+quantities (e.g. surface mass density) - VOS (Virtual Observatory Software) -
+Command line logging - Plotting - Basic statistic calculations - UNIONS/CFIS
+weak-lensing survey handling
```

### Comparing `cs_util-0.0.3/cs_util.egg-info/SOURCES.txt` & `cs_util-0.0.4/cs_util.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENCE.txt
 MANIFEST.in
 README.md
 develop.txt
 environment.yml
+pyproject.toml
 requirements.txt
-setup.cfg
-setup.py
 .github/workflows/cd-build.yml
 .github/workflows/ci-build.yml
 cs_util/__init__.py
 cs_util/calc.py
 cs_util/canfar.py
 cs_util/cat.py
 cs_util/cfis.py
```

### Comparing `cs_util-0.0.3/docs/_script_templates/package.rst_t` & `cs_util-0.0.4/docs/_script_templates/package.rst_t`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.3/docs/_templates/package.rst_t` & `cs_util-0.0.4/docs/_templates/package.rst_t`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.3/docs/source/conf.py` & `cs_util-0.0.4/docs/source/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,108 +5,109 @@
 import sys
 import os
 from importlib_metadata import metadata
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-sys.path.insert(0, os.path.abspath('../..'))
+sys.path.insert(0, os.path.abspath("../.."))
+sys.path.insert(0, os.path.abspath("../.."))
 
 # -- General configuration ------------------------------------------------
 
 # General information about the project.
-project = 'cs_util'
+project = "cs_util"
 
 mdata = metadata(project)
-author = mdata['Author']
-version = mdata['Version']
-copyright = '2022, {}'.format(author)
-gh_user = 'martinkilbinger'
+author = mdata["Author"]
+version = mdata["Version"]
+copyright = "2022, {}".format(author)
+gh_user = "martinkilbinger"
 
 # If your documentation needs a minimal Sphinx version, state it here.
-needs_sphinx = '3.3'
+needs_sphinx = "3.3"
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.autosummary',
-    'sphinx.ext.coverage',
-    'sphinx.ext.doctest',
-    'sphinx.ext.ifconfig',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.mathjax',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.todo',
-    'sphinx.ext.viewcode',
-    'sphinxawesome_theme',
-    'sphinxcontrib.bibtex',
-    'nbsphinx',
-    'nbsphinx_link',
-    'numpydoc',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.ifconfig",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.todo",
+    "sphinx.ext.viewcode",
+    "sphinxawesome_theme",
+    "sphinxcontrib.bibtex",
+    "nbsphinx",
+    "nbsphinx_link",
+    "numpydoc",
 ]
 
 # Include module names for objects
 add_module_names = False
 
 # Set class documentation standard.
-autoclass_content = 'class'
+autoclass_content = "class"
 
 # Order docstrings as in the source
-autodoc_member_order = 'bysource'
+autodoc_member_order = "bysource"
 
 # Include private class methods
-autodoc_default_flags = ['members', 'private-members']
+autodoc_default_flags = ["members", "private-members"]
 
 # Generate summaries
 autosummary_generate = True
 
 # Suppress class members in toctree.
 numpydoc_show_class_members = False
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
-source_suffix = ['.rst', '.md']
+source_suffix = [".rst", ".md"]
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 show_authors = True
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'default'
+pygments_style = "default"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'sphinxawesome_theme'
+html_theme = "sphinxawesome_theme"
 # html_theme = 'sphinx_book_theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     "nav_include_hidden": True,
     "show_nav": True,
     "show_breadcrumbs": False,
-    "breadcrumbs_separator": "/"
+    "breadcrumbs_separator": "/",
 }
 html_collapsible_definitions = True
 
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-html_title = '{0} v{1}'.format(project, version)
+html_title = "{0} v{1}".format(project, version)
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 # html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 # html_logo = None
@@ -114,15 +115,15 @@
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 # html_favicon = None
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-html_last_updated_fmt = '%d %b, %Y'
+html_last_updated_fmt = "%d %b, %Y"
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
 html_use_smartypants = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
 html_show_sphinx = True
@@ -131,56 +132,54 @@
 html_show_copyright = True
 
 # -- Options for nbshpinx output ------------------------------------------
 
 
 # Custom fucntion to find notebooks, create .nblink files and update the
 # notebooks.rst file
-def add_notebooks(nb_path='../../notebooks'):
-
-    print('Looking for notebooks')
-    nb_ext = '.ipynb'
-    nb_rst_file_name = 'notebooks.rst'
+def add_notebooks(nb_path="../../notebooks"):
+    print("Looking for notebooks")
+    nb_ext = ".ipynb"
+    nb_rst_file_name = "notebooks.rst"
     nb_link_format = '{{\n   "path": "{0}/{1}"\n}}'
 
     nbs = sorted([nb for nb in os.listdir(nb_path) if nb.endswith(nb_ext)])
 
     for list_pos, nb in enumerate(nbs):
-
         nb_name = nb.rstrip(nb_ext)
 
-        nb_link_file_name = nb_name + '.nblink'
-        print('Writing {0}'.format(nb_link_file_name))
-        with open(nb_link_file_name, 'w') as nb_link_file:
+        nb_link_file_name = nb_name + ".nblink"
+        print("Writing {0}".format(nb_link_file_name))
+        with open(nb_link_file_name, "w") as nb_link_file:
             nb_link_file.write(nb_link_format.format(nb_path, nb))
 
-        print('Looking for {0} in {1}'.format(nb_name, nb_rst_file_name))
-        with open(nb_rst_file_name, 'r') as nb_rst_file:
+        print("Looking for {0} in {1}".format(nb_name, nb_rst_file_name))
+        with open(nb_rst_file_name, "r") as nb_rst_file:
             check_name = nb_name not in nb_rst_file.read()
 
         if check_name:
-            print('Adding {0} to {1}'.format(nb_name, nb_rst_file_name))
-            with open(nb_rst_file_name, 'a') as nb_rst_file:
+            print("Adding {0} to {1}".format(nb_name, nb_rst_file_name))
+            with open(nb_rst_file_name, "a") as nb_rst_file:
                 if list_pos == 0:
-                    nb_rst_file.write('\n')
-                nb_rst_file.write('   {0}\n'.format(nb_name))
+                    nb_rst_file.write("\n")
+                nb_rst_file.write("   {0}\n".format(nb_name))
 
     return nbs
 
 
 # Add notebooks
-#add_notebooks()
+# add_notebooks()
 
-binder = 'https://mybinder.org/v2/gh'
-binder_badge = 'https://mybinder.org/badge_logo.svg'
-github = 'https://github.com/'
-github_badge = 'https://badgen.net/badge/icon/github?icon=github&label'
+binder = "https://mybinder.org/v2/gh"
+binder_badge = "https://mybinder.org/badge_logo.svg"
+github = "https://github.com/"
+github_badge = "https://badgen.net/badge/icon/github?icon=github&label"
 
 # Remove promts and add binder badge
-nb_header_pt1 = r'''
+nb_header_pt1 = r"""
 {% if env.metadata[env.docname]['nbsphinx-link-target'] %}
 {% set docpath = env.metadata[env.docname]['nbsphinx-link-target'] %}
 {% else %}
 {% set docpath = env.doc2path(env.docname, base='docs/source/') %}
 {% endif %}
 
 .. raw:: html
@@ -188,37 +187,37 @@
     <style>
         .nbinput .prompt,
         .nboutput .prompt {
             display: none;
         }
     </style>
 
-'''
+"""
 nb_header_pt2 = (
-    r'''    <p><div class="inline-block">'''
-    r'''<a href="{0}/{1}/{2}/'''.format(binder, gh_user, project) +
-    r'''master?filepath={{ docpath }}">''' +
-    r'''<img alt="Binder badge" src="{0}" '''.format(binder_badge) +
-    r'''style="vertical-align:text-bottom"></a></div>'''
-    r'''<div class="inline-block"><a href=''' +
-    r'''"{0}/{1}/{2}/blob/master/'''.format(github, gh_user, project) +
-    r'''{{ docpath }}"><img alt="GitHub badge" ''' +
-    r'''src="{0}" style="vertical-align:text-bottom">'''.format(github_badge) +
-    r'''</a></div></p>'''
+    r"""    <p><div class="inline-block">"""
+    r"""<a href="{0}/{1}/{2}/""".format(binder, gh_user, project)
+    + r"""master?filepath={{ docpath }}">"""
+    + r"""<img alt="Binder badge" src="{0}" """.format(binder_badge)
+    + r"""style="vertical-align:text-bottom"></a></div>"""
+    r"""<div class="inline-block"><a href="""
+    + r""""{0}/{1}/{2}/blob/master/""".format(github, gh_user, project)
+    + r"""{{ docpath }}"><img alt="GitHub badge" """
+    + r"""src="{0}" style="vertical-align:text-bottom">""".format(github_badge)
+    + r"""</a></div></p>"""
 )
 
 nbsphinx_prolog = nb_header_pt1 + nb_header_pt2
 
 # -- Intersphinx Mapping ----------------------------------------------
 
 # Refer to the package libraries for type definitions
 intersphinx_mapping = {
-    'python': ('http://docs.python.org/3', None),
-    'astropy': ('http://docs.astropy.org/en/latest/', None),
-    'numpy': ('https://numpy.org/doc/stable/', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference', None),
-    'matplotlib': ('https://matplotlib.org', None),
+    "python": ("http://docs.python.org/3", None),
+    "astropy": ("http://docs.astropy.org/en/latest/", None),
+    "numpy": ("https://numpy.org/doc/stable/", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
+    "matplotlib": ("https://matplotlib.org", None),
 }
 
 # -- BibTeX Setting  ----------------------------------------------
 
-bibtex_bibfiles = ['refs.bib', 'my_ref.bib']
+bibtex_bibfiles = ["refs.bib", "my_ref.bib"]
```

### Comparing `cs_util-0.0.3/docs/source/index.rst` & `cs_util-0.0.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.3/docs/source/installation.rst` & `cs_util-0.0.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.3/docs/source/refs.bib` & `cs_util-0.0.4/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.3/scripts/__init__.py` & `cs_util-0.0.4/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cs_util-0.0.3/scripts/example_script.py` & `cs_util-0.0.4/scripts/example_script.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,32 +22,36 @@
 
 import argparse as ap
 import sys
 
 from cs_util.example.classes import StefBoltz
 from cs_util.example.hello import hello_world
 
-line = '----------------'
+line = "----------------"
 
 
 def get_args():
     """Get Script Arguments.
 
     Returns
     -------
     argparse.Namespace
         Command line arguments
 
     """
     parser = ap.ArgumentParser()
     parser.add_argument(
-        '--radius', type=float, help='Radius in meters.',
+        "--radius",
+        type=float,
+        help="Radius in meters.",
     )
     parser.add_argument(
-        '--eff_temp', type=float, help='Effective temperature in Kelvin.',
+        "--eff_temp",
+        type=float,
+        help="Effective temperature in Kelvin.",
     )
 
     return parser.parse_args()
 
 
 def call_hello():
     """Call Hello World.
@@ -57,18 +61,18 @@
     See Also
     --------
     cs_util.example.hello.hello_world : Implementation of the
         ``hello_world`` function.
 
     """
     print(line)
-    print('Example 1')
-    print('Call hello_world')
+    print("Example 1")
+    print("Call hello_world")
     print(line)
-    print('Result:', hello_world())
+    print("Result:", hello_world())
 
 
 def call_stefboltz(radius: float, eff_temp: float):
     """Call StefBoltz.
 
     This function calls the ``StefBoltz`` class and prints the luminosity
     corresponding to the radius and effective temperature provided.
@@ -85,18 +89,18 @@
     cs_util.example.classes.StefBoltz : Implementation of the ``StefBoltz``
         class.
 
     """
     luminosity = StefBoltz(radius, eff_temp).luminosity()
 
     print(line)
-    print('Example 2')
-    print('Call StefBoltz')
+    print("Example 2")
+    print("Call StefBoltz")
     print(line)
-    print('Result:', 'The luminosity is {0:.2e}w.'.format(luminosity))
+    print("Result:", "The luminosity is {0:.2e}w.".format(luminosity))
 
 
 def run_steps():
     """Call Script Steps.
 
     This is the main method called by the script. It runs the various
     steps involved.
```

