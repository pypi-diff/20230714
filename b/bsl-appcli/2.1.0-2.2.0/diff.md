# Comparing `tmp/bsl-appcli-2.1.0.tar.gz` & `tmp/bsl-appcli-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsl-appcli-2.1.0.tar", last modified: Tue Jun 13 23:46:58 2023, max compression
+gzip compressed data, was "bsl-appcli-2.2.0.tar", last modified: Fri Jul 14 03:21:33 2023, max compression
```

## Comparing `bsl-appcli-2.1.0.tar` & `bsl-appcli-2.2.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    36362 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36003 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/backup_manager/backup_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/backup_manager/remote_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16721 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/cli_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/appcli_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/backup_manager_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/configure_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/configure_template_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/debug_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/encrypt_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/init_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/install_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/launcher_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/migrate_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/service_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/task_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/commands/version_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/common/data_class_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/configuration/configuration_dir_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/crypto/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/crypto/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/dev_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/git_repositories/git_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/keycloak_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/models/cli_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/models/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    28248 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/orchestrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/appcli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/templates/installer.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/templates/launcher.j2
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/appcli/variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/bsl_appcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36362 2023-06-13 23:46:58.000000 bsl-appcli-2.1.0/bsl_appcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-13 23:46:58.000000 bsl-appcli-2.1.0/bsl_appcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:46:58.000000 bsl-appcli-2.1.0/bsl_appcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-13 23:46:58.000000 bsl-appcli-2.1.0/bsl_appcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 23:46:58.000000 bsl-appcli-2.1.0/bsl_appcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/tests/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    36566 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/backup_manager/test_backup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/tests/cipher/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/cipher/test_cipher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/tests/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/tests/commands/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/commands/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/commands/test_install_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.820437 bsl-appcli-2.1.0/tests/commands_task/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands_task/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands_task/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/commands_task/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/commands_task/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/commands_task/test_commands_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/configuration/test_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/configuration_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/configuration_manager/expected_generated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/configuration_manager/expected_generated/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/configuration_manager/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/configuration_manager/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.816437 bsl-appcli-2.1.0/tests/configuration_manager/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/configuration_manager/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/configuration_manager/test_configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/configuration_state/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/configuration_state/test_configuration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/crypto/test_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/git_repositories/test_git_repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/string_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/string_transformer/test_string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/variables_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/variables_manager/test_variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:58.824437 bsl-appcli-2.1.0/tests/version/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-13 23:46:06.000000 bsl-appcli-2.1.0/tests/version/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    36725 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36366 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/appcli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/appcli/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/backup_manager/backup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/backup_manager/remote_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/cli_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/appcli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/appcli_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/backup_manager_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/configure_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/configure_template_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/debug_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/encrypt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/init_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/install_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/launcher_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/migrate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/service_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/task_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/commands/version_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/appcli/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/common/data_class_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/appcli/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/configuration/configuration_dir_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/appcli/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/crypto/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/crypto/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/dev_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/appcli/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/git_repositories/git_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/keycloak_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/appcli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/models/cli_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31125 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/orchestrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/appcli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/templates/installer.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/templates/launcher.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/appcli/variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/bsl_appcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36725 2023-07-14 03:21:33.000000 bsl-appcli-2.2.0/bsl_appcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-14 03:21:33.000000 bsl-appcli-2.2.0/bsl_appcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 03:21:33.000000 bsl-appcli-2.2.0/bsl_appcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-14 03:21:33.000000 bsl-appcli-2.2.0/bsl_appcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 03:21:33.000000 bsl-appcli-2.2.0/bsl_appcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    36566 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/backup_manager/test_backup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/cipher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/cipher/test_cipher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/tests/commands/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/tests/commands/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/tests/commands/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/commands/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/commands/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/commands/test_install_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/commands_task/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/tests/commands_task/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/tests/commands_task/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/tests/commands_task/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/commands_task/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/commands_task/test_commands_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/configuration/test_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/configuration_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/tests/configuration_manager/expected_generated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/configuration_manager/expected_generated/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/tests/configuration_manager/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/tests/configuration_manager/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.786692 bsl-appcli-2.2.0/tests/configuration_manager/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/configuration_manager/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/configuration_manager/test_configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/configuration_state/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/configuration_state/test_configuration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/crypto/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/git_repositories/test_git_repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/string_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/string_transformer/test_string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/variables_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/variables_manager/test_variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:21:33.790692 bsl-appcli-2.2.0/tests/version/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-14 03:20:39.000000 bsl-appcli-2.2.0/tests/version/test_version.py
```

### Comparing `bsl-appcli-2.1.0/LICENSE` & `bsl-appcli-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/PKG-INFO` & `bsl-appcli-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsl-appcli
-Version: 2.1.0
+Version: 2.2.0
 Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
 Home-page: https://www.brightsparklabs.com
 Author: brightSPARK Labs
 Author-email: enquire@brightsparklabs.com
 License: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -137,14 +137,24 @@
     app_name='myapp',
     docker_image='brightsparklabs/myapp',
 )
 cli = create_cli(configuration)
 cli()
 ```
 
+#### NullOrchestrator
+
+For applications with no services to orchestrate, the `NullOrchestrator` can be used. This is useful
+for appcli applications which consist only of the launcher container containing various additional CLI 
+command groups. The `NullOrchestrator` disables commands related to managing services.
+
+```python
+orchestrator=NullOrchestrator()
+```
+
 #### Custom Commands
 
 You can specify some custom top-level commands by adding click commands or command groups to the
 configuration object.  Assuming 'web' is the name of the service in the docker-compose.yml file
 which you wish to exec against, we can create three custom commands in the following example:
 
 - `myapp ls-root` which lists the contents of the root directory within the `web` service container
```

### Comparing `bsl-appcli-2.1.0/README.md` & `bsl-appcli-2.2.0/bsl_appcli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: bsl-appcli
+Version: 2.2.0
+Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
+Home-page: https://www.brightsparklabs.com
+Author: brightSPARK Labs
+Author-email: enquire@brightsparklabs.com
+License: MIT License
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # BSL Application CLI Library
 
 [![PyPI version](https://badge.fury.io/py/bsl-appcli.svg)](https://badge.fury.io/py/bsl-appcli)
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
 
@@ -125,14 +137,24 @@
     app_name='myapp',
     docker_image='brightsparklabs/myapp',
 )
 cli = create_cli(configuration)
 cli()
 ```
 
+#### NullOrchestrator
+
+For applications with no services to orchestrate, the `NullOrchestrator` can be used. This is useful
+for appcli applications which consist only of the launcher container containing various additional CLI 
+command groups. The `NullOrchestrator` disables commands related to managing services.
+
+```python
+orchestrator=NullOrchestrator()
+```
+
 #### Custom Commands
 
 You can specify some custom top-level commands by adding click commands or command groups to the
 configuration object.  Assuming 'web' is the name of the service in the docker-compose.yml file
 which you wish to exec against, we can create three custom commands in the following example:
 
 - `myapp ls-root` which lists the contents of the root directory within the `web` service container
```

### Comparing `bsl-appcli-2.1.0/appcli/backup_manager/backup_manager.py` & `bsl-appcli-2.2.0/appcli/backup_manager/backup_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/backup_manager/remote_strategy.py` & `bsl-appcli-2.2.0/appcli/backup_manager/remote_strategy.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/cli_builder.py` & `bsl-appcli-2.2.0/appcli/cli_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,18 @@
         TaskCli,
         BackupManagerCli,
         VersionCli,
     ):
         commands = cli_class(configuration).commands
         default_commands.update(**commands)
 
+    # Remove any default actions which the orchestrator does not support.
+    for disabled_command in configuration.orchestrator.get_disabled_commands():
+        default_commands.pop(disabled_command)
+
     # --------------------------------------------------------------------------
     # CREATE_CLI: NESTED METHODS
     # --------------------------------------------------------------------------
 
     @click.group(
         cls=ArgsGroup, invoke_without_command=True, help=f"CLI for managing {APP_NAME}."
     )
```

### Comparing `bsl-appcli-2.1.0/appcli/commands/appcli_command.py` & `bsl-appcli-2.2.0/appcli/commands/appcli_command.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/commands/backup_manager_cli.py` & `bsl-appcli-2.2.0/appcli/commands/backup_manager_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,24 @@
         @click.pass_context
         def backup(ctx, pre_stop_services, post_start_services, backup_name):
             cli_context: CliContext = ctx.obj
 
             cli_context.get_configuration_dir_state().verify_command_allowed(
                 AppcliCommand.BACKUP
             )
-            services_cli = cli_context.commands["service"]
+
+            try:
+                services_cli = cli_context.commands["service"]
+            except KeyError:
+                # The `service` command is not available, which means the orchestrator has no services to manage.
+                # Therefore there are no services to stop.
+                logger.info("No services to stop.")
+                services_cli = None
+                pre_stop_services = False
+                post_start_services = False
 
             if pre_stop_services:
                 logger.info("Stopping application services ...")
                 try:
                     ctx.invoke(services_cli.commands["shutdown"])
                 except SystemExit:
                     # At completion, the invoked command tries to exit the script, so we have to catch
@@ -131,15 +140,23 @@
 
             backup_manager: BackupManager = self.__create_backup_manager(cli_context)
 
             # Ensure the backup file exists before attempting restore
             if not backup_manager.backup_file_exists(ctx, backup_file):
                 error_and_exit(f"Backup file [{backup_file}] not found.")
 
-            services_cli = cli_context.commands["service"]
+            try:
+                services_cli = cli_context.commands["service"]
+            except KeyError:
+                # The `service` command is not available, which means the orchestrator has no services to manage.
+                # Therefore there are no services to stop.
+                logger.info("No services to stop.")
+                services_cli = None
+                pre_stop_services = False
+                post_start_services = False
 
             if pre_stop_services:
                 logger.info("Stopping application services ...")
                 try:
                     ctx.invoke(services_cli.commands["shutdown"])
                 except SystemExit:
                     # At completion, the invoked command tries to exit the script, so we have to catch
```

### Comparing `bsl-appcli-2.1.0/appcli/commands/configure_cli.py` & `bsl-appcli-2.2.0/appcli/commands/configure_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/commands/configure_template_cli.py` & `bsl-appcli-2.2.0/appcli/commands/configure_template_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/commands/debug_cli.py` & `bsl-appcli-2.2.0/appcli/commands/debug_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/commands/encrypt_cli.py` & `bsl-appcli-2.2.0/appcli/commands/encrypt_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/commands/init_cli.py` & `bsl-appcli-2.2.0/appcli/commands/init_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/commands/install_cli.py` & `bsl-appcli-2.2.0/appcli/commands/install_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/commands/launcher_cli.py` & `bsl-appcli-2.2.0/appcli/commands/launcher_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/commands/migrate_cli.py` & `bsl-appcli-2.2.0/appcli/commands/migrate_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/commands/service_cli.py` & `bsl-appcli-2.2.0/appcli/commands/service_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/commands/task_cli.py` & `bsl-appcli-2.2.0/appcli/commands/task_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/commands/version_cli.py` & `bsl-appcli-2.2.0/appcli/commands/version_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/common/data_class_extensions.py` & `bsl-appcli-2.2.0/appcli/common/data_class_extensions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/configuration/configuration_dir_state.py` & `bsl-appcli-2.2.0/appcli/configuration/configuration_dir_state.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/configuration_manager.py` & `bsl-appcli-2.2.0/appcli/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/crypto/cipher.py` & `bsl-appcli-2.2.0/appcli/crypto/cipher.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/crypto/crypto.py` & `bsl-appcli-2.2.0/appcli/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/dev_mode.py` & `bsl-appcli-2.2.0/appcli/dev_mode.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/functions.py` & `bsl-appcli-2.2.0/appcli/functions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/git_repositories/git_repositories.py` & `bsl-appcli-2.2.0/appcli/git_repositories/git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/keycloak_manager.py` & `bsl-appcli-2.2.0/appcli/keycloak_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/logger.py` & `bsl-appcli-2.2.0/appcli/logger.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/models/cli_context.py` & `bsl-appcli-2.2.0/appcli/models/cli_context.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/models/configuration.py` & `bsl-appcli-2.2.0/appcli/models/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,18 +171,21 @@
         return "".join(
             [
                 re.sub(r"[^a-zA-Z_]", "_", self.app_name[0]),  # First character.
                 re.sub(r"[^a-zA-Z0-9_]", "_", self.app_name[1:]),
             ]
         )
 
-    class Config:
-        # This is a requirement for pydantic to disable type checking for arbitrary user types for fields.
-        # This is necessary as one or more of the fields are custom classes (e.g. Orchestrator)
-        arbitrary_types_allowed = True
+    model_config: dict = {"arbitrary_types_allowed": True}
+    """
+    This is a requirement for pydantic to disable type checking for arbitrary user types for fields.
+    This is necessary as one or more of the fields are custom classes (e.g. Orchestrator).
+    NOTE: This was updated in `pydantic==2.0`.
+    See class attribute
+    """
 
 
 def is_matching_dict_structure(dict_to_validate: Dict, clean_dict: Dict):
     """Validate the structure of a Dict against another Dict. Recursively checks the keys and
     types of the values match for all Dicts in the base Dict, relative to the clean dict.
 
     TODO: (Github issue #77) This should be used as the default function for
```

### Comparing `bsl-appcli-2.1.0/appcli/orchestrators.py` & `bsl-appcli-2.2.0/appcli/orchestrators.py`

 * *Files 8% similar despite different names*

```diff
@@ -172,14 +172,26 @@
             service_names (tuple[str,...]): Names of the services.
 
         Returns:
             bool: if the services exists.
         """
         raise NotImplementedError
 
+    def get_disabled_commands(self) -> list[str]:
+        """
+        Returns the list of default appcli commands which this orchestrator wants to disable.
+        E.g. ['init', 'backup'].
+
+        This allows orchestrators to prevent commands being run which are not supported.
+
+        Returns:
+            list[str]: The disabled command names.
+        """
+        return []
+
 
 class DockerComposeOrchestrator(Orchestrator):
     """
     Uses Docker Compose to orchestrate containers.
     """
 
     def __init__(
@@ -573,14 +585,87 @@
         )
 
     def __exec_command(self, command: Iterable[str]) -> CompletedProcess:
         logger.debug("Running [%s]", " ".join(command))
         return subprocess.run(command, capture_output=True)
 
 
+class NullOrchestrator(Orchestrator):
+    """
+    Orchestrator which has no services to orchestrate. This is useful for appcli applications which
+    consist only of the launcher container containing various additional CLI command groups.
+    """
+
+    def start(
+        self, cli_context: CliContext, service_name: tuple[str, ...] = None
+    ) -> CompletedProcess:
+        logger.info("NullOrchestrator has no services to start.")
+        return None
+
+    def shutdown(
+        self, cli_context: CliContext, service_name: tuple[str, ...] = None
+    ) -> CompletedProcess:
+        logger.info("NullOrchestrator has no services to shutdown.")
+        return None
+
+    def status(
+        self, cli_context: CliContext, service_name: tuple[str, ...] = None
+    ) -> CompletedProcess:
+        logger.info("NullOrchestrator has no services to get the status of.")
+        return None
+
+    def task(
+        self,
+        cli_context: CliContext,
+        service_name: str,
+        extra_args: Iterable[str],
+        detached: bool = False,
+    ) -> CompletedProcess:
+        logger.info("NullOrchestrator has no services to run tasks for.")
+        return None
+
+    def exec(
+        self,
+        cli_context: CliContext,
+        service_name: str,
+        command: Iterable[str],
+        stdin_input: str = None,
+    ) -> CompletedProcess:
+        logger.info(
+            "NullOrchestrator has no running containers to execute commands in."
+        )
+        return None
+
+    def get_logs_command(self) -> click.Command:
+        @click.command()
+        def log():
+            logger.info("NullOrchestrator has no services to get logs of.")
+            return None
+
+        return log
+
+    def get_name(self) -> str:
+        return "null_orchestrator"
+
+    def verify_service_names(
+        self, cli_context: CliContext, service_names: tuple[str, ...]
+    ) -> bool:
+        if service_names is None or len(service_names) == 0:
+            return True
+        logger.info("NullOrchestrator has no services.")
+        return False
+
+    def get_disabled_commands(self) -> list[str]:
+        # The `service` and `task` commands are disabled because they are used for managing and interacting with
+        # services, and this orchestrator has no services.
+        # The `init` command is disabled because it's used to initialise additional services, and this orchestrator
+        # has no services. NOTE: The `init` command will be removed in the future.
+        return ["init", "service", "task"]
+
+
 # ------------------------------------------------------------------------------
 # PUBLIC METHODS
 # ------------------------------------------------------------------------------
 
 
 def service_name_verifier(
     service_names: tuple[str, ...], valid_service_names: List[str]
```

### Comparing `bsl-appcli-2.1.0/appcli/string_transformer.py` & `bsl-appcli-2.2.0/appcli/string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/templates/installer.j2` & `bsl-appcli-2.2.0/appcli/templates/installer.j2`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/templates/launcher.j2` & `bsl-appcli-2.2.0/appcli/templates/launcher.j2`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/appcli/variables_manager.py` & `bsl-appcli-2.2.0/appcli/variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/bsl_appcli.egg-info/PKG-INFO` & `bsl-appcli-2.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: bsl-appcli
-Version: 2.1.0
-Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
-Home-page: https://www.brightsparklabs.com
-Author: brightSPARK Labs
-Author-email: enquire@brightsparklabs.com
-License: MIT License
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # BSL Application CLI Library
 
 [![PyPI version](https://badge.fury.io/py/bsl-appcli.svg)](https://badge.fury.io/py/bsl-appcli)
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
 
@@ -137,14 +125,24 @@
     app_name='myapp',
     docker_image='brightsparklabs/myapp',
 )
 cli = create_cli(configuration)
 cli()
 ```
 
+#### NullOrchestrator
+
+For applications with no services to orchestrate, the `NullOrchestrator` can be used. This is useful
+for appcli applications which consist only of the launcher container containing various additional CLI 
+command groups. The `NullOrchestrator` disables commands related to managing services.
+
+```python
+orchestrator=NullOrchestrator()
+```
+
 #### Custom Commands
 
 You can specify some custom top-level commands by adding click commands or command groups to the
 configuration object.  Assuming 'web' is the name of the service in the docker-compose.yml file
 which you wish to exec against, we can create three custom commands in the following example:
 
 - `myapp ls-root` which lists the contents of the root directory within the `web` service container
```

### Comparing `bsl-appcli-2.1.0/bsl_appcli.egg-info/SOURCES.txt` & `bsl-appcli-2.2.0/bsl_appcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/setup.py` & `bsl-appcli-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,27 +53,27 @@
     license="MIT License",
     author="brightSPARK Labs",
     author_email="enquire@brightsparklabs.com",
     url="https://www.brightsparklabs.com",
     packages=find_namespace_packages(exclude=["contrib", "docs", "tests"]),
     include_package_data=True,
     install_requires=[
-        "boto3==1.26.145",
+        "boto3==1.26.165",
         "click==8.1.3",
         "coloredlogs==15.0.1",
         "cronex==0.1.3.1",
         "dataclasses-json==0.5.7",
         "deepdiff==6.3.0",
         "GitPython==3.1.31",
         "jinja2==3.1.2",
-        "pre-commit==3.3.2",
+        "pre-commit==3.3.3",
         "pycryptodome==3.18.0",
-        "pydantic==1.10.8",
+        "pydantic==2.0.1",
         "pyfiglet==0.8.post1",
         "python-keycloak==0.22.0",
         "python-slugify==8.0.1",
-        "ruamel-yaml==0.17.31",
+        "ruamel-yaml==0.17.32",
         "tabulate==0.9.0",
         "wheel==0.40.0",
     ],
     extras_require={"dev": ["black", "flake8", "isort", "pytest"]},
 )
```

### Comparing `bsl-appcli-2.1.0/tests/backup_manager/test_backup_manager.py` & `bsl-appcli-2.2.0/tests/backup_manager/test_backup_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/cipher/test_cipher.py` & `bsl-appcli-2.2.0/tests/cipher/test_cipher.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/commands/test_commands.py` & `bsl-appcli-2.2.0/tests/commands/test_commands.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/commands/test_install_script.py` & `bsl-appcli-2.2.0/tests/commands/test_install_script.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/commands_task/test_commands_task.py` & `bsl-appcli-2.2.0/tests/commands_task/test_commands_task.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/configuration/test_configuration.py` & `bsl-appcli-2.2.0/tests/configuration/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/configuration_manager/test_configuration_manager.py` & `bsl-appcli-2.2.0/tests/configuration_manager/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/configuration_state/test_configuration_state.py` & `bsl-appcli-2.2.0/tests/configuration_state/test_configuration_state.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/crypto/test_crypto.py` & `bsl-appcli-2.2.0/tests/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/git_repositories/test_git_repositories.py` & `bsl-appcli-2.2.0/tests/git_repositories/test_git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/string_transformer/test_string_transformer.py` & `bsl-appcli-2.2.0/tests/string_transformer/test_string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/variables_manager/test_variables_manager.py` & `bsl-appcli-2.2.0/tests/variables_manager/test_variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-2.1.0/tests/version/test_version.py` & `bsl-appcli-2.2.0/tests/version/test_version.py`

 * *Files identical despite different names*

