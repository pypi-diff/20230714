# Comparing `tmp/looper-1.4.0.tar.gz` & `tmp/looper-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "looper-1.4.0.tar", last modified: Mon Apr 24 20:40:38 2023, max compression
+gzip compressed data, was "looper-1.4.1.tar", last modified: Fri Jul 14 21:11:25 2023, max compression
```

## Comparing `looper-1.4.0.tar` & `looper-1.4.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.388970 looper-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-24 20:40:25.000000 looper-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 20:40:25.000000 looper-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-24 20:40:38.388970 looper-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-24 20:40:25.000000 looper-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-24 20:40:25.000000 looper-1.4.0/logo_looper.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.384969 looper-1.4.0/looper/
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-04-24 20:40:25.000000 looper-1.4.0/looper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 20:40:25.000000 looper-1.4.0/looper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-24 20:40:25.000000 looper-1.4.0/looper/_devtools.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 20:40:25.000000 looper-1.4.0/looper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    35293 2023-04-24 20:40:25.000000 looper-1.4.0/looper/conductor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-24 20:40:25.000000 looper-1.4.0/looper/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-24 20:40:25.000000 looper-1.4.0/looper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    43820 2023-04-24 20:40:25.000000 looper-1.4.0/looper/html_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-04-24 20:40:25.000000 looper-1.4.0/looper/html_reports_pipestat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-24 20:40:25.000000 looper-1.4.0/looper/html_reports_project_pipestat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.388970 looper-1.4.0/looper/jinja_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/footer_index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/head.html
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/navbar_links.html
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/navbar_list_parent.html
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/object.html
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/project_object.html
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/sample.html
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/status.html
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/status_table.html
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/status_table_no_links.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.388970 looper-1.4.0/looper/jinja_templates_old/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/footer_index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/head.html
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/logo.html
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/navbar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/navbar_links.html
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/navbar_list_parent.html
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/object.html
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/project_object.html
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/sample.html
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/status.html
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/status_table.html
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/status_table_no_links.html
--rwxr-xr-x   0 runner    (1001) docker     (123)    45084 2023-04-24 20:40:25.000000 looper-1.4.0/looper/looper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-24 20:40:25.000000 looper-1.4.0/looper/parser_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-04-24 20:40:25.000000 looper-1.4.0/looper/pipeline_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-24 20:40:25.000000 looper-1.4.0/looper/processed_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-04-24 20:40:25.000000 looper-1.4.0/looper/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.388970 looper-1.4.0/looper/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-24 20:40:25.000000 looper-1.4.0/looper/schemas/pipeline_interface_schema_generic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-24 20:40:25.000000 looper-1.4.0/looper/schemas/pipeline_interface_schema_project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-24 20:40:25.000000 looper-1.4.0/looper/schemas/pipeline_interface_schema_sample.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20474 2023-04-24 20:40:25.000000 looper-1.4.0/looper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.384969 looper-1.4.0/looper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.388970 looper-1.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 20:40:25.000000 looper-1.4.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 20:40:25.000000 looper-1.4.0/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 20:40:25.000000 looper-1.4.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-24 20:40:38.388970 looper-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-24 20:40:25.000000 looper-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.014073 looper-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-14 21:11:09.000000 looper-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 21:11:09.000000 looper-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-14 21:11:25.014073 looper-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-14 21:11:09.000000 looper-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-14 21:11:09.000000 looper-1.4.1/logo_looper.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.002073 looper-1.4.1/looper/
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-07-14 21:11:09.000000 looper-1.4.1/looper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-14 21:11:09.000000 looper-1.4.1/looper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-14 21:11:09.000000 looper-1.4.1/looper/_devtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 21:11:09.000000 looper-1.4.1/looper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-07-14 21:11:09.000000 looper-1.4.1/looper/conductor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-14 21:11:09.000000 looper-1.4.1/looper/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-14 21:11:09.000000 looper-1.4.1/looper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43820 2023-07-14 21:11:09.000000 looper-1.4.1/looper/html_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-14 21:11:09.000000 looper-1.4.1/looper/html_reports_pipestat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-07-14 21:11:09.000000 looper-1.4.1/looper/html_reports_project_pipestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.010073 looper-1.4.1/looper/jinja_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/sample.html
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/status_table_no_links.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.014073 looper-1.4.1/looper/jinja_templates_old/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/sample.html
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/status_table_no_links.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45072 2023-07-14 21:11:09.000000 looper-1.4.1/looper/looper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-14 21:11:09.000000 looper-1.4.1/looper/parser_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-07-14 21:11:09.000000 looper-1.4.1/looper/pipeline_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-14 21:11:09.000000 looper-1.4.1/looper/processed_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-07-14 21:11:09.000000 looper-1.4.1/looper/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.014073 looper-1.4.1/looper/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-14 21:11:09.000000 looper-1.4.1/looper/schemas/pipeline_interface_schema_generic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-14 21:11:09.000000 looper-1.4.1/looper/schemas/pipeline_interface_schema_project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-14 21:11:09.000000 looper-1.4.1/looper/schemas/pipeline_interface_schema_sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20474 2023-07-14 21:11:09.000000 looper-1.4.1/looper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.006073 looper-1.4.1/looper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.014073 looper-1.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 21:11:09.000000 looper-1.4.1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 21:11:09.000000 looper-1.4.1/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 21:11:09.000000 looper-1.4.1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-14 21:11:25.018073 looper-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-14 21:11:09.000000 looper-1.4.1/setup.py
```

### Comparing `looper-1.4.0/LICENSE.txt` & `looper-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/PKG-INFO` & `looper-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looper
-Version: 1.4.0
+Version: 1.4.1
 Summary: A pipeline submission engine that parses sample inputs and submits pipelines for each sample.
 Home-page: https://github.com/pepkit/looper
 Author: Nathan Sheffield, Vince Reuter, Michal Stolarczyk, Johanna Klughammer, Andre Rendeiro
 License: BSD2
 Keywords: bioinformatics,sequencing,ngs
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `looper-1.4.0/README.md` & `looper-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/logo_looper.svg` & `looper-1.4.1/logo_looper.svg`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/__init__.py` & `looper-1.4.1/looper/__init__.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/_devtools.py` & `looper-1.4.1/looper/_devtools.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/conductor.py` & `looper-1.4.1/looper/conductor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import importlib
 import logging
 import os
 import subprocess
 import time
 from copy import copy, deepcopy
 from json import loads
-from subprocess import CalledProcessError, check_output
+from subprocess import check_output
 from typing import *
 
-from eido import read_schema, validate_inputs
+from eido import read_schema, get_input_files_size
 from eido.const import INPUT_FILE_SIZE_KEY, MISSING_KEY
 from jinja2.exceptions import UndefinedError
 
 from peppy.const import CONFIG_KEY, SAMPLE_NAME_ATTR, SAMPLE_YAML_EXT
 from peppy.exceptions import RemoteYAMLError
 from pipestat import PipestatError
 from ubiquerg import expandpath
@@ -450,15 +450,15 @@
         validation = {}
         validation.setdefault(INPUT_FILE_SIZE_KEY, 0)
         # Check for any missing requirements before submitting.
         _LOGGER.debug("Determining missing requirements")
         schema_source = self.pl_iface.get_pipeline_schemas()
         if schema_source and self.prj.file_checks:
             try:
-                validation = validate_inputs(sample, read_schema(schema_source))
+                validation = get_input_files_size(sample, read_schema(schema_source))
             except RemoteYAMLError:
                 _LOGGER.warn(
                     "Could not read remote schema. Skipping inputs validation."
                 )
             else:
                 if validation[MISSING_KEY]:
                     missing_reqs_msg = (
```

### Comparing `looper-1.4.0/looper/const.py` & `looper-1.4.1/looper/const.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/exceptions.py` & `looper-1.4.1/looper/exceptions.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/html_reports.py` & `looper-1.4.1/looper/html_reports.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/html_reports_pipestat.py` & `looper-1.4.1/looper/html_reports_pipestat.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/html_reports_project_pipestat.py` & `looper-1.4.1/looper/html_reports_project_pipestat.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/footer_index.html` & `looper-1.4.1/looper/jinja_templates/footer_index.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/head.html` & `looper-1.4.1/looper/jinja_templates/head.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/index.html` & `looper-1.4.1/looper/jinja_templates/index.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/logo.html` & `looper-1.4.1/looper/jinja_templates/logo.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/navbar.html` & `looper-1.4.1/looper/jinja_templates/navbar.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/navbar_links.html` & `looper-1.4.1/looper/jinja_templates/navbar_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/navbar_list_parent.html` & `looper-1.4.1/looper/jinja_templates/navbar_list_parent.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/object.html` & `looper-1.4.1/looper/jinja_templates/object.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/project_object.html` & `looper-1.4.1/looper/jinja_templates/project_object.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/sample.html` & `looper-1.4.1/looper/jinja_templates/sample.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/status_table.html` & `looper-1.4.1/looper/jinja_templates/status_table.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates/status_table_no_links.html` & `looper-1.4.1/looper/jinja_templates/status_table_no_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/footer_index.html` & `looper-1.4.1/looper/jinja_templates_old/footer_index.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/head.html` & `looper-1.4.1/looper/jinja_templates_old/head.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/index.html` & `looper-1.4.1/looper/jinja_templates_old/index.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/logo.html` & `looper-1.4.1/looper/jinja_templates_old/logo.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/navbar.html` & `looper-1.4.1/looper/jinja_templates_old/navbar.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/navbar_links.html` & `looper-1.4.1/looper/jinja_templates_old/navbar_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/navbar_list_parent.html` & `looper-1.4.1/looper/jinja_templates_old/navbar_list_parent.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/object.html` & `looper-1.4.1/looper/jinja_templates_old/object.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/project_object.html` & `looper-1.4.1/looper/jinja_templates_old/project_object.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/sample.html` & `looper-1.4.1/looper/jinja_templates_old/sample.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/status_table.html` & `looper-1.4.1/looper/jinja_templates_old/status_table.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/jinja_templates_old/status_table_no_links.html` & `looper-1.4.1/looper/jinja_templates_old/status_table_no_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/looper.py` & `looper-1.4.1/looper/looper.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
         num_commands_possible = 0
         failed_submission_scripts = []
 
         # config validation (samples excluded) against all schemas defined
         # for every pipeline matched for this project
         for schema_file in self.prj.get_schemas(self.prj.pipeline_interfaces):
             try:
-                validate_config(self.prj, schema_file, True)
+                validate_config(self.prj, schema_file)
             except RemoteYAMLError:
                 _LOGGER.warn(
                     "Could not read remote schema, skipping config validation."
                 )
 
         submission_conductors = {}
         for piface in self.prj.pipeline_interfaces:
@@ -472,15 +472,15 @@
                 failures[sample.sample_name] = skip_reasons
                 continue
 
             # single sample validation against a single schema
             # (from sample's piface)
             for schema_file in self.prj.get_schemas(sample_pifaces):
                 try:
-                    validate_sample(self.prj, sample.sample_name, schema_file, True)
+                    validate_sample(self.prj, sample.sample_name, schema_file)
                 except EidoValidationError as e:
                     _LOGGER.error(f"Short-circuiting due to validation error: {e}")
                     return False
                 except RemoteYAMLError:
                     _LOGGER.warn(
                         f"Could not read remote schema, skipping '{sample.sample_name}' "
                         f"sample validation against {schema_file}"
```

### Comparing `looper-1.4.0/looper/parser_types.py` & `looper-1.4.1/looper/parser_types.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/pipeline_interface.py` & `looper-1.4.1/looper/pipeline_interface.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/processed_project.py` & `looper-1.4.1/looper/processed_project.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/project.py` & `looper-1.4.1/looper/project.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/schemas/pipeline_interface_schema_generic.yaml` & `looper-1.4.1/looper/schemas/pipeline_interface_schema_generic.yaml`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/schemas/pipeline_interface_schema_project.yaml` & `looper-1.4.1/looper/schemas/pipeline_interface_schema_project.yaml`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/schemas/pipeline_interface_schema_sample.yaml` & `looper-1.4.1/looper/schemas/pipeline_interface_schema_sample.yaml`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper/utils.py` & `looper-1.4.1/looper/utils.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/looper.egg-info/PKG-INFO` & `looper-1.4.1/looper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looper
-Version: 1.4.0
+Version: 1.4.1
 Summary: A pipeline submission engine that parses sample inputs and submits pipelines for each sample.
 Home-page: https://github.com/pepkit/looper
 Author: Nathan Sheffield, Vince Reuter, Michal Stolarczyk, Johanna Klughammer, Andre Rendeiro
 License: BSD2
 Keywords: bioinformatics,sequencing,ngs
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `looper-1.4.0/looper.egg-info/SOURCES.txt` & `looper-1.4.1/looper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `looper-1.4.0/setup.py` & `looper-1.4.1/setup.py`

 * *Files identical despite different names*

