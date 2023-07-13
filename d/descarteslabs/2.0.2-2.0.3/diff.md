# Comparing `tmp/descarteslabs-2.0.2.tar.gz` & `tmp/descarteslabs-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descarteslabs-2.0.2.tar", last modified: Mon Jun 26 22:17:43 2023, max compression
+gzip compressed data, was "descarteslabs-2.0.3.tar", last modified: Thu Jul 13 23:13:50 2023, max compression
```

## Comparing `descarteslabs-2.0.2.tar` & `descarteslabs-2.0.3.tar`

### file list

```diff
@@ -1,243 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    85669 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.622655 descarteslabs-2.0.2/descarteslabs/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.622655 descarteslabs-2.0.2/descarteslabs/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29383 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.622655 descarteslabs-2.0.2/descarteslabs/auth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/auth/tests/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.622655 descarteslabs-2.0.2/descarteslabs/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.622655 descarteslabs-2.0.2/descarteslabs/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.622655 descarteslabs-2.0.2/descarteslabs/config/
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/config/settings.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.622655 descarteslabs-2.0.2/descarteslabs/config/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/config/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/config/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.622655 descarteslabs-2.0.2/descarteslabs/core/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.626655 descarteslabs-2.0.2/descarteslabs/core/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64062 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    36605 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/band.py
--rw-r--r--   0 runner    (1001) docker     (123)    29762 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/blob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/blob_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/blob_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    37861 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/catalog_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/catalog_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    63243 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    50022 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/image_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/image_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/image_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/named_catalog_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/product.py
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.626655 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   118250 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36523 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    28972 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_band.py
--rw-r--r--   0 runner    (1001) docker     (123)    16050 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_catalog_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    45554 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_image_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_image_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    28485 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_product.py
--rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    20303 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.626655 descarteslabs-2.0.2/descarteslabs/core/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/addons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.626655 descarteslabs-2.0.2/descarteslabs/core/client/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/auth/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.626655 descarteslabs-2.0.2/descarteslabs/core/client/auth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/auth/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.626655 descarteslabs-2.0.2/descarteslabs/core/client/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/scripts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/scripts/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/client/scripts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/scripts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/scripts/tests/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/client/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    35310 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/tests/e2e/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/tests/test_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/geotiff_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33684 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41637 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/client/services/service/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/service/api_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    29553 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/client/services/service/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/service/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19843 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/services/service/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/common/client/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/client/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/client/document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/common/client/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/client/tests/test_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/common/collection/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/collection/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/common/collection/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/collection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/collection/tests/test_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/common/display/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/display/_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.630655 descarteslabs-2.0.2/descarteslabs/core/common/display/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/display/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/display/tests/test_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/dltile/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dltile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dltile/_tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dltile/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dltile/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dltile/rasterize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/dltile/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dltile/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dltile/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dltile/tests/test_dltiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dltile/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dltile/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dltile/utm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/dotdict/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dotdict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dotdict/dotdict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/dotdict/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dotdict/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/dotdict/tests/test_dotdict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/geo/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53135 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/geo/geocontext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/geo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/geo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23527 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/geo/tests/test_geocontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/geo/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/geo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/http/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/http/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/http/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/http/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/http/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/http/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/http/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/http/tests/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/http/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/http/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/http/tests/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/property_filtering/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/property_filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/property_filtering/filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/property_filtering/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/property_filtering/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/property_filtering/tests/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/retry/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/retry/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/retry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/retry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/retry/tests/test_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/shapely_support/
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/shapely_support/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/shapely_support/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/shapely_support/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/threading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/threading/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/common/threading/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/threading/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/common/threading/tests/test_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.634655 descarteslabs-2.0.2/descarteslabs/core/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26184 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/compute/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/compute/compute_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/descarteslabs/core/compute/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/compute/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/compute/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/compute/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/compute/tests/test_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/descarteslabs/core/geo/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/descarteslabs/core/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/scenes/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    33638 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/scenes/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    28225 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/scenes/scenecollection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/scenes/search_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/descarteslabs/core/scenes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/scenes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/scenes/tests/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/scenes/tests/test_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/scenes/tests/test_scenecollection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/scenes/tests/test_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/descarteslabs/core/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/descarteslabs/core/third_party/boltons/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/third_party/boltons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32185 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/third_party/boltons/funcutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/descarteslabs/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/descarteslabs/geo/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/descarteslabs/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/scenes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/descarteslabs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/descarteslabs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:17:43.622655 descarteslabs-2.0.2/descarteslabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-26 22:17:43.000000 descarteslabs-2.0.2/descarteslabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-06-26 22:17:43.000000 descarteslabs-2.0.2/descarteslabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 22:17:43.000000 descarteslabs-2.0.2/descarteslabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 22:17:43.000000 descarteslabs-2.0.2/descarteslabs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-26 22:17:43.000000 descarteslabs-2.0.2/descarteslabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 22:17:43.000000 descarteslabs-2.0.2/descarteslabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 22:17:43.638655 descarteslabs-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-26 22:17:39.000000 descarteslabs-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    86754 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.106923 descarteslabs-2.0.3/descarteslabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.106923 descarteslabs-2.0.3/descarteslabs/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29383 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.106923 descarteslabs-2.0.3/descarteslabs/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/auth/tests/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.106923 descarteslabs-2.0.3/descarteslabs/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.106923 descarteslabs-2.0.3/descarteslabs/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.106923 descarteslabs-2.0.3/descarteslabs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/config/settings.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.106923 descarteslabs-2.0.3/descarteslabs/config/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/config/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/config/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.106923 descarteslabs-2.0.3/descarteslabs/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.106923 descarteslabs-2.0.3/descarteslabs/core/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64062 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36605 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/band.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29762 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/blob_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/blob_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37861 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/catalog_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/catalog_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63243 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50022 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/image_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/image_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/image_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/named_catalog_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118250 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36523 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28972 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16050 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_catalog_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45554 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_image_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_image_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28485 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20303 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/addons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/auth/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/auth/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/scripts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/scripts/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/scripts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/scripts/tests/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35310 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/tests/e2e/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/geotiff_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33684 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41637 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/services/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/service/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29553 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/client/services/service/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/service/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19843 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/services/service/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.110923 descarteslabs-2.0.3/descarteslabs/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/client/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/client/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/client/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/client/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/client/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/client/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/collection/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/collection/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/collection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/collection/tests/test_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/display/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/display/_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/display/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/display/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/display/tests/test_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/dltile/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dltile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dltile/_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dltile/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dltile/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dltile/rasterize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/dltile/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dltile/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dltile/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dltile/tests/test_dltiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dltile/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dltile/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dltile/utm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/dotdict/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dotdict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dotdict/dotdict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/dotdict/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dotdict/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/dotdict/tests/test_dotdict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53135 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/geo/geocontext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/geo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/geo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23527 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/geo/tests/test_geocontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/geo/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/geo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/http/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/http/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/http/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/http/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/http/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/http/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/http/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/http/tests/test_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/http/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/http/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/http/tests/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/property_filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/property_filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16948 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/property_filtering/filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/property_filtering/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/property_filtering/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/property_filtering/tests/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/retry/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/retry/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.114923 descarteslabs-2.0.3/descarteslabs/core/common/retry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/retry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/retry/tests/test_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/common/shapely_support/
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/shapely_support/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/common/shapely_support/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/shapely_support/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/common/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/threading/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/common/threading/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/threading/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/common/threading/tests/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42577 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/compute/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/compute/compute_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/compute/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/compute/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/compute/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16900 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/compute/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/compute/tests/test_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/scenes/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33638 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/scenes/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28225 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/scenes/scenecollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/scenes/search_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/scenes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/scenes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/scenes/tests/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/scenes/tests/test_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/scenes/tests/test_scenecollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/scenes/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/third_party/boltons/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/third_party/boltons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32185 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/third_party/boltons/funcutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/scenes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/descarteslabs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/descarteslabs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:50.106923 descarteslabs-2.0.3/descarteslabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 23:13:50.000000 descarteslabs-2.0.3/descarteslabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-07-13 23:13:50.000000 descarteslabs-2.0.3/descarteslabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 23:13:50.000000 descarteslabs-2.0.3/descarteslabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-13 23:13:50.000000 descarteslabs-2.0.3/descarteslabs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-13 23:13:50.000000 descarteslabs-2.0.3/descarteslabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 23:13:50.000000 descarteslabs-2.0.3/descarteslabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 23:13:50.118923 descarteslabs-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-07-13 23:13:45.000000 descarteslabs-2.0.3/setup.py
```

### Comparing `descarteslabs-2.0.2/LICENSE` & `descarteslabs-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/PKG-INFO` & `descarteslabs-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: descarteslabs
-Version: 2.0.2
+Version: 2.0.3
 Summary: Descartes Labs Python Client
 Home-page: https://github.com/descarteslabs/descarteslabs-python
 Author: Descartes Labs
 Author-email: hello@descarteslabs.com
 License: Apache 2.0
-Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v2.0.2.tar.gz
+Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v2.0.3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `descarteslabs-2.0.2/README.md` & `descarteslabs-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,31 @@
 The `descarteslabs` python package, available at [https://pypi.org/project/descarteslabs/](https://pypi.org/project/descarteslabs/), provides client-side access to the Descartes Labs Platform for our customers. You must be a registered customer with access to our Descartes Labs Platform before you can make use of this package with our platform.
 
 The documentation for the latest release can be found at [https://docs.descarteslabs.com](https://docs.descarteslabs.com). For any issues please request Customer Support at [https://support.descarteslabs.com](https://support.descarteslabs.com).
 
 Changelog
 =========
 
+## [Unreleased]
+
+## [2.0.3] - 2023-07-13
+
+### Compute
+
+- Allow deletion of `Function` objects.
+  - Deleting a Function will deleted all associated Jobs.
+- Allow deletion of `Job` objects.
+  - Deleting a Job will delete all associated resources (logs, results, etc). 
+- Added attribute filter to `Function` and `Job` objects.
+  - Attributes marked `filterable=True` can be used to filter objects on the compute backend api.
+  - Minor optimization to `Job.iter_results` which now uses backend filters to load successful jobs.
+- `Function` bundling has been enhanced.
+  - New `include_modules` and `include_data` parameters allow for multiple other modules, non-code data files, etc to be added to the code bundle.
+  - The `requirements` parameter has been improved to allow a user to pass a path to their own `requirements.txt` file instead of a list of strings.
+
 ## [2.0.2] - 2023-06-26
 
 ### Catalog
 
 - Allow data type `int32` in geotiff downloads.
 - `BlobCollection` now importable from `descarteslabs.catalog`.
 
@@ -813,15 +830,15 @@
 - Field access on `Feature`, `FeatureCollection`, `Geometry`, and `GeomeryCollection` no longer fails.
 - In `from_id`, processing level 'cubespline' no longer fails.
 
 
 ## [1.0.0] - 2020-01-20
 
 | As of January 1st, 2020, the client library no longer supports Python 2. For more information, please contact support@descarteslabs.com. For help with porting to Python 3, please visit https://docs.python.org/3/howto/pyporting.html. |
-| --------- |
+| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 
 ### Catalog client
 - There is an entirely new backend supporting asynchronous uploads of image files and ndarrays with
   the catalog client. There are minor changes to the `ImageUpload` class (a new `events` field has subsumed
   `errors`, and the `job_id` field has been removed) but the basic interface is unchanged so most
   code will keep functioning without any changes.
 - It is now possible to cancel image uploads.
```

### Comparing `descarteslabs-2.0.2/descarteslabs/__init__.py` & `descarteslabs-2.0.3/descarteslabs/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/auth/__init__.py` & `descarteslabs-2.0.3/descarteslabs/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/auth/auth.py` & `descarteslabs-2.0.3/descarteslabs/auth/auth.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/auth/tests/test_auth.py` & `descarteslabs-2.0.3/descarteslabs/auth/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/catalog/__init__.py` & `descarteslabs-2.0.3/descarteslabs/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/compute/__init__.py` & `descarteslabs-2.0.3/descarteslabs/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/config/__init__.py` & `descarteslabs-2.0.3/descarteslabs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/config/settings.toml` & `descarteslabs-2.0.3/descarteslabs/config/settings.toml`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/config/tests/test_config.py` & `descarteslabs-2.0.3/descarteslabs/config/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/attributes.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/attributes.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/band.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/band.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/blob.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/blob.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/blob_download.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/blob_download.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/blob_upload.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/blob_upload.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/catalog_base.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/catalog_base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/catalog_client.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/catalog_client.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/helpers.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/helpers.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/image.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/image.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/image_collection.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/image_collection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/image_types.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/image_types.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/image_upload.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/image_upload.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/named_catalog_base.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/named_catalog_base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/product.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/product.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/scaling.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/scaling.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/search.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/search.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/base.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/mock_data.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/mock_data.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_attributes.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_band.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_band.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_catalog_base.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_catalog_base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_download.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_filters.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_image.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_image_collection.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_image_collection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_image_upload.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_image_upload.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_product.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_product.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_scaling.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_search.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/catalog/tests/test_summary.py` & `descarteslabs-2.0.3/descarteslabs/core/catalog/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/client/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,7 +28,21 @@
     warnings.warn(msg, FutureWarning)
 
 if sys.version_info >= (3, 12):
     msg = "Python version {}.{} is not supported yet. You may encounter unexpected errors.".format(
         sys.version_info.major, sys.version_info.minor
     )
     warnings.warn(msg, FutureWarning)
+
+
+def clear_client_state():
+    """Clear all cached client state."""
+    from .auth import Auth
+    from ..common.http.service import DefaultClientMixin
+    from ..scenes.helpers import BANDS_BY_PRODUCT_CACHE
+
+    Auth.set_default_auth(None)
+    DefaultClientMixin.clear_all_default_clients()
+    BANDS_BY_PRODUCT_CACHE.clear()
+
+
+__all__ = ["clear_client_state"]
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/addons.py` & `descarteslabs-2.0.3/descarteslabs/core/client/addons.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/auth/cli.py` & `descarteslabs-2.0.3/descarteslabs/core/client/auth/cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/auth/tests/test_cli.py` & `descarteslabs-2.0.3/descarteslabs/core/client/auth/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/deprecation.py` & `descarteslabs-2.0.3/descarteslabs/core/client/deprecation.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/exceptions.py` & `descarteslabs-2.0.3/descarteslabs/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/scripts/__main__.py` & `descarteslabs-2.0.3/descarteslabs/core/client/scripts/__main__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/scripts/cli.py` & `descarteslabs-2.0.3/descarteslabs/core/client/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/scripts/tests/test_scripts.py` & `descarteslabs-2.0.3/descarteslabs/core/client/scripts/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/cli.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/metadata.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/tests/e2e/test_metadata.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/tests/e2e/test_metadata.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/metadata/tests/test_metadata.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/metadata/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/raster/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/raster/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/raster/cli.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/raster/cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/raster/geotiff_utils.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/raster/geotiff_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/raster/raster.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/raster/raster.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/test_raster.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/service/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/service/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/service/api_service.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/service/api_service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/service/service.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/service/service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/services/service/tests/test_service.py` & `descarteslabs-2.0.3/descarteslabs/core/client/services/service/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/client/version.py` & `descarteslabs-2.0.3/descarteslabs/core/client/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/client/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/third_party/boltons/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,11 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .attributes import Attribute, DatetimeAttribute
-from .document import Document, DocumentState
+from . import funcutils
 
-__all__ = ["Attribute", "DatetimeAttribute", "Document", "DocumentState"]
+__all__ = ["funcutils"]
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/client/attributes.py` & `descarteslabs-2.0.3/descarteslabs/core/common/client/attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,30 +11,35 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime, timezone
 from typing import TYPE_CHECKING, Callable, Type, TypeVar, Union
 
+from ..property_filtering import Property
+from .sort import Sort
+
 if TYPE_CHECKING:
     from .document import Document
 
 T = TypeVar("T")
 
 
-class Attribute(object):
+class Attribute(Property):
     """An attribute defined on a Document."""
 
     def __init__(
         self,
         type: Type[T] = None,
         default: Union[T, Callable] = None,
         doc: str = None,
+        filterable: bool = False,
         mutable: bool = True,
         readonly: bool = False,
+        sortable: bool = False,
         sticky: bool = False,
     ):
         """Defines a document attribute.
 
         Examples
         --------
         .. code::
@@ -51,31 +56,38 @@
         ----------
         default : Any, Callable, None
             The default value for the attribute when no value is defined.
             If a callable is provided, it will be called once when the attribute is first
             fetched.
         doc : str, None
             Sets the doc string for the attribute.
+        filterable: bool, False
+            If set, the attribute can be used as a filter.
         mutable : bool, True
             If not set, the attribute will be immutable and can only be set once.
         readonly : bool, False
             If set, the attribute cannot be modified by the user.
             This is designed for attributes set and managed exclusively by the server.
+        sortable : bool, False
+            If set, the attribute can be used to sort results.
         sticky : bool, False
             If set, the attribute exists on the client only.
             This attribute will be ignored when set by the server.
         """
+        super().__init__(None)
 
         if sticky and readonly:
             raise ValueError("Using sticky and readonly together does not make sense.")
 
         self.type = type
         self.default = default
+        self.filterable = filterable
         self.mutable = mutable
         self.readonly = readonly
+        self.sortable = sortable
         self.sticky = sticky
 
         if doc is None and type:
             doc = type.__doc__
 
         doc_modifiers = []
 
@@ -167,14 +179,23 @@
     def __delete__(self, instance: "Document", force: bool = False):
         """Called when an attribute is deleted."""
         if not force:
             self._raise_immutable("delete", instance)
 
         instance._attributes.pop(self.name, None)
 
+    def __neg__(self):
+        return self._to_sort(ascending=False)
+
+    def _to_sort(self, ascending: bool = True):
+        if not self.sortable:
+            raise ValueError(f"Cannot sort on property: {self.name}")
+
+        return Sort(self.name, ascending)
+
     def _raise_immutable(self, operation: str, instance: "Document"):
         """Raises an error when an attribute cannot be modified."""
         if self.readonly:
             raise ValueError(
                 "Unable to {} readonly attribute '{}'".format(operation, self.name)
             )
 
@@ -195,14 +216,25 @@
         except (ValueError, TypeError) as e:
             raise ValueError(f"Unable to assign {type(value)} to type {self.type}: {e}")
 
     def serialize(self, value):
         """Serializes a value to a JSON encodable type."""
         return value
 
+    def __repr__(self):
+        return (
+            "<Attribute name={} filterable={} mutable={} readonly={} sticky={}>".format(
+                repr(self.name),
+                self.filterable,
+                self.mutable,
+                self.readonly,
+                self.sticky,
+            )
+        )
+
 
 class DatetimeAttribute(Attribute):
     """Represents a datetime attribute on a document."""
 
     def __init__(
         self,
         timezone=None,
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/client/document.py` & `descarteslabs-2.0.3/descarteslabs/core/common/client/document.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from enum import auto
-from typing import Any, Dict
+from typing import Any, Dict, Tuple
 
 from strenum import LowercaseStrEnum
 
 from .attributes import Attribute
 
 
 class DocumentState(LowercaseStrEnum):
@@ -29,18 +29,35 @@
 
 class Document(object):
     """An Object or Document in a Descartes Labs service."""
 
     def __init__(self, saved=False, **kwargs) -> None:
         self._attributes = dict()
         self._modified = set()
-        self._fill(kwargs, remote=saved)
+
+        if saved:
+            self._load_from_remote(kwargs)
+        else:
+            self._fill(kwargs, remote=saved)
+
         self._saved = saved
         self._deleted = False
 
+    def __getattribute__(self, name: str) -> Any:
+        try:
+            deleted = object.__getattribute__(self, "_deleted")
+        except AttributeError:
+            deleted = False
+
+        if deleted and name != "state" and not name.startswith("_"):
+            class_name = object.__getattribute__(self, "__class__").__name__
+            raise AttributeError(f"{class_name} has been deleted")
+
+        return object.__getattribute__(self, name)
+
     def _clear_modified(self):
         """Clears the list of modified attributes."""
         self._modified = set()
 
     def _get_attributes(self) -> Dict[str, Attribute]:
         """Returns all of the Attributes in the document.
 
@@ -87,14 +104,33 @@
         Parameters
         ----------
         data : dict
             The response json to populate the document with.
         """
         self._fill(data, ignore_missing=True, remote=True)
 
+    @classmethod
+    def _serialize_filter_attribute(cls, name: str, value: Any) -> Tuple[str, Any]:
+        """Serializes a filter attribute.
+
+        Parameters
+        ----------
+        name : str
+            The name of the attribute.
+        value : Any
+            The value of the attribute.
+
+        Returns
+        -------
+        Tuple[str, Any]
+            The serialized attribute name and value.
+        """
+        attribute: Attribute = getattr(cls, name)
+        return (attribute.name, attribute.serialize(attribute.deserialize(value)))
+
     def update(self, ignore_missing=False, **kwargs):
         """Updates the document setting multiple attributes at a time.
 
         Parameters
         ----------
         ignore_missing : bool, False
             If set, unknown attributes will be ignored.
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/client/tests/test_attributes.py` & `descarteslabs-2.0.3/descarteslabs/core/common/client/tests/test_attributes.py`

 * *Files 11% similar despite different names*

```diff
@@ -89,14 +89,38 @@
         assert "Unable to set readonly attribute 'id'" == str(ctx.exception)
 
         doc = MyDocument()
         with self.assertRaises(ValueError) as ctx:
             doc.id = "123"
         assert "Unable to set readonly attribute 'id'" == str(ctx.exception)
 
+    def test_init_from_server(self):
+        now = datetime.utcnow()
+        # 2000-01-01, if set to 0 astimezone on windows in python 3.8 will error
+        timestamp = 946710000
+        data = {
+            "id": 1,
+            "name": "server",
+            "local": "server",
+            "once": 2,
+            "default": datetime.fromtimestamp(timestamp).isoformat(),
+            "created_at": now.isoformat(),
+            "extra": "should be ignored",
+        }
+
+        doc = MyDocument(**data, saved=True)
+        assert doc.id == 1
+        assert doc.name == "server"
+        assert doc.local == "local"
+        assert doc.once == 2
+        assert doc.default == datetime.fromtimestamp(timestamp, tz=timezone.utc)
+        assert doc.created_at == now.replace(tzinfo=timezone.utc)
+        with self.assertRaises(AttributeError):
+            doc.extra
+
     def test_set_from_server(self):
         now = datetime.utcnow()
         doc = MyDocument(name="local", once="1", default=now)
         # 2000-01-01, if set to 0 astimezone on windows in python 3.8 will error
         timestamp = 946710000
         assert doc.once == 1
 
@@ -123,14 +147,22 @@
             "name": "local",
             "local": "local",
             "once": 1,
             "default": doc.default.isoformat(),
             "created_at": None,
         }
 
+    def test_deleted(self):
+        doc = MyDocument(name="local", once="1")
+        doc._deleted = True
+
+        with self.assertRaises(AttributeError) as ctx:
+            doc.name
+        assert "MyDocument has been deleted" == str(ctx.exception)
+
 
 class TestDatetimeAttribute(unittest.TestCase):
     def test_local_time(self):
         class TzTest(Document):
             date: datetime = DatetimeAttribute(timezone=pytz.timezone("MST"))
 
         now = datetime.utcnow()
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/collection/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/common/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/collection/collection.py` & `descarteslabs-2.0.3/descarteslabs/core/common/collection/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,34 +12,41 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 A list-based sequence with helper methods, which serves as the base class for `SceneCollection`.
 """
 
-import itertools
 import collections
+import itertools
+from typing import Generic, TypeVar
 
 from ...client.deprecation import deprecate
 from ...common.property_filtering.filtering import Expression
 
+T = TypeVar("T")
+
 
 # TODO: maybe subclass collections.UserList?
-class Collection(object):
+class Collection(Generic[T]):
     """
     List-based sequence with convenience methods for mapping and filtering,
     and NumPy-style fancy indexing
     """
 
-    def __init__(self, iterable=None):
+    def __init__(self, iterable=None, item_type=None):
         if iterable is None:
             self._list = []
         else:
             self._list = list(iterable)
-            item_type = getattr(self, "_item_type", None)
+            if item_type is not None:
+                self._item_type = item_type
+            else:
+                item_type = getattr(self, "_item_type", None)
+
             if item_type is not None:
                 if not all(map(lambda i: isinstance(i, item_type), self._list)):
                     raise ValueError(
                         f"item is not of required type {item_type.__name__}"
                     )
 
     def __getitem__(self, idx):
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/collection/tests/test_collection.py` & `descarteslabs-2.0.3/descarteslabs/core/common/collection/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/display/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/common/display/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/display/_display.py` & `descarteslabs-2.0.3/descarteslabs/core/common/display/_display.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/display/tests/test_display.py` & `descarteslabs-2.0.3/descarteslabs/core/common/display/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dltile/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dltile/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dltile/_tiling.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dltile/_tiling.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dltile/conversions.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dltile/conversions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dltile/exceptions.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dltile/exceptions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dltile/rasterize.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dltile/rasterize.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dltile/tests/test_conversions.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dltile/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dltile/tests/test_dltiles.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dltile/tests/test_dltiles.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dltile/tile.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dltile/tile.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dltile/utils.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dltile/utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dltile/utm.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dltile/utm.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dotdict/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dotdict/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dotdict/dotdict.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dotdict/dotdict.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/dotdict/tests/test_dotdict.py` & `descarteslabs-2.0.3/descarteslabs/core/common/dotdict/tests/test_dotdict.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/geo/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/common/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/geo/geocontext.py` & `descarteslabs-2.0.3/descarteslabs/core/common/geo/geocontext.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/geo/tests/test_geocontext.py` & `descarteslabs-2.0.3/descarteslabs/core/common/geo/tests/test_geocontext.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/geo/tests/test_utils.py` & `descarteslabs-2.0.3/descarteslabs/core/common/geo/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/geo/utils.py` & `descarteslabs-2.0.3/descarteslabs/core/common/geo/utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/http/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/http/authorization.py` & `descarteslabs-2.0.3/descarteslabs/core/common/http/authorization.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/http/proxy.py` & `descarteslabs-2.0.3/descarteslabs/core/common/http/proxy.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/http/retry.py` & `descarteslabs-2.0.3/descarteslabs/core/common/http/retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/http/service.py` & `descarteslabs-2.0.3/descarteslabs/core/common/http/service.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,7 +41,16 @@
         client
         """
 
         if not isinstance(client, cls):
             raise ValueError(f"client must be an instance of {cls.__name__}")
 
         cls._instance = client
+
+    @classmethod
+    def clear_all_default_clients(cls):
+        """Clear all default clients of this class and all its subclasses."""
+
+        cls._instance = None
+
+        for subclass in cls.__subclasses__():
+            subclass.clear_all_default_clients()
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/http/session.py` & `descarteslabs-2.0.3/descarteslabs/core/common/http/session.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/http/tests/test_authorization.py` & `descarteslabs-2.0.3/descarteslabs/core/common/http/tests/test_authorization.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/http/tests/test_proxy.py` & `descarteslabs-2.0.3/descarteslabs/core/common/http/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/http/tests/test_retry.py` & `descarteslabs-2.0.3/descarteslabs/core/common/http/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/http/tests/test_service.py` & `descarteslabs-2.0.3/descarteslabs/core/common/http/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/property_filtering/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/common/property_filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/property_filtering/filtering.py` & `descarteslabs-2.0.3/descarteslabs/core/common/property_filtering/filtering.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+import functools
 import re
 
 
 class Expression(object):
     """An expression is the result of a filtering operation.
 
     An expression can contain a :py:class:`Property`, a comparison operator, and a
@@ -98,14 +99,17 @@
 
     def _convert_name_value_pair(self, name, value):
         if hasattr(value, "id"):
             return name + "_id", value.id
         else:
             return name, value
 
+    def jsonapi_serialize(self, model=None):
+        raise NotImplementedError
+
 
 # A convention was added to allow for serialization of catalog V2 attributes
 # If a model is given, the model class method `_serialize_filter_attribute` will be
 # called to retrieve the serialized value of an attribute.
 
 # A second convention was added to allow for Catalog V2 object to be used
 # instead of the name for == and != operations, and to convert
@@ -265,48 +269,45 @@
 
 class LikeExpression(Expression):
     """Whether a property value matches the given wildcard expression.
 
     The wildcard expression can contain ``%`` for zero or more characters and
     ``_`` for a single character.
 
-    This can only be used in expressions for the ``Vector`` product.
+    This expression is not supported by the `Catalog` service.
     """
 
     def __init__(self, name, value):
         self.name = name
         self.value = value
 
     def serialize(self):
         return {"like": {self.name: self.value}}
 
     def jsonapi_serialize(self, model=None):
-        # catalog does not support this, and at present this method
-        # is only used for Catalog V2. If it does start being used
-        # for something else, we'll have to generate the error server
-        # side
-        raise TypeError("'like' expression is not supported")
-        # name, value = (
-        #     model._serialize_filter_attribute(self.name, self.value)
-        #     if model
-        #     else (self.name, self.value)
-        # )
-        # return (name, {"name": name, "op": "ilike", "val": value})
+        name, value = (
+            model._serialize_filter_attribute(self.name, self.value)
+            if model
+            else (self.name, self.value)
+        )
+        return {"name": name, "op": "ilike", "val": value}
 
     def evaluate(self, obj):
         expr = re.escape(self.value).replace("_", ".").replace("%", ".*")
         return re.match(f"^{expr}$", getattr(obj, self.name)) is not None
 
 
-class AndExpression(object):
-    """``True`` if both expressions are ``True``, ``False`` otherwise."""
-
+class LogicalExpression(object):
     def __init__(self, parts):
         self.parts = parts
 
+
+class AndExpression(LogicalExpression):
+    """``True`` if both expressions are ``True``, ``False`` otherwise."""
+
     def __and__(self, other):
         if isinstance(other, AndExpression):
             self.parts.extend(other.parts)
             return self
         if isinstance(other, (OrExpression, Expression)):
             self.parts.append(other)
             return self
@@ -328,20 +329,17 @@
         for part in self.parts:
             if not part.evaluate(obj):
                 return False
 
         return True
 
 
-class OrExpression(object):
+class OrExpression(LogicalExpression):
     """``True`` if either expression is ``True``, ``False`` otherwise."""
 
-    def __init__(self, parts):
-        self.parts = parts
-
     def __or__(self, other):
         if isinstance(other, OrExpression):
             self.parts.extend(other.parts)
             return self
         if isinstance(other, (AndExpression, Expression)):
             self.parts.append(other)
             return self
@@ -373,14 +371,30 @@
         # such as 10 < a < 20
         self.parts[op] = other
         return RangeExpression(self.name, self.parts.copy())
 
     return f
 
 
+def check_can_filter(fn):
+    """Decorator to check whether a property can be filtered on.
+
+    This is used by Documents in some object oriented clients.
+    """
+
+    @functools.wraps(fn)
+    def wrapper(self, *args, **kwargs):
+        if getattr(self, "filterable", True):
+            return fn(self, *args, **kwargs)
+        else:
+            raise ValueError(f"Cannot filter on property: {self.name}")
+
+    return wrapper
+
+
 class Property(object):
     """A filter property that can be used in an expression.
 
     Although you can generate filter properties by instantiating this class, a more
     convenient method is to use a
     :py:class:`~descarteslabs.common.property_filtering.filtering.Properties`
     instance.
@@ -397,34 +411,39 @@
     >>> e = Property("modified") > "2020-01-01"
     """
 
     def __init__(self, name, parts=None):
         self.name = name
         self.parts = parts or {}
 
-    __ge__ = range_expr("gte")
-    __gt__ = range_expr("gt")
-    __le__ = range_expr("lte")
-    __lt__ = range_expr("lt")
+    __ge__ = check_can_filter(range_expr("gte"))
+    __gt__ = check_can_filter(range_expr("gt"))
+    __le__ = check_can_filter(range_expr("lte"))
+    __lt__ = check_can_filter(range_expr("lt"))
 
+    @check_can_filter
     def __eq__(self, other):
         return EqExpression(self.name, other)
 
+    @check_can_filter
     def __ne__(self, other):
         return NeExpression(self.name, other)
 
+    @check_can_filter
     def __repr__(self):
         return "<Property {}>".format(self.name)
 
+    @check_can_filter
     def prefix(self, prefix):
         """Compare against a prefix string."""
         return PrefixExpression(self.name, prefix)
 
     startswith = prefix
 
+    @check_can_filter
     def like(self, wildcard):
         """Compare against a wildcard string.
 
         This can only be used in expressions for the ``Vector`` service.
         This allows for wildcards, e.g. ``like("bar%foo")`` where any
         string that starts with ``'bar'`` and ends with ``'foo'`` will be
         matched.
@@ -435,14 +454,15 @@
         To escape either of these wilcard characters prepend it
         with a backslash, which becomes a double backslash in the
         python string, i.e. use ``like("bar\\\\%foo")`` to match exactly
         ``'bar%foo'``.
         """
         return LikeExpression(self.name, wildcard)
 
+    @check_can_filter
     def any_of(self, iterable):
         """The property must have any of the given values.
 
         Asserts that this property must have a value equal to one of the
         values in the given iterable. This can be thought of as behaving
         like an ``in`` expression in Python or an ``IN`` expression in SQL.
         """
@@ -458,22 +478,24 @@
             # we can do here to create such an expression, so instead error to the user
             # since they surely didn't mean this.
             raise ValueError("in_ expression requires at least one item")
 
     in_ = any_of
 
     @property
+    @check_can_filter
     def isnull(self):
         """Whether a property value is ``None`` or ``[]``.
 
         This can only be used in expressions for the ``Catalog`` service.
         """
         return IsNullExpression(self.name)
 
     @property
+    @check_can_filter
     def isnotnull(self):
         """Whether a property value is not ``None`` or ``[]``.
 
         This can only be used in expressions for the ``Catalog`` service.
         """
         return IsNotNullExpression(self.name)
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/property_filtering/tests/test_filtering.py` & `descarteslabs-2.0.3/descarteslabs/core/common/property_filtering/tests/test_filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
 
 import pytest
-from ....catalog import Product, MaskBand
-from .. import (
-    GenericProperties,
-    Properties,
-    Property,
-)
+
+from ....catalog import MaskBand, Product
+from .. import GenericProperties, Properties, Property
 
 
 def v1_expression(expression, expected_expression):
     assert expression.serialize() == expected_expression
 
 
 def v2_expression(expression, expected_expression):
@@ -125,16 +122,16 @@
     property = Property(name)
     expression = property.like(value)
 
     assert expression.name == name
 
     v1_expression(expression, dict(like=dict(description=value)))
 
-    with pytest.raises(TypeError):
-        expression.jsonapi_serialize()
+    expected = dict(name=name, op="like", val=value)
+    expression.jsonapi_serialize() == expected
 
 
 def test_any_of_expression():
     name = "tags"
     value = ["one", "two"]
 
     property = Property(name)
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/registry/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/common/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/registry/registry.py` & `descarteslabs-2.0.3/descarteslabs/core/common/registry/registry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/retry/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/common/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/retry/retry.py` & `descarteslabs-2.0.3/descarteslabs/core/common/retry/retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/retry/tests/test_retry.py` & `descarteslabs-2.0.3/descarteslabs/core/common/retry/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/shapely_support/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/common/shapely_support/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py` & `descarteslabs-2.0.3/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/threading/local.py` & `descarteslabs-2.0.3/descarteslabs/core/common/threading/local.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/common/threading/tests/test_local.py` & `descarteslabs-2.0.3/descarteslabs/core/common/threading/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/compute/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/compute/compute_client.py` & `descarteslabs-2.0.3/descarteslabs/core/compute/compute_client.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/compute/tests/base.py` & `descarteslabs-2.0.3/descarteslabs/core/compute/tests/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 import json
 import json as jsonlib
 import time
+import urllib.parse
 import uuid
 from datetime import datetime
 from unittest import TestCase
 
 import responses
 from requests import PreparedRequest
 
@@ -107,34 +108,73 @@
             "creation_date": self.now.isoformat(),
             "status": FunctionStatus.AWAITING_BUNDLE,
         }
         function.update(data)
 
         return function
 
-    def assert_url_called(self, uri, times=1, json=None, body=None):
+    def assert_url_called(self, uri, times=1, json=None, body=None, params=None):
         if json and body:
             raise ValueError("Using json and body together does not make sense")
 
-        calls = [call for call in responses.calls if call.request.url.endswith(uri)]
+        url = f"{self.compute_url}{uri}"
+        calls = [call for call in responses.calls if call.request.url.startswith(url)]
         assert calls, f"No requests were made to uri: {uri}"
 
         data = json or body
         matches = []
+        calls_with_params = set()
+
         for call in calls:
             request: PreparedRequest = call.request
 
             if json is not None:
                 request_data = jsonlib.loads(request.body)
             else:
                 request_data = request.body
 
-            if data is None or request_data == data:
+            if params is not None:
+                request_params = {}
+
+                for key, value in urllib.parse.parse_qsl(
+                    urllib.parse.urlsplit(request.url).query
+                ):
+                    try:
+                        value = jsonlib.loads(value)
+                    except jsonlib.JSONDecodeError:
+                        value = value
+
+                    if key in request_params:
+                        values = request_params[key]
+
+                        if not isinstance(values, list):
+                            values = [values]
+
+                        values.append(value)
+                    else:
+                        values = value
+
+                    request_params[key] = values
+
+                if request_params:
+                    calls_with_params.add(jsonlib.dumps(request_params))
+            else:
+                request_params = None
+
+            if (data is None or request_data == data) and (
+                params is None or request_params == params
+            ):
                 matches.append(call)
 
         count = len(matches)
         msg = f"Expected {times} calls found {count} for {uri}"
 
         if data is not None:
             msg += f" with data: {data}"
 
+        if params is not None:
+            msg += f" with params: {params}"
+
+            if calls_with_params:
+                msg += "\n\nParams:\n" + "\n".join(calls_with_params)
+
         assert count == times, msg
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/compute/tests/test_function.py` & `descarteslabs-2.0.3/descarteslabs/core/compute/tests/test_function.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import gzip
 import json
 import random
 import string
-from collections.abc import Iterator
+import sys
+import unittest
+from collections.abc import Iterable
 from datetime import timezone
 
 import responses
 
 from descarteslabs import exceptions
 from descarteslabs.compute import Function, FunctionStatus, Job, JobStatus
 
@@ -117,17 +119,18 @@
             fn.save()
         assert fn.state == "new"
         assert "image" in str(ctx.exception)
         assert "Field is required" in str(ctx.exception)
         assert "Must be a valid docker image" in str(ctx.exception)
 
     @responses.activate
+    @unittest.skipIf(sys.version_info >= (3, 11), "Python >= 3.11 not supported")
     def test_create_function(self):
         params = {
-            "image": "python3:8",
+            "image": "python3.8",
             "cpus": 1,
             "memory": 8 * 1024,
             "maximum_concurrency": 1,
             "timeout": 60,
             "retry_count": 1,
         }
 
@@ -144,17 +147,18 @@
         assert fn.name == "test_compute_fn"
         assert fn.status == FunctionStatus.BUILDING
         assert fn.creation_date == self.now.replace(tzinfo=timezone.utc)
         assert fn.id
         self.assertDictContainsSubset(params, fn.to_dict())
 
     @responses.activate
+    @unittest.skipIf(sys.version_info >= (3, 11), "Python >= 3.11 not supported")
     def test_call_creates_function(self):
         params = {
-            "image": "python3:8",
+            "image": "python3.8",
             "cpus": 1,
             "memory": 8 * 1024,
             "maximum_concurrency": 1,
             "timeout": 60,
             "retry_count": 1,
         }
 
@@ -181,23 +185,25 @@
         self.assertDictContainsSubset(job_params, job.to_dict())
 
     @responses.activate
     def test_bundle_lambda(self):
         fn = Function(lambda: 1)
         with self.assertRaises(ValueError) as ctx:
             fn.save()
-        assert "Cannot execute lambda functions" in str(ctx.exception)
+        assert "Compute main function cannot be a lambda expression" in str(
+            ctx.exception
+        )
 
 
 class TestListFunctions(FunctionTestCase):
     @responses.activate
     def test_list_function_empty(self):
         self.mock_response(responses.GET, "/functions", json=self.make_page([]))
         fn_iter = Function.list()
-        assert isinstance(fn_iter, Iterator)
+        assert isinstance(fn_iter, Iterable)
         assert list(fn_iter) == []
 
     @responses.activate
     def test_list_function(self):
         self.mock_response(
             responses.GET,
             "/functions",
@@ -224,18 +230,18 @@
     @responses.activate
     def test_list_function_filters(self):
         self.mock_response(
             responses.GET,
             "/functions",
             json=self.make_page([self.generate_function()]),
         )
-        next(Function.list(status=FunctionStatus.BUILDING))
+        list(Function.list(status=FunctionStatus.BUILDING))
         self.assert_url_called("/functions?page_size=100&status=building", 1)
 
-        next(
+        list(
             Function.list(
                 status=[FunctionStatus.BUILDING, FunctionStatus.AWAITING_BUNDLE]
             )
         )
         self.assert_url_called(
             "/functions?page_size=100&status=building&status=awaiting_bundle", 1
         )
@@ -268,14 +274,93 @@
         buffer = gzip.compress(log_bytes)
         self.mock_response(responses.GET, "/functions/some-id/log", body=buffer)
 
         fn = Function(id="some-id", saved=True)
         fn.build_log()
 
     @responses.activate
+    def test_delete(self):
+        self.mock_response(
+            responses.GET,
+            "/jobs",
+            json=self.make_page(
+                [
+                    self.make_job(id="1", status=JobStatus.SUCCESS),
+                    self.make_job(id="2", status=JobStatus.SUCCESS),
+                    self.make_job(id="3", status=JobStatus.RUNNING),
+                    self.make_job(id="4", status=JobStatus.FAILURE),
+                ]
+            ),
+        )
+        self.mock_response(responses.DELETE, "/jobs/1", status=204)
+        self.mock_response(responses.DELETE, "/jobs/2", status=204)
+        self.mock_response(responses.DELETE, "/jobs/3", status=204)
+        self.mock_response(responses.DELETE, "/jobs/4", status=204)
+        self.mock_response(responses.DELETE, "/functions/some-id", status=204)
+
+        fn = Function(id="some-id", saved=True)
+        fn.delete()
+        self.assert_url_called("/functions/some-id")
+        assert fn._deleted is True
+        assert fn.state == "deleted"
+
+        with self.assertRaises(AttributeError) as ctx:
+            fn.id
+        assert "Function has been deleted" in str(ctx.exception)
+
+    @responses.activate
+    def test_delete_new(self):
+        fn = Function(id="some-id", saved=True)
+        fn._saved = False
+
+        with self.assertRaises(ValueError) as ctx:
+            fn.delete()
+        assert "has not been saved" in str(ctx.exception)
+        assert fn._deleted is False
+        assert fn.state == "new"
+
+    @responses.activate
+    def test_delete_no_jobs(self):
+        self.mock_response(responses.GET, "/jobs", json=self.make_page([]))
+        self.mock_response(responses.DELETE, "/functions/some-id", status=204)
+
+        fn = Function(id="some-id", saved=True)
+        fn.delete()
+        self.assert_url_called("/functions/some-id")
+        assert fn._deleted is True
+        assert fn.state == "deleted"
+
+        with self.assertRaises(AttributeError) as ctx:
+            fn.id
+        assert "Function has been deleted" in str(ctx.exception)
+
+    @responses.activate
+    def test_delete_failed(self):
+        self.mock_response(
+            responses.GET,
+            "/jobs",
+            json=self.make_page(
+                [
+                    self.make_job(id="1", status=JobStatus.SUCCESS),
+                ]
+            ),
+        )
+        self.mock_response(responses.DELETE, "/jobs/1", status=400)
+
+        fn = Function(id="some-id", saved=True)
+
+        with self.assertRaises(Exception):
+            fn.delete()
+
+        self.assert_url_called("/jobs/1")
+        assert fn._deleted is False
+        assert fn.state == "saved"
+        assert fn.id == "some-id"
+
+    @responses.activate
     def test_rerun(self):
         self.mock_response(
             responses.POST,
             "/jobs/rerun",
             json=[self.make_job(function_id="some-id", args=[1, 2])],
         )
 
@@ -343,24 +428,31 @@
         self.mock_response(
             responses.GET,
             "/jobs",
             json=self.make_page(
                 [
                     self.make_job(id="1", status=JobStatus.SUCCESS),
                     self.make_job(id="2", status=JobStatus.SUCCESS),
-                    self.make_job(id="3", status=JobStatus.RUNNING),
-                    self.make_job(id="4", status=JobStatus.FAILURE),
                 ]
             ),
         )
         self.mock_response(responses.GET, "/jobs/1/result", body=json.dumps(1))
         self.mock_response(responses.GET, "/jobs/2/result", body=json.dumps(2))
 
         fn = Function(id="some-id", saved=True)
         assert fn.results() == [1, 2]
+        self.assert_url_called(
+            "/jobs",
+            params={
+                "filter": [
+                    {"op": "eq", "name": "function_id", "val": "some-id"},
+                    {"op": "eq", "name": "status", "val": "success"},
+                ]
+            },
+        )
 
     @responses.activate
     def test_wait_for_completion(self):
         self.mock_response(
             responses.GET,
             "/functions/some-id",
             json=self.make_function(
@@ -432,7 +524,16 @@
 
 class TestFunctionNoApi(BaseTestCase):
     @responses.activate
     def test_no_request_when_saved(self):
         fn = Function(id="some-id", saved=True)
         fn.save()
         assert len(responses.calls) == 0
+
+    @responses.activate
+    def test_deleted(self):
+        fn = Function(id="some-id", saved=True)
+        fn._deleted = True
+
+        with self.assertRaises(AttributeError) as ctx:
+            fn.save()
+        assert "Function has been deleted" in str(ctx.exception)
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/compute/tests/test_job.py` & `descarteslabs-2.0.3/descarteslabs/core/compute/tests/test_job.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,27 +47,38 @@
             assert job.to_dict()
 
         assert len(jobs) == 3
         self.assert_url_called("/jobs?page_size=100", 1)
         self.assert_url_called("/jobs?page_cursor=page2", 1)
 
     @responses.activate
-    def test_list_jobs_filters(self):
+    def test_list_jobs_compatible(self):
         self.mock_response(
             responses.GET,
             "/jobs",
             json=self.make_page([self.make_job()]),
         )
         list(Job.list(status=JobStatus.PENDING, function_id="some-fn"))
         self.assert_url_called(
-            "/jobs?page_size=100&function_id=some-fn&status=pending", 1
+            "/jobs",
+            params={
+                "page_size": 100,
+                "status": "pending",
+                "function_id": "some-fn",
+            },
         )
 
         list(Job.list(status=[JobStatus.PENDING, JobStatus.RUNNING]))
-        self.assert_url_called("/jobs?page_size=100&status=pending&status=running", 1)
+        self.assert_url_called(
+            "/jobs",
+            params={
+                "page_size": 100,
+                "status": ["pending", "running"],
+            },
+        )
 
 
 class TestJob(BaseTestCase):
     @responses.activate
     def test_get(self):
         self.mock_response(
             responses.GET,
@@ -88,14 +99,46 @@
             "id": "some-id",
             "kwargs": {"first": "blah", "second": "blah"},
             "runtime": None,
             "status": JobStatus.PENDING,
         }
 
     @responses.activate
+    def test_delete(self):
+        self.mock_response(responses.DELETE, "/jobs/some-id")
+        job = Job(id="some-id", function_id="some-fn", saved=True)
+        job.delete()
+        self.assert_url_called("/jobs/some-id")
+        assert job._deleted is True
+        assert job.state == "deleted"
+
+    @responses.activate
+    def test_delete_new(self):
+        job = Job(id="some-id", function_id="some-fn", saved=True)
+        job._saved = False
+
+        with self.assertRaises(ValueError) as ctx:
+            job.delete()
+        assert "has not been saved" in str(ctx.exception)
+        assert job._deleted is False
+        assert job.state == "new"
+
+    @responses.activate
+    def test_delete_failed(self):
+        self.mock_response(responses.DELETE, "/jobs/some-id", status=400)
+        job = Job(id="some-id", function_id="some-fn", saved=True)
+
+        with self.assertRaises(Exception):
+            job.delete()
+
+        self.assert_url_called("/jobs/some-id")
+        assert job._deleted is False
+        assert job.state == "saved"
+
+    @responses.activate
     def test_result_empty(self):
         self.mock_response(responses.GET, "/jobs/some-id/result", body=None)
         job = Job(id="some-id", function_id="some-fn", saved=True)
         assert job.result() is None
 
     @responses.activate
     def test_result_json(self):
@@ -201,7 +244,16 @@
 
 class TestJobNoApi(BaseTestCase):
     @responses.activate
     def test_no_request_when_saved(self):
         job = Job(id="some-id", function_id="some-fn", saved=True)
         job.save()
         assert len(responses.calls) == 0
+
+    @responses.activate
+    def test_deleted(self):
+        job = Job(id="some-id", function_id="some-fn", saved=True)
+        job._deleted = True
+
+        with self.assertRaises(AttributeError) as ctx:
+            job.save()
+        assert "Job has been deleted" in str(ctx.exception)
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/scenes/__init__.py` & `descarteslabs-2.0.3/descarteslabs/core/scenes/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/scenes/scene.py` & `descarteslabs-2.0.3/descarteslabs/core/scenes/scene.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/scenes/scenecollection.py` & `descarteslabs-2.0.3/descarteslabs/core/scenes/scenecollection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/scenes/search_api.py` & `descarteslabs-2.0.3/descarteslabs/core/scenes/search_api.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/scenes/tests/mock_data.py` & `descarteslabs-2.0.3/descarteslabs/core/scenes/tests/mock_data.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/scenes/tests/test_scene.py` & `descarteslabs-2.0.3/descarteslabs/core/scenes/tests/test_scene.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/scenes/tests/test_scenecollection.py` & `descarteslabs-2.0.3/descarteslabs/core/scenes/tests/test_scenecollection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/scenes/tests/test_search.py` & `descarteslabs-2.0.3/descarteslabs/core/scenes/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/core/third_party/boltons/__init__.py` & `descarteslabs-2.0.3/descarteslabs/scenes/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import funcutils
-
-__all__ = ["funcutils"]
+from descarteslabs.core.scenes import *  # noqa F401 F403
```

### Comparing `descarteslabs-2.0.2/descarteslabs/core/third_party/boltons/funcutils.py` & `descarteslabs-2.0.3/descarteslabs/core/third_party/boltons/funcutils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/exceptions.py` & `descarteslabs-2.0.3/descarteslabs/exceptions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs/geo/__init__.py` & `descarteslabs-2.0.3/descarteslabs/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/descarteslabs.egg-info/PKG-INFO` & `descarteslabs-2.0.3/descarteslabs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: descarteslabs
-Version: 2.0.2
+Version: 2.0.3
 Summary: Descartes Labs Python Client
 Home-page: https://github.com/descarteslabs/descarteslabs-python
 Author: Descartes Labs
 Author-email: hello@descarteslabs.com
 License: Apache 2.0
-Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v2.0.2.tar.gz
+Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v2.0.3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `descarteslabs-2.0.2/descarteslabs.egg-info/SOURCES.txt` & `descarteslabs-2.0.3/descarteslabs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,19 @@
 descarteslabs/core/client/services/service/service.py
 descarteslabs/core/client/services/service/tests/__init__.py
 descarteslabs/core/client/services/service/tests/test_service.py
 descarteslabs/core/common/__init__.py
 descarteslabs/core/common/client/__init__.py
 descarteslabs/core/common/client/attributes.py
 descarteslabs/core/common/client/document.py
+descarteslabs/core/common/client/search.py
+descarteslabs/core/common/client/sort.py
 descarteslabs/core/common/client/tests/__init__.py
 descarteslabs/core/common/client/tests/test_attributes.py
+descarteslabs/core/common/client/tests/test_search.py
 descarteslabs/core/common/collection/__init__.py
 descarteslabs/core/common/collection/collection.py
 descarteslabs/core/common/collection/tests/__init__.py
 descarteslabs/core/common/collection/tests/test_collection.py
 descarteslabs/core/common/display/__init__.py
 descarteslabs/core/common/display/_display.py
 descarteslabs/core/common/display/tests/__init__.py
```

### Comparing `descarteslabs-2.0.2/descarteslabs.egg-info/requires.txt` & `descarteslabs-2.0.3/descarteslabs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.2/setup.py` & `descarteslabs-2.0.3/setup.py`

 * *Files identical despite different names*

