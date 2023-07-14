# Comparing `tmp/gable-0.0.1a2.tar.gz` & `tmp/gable-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gable-0.0.1a2.tar", max compression
+gzip compressed data, was "gable-0.1.0.tar", max compression
```

## Comparing `gable-0.0.1a2.tar` & `gable-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,24 @@
--rw-r--r--   0        0        0        0 2023-06-13 23:27:44.590688 gable-0.0.1a2/gable/__init__.py
--rw-r--r--   0        0        0       76 2023-07-09 16:59:25.836461 gable-0.0.1a2/gable/cli.py
--rw-r--r--   0        0        0      652 2023-07-09 16:59:48.589676 gable-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 gable-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     2581 2023-07-14 21:13:07.778057 gable-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 23:27:44.590688 gable-0.1.0/gable/__init__.py
+-rw-r--r--   0        0        0     1064 2023-07-14 02:46:30.175869 gable-0.1.0/gable/cli.py
+-rw-r--r--   0        0        0     1946 2023-07-12 15:45:20.731121 gable-0.1.0/gable/client.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:23:36.262951 gable-0.1.0/gable/commands/__init__.py
+-rw-r--r--   0        0        0      448 2023-07-14 02:46:30.175999 gable-0.1.0/gable/commands/auth.py
+-rw-r--r--   0        0        0     4549 2023-07-14 21:03:16.563277 gable-0.1.0/gable/commands/contract.py
+-rw-r--r--   0        0        0    21700 2023-07-14 21:03:16.563495 gable-0.1.0/gable/commands/data_asset.py
+-rw-r--r--   0        0        0      629 2023-07-14 02:46:30.176575 gable-0.1.0/gable/commands/ping.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:23:36.263584 gable-0.1.0/gable/helpers/__init__.py
+-rw-r--r--   0        0        0     3071 2023-07-14 21:03:16.563951 gable-0.1.0/gable/helpers/check.py
+-rw-r--r--   0        0        0     1824 2023-07-14 02:46:30.176848 gable-0.1.0/gable/helpers/contract.py
+-rw-r--r--   0        0        0     4260 2023-07-14 21:03:16.564126 gable-0.1.0/gable/helpers/data_asset.py
+-rw-r--r--   0        0        0      143 2023-07-12 20:37:22.605800 gable-0.1.0/gable/helpers/emoji.py
+-rw-r--r--   0        0        0     1774 2023-07-14 21:03:16.564231 gable-0.1.0/gable/helpers/multi_option.py
+-rw-r--r--   0        0        0     1039 2023-07-14 21:03:16.564779 gable-0.1.0/gable/helpers/repo_interactions.py
+-rw-r--r--   0        0        0    13598 2023-07-14 02:46:30.177304 gable-0.1.0/gable/openapi.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:14:49.025833 gable-0.1.0/gable/readers/__init__.py
+-rw-r--r--   0        0        0     4027 2023-07-12 19:04:49.765702 gable-0.1.0/gable/readers/dbapi.py
+-rw-r--r--   0        0        0      255 2023-07-14 02:57:36.313991 gable-0.1.0/gable/readers/file.py
+-rw-r--r--   0        0        0      638 2023-07-12 19:04:49.766457 gable-0.1.0/gable/readers/mysql.py
+-rw-r--r--   0        0        0      668 2023-07-12 19:04:49.766743 gable-0.1.0/gable/readers/postgres.py
+-rw-r--r--   0        0        0     1249 2023-07-14 21:13:07.778312 gable-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3487 1970-01-01 00:00:00.000000 gable-0.1.0/PKG-INFO
```

