# Comparing `tmp/kestrel-lang-1.7.0.tar.gz` & `tmp/kestrel-lang-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel-lang-1.7.0.tar", last modified: Wed Jun 14 19:55:14 2023, max compression
+gzip compressed data, was "kestrel-lang-1.7.1.tar", last modified: Fri Jul 14 00:16:22 2023, max compression
```

## Comparing `kestrel-lang-1.7.0.tar` & `kestrel-lang-1.7.1.tar`

### file list

```diff
@@ -1,108 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.083361 kestrel-lang-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-06-14 19:55:14.083361 kestrel-lang-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.063361 kestrel-lang-1.7.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/bin/kestrel
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-14 19:55:14.083361 kestrel-lang-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.059361 kestrel-lang-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.063361 kestrel-lang-1.7.0/src/kestrel/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.063361 kestrel-lang-1.7.0/src/kestrel/absinterface/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/absinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/absinterface/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.067360 kestrel-lang-1.7.0/src/kestrel/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/analytics/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/analytics/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.067360 kestrel-lang-1.7.0/src/kestrel/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/codegen/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.067360 kestrel-lang-1.7.0/src/kestrel/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/datasource/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/datasource/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/datasource/retstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.067360 kestrel-lang-1.7.0/src/kestrel/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/semantics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/semantics/completor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/semantics/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/semantics/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.071360 kestrel-lang-1.7.0/src/kestrel/symboltable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/symboltable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/symboltable/symtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/symboltable/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.071360 kestrel-lang-1.7.0/src/kestrel/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/ecgpattern.lark
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/ecgpattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/kestrel.lark
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/syntax/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.071360 kestrel-lang-1.7.0/src/kestrel_analytics_docker/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_docker/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.071360 kestrel-lang-1.7.0/src/kestrel_analytics_python/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_python/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_analytics_python/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.071360 kestrel-lang-1.7.0/src/kestrel_datasource_stixbundle/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixbundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixbundle/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.075361 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.075361 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/transmitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.075361 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-06-14 19:55:14.000000 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-14 19:55:14.000000 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:55:14.000000 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-14 19:55:14.000000 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-14 19:55:14.000000 kestrel-lang-1.7.0/src/kestrel_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:55:14.083361 kestrel-lang-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_find.py
--rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_command_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_python_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_stixshifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_stixshifter_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-14 19:54:48.000000 kestrel-lang-1.7.0/tests/test_timestamped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.975632 kestrel-lang-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-07-14 00:16:22.975632 kestrel-lang-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.955632 kestrel-lang-1.7.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/bin/kestrel
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-14 00:16:22.975632 kestrel-lang-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.955632 kestrel-lang-1.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.959632 kestrel-lang-1.7.1/src/kestrel/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.959632 kestrel-lang-1.7.1/src/kestrel/absinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/absinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/absinterface/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.959632 kestrel-lang-1.7.1/src/kestrel/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/analytics/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/analytics/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.963632 kestrel-lang-1.7.1/src/kestrel/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/prefetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.963632 kestrel-lang-1.7.1/src/kestrel/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/datasource/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/datasource/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/datasource/retstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.963632 kestrel-lang-1.7.1/src/kestrel/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/semantics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/semantics/completor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/semantics/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/semantics/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.967632 kestrel-lang-1.7.1/src/kestrel/symboltable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/symboltable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/symboltable/symtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/symboltable/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.967632 kestrel-lang-1.7.1/src/kestrel/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/ecgpattern.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/ecgpattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/kestrel.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.967632 kestrel-lang-1.7.1/src/kestrel_analytics_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_docker/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.971632 kestrel-lang-1.7.1/src/kestrel_analytics_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_python/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.971632 kestrel-lang-1.7.1/src/kestrel_datasource_stixbundle/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixbundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixbundle/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.971632 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.971632 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/transmitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.971632 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-07-14 00:16:22.000000 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-14 00:16:22.000000 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:16:22.000000 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-14 00:16:22.000000 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 00:16:22.000000 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.975632 kestrel-lang-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_python_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_stixshifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_stixshifter_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_timestamped.py
```

### Comparing `kestrel-lang-1.7.0/AUTHORS.rst` & `kestrel-lang-1.7.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/LICENSE.md` & `kestrel-lang-1.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/PKG-INFO` & `kestrel-lang-1.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.7.0
+Version: 1.7.1
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
@@ -43,38 +43,41 @@
 
 .. image:: https://readthedocs.org/projects/kestrel/badge/?version=latest
         :target: https://kestrel.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 |
 
-**[News]** Kestrel hunt at `Infosec Jupyterthon 2022`_ [`IJ'22 live hunt recording`_]
-
-**[News]** Kestrel session at `Black Hat USA 2022`_ [`BH'22 recording`_ | `BH'22 hunting lab`_]
+**[News]** Kestrel session at `Black Hat USA 2023`_
 
 --------
 
 Kestrel is a threat hunting language aiming to make cyber threat hunting *fast*
 by providing a layer of abstraction to build reusable, composable, and
-shareable hunt-flow.
+shareable hunt-flow. Starting with:
+
+#. `Black Hat USA 2022 session recording`_
+#. `Black Hat USA 2022 Kestrel hunting lab`_
+#. `Kestrel live tutorial in a cloud sandbox`_
 
-`Try Kestrel in a cloud sandbox without install`_ (Blog: `Try Kestrel in a Cloud Sandbox`_).
+The Goal
+========
 
 Software developers write Python or Swift than machine code to quickly turn
 business logic into applications. Threat hunters write Kestrel to quickly turn
 threat hypotheses into hunt-flow. We see threat hunting as an interactive
 procedure to create customized intrusion detection systems on the fly, and
 hunt-flow is to hunts as control-flow is to ordinary programs.
 
 What does it mean by *hunt fast*?
 
-- Do not write the same TTP pattern in different data source queries.
-- Do not write one-time-use adapaters to connect hunt steps.
-- Do not waste your existing analytic scripts/programs in future hunts.
-- Do construct your hunt-flow from smaller reuseable hunt-flow.
+- Do NOT write the same TTP pattern in different data source queries.
+- Do NOT write one-time-use adapaters to connect hunt steps.
+- Do NOT waste your existing analytic scripts/programs in future hunts.
+- DD construct your hunt-flow from smaller reuseable hunt-flow.
 - Do share your huntbook with your future self and your colleagues.
 - Do get interactive feedback and revise hunt-flow on the fly.
 
 |
 
 .. image:: https://github.com/opencybersecurityalliance/data-bucket-kestrel/raw/main/images/github_homepage_animation.gif
    :width: 90%
@@ -143,14 +146,15 @@
 #. `Fun with securitydatasets.com and the Kestrel PowerShell Deobfuscator`_
 
 Talks And Demos
 ===============
 
 Talk summary (visit `Kestrel documentation on talks`_ to learn details):
 
+- 2023/08 `Black Hat USA 2023`_
 - 2022/12 `Infosec Jupyterthon 2022`_ [`IJ'22 live hunt recording`_]
 - 2022/08 `Black Hat USA 2022`_ [`BH'22 recording`_ | `BH'22 hunting lab`_]
 - 2022/06 `Cybersecurity Automation Workshop`_
 - 2022/04 `SC eSummit on Threat Hunting & Offense Security`_ (free to register/playback)
 - 2021/12 `Infosec Jupyterthon 2021`_ [`IJ'21 live hunt recording`_]
 - 2021/11 `BlackHat Europe 2021`_
 - 2021/10 `SANS Threat Hunting Summit 2021`_: [`SANS'21 session recording`_]
@@ -179,15 +183,15 @@
 
   - `Kestrel huntbook`_
   - `Kestrel analytics`_
 
 
 
 
-.. _Try Kestrel in a cloud sandbox without install: https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=tutorial
+.. _Kestrel live tutorial in a cloud sandbox: https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=tutorial
 .. _Kestrel documentation: https://kestrel.readthedocs.io/
 
 .. _A comprehensive introduction to Kestrel: https://kestrel.readthedocs.io/en/stable/overview/
 .. _The two key concepts of Kestrel: https://kestrel.readthedocs.io/en/stable/language/tac.html#key-concepts
 .. _Interactive tutorial with quiz: https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=tutorial
 .. _Kestrel runtime installation: https://kestrel.readthedocs.io/en/stable/installation/runtime.html
 .. _How to connect to your data sources: https://kestrel.readthedocs.io/en/stable/installation/datasource.html
@@ -213,17 +217,20 @@
 .. _BlackHat Europe 2021: https://www.blackhat.com/eu-21/arsenal/schedule/index.html#an-open-stack-for-threat-hunting-in-hybrid-cloud-with-connected-observability-25112
 .. _Infosec Jupyterthon 2021: https://infosecjupyterthon.com/2021/agenda.html
 .. _IJ'21 live hunt recording: https://www.youtube.com/embed/nMnHBnYfIaI?start=20557&end=22695
 .. _Infosec Jupyterthon 2022: https://infosecjupyterthon.com/2022/agenda.html
 .. _IJ'22 live hunt recording: https://www.youtube.com/embed/8Mw1yyYkeqM?start=23586&end=26545
 .. _SC eSummit on Threat Hunting & Offense Security: https://www.scmagazine.com/esummit/automating-the-hunt-for-advanced-threats
 .. _Cybersecurity Automation Workshop: http://www.cybersecurityautomationworkshop.org/
+.. _Black Hat USA 2023: https://www.blackhat.com/us-23/arsenal/schedule/index.html#identity-threat-hunting-with-kestrel-33662
 .. _Black Hat USA 2022: https://www.blackhat.com/us-22/arsenal/schedule/index.html#streamlining-and-automating-threat-hunting-with-kestrel-28014
 .. _BH'22 recording: https://www.youtube.com/watch?v=tf1VLIpFefs
+.. _Black Hat USA 2022 session recording: https://www.youtube.com/watch?v=tf1VLIpFefs
 .. _BH'22 hunting lab: https://mybinder.org/v2/gh/opencybersecurityalliance/black-hat-us-2022/HEAD?filepath=demo
+.. _Black Hat USA 2022 Kestrel hunting lab: https://mybinder.org/v2/gh/opencybersecurityalliance/black-hat-us-2022/HEAD?filepath=demo
 
 .. _slack invitation: https://join.slack.com/t/open-cybersecurity/shared_invite/zt-19pliofsm-L7eSSB8yzABM2Pls1nS12w
 .. _Open Cybersecurity Alliance workspace: https://open-cybersecurity.slack.com/
 .. _GitHub Issue: https://github.com/opencybersecurityalliance/kestrel-lang/issues
 .. _contributing guideline: CONTRIBUTING.rst
 .. _governance documentation: GOVERNANCE.rst
 .. _Apache License 2.0: LICENSE.md
```

### Comparing `kestrel-lang-1.7.0/README.rst` & `kestrel-lang-1.7.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -24,38 +24,41 @@
 
 .. image:: https://readthedocs.org/projects/kestrel/badge/?version=latest
         :target: https://kestrel.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 |
 
-**[News]** Kestrel hunt at `Infosec Jupyterthon 2022`_ [`IJ'22 live hunt recording`_]
-
-**[News]** Kestrel session at `Black Hat USA 2022`_ [`BH'22 recording`_ | `BH'22 hunting lab`_]
+**[News]** Kestrel session at `Black Hat USA 2023`_
 
 --------
 
 Kestrel is a threat hunting language aiming to make cyber threat hunting *fast*
 by providing a layer of abstraction to build reusable, composable, and
-shareable hunt-flow.
+shareable hunt-flow. Starting with:
+
+#. `Black Hat USA 2022 session recording`_
+#. `Black Hat USA 2022 Kestrel hunting lab`_
+#. `Kestrel live tutorial in a cloud sandbox`_
 
-`Try Kestrel in a cloud sandbox without install`_ (Blog: `Try Kestrel in a Cloud Sandbox`_).
+The Goal
+========
 
 Software developers write Python or Swift than machine code to quickly turn
 business logic into applications. Threat hunters write Kestrel to quickly turn
 threat hypotheses into hunt-flow. We see threat hunting as an interactive
 procedure to create customized intrusion detection systems on the fly, and
 hunt-flow is to hunts as control-flow is to ordinary programs.
 
 What does it mean by *hunt fast*?
 
-- Do not write the same TTP pattern in different data source queries.
-- Do not write one-time-use adapaters to connect hunt steps.
-- Do not waste your existing analytic scripts/programs in future hunts.
-- Do construct your hunt-flow from smaller reuseable hunt-flow.
+- Do NOT write the same TTP pattern in different data source queries.
+- Do NOT write one-time-use adapaters to connect hunt steps.
+- Do NOT waste your existing analytic scripts/programs in future hunts.
+- DD construct your hunt-flow from smaller reuseable hunt-flow.
 - Do share your huntbook with your future self and your colleagues.
 - Do get interactive feedback and revise hunt-flow on the fly.
 
 |
 
 .. image:: https://github.com/opencybersecurityalliance/data-bucket-kestrel/raw/main/images/github_homepage_animation.gif
    :width: 90%
@@ -124,14 +127,15 @@
 #. `Fun with securitydatasets.com and the Kestrel PowerShell Deobfuscator`_
 
 Talks And Demos
 ===============
 
 Talk summary (visit `Kestrel documentation on talks`_ to learn details):
 
+- 2023/08 `Black Hat USA 2023`_
 - 2022/12 `Infosec Jupyterthon 2022`_ [`IJ'22 live hunt recording`_]
 - 2022/08 `Black Hat USA 2022`_ [`BH'22 recording`_ | `BH'22 hunting lab`_]
 - 2022/06 `Cybersecurity Automation Workshop`_
 - 2022/04 `SC eSummit on Threat Hunting & Offense Security`_ (free to register/playback)
 - 2021/12 `Infosec Jupyterthon 2021`_ [`IJ'21 live hunt recording`_]
 - 2021/11 `BlackHat Europe 2021`_
 - 2021/10 `SANS Threat Hunting Summit 2021`_: [`SANS'21 session recording`_]
@@ -160,15 +164,15 @@
 
   - `Kestrel huntbook`_
   - `Kestrel analytics`_
 
 
 
 
-.. _Try Kestrel in a cloud sandbox without install: https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=tutorial
+.. _Kestrel live tutorial in a cloud sandbox: https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=tutorial
 .. _Kestrel documentation: https://kestrel.readthedocs.io/
 
 .. _A comprehensive introduction to Kestrel: https://kestrel.readthedocs.io/en/stable/overview/
 .. _The two key concepts of Kestrel: https://kestrel.readthedocs.io/en/stable/language/tac.html#key-concepts
 .. _Interactive tutorial with quiz: https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=tutorial
 .. _Kestrel runtime installation: https://kestrel.readthedocs.io/en/stable/installation/runtime.html
 .. _How to connect to your data sources: https://kestrel.readthedocs.io/en/stable/installation/datasource.html
@@ -194,17 +198,20 @@
 .. _BlackHat Europe 2021: https://www.blackhat.com/eu-21/arsenal/schedule/index.html#an-open-stack-for-threat-hunting-in-hybrid-cloud-with-connected-observability-25112
 .. _Infosec Jupyterthon 2021: https://infosecjupyterthon.com/2021/agenda.html
 .. _IJ'21 live hunt recording: https://www.youtube.com/embed/nMnHBnYfIaI?start=20557&end=22695
 .. _Infosec Jupyterthon 2022: https://infosecjupyterthon.com/2022/agenda.html
 .. _IJ'22 live hunt recording: https://www.youtube.com/embed/8Mw1yyYkeqM?start=23586&end=26545
 .. _SC eSummit on Threat Hunting & Offense Security: https://www.scmagazine.com/esummit/automating-the-hunt-for-advanced-threats
 .. _Cybersecurity Automation Workshop: http://www.cybersecurityautomationworkshop.org/
+.. _Black Hat USA 2023: https://www.blackhat.com/us-23/arsenal/schedule/index.html#identity-threat-hunting-with-kestrel-33662
 .. _Black Hat USA 2022: https://www.blackhat.com/us-22/arsenal/schedule/index.html#streamlining-and-automating-threat-hunting-with-kestrel-28014
 .. _BH'22 recording: https://www.youtube.com/watch?v=tf1VLIpFefs
+.. _Black Hat USA 2022 session recording: https://www.youtube.com/watch?v=tf1VLIpFefs
 .. _BH'22 hunting lab: https://mybinder.org/v2/gh/opencybersecurityalliance/black-hat-us-2022/HEAD?filepath=demo
+.. _Black Hat USA 2022 Kestrel hunting lab: https://mybinder.org/v2/gh/opencybersecurityalliance/black-hat-us-2022/HEAD?filepath=demo
 
 .. _slack invitation: https://join.slack.com/t/open-cybersecurity/shared_invite/zt-19pliofsm-L7eSSB8yzABM2Pls1nS12w
 .. _Open Cybersecurity Alliance workspace: https://open-cybersecurity.slack.com/
 .. _GitHub Issue: https://github.com/opencybersecurityalliance/kestrel-lang/issues
 .. _contributing guideline: CONTRIBUTING.rst
 .. _governance documentation: GOVERNANCE.rst
 .. _Apache License 2.0: LICENSE.md
```

### Comparing `kestrel-lang-1.7.0/setup.cfg` & `kestrel-lang-1.7.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kestrel-lang
-version = 1.7.0
+version = 1.7.1
 description = Kestrel Threat Hunting Language
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 keywords = 
 	domain specific language
 	cyber threat hunting
 	extended detection and response
@@ -31,17 +31,17 @@
 	lxml
 	pandas
 	requests
 	nest-asyncio>=1.5.6
 	lark>=1.1.5
 	pyarrow>=5.0.0
 	docker>=5.0.0
-	stix-shifter>=5.3.0
-	stix-shifter-utils>=5.3.0
-	firepit>=2.3.21
+	stix-shifter>=5.3.1
+	stix-shifter-utils>=5.3.1
+	firepit>=2.3.24
 	typeguard
 tests_require = 
 	pytest
 
 [options.packages.find]
 where = src
```

### Comparing `kestrel-lang-1.7.0/src/kestrel/__main__.py` & `kestrel-lang-1.7.1/src/kestrel/__main__.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/absinterface/manager.py` & `kestrel-lang-1.7.1/src/kestrel/absinterface/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/analytics/interface.py` & `kestrel-lang-1.7.1/src/kestrel/analytics/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/analytics/manager.py` & `kestrel-lang-1.7.1/src/kestrel/analytics/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/codegen/commands.py` & `kestrel-lang-1.7.1/src/kestrel/codegen/commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,44 +18,37 @@
 #     - a table that can be imported to pandas dataframe
 ################################################################
 
 import functools
 import logging
 import itertools
 from collections import OrderedDict
-from copy import deepcopy
 
 from firepit.deref import auto_deref
 from firepit.exceptions import InvalidAttr
 from firepit.query import Limit, Offset, Order, Predicate, Projection, Query
 from firepit.stix20 import summarize_pattern
 
-from kestrel.semantics.reference import make_deref_func, make_var_timerange_func
-from kestrel.utils import remove_empty_dicts, dedup_ordered_dicts, lowered_str_list
+from kestrel.utils import remove_empty_dicts, dedup_ordered_dicts
 from kestrel.exceptions import *
 from kestrel.symboltable.variable import new_var
-from kestrel.symboltable.symtable import SymbolTable
-from kestrel.syntax.parser import parse_ecgpattern
 from kestrel.syntax.utils import (
     get_entity_types,
     get_all_input_var_names,
-    timedelta_seconds,
 )
 from kestrel.codegen.data import load_data, load_data_file, dump_data_to_file
 from kestrel.codegen.display import DisplayDataframe, DisplayDict, DisplayWarning
-from kestrel.codegen.queries import (
-    compile_specific_relation_to_query,
-    compile_generic_relation_to_query,
-)
 from kestrel.codegen.relations import (
     generic_relations,
-    compile_identical_entity_search_pattern,
-    fine_grained_relational_process_filtering,
     get_entity_id_attribute,
-    build_pattern_from_ids,
+)
+from kestrel.codegen.prefetch import do_prefetch
+from kestrel.codegen.queries import (
+    compile_specific_relation_to_query,
+    compile_generic_relation_to_query,
 )
 
 _logger = logging.getLogger(__name__)
 
 
 ################################################################
 #                       Private Decorators
@@ -109,22 +102,15 @@
 
 @_debug_logger
 @_default_output
 def assign(stmt, session):
     entity_table = session.symtable[stmt["input"]].entity_table
     transform = stmt.get("transformer")
     if transform:
-        if transform.lower() == "timestamped":
-            qry = session.store.timestamped(entity_table, run=False)
-        elif transform.lower() == "addobsid":
-            qry = session.store.extract_observeddata_attribute(
-                entity_table, name_of_attribute="id", run=False
-            )
-        else:
-            qry = Query(entity_table)
+        qry = _transform_query(session.store, entity_table, transform)
     else:
         qry = Query(entity_table)
 
     qry = _build_query(session.store, entity_table, qry, stmt, [])
 
     try:
         session.store.assign_query(stmt["output"], qry)
@@ -216,22 +202,15 @@
 
 
 @_debug_logger
 def disp(stmt, session):
     entity_table = session.symtable[stmt["input"]].entity_table
     transform = stmt.get("transformer")
     if transform and entity_table:
-        if transform.lower() == "timestamped":
-            qry = session.store.timestamped(entity_table, run=False)
-        elif transform.lower() == "addobsid":
-            qry = session.store.extract_observeddata_attribute(
-                entity_table, name_of_attribute="id", run=False
-            )
-        else:
-            qry = Query(entity_table)
+        qry = _transform_query(session.store, entity_table, transform)
     else:
         qry = Query(entity_table)
 
     qry = _build_query(session.store, entity_table, qry, stmt)
     try:
         cursor = session.store.run_query(qry)
     except InvalidAttr as e:
@@ -246,253 +225,124 @@
 @_debug_logger
 @_default_output
 def get(stmt, session):
     pattern = stmt["stixpattern"]
     local_var_table = stmt["output"] + "_local"
     return_var_table = stmt["output"]
     return_type = stmt["type"]
-    start_offset = session.config["stixquery"]["timerange_start_offset"]
-    end_offset = session.config["stixquery"]["timerange_stop_offset"]
+    limit = stmt.get("limit")
     display = None
 
     if "variablesource" in stmt:
         input_type = session.symtable[stmt["variablesource"]].type
         output_type = stmt["type"]
         if input_type != output_type:
             raise InvalidECGPattern(
                 f"input variable type {input_type} does not match output type {output_type}"
             )
         session.store.filter(
-            stmt["output"],
-            stmt["type"],
+            return_var_table,
+            return_type,
             input_type,
             pattern,
         )
-        output = new_var(session.store, return_var_table, [], stmt, session.symtable)
         _logger.debug(f"get from variable source \"{stmt['variablesource']}\"")
 
     elif "datasource" in stmt:
         # rs: RetStruct
         rs = session.data_source_manager.query(
-            stmt["datasource"], pattern, session.session_id, session.store
+            stmt["datasource"], pattern, session.session_id, session.store, limit
         )
         query_id = rs.load_to_store(session.store)
         session.store.extract(local_var_table, return_type, query_id, pattern)
-        _output = new_var(session.store, local_var_table, [], stmt, session.symtable)
+        local_stage_varstruct = new_var(
+            session.store, local_var_table, [], stmt, session.symtable
+        )
         _logger.debug(
             f"native GET pattern executed and DB view {local_var_table} extracted."
         )
 
         # TODO: add a ECGP method to do this directly
         pat_summary = summarize_pattern(pattern)
 
+        local_stage_var_entity_id = get_entity_id_attribute(local_stage_varstruct)
         if (
             pat_summary
             and return_type in pat_summary  # allow extended subgraph
             and len(pat_summary[return_type]) == 1  # only one attr for center node
-            and pat_summary[return_type].pop() == get_entity_id_attribute(_output)
+            and pat_summary[return_type].pop() == local_stage_var_entity_id
         ):
             _logger.debug("To skip prefetch for direct query")
             is_direct_query = True
         else:
             is_direct_query = False
 
-        if (
-            not is_direct_query
-            and _is_prefetch_allowed_in_config(
-                session.config["prefetch"], "get", return_type
-            )
-            and len(_output)
-        ):
-            prefetch_ret_var_table = return_var_table + "_prefetch"
-            ext_graph_pattern = deepcopy(stmt["where"])
-            ext_graph_pattern.prune_away_centered_graph(return_type)
-            prefetch_ret_entity_table = _prefetch(
-                return_type,
-                prefetch_ret_var_table,
-                local_var_table,
-                stmt["timerange"],
-                start_offset,
-                end_offset,
-                SymbolTable({local_var_table: _output}),
-                session.store,
-                ext_graph_pattern,
-                session.session_id,
-                session.data_source_manager,
-                session.config["stixquery"]["support_id"],
-            )
-
-            if return_type == "process" and get_entity_id_attribute(_output) not in (
-                "id",
-                "x_unique_id",
-            ):
-                prefetch_ret_entity_table = _filter_prefetched_process(
-                    return_var_table,
-                    session,
-                    _output,
-                    prefetch_ret_entity_table,
-                    return_type,
-                )
-        else:
-            prefetch_ret_entity_table = None
-
-        if prefetch_ret_entity_table:
-            _logger.debug(
-                f"merge {local_var_table} and {prefetch_ret_entity_table} into {return_var_table}."
-            )
-            session.store.merge(
-                return_var_table, [local_var_table, prefetch_ret_entity_table]
-            )
-            for v in list(
-                set(
-                    [local_var_table, prefetch_ret_entity_table, prefetch_ret_var_table]
-                )
-            ):
-                if not session.debug_mode:
-                    _logger.debug(f"remove temp store view {v}.")
-                    session.store.remove_view(v)
-        else:
-            _logger.debug(
-                f'prefetch return None, just rename native GET pattern matching results into "{return_var_table}".'
-            )
-            session.store.rename_view(local_var_table, return_var_table)
-
-        output = new_var(session.store, return_var_table, [], stmt, session.symtable)
+        return_var_table = do_prefetch(
+            local_var_table, local_stage_varstruct, session, stmt, not is_direct_query
+        )
 
-        if not len(output):
-            if not return_type.startswith("x-") and return_type not in (
-                set(session.store.types()) | set(get_entity_types())
-            ):
-                display = DisplayWarning(f'unknown entity type "{return_type}"')
     else:
         raise KestrelInternalError(f"unknown type of source in {str(stmt)}")
 
+    output = new_var(session.store, return_var_table, [], stmt, session.symtable)
+
+    if not len(output):
+        if not return_type.startswith("x-") and return_type not in (
+            set(session.store.types()) | set(get_entity_types())
+        ):
+            display = DisplayWarning(f'unknown entity type "{return_type}"')
+
     return output, display
 
 
 @_debug_logger
 @_default_output
 @_guard_empty_input
 def find(stmt, session):
+    # shortcuts
     return_type = stmt["type"]
     input_type = session.symtable[stmt["input"]].type
-    input_var_name = stmt["input"]
-    return_var_table = stmt["output"]
     local_var_table = stmt["output"] + "_local"
-    relation = stmt["relation"]
-    is_reversed = stmt["reversed"]
-    start_offset = session.config["stixquery"]["timerange_start_offset"]
-    end_offset = session.config["stixquery"]["timerange_stop_offset"]
-    rel_query = None
 
-    if return_type not in session.store.types():
-        # return empty variable
-        output = new_var(session.store, None, [], stmt, session.symtable)
+    # init
+    rel_query = None
+    return_var_table = None
 
-    else:
-        _symtable = SymbolTable({input_var_name: session.symtable[input_var_name]})
+    if return_type in session.store.types():
         input_var_attrs = session.store.columns(input_type)
         return_type_attrs = session.store.columns(return_type)
 
         # First, get information from local store
-        if relation in generic_relations:
+        if stmt["relation"] in generic_relations:
             rel_query = compile_generic_relation_to_query(
-                return_type, input_type, session.symtable[input_var_name].entity_table
+                return_type, input_type, session.symtable[stmt["input"]].entity_table
             )
 
         else:
             rel_query = compile_specific_relation_to_query(
                 return_type,
-                relation,
+                stmt["relation"],
                 input_type,
-                is_reversed,
-                input_var_name,
+                stmt["reversed"],
+                stmt["input"],
                 input_var_attrs,
                 return_type_attrs,
             )
 
         # `session.store.assign_query` will generate new entity_table named `local_var_table`
         if rel_query:
             session.store.assign_query(local_var_table, rel_query, return_type)
-            _output = new_var(
+            local_stage_varstruct = new_var(
                 session.store, local_var_table, [], stmt, session.symtable
             )
+            return_var_table = do_prefetch(
+                local_var_table, local_stage_varstruct, session, stmt
+            )
 
-            # Second, prefetch all records of the entities and associated entities
-            if (
-                _is_prefetch_allowed_in_config(
-                    session.config["prefetch"], "find", return_type
-                )
-                and len(_output)
-                and _output.data_source
-            ):
-                prefetch_ret_var_table = return_var_table + "_prefetch"
-                ext_graph_pattern = stmt["where"] if "where" in stmt else None
-                prefetch_ret_entity_table = _prefetch(
-                    return_type,
-                    prefetch_ret_var_table,
-                    local_var_table,
-                    stmt["timerange"],
-                    start_offset,
-                    end_offset,
-                    SymbolTable({local_var_table: _output}),
-                    session.store,
-                    ext_graph_pattern,
-                    session.session_id,
-                    session.data_source_manager,
-                    session.config["stixquery"]["support_id"],
-                )
-
-                # special handling for process to filter out impossible relational processes
-                # this is needed since STIX 2.0 does not have mandatory fields for
-                # process and field like `pid` is not unique
-                if return_type == "process" and get_entity_id_attribute(
-                    _output
-                ) not in ("id", "x_unique_id"):
-                    prefetch_ret_entity_table = _filter_prefetched_process(
-                        return_var_table,
-                        session,
-                        _output,
-                        prefetch_ret_entity_table,
-                        return_type,
-                    )
-            else:
-                prefetch_ret_entity_table = None
-
-            if prefetch_ret_entity_table:
-                _logger.debug(
-                    f"merge {local_var_table} and {prefetch_ret_entity_table} into {return_var_table}."
-                )
-                session.store.merge(
-                    return_var_table, [local_var_table, prefetch_ret_entity_table]
-                )
-                for v in list(
-                    set(
-                        [
-                            local_var_table,
-                            prefetch_ret_entity_table,
-                            prefetch_ret_var_table,
-                        ]
-                    )
-                ):
-                    if not session.debug_mode:
-                        _logger.debug(f"remove temp store view {v}.")
-                        session.store.remove_view(v)
-            else:
-                _logger.debug(
-                    f'prefetch return None, just rename native GET pattern matching results into "{return_var_table}".'
-                )
-                session.store.rename_view(local_var_table, return_var_table)
-
-        else:
-            return_var_table = None
-            _logger.info(f'no relation "{relation}" on this dataset')
-
-        output = new_var(session.store, return_var_table, [], stmt, session.symtable)
-
+    output = new_var(session.store, return_var_table, [], stmt, session.symtable)
     return output, None
 
 
 @_debug_logger
 @_default_output
 @_guard_empty_input
 def join(stmt, session):
@@ -546,124 +396,14 @@
 
 
 ################################################################
 #                       Helper Functions
 ################################################################
 
 
-def _prefetch(
-    return_type,
-    return_var_name,
-    input_var_name,
-    time_range,
-    start_offset,
-    end_offset,
-    symtable,
-    store,
-    where_clause,
-    session_id,
-    ds_manager,
-    does_support_id,
-):
-    """prefetch identical entities and associated entities.
-
-    Put the input entities in the center of an observation and query the remote
-    data source of associated with input variable, so we get back:
-
-    1. all records about the input entities.
-
-    2. associated entities such as parent/child processes of processes, processes of network-traffic, etc.
-
-    The function does not have explicit return, but a side effect: a view in
-    the store named after `return_var_name`.
-
-    Args:
-        input_var_name (str): input variable name.
-
-        return_var_name (str): return variable name.
-
-        return_type (str): return entity type.
-
-        time_range ((datetime, datetime)).
-
-        start_offset (int): start time offset by seconds.
-
-        end_offset (int): end time offset by seconds.
-
-        symtable ({str:VarStruct}): should has ``input_var_name``.
-
-        store (firepit.SqlStorage): store.
-
-        where_clause (ExtCenteredGraphPattern): pattern to merge to the prefetch auto-gen pattern
-
-        session_id (str): session ID.
-
-        does_support_id (bool): whether "id" can be an attribute in data source query.
-
-    Returns:
-        str: the entity table in store if the prefetch is performed else None.
-    """
-
-    _logger.debug(f"prefetch {return_type} to extend {input_var_name}.")
-
-    pattern_raw = compile_identical_entity_search_pattern(
-        input_var_name, symtable[input_var_name], does_support_id
-    )
-
-    if pattern_raw:
-        pattern_ast = parse_ecgpattern(pattern_raw)
-        deref_func = make_deref_func(store, symtable)
-        get_timerange_func = make_var_timerange_func(store, symtable)
-        pattern_ast.deref(deref_func, get_timerange_func)
-        pattern_ast.add_center_entity(symtable[input_var_name].type)
-        time_adj = tuple(map(timedelta_seconds, (start_offset, end_offset)))
-        _logger.info(f"ext pattern in prefetch: {where_clause}")
-        _logger.info(f"prefetch pattern before extend: {pattern_ast}")
-        pattern_ast.extend("AND", where_clause)
-        _logger.info(f"prefetch pattern after extend: {pattern_ast}")
-        stix_pattern = pattern_ast.to_stix(time_range, time_adj)
-        _logger.info(f"STIX pattern generated in prefetch: {stix_pattern}")
-
-        if stix_pattern:
-            data_source = symtable[input_var_name].data_source
-            resp = ds_manager.query(data_source, stix_pattern, session_id, store)
-            query_id = resp.load_to_store(store)
-
-            # build the return_var_name view in store
-            store.extract(return_var_name, return_type, query_id, stix_pattern)
-
-            _logger.debug(f"prefetch successful.")
-            return return_var_name
-
-    _logger.info(f"prefetch return empty.")
-    return None
-
-
-def _filter_prefetched_process(
-    return_var_name, session, local_var, prefetched_entity_table, return_type
-):
-    _logger.debug(f"filter prefetched {return_type} for {prefetched_entity_table}.")
-
-    prefetch_filtered_var_name = return_var_name + "_prefetch_filtered"
-    entity_ids = fine_grained_relational_process_filtering(
-        local_var,
-        prefetched_entity_table,
-        session.store,
-        session.config["prefetch"]["process_identification"],
-    )
-    if entity_ids:
-        id_pattern = build_pattern_from_ids(return_type, entity_ids)
-        session.store.extract(prefetch_filtered_var_name, return_type, None, id_pattern)
-        _logger.debug("filter successful.")
-        return prefetch_filtered_var_name
-    else:
-        _logger.info("no prefetched process found after filtering.")
-        return None
-
-
 def _set_projection(store, entity_table, query, paths):
     joins, proj = auto_deref(store, entity_table, paths=paths)
     query.joins.extend(joins)
     joined = [j.name for j in query.joins]
     _logger.debug("%s: joining %s", query.table.name, joined)
     if query.proj:
         # Need to merge projections?  More-specific overrides less-specific ("*")
@@ -733,14 +473,28 @@
         qry.append(Limit(limit))
     offset = stmt.get("offset")
     if offset:
         qry.append(Offset(offset))
     return qry
 
 
-def _is_prefetch_allowed_in_config(pre_fetch_config, command_name, entity_type):
-    if pre_fetch_config["switch_per_command"][
-        command_name
-    ] and entity_type not in lowered_str_list(pre_fetch_config["excluded_entities"]):
-        return True
+def _transform_query(store, entity_table, transform):
+    if transform.lower() == "timestamped":
+        qry = store.timestamped(entity_table, run=False)
+    elif transform.lower() == "addobsid":
+        qry = store.extract_observeddata_attribute(
+            entity_table, name_of_attribute="id", run=False
+        )
+    elif transform.lower() == "records":
+        qry = store.extract_observeddata_attribute(
+            entity_table,
+            name_of_attribute=[
+                "number_observed",
+                "first_observed",
+                "last_observed",
+                "id",
+            ],
+            run=False,
+        )
     else:
-        return False
+        qry = Query(entity_table)
+    return qry
```

### Comparing `kestrel-lang-1.7.0/src/kestrel/codegen/data.py` & `kestrel-lang-1.7.1/src/kestrel/codegen/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import csv
 import json
 import pathlib
 import uuid
 
 import pandas as pd
 
 from kestrel.exceptions import MissingEntityType, NonUniformEntityType
@@ -51,15 +52,15 @@
     p = pathlib.Path(file_path)
     p.parent.mkdir(parents=True, exist_ok=True)
 
     input_data = store.lookup(input_entity_table) if input_entity_table else []
     df = pd.DataFrame(input_data)
     dump_format = _get_dump_format(p)
     if dump_format == "csv":
-        df.to_csv(file_path)
+        df.to_csv(file_path, index=False, quoting=csv.QUOTE_NONNUMERIC)
     elif dump_format == "parquet":
         df.to_parquet(file_path)
     elif dump_format == "json":
         data = df.to_json(orient="records")
         with open(file_path, "w") as output_file:
             output_file.write(data)
```

### Comparing `kestrel-lang-1.7.0/src/kestrel/codegen/display.py` & `kestrel-lang-1.7.1/src/kestrel/codegen/display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/codegen/queries.py` & `kestrel-lang-1.7.1/src/kestrel/codegen/queries.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/codegen/relations.py` & `kestrel-lang-1.7.1/src/kestrel/codegen/relations.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/codegen/summary.py` & `kestrel-lang-1.7.1/src/kestrel/codegen/summary.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/config.py` & `kestrel-lang-1.7.1/src/kestrel/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/config.yaml` & `kestrel-lang-1.7.1/src/kestrel/config.yaml`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/datasource/interface.py` & `kestrel-lang-1.7.1/src/kestrel/datasource/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             [str]: A list of data source names accessible from this interface.
 
         """
         return []
 
     @staticmethod
     @abstractmethod
-    def query(uri, pattern, session_id, config, store=None):
+    def query(uri, pattern, session_id, config, store=None, limit=None):
         """Sending a data query to a specific data source.
 
         If the store of the session is modified and directly gets the data
         loaded into a ``query_id``, it should return
         :attr:`kestrel.datasource.ReturnFromStore`.
 
         If the interface uses local files as intermediate/temporary storage
@@ -102,14 +102,17 @@
               directly writing into the store.
 
             config (dict): a layered list/dict that contains config for the
               interface and can be edited/updated by the interface.
 
             store (firepit.SqlStorage): The internal store used by the session
 
+            limit (Optional[int]): limit on the number of records to return;
+              None if there is no limit
+
         Returns:
             kestrel.datasource.retstruct.AbstractReturnStruct: returned data.
             Currently there are two choices:
             :attr:`kestrel.datasource.ReturnFromFile` and
             :attr:`kestrel.datasource.ReturnFromStore`.
 
         """
```

### Comparing `kestrel-lang-1.7.0/src/kestrel/datasource/manager.py` & `kestrel-lang-1.7.1/src/kestrel/datasource/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,13 +23,13 @@
         # important state keeper, required in Session()
         self.queried_data_sources = [None]
 
     def list_data_sources_from_scheme(self, scheme):
         i, c = self._get_interface_with_config(scheme)
         return i.list_data_sources(c)
 
-    def query(self, uri, pattern, session_id, store):
+    def query(self, uri, pattern, session_id, store, limit=None):
         scheme, uri = self._parse_and_complete_uri(uri)
         i, c = self._get_interface_with_config(scheme)
-        rs = i.query(uri, pattern, session_id, c, store)
+        rs = i.query(uri, pattern, session_id, c, store, limit)
         self.queried_data_sources.append(uri)
         return rs
```

### Comparing `kestrel-lang-1.7.0/src/kestrel/datasource/retstruct.py` & `kestrel-lang-1.7.1/src/kestrel/datasource/retstruct.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/exceptions.py` & `kestrel-lang-1.7.1/src/kestrel/exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/semantics/completor.py` & `kestrel-lang-1.7.1/src/kestrel/semantics/completor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/semantics/processor.py` & `kestrel-lang-1.7.1/src/kestrel/semantics/processor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/semantics/reference.py` & `kestrel-lang-1.7.1/src/kestrel/semantics/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/session.py` & `kestrel-lang-1.7.1/src/kestrel/session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/symboltable/variable.py` & `kestrel-lang-1.7.1/src/kestrel/symboltable/variable.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/syntax/ecgpattern.py` & `kestrel-lang-1.7.1/src/kestrel/syntax/ecgpattern.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/syntax/kestrel.lark` & `kestrel-lang-1.7.1/src/kestrel/syntax/kestrel.lark`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
                   | info
                   | save
 
 //
 // All commands
 //
 
-find: "FIND"i ENTITY_TYPE RELATION (REVERSED)? VARIABLE where_clause? timespan?
+find: "FIND"i ENTITY_TYPE RELATION (REVERSED)? VARIABLE where_clause? limit_clause? timespan?
 
-get: "GET"i ENTITY_TYPE ("FROM"i datasource)? where_clause timespan?
+get: "GET"i ENTITY_TYPE ("FROM"i datasource)? where_clause limit_clause? timespan?
 
 group: "GROUP"i VARIABLE BY grp_spec ("WITH"i agg_list)?
 
 join: "JOIN"i VARIABLE "," VARIABLE (BY ATTRIBUTE "," ATTRIBUTE)?
 
 load: "LOAD"i stdpath ("AS"i ENTITY_TYPE)?
 
@@ -75,18 +75,19 @@
 // not use rule name `transform` since it is a special function in Lark
 // the function in transformer will mal-function in `merge_transformers()`
 vtrans: transformer "(" VARIABLE ")"
       | VARIABLE
 
 transformer: TIMESTAMPED
            | ADDOBSID
+           | RECORDS
 
 TIMESTAMPED: "TIMESTAMPED"i
-
 ADDOBSID: "ADDOBSID"i
+RECORDS: "RECORDS"i
 
 where_clause: "WHERE"i ecg_pattern
 attr_clause: "ATTR"i ATTRIBUTES
 sort_clause: "SORT"i BY ATTRIBUTE (ASC|DESC)?
 limit_clause: "LIMIT"i INT
 offset_clause: "OFFSET"i INT
```

### Comparing `kestrel-lang-1.7.0/src/kestrel/syntax/parser.py` & `kestrel-lang-1.7.1/src/kestrel/syntax/parser.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/syntax/reference.py` & `kestrel-lang-1.7.1/src/kestrel/syntax/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel/syntax/utils.py` & `kestrel-lang-1.7.1/src/kestrel/syntax/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     stix_2_0_ref_mapping,
     stix_2_0_identical_mapping,
 )
 
 LITERALS = {"CNAME", "LETTER", "DIGIT", "WS", "INT", "WORD", "ESCAPED_STRING", "NUMBER"}
 AGG_FUNCS = {"MIN", "MAX", "AVG", "SUM", "COUNT", "NUNIQUE"}
 EXPRESSION_OPTIONS = {"WHERE", "ATTR", "SORT", "LIMIT", "OFFSET"}
-TRANSFORMS = {"TIMESTAMPED", "ADDOBSID"}
+TRANSFORMS = {"TIMESTAMPED", "ADDOBSID", "RECORDS"}
 
 
 def get_keywords():
     grammar = get_data(__name__, "kestrel.lark").decode("utf-8")
     parser = Lark(grammar, parser="lalr")
     alphabet_patterns = filter(lambda x: x.pattern.value.isalnum(), parser.terminals)
     keywords = [x.pattern.value for x in alphabet_patterns] + all_relations
```

### Comparing `kestrel-lang-1.7.0/src/kestrel/utils.py` & `kestrel-lang-1.7.1/src/kestrel/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 
 
 def lowered_str_list(xs):
     return [x.lower() for x in xs if isinstance(x, str)]
 
 
 def update_nested_dict(dict_old, dict_new):
-    for k, v in dict_new.items():
-        if isinstance(v, collections.abc.Mapping) and k in dict_old:
-            dict_old[k] = update_nested_dict(dict_old[k], v)
-        else:
-            dict_old[k] = v
+    if dict_new:
+        for k, v in dict_new.items():
+            if isinstance(v, collections.abc.Mapping) and k in dict_old:
+                dict_old[k] = update_nested_dict(dict_old[k], v)
+            else:
+                dict_old[k] = v
     return dict_old
 
 
 def remove_empty_dicts(ds):
     # remove dict with all values as None in list({string:string})
     # this is the results from SQL query
     return [d for d in ds if set(d.values()) != {None}]
```

### Comparing `kestrel-lang-1.7.0/src/kestrel_analytics_docker/config.py` & `kestrel-lang-1.7.1/src/kestrel_analytics_docker/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel_analytics_docker/interface.py` & `kestrel-lang-1.7.1/src/kestrel_analytics_docker/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel_analytics_python/config.py` & `kestrel-lang-1.7.1/src/kestrel_analytics_python/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel_analytics_python/interface.py` & `kestrel-lang-1.7.1/src/kestrel_analytics_python/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel_datasource_stixbundle/interface.py` & `kestrel-lang-1.7.1/src/kestrel_datasource_stixbundle/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     @staticmethod
     def list_data_sources(config=None):
         """This interface does not list data sources."""
         return []
 
     @staticmethod
-    def query(uri, pattern, session_id=None, config=None, store=None):
+    def query(uri, pattern, session_id=None, config=None, store=None, limit=None):
         """Query a STIX bundle locally or remotely."""
 
         _logger.debug(f"query URI received at interface_stixbundle: {uri}")
 
         scheme, _, data_paths = uri.rpartition("://")
         data_paths = data_paths.split(",")
         pattern = fixup_pattern(pattern)
@@ -81,14 +81,15 @@
         try:
             ingestdir = _make_query_dir(query_id)
         except FileExistsError:
             # We already cached this bundle
             data_paths = []
 
         bundles = []
+        num_records = 0
         for i, data_path in enumerate(data_paths):
             _logger.debug(f"requesting data from path: {data_path}")
 
             if scheme == "file":
                 rawfile = data_path
                 try:
                     with open(data_path, "r") as f:
@@ -159,16 +160,21 @@
                 if prop == "objects":
                     bundle_out[prop] = []
                     for obj in val:
                         count += 1
                         if obj["type"] != "observed-data" or compiled_pattern.match(
                             [obj], False
                         ):
-                            bundle_out[prop].append(obj)
                             matched += 1
+                            if obj["type"] == "observed-data":
+                                num_records += 1
+                                if not limit or num_records <= limit:
+                                    bundle_out[prop].append(obj)
+                            else:
+                                bundle_out[prop].append(obj)
                 else:
                     bundle_out[prop] = val
             _logger.debug("Matched %d of %d observations: %s", matched, count, rawfile)
 
             ingestfile = ingestdir / f"{i}.json"
             with ingestfile.open("w") as f:
                 json.dump(bundle_out, f)
```

### Comparing `kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/config.py` & `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/connector.py` & `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,17 @@
     package_w_ver = package_name + "==" + package_version
     _logger.info(
         f"{package_name} version {package_version} is different "
         f"from stix-shifter version {stixshifter_version}."
     )
     _logger.info(f'uninstalling Python package "{package_w_ver}".')
     try:
-        subprocess.check_call([sys.executable, "-m", "pip", "uninstall", package_w_ver])
+        subprocess.check_call(
+            [sys.executable, "-m", "pip", "uninstall", "--yes", package_w_ver]
+        )
     except:
         _logger.info(f"failed to uninstall package {package_w_ver}")
     install_package(connector_name)
 
 
 def check_module_availability(connector_name):
     try:
```

### Comparing `kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/interface.py` & `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,11 +121,11 @@
         config["profiles"] = load_profiles()
 
         data_sources = list(config["profiles"].keys())
         data_sources.sort()
         return data_sources
 
     @staticmethod
-    def query(uri, pattern, session_id, config, store):
+    def query(uri, pattern, session_id, config, store, limit=None):
         """Query a stixshifter data source."""
 
-        return query_datasource(uri, pattern, session_id, config, store)
+        return query_datasource(uri, pattern, session_id, config, store, limit)
```

### Comparing `kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/multiproc.py` & `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/multiproc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 from typing import Optional
 from typeguard import typechecked
 from contextlib import contextmanager
 from multiprocessing import Queue
 
-from kestrel.exceptions import DataSourceManagerInternalError
+from kestrel.exceptions import DataSourceError, DataSourceManagerInternalError
 from kestrel_datasource_stixshifter.worker.transmitter import TransmitterPool
 from kestrel_datasource_stixshifter.worker.translator import Translator
+from kestrel_datasource_stixshifter.worker import STOP_SIGN
 
 
 _logger = logging.getLogger(__name__)
 
 
 @contextmanager
 @typechecked
@@ -18,24 +19,26 @@
     connector_name: str,
     connection_dict: dict,
     configuration_dict: dict,
     retrieval_batch_size: int,
     translators_count: int,
     queries: list,
     raw_records_queue: Queue,
+    limit: Optional[int],
 ):
     _logger.debug(f"{translators_count} translation workers to be started")
     transmitter_pool = TransmitterPool(
         connector_name,
         connection_dict,
         configuration_dict,
         retrieval_batch_size,
         translators_count,
         queries,
         raw_records_queue,
+        limit,
     )
 
     try:
         transmitter_pool.start()
         yield transmitter_pool
     finally:
         transmitter_pool.join(2)
@@ -78,7 +81,27 @@
     finally:
         for translator in translators:
             translator.join(1)
             if translator.is_alive():
                 raise DataSourceManagerInternalError(
                     f"one or more translators do not terminate in interface {__package__}"
                 )
+
+
+@typechecked
+def read_translated_results(queue: Queue, translator_cnt: int):
+    for _ in range(translator_cnt):
+        for packet in iter(queue.get, STOP_SIGN):
+            if packet.success:
+                yield packet.data
+            else:
+                log_msg = f"[worker: {packet.worker}] {packet.log.log}"
+                if packet.log.level == logging.ERROR:
+                    _logger.debug(log_msg)
+                    raise DataSourceError(log_msg)
+                else:
+                    if packet.log.level == logging.WARN:
+                        _logger.warn(log_msg)
+                    elif packet.log.level == logging.INFO:
+                        _logger.info(log_msg)
+                    else:  # all others as debug logs
+                        _logger.debug(log_msg)
```

### Comparing `kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/query.py` & `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/query.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from pandas import DataFrame
 from multiprocessing import Queue
 
 from kestrel.datasource import ReturnFromStore
 from kestrel.utils import mkdtemp
 from kestrel.exceptions import DataSourceError, DataSourceManagerInternalError
 from kestrel_datasource_stixshifter.connector import check_module_availability
-from kestrel_datasource_stixshifter.worker import STOP_SIGN
 from kestrel_datasource_stixshifter import multiproc
 from kestrel_datasource_stixshifter.config import (
     get_datasource_from_profiles,
     load_options,
     load_profiles,
     set_stixshifter_logging_level,
 )
@@ -31,15 +30,15 @@
 
 nest_asyncio.apply()
 
 
 _logger = logging.getLogger(__name__)
 
 
-def query_datasource(uri, pattern, session_id, config, store):
+def query_datasource(uri, pattern, session_id, config, store, limit=None):
     # CONFIG command is not supported
     # profiles will be updated according to YAML file and env var
     config["profiles"] = load_profiles()
 
     config["options"] = load_options()
 
     _logger.debug(
@@ -59,17 +58,25 @@
     # however, the directory guarantees unique and non-exist query ID
     # so it always needs to be created
     cache_dir = mkdtemp()
     query_id = cache_dir.name
 
     _logger.debug(f"prepare query with ID: {query_id}")
 
+    num_records = 0
+    profile_limit = limit
+
     for profile in profiles:
+        if limit:
+            if num_records >= limit:
+                break
+            if num_records > 0:
+                profile_limit = limit - num_records
         _logger.debug(f"entering stix-shifter data source: {profile}")
-
+        _logger.debug(f"profile = {profile}, profile_limit = {profile_limit}")
         # STIX-shifter will alter the config objects, thus making them not reusable.
         # So only give STIX-shifter a copy of the configs.
         # Check `modernize` functions in the `stix_shifter_utils` for details.
         (
             connector_name,
             connection_dict,
             configuration_dict,
@@ -91,14 +98,16 @@
         dsl = translate_query(
             connector_name, observation_metadata, pattern, connection_dict
         )
 
         raw_records_queue = Queue()
         translated_data_queue = Queue()
 
+        exceptions = []
+
         with multiproc.translate(
             connector_name,
             observation_metadata,
             connection_dict.get("options", {}),
             cache_data_path_prefix,
             connector_name in config["options"]["fast_translate"],
             raw_records_queue,
@@ -109,21 +118,22 @@
                 connector_name,
                 connection_dict,
                 configuration_dict,
                 retrieval_batch_size,
                 config["options"]["translation_workers_count"],
                 dsl["queries"],
                 raw_records_queue,
+                profile_limit,
             ):
-                for _ in range(config["options"]["translation_workers_count"]):
-                    for packet in iter(translated_data_queue.get, STOP_SIGN):
-                        if packet.success:
-                            ingest(packet.data, observation_metadata, query_id, store)
-                        else:
-                            process_log_msg(packet)
+                for result in multiproc.read_translated_results(
+                    translated_data_queue,
+                    config["options"]["translation_workers_count"],
+                ):
+                    num_records += get_num_objects(result)
+                    ingest(result, observation_metadata, query_id, store)
 
     return ReturnFromStore(query_id)
 
 
 @typechecked
 def gen_observation_metadata(connector_name: str, query_id: str):
     return {
@@ -181,19 +191,16 @@
         )
     else:
         # STIX bundle (normal stix-shifter translation result)
         store.cache(query_id, result)
     _logger.debug("ingestion of a batch/page ends")
 
 
-def process_log_msg(packet):
-    log_msg = f"[worker: {packet.worker}] {packet.log.log}"
-    if packet.log.level == logging.ERROR:
-        _logger.debug(log_msg)
-        raise DataSourceError(log_msg)
+@typechecked
+def get_num_objects(data: Union[dict, DataFrame]):
+    if isinstance(data, DataFrame):
+        num_objects = len(data)
     else:
-        if packet.log.level == logging.WARN:
-            _logger.warn(log_msg)
-        elif packet.log.level == logging.INFO:
-            _logger.info(log_msg)
-        else:  #  all others as debug logs
-            _logger.debug(log_msg)
+        num_objects = len(data.get("objects", []))
+        if num_objects > 0:
+            num_objects -= 1  # minus the identify object
+    return num_objects
```

### Comparing `kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/translator.py` & `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/translator.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,50 +67,50 @@
                         try:
                             dataframe = firepit.aio.ingest.translate(
                                 mapping["to_stix_map"],
                                 transformers,
                                 input_batch.data,
                                 self.observation_metadata,
                             )
-                        except e:
+                        except Exception as e:
                             packet = TranslationResult(
                                 worker_name,
                                 False,
                                 None,
                                 WorkerLog(
-                                    logging.Error,
-                                    str(e),
+                                    logging.ERROR,
+                                    f"firepit.aio.ingest.translate() failed with msg: {str(e)}",
                                 ),
                             )
                         else:
                             packet = TranslationResult(
                                 worker_name,
                                 True,
                                 dataframe,
                                 None,
                             )
 
-                    if self.cache_data_path_prefix:
-                        debug_df_filepath = self.get_cache_data_path(
-                            input_batch.offset,
-                            "parquet",
-                        )
-                        try:
-                            dataframe.to_parquet(debug_df_filepath)
-                        except:
-                            packet_extra = TranslationResult(
-                                worker_name,
-                                False,
-                                None,
-                                WorkerLog(
-                                    logging.ERROR,
-                                    f"STIX-shifter fast translation parquet write to disk failed",
-                                ),
-                            )
-                            self.output_queue.put(packet_extra)
+                            if self.cache_data_path_prefix:
+                                debug_df_filepath = self.get_cache_data_path(
+                                    input_batch.offset,
+                                    "parquet",
+                                )
+                                try:
+                                    dataframe.to_parquet(debug_df_filepath)
+                                except Exception as e:
+                                    packet_extra = TranslationResult(
+                                        worker_name,
+                                        False,
+                                        None,
+                                        WorkerLog(
+                                            logging.ERROR,
+                                            f"STIX-shifter fast translation parquet write to disk failed: [{type(e).__name__}] {e}",
+                                        ),
+                                    )
+                                    self.output_queue.put(packet_extra)
 
                 else:
                     stixbundle = translation.translate(
                         self.connector_name,
                         "results",
                         self.observation_metadata,
                         input_batch.data,
```

### Comparing `kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/transmitter.py` & `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/transmitter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 import logging
 from multiprocessing import Process, Queue, current_process
+from typing import Optional
 from typeguard import typechecked
 
 from stix_shifter.stix_transmission import stix_transmission
 from kestrel_datasource_stixshifter.worker import STOP_SIGN
 from kestrel_datasource_stixshifter.worker.utils import TransmissionResult, WorkerLog
 
 
@@ -15,34 +16,37 @@
         connector_name: str,
         connection_dict: dict,
         configuration_dict: dict,
         retrieval_batch_size: int,
         number_of_translators: int,
         queries: list,
         output_queue: Queue,
+        limit: Optional[int],
     ):
         super().__init__()
 
         self.connector_name = connector_name
         self.connection_dict = connection_dict
         self.configuration_dict = configuration_dict
         self.retrieval_batch_size = retrieval_batch_size
         self.number_of_translators = number_of_translators
         self.queries = queries
         self.queue = output_queue
+        self.limit = limit
 
     def run(self):
         transmitters = [
             Transmitter(
                 self.connector_name,
                 self.connection_dict,
                 self.configuration_dict,
                 self.retrieval_batch_size,
                 query,
                 self.queue,
+                self.limit,
             )
             for query in self.queries
         ]
         for transmitter in transmitters:
             transmitter.start()
         for transmitter in transmitters:
             transmitter.join()
@@ -55,32 +59,35 @@
         self,
         connector_name: str,
         connection_dict: dict,
         configuration_dict: dict,
         retrieval_batch_size: int,
         query: str,
         output_queue: Queue,
+        limit: Optional[int],
     ):
         super().__init__()
 
         self.connector_name = connector_name
         self.connection_dict = connection_dict
         self.configuration_dict = configuration_dict
         self.retrieval_batch_size = retrieval_batch_size
         self.query = query
         self.queue = output_queue
+        self.limit = limit
 
     def run(self):
         self.worker_name = current_process().name
         self.transmission = stix_transmission.StixTransmission(
             self.connector_name,
             self.connection_dict,
             self.configuration_dict,
         )
         search_meta_result = self.transmission.query(self.query)
+
         if search_meta_result["success"]:
             self.search_id = search_meta_result["search_id"]
             if self.wait_datasource_search():
                 # no error so far
                 self.retrieve_data()
         else:
             err_msg = (
@@ -88,14 +95,15 @@
                 if "error" in search_meta_result
                 else "details not avaliable"
             )
             packet = TransmissionResult(
                 self.worker_name,
                 False,
                 None,
+                None,
                 WorkerLog(
                     logging.ERROR,
                     f"STIX-shifter transmission.query() failed: {err_msg}",
                 ),
             )
             self.queue.put(packet)
 
@@ -115,36 +123,39 @@
                 err_msg = (
                     status["error"] if "error" in status else "details not avaliable"
                 )
                 packet = TransmissionResult(
                     self.worker_name,
                     False,
                     None,
+                    None,
                     WorkerLog(
                         logging.ERROR,
                         f"STIX-shifter transmission.status() failed: {err_msg}",
                     ),
                 )
                 self.queue.put(packet)
                 return False
         return True
 
     def retrieve_data(self):
         result_retrieval_offset = 0
         has_remaining_results = True
         metadata = None
         is_retry_cycle = False
+        batch_size = self.retrieval_batch_size
+        if self.limit and self.limit < self.retrieval_batch_size:
+            batch_size = self.limit
 
         while has_remaining_results:
             packet = None
-
             result_batch = self.transmission.results(
                 self.search_id,
                 result_retrieval_offset,
-                self.retrieval_batch_size,
+                batch_size,
                 metadata,
             )
 
             if result_batch["success"]:
                 if result_batch["data"]:
                     packet = TransmissionResult(
                         self.worker_name,
@@ -155,14 +166,21 @@
                     )
 
                     # prepare for next round retrieval
                     result_retrieval_offset += len(result_batch["data"])
                     if "metadata" in result_batch:
                         metadata = result_batch["metadata"]
 
+                    if self.limit:
+                        if result_retrieval_offset >= self.limit:
+                            has_remaining_results = False
+                        else:
+                            batch_size = self.limit - result_retrieval_offset
+                            if batch_size > self.retrieval_batch_size:
+                                batch_size = self.retrieval_batch_size
                 else:
                     has_remaining_results = False
 
                 is_retry_cycle = False
 
             else:
                 err_msg = (
@@ -200,10 +218,11 @@
                         None,
                         None,
                         WorkerLog(
                             logging.ERROR,
                             f"STIX-shifter transmission.result() failed: {err_msg}",
                         ),
                     )
+                    has_remaining_results = False
 
             if packet:
                 self.queue.put(packet)
```

### Comparing `kestrel-lang-1.7.0/src/kestrel_datasource_stixshifter/worker/utils.py` & `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/src/kestrel_lang.egg-info/PKG-INFO` & `kestrel-lang-1.7.1/src/kestrel_lang.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.7.0
+Version: 1.7.1
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
@@ -43,38 +43,41 @@
 
 .. image:: https://readthedocs.org/projects/kestrel/badge/?version=latest
         :target: https://kestrel.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 |
 
-**[News]** Kestrel hunt at `Infosec Jupyterthon 2022`_ [`IJ'22 live hunt recording`_]
-
-**[News]** Kestrel session at `Black Hat USA 2022`_ [`BH'22 recording`_ | `BH'22 hunting lab`_]
+**[News]** Kestrel session at `Black Hat USA 2023`_
 
 --------
 
 Kestrel is a threat hunting language aiming to make cyber threat hunting *fast*
 by providing a layer of abstraction to build reusable, composable, and
-shareable hunt-flow.
+shareable hunt-flow. Starting with:
+
+#. `Black Hat USA 2022 session recording`_
+#. `Black Hat USA 2022 Kestrel hunting lab`_
+#. `Kestrel live tutorial in a cloud sandbox`_
 
-`Try Kestrel in a cloud sandbox without install`_ (Blog: `Try Kestrel in a Cloud Sandbox`_).
+The Goal
+========
 
 Software developers write Python or Swift than machine code to quickly turn
 business logic into applications. Threat hunters write Kestrel to quickly turn
 threat hypotheses into hunt-flow. We see threat hunting as an interactive
 procedure to create customized intrusion detection systems on the fly, and
 hunt-flow is to hunts as control-flow is to ordinary programs.
 
 What does it mean by *hunt fast*?
 
-- Do not write the same TTP pattern in different data source queries.
-- Do not write one-time-use adapaters to connect hunt steps.
-- Do not waste your existing analytic scripts/programs in future hunts.
-- Do construct your hunt-flow from smaller reuseable hunt-flow.
+- Do NOT write the same TTP pattern in different data source queries.
+- Do NOT write one-time-use adapaters to connect hunt steps.
+- Do NOT waste your existing analytic scripts/programs in future hunts.
+- DD construct your hunt-flow from smaller reuseable hunt-flow.
 - Do share your huntbook with your future self and your colleagues.
 - Do get interactive feedback and revise hunt-flow on the fly.
 
 |
 
 .. image:: https://github.com/opencybersecurityalliance/data-bucket-kestrel/raw/main/images/github_homepage_animation.gif
    :width: 90%
@@ -143,14 +146,15 @@
 #. `Fun with securitydatasets.com and the Kestrel PowerShell Deobfuscator`_
 
 Talks And Demos
 ===============
 
 Talk summary (visit `Kestrel documentation on talks`_ to learn details):
 
+- 2023/08 `Black Hat USA 2023`_
 - 2022/12 `Infosec Jupyterthon 2022`_ [`IJ'22 live hunt recording`_]
 - 2022/08 `Black Hat USA 2022`_ [`BH'22 recording`_ | `BH'22 hunting lab`_]
 - 2022/06 `Cybersecurity Automation Workshop`_
 - 2022/04 `SC eSummit on Threat Hunting & Offense Security`_ (free to register/playback)
 - 2021/12 `Infosec Jupyterthon 2021`_ [`IJ'21 live hunt recording`_]
 - 2021/11 `BlackHat Europe 2021`_
 - 2021/10 `SANS Threat Hunting Summit 2021`_: [`SANS'21 session recording`_]
@@ -179,15 +183,15 @@
 
   - `Kestrel huntbook`_
   - `Kestrel analytics`_
 
 
 
 
-.. _Try Kestrel in a cloud sandbox without install: https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=tutorial
+.. _Kestrel live tutorial in a cloud sandbox: https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=tutorial
 .. _Kestrel documentation: https://kestrel.readthedocs.io/
 
 .. _A comprehensive introduction to Kestrel: https://kestrel.readthedocs.io/en/stable/overview/
 .. _The two key concepts of Kestrel: https://kestrel.readthedocs.io/en/stable/language/tac.html#key-concepts
 .. _Interactive tutorial with quiz: https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=tutorial
 .. _Kestrel runtime installation: https://kestrel.readthedocs.io/en/stable/installation/runtime.html
 .. _How to connect to your data sources: https://kestrel.readthedocs.io/en/stable/installation/datasource.html
@@ -213,17 +217,20 @@
 .. _BlackHat Europe 2021: https://www.blackhat.com/eu-21/arsenal/schedule/index.html#an-open-stack-for-threat-hunting-in-hybrid-cloud-with-connected-observability-25112
 .. _Infosec Jupyterthon 2021: https://infosecjupyterthon.com/2021/agenda.html
 .. _IJ'21 live hunt recording: https://www.youtube.com/embed/nMnHBnYfIaI?start=20557&end=22695
 .. _Infosec Jupyterthon 2022: https://infosecjupyterthon.com/2022/agenda.html
 .. _IJ'22 live hunt recording: https://www.youtube.com/embed/8Mw1yyYkeqM?start=23586&end=26545
 .. _SC eSummit on Threat Hunting & Offense Security: https://www.scmagazine.com/esummit/automating-the-hunt-for-advanced-threats
 .. _Cybersecurity Automation Workshop: http://www.cybersecurityautomationworkshop.org/
+.. _Black Hat USA 2023: https://www.blackhat.com/us-23/arsenal/schedule/index.html#identity-threat-hunting-with-kestrel-33662
 .. _Black Hat USA 2022: https://www.blackhat.com/us-22/arsenal/schedule/index.html#streamlining-and-automating-threat-hunting-with-kestrel-28014
 .. _BH'22 recording: https://www.youtube.com/watch?v=tf1VLIpFefs
+.. _Black Hat USA 2022 session recording: https://www.youtube.com/watch?v=tf1VLIpFefs
 .. _BH'22 hunting lab: https://mybinder.org/v2/gh/opencybersecurityalliance/black-hat-us-2022/HEAD?filepath=demo
+.. _Black Hat USA 2022 Kestrel hunting lab: https://mybinder.org/v2/gh/opencybersecurityalliance/black-hat-us-2022/HEAD?filepath=demo
 
 .. _slack invitation: https://join.slack.com/t/open-cybersecurity/shared_invite/zt-19pliofsm-L7eSSB8yzABM2Pls1nS12w
 .. _Open Cybersecurity Alliance workspace: https://open-cybersecurity.slack.com/
 .. _GitHub Issue: https://github.com/opencybersecurityalliance/kestrel-lang/issues
 .. _contributing guideline: CONTRIBUTING.rst
 .. _governance documentation: GOVERNANCE.rst
 .. _Apache License 2.0: LICENSE.md
```

### Comparing `kestrel-lang-1.7.0/src/kestrel_lang.egg-info/SOURCES.txt` & `kestrel-lang-1.7.1/src/kestrel_lang.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/kestrel/analytics/__init__.py
 src/kestrel/analytics/interface.py
 src/kestrel/analytics/manager.py
 src/kestrel/codegen/__init__.py
 src/kestrel/codegen/commands.py
 src/kestrel/codegen/data.py
 src/kestrel/codegen/display.py
+src/kestrel/codegen/prefetch.py
 src/kestrel/codegen/queries.py
 src/kestrel/codegen/relations.py
 src/kestrel/codegen/summary.py
 src/kestrel/datasource/__init__.py
 src/kestrel/datasource/interface.py
 src/kestrel/datasource/manager.py
 src/kestrel/datasource/retstruct.py
@@ -79,11 +80,12 @@
 tests/test_command_save.py
 tests/test_completion.py
 tests/test_display.py
 tests/test_exceptions.py
 tests/test_expressions.py
 tests/test_parser.py
 tests/test_python_analytics.py
+tests/test_records.py
 tests/test_session.py
 tests/test_stixshifter.py
 tests/test_stixshifter_translator.py
 tests/test_timestamped.py
```

### Comparing `kestrel-lang-1.7.0/tests/test_cli.py` & `kestrel-lang-1.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_command_assign.py` & `kestrel-lang-1.7.1/tests/test_command_assign.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_command_disp.py` & `kestrel-lang-1.7.1/tests/test_command_disp.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_command_group.py` & `kestrel-lang-1.7.1/tests/test_command_group.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_command_join.py` & `kestrel-lang-1.7.1/tests/test_command_join.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_command_load.py` & `kestrel-lang-1.7.1/tests/test_command_load.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_command_merge.py` & `kestrel-lang-1.7.1/tests/test_command_merge.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_command_new.py` & `kestrel-lang-1.7.1/tests/test_command_new.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_command_save.py` & `kestrel-lang-1.7.1/tests/test_command_save.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_completion.py` & `kestrel-lang-1.7.1/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_display.py` & `kestrel-lang-1.7.1/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_exceptions.py` & `kestrel-lang-1.7.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_expressions.py` & `kestrel-lang-1.7.1/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_parser.py` & `kestrel-lang-1.7.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_python_analytics.py` & `kestrel-lang-1.7.1/tests/test_python_analytics.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_session.py` & `kestrel-lang-1.7.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_stixshifter.py` & `kestrel-lang-1.7.1/tests/test_stixshifter.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.0/tests/test_stixshifter_translator.py` & `kestrel-lang-1.7.1/tests/test_stixshifter_translator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import json
 import pandas
+import pytest
 from multiprocessing import Queue
 
 from kestrel_datasource_stixshifter.connector import check_module_availability
 from kestrel_datasource_stixshifter import multiproc
 from kestrel_datasource_stixshifter.worker.utils import TransmissionResult
 from kestrel_datasource_stixshifter.worker import STOP_SIGN
 
@@ -92,21 +93,18 @@
         output_queue,
         1,
     ) as translators:
 
         input_queue.put(SAMPLE_RESULT)
         input_queue.put(STOP_SIGN)
 
-        result = output_queue.get()
-        id_object = result.data["objects"][0]
-        assert id_object["id"] == "identity--" + query_id
-        assert id_object["name"] == CONNECTOR_NAME
-
-        result = output_queue.get()
-        assert result == STOP_SIGN
+        for result in multiproc.read_translated_results(output_queue, 1):
+            id_object = result["objects"][0]
+            assert id_object["id"] == "identity--" + query_id
+            assert id_object["name"] == CONNECTOR_NAME
 
     for translator in translators:
         assert translator.is_alive() == False
 
 
 def test_stixshifter_translate_with_bundle_writing_to_disk(tmpdir):
     query_id = "8df266aa-2901-4a94-ace9-a4403e310fa1"
@@ -127,22 +125,23 @@
         input_queue,
         output_queue,
         1,
     ) as translators:
 
         input_queue.put(SAMPLE_RESULT)
         input_queue.put(STOP_SIGN)
-        result = output_queue.get()
-        result = output_queue.get()
+
+        for result in multiproc.read_translated_results(output_queue, 1):
+            pass
 
         with open(cache_bundle_path, "r") as bundle_fp:
             bundle = json.load(bundle_fp)
-        id_object = bundle["objects"][0]
-        assert id_object["id"] == "identity--" + query_id
-        assert id_object["name"] == CONNECTOR_NAME
+            id_object = bundle["objects"][0]
+            assert id_object["id"] == "identity--" + query_id
+            assert id_object["name"] == CONNECTOR_NAME
 
     for translator in translators:
         assert translator.is_alive() == False
 
 
 def test_fast_translate():
     query_id = "8df266aa-2901-4a94-ace9-a4403e310fa1"
@@ -161,26 +160,23 @@
         output_queue,
         1,
     ) as translators:
 
         input_queue.put(SAMPLE_RESULT)
         input_queue.put(STOP_SIGN)
 
-        packet = output_queue.get()
-        result = packet.data
-        assert isinstance(result, pandas.DataFrame)
-        assert result.empty == False
-
-        result = output_queue.get()
-        assert result == STOP_SIGN
+        for result in multiproc.read_translated_results(output_queue, 1):
+            assert isinstance(result, pandas.DataFrame)
+            assert result.empty == False
 
     for translator in translators:
         assert translator.is_alive() == False
 
 
+@pytest.mark.skip(reason="kestrel v1.7.1 released with issue #370 unfixed")
 def test_stixshifter_fast_translate_with_parquet_writing_to_disk(tmpdir):
     query_id = "8df266aa-2901-4a94-ace9-a4403e310fa1"
     check_module_availability(CONNECTOR_NAME)
     cache_parquet_path_prefix = str(tmpdir.join("test"))
     offset_str = str(SAMPLE_RESULT.offset).zfill(32)
     cache_parquet_path = cache_parquet_path_prefix + f"_{offset_str}.parquet"
 
@@ -196,14 +192,15 @@
         input_queue,
         output_queue,
         1,
     ) as translators:
 
         input_queue.put(SAMPLE_RESULT)
         input_queue.put(STOP_SIGN)
-        result = output_queue.get()
-        result = output_queue.get()
+
+        for result in multiproc.read_translated_results(output_queue, 1):
+            pass
 
         df = pandas.read_parquet(cache_parquet_path)
 
     for translator in translators:
         assert translator.is_alive() == False
```

### Comparing `kestrel-lang-1.7.0/tests/test_timestamped.py` & `kestrel-lang-1.7.1/tests/test_timestamped.py`

 * *Files identical despite different names*

