# Comparing `tmp/hipscat-import-0.0.5.tar.gz` & `tmp/hipscat-import-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat-import-0.0.5.tar", last modified: Thu Jul 13 13:38:28 2023, max compression
+gzip compressed data, was "hipscat-import-0.1.tar", last modified: Fri Jul 14 14:09:10 2023, max compression
```

## Comparing `hipscat-import-0.0.5.tar` & `hipscat-import-0.1.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.github/workflows/type-checking.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/docs/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/debug.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/docs/catalogs/public/
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/public/allwise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/public/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/public/neowise.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/public/tic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/public/zubercal.rst
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/catalogs/resume.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/guide/association.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/guide/contact.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/guide/index_table.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/guide/margin_cache.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/notebooks/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     9556 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/notebooks/estimate_pixel_threshold.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)   136863 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/static/allwise_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/static/allwise_types.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/static/neowise_types.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/docs/static/tic_types.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20793 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/src/hipscat_import/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/src/hipscat_import/association/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/association/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/association/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/association/run_association.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/src/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/file_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/catalog/run_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/src/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/index/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/index/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/index/run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/src/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/margin_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/src/hipscat_import/runtime_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.649783 hipscat-import-0.0.5/src/hipscat_import.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 13:38:28.000000 hipscat-import-0.0.5/src/hipscat_import.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/hipscat_import/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/hipscat_import/association/
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/association/test_association_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/association/test_association_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/association/test_run_association.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_file_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_run_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/catalog/test_run_round_trip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/tests/hipscat_import/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/hipscat_import/data/blank/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/blank/blank.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.653783 hipscat-import-0.0.5/tests/hipscat_import/data/mixed_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/mixed_schema/input_01.csv
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/mixed_schema/input_02.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/mixed_schema/schema.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/resume/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/resume/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/resume/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/resume/intermediate/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/resume/intermediate/reducing_log.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.657783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.661783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.661783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.661783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.661783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source/
--rw-r--r--   0 runner    (1001) docker     (123)  1688789 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.665783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.641783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.665783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.665783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)   133704 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.645783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.665783 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    86295 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    92667 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    99907 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    42210 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    54775 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    72993 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    67804 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    80298 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
--rw-r--r--   0 runner    (1001) docker     (123)   162097 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    31794 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    43738 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)    29241 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/catalog.starr
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/multiindex.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/pandasindex.parquet
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/pipe_delimited.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/small_sky.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/tests/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/index/test_index_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/index/test_index_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/index/test_run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:28.669783 hipscat-import-0.0.5/tests/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-13 13:38:12.000000 hipscat-import-0.0.5/tests/hipscat_import/test_runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.784211 hipscat-import-0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-14 14:08:58.000000 hipscat-import-0.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-14 14:08:58.000000 hipscat-import-0.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.760210 hipscat-import-0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-14 14:08:58.000000 hipscat-import-0.1/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-14 14:08:58.000000 hipscat-import-0.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 14:08:58.000000 hipscat-import-0.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-14 14:08:58.000000 hipscat-import-0.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-14 14:08:58.000000 hipscat-import-0.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-14 14:08:58.000000 hipscat-import-0.1/.github/workflows/type-checking.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-14 14:08:58.000000 hipscat-import-0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-14 14:08:58.000000 hipscat-import-0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-14 14:08:58.000000 hipscat-import-0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-14 14:08:58.000000 hipscat-import-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-14 14:09:10.784211 hipscat-import-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-14 14:08:58.000000 hipscat-import-0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.760210 hipscat-import-0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.760210 hipscat-import-0.1/docs/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/catalogs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/catalogs/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/catalogs/debug.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.760210 hipscat-import-0.1/docs/catalogs/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/catalogs/public/allwise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/catalogs/public/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/catalogs/public/neowise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/catalogs/public/tic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/catalogs/public/zubercal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/catalogs/resume.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.760210 hipscat-import-0.1/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/guide/association.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/guide/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/guide/index_table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/guide/margin_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.760210 hipscat-import-0.1/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/notebooks/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9556 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/notebooks/estimate_pixel_threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.764211 hipscat-import-0.1/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   136863 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/static/allwise_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/static/allwise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/static/neowise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-14 14:08:58.000000 hipscat-import-0.1/docs/static/tic_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-14 14:08:58.000000 hipscat-import-0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:09:10.784211 hipscat-import-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.764211 hipscat-import-0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20793 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.764211 hipscat-import-0.1/src/hipscat_import/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-14 14:09:10.000000 hipscat-import-0.1/src/hipscat_import/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.764211 hipscat-import-0.1/src/hipscat_import/association/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/association/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/association/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/association/run_association.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.764211 hipscat-import-0.1/src/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/catalog/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/catalog/file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/catalog/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/catalog/resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/catalog/run_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.768211 hipscat-import-0.1/src/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/index/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/index/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/index/run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.768211 hipscat-import-0.1/src/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/margin_cache/margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/margin_cache/margin_cache_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-14 14:08:58.000000 hipscat-import-0.1/src/hipscat_import/runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.764211 hipscat-import-0.1/src/hipscat_import.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-14 14:09:10.000000 hipscat-import-0.1/src/hipscat_import.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-07-14 14:09:10.000000 hipscat-import-0.1/src/hipscat_import.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:09:10.000000 hipscat-import-0.1/src/hipscat_import.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-14 14:09:10.000000 hipscat-import-0.1/src/hipscat_import.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 14:09:10.000000 hipscat-import-0.1/src/hipscat_import.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.768211 hipscat-import-0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.768211 hipscat-import-0.1/tests/hipscat_import/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.768211 hipscat-import-0.1/tests/hipscat_import/association/
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/association/test_association_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/association/test_association_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/association/test_run_association.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.768211 hipscat-import-0.1/tests/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/catalog/test_argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/catalog/test_file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/catalog/test_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/catalog/test_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/catalog/test_run_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/catalog/test_run_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.768211 hipscat-import-0.1/tests/hipscat_import/data/blank/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/blank/blank.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.768211 hipscat-import-0.1/tests/hipscat_import/data/mixed_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/mixed_schema/input_01.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/mixed_schema/input_02.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/mixed_schema/schema.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.768211 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.772210 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.772210 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.772210 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.772210 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/resume/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/resume/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.772210 hipscat-import-0.1/tests/hipscat_import/data/resume/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.772210 hipscat-import-0.1/tests/hipscat_import/data/resume/intermediate/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/resume/intermediate/reducing_log.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.772210 hipscat-import-0.1/tests/hipscat_import/data/small_sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.772210 hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.776211 hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.776211 hipscat-import-0.1/tests/hipscat_import/data/small_sky_parts/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.776211 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source/
+-rw-r--r--   0 runner    (1001) docker     (123)  1688789 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.776211 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.776211 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.780211 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)   133704 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.756210 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.780211 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    86295 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    92667 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    99907 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    42210 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    54775 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    72993 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    67804 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    80298 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)   162097 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    31794 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    43738 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)    29241 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.780211 hipscat-import-0.1/tests/hipscat_import/data/test_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/test_formats/catalog.starr
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/test_formats/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/test_formats/multiindex.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/test_formats/pandasindex.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/test_formats/pipe_delimited.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/data/test_formats/small_sky.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.784211 hipscat-import-0.1/tests/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/index/test_index_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/index/test_index_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/index/test_run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:09:10.784211 hipscat-import-0.1/tests/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/margin_cache/test_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-14 14:08:58.000000 hipscat-import-0.1/tests/hipscat_import/test_runtime_arguments.py
```

### Comparing `hipscat-import-0.0.5/.github/pull_request_template.md` & `hipscat-import-0.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/.github/workflows/build-documentation.yml` & `hipscat-import-0.1/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/.github/workflows/linting.yml` & `hipscat-import-0.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/.github/workflows/publish-to-pypi.yml` & `hipscat-import-0.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/.github/workflows/smoke-test.yml` & `hipscat-import-0.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/.github/workflows/testing-and-coverage.yml` & `hipscat-import-0.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/.github/workflows/type-checking.yml` & `hipscat-import-0.1/.github/workflows/type-checking.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/.gitignore` & `hipscat-import-0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/.pre-commit-config.yaml` & `hipscat-import-0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/LICENSE` & `hipscat-import-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/PKG-INFO` & `hipscat-import-0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.0.5
+Version: 0.1
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hipscat-import-0.0.5/README.md` & `hipscat-import-0.1/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/Makefile` & `hipscat-import-0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/catalogs/advanced.rst` & `hipscat-import-0.1/docs/catalogs/advanced.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/catalogs/arguments.rst` & `hipscat-import-0.1/docs/catalogs/arguments.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/catalogs/public/allwise.rst` & `hipscat-import-0.1/docs/catalogs/public/allwise.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/catalogs/public/index.rst` & `hipscat-import-0.1/docs/catalogs/public/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/catalogs/public/neowise.rst` & `hipscat-import-0.1/docs/catalogs/public/neowise.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/catalogs/public/tic.rst` & `hipscat-import-0.1/docs/catalogs/public/tic.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/catalogs/public/zubercal.rst` & `hipscat-import-0.1/docs/catalogs/public/zubercal.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/catalogs/resume.rst` & `hipscat-import-0.1/docs/catalogs/resume.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/conf.py` & `hipscat-import-0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/guide/contributing.rst` & `hipscat-import-0.1/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/index.rst` & `hipscat-import-0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/notebooks/estimate_pixel_threshold.ipynb` & `hipscat-import-0.1/docs/notebooks/estimate_pixel_threshold.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/static/allwise_schema.parquet` & `hipscat-import-0.1/docs/static/allwise_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/static/allwise_types.csv` & `hipscat-import-0.1/docs/static/allwise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/static/neowise_types.csv` & `hipscat-import-0.1/docs/static/neowise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/docs/static/tic_types.csv` & `hipscat-import-0.1/docs/static/tic_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/pyproject.toml` & `hipscat-import-0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/.pylintrc` & `hipscat-import-0.1/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/association/arguments.py` & `hipscat-import-0.1/src/hipscat_import/association/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/association/map_reduce.py` & `hipscat-import-0.1/src/hipscat_import/association/map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/association/run_association.py` & `hipscat-import-0.1/src/hipscat_import/association/run_association.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/catalog/arguments.py` & `hipscat-import-0.1/src/hipscat_import/catalog/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/catalog/file_readers.py` & `hipscat-import-0.1/src/hipscat_import/catalog/file_readers.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/catalog/map_reduce.py` & `hipscat-import-0.1/src/hipscat_import/catalog/map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/catalog/resume_plan.py` & `hipscat-import-0.1/src/hipscat_import/catalog/resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/catalog/run_import.py` & `hipscat-import-0.1/src/hipscat_import/catalog/run_import.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/index/arguments.py` & `hipscat-import-0.1/src/hipscat_import/index/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/index/map_reduce.py` & `hipscat-import-0.1/src/hipscat_import/index/map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/index/run_index.py` & `hipscat-import-0.1/src/hipscat_import/index/run_index.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache.py` & `hipscat-import-0.1/src/hipscat_import/margin_cache/margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache_arguments.py` & `hipscat-import-0.1/src/hipscat_import/margin_cache/margin_cache_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/margin_cache/margin_cache_map_reduce.py` & `hipscat-import-0.1/src/hipscat_import/margin_cache/margin_cache_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/pipeline.py` & `hipscat-import-0.1/src/hipscat_import/pipeline.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import/runtime_arguments.py` & `hipscat-import-0.1/src/hipscat_import/runtime_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/src/hipscat_import.egg-info/PKG-INFO` & `hipscat-import-0.1/src/hipscat_import.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.0.5
+Version: 0.1
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hipscat-import-0.0.5/src/hipscat_import.egg-info/SOURCES.txt` & `hipscat-import-0.1/src/hipscat_import.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/.pylintrc` & `hipscat-import-0.1/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/association/test_association_argument.py` & `hipscat-import-0.1/tests/hipscat_import/association/test_association_argument.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/association/test_association_map_reduce.py` & `hipscat-import-0.1/tests/hipscat_import/association/test_association_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/association/test_run_association.py` & `hipscat-import-0.1/tests/hipscat_import/association/test_run_association.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/catalog/test_argument_validation.py` & `hipscat-import-0.1/tests/hipscat_import/catalog/test_argument_validation.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/catalog/test_file_readers.py` & `hipscat-import-0.1/tests/hipscat_import/catalog/test_file_readers.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/catalog/test_map_reduce.py` & `hipscat-import-0.1/tests/hipscat_import/catalog/test_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/catalog/test_resume_plan.py` & `hipscat-import-0.1/tests/hipscat_import/catalog/test_resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/catalog/test_run_import.py` & `hipscat-import-0.1/tests/hipscat_import/catalog/test_run_import.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/catalog/test_run_round_trip.py` & `hipscat-import-0.1/tests/hipscat_import/catalog/test_run_round_trip.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/conftest.py` & `hipscat-import-0.1/tests/hipscat_import/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/mixed_schema/schema.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/mixed_schema/schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky/catalog.csv` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky/catalog.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/_metadata` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source/small_sky_source.csv` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source/small_sky_source.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/_metadata` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json` & `hipscat-import-0.1/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/catalog.starr` & `hipscat-import-0.1/tests/hipscat_import/data/test_formats/catalog.starr`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/multiindex.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/test_formats/multiindex.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/pandasindex.parquet` & `hipscat-import-0.1/tests/hipscat_import/data/test_formats/pandasindex.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/data/test_formats/small_sky.fits` & `hipscat-import-0.1/tests/hipscat_import/data/test_formats/small_sky.fits`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/index/test_index_argument.py` & `hipscat-import-0.1/tests/hipscat_import/index/test_index_argument.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/index/test_index_map_reduce.py` & `hipscat-import-0.1/tests/hipscat_import/index/test_index_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/index/test_run_index.py` & `hipscat-import-0.1/tests/hipscat_import/index/test_run_index.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py` & `hipscat-import-0.1/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_margin_cache.py` & `hipscat-import-0.1/tests/hipscat_import/margin_cache/test_margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py` & `hipscat-import-0.1/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.5/tests/hipscat_import/test_runtime_arguments.py` & `hipscat-import-0.1/tests/hipscat_import/test_runtime_arguments.py`

 * *Files identical despite different names*

