# Comparing `tmp/somef-0.9.3.tar.gz` & `tmp/somef-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somef-0.9.3.tar", last modified: Mon Jan 16 20:40:22 2023, max compression
+gzip compressed data, was "somef-0.9.4.tar", last modified: Fri Jul 14 15:08:03 2023, max compression
```

## Comparing `somef-0.9.3.tar` & `somef-0.9.4.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.147588 somef-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-16 20:40:10.000000 somef-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13748 2023-01-16 20:40:22.147588 somef-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-01-16 20:40:10.000000 somef-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-01-16 20:40:10.000000 somef-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 20:40:22.147588 somef-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-01-16 20:40:10.000000 somef-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.127586 somef-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.131586 somef-0.9.3/src/somef/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.131586 somef-0.9.3/src/somef/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/export/json_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/export/turtle_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/extract_ontologies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/header_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.131586 somef-0.9.3/src/somef/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19932 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/mapping/rml.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/mapping/yarrrml.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.131586 somef-0.9.3/src/somef/models/
--rw-r--r--   0 runner    (1001) docker     (123)    86221 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/models/citation.p
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.135587 somef-0.9.3/src/somef/models/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)   111360 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/models/deprecated/citation.sk
--rw-r--r--   0 runner    (1001) docker     (123)   160624 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/models/deprecated/description.sk
--rw-r--r--   0 runner    (1001) docker     (123)   208073 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/models/deprecated/installation.sk
--rw-r--r--   0 runner    (1001) docker     (123)   262875 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/models/deprecated/invocation.sk
--rw-r--r--   0 runner    (1001) docker     (123)    92547 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/models/description.p
--rw-r--r--   0 runner    (1001) docker     (123)   125208 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/models/installation.p
--rw-r--r--   0 runner    (1001) docker     (123)   248668 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/models/invocation.p
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.135587 somef-0.9.3/src/somef/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/parser/create_excerpts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16707 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/parser/mardown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/process_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    24055 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/process_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/process_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    23953 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/regular_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.135587 somef-0.9.3/src/somef/rolf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/rolf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.139587 somef-0.9.3/src/somef/rolf/models/
--rw-r--r--   0 runner    (1001) docker     (123)   211957 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/rolf/models/audio.sav
--rw-r--r--   0 runner    (1001) docker     (123)   908203 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/rolf/models/computer_vision.sav
--rw-r--r--   0 runner    (1001) docker     (123)   256071 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/rolf/models/graphs.sav
--rw-r--r--   0 runner    (1001) docker     (123)   586740 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/rolf/models/natural_language_processing.sav
--rw-r--r--   0 runner    (1001) docker     (123)   384127 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/rolf/models/reinforcement_learning.sav
--rw-r--r--   0 runner    (1001) docker     (123)   595013 2023-01-16 20:40:10.000000 somef-0.9.3/src/somef/rolf/models/semantic_web.sav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.143587 somef-0.9.3/src/somef/rolf/models_test/
--rw-r--r--   0 runner    (1001) docker     (123)  3831761 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/rolf/models_test/astrophysics.sav
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/rolf/models_test/rationale.md
--rw-r--r--   0 runner    (1001) docker     (123)   244691 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/rolf/models_test/sequential.sav
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/rolf/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/somef_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/supervised_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.147588 somef-0.9.3/src/somef/test/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/test_JSON_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    40284 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/test_extract_ontologies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/test_header_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/test_parser_somef.py
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/test_process_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/test_process_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    21092 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/test_regular_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/test_supervised_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/test/test_turtle_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.147588 somef-0.9.3/src/somef/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-01-16 20:40:11.000000 somef-0.9.3/src/somef/utils/markdown_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 20:40:22.131586 somef-0.9.3/src/somef.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13748 2023-01-16 20:40:22.000000 somef-0.9.3/src/somef.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-01-16 20:40:22.000000 somef-0.9.3/src/somef.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 20:40:22.000000 somef-0.9.3/src/somef.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-16 20:40:22.000000 somef-0.9.3/src/somef.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 20:40:22.000000 somef-0.9.3/src/somef.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-16 20:40:22.000000 somef-0.9.3/src/somef.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-16 20:40:22.000000 somef-0.9.3/src/somef.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.892263 somef-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-14 15:07:53.000000 somef-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14300 2023-07-14 15:08:03.892263 somef-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-14 15:07:53.000000 somef-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-14 15:07:54.000000 somef-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 15:08:03.892263 somef-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-14 15:07:54.000000 somef-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.876263 somef-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.876263 somef-0.9.4/src/somef/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.880262 somef-0.9.4/src/somef/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/export/json_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/export/turtle_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/extract_ontologies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/extract_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/header_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.880262 somef-0.9.4/src/somef/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19932 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/mapping/rml.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/mapping/yarrrml.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.880262 somef-0.9.4/src/somef/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    86221 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/models/citation.p
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.880262 somef-0.9.4/src/somef/models/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)   111360 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/models/deprecated/citation.sk
+-rw-r--r--   0 runner    (1001) docker     (123)   160624 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/models/deprecated/description.sk
+-rw-r--r--   0 runner    (1001) docker     (123)   208073 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/models/deprecated/installation.sk
+-rw-r--r--   0 runner    (1001) docker     (123)   262875 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/models/deprecated/invocation.sk
+-rw-r--r--   0 runner    (1001) docker     (123)    92547 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/models/description.p
+-rw-r--r--   0 runner    (1001) docker     (123)   125208 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/models/installation.p
+-rw-r--r--   0 runner    (1001) docker     (123)   248668 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/models/invocation.p
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.880262 somef-0.9.4/src/somef/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/parser/create_excerpts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16707 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/parser/mardown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/process_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24055 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/process_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/process_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24848 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/regular_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.880262 somef-0.9.4/src/somef/rolf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/rolf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.884262 somef-0.9.4/src/somef/rolf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)   211957 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/rolf/models/audio.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   908203 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/rolf/models/computer_vision.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   256071 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/rolf/models/graphs.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   586740 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/rolf/models/natural_language_processing.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   384127 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/rolf/models/reinforcement_learning.sav
+-rw-r--r--   0 runner    (1001) docker     (123)   595013 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/rolf/models/semantic_web.sav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.888263 somef-0.9.4/src/somef/rolf/models_test/
+-rw-r--r--   0 runner    (1001) docker     (123)  3831761 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/rolf/models_test/astrophysics.sav
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/rolf/models_test/rationale.md
+-rw-r--r--   0 runner    (1001) docker     (123)   244691 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/rolf/models_test/sequential.sav
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/rolf/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/somef_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/supervised_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.888263 somef-0.9.4/src/somef/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_JSON_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40284 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_extract_ontologies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_extract_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_header_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_parser_somef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_process_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_process_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22369 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_regular_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_supervised_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/test/test_turtle_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.892263 somef-0.9.4/src/somef/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-14 15:07:54.000000 somef-0.9.4/src/somef/utils/markdown_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:08:03.880262 somef-0.9.4/src/somef.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14300 2023-07-14 15:08:03.000000 somef-0.9.4/src/somef.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-14 15:08:03.000000 somef-0.9.4/src/somef.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:08:03.000000 somef-0.9.4/src/somef.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 15:08:03.000000 somef-0.9.4/src/somef.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:08:03.000000 somef-0.9.4/src/somef.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-14 15:08:03.000000 somef-0.9.4/src/somef.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 15:08:03.000000 somef-0.9.4/src/somef.egg-info/top_level.txt
```

### Comparing `somef-0.9.3/LICENSE` & `somef-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/PKG-INFO` & `somef-0.9.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somef
-Version: 0.9.3
+Version: 0.9.4
 Summary: SOftware Metadata Extraction Framework: A tool for automatically extracting relevant software information from readme files
 Home-page: https://github.com/KnowledgeCaptureAndDiscovery/somef
 Author: Daniel Garijo
 Author-email: daniel.garijo@upm.es
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
@@ -18,14 +18,16 @@
 # Software Metadata Extraction Framework (SOMEF) 
 [![Python](https://img.shields.io/pypi/pyversions/somef.svg?style=plastic)](https://badge.fury.io/py/somef) [![PyPI](https://badge.fury.io/py/somef.svg)](https://badge.fury.io/py/somef) [![DOI](https://zenodo.org/badge/190487675.svg)](https://zenodo.org/badge/latestdoi/190487675) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/KnowledgeCaptureAndDiscovery/somef/HEAD?filepath=notebook%2FSOMEF%20Usage%20Example.ipynb)  [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 
 <img src="docs/logo.png" alt="logo" width="150"/>
 
 A command line interface for automatically extracting relevant information from readme files.
 
+**Demo:** See a [demo running somef as a service](https://somef.linkeddata.es), through the [SOMEF-Vider tool](https://github.com/SoftwareUnderstanding/SOMEF-Vider/). 
+
 **Authors:** Daniel Garijo, Allen Mao, Miguel Ángel García Delgado, Haripriya Dharmala, Vedant Diwanji, Jiaying Wang, Aidan Kelley and Jenifer Tabita Ciuciu-Kiss.
 
 ## Features
 Given a readme file (or a GitHub/Gitlab repository) SOMEF will extract the following categories (if present):
 
 - **Name**: Name identifying a software component
 - **Full name**: Name + owner (owner/name)
@@ -63,14 +65,16 @@
 - **Code of Conduct**: Link to the code of conduct of the project
 - **Scripts**: Snippets of code contained in the repository.
 - **Support channels**: Help channels one can use to get support about the target software component.
 - **Images**: Images used to illustrate the software component.
 - **Logo**: Main logo used to represent the target software component.
 - **Ontologies**: URL and path to the ontology files present in the repository.
 - **Application domain**: The application domain of the repository. Current supported domains include: Astrophisics, Audio, Computer vision, Graphs, Natural language processing, Reinforcement learning, Semantc web, Sequential. Domains are not mutually exclusive. These domains have been extracted from [awesome lists](https://github.com/topics/awesome-list) and [Papers with code](https://paperswithcode.com/). Find more information in our [documentation](https://somef.readthedocs.io/en/latest/).
+- **Workflows**: URL and path to the workflow files present in the repository.
+- **Related papers**: URL to possible related papers within the repository stated within the readme file.
 
 
 We use different supervised classifiers, header analysis, regular expressions and the GitHub/Gitlab API to retrieve all these fields (more than one technique may be used for each field). Each extraction records its provenance, with the confidence and technique used on each step. For more information check the [output format description](https://somef.readthedocs.io/en/latest/output/)
 
 ## Documentation
 See full documentation at [https://somef.readthedocs.io/en/latest/](https://somef.readthedocs.io/en/latest/)
 
@@ -179,17 +183,24 @@
 
 ```bash
 docker run -it --rm -v $PWD/:/out kcapd/somef /bin/bash
 ```
 If you move any files produced by somef into `/out`, then you will be able to see them in your current directory.
 
 
-## Usage
+## Configure
 
-Before running SOMEF for the first time, you must **configure** it appropriately (you only need to do this once). Run
+Before running SOMEF for the first time, you must **configure** it appropriately (you only need to do this once). Run:
+```bash
+python -m nltk.downloader wordnet
+python -m nltk.downloader omw-1.4
+python -m nltk.downloader punkt
+python -m nltk.downloader stopwords
+```
+To download two wordnet modules needed. Then run:
 
 ```bash
 somef configure
 ```
 
 And you will be asked to provide the following:
 
@@ -218,15 +229,15 @@
   -a, --auto  Automatically configure SOMEF
   -h, --help  Show this message and exit.
 ```
 
 ### Updating SOMEF
 If you update SOMEF to a newer version, we recommend you `configure` again the library (by running `somef configure`). The rationale is that different versions may rely on classifiers which may be stored in a different path. 
 
-### Run SOMEF
+## Usage
 
 ```bash
 $ somef describe --help
   SOMEF Command Line Interface
 Usage: somef describe [OPTIONS]
 
   Running the Command Line Interface
```

### Comparing `somef-0.9.3/README.md` & `somef-0.9.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Software Metadata Extraction Framework (SOMEF) 
 [![Python](https://img.shields.io/pypi/pyversions/somef.svg?style=plastic)](https://badge.fury.io/py/somef) [![PyPI](https://badge.fury.io/py/somef.svg)](https://badge.fury.io/py/somef) [![DOI](https://zenodo.org/badge/190487675.svg)](https://zenodo.org/badge/latestdoi/190487675) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/KnowledgeCaptureAndDiscovery/somef/HEAD?filepath=notebook%2FSOMEF%20Usage%20Example.ipynb)  [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 
 <img src="docs/logo.png" alt="logo" width="150"/>
 
 A command line interface for automatically extracting relevant information from readme files.
 
+**Demo:** See a [demo running somef as a service](https://somef.linkeddata.es), through the [SOMEF-Vider tool](https://github.com/SoftwareUnderstanding/SOMEF-Vider/). 
+
 **Authors:** Daniel Garijo, Allen Mao, Miguel Ángel García Delgado, Haripriya Dharmala, Vedant Diwanji, Jiaying Wang, Aidan Kelley and Jenifer Tabita Ciuciu-Kiss.
 
 ## Features
 Given a readme file (or a GitHub/Gitlab repository) SOMEF will extract the following categories (if present):
 
 - **Name**: Name identifying a software component
 - **Full name**: Name + owner (owner/name)
@@ -46,14 +48,16 @@
 - **Code of Conduct**: Link to the code of conduct of the project
 - **Scripts**: Snippets of code contained in the repository.
 - **Support channels**: Help channels one can use to get support about the target software component.
 - **Images**: Images used to illustrate the software component.
 - **Logo**: Main logo used to represent the target software component.
 - **Ontologies**: URL and path to the ontology files present in the repository.
 - **Application domain**: The application domain of the repository. Current supported domains include: Astrophisics, Audio, Computer vision, Graphs, Natural language processing, Reinforcement learning, Semantc web, Sequential. Domains are not mutually exclusive. These domains have been extracted from [awesome lists](https://github.com/topics/awesome-list) and [Papers with code](https://paperswithcode.com/). Find more information in our [documentation](https://somef.readthedocs.io/en/latest/).
+- **Workflows**: URL and path to the workflow files present in the repository.
+- **Related papers**: URL to possible related papers within the repository stated within the readme file.
 
 
 We use different supervised classifiers, header analysis, regular expressions and the GitHub/Gitlab API to retrieve all these fields (more than one technique may be used for each field). Each extraction records its provenance, with the confidence and technique used on each step. For more information check the [output format description](https://somef.readthedocs.io/en/latest/output/)
 
 ## Documentation
 See full documentation at [https://somef.readthedocs.io/en/latest/](https://somef.readthedocs.io/en/latest/)
 
@@ -162,17 +166,24 @@
 
 ```bash
 docker run -it --rm -v $PWD/:/out kcapd/somef /bin/bash
 ```
 If you move any files produced by somef into `/out`, then you will be able to see them in your current directory.
 
 
-## Usage
+## Configure
 
-Before running SOMEF for the first time, you must **configure** it appropriately (you only need to do this once). Run
+Before running SOMEF for the first time, you must **configure** it appropriately (you only need to do this once). Run:
+```bash
+python -m nltk.downloader wordnet
+python -m nltk.downloader omw-1.4
+python -m nltk.downloader punkt
+python -m nltk.downloader stopwords
+```
+To download two wordnet modules needed. Then run:
 
 ```bash
 somef configure
 ```
 
 And you will be asked to provide the following:
 
@@ -201,15 +212,15 @@
   -a, --auto  Automatically configure SOMEF
   -h, --help  Show this message and exit.
 ```
 
 ### Updating SOMEF
 If you update SOMEF to a newer version, we recommend you `configure` again the library (by running `somef configure`). The rationale is that different versions may rely on classifiers which may be stored in a different path. 
 
-### Run SOMEF
+## Usage
 
 ```bash
 $ somef describe --help
   SOMEF Command Line Interface
 Usage: somef describe [OPTIONS]
 
   Running the Command Line Interface
```

### Comparing `somef-0.9.3/pyproject.toml` & `somef-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/setup.py` & `somef-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/__main__.py` & `somef-0.9.4/src/somef/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import click
 from click_option_group import optgroup, RequiredMutuallyExclusiveOptionGroup, RequiredAnyOptionGroup
 
 import logging
 from . import configuration
 from .utils import constants
 from . import __version__
-from . import somef_cli
 
 
 class URLParamType(click.types.StringParamType):
     name = "url"
 
 
 @click.group(context_settings={'help_option_names': ['-h', '--help']})
@@ -149,9 +148,11 @@
     "--keep_tmp",
     "-kt",
     type=click.Path(),
     help="""SOMEF will NOT delete the temporary folder where files are stored for analysis. Files will be stored at the
     desired path"""
 )
 def describe(**kwargs):
+    # import so missing packages get installed when appropriate
+    from . import somef_cli
     somef_cli.run_cli(**kwargs)
     click.secho(f"Success", fg="green")
```

### Comparing `somef-0.9.3/src/somef/configuration.py` & `somef-0.9.4/src/somef/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
               installation=default_installation,
               citation=default_citation,
               base_uri=constants.CONF_DEFAULT_BASE_URI):
     """ Function to configure the main program"""
     import nltk
     nltk.download('wordnet')
     nltk.download('omw-1.4')
+    nltk.download('punkt')
+    nltk.download('stopwords')
 
     credentials_file = Path(
         os.getenv("SOMEF_CONFIGURATION_FILE", constants.__DEFAULT_SOMEF_CONFIGURATION_FILE__)
     ).expanduser()
     os.makedirs(str(credentials_file.parent), exist_ok=True)
 
     # if credentials_file.exists():
```

### Comparing `somef-0.9.3/src/somef/export/json_export.py` & `somef-0.9.4/src/somef/export/json_export.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/export/turtle_export.py` & `somef-0.9.4/src/somef/export/turtle_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                                 else:
                                     out[key] = [obj[constants.PROP_RESULT][constants.PROP_VALUE] for obj in value]
                             except:
                                 logging.warning("Error when converting field in RDF: " + key)
                 # if it is not a list, just get the excerpt
                 else:
                     out[key] = value[constants.PROP_RESULT][constants.PROP_VALUE]
-        # print(out)
+        print(out)
         return out
 
     @staticmethod
     def apply_mapping(mapping_path, data_path) -> Graph:
         """
         Given a mapping file and a data file, this method returns the MORPH-KGC materialization for the mapping
         Parameters
```

### Comparing `somef-0.9.3/src/somef/extract_ontologies.py` & `somef-0.9.4/src/somef/extract_ontologies.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/header_analysis.py` & `somef-0.9.4/src/somef/header_analysis.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/mapping/rml.ttl` & `somef-0.9.4/src/somef/mapping/rml.ttl`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/mapping/yarrrml.yml` & `somef-0.9.4/src/somef/mapping/yarrrml.yml`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/models/citation.p` & `somef-0.9.4/src/somef/models/citation.p`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/models/deprecated/citation.sk` & `somef-0.9.4/src/somef/models/deprecated/citation.sk`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/models/deprecated/description.sk` & `somef-0.9.4/src/somef/models/deprecated/description.sk`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/models/deprecated/installation.sk` & `somef-0.9.4/src/somef/models/deprecated/installation.sk`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/models/deprecated/invocation.sk` & `somef-0.9.4/src/somef/models/deprecated/invocation.sk`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/models/description.p` & `somef-0.9.4/src/somef/models/description.p`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/models/installation.p` & `somef-0.9.4/src/somef/models/installation.p`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/models/invocation.p` & `somef-0.9.4/src/somef/models/invocation.p`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/parser/create_excerpts.py` & `somef-0.9.4/src/somef/parser/create_excerpts.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/parser/mardown_parser.py` & `somef-0.9.4/src/somef/parser/mardown_parser.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/process_files.py` & `somef-0.9.4/src/somef/process_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 import re
 import urllib
 from .utils import constants, markdown_utils
-from . import extract_ontologies
+from . import extract_ontologies,extract_workflows
 from .process_results import Result
 from chardet import detect
 
 
 def process_repository_files(repo_dir, metadata_result: Result, repo_type, owner="", repo_name="",
                              repo_default_branch=""):
     """
@@ -146,15 +146,23 @@
                                                  repo_relative_path, filename)
                         metadata_result.add_result(constants.CAT_ONTOLOGIES,
                                                    {
                                                        constants.PROP_VALUE: onto_url,
                                                        constants.PROP_TYPE: constants.URL
                                                    }, 1, constants.TECHNIQUE_FILE_EXPLORATION
                                                    )
-
+                if filename.endswith(".ga") or filename.endswith(".cwl") or filename.endswith(".nf") or (filename.endswith(".snake") or filename.endswith(".smk")  or "Snakefile"==filename_no_ext) or filename.endswith(".knwf") or filename.endswith(".t2flow") or filename.endswith(".dag") or filename.endswith(".kar") or filename.endswith(".wdl"):
+                    analysis = extract_workflows.is_file_workflow(os.path.join(repo_dir, file_path))
+                    if analysis == True:
+                        Workflow_url=get_file_link(repo_type,file_path,owner,repo_name,repo_default_branch,repo_dir,repo_relative_path,filename) 
+                        metadata_result.add_result(constants.CAT_WORKFLOWS,
+                                                    {
+                                                        constants.PROP_VALUE: Workflow_url,
+                                                        constants.PROP_TYPE: constants.URL
+                                                    }, 1, constants.TECHNIQUE_FILE_EXPLORATION)
             # TO DO: Improve this a bit, as just returning the docs folder is not that informative
             for dir_name in dir_names:
                 if dir_name.lower() == "docs":
                     if repo_relative_path == ".":
                         docs_path = dir_name
                     else:
                         if repo_relative_path.find("\\") >= 0:
```

### Comparing `somef-0.9.3/src/somef/process_repository.py` & `somef-0.9.4/src/somef/process_repository.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/process_results.py` & `somef-0.9.4/src/somef/process_results.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/regular_expressions.py` & `somef-0.9.4/src/somef/regular_expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,29 +183,50 @@
                                            constants.PROP_TYPE: constants.URL,
                                            constants.PROP_VALUE: "https://www.repostatus.org/#" + short_status,
                                            constants.PROP_DESCRIPTION: repo_status
                                        }, 1, constants.TECHNIQUE_REGULAR_EXPRESSION, readme_source)
     return repository_metadata
 
 
-def extract_arxiv_links(unfiltered_text):
-    """Extracts arxiv links from a given text"""
+def extract_arxiv_links(unfiltered_text,repository_metadata: Result, readme_source) -> Result:
+    """
+    Regexp to extract arxiv url from a repository
+    Parameters
+    ----------
+    @param unfiltered_text: repo text
+    @param repository_metadata: Result with the extractions so far
+    @param readme_source: url to the file used (for provenance)
+
+    Returns
+    -------
+    @returns a Result including the arxiv url 
+    """
     result_links = [m.start() for m in re.finditer('https://arxiv.org/', unfiltered_text)]
     result_refs = [m.start() for m in re.finditer('arXiv:', unfiltered_text)]
     results = []
     for position in result_links:
-        end = unfiltered_text.find(')', position)
+        end = unfiltered_text.find(')',position)
+        if end < 0:
+            end = unfiltered_text.find('}',position)
         link = unfiltered_text[position:end]
         results.append(link)
     for position in result_refs:
         end = unfiltered_text.find('}', position)
         link = unfiltered_text[position:end]
         results.append(link.replace('arXiv:', 'https://arxiv.org/abs/'))
 
-    return results
+    for link in set(results):
+        repository_metadata.add_result(constants.CAT_RELATED_PAPERS,
+                                        {
+                                            constants.PROP_TYPE: constants.URL,
+                                            constants.PROP_VALUE: link
+                                        },
+                                        1, constants.TECHNIQUE_REGULAR_EXPRESSION, readme_source
+                                    )
+    return repository_metadata
 
 
 def extract_wiki_links(unfiltered_text, repo_url, repository_metadata: Result, readme_source) -> Result:
     """
 
     Parameters
     ----------
```

### Comparing `somef-0.9.3/src/somef/rolf/models/audio.sav` & `somef-0.9.4/src/somef/rolf/models/audio.sav`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/rolf/models/computer_vision.sav` & `somef-0.9.4/src/somef/rolf/models/computer_vision.sav`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/rolf/models/graphs.sav` & `somef-0.9.4/src/somef/rolf/models/graphs.sav`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/rolf/models/natural_language_processing.sav` & `somef-0.9.4/src/somef/rolf/models/natural_language_processing.sav`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/rolf/models/reinforcement_learning.sav` & `somef-0.9.4/src/somef/rolf/models/reinforcement_learning.sav`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/rolf/models/semantic_web.sav` & `somef-0.9.4/src/somef/rolf/models/semantic_web.sav`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/rolf/models_test/astrophysics.sav` & `somef-0.9.4/src/somef/rolf/models_test/astrophysics.sav`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/rolf/models_test/sequential.sav` & `somef-0.9.4/src/somef/rolf/models_test/sequential.sav`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/rolf/preprocessing.py` & `somef-0.9.4/src/somef/rolf/preprocessing.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/somef_cli.py` & `somef-0.9.4/src/somef/somef_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
             repository_metadata = regular_expressions.extract_support_channels(unfiltered_text, repository_metadata,
                                                                                readme_source)
             repository_metadata = regular_expressions.extract_package_distributions(unfiltered_text,
                                                                                     repository_metadata,
                                                                                     readme_source)
             repository_metadata = regular_expressions.extract_images(unfiltered_text, repo_url, local_repo,
                                                                      repository_metadata, readme_source, def_branch)
+            repository_metadata = regular_expressions.extract_arxiv_links(unfiltered_text,repository_metadata,readme_source)
             logging.info("Completed extracting regular expressions")
             return repository_metadata
 
     except Exception as e:
         logging.error("Error processing repository " + str(e))
         return repository_metadata
```

### Comparing `somef-0.9.3/src/somef/supervised_classification.py` & `somef-0.9.4/src/somef/supervised_classification.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/test/test_JSON_export.py` & `somef-0.9.4/src/somef/test/test_JSON_export.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/test/test_cli.py` & `somef-0.9.4/src/somef/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/test/test_extract_ontologies.py` & `somef-0.9.4/src/somef/test/test_extract_ontologies.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/test/test_header_analysis.py` & `somef-0.9.4/src/somef/test/test_header_analysis.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/test/test_parser_somef.py` & `somef-0.9.4/src/somef/test/test_parser_somef.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/test/test_process_repository.py` & `somef-0.9.4/src/somef/test/test_process_repository.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/test/test_process_results.py` & `somef-0.9.4/src/somef/test/test_process_results.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/test/test_regular_expressions.py` & `somef-0.9.4/src/somef/test/test_regular_expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,21 +171,39 @@
             test_text = data_file.read()
             results = regular_expressions.extract_images(test_text, repo_url, None, Result(),
                                                          test_data_path + "test_issue_images.txt", "main")
             img = results.results[constants.CAT_IMAGE]
             print(img)
             assert len(img) == 2
 
-    # Test commented out because arxiv links with no context has demonstrated not to be useful
-    # def test_issue_181(self):
-    #     """Test designed to check if arxiv papers are detected"""
-    #     with open(test_data_path + "test_issue_181.txt", "r") as data_file:
-    #         test_text = data_file.read()
-    #         arxiv_links = regular_expressions.extract_arxiv_links(test_text)
-    #         assert len(arxiv_links) > 0
+    #Test commented out because arxiv links with no context has demonstrated not to be useful
+    def test_issue_181(self):
+        """Test designed to check if arxiv papers are detected"""
+        with open(test_data_path + "test_issue_181.txt", "r") as data_file:
+            test_text = data_file.read()
+            result = regular_expressions.extract_arxiv_links(test_text, Result(), test_data_path + "test_issue_181.txt")
+            arxiv_urls = result.results[constants.CAT_RELATED_PAPERS]
+            assert len(arxiv_urls) > 0
+    def test_issue_181_2(self):
+        """Test designed to check if arxiv papers are detected"""
+        with open(test_data_path + "test_issue_181_2.txt", "r") as data_file:
+            test_text = data_file.read()
+            result = regular_expressions.extract_arxiv_links(test_text, Result(), test_data_path + "test_issue_181_2.txt")
+            arxiv_url = result.results[constants.CAT_RELATED_PAPERS][0]['result']['value']
+            expected_result = "https://arxiv.org/abs/2203.01044"
+            self.assertEquals(expected_result,arxiv_url)
+    def test_issue_181_3(self):
+        """Test to test arxiv as embedded url, including same in bibtex"""
+        with open(test_data_path + "test_issue_181_3.txt", "r") as data_file:
+            test_text = data_file.read()
+            result = regular_expressions.extract_arxiv_links(test_text, Result(),
+                                                             test_data_path + "test_issue_181_3.txt")
+            arxiv_url = result.results[constants.CAT_RELATED_PAPERS][0]['result']['value']
+            expected_result = "https://arxiv.org/abs/1907.11111"
+            self.assertEquals(expected_result, arxiv_url)
 
     def test_issue_270(self):
         """Test designed to check if support channels are detected"""
         with open(test_data_path + "test_issue_270.txt", "r") as data_file:
             test_text = data_file.read()
             support_channels = regular_expressions.extract_support_channels(test_text, Result(),
                                                                             test_data_path + "test_issue_270.txt")
```

### Comparing `somef-0.9.3/src/somef/test/test_supervised_classification.py` & `somef-0.9.4/src/somef/test/test_supervised_classification.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/test/test_turtle_export.py` & `somef-0.9.4/src/somef/test/test_turtle_export.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef/utils/constants.py` & `somef-0.9.4/src/somef/utils/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,22 +65,24 @@
 CAT_NAME = "name"
 CAT_ONTOLOGIES = "ontologies"
 CAT_OWNER = "owner"
 CAT_PACKAGE_DISTRIBUTION = "package_distribution"
 CAT_PROGRAMMING_LANGUAGES = "programming_languages"
 CAT_README_URL = "readme_url"
 CAT_RELATED_DOCUMENTATION = "related_documentation"
+CAT_RELATED_PAPERS = "related_papers"
 CAT_RELEASES = "releases"
 CAT_RUN = "run"
 CAT_STATUS = "repository_status"
 CAT_REQUIREMENTS = "requirements"
 CAT_STARS = "stargazers_count"
 CAT_SUPPORT = "support"
 CAT_SUPPORT_CHANNELS = "support_channels"
 CAT_USAGE = "usage"
+CAT_WORKFLOWS = "workflows"
 
 # Special category: missing categories
 CAT_MISSING = "somef_missing_categories"
 
 # list of those categories to be analyzed with supervised classification.
 # supervised_categories = [CAT_DESCRIPTION, CAT_CITATION, CAT_INSTALLATION, CAT_INVOCATION]
 supervised_categories = [CAT_DESCRIPTION, CAT_INSTALLATION, CAT_INVOCATION]
```

### Comparing `somef-0.9.3/src/somef/utils/markdown_utils.py` & `somef-0.9.4/src/somef/utils/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `somef-0.9.3/src/somef.egg-info/PKG-INFO` & `somef-0.9.4/src/somef.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somef
-Version: 0.9.3
+Version: 0.9.4
 Summary: SOftware Metadata Extraction Framework: A tool for automatically extracting relevant software information from readme files
 Home-page: https://github.com/KnowledgeCaptureAndDiscovery/somef
 Author: Daniel Garijo
 Author-email: daniel.garijo@upm.es
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
@@ -18,14 +18,16 @@
 # Software Metadata Extraction Framework (SOMEF) 
 [![Python](https://img.shields.io/pypi/pyversions/somef.svg?style=plastic)](https://badge.fury.io/py/somef) [![PyPI](https://badge.fury.io/py/somef.svg)](https://badge.fury.io/py/somef) [![DOI](https://zenodo.org/badge/190487675.svg)](https://zenodo.org/badge/latestdoi/190487675) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/KnowledgeCaptureAndDiscovery/somef/HEAD?filepath=notebook%2FSOMEF%20Usage%20Example.ipynb)  [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 
 <img src="docs/logo.png" alt="logo" width="150"/>
 
 A command line interface for automatically extracting relevant information from readme files.
 
+**Demo:** See a [demo running somef as a service](https://somef.linkeddata.es), through the [SOMEF-Vider tool](https://github.com/SoftwareUnderstanding/SOMEF-Vider/). 
+
 **Authors:** Daniel Garijo, Allen Mao, Miguel Ángel García Delgado, Haripriya Dharmala, Vedant Diwanji, Jiaying Wang, Aidan Kelley and Jenifer Tabita Ciuciu-Kiss.
 
 ## Features
 Given a readme file (or a GitHub/Gitlab repository) SOMEF will extract the following categories (if present):
 
 - **Name**: Name identifying a software component
 - **Full name**: Name + owner (owner/name)
@@ -63,14 +65,16 @@
 - **Code of Conduct**: Link to the code of conduct of the project
 - **Scripts**: Snippets of code contained in the repository.
 - **Support channels**: Help channels one can use to get support about the target software component.
 - **Images**: Images used to illustrate the software component.
 - **Logo**: Main logo used to represent the target software component.
 - **Ontologies**: URL and path to the ontology files present in the repository.
 - **Application domain**: The application domain of the repository. Current supported domains include: Astrophisics, Audio, Computer vision, Graphs, Natural language processing, Reinforcement learning, Semantc web, Sequential. Domains are not mutually exclusive. These domains have been extracted from [awesome lists](https://github.com/topics/awesome-list) and [Papers with code](https://paperswithcode.com/). Find more information in our [documentation](https://somef.readthedocs.io/en/latest/).
+- **Workflows**: URL and path to the workflow files present in the repository.
+- **Related papers**: URL to possible related papers within the repository stated within the readme file.
 
 
 We use different supervised classifiers, header analysis, regular expressions and the GitHub/Gitlab API to retrieve all these fields (more than one technique may be used for each field). Each extraction records its provenance, with the confidence and technique used on each step. For more information check the [output format description](https://somef.readthedocs.io/en/latest/output/)
 
 ## Documentation
 See full documentation at [https://somef.readthedocs.io/en/latest/](https://somef.readthedocs.io/en/latest/)
 
@@ -179,17 +183,24 @@
 
 ```bash
 docker run -it --rm -v $PWD/:/out kcapd/somef /bin/bash
 ```
 If you move any files produced by somef into `/out`, then you will be able to see them in your current directory.
 
 
-## Usage
+## Configure
 
-Before running SOMEF for the first time, you must **configure** it appropriately (you only need to do this once). Run
+Before running SOMEF for the first time, you must **configure** it appropriately (you only need to do this once). Run:
+```bash
+python -m nltk.downloader wordnet
+python -m nltk.downloader omw-1.4
+python -m nltk.downloader punkt
+python -m nltk.downloader stopwords
+```
+To download two wordnet modules needed. Then run:
 
 ```bash
 somef configure
 ```
 
 And you will be asked to provide the following:
 
@@ -218,15 +229,15 @@
   -a, --auto  Automatically configure SOMEF
   -h, --help  Show this message and exit.
 ```
 
 ### Updating SOMEF
 If you update SOMEF to a newer version, we recommend you `configure` again the library (by running `somef configure`). The rationale is that different versions may rely on classifiers which may be stored in a different path. 
 
-### Run SOMEF
+## Usage
 
 ```bash
 $ somef describe --help
   SOMEF Command Line Interface
 Usage: somef describe [OPTIONS]
 
   Running the Command Line Interface
```

### Comparing `somef-0.9.3/src/somef.egg-info/SOURCES.txt` & `somef-0.9.4/src/somef.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.py
 src/somef/__init__.py
 src/somef/__main__.py
 src/somef/configuration.py
 src/somef/extract_ontologies.py
+src/somef/extract_workflows.py
 src/somef/header_analysis.py
 src/somef/process_files.py
 src/somef/process_repository.py
 src/somef/process_results.py
 src/somef/regular_expressions.py
 src/somef/somef_cli.py
 src/somef/supervised_classification.py
@@ -49,14 +50,15 @@
 src/somef/rolf/models_test/rationale.md
 src/somef/rolf/models_test/sequential.sav
 src/somef/test/__init__.py
 src/somef/test/test_JSON_export.py
 src/somef/test/test_cli.py
 src/somef/test/test_configuration.py
 src/somef/test/test_extract_ontologies.py
+src/somef/test/test_extract_workflows.py
 src/somef/test/test_header_analysis.py
 src/somef/test/test_parser_somef.py
 src/somef/test/test_process_repository.py
 src/somef/test/test_process_results.py
 src/somef/test/test_regular_expressions.py
 src/somef/test/test_supervised_classification.py
 src/somef/test/test_turtle_export.py
```

