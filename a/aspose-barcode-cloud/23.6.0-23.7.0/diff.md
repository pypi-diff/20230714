# Comparing `tmp/aspose-barcode-cloud-23.6.0.tar.gz` & `tmp/aspose-barcode-cloud-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aspose-barcode-cloud-23.6.0.tar", last modified: Thu Jun 29 05:49:35 2023, max compression
+gzip compressed data, was "aspose-barcode-cloud-23.7.0.tar", last modified: Fri Jul 14 14:17:37 2023, max compression
```

## Comparing `aspose-barcode-cloud-23.6.0.tar` & `aspose-barcode-cloud-23.7.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:49:35.487191 aspose-barcode-cloud-23.6.0/
--rw-r--r--   0 root         (0) root         (0)     1071 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15061 2023-06-29 05:49:35.487191 aspose-barcode-cloud-23.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12310 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:49:35.477191 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/
--rw-r--r--   0 root         (0) root         (0)     7155 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:49:35.477191 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api/
--rw-r--r--   0 root         (0) root         (0)      319 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99385 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api/barcode_api.py
--rw-r--r--   0 root         (0) root         (0)    24296 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api/file_api.py
--rw-r--r--   0 root         (0) root         (0)    22451 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api/folder_api.py
--rw-r--r--   0 root         (0) root         (0)    16119 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api/storage_api.py
--rw-r--r--   0 root         (0) root         (0)    26047 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api_client.py
--rw-r--r--   0 root         (0) root         (0)    10460 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:49:35.487191 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/
--rw-r--r--   0 root         (0) root         (0)     6699 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6521 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/api_error.py
--rw-r--r--   0 root         (0) root         (0)     4574 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/api_error_response.py
--rw-r--r--   0 root         (0) root         (0)     5429 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/australian_post_params.py
--rw-r--r--   0 root         (0) root         (0)     3371 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/auto_size_mode.py
--rw-r--r--   0 root         (0) root         (0)     3417 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/available_graphics_unit.py
--rw-r--r--   0 root         (0) root         (0)     6810 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/aztec_params.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/aztec_symbol_mode.py
--rw-r--r--   0 root         (0) root         (0)     6225 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/barcode_response.py
--rw-r--r--   0 root         (0) root         (0)     4135 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/barcode_response_list.py
--rw-r--r--   0 root         (0) root         (0)     3413 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/border_dash_style.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/caption_params.py
--rw-r--r--   0 root         (0) root         (0)     3371 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/checksum_validation.py
--rw-r--r--   0 root         (0) root         (0)     3361 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/codabar_checksum_mode.py
--rw-r--r--   0 root         (0) root         (0)     6349 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/codabar_params.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/codabar_symbol.py
--rw-r--r--   0 root         (0) root         (0)     5474 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/codablock_params.py
--rw-r--r--   0 root         (0) root         (0)     3399 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/code128_emulation.py
--rw-r--r--   0 root         (0) root         (0)     3457 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/code128_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     4240 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/code128_params.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/code16_k_params.py
--rw-r--r--   0 root         (0) root         (0)     3351 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/code_location.py
--rw-r--r--   0 root         (0) root         (0)     4238 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/coupon_params.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py
--rw-r--r--   0 root         (0) root         (0)     8008 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/data_bar_params.py
--rw-r--r--   0 root         (0) root         (0)     3469 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py
--rw-r--r--   0 root         (0) root         (0)     3527 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)    10136 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/data_matrix_params.py
--rw-r--r--   0 root         (0) root         (0)     5729 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/decode_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/disc_usage.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/dot_code_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     9394 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/dot_code_params.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/eci_encodings.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/enable_checksum.py
--rw-r--r--   0 root         (0) root         (0)     5409 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/encode_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)     5970 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/error.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/error_details.py
--rw-r--r--   0 root         (0) root         (0)     8827 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/file_version.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/file_versions.py
--rw-r--r--   0 root         (0) root         (0)     3995 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/files_list.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/files_upload_result.py
--rw-r--r--   0 root         (0) root         (0)     3317 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/font_mode.py
--rw-r--r--   0 root         (0) root         (0)     5207 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/font_params.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/font_style.py
--rw-r--r--   0 root         (0) root         (0)    57243 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/generator_params.py
--rw-r--r--   0 root         (0) root         (0)     5896 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/generator_params_list.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/han_xin_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     3365 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/han_xin_error_level.py
--rw-r--r--   0 root         (0) root         (0)     7412 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/han_xin_params.py
--rw-r--r--   0 root         (0) root         (0)     5667 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/han_xin_version.py
--rw-r--r--   0 root         (0) root         (0)     3407 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/itf14_border_type.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/itf_params.py
--rw-r--r--   0 root         (0) root         (0)     3367 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/macro_character.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/maxi_code_mode.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/maxi_code_params.py
--rw-r--r--   0 root         (0) root         (0)     4944 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/object_exist.py
--rw-r--r--   0 root         (0) root         (0)     5750 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/padding.py
--rw-r--r--   0 root         (0) root         (0)     5467 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/patch_code_params.py
--rw-r--r--   0 root         (0) root         (0)     3441 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/patch_format.py
--rw-r--r--   0 root         (0) root         (0)     3407 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py
--rw-r--r--   0 root         (0) root         (0)     3507 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/pdf417_error_level.py
--rw-r--r--   0 root         (0) root         (0)     3381 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py
--rw-r--r--   0 root         (0) root         (0)    24492 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/pdf417_params.py
--rw-r--r--   0 root         (0) root         (0)     4177 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/postal_params.py
--rw-r--r--   0 root         (0) root         (0)     3523 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/preset_type.py
--rw-r--r--   0 root         (0) root         (0)     3459 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/qr_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     3369 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/qr_encode_type.py
--rw-r--r--   0 root         (0) root         (0)     3381 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/qr_error_level.py
--rw-r--r--   0 root         (0) root         (0)    11027 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/qr_params.py
--rw-r--r--   0 root         (0) root         (0)     4531 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/qr_version.py
--rw-r--r--   0 root         (0) root         (0)    46322 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/reader_params.py
--rw-r--r--   0 root         (0) root         (0)     4540 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/region_point.py
--rw-r--r--   0 root         (0) root         (0)     5716 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/result_image_info.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/storage_exist.py
--rw-r--r--   0 root         (0) root         (0)     7017 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/storage_file.py
--rw-r--r--   0 root         (0) root         (0)     6065 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/structured_append.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/text_alignment.py
--rw-r--r--   0 root         (0) root         (0)    14400 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:49:35.477191 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15061 2023-06-29 05:49:35.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4281 2023-06-29 05:49:35.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 05:49:35.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-29 05:49:35.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-29 05:49:35.000000 aspose-barcode-cloud-23.6.0/aspose_barcode_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 05:49:35.487191 aspose-barcode-cloud-23.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5750 2023-06-29 05:48:31.000000 aspose-barcode-cloud-23.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:17:37.808158 aspose-barcode-cloud-23.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15073 2023-07-14 14:17:37.808158 aspose-barcode-cloud-23.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12322 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:17:37.798158 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/
+-rw-r--r--   0 root         (0) root         (0)     7155 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:17:37.798158 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99415 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api/barcode_api.py
+-rw-r--r--   0 root         (0) root         (0)    24326 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api/file_api.py
+-rw-r--r--   0 root         (0) root         (0)    22481 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api/folder_api.py
+-rw-r--r--   0 root         (0) root         (0)    16149 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api/storage_api.py
+-rw-r--r--   0 root         (0) root         (0)    26047 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    10460 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:17:37.808158 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/
+-rw-r--r--   0 root         (0) root         (0)     6699 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6551 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/api_error.py
+-rw-r--r--   0 root         (0) root         (0)     4604 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/api_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     5459 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/australian_post_params.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/auto_size_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3447 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/available_graphics_unit.py
+-rw-r--r--   0 root         (0) root         (0)     6840 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/aztec_params.py
+-rw-r--r--   0 root         (0) root         (0)     3423 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/aztec_symbol_mode.py
+-rw-r--r--   0 root         (0) root         (0)     6255 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/barcode_response.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/barcode_response_list.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/border_dash_style.py
+-rw-r--r--   0 root         (0) root         (0)     8345 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/caption_params.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/checksum_validation.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/codabar_checksum_mode.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/codabar_params.py
+-rw-r--r--   0 root         (0) root         (0)     3375 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/codabar_symbol.py
+-rw-r--r--   0 root         (0) root         (0)     5504 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/codablock_params.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/code128_emulation.py
+-rw-r--r--   0 root         (0) root         (0)     3487 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/code128_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4270 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/code128_params.py
+-rw-r--r--   0 root         (0) root         (0)     6543 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/code16_k_params.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     4268 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/coupon_params.py
+-rw-r--r--   0 root         (0) root         (0)     3479 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py
+-rw-r--r--   0 root         (0) root         (0)     8038 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/data_bar_params.py
+-rw-r--r--   0 root         (0) root         (0)     3499 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py
+-rw-r--r--   0 root         (0) root         (0)     3557 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)    10896 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/data_matrix_params.py
+-rw-r--r--   0 root         (0) root         (0)     5759 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/decode_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/disc_usage.py
+-rw-r--r--   0 root         (0) root         (0)     3423 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/dot_code_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     9424 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/dot_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/eci_encodings.py
+-rw-r--r--   0 root         (0) root         (0)     3385 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/enable_checksum.py
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/encode_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)     6000 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     4767 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/error_details.py
+-rw-r--r--   0 root         (0) root         (0)     8857 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/file_version.py
+-rw-r--r--   0 root         (0) root         (0)     4001 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/file_versions.py
+-rw-r--r--   0 root         (0) root         (0)     4025 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/files_list.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/files_upload_result.py
+-rw-r--r--   0 root         (0) root         (0)     3347 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/font_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/font_params.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/font_style.py
+-rw-r--r--   0 root         (0) root         (0)    57609 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/generator_params.py
+-rw-r--r--   0 root         (0) root         (0)     5926 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/generator_params_list.py
+-rw-r--r--   0 root         (0) root         (0)     3461 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/han_xin_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/han_xin_error_level.py
+-rw-r--r--   0 root         (0) root         (0)     7442 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/han_xin_params.py
+-rw-r--r--   0 root         (0) root         (0)     5697 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/han_xin_version.py
+-rw-r--r--   0 root         (0) root         (0)     3437 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/itf14_border_type.py
+-rw-r--r--   0 root         (0) root         (0)     6218 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/itf_params.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/macro_character.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3423 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/maxi_code_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5715 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/maxi_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     4974 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/object_exist.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/padding.py
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/patch_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/patch_format.py
+-rw-r--r--   0 root         (0) root         (0)     3437 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/pdf417_error_level.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py
+-rw-r--r--   0 root         (0) root         (0)    24522 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/pdf417_params.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/postal_params.py
+-rw-r--r--   0 root         (0) root         (0)     3553 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/preset_type.py
+-rw-r--r--   0 root         (0) root         (0)     3489 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/qr_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/qr_encode_type.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/qr_error_level.py
+-rw-r--r--   0 root         (0) root         (0)    11057 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/qr_params.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/qr_version.py
+-rw-r--r--   0 root         (0) root         (0)    46352 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/reader_params.py
+-rw-r--r--   0 root         (0) root         (0)     4570 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/region_point.py
+-rw-r--r--   0 root         (0) root         (0)     5746 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/result_image_info.py
+-rw-r--r--   0 root         (0) root         (0)     4075 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/storage_exist.py
+-rw-r--r--   0 root         (0) root         (0)     7047 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/storage_file.py
+-rw-r--r--   0 root         (0) root         (0)     6095 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/structured_append.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/text_alignment.py
+-rw-r--r--   0 root         (0) root         (0)    14400 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:17:37.798158 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15073 2023-07-14 14:17:37.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4281 2023-07-14 14:17:37.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 14:17:37.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-14 14:17:37.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-14 14:17:37.000000 aspose-barcode-cloud-23.7.0/aspose_barcode_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 14:17:37.808158 aspose-barcode-cloud-23.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5750 2023-07-14 14:16:24.000000 aspose-barcode-cloud-23.7.0/setup.py
```

### Comparing `aspose-barcode-cloud-23.6.0/LICENSE` & `aspose-barcode-cloud-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.6.0/PKG-INFO` & `aspose-barcode-cloud-23.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-barcode-cloud
-Version: 23.6.0
+Version: 23.7.0
 Summary: Aspose.Barcode Cloud API Reference
 Home-page: https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Author: Aspose Barcode Cloud
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Project-URL: Website, https://www.aspose.cloud
 Project-URL: Product Home, https://products.aspose.cloud/barcode/
@@ -30,19 +30,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Aspose.BarCode Cloud SDK for Python
 
 [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
-[![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
+[![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
 
 - API version: 3.0
-- Package version: 23.6.0
+- Package version: 23.7.0
 
 ## Demo applications
 
 [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
 :---: | :---: | :---:
 [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
 [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
```

### Comparing `aspose-barcode-cloud-23.6.0/README.md` & `aspose-barcode-cloud-23.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Aspose.BarCode Cloud SDK for Python
 
 [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
-[![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
+[![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
 
 - API version: 3.0
-- Package version: 23.6.0
+- Package version: 23.7.0
 
 ## Demo applications
 
 [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
 :---: | :---: | :---:
 [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
 [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/__init__.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api/barcode_api.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api/barcode_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 from __future__ import absolute_import, division
 
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from aspose_barcode_cloud.api_client import ApiClient
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api/file_api.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api/file_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 from __future__ import absolute_import, division
 
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from aspose_barcode_cloud.api_client import ApiClient
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api/folder_api.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api/folder_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 from __future__ import absolute_import, division
 
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from aspose_barcode_cloud.api_client import ApiClient
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api/storage_api.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api/storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 from __future__ import absolute_import, division
 
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from aspose_barcode_cloud.api_client import ApiClient
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/api_client.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,21 +86,21 @@
         self.configuration = configuration
 
         # Use the pool property to lazily initialize the ThreadPool.
         self._pool = None
         self.rest_client = RESTClientObject(configuration)
         self.default_headers = {
             "x-aspose-client": "python sdk",
-            "x-aspose-client-version": "23.6.0",
+            "x-aspose-client-version": "23.7.0",
         }
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "Aspose-Barcode-SDK/23.6.0/python"
+        self.user_agent = "Aspose-Barcode-SDK/23.7.0/python"
 
     def __del__(self):
         self.rest_client.close()
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/configuration.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: 3.0\n"
-            "SDK Package Version: 23.6.0".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 23.7.0".format(env=sys.platform, pyversion=sys.version)
         )
 
     @staticmethod
     def fetch_token(client_id, client_secret, token_url):
         with contextlib.closing(
             RESTClientObject(Configuration(client_id=client_id, client_secret=client_secret, token_url=token_url))
         ) as client:
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/__init__.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/api_error.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/api_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class ApiError(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/api_error_response.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/api_error_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class ApiErrorResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/australian_post_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/australian_post_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class AustralianPostParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/auto_size_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/auto_size_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class AutoSizeMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/available_graphics_unit.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/available_graphics_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class AvailableGraphicsUnit(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/aztec_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/aztec_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class AztecParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/aztec_symbol_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/aztec_symbol_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class AztecSymbolMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/barcode_response.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/barcode_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class BarcodeResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/barcode_response_list.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/barcode_response_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class BarcodeResponseList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/border_dash_style.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/enable_checksum.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,46 +23,45 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
-class BorderDashStyle(object):
+class EnableChecksum(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    SOLID = "Solid"
-    DASH = "Dash"
-    DOT = "Dot"
-    DASHDOT = "DashDot"
-    DASHDOTDOT = "DashDotDot"
+    DEFAULT = "Default"
+    YES = "Yes"
+    NO = "No"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {}
 
     attribute_map = {}
 
     def __init__(self):  # noqa: E501
-        """BorderDashStyle - a model defined in Swagger"""  # noqa: E501
+        """EnableChecksum - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -76,15 +75,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(BorderDashStyle, dict):
+        if issubclass(EnableChecksum, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -92,15 +91,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BorderDashStyle):
+        if not isinstance(other, EnableChecksum):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/caption_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/caption_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class CaptionParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/checksum_validation.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/checksum_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class ChecksumValidation(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/codabar_checksum_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/codabar_checksum_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class CodabarChecksumMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/codabar_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/codabar_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class CodabarParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/codabar_symbol.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/codabar_symbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class CodabarSymbol(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/codablock_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/codablock_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class CodablockParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/code128_emulation.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/code128_emulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class Code128Emulation(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/code128_encode_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/code128_encode_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class Code128EncodeMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/code128_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/code128_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class Code128Params(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/code16_k_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/code16_k_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class Code16KParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/code_location.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/code_location.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class CodeLocation(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/coupon_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/coupon_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class CouponParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class CustomerInformationInterpretingType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/data_bar_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/data_bar_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class DataBarParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class DataMatrixEccType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class DataMatrixEncodeMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/data_matrix_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/data_matrix_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class DataMatrixParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
@@ -146,30 +147,34 @@
 
         self._text_encoding = text_encoding
 
     @property
     def columns(self):
         """Gets the columns of this DataMatrixParams.  # noqa: E501
 
-        Columns count.  # noqa: E501
+        DEPRECATED: Will be replaced with 'DataMatrix.Version' in the next release  Columns count.  # noqa: E501
 
         :return: The columns of this DataMatrixParams.  # noqa: E501
         :rtype: int
         """
         return self._columns
 
     @columns.setter
     def columns(self, columns):
         """Sets the columns of this DataMatrixParams.
 
-        Columns count.  # noqa: E501
+        DEPRECATED: Will be replaced with 'DataMatrix.Version' in the next release  Columns count.  # noqa: E501
 
         :param columns: The columns of this DataMatrixParams.  # noqa: E501
         :type: int
         """
+        warnings.warn(
+            "Property 'columns' is deprecated. Will be replaced with 'DataMatrix.Version' in the next release  Columns count.",  # noqa: E501
+            category=DeprecationWarning,
+        )
 
         self._columns = columns
 
     @property
     def data_matrix_ecc(self):
         """Gets the data_matrix_ecc of this DataMatrixParams.  # noqa: E501
 
@@ -215,30 +220,34 @@
 
         self._data_matrix_encode_mode = data_matrix_encode_mode
 
     @property
     def rows(self):
         """Gets the rows of this DataMatrixParams.  # noqa: E501
 
-        Rows count.  # noqa: E501
+        DEPRECATED: Will be replaced with 'DataMatrix.Version' in the next release  Rows count.  # noqa: E501
 
         :return: The rows of this DataMatrixParams.  # noqa: E501
         :rtype: int
         """
         return self._rows
 
     @rows.setter
     def rows(self, rows):
         """Sets the rows of this DataMatrixParams.
 
-        Rows count.  # noqa: E501
+        DEPRECATED: Will be replaced with 'DataMatrix.Version' in the next release  Rows count.  # noqa: E501
 
         :param rows: The rows of this DataMatrixParams.  # noqa: E501
         :type: int
         """
+        warnings.warn(
+            "Property 'rows' is deprecated. Will be replaced with 'DataMatrix.Version' in the next release  Rows count.",  # noqa: E501
+            category=DeprecationWarning,
+        )
 
         self._rows = rows
 
     @property
     def macro_characters(self):
         """Gets the macro_characters of this DataMatrixParams.  # noqa: E501
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/decode_barcode_type.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/decode_barcode_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class DecodeBarcodeType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/disc_usage.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/disc_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class DiscUsage(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/dot_code_encode_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/dot_code_encode_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class DotCodeEncodeMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/dot_code_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/dot_code_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class DotCodeParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/eci_encodings.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/eci_encodings.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class ECIEncodings(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/enable_checksum.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/text_alignment.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,44 +23,45 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
-class EnableChecksum(object):
+class TextAlignment(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    DEFAULT = "Default"
-    YES = "Yes"
-    NO = "No"
+    LEFT = "Left"
+    CENTER = "Center"
+    RIGHT = "Right"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {}
 
     attribute_map = {}
 
     def __init__(self):  # noqa: E501
-        """EnableChecksum - a model defined in Swagger"""  # noqa: E501
+        """TextAlignment - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -74,15 +75,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(EnableChecksum, dict):
+        if issubclass(TextAlignment, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -90,15 +91,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, EnableChecksum):
+        if not isinstance(other, TextAlignment):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/encode_barcode_type.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/encode_barcode_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class EncodeBarcodeType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/error.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class Error(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/error_details.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/error_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class ErrorDetails(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/file_version.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/file_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class FileVersion(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/file_versions.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/file_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class FileVersions(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/files_list.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/files_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class FilesList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/files_upload_result.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/files_upload_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class FilesUploadResult(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/font_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/font_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class FontMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/font_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/font_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class FontParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/font_style.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/font_style.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class FontStyle(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/generator_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/generator_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class GeneratorParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
@@ -642,14 +643,18 @@
         """Sets the resolution_x of this GeneratorParams.
 
         DEPRECATED: Use 'Resolution' instead.  # noqa: E501
 
         :param resolution_x: The resolution_x of this GeneratorParams.  # noqa: E501
         :type: float
         """
+        warnings.warn(
+            "Property 'resolution_x' is deprecated. Use 'Resolution' instead.",  # noqa: E501
+            category=DeprecationWarning,
+        )
 
         self._resolution_x = resolution_x
 
     @property
     def resolution_y(self):
         """Gets the resolution_y of this GeneratorParams.  # noqa: E501
 
@@ -665,14 +670,18 @@
         """Sets the resolution_y of this GeneratorParams.
 
         DEPRECATED: Use 'Resolution' instead.  # noqa: E501
 
         :param resolution_y: The resolution_y of this GeneratorParams.  # noqa: E501
         :type: float
         """
+        warnings.warn(
+            "Property 'resolution_y' is deprecated. Use 'Resolution' instead.",  # noqa: E501
+            category=DeprecationWarning,
+        )
 
         self._resolution_y = resolution_y
 
     @property
     def dimension_x(self):
         """Gets the dimension_x of this GeneratorParams.  # noqa: E501
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/generator_params_list.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/generator_params_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class GeneratorParamsList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/han_xin_encode_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/han_xin_encode_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class HanXinEncodeMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/han_xin_error_level.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/han_xin_error_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class HanXinErrorLevel(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/han_xin_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/han_xin_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class HanXinParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/han_xin_version.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/han_xin_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class HanXinVersion(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/itf14_border_type.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/itf14_border_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class ITF14BorderType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/itf_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/itf_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class ITFParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/macro_character.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/macro_character.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class MacroCharacter(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class MaxiCodeEncodeMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/maxi_code_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/maxi_code_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class MaxiCodeMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/maxi_code_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/maxi_code_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class MaxiCodeParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/object_exist.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/object_exist.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class ObjectExist(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/padding.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/padding.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class Padding(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/patch_code_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/patch_code_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class PatchCodeParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/patch_format.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/patch_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class PatchFormat(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class Pdf417CompactionMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/pdf417_error_level.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/pdf417_error_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class Pdf417ErrorLevel(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class Pdf417MacroTerminator(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/pdf417_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/pdf417_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class Pdf417Params(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/postal_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/postal_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class PostalParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/preset_type.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/preset_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class PresetType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/qr_encode_mode.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/qr_encode_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class QREncodeMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/qr_encode_type.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/qr_encode_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class QREncodeType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/qr_error_level.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/qr_error_level.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class QRErrorLevel(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/qr_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/qr_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class QrParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/qr_version.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/qr_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class QRVersion(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/reader_params.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/reader_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class ReaderParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/region_point.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/region_point.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class RegionPoint(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/result_image_info.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/result_image_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class ResultImageInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/storage_exist.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/storage_exist.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class StorageExist(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/storage_file.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/storage_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class StorageFile(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/structured_append.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/structured_append.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
 class StructuredAppend(object):
     """NOTE: This class is auto generated by the swagger code generator program.
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/models/text_alignment.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/models/border_dash_style.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,44 +23,47 @@
  SOFTWARE.
 
 """
 
 
 import pprint
 import re  # noqa: F401
+import warnings  # noqa: F401
 
 import six
 
 
-class TextAlignment(object):
+class BorderDashStyle(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    LEFT = "Left"
-    CENTER = "Center"
-    RIGHT = "Right"
+    SOLID = "Solid"
+    DASH = "Dash"
+    DOT = "Dot"
+    DASHDOT = "DashDot"
+    DASHDOTDOT = "DashDotDot"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {}
 
     attribute_map = {}
 
     def __init__(self):  # noqa: E501
-        """TextAlignment - a model defined in Swagger"""  # noqa: E501
+        """BorderDashStyle - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -74,15 +77,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(TextAlignment, dict):
+        if issubclass(BorderDashStyle, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -90,15 +93,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TextAlignment):
+        if not isinstance(other, BorderDashStyle):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud/rest.py` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud/rest.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud.egg-info/PKG-INFO` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-barcode-cloud
-Version: 23.6.0
+Version: 23.7.0
 Summary: Aspose.Barcode Cloud API Reference
 Home-page: https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Author: Aspose Barcode Cloud
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Project-URL: Website, https://www.aspose.cloud
 Project-URL: Product Home, https://products.aspose.cloud/barcode/
@@ -30,19 +30,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Aspose.BarCode Cloud SDK for Python
 
 [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
-[![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
+[![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
 
 - API version: 3.0
-- Package version: 23.6.0
+- Package version: 23.7.0
 
 ## Demo applications
 
 [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
 :---: | :---: | :---:
 [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
 [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
```

### Comparing `aspose-barcode-cloud-23.6.0/aspose_barcode_cloud.egg-info/SOURCES.txt` & `aspose-barcode-cloud-23.7.0/aspose_barcode_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.6.0/setup.py` & `aspose-barcode-cloud-23.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 """
 
 import os
 
 from setuptools import setup, find_packages
 
 NAME = "aspose-barcode-cloud"
-VERSION = "23.6.0"
+VERSION = "23.7.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

