# Comparing `tmp/kiara_plugin.service-0.4.5.tar.gz` & `tmp/kiara_plugin.service-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.service-0.4.5.tar", last modified: Fri Jul 14 12:09:09 2023, max compression
+gzip compressed data, was "kiara_plugin.service-0.4.6.tar", last modified: Fri Jul 14 14:13:20 2023, max compression
```

## Comparing `kiara_plugin.service-0.4.5.tar` & `kiara_plugin.service-0.4.6.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/ci/conda/kiara_plugin.service/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/ci/conda/kiara_plugin.service/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/examples/pipelines/example_pipeline_service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   171640 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/kiara_import.profile
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.178070 kiara_plugin.service-0.4.5/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.174070 kiara_plugin.service-0.4.5/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/service/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/context_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/input.css
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/main.css
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/simple.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/operations/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/operations/operation_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/operations/operations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/table.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/value_select.html
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/value_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/values.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.182070 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:08:39.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 12:09:09.000000 kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/tailwind.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:09:09.186070 kiara_plugin.service-0.4.5/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-07-14 12:08:28.000000 kiara_plugin.service-0.4.5/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/ci/conda/kiara_plugin.service/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/ci/conda/kiara_plugin.service/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/pipelines/example_pipeline_service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   171640 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/kiara_import.profile
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/service/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/context_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/input.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/simple.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/operations/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/operations/operation_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/operations/operations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/value_select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/value_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/values.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:12:53.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/tailwind.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.service-0.4.5/.cruft.json` & `kiara_plugin.service-0.4.6/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.service-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.service-0.4.6/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/.github/workflows/build-darwin.yaml` & `kiara_plugin.service-0.4.6/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/.github/workflows/build-linux.yaml` & `kiara_plugin.service-0.4.6/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/.github/workflows/build-windows.yaml` & `kiara_plugin.service-0.4.6/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/.gitignore` & `kiara_plugin.service-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/.pre-commit-config.yaml` & `kiara_plugin.service-0.4.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/LICENSE` & `kiara_plugin.service-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/Makefile` & `kiara_plugin.service-0.4.6/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/PKG-INFO` & `kiara_plugin.service-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.service
-Version: 0.4.5
+Version: 0.4.6
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
```

### Comparing `kiara_plugin.service-0.4.5/README.md` & `kiara_plugin.service-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/ci/conda/kiara_plugin.service/meta.yaml.template` & `kiara_plugin.service-0.4.6/ci/conda/kiara_plugin.service/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/docs/development.md` & `kiara_plugin.service-0.4.6/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/docs/index.md` & `kiara_plugin.service-0.4.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.service-0.4.6/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.service-0.4.6/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/examples/pipelines/example_pipeline_service.yaml` & `kiara_plugin.service-0.4.6/examples/pipelines/example_pipeline_service.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/kiara_import.profile` & `kiara_plugin.service-0.4.6/kiara_import.profile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/mkdocs.yml` & `kiara_plugin.service-0.4.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/pyproject.toml` & `kiara_plugin.service-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.service-0.4.6/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/scripts/documentation/gen_info_pages.py` & `kiara_plugin.service-0.4.6/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/scripts/documentation/gen_module_doc.py` & `kiara_plugin.service-0.4.6/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/setup.cfg` & `kiara_plugin.service-0.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/setup.py` & `kiara_plugin.service-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/__init__.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/defaults.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/interfaces/cli/service/commands.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/service/commands.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/models.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/modules/__init__.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/__init__.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/__init__.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/context_info.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/context_info.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/jobs.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/jobs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/modules.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/modules.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/operations.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,19 @@
 
         if data.python_package is not None:
             python_packages = [data.python_package]
         else:
             python_packages = None
 
         operations = kiara_api.retrieve_operations_info(
-            *filters, include_internal=include_internal, python_packages=python_packages
+            *filters,
+            include_internal=include_internal,
+            python_packages=python_packages,
+            input_types=data.input_types,
+            output_types=data.output_types
         )
         return operations.item_infos  # type: ignore
 
     @post(path="/ids", api_func=KiaraAPI.list_operation_ids)
     async def list_operation_ids(
         self, kiara_api: KiaraAPI, data: OperationMatcher
     ) -> List[str]:
@@ -89,14 +93,16 @@
         else:
             python_packages = None
 
         operation_ids = kiara_api.list_operation_ids(
             filter=filters,
             include_internal=include_internal,
             python_packages=python_packages,
+            input_types=data.input_types,
+            output_types=data.output_types,
         )
         return operation_ids
 
     @get(path="/{operation_id:str}", api_func=KiaraAPI.retrieve_operation_info)
     async def get_operation_info(
         self, kiara_api: KiaraAPI, operation_id: str
     ) -> OperationInfo:
```

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/pipeline.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/render.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/render.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/values.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/values.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/controllers/workflows.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/workflows.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/openapi/service.py` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/service.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/favicon.ico` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/main.css` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/main.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/static/simple.css` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/simple.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/jobs/job_finished.html` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/jobs/job_finished.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/macros.html` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/macros.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html` & `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/PKG-INFO` & `kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.service
-Version: 0.4.5
+Version: 0.4.6
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
```

### Comparing `kiara_plugin.service-0.4.5/src/kiara_plugin.service.egg-info/SOURCES.txt` & `kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/tests/conftest.py` & `kiara_plugin.service-0.4.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.5/tests/test_job_descs.py` & `kiara_plugin.service-0.4.6/tests/test_job_descs.py`

 * *Files identical despite different names*

