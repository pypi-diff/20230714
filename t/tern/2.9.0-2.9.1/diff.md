# Comparing `tmp/tern-2.9.0.tar.gz` & `tmp/tern-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tern-2.9.0.tar", last modified: Thu Dec 16 05:51:53 2021, max compression
+gzip compressed data, was "tern-2.9.1.tar", last modified: Fri Jan 21 23:21:08 2022, max compression
```

## Comparing `tern-2.9.0.tar` & `tern-2.9.1.tar`

### file list

```diff
@@ -1,250 +1,252 @@
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.362887 tern-2.9.0/
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.330887 tern-2.9.0/.devcontainer/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      442 2021-12-16 03:47:49.000000 tern-2.9.0/.devcontainer/Dockerfile
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      541 2021-12-16 03:47:49.000000 tern-2.9.0/.devcontainer/devcontainer.json
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)       18 2021-12-16 03:47:49.000000 tern-2.9.0/.gitattributes
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.322887 tern-2.9.0/.github/
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.330887 tern-2.9.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      737 2021-12-16 03:47:49.000000 tern-2.9.0/.github/ISSUE_TEMPLATE/bug.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      400 2021-12-16 03:47:49.000000 tern-2.9.0/.github/ISSUE_TEMPLATE/feature.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      383 2021-12-16 03:47:49.000000 tern-2.9.0/.github/ISSUE_TEMPLATE/proposal.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      187 2021-12-16 03:47:49.000000 tern-2.9.0/.github/ISSUE_TEMPLATE/question.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      315 2021-12-16 03:47:49.000000 tern-2.9.0/.github/ISSUE_TEMPLATE/task.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      377 2021-12-16 03:47:49.000000 tern-2.9.0/.github/ISSUE_TEMPLATE/tinytask.md
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.330887 tern-2.9.0/.github/workflows/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2736 2021-12-16 03:47:49.000000 tern-2.9.0/.github/workflows/pull_request.yml
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      396 2021-12-16 03:47:49.000000 tern-2.9.0/.prospector.yaml
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.330887 tern-2.9.0/.vscode/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)       46 2021-12-16 03:47:49.000000 tern-2.9.0/.vscode/extensions.json
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      423 2021-12-16 03:47:49.000000 tern-2.9.0/.vscode/launch.json
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      141 2021-12-16 03:47:49.000000 tern-2.9.0/.vscode/tasks.json
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3110 2021-12-16 05:51:53.000000 tern-2.9.0/AUTHORS
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3241 2021-12-16 03:47:49.000000 tern-2.9.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    17636 2021-12-16 03:47:49.000000 tern-2.9.0/CONTRIBUTING.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    43528 2021-12-16 05:51:53.000000 tern-2.9.0/ChangeLog
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3104 2021-12-16 03:47:49.000000 tern-2.9.0/GOVERNANCE.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1489 2021-12-16 03:47:49.000000 tern-2.9.0/LICENSE.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      463 2021-12-16 03:47:49.000000 tern-2.9.0/MAINTAINERS.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      125 2021-12-16 03:47:49.000000 tern-2.9.0/MANIFEST.in
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      456 2021-12-16 03:47:49.000000 tern-2.9.0/NOTICE.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    29418 2021-12-16 05:51:53.362887 tern-2.9.0/PKG-INFO
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    25289 2021-12-16 05:51:18.000000 tern-2.9.0/README.md
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.330887 tern-2.9.0/docker/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      814 2021-12-16 03:47:49.000000 tern-2.9.0/docker/Dockerfile
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      982 2021-12-16 03:47:49.000000 tern-2.9.0/docker/Dockerfile.scancode
--rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)      593 2021-12-16 03:47:49.000000 tern-2.9.0/docker_run.sh
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.334887 tern-2.9.0/docs/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    14872 2021-12-16 03:47:49.000000 tern-2.9.0/docs/adding-to-command-library.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     8260 2021-12-16 03:47:49.000000 tern-2.9.0/docs/architecture.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7176 2021-12-16 03:47:49.000000 tern-2.9.0/docs/creating-custom-templates.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3575 2021-12-16 03:47:49.000000 tern-2.9.0/docs/creating-tool-extensions.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1415 2021-12-16 03:47:49.000000 tern-2.9.0/docs/data-model.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1505 2021-12-16 03:47:49.000000 tern-2.9.0/docs/faq.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1534 2021-12-16 03:47:49.000000 tern-2.9.0/docs/glossary.md
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.342887 tern-2.9.0/docs/img/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    69697 2021-12-16 03:47:49.000000 tern-2.9.0/docs/img/arch.png
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)   153745 2021-12-16 03:47:49.000000 tern-2.9.0/docs/img/tern_data_model.png
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)  3016831 2021-12-16 03:47:49.000000 tern-2.9.0/docs/img/tern_demo_fast.gif
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    30862 2021-12-16 03:47:49.000000 tern-2.9.0/docs/img/tern_flow.png
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5059 2021-12-16 03:47:49.000000 tern-2.9.0/docs/img/tern_logo.png
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6150 2021-12-16 03:47:49.000000 tern-2.9.0/docs/navigating-the-code.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4396 2021-12-16 05:51:18.000000 tern-2.9.0/docs/project-roadmap-archive.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      726 2021-12-16 05:51:18.000000 tern-2.9.0/docs/project-roadmap.md
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.346887 tern-2.9.0/docs/releases/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4243 2021-12-16 05:51:18.000000 tern-2.9.0/docs/releases/release_checklist.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1457 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v0_1_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9564 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v0_2_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3572 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v0_3_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10431 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v0_4_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      428 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v0_5_0-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6690 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v0_5_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      428 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v0_5_4-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      463 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v0_5_4.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3282 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v1_0_0-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7232 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v1_0_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3111 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v1_0_1-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      900 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v1_0_1.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3428 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_0_0-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     8513 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_0_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4021 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_1_0-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7660 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_1_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6192 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_2_0-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7698 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_2_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7613 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_3_0-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5414 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_3_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9086 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_4_0-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4761 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_4_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10384 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_5_0-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4973 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_5_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10055 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_6_1-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5183 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_6_1.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10072 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_7_0-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3261 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_7_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10788 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_8_0-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2780 2021-12-16 03:47:49.000000 tern-2.9.0/docs/releases/v2_8_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    13844 2021-12-16 05:51:18.000000 tern-2.9.0/docs/releases/v2_9_0-requirements.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5937 2021-12-16 05:51:18.000000 tern-2.9.0/docs/releases/v2_9_0.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    13175 2021-12-16 03:47:49.000000 tern-2.9.0/docs/spdx-tag-value-mapping.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5181 2021-12-16 03:47:49.000000 tern-2.9.0/docs/spdx-tag-value-overview.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5358 2021-12-16 03:47:49.000000 tern-2.9.0/docs/tern-lab-tutorial.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2549 2021-12-16 03:47:49.000000 tern-2.9.0/docs/yaml_output.md
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      377 2021-12-16 03:47:49.000000 tern-2.9.0/requirements.in
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1123 2021-12-16 05:51:37.000000 tern-2.9.0/requirements.txt
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.326887 tern-2.9.0/samples/
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.346887 tern-2.9.0/samples/alpine_python/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)       74 2021-12-16 03:47:49.000000 tern-2.9.0/samples/alpine_python/Dockerfile
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.346887 tern-2.9.0/samples/debian_vim/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      176 2021-12-16 03:47:49.000000 tern-2.9.0/samples/debian_vim/Dockerfile
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.346887 tern-2.9.0/samples/photon_3_layers/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      218 2021-12-16 03:47:49.000000 tern-2.9.0/samples/photon_3_layers/Dockerfile
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.346887 tern-2.9.0/samples/photon_git/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      176 2021-12-16 03:47:49.000000 tern-2.9.0/samples/photon_git/Dockerfile
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.346887 tern-2.9.0/samples/photon_openjre/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      180 2021-12-16 03:47:49.000000 tern-2.9.0/samples/photon_openjre/Dockerfile
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.346887 tern-2.9.0/samples/single_stage_tern/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1155 2021-12-16 03:47:49.000000 tern-2.9.0/samples/single_stage_tern/Dockerfile
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1869 2021-12-16 05:51:53.362887 tern-2.9.0/setup.cfg
--rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)      259 2021-12-16 03:47:49.000000 tern-2.9.0/setup.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.346887 tern-2.9.0/tern/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/__init__.py
--rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)    13525 2021-12-16 03:47:49.000000 tern-2.9.0/tern/__main__.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.346887 tern-2.9.0/tern/analyze/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    11035 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/common.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.346887 tern-2.9.0/tern/analyze/default/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2967 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/bundle.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7575 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/collect.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.350887 tern-2.9.0/tern/analyze/default/command_lib/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/command_lib/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    16062 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/command_lib/base.yml
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     8374 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/command_lib/command_lib.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      260 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/command_lib/common.yml
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2907 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/command_lib/snippets.yml
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.350887 tern-2.9.0/tern/analyze/default/container/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/container/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2927 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/container/image.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7045 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/container/multi_layer.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3038 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/container/run.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7238 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/container/single_layer.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5194 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/core.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.350887 tern-2.9.0/tern/analyze/default/debug/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/debug/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7487 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/debug/run.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6573 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/default_common.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.350887 tern-2.9.0/tern/analyze/default/dockerfile/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/dockerfile/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9467 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/dockerfile/lock.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    11829 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/dockerfile/parse.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9987 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/dockerfile/run.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4865 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/filter.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.350887 tern-2.9.0/tern/analyze/default/live/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/live/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2676 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/live/collect.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6474 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/default/live/run.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3717 2021-12-16 03:47:49.000000 tern-2.9.0/tern/analyze/passthrough.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.354887 tern-2.9.0/tern/classes/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5071 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/command.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7333 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/docker_image.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10618 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/file_data.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6847 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/image.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    13218 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/image_layer.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2152 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/notice.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2865 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/notice_origin.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5449 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/oci_image.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2024 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/origins.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9445 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/package.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1567 2021-12-16 03:47:49.000000 tern-2.9.0/tern/classes/template.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.354887 tern-2.9.0/tern/extensions/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/extensions/__init__.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.354887 tern-2.9.0/tern/extensions/cve_bin_tool/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/extensions/cve_bin_tool/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1404 2021-12-16 03:47:49.000000 tern-2.9.0/tern/extensions/cve_bin_tool/executor.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      626 2021-12-16 03:47:49.000000 tern-2.9.0/tern/extensions/executor.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.354887 tern-2.9.0/tern/extensions/scancode/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/extensions/scancode/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     8744 2021-12-16 03:47:49.000000 tern-2.9.0/tern/extensions/scancode/executor.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.354887 tern-2.9.0/tern/formats/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      564 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/consumer.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.354887 tern-2.9.0/tern/formats/cyclonedx/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      123 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/cyclonedx/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1682 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/cyclonedx/cyclonedx_common.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.354887 tern-2.9.0/tern/formats/cyclonedx/cyclonedxjson/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      123 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/cyclonedx/cyclonedxjson/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2080 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/cyclonedx/cyclonedxjson/generator.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1393 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/cyclonedx/cyclonedxjson/image_helpers.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1669 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/cyclonedx/cyclonedxjson/package_helpers.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.354887 tern-2.9.0/tern/formats/default/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/default/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5568 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/default/generator.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      463 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/generator.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.354887 tern-2.9.0/tern/formats/html/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/html/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    11845 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/html/generator.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.354887 tern-2.9.0/tern/formats/json/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/json/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2497 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/json/consumer.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      703 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/json/generator.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.358887 tern-2.9.0/tern/formats/spdx/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      863 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdx.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5741 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdx_common.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.358887 tern-2.9.0/tern/formats/spdx/spdxjson/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxjson/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3693 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxjson/consumer.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4027 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxjson/file_helpers.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1755 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxjson/formats.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6919 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxjson/generator.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3592 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxjson/image_helpers.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     8032 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxjson/layer_helpers.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3241 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxjson/package_helpers.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.358887 tern-2.9.0/tern/formats/spdx/spdxtagvalue/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxtagvalue/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3515 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxtagvalue/file_helpers.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1287 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxtagvalue/formats.py
--rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)     5063 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxtagvalue/generator.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5401 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxtagvalue/image_helpers.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5547 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxtagvalue/layer_helpers.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2535 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/spdx/spdxtagvalue/package_helpers.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.358887 tern-2.9.0/tern/formats/yaml/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/yaml/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1021 2021-12-16 03:47:49.000000 tern-2.9.0/tern/formats/yaml/generator.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.358887 tern-2.9.0/tern/load/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/load/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7648 2021-12-16 03:47:49.000000 tern-2.9.0/tern/load/docker_api.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1163 2021-12-16 03:47:49.000000 tern-2.9.0/tern/load/skopeo.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1878 2021-12-16 03:47:49.000000 tern-2.9.0/tern/prep.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.358887 tern-2.9.0/tern/report/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/report/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4436 2021-12-16 03:47:49.000000 tern-2.9.0/tern/report/content.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4937 2021-12-16 03:47:49.000000 tern-2.9.0/tern/report/errors.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3530 2021-12-16 03:47:49.000000 tern-2.9.0/tern/report/formats.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3441 2021-12-16 03:47:49.000000 tern-2.9.0/tern/report/report.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.326887 tern-2.9.0/tern/scripts/
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.358887 tern-2.9.0/tern/scripts/debian/
--rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)      364 2021-12-16 03:47:49.000000 tern-2.9.0/tern/scripts/debian/apt_get_sources.sh
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.358887 tern-2.9.0/tern/scripts/debian/jessie/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      294 2021-12-16 03:47:49.000000 tern-2.9.0/tern/scripts/debian/jessie/sources.list
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.358887 tern-2.9.0/tern/tools/
--rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)      831 2021-12-16 03:47:49.000000 tern-2.9.0/tern/tools/fs_hash.sh
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.362887 tern-2.9.0/tern/utils/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2021-12-16 03:47:49.000000 tern-2.9.0/tern/utils/__init__.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2661 2021-12-16 03:47:49.000000 tern-2.9.0/tern/utils/cache.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1320 2021-12-16 03:47:49.000000 tern-2.9.0/tern/utils/constants.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    12250 2021-12-16 03:47:49.000000 tern-2.9.0/tern/utils/general.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      285 2021-12-16 03:47:49.000000 tern-2.9.0/tern/utils/host.py
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9905 2021-12-16 03:47:49.000000 tern-2.9.0/tern/utils/rootfs.py
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.346887 tern-2.9.0/tern.egg-info/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    29418 2021-12-16 05:51:53.000000 tern-2.9.0/tern.egg-info/PKG-INFO
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5969 2021-12-16 05:51:53.000000 tern-2.9.0/tern.egg-info/SOURCES.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)        1 2021-12-16 05:51:53.000000 tern-2.9.0/tern.egg-info/dependency_links.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      667 2021-12-16 05:51:53.000000 tern-2.9.0/tern.egg-info/entry_points.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)        1 2021-12-16 03:57:59.000000 tern-2.9.0/tern.egg-info/not-zip-safe
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      449 2021-12-16 05:51:53.000000 tern-2.9.0/tern.egg-info/requires.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)        5 2021-12-16 05:51:53.000000 tern-2.9.0/tern.egg-info/top_level.txt
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      700 2021-12-16 03:47:49.000000 tern-2.9.0/tox.ini
-drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2021-12-16 05:51:53.362887 tern-2.9.0/vagrant/
--rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3493 2021-12-16 03:47:49.000000 tern-2.9.0/vagrant/Vagrantfile
--rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)     1113 2021-12-16 03:47:49.000000 tern-2.9.0/vagrant/bootstrap.sh
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.791336 tern-2.9.1/
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.747339 tern-2.9.1/.devcontainer/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      442 2022-01-21 22:40:28.000000 tern-2.9.1/.devcontainer/Dockerfile
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      541 2022-01-21 22:40:28.000000 tern-2.9.1/.devcontainer/devcontainer.json
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)       18 2022-01-21 22:40:28.000000 tern-2.9.1/.gitattributes
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.727340 tern-2.9.1/.github/
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.747339 tern-2.9.1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      737 2022-01-21 22:40:28.000000 tern-2.9.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      400 2022-01-21 22:40:28.000000 tern-2.9.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      383 2022-01-21 22:40:28.000000 tern-2.9.1/.github/ISSUE_TEMPLATE/proposal.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      187 2022-01-21 22:40:28.000000 tern-2.9.1/.github/ISSUE_TEMPLATE/question.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      315 2022-01-21 22:40:28.000000 tern-2.9.1/.github/ISSUE_TEMPLATE/task.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      377 2022-01-21 22:40:28.000000 tern-2.9.1/.github/ISSUE_TEMPLATE/tinytask.md
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.747339 tern-2.9.1/.github/workflows/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2736 2022-01-21 22:40:28.000000 tern-2.9.1/.github/workflows/pull_request.yml
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      396 2022-01-21 22:40:28.000000 tern-2.9.1/.prospector.yaml
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.747339 tern-2.9.1/.vscode/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)       46 2022-01-21 22:40:28.000000 tern-2.9.1/.vscode/extensions.json
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      423 2022-01-21 22:40:28.000000 tern-2.9.1/.vscode/launch.json
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      141 2022-01-21 22:40:28.000000 tern-2.9.1/.vscode/tasks.json
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3110 2022-01-21 23:21:08.000000 tern-2.9.1/AUTHORS
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3241 2022-01-21 22:40:28.000000 tern-2.9.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    17636 2022-01-21 22:40:28.000000 tern-2.9.1/CONTRIBUTING.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    43728 2022-01-21 23:21:08.000000 tern-2.9.1/ChangeLog
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3104 2022-01-21 22:40:28.000000 tern-2.9.1/GOVERNANCE.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1489 2022-01-21 22:40:28.000000 tern-2.9.1/LICENSE.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      463 2022-01-21 22:40:28.000000 tern-2.9.1/MAINTAINERS.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      125 2022-01-21 22:40:28.000000 tern-2.9.1/MANIFEST.in
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      456 2022-01-21 22:40:28.000000 tern-2.9.1/NOTICE.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    29418 2022-01-21 23:21:08.791336 tern-2.9.1/PKG-INFO
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    25289 2022-01-21 22:40:28.000000 tern-2.9.1/README.md
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.751339 tern-2.9.1/docker/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      814 2022-01-21 22:40:28.000000 tern-2.9.1/docker/Dockerfile
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      982 2022-01-21 22:40:28.000000 tern-2.9.1/docker/Dockerfile.scancode
+-rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)      593 2022-01-21 22:40:28.000000 tern-2.9.1/docker_run.sh
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.751339 tern-2.9.1/docs/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    14872 2022-01-21 22:40:28.000000 tern-2.9.1/docs/adding-to-command-library.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     8260 2022-01-21 22:40:28.000000 tern-2.9.1/docs/architecture.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7176 2022-01-21 22:40:28.000000 tern-2.9.1/docs/creating-custom-templates.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3575 2022-01-21 22:40:28.000000 tern-2.9.1/docs/creating-tool-extensions.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1415 2022-01-21 22:40:28.000000 tern-2.9.1/docs/data-model.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1505 2022-01-21 22:40:28.000000 tern-2.9.1/docs/faq.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1534 2022-01-21 22:40:28.000000 tern-2.9.1/docs/glossary.md
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.759338 tern-2.9.1/docs/img/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    69697 2022-01-21 22:40:28.000000 tern-2.9.1/docs/img/arch.png
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)   153745 2022-01-21 22:40:28.000000 tern-2.9.1/docs/img/tern_data_model.png
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)  3016831 2022-01-21 22:40:28.000000 tern-2.9.1/docs/img/tern_demo_fast.gif
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    30862 2022-01-21 22:40:28.000000 tern-2.9.1/docs/img/tern_flow.png
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5059 2022-01-21 22:40:28.000000 tern-2.9.1/docs/img/tern_logo.png
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6150 2022-01-21 22:40:28.000000 tern-2.9.1/docs/navigating-the-code.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4396 2022-01-21 22:40:28.000000 tern-2.9.1/docs/project-roadmap-archive.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      726 2022-01-21 22:40:28.000000 tern-2.9.1/docs/project-roadmap.md
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.767338 tern-2.9.1/docs/releases/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4243 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/release_checklist.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1457 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v0_1_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9564 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v0_2_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3572 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v0_3_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10431 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v0_4_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      428 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v0_5_0-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6690 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v0_5_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      428 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v0_5_4-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      463 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v0_5_4.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3282 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v1_0_0-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7232 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v1_0_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3111 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v1_0_1-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      900 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v1_0_1.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3428 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_0_0-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     8513 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_0_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4021 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_1_0-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7660 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_1_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6192 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_2_0-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7698 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_2_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7613 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_3_0-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5414 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_3_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9086 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_4_0-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4761 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_4_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10384 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_5_0-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4973 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_5_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10055 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_6_1-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5183 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_6_1.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10072 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_7_0-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3261 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_7_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10788 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_8_0-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2780 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_8_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    13844 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_9_0-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5937 2022-01-21 22:40:28.000000 tern-2.9.1/docs/releases/v2_9_0.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    13629 2022-01-21 23:20:32.000000 tern-2.9.1/docs/releases/v2_9_1-requirements.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      823 2022-01-21 23:20:32.000000 tern-2.9.1/docs/releases/v2_9_1.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    13175 2022-01-21 22:40:28.000000 tern-2.9.1/docs/spdx-tag-value-mapping.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5181 2022-01-21 22:40:28.000000 tern-2.9.1/docs/spdx-tag-value-overview.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5358 2022-01-21 22:40:28.000000 tern-2.9.1/docs/tern-lab-tutorial.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2549 2022-01-21 22:40:28.000000 tern-2.9.1/docs/yaml_output.md
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      377 2022-01-21 22:40:28.000000 tern-2.9.1/requirements.in
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1078 2022-01-21 23:20:40.000000 tern-2.9.1/requirements.txt
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.731340 tern-2.9.1/samples/
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.767338 tern-2.9.1/samples/alpine_python/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)       74 2022-01-21 22:40:28.000000 tern-2.9.1/samples/alpine_python/Dockerfile
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.767338 tern-2.9.1/samples/debian_vim/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      176 2022-01-21 22:40:28.000000 tern-2.9.1/samples/debian_vim/Dockerfile
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.767338 tern-2.9.1/samples/photon_3_layers/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      218 2022-01-21 22:40:28.000000 tern-2.9.1/samples/photon_3_layers/Dockerfile
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.767338 tern-2.9.1/samples/photon_git/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      176 2022-01-21 22:40:28.000000 tern-2.9.1/samples/photon_git/Dockerfile
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.767338 tern-2.9.1/samples/photon_openjre/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      180 2022-01-21 22:40:28.000000 tern-2.9.1/samples/photon_openjre/Dockerfile
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.767338 tern-2.9.1/samples/single_stage_tern/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1155 2022-01-21 22:40:28.000000 tern-2.9.1/samples/single_stage_tern/Dockerfile
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1869 2022-01-21 23:21:08.791336 tern-2.9.1/setup.cfg
+-rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)      259 2022-01-21 22:40:28.000000 tern-2.9.1/setup.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.767338 tern-2.9.1/tern/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/__init__.py
+-rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)    13525 2022-01-21 22:40:28.000000 tern-2.9.1/tern/__main__.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.771338 tern-2.9.1/tern/analyze/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    11035 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/common.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.771338 tern-2.9.1/tern/analyze/default/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2967 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/bundle.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7575 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/collect.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.771338 tern-2.9.1/tern/analyze/default/command_lib/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/command_lib/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    16062 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/command_lib/base.yml
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     8374 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/command_lib/command_lib.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      260 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/command_lib/common.yml
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2907 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/command_lib/snippets.yml
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.771338 tern-2.9.1/tern/analyze/default/container/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/container/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2927 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/container/image.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7045 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/container/multi_layer.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3038 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/container/run.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7238 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/container/single_layer.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5194 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/core.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.775337 tern-2.9.1/tern/analyze/default/debug/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/debug/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7487 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/debug/run.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6573 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/default_common.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.775337 tern-2.9.1/tern/analyze/default/dockerfile/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/dockerfile/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9467 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/dockerfile/lock.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    11829 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/dockerfile/parse.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9987 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/dockerfile/run.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4865 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/filter.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.775337 tern-2.9.1/tern/analyze/default/live/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/live/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2676 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/live/collect.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6474 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/default/live/run.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3717 2022-01-21 22:40:28.000000 tern-2.9.1/tern/analyze/passthrough.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.775337 tern-2.9.1/tern/classes/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5071 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/command.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7333 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/docker_image.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    10618 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/file_data.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6847 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/image.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    14728 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/image_layer.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2152 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/notice.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2865 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/notice_origin.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5413 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/oci_image.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2024 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/origins.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9445 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/package.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1567 2022-01-21 22:40:28.000000 tern-2.9.1/tern/classes/template.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.775337 tern-2.9.1/tern/extensions/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/extensions/__init__.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.779337 tern-2.9.1/tern/extensions/cve_bin_tool/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/extensions/cve_bin_tool/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1404 2022-01-21 22:40:28.000000 tern-2.9.1/tern/extensions/cve_bin_tool/executor.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      626 2022-01-21 22:40:28.000000 tern-2.9.1/tern/extensions/executor.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.779337 tern-2.9.1/tern/extensions/scancode/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/extensions/scancode/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     8982 2022-01-21 22:40:28.000000 tern-2.9.1/tern/extensions/scancode/executor.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.779337 tern-2.9.1/tern/formats/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      564 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/consumer.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.779337 tern-2.9.1/tern/formats/cyclonedx/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      123 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/cyclonedx/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1682 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/cyclonedx/cyclonedx_common.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.779337 tern-2.9.1/tern/formats/cyclonedx/cyclonedxjson/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      123 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/cyclonedx/cyclonedxjson/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2080 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/cyclonedx/cyclonedxjson/generator.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1651 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/cyclonedx/cyclonedxjson/image_helpers.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1669 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/cyclonedx/cyclonedxjson/package_helpers.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.779337 tern-2.9.1/tern/formats/default/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/default/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5568 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/default/generator.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      463 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/generator.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.779337 tern-2.9.1/tern/formats/html/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/html/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    11845 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/html/generator.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.779337 tern-2.9.1/tern/formats/json/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/json/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2497 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/json/consumer.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      703 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/json/generator.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.783337 tern-2.9.1/tern/formats/spdx/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      863 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdx.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5741 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdx_common.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.783337 tern-2.9.1/tern/formats/spdx/spdxjson/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxjson/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3693 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxjson/consumer.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4027 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxjson/file_helpers.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1755 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxjson/formats.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6919 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxjson/generator.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3592 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxjson/image_helpers.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     8032 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxjson/layer_helpers.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3241 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxjson/package_helpers.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.783337 tern-2.9.1/tern/formats/spdx/spdxtagvalue/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxtagvalue/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3515 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxtagvalue/file_helpers.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1287 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxtagvalue/formats.py
+-rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)     5063 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxtagvalue/generator.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5401 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxtagvalue/image_helpers.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     5547 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxtagvalue/layer_helpers.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2535 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/spdx/spdxtagvalue/package_helpers.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.787337 tern-2.9.1/tern/formats/yaml/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/yaml/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1021 2022-01-21 22:40:28.000000 tern-2.9.1/tern/formats/yaml/generator.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.787337 tern-2.9.1/tern/load/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/load/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     7648 2022-01-21 22:40:28.000000 tern-2.9.1/tern/load/docker_api.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1913 2022-01-21 22:40:28.000000 tern-2.9.1/tern/load/skopeo.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1878 2022-01-21 22:40:28.000000 tern-2.9.1/tern/prep.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.787337 tern-2.9.1/tern/report/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/report/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4436 2022-01-21 22:40:28.000000 tern-2.9.1/tern/report/content.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     4937 2022-01-21 22:40:28.000000 tern-2.9.1/tern/report/errors.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3530 2022-01-21 22:40:28.000000 tern-2.9.1/tern/report/formats.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3441 2022-01-21 22:40:28.000000 tern-2.9.1/tern/report/report.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.743339 tern-2.9.1/tern/scripts/
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.787337 tern-2.9.1/tern/scripts/debian/
+-rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)      364 2022-01-21 22:40:28.000000 tern-2.9.1/tern/scripts/debian/apt_get_sources.sh
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.787337 tern-2.9.1/tern/scripts/debian/jessie/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      294 2022-01-21 22:40:28.000000 tern-2.9.1/tern/scripts/debian/jessie/sources.list
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.787337 tern-2.9.1/tern/tools/
+-rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)      831 2022-01-21 22:40:28.000000 tern-2.9.1/tern/tools/fs_hash.sh
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.791336 tern-2.9.1/tern/utils/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      121 2022-01-21 22:40:28.000000 tern-2.9.1/tern/utils/__init__.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     2661 2022-01-21 22:40:28.000000 tern-2.9.1/tern/utils/cache.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     1320 2022-01-21 22:40:28.000000 tern-2.9.1/tern/utils/constants.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    12250 2022-01-21 22:40:28.000000 tern-2.9.1/tern/utils/general.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      285 2022-01-21 22:40:28.000000 tern-2.9.1/tern/utils/host.py
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     9905 2022-01-21 22:40:28.000000 tern-2.9.1/tern/utils/rootfs.py
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.767338 tern-2.9.1/tern.egg-info/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)    29418 2022-01-21 23:21:08.000000 tern-2.9.1/tern.egg-info/PKG-INFO
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     6031 2022-01-21 23:21:08.000000 tern-2.9.1/tern.egg-info/SOURCES.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)        1 2022-01-21 23:21:08.000000 tern-2.9.1/tern.egg-info/dependency_links.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      667 2022-01-21 23:21:08.000000 tern-2.9.1/tern.egg-info/entry_points.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)        1 2022-01-21 22:43:40.000000 tern-2.9.1/tern.egg-info/not-zip-safe
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      424 2022-01-21 23:21:08.000000 tern-2.9.1/tern.egg-info/requires.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)        5 2022-01-21 23:21:08.000000 tern-2.9.1/tern.egg-info/top_level.txt
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)      700 2022-01-21 22:40:28.000000 tern-2.9.1/tox.ini
+drwxrwxr-x   0 rjudge    (1000) rjudge    (1000)        0 2022-01-21 23:21:08.791336 tern-2.9.1/vagrant/
+-rw-rw-r--   0 rjudge    (1000) rjudge    (1000)     3493 2022-01-21 22:40:28.000000 tern-2.9.1/vagrant/Vagrantfile
+-rwxrwxr-x   0 rjudge    (1000) rjudge    (1000)     1113 2022-01-21 22:40:28.000000 tern-2.9.1/vagrant/bootstrap.sh
```

### Comparing `tern-2.9.0/.devcontainer/devcontainer.json` & `tern-2.9.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/.github/ISSUE_TEMPLATE/bug.md` & `tern-2.9.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/.github/workflows/pull_request.yml` & `tern-2.9.1/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/AUTHORS` & `tern-2.9.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/CODE_OF_CONDUCT.md` & `tern-2.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/CONTRIBUTING.md` & `tern-2.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/ChangeLog` & `tern-2.9.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+v2.9.1
+------
+
+* Prepare for patched release 2.9.1
+* Fix scancode KeyError during license parsing
+* classes: Parse extended attributes
+* Fix retrieving image digest
+* Fix CycloneDX report generation
+
 v2.9.0
 ------
 
 * Prepare for Release 2.9.0
 * Use Skopeo to pull container images
 * formats: Modify layer title based on manifest
 * Modify environments to install skopeo
```

### Comparing `tern-2.9.0/GOVERNANCE.md` & `tern-2.9.1/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/LICENSE.txt` & `tern-2.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/PKG-INFO` & `tern-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tern
-Version: 2.9.0
+Version: 2.9.1
 Summary: An inspection tool to find the OSS compliance metadata of the packages installed in a container image.
 Home-page: https://github.com/tern-tools/tern/
 Author: VMware Inc
 Author-email: nishak@vmware.com
 License: BSD-2.0
 Project-URL: Documentation, https://github.com/tern-tools/tern/tree/master/docs
 Project-URL: Source Code, https://github.com/tern-tools/tern
```

### Comparing `tern-2.9.0/README.md` & `tern-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docker/Dockerfile` & `tern-2.9.1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docker/Dockerfile.scancode` & `tern-2.9.1/docker/Dockerfile.scancode`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docker_run.sh` & `tern-2.9.1/docker_run.sh`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/adding-to-command-library.md` & `tern-2.9.1/docs/adding-to-command-library.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/architecture.md` & `tern-2.9.1/docs/architecture.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/creating-custom-templates.md` & `tern-2.9.1/docs/creating-custom-templates.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/creating-tool-extensions.md` & `tern-2.9.1/docs/creating-tool-extensions.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/data-model.md` & `tern-2.9.1/docs/data-model.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/faq.md` & `tern-2.9.1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/glossary.md` & `tern-2.9.1/docs/glossary.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/img/arch.png` & `tern-2.9.1/docs/img/arch.png`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/img/tern_data_model.png` & `tern-2.9.1/docs/img/tern_data_model.png`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/img/tern_demo_fast.gif` & `tern-2.9.1/docs/img/tern_demo_fast.gif`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/img/tern_flow.png` & `tern-2.9.1/docs/img/tern_flow.png`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/img/tern_logo.png` & `tern-2.9.1/docs/img/tern_logo.png`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/navigating-the-code.md` & `tern-2.9.1/docs/navigating-the-code.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/project-roadmap-archive.md` & `tern-2.9.1/docs/project-roadmap-archive.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/project-roadmap.md` & `tern-2.9.1/docs/project-roadmap.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/release_checklist.md` & `tern-2.9.1/docs/releases/release_checklist.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v0_1_0.md` & `tern-2.9.1/docs/releases/v0_1_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v0_2_0.md` & `tern-2.9.1/docs/releases/v0_2_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v0_3_0.md` & `tern-2.9.1/docs/releases/v0_3_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v0_4_0.md` & `tern-2.9.1/docs/releases/v0_4_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v0_5_0.md` & `tern-2.9.1/docs/releases/v0_5_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v1_0_0-requirements.txt` & `tern-2.9.1/docs/releases/v1_0_0-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v1_0_0.md` & `tern-2.9.1/docs/releases/v1_0_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v1_0_1-requirements.txt` & `tern-2.9.1/docs/releases/v1_0_1-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v1_0_1.md` & `tern-2.9.1/docs/releases/v1_0_1.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_0_0-requirements.txt` & `tern-2.9.1/docs/releases/v2_0_0-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_0_0.md` & `tern-2.9.1/docs/releases/v2_0_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_1_0-requirements.txt` & `tern-2.9.1/docs/releases/v2_1_0-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_1_0.md` & `tern-2.9.1/docs/releases/v2_1_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_2_0-requirements.txt` & `tern-2.9.1/docs/releases/v2_2_0-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_2_0.md` & `tern-2.9.1/docs/releases/v2_2_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_3_0-requirements.txt` & `tern-2.9.1/docs/releases/v2_3_0-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_3_0.md` & `tern-2.9.1/docs/releases/v2_3_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_4_0-requirements.txt` & `tern-2.9.1/docs/releases/v2_4_0-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_4_0.md` & `tern-2.9.1/docs/releases/v2_4_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_5_0-requirements.txt` & `tern-2.9.1/docs/releases/v2_5_0-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_5_0.md` & `tern-2.9.1/docs/releases/v2_5_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_6_1-requirements.txt` & `tern-2.9.1/docs/releases/v2_6_1-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_6_1.md` & `tern-2.9.1/docs/releases/v2_6_1.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_7_0-requirements.txt` & `tern-2.9.1/docs/releases/v2_7_0-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_7_0.md` & `tern-2.9.1/docs/releases/v2_7_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_8_0-requirements.txt` & `tern-2.9.1/docs/releases/v2_8_0-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_8_0.md` & `tern-2.9.1/docs/releases/v2_8_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_9_0-requirements.txt` & `tern-2.9.1/docs/releases/v2_9_0-requirements.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/releases/v2_9_0.md` & `tern-2.9.1/docs/releases/v2_9_0.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/spdx-tag-value-mapping.md` & `tern-2.9.1/docs/spdx-tag-value-mapping.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/spdx-tag-value-overview.md` & `tern-2.9.1/docs/spdx-tag-value-overview.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/tern-lab-tutorial.md` & `tern-2.9.1/docs/tern-lab-tutorial.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/docs/yaml_output.md` & `tern-2.9.1/docs/yaml_output.md`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/requirements.txt` & `tern-2.9.1/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 #
 # This file is autogenerated by pip-compile with python 3.8
 # To update, run:
 #
 #    pip-compile
 #
-attrs==21.2.0
+attrs==21.4.0
     # via debian-inspector
 certifi==2021.10.8
     # via requests
 chardet==4.0.0
     # via debian-inspector
-charset-normalizer==2.0.9
+charset-normalizer==2.0.10
     # via requests
 debian-inspector==30.0.0
     # via -r requirements.in
 docker==5.0.3
     # via -r requirements.in
 dockerfile-parse==1.2.0
     # via -r requirements.in
 gitdb==4.0.9
     # via gitpython
-gitpython==3.1.24
+gitpython==3.1.26
     # via -r requirements.in
 idna==3.3
     # via requests
 packageurl-python==0.9.6
     # via -r requirements.in
 pbr==5.8.0
     # via
     #   -r requirements.in
     #   stevedore
-prettytable==2.4.0
+prettytable==3.0.0
     # via -r requirements.in
 pyyaml==6.0
     # via -r requirements.in
-regex==2021.11.10
+regex==2022.1.18
     # via -r requirements.in
-requests==2.26.0
+requests==2.27.1
     # via
     #   -r requirements.in
     #   docker
 six==1.16.0
     # via dockerfile-parse
 smmap==5.0.0
     # via gitdb
 stevedore==3.5.0
     # via -r requirements.in
-typing-extensions==4.0.1
-    # via gitpython
-urllib3==1.26.7
+urllib3==1.26.8
     # via requests
 wcwidth==0.2.5
     # via prettytable
 websocket-client==1.2.3
     # via docker
```

### Comparing `tern-2.9.0/samples/single_stage_tern/Dockerfile` & `tern-2.9.1/samples/single_stage_tern/Dockerfile`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/setup.cfg` & `tern-2.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/__main__.py` & `tern-2.9.1/tern/__main__.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/common.py` & `tern-2.9.1/tern/analyze/common.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/bundle.py` & `tern-2.9.1/tern/analyze/default/bundle.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/collect.py` & `tern-2.9.1/tern/analyze/default/collect.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/command_lib/base.yml` & `tern-2.9.1/tern/analyze/default/command_lib/base.yml`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/command_lib/command_lib.py` & `tern-2.9.1/tern/analyze/default/command_lib/command_lib.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/command_lib/snippets.yml` & `tern-2.9.1/tern/analyze/default/command_lib/snippets.yml`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/container/image.py` & `tern-2.9.1/tern/analyze/default/container/image.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/container/multi_layer.py` & `tern-2.9.1/tern/analyze/default/container/multi_layer.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/container/run.py` & `tern-2.9.1/tern/analyze/default/container/run.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/container/single_layer.py` & `tern-2.9.1/tern/analyze/default/container/single_layer.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/core.py` & `tern-2.9.1/tern/analyze/default/core.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/debug/run.py` & `tern-2.9.1/tern/analyze/default/debug/run.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/default_common.py` & `tern-2.9.1/tern/analyze/default/default_common.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/dockerfile/lock.py` & `tern-2.9.1/tern/analyze/default/dockerfile/lock.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/dockerfile/parse.py` & `tern-2.9.1/tern/analyze/default/dockerfile/parse.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/dockerfile/run.py` & `tern-2.9.1/tern/analyze/default/dockerfile/run.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/filter.py` & `tern-2.9.1/tern/analyze/default/filter.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/live/collect.py` & `tern-2.9.1/tern/analyze/default/live/collect.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/default/live/run.py` & `tern-2.9.1/tern/analyze/default/live/run.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/analyze/passthrough.py` & `tern-2.9.1/tern/analyze/passthrough.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/classes/command.py` & `tern-2.9.1/tern/classes/command.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/classes/docker_image.py` & `tern-2.9.1/tern/classes/docker_image.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/classes/file_data.py` & `tern-2.9.1/tern/classes/file_data.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/classes/image.py` & `tern-2.9.1/tern/classes/image.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/classes/image_layer.py` & `tern-2.9.1/tern/classes/image_layer.py`

 * *Files 16% similar despite different names*

```diff
@@ -334,31 +334,63 @@
             # make directory structure if it doesn't exist
             if not os.path.exists(fs_dir):
                 os.makedirs(fs_dir)
             tar_file = os.path.join(rootfs.get_working_dir(), self.tar_file)
             rootfs.extract_tarfile(tar_file, fs_dir)
             self.__fs_hash = rootfs.calc_fs_hash(fs_dir)
 
+    def _parse_hash_content(self, content):
+        """This is an internal function to parse the content of the hash
+        and return a list of FileData objects
+        The content consists of lines of the form:
+        permissions|uid|gid|size|hard links|  sha256sum  filepath xattrs
+        where xattrs is the list of extended attributes for the file
+        The extended attributes start with a '# file' indicator, followed
+        by a list of key-value pairs separated by newlines. For now, we will
+        conserve the key-value pair list as they appear and separate
+        each one by a comma"""
+        file_list = []
+        # keep track of where we are on the list of files
+        index = 0
+        # loop through the content
+        while content:
+            line = content.pop(0)
+            if "# file" in line:
+                # collect the extended attributes
+                xattrlist = []
+                xattrline = content.pop(0)
+                while xattrline != '\n':
+                    xattrlist.append(xattrline.strip())
+                    xattrline = content.pop(0)
+                # when we break out of the extended attributes loop
+                # we combine the results and update the FileData object
+                # existing in the previous index
+                file_list[index-1].extattrs = file_list[index-1].extattrs + \
+                    "  " + ','.join(xattrlist)
+            else:
+                # collect the regular attributes
+                file_info = line[:-1].split('  ')
+                file_data = FileData(os.path.basename(file_info[2]),
+                                     os.path.relpath(file_info[2], '.'))
+                file_data.set_checksum('sha256', file_info[1])
+                file_data.set_whiteout()
+                file_list.append(file_data)
+                index = index + 1
+        return file_list
+
     def add_files(self):
         '''Get all the files present in a layer and store
         them as a list of FileData objects'''
         fs_path = self.get_untar_dir()
         hash_file = os.path.join(os.path.dirname(fs_path),
                                  self.__fs_hash) + '.txt'
         with open(hash_file, encoding='utf-8') as f:
             content = f.readlines()
-        for line in content:
-            # lines are of the form:
-            # permissions|uid|gid|size|hard links|  sha256sum  filepath
-            file_info = line[:-1].split('  ')
-            file_data = FileData(os.path.basename(file_info[2]),
-                                 os.path.relpath(file_info[2], '.'))
-            file_data.set_checksum('sha256', file_info[1])
-            file_data.extattrs = file_info[0]
-            file_data.set_whiteout()
+        file_list = self._parse_hash_content(content)
+        for file_data in file_list:
             self.add_file(file_data)
 
     def get_layer_workdir(self):
         # If the layer is created by a WORKDIR command then return the workdir
         match = re.search(r"\bWORKDIR\ (\/\w+)+\b", self.created_by)
         if match:
             return match.group().split()[1]
```

### Comparing `tern-2.9.0/tern/classes/notice.py` & `tern-2.9.1/tern/classes/notice.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/classes/notice_origin.py` & `tern-2.9.1/tern/classes/notice_origin.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/classes/oci_image.py` & `tern-2.9.1/tern/classes/oci_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import subprocess  # nosec
 
 from tern.utils import rootfs
 from tern.utils import general
 from tern.classes.image import Image
 from tern.utils.constants import manifest_file
 from tern.classes.image_layer import ImageLayer
+from tern.load import skopeo
 
 
 class OCIImage(Image):
     """A representation of an OCI compatible image that exists on disk"""
     def __init__(self, repotag=None):
         super().__init__(repotag)
         # In case the OCI image corresponds with an image built by Docker
@@ -96,20 +97,19 @@
             self._load_until_layer = load_until_layer
         try:
             self._manifest = self.get_image_manifest()
             self._config = self.get_image_config(self._manifest)
             self.__history = self.get_image_history(self._config)
             layer_paths = self.get_image_layers(self._manifest)
             layer_diffs = self.get_diff_ids(self._config)
-            # if the digest isn't in the repotag, get it from the config
+            # if the digest isn't in the repotag, get it using skopeo
             if not self.checksum:
-                repo_dict = general.parse_image_string(
-                    self._config.get("config").get("Image"))
-                self.set_checksum(repo_dict.get("digest_type"),
-                                  repo_dict.get("digest"))
+                digest_type, digest = skopeo.get_image_digest(self.repotag)
+                if digest_type and digest:
+                    self.set_checksum(digest_type, digest)
             layer_checksum_type = self.get_diff_checksum_type(self._config)
             layer_count = 1
             while layer_diffs and layer_paths:
                 layer = ImageLayer(layer_diffs.pop(0), layer_paths.pop(0))
                 if (self.load_until_layer >= layer_count
                         or self.load_until_layer == 0):
                     layer.set_checksum(layer_checksum_type, layer.diff_id)
```

### Comparing `tern-2.9.0/tern/classes/origins.py` & `tern-2.9.1/tern/classes/origins.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/classes/package.py` & `tern-2.9.1/tern/classes/package.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/classes/template.py` & `tern-2.9.1/tern/classes/template.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/extensions/cve_bin_tool/executor.py` & `tern-2.9.1/tern/extensions/cve_bin_tool/executor.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/extensions/executor.py` & `tern-2.9.1/tern/extensions/executor.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/extensions/scancode/executor.py` & `tern-2.9.1/tern/extensions/scancode/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,22 +77,28 @@
 
 def filter_pkg_license(declared_license):
     '''When scancode detects python package licenses, it attaches classifiers
     to the declared_license field as a dictionary object, otherwise
     it will represent the license as a string or list of strings.
     Given a scancode declared_license field, extract and return a
     license string'''
-    if isinstance(declared_license, dict):
+    if isinstance(declared_license, dict) and len(declared_license) != 0:
         try:
             return declared_license['license']
         except KeyError:
-            # parse classifiers for PyPI licenses
-            # According to https://pypi.org/pypi?%3Aaction=list_classifiers
-            # we can always take the value after the last '::'
-            return declared_license['classifiers'][0].split('::')[-1].strip()
+            try:
+                return declared_license['License']
+            except KeyError:
+                try:
+                    # parse classifiers for PyPI licenses
+                    # According to pypi.org/pypi?%3Aaction=list_classifiers
+                    # we can always take the value after the last '::'
+                    return declared_license['classifiers'][0].split('::')[-1].strip()
+                except KeyError:
+                    return None
     if isinstance(declared_license, list):
         for i, lic in enumerate(declared_license):
             # Some license lists from Scancode have dictionary entries
             # Extract license 'types' from license dictionaries
             if isinstance(lic, dict):
                 declared_license[i] = lic["type"]
         # Get rid of duplicate licenses
```

### Comparing `tern-2.9.0/tern/formats/consumer.py` & `tern-2.9.1/tern/formats/consumer.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/cyclonedx/cyclonedx_common.py` & `tern-2.9.1/tern/formats/cyclonedx/cyclonedx_common.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/cyclonedx/cyclonedxjson/generator.py` & `tern-2.9.1/tern/formats/cyclonedx/cyclonedxjson/generator.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/cyclonedx/cyclonedxjson/image_helpers.py` & `tern-2.9.1/tern/formats/cyclonedx/cyclonedxjson/image_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 '''
 Helper functions for image level JSON CycloneDX document dictionaries
 '''
 
 
 from tern.formats.cyclonedx import cyclonedx_common
 from packageurl import PackageURL
+from tern.classes.oci_image import OCIImage
+from tern.classes.docker_image import DockerImage
 
 
 def get_image_dict(image_obj):
     ''' Given an image object return the CycloneDX document dictionary for the
     given image. For CycloneDX, the image is a component and hence follows the
     JSON spec for components. '''
     image_dict = {
@@ -24,17 +26,19 @@
         'hashes': [],
         'properties': []
     }
 
     purl = PackageURL('docker', None, image_dict['name'], image_dict['version'])
     image_dict['purl'] = str(purl)
 
-    if image_obj.repotags:
+    if isinstance(image_obj, DockerImage):
         for repotag in image_obj.repotags:
             image_dict['properties'].append(cyclonedx_common.get_property('tern:repotag', repotag))
+    elif isinstance(image_obj, OCIImage):
+        image_dict['properties'].append(cyclonedx_common.get_property('tern:repotag', image_obj.repotag))
 
     os_guess = cyclonedx_common.get_os_guess(image_obj)
     if os_guess:
         image_dict['properties'].append(cyclonedx_common.get_property('tern:os_guess', os_guess))
 
     cdx_hash = cyclonedx_common.get_hash(image_obj.checksum_type, image_obj.checksum)
     if cdx_hash is not None:
```

### Comparing `tern-2.9.0/tern/formats/cyclonedx/cyclonedxjson/package_helpers.py` & `tern-2.9.1/tern/formats/cyclonedx/cyclonedxjson/package_helpers.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/default/generator.py` & `tern-2.9.1/tern/formats/default/generator.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/html/generator.py` & `tern-2.9.1/tern/formats/html/generator.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/json/consumer.py` & `tern-2.9.1/tern/formats/json/consumer.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/json/generator.py` & `tern-2.9.1/tern/formats/json/generator.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdx.py` & `tern-2.9.1/tern/formats/spdx/spdx.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdx_common.py` & `tern-2.9.1/tern/formats/spdx/spdx_common.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxjson/consumer.py` & `tern-2.9.1/tern/formats/spdx/spdxjson/consumer.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxjson/file_helpers.py` & `tern-2.9.1/tern/formats/spdx/spdxjson/file_helpers.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxjson/formats.py` & `tern-2.9.1/tern/formats/spdx/spdxjson/formats.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxjson/generator.py` & `tern-2.9.1/tern/formats/spdx/spdxjson/generator.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxjson/image_helpers.py` & `tern-2.9.1/tern/formats/spdx/spdxjson/image_helpers.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxjson/layer_helpers.py` & `tern-2.9.1/tern/formats/spdx/spdxjson/layer_helpers.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxjson/package_helpers.py` & `tern-2.9.1/tern/formats/spdx/spdxjson/package_helpers.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxtagvalue/file_helpers.py` & `tern-2.9.1/tern/formats/spdx/spdxtagvalue/file_helpers.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxtagvalue/formats.py` & `tern-2.9.1/tern/formats/spdx/spdxtagvalue/formats.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxtagvalue/generator.py` & `tern-2.9.1/tern/formats/spdx/spdxtagvalue/generator.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxtagvalue/image_helpers.py` & `tern-2.9.1/tern/formats/spdx/spdxtagvalue/image_helpers.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxtagvalue/layer_helpers.py` & `tern-2.9.1/tern/formats/spdx/spdxtagvalue/layer_helpers.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/spdx/spdxtagvalue/package_helpers.py` & `tern-2.9.1/tern/formats/spdx/spdxtagvalue/package_helpers.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/formats/yaml/generator.py` & `tern-2.9.1/tern/formats/yaml/generator.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/load/docker_api.py` & `tern-2.9.1/tern/load/docker_api.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/load/skopeo.py` & `tern-2.9.1/tern/load/skopeo.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c) 2021 VMware, Inc. All Rights Reserved.
 # SPDX-License-Identifier: BSD-2-Clause
 
 """
 Interactions with remote container images using skopeo
 """
 
+import json
 import logging
 import sys
 import shutil
 
 from tern.utils import constants
 from tern.utils import rootfs
 
@@ -36,7 +37,27 @@
     logger.debug("Attempting to pull image \"%s\"", image_tag_string)
     result, error = rootfs.shell_command(
         False, ['skopeo', 'copy', remote, local])
     if error:
         logger.error("Error when downloading image: \"%s\"", error)
         return None
     return result
+
+
+def get_image_digest(image_tag_string):
+    """Use skopeo to get the remote image's digest"""
+    # check if skopeo is set up
+    check_skopeo_setup()
+    remote = f'docker://{image_tag_string}'
+    logger.debug("Inspecting remote image \"%s\"", image_tag_string)
+    result, error = rootfs.shell_command(
+        False, ['skopeo', 'inspect', remote])
+    if error or not result:
+        logger.error("Unable to retrieve image digest")
+        return None, None
+    result_string = json.loads(result)
+    digest_string = result_string.get("Digest")
+    if not digest_string:
+        logger.error("No image digest available")
+        return None, None
+    digest_list = digest_string.split(":")
+    return digest_list[0], digest_list[1]
```

### Comparing `tern-2.9.0/tern/prep.py` & `tern-2.9.1/tern/prep.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/report/content.py` & `tern-2.9.1/tern/report/content.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/report/errors.py` & `tern-2.9.1/tern/report/errors.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/report/formats.py` & `tern-2.9.1/tern/report/formats.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/report/report.py` & `tern-2.9.1/tern/report/report.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/tools/fs_hash.sh` & `tern-2.9.1/tern/tools/fs_hash.sh`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/utils/cache.py` & `tern-2.9.1/tern/utils/cache.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/utils/constants.py` & `tern-2.9.1/tern/utils/constants.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/utils/general.py` & `tern-2.9.1/tern/utils/general.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern/utils/rootfs.py` & `tern-2.9.1/tern/utils/rootfs.py`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tern.egg-info/PKG-INFO` & `tern-2.9.1/tern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tern
-Version: 2.9.0
+Version: 2.9.1
 Summary: An inspection tool to find the OSS compliance metadata of the packages installed in a container image.
 Home-page: https://github.com/tern-tools/tern/
 Author: VMware Inc
 Author-email: nishak@vmware.com
 License: BSD-2.0
 Project-URL: Documentation, https://github.com/tern-tools/tern/tree/master/docs
 Project-URL: Source Code, https://github.com/tern-tools/tern
```

### Comparing `tern-2.9.0/tern.egg-info/SOURCES.txt` & `tern-2.9.1/tern.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 docs/releases/v2_6_1.md
 docs/releases/v2_7_0-requirements.txt
 docs/releases/v2_7_0.md
 docs/releases/v2_8_0-requirements.txt
 docs/releases/v2_8_0.md
 docs/releases/v2_9_0-requirements.txt
 docs/releases/v2_9_0.md
+docs/releases/v2_9_1-requirements.txt
+docs/releases/v2_9_1.md
 samples/alpine_python/Dockerfile
 samples/debian_vim/Dockerfile
 samples/photon_3_layers/Dockerfile
 samples/photon_git/Dockerfile
 samples/photon_openjre/Dockerfile
 samples/single_stage_tern/Dockerfile
 tern/__init__.py
```

### Comparing `tern-2.9.0/tern.egg-info/entry_points.txt` & `tern-2.9.1/tern.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/tox.ini` & `tern-2.9.1/tox.ini`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/vagrant/Vagrantfile` & `tern-2.9.1/vagrant/Vagrantfile`

 * *Files identical despite different names*

### Comparing `tern-2.9.0/vagrant/bootstrap.sh` & `tern-2.9.1/vagrant/bootstrap.sh`

 * *Files identical despite different names*

