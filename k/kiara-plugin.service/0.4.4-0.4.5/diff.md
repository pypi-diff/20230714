# Comparing `tmp/kiara_plugin.service-0.4.4.tar.gz` & `tmp/kiara_plugin.service-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.service-0.4.4.tar", last modified: Thu Jul 13 10:57:10 2023, max compression
+gzip compressed data, was "kiara_plugin.service-0.4.5.tar", last modified: Fri Jul 14 12:09:09 2023, max compression
```

## Comparing `kiara_plugin.service-0.4.4.tar` & `kiara_plugin.service-0.4.5.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/ci/conda/kiara_plugin.service/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/ci/conda/kiara_plugin.service/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/pipelines/example_pipeline_service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   171640 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/kiara_import.profile
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/service/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/context_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/input.css
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/main.css
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/simple.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/operations/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/operations/operation_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/operations/operations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/table.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/value_select.html
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/value_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/values.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:56:43.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/tailwind.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/ci/conda/kiara_plugin.service/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/ci/conda/kiara_plugin.service/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/pipelines/example_pipeline_service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   171640 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/kiara_import.profile
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/service/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/context_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/input.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/simple.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/operations/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/operations/operation_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/operations/operations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/value_select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/value_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/values.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:08:39.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/tailwind.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.service-0.4.4/.cruft.json` & `kiara_plugin.service-0.4.5/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.service-0.4.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.service-0.4.5/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/.github/workflows/build-darwin.yaml` & `kiara_plugin.service-0.4.5/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/.github/workflows/build-linux.yaml` & `kiara_plugin.service-0.4.5/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/.github/workflows/build-windows.yaml` & `kiara_plugin.service-0.4.5/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/.gitignore` & `kiara_plugin.service-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/.pre-commit-config.yaml` & `kiara_plugin.service-0.4.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/LICENSE` & `kiara_plugin.service-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/Makefile` & `kiara_plugin.service-0.4.5/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/PKG-INFO` & `kiara_plugin.service-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.service
-Version: 0.4.4
+Version: 0.4.5
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
```

### Comparing `kiara_plugin.service-0.4.4/README.md` & `kiara_plugin.service-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/ci/conda/kiara_plugin.service/meta.yaml.template` & `kiara_plugin.service-0.4.5/ci/conda/kiara_plugin.service/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/docs/development.md` & `kiara_plugin.service-0.4.5/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/docs/index.md` & `kiara_plugin.service-0.4.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.service-0.4.5/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.service-0.4.5/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/examples/pipelines/example_pipeline_service.yaml` & `kiara_plugin.service-0.4.5/examples/pipelines/example_pipeline_service.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/kiara_import.profile` & `kiara_plugin.service-0.4.5/kiara_import.profile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/mkdocs.yml` & `kiara_plugin.service-0.4.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/pyproject.toml` & `kiara_plugin.service-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.service-0.4.5/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/scripts/documentation/gen_info_pages.py` & `kiara_plugin.service-0.4.5/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/scripts/documentation/gen_module_doc.py` & `kiara_plugin.service-0.4.5/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/setup.cfg` & `kiara_plugin.service-0.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/setup.py` & `kiara_plugin.service-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/__init__.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/defaults.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/service/commands.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/service/commands.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/models.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/modules/__init__.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/__init__.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/__init__.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/context_info.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/context_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 
 from pydantic import BaseModel, Field
 from starlite import (
     Controller,
 )
 
 from kiara.api import KiaraAPI
-from kiara.interfaces.python_api import ModuleTypeInfo
+from kiara.interfaces.python_api import DataTypeClassInfo
 from kiara.models.runtime_environment.python import (
     PythonRuntimeEnvironment,
 )
-from kiara.models.values.value import DataTypeInfo
 from kiara.registries.environment import EnvironmentRegistry
 from kiara_plugin.service.openapi.controllers import get, post
 
 
 class DataTypeMatcher(BaseModel):
 
     filters: List[str] = Field(
@@ -27,18 +26,18 @@
         default=None,
     )
 
 
 class DataTypeControllerJson(Controller):
     path = "/"
 
-    @post(path="/", api_func=KiaraAPI.retrieve_module_types_info)
+    @post(path="/", api_func=KiaraAPI.retrieve_data_types_info)
     async def list_data_types(
         self, kiara_api: KiaraAPI, data: DataTypeMatcher
-    ) -> Dict[str, DataTypeInfo]:
+    ) -> Dict[str, DataTypeClassInfo]:
 
         filters = data.filters
         python_package = data.python_package
 
         data_types = kiara_api.retrieve_data_types_info(
             filter=filters, python_package=python_package
         )
@@ -47,21 +46,21 @@
     @get(path="/type_names", api_func=KiaraAPI.list_module_type_names)
     async def list_module_type_names(self, kiara_api: KiaraAPI) -> List[str]:
         """List the ids of all available operations."""
 
         module_names = kiara_api.list_module_type_names()
         return module_names
 
-    @get(path="/{module_type_name:str}", api_func=KiaraAPI.retrieve_module_type_info)
+    @get(path="/{data_type_name:str}", api_func=KiaraAPI.retrieve_data_type_info)
     async def get_module_type_info(
-        self, kiara_api: KiaraAPI, module_type_name: str
-    ) -> ModuleTypeInfo:
+        self, kiara_api: KiaraAPI, data_type_name: str
+    ) -> DataTypeClassInfo:
 
-        module = kiara_api.retrieve_module_type_info(module_type=module_type_name)
-        return module
+        data_type = kiara_api.retrieve_data_type_info(data_type_name=data_type_name)
+        return data_type
 
 
 class KiaraContextControllerJson(Controller):
 
     path = "/"
 
     @get(path="/installed_plugins")
```

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/jobs.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/jobs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/modules.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/modules.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/operations.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,22 @@
         description="Whether to include internal operations in the result.",
         default=False,
     )
     python_package: Union[str, None] = Field(
         description="If specified, only operations that are contained in this Python package are returned.",
         default=None,
     )
+    input_types: List[str] = Field(
+        description="each operation must have at least one input that matches one of the specified types",
+        default_factory=list,
+    )
+    output_types: List[str] = Field(
+        description="each operation must have at least one output that matches one of the specified types",
+        default_factory=list,
+    )
 
 
 class OperationControllerJson(Controller):
     path = "/"
 
     @post(path="/", api_func=KiaraAPI.retrieve_operations_info)
     async def list_operations(
```

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/pipeline.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/render.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/render.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/values.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/values.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/workflows.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/workflows.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/service.py` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/service.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/favicon.ico` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/main.css` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/main.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/simple.css` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/simple.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/jobs/job_finished.html` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/jobs/job_finished.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/macros.html` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/macros.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html` & `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/PKG-INFO` & `kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.service
-Version: 0.4.4
+Version: 0.4.5
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
```

### Comparing `kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/SOURCES.txt` & `kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/tests/conftest.py` & `kiara_plugin.service-0.4.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.4/tests/test_job_descs.py` & `kiara_plugin.service-0.4.5/tests/test_job_descs.py`

 * *Files identical despite different names*

