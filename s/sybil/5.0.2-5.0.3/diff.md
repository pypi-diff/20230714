# Comparing `tmp/sybil-5.0.2.tar.gz` & `tmp/sybil-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil-5.0.2.tar", last modified: Fri May 19 07:44:54 2023, max compression
+gzip compressed data, was "sybil-5.0.3.tar", last modified: Fri Jul 14 07:04:42 2023, max compression
```

## Comparing `sybil-5.0.2.tar` & `sybil-5.0.3.tar`

### file list

```diff
@@ -1,59 +1,78 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-05-19 07:44:42.000000 sybil-5.0.2/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-05-19 07:44:54.212619 sybil-5.0.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2023-05-19 07:44:42.000000 sybil-5.0.2/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-05-19 07:44:54.216619 sybil-5.0.2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1136 2023-05-19 07:44:42.000000 sybil-5.0.2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.208618 sybil-5.0.2/sybil/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      133 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8309 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/document.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/evaluators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/evaluators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      143 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/evaluators/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1882 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/evaluators/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1011 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/evaluators/python.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1775 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/evaluators/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/example.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/integration/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/integration/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3911 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/integration/pytest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1428 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/integration/unittest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/parsers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/parsers/abstract/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1915 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2145 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3208 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/doctest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/parsers/myst/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2784 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      989 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5747 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      277 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/skip.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/parsers/rest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2862 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      368 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1465 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2690 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1114 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/python.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3299 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/region.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6442 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/sybil.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/text.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/typing.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.208618 sybil-5.0.2/sybil.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-05-19 07:44:54.000000 sybil-5.0.2/sybil.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-05-19 07:44:54.000000 sybil-5.0.2/sybil.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-19 07:44:54.000000 sybil-5.0.2/sybil.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-19 07:44:54.000000 sybil-5.0.2/sybil.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-19 07:44:54.000000 sybil-5.0.2/sybil.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:42.106631 sybil-5.0.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-07-14 07:04:30.000000 sybil-5.0.3/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1120 2023-07-14 07:04:42.106631 sybil-5.0.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2023-07-14 07:04:30.000000 sybil-5.0.3/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-07-14 07:04:42.106631 sybil-5.0.3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1136 2023-07-14 07:04:30.000000 sybil-5.0.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:42.098631 sybil-5.0.3/sybil/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      133 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8309 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/document.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:42.098631 sybil-5.0.3/sybil/evaluators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/evaluators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      143 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/evaluators/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1882 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/evaluators/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1011 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/evaluators/python.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1775 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/evaluators/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/example.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:42.102631 sybil-5.0.3/sybil/integration/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/integration/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4331 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/integration/pytest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1428 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/integration/unittest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:42.102631 sybil-5.0.3/sybil/parsers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:42.102631 sybil-5.0.3/sybil/parsers/abstract/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/abstract/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/abstract/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1915 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/abstract/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2145 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/abstract/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3208 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/abstract/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/abstract/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/doctest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:42.102631 sybil-5.0.3/sybil/parsers/myst/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/myst/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/myst/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2784 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/myst/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      989 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/myst/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5747 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/myst/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      277 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/myst/skip.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:42.102631 sybil-5.0.3/sybil/parsers/rest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/rest/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2862 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/rest/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      368 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/rest/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/rest/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1465 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/rest/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2690 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/rest/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/rest/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/parsers/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1114 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/python.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3299 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/region.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6442 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/sybil.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/text.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-07-14 07:04:30.000000 sybil-5.0.3/sybil/typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:42.098631 sybil-5.0.3/sybil.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1120 2023-07-14 07:04:42.000000 sybil-5.0.3/sybil.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1681 2023-07-14 07:04:42.000000 sybil-5.0.3/sybil.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-14 07:04:42.000000 sybil-5.0.3/sybil.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-07-14 07:04:42.000000 sybil-5.0.3/sybil.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-14 07:04:42.000000 sybil-5.0.3/sybil.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 07:04:42.106631 sybil-5.0.3/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1675 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5195 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_compatibility.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1980 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_docs_examples.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6625 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1585 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18457 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_functional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1436 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      754 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_lexing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      345 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_myst_clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4210 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_myst_codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2796 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_myst_doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4296 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_myst_lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      305 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_myst_skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_rest_lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1847 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11244 2023-07-14 07:04:30.000000 sybil-5.0.3/tests/test_sybil.py
```

### Comparing `sybil-5.0.2/LICENSE.txt` & `sybil-5.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/PKG-INFO` & `sybil-5.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sybil
-Version: 5.0.2
+Version: 5.0.3
 Summary: Automated testing for the examples in your code and documentation.
 Home-page: https://github.com/simplistix/sybil
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: build
 License-File: LICENSE.txt
@@ -29,9 +28,7 @@
 
 This library provides a way to check examples in your code and documentation by parsing
 them from their source and evaluating the parsed examples as part of
 your normal test run. Integration is provided for the main Python test
 runners.
 
 The `documentation <https://sybil.readthedocs.io/>`__ is the best place to start.
-
-
```

### Comparing `sybil-5.0.2/README.rst` & `sybil-5.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/setup.py` & `sybil-5.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import setup, find_packages
 
 base_dir = os.path.dirname(__file__)
 
 setup(
     name='sybil',
-    version='5.0.2',
+    version='5.0.3',
     author='Chris Withers',
     author_email='chris@withers.org',
     license='MIT',
     description="Automated testing for the examples in your code and documentation.",
     long_description=open('README.rst').read(),
     url='https://github.com/simplistix/sybil',
     classifiers=[
```

### Comparing `sybil-5.0.2/sybil/document.py` & `sybil-5.0.3/sybil/document.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/evaluators/doctest.py` & `sybil-5.0.3/sybil/evaluators/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/evaluators/python.py` & `sybil-5.0.3/sybil/evaluators/python.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/evaluators/skip.py` & `sybil-5.0.3/sybil/evaluators/skip.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/example.py` & `sybil-5.0.3/sybil/example.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/integration/pytest.py` & `sybil-5.0.3/sybil/integration/pytest.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,19 +74,31 @@
         self._request._fillfixtures()
         for name, fixture in self.funcargs.items():
             self.example.namespace[name] = fixture
 
     def runtest(self):
         self.example.evaluate()
 
-    def _prunetraceback(self, excinfo):
-        tb = excinfo.traceback.cut(path=example_module_path)
-        tb = tb[1]
-        if getattr(tb, '_rawentry', None) is not None:
-            excinfo.traceback = Traceback(tb._rawentry, excinfo)
+    if PYTEST_VERSION >= (7, 4, 0):
+
+        def _traceback_filter(self, excinfo: ExceptionInfo[BaseException]) -> Traceback:
+            traceback = excinfo.traceback
+            tb = traceback.cut(path=example_module_path)
+            tb = tb[1]
+            if getattr(tb, '_rawentry', None) is not None:
+                traceback = Traceback(tb._rawentry)
+            return traceback
+
+    else:
+
+        def _prunetraceback(self, excinfo):
+            tb = excinfo.traceback.cut(path=example_module_path)
+            tb = tb[1]
+            if getattr(tb, '_rawentry', None) is not None:
+                excinfo.traceback = Traceback(tb._rawentry, excinfo)
 
     def repr_failure(
         self,
         excinfo: ExceptionInfo[BaseException],
         style = None,
     ) -> Union[str, TerminalRepr]:
         if isinstance(excinfo.value, SybilFailure):
```

### Comparing `sybil-5.0.2/sybil/integration/unittest.py` & `sybil-5.0.3/sybil/integration/unittest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/abstract/clear.py` & `sybil-5.0.3/sybil/parsers/abstract/clear.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/abstract/codeblock.py` & `sybil-5.0.3/sybil/parsers/abstract/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/abstract/doctest.py` & `sybil-5.0.3/sybil/parsers/abstract/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/abstract/lexers.py` & `sybil-5.0.3/sybil/parsers/abstract/lexers.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/abstract/skip.py` & `sybil-5.0.3/sybil/parsers/abstract/skip.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/myst/codeblock.py` & `sybil-5.0.3/sybil/parsers/myst/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/myst/doctest.py` & `sybil-5.0.3/sybil/parsers/myst/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/myst/lexers.py` & `sybil-5.0.3/sybil/parsers/myst/lexers.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/rest/capture.py` & `sybil-5.0.3/sybil/parsers/rest/capture.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/rest/codeblock.py` & `sybil-5.0.3/sybil/parsers/rest/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/rest/doctest.py` & `sybil-5.0.3/sybil/parsers/rest/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/parsers/rest/lexers.py` & `sybil-5.0.3/sybil/parsers/rest/lexers.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/python.py` & `sybil-5.0.3/sybil/python.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/region.py` & `sybil-5.0.3/sybil/region.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil/sybil.py` & `sybil-5.0.3/sybil/sybil.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.2/sybil.egg-info/PKG-INFO` & `sybil-5.0.3/sybil.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sybil
-Version: 5.0.2
+Version: 5.0.3
 Summary: Automated testing for the examples in your code and documentation.
 Home-page: https://github.com/simplistix/sybil
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: build
 License-File: LICENSE.txt
@@ -29,9 +28,7 @@
 
 This library provides a way to check examples in your code and documentation by parsing
 them from their source and evaluating the parsed examples as part of
 your normal test run. Integration is provided for the main Python test
 runners.
 
 The `documentation <https://sybil.readthedocs.io/>`__ is the best place to start.
-
-
```

### Comparing `sybil-5.0.2/sybil.egg-info/SOURCES.txt` & `sybil-5.0.3/sybil.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -42,8 +42,26 @@
 sybil/parsers/myst/skip.py
 sybil/parsers/rest/__init__.py
 sybil/parsers/rest/capture.py
 sybil/parsers/rest/clear.py
 sybil/parsers/rest/codeblock.py
 sybil/parsers/rest/doctest.py
 sybil/parsers/rest/lexers.py
-sybil/parsers/rest/skip.py
+sybil/parsers/rest/skip.py
+tests/test_capture.py
+tests/test_clear.py
+tests/test_codeblock.py
+tests/test_compatibility.py
+tests/test_docs_examples.py
+tests/test_doctest.py
+tests/test_document.py
+tests/test_functional.py
+tests/test_helpers.py
+tests/test_lexing.py
+tests/test_myst_clear.py
+tests/test_myst_codeblock.py
+tests/test_myst_doctest.py
+tests/test_myst_lexers.py
+tests/test_myst_skip.py
+tests/test_rest_lexers.py
+tests/test_skip.py
+tests/test_sybil.py
```

