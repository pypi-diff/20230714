# Comparing `tmp/mtg_ssm-2.6.2.dev6.tar.gz` & `tmp/mtg_ssm-2.6.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtg_ssm-2.6.2.dev6.tar", last modified: Thu Jul 13 09:05:24 2023, max compression
+gzip compressed data, was "mtg_ssm-2.6.3.dev1.tar", last modified: Fri Jul 14 07:57:12 2023, max compression
```

## Comparing `mtg_ssm-2.6.2.dev6.tar` & `mtg_ssm-2.6.3.dev1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.391107 mtg_ssm-2.6.2.dev6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.391107 mtg_ssm-2.6.2.dev6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.github/workflows/integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.395107 mtg_ssm-2.6.2.dev6/mtg_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.395107 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.395107 mtg_ssm-2.6.2.dev6/mtg_ssm/mtg/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/mtg/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.395107 mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.399107 mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.395107 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.399107 mtg_ssm-2.6.2.dev6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.399107 mtg_ssm-2.6.2.dev6/tests/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/containers/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/containers/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/containers/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/containers/test_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.399107 mtg_ssm-2.6.2.dev6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/bulk_data.json
--rw-r--r--   0 runner    (1001) docker     (123)   456765 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/cards.json
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/migrations.json
--rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/sets.json
--rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/sets1.json
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/sets2.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     6650 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/gen_testdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.399107 mtg_ssm-2.6.2.dev6/tests/mtg/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/mtg/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/tests/scryfall/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/scryfall/test_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/tests/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/tests/serialization/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/__snapshots__/test_csv.ambr
--rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/__snapshots__/test_xlsx.ambr
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/test_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/test_ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.479776 mtg_ssm-2.6.3.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.471776 mtg_ssm-2.6.3.dev1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.471776 mtg_ssm-2.6.3.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/.github/workflows/integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-14 07:57:12.479776 mtg_ssm-2.6.3.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.471776 mtg_ssm-2.6.3.dev1/mtg_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 07:57:12.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.475776 mtg_ssm-2.6.3.dev1/mtg_ssm/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/containers/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/containers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/containers/counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/containers/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/containers/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.475776 mtg_ssm-2.6.3.dev1/mtg_ssm/mtg/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/mtg/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.475776 mtg_ssm-2.6.3.dev1/mtg_ssm/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/scryfall/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/scryfall/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.475776 mtg_ssm-2.6.3.dev1/mtg_ssm/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/serialization/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/serialization/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/serialization/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/mtg_ssm/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.471776 mtg_ssm-2.6.3.dev1/mtg_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-14 07:57:12.000000 mtg_ssm-2.6.3.dev1/mtg_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-14 07:57:12.000000 mtg_ssm-2.6.3.dev1/mtg_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:57:12.000000 mtg_ssm-2.6.3.dev1/mtg_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 07:57:12.000000 mtg_ssm-2.6.3.dev1/mtg_ssm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-14 07:57:12.000000 mtg_ssm-2.6.3.dev1/mtg_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 07:57:12.000000 mtg_ssm-2.6.3.dev1/mtg_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 07:57:12.479776 mtg_ssm-2.6.3.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.475776 mtg_ssm-2.6.3.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.475776 mtg_ssm-2.6.3.dev1/tests/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/containers/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/containers/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/containers/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/containers/test_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.475776 mtg_ssm-2.6.3.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/data/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/data/bulk_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)   456765 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/data/cards.json
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/data/migrations.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/data/sets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/data/sets1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/data/sets2.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6650 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/gen_testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.479776 mtg_ssm-2.6.3.dev1/tests/mtg/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/mtg/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.479776 mtg_ssm-2.6.3.dev1/tests/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/scryfall/test_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.479776 mtg_ssm-2.6.3.dev1/tests/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/serialization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:57:12.479776 mtg_ssm-2.6.3.dev1/tests/serialization/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/serialization/__snapshots__/test_csv.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/serialization/__snapshots__/test_xlsx.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/serialization/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/serialization/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/serialization/test_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-14 07:57:03.000000 mtg_ssm-2.6.3.dev1/tests/test_ssm.py
```

### Comparing `mtg_ssm-2.6.2.dev6/.github/workflows/integration.yml` & `mtg_ssm-2.6.3.dev1/.github/workflows/integration.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/.github/workflows/publish.yml` & `mtg_ssm-2.6.3.dev1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/.github/workflows/run-tests.yml` & `mtg_ssm-2.6.3.dev1/.github/workflows/run-tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -35,25 +35,25 @@
       - name: Execute pytest
         run: pytest tests/
 
       - name: Convert coverage
         run: coverage lcov
 
       - name: Coveralls Parallel
-        uses: coverallsapp/github-action@v1.2.4
+        uses: coverallsapp/github-action@v2.2.1
         with:
           github-token: ${{ secrets.github_token }}
           flag-name: python-${{ matrix.python-version }}
           path-to-lcov: coverage.lcov
           parallel: true
 
   finish:
     needs:
       - pytest
     runs-on: ubuntu-latest
     steps:
       - name: Coveralls Finished
-        uses: coverallsapp/github-action@v1.2.4
+        uses: coverallsapp/github-action@v2.2.1
         with:
           github-token: ${{ secrets.github_token }}
           path-to-lcov: coverage.lcov
           parallel-finished: true
```

### Comparing `mtg_ssm-2.6.2.dev6/.gitignore` & `mtg_ssm-2.6.3.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/.pre-commit-config.yaml` & `mtg_ssm-2.6.3.dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/LICENSE.txt` & `mtg_ssm-2.6.3.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/PKG-INFO` & `mtg_ssm-2.6.3.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg_ssm
-Version: 2.6.2.dev6
+Version: 2.6.3.dev1
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mtg_ssm-2.6.2.dev6/README.rst` & `mtg_ssm-2.6.3.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/containers/bundles.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/containers/bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/containers/collection.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/containers/collection.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/containers/counts.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/containers/counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/containers/indexes.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/containers/indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/containers/legacy.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/containers/legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/mtg/util.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/mtg/util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/fetcher.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/scryfall/fetcher.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/models.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/scryfall/models.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/csv.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/serialization/csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/interface.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/serialization/interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/xlsx.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/serialization/xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm/ssm.py` & `mtg_ssm-2.6.3.dev1/mtg_ssm/ssm.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/PKG-INFO` & `mtg_ssm-2.6.3.dev1/mtg_ssm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg-ssm
-Version: 2.6.2.dev6
+Version: 2.6.3.dev1
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/SOURCES.txt` & `mtg_ssm-2.6.3.dev1/mtg_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/pylintrc` & `mtg_ssm-2.6.3.dev1/pylintrc`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/pyproject.toml` & `mtg_ssm-2.6.3.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/conftest.py` & `mtg_ssm-2.6.3.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/containers/test_bundles.py` & `mtg_ssm-2.6.3.dev1/tests/containers/test_bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/containers/test_counts.py` & `mtg_ssm-2.6.3.dev1/tests/containers/test_counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/containers/test_indexes.py` & `mtg_ssm-2.6.3.dev1/tests/containers/test_indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/containers/test_legacy.py` & `mtg_ssm-2.6.3.dev1/tests/containers/test_legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/data/bulk_data.json` & `mtg_ssm-2.6.3.dev1/tests/data/bulk_data.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/data/cards.json` & `mtg_ssm-2.6.3.dev1/tests/data/cards.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/data/migrations.json` & `mtg_ssm-2.6.3.dev1/tests/data/migrations.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/data/sets.json` & `mtg_ssm-2.6.3.dev1/tests/data/sets.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/data/sets1.json` & `mtg_ssm-2.6.3.dev1/tests/data/sets1.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/data/sets2.json` & `mtg_ssm-2.6.3.dev1/tests/data/sets2.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/gen_testdata.py` & `mtg_ssm-2.6.3.dev1/tests/gen_testdata.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/mtg/test_util.py` & `mtg_ssm-2.6.3.dev1/tests/mtg/test_util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/scryfall/test_fetcher.py` & `mtg_ssm-2.6.3.dev1/tests/scryfall/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/serialization/__snapshots__/test_csv.ambr` & `mtg_ssm-2.6.3.dev1/tests/serialization/__snapshots__/test_csv.ambr`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/serialization/__snapshots__/test_xlsx.ambr` & `mtg_ssm-2.6.3.dev1/tests/serialization/__snapshots__/test_xlsx.ambr`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/serialization/test_csv.py` & `mtg_ssm-2.6.3.dev1/tests/serialization/test_csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/serialization/test_interface.py` & `mtg_ssm-2.6.3.dev1/tests/serialization/test_interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/serialization/test_xlsx.py` & `mtg_ssm-2.6.3.dev1/tests/serialization/test_xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev6/tests/test_ssm.py` & `mtg_ssm-2.6.3.dev1/tests/test_ssm.py`

 * *Files identical despite different names*

