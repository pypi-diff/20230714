# Comparing `tmp/zhmcclient-1.8.2.tar.gz` & `tmp/zhmcclient-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmcclient-1.8.2.tar", last modified: Mon Jul  3 17:23:31 2023, max compression
+gzip compressed data, was "zhmcclient-1.9.0.tar", last modified: Fri Jul 14 08:44:31 2023, max compression
```

## Comparing `zhmcclient-1.8.2.tar` & `zhmcclient-1.9.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:23:31.914493 zhmcclient-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-03 17:23:27.000000 zhmcclient-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-03 17:23:31.914493 zhmcclient-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/extra-testutils-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:23:31.914493 zhmcclient-1.8.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5458 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:23:31.910493 zhmcclient-1.8.2/zhmcclient/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_activation_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    27187 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_capacity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32528 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    94301 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    46440 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_hba.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_ldap_server_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    78470 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_lpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    33251 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    36561 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_nic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15902 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_password_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_port.py
--rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_resource_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    69684 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    33564 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_storage_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_storage_group_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    25230 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_storage_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_storage_volume_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_timestats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_unmanaged_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_user_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_virtual_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_virtual_storage_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_virtual_switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:23:31.914493 zhmcclient-1.8.2/zhmcclient/testutils/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_cpc_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definition_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_hmc_inventory_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_hmc_vault_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:23:31.910493 zhmcclient-1.8.2/zhmcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-03 17:23:31.000000 zhmcclient-1.8.2/zhmcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-03 17:23:31.000000 zhmcclient-1.8.2/zhmcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:23:31.000000 zhmcclient-1.8.2/zhmcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-03 17:23:31.000000 zhmcclient-1.8.2/zhmcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 17:23:31.000000 zhmcclient-1.8.2/zhmcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:22:48.000000 zhmcclient-1.8.2/zhmcclient.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:23:31.914493 zhmcclient-1.8.2/zhmcclient_mock/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   134108 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient_mock/_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient_mock/_idpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    42583 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient_mock/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)   201548 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient_mock/_urihandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:44:31.550871 zhmcclient-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-14 08:44:27.000000 zhmcclient-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-14 08:44:31.550871 zhmcclient-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/extra-testutils-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:44:31.550871 zhmcclient-1.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5458 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:44:31.546871 zhmcclient-1.9.0/zhmcclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_activation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28638 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_auto_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_capacity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32810 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95566 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47315 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_hba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_ldap_server_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79949 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_lpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43902 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36278 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_nic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18861 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53547 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_password_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25001 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69514 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34976 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_storage_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_storage_group_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26644 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_storage_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_storage_volume_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_timestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_unmanaged_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_user_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_virtual_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_virtual_storage_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_virtual_switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:44:31.550871 zhmcclient-1.9.0/zhmcclient/testutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_cpc_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definition_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_hmc_inventory_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_hmc_vault_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:44:31.546871 zhmcclient-1.9.0/zhmcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-14 08:44:31.000000 zhmcclient-1.9.0/zhmcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-14 08:44:31.000000 zhmcclient-1.9.0/zhmcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:44:31.000000 zhmcclient-1.9.0/zhmcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-14 08:44:31.000000 zhmcclient-1.9.0/zhmcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 08:44:31.000000 zhmcclient-1.9.0/zhmcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:43:41.000000 zhmcclient-1.9.0/zhmcclient.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:44:31.550871 zhmcclient-1.9.0/zhmcclient_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134108 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient_mock/_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient_mock/_idpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42583 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient_mock/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)   201548 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient_mock/_urihandler.py
```

### Comparing `zhmcclient-1.8.2/LICENSE` & `zhmcclient-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/MANIFEST.in` & `zhmcclient-1.9.0/MANIFEST.in`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 include LICENSE
 include README.rst
 include requirements.txt
 include extra-testutils-requirements.txt
 include zhmcclient/__init__.py
 include zhmcclient/_activation_profile.py
 include zhmcclient/_adapter.py
+include zhmcclient/_auto_updater.py
 include zhmcclient/_capacity_group.py
 include zhmcclient/_certificates.py
 include zhmcclient/_client.py
 include zhmcclient/_console.py
 include zhmcclient/_constants.py
 include zhmcclient/_cpc.py
 include zhmcclient/_debug_info.py
@@ -24,15 +25,14 @@
 include zhmcclient/_metrics.py
 include zhmcclient/_nic.py
 include zhmcclient/_notification.py
 include zhmcclient/_partition.py
 include zhmcclient/_password_rule.py
 include zhmcclient/_port.py
 include zhmcclient/_resource.py
-include zhmcclient/_resource_updater.py
 include zhmcclient/_session.py
 include zhmcclient/_storage_group.py
 include zhmcclient/_storage_group_template.py
 include zhmcclient/_storage_volume.py
 include zhmcclient/_storage_volume_template.py
 include zhmcclient/_task.py
 include zhmcclient/_timestats.py
```

### Comparing `zhmcclient-1.8.2/PKG-INFO` & `zhmcclient-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmcclient
-Version: 1.8.2
+Version: 1.9.0
 Summary: A pure Python client library for the IBM Z HMC Web Services API.
 Home-page: https://github.com/zhmcclient/python-zhmcclient
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmcclient-1.8.2/README.rst` & `zhmcclient-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/extra-testutils-requirements.txt` & `zhmcclient-1.9.0/extra-testutils-requirements.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/requirements.txt` & `zhmcclient-1.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/setup.py` & `zhmcclient-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/__init__.py` & `zhmcclient-1.9.0/zhmcclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from ._version import *       # noqa: F401
 from ._constants import *     # noqa: F401
 from ._exceptions import *    # noqa: F401 pylint: disable=redefined-builtin
 from ._manager import *       # noqa: F401
 from ._resource import *      # noqa: F401
 from ._logging import *       # noqa: F401
 from ._session import *       # noqa: F401
-from ._resource_updater import *       # noqa: F401
+from ._auto_updater import *  # noqa: F401
 from ._timestats import *     # noqa: F401
 from ._client import *        # noqa: F401
 from ._cpc import *           # noqa: F401
 from ._group import *         # noqa: F401
 from ._lpar import *          # noqa: F401
 from ._partition import *     # noqa: F401
 from ._activation_profile import *     # noqa: F401
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_activation_profile.py` & `zhmcclient-1.9.0/zhmcclient/_activation_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,14 +149,34 @@
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the Activation Profiles of this CPC, of the profile type
         managed by this object.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to this CPC.
 
         Parameters:
 
           full_properties (bool):
@@ -180,40 +200,48 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
-
-            resources_name = self._profile_type + '-activation-profiles'
-            uri = '{}/{}{}'.format(self.cpc.uri, resources_name, query_parms)
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+
+                resources_name = self._profile_type + '-activation-profiles'
+                uri = '{}/{}{}'.format(self.cpc.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
 
-            result = self.session.get(uri)
-            if result:
-                props_list = result[resources_name]
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
 
 class ActivationProfile(BaseResource):
     """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_adapter.py` & `zhmcclient-1.9.0/zhmcclient/_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -136,14 +136,34 @@
         return self._parent
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the Adapters in this CPC.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to this CPC.
         * Object-access permission to any Adapter to be included in the result.
 
         Parameters:
 
@@ -168,40 +188,48 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
-
-            resources_name = 'adapters'
-            uri = '{}/{}{}'.format(self.cpc.uri, resources_name, query_parms)
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+
+                resources_name = 'adapters'
+                uri = '{}/{}{}'.format(self.cpc.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
 
-            result = self.session.get(uri)
-            if result:
-                props_list = result[resources_name]
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create_hipersocket(self, properties):
         """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_capacity_group.py` & `zhmcclient-1.9.0/zhmcclient/_capacity_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,34 @@
         return self._parent
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the Capacity Groups in this CPC.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to this CPC.
 
         Parameters:
 
           full_properties (bool):
@@ -108,41 +128,48 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
-
-            resources_name = 'capacity-groups'
-            uri = '{}/{}{}'.format(self.cpc.uri, resources_name, query_parms)
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+
+                resources_name = 'capacity-groups'
+                uri = '{}/{}{}'.format(self.cpc.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
 
-            result = self.session.get(uri)
-            if result:
-                props_list = result[resources_name]
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties):
         """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_certificates.py` & `zhmcclient-1.9.0/zhmcclient/_certificates.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/_client.py` & `zhmcclient-1.9.0/zhmcclient/_client.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/_console.py` & `zhmcclient-1.9.0/zhmcclient/_console.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,20 @@
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the (one) :term:`Console` representing the HMC this client is
         connected to.
 
+        Any provided filter argument will be ignored; the `filter_args`
+        parameter exists only for consistency with other list() methods.
+
+        The listing of resources is handled by constructing a singleton
+        object that represents the HMC of the current session.
+
         Authorization requirements:
 
         * None
 
         Parameters:
 
           full_properties (bool):
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_constants.py` & `zhmcclient-1.9.0/zhmcclient/_constants.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/_cpc.py` & `zhmcclient-1.9.0/zhmcclient/_cpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 from ._activation_profile import ActivationProfileManager
 from ._adapter import AdapterManager
 from ._virtual_switch import VirtualSwitchManager
 from ._capacity_group import CapacityGroupManager
 from ._logging import logged_api_call
 from ._exceptions import ParseError, ConsistencyError
 from ._utils import get_features, matches_filters, divide_filter_args, \
-    RC_CPC, RC_ADAPTER, RC_CAPACITY_GROUP, RC_HBA, RC_NIC, RC_PARTITION, \
+    RC_CPC, RC_ADAPTER, RC_HBA, RC_NIC, RC_PARTITION, \
     RC_NETWORK_PORT, RC_STORAGE_PORT, RC_STORAGE_TEMPLATE, RC_STORAGE_GROUP, \
     RC_STORAGE_TEMPLATE_VOLUME, RC_STORAGE_VOLUME, RC_VIRTUAL_FUNCTION, \
     RC_VIRTUAL_STORAGE_RESOURCE, RC_VIRTUAL_SWITCH, RC_STORAGE_SITE, \
     RC_STORAGE_FABRIC, RC_STORAGE_SWITCH, RC_STORAGE_SUBSYSTEM, \
     RC_STORAGE_PATH, RC_STORAGE_CONTROL_UNIT, RC_VIRTUAL_TAPE_RESOURCE, \
     RC_TAPE_LINK, RC_TAPE_LIBRARY, RC_CERTIFICATE
 
@@ -146,14 +146,34 @@
         return self.client.consoles.console
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the CPCs managed by the HMC this client is connected to.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to any CPC to be included in the result.
 
         Parameters:
 
           full_properties (bool):
@@ -177,40 +197,47 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+
+                resources_name = 'cpcs'
+                uri = '/api/{}{}'.format(resources_name, query_parms)
 
-            resources_name = 'cpcs'
-            uri = '/api/{}{}'.format(resources_name, query_parms)
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
 
-            result = self.session.get(uri)
-            if result:
-                props_list = result[resources_name]
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
 
 class Cpc(BaseResource):
     """
@@ -326,42 +353,42 @@
         """
         :class:`~zhmcclient.ActivationProfileManager`: Access to the
         :term:`Reset Activation Profiles <Reset Activation Profile>` in this
         CPC.
         """
         # We do here some lazy loading.
         if not self._reset_activation_profiles:
-            self._reset_activation_profiles = \
-                ActivationProfileManager(self, profile_type='reset')
+            self._reset_activation_profiles = ActivationProfileManager(
+                self, profile_type='reset')
         return self._reset_activation_profiles
 
     @property
     def image_activation_profiles(self):
         """
         :class:`~zhmcclient.ActivationProfileManager`: Access to the
         :term:`Image Activation Profiles <Image Activation Profile>` in this
         CPC.
         """
         # We do here some lazy loading.
         if not self._image_activation_profiles:
-            self._image_activation_profiles = \
-                ActivationProfileManager(self, profile_type='image')
+            self._image_activation_profiles = ActivationProfileManager(
+                self, profile_type='image')
         return self._image_activation_profiles
 
     @property
     def load_activation_profiles(self):
         """
         :class:`~zhmcclient.ActivationProfileManager`: Access to the
         :term:`Load Activation Profiles <load Activation Profile>` in this
         CPC.
         """
         # We do here some lazy loading.
         if not self._load_activation_profiles:
-            self._load_activation_profiles = \
-                ActivationProfileManager(self, profile_type='load')
+            self._load_activation_profiles = ActivationProfileManager(
+                self, profile_type='load')
         return self._load_activation_profiles
 
     @property
     @logged_api_call
     def dpm_enabled(self):
         """
         bool: Indicates whether this CPC is currently in DPM mode
@@ -2031,17 +2058,16 @@
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
           :exc:`~zhmcclient.ConsistencyError` - issues with inventory data
         """
         inventory_list = retrieveInventoryData(self.manager.client)
-        cpc_uri = self.get_property('object-uri')
-        config_dict = convertToConfig(self.manager.console, inventory_list,
-                                      cpc_uri, include_unused_adapters)
+        config_dict = self._convert_to_config(inventory_list,
+                                              include_unused_adapters)
         features = self.list_api_features()
         if len(features) > 0:
             config_dict['available-api-features-list'] = features
         return config_dict
 
     @logged_api_call
     def list_api_features(self, name=None):
@@ -2065,14 +2091,184 @@
           list of strings: The list of API features that are available on this
           CPC. For API versions prior to 4.10, an empty list is returned.
 
         """
         # TODO: add reference to WSAPI book chapter regarding API features
         return get_features(self.manager.session, self.uri, name)
 
+    def _convert_to_config(self, inventory_list, include_unused_adapters):
+        """
+        Convert the inventory list to a DPM configuration dict.
+
+        Important: In order to support export of DPM configs with zhmcclient
+        versions that have support for newer features from older machines and
+        import into older machines, any dictionary items for NEWLY added
+        features must be omitted if empty.
+        """
+        cpc_uri = self.get_property('object-uri')
+        cpc_uris = [cpc_uri]
+
+        config_dict = OrderedDict()
+
+        config_dict['se-version'] = self.prop('se-version')
+        config_dict['available-features-list'] = self.prop(
+            'available-features-list', [])
+        config_dict['cpc-properties'] = {
+            'auto-start-list': self.prop('auto-start-list'),
+            'description': self.prop('description'),
+            'management-world-wide-port-name':
+                self.prop('management-world-wide-port-name'),
+        }
+        config_dict['capacity-groups'] = [
+            dict(group.properties) for group in
+            self.capacity_groups.list(full_properties=True)]
+
+        partitions = extractByParent(
+            RC_PARTITION, cpc_uris, inventory_list)
+        # This item is required by the "Import DPM Configuration" operation
+        config_dict['partitions'] = partitions
+        partition_uris = [x['object-uri'] for x in partitions]
+
+        adapters = extractAdapters(cpc_uri, inventory_list)
+        if adapters:
+            config_dict['adapters'] = adapters
+        adapter_uris = [x['object-uri'] for x in adapters]
+
+        nics = extractByParent(
+            RC_NIC, partition_uris, inventory_list)
+        if nics:
+            config_dict['nics'] = nics
+
+        hbas = extractByParent(
+            RC_HBA, partition_uris, inventory_list)
+        if hbas:
+            config_dict['hbas'] = hbas
+
+        virtual_functions = extractByParent(
+            RC_VIRTUAL_FUNCTION, partition_uris, inventory_list)
+        if virtual_functions:
+            config_dict['virtual-functions'] = virtual_functions
+
+        virtual_switches = extractByParent(
+            RC_VIRTUAL_SWITCH, cpc_uris, inventory_list)
+        if virtual_switches:
+            config_dict['virtual-switches'] = virtual_switches
+
+        storage_sites = extractByValueInListProperty(
+            RC_STORAGE_SITE, cpc_uri, 'cpc-uris', inventory_list)
+        if storage_sites:
+            config_dict['storage-sites'] = storage_sites
+        storage_site_uris = [x['object-uri'] for x in storage_sites]
+
+        storage_subsystems = extractByPropertyInListValue(
+            RC_STORAGE_SUBSYSTEM, 'storage-site-uri', storage_site_uris,
+            inventory_list)
+        if storage_subsystems:
+            config_dict['storage-subsystems'] = storage_subsystems
+        storage_subsystem_uris = [x['object-uri'] for x in storage_subsystems]
+
+        storage_fabrics = extractByPropertyInListValue(
+            RC_STORAGE_FABRIC, 'cpc-uri', cpc_uris, inventory_list)
+        if storage_fabrics:
+            config_dict['storage-fabrics'] = storage_fabrics
+
+        storage_switches = extractByPropertyInListValue(
+            RC_STORAGE_SWITCH, 'storage-site-uri', storage_site_uris,
+            inventory_list)
+        if storage_switches:
+            config_dict['storage-switches'] = storage_switches
+
+        storage_control_units = extractByPropertyInListValue(
+            RC_STORAGE_CONTROL_UNIT, 'parent', storage_subsystem_uris,
+            inventory_list)
+        if storage_control_units:
+            config_dict['storage-control-units'] = storage_control_units
+        storage_control_unit_uris = [x['object-uri']
+                                     for x in storage_control_units]
+
+        storage_paths = extractByPropertyInListValue(
+            RC_STORAGE_PATH, 'parent', storage_control_unit_uris,
+            inventory_list)
+        if storage_paths:
+            config_dict['storage-paths'] = storage_paths
+
+        storage_ports = extractByPropertyInListValue(
+            RC_STORAGE_PORT, 'parent', adapter_uris, inventory_list)
+        if storage_ports:
+            config_dict['storage-ports'] = storage_ports
+
+        network_ports = extractByPropertyInListValue(
+            RC_NETWORK_PORT, 'parent', adapter_uris, inventory_list)
+        if network_ports:
+            config_dict['network-ports'] = network_ports
+
+        storage_groups = extractByPropertyInListValue(
+            RC_STORAGE_GROUP, 'cpc-uri', cpc_uris, inventory_list)
+        if storage_groups:
+            config_dict['storage-groups'] = storage_groups
+        storage_group_uris = [x['object-uri'] for x in storage_groups]
+
+        storage_volumes = extractByPropertyInListValue(
+            RC_STORAGE_VOLUME, 'parent', storage_group_uris, inventory_list)
+        if storage_volumes:
+            config_dict['storage-volumes'] = storage_volumes
+
+        storage_templates = extractByPropertyInListValue(
+            RC_STORAGE_TEMPLATE, 'cpc-uri', cpc_uris, inventory_list)
+        if storage_templates:
+            config_dict['storage-templates'] = storage_templates
+        storage_template_uris = [x['object-uri'] for x in storage_templates]
+
+        storage_template_volumes = extractByPropertyInListValue(
+            RC_STORAGE_TEMPLATE_VOLUME, 'parent', storage_template_uris,
+            inventory_list)
+        if storage_template_volumes:
+            config_dict['storage-template-volumes'] = storage_template_volumes
+
+        virtual_storage_resources = extractByPropertyInListValue(
+            RC_VIRTUAL_STORAGE_RESOURCE, 'parent', storage_group_uris,
+            inventory_list)
+        if virtual_storage_resources:
+            config_dict['virtual-storage-resources'] = virtual_storage_resources
+
+        tape_links = extractByPropertyInListValue(
+            RC_TAPE_LINK, 'cpc-uri', cpc_uris, inventory_list)
+        if tape_links:
+            config_dict['tape-links'] = tape_links
+        tape_link_uris = [x['object-uri'] for x in tape_links]
+
+        tape_libraries = extractByPropertyInListValue(
+            RC_TAPE_LIBRARY, 'cpc-uri', cpc_uris, inventory_list)
+        if tape_libraries:
+            config_dict['tape-libraries'] = tape_libraries
+
+        virtual_tape_resources = extractByParent(
+            RC_VIRTUAL_TAPE_RESOURCE, tape_link_uris, inventory_list)
+        if virtual_tape_resources:
+            config_dict['virtual-tape-resources'] = virtual_tape_resources
+
+        classname_for_partition_links = 'partition-link'
+        partition_links = extractByPropertyInListValue(
+            classname_for_partition_links, 'cpc-uri', cpc_uris, inventory_list)
+        if partition_links:
+            config_dict['partition-links'] = partition_links
+
+        certificates = extractByPropertyInListValue(
+            RC_CERTIFICATE, 'parent', cpc_uris, inventory_list)
+        if certificates:
+            _add_encoded(self.manager.console, certificates)
+            config_dict['certificates'] = certificates
+
+        if not include_unused_adapters:
+            _remove_unreferenced_adapters(config_dict)
+
+        sort_lists(config_dict)
+
+        return config_dict
+
 
 # Functions used by Cpc.export_dpm_configuration().
 # Some of these functions were adapted from code in the
 # exportDpmResourcesToFile.py script available at
 # https://www-01.ibm.com/servers/resourcelink/lib03020.nsf/0/2C88A77CEA71062E8525829500667BCD?OpenDocument
 
 def extractByParent(classname, parent_list, inventory_list):
@@ -2110,33 +2306,14 @@
     containing the specified cpc-uri value.
     """
     result_list = [x for x in inventory_list
                    if x['class'] == classname and value in x[prop_name]]
     return result_list
 
 
-def extractCpc(cpc_uri, inventory_list):
-    """
-    Extract the CPC item from inventory_list that has the specified cpc_uri.
-    """
-    cpcs = [x for x in inventory_list
-            if x['class'] == RC_CPC and x['object-uri'] == cpc_uri]
-    cpc_len = len(cpcs)
-    if cpc_len == 0:
-        raise ConsistencyError(
-            "Inventory data does not contain CPC with URI {}".
-            format(cpc_uri))
-    if cpc_len > 1:
-        raise ConsistencyError(
-            "Inventory data contains multiple ({}) CPCs with URI {}".
-            format(cpc_len, cpc_uri))
-    cpc = cpcs[0]
-    return cpc
-
-
 def extractAdapters(cpc_uri, inventory_list):
     """
     Extract all items from inventory_list with class "adapter" and parent
     cpc_uri.
     """
 
     # Export all adapters even when not used. If False, only adapters that
@@ -2179,15 +2356,15 @@
 
 
 def retrieveInventoryData(client):
     """
     Retrieve inventory data from the HMC.
     Returns the inventory list from Client.get_inventory().
     """
-    resource_classes = ['dpm-resources', 'cpc']
+    resource_classes = ['dpm-resources']
     api_features = client.consoles.console.list_api_features()
     if 'secure-boot-with-certificates' in api_features:
         resource_classes.append('certificate-resources')
 
     inventory_list = client.get_inventory(resource_classes)
     error_msgs = []
     for item in inventory_list:
@@ -2202,185 +2379,14 @@
     if error_msgs:
         raise ConsistencyError(
             "Some resources could not be fully inventoried:\n  {}".
             format('\n  '.join(error_msgs)))
     return inventory_list
 
 
-def convertToConfig(console, inventory_list, cpc_uri, include_unused_adapters):
-    """
-    Convert the inventory list to a DPM configuration dict.
-
-    Important: In order to support export of DPM configs with zhmcclient
-    versions that have support for newer features from older machines and
-    import into older machines, any dictionary items for newly added features
-    must be omitted if empty.
-    """
-    config_dict = OrderedDict()
-
-    cpc = extractCpc(cpc_uri, inventory_list)
-    cpc_uris = [cpc_uri]
-
-    config_dict['se-version'] = cpc.get('se-version', None)
-    config_dict['available-features-list'] = \
-        cpc.get('available-features-list', [])
-    config_dict['cpc-properties'] = {
-        'auto-start-list': cpc.get('auto-start-list', None),
-        'description': cpc.get('description', None),
-        'management-world-wide-port-name':
-            cpc.get('management-world-wide-port-name', None),
-    }
-
-    partitions = extractByParent(
-        RC_PARTITION, cpc_uris, inventory_list)
-    # This item is required by the "Import DPM Configuration" operation
-    config_dict['partitions'] = partitions
-    partition_uris = [x['object-uri'] for x in partitions]
-
-    adapters = extractAdapters(cpc_uri, inventory_list)
-    if adapters:
-        config_dict['adapters'] = adapters
-    adapter_uris = [x['object-uri'] for x in adapters]
-
-    nics = extractByParent(
-        RC_NIC, partition_uris, inventory_list)
-    if nics:
-        config_dict['nics'] = nics
-
-    hbas = extractByParent(
-        RC_HBA, partition_uris, inventory_list)
-    if hbas:
-        config_dict['hbas'] = hbas
-
-    virtual_functions = extractByParent(
-        RC_VIRTUAL_FUNCTION, partition_uris, inventory_list)
-    if virtual_functions:
-        config_dict['virtual-functions'] = virtual_functions
-
-    virtual_switches = extractByParent(
-        RC_VIRTUAL_SWITCH, cpc_uris, inventory_list)
-    if virtual_switches:
-        config_dict['virtual-switches'] = virtual_switches
-
-    capacity_groups = extractByParent(
-        RC_CAPACITY_GROUP, cpc_uris, inventory_list)
-    if capacity_groups:
-        config_dict['capacity-groups'] = capacity_groups
-
-    storage_sites = extractByValueInListProperty(
-        RC_STORAGE_SITE, cpc_uri, 'cpc-uris', inventory_list)
-    if storage_sites:
-        config_dict['storage-sites'] = storage_sites
-    storage_site_uris = [x['object-uri'] for x in storage_sites]
-
-    storage_subsystems = extractByPropertyInListValue(
-        RC_STORAGE_SUBSYSTEM, 'storage-site-uri', storage_site_uris,
-        inventory_list)
-    if storage_subsystems:
-        config_dict['storage-subsystems'] = storage_subsystems
-    storage_subsystem_uris = [x['object-uri'] for x in storage_subsystems]
-
-    storage_fabrics = extractByPropertyInListValue(
-        RC_STORAGE_FABRIC, 'cpc-uri', cpc_uris, inventory_list)
-    if storage_fabrics:
-        config_dict['storage-fabrics'] = storage_fabrics
-
-    storage_switches = extractByPropertyInListValue(
-        RC_STORAGE_SWITCH, 'storage-site-uri', storage_site_uris,
-        inventory_list)
-    if storage_switches:
-        config_dict['storage-switches'] = storage_switches
-
-    storage_control_units = extractByPropertyInListValue(
-        RC_STORAGE_CONTROL_UNIT, 'parent', storage_subsystem_uris,
-        inventory_list)
-    if storage_control_units:
-        config_dict['storage-control-units'] = storage_control_units
-    storage_control_unit_uris = [x['object-uri'] for x in storage_control_units]
-
-    storage_paths = extractByPropertyInListValue(
-        RC_STORAGE_PATH, 'parent', storage_control_unit_uris, inventory_list)
-    if storage_paths:
-        config_dict['storage-paths'] = storage_paths
-
-    storage_ports = extractByPropertyInListValue(
-        RC_STORAGE_PORT, 'parent', adapter_uris, inventory_list)
-    if storage_ports:
-        config_dict['storage-ports'] = storage_ports
-
-    network_ports = extractByPropertyInListValue(
-        RC_NETWORK_PORT, 'parent', adapter_uris, inventory_list)
-    if network_ports:
-        config_dict['network-ports'] = network_ports
-
-    storage_groups = extractByPropertyInListValue(
-        RC_STORAGE_GROUP, 'cpc-uri', cpc_uris, inventory_list)
-    if storage_groups:
-        config_dict['storage-groups'] = storage_groups
-    storage_group_uris = [x['object-uri'] for x in storage_groups]
-
-    storage_volumes = extractByPropertyInListValue(
-        RC_STORAGE_VOLUME, 'parent', storage_group_uris, inventory_list)
-    if storage_volumes:
-        config_dict['storage-volumes'] = storage_volumes
-
-    storage_templates = extractByPropertyInListValue(
-        RC_STORAGE_TEMPLATE, 'cpc-uri', cpc_uris, inventory_list)
-    if storage_templates:
-        config_dict['storage-templates'] = storage_templates
-    storage_template_uris = [x['object-uri'] for x in storage_templates]
-
-    storage_template_volumes = extractByPropertyInListValue(
-        RC_STORAGE_TEMPLATE_VOLUME, 'parent', storage_template_uris,
-        inventory_list)
-    if storage_template_volumes:
-        config_dict['storage-template-volumes'] = storage_template_volumes
-
-    virtual_storage_resources = extractByPropertyInListValue(
-        RC_VIRTUAL_STORAGE_RESOURCE, 'parent', storage_group_uris,
-        inventory_list)
-    if virtual_storage_resources:
-        config_dict['virtual-storage-resources'] = virtual_storage_resources
-
-    tape_links = extractByPropertyInListValue(
-        RC_TAPE_LINK, 'cpc-uri', cpc_uris, inventory_list)
-    if tape_links:
-        config_dict['tape-links'] = tape_links
-    tape_link_uris = [x['object-uri'] for x in tape_links]
-
-    tape_libraries = extractByPropertyInListValue(
-        RC_TAPE_LIBRARY, 'cpc-uri', cpc_uris, inventory_list)
-    if tape_libraries:
-        config_dict['tape-libraries'] = tape_libraries
-
-    virtual_tape_resources = extractByParent(
-        RC_VIRTUAL_TAPE_RESOURCE, tape_link_uris, inventory_list)
-    if virtual_tape_resources:
-        config_dict['virtual-tape-resources'] = virtual_tape_resources
-
-    classname_for_partition_links = 'partition-link'
-    partition_links = extractByPropertyInListValue(
-        classname_for_partition_links, 'cpc-uri', cpc_uris, inventory_list)
-    if partition_links:
-        config_dict['partition-links'] = partition_links
-
-    certificates = extractByPropertyInListValue(
-        RC_CERTIFICATE, 'parent', cpc_uris, inventory_list)
-    if certificates:
-        _add_encoded(console, certificates)
-        config_dict['certificates'] = certificates
-
-    if not include_unused_adapters:
-        _remove_unreferenced_adapters(config_dict)
-
-    sort_lists(config_dict)
-
-    return config_dict
-
-
 def _add_encoded(console, certificates):
     """
     Takes a list of dicts representing certificate objects and adds
     the corresponding encoded certificate data to each dict.
     """
     for cert_dict in certificates:
         cert = console.certificates.list(
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_debug_info.py` & `zhmcclient-1.9.0/zhmcclient/_debug_info.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/_exceptions.py` & `zhmcclient-1.9.0/zhmcclient/_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 
 __all__ = ['Error', 'ConnectionError', 'ConnectTimeout', 'ReadTimeout',
            'RetriesExceeded', 'AuthError', 'ClientAuthError',
            'ServerAuthError', 'ParseError', 'VersionError', 'HTTPError',
            'OperationTimeout', 'StatusTimeout', 'NoUniqueMatch', 'NotFound',
            'MetricsResourceNotFound', 'NotificationError',
-           'NotificationJMSError', 'NotificationParseError', 'ConsistencyError',
-           'CeasedExistence']
+           'NotificationJMSError', 'NotificationParseError',
+           'SubscriptionNotFound', 'ConsistencyError', 'CeasedExistence']
 
 
 class Error(Exception):
     """
     Abstract base class for exceptions specific to this package.
 
     Exceptions of this class are not raised; only derived exceptions are
@@ -1368,14 +1368,46 @@
 
             classname={}; message={}
         """
         return "classname={!r}; message={!r};". \
             format(self.__class__.__name__, self.args[0])
 
 
+class SubscriptionNotFound(NotificationError):
+    """
+    This exception indicates that a subscripton for a topic was not found.
+
+    Derived from :exc:`~zhmcclient.NotificationError`.
+    """
+
+    def __init__(self, msg):
+        """
+        Parameters:
+
+          msg (:term:`string`):
+            A human readable message describing the problem.
+
+        ``args[0]`` will be set to the ``msg`` parameter.
+        """
+        # pylint: disable=useless-super-delegation
+        super(SubscriptionNotFound, self).__init__(msg)
+
+    def str_def(self):
+        """
+        :term:`string`: The exception as a string in a Python definition-style
+        format, e.g. for parsing by scripts:
+
+        .. code-block:: text
+
+            classname={}; message={}
+        """
+        return "classname={!r}; message={!r};". \
+            format(self.__class__.__name__, self.args[0])
+
+
 class ConsistencyError(Error):
     # pylint: disable=abstract-method
     """
     This exception indicates that an inconsistency has been detected.
 
     Please report such exceptions in the zhmcclient issue tracker
     at https://github.com/zhmcclient/python-zhmcclient/issues.
@@ -1388,15 +1420,15 @@
 class CeasedExistence(Error):
     # pylint: disable=abstract-method
     """
     This exception indicates that the corresponding HMC resource for an
     auto-updated zhmcclient resource no longer exists.
 
     This exception will only be raised for zhmcclient resources that are
-    enabled for :ref:`auto-update <Auto-updating of resources>`.
+    enabled for :ref:`auto-updating`.
 
     Derived from :exc:`~zhmcclient.Error`.
     """
 
     def __init__(self, resource_uri):
         """
         Parameters:
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_group.py` & `zhmcclient-1.9.0/zhmcclient/_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/_hba.py` & `zhmcclient-1.9.0/zhmcclient/_hba.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,17 +84,32 @@
         return self._parent
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the HBAs in this Partition.
 
-        The returned HBAs have only the 'element-uri' property set.
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
 
-        Filtering is supported only for the 'element-uri' property.
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the corresponding array property for this resource in the
+          parent object is used to list the resources, and the provided filter
+          arguments are applied.
 
         Authorization requirements:
 
         * Object-access permission to this Partition.
 
         Parameters:
 
@@ -119,28 +134,35 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        uris = self.partition.get_property('hba-uris')
-        if uris:
-            for uri in uris:
-
-                resource_obj = self.resource_class(
-                    manager=self,
-                    uri=uri,
-                    name=None,
-                    properties=None)
-
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
                 if matches_filters(resource_obj, filter_args):
                     resource_obj_list.append(resource_obj)
-                    if full_properties:
-                        resource_obj.pull_full_properties()
+        else:
+            uris = self.partition.get_property('hba-uris')
+            if uris:
+                for uri in uris:
+
+                    resource_obj = self.resource_class(
+                        manager=self,
+                        uri=uri,
+                        name=None,
+                        properties=None)
+
+                    if matches_filters(resource_obj, filter_args):
+                        resource_obj_list.append(resource_obj)
+                        if full_properties:
+                            resource_obj.pull_full_properties()
+
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties):
         """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_ldap_server_definition.py` & `zhmcclient-1.9.0/zhmcclient/_ldap_server_definition.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,14 +84,34 @@
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the :term:`LDAP Server Definition` resources representing the
         definitions of LDAp servers in this HMC.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * User-related-access permission to the LDAP Server Definition objects
           included in the result, or task permission to the "Manage LDAP Server
           Definitions" task.
 
         Parameters:
@@ -117,34 +137,47 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        query_parms, client_filters = divide_filter_args(
-            self._query_props, filter_args)
-        resources_name = 'ldap-server-definitions'
-        uri = '{}/{}{}'.format(self.console.uri, resources_name, query_parms)
-
-        result = self.session.get(uri)
-        if result:
-            props_list = result[resources_name]
-            for props in props_list:
-
-                resource_obj = self.resource_class(
-                    manager=self,
-                    uri=props[self._uri_prop],
-                    name=props.get(self._name_prop, None),
-                    properties=props)
-
-                if matches_filters(resource_obj, client_filters):
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
                     resource_obj_list.append(resource_obj)
-                    if full_properties:
-                        resource_obj.pull_full_properties()
+        else:
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+                resources_name = 'ldap-server-definitions'
+                uri = '{}/{}{}'.format(self.console.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
+
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties):
         """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_logging.py` & `zhmcclient-1.9.0/zhmcclient/_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   debug level. Internal calls to API functions are not logged.
 
 * 'zhmcclient.hmc' for operations from zhmcclient to the HMC, at the
   debug level.
 
 * 'zhmcclient.jms' for notifications from the HMC to zhmcclient, at the
   debug, info, warning and error level. At this point, this logger is used only
-  for the :ref:`auto-update <Auto-updating of resources>` support, but not for
+  for the :ref:`auto-updating` support, but not for
   the :class:`~zhmcclient.NotificationReceiver` class.
 
 For HMC operations and API calls that contain the HMC password or HMC session
 tokens, the password is hidden in the log message by replacing it with a few
 '*' characters.
 
 All these loggers have a null-handler (see :class:`~py:logging.NullHandler`)
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_lpar.py` & `zhmcclient-1.9.0/zhmcclient/_lpar.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,34 @@
         return self._parent
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the LPARs in this CPC.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to this CPC.
         * Object-access permission to any LPAR to be included in the result.
 
         Parameters:
 
@@ -121,47 +141,55 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
-
-            resources_name = 'logical-partitions'
-            uri = '{}/{}{}'.format(self.cpc.uri, resources_name, query_parms)
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+
+                resources_name = 'logical-partitions'
+                uri = '{}/{}{}'.format(self.cpc.uri, resources_name,
+                                       query_parms)
+
+                try:
+                    result = self.session.get(uri)
+                except HTTPError as exc:
+                    if exc.http_status == 404 and exc.reason == 1:
+                        # Unlike other list operations, "List Logical Partitions
+                        # of CPC" fails with 404.1 "ERROR: found no Images" if
+                        # no LPAR matches the filters in the query parms.
+                        result = []
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
 
-            try:
-                result = self.session.get(uri)
-            except HTTPError as exc:
-                if exc.http_status == 404 and exc.reason == 1:
-                    # Unlike other list operations, "List Logical Partitions
-                    # of CPC" fails with 404.1 "ERROR: found no Images" if
-                    # no LPAR matches the filters in the query parms.
-                    result = []
-            if result:
-                props_list = result[resources_name]
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
 
 class Lpar(BaseResource):
     """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_manager.py` & `zhmcclient-1.9.0/zhmcclient/_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 """
 
 from __future__ import absolute_import
 
 import re
 from datetime import datetime, timedelta
 import warnings
+import threading
 import six
 from nocasedict import NocaseDict
 
 from ._logging import logged_api_call
 from ._exceptions import NotFound, NoUniqueMatch, HTTPError
 from ._utils import repr_list
 
@@ -169,14 +170,191 @@
         if name:
             try:
                 del self._uris[name]
             except KeyError:
                 pass
 
 
+class _ResourceList(object):
+    """
+    A list of resources, for use by resource manager objects for auto-updating.
+
+    The resources in the list are the zhmcclient resource objects, organized by
+    resource URI.
+
+    This class is used by the implementation of manager classes, and is not
+    part of the external API.
+    """
+
+    def __init__(self, manager):
+        """
+        Parameters:
+
+          manager (BaseManager): Manager that holds this list of resources. The
+            manager object is expected to have a ``list()`` method, which is
+            used to list the resources of that manager.
+        """
+        self._manager = manager
+
+        # Attributes that are updated under the lock
+        self._lock = threading.RLock()
+        self._resources = {}  # key: resource URI, value: resource obj
+        self._needs_pull = True  # list() method needs to pull from HMC
+        self._enabled = False  # Auto-updating of manager is enabled
+
+    def __repr__(self):
+        """
+        Return a string with the state of this object, for debug purposes.
+        """
+        ret = (
+            "{classname} at 0x{id:08x} (\n"
+            "  _enabled={_enabled!r},\n"
+            "  _resources(keys)={_resource_keys!r}\n"
+            ")".format(
+                classname=self.__class__.__name__,
+                id=id(self),
+                _enabled=self._enabled,
+                _resource_keys=list(self._resources.keys()),
+            ))
+        return ret
+
+    def enabled(self):
+        """
+        Return whether this list of resources is enabled.
+
+        Return:
+          bool: Indicates whether this list of resources is enabled.
+        """
+        return self._enabled
+
+    def needs_pull(self):
+        """
+        Return whether this list of resources needs to be pulled from the HMC.
+        """
+        return self._needs_pull
+
+    def enable(self):
+        """
+        Enable this list of resources, if currently disabled.
+
+        When enabling, the session to which this manager belongs is subscribed
+        for auto-updating if needed (see
+        :meth:`~zhmcclient.Session.subscribe_auto_update`), the manager
+        object is registered with the session's auto updater via
+        :meth:`~zhmcclient.AutoUpdater.register_object`, and all resources
+        of this manager object are retrieved using :meth:`list` in order to
+        have the most current list of resources as a basis for the future
+        auto-updating.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """
+        if not self._enabled:
+            session = self._manager.session
+            session.subscribe_auto_update()
+            session.auto_updater.register_object(self._manager)
+
+            # The following list() call needs to pull from HMC. That is
+            # happening because the resource list is still disabled at this
+            # point.
+            resource_list = self._manager.list()
+
+            with self._lock:
+                self._resources = {}
+                for res_obj in resource_list:
+                    self._resources[res_obj.uri] = res_obj
+                self._needs_pull = False
+                self._enabled = True
+
+    def disable(self):
+        """
+        Disable this list of resources, if currently enabled.
+
+        When disabling, the manager object is unregistered from the session's
+        auto updater via
+        :meth:`~zhmcclient.AutoUpdater.unregister_object`, and the session
+        is unsubscribed from auto-updating if the auto updater has no more
+        objects registered. Also, the list of resources is cleared.
+        """
+        if self._enabled:
+            session = self._manager.session
+            session.auto_updater.unregister_object(self._manager)
+            if not session.auto_updater.has_objects():
+                session.unsubscribe_auto_update()
+            with self._lock:
+                self._resources = {}
+                self._needs_pull = True
+                self._enabled = False
+
+    def list(self):
+        """
+        Return a new list with the resource objects from this list of resources.
+        """
+        res_list = []
+        with self._lock:
+            for res_obj in self._resources.values():
+                res_list.append(res_obj)
+        return res_list
+
+    def list_uris(self):
+        """
+        Return a new list with the resource URIs from this list of resources.
+        """
+        uri_list = []
+        with self._lock:
+            for res_uri in self._resources:
+                uri_list.append(res_uri)
+        return uri_list
+
+    def add_list(self, resource_obj_list):
+        """
+        Add a new resource object list to this list of resources and mark
+        it as no longer needing pull from the HMC.
+
+        This method is called in list() to put resources pulled from the HMC
+        into the list of resources. It should not be called by the user.
+        """
+        with self._lock:
+            for res_obj in resource_obj_list:
+                self._resources[res_obj.uri] = res_obj
+            self._needs_pull = False
+
+    def trigger_pull(self):
+        """
+        Trigger that resources need to be pulled from the HMC upon the next
+        list() call of the manager object.
+
+        This method is called when an inventory change notification indicates
+        that a new object on the HMC has been created. It should not be called
+        by the user.
+        """
+        with self._lock:
+            self._needs_pull = True
+
+    def remove(self, resource_uri):
+        """
+        Remove the item for a resource URI from this list of resources.
+
+        If the resource URI is not in that list, do nothing.
+
+        This method is called when an inventory change notification indicates
+        that an object on the HMC has been deleted. It should not be called
+        by the user.
+        """
+        with self._lock:
+            try:
+                del self._resources[resource_uri]
+            except KeyError:
+                pass
+
+
 class BaseManager(object):
     """
     Abstract base class for manager classes (e.g.
     :class:`~zhmcclient.CpcManager`).
 
     It defines the interface for the derived manager classes, and implements
     methods that have a common implementation for the derived manager classes.
@@ -257,66 +435,72 @@
         assert base_uri is not None
         assert oid_prop is not None
         assert uri_prop is not None
         assert name_prop is not None
 
         self._resource_class = resource_class
         self._class_name = class_name
+        self._uri = None
         self._session = session
         self._parent = parent
         self._base_uri = base_uri
         self._oid_prop = oid_prop
         self._uri_prop = uri_prop
         self._name_prop = name_prop
         self._query_props = query_props
         self._list_has_name = list_has_name
         self._case_insensitive_names = case_insensitive_names
         self._supports_properties = supports_properties
 
+        self._resource_list = _ResourceList(self)
         self._name_uri_cache = _NameUriCache(
             self, session.retry_timeout_config.name_uri_cache_timetolive,
             case_insensitive_names)
 
     def __repr__(self):
         """
         Return a string with the state of this manager object, for debug
         purposes.
         """
         ret = (
             "{classname} at 0x{id:08x} (\n"
             "  _resource_class={_resource_class!r},\n"
             "  _class_name={_class_name!r},\n"
+            "  _uri={_uri!r},\n"
             "  _session={_session_classname} at 0x{_session_id:08x},\n"
             "  _parent={_parent_classname} at 0x{_parent_id:08x},\n"
             "  _base_uri={_base_uri!r},\n"
             "  _oid_prop={_oid_prop!r},\n"
             "  _uri_prop={_uri_prop!r},\n"
             "  _name_prop={_name_prop!r},\n"
             "  _query_props={_query_props},\n"
             "  _list_has_name={_list_has_name!r},\n"
             "  _case_insensitive_names={_case_insensitive_names!r},\n"
             "  _supports_properties={_supports_properties!r},\n"
+            "  _resource_list={_resource_list!r},\n"
             "  _name_uri_cache={_name_uri_cache!r}\n"
             ")".format(
                 classname=self.__class__.__name__,
                 id=id(self),
                 _resource_class=self._resource_class,
                 _class_name=self._class_name,
+                _uri=self._uri,
                 _session_classname=self._session.__class__.__name__,
                 _session_id=id(self._session),
                 _parent_classname=self._parent.__class__.__name__,
                 _parent_id=id(self._parent),
                 _base_uri=self._base_uri,
                 _oid_prop=self._oid_prop,
                 _uri_prop=self._uri_prop,
                 _name_prop=self._name_prop,
                 _query_props=repr_list(self._query_props, indent=2),
                 _list_has_name=self._list_has_name,
                 _case_insensitive_names=self._case_insensitive_names,
                 _supports_properties=self._supports_properties,
+                _resource_list=self._resource_list,
                 _name_uri_cache=self._name_uri_cache,
             ))
         return ret
 
     def invalidate_cache(self):
         """
         Invalidate the Name-URI cache of this manager.
@@ -436,14 +620,37 @@
 
           `None`, if the manager has no parent, i.e. when it manages top-level
           resources.
         """
         return self._parent
 
     @property
+    def uri(self):
+        """
+        string: The canonical URI path of the manager. Will not be `None`.
+
+        This URI uniquely identifies the list of HMC resources in scope of the
+        manager, consistent with how the canonical URI path of a resource
+        identifies the HMC resource.
+
+        The format of this URI is undocumented.
+
+        This URI is used in the implementation of auto-updated manager objects,
+        it does not have any meaning on the HMC, and there should be no need
+        for users to use it.
+        """
+        if self._uri is None:
+            if self._parent:
+                parent_uri = self._parent.uri
+            else:
+                parent_uri = '/'  # top-level resource
+            self._uri = '{}#{}'.format(parent_uri, self._class_name)
+        return self._uri
+
+    @property
     def case_insensitive_names(self):
         """
         :class:`py:bool`:
           Indicates whether the names of the resources are treated case
           insensitively.
         """
         return self._case_insensitive_names
@@ -454,14 +661,112 @@
         :class:`py:bool`:
           Indicates whether the "Get Properties" operation for this type of
           resource supports the 'properties' query parameter in the latest
           released version of the HMC.
         """
         return self._supports_properties
 
+    def auto_update_enabled(self):
+        """
+        Return whether :ref:`auto-updating` is
+        currently enabled for the manager object.
+
+        Return:
+          bool: Indicates whether auto-update is enabled.
+        """
+        return self._resource_list.enabled()
+
+    def auto_update_needs_pull(self):
+        """
+        Return whether there is a need to pull the resources from the HMC, in
+        the list() method.
+
+        This method is called in the list() method. It should not be called
+        by the user.
+        """
+        return self._resource_list.needs_pull()
+
+    def enable_auto_update(self):
+        """
+        Enable :ref:`auto-updating` for this manager object, if currently
+        disabled.
+
+        When enabling auto-update, the session to which this manager belongs is
+        subscribed for auto-updating if needed (see
+        :meth:`~zhmcclient.Session.subscribe_auto_update`), the manager
+        object is registered with the session's auto updater via
+        :meth:`~zhmcclient.AutoUpdater.register_object`, and all resources
+        of this manager object are retrieved using :meth:`list` in order to
+        have the most current list of resources as a basis for the future
+        auto-updating.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """
+        self._resource_list.enable()
+
+    def disable_auto_update(self):
+        """
+        Disable :ref:`auto-updating` for this manager object, if currently
+        enabled.
+
+        When disabling auto-updating, the manager object is unregistered from
+        the session's auto updater via
+        :meth:`~zhmcclient.AutoUpdater.unregister_object`, and the session
+        is unsubscribed from auto-updating if the auto updater has no more
+        objects registered.
+        """
+        self._resource_list.disable()
+
+    def auto_update_trigger_pull(self):
+        """
+        Trigger the need to pull the resources from the HMC, in the list()
+        method.
+
+        This method is called when an inventory change notification indicates
+        that a new object on the HMC has been created. It should not be called
+        by the user.
+        """
+        self._resource_list.trigger_pull()
+
+    def add_resources_local(self, resource_obj_list):
+        """
+        Add a resource object to the local auto-updated list of resources.
+
+        This method is called in list() to put resources pulled from the HMC
+        into the list of resources. It should not be called by the user.
+        """
+        self._resource_list.add_list(resource_obj_list)
+
+    def remove_resource_local(self, resource_uri):
+        """
+        Remove the resource object for a resource URI from the local
+        auto-updated list of resources.
+
+        If the resource URI is not in that list, do nothing.
+
+        This method is called when an inventory change notification indicates
+        that an object on the HMC has been deleted. It should not be called
+        by the user.
+        """
+        self._resource_list.remove(resource_uri)
+
+    def list_resources_local(self):
+        """
+        List the resource objects from the local auto-updated list of resources.
+
+        This method is called by the list() methods of resource manager classes.
+        It should not be called by the user.
+        """
+        return self._resource_list.list()
+
     def resource_object(self, uri_or_oid, props=None):
         """
         Return a minimalistic Python resource object for this resource class,
         that is scoped to this manager.
 
         This method is an internal helper function and is not normally called
         by users.
@@ -522,24 +827,16 @@
         resource properties against the specified filter arguments, and return
         a list of their Python resource objects (e.g. for CPCs, a list of
         :class:`~zhmcclient.Cpc` objects is returned).
 
         Any resource property may be specified in a filter argument. For
         details about filter arguments, see :ref:`Filtering`.
 
-        The zhmcclient implementation handles the specified properties in an
-        optimized way: Properties that can be filtered on the HMC are actually
-        filtered there (this varies by resource type), and the remaining
-        properties are filtered on the client side.
-
-        If the "name" property is specified as the only filter argument, an
-        optimized lookup is performed that uses a name-to-URI cache in this
-        manager object. This this optimized lookup uses the specified match
-        value for exact matching and is not interpreted as a regular
-        expression.
+        The listing of resources is handled in an optimized way, as described
+        in :meth:`~zhmcclient.BaseManager.list`.
 
         Authorization requirements:
 
         * see the `list()` method in the derived classes.
 
         Parameters:
 
@@ -601,24 +898,16 @@
         resource properties against the specified filter arguments, and return
         its Python resource object (e.g. for a CPC, a :class:`~zhmcclient.Cpc`
         object is returned).
 
         Any resource property may be specified in a filter argument. For
         details about filter arguments, see :ref:`Filtering`.
 
-        The zhmcclient implementation handles the specified properties in an
-        optimized way: Properties that can be filtered on the HMC are actually
-        filtered there (this varies by resource type), and the remaining
-        properties are filtered on the client side.
-
-        If the "name" property is specified as the only filter argument, an
-        optimized lookup is performed that uses a name-to-URI cache in this
-        manager object. This this optimized lookup uses the specified match
-        value for exact matching and is not interpreted as a regular
-        expression.
+        The listing of resources is handled in an optimized way, as described
+        in :meth:`~zhmcclient.BaseManager.list`.
 
         Authorization requirements:
 
         * see the `list()` method in the derived classes.
 
         Parameters:
 
@@ -679,18 +968,34 @@
         resource properties against the specified filter arguments, and return
         a list of their Python resource objects (e.g. for CPCs, a list of
         :class:`~zhmcclient.Cpc` objects is returned).
 
         Any resource property may be specified in a filter argument. For
         details about filter arguments, see :ref:`Filtering`.
 
-        The zhmcclient implementation handles the specified properties in an
-        optimized way: Properties that can be filtered on the HMC are actually
-        filtered there (this varies by resource type), and the remaining
-        properties are filtered on the client side.
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, for resources that have a List operation, the List
+          operation is performed with the subset of the provided filter
+          arguments that can be handled on the HMC side (this varies by
+          resource type) and the remaining filter arguments are applied on the
+          client side on the list result. For resources that are element objects
+          without a List operation, the corresponding array property of the
+          parent object is used to list the resources, and the provided filter
+          arguments are applied.
 
         At the level of the :class:`~zhmcclient.BaseManager` class, this method
         defines the interface for the `list()` methods implemented in the
         derived resource classes.
 
         Authorization requirements:
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_metrics.py` & `zhmcclient-1.9.0/zhmcclient/_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -901,30 +901,22 @@
             else:
                 raise MetricsResourceNotFound(
                     "{} with URI {} not found in CPCs {}".
                     format(resource_class, resource_uri,
                            ', '.join([cpc.name for cpc in cpc_list])),
                     Lpar, lpar_managers)
         elif resource_class == 'partition':
-            cpc_list = self.client.cpcs.list()
-            partition_managers = []
-            for cpc in cpc_list:
-                partition_managers.append(cpc.partitions)
-                try:
-                    filter_args = {'object-uri': resource_uri}
-                    resource = cpc.partitions.find(**filter_args)
-                    break
-                except NotFound:
-                    pass  # Try next CPC
-            else:
+            partitions = self.client.consoles.console.list_permitted_partitions(
+                filter_args={'object-uri': resource_uri})
+            if len(partitions) < 1:
                 raise MetricsResourceNotFound(
-                    "{} with URI {} not found in CPCs {}".
-                    format(resource_class, resource_uri,
-                           ', '.join([cpc.name for cpc in cpc_list])),
-                    Partition, partition_managers)
+                    "Partition with URI {} not found".
+                    format(resource_uri),
+                    Partition, [])
+            resource = partitions[0]
         elif resource_class == 'adapter':
             cpc_list = self.client.cpcs.list()
             adapter_managers = []
             for cpc in cpc_list:
                 adapter_managers.append(cpc.adapters)
                 try:
                     filter_args = {'object-uri': resource_uri}
@@ -935,34 +927,32 @@
             else:
                 raise MetricsResourceNotFound(
                     "{} with URI {} not found in CPCs {}".
                     format(resource_class, resource_uri,
                            ', '.join([cpc.name for cpc in cpc_list])),
                     Adapter, adapter_managers)
         elif resource_class == 'nic':
-            cpc_list = self.client.cpcs.list()
-            nic_managers = []
-            for cpc in cpc_list:
-                found = False
-                for partition in cpc.partitions.list():
-                    nic_managers.append(partition.nics)
-                    try:
-                        filter_args = {'element-uri': resource_uri}
-                        resource = partition.nics.find(**filter_args)
-                        found = True
-                        break
-                    except NotFound:
-                        pass  # Try next partition / next CPC
-                if found:
-                    break
-            else:
+            nic_properties = self.client.session.get(resource_uri)
+            partition_uri = nic_properties['parent']
+            partitions = self.client.consoles.console.list_permitted_partitions(
+                filter_args={'object-uri': partition_uri})
+            if len(partitions) < 1:
                 raise MetricsResourceNotFound(
-                    "{} with URI {} not found in the partitions of CPCs {}".
-                    format(resource_class, resource_uri,
-                           ', '.join([cpc.name for cpc in cpc_list])),
+                    "Parent partition with URI {} of NIC with URI {} not found".
+                    format(partition_uri, resource_uri),
+                    Partition, [])
+            partition = partitions[0]
+            nic_managers = [partition.nics]
+            filter_args = {'element-uri': resource_uri}
+            try:
+                resource = partition.nics.find(**filter_args)
+            except NotFound:
+                raise MetricsResourceNotFound(
+                    "NIC with URI {} not found in its parent partition {}.{}".
+                    format(resource_uri, cpc.name, partition.name),
                     Nic, nic_managers)
         else:
             raise ValueError(
                 "Invalid resource class: {!r}".format(resource_class))
 
         self._resource = resource
         return self._resource
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_nic.py` & `zhmcclient-1.9.0/zhmcclient/_nic.py`

 * *Files 13% similar despite different names*

```diff
@@ -78,14 +78,33 @@
         return self._parent
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the NICs in this Partition.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the corresponding array property for this resource in the
+          parent object is used to list the resources, and the provided filter
+          arguments are applied.
+
         Authorization requirements:
 
         * Object-access permission to this Partition.
 
         Parameters:
 
           full_properties (bool):
@@ -109,28 +128,35 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        uris = self.partition.get_property('nic-uris')
-        if uris:
-            for uri in uris:
-
-                resource_obj = self.resource_class(
-                    manager=self,
-                    uri=uri,
-                    name=None,
-                    properties=None)
-
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
                 if matches_filters(resource_obj, filter_args):
                     resource_obj_list.append(resource_obj)
-                    if full_properties:
-                        resource_obj.pull_full_properties()
+        else:
+            uris = self.partition.get_property('nic-uris')
+            if uris:
+                for uri in uris:
+
+                    resource_obj = self.resource_class(
+                        manager=self,
+                        uri=uri,
+                        name=None,
+                        properties=None)
+
+                    if matches_filters(resource_obj, filter_args):
+                        resource_obj_list.append(resource_obj)
+                        if full_properties:
+                            resource_obj.pull_full_properties()
+
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties):
         """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_notification.py` & `zhmcclient-1.9.0/zhmcclient/_notification.py`

 * *Files 14% similar despite different names*

```diff
@@ -63,20 +63,22 @@
 
 .. code-block:: text
 
     $ zhmc partition stop {cpc-name} {partition-name}
     $ zhmc partition start {cpc-name} {partition-name}
 """
 
+import os
 import threading
 import json
 
 from ._logging import logged_api_call
 from ._constants import DEFAULT_STOMP_PORT
-from ._exceptions import NotificationJMSError, NotificationParseError
+from ._exceptions import NotificationJMSError, NotificationParseError, \
+    SubscriptionNotFound
 
 __all__ = ['NotificationReceiver']
 
 
 class NotificationReceiver(object):
     """
     A class for receiving HMC notifications that are published to particular
@@ -127,22 +129,31 @@
             topic_names = [topic_names]
         self._topic_names = topic_names
         self._host = host
         self._port = port
         self._userid = userid
         self._password = password
 
+        # Subscription ID numbers that are in use.
+        # Each subscription for a topic gets its own unique ID.
+        # - key: topic name
+        # - value: Subscription ID number
+        self._sub_ids = {}
+
+        # Next subscription ID number to be used.
+        # After allocating a subscription ID number, this number is increased.
+        # It is never decreased again.
+        self._next_sub_id = 1
+
+        # Process PID, used to ensure uniqueness of subscription ID
+        self._process_pid = os.getpid()
+
         # Wait timeout to honor keyboard interrupts after this time:
         self._wait_timeout = 10.0  # seconds
 
-        # Subscription ID. We use some value that allows to identify on the
-        # HMC that this is the zhmcclient, but otherwise we are not using
-        # this value ourselves.
-        self._sub_id = 'zhmcclient.%s' % id(self)
-
         # Sync variables for thread-safe handover between listener thread and
         # receiver thread:
         self._handover_dict = {}
         self._handover_cond = threading.Condition()
 
         # Lazy importing for stomp, because it is so slow (ca. 5 sec)
         if 'Stomp_Connection' not in globals():
@@ -153,16 +164,103 @@
             [(self._host, self._port)], use_ssl="SSL")
         listener = _NotificationListener(self._handover_dict,
                                          self._handover_cond)
         self._conn.set_listener('', listener)
         self._conn.connect(self._userid, self._password, wait=True)
 
         for topic_name in self._topic_names:
-            dest = "/topic/" + topic_name
-            self._conn.subscribe(destination=dest, id=self._sub_id, ack='auto')
+            self.subscribe(topic_name)
+
+    def _id_value(self, sub_id):
+        """
+        Create the subscription ID from the subscription ID number.
+        """
+        id_value = ('zhmcclient.{pid}.{conn_id}.{sub_id}'.
+                    format(pid=self._process_pid, conn_id=id(self),
+                           sub_id=sub_id))
+        return id_value
+
+    @logged_api_call
+    def subscribe(self, topic_name):
+        """
+        Subscribe this notification receiver for a topic.
+
+        Parameters:
+
+          topic_name (:term:`string`): Name of the HMC notification topic.
+            Must not be `None`.
+
+        Returns:
+            string: Subscription ID
+        """
+        dest = "/topic/" + topic_name
+        sub_id = self._next_sub_id
+        self._next_sub_id += 1
+        self._sub_ids[topic_name] = sub_id
+        id_value = self._id_value(sub_id)
+        self._conn.subscribe(destination=dest, id=id_value, ack='auto')
+        return id_value
+
+    @logged_api_call
+    def unsubscribe(self, topic_name):
+        """
+        Unsubscribe this notification receiver from a topic.
+
+        If the topic is not currently subscribed for by this receiver,
+        SubscriptionNotFound is raised.
+
+        Parameters:
+
+          topic_name (:term:`string`): Name of the HMC notification topic.
+            Must not be `None`.
+
+        Raises:
+            SubscriptionNotFound: Topic is not currently subscribed for.
+        """
+        try:
+            sub_id = self._sub_ids[topic_name]
+        except KeyError:
+            raise SubscriptionNotFound(
+                "Subscription topic {!r} is not currently subscribed for")
+        id_value = self._id_value(sub_id)
+        self._conn.unsubscribe(id=id_value)
+
+    @logged_api_call
+    def is_subscribed(self, topic_name):
+        """
+        Return whether this notification receiver is currently subscribed for a
+        topic.
+
+        Parameters:
+
+          topic_name (:term:`string`): Name of the HMC notification topic.
+            Must not be `None`.
+        """
+        return topic_name in self._sub_ids
+
+    @logged_api_call
+    def get_subscription(self, topic_name):
+        """
+        Return the subscription ID for a topic this notification receiver is
+        subscribed for.
+
+        If the topic is not currently subscribed for by this receiver,
+        SubscriptionNotFound is raised.
+
+        Parameters:
+
+          topic_name (:term:`string`): Name of the HMC notification topic.
+            Must not be `None`.
+        """
+        try:
+            sub_id = self._sub_ids[topic_name]
+        except KeyError:
+            raise SubscriptionNotFound(
+                "Subscription topic {!r} is not currently subscribed for")
+        return self._id_value(sub_id)
 
     @logged_api_call
     def notifications(self):
         """
         Generator method that yields all HMC notifications (= JMS messages)
         received by this notification receiver.
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_partition.py` & `zhmcclient-1.9.0/zhmcclient/_partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,34 @@
         return self._parent
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the Partitions in this CPC.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to this CPC.
         * Object-access permission to any Partition to be included in the
           result.
 
         Parameters:
@@ -130,43 +150,49 @@
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
-
         resource_obj_list = []
-
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
-
-            resources_name = 'partitions'
-            uri = '{}/{}{}'.format(self.cpc.uri, resources_name, query_parms)
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+
+                resources_name = 'partitions'
+                uri = '{}/{}{}'.format(self.cpc.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
 
-            result = self.session.get(uri)
-            if result:
-                props_list = result[resources_name]
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties):
         """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_password_rule.py` & `zhmcclient-1.9.0/zhmcclient/_password_rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,14 +84,34 @@
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the :term:`Password Rule` resources representing the password
         rules defined in this HMC.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * User-related-access permission to the Password Rule objects included
           in the result, or task permission to the "Manage Password Rules"
           task.
 
         Parameters:
@@ -117,34 +137,47 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        query_parms, client_filters = divide_filter_args(
-            self._query_props, filter_args)
-        resources_name = 'password-rules'
-        uri = '{}/{}{}'.format(self.console.uri, resources_name, query_parms)
-
-        result = self.session.get(uri)
-        if result:
-            props_list = result[resources_name]
-            for props in props_list:
-
-                resource_obj = self.resource_class(
-                    manager=self,
-                    uri=props[self._uri_prop],
-                    name=props.get(self._name_prop, None),
-                    properties=props)
-
-                if matches_filters(resource_obj, client_filters):
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
                     resource_obj_list.append(resource_obj)
-                    if full_properties:
-                        resource_obj.pull_full_properties()
+        else:
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+                resources_name = 'password-rules'
+                uri = '{}/{}{}'.format(self.console.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
+
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties):
         """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_port.py` & `zhmcclient-1.9.0/zhmcclient/_port.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,14 +111,33 @@
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the Ports of this Adapter.
 
         If the adapter does not have any ports, an empty list is returned.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the corresponding array property for this resource in the
+          parent object is used to list the resources, and the provided filter
+          arguments are applied.
+
         Authorization requirements:
 
         * Object-access permission to this Adapter.
 
         Parameters:
 
           full_properties (bool):
@@ -141,40 +160,47 @@
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
-        uris_prop = self.adapter.port_uris_prop
-        if not uris_prop:
-            # Adapter does not have any ports
-            return []
-
-        uris = self.adapter.get_property(uris_prop)
-        assert uris is not None
-
-        # TODO: Remove the following circumvention once fixed.
-        # The following line circumvents a bug for FCP adapters that sometimes
-        # causes duplicate URIs to show up in this property:
-        uris = list(set(uris))
-
         resource_obj_list = []
-        for uri in uris:
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
+        else:
+            uris_prop = self.adapter.port_uris_prop
+            if not uris_prop:
+                # Adapter does not have any ports
+                return []
+
+            uris = self.adapter.get_property(uris_prop)
+            assert uris is not None
+
+            # TODO: Remove the following circumvention once fixed.
+            # The following line circumvents a bug for FCP adapters that
+            # sometimes causes duplicate URIs to show up in this property:
+            uris = list(set(uris))
+
+            for uri in uris:
+
+                resource_obj = self.resource_class(
+                    manager=self,
+                    uri=uri,
+                    name=None,
+                    properties=None)
+
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
+                    if full_properties:
+                        resource_obj.pull_full_properties()
 
-            resource_obj = self.resource_class(
-                manager=self,
-                uri=uri,
-                name=None,
-                properties=None)
-
-            if matches_filters(resource_obj, filter_args):
-                resource_obj_list.append(resource_obj)
-                if full_properties:
-                    resource_obj.pull_full_properties()
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
 
 class Port(BaseResource):
     """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_resource.py` & `zhmcclient-1.9.0/zhmcclient/_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
           :meth:`~zhmcclient.BaseResource.prop` methods.
 
         Updates to property values can be done via the ``update_properties()``
         method of the resource class. Which properties can be updated
         is indicated with the 'w' qualifier in the data model of the resource
         in the :term:`HMC API` book.
 
-        If :ref:`auto-update <Auto-updating of resources>` is enabled for the
+        If :ref:`auto-updating` is enabled for the
         resource object and the session is enabled for auto-updating as well,
         the property values in the returned :class:`iv:immutable_views.DictView`
         object will change as they change on the HMC.
 
         If the resource object on the HMC no longer exists, the properties
         show the values that were last updated from the HMC when the object
         still existed.
@@ -576,32 +576,32 @@
                         self._properties_timestamp),
                     _properties=repr_dict(self._properties, indent=4),
                 ))
             return ret
 
     def auto_update_enabled(self):
         """
-        Return whether :ref:`auto-update <Auto-updating of resources>` is
+        Return whether :ref:`auto-updating` is
         currently enabled for the resource object.
 
         Return:
           bool: Indicates whether auto-update is enabled.
         """
         return self._auto_update
 
     def enable_auto_update(self):
         """
-        Enable :ref:`auto-update <Auto-updating of resources>` for this
+        Enable :ref:`auto-updating` for this
         resource object, if currently disabled.
 
         When enabling auto-update, the session to which this resource belongs is
         subscribed for auto-updating if needed (see
         :meth:`~zhmcclient.Session.subscribe_auto_update`), the resource
-        object is registered with the session's resource updater via
-        :meth:`~zhmcclient.ResourceUpdater.register_object`, and all properties
+        object is registered with the session's auto updater via
+        :meth:`~zhmcclient.AutoUpdater.register_object`, and all properties
         of this resource object are retrieved using :meth:`pull_full_properties`
         in order to have the most current values as a basis for the future
         auto-updating.
 
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
@@ -609,34 +609,34 @@
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
           :exc:`~zhmcclient.CeasedExistence`
         """
         if not self._auto_update:
             session = self.manager.session
             session.subscribe_auto_update()
-            session.resource_updater.register_object(self)
+            session.auto_updater.register_object(self)
             self._auto_update = True
             self.pull_full_properties()
 
     def disable_auto_update(self):
         """
-        Disable :ref:`auto-update <Auto-updating of resources>` for this
+        Disable :ref:`auto-updating` for this
         resource object, if currently enabled.
 
-        When disabling auto-update, the resource object is unregistered from
-        the session's resource updater via
-        :meth:`~zhmcclient.ResourceUpdater.unregister_object`, and the session
-        is unsubscribed from auto-updating if the resource updater has no more
+        When disabling auto-updating, the resource object is unregistered from
+        the session's auto updater via
+        :meth:`~zhmcclient.AutoUpdater.unregister_object`, and the session
+        is unsubscribed from auto-updating if the auto updater has no more
         objects registered.
         """
         if self._auto_update:
             self._auto_update = False
             session = self.manager.session
-            session.resource_updater.unregister_object(self)
-            if not session.resource_updater.has_objects():
+            session.auto_updater.unregister_object(self)
+            if not session.auto_updater.has_objects():
                 session.unsubscribe_auto_update()
 
     def dump(self):
         """
         Dump this resource with its properties and child resources
         (recursively) as a resource definition.
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_resource_updater.py` & `zhmcclient-1.9.0/zhmcclient/_user_pattern.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,293 +1,351 @@
-#!/usr/bin/env python
-# Copyright 2021 IBM Corp. All Rights Reserved.
+# Copyright 2017-2021 IBM Corp. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Resource updater for
-:ref:`auto-updating of resources <Auto-updating of resources>`.
+A :term:`User Pattern` resource represents a pattern for HMC user IDs that are
+not defined on the HMC but can be verified by an LDAP server for user
+authentication.
+
+User Patterns and user templates allow a system administrator to define a group
+of HMC users at once whose user IDs all match a certain pattern (for example,
+a regular expression) and who have a certain set of attributes. Each pattern
+identifies a template User object which defines many characteristics of such
+users. A successful logon with a user ID that matches a User Pattern results in
+the creation of a pattern-based user, with many of its attributes coming from
+the associated template.
+
+User Patterns are searched in a defined order during logon processing. That
+order can be customized through the
+:meth:`~zhmcclient.UserPatternManager.reorder` method.
 """
 
-import logging
-import json
-try:
-    from json import JSONDecodeError as _JSONDecodeError
-except ImportError:
-    _JSONDecodeError = ValueError
+from __future__ import absolute_import
 
-from ._logging import logged_api_call
-from ._constants import DEFAULT_STOMP_PORT, JMS_LOGGER_NAME
+import copy
 
-__all__ = ['ResourceUpdater']
+from ._manager import BaseManager
+from ._resource import BaseResource
+from ._logging import logged_api_call
+from ._utils import matches_filters, divide_filter_args, RC_USER_PATTERN
 
-JMS_LOGGER = logging.getLogger(JMS_LOGGER_NAME)
+__all__ = ['UserPatternManager', 'UserPattern']
 
 
-class ResourceUpdater(object):
+class UserPatternManager(BaseManager):
     """
-    A class that updates the properties of zhmcclient resource objects that are
-    enabled for auto-updating.
+    Manager providing access to the :term:`User Pattern` resources of a HMC.
 
-    **Experimental:** This class is considered experimental at this point, and
-    its API may change incompatibly as long as it is experimental.
+    Derived from :class:`~zhmcclient.BaseManager`; see there for common methods
+    and attributes.
 
-    Note: The user should not create any objects of this class nor invoke any
-    methods of this class, because the objects are created automatically
-    when a :class:`~zhmcclient.Session` object is subscribed for
-    auto-update (via its :meth:`~zhmcclient.Session.subscribe_auto_update`
-    method).
-
-    Creating an object of this class establishes a JMS session with the HMC and
-    subscribes for the object notification topic of the session. This causes
-    the HMC to emit status notifications, property notifications, and inventory
-    notifications, which are processed by this class and cause the properties of
-    zhmcclient resource objects to be updated that are registered to this class
-    as a result of enabling auto-update for the resorce object
-    (via their :meth:`~zhmcclient.BaseResource.enable_auto_update` method).
+    Objects of this class are not directly created by the user; they are
+    accessible via the following instance variable of a
+    :class:`~zhmcclient.Console` object:
 
-    Zhmcclient resource objects that are not enabled for auto-updating remain
-    unchanged.
+    * :attr:`zhmcclient.Console.user_patterns`
     """
 
-    def __init__(self, session):
+    def __init__(self, console):
+        # This function should not go into the docs.
+        # Parameters:
+        #   console (:class:`~zhmcclient.Console`):
+        #      Console object representing the HMC.
+
+        # Resource properties that are supported as filter query parameters.
+        # If the support for a resource property changes within the set of HMC
+        # versions that support this type of resource, this list must be set up
+        # for the version of the HMC this session is connected to.
+        # Because this resource has case-insensitive names, this list must
+        # contain the name property.
+        query_props = [
+            'name',
+            'type',
+        ]
+
+        super(UserPatternManager, self).__init__(
+            resource_class=UserPattern,
+            class_name=RC_USER_PATTERN,
+            session=console.manager.session,
+            parent=console,
+            base_uri='/api/console/user-patterns',
+            oid_prop='element-id',
+            uri_prop='element-uri',
+            name_prop='name',
+            query_props=query_props,
+            case_insensitive_names=True)
+
+    @property
+    def console(self):
+        """
+        :class:`~zhmcclient.Console`: :term:`Console` defining the scope for
+        this manager.
+        """
+        return self._parent
+
+    @logged_api_call
+    def list(self, full_properties=False, filter_args=None):
         """
+        List the :term:`User Pattern` resources representing the user patterns
+        defined in this HMC.
+
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
+        Authorization requirements:
+
+        * User-related-access permission to the User Pattern objects included
+          in the result, or task permission to the "Manage User Patterns" task.
+
         Parameters:
 
-          session (:class:`~zhmcclient.Session`): Session for which the
-            resource updater should do its work. This defines the HMC host
-            and credentials that are used to establish the JMS session with
-            the HMC.
-        """
-
-        # Registered resource objects, as:
-        #   dict(key: uri, value: dict(key: id, value: object))
-        self._registered_objects = {}
-
-        # Subscription ID. We use some value that allows to identify on the
-        # HMC that this is the zhmcclient, but otherwise we are not using
-        # this value ourselves.
-        self._sub_id = 'zhmcclient.%s' % id(self)
-
-        # Lazy importing for stomp, because it is so slow (ca. 5 sec)
-        if 'Stomp_Connection' not in globals():
-            # pylint: disable=import-outside-toplevel
-            from stomp import Connection as Stomp_Connection
-
-        self._conn = Stomp_Connection(
-            [(session.host, DEFAULT_STOMP_PORT)], use_ssl="SSL")
-        listener = _UpdateListener(self, session)
-        self._conn.set_listener('', listener)
-        # pylint: disable=protected-access
-        self._conn.connect(session.userid, session._password, wait=True)
+          full_properties (bool):
+            Controls whether the full set of resource properties should be
+            retrieved, vs. only the short set as returned by the list
+            operation.
+
+          filter_args (dict):
+            Filter arguments that narrow the list of returned resources to
+            those that match the specified filter arguments. For details, see
+            :ref:`Filtering`.
+
+            `None` causes no filtering to happen, i.e. all resources are
+            returned.
+
+        Returns:
+
+          : A list of :class:`~zhmcclient.UserPattern` objects.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """
+        resource_obj_list = []
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
+        else:
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+                resources_name = 'user-patterns'
+                uri = '{}/{}{}'.format(self.console.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
 
-        dest = "/topic/" + session.object_topic
-        self._conn.subscribe(destination=dest, id=self._sub_id, ack='auto')
+            self.add_resources_local(resource_obj_list)
 
-        JMS_LOGGER.info(
-            "JMS session for object notification topic '%s' has been "
-            "established", session.object_topic)
+        self._name_uri_cache.update_from(resource_obj_list)
+        return resource_obj_list
 
     @logged_api_call
-    def close(self):
+    def create(self, properties):
         """
-        Disconnect and close the JMS session with the HMC.
+        Create a new User Pattern in this HMC.
 
-        This implicitly unsubscribes from the object notification topic this
-        updater was created for.
-        """
-        self._conn.disconnect()
+        Authorization requirements:
 
-    def register_object(self, resource_obj):
-        """
-        Register a resource object to this resource updater.
+        * Task permission to the "Manage User Patterns" task.
 
-        If this resource object (by id) is already registered, nothing is done.
-        """
-        res_uri = resource_obj.uri
-        res_id = id(resource_obj)
-        if res_uri not in self._registered_objects:
-            self._registered_objects[res_uri] = {}
-        id_dict = self._registered_objects[res_uri]
-        if res_id not in id_dict:
-            id_dict[res_id] = resource_obj
+        Parameters:
 
-    def unregister_object(self, resource_obj):
-        """
-        Unregister a resource object from this resource updater.
+          properties (dict): Initial property values.
+            Allowable properties are defined in section 'Request body contents'
+            in section 'Create User Pattern' in the :term:`HMC API` book.
+
+        Returns:
+
+          UserPattern:
+            The resource object for the new User Pattern.
+            The object will have its 'element-uri' property set as returned by
+            the HMC, and will also have the input properties set.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """
+        result = self.session.post(self.console.uri + '/user-patterns',
+                                   body=properties)
+        # There should not be overlaps, but just in case there are, the
+        # returned props should overwrite the input props:
+        props = copy.deepcopy(properties)
+        props.update(result)
+        name = props.get(self._name_prop, None)
+        uri = props[self._uri_prop]
+        user_pattern = UserPattern(self, uri, name, props)
+        self._name_uri_cache.update(name, uri)
+        return user_pattern
 
-        If this resource object (by id) is already unregistered, nothing is
-        done.
+    @logged_api_call
+    def reorder(self, user_patterns):
         """
-        res_uri = resource_obj.uri
-        res_id = id(resource_obj)
-        if res_uri in self._registered_objects:
-            id_dict = self._registered_objects[res_uri]
-            if res_id in id_dict:
-                del id_dict[res_id]
-            if not id_dict:
-                del self._registered_objects[res_uri]
+        Reorder the User Patterns of the HMC as specified.
 
-    def registered_objects(self, resource_uri):
-        """
-        Generator that yields the resource objects for the specified URI.
-        """
-        if resource_uri in self._registered_objects:
-            id_dict = self._registered_objects[resource_uri]
-            for res_obj in id_dict.values():
-                yield res_obj
+        The order of User Patterns determines the search order during logon
+        processing.
 
-    def has_objects(self):
-        """
-        Return boolean indicating whether there are any resource objects
-        registered.
-        """
-        return bool(self._registered_objects)
+        Authorization requirements:
+
+        * Task permission to the "Manage User Patterns" task.
+
+        Parameters:
+
+          user_patterns (list of :class:`~zhmcclient.UserPattern`):
+            The User Patterns in the desired order.
 
+            Must not be `None`.
 
-class _UpdateListener(object):
-    # pylint: disable=too-few-public-methods
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """  # noqa: E501
+        body = {
+            'user-pattern-uris': [up.uri for up in user_patterns]
+        }
+        self.session.post(
+            '/api/console/operations/reorder-user-patterns',
+            body=body)
+
+
+class UserPattern(BaseResource):
     """
-    A notification listener class for use by the Python `stomp` package.
+    Representation of a :term:`User Pattern`.
 
-    This is an internal class that does not need to be accessed or created by
-    the user. An object of this class is automatically created by the
-    :class:`~zhmcclient.ResourceUpdater` class, for its notification
-    topic.
-
-    Note: In the stomp examples, this class inherits from
-    stomp.ConnectionListener. However, since that class defines only empty
-    methods and since we want to import the stomp module in a lazy manner,
-    we are not using that class, and stomp does not require us to.
+    Derived from :class:`~zhmcclient.BaseResource`; see there for common
+    methods and attributes.
+
+    Objects of this class are not directly created by the user; they are
+    returned from creation or list functions on their manager object
+    (in this case, :class:`~zhmcclient.UserPatternManager`).
     """
 
-    def __init__(self, updater, session):
-        self._updater = updater
-        self._session = session
+    def __init__(self, manager, uri, name=None, properties=None):
+        # This function should not go into the docs.
+        #   manager (:class:`~zhmcclient.UserPatternManager`):
+        #     Manager object for this resource object.
+        #   uri (string):
+        #     Canonical URI path of the resource.
+        #   name (string):
+        #     Name of the resource.
+        #   properties (dict):
+        #     Properties to be set for this resource object. May be `None` or
+        #     empty.
+        assert isinstance(manager, UserPatternManager), \
+            "Console init: Expected manager type %s, got %s" % \
+            (UserPatternManager, type(manager))
+        super(UserPattern, self).__init__(manager, uri, name, properties)
 
-    def on_message(self, headers, message):
+    @logged_api_call
+    def delete(self):
         """
-        Event method that gets called when this listener has received a JMS
-        message (representing an HMC notification).
+        Delete this User Pattern.
 
-        Parameters:
+        Authorization requirements:
 
-          headers (dict): JMS message headers, see HMC API book.
+        * Task permission to the "Manage User Patterns" task.
 
-          message (string): JMS message body as a string, which contains a
-            serialized JSON object, see HMC API book.
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
         """
-        try:
-            uri = headers['object-uri']
-        except KeyError:
-            try:
-                uri = headers['element-uri']
-            except KeyError:
-                JMS_LOGGER.error(
-                    "JMS message for object notification topic '%s' "
-                    "has no URI field in its headers (ignored): %r",
-                    self._session.object_topic, headers)
-                return
-
-        noti_type = headers['notification-type']
-        if noti_type == 'property-change':
-            try:
-                msg_obj = json.loads(message)
-            except _JSONDecodeError:
-                JMS_LOGGER.error(
-                    "JMS message for object notification topic '%s' "
-                    "has a non-JSON message body (ignored): %r",
-                    self._session.object_topic, message)
-                return
-            JMS_LOGGER.debug(
-                "JMS message for property change notification for topic '%s' "
-                "for resource %s with change reports: %r",
-                self._session.object_topic, uri, msg_obj['change-reports'])
-            # Build the latest values from all change records. They are ordered
-            # old to new.
-            new_props = {}
-            for cr in msg_obj['change-reports']:
-                new_props[cr['property-name']] = cr['new-value']
-            for obj in self._updater.registered_objects(uri):
-                if obj.auto_update_enabled():
-                    obj.update_properties_local(new_props)
-        elif noti_type == 'status-change':
-            try:
-                msg_obj = json.loads(message)
-            except _JSONDecodeError:
-                JMS_LOGGER.error(
-                    "JMS message for object notification topic '%s' "
-                    "has a non-JSON message body (ignored): %r",
-                    self._session.object_topic, message)
-                return
-            JMS_LOGGER.debug(
-                "JMS message for status change notification for topic '%s' "
-                "for resource %s with change reports: %r",
-                self._session.object_topic, uri, msg_obj['change-reports'])
-            # Build the latest values from all change records. They are ordered
-            # old to new.
-            new_props = {}
-            for cr in msg_obj['change-reports']:
-                if 'new-status' in cr:
-                    new_props['status'] = cr['new-status']
-                if 'new-additional-status' in cr:
-                    new_props['additional-status'] = cr['new-additional-status']
-                if 'has-unacceptable-status' in cr:
-                    new_props['has-unacceptable-status'] = \
-                        cr['has-unacceptable-status']
-            for obj in self._updater.registered_objects(uri):
-                if obj.auto_update_enabled():
-                    obj.update_properties_local(new_props)
-        elif noti_type == 'inventory-change':
-            action = headers['action']
-            JMS_LOGGER.debug(
-                "JMS message for inventory change notification for topic '%s' "
-                "for resource %s with action: %r",
-                self._session.object_topic, uri, action)
-            if action == 'remove':
-                for obj in self._updater.registered_objects(uri):
-                    if obj.auto_update_enabled():
-                        obj.cease_existence_local()
-        else:
-            JMS_LOGGER.warning(
-                "JMS message for notification of type %s for topic '%s' "
-                "for resource %s is ignored",
-                noti_type, self._session.object_topic, uri)
-
-    def on_error(self, headers, message):
-        # pylint: disable=unused-argument
-        """
-        Event method that gets called when this listener has received a JMS
-        error. This happens for example when the client registers for a
-        non-existing topic.
+        # pylint: disable=protected-access
+        self.manager.session.delete(self.uri)
+        self.manager._name_uri_cache.delete(
+            self.get_properties_local(self.manager._name_prop, None))
 
-        Parameters:
+    @logged_api_call
+    def update_properties(self, properties):
+        """
+        Update writeable properties of this UserPattern.
 
-          headers (dict): JMS message headers.
+        This method serializes with other methods that access or change
+        properties on the same Python object.
 
-          message (string): JMS message body as a string, which contains a
-            serialized JSON object.
-        """
-        JMS_LOGGER.error(
-            "JMS error message received for object notification topic '%s' "
-            "(ignored): %s",
-            self._session.object_topic, message)
+        Authorization requirements:
 
-    def on_disconnected(self):
-        """
-        Event method that gets called when the JMS session has been
-        disconnected.
+        * Task permission to the "Manage User Patterns" task.
+
+        Parameters:
+
+          properties (dict): New values for the properties to be updated.
+            Properties not to be updated are omitted.
+            Allowable properties are the properties with qualifier (w) in
+            section 'Data model' in section 'User Pattern object' in the
+            :term:`HMC API` book.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
         """
-        JMS_LOGGER.info(
-            "JMS session for object notification topic '%s' has been "
-            "disconnected",
-            self._session.object_topic)
+        # pylint: disable=protected-access
+        self.manager.session.post(self.uri, body=properties)
+        is_rename = self.manager._name_prop in properties
+        if is_rename:
+            # Delete the old name from the cache
+            self.manager._name_uri_cache.delete(self.name)
+        self.update_properties_local(copy.deepcopy(properties))
+        if is_rename:
+            # Add the new name to the cache
+            self.manager._name_uri_cache.update(self.name, self.uri)
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_session.py` & `zhmcclient-1.9.0/zhmcclient/_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 from ._exceptions import HTTPError, ServerAuthError, ClientAuthError, \
     ParseError, ConnectTimeout, ReadTimeout, RetriesExceeded, \
     OperationTimeout, Error
 from ._exceptions import ConnectionError  # pylint: disable=redefined-builtin
 
 from ._timestats import TimeStatsKeeper
-from ._resource_updater import ResourceUpdater
+from ._auto_updater import AutoUpdater
 from ._logging import get_logger, logged_api_call
 from ._constants import DEFAULT_CONNECT_TIMEOUT, DEFAULT_CONNECT_RETRIES, \
     DEFAULT_READ_TIMEOUT, DEFAULT_READ_RETRIES, DEFAULT_MAX_REDIRECTS, \
     DEFAULT_OPERATION_TIMEOUT, DEFAULT_STATUS_TIMEOUT, \
     DEFAULT_NAME_URI_CACHE_TIMETOLIVE, HMC_LOGGER_NAME, \
     HTML_REASON_WEB_SERVICES_DISABLED, HTML_REASON_OTHER, \
     DEFAULT_HMC_PORT
@@ -425,15 +425,15 @@
         else:
             # Create a logged-off state (same state as in _do_logoff())
             self._session_id = None
             self._session = None
         self._time_stats_keeper = TimeStatsKeeper()
         self._object_topic = None
         self._job_topic = None
-        self._resource_updater = None
+        self._auto_updater = AutoUpdater(self)
 
     def __repr__(self):
         """
         Return a string with the state of this session, for debug purposes.
         """
         headers = _headers_for_logging(self.headers)
         ret = (
@@ -446,15 +446,15 @@
             "  _retry_timeout_config={s._retry_timeout_config!r},\n"
             "  _base_url={s._base_url!r},\n"
             "  _headers={headers!r},\n"
             "  _session_id={blanked_out!r},\n"
             "  _session={s._session!r}\n"
             "  _object_topic={s._object_topic!r}\n"
             "  _job_topic={s._job_topic!r}\n"
-            "  _resource_updater={s._resource_updater!r}\n"
+            "  _auto_updater={s._auto_updater!r}\n"
             ")".
             format(classname=self.__class__.__name__, id=id(self), s=self,
                    headers=headers, blanked_out=BLANKED_OUT))
         return ret
 
     @property
     def host(self):
@@ -605,20 +605,20 @@
         When not logged on, this property is `None`.
 
         The associated topic type is "job-notification".
         """
         return self._job_topic
 
     @property
-    def resource_updater(self):
+    def auto_updater(self):
         """
-        :class:`~zhmcclient.ResourceUpdater`: Resource updater for
-        :ref:`auto-updating <Auto-updating of resources>` of resources.
+        :class:`~zhmcclient.AutoUpdater`: Updater for
+        :ref:`auto-updating` of resource and manager objects.
         """
-        return self._resource_updater
+        return self._auto_updater
 
     @logged_api_call
     def logon(self, verify=False):
         """
         Make sure this session object is logged on to the HMC.
 
         If `verify=False`, this method determines the logged-on state of this
@@ -1388,57 +1388,56 @@
         topics_uri = '/api/sessions/operations/get-notification-topics'
         response = self.get(topics_uri)
         return response['topics']
 
     def auto_update_subscribed(self):
         """
         Return whether this session is currently subscribed for
-        :ref:`auto-updating of resources <Auto-updating of resources>`.
+        :ref:`auto-updating`.
 
         Return:
           bool: Indicates whether session is subscribed.
         """
-        return bool(self._resource_updater)
+        return self._auto_updater.is_open()
 
     @logged_api_call
     def subscribe_auto_update(self):
         """
-        Subscribe this session for
-        :ref:`auto-updating of resources <Auto-updating of resources>`, if not
-        currently subscribed.
+        Subscribe this session for :ref:`auto-updating`, if not currently
+        subscribed.
+
+        When not yet subscribed, the session is also logged on.
 
         When subscribed, object notifications will be sent by the HMC as
         resource objects on the HMC change their properties or come or go.
         These object notifications will be received by the client and will then
         update the properties of any Python resource objects that are enabled
         for auto-updating.
 
         This method is automatically called by
         :meth:`~zhmcclient.BaseResource.enable_auto_update` and thus does not
         need to be called by the user.
         """
-        if not self._resource_updater:
-            self._resource_updater = ResourceUpdater(self)
+        if not self._auto_updater.is_open():
+            self._auto_updater.open()
 
     @logged_api_call
     def unsubscribe_auto_update(self):
         """
-        Unsubscribe this session from
-        :ref:`auto-updating of resources <Auto-updating of resources>`, if
+        Unsubscribe this session from :ref:`auto-updating`, if
         currently subscribed.
 
         When unsubscribed, object notifications are no longer sent by the HMC.
 
         This method is automatically called by
         :meth:`~zhmcclient.BaseResource.disable_auto_update` and thus does not
         need to be called by the user.
         """
-        if self._resource_updater:
-            self._resource_updater.close()
-            self._resource_updater = None
+        if self._auto_updater.is_open():
+            self._auto_updater.close()
 
 
 class Job(object):
     """
     A job on the HMC that performs an asynchronous HMC operation.
 
     This class supports checking the job for completion, and waiting for job
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_storage_group.py` & `zhmcclient-1.9.0/zhmcclient/_storage_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,34 @@
     def list(self, full_properties=False, filter_args=None):
         """
         List the storage groups defined in the HMC.
 
         Storage groups for which the authenticated user does not have
         object-access permission are not included.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to any storage groups to be included in the
           result.
 
         Parameters:
 
@@ -180,44 +200,48 @@
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
-
         resource_obj_list = []
-
-        if filter_args is None:
-            filter_args = {}
-
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
-            uri = '{}{}'.format(self._base_uri, query_parms)
-
-            result = self.session.get(uri)
-            if result:
-                props_list = result['storage-groups']
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            if filter_args is None:
+                filter_args = {}
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+                uri = '{}{}'.format(self._base_uri, query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result['storage-groups']
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
+
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties=None, template=None):
         """
@@ -349,16 +373,16 @@
         """
         :class:`~zhmcclient.VirtualStorageResourceManager`: Access to the
         :term:`virtual storage resources <Virtual Storage Resource>` in this
         storage group.
         """
         # We do here some lazy loading.
         if not self._virtual_storage_resources:
-            self._virtual_storage_resources = \
-                VirtualStorageResourceManager(self)
+            self._virtual_storage_resources = VirtualStorageResourceManager(
+                self)
         return self._virtual_storage_resources
 
     @property
     def cpc(self):
         """
         :class:`~zhmcclient.Cpc`: The :term:`CPC` to which this storage group
         is associated.
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_storage_group_template.py` & `zhmcclient-1.9.0/zhmcclient/_storage_group_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,34 @@
     def list(self, full_properties=False, filter_args=None):
         """
         List the storage group templates defined in the HMC.
 
         Storage group templates for which the authenticated user does not have
         object-access permission are not included.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to any storage group templates to be
           included in the result.
 
         Parameters:
 
@@ -122,44 +142,48 @@
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
-
         resource_obj_list = []
-
-        if filter_args is None:
-            filter_args = {}
-
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
-            uri = '{}{}'.format(self._base_uri, query_parms)
-
-            result = self.session.get(uri)
-            if result:
-                props_list = result['storage-templates']
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            if filter_args is None:
+                filter_args = {}
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+                uri = '{}{}'.format(self._base_uri, query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result['storage-templates']
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
+
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties):
         """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_storage_volume.py` & `zhmcclient-1.9.0/zhmcclient/_storage_volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,34 @@
         return self._parent
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the storage volumes in this storage group.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to this storage group.
 
         Parameters:
 
           full_properties (bool):
@@ -134,44 +154,49 @@
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
-
         resource_obj_list = []
-
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+
+                resources_name = 'storage-volumes'
+                uri = '{}/{}{}'.format(self.storage_group.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
 
-            resources_name = 'storage-volumes'
-            uri = '{}/{}{}'.format(self.storage_group.uri, resources_name,
-                                   query_parms)
-
-            result = self.session.get(uri)
-            if result:
-                props_list = result[resources_name]
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties, email_to_addresses=None,
                email_cc_addresses=None, email_insert=None):
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_storage_volume_template.py` & `zhmcclient-1.9.0/zhmcclient/_storage_volume_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,14 +100,34 @@
         return self._parent
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the storage volume templates in this storage group template.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to this storage group template.
 
         Parameters:
 
           full_properties (bool):
@@ -130,44 +150,49 @@
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
-
         resource_obj_list = []
-
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+
+                resources_name = 'storage-template-volumes'
+                uri = '{}/{}{}'.format(self.storage_group_template.uri,
+                                       resources_name, query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
 
-            resources_name = 'storage-template-volumes'
-            uri = '{}/{}{}'.format(self.storage_group_template.uri,
-                                   resources_name, query_parms)
-
-            result = self.session.get(uri)
-            if result:
-                props_list = result[resources_name]
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties):
         """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_task.py` & `zhmcclient-1.9.0/zhmcclient/_task.py`

 * *Files 20% similar despite different names*

```diff
@@ -79,14 +79,34 @@
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the :term:`Task` resources representing the tasks defined in this
         HMC.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * None
 
         Parameters:
 
           full_properties (bool):
@@ -110,34 +130,47 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        query_parms, client_filters = divide_filter_args(
-            self._query_props, filter_args)
-        resources_name = 'tasks'
-        uri = '{}/{}{}'.format(self.console.uri, resources_name, query_parms)
-
-        result = self.session.get(uri)
-        if result:
-            props_list = result[resources_name]
-            for props in props_list:
-
-                resource_obj = self.resource_class(
-                    manager=self,
-                    uri=props[self._uri_prop],
-                    name=props.get(self._name_prop, None),
-                    properties=props)
-
-                if matches_filters(resource_obj, client_filters):
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
                     resource_obj_list.append(resource_obj)
-                    if full_properties:
-                        resource_obj.pull_full_properties()
+        else:
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+                resources_name = 'tasks'
+                uri = '{}/{}{}'.format(self.console.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
+
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
 
 class Task(BaseResource):
     """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_timestats.py` & `zhmcclient-1.9.0/zhmcclient/_timestats.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/_unmanaged_cpc.py` & `zhmcclient-1.9.0/zhmcclient/_unmanaged_cpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -90,14 +90,34 @@
         Because the CPCs are unmanaged, the returned
         :class:`~zhmcclient.UnmanagedCpc` objects cannot perform any operations
         and will have only the following properties:
 
         * ``object-uri``
         * ``name``
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * None
 
         Parameters:
 
           full_properties (bool):
@@ -119,37 +139,44 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
-
-            uri = self.parent.uri + '/operations/list-unmanaged-cpcs' + \
-                query_parms
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+
+                uri = self.parent.uri + '/operations/list-unmanaged-cpcs' + \
+                    query_parms
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result['cpcs']
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
 
-            result = self.session.get(uri)
-            if result:
-                props_list = result['cpcs']
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
 
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
 
 class UnmanagedCpc(BaseResource):
     """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_user.py` & `zhmcclient-1.9.0/zhmcclient/_user.py`

 * *Files 23% similar despite different names*

```diff
@@ -81,14 +81,34 @@
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the :term:`User` resources representing the users defined in this
         HMC.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * User-related-access permission to the User object included in the
           result, or, depending on the type of User object, task permission to
           the "Manage Users" task or the "Manage User Templates" task.
 
         Parameters:
@@ -114,34 +134,47 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        query_parms, client_filters = divide_filter_args(
-            self._query_props, filter_args)
-        resources_name = 'users'
-        uri = '{}/{}{}'.format(self.console.uri, resources_name, query_parms)
-
-        result = self.session.get(uri)
-        if result:
-            props_list = result[resources_name]
-            for props in props_list:
-
-                resource_obj = self.resource_class(
-                    manager=self,
-                    uri=props[self._uri_prop],
-                    name=props.get(self._name_prop, None),
-                    properties=props)
-
-                if matches_filters(resource_obj, client_filters):
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
                     resource_obj_list.append(resource_obj)
-                    if full_properties:
-                        resource_obj.pull_full_properties()
+        else:
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+                resources_name = 'users'
+                uri = '{}/{}{}'.format(self.console.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
+
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties):
         """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_user_pattern.py` & `zhmcclient-1.9.0/zhmcclient/_virtual_function.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,112 +1,111 @@
-# Copyright 2017-2021 IBM Corp. All Rights Reserved.
+# Copyright 2016-2021 IBM Corp. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-A :term:`User Pattern` resource represents a pattern for HMC user IDs that are
-not defined on the HMC but can be verified by an LDAP server for user
-authentication.
-
-User Patterns and user templates allow a system administrator to define a group
-of HMC users at once whose user IDs all match a certain pattern (for example,
-a regular expression) and who have a certain set of attributes. Each pattern
-identifies a template User object which defines many characteristics of such
-users. A successful logon with a user ID that matches a User Pattern results in
-the creation of a pattern-based user, with many of its attributes coming from
-the associated template.
-
-User Patterns are searched in a defined order during logon processing. That
-order can be customized through the
-:meth:`~zhmcclient.UserPatternManager.reorder` method.
+A :term:`Virtual Function` is a logical entity that provides a
+:term:`Partition` with access to
+:term:`Accelerator Adapters <Accelerator Adapter>`.
+
+Virtual Function resources are contained in Partition resources.
+
+Virtual Functions only exist in :term:`CPCs <CPC>` that are in DPM mode.
 """
 
 from __future__ import absolute_import
 
 import copy
 
 from ._manager import BaseManager
 from ._resource import BaseResource
 from ._logging import logged_api_call
-from ._utils import matches_filters, divide_filter_args, RC_USER_PATTERN
+from ._utils import matches_filters, RC_VIRTUAL_FUNCTION
 
-__all__ = ['UserPatternManager', 'UserPattern']
+__all__ = ['VirtualFunctionManager', 'VirtualFunction']
 
 
-class UserPatternManager(BaseManager):
+class VirtualFunctionManager(BaseManager):
     """
-    Manager providing access to the :term:`User Pattern` resources of a HMC.
+    Manager providing access to the
+    :term:`Virtual Functions <Virtual Function>` in a particular
+    :term:`Partition`.
 
     Derived from :class:`~zhmcclient.BaseManager`; see there for common methods
     and attributes.
 
     Objects of this class are not directly created by the user; they are
     accessible via the following instance variable of a
-    :class:`~zhmcclient.Console` object:
+    :class:`~zhmcclient.Partition` object (in DPM mode):
 
-    * :attr:`zhmcclient.Console.user_patterns`
+    * :attr:`~zhmcclient.Partition.virtual_functions`
     """
 
-    def __init__(self, console):
+    def __init__(self, partition):
         # This function should not go into the docs.
         # Parameters:
-        #   console (:class:`~zhmcclient.Console`):
-        #      Console object representing the HMC.
-
-        # Resource properties that are supported as filter query parameters.
-        # If the support for a resource property changes within the set of HMC
-        # versions that support this type of resource, this list must be set up
-        # for the version of the HMC this session is connected to.
-        # Because this resource has case-insensitive names, this list must
-        # contain the name property.
-        query_props = [
-            'name',
-            'type',
-        ]
-
-        super(UserPatternManager, self).__init__(
-            resource_class=UserPattern,
-            class_name=RC_USER_PATTERN,
-            session=console.manager.session,
-            parent=console,
-            base_uri='/api/console/user-patterns',
+        #   partition (:class:`~zhmcclient.Partition`):
+        #     Partition defining the scope for this manager.
+        super(VirtualFunctionManager, self).__init__(
+            resource_class=VirtualFunction,
+            class_name=RC_VIRTUAL_FUNCTION,
+            session=partition.manager.session,
+            parent=partition,
+            base_uri='{}/virtual-functions'.format(partition.uri),
             oid_prop='element-id',
             uri_prop='element-uri',
             name_prop='name',
-            query_props=query_props,
-            case_insensitive_names=True)
+            query_props=[],
+            list_has_name=False)
 
     @property
-    def console(self):
+    def partition(self):
         """
-        :class:`~zhmcclient.Console`: :term:`Console` defining the scope for
-        this manager.
+        :class:`~zhmcclient.Partition`: :term:`Partition` defining the scope
+        for this manager.
         """
         return self._parent
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
-        List the :term:`User Pattern` resources representing the user patterns
-        defined in this HMC.
+        List the Virtual Functions of this Partition.
+
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the corresponding array property for this resource in the
+          parent object is used to list the resources, and the provided filter
+          arguments are applied.
 
         Authorization requirements:
 
-        * User-related-access permission to the User Pattern objects included
-          in the result, or task permission to the "Manage User Patterns" task.
+        * Object-access permission to this Partition.
 
         Parameters:
 
           full_properties (bool):
             Controls whether the full set of resource properties should be
             retrieved, vs. only the short set as returned by the list
             operation.
@@ -117,190 +116,176 @@
             :ref:`Filtering`.
 
             `None` causes no filtering to happen, i.e. all resources are
             returned.
 
         Returns:
 
-          : A list of :class:`~zhmcclient.UserPattern` objects.
+          : A list of :class:`~zhmcclient.VirtualFunction` objects.
 
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        query_parms, client_filters = divide_filter_args(
-            self._query_props, filter_args)
-        resources_name = 'user-patterns'
-        uri = '{}/{}{}'.format(self.console.uri, resources_name, query_parms)
-
-        result = self.session.get(uri)
-        if result:
-            props_list = result[resources_name]
-            for props in props_list:
-
-                resource_obj = self.resource_class(
-                    manager=self,
-                    uri=props[self._uri_prop],
-                    name=props.get(self._name_prop, None),
-                    properties=props)
-
-                if matches_filters(resource_obj, client_filters):
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
                     resource_obj_list.append(resource_obj)
-                    if full_properties:
-                        resource_obj.pull_full_properties()
+        else:
+            uris = self.partition.get_property('virtual-function-uris')
+            if uris:
+                for uri in uris:
+
+                    resource_obj = self.resource_class(
+                        manager=self,
+                        uri=uri,
+                        name=None,
+                        properties=None)
+
+                    if matches_filters(resource_obj, filter_args):
+                        resource_obj_list.append(resource_obj)
+                        if full_properties:
+                            resource_obj.pull_full_properties()
+
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties):
         """
-        Create a new User Pattern in this HMC.
+        Create a Virtual Function in this Partition.
 
         Authorization requirements:
 
-        * Task permission to the "Manage User Patterns" task.
+        * Object-access permission to this Partition.
+        * Object-access permission to the backing accelerator Adapter.
+        * Task permission for the "Partition Details" task.
 
         Parameters:
 
           properties (dict): Initial property values.
             Allowable properties are defined in section 'Request body contents'
-            in section 'Create User Pattern' in the :term:`HMC API` book.
+            in section 'Create Virtual Function' in the :term:`HMC API` book.
 
         Returns:
 
-          UserPattern:
-            The resource object for the new User Pattern.
+          VirtualFunction:
+            The resource object for the new Virtual Function.
             The object will have its 'element-uri' property set as returned by
             the HMC, and will also have the input properties set.
 
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
-        result = self.session.post(self.console.uri + '/user-patterns',
+        result = self.session.post(self.partition.uri + '/virtual-functions',
                                    body=properties)
         # There should not be overlaps, but just in case there are, the
         # returned props should overwrite the input props:
         props = copy.deepcopy(properties)
         props.update(result)
         name = props.get(self._name_prop, None)
         uri = props[self._uri_prop]
-        user_pattern = UserPattern(self, uri, name, props)
+        vf = VirtualFunction(self, uri, name, props)
         self._name_uri_cache.update(name, uri)
-        return user_pattern
-
-    @logged_api_call
-    def reorder(self, user_patterns):
-        """
-        Reorder the User Patterns of the HMC as specified.
-
-        The order of User Patterns determines the search order during logon
-        processing.
-
-        Authorization requirements:
+        return vf
 
-        * Task permission to the "Manage User Patterns" task.
 
-        Parameters:
-
-          user_patterns (list of :class:`~zhmcclient.UserPattern`):
-            The User Patterns in the desired order.
-
-            Must not be `None`.
-
-        Raises:
-
-          :exc:`~zhmcclient.HTTPError`
-          :exc:`~zhmcclient.ParseError`
-          :exc:`~zhmcclient.AuthError`
-          :exc:`~zhmcclient.ConnectionError`
-        """  # noqa: E501
-        body = {
-            'user-pattern-uris': [up.uri for up in user_patterns]
-        }
-        self.session.post(
-            '/api/console/operations/reorder-user-patterns',
-            body=body)
-
-
-class UserPattern(BaseResource):
+class VirtualFunction(BaseResource):
     """
-    Representation of a :term:`User Pattern`.
+    Representation of a :term:`Virtual Function`.
 
     Derived from :class:`~zhmcclient.BaseResource`; see there for common
     methods and attributes.
 
+    For the properties of a Virtual Function, see section
+    'Data model - Virtual Function Element Object' in section
+    'Partition object' in the :term:`HMC API` book.
+
     Objects of this class are not directly created by the user; they are
     returned from creation or list functions on their manager object
-    (in this case, :class:`~zhmcclient.UserPatternManager`).
+    (in this case, :class:`~zhmcclient.VirtualFunctionManager`).
     """
 
     def __init__(self, manager, uri, name=None, properties=None):
         # This function should not go into the docs.
-        #   manager (:class:`~zhmcclient.UserPatternManager`):
+        #   manager (:class:`~zhmcclient.VirtualFunctionManager`):
         #     Manager object for this resource object.
         #   uri (string):
         #     Canonical URI path of the resource.
         #   name (string):
         #     Name of the resource.
         #   properties (dict):
         #     Properties to be set for this resource object. May be `None` or
         #     empty.
-        assert isinstance(manager, UserPatternManager), \
-            "Console init: Expected manager type %s, got %s" % \
-            (UserPatternManager, type(manager))
-        super(UserPattern, self).__init__(manager, uri, name, properties)
+        assert isinstance(manager, VirtualFunctionManager), \
+            "VirtualFunction init: Expected manager type %s, got %s" % \
+            (VirtualFunctionManager, type(manager))
+        super(VirtualFunction, self).__init__(manager, uri, name, properties)
 
     @logged_api_call
     def delete(self):
         """
-        Delete this User Pattern.
+        Delete this Virtual Function.
 
         Authorization requirements:
 
-        * Task permission to the "Manage User Patterns" task.
+        * Object-access permission to the Partition of this Virtual Function.
+        * Task permission for the "Partition Details" task.
 
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         # pylint: disable=protected-access
-        self.manager.session.delete(self.uri)
+        self.manager.session.delete(self._uri)
         self.manager._name_uri_cache.delete(
             self.get_properties_local(self.manager._name_prop, None))
 
+        parent_vf_uris = self.manager.parent.get_properties_local(
+            'virtual-function-uris')
+        if parent_vf_uris:
+            try:
+                parent_vf_uris.remove(self._uri)
+            except ValueError:
+                pass
+
     @logged_api_call
     def update_properties(self, properties):
         """
-        Update writeable properties of this UserPattern.
+        Update writeable properties of this Virtual Function.
 
         This method serializes with other methods that access or change
         properties on the same Python object.
 
         Authorization requirements:
 
-        * Task permission to the "Manage User Patterns" task.
+        * Object-access permission to the Partition of this Virtual Function.
+        * When updating the "adapter-uri" property, object-access permission to
+          the Adapter identified in that URI.
+        * Task permission for the "Partition Details" task.
 
         Parameters:
 
           properties (dict): New values for the properties to be updated.
             Properties not to be updated are omitted.
             Allowable properties are the properties with qualifier (w) in
-            section 'Data model' in section 'User Pattern object' in the
+            section 'Data model - Virtual Function element object' in the
             :term:`HMC API` book.
 
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_user_role.py` & `zhmcclient-1.9.0/zhmcclient/_user_role.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,14 +89,34 @@
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the :term:`User Role` resources representing the user roles
         defined in this HMC.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * User-related-access permission to the User Role objects included in
           the result, or task permission to the "Manage User Roles" task.
 
         Parameters:
 
@@ -121,34 +141,47 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        query_parms, client_filters = divide_filter_args(
-            self._query_props, filter_args)
-        resources_name = 'user-roles'
-        uri = '{}/{}{}'.format(self.console.uri, resources_name, query_parms)
-
-        result = self.session.get(uri)
-        if result:
-            props_list = result[resources_name]
-            for props in props_list:
-
-                resource_obj = self.resource_class(
-                    manager=self,
-                    uri=props[self._uri_prop],
-                    name=props.get(self._name_prop, None),
-                    properties=props)
-
-                if matches_filters(resource_obj, client_filters):
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
                     resource_obj_list.append(resource_obj)
-                    if full_properties:
-                        resource_obj.pull_full_properties()
+        else:
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+                resources_name = 'user-roles'
+                uri = '{}/{}{}'.format(self.console.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
+
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
     @logged_api_call
     def create(self, properties):
         """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_utils.py` & `zhmcclient-1.9.0/zhmcclient/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,44 @@
 RC_PASSWORD_RULE = 'password-rule'
 RC_TASK = 'task'
 RC_USER_PATTERN = 'user-pattern'
 RC_USER_ROLE = 'user-role'
 RC_USER = 'user'
 RC_GROUP = 'group'
 
+# Resource classes that are children of zhmcclient.Cpc
+RC_CHILDREN_CPC = (
+    RC_PARTITION,
+    RC_ADAPTER,
+    RC_VIRTUAL_SWITCH,
+    RC_CAPACITY_GROUP,
+    RC_LOGICAL_PARTITION,
+    RC_RESET_ACTIVATION_PROFILE,
+    RC_IMAGE_ACTIVATION_PROFILE,
+    RC_LOAD_ACTIVATION_PROFILE,
+)
+# Resource classes that are children of zhmcclient.Console
+RC_CHILDREN_CONSOLE = (
+    RC_STORAGE_GROUP,
+    RC_STORAGE_TEMPLATE,
+    RC_PASSWORD_RULE,
+    RC_TASK,
+    RC_USER_PATTERN,
+    RC_USER_ROLE,
+    RC_USER,
+    RC_LDAP_SERVER_DEFINITION,
+    RC_CPC,  # For unmanaged CPCs
+)
+# Resource classes that are children of zhmcclient.Client (= top level)
+RC_CHILDREN_CLIENT = (
+    RC_CPC,  # For managed CPCs
+    RC_CONSOLE,
+)
+
+
 # Valid resource class names
 #:
 VALID_RESOURCE_CLASSES = frozenset([
     RC_ADAPTER,
     RC_CAPACITY_GROUP,
     RC_HBA,
     RC_NIC,
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_version.py` & `zhmcclient-1.9.0/zhmcclient/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.P.dev1": A not yet released version M.N.P
 #: * "M.N.P": A released version M.N.P
-__version__ = '1.8.2'
+__version__ = '1.9.0'
 
 # Check supported Python versions
 # Keep these Python versions in sync with:
 # - python_requires and classifiers in setup.py
 # - Section "Supported environments" in docs/intro.rst
 _PYTHON_M = sys.version_info[0]
 _PYTHON_N = sys.version_info[1]
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_virtual_storage_resource.py` & `zhmcclient-1.9.0/zhmcclient/_virtual_storage_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,14 +113,34 @@
         return self._parent
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the virtual storage resources in this storage group.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to this storage group.
 
         Parameters:
 
           full_properties (bool):
@@ -144,44 +164,49 @@
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
-
         resource_obj_list = []
-
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+
+                resources_name = 'virtual-storage-resources'
+                uri = '{}/{}{}'.format(self.storage_group.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
 
-            resources_name = 'virtual-storage-resources'
-            uri = '{}/{}{}'.format(self.storage_group.uri, resources_name,
-                                   query_parms)
-
-            result = self.session.get(uri)
-            if result:
-                props_list = result[resources_name]
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
 
 class VirtualStorageResource(BaseResource):
     """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/_virtual_switch.py` & `zhmcclient-1.9.0/zhmcclient/_virtual_switch.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,14 +87,34 @@
         return self._parent
 
     @logged_api_call
     def list(self, full_properties=False, filter_args=None):
         """
         List the Virtual Switches in this CPC.
 
+        Any resource property may be specified in a filter argument. For
+        details about filter arguments, see :ref:`Filtering`.
+
+        The listing of resources is handled in an optimized way:
+
+        * If this manager is enabled for :ref:`auto-updating`, a locally
+          maintained resource list is used (which is automatically updated via
+          inventory notifications from the HMC) and the provided filter
+          arguments are applied.
+
+        * Otherwise, if the filter arguments specify the resource name as a
+          single filter argument with a straight match string (i.e. without
+          regular expressions), an optimized lookup is performed based on a
+          locally maintained name-URI cache.
+
+        * Otherwise, the HMC List operation is performed with the subset of the
+          provided filter arguments that can be handled on the HMC side and the
+          remaining filter arguments are applied on the client side on the list
+          result.
+
         Authorization requirements:
 
         * Object-access permission to this CPC.
         * Object-access permission to the backing Adapters of any Virtual
           Switches to be included in the result.
 
         Parameters:
@@ -120,40 +140,48 @@
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
         resource_obj_list = []
-        resource_obj = self._try_optimized_lookup(filter_args)
-        if resource_obj:
-            resource_obj_list.append(resource_obj)
-            # It already has full properties
+        if self.auto_update_enabled() and not self.auto_update_needs_pull():
+            for resource_obj in self.list_resources_local():
+                if matches_filters(resource_obj, filter_args):
+                    resource_obj_list.append(resource_obj)
         else:
-            query_parms, client_filters = divide_filter_args(
-                self._query_props, filter_args)
-
-            resources_name = 'virtual-switches'
-            uri = '{}/{}{}'.format(self.cpc.uri, resources_name, query_parms)
+            resource_obj = self._try_optimized_lookup(filter_args)
+            if resource_obj:
+                resource_obj_list.append(resource_obj)
+                # It already has full properties
+            else:
+                query_parms, client_filters = divide_filter_args(
+                    self._query_props, filter_args)
+
+                resources_name = 'virtual-switches'
+                uri = '{}/{}{}'.format(self.cpc.uri, resources_name,
+                                       query_parms)
+
+                result = self.session.get(uri)
+                if result:
+                    props_list = result[resources_name]
+                    for props in props_list:
+
+                        resource_obj = self.resource_class(
+                            manager=self,
+                            uri=props[self._uri_prop],
+                            name=props.get(self._name_prop, None),
+                            properties=props)
+
+                        if matches_filters(resource_obj, client_filters):
+                            resource_obj_list.append(resource_obj)
+                            if full_properties:
+                                resource_obj.pull_full_properties()
 
-            result = self.session.get(uri)
-            if result:
-                props_list = result[resources_name]
-                for props in props_list:
-
-                    resource_obj = self.resource_class(
-                        manager=self,
-                        uri=props[self._uri_prop],
-                        name=props.get(self._name_prop, None),
-                        properties=props)
-
-                    if matches_filters(resource_obj, client_filters):
-                        resource_obj_list.append(resource_obj)
-                        if full_properties:
-                            resource_obj.pull_full_properties()
+            self.add_resources_local(resource_obj_list)
 
         self._name_uri_cache.update_from(resource_obj_list)
         return resource_obj_list
 
 
 class VirtualSwitch(BaseResource):
     """
```

### Comparing `zhmcclient-1.8.2/zhmcclient/testutils/__init__.py` & `zhmcclient-1.9.0/zhmcclient/testutils/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/testutils/_cpc_fixtures.py` & `zhmcclient-1.9.0/zhmcclient/testutils/_cpc_fixtures.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definition.py` & `zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definition.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definition_fixtures.py` & `zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definition_fixtures.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definitions.py` & `zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definitions.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/testutils/_hmc_inventory_file.py` & `zhmcclient-1.9.0/zhmcclient/testutils/_hmc_inventory_file.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient/testutils/_hmc_vault_file.py` & `zhmcclient-1.9.0/zhmcclient/testutils/_hmc_vault_file.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient.egg-info/PKG-INFO` & `zhmcclient-1.9.0/zhmcclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmcclient
-Version: 1.8.2
+Version: 1.9.0
 Summary: A pure Python client library for the IBM Z HMC Web Services API.
 Home-page: https://github.com/zhmcclient/python-zhmcclient
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmcclient-1.8.2/zhmcclient.egg-info/SOURCES.txt` & `zhmcclient-1.9.0/zhmcclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.rst
 extra-testutils-requirements.txt
 requirements.txt
 setup.py
 zhmcclient/__init__.py
 zhmcclient/_activation_profile.py
 zhmcclient/_adapter.py
+zhmcclient/_auto_updater.py
 zhmcclient/_capacity_group.py
 zhmcclient/_certificates.py
 zhmcclient/_client.py
 zhmcclient/_console.py
 zhmcclient/_constants.py
 zhmcclient/_cpc.py
 zhmcclient/_debug_info.py
@@ -24,15 +25,14 @@
 zhmcclient/_metrics.py
 zhmcclient/_nic.py
 zhmcclient/_notification.py
 zhmcclient/_partition.py
 zhmcclient/_password_rule.py
 zhmcclient/_port.py
 zhmcclient/_resource.py
-zhmcclient/_resource_updater.py
 zhmcclient/_session.py
 zhmcclient/_storage_group.py
 zhmcclient/_storage_group_template.py
 zhmcclient/_storage_volume.py
 zhmcclient/_storage_volume_template.py
 zhmcclient/_task.py
 zhmcclient/_timestats.py
```

### Comparing `zhmcclient-1.8.2/zhmcclient.egg-info/requires.txt` & `zhmcclient-1.9.0/zhmcclient.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient_mock/__init__.py` & `zhmcclient-1.9.0/zhmcclient_mock/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient_mock/_hmc.py` & `zhmcclient-1.9.0/zhmcclient_mock/_hmc.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient_mock/_idpool.py` & `zhmcclient-1.9.0/zhmcclient_mock/_idpool.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient_mock/_session.py` & `zhmcclient-1.9.0/zhmcclient_mock/_session.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.2/zhmcclient_mock/_urihandler.py` & `zhmcclient-1.9.0/zhmcclient_mock/_urihandler.py`

 * *Files identical despite different names*

