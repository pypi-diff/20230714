# Comparing `tmp/spdx-tools-0.8.0rc1.tar.gz` & `tmp/spdx-tools-0.8.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/tools-python/tools-python/dist/.tmp-fnqkgbkt/spdx-tools-0.8.0rc1.tar", last modified: Fri Jun 30 12:07:16 2023, max compression
+gzip compressed data, was "/home/runner/work/tools-python/tools-python/dist/.tmp-clg_6a6y/spdx-tools-0.8.0rc2.tar", last modified: Fri Jul 14 06:55:11 2023, max compression
```

## Comparing `spdx-tools-0.8.0rc1.tar` & `spdx-tools-0.8.0rc2.tar`

### file list

```diff
@@ -1,562 +1,564 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/.github/workflows/check_codestyle.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/.github/workflows/install_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/.github/workflows/integration_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/.github/workflows/prepare_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/appveyor.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   147064 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/assets/SPDXJSONExample-v2.3.spdx.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/examples/spdx2_convert_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/examples/spdx2_convert_to_spdx3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/examples/spdx2_document_from_scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/examples/spdx2_generate_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/examples/spdx2_parse_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/common/typing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/common/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/common/typing/constructor_type_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/common/typing/dataclass_with_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/common/typing/type_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/casing_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/clitools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/clitools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/clitools/pyspdxtools.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/datetime_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/document_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/graph_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/annotation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/annotation_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/checksum_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/checksum_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/creation_info_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/creation_info_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/document_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/document_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/external_document_ref_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/external_document_ref_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/external_package_ref_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/external_package_ref_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/file_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/file_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/json_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/optional_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/package_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/package_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/package_verification_code_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/package_verification_code_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/relationship_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/relationship_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/snippet_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/snippet_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/external_document_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/extracted_licensing_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/relationship_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/snippet.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/spdx_no_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/spdx_none.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/actor_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/json/json_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/annotation_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/checksum_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/creation_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/dict_parsing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/extracted_licensing_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/json_like_dict_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/license_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/package_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/relationship_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/snippet_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/parse_anything.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/parsing_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/annotation_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/checksum_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/creation_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/extracted_licensing_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/graph_parsing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/license_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/package_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/rdf_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/relationship_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/snippet_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/tagvalue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/tagvalue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/tagvalue/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/tagvalue/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29564 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/tagvalue/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/tagvalue/tagvalue_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/xml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/xml/xml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/yaml/yaml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/rdfschema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/rdfschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/rdfschema/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/spdx_element_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/actor_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/annotation_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/checksum_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/creation_info_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/document_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/external_document_ref_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/external_package_ref_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/extracted_licensing_info_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/file_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/license_expression_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/package_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/package_verification_code_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/relationship_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/snippet_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/spdx_id_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/uri_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/validation_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/json/json_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/annotation_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/checksum_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/creation_info_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/external_document_ref_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/extracted_licensing_info_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/license_expression_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/package_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/rdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/relationship_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/snippet_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/writer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/annotation_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/checksum_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/creation_info_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/extracted_licensing_info_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/package_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/relationship_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/snippet_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/write_anything.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/write_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/xml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/xml/xml_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/yaml/yaml_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/bump_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/creation_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/external_document_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/license_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/snippet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/spdx_document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/clitools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/clitools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/clitools/pyspdxtools3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/ai/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/ai/ai_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/bom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/build/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/build/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/creation_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/external_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/external_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/external_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/integrity_method.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/any_license_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/conjunctive_license_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/custom_license.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/custom_license_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/disjunctive_license_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/license.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/license_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/license_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/listed_license.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/listed_license_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/no_assertion_license.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/none_license.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/or_later_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/with_addition_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/lifecycle_scoped_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/namespace_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/person.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/positive_integer_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/profile_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/relationship.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/cvss_v2_vuln_assessment_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/cvss_v3_vuln_assessment_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/epss_vuln_assessment_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/exploit_catalog_vuln_assessment_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/ssvc_vuln_assessment_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vex_affected_vuln_assessment_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vex_fixed_vuln_assessment_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vex_not_affected_vuln_assessment_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vex_under_investigation_vuln_assessment_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vex_vuln_assessment_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vuln_assessment_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vulnerability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/sbom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/snippet.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/software_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/software_dependency_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/software_purpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/spdx_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/spdx_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/validation/json_ld/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/validation/json_ld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/validation/json_ld/shacl_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/agent_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/ai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/ai/ai_package_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/annotation_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/artifact_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/bom_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/build/build_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/bundle_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/creation_info_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/dataset/dataset_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/element_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/external_identifier_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/external_map_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/external_reference_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/hash_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/integrity_method_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/lifecycle_scoped_relationship_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/namespace_map_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/payload_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/relationship_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/software/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/software/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/software/package_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/software/sbom_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/software/snippet_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/software/software_dependency_relationship_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/spdx_collection_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/spdx_document_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/tool_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/
--rw-r--r--   0 runner    (1001) docker     (123)   196691 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/SPDX_OWL.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21597 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/context.json
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/json_ld_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/json_ld_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)   148062 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/model.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/owl_to_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/src/spdx_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/stdeb.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/data/
--rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/SPDXJSONExample-v2.2.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/SPDXLite.spdx
--rw-r--r--   0 runner    (1001) docker     (123)   338588 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/SPDXRdfExample-v2.2.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)   342594 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/SPDXTagExample-v2.2.spdx
--rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (123)    24020 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/SPDXXMLExample-v2.2.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (123)    24809 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (123)    19895 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/SPDXYAMLExample-v2.2.spdx.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/SPDXYAMLExample-v2.3.spdx.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    25618 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/data/circleConversionTestInitialDocument.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/examples/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/examples/test_spdx2_document_from_scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_annotation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_checksum_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_creation_info_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_document_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_external_document_ref_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_external_package_ref_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_extracted_licensing_info_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_file_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_package_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_package_verification_code_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_relationship_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_snippet_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_creation_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_external_document_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_external_package_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_extracted_licensing_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_package_verification_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_snippet.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/model/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/all_formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/all_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/all_formats/test_parse_from_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_annotation_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_checksum_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_creation_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_dict_parsing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_extracted_licensing_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_license_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_package_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_relationship_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_snippet_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/data/
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/data/file_to_test_rdf_parser.rdf.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/data/invalid_documents/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/data/invalid_documents/file_without_spdx_ids.xml
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info_with_snippet.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_annotation_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_checksum_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_creation_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_extracted_licensing_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_graph_parsing_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_license_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_package_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_relationship_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_snippet_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_annotation_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_creation_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_extracted_licensing_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_package_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_relationship_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_snippet_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_tag_value_lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_tag_value_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/test_actor_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/test_casing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/test_datetime_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/test_document_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/test_graph_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_actor_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_annotation_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_checksum_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_creation_info_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_document_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_external_document_ref_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_external_package_ref_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_extracted_licensing_info_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_file_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_license_expression_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_package_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_package_verification_code_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_relationship_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_snippet_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_spdx_id_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/validation/test_uri_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/json/expected_results/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/json/expected_results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/json/expected_results/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/json/test_json_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_annotation_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_checksum_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_creation_info_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_external_document_ref_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_extracted_licensing_info_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_license_expression_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_package_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_rdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_relationship_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_snippet_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_writer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/expected_results/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/expected_results/expected_tag_value.spdx
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_annotation_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_checksum_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_creation_info_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_extracted_licensing_info_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_package_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_relationship_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_snippet_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_tagvalue_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_tagvalue_writer_helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/test_actor_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/test_bump_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/test_checksum_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/test_external_document_ref_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/test_external_element_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/test_file_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/test_license_expression_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/test_package_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/test_relationship_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/test_snippet_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/bump/test_spdx_document_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)    19138 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/licensing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/licensing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/licensing/test_conjunctive_license_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/licensing/test_disjunctive_license_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/licensing/test_or_later_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/licensing/test_with_addition_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/model_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/test_abstract_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/test_creation_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/test_element_and_licensing_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/test_external_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/test_external_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/test_external_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/model/test_namespace_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx3/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx3/validation/json_ld/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/validation/json_ld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/validation/json_ld/test_shacl_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx3/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/writer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:07:16.000000 spdx-tools-0.8.0rc1/tests/spdx3/writer/json_ld/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/writer/json_ld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-30 12:06:50.000000 spdx-tools-0.8.0rc1/tests/spdx3/writer/json_ld/test_json_ld_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/.github/workflows/check_codestyle.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/.github/workflows/install_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/.github/workflows/integration_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/.github/workflows/prepare_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/appveyor.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   147064 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/assets/SPDXJSONExample-v2.3.spdx.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/examples/spdx2_convert_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/examples/spdx2_convert_to_spdx3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/examples/spdx2_document_from_scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/examples/spdx2_generate_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/examples/spdx2_parse_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/common/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/common/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/common/typing/constructor_type_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/common/typing/dataclass_with_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/common/typing/type_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/casing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/clitools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/clitools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/clitools/pyspdxtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/datetime_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/document_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/graph_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/annotation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/annotation_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/checksum_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/checksum_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/creation_info_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/creation_info_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/document_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/document_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/external_document_ref_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/external_document_ref_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/external_package_ref_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/external_package_ref_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/file_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/file_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/json_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/optional_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/package_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/package_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/package_verification_code_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/package_verification_code_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/relationship_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/relationship_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/snippet_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/snippet_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/external_document_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/extracted_licensing_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/relationship_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/snippet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/spdx_no_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/spdx_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/actor_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/json/json_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/annotation_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/checksum_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/creation_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/dict_parsing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/extracted_licensing_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/json_like_dict_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/license_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/package_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/relationship_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/snippet_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/parse_anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/parsing_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/annotation_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/checksum_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/creation_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/extracted_licensing_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/graph_parsing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/license_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/package_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/rdf_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/relationship_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/snippet_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/tagvalue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/tagvalue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/tagvalue/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/tagvalue/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29564 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/tagvalue/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/tagvalue/tagvalue_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/xml/xml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/yaml/yaml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/rdfschema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/rdfschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/rdfschema/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/spdx_element_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/actor_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/annotation_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/checksum_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/creation_info_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/document_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/external_document_ref_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/external_package_ref_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/extracted_licensing_info_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/file_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/license_expression_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/package_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/package_verification_code_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/relationship_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/snippet_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/spdx_id_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/uri_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/validation_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/json/json_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/annotation_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/checksum_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/creation_info_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/external_document_ref_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/extracted_licensing_info_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/license_expression_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/package_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/rdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/relationship_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/snippet_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/writer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/annotation_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/checksum_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/creation_info_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/extracted_licensing_info_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/package_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/relationship_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/snippet_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/write_anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/write_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/xml/xml_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/yaml/yaml_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/bump_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/creation_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/external_document_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/license_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/snippet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/spdx_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/clitools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/clitools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/clitools/pyspdxtools3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/ai/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/ai/ai_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/bom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/build/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/creation_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/external_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/external_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/external_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/integrity_method.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/any_license_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/conjunctive_license_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/custom_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/custom_license_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/disjunctive_license_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/license_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/license_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/listed_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/listed_license_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/no_assertion_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/none_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/or_later_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/with_addition_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/lifecycle_scoped_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/namespace_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/positive_integer_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/profile_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/relationship.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/cvss_v2_vuln_assessment_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/cvss_v3_vuln_assessment_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/epss_vuln_assessment_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/exploit_catalog_vuln_assessment_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/ssvc_vuln_assessment_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vex_affected_vuln_assessment_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vex_fixed_vuln_assessment_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vex_not_affected_vuln_assessment_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vex_under_investigation_vuln_assessment_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vex_vuln_assessment_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vuln_assessment_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vulnerability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/sbom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/snippet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/software_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/software_dependency_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/software_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/spdx_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/spdx_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/validation/json_ld/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/validation/json_ld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/validation/json_ld/shacl_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/agent_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/ai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/ai/ai_package_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/annotation_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/artifact_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/bom_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/build/build_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/bundle_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/creation_info_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/dataset/dataset_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/element_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/external_identifier_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/external_map_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/external_reference_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/hash_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/integrity_method_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/lifecycle_scoped_relationship_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/namespace_map_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/payload_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/relationship_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/software/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/software/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/software/package_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/software/sbom_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/software/snippet_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/software/software_dependency_relationship_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/spdx_collection_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/spdx_document_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/tool_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/
+-rw-r--r--   0 runner    (1001) docker     (123)   196691 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/SPDX_OWL.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21597 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/context.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/json_ld_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/json_ld_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148062 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/model.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/owl_to_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/src/spdx_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/stdeb.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/SPDXJSONExample-v2.2.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/SPDXLite.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)   338588 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/SPDXRdfExample-v2.2.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   342594 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/SPDXTagExample-v2.2.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)    24020 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/SPDXXMLExample-v2.2.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    24809 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    19895 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/SPDXYAMLExample-v2.2.spdx.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/SPDXYAMLExample-v2.3.spdx.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    25618 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/data/circleConversionTestInitialDocument.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/examples/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/examples/test_spdx2_document_from_scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_annotation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_checksum_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_creation_info_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_document_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_external_document_ref_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_external_package_ref_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_extracted_licensing_info_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_file_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_package_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_package_verification_code_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_relationship_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_snippet_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_creation_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_external_document_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_external_package_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_extracted_licensing_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_package_verification_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_snippet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/model/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/all_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/all_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/all_formats/test_parse_from_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_annotation_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_checksum_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_creation_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_dict_parsing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_extracted_licensing_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_license_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_package_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_relationship_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_snippet_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/data/file_to_test_rdf_parser.rdf.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/data/invalid_documents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/data/invalid_documents/file_without_spdx_ids.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info_with_snippet.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_annotation_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_checksum_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_creation_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_extracted_licensing_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_graph_parsing_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_license_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_package_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_relationship_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_snippet_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_annotation_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_creation_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_extracted_licensing_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_package_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_relationship_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_snippet_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_tag_value_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_tag_value_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/test_actor_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/test_casing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/test_checksum_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/test_datetime_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/test_document_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/test_graph_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_actor_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_annotation_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_checksum_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_creation_info_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_document_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_external_document_ref_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_external_package_ref_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_extracted_licensing_info_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_file_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_license_expression_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_package_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_package_verification_code_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_relationship_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_snippet_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_spdx_id_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/validation/test_uri_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/json/expected_results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/json/expected_results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/json/expected_results/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/json/test_json_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_annotation_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_checksum_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_creation_info_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_external_document_ref_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_extracted_licensing_info_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_license_expression_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_package_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_rdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_relationship_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_snippet_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_writer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/expected_results/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/expected_results/expected_tag_value.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_annotation_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_checksum_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_creation_info_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_extracted_licensing_info_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_package_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_relationship_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_snippet_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_tagvalue_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_tagvalue_writer_helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/test_actor_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/test_bump_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/test_checksum_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/test_external_document_ref_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/test_external_element_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/test_file_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/test_license_expression_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/test_package_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/test_relationship_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/test_snippet_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/bump/test_spdx_document_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19154 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/licensing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/licensing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/licensing/test_conjunctive_license_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/licensing/test_disjunctive_license_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/licensing/test_or_later_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/licensing/test_with_addition_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/model_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/test_abstract_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/test_creation_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/test_element_and_licensing_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/test_external_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/test_external_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/test_external_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/model/test_namespace_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx3/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx3/validation/json_ld/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/validation/json_ld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/validation/json_ld/test_shacl_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx3/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/writer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:55:11.000000 spdx-tools-0.8.0rc2/tests/spdx3/writer/json_ld/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/writer/json_ld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-14 06:54:40.000000 spdx-tools-0.8.0rc2/tests/spdx3/writer/json_ld/test_json_ld_writer.py
```

### Comparing `spdx-tools-0.8.0rc1/.github/workflows/check_codestyle.yml` & `spdx-tools-0.8.0rc2/.github/workflows/check_codestyle.yml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/.github/workflows/install_and_test.yml` & `spdx-tools-0.8.0rc2/.github/workflows/install_and_test.yml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/.github/workflows/integration_test.yml` & `spdx-tools-0.8.0rc2/.github/workflows/integration_test.yml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/.github/workflows/prepare_release.yml` & `spdx-tools-0.8.0rc2/.github/workflows/prepare_release.yml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/CHANGELOG.md` & `spdx-tools-0.8.0rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/CONTRIBUTING.md` & `spdx-tools-0.8.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/LICENSE` & `spdx-tools-0.8.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/PKG-INFO` & `spdx-tools-0.8.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spdx-tools
-Version: 0.8.0rc1
+Version: 0.8.0rc2
 Summary: SPDX parser and tools.
 Author-email: "Ahmed H. Ismail" <ahm3d.hisham@gmail.com>
 Maintainer: SPDX group at the Linux Foundation and others
 Maintainer-email: Philippe Ombredanne <pombredanne@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/spdx/tools-python
 Classifier: Intended Audience :: Developers
@@ -50,14 +50,15 @@
 # Information
 
 This library implements SPDX parsers, convertors, validators and handlers in Python.
 
 - Home: https://github.com/spdx/tools-python
 - Issues: https://github.com/spdx/tools-python/issues
 - PyPI: https://pypi.python.org/pypi/spdx-tools
+- Browse the API: https://spdx.github.io/tools-python
 
 
 # License
 
 [Apache-2.0](LICENSE)
 
 # Features
```

### Comparing `spdx-tools-0.8.0rc1/README.md` & `spdx-tools-0.8.0rc2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # Information
 
 This library implements SPDX parsers, convertors, validators and handlers in Python.
 
 - Home: https://github.com/spdx/tools-python
 - Issues: https://github.com/spdx/tools-python/issues
 - PyPI: https://pypi.python.org/pypi/spdx-tools
+- Browse the API: https://spdx.github.io/tools-python
 
 
 # License
 
 [Apache-2.0](LICENSE)
 
 # Features
```

### Comparing `spdx-tools-0.8.0rc1/appveyor.yml` & `spdx-tools-0.8.0rc2/appveyor.yml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/assets/SPDXJSONExample-v2.3.spdx.png` & `spdx-tools-0.8.0rc2/assets/SPDXJSONExample-v2.3.spdx.png`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/examples/spdx2_convert_format.py` & `spdx-tools-0.8.0rc2/examples/spdx2_convert_format.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/examples/spdx2_convert_to_spdx3.py` & `spdx-tools-0.8.0rc2/examples/spdx2_convert_to_spdx3.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/examples/spdx2_document_from_scratch.py` & `spdx-tools-0.8.0rc2/examples/spdx2_document_from_scratch.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/examples/spdx2_generate_graph.py` & `spdx-tools-0.8.0rc2/examples/spdx2_generate_graph.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/examples/spdx2_parse_file.py` & `spdx-tools-0.8.0rc2/examples/spdx2_parse_file.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/pyproject.toml` & `spdx-tools-0.8.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/common/typing/constructor_type_errors.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/common/typing/constructor_type_errors.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/common/typing/dataclass_with_properties.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/common/typing/dataclass_with_properties.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/common/typing/type_checks.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/common/typing/type_checks.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/clitools/pyspdxtools.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/clitools/pyspdxtools.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/datetime_conversions.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/datetime_conversions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/document_utils.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/document_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/formats.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/formats.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/graph_generation.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/graph_generation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/annotation_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/annotation_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/checksum_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/checksum_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/creation_info_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/creation_info_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/document_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/document_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/document_properties.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/document_properties.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/external_document_ref_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/external_document_ref_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/external_package_ref_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/external_package_ref_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/file_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/file_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/file_properties.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/file_properties.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/package_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/package_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/package_properties.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/package_properties.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/package_verification_code_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/package_verification_code_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/relationship_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/relationship_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/jsonschema/snippet_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/jsonschema/snippet_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/__init__.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/__init__.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/actor.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/actor.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/annotation.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/annotation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/checksum.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/checksum.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/document.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/document.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/external_document_ref.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/external_document_ref.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/extracted_licensing_info.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/extracted_licensing_info.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/file.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/file.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/package.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/package.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/relationship_filters.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/relationship_filters.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/snippet.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/snippet.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/model/version.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/model/version.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/actor_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/actor_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 # SPDX-FileCopyrightText: 2022 spdx contributors
 #
 # SPDX-License-Identifier: Apache-2.0
 import re
 
-from beartype.typing import Match, Optional, Pattern
+from beartype.typing import Match, Pattern
 
 from spdx_tools.spdx.model import Actor, ActorType
 from spdx_tools.spdx.parser.error import SPDXParsingError
 from spdx_tools.spdx.parser.parsing_functions import construct_or_raise_parsing_error
 
 
 class ActorParser:
     @staticmethod
     def parse_actor(actor: str) -> Actor:
         tool_re: Pattern = re.compile(r"^Tool:\s*(.+)", re.UNICODE)
-        person_re: Pattern = re.compile(r"^Person:\s*(([^(])+)(\((.*)\))?", re.UNICODE)
-        org_re: Pattern = re.compile(r"^Organization:\s*(([^(])+)(\((.*)\))?", re.UNICODE)
+        person_re: Pattern = re.compile(r"^Person:\s*(?:(.*)\((.*)\)|(.*))$", re.UNICODE)
+        org_re: Pattern = re.compile(r"^Organization:\s*(?:(.*)\((.*)\)|(.*))$", re.UNICODE)
         tool_match: Match = tool_re.match(actor)
         person_match: Match = person_re.match(actor)
         org_match: Match = org_re.match(actor)
 
         if tool_match:
             name: str = tool_match.group(1).strip()
             if not name:
                 raise SPDXParsingError([f"No name for Tool provided: {actor}."])
-            creator = construct_or_raise_parsing_error(Actor, dict(actor_type=ActorType.TOOL, name=name))
+            return construct_or_raise_parsing_error(Actor, dict(actor_type=ActorType.TOOL, name=name))
 
-        elif person_match:
-            name: str = person_match.group(1).strip()
-            if not name:
-                raise SPDXParsingError([f"No name for Person provided: {actor}."])
-            email: Optional[str] = ActorParser.get_email_or_none(person_match)
-            creator = construct_or_raise_parsing_error(
-                Actor, dict(actor_type=ActorType.PERSON, name=name, email=email)
-            )
+        if person_match:
+            actor_type = ActorType.PERSON
+            match = person_match
         elif org_match:
-            name: str = org_match.group(1).strip()
-            if not name:
-                raise SPDXParsingError([f"No name for Organization provided: {actor}."])
-            email: Optional[str] = ActorParser.get_email_or_none(org_match)
-            creator = construct_or_raise_parsing_error(
-                Actor, dict(actor_type=ActorType.ORGANIZATION, name=name, email=email)
-            )
+            actor_type = ActorType.ORGANIZATION
+            match = org_match
         else:
             raise SPDXParsingError([f"Actor {actor} doesn't match any of person, organization or tool."])
 
-        return creator
-
-    @staticmethod
-    def get_email_or_none(match: Match) -> Optional[str]:
-        email_match = match.group(4)
-        if email_match and email_match.strip():
-            email = email_match.strip()
+        if match.group(3):
+            return construct_or_raise_parsing_error(
+                Actor, dict(actor_type=actor_type, name=match.group(3).strip(), email=None)
+            )
         else:
-            email = None
-        return email
+            name = match.group(1)
+            if not name:
+                raise SPDXParsingError([f"No name for Actor provided: {actor}."])
+            else:
+                name = name.strip()
+
+            email = match.group(2).strip()
+
+            return construct_or_raise_parsing_error(
+                Actor, dict(actor_type=actor_type, name=name, email=email if email else None)
+            )
```

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/annotation_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/annotation_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/checksum_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/checksum_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/creation_info_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/creation_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/dict_parsing_functions.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/dict_parsing_functions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/extracted_licensing_info_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/extracted_licensing_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/file_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/file_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/json_like_dict_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/json_like_dict_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/license_expression_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/license_expression_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/package_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/package_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/relationship_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/relationship_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/jsonlikedict/snippet_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/jsonlikedict/snippet_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/logger.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/logger.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/parse_anything.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/parse_anything.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/parsing_functions.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/parsing_functions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/annotation_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/annotation_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/checksum_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/checksum_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/creation_info_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/creation_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/extracted_licensing_info_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/extracted_licensing_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/file_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/file_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/graph_parsing_functions.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/graph_parsing_functions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/license_expression_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/license_expression_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/package_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/package_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/rdf_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/rdf_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/relationship_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/relationship_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/rdf/snippet_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/rdf/snippet_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/tagvalue/helper_methods.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/tagvalue/helper_methods.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/tagvalue/lexer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/tagvalue/lexer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/tagvalue/parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/tagvalue/parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/parser/xml/xml_parser.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/parser/xml/xml_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/actor_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/actor_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/annotation_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/annotation_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/checksum_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/checksum_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/creation_info_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/creation_info_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/document_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/document_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/external_document_ref_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/external_document_ref_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/external_package_ref_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/external_package_ref_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/extracted_licensing_info_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/extracted_licensing_info_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/file_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/file_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/license_expression_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/license_expression_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/package_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/package_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/package_verification_code_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/package_verification_code_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/relationship_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/relationship_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/snippet_validator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/snippet_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/spdx_id_validators.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/spdx_id_validators.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/uri_validators.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/uri_validators.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/validation/validation_message.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/validation/validation_message.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/json/json_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/json/json_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/annotation_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/annotation_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/checksum_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/checksum_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/creation_info_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/creation_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/external_document_ref_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/external_document_ref_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/extracted_licensing_info_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/extracted_licensing_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/file_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/file_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/license_expression_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/license_expression_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/package_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/package_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/rdf_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/rdf_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/relationship_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/relationship_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/snippet_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/snippet_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/rdf/writer_utils.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/rdf/writer_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/annotation_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/annotation_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/checksum_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/checksum_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/creation_info_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/creation_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/extracted_licensing_info_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/extracted_licensing_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/file_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/file_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/package_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/package_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/relationship_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/relationship_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/snippet_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/snippet_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer_helper_functions.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer_helper_functions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/write_anything.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/write_anything.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/write_utils.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/write_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/xml/xml_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/xml/xml_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx/writer/yaml/yaml_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx/writer/yaml/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/actor.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/actor.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/annotation.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/annotation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/bump_utils.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/bump_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/checksum.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/checksum.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/creation_info.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/creation_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 from beartype.typing import List
 from semantic_version import Version
 
 from spdx_tools.spdx3.bump_from_spdx2.actor import bump_actor
 from spdx_tools.spdx3.bump_from_spdx2.external_document_ref import bump_external_document_ref
 from spdx_tools.spdx3.bump_from_spdx2.message import print_missing_conversion
-from spdx_tools.spdx3.model import CreationInfo, ProfileIdentifier, SpdxDocument
+from spdx_tools.spdx3.model import CreationInfo, ProfileIdentifierType, SpdxDocument
 from spdx_tools.spdx3.payload import Payload
 from spdx_tools.spdx.model.actor import ActorType
 from spdx_tools.spdx.model.document import CreationInfo as Spdx2_CreationInfo
 
 
 def bump_creation_info(spdx2_creation_info: Spdx2_CreationInfo, payload: Payload) -> SpdxDocument:
     document_namespace = spdx2_creation_info.document_namespace
@@ -36,15 +36,15 @@
         0,
         "part of licensing profile, " "https://github.com/spdx/spdx-3-model/issues/131",
     )
     creation_info = CreationInfo(
         spec_version=Version("3.0.0"),
         created=spdx2_creation_info.created,
         created_by=[],
-        profile=[ProfileIdentifier.CORE, ProfileIdentifier.SOFTWARE, ProfileIdentifier.LICENSING],
+        profile=[ProfileIdentifierType.CORE, ProfileIdentifierType.SOFTWARE, ProfileIdentifierType.LICENSING],
         data_license="https://spdx.org/licenses/" + spdx2_creation_info.data_license,
     )
 
     # due to creators having a creation_info themselves which inherits from the document's one,
     # we have to add them after the creation_info has been initialized
     creator_ids: List[str] = []
     tool_ids: List[str] = []
```

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/external_document_ref.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/external_document_ref.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/file.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/file.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/license_expression.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/license_expression.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/package.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/package.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/snippet.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/snippet.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/bump_from_spdx2/spdx_document.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/bump_from_spdx2/spdx_document.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/clitools/pyspdxtools3.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/clitools/pyspdxtools3.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/__init__.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-FileCopyrightText: 2023 spdx contributors
 #
 # SPDX-License-Identifier: Apache-2.0
-from spdx_tools.spdx3.model.profile_identifier import ProfileIdentifier
+from spdx_tools.spdx3.model.profile_identifier import ProfileIdentifierType
 from spdx_tools.spdx3.model.creation_info import CreationInfo
 from spdx_tools.spdx3.model.integrity_method import IntegrityMethod
 from spdx_tools.spdx3.model.hash import Hash, HashAlgorithm
 from spdx_tools.spdx3.model.external_reference import ExternalReference, ExternalReferenceType
 from spdx_tools.spdx3.model.external_identifier import ExternalIdentifier, ExternalIdentifierType
 from spdx_tools.spdx3.model.external_map import ExternalMap
 from spdx_tools.spdx3.model.namespace_map import NamespaceMap
```

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/agent.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/agent.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/ai/ai_package.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/ai/ai_package.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/annotation.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/annotation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/artifact.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/artifact.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/bom.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/bom.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/build/build.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/build/build.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/bundle.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/bundle.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/creation_info.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/creation_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 from datetime import datetime
 
 from beartype.typing import List, Optional
 from semantic_version import Version
 
 from spdx_tools.common.typing.dataclass_with_properties import dataclass_with_properties
 from spdx_tools.common.typing.type_checks import check_types_and_set_values
-from spdx_tools.spdx3.model import ProfileIdentifier
+from spdx_tools.spdx3.model import ProfileIdentifierType
 
 
 @dataclass_with_properties
 class CreationInfo:
     spec_version: Version
     created: datetime
     created_by: List[str]  # SPDXID of Agents
-    profile: List[ProfileIdentifier]
+    profile: List[ProfileIdentifierType]
     data_license: Optional[str] = "CC0-1.0"
     created_using: List[str] = field(default_factory=list)  # SPDXID of Tools
     comment: Optional[str] = None
 
     def __init__(
         self,
         spec_version: Version,
         created: datetime,
         created_by: List[str],
-        profile: List[ProfileIdentifier],
+        profile: List[ProfileIdentifierType],
         data_license: Optional[str] = "CC0-1.0",
         created_using: List[str] = None,
         comment: Optional[str] = None,
     ):
         created_using = [] if created_using is None else created_using
         check_types_and_set_values(self, locals())
```

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/dataset/dataset.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/element.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/element.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/external_identifier.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/external_identifier.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/external_map.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/external_map.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/external_reference.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/external_reference.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/hash.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/hash.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/__init__.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/__init__.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/conjunctive_license_set.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/conjunctive_license_set.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/custom_license.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/custom_license.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/custom_license_addition.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/custom_license_addition.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/disjunctive_license_set.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/disjunctive_license_set.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/license.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/license.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/license_addition.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/license_addition.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/listed_license.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/listed_license.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/listed_license_exception.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/listed_license_exception.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/or_later_operator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/or_later_operator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/licensing/with_addition_operator.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/licensing/with_addition_operator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/lifecycle_scoped_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/lifecycle_scoped_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/organization.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/organization.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/person.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/person.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/__init__.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/__init__.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/cvss_v2_vuln_assessment_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/cvss_v2_vuln_assessment_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/cvss_v3_vuln_assessment_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/cvss_v3_vuln_assessment_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/epss_vuln_assessment_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/epss_vuln_assessment_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/exploit_catalog_vuln_assessment_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/exploit_catalog_vuln_assessment_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/ssvc_vuln_assessment_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/ssvc_vuln_assessment_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vex_affected_vuln_assessment_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vex_affected_vuln_assessment_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vex_fixed_vuln_assessment_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vex_fixed_vuln_assessment_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vex_not_affected_vuln_assessment_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vex_not_affected_vuln_assessment_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vex_under_investigation_vuln_assessment_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vex_under_investigation_vuln_assessment_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vex_vuln_assessment_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vex_vuln_assessment_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vuln_assessment_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vuln_assessment_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/security/vulnerability.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/security/vulnerability.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/__init__.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/__init__.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/file.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/file.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/package.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/package.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/sbom.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/sbom.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/snippet.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/snippet.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/software_artifact.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/software_artifact.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/software_dependency_relationship.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/software_dependency_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software/software_purpose.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software/software_purpose.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/software_agent.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/software_agent.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/spdx_collection.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/spdx_collection.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/spdx_document.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/spdx_document.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/model/tool.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/model/tool.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/payload.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/payload.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/validation/json_ld/shacl_validation.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/validation/json_ld/shacl_validation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/agent_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/agent_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/ai/ai_package_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/ai/ai_package_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/annotation_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/annotation_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/artifact_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/artifact_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/build/build_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/build/build_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/bundle_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/bundle_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/console.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/console.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/creation_info_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/creation_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/dataset/dataset_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/dataset/dataset_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/element_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/element_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/external_map_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/external_map_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/hash_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/hash_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/lifecycle_scoped_relationship_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/lifecycle_scoped_relationship_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/payload_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/payload_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/relationship_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/relationship_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/software/file_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/software/file_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/software/package_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/software/package_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/software/snippet_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/software/snippet_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/software/software_dependency_relationship_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/software/software_dependency_relationship_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/spdx_collection_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/spdx_collection_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/console/tool_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/console/tool_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/SPDX_OWL.json` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/SPDX_OWL.json`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/context.json` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/context.json`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/json_ld_converter.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/json_ld_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/json_ld_writer.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/json_ld_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/model.ttl` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/model.ttl`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/owl_to_context.py` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/owl_to_context.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools/spdx3/writer/json_ld/process.md` & `spdx-tools-0.8.0rc2/src/spdx_tools/spdx3/writer/json_ld/process.md`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/src/spdx_tools.egg-info/SOURCES.txt` & `spdx-tools-0.8.0rc2/src/spdx_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 appveyor.yml
 pyproject.toml
 setup.py
 stdeb.cfg
 .circleci/config.yml
 .github/dependabot.yml
 .github/workflows/check_codestyle.yml
+.github/workflows/docs.yml
 .github/workflows/install_and_test.yml
 .github/workflows/integration_test.yml
 .github/workflows/prepare_release.yml
 assets/SPDXJSONExample-v2.3.spdx.png
 examples/spdx2_convert_format.py
 examples/spdx2_convert_to_spdx3.py
 examples/spdx2_document_from_scratch.py
@@ -306,14 +307,15 @@
 src/spdx_tools/spdx3/writer/json_ld/process.md
 tests/__init__.py
 tests/spdx/__init__.py
 tests/spdx/fixtures.py
 tests/spdx/mock_utils.py
 tests/spdx/test_actor_parser.py
 tests/spdx/test_casing_tools.py
+tests/spdx/test_checksum_calculation.py
 tests/spdx/test_cli.py
 tests/spdx/test_datetime_conversions.py
 tests/spdx/test_document_utils.py
 tests/spdx/test_graph_generation.py
 tests/spdx/data/SPDXJSONExample-v2.2.spdx.json
 tests/spdx/data/SPDXJSONExample-v2.3.spdx.json
 tests/spdx/data/SPDXLite.spdx
```

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/SPDXJSONExample-v2.2.spdx.json` & `spdx-tools-0.8.0rc2/tests/spdx/data/SPDXJSONExample-v2.2.spdx.json`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/SPDXJSONExample-v2.3.spdx.json` & `spdx-tools-0.8.0rc2/tests/spdx/data/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/SPDXLite.spdx` & `spdx-tools-0.8.0rc2/tests/spdx/data/SPDXLite.spdx`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/SPDXRdfExample-v2.2.spdx.rdf.xml` & `spdx-tools-0.8.0rc2/tests/spdx/data/SPDXRdfExample-v2.2.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/SPDXRdfExample-v2.3.spdx.rdf.xml` & `spdx-tools-0.8.0rc2/tests/spdx/data/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/SPDXTagExample-v2.2.spdx` & `spdx-tools-0.8.0rc2/tests/spdx/data/SPDXTagExample-v2.2.spdx`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/SPDXTagExample-v2.3.spdx` & `spdx-tools-0.8.0rc2/tests/spdx/data/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/SPDXXMLExample-v2.2.spdx.xml` & `spdx-tools-0.8.0rc2/tests/spdx/data/SPDXXMLExample-v2.2.spdx.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml` & `spdx-tools-0.8.0rc2/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/SPDXYAMLExample-v2.2.spdx.yaml` & `spdx-tools-0.8.0rc2/tests/spdx/data/SPDXYAMLExample-v2.2.spdx.yaml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/SPDXYAMLExample-v2.3.spdx.yaml` & `spdx-tools-0.8.0rc2/tests/spdx/data/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/data/circleConversionTestInitialDocument.json` & `spdx-tools-0.8.0rc2/tests/spdx/data/circleConversionTestInitialDocument.json`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/examples/test_examples.py` & `spdx-tools-0.8.0rc2/tests/spdx/examples/test_examples.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/examples/test_spdx2_document_from_scratch.py` & `spdx-tools-0.8.0rc2/tests/spdx/examples/test_spdx2_document_from_scratch.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/fixtures.py` & `spdx-tools-0.8.0rc2/tests/spdx/fixtures.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_annotation_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_annotation_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_checksum_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_checksum_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_creation_info_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_creation_info_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_document_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_document_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_external_document_ref_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_external_document_ref_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_external_package_ref_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_external_package_ref_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_extracted_licensing_info_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_extracted_licensing_info_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_file_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_file_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_package_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_package_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_package_verification_code_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_package_verification_code_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_relationship_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_relationship_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/jsonschema/test_snippet_converter.py` & `spdx-tools-0.8.0rc2/tests/spdx/jsonschema/test_snippet_converter.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/mock_utils.py` & `spdx-tools-0.8.0rc2/tests/spdx/mock_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_actor.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_actor.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_annotation.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_annotation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_checksum.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_checksum.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_creation_info.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_creation_info.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_document.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_document.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_external_document_ref.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_external_document_ref.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_external_package_reference.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_external_package_reference.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_extracted_licensing_info.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_extracted_licensing_info.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_file.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_file.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_package.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_package.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_package_verification_code.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_package_verification_code.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_relationship.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_relationship.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_snippet.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_snippet.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/model/test_version.py` & `spdx-tools-0.8.0rc2/tests/spdx/model/test_version.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/all_formats/test_parse_from_file.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/all_formats/test_parse_from_file.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_annotation_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_checksum_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_checksum_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_creation_info_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_creation_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_dict_parsing_functions.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_dict_parsing_functions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_extracted_licensing_info_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_extracted_licensing_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_file_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_file_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_license_expression_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_license_expression_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_package_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_package_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_relationship_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_relationship_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/jsonlikedict/test_snippet_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/jsonlikedict/test_snippet_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/data/file_to_test_rdf_parser.rdf.xml` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/data/file_to_test_rdf_parser.rdf.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/data/invalid_documents/file_without_spdx_ids.xml` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/data/invalid_documents/file_without_spdx_ids.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info.rdf.xml` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info.rdf.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info_with_snippet.rdf.xml` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/data/invalid_documents/invalid_creation_info_with_snippet.rdf.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_annotation_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_checksum_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_checksum_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_creation_info_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_creation_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_extracted_licensing_info_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_extracted_licensing_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_file_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_file_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_graph_parsing_function.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_graph_parsing_function.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_license_expression_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_license_expression_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_package_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_package_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_relationship_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_relationship_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/rdf/test_snippet_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/rdf/test_snippet_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_annotation_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_annotation_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             "Annotator: Jane Doe()\nAnnotationDate: 201001-29T18:30:22Z\n"
             "AnnotationComment: <text>Document level annotation</text>\nAnnotationType: OTHER\n"
             f"SPDXREF: {DOCUMENT_SPDX_ID}",
             "Error while parsing Annotation: ['Error while parsing Annotator: Token did "
             "not match specified grammar rule. Line: 1', 'Error while parsing "
             "AnnotationDate: Token did not match specified grammar rule. Line: 2']",
         ),
-        ("Annotator: Person: ()", "Error while parsing Annotation: [['No name for Person provided: Person: ().']]"),
+        ("Annotator: Person: ()", "Error while parsing Annotation: [['No name for Actor provided: Person: ().']]"),
         (
             "AnnotationType: REVIEW",
             "Element Annotation is not the current element in scope, probably the "
             "expected tag to start the element (Annotator) is missing. Line: 1",
         ),
     ],
 )
```

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_creation_info_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_creation_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_extracted_licensing_info_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_extracted_licensing_info_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_file_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_file_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_helper_methods.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_helper_methods.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_package_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_package_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_relationship_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_relationship_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_snippet_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_snippet_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_tag_value_lexer.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_tag_value_lexer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/parser/tagvalue/test_tag_value_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/parser/tagvalue/test_tag_value_parser.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/test_actor_parser.py` & `spdx-tools-0.8.0rc2/tests/spdx/test_actor_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,24 @@
         (
             "Organization: Example organization (organization@example.com)",
             ActorType.ORGANIZATION,
             "Example organization",
             "organization@example.com",
         ),
         ("Organization: Example organization ( )", ActorType.ORGANIZATION, "Example organization", None),
+        ("Person: Example person ()", ActorType.PERSON, "Example person", None),
+        ("Person: Example person ", ActorType.PERSON, "Example person", None),
         ("Tool: Example tool ", ActorType.TOOL, "Example tool", None),
+        ("Tool: Example tool (email@mail.com)", ActorType.TOOL, "Example tool (email@mail.com)", None),
+        (
+            "Organization: (c) Chris Sainty (chris@sainty.com)",
+            ActorType.ORGANIZATION,
+            "(c) Chris Sainty",
+            "chris@sainty.com",
+        ),
     ],
 )
 def test_parse_actor(actor_string, expected_type, expected_name, expected_mail):
     actor_parser = ActorParser()
 
     actor = actor_parser.parse_actor(actor_string)
 
@@ -38,14 +47,16 @@
     "actor_string,expected_message",
     [
         (
             "Perso: Jane Doe (jane.doe@example.com)",
             ["Actor Perso: Jane Doe (jane.doe@example.com) doesn't match any of person, organization or tool."],
         ),
         ("Toole Example Tool ()", ["Actor Toole Example Tool () doesn't match any of person, organization or tool."]),
+        ("Organization:", ["No name for Actor provided: Organization:."]),
+        ("Person: ( )", ["No name for Actor provided: Person: ( )."]),
     ],
 )
 def test_parse_invalid_actor(actor_string, expected_message):
     actor_parser = ActorParser()
     actor_string = actor_string
 
     with pytest.raises(SPDXParsingError) as err:
```

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/test_casing_tools.py` & `spdx-tools-0.8.0rc2/tests/spdx/test_casing_tools.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/test_cli.py` & `spdx-tools-0.8.0rc2/tests/spdx/test_cli.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/test_datetime_conversions.py` & `spdx-tools-0.8.0rc2/tests/spdx/test_datetime_conversions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/test_document_utils.py` & `spdx-tools-0.8.0rc2/tests/spdx/test_document_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/test_graph_generation.py` & `spdx-tools-0.8.0rc2/tests/spdx/test_graph_generation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_actor_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_actor_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_annotation_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_annotation_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_checksum_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_checksum_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_creation_info_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_creation_info_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_document_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_document_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_external_document_ref_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_external_document_ref_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_external_package_ref_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_external_package_ref_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_extracted_licensing_info_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_extracted_licensing_info_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_file_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_file_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_license_expression_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_license_expression_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_package_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_package_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_package_verification_code_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_package_verification_code_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_relationship_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_relationship_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_snippet_validator.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_snippet_validator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_spdx_id_validators.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_spdx_id_validators.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/validation/test_uri_validators.py` & `spdx-tools-0.8.0rc2/tests/spdx/validation/test_uri_validators.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/json/expected_results/expected.json` & `spdx-tools-0.8.0rc2/tests/spdx/writer/json/expected_results/expected.json`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/json/test_json_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/json/test_json_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_annotation_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_checksum_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_checksum_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_creation_info_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_creation_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_external_document_ref_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_external_document_ref_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_extracted_licensing_info_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_extracted_licensing_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_file_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_license_expression_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_license_expression_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_package_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_package_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_rdf_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_relationship_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_relationship_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_snippet_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_snippet_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/rdf/test_writer_utils.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/rdf/test_writer_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/expected_results/expected_tag_value.spdx` & `spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/expected_results/expected_tag_value.spdx`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_annotation_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_checksum_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_checksum_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_creation_info_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_creation_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_extracted_licensing_info_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_extracted_licensing_info_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_file_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_package_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_package_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_relationship_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_relationship_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_snippet_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_snippet_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_tagvalue_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_tagvalue_writer.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx/writer/tagvalue/test_tagvalue_writer_helper_functions.py` & `spdx-tools-0.8.0rc2/tests/spdx/writer/tagvalue/test_tagvalue_writer_helper_functions.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/bump/test_actor_bump.py` & `spdx-tools-0.8.0rc2/tests/spdx3/bump/test_actor_bump.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from spdx_tools.spdx3.bump_from_spdx2.actor import bump_actor
 from spdx_tools.spdx3.model import (
     CreationInfo,
     ExternalIdentifier,
     ExternalIdentifierType,
     Organization,
     Person,
-    ProfileIdentifier,
+    ProfileIdentifierType,
     Tool,
 )
 from spdx_tools.spdx3.payload import Payload
 from spdx_tools.spdx.model.actor import Actor, ActorType
 
 
 @pytest.mark.parametrize(
@@ -33,15 +33,15 @@
         ),
         (ActorType.TOOL, "tool name", None, Tool, "SPDXRef-Actor-toolname"),
     ],
 )
 def test_bump_actor(actor_type, actor_name, actor_mail, element_type, new_spdx_id):
     payload = Payload()
     document_namespace = "https://doc.namespace"
-    creation_info = CreationInfo(Version("3.0.0"), datetime(2022, 1, 1), ["Creator"], [ProfileIdentifier.CORE])
+    creation_info = CreationInfo(Version("3.0.0"), datetime(2022, 1, 1), ["Creator"], [ProfileIdentifierType.CORE])
     actor = Actor(actor_type, actor_name, actor_mail)
 
     agent_or_tool_id = bump_actor(actor, payload, document_namespace, creation_info)
     agent_or_tool = payload.get_element(agent_or_tool_id)
 
     assert isinstance(agent_or_tool, element_type)
     assert agent_or_tool.spdx_id == f"{document_namespace}#{new_spdx_id}"
@@ -50,16 +50,16 @@
         assert len(agent_or_tool.external_identifier) == 1
         assert agent_or_tool.external_identifier[0] == ExternalIdentifier(ExternalIdentifierType.EMAIL, actor_mail)
     else:
         assert len(agent_or_tool.external_identifier) == 0
 
 
 def test_bump_actor_that_already_exists():
-    creation_info_old = CreationInfo(Version("3.0.0"), datetime(2022, 1, 1), ["Creator"], [ProfileIdentifier.CORE])
-    creation_info_new = CreationInfo(Version("3.0.0"), datetime(2023, 2, 2), ["Creator"], [ProfileIdentifier.CORE])
+    creation_info_old = CreationInfo(Version("3.0.0"), datetime(2022, 1, 1), ["Creator"], [ProfileIdentifierType.CORE])
+    creation_info_new = CreationInfo(Version("3.0.0"), datetime(2023, 2, 2), ["Creator"], [ProfileIdentifierType.CORE])
 
     name = "some name"
     document_namespace = "https://doc.namespace"
     payload = Payload(
         {
             "https://doc.namespace#SPDXRef-Actor-somename-some@mail.com": Person(
                 "https://doc.namespace#SPDXRef-Actor-somename-some@mail.com", creation_info_old, name
```

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/bump/test_bump_utils.py` & `spdx-tools-0.8.0rc2/tests/spdx3/bump/test_bump_utils.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/bump/test_checksum_bump.py` & `spdx-tools-0.8.0rc2/tests/spdx3/bump/test_checksum_bump.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/bump/test_external_document_ref_bump.py` & `spdx-tools-0.8.0rc2/tests/spdx3/bump/test_external_document_ref_bump.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/bump/test_external_element_bump.py` & `spdx-tools-0.8.0rc2/tests/spdx3/bump/test_external_element_bump.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/bump/test_file_bump.py` & `spdx-tools-0.8.0rc2/tests/spdx3/bump/test_file_bump.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/bump/test_license_expression_bump.py` & `spdx-tools-0.8.0rc2/tests/spdx3/bump/test_license_expression_bump.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/bump/test_package_bump.py` & `spdx-tools-0.8.0rc2/tests/spdx3/bump/test_package_bump.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/bump/test_relationship_bump.py` & `spdx-tools-0.8.0rc2/tests/spdx3/bump/test_relationship_bump.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/bump/test_snippet_bump.py` & `spdx-tools-0.8.0rc2/tests/spdx3/bump/test_snippet_bump.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/bump/test_spdx_document_bump.py` & `spdx-tools-0.8.0rc2/tests/spdx3/bump/test_spdx_document_bump.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/fixtures.py` & `spdx-tools-0.8.0rc2/tests/spdx3/fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Hash,
     HashAlgorithm,
     LifecycleScopedRelationship,
     LifecycleScopeType,
     NamespaceMap,
     Organization,
     Person,
-    ProfileIdentifier,
+    ProfileIdentifierType,
     Relationship,
     RelationshipCompleteness,
     RelationshipType,
     SoftwareAgent,
     SpdxDocument,
     Tool,
 )
@@ -89,15 +89,15 @@
     comment="creationInfoComment",
 ) -> CreationInfo:
     created_by = ["https://spdx.test/tools-python/creation_info_created_by"] if created_by is None else created_by
     created_using = (
         ["https://spdx.test/tools-python/creation_info_created_using"] if created_using is None else created_using
     )
     profile = (
-        [ProfileIdentifier.CORE, ProfileIdentifier.SOFTWARE, ProfileIdentifier.LICENSING]
+        [ProfileIdentifierType.CORE, ProfileIdentifierType.SOFTWARE, ProfileIdentifierType.LICENSING]
         if profile is None
         else profile
     )
     return CreationInfo(
         spec_version=spec_version,
         created=created,
         created_by=created_by,
```

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/model/licensing/test_conjunctive_license_set.py` & `spdx-tools-0.8.0rc2/tests/spdx3/model/licensing/test_conjunctive_license_set.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/model/licensing/test_disjunctive_license_set.py` & `spdx-tools-0.8.0rc2/tests/spdx3/model/licensing/test_disjunctive_license_set.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/model/licensing/test_or_later_operator.py` & `spdx-tools-0.8.0rc2/tests/spdx3/model/licensing/test_or_later_operator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/model/licensing/test_with_addition_operator.py` & `spdx-tools-0.8.0rc2/tests/spdx3/model/licensing/test_with_addition_operator.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/model/test_creation_info.py` & `spdx-tools-0.8.0rc2/tests/spdx3/model/test_creation_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 from datetime import datetime
 
 import pytest
 from semantic_version import Version
 
-from spdx_tools.spdx3.model import CreationInfo, ProfileIdentifier
+from spdx_tools.spdx3.model import CreationInfo, ProfileIdentifierType
 from tests.spdx3.fixtures import creation_info_fixture
 from tests.spdx3.model.model_test_utils import get_property_names
 
 
 def test_correct_initialization():
     creation_info = creation_info_fixture()
 
@@ -18,17 +18,17 @@
         assert getattr(creation_info, property_name) is not None
 
     assert creation_info.spec_version == Version("3.0.0")
     assert creation_info.created == datetime(2022, 12, 1)
     assert creation_info.created_by == ["https://spdx.test/tools-python/creation_info_created_by"]
     assert creation_info.created_using == ["https://spdx.test/tools-python/creation_info_created_using"]
     assert creation_info.profile == [
-        ProfileIdentifier.CORE,
-        ProfileIdentifier.SOFTWARE,
-        ProfileIdentifier.LICENSING,
+        ProfileIdentifierType.CORE,
+        ProfileIdentifierType.SOFTWARE,
+        ProfileIdentifierType.LICENSING,
     ]
     assert creation_info.data_license == "CC0-1.0"
     assert creation_info.comment == "creationInfoComment"
 
 
 def test_invalid_initialization():
     with pytest.raises(TypeError) as err:
```

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/model/test_element_and_licensing_subclasses.py` & `spdx-tools-0.8.0rc2/tests/spdx3/model/test_element_and_licensing_subclasses.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/model/test_external_identifier.py` & `spdx-tools-0.8.0rc2/tests/spdx3/model/test_external_identifier.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/model/test_external_map.py` & `spdx-tools-0.8.0rc2/tests/spdx3/model/test_external_map.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/model/test_external_reference.py` & `spdx-tools-0.8.0rc2/tests/spdx3/model/test_external_reference.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/model/test_hash.py` & `spdx-tools-0.8.0rc2/tests/spdx3/model/test_hash.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/model/test_namespace_map.py` & `spdx-tools-0.8.0rc2/tests/spdx3/model/test_namespace_map.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/validation/json_ld/test_shacl_validation.py` & `spdx-tools-0.8.0rc2/tests/spdx3/validation/json_ld/test_shacl_validation.py`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.8.0rc1/tests/spdx3/writer/json_ld/test_json_ld_writer.py` & `spdx-tools-0.8.0rc2/tests/spdx3/writer/json_ld/test_json_ld_writer.py`

 * *Files identical despite different names*

