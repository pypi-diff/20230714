# Comparing `tmp/hipscat-0.0.9.tar.gz` & `tmp/hipscat-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat-0.0.9.tar", last modified: Thu Apr 13 18:52:35 2023, max compression
+gzip compressed data, was "hipscat-0.1.tar", last modified: Fri Jul 14 14:08:34 2023, max compression
```

## Comparing `hipscat-0.0.9.tar` & `hipscat-0.1.tar`

### file list

```diff
@@ -1,111 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.544044 hipscat-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-13 18:52:25.000000 hipscat-0.0.9/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.512043 hipscat-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.524043 hipscat-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-13 18:52:25.000000 hipscat-0.0.9/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 18:52:25.000000 hipscat-0.0.9/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 18:52:25.000000 hipscat-0.0.9/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-13 18:52:25.000000 hipscat-0.0.9/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-13 18:52:25.000000 hipscat-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-13 18:52:25.000000 hipscat-0.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-13 18:52:25.000000 hipscat-0.0.9/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-13 18:52:25.000000 hipscat-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-13 18:52:35.540044 hipscat-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-13 18:52:25.000000 hipscat-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 18:52:25.000000 hipscat-0.0.9/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.524043 hipscat-0.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.528044 hipscat-0.0.9/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/guide/directory_scheme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.528044 hipscat-0.0.9/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 18:52:25.000000 hipscat-0.0.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.528044 hipscat-0.0.9/nb/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 18:52:25.000000 hipscat-0.0.9/nb/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-13 18:52:25.000000 hipscat-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:52:35.544044 hipscat-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.528044 hipscat-0.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20808 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.528044 hipscat-0.0.9/src/hipscat/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/src/hipscat/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/catalog_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/partition_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/pixel_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/pixel_node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/catalog/pixel_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/src/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/inspection/visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/src/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/src/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/file_io/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/file_io/file_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/io/write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/src/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-13 18:52:25.000000 hipscat-0.0.9/src/hipscat/pixel_math/pixel_margins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.532044 hipscat-0.0.9/src/hipscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 18:52:35.000000 hipscat-0.0.9/src/hipscat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.516044 hipscat-0.0.9/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/tests/data/small_sky/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.516044 hipscat-0.0.9/tests/data/small_sky/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.536044 hipscat-0.0.9/tests/data/small_sky/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky/point_map.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/data/small_sky_order1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.516044 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/data/small_sky_order1/point_map.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.520043 hipscat-0.0.9/tests/hipscat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/hipscat/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/test_catalog_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/test_partition_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/test_pixel_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/catalog/test_pixel_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/inspection/test_visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/io/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/io/file_io/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/io/file_io/test_file_pointers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/io/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/io/test_write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:35.540044 hipscat-0.0.9/tests/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/pixel_math/test_healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/pixel_math/test_hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/pixel_math/test_margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/pixel_math/test_partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-13 18:52:25.000000 hipscat-0.0.9/tests/hipscat/pixel_math/test_pixel_margins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-14 14:08:22.000000 hipscat-0.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.568761 hipscat-0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-14 14:08:22.000000 hipscat-0.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-14 14:08:22.000000 hipscat-0.1/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-14 14:08:22.000000 hipscat-0.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 14:08:22.000000 hipscat-0.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-14 14:08:22.000000 hipscat-0.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-14 14:08:22.000000 hipscat-0.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-14 14:08:22.000000 hipscat-0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-14 14:08:22.000000 hipscat-0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-14 14:08:22.000000 hipscat-0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-14 14:08:22.000000 hipscat-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-14 14:08:34.588762 hipscat-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-14 14:08:22.000000 hipscat-0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 14:08:22.000000 hipscat-0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-14 14:08:22.000000 hipscat-0.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-14 14:08:22.000000 hipscat-0.1/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-14 14:08:22.000000 hipscat-0.1/docs/guide/directory_scheme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-14 14:08:22.000000 hipscat-0.1/docs/guide/pixel_math.md
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-14 14:08:22.000000 hipscat-0.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-14 14:08:22.000000 hipscat-0.1/docs/notebooks/catalog_size_inspection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-14 14:08:22.000000 hipscat-0.1/docs/notebooks/cone_search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 14:08:22.000000 hipscat-0.1/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 14:08:22.000000 hipscat-0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-14 14:08:22.000000 hipscat-0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:08:34.588762 hipscat-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20808 2023-07-14 14:08:22.000000 hipscat-0.1/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/src/hipscat/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/src/hipscat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/src/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/association_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/association_catalog/association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/association_catalog/association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/association_catalog/partition_join_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/catalog_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/dataset/base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/dataset/catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/index/index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/partition_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/source_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/source_catalog/source_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/inspection/almanac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/inspection/almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/inspection/visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/file_io/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/file_io/file_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/src/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/healpix_pixel_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/pixel_margins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/src/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_tree/pixel_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_tree/pixel_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_tree/pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_tree/pixel_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/src/hipscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-07-14 14:08:22.000000 hipscat-0.1/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-14 14:08:22.000000 hipscat-0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.568761 hipscat-0.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/tests/data/almanac/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/dataset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/deprecated.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/index_catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/margin_cache.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/small_sky.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/small_sky_order1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/small_sky_source_catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/small_sky_to_small_sky_order1.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/tests/data/almanac_exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/association_missing_join.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/association_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/bad_catalog_path.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/bad_primary_path.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/bad_type.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/index_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/margin_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/standalone_source_catalog.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/tests/data/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/dataset/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/index_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/index_catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/margin_cache/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.568761 hipscat-0.1/tests/data/small_sky/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky/point_map.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky_order1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.568761 hipscat-0.1/tests/data/small_sky_order1/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/point_map.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_source/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_source/partition_info.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky_to_small_sky_order1/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_to_small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_to_small_sky_order1/partition_join_info.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/hipscat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/hipscat/catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/association_catalog/test_association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/association_catalog/test_partition_join_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/dataset/test_base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/dataset/test_catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/dataset/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/index/test_index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/test_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/test_partition_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/inspection/test_almanac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/inspection/test_almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/inspection/test_visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/io/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/io/file_io/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/io/file_io/test_file_pointers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/io/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/io/test_write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_math/test_healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_math/test_hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_math/test_margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_math/test_partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_math/test_pixel_margins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_tree/test_pixel_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_tree/test_pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_tree/test_pixel_tree_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/util/test_healpix_pixel_convertor.py
```

### Comparing `hipscat-0.0.9/.github/workflows/linting.yml` & `hipscat-0.1/.github/workflows/linting.yml`

 * *Files 18% similar despite different names*

```diff
@@ -8,20 +8,24 @@
     branches: [ main ]
   pull_request:
     branches: [ main ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ['3.8', '3.9', '3.10']
+
     steps:
     - uses: actions/checkout@v3
-    - name: Set up Python 3.10
+    - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
-        python-version: '3.10'
+        python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         sudo apt-get update
         python -m pip install --upgrade pip
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
```

### Comparing `hipscat-0.0.9/.github/workflows/publish-to-pypi.yml` & `hipscat-0.1/.github/workflows/publish-to-pypi.yml`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: '3.x'
+        python-version: '3.10'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
```

### Comparing `hipscat-0.0.9/.github/workflows/smoke-test.yml` & `hipscat-0.1/.github/workflows/smoke-test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # It will install Python dependencies and run tests with a variety of Python versions.
 
 name: Unit test smoke test
 
 on:
   schedule:
     - cron: 45 6 * * *
+  # Allows you to run this workflow manually from the Actions tab
+  workflow_dispatch:
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
@@ -24,10 +26,13 @@
     - name: Install dependencies
       run: |
         sudo apt-get update
         python -m pip install --upgrade pip
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+    - name: List dependencies
+      run: |
+        pip list
     - name: Run unit tests with pytest
       run: |
         python -m pytest tests
```

### Comparing `hipscat-0.0.9/.github/workflows/testing-and-coverage.yml` & `hipscat-0.1/.github/workflows/testing-and-coverage.yml`

 * *Files 15% similar despite different names*

```diff
@@ -31,10 +31,7 @@
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Run unit tests with pytest
       run: |
         python -m pytest tests --cov=hipscat --cov-report=xml
     - name: Upload coverage report to codecov
       uses: codecov/codecov-action@v3
-    - name: Build docs
-      run: |
-        sphinx-build -T -E -b html -d docs/build/doctrees ./docs docs/build/html
```

### Comparing `hipscat-0.0.9/.gitignore` & `hipscat-0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/.pre-commit-config.yaml` & `hipscat-0.1/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -11,54 +11,54 @@
         description: Compare current template version against latest
         verbose: true
 
     # Clear output from jupyter notebooks so that only the input cells are committed.
   - repo: local
     hooks:
       - id: jupyter-nb-clear-output
-        name: jupyter-nb-clear-output
+        name: Clear output from Jupyter notebooks
         description: Clear output from Jupyter notebooks.
         files: \.ipynb$
         stages: [commit]
         language: system
-        entry: jupyter nbconvert --ClearOutputPreprocessor.enabled=True --inplace
+        entry: jupyter nbconvert --clear-output
 
     # Run unit tests, verify that they pass. Note that coverage is run against
     # the ./src directory here because that is what will be committed. In the 
     # github workflow script, the coverage is run against the installed package
     # and uploaded to Codecov by calling pytest like so:
     # `python -m pytest --cov=<package_name> --cov-report=xml`
   - repo: local
     hooks:
       - id: pytest-check
-        name: pytest-check
+        name: Run unit tests
         description: Run unit tests with pytest.
         entry: bash -c "if python -m pytest --co -qq; then python -m pytest --cov=./src --cov-report=html; fi"
         language: system
         pass_filenames: false
         always_run: true
 
     # prevents committing directly branches named 'main' and 'master'.
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: no-commit-to-branch
-        name: Don't commit to main or master branch
+        name: Prevent main branch commits
         description: Prevent the user from committing directly to the primary branch.
       - id: check-added-large-files
         name: Check for large files
         description: Prevent the user from committing very large files.
         args: ['--maxkb=500']
 
     # verify that pyproject.toml is well formed
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.12.1
     hooks:
       - id: validate-pyproject
-        name: Validate syntax of pyproject.toml
+        name: Validate pyproject.toml
         description: Verify that pyproject.toml adheres to the established schema.
 
     # Automatically sort the imports used in .py files
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
@@ -96,43 +96,33 @@
           [
             "-rn", # Only display messages
             "-sn", # Don't display the score
             "--rcfile=tests/.pylintrc",
           ]
 
 
-    # Analyze type hints and report errors.
-  - repo: local
-    hooks:
-      - id: mypy
-        name: mypy (python files in src/ and tests/)
-        entry: mypy
-        language: system
-        types: [python]
-        files: ^(src|tests)/
-        args:
-          [
-          
-            "--ignore-missing-imports", # Ignore imports without type hints
-          
-          ]
-
-    # Make sure Sphinx can build the documentation without issues.
+    # Make sure Sphinx can build the documentation while explicitly omitting 
+    # notebooks from the docs, so users don't have to wait through the execution 
+    # of each notebook or each commit. By default, these will be checked in the 
+    # GitHub workflows.
   - repo: local
     hooks:
       - id: sphinx-build
         name: Build documentation with Sphinx
         entry: sphinx-build
         language: system
         always_run: true
         exclude_types: [file, symlink]
         args:
           [
+            "-M", # Run sphinx in make mode, so we can use -D flag later
+                  # Note: -M requires next 3 args to be builder, source, output
+            "html", # Specify builder
+            "./docs", # Source directory of documents
+            "./_readthedocs", # Output directory for rendered documents
             "-T", # Show full trace back on exception
-            "-E", # Don't use saved env. always read all files.
-            "-b", # Flag to select which builder to use
-            "html", # Use the HTML builder
+            "-E", # Don't use saved env; always read all files
             "-d", # Flag for cached environment and doctrees
-            "docs/build/doctrees", # directory
-            "./docs", # Source directory of documents
-            "docs/build/html", # Output directory for rendered documents.
-          ]
+            "./docs/_build/doctrees", # Directory
+            "-D", # Flag to override settings in conf.py
+            "exclude_patterns=notebooks/*", # Exclude our notebooks from pre-commit
+          ]
```

### Comparing `hipscat-0.0.9/LICENSE` & `hipscat-0.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Astronomy Data Commons
+Copyright (c) 2023, LINCC Frameworks
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
 
@@ -21,8 +21,8 @@
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `hipscat-0.0.9/PKG-INFO` & `hipscat-0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.0.9
+Version: 0.1
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Astronomy Data Commons
+        Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
         
@@ -26,14 +26,15 @@
         DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
@@ -67,9 +68,15 @@
 * LSDB ([on GitHub](https://github.com/astronomy-commons/lsdb)) 
   ([on ReadTheDocs](https://lsdb.readthedocs.io/en/latest/))
 
 ## Contributing
 
 [![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/astronomy-commons/hipscat?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/astronomy-commons/hipscat/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
-See the [contribution guide](https://hipscat.readthedocs.io/en/latest/overview/contributing.html)
+See the [contribution guide](https://hipscat.readthedocs.io/en/latest/guide/contributing.html)
 for completed installation instructions and contribution best practices.
+
+## Acknowledgements
+
+LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative
+founded by Eric and Wendy Schmidt, as part of the Virtual Institute of 
+Astrophysics (VIA).
```

### Comparing `hipscat-0.0.9/README.md` & `hipscat-0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,9 +24,15 @@
 * LSDB ([on GitHub](https://github.com/astronomy-commons/lsdb)) 
   ([on ReadTheDocs](https://lsdb.readthedocs.io/en/latest/))
 
 ## Contributing
 
 [![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/astronomy-commons/hipscat?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/astronomy-commons/hipscat/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
-See the [contribution guide](https://hipscat.readthedocs.io/en/latest/overview/contributing.html)
+See the [contribution guide](https://hipscat.readthedocs.io/en/latest/guide/contributing.html)
 for completed installation instructions and contribution best practices.
+
+## Acknowledgements
+
+LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative
+founded by Eric and Wendy Schmidt, as part of the Virtual Institute of 
+Astrophysics (VIA).
```

### Comparing `hipscat-0.0.9/docs/Makefile` & `hipscat-0.1/docs/Makefile`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # Makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?= -T -E -d _build/doctrees -D language=en
+EXCLUDENB     ?= -D exclude_patterns="notebooks/*","_build","**.ipynb_checkpoints"
 SPHINXBUILD   ?= sphinx-build
 SOURCEDIR     = .
 BUILDDIR      = ../_readthedocs/
 
-.PHONY: help clean Makefile 
+.PHONY: help clean Makefile no-nb no-notebooks
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
+# Build all Sphinx docs locally, except the notebooks
+no-nb no-notebooks:
+	@$(SPHINXBUILD) -M html "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(EXCLUDENB) $(O)
+
 # Cleans up files generated by the build process
 clean:
 	rm -r "_build/doctrees"
 	rm -r "$(BUILDDIR)"
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
```

### Comparing `hipscat-0.0.9/docs/conf.py` & `hipscat-0.1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.mathjax", "sphinx.ext.napoleon", "sphinx.ext.viewcode"]
 
 extensions.append("autoapi.extension")
+extensions.append("nbsphinx")
+extensions.append("myst_parser")
 
 templates_path = []
 exclude_patterns = ["_build", "**.ipynb_checkpoints"]
 
 # This assumes that sphinx-build is called from the root directory
 master_doc = "index"
 # Remove 'view source code' from top of page (for html, not python)
```

### Comparing `hipscat-0.0.9/docs/guide/contributing.rst` & `hipscat-0.1/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/docs/guide/directory_scheme.rst` & `hipscat-0.1/docs/guide/directory_scheme.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/src/.pylintrc` & `hipscat-0.1/src/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -276,21 +276,21 @@
 # R0901)
 ignored-parents=
 
 # Maximum number of arguments for function / method.
 max-args=15
 
 # Maximum number of attributes for a class (see R0902).
-max-attributes=15
+max-attributes=25
 
 # Maximum number of boolean expressions in an if statement (see R0916).
 max-bool-expr=5
 
 # Maximum number of branch for function / method body.
-max-branches=12
+max-branches=20
 
 # Maximum number of locals for function / method body.
 max-locals=15
 
 # Maximum number of parents for a class (see R0901).
 max-parents=7
 
@@ -325,15 +325,15 @@
 indent-after-paren=4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
 indent-string='    '
 
 # Maximum number of characters on a single line.
-max-line-length=100
+max-line-length=110
 
 # Maximum number of lines in a module.
 max-module-lines=1000
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
```

### Comparing `hipscat-0.0.9/src/hipscat/catalog/catalog_parameters.py` & `hipscat-0.1/src/hipscat/catalog/dataset/dataset.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,74 @@
-"""Container class for properties of a catalog that is being created"""
+from typing import Tuple, Type
 
-from dataclasses import dataclass
+from typing_extensions import Self
 
-from hipscat.io import file_io
+from hipscat.catalog.dataset.base_catalog_info import BaseCatalogInfo
+from hipscat.io import FilePointer, file_io, paths
 
 
-@dataclass
-class CatalogParameters:
-    """Container class for catalog properties"""
-
-    catalog_name: str = ""
-    catalog_type: str = "object"
-    output_path: str = ""
-    epoch: str = "J2000"
-    ra_column: str = "ra"
-    dec_column: str = "dec"
-    total_rows: int = 0
-
-    CATALOG_TYPES = [
-        "object",
-        "source",
-        "index",
-        "association",
-        "margin",
-    ]
+class Dataset:
+    """A base HiPSCat dataset
 
-    def __post_init__(
-        self,
-    ):
+    A base dataset contains a catalog_info metadata file and the data contained in parquet files
+
+    TODO - create factory methods to get appropriately-typed datasets for
+    some catalog info or catalog directory
+    """
 
-        if self.catalog_type not in self.CATALOG_TYPES:
-            raise ValueError(f"Unknown catalog type: {self.catalog_type}")
+    CatalogInfoClass: Type[BaseCatalogInfo] = BaseCatalogInfo
 
-        output_path_pointer = file_io.get_file_pointer_from_path(self.output_path)
-        self.catalog_base_dir = file_io.append_paths_to_pointer(
-            output_path_pointer, self.catalog_name
-        )
-        self.catalog_path = str(self.catalog_base_dir)
-        file_io.make_directory(self.catalog_base_dir, exist_ok=True)
-
-    def __str__(self):
-        formatted_string = (
-            f"  catalog_name {self.catalog_name}\n"
-            f"  catalog_type {self.catalog_type}\n"
-            f"  epoch {self.epoch}\n"
-            f"  ra_column {self.ra_column}\n"
-            f"  dec_column {self.dec_column}\n"
-            f"  total_rows {self.total_rows}\n"
-            f"  output_path {self.output_path}\n"
-        )
-        return formatted_string
-
-
-def read_from_metadata_file(catalog_info_file):
-    """Read catalog parameters from a catalog_info.json file. Validate the parameters"""
-    metadata_keywords = file_io.load_json_file(catalog_info_file)
-    catalog_name = metadata_keywords["catalog_name"]
-    if not catalog_name:
-        raise ValueError("Catalog name is required in catalog info file.")
-
-    catalog_type = metadata_keywords.get("catalog_type", "object")
-    if catalog_type not in CatalogParameters.CATALOG_TYPES:
-        raise ValueError(f"Unknown catalog type: {catalog_type}")
-
-    return CatalogParameters(
-        catalog_name=catalog_name,
-        catalog_type=catalog_type,
-        epoch=metadata_keywords.get("epoch", "J2000"),
-        ra_column=metadata_keywords.get("ra_column", "ra"),
-        dec_column=metadata_keywords.get("dec_column", "dec"),
-        total_rows=int(metadata_keywords.get("total_rows", 0)),
-    )
+    def __init__(
+        self,
+        catalog_info: CatalogInfoClass,
+        catalog_path=None,
+    ) -> None:
+        """Initializes a Dataset
+
+        Args:
+            catalog_info: A catalog_info object with the catalog metadata
+            catalog_path: If the catalog is stored on disk, specify the location of the catalog
+                Does not load the catalog from this path, only store as metadata
+        """
+        if not isinstance(catalog_info, self.CatalogInfoClass):
+            raise TypeError(f"catalog_info type must be {self.CatalogInfoClass}")
+
+        self.catalog_info = catalog_info
+        self.catalog_name = self.catalog_info.catalog_name
+
+        self.catalog_path = catalog_path
+        self.on_disk = catalog_path is not None
+        self.catalog_base_dir = file_io.get_file_pointer_from_path(self.catalog_path)
+
+    @classmethod
+    def read_from_hipscat(cls, catalog_path: str) -> Self:
+        """Reads a HiPSCat Catalog from a HiPSCat directory
+
+        Args:
+            catalog_path: path to the root directory of the catalog
+
+        Returns:
+            The initialized catalog object
+        """
+        catalog_base_dir = file_io.get_file_pointer_from_path(catalog_path)
+        cls._check_files_exist(catalog_base_dir)
+        args = cls._read_args(catalog_base_dir)
+        kwargs = cls._read_kwargs(catalog_base_dir)
+        return cls(*args, **kwargs)
+
+    @classmethod
+    def _read_args(cls, catalog_base_dir: FilePointer) -> Tuple[CatalogInfoClass]:
+        catalog_info_file = paths.get_catalog_info_pointer(catalog_base_dir)
+        catalog_info = cls.CatalogInfoClass.read_from_metadata_file(catalog_info_file)
+        return (catalog_info,)
+
+    @classmethod
+    def _read_kwargs(cls, catalog_base_dir: FilePointer) -> dict:
+        return {"catalog_path": str(catalog_base_dir)}
+
+    @classmethod
+    def _check_files_exist(cls, catalog_base_dir: FilePointer):
+        if not file_io.does_file_or_directory_exist(catalog_base_dir):
+            raise FileNotFoundError(f"No directory exists at {str(catalog_base_dir)}")
+        catalog_info_file = paths.get_catalog_info_pointer(catalog_base_dir)
+        if not file_io.does_file_or_directory_exist(catalog_info_file):
+            raise FileNotFoundError(f"No catalog info found where expected: {str(catalog_info_file)}")
```

### Comparing `hipscat-0.0.9/src/hipscat/catalog/partition_info.py` & `hipscat-0.1/src/hipscat/catalog/association_catalog/partition_join_info.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,47 @@
-"""Container class to hold per-partition metadata"""
+import pandas as pd
+from typing_extensions import Self
 
-from typing import List
+from hipscat.io import FilePointer, file_io
 
-from hipscat.io import file_io, paths
-from hipscat.pixel_math import HealpixPixel
 
+class PartitionJoinInfo:
+    """Association catalog metadata with which partitions matches occur in the join"""
 
-class PartitionInfo:
-    """Container class for per-partition info."""
+    PRIMARY_ORDER_COLUMN_NAME = "Norder"
+    PRIMARY_PIXEL_COLUMN_NAME = "Npix"
+    JOIN_ORDER_COLUMN_NAME = "join_Norder"
+    JOIN_PIXEL_COLUMN_NAME = "join_Npix"
+
+    COLUMN_NAMES = [
+        PRIMARY_PIXEL_COLUMN_NAME,
+        PRIMARY_PIXEL_COLUMN_NAME,
+        JOIN_ORDER_COLUMN_NAME,
+        JOIN_PIXEL_COLUMN_NAME,
+    ]
+
+    def __init__(self, join_info_df: pd.DataFrame) -> None:
+        self.data_frame = join_info_df
+        self._check_column_names()
+
+    def _check_column_names(self):
+        for column in self.COLUMN_NAMES:
+            if column not in self.data_frame.columns:
+                raise ValueError(f"join_info_df does not contain column {column}")
+
+    @classmethod
+    def read_from_file(cls, partition_join_info_file: FilePointer) -> Self:
+        """Read partition join info from a `partition_join_info.csv` file to create an object
 
-    METADATA_ORDER_COLUMN_NAME = "Norder"
-    METADATA_DIR_COLUMN_NAME = "Dir"
-    METADATA_PIXEL_COLUMN_NAME = "Npix"
-
-    def __init__(self, catalog_base_dir: file_io.FilePointer) -> None:
-        self.catalog_base_dir = catalog_base_dir
-
-        partition_info_pointer = paths.get_partition_info_pointer(self.catalog_base_dir)
-        if not file_io.does_file_or_directory_exist(partition_info_pointer):
-            raise FileNotFoundError(
-                f"No partition info found where expected: {str(partition_info_pointer)}"
-            )
-
-        self.data_frame = file_io.load_csv_to_pandas(partition_info_pointer)
-
-    def get_healpix_pixels(self) -> List[HealpixPixel]:
-        """Get healpix pixel objects for all pixels represented as partitions.
+        Args:
+            partition_join_info_file: FilePointer to the `partition_join_info.csv` file
 
         Returns:
-            List of HealpixPixel
+            A `PartitionJoinInfo` object with the data from the file
         """
-        return [
-            HealpixPixel(order, pixel)
-            for order, pixel in zip(
-                self.data_frame[self.METADATA_ORDER_COLUMN_NAME],
-                self.data_frame[self.METADATA_PIXEL_COLUMN_NAME],
-            )
-        ]
-
-    def get_file_names(self):
-        """Get file handles for all partition files in the catalog
-
-        Returns:
-            one-dimensional array of strings, where each string is a partition file
-        """
-        file_names = []
-        for _, partition in self.data_frame.iterrows():
-            file_names.append(
-                paths.pixel_catalog_file(
-                    self.catalog_base_dir,
-                    partition[self.METADATA_ORDER_COLUMN_NAME],
-                    partition[self.METADATA_PIXEL_COLUMN_NAME],
-                )
+        if not file_io.does_file_or_directory_exist(partition_join_info_file):
+            raise FileNotFoundError(
+                f"No partition info found where expected: {str(partition_join_info_file)}"
             )
 
-        return file_names
+        data_frame = file_io.load_csv_to_pandas(partition_join_info_file)
+        return cls(data_frame)
```

### Comparing `hipscat-0.0.9/src/hipscat/catalog/pixel_node.py` & `hipscat-0.1/src/hipscat/pixel_tree/pixel_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,103 @@
 from __future__ import annotations
 
 from bisect import bisect
 from typing import List
 
-from hipscat.catalog.pixel_node_type import PixelNodeType
+from hipscat.pixel_math import HealpixInputTypes, get_healpix_pixel
+from hipscat.pixel_tree.pixel_node_type import PixelNodeType
 
 
 class PixelNode:
     """A node in the HiPSCat quadtree of HEALPix pixels
 
     Attributes:
-        hp_order: HEALPix order of the pixel
-        hp_pixel: HEALPix pixel number
         node_type: If the node is a leaf, root, or inner type
         parent: The parent pixel node in the tree
         children: The child nodes of the pixel
 
     """
 
     _NODE_TYPE_MAX_CHILDREN = {
         PixelNodeType.ROOT: 12,
         PixelNodeType.INNER: 4,
         PixelNodeType.LEAF: 0,
     }
 
     def __init__(
         self,
-        hp_order: int,
-        hp_pixel: int,
+        pixel: HealpixInputTypes,
         node_type: PixelNodeType,
         parent: PixelNode | None,
         children: List[PixelNode] | None = None,
-    ):
+    ) -> None:
         """Inits PixelNode with its attributes
 
         Raises:
             ValueError: Invalid arguments for the specified pixel type
         """
 
+        pixel = get_healpix_pixel(pixel)
+
         if node_type == PixelNodeType.ROOT:
             if parent is not None:
                 raise ValueError("Root node cannot have a parent")
-            if hp_order != -1:
+            if pixel.order != -1:
                 raise ValueError("Root node must be at order -1")
 
         if node_type in (PixelNodeType.INNER, PixelNodeType.LEAF):
             if parent is None:
                 raise ValueError("Inner and leaf nodes must have a parent")
-            if hp_pixel < 0 or hp_order < 0:
-                raise ValueError(
-                    "Inner and leaf nodes must have an order and pixel number >= 0"
-                )
+            if pixel.order < 0 or pixel.pixel < 0:
+                raise ValueError("Inner and leaf nodes must have an order and pixel number >= 0")
 
-        if parent is not None and parent.hp_order != hp_order - 1:
+        if parent is not None and parent.hp_order != pixel.order - 1:
             raise ValueError("Parent node must be at order one less than current node")
 
-        self.hp_order = hp_order
-        self.hp_pixel = hp_pixel
+        self.pixel = pixel
         self.node_type = node_type
         self.parent = parent
         self.children = []
 
         if children is not None:
             for child in children:
                 self.add_child_node(child)
 
         if self.parent is not None:
             self.parent.add_child_node(self)
 
+    @property
+    def hp_order(self):
+        """The order of the HealpixPixel the node is at"""
+        return self.pixel.order
+
+    @property
+    def hp_pixel(self):
+        """The pixel number in NESTED ordering of the HealpixPixel the node is at"""
+        return self.pixel.pixel
+
     def add_child_node(self, child: PixelNode):
         """Adds a child node to the node
 
         Maintains order of children based on pixel index
 
         Args:
             child: child node to add
 
         Raises:
             ValueError: The child to add does not have the current node set as a parent
             OverflowError: The node already has the maximum amount of children
         """
         if not child.parent == self:
-            raise ValueError(
-                "Child node to add must have the node it is adding to as its parent"
-            )
+            raise ValueError("Child node to add must have the node it is adding to as its parent")
 
         if len(self.children) >= self._NODE_TYPE_MAX_CHILDREN[self.node_type]:
             raise OverflowError("Node already has the maximum amount of children")
 
-        insert_index = bisect(
-            list(map(lambda node: node.hp_pixel, self.children)), child.hp_pixel
-        )
+        insert_index = bisect(list(map(lambda node: node.hp_pixel, self.children)), child.hp_pixel)
         self.children.insert(insert_index, child)
 
     def get_all_leaf_descendants(self) -> List[PixelNode]:
         """Gets all descendant nodes that are leaf nodes.
 
         Leafs nodes correspond to pixels that have data files containing astronomical objects, so
         this method is used to get the files containing all astronomical objects within the pixel.
```

### Comparing `hipscat-0.0.9/src/hipscat/inspection/visualize_catalog.py` & `hipscat-0.1/src/hipscat/inspection/visualize_catalog.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 def _read_point_map(catalog_base_dir):
     """Read the object spatial distribution information from a healpix FITS file.
 
     Args:
         catalog_base_dir: path to a catalog
     Returns:
-        histogram (:obj:`np.ndarray`): one-dimensional numpy array of long integers where the
-            value at each index corresponds to the number of objects found at the healpix pixel.
+        one-dimensional numpy array of long integers where the value at each index
+        corresponds to the number of objects found at the healpix pixel.
     """
     map_file_pointer = paths.get_point_map_file_pointer(catalog_base_dir)
     return file_io.read_fits_image(map_file_pointer)
 
 
 def plot_points(catalog: Catalog, projection="moll", draw_map=True):
     """Create a visual map of the input points of the catalog.
@@ -42,14 +42,15 @@
         f"Catalog point density map - {catalog.catalog_name}",
         draw_map=draw_map,
     )
 
 
 def plot_pixels(catalog: Catalog, projection="moll", draw_map=True):
     """Create a visual map of the pixel density of the catalog.
+
     Args:
         catalog (`hipscat.catalog.Catalog`) Catalog to display
         projection (str) The map projection to use. Valid values include:
             - moll - Molleweide projection (default)
             - gnom - Gnomonic projection
             - cart - Cartesian projection
             - orth - Orthographic projection
@@ -59,22 +60,19 @@
     catalog_orders = pixels[PartitionInfo.METADATA_ORDER_COLUMN_NAME].unique()
     catalog_orders.sort()
     max_order = catalog_orders[-1]
 
     order_map = np.full(hp.order2npix(max_order), hp.pixelfunc.UNSEEN)
 
     for _, pixel in pixels.iterrows():
-        explosion_factor = 4 ** (
-            max_order - pixel[PartitionInfo.METADATA_ORDER_COLUMN_NAME]
-        )
+        explosion_factor = 4 ** (max_order - pixel[PartitionInfo.METADATA_ORDER_COLUMN_NAME])
         exploded_pixels = [
             *range(
                 pixel[PartitionInfo.METADATA_PIXEL_COLUMN_NAME] * explosion_factor,
-                (pixel[PartitionInfo.METADATA_PIXEL_COLUMN_NAME] + 1)
-                * explosion_factor,
+                (pixel[PartitionInfo.METADATA_PIXEL_COLUMN_NAME] + 1) * explosion_factor,
             )
         ]
         order_map[exploded_pixels] = pixel[PartitionInfo.METADATA_ORDER_COLUMN_NAME]
     _plot_healpix_map(
         order_map,
         projection,
         f"Catalog pixel density map - {catalog.catalog_name}",
```

### Comparing `hipscat-0.0.9/src/hipscat/io/__init__.py` & `hipscat-0.1/src/hipscat/io/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 """Utilities for reading and writing catalog files"""
 
 from .file_io import FilePointer, get_file_pointer_from_path
-from .paths import (create_hive_directory_name, create_hive_parquet_file_name,
-                    get_catalog_info_pointer, get_common_metadata_pointer,
-                    get_parquet_metadata_pointer, get_partition_info_pointer,
-                    get_point_map_file_pointer, get_provenance_pointer,
-                    pixel_association_directory, pixel_association_file,
-                    pixel_catalog_file, pixel_directory)
-from .write_metadata import (write_catalog_info, write_parquet_metadata,
-                             write_partition_info, write_provenance_info)
+from .paths import (
+    create_hive_directory_name,
+    create_hive_parquet_file_name,
+    get_catalog_info_pointer,
+    get_common_metadata_pointer,
+    get_parquet_metadata_pointer,
+    get_partition_info_pointer,
+    get_point_map_file_pointer,
+    get_provenance_pointer,
+    pixel_association_directory,
+    pixel_association_file,
+    pixel_catalog_file,
+    pixel_directory,
+)
+from .write_metadata import (
+    write_catalog_info,
+    write_parquet_metadata,
+    write_partition_info,
+    write_provenance_info,
+)
```

### Comparing `hipscat-0.0.9/src/hipscat/io/file_io/file_io.py` & `hipscat-0.1/src/hipscat/io/file_io/file_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,15 @@
     Args:
         file_pointer: directory in file system to remove
         ignore_errors: if True errors resulting from failed removals will be ignored
     """
     shutil.rmtree(file_pointer, ignore_errors=ignore_errors)
 
 
-def write_string_to_file(
-    file_pointer: FilePointer, string: str, encoding: str = "utf-8"
-):
+def write_string_to_file(file_pointer: FilePointer, string: str, encoding: str = "utf-8"):
     """Write a string to a text file
 
     Args:
         file_pointer: file location to write file to
         string: string to write to file
         encoding: Default: 'utf-8', encoding method to write to file with
     """
@@ -75,17 +73,15 @@
         **kwargs: arguments to pass to pandas `read_csv` loading method
     Returns:
         pandas dataframe loaded from CSV
     """
     return pd.read_csv(file_pointer, **kwargs)
 
 
-def write_dataframe_to_csv(
-    dataframe: pd.DataFrame, file_pointer: FilePointer, **kwargs
-):
+def write_dataframe_to_csv(dataframe: pd.DataFrame, file_pointer: FilePointer, **kwargs):
     """Write a pandas DataFrame to a CSV file
 
     Args:
         dataframe: DataFrame to write
         file_pointer: location of file to write to
         **kwargs: args to pass to pandas `to_csv` method
     """
@@ -98,28 +94,24 @@
     Args:
         file_pointer: location of file to read metadata from
         **kwargs: additional arguments to be passed to pyarrow.parquet.read_metadata
     """
     return pq.read_metadata(file_pointer, **kwargs)
 
 
-def write_parquet_metadata(
-    schema: Any, file_pointer: FilePointer, metadata_collector: list = None, **kwargs
-):
+def write_parquet_metadata(schema: Any, file_pointer: FilePointer, metadata_collector: list = None, **kwargs):
     """Write a metadata only parquet file from a schema
 
     Args:
         schema: schema to be written
         file_pointer: location of file to be written to
         metadata_collector: where to collect metadata information
         **kwargs: additional arguments to be passed to pyarrow.parquet.write_metadata
     """
-    pq.write_metadata(
-        schema, file_pointer, metadata_collector=metadata_collector, **kwargs
-    )
+    pq.write_metadata(schema, file_pointer, metadata_collector=metadata_collector, **kwargs)
 
 
 def read_fits_image(map_file_pointer: FilePointer):
     """Read the object spatial distribution information from a healpix FITS file.
 
     Args:
         file_pointer: location of file to be written
```

### Comparing `hipscat-0.0.9/src/hipscat/io/file_io/file_pointer.py` & `hipscat-0.1/src/hipscat/io/file_io/file_pointer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import glob
 import os
 from typing import List, NewType
 
 FilePointer = NewType("FilePointer", str)
+"""Unified type for references to files."""
 
 
 def get_file_pointer_from_path(path: str) -> FilePointer:
     """Returns a file pointer from a path string"""
     return FilePointer(path)
```

### Comparing `hipscat-0.0.9/src/hipscat/io/paths.py` & `hipscat-0.1/src/hipscat/io/paths.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Methods for creating partitioned data paths"""
 from __future__ import annotations
 
-from hipscat.io.file_io.file_pointer import (FilePointer,
-                                             append_paths_to_pointer)
+from hipscat.io.file_io.file_pointer import FilePointer, append_paths_to_pointer
 
 ORDER_DIRECTORY_PREFIX = "Norder"
 DIR_DIRECTORY_PREFIX = "Dir"
 PIXEL_DIRECTORY_PREFIX = "Npix"
 JOIN_ORDER_DIRECTORY_PREFIX = "join_Norder"
 JOIN_DIR_DIRECTORY_PREFIX = "join_Dir"
 JOIN_PIXEL_DIRECTORY_PREFIX = "join_Npix"
 
 CATALOG_INFO_FILENAME = "catalog_info.json"
 PARTITION_INFO_FILENAME = "partition_info.csv"
+PARTITION_JOIN_INFO_FILENAME = "partition_join_info.csv"
 PROVENANCE_INFO_FILENAME = "provenance_info.json"
 PARQUET_METADATA_FILENAME = "_metadata"
 PARQUET_COMMON_METADATA_FILENAME = "_common_metadata"
 POINT_MAP_FILENAME = "point_map.fits"
 
 
 def pixel_directory(
@@ -42,32 +42,28 @@
         directory_number (int): directory number
         pixel_number (int): the healpix pixel
     Returns:
         FilePointer directory name
     """
     norder = int(pixel_order)
     if pixel_number is None and directory_number is None:
-        raise ValueError(
-            "One of pixel_number or directory_number is required to create pixel directory"
-        )
+        raise ValueError("One of pixel_number or directory_number is required to create pixel directory")
     if directory_number is not None:
         ndir = directory_number
     else:
         npix = int(pixel_number)
         ndir = int(npix / 10_000) * 10_000
     return create_hive_directory_name(
         catalog_base_dir,
         [ORDER_DIRECTORY_PREFIX, DIR_DIRECTORY_PREFIX],
         [norder, ndir],
     )
 
 
-def pixel_catalog_file(
-    catalog_base_dir: FilePointer, pixel_order: int, pixel_number: int
-) -> FilePointer:
+def pixel_catalog_file(catalog_base_dir: FilePointer, pixel_order: int, pixel_number: int) -> FilePointer:
     """Create path *pointer* for a pixel catalog file. This will not create the directory or file.
 
     The catalog file name will take the HiPS standard form of:
 
         <catalog_base_dir>/Norder=<pixel_order>/Dir=<directory number>/Npix=<pixel_number>.parquet
 
     Where the directory number is calculated using integer division as:
@@ -181,55 +177,49 @@
             int(join_pixel_order),
             int(join_pixel_number / 10_000) * 10_000,
             int(join_pixel_number),
         ],
     )
 
 
-def create_hive_directory_name(
-    base_dir, partition_token_names, partition_token_values
-):
+def create_hive_directory_name(base_dir, partition_token_names, partition_token_values):
     """Create path *pointer* for a directory with hive partitioning naming.
     This will not create the directory.
 
     The directory name will have the form of:
 
         <catalog_base_dir>/<name_1>=<value_1>/.../<name_n>=<value_n>
-    
+
     Args:
         catalog_base_dir (FilePointer): base directory of the catalog (includes catalog name)
         partition_token_names (list[string]): list of partition name parts.
         partition_token_values (list[string]): list of partition values that
             correspond to the token name parts.
     """
     partition_tokens = [
-        f"{name}={value}"
-        for name, value in zip(partition_token_names, partition_token_values)
+        f"{name}={value}" for name, value in zip(partition_token_names, partition_token_values)
     ]
     return append_paths_to_pointer(base_dir, *partition_tokens)
 
 
-def create_hive_parquet_file_name(
-    base_dir, partition_token_names, partition_token_values
-):
+def create_hive_parquet_file_name(base_dir, partition_token_names, partition_token_values):
     """Create path *pointer* for a single parquet with hive partitioning naming.
-    
+
     The file name will have the form of:
 
         <catalog_base_dir>/<name_1>=<value_1>/.../<name_n>=<value_n>.parquet
-    
+
     Args:
         catalog_base_dir (FilePointer): base directory of the catalog (includes catalog name)
         partition_token_names (list[string]): list of partition name parts.
         partition_token_values (list[string]): list of partition values that
             correspond to the token name parts.
     """
     partition_tokens = [
-        f"{name}={value}"
-        for name, value in zip(partition_token_names, partition_token_values)
+        f"{name}={value}" for name, value in zip(partition_token_names, partition_token_values)
     ]
     return f"{append_paths_to_pointer(base_dir, *partition_tokens)}.parquet"
 
 
 def get_catalog_info_pointer(catalog_base_dir: FilePointer) -> FilePointer:
     """Get file pointer to `catalog_info.json` metadata file
 
@@ -290,7 +280,18 @@
 
     Args:
         catalog_base_dir: pointer to base catalog directory
     Returns:
         File Pointer to the catalog's `point_map.fits` FITS image file.
     """
     return append_paths_to_pointer(catalog_base_dir, POINT_MAP_FILENAME)
+
+
+def get_partition_join_info_pointer(catalog_base_dir: FilePointer) -> FilePointer:
+    """Get file pointer to `partition_join_info.csv` association metadata file
+
+    Args:
+        catalog_base_dir: pointer to base catalog directory
+    Returns:
+        File Pointer to the catalog's `partition_join_info.csv` association metadata file
+    """
+    return append_paths_to_pointer(catalog_base_dir, PARTITION_JOIN_INFO_FILENAME)
```

### Comparing `hipscat-0.0.9/src/hipscat/pixel_math/README.md` & `hipscat-0.1/docs/guide/pixel_math.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/src/hipscat/pixel_math/healpix_pixel.py` & `hipscat-0.1/src/hipscat/pixel_math/healpix_pixel.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,16 +18,14 @@
     def __post_init__(self) -> None:
         """Initialize a HEALPix pixel
         Args:
             order: HEALPix order
             pixel: HEALPix pixel number in NESTED ordering scheme
         """
         if self.order > HIPSCAT_ID_HEALPIX_ORDER:
-            raise ValueError(
-                f"HEALPix order cannot be greater than {HIPSCAT_ID_HEALPIX_ORDER}"
-            )
+            raise ValueError(f"HEALPix order cannot be greater than {HIPSCAT_ID_HEALPIX_ORDER}")
 
     def __str__(self) -> str:
         return f"Order: {self.order}, Pixel: {self.pixel}"
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `hipscat-0.0.9/src/hipscat/pixel_math/hipscat_id.py` & `hipscat-0.1/src/hipscat/pixel_math/hipscat_id.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 """
-Compute the hipscat ID field
+Compute the hipscat index field
+
+This index is defined as a 64-bit integer which has two parts:
+    - healpix pixel (at order 19)
+    - incrementing counter (within same healpix, for uniqueness)
+    
+::
+
+    |------------------------------------------|-------------------|
+    |<-----    healpixel at order 19    ------>|<--   counter   -->|
+
+This provides us with an increasing index, that will not overlap
+between spatially partitioned data files.
 
 See the README in this directory for more information on the fiddly pixel math.
 """
 
 import healpy as hp
 import numpy as np
 
 HIPSCAT_ID_HEALPIX_ORDER = 19
 
 
 def compute_hipscat_id(ra_values, dec_values):
     """Compute the hipscat ID field.
 
-    This index is defined as a 64-bit integer which has two parts:
-        - healpix pixel (at order 19)
-        - incrementing counter (within same healpix, for uniqueness)
-    |------------------------------------------|-------------------|
-    |<-----    healpixel at order 19    ------>|<--   counter   -->|
-
-    This provides us with an increasing index, that will not overlap
-    between spatially partitioned data files.
-
     Args:
         ra_values (list[float]): celestial coordinates, right ascension
         dec_values (list[float]): celestial coordinates, declination
     Returns:
         one-dimensional array of int64s with hipscat IDs for the sky positions.
     Raises:
         ValueError: if the length of the input lists don't match.
     """
     if len(ra_values) != len(dec_values):
         raise ValueError("ra and dec arrays should have the same length")
 
     ## Construct the bit-shifted healpix segment
     value_count = len(ra_values)
-    mapped_pixels = hp.ang2pix(
-        2**HIPSCAT_ID_HEALPIX_ORDER, ra_values, dec_values, nest=True, lonlat=True
-    )
+    mapped_pixels = hp.ang2pix(2**HIPSCAT_ID_HEALPIX_ORDER, ra_values, dec_values, nest=True, lonlat=True)
 
     ## We sort to put pixels next to each other that will need to be counted.
     ## This simplifies the counter logic, as we can subtract the index where
     ## we first see the pixel value from the current index to get the offset counter.
-    sort_index = np.argsort(mapped_pixels)
+    sort_index = np.argsort(mapped_pixels, kind="stable")
     mapped_pixels = mapped_pixels[sort_index]
 
     ## Construct the counter.
-    _, unique_indices, unique_inverse = np.unique(
-        mapped_pixels, return_inverse=True, return_index=True
-    )
+    _, unique_indices, unique_inverse = np.unique(mapped_pixels, return_inverse=True, return_index=True)
     unique_indices = unique_indices.astype(np.uint64)
     boring_number_index = np.arange(value_count, dtype=np.uint64)
     offset_counter = boring_number_index - unique_indices[unique_inverse]
 
     ## Add counter to shifted pixel, and map back to the original, unsorted, values
-    shifted_pixels = mapped_pixels.astype(np.uint64) << (
-        64 - (4 + 2 * HIPSCAT_ID_HEALPIX_ORDER)
-    )
+    shifted_pixels = mapped_pixels.astype(np.uint64) << (64 - (4 + 2 * HIPSCAT_ID_HEALPIX_ORDER))
     shifted_pixels = shifted_pixels + offset_counter
 
-    unsort_index = np.argsort(sort_index)
+    unsort_index = np.argsort(sort_index, kind="stable")
     return shifted_pixels[unsort_index]
 
 
 def hipscat_id_to_healpix(ids):
     """Convert some hipscat ids to the healpix pixel at order 19.
     This is just bit-shifting the counter away.
```

### Comparing `hipscat-0.0.9/src/hipscat/pixel_math/margin_bounding.py` & `hipscat-0.1/src/hipscat/pixel_math/margin_bounding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Utilities to build bounding boxes around healpixels that include a neighor margin."""
 
+import astropy.units as u
+import astropy.wcs as world_coordinate_system
 import healpy as hp
 import numpy as np
-
 from astropy.coordinates import SkyCoord
 from regions import PixCoord, PolygonSkyRegion
-import astropy.wcs as world_coordinate_system
-import astropy.units as u
 
 from . import pixel_margins as pm
 
 
 def get_margin_scale(pixel_order, margin_threshold=0.1):
     """Get the scale value need to expand the pixel bounding box to include the `margin_threshold`.
 
@@ -43,58 +42,52 @@
     Returns:
         polygons (list of tuples): a list of :obj:`regions.PolygonPixelRegion`
             and :obj:`wcs.WCS` tuples, covering the full area of the given healpixels
             scaled up area.
     """
     # pylint: disable=too-many-locals
     # pylint: disable=too-many-statements
-    corners = hp.vec2dir(
-        hp.boundaries(2**pixel_order, pix, step=1, nest=True), lonlat=True
-    )
-
-    min_ra = corners[0][1] # western corner
-    max_ra = corners[0][3] # eastern corner
-    min_dec = corners[1][2] # southern corner
-    max_dec = corners[1][0] #  northern corner
-
-    pixel_boundaries = hp.vec2dir(
-        hp.boundaries(2**pixel_order, pix, step=step, nest=True), lonlat=True
-    )
+    corners = hp.vec2dir(hp.boundaries(2**pixel_order, pix, step=1, nest=True), lonlat=True)
+
+    min_ra = corners[0][1]  # western corner
+    max_ra = corners[0][3]  # eastern corner
+    min_dec = corners[1][2]  # southern corner
+    max_dec = corners[1][0]  #  northern corner
+
+    pixel_boundaries = hp.vec2dir(hp.boundaries(2**pixel_order, pix, step=step, nest=True), lonlat=True)
 
     # if the eastern corner is less than the western corner, then we've hit the
     # ra rollover and need to normalize to 0 -> 360.
     if max_ra < min_ra:
-        max_ra = max_ra + 360.
+        max_ra = max_ra + 360.0
         ra_vals = pixel_boundaries[0]
-        normal = np.where(ra_vals < 0., ra_vals + 360., ra_vals)
+        normal = np.where(ra_vals < 0.0, ra_vals + 360.0, ra_vals)
         pixel_boundaries[0] = normal
 
     # find the translation values to keep the bounding box
     # centered around the orignal healpixel.
     n_samples = len(pixel_boundaries[0])
     centroid_lon = np.sum(pixel_boundaries[0]) / n_samples
     centroid_lat = np.sum(pixel_boundaries[1]) / n_samples
     translate_lon = centroid_lon - (centroid_lon * scale)
     translate_lat = centroid_lat - (centroid_lat * scale)
 
-    affine_matrix = np.array(
-        [[scale, 0, translate_lon], [0, scale, translate_lat], [0, 0, 1]]
-    )
+    affine_matrix = np.array([[scale, 0, translate_lon], [0, scale, translate_lat], [0, 0, 1]])
 
     # convert the orignal boundary coordinates into
     # a homogenous coordinate space (3-dim)
     homogeneous = np.ones((3, n_samples))
     homogeneous[0] = pixel_boundaries[0]
     homogeneous[1] = pixel_boundaries[1]
 
     transformed_bounding_box = np.matmul(affine_matrix, homogeneous)
 
     # if the transform places the declination of any points outside of
     # the range 90 > dec > -90, change it to a proper dec value.
-    transformed_bounding_box[1] = np.clip(transformed_bounding_box[1], -90., 90.)
+    transformed_bounding_box[1] = np.clip(transformed_bounding_box[1], -90.0, 90.0)
 
     # one arcsecond
     pix_size = 0.0002777777778
 
     ra_naxis = int((max_ra - min_ra) / pix_size)
     dec_naxis = int((max_dec - min_dec) / pix_size)
 
@@ -144,29 +137,27 @@
         wcs_margin.wcs.crpix = [1, 1]
         wcs_margin.wcs.crval = [min_ra, min_dec]
         wcs_margin.wcs.cunit = ["deg", "deg"]
         wcs_margin.wcs.ctype = ["RA---TAN", "DEC--TAN"]
         wcs_margin.wcs.cdelt = [pix_size, pix_size]
         wcs_margin.array_shape = [ra_naxis, dec_naxis]
 
-        vertices = SkyCoord(
-            transformed_bounding_box[0], transformed_bounding_box[1], unit="deg"
-        )
+        vertices = SkyCoord(transformed_bounding_box[0], transformed_bounding_box[1], unit="deg")
         sky_region = PolygonSkyRegion(vertices=vertices)
         polygon_region = sky_region.to_pixel(wcs_margin)
         polygons = [(polygon_region, wcs_margin)]
 
     return polygons
 
 
 def check_margin_bounds(r_asc, dec, poly_and_wcs):
     """Get the astropy `regions.PolygonPixelRegion` and `astropy.wcs` objects
         for a given margin bounding box scale.
         For pixels that fall along the poles, this code must be used in conjunction
-        with `check_polar_margin_bounds` and 
+        with `check_polar_margin_bounds` and
         `pixel_margins.get_truncated_margin_pixels`.
 
     Args:
         r_asc (:obj:`np.array`): one dimmensional array representing the ra of a
             given set of points.
         dec (:obj:`np.array`): one dimmensional array representing the dec of a
             given set of points.
@@ -177,22 +168,21 @@
         :obj:`numpy.array` of boolean values corresponding to the ra and dec
             coordinates checked against whether a given point is within any of the
             provided polygons.
     """
     sky_coords = SkyCoord(r_asc, dec, unit="deg")
     bound_vals = []
     for poly, wcs in poly_and_wcs:
-        x_coords, y_coords = world_coordinate_system.utils.skycoord_to_pixel(
-            sky_coords, wcs
-        )
+        x_coords, y_coords = world_coordinate_system.utils.skycoord_to_pixel(sky_coords, wcs)
         pix_coords = PixCoord(x_coords, y_coords)
         vals = poly.contains(pix_coords)
         bound_vals.append(vals)
     return np.array(bound_vals).any(axis=0)
 
+
 # pylint: disable=too-many-locals
 def check_polar_margin_bounds(r_asc, dec, order, pix, margin_order, margin_threshold, step=1000):
     """Given a set of ra and dec values that are around one of the poles,
         determine if they are within `margin_threshold` of a provided
         partition pixel. This method helps us solve the edge cases that
         occur for margin bounding around the poles.
 
@@ -221,48 +211,45 @@
 
     part_pix_res = hp.nside2resol(2**order)
     marg_pix_res = hp.nside2resol(2**margin_order)
 
     # get the approximate number of boundary samples to cover a highest_k pixel
     # on the boundary of the main pixel
     boundary_range = int((marg_pix_res / part_pix_res) * step)
-    pixel_boundaries = hp.vec2dir(
-        hp.boundaries(2**order, pix, step=step, nest=True),
-        lonlat=True
-    )
+    pixel_boundaries = hp.vec2dir(hp.boundaries(2**order, pix, step=step, nest=True), lonlat=True)
 
     # to optimize our code, we only want to take boundary samples from the part
     # of the pixel that directly abuts the polar margin pixels.
     if pole == "North":
         end = len(pixel_boundaries[0])
-        east_ra = pixel_boundaries[0][0:boundary_range+1]
-        east_dec = pixel_boundaries[1][0:boundary_range+1]
+        east_ra = pixel_boundaries[0][0 : boundary_range + 1]
+        east_dec = pixel_boundaries[1][0 : boundary_range + 1]
 
-        west_ra = pixel_boundaries[0][end-boundary_range:end]
-        west_dec = pixel_boundaries[1][end-boundary_range:end]
+        west_ra = pixel_boundaries[0][end - boundary_range : end]
+        west_dec = pixel_boundaries[1][end - boundary_range : end]
 
         bound_ra = np.concatenate((east_ra, west_ra), axis=None)
         bound_dec = np.concatenate((east_dec, west_dec), axis=None)
         polar_boundaries = np.array([bound_ra, bound_dec])
     else:
         start = (2 * step) - boundary_range
         end = (2 * step) + boundary_range + 1
         south_ra = pixel_boundaries[0][start:end]
         south_dec = pixel_boundaries[1][start:end]
         polar_boundaries = np.array([south_ra, south_dec])
 
     # healpy.boundaries sometimes returns dec values greater than 90, especially
     # when taking many samples...
-    polar_boundaries[1] = np.clip(polar_boundaries[1], -90., 90.)
+    polar_boundaries[1] = np.clip(polar_boundaries[1], -90.0, 90.0)
 
-    sky_coords = SkyCoord(r_asc, dec, unit='deg')
+    sky_coords = SkyCoord(r_asc, dec, unit="deg")
 
     checks = []
     for i in range(len(polar_boundaries[0])):
         lon = polar_boundaries[0][i]
         lat = polar_boundaries[1][i]
-        bound_coord = SkyCoord(lon, lat, unit='deg')
+        bound_coord = SkyCoord(lon, lat, unit="deg")
 
         ang_dist = bound_coord.separation(sky_coords)
-        checks.append(ang_dist <= margin_threshold*u.deg)
+        checks.append(ang_dist <= margin_threshold * u.deg)
 
     return np.array(checks).any(axis=0)
```

### Comparing `hipscat-0.0.9/src/hipscat/pixel_math/partition_stats.py` & `hipscat-0.1/src/hipscat/pixel_math/partition_stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     highest_order,
     ra_column="ra",
     dec_column="dec",
 ):
     """Generate a histogram of counts for objects found in `data`
 
     Args:
-        data (obj:`pd.DataFrame`): tabular object data
+        data (:obj:`pd.DataFrame`): tabular object data
         highest_order (int):  the highest healpix order (e.g. 0-10)
         ra_column (str): where in the input to find the celestial coordinate, right ascension
         dec_column (str): where in the input to find the celestial coordinate, declination
     Returns:
         one-dimensional numpy array of long integers where the value at each index corresponds
         to the number of objects found at the healpix pixel.
     Raises:
@@ -52,64 +52,68 @@
         nest=True,
     )
     mapped_pixel, count_at_pixel = np.unique(mapped_pixels, return_counts=True)
     histogram_result[mapped_pixel] += count_at_pixel.astype(np.int64)
     return histogram_result
 
 
-def generate_alignment(histogram, highest_order=10, threshold=1_000_000):
+def generate_alignment(histogram, highest_order=10, lowest_order=0, threshold=1_000_000):
     """Generate alignment from high order pixels to those of equal or lower order
 
     We may initially find healpix pixels at order 10, but after aggregating up to the pixel
     threshold, some final pixels are order 4 or 7. This method provides a map from pixels
     at order 10 to their destination pixel. This may be used as an input into later partitioning
     map reduce steps.
 
     Args:
         histogram (:obj:`np.array`): one-dimensional numpy array of long integers where the
             value at each index corresponds to the number of objects found at the healpix pixel.
-        highest_order (int):  the highest healpix order (e.g. 0-10)
+        highest_order (int):  the highest healpix order (e.g. 5-10)
+        lowest_order (int): the lowest healpix order (e.g. 1-5). specifying a lowest order
+            constrains the partitioning to prevent spatially large pixels.
         threshold (int): the maximum number of objects allowed in a single pixel
     Returns:
         one-dimensional numpy array of integer 3-tuples, where the value at each index corresponds
         to the destination pixel at order less than or equal to the `highest_order`.
 
         The tuple contains three integers:
 
         - order of the destination pixel
         - pixel number *at the above order*
         - the number of objects in the pixel
     Raises:
-        ValueError if the histogram is the wrong size, or some initial histogram bins
+        ValueError: if the histogram is the wrong size, or some initial histogram bins
             exceed threshold.
     """
     if len(histogram) != hp.order2npix(highest_order):
         raise ValueError("histogram is not the right size")
+    if lowest_order > highest_order:
+        raise ValueError("lowest_order should be less than highest_order")
     max_bin = np.amax(histogram)
     if max_bin > threshold:
         raise ValueError(f"single pixel count {max_bin} exceeds threshold {threshold}")
 
     nested_sums = []
     for i in range(0, highest_order):
         nested_sums.append(empty_histogram(i))
     nested_sums.append(histogram)
 
     # work backward - from highest order, fill in the sums of lower order pixels
-    for read_order in range(highest_order, 0, -1):
+    for read_order in range(highest_order, lowest_order, -1):
         parent_order = read_order - 1
         for index in range(0, len(nested_sums[read_order])):
             parent_pixel = index >> 2
             nested_sums[parent_order][parent_pixel] += nested_sums[read_order][index]
 
     nested_alignment = []
     for i in range(0, highest_order + 1):
         nested_alignment.append(np.full(hp.order2npix(i), None))
 
     # work forward - determine if we should map to a lower order pixel, this pixel, or keep looking.
-    for read_order in range(0, highest_order + 1):
+    for read_order in range(lowest_order, highest_order + 1):
         parent_order = read_order - 1
         for index in range(0, len(nested_sums[read_order])):
             parent_alignment = None
             if parent_order >= 0:
                 parent_pixel = index >> 2
                 parent_alignment = nested_alignment[parent_order][parent_pixel]
 
@@ -125,14 +129,15 @@
                 )
 
     return nested_alignment[highest_order]
 
 
 def generate_destination_pixel_map(histogram, pixel_map):
     """Generate mapping from destination pixel to all the constituent pixels.
+
     Args:
         histogram (:obj:`np.array`): one-dimensional numpy array of long integers where the
             value at each index corresponds to the number of objects found at the healpix pixel.
         pixel_map (:obj:`np.array`): one-dimensional numpy array of integer 3-tuples.
             See :func:`generate_alignment` for more details on this format.
     Returns:
         dictionary that maps the integer 3-tuple of a pixel at destination order to the set of
@@ -155,74 +160,74 @@
 
         non_zero_indexes = np.nonzero(histogram[start_pixel:end_pixel])[0] + start_pixel
         result[(order, pixel, count)] = non_zero_indexes.tolist()
 
     return result
 
 
-def compute_pixel_map(histogram, highest_order=10, threshold=1_000_000):
+def compute_pixel_map(histogram, highest_order=10, lowest_order=0, threshold=1_000_000):
     # pylint: disable=too-many-locals
     """Generate alignment from high order pixels to those of equal or lower order
 
     We may initially find healpix pixels at order 10, but after aggregating up to the pixel
     threshold, some final pixels are order 4 or 7. This method provides a map from destination
     healpix pixels at a lower order to the origin pixels at the highest order. This may be used
     as an input into later partitioning map reduce steps.
 
     Args:
         histogram (:obj:`np.array`): one-dimensional numpy array of long integers where the
             value at each index corresponds to the number of objects found at the healpix pixel.
         highest_order (int):  the highest healpix order (e.g. 0-10)
+        lowest_order (int): the lowest healpix order (e.g. 1-5). specifying a lowest order
+            constrains the partitioning to prevent spatially large pixels.
         threshold (int): the maximum number of objects allowed in a single pixel
     Returns:
         dictionary that maps the HealpixPixel (a pixel at destination order) to a tuple of
-            origin pixel information:
+        origin pixel information.
+
+        The tuple contains the following:
 
-            - 0 - the total number of rows found in this destination pixel
-            - 1 - the set of indexes in histogram for the pixels at the original healpix order.
+        - 0 - the total number of rows found in this destination pixel
+        - 1 - the set of indexes in histogram for the pixels at the original healpix order.
     Raises:
-        ValueError if the histogram is the wrong size, or some initial histogram bins
+        ValueError: if the histogram is the wrong size, or some initial histogram bins
             exceed threshold.
     """
     if len(histogram) != hp.order2npix(highest_order):
         raise ValueError("histogram is not the right size")
+    if lowest_order > highest_order:
+        raise ValueError("lowest_order should be less than highest_order")
     max_bin = np.amax(histogram)
     if max_bin > threshold:
         raise ValueError(f"single pixel count {max_bin} exceeds threshold {threshold}")
 
     nested_sums = []
 
     for order in range(0, highest_order):
         explosion_factor = 4 ** (highest_order - order)
         nested_sums.append(histogram.reshape(-1, explosion_factor).sum(axis=1))
     nested_sums.append(histogram)
 
-    ## Determine the highest order that does not exceed the threshold
-    orders_at_threshold = [0 if 0 < k <= threshold else None for k in nested_sums[0]]
-    for order in range(1, highest_order + 1):
+    ## Determine the lowest order that does not exceed the threshold
+    orders_at_threshold = [lowest_order if 0 < k <= threshold else None for k in nested_sums[lowest_order]]
+    for order in range(lowest_order + 1, highest_order + 1):
         new_orders_at_threshold = np.array(
             [order if 0 < k <= threshold else None for k in nested_sums[order]]
         )
         parent_alignment = np.repeat(orders_at_threshold, 4, axis=0)
         orders_at_threshold = [
             parent_order if parent_order is not None else new_order
-            for parent_order, new_order in zip(
-                parent_alignment, new_orders_at_threshold
-            )
+            for parent_order, new_order in zip(parent_alignment, new_orders_at_threshold)
         ]
 
     ## Zip up the orders and the pixel numbers.
     healpix_pixels = np.array(
         [
-            HealpixPixel(order, pixel >> 2 * (highest_order - order))
-            if order is not None
-            else None
-            for order, pixel in zip(
-                orders_at_threshold, np.arange(0, len(orders_at_threshold))
-            )
+            HealpixPixel(order, pixel >> 2 * (highest_order - order)) if order is not None else None
+            for order, pixel in zip(orders_at_threshold, np.arange(0, len(orders_at_threshold)))
         ]
     )
 
     ## Create a map from healpix pixel to origin pixel data
     non_none_elements = healpix_pixels[healpix_pixels != np.array(None)]
     unique_pixels = np.unique(non_none_elements)
 
@@ -235,7 +240,42 @@
 
         non_zero_indexes = np.nonzero(histogram[start_pixel:end_pixel])[0] + start_pixel
         result[healpix_pixel] = (
             nested_sums[healpix_pixel.order][healpix_pixel.pixel],
             non_zero_indexes.tolist(),
         )
     return result
+
+
+def generate_constant_pixel_map(histogram, constant_healpix_order):
+    """Special case of creating a destination pixel map where you want to
+    preserve some constant healpix order across the sky.
+
+    NB:
+        - this method filters out pixels with no counts
+        - no upper thresholds are applied, and single pixel may contain many rows
+
+    Args:
+        histogram (:obj:`np.array`): one-dimensional numpy array of long integers where the
+            value at each index corresponds to the number of objects found at the healpix pixel.
+        constant_healpix_order (int):  the desired healpix order (e.g. 0-10)
+    Returns:
+        dictionary that maps non-empty bins as HealpixPixel to a tuple of origin pixel
+        information.
+
+        The tuple contains the following:
+
+        - 0 - the total number of rows found in this destination pixel, same as the origin bin
+        - 1 - the set of indexes in histogram for the pixels at the original healpix
+          order, which will be a list containing only the origin pixel.
+    Raises:
+        ValueError: if the histogram is the wrong size
+    """
+    if len(histogram) != hp.order2npix(constant_healpix_order):
+        raise ValueError("histogram is not the right size")
+
+    non_zero_indexes = np.nonzero(histogram)[0]
+    healpix_pixels = [HealpixPixel(constant_healpix_order, pixel) for pixel in non_zero_indexes]
+
+    value_list = [(histogram[pixel], [pixel]) for pixel in non_zero_indexes]
+
+    return dict(zip(healpix_pixels, value_list))
```

### Comparing `hipscat-0.0.9/src/hipscat/pixel_math/pixel_margins.py` & `hipscat-0.1/src/hipscat/pixel_math/pixel_margins.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     margins = []
     for edge, pixel in zip(which, neighbors):
         if pixel != -1:
             margins.append(get_edge(d_order, pixel, edge))
     margins = np.concatenate(margins)
     return margins
 
+
 def pixel_is_polar(order, pix):
     """Checks if a healpixel is a polar pixel.
 
     Args:
         order (int): the healpix order of the pixel to be checked.
         pix (int): the id of a healpixel to be checked. must be in the nested id scheme.
     Returns:
@@ -126,33 +127,34 @@
     """
     nside = hp.order2nside(order)
     npix = hp.nside2npix(nside)
     ring_pix = hp.nest2ring(nside, pix)
 
     # in the ring numbering scheme, the first and last 4 pixels are the poles.
     if ring_pix <= 3:
-        return (True, 'North')
+        return (True, "North")
     if ring_pix >= npix - 4:
-        return (True, 'South')
-    return (False, '')
+        return (True, "South")
+    return (False, "")
+
 
 def get_truncated_margin_pixels(order, pix, margin_order):
     """Given a polar healpixel, find the margin pixels at order highest_k that will be
     truncated at the poles. In other words, find the margin pixels that are also
     polar pixels.
 
     Args:
         order (int): the healpix order of the pixel that we wish to
-            find the truncated margin pixels for. 
+            find the truncated margin pixels for.
         pix (int): the healpixel we wish to find the truncated margin pixels for.
         margin_order (int): the healpixel order that our margin pixels are at. Must
             be larger than `order`.
     Returns:
-        a list of margin pixels at margin_order order that will be truncated at 
-            the poles, i.e. the margin pixels that are also polar pixels 
+        a list of margin pixels at margin_order order that will be truncated at
+            the poles, i.e. the margin pixels that are also polar pixels
             themselves. In the case that pix is a polar pixel, it will return
             3 pixels, otherwise it will return an empty list.
     """
     if margin_order <= order:
         raise ValueError("margin_order must be larger than order")
 
     partition_nside = hp.order2nside(order)
@@ -168,15 +170,15 @@
     if pole == "North":
         excluded_pixel = hp.nest2ring(partition_nside, pix)
         for i in range(4):
             if i != excluded_pixel:
                 truncs.append(hp.ring2nest(margin_nside, i))
     else:
         d_order = margin_order - order
-        excluded_pixel_nest = (4 ** d_order) * pix
+        excluded_pixel_nest = (4**d_order) * pix
         excluded_pixel_ring = hp.nest2ring(margin_nside, excluded_pixel_nest)
         npix = hp.nside2npix(margin_nside)
 
         for j in range(npix - 4, npix):
             if j != excluded_pixel_ring:
                 truncs.append(hp.ring2nest(margin_nside, j))
```

### Comparing `hipscat-0.0.9/src/hipscat.egg-info/PKG-INFO` & `hipscat-0.1/src/hipscat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.0.9
+Version: 0.1
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Astronomy Data Commons
+        Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
         
@@ -26,14 +26,15 @@
         DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
@@ -67,9 +68,15 @@
 * LSDB ([on GitHub](https://github.com/astronomy-commons/lsdb)) 
   ([on ReadTheDocs](https://lsdb.readthedocs.io/en/latest/))
 
 ## Contributing
 
 [![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/astronomy-commons/hipscat?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/astronomy-commons/hipscat/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
-See the [contribution guide](https://hipscat.readthedocs.io/en/latest/overview/contributing.html)
+See the [contribution guide](https://hipscat.readthedocs.io/en/latest/guide/contributing.html)
 for completed installation instructions and contribution best practices.
+
+## Acknowledgements
+
+LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative
+founded by Eric and Wendy Schmidt, as part of the Virtual Institute of 
+Astrophysics (VIA).
```

### Comparing `hipscat-0.0.9/tests/.pylintrc` & `hipscat-0.1/tests/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -282,18 +282,19 @@
 # Maximum number of attributes for a class (see R0902).
 max-attributes=7
 
 # Maximum number of boolean expressions in an if statement (see R0916).
 max-bool-expr=5
 
 # Maximum number of branch for function / method body.
-max-branches=12
+max-branches=20
 
 # Maximum number of locals for function / method body.
-max-locals=15
+# We set this higher in tests to allow a more narrative style.
+max-locals=30
 
 # Maximum number of parents for a class (see R0901).
 max-parents=7
 
 # Maximum number of public methods for a class (see R0904).
 max-public-methods=20
 
@@ -325,15 +326,15 @@
 indent-after-paren=4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
 indent-string='    '
 
 # Maximum number of characters on a single line.
-max-line-length=100
+max-line-length=110
 
 # Maximum number of lines in a module.
 max-module-lines=1000
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
@@ -499,15 +500,15 @@
 # Imports are removed from the similarity computation
 ignore-imports=yes
 
 # Signatures are removed from the similarity computation
 ignore-signatures=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=6
 
 
 [SPELLING]
 
 # Limits count of emitted suggestions for spelling mistakes.
 max-spelling-suggestions=4
```

### Comparing `hipscat-0.0.9/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-0.1/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/tests/data/small_sky/point_map.fits` & `hipscat-0.1/tests/data/small_sky/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet` & `hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet` & `hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet` & `hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/tests/data/small_sky_order1/point_map.fits` & `hipscat-0.1/tests/data/small_sky_order1/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/tests/hipscat/catalog/test_catalog_parameters.py` & `hipscat-0.1/tests/hipscat/catalog/test_catalog.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,103 @@
-"""Tests of catalog creation properties"""
+"""Tests of catalog functionality"""
 
 import os
 
+import pandas.testing
 import pytest
 
-import hipscat.io.write_metadata as io
-from hipscat.catalog.catalog_parameters import (CatalogParameters,
-                                                read_from_metadata_file)
+from hipscat.catalog import Catalog, CatalogType, PartitionInfo
+from hipscat.pixel_tree.pixel_node_type import PixelNodeType
 
 
-def test_create_catalog_params(tmp_path):
-    """Test that we can create catalog parameters with good values"""
-    args = CatalogParameters(
-        catalog_name="catalog",
-        output_path=tmp_path,
-    )
+def test_catalog_load(catalog_info, catalog_pixels):
+    catalog = Catalog(catalog_info, catalog_pixels)
+    assert len(catalog.get_pixels()) == catalog_pixels.shape[0]
+    assert catalog.catalog_name == catalog_info.catalog_name
+    for _, pixel in catalog_pixels.iterrows():
+        order = pixel[PartitionInfo.METADATA_ORDER_COLUMN_NAME]
+        pixel = pixel[PartitionInfo.METADATA_PIXEL_COLUMN_NAME]
+        assert (order, pixel) in catalog.pixel_tree
+        assert catalog.pixel_tree[(order, pixel)].node_type == PixelNodeType.LEAF
 
-    ## We didn't specify the catalog path - make sure it exists
-    assert args.catalog_path
 
-    formatted_string = str(args)
-    assert "catalog" in formatted_string
-    assert str(tmp_path) in formatted_string
+def test_catalog_load_wrong_catalog_info(base_catalog_info, catalog_pixels):
+    with pytest.raises(TypeError):
+        Catalog(base_catalog_info, catalog_pixels)
 
 
-def test_bad_catalog_params(tmp_path):
-    """Test that we can't create parameters with bad values"""
-
+def test_catalog_wrong_catalog_type(catalog_info, catalog_pixels):
+    catalog_info.catalog_type = CatalogType.INDEX
     with pytest.raises(ValueError):
-        CatalogParameters(
-            catalog_name="catalog",
-            catalog_type="unknown",
-            output_path=tmp_path,
-        )
-
-
-def test_read_from_metadata_file(tmp_path):
-    """Test basic reading from metadata file."""
-    basic_catalog_info = CatalogParameters(
-        catalog_name="catalog",
-        output_path=tmp_path,
-    )
-
-    io.write_catalog_info(basic_catalog_info)
-    metadata_filename = os.path.join(tmp_path, "catalog", "catalog_info.json")
-
-    read_catalog_info = read_from_metadata_file(metadata_filename)
-    assert basic_catalog_info.catalog_name == read_catalog_info.catalog_name
-    assert basic_catalog_info.catalog_type == read_catalog_info.catalog_type
-    assert basic_catalog_info.epoch == read_catalog_info.epoch
-    assert basic_catalog_info.ra_column == read_catalog_info.ra_column
-    assert basic_catalog_info.dec_column == read_catalog_info.dec_column
-    assert basic_catalog_info.total_rows == read_catalog_info.total_rows
+        Catalog(catalog_info, catalog_pixels)
 
 
-def test_bad_file_contents(tmp_path):
-    """Test parsing the catalog info file with bad file contents."""
+def test_different_pixel_input_types(catalog_info, catalog_pixels):
+    partition_info = PartitionInfo(catalog_pixels)
+    catalog = Catalog(catalog_info, partition_info)
+    assert len(catalog.get_pixels()) == catalog_pixels.shape[0]
+    for _, pixel in catalog_pixels.iterrows():
+        order = pixel[PartitionInfo.METADATA_ORDER_COLUMN_NAME]
+        pixel = pixel[PartitionInfo.METADATA_PIXEL_COLUMN_NAME]
+        assert (order, pixel) in catalog.pixel_tree
+        assert catalog.pixel_tree[(order, pixel)].node_type == PixelNodeType.LEAF
 
-    catalog_path = os.path.join(tmp_path, "empty")
-    os.makedirs(catalog_path, exist_ok=True)
 
-    file_name = os.path.join(catalog_path, "catalog_info.json")
+def test_wrong_pixel_input_type(catalog_info):
+    with pytest.raises(TypeError):
+        Catalog(catalog_info, "test")
+    with pytest.raises(TypeError):
+        Catalog._get_pixel_tree_from_pixels("test")
+    with pytest.raises(TypeError):
+        Catalog._get_partition_info_from_pixels("test")
 
-    ## Malformed json
-    with pytest.raises(ValueError):
-        with open(
-            file_name,
-            "w",
-            encoding="utf-8",
-        ) as metadata_file:
-            metadata_file.write('{catalog_name:"empty"}')
 
-        read_from_metadata_file(file_name)
+def test_get_pixels(catalog_info, catalog_pixels):
+    catalog = Catalog(catalog_info, catalog_pixels)
+    pixels = catalog.get_pixels()
+    pandas.testing.assert_frame_equal(pixels, catalog_pixels)
 
-    ## Empty catalog name
-    with pytest.raises(ValueError):
-        with open(
-            file_name,
-            "w",
-            encoding="utf-8",
-        ) as metadata_file:
-            metadata_file.write('{"catalog_name":""}')
 
-        read_from_metadata_file(file_name)
+def test_load_catalog_small_sky(small_sky_dir):
+    """Instantiate a catalog with 1 pixel"""
+    cat = Catalog.read_from_hipscat(small_sky_dir)
 
-    ## Bad catalog type
-    with pytest.raises(ValueError):
-        with open(
-            file_name,
-            "w",
-            encoding="utf-8",
-        ) as metadata_file:
-            metadata_file.write('{"catalog_name":"empty", "catalog_type": "empty"}')
+    assert cat.catalog_name == "small_sky"
+    assert len(cat.get_pixels()) == 1
 
-        read_from_metadata_file(file_name)
 
-    ## Non-integer total_rows
-    with pytest.raises(ValueError):
-        with open(
-            file_name,
-            "w",
-            encoding="utf-8",
-        ) as metadata_file:
-            metadata_file.write('{"catalog_name":"empty", "total_rows":"empty"}')
+def test_load_catalog_small_sky_order1(small_sky_order1_dir):
+    """Instantiate a catalog with 4 pixels"""
+    cat = Catalog.read_from_hipscat(small_sky_order1_dir)
+
+    assert cat.catalog_name == "small_sky_order1"
+    assert len(cat.get_pixels()) == 4
+
+
+def test_empty_directory(tmp_path):
+    """Test loading empty or incomplete data"""
+    ## Path doesn't exist
+    with pytest.raises(FileNotFoundError):
+        Catalog.read_from_hipscat(os.path.join("path", "empty"))
+
+    catalog_path = os.path.join(tmp_path, "empty")
+    os.makedirs(catalog_path, exist_ok=True)
+
+    ## Path exists but there's nothing there
+    with pytest.raises(FileNotFoundError):
+        Catalog.read_from_hipscat(catalog_path)
+
+    ## catalog_info file exists - getting closer
+    file_name = os.path.join(catalog_path, "catalog_info.json")
+    with open(file_name, "w", encoding="utf-8") as metadata_file:
+        metadata_file.write('{"catalog_name":"empty", "catalog_type":"source"}')
+
+    with pytest.raises(FileNotFoundError):
+        Catalog.read_from_hipscat(catalog_path)
+
+    ## partition_info file exists - enough to create a catalog
+    file_name = os.path.join(catalog_path, "partition_info.csv")
+    with open(file_name, "w", encoding="utf-8") as metadata_file:
+        metadata_file.write("foo")
 
-        read_from_metadata_file(file_name)
+    catalog = Catalog.read_from_hipscat(catalog_path)
+    assert catalog.catalog_name == "empty"
```

### Comparing `hipscat-0.0.9/tests/hipscat/catalog/test_pixel_node.py` & `hipscat-0.1/tests/hipscat/pixel_tree/test_pixel_node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import pytest
 
-from hipscat.catalog.pixel_node import PixelNode
+from hipscat.pixel_math import HealpixPixel
+from hipscat.pixel_tree.pixel_node import PixelNode
 
 
 def check_node_data_correct(node, node_dict):
-    assert node.hp_order == node_dict["hp_order"]
-    assert node.hp_pixel == node_dict["hp_pixel"]
+    assert node.pixel == node_dict["pixel"]
     assert node.node_type == node_dict["node_type"]
     assert node.parent == node_dict["parent"]
 
 
 def test_create_root_node(root_pixel_node_data):
     root_node = PixelNode(**root_pixel_node_data)
     assert root_node
     check_node_data_correct(root_node, root_pixel_node_data)
 
 
-def test_create_root_node_with_parent_raises_error(
-    root_pixel_node, root_pixel_node_data
-):
+def test_create_root_node_with_parent_raises_error(root_pixel_node, root_pixel_node_data):
     with pytest.raises(ValueError):
         root_pixel_node_data["parent"] = root_pixel_node
         PixelNode(**root_pixel_node_data)
 
 
 def test_create_root_node_with_wrong_order_raises_error(root_pixel_node_data):
     with pytest.raises(ValueError):
-        root_pixel_node_data["hp_order"] = 1
+        root_pixel_node_data["pixel"] = HealpixPixel(1, root_pixel_node_data["pixel"].pixel)
         PixelNode(**root_pixel_node_data)
 
 
 def test_create_inner_node(inner_pixel_node_data, root_pixel_node):
     leaf_node = PixelNode(**inner_pixel_node_data)
     assert leaf_node
     check_node_data_correct(leaf_node, inner_pixel_node_data)
@@ -56,83 +54,95 @@
     with pytest.raises(ValueError):
         leaf_pixel_node_data["parent"] = None
         PixelNode(**leaf_pixel_node_data)
 
 
 def test_create_leaf_node_with_negative_hp_order_raises_error(leaf_pixel_node_data):
     with pytest.raises(ValueError):
-        leaf_pixel_node_data["hp_order"] = -1
+        leaf_pixel_node_data["pixel"] = HealpixPixel(-1, leaf_pixel_node_data["pixel"].pixel)
         PixelNode(**leaf_pixel_node_data)
 
 
 def test_create_leaf_node_with_negative_hp_pixel_raises_error(leaf_pixel_node_data):
     with pytest.raises(ValueError):
-        leaf_pixel_node_data["hp_pixel"] = -1
+        leaf_pixel_node_data["pixel"] = HealpixPixel(leaf_pixel_node_data["pixel"].order, -1)
         PixelNode(**leaf_pixel_node_data)
 
 
-def test_create_node_with_wrong_order_parent_raises_error(
-    leaf_pixel_node_data, root_pixel_node
-):
+def test_create_node_with_wrong_order_parent_raises_error(leaf_pixel_node_data, root_pixel_node):
     with pytest.raises(ValueError):
         leaf_pixel_node_data["parent"] = root_pixel_node
         PixelNode(**leaf_pixel_node_data)
 
 
-def test_add_child_node_with_wrong_child_parent_raises_error(
-    leaf_pixel_node, root_pixel_node
-):
+def test_add_child_node_with_wrong_child_parent_raises_error(leaf_pixel_node, root_pixel_node):
     with pytest.raises(ValueError):
         root_pixel_node.add_child_node(leaf_pixel_node)
 
 
 def test_add_max_children_to_root_node(inner_pixel_node_data):
     inner_nodes = []
     for _ in range(12):
-        inner_pixel_node_data["hp_pixel"] += 1
+        inner_pixel_node_data["pixel"] = HealpixPixel(
+            inner_pixel_node_data["pixel"].order,
+            inner_pixel_node_data["pixel"].pixel + 1,
+        )
         inner_nodes.append(PixelNode(**inner_pixel_node_data))
 
 
 def test_add_too_many_children_to_root_node_fails(inner_pixel_node_data):
     with pytest.raises(OverflowError):
         inner_nodes = []
         for _ in range(13):
-            inner_pixel_node_data["hp_pixel"] += 1
+            inner_pixel_node_data["pixel"] = HealpixPixel(
+                inner_pixel_node_data["pixel"].order,
+                inner_pixel_node_data["pixel"].pixel + 1,
+            )
             inner_nodes.append(PixelNode(**inner_pixel_node_data))
 
 
 def test_add_max_children_to_inner_node(leaf_pixel_node_data):
     leaf_nodes = []
     for _ in range(4):
-        leaf_pixel_node_data["hp_pixel"] += 1
+        leaf_pixel_node_data["pixel"] = HealpixPixel(
+            leaf_pixel_node_data["pixel"].order, leaf_pixel_node_data["pixel"].pixel + 1
+        )
+
         leaf_nodes.append(PixelNode(**leaf_pixel_node_data))
 
 
 def test_add_too_many_children_to_inner_node_fails(leaf_pixel_node_data):
     with pytest.raises(OverflowError):
         leaf_nodes = []
         for _ in range(5):
-            leaf_pixel_node_data["hp_pixel"] += 1
+            leaf_pixel_node_data["pixel"] = HealpixPixel(
+                leaf_pixel_node_data["pixel"].order,
+                leaf_pixel_node_data["pixel"].pixel + 1,
+            )
+
             leaf_nodes.append(PixelNode(**leaf_pixel_node_data))
 
 
 def test_add_child_to_leaf_node_fails(leaf_pixel_node, leaf_pixel_node_data):
     with pytest.raises(OverflowError):
-        leaf_pixel_node_data["hp_order"] = leaf_pixel_node.hp_order + 1
+        leaf_pixel_node_data["pixel"] = HealpixPixel(
+            leaf_pixel_node.hp_order + 1, leaf_pixel_node_data["pixel"].pixel
+        )
+
         leaf_pixel_node_data["parent"] = leaf_pixel_node
         PixelNode(**leaf_pixel_node_data)
 
 
 def test_get_leaf_descendants_with_leaf_node(leaf_pixel_node):
     assert leaf_pixel_node.get_all_leaf_descendants() == [leaf_pixel_node]
 
 
 def test_get_leaf_descendants_with_root_node(root_pixel_node, leaf_pixel_node):
     assert root_pixel_node.get_all_leaf_descendants() == [leaf_pixel_node]
 
 
-def test_get_leaf_descendants_with_multiple_leafs(
-    root_pixel_node, leaf_pixel_node, leaf_pixel_node_data
-):
-    leaf_pixel_node_data["hp_pixel"] += 1
+def test_get_leaf_descendants_with_multiple_leafs(root_pixel_node, leaf_pixel_node, leaf_pixel_node_data):
+    leaf_pixel_node_data["pixel"] = HealpixPixel(
+        leaf_pixel_node_data["pixel"].order, leaf_pixel_node_data["pixel"].pixel + 1
+    )
     second_leaf = PixelNode(**leaf_pixel_node_data)
     assert root_pixel_node.get_all_leaf_descendants() == [leaf_pixel_node, second_leaf]
```

### Comparing `hipscat-0.0.9/tests/hipscat/inspection/test_visualize_catalog.py` & `hipscat-0.1/tests/hipscat/inspection/test_visualize_catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 from hipscat.inspection import plot_pixels, plot_points
 
 
 @pytest.mark.parametrize("projection", ["moll", "gnom", "cart", "orth"])
 def test_generate_map(small_sky_dir, projection):
     """Basic test that map data can be generated (does not test that a plot is rendered)"""
 
-    cat = Catalog(small_sky_dir)
+    cat = Catalog.read_from_hipscat(small_sky_dir)
     plot_pixels(cat, projection=projection, draw_map=False)
     plot_points(cat, projection=projection, draw_map=False)
 
 
 def test_generate_map_unknown_projection(small_sky_dir):
     """Test for error with unknown projection type"""
 
-    cat = Catalog(small_sky_dir)
+    cat = Catalog.read_from_hipscat(small_sky_dir)
     with pytest.raises(NotImplementedError):
         plot_pixels(cat, projection=None, draw_map=False)
 
     with pytest.raises(NotImplementedError):
         plot_pixels(cat, projection="", draw_map=False)
 
     with pytest.raises(NotImplementedError):
         plot_pixels(cat, projection="projection", draw_map=False)
 
 
 def test_generate_map_order1(small_sky_order1_dir):
     """Basic test that map data can be generated (does not test that a plot is rendered)"""
 
-    cat = Catalog(small_sky_order1_dir)
+    cat = Catalog.read_from_hipscat(small_sky_order1_dir)
     plot_pixels(cat, draw_map=False)
     plot_points(cat, draw_map=False)
```

### Comparing `hipscat-0.0.9/tests/hipscat/io/conftest.py` & `hipscat-0.1/tests/hipscat/io/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 import os
 import re
 
 import pyarrow as pa
 import pytest
 
-from hipscat.catalog.catalog_parameters import CatalogParameters
-
 # pylint: disable=missing-function-docstring, redefined-outer-name
 
 
 @pytest.fixture
 def assert_text_file_matches():
     def assert_text_file_matches(expected_lines, file_name):
         """Convenience method to read a text file and compare the contents, line for line.
@@ -26,46 +24,31 @@
             contents of `expected_lines`.
 
         Args:
             expected_lines(:obj:`string array`) list of strings, formatted as regular expressions.
             file_name (str): fully-specified path of the file to read
         """
         assert os.path.exists(file_name), f"file not found [{file_name}]"
-        with open(
-            file_name,
-            "r",
-            encoding="utf-8",
-        ) as metadata_file:
-
+        with open(file_name, "r", encoding="utf-8") as metadata_file:
             contents = metadata_file.readlines()
 
         assert len(expected_lines) == len(
             contents
         ), f"files not the same length ({len(contents)} vs {len(expected_lines)})"
         for i, expected in enumerate(expected_lines):
             assert re.match(expected, contents[i]), (
-                f"files do not match at line {i+1} "
-                f"(actual: [{contents[i]}] vs expected: [{expected}])"
+                f"files do not match at line {i+1} " f"(actual: [{contents[i]}] vs expected: [{expected}])"
             )
 
         metadata_file.close()
 
     return assert_text_file_matches
 
 
 @pytest.fixture
-def basic_catalog_info(tmp_path):
-    return CatalogParameters(
-        catalog_name="small_sky",
-        output_path=tmp_path,
-        total_rows=131,
-    )
-
-
-@pytest.fixture
 def basic_catalog_parquet_metadata():
     return pa.schema(
         [
             pa.field("id", pa.int64()),
             pa.field("ra", pa.float64()),
             pa.field("dec", pa.float64()),
             pa.field("ra_error", pa.int64()),
```

### Comparing `hipscat-0.0.9/tests/hipscat/io/file_io/test_file_io.py` & `hipscat-0.1/tests/hipscat/io/file_io/test_file_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,13 +89,13 @@
     csv_df = pd.read_csv(partition_info_path)
     partition_info_pointer = get_file_pointer_from_path(partition_info_path)
     loaded_df = load_csv_to_pandas(partition_info_pointer)
     pd.testing.assert_frame_equal(csv_df, loaded_df)
 
 
 def test_write_df_to_csv(tmp_path):
-    df = pd.DataFrame(np.random.randint(0, 100, size=(100, 4)), columns=list("ABCD"))
+    random_df = pd.DataFrame(np.random.randint(0, 100, size=(100, 4)), columns=list("ABCD"))
     test_file_path = os.path.join(tmp_path, "test.csv")
     test_file_pointer = get_file_pointer_from_path(test_file_path)
-    write_dataframe_to_csv(df, test_file_pointer, index=False)
+    write_dataframe_to_csv(random_df, test_file_pointer, index=False)
     loaded_df = pd.read_csv(test_file_path)
-    pd.testing.assert_frame_equal(loaded_df, df)
+    pd.testing.assert_frame_equal(loaded_df, random_df)
```

### Comparing `hipscat-0.0.9/tests/hipscat/io/file_io/test_file_pointers.py` & `hipscat-0.1/tests/hipscat/io/file_io/test_file_pointers.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.0.9/tests/hipscat/io/test_paths.py` & `hipscat-0.1/tests/hipscat/io/test_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,15 @@
     result = paths.pixel_directory("/foo", 0, 5)
     assert result == expected
 
 
 def test_pixel_directory_number():
     """Simple case with sensical inputs"""
     expected = "/foo/Norder=0/Dir=0"
-    result = paths.pixel_directory(
-        "/foo", pixel_order=0, pixel_number=5, directory_number=0
-    )
+    result = paths.pixel_directory("/foo", pixel_order=0, pixel_number=5, directory_number=0)
     assert result == expected
 
     result = paths.pixel_directory("/foo", pixel_order=0, directory_number=0)
     assert result == expected
 
 
 def test_pixel_directory_missing():
```

### Comparing `hipscat-0.0.9/tests/hipscat/io/test_write_metadata.py` & `hipscat-0.1/tests/hipscat/io/test_write_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Tests of file IO (reads and writes)"""
 
-
 import os
 import shutil
 
 import numpy.testing as npt
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
-import hipscat.io.file_io as file_io
+from hipscat.io import file_io
 import hipscat.io.write_metadata as io
 import hipscat.pixel_math as hist
+from hipscat.pixel_math.healpix_pixel import HealpixPixel
 
 
 def test_write_json_file(assert_text_file_matches, tmp_path):
     """Test of arbitrary json dictionary with strings and numbers"""
 
     expected_lines = [
         "{\n",
@@ -39,44 +39,48 @@
     dictionary["first_five_fib"] = [1, 1, 2, 3, 5]
 
     json_filename = os.path.join(tmp_path, "dictionary.json")
     io.write_json_file(dictionary, json_filename)
     assert_text_file_matches(expected_lines, json_filename)
 
 
-def test_write_catalog_info(assert_text_file_matches, tmp_path, basic_catalog_info):
+def test_write_catalog_info(assert_text_file_matches, tmp_path, catalog_info):
     """Test that we accurately write out catalog metadata"""
+    catalog_base_dir = os.path.join(tmp_path, "test_name")
+    os.makedirs(catalog_base_dir)
     expected_lines = [
         "{",
-        '    "catalog_name": "small_sky",',
+        '    "catalog_name": "test_name",',
         '    "catalog_type": "object",',
+        '    "total_rows": 10,',
         '    "epoch": "J2000",',
-        '    "ra_kw": "ra",',
-        '    "dec_kw": "dec",',
-        '    "total_rows": 131',
+        '    "ra_column": "ra",',
+        '    "dec_column": "dec"',
         "}",
     ]
 
-    io.write_catalog_info(basic_catalog_info)
-    metadata_filename = os.path.join(tmp_path, "small_sky", "catalog_info.json")
+    io.write_catalog_info(dataset_info=catalog_info, catalog_base_dir=catalog_base_dir)
+    metadata_filename = os.path.join(catalog_base_dir, "catalog_info.json")
     assert_text_file_matches(expected_lines, metadata_filename)
 
 
-def test_write_provenance_info(assert_text_file_matches, tmp_path, basic_catalog_info):
+def test_write_provenance_info(assert_text_file_matches, tmp_path, catalog_info):
     """Test that we accurately write out tool-provided generation metadata"""
+    catalog_base_dir = os.path.join(tmp_path, "test_name")
+    os.makedirs(catalog_base_dir)
     expected_lines = [
         "{",
-        '    "catalog_name": "small_sky",',
+        '    "catalog_name": "test_name",',
         '    "catalog_type": "object",',
+        '    "total_rows": 10,',
+        '    "epoch": "J2000",',
+        '    "ra_column": "ra",',
+        '    "dec_column": "dec",',
         r'    "version": ".*",',  # version matches digits
         r'    "generation_date": "[.\d]+",',  # date matches date format
-        '    "epoch": "J2000",',
-        '    "ra_kw": "ra",',
-        '    "dec_kw": "dec",',
-        '    "total_rows": 131,',
         '    "tool_args": {',
         '        "tool_name": "hipscat-import",',
         '        "tool_version": "1.0.0",',
         r'        "input_file_names": \[',
         '            "file1",',
         '            "file2",',
         '            "file3"',
@@ -87,98 +91,92 @@
 
     tool_args = {
         "tool_name": "hipscat-import",
         "tool_version": "1.0.0",
         "input_file_names": ["file1", "file2", "file3"],
     }
 
-    io.write_provenance_info(basic_catalog_info, tool_args)
-    metadata_filename = os.path.join(tmp_path, "small_sky", "provenance_info.json")
+    io.write_provenance_info(
+        catalog_base_dir=catalog_base_dir, dataset_info=catalog_info, tool_args=tool_args
+    )
+    metadata_filename = os.path.join(catalog_base_dir, "provenance_info.json")
     assert_text_file_matches(expected_lines, metadata_filename)
 
 
-def test_write_partition_info(assert_text_file_matches, tmp_path, basic_catalog_info):
-    """Test that we accurately write out the individual partition stats"""
+def test_write_partition_info_healpix_pixel_map(assert_text_file_matches, tmp_path):
+    """Test that we accurately write out the partition stats for overloaded input"""
+    catalog_base_dir = os.path.join(tmp_path, "test_name")
+    os.makedirs(catalog_base_dir)
     expected_lines = [
-        "Norder,Dir,Npix,num_objects",
+        "Norder,Dir,Npix,num_rows",
         "0,0,11,131",
     ]
-    pixel_map = {tuple([0, 11, 131]): [44, 45, 46]}
-    io.write_partition_info(basic_catalog_info, pixel_map)
-    metadata_filename = os.path.join(tmp_path, "small_sky", "partition_info.csv")
+    pixel_map = {HealpixPixel(0, 11): (131, [11])}
+    io.write_partition_info(catalog_base_dir, destination_healpix_pixel_map=pixel_map)
+    metadata_filename = os.path.join(catalog_base_dir, "partition_info.csv")
     assert_text_file_matches(expected_lines, metadata_filename)
 
     expected_lines = [
-        "Norder,Dir,Npix,num_objects",
-        "1,0,44,42",
+        "Norder,Dir,Npix,num_rows",
+        "1,0,44,51",
         "1,0,45,29",
-        "1,0,46,42",
-        "1,0,47,18",
+        "1,0,46,51",
     ]
     pixel_map = {
-        tuple([1, 44, 42]): [44],
-        tuple([1, 45, 29]): [45],
-        tuple([1, 46, 42]): [46],
-        tuple([1, 47, 18]): [47],
+        HealpixPixel(1, 44): (51, [44]),
+        HealpixPixel(1, 45): (29, [45]),
+        HealpixPixel(1, 46): (51, [46]),
     }
-    io.write_partition_info(basic_catalog_info, pixel_map)
-    metadata_filename = os.path.join(tmp_path, "small_sky", "partition_info.csv")
+    io.write_partition_info(catalog_base_dir, destination_healpix_pixel_map=pixel_map)
+    metadata_filename = os.path.join(catalog_base_dir, "partition_info.csv")
     assert_text_file_matches(expected_lines, metadata_filename)
 
 
-def test_write_partition_info_float(
-    assert_text_file_matches, tmp_path, basic_catalog_info
-):
+def test_write_partition_info_float(assert_text_file_matches, tmp_path):
     """Test that we accurately write out the individual partition stats
     even when the input is floats instead of ints"""
+    catalog_base_dir = os.path.join(tmp_path, "test_name")
+    os.makedirs(catalog_base_dir)
     expected_lines = [
-        "Norder,Dir,Npix,num_objects",
+        "Norder,Dir,Npix,num_rows",
         "0,0,11,131",
     ]
-    pixel_map = {tuple([0.0, 11.0, 131.0]): [44.0, 45.0, 46.0]}
-    io.write_partition_info(basic_catalog_info, pixel_map)
-    metadata_filename = os.path.join(tmp_path, "small_sky", "partition_info.csv")
+    pixel_map = {HealpixPixel(0.0, 11.0): (131, [44.0, 45.0, 46.0])}
+    io.write_partition_info(catalog_base_dir, pixel_map)
+    metadata_filename = os.path.join(catalog_base_dir, "partition_info.csv")
     assert_text_file_matches(expected_lines, metadata_filename)
 
 
-def test_write_parquet_metadata(
-    tmp_path, small_sky_dir, basic_catalog_parquet_metadata
-):
+def test_write_parquet_metadata(tmp_path, small_sky_dir, basic_catalog_parquet_metadata):
     """Copy existing catalog and create new metadata files for it"""
-    temp_path = os.path.join(tmp_path, "catalog")
+    catalog_base_dir = os.path.join(tmp_path, "catalog")
     shutil.copytree(
         small_sky_dir,
-        temp_path,
-    )
-    io.write_parquet_metadata(temp_path)
-    check_parquet_schema(
-        os.path.join(temp_path, "_metadata"), basic_catalog_parquet_metadata
+        catalog_base_dir,
     )
+    io.write_parquet_metadata(catalog_base_dir)
+    check_parquet_schema(os.path.join(catalog_base_dir, "_metadata"), basic_catalog_parquet_metadata)
     ## _common_metadata has 0 row groups
     check_parquet_schema(
-        os.path.join(temp_path, "_common_metadata"),
+        os.path.join(catalog_base_dir, "_common_metadata"),
         basic_catalog_parquet_metadata,
         0,
     )
     ## Re-write - should still have the same properties.
-    io.write_parquet_metadata(temp_path)
-    check_parquet_schema(
-        os.path.join(temp_path, "_metadata"), basic_catalog_parquet_metadata
-    )
+    io.write_parquet_metadata(catalog_base_dir)
+    check_parquet_schema(os.path.join(catalog_base_dir, "_metadata"), basic_catalog_parquet_metadata)
     ## _common_metadata has 0 row groups
     check_parquet_schema(
-        os.path.join(temp_path, "_common_metadata"),
+        os.path.join(catalog_base_dir, "_common_metadata"),
         basic_catalog_parquet_metadata,
         0,
     )
 
 
-def test_write_parquet_metadata_order1(
-    tmp_path, small_sky_order1_dir, basic_catalog_parquet_metadata
-):
+def test_write_parquet_metadata_order1(tmp_path, small_sky_order1_dir, basic_catalog_parquet_metadata):
     """Copy existing catalog and create new metadata files for it,
     using a catalog with multiple files."""
     temp_path = os.path.join(tmp_path, "catalog")
     shutil.copytree(
         small_sky_order1_dir,
         temp_path,
     )
@@ -211,17 +209,15 @@
         [
             pa.field("_hipscat_id", pa.int64()),
             pa.field("ps1_objid", pa.int64()),
         ]
     )
 
     io.write_parquet_metadata(temp_path)
-    check_parquet_schema(
-        os.path.join(tmp_path, "index", "_metadata"), index_catalog_parquet_metadata
-    )
+    check_parquet_schema(os.path.join(tmp_path, "index", "_metadata"), index_catalog_parquet_metadata)
     ## _common_metadata has 0 row groups
     check_parquet_schema(
         os.path.join(tmp_path, "index", "_common_metadata"),
         index_catalog_parquet_metadata,
         0,
     )
 
@@ -247,15 +243,14 @@
     for row_index in range(0, parquet_file.metadata.num_row_groups):
         row_md = parquet_file.metadata.row_group(row_index)
         for column_index in range(0, row_md.num_columns):
             column_metadata = row_md.column(column_index)
             assert column_metadata.file_path.endswith(".parquet")
 
 
-
 def test_read_write_fits_point_map(tmp_path):
     """Check that we write and can read a FITS file for spatial distribution."""
     initial_histogram = hist.empty_histogram(1)
     filled_pixels = [51, 29, 51, 0]
     initial_histogram[44:] = filled_pixels[:]
     io.write_fits_map(tmp_path, initial_histogram)
```

### Comparing `hipscat-0.0.9/tests/hipscat/pixel_math/test_healpix_pixel.py` & `hipscat-0.1/tests/hipscat/pixel_math/test_healpix_pixel.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,7 +25,16 @@
     pix1 = HealpixPixel(order=order, pixel=pixel)
     test_dict = {}
     test_dict[pix1] = test_string
     pix2 = HealpixPixel(order=order, pixel=pixel)
     assert pix1 == pix2
     assert pix2 in test_dict
     assert test_dict[pix2] == test_string
+
+
+def test_pixel_str_and_repr():
+    order = 3
+    pixel = 42
+    test_string = f"Order: {order}, Pixel: {pixel}"
+    pix = HealpixPixel(order=order, pixel=pixel)
+    assert str(pix) == test_string
+    assert repr(pix) == test_string
```

### Comparing `hipscat-0.0.9/tests/hipscat/pixel_math/test_hipscat_id.py` & `hipscat-0.1/tests/hipscat/pixel_math/test_hipscat_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,15 @@
     There are a handful of points at (5,5), and these should be assigned
     hipscat_id in sequential order, starting at
     5482513871577022464 (0x4C15CD518F800000).
 
     Interspersed are points at (1,1), which will start at
     5476738131329810432 (0x4C0148503DC00000)
     """
-    result = compute_hipscat_id(
-        [5, 5, 5, 1, 5, 5, 5, 1, 5], [5, 5, 5, 1, 5, 5, 5, 1, 5]
-    )
+    result = compute_hipscat_id([5, 5, 5, 1, 5, 5, 5, 1, 5], [5, 5, 5, 1, 5, 5, 5, 1, 5])
     expected = [
         5482513871577022464,
         5482513871577022465,
         5482513871577022466,
         5476738131329810432,  # out of sequence
         5482513871577022467,
         5482513871577022468,
@@ -66,15 +64,16 @@
     ]
     npt.assert_array_equal(result, expected)
 
 
 @pytest.mark.timeout(1)
 def test_load():
     """Generate a kinda big array and make sure the method completes in under a second.
-    If this method is failing due to timeouts, please refactor to keep within the time limit."""
+    If this method is failing due to timeouts, please refactor to keep within the time limit.
+    """
     rng = np.random.default_rng(seed=800)
     test_num = 1_000_000
 
     ra_arr = rng.random(test_num)
     dec_arr = rng.random(test_num)
     result = compute_hipscat_id(ra_arr, dec_arr)
```

### Comparing `hipscat-0.0.9/tests/hipscat/pixel_math/test_margin_bounding.py` & `hipscat-0.1/tests/hipscat/pixel_math/test_margin_bounding.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 """Tests of margin bounding utility functions"""
 
 import numpy as np
 import numpy.testing as npt
 import pytest
+from astropy.coordinates import SkyCoord
+from regions import PixCoord
 
 import hipscat.pixel_math as pm
 
-from astropy.coordinates import SkyCoord
-from regions import PixCoord
 
 def test_get_margin_scale():
     """Check to make sure that get_margin_scale works as expected."""
     scale = pm.get_margin_scale(3, 0.1)
-    
+
     expected = 1.0272887122119063
 
     assert scale == expected
 
+
 def test_get_margin_scale_k_zero():
     """Make sure get_margin_scale works when k == 0"""
     scale = pm.get_margin_scale(0, 0.1)
 
     expected = 1.0034110890264882
 
     assert scale == expected
 
+
 def test_get_margin_scale_k_high():
     """Make sure get_margin_scale works when k is a high order"""
     scale = pm.get_margin_scale(64, 0.1)
 
-    expected = 6.292348628426864e+16
+    expected = 6.292348628426864e16
 
     assert scale == expected
 
+
 def test_negative_margin_threshold():
     """Make sure that get_marin_scale raises a value error when threshold is < 0.0"""
     with pytest.raises(ValueError) as value_error:
         pm.get_margin_scale(3, -0.1)
 
-    assert(
-        str(value_error.value)
-        == "margin_threshold must be greater than 0."
-    )
+    assert str(value_error.value) == "margin_threshold must be greater than 0."
+
 
 def test_zero_margin_threshold():
     """Make sure that get_marin_scale raises a value error when threshold is == 0.0"""
     with pytest.raises(ValueError) as value_error:
         pm.get_margin_scale(3, 0.0)
 
-    assert(
-        str(value_error.value)
-        == "margin_threshold must be greater than 0."
-    )
+    assert str(value_error.value) == "margin_threshold must be greater than 0."
+
 
 def test_get_margin_bounds_and_wcs():
     """Make sure get_margin_bounds_and wcs works as expected."""
     # far out point, expect False
-    test_ra1 = 42.
-    test_dec1 = 1.
+    test_ra1 = 42.0
+    test_dec1 = 1.0
 
     # middle of our healpixel, expect True
     test_ra2 = 56.25
     test_dec2 = 14.49584495
 
     # actual point from Norder3/Npix4 of my
     # gaia test catalog, expect True
@@ -75,225 +74,196 @@
     test_sc = SkyCoord(test_ra, test_dec, unit="deg")
 
     scale = pm.get_margin_scale(3, 0.1)
     polygon, wcs_margin = pm.get_margin_bounds_and_wcs(3, 4, scale)[0]
 
     assert polygon.area == pytest.approx(756822775.0000424, 0.001)
 
-    x, y = wcs_margin.world_to_pixel(test_sc)
+    coord_x, coord_y = wcs_margin.world_to_pixel(test_sc)
+    expected_pixel_coord = PixCoord(coord_x, coord_y)
+    expected_contains_checks = np.array([False, True, True])
 
-    pc = PixCoord(x, y)
-    checks = polygon.contains(pc)
+    contains_checks = polygon.contains(expected_pixel_coord)
 
-    expected = np.array([False, True, True])
+    npt.assert_array_equal(contains_checks, expected_contains_checks)
 
-    npt.assert_array_equal(checks, expected)
+
+def get_checks_for_bounds(bounds, test_sky_coords):
+    """Helper method for getting the check flags for
+    some boundaries and sky coordinates to check."""
+    vals = []
+    for polygon, margin in bounds:
+        coord_x, coord_y = margin.world_to_pixel(test_sky_coords)
+
+        vals.append(polygon.contains(PixCoord(coord_x, coord_y)))
+
+    return np.array(vals).any(axis=0)
 
 
 def test_get_margin_bounds_and_wcs_low_order():
     """Make sure get_margin_bounds_and wcs works as expected."""
     # far out point, expect False
-    test_ra1 = 90.
-    test_dec1 = -2.
+    test_ra1 = 90.0
+    test_dec1 = -2.0
 
     # middle of our healpixel, expect True
-    test_ra2 = -100.
-    test_dec2 = -45.
+    test_ra2 = -100.0
+    test_dec2 = -45.0
 
     test_ra = np.array([test_ra1, test_ra2])
     test_dec = np.array([test_dec1, test_dec2])
 
     test_sc = SkyCoord(test_ra, test_dec, unit="deg")
 
     scale = pm.get_margin_scale(0, 0.1)
     bounds = pm.get_margin_bounds_and_wcs(0, 5, scale)
 
     assert len(bounds) == 16
 
-    vals = []
-    for p, w in bounds:
-        x, y = w.world_to_pixel(test_sc)
-
-        pc = PixCoord(x, y)
-        vals.append(p.contains(pc))
-
-    checks = np.array(vals).any(axis=0)
-    
     expected = np.array([True, False])
 
-    npt.assert_array_equal(checks, expected)
+    npt.assert_array_equal(get_checks_for_bounds(bounds, test_sc), expected)
+
 
 def test_get_margin_bounds_and_wcs_north_pole():
     """Make sure get_margin_bounds_and_wcs works at pixels along the north polar region"""
     scale = pm.get_margin_scale(1, 0.1)
-    bounds = pm.get_margin_bounds_and_wcs(1, 7, scale, step = 100)
+    bounds = pm.get_margin_bounds_and_wcs(1, 7, scale, step=100)
 
     assert len(bounds) == 4
 
-    test_ra = np.array([50, 100., 130., 130., 100.])
-    test_dec = np.array([-60., 89.9, 65., 85., 50.])
+    test_ra = np.array([50, 100.0, 130.0, 130.0, 100.0])
+    test_dec = np.array([-60.0, 89.9, 65.0, 85.0, 50.0])
 
     test_sc = SkyCoord(test_ra, test_dec, unit="deg")
 
-    vals = []
-    for p, w in bounds:
-        x, y = w.world_to_pixel(test_sc)
-
-        pc = PixCoord(x, y)
-        vals.append(p.contains(pc))
-
-    checks = np.array(vals).any(axis=0)
-    
     expected = np.array([False, True, True, True, False])
 
-    npt.assert_array_equal(checks, expected)
+    npt.assert_array_equal(get_checks_for_bounds(bounds, test_sc), expected)
+
 
 def test_get_margin_bounds_and_wcs_south_pole():
     """Make sure get_margin_bounds_and_wcs works at pixels along the south polar region"""
     scale = pm.get_margin_scale(1, 0.1)
     bounds = pm.get_margin_bounds_and_wcs(1, 36, scale)
 
     assert len(bounds) == 4
 
-    test_ra = np.array([50, 120., 108., 150., 100., 104.])
-    test_dec = np.array([-60., -70., -66.2, -70., -90., -80])
+    test_ra = np.array([50, 120.0, 108.0, 150.0, 100.0, 104.0])
+    test_dec = np.array([-60.0, -70.0, -66.2, -70.0, -90.0, -80])
 
     test_sc = SkyCoord(test_ra, test_dec, unit="deg")
 
-    vals = []
-    for p, w in bounds:
-        x, y = w.world_to_pixel(test_sc)
-
-        pc = PixCoord(x, y)
-        vals.append(p.contains(pc))
-
-    checks = np.array(vals).any(axis=0)
-    
     expected = np.array([False, True, True, True, False, True])
 
-    npt.assert_array_equal(checks, expected)
+    npt.assert_array_equal(get_checks_for_bounds(bounds, test_sc), expected)
+
 
 def test_get_margin_bounds_and_wcs_ra_rollover():
     """Make sure get_margin_bounds_and_wcs works at the rollover point for right ascension"""
     scale = pm.get_margin_scale(1, 0.1)
     bounds = pm.get_margin_bounds_and_wcs(1, 27, scale)
 
     assert len(bounds) == 4
 
-    test_ra = np.array([180., 0., -157.5, 120., 157.5])
-    test_dec = np.array([20., 0., 19.4, 20., 19.4])
+    test_ra = np.array([180.0, 0.0, -157.5, 120.0, 157.5])
+    test_dec = np.array([20.0, 0.0, 19.4, 20.0, 19.4])
 
     test_sc = SkyCoord(test_ra, test_dec, unit="deg")
 
-    vals = []
-    for p, w in bounds:
-        x, y = w.world_to_pixel(test_sc)
-
-        pc = PixCoord(x, y)
-        vals.append(p.contains(pc))
-
-    checks = np.array(vals).any(axis=0)
-    
     expected = np.array([True, False, True, False, True])
 
-    npt.assert_array_equal(checks, expected)
+    npt.assert_array_equal(get_checks_for_bounds(bounds, test_sc), expected)
+
 
 def test_get_margin_bounds_and_wcs_origin():
     """Make sure get_margin_bounds_and_wcs works at the origin of ra and dec."""
     scale = pm.get_margin_scale(0, 0.1)
     bounds = pm.get_margin_bounds_and_wcs(0, 4, scale)
 
     assert len(bounds) == 16
 
-    test_ra = np.array([180.,-20.])
-    test_dec = np.array([20., -10.])
+    test_ra = np.array([180.0, -20.0])
+    test_dec = np.array([20.0, -10.0])
 
     test_sc = SkyCoord(test_ra, test_dec, unit="deg")
 
-    vals = []
-    for p, w in bounds:
-        x, y = w.world_to_pixel(test_sc)
-
-        pc = PixCoord(x, y)
-        vals.append(p.contains(pc))
-
-    checks = np.array(vals).any(axis=0)
-    
     expected = np.array([False, True])
 
-    npt.assert_array_equal(checks, expected)
+    npt.assert_array_equal(get_checks_for_bounds(bounds, test_sc), expected)
 
 
 def test_check_margin_bounds():
     """Make sure check_margin_bounds works properly"""
     scale = pm.get_margin_scale(3, 0.1)
     bounds = pm.get_margin_bounds_and_wcs(3, 4, scale)
 
-    ra = np.array([42.4704538, 56.25, 50.61225197])
-    dec = np.array([1.4593925, 14.49584495, 14.4767556])
+    test_ra = np.array([42.4704538, 56.25, 50.61225197])
+    test_dec = np.array([1.4593925, 14.49584495, 14.4767556])
 
-    checks = pm.check_margin_bounds(ra, dec, bounds)
+    checks = pm.check_margin_bounds(test_ra, test_dec, bounds)
 
     expected = np.array([False, True, True])
 
     npt.assert_array_equal(checks, expected)
 
+
 def test_check_margin_bounds_multi_poly():
     """Make sure check_margin_bounds works when poly_and_wcs has multiple entries"""
     scale = pm.get_margin_scale(1, 0.1)
     bounds = pm.get_margin_bounds_and_wcs(1, 4, scale)
 
-    ra = np.array([42.4704538, 120., 135.0])
-    dec = np.array([1.4593925, 25.0, 19.92530172])
+    test_ra = np.array([42.4704538, 120.0, 135.0])
+    test_dec = np.array([1.4593925, 25.0, 19.92530172])
 
-    checks = pm.check_margin_bounds(ra, dec, bounds)
+    checks = pm.check_margin_bounds(test_ra, test_dec, bounds)
 
     expected = np.array([False, True, True])
 
     npt.assert_array_equal(checks, expected)
 
+
 def test_check_polar_margin_bounds_north():
     """Make sure check_polar_margin_bounds works at the north pole"""
     order = 0
     pix = 1
     margin_order = 2
 
-    ra = np.array([89, -179, -45])
-    dec = np.array([89.9, 89.9, 85.])
+    test_ra = np.array([89, -179, -45])
+    test_dec = np.array([89.9, 89.9, 85.0])
 
-    vals = pm.check_polar_margin_bounds(ra, dec, order, pix, margin_order, 0.1)
+    vals = pm.check_polar_margin_bounds(test_ra, test_dec, order, pix, margin_order, 0.1)
 
     expected = np.array([True, True, False])
 
     npt.assert_array_equal(vals, expected)
 
+
 def test_check_polar_margin_bounds_south():
     """Make sure check_polar_margin_bounds works at the south pole"""
     order = 0
     pix = 9
     margin_order = 2
 
-    ra = np.array([89, -179, -45])
-    dec = np.array([-89.9, -89.9, -85.])
+    test_ra = np.array([89, -179, -45])
+    test_dec = np.array([-89.9, -89.9, -85.0])
 
-    vals = pm.check_polar_margin_bounds(ra, dec, order, pix, margin_order, 0.1)
+    vals = pm.check_polar_margin_bounds(test_ra, test_dec, order, pix, margin_order, 0.1)
 
     expected = np.array([True, True, False])
 
     npt.assert_array_equal(vals, expected)
 
+
 def test_check_polar_margin_bounds_non_pole():
     """Make sure check_polar_margin_bounds raises a ValueError when pix isn't polar"""
     order = 0
     pix = 7
     margin_order = 2
 
-    ra = np.array([89, -179, -45])
-    dec = np.array([-89.9, -89.9, -85.])
+    test_ra = np.array([89, -179, -45])
+    test_dec = np.array([-89.9, -89.9, -85.0])
 
     with pytest.raises(ValueError) as value_error:
-        vals = pm.check_polar_margin_bounds(ra, dec, order, pix, margin_order, 0.1)
+        pm.check_polar_margin_bounds(test_ra, test_dec, order, pix, margin_order, 0.1)
 
-    assert (
-        str(value_error.value)
-        == "provided healpixel must be polar"
-    )
+    assert str(value_error.value) == "provided healpixel must be polar"
```

### Comparing `hipscat-0.0.9/tests/hipscat/pixel_math/test_pixel_margins.py` & `hipscat-0.1/tests/hipscat/pixel_math/test_pixel_margins.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,104 +124,102 @@
 
 
 def test_edge_negative_value():
     """Check to make sure get_edge fails when passed a negative edge value."""
     with pytest.raises(ValueError) as value_error:
         pm.get_edge(2, 5, -1)
 
-    assert (
-        str(value_error.value)
-        == "edge can only be values between 0 and 7 (see docstring)"
-    )
+    assert str(value_error.value) == "edge can only be values between 0 and 7 (see docstring)"
 
 
 def test_edge_greater_than_7():
     """Check to make sure get_edge fails when passed an edge value greater than 7."""
     with pytest.raises(ValueError) as value_error:
         pm.get_edge(2, 5, 8)
 
-    assert (
-        str(value_error.value)
-        == "edge can only be values between 0 and 7 (see docstring)"
-    )
+    assert str(value_error.value) == "edge can only be values between 0 and 7 (see docstring)"
+
 
 def test_pixel_is_polar_north():
     """Check to make sure pixel_is_polar works for a pixel at the north pole."""
     order = 2
     pix = 31
 
     polar, pole = pm.pixel_is_polar(order, pix)
 
     assert polar
     assert pole == "North"
 
+
 def test_pixel_is_polar_south():
     """Check to make sure pixel_is_polar works for a pixel at the south pole."""
     order = 2
     pix = 160
 
     polar, pole = pm.pixel_is_polar(order, pix)
 
     assert polar
     assert pole == "South"
 
+
 def test_pixel_is_polar_non_pole():
     """Check to make sure pixel_is_polar works for non-polar pixels."""
     order = 2
     pix = 105
 
     polar, pole = pm.pixel_is_polar(order, pix)
 
     assert not polar
     assert pole == ""
 
+
 def test_get_truncated_margin_pixels_north():
     """Check to make sure get_truncated_margin_pixels works for pixels at the north pole"""
     order = 1
     pix = 7
     margin_order = 2
 
     truncs = pm.get_truncated_margin_pixels(order, pix, margin_order)
 
     expected = np.array([15, 47, 63])
 
     npt.assert_array_equal(truncs, expected)
 
+
 def test_get_truncated_margin_pixels_south():
     """Check to make sure get_truncated_margin_pixels works for pixels at the south pole"""
     order = 1
     pix = 36
     margin_order = 2
 
     truncs = pm.get_truncated_margin_pixels(order, pix, margin_order)
 
     expected = np.array([128, 160, 176])
 
     npt.assert_array_equal(truncs, expected)
 
+
 def test_get_truncated_margin_pixels_non_pole():
     """Check to make sure get_truncated_margin_pixels works for non-polar pixels"""
     order = 1
     pix = 26
     margin_order = 2
 
     truncs = pm.get_truncated_margin_pixels(order, pix, margin_order)
 
     expected = np.array([])
 
     npt.assert_array_equal(truncs, expected)
 
+
 def test_get_truncated_margin_pixels_bad_margin_order():
     """Check to make sure get_truncated_margin_pixels returns a ValueError when
-        margin_order is less than or equal to order.
+    margin_order is less than or equal to order.
     """
     order = 1
     pix = 26
     margin_order = 1
 
     with pytest.raises(ValueError) as value_error:
         pm.get_truncated_margin_pixels(order, pix, margin_order)
 
-    assert (
-        str(value_error.value)
-        == "margin_order must be larger than order"
-    )
+    assert str(value_error.value) == "margin_order must be larger than order"
```

