# Comparing `tmp/avimigrationtools-22.1.4.tar.gz` & `tmp/avimigrationtools-22.1.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avimigrationtools-22.1.4.tar", last modified: Wed Jun 28 11:00:53 2023, max compression
+gzip compressed data, was "avimigrationtools-22.1.4.post1.tar", last modified: Fri Jul 14 06:11:38 2023, max compression
```

## Comparing `avimigrationtools-22.1.4.tar` & `avimigrationtools-22.1.4.post1.tar`

### file list

```diff
@@ -1,214 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.478458 avimigrationtools-22.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-28 11:00:53.000000 avimigrationtools-22.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-28 11:00:53.478458 avimigrationtools-22.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.458458 avimigrationtools-22.1.4/avi/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.458458 avimigrationtools-22.1.4/avi/migrationtools/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-28 11:00:53.000000 avimigrationtools-22.1.4/avi/migrationtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.462458 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ace_config_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ace_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ace_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    36960 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ace_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ace_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/monitor_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/persistance_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/pool_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ssl_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.462458 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/test/dummy_input.json
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/test/test_input.json
--rw-r--r--   0 runner    (1001) docker     (123)    24891 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ace_converter/vs_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.462458 avimigrationtools-22.1.4/avi/migrationtools/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24991 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ansible/ansible_config_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ansible/ansible_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ansible/ansible_traffic_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/ansible/avi_config_to_ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/avi_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    65224 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/avi_migration_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/avi_orphan_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/avi_rest_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.462458 avimigrationtools-22.1.4/avi/migrationtools/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/common/avi_resource_types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/config_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/custom_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.462458 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/ciphers_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/clone_cross_tenant_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    25572 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/command_status.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   114166 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/conversion_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/converter_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/datagroup_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/f5_config_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    37760 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/f5_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/f5_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/f5_v10_defaults.conf
--rw-r--r--   0 runner    (1001) docker     (123)    14270 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/f5_v11_defaults.conf
--rw-r--r--   0 runner    (1001) docker     (123)    55819 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/monitor_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20583 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/persistence_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    60491 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/policy_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    33192 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/pool_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    97693 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/profile_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/scp_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.466458 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93760 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/avi_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/bigip_v10.conf
--rw-r--r--   0 runner    (1001) docker     (123)    85001 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/bigip_v11.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.466458 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/cakey.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/default.crt
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/default.key
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/monitor.fmr.com.crt
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/monitor.fmr.com.key
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/custom_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/excel_reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    69722 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/hol_advanced_bigip.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/ignore-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/passphrase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_avi_to_ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_config_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_f5_conversion_v10.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_f5_conversion_v11.py
--rw-r--r--   0 runner    (1001) docker     (123)    84361 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_migrationtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_pool_converter.conf
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_pool_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_profile_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_profile_converter.conf
--rw-r--r--   0 runner    (1001) docker     (123)    49578 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_converter/vs_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/f5_discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.466458 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/gss_config_convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/gss_convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/gss_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/gss_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.466458 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/parser_files/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/parser_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/parser_files/gslb_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.466458 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/test/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/test/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.470458 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/command_status.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35467 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/csvs_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/gslb_config_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/gslb_monitor_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/gslb_service_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/gslb_vs_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    40647 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/lbvs_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/monitor_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/netscaler_config_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/netscaler_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/netscaler_gslb_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/netscaler_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/ns_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    51345 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/ns_service_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    88618 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/ns_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/passpharse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    65137 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/policy_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46301 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/profile_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/scp_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/ssl_ciphers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.470458 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.470458 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/certs/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/certs/CD.cert.key
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/certs/ns-server.key
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/certs/test1.key
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/ignore-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/input_vs_configuration.conf
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/netscaler_e2e_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38465 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/ns.conf
--rw-r--r--   0 runner    (1001) docker     (123)    25093 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/ns_passphrase.conf
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/passphrase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    56484 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_complete_vs_configuration.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_complete_vs_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_csv_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    26339 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_migrationtool.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_netscaler_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_upload_output_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.474458 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5537 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/alb_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/base_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4780 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/cleanup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9273 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/command_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    67595 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/conversion_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/converter_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/custom_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/get_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/install_nsx_dependencies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26944 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/monitor_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsx_cleanup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4780 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10528 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_config_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7033 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_rollback.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6110 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_traffic_cutover.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51536 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/persistant_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    60825 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/policy_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25607 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/pools_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13084 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/profile_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7033 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/rollback.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14283 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/ssl_profile_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.474458 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/avi_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    64868 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/default_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    22979 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_migrationtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_monitor_converter.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_monitor_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28399 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_nsxt_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_nsxt_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_pool_converter.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_pool_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_profile_converter.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_profile_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test_cd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6110 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/traffic_cutover.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/v_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    81344 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/vs_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)  1094786 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/pb_attributes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/scp_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.474458 avimigrationtools-22.1.4/avi/migrationtools/test/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.474458 avimigrationtools-22.1.4/avi/migrationtools/test/common/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/test/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/test/common/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/test/common/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/test/common/test_clean_reboot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/test/common/test_tenant_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/test/common/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    48026 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/test/common/test_validation_avi.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.474458 avimigrationtools-22.1.4/avi/migrationtools/v2alb_converter/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/v2alb_converter/discovery_status.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-06-28 10:59:24.000000 avimigrationtools-22.1.4/avi/migrationtools/vs_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:00:53.478458 avimigrationtools-22.1.4/avimigrationtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-28 11:00:53.000000 avimigrationtools-22.1.4/avimigrationtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-28 11:00:53.000000 avimigrationtools-22.1.4/avimigrationtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:00:53.000000 avimigrationtools-22.1.4/avimigrationtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-28 11:00:53.000000 avimigrationtools-22.1.4/avimigrationtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-28 11:00:53.000000 avimigrationtools-22.1.4/avimigrationtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 11:00:53.478458 avimigrationtools-22.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-28 11:00:53.000000 avimigrationtools-22.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.997093 avimigrationtools-22.1.4.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-14 06:11:37.000000 avimigrationtools-22.1.4.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-14 06:11:37.993093 avimigrationtools-22.1.4.post1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.957093 avimigrationtools-22.1.4.post1/avi/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.961093 avimigrationtools-22.1.4.post1/avi/migrationtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-14 06:11:37.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.965093 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ace_config_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ace_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ace_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36960 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ace_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/monitor_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/persistance_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/pool_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ssl_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.965093 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/test/dummy_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/test/test_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24891 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/vs_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.965093 avimigrationtools-22.1.4.post1/avi/migrationtools/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24991 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ansible/ansible_config_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ansible/ansible_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ansible/ansible_traffic_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/ansible/avi_config_to_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/avi_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65224 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/avi_migration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/avi_orphan_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/avi_rest_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.965093 avimigrationtools-22.1.4.post1/avi/migrationtools/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/common/avi_resource_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/config_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/custom_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.969093 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/ciphers_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/clone_cross_tenant_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25572 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/command_status.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   114166 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/conversion_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/converter_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/datagroup_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/f5_config_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37760 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/f5_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/f5_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/f5_v10_defaults.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    14270 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/f5_v11_defaults.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    55819 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/monitor_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20583 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/persistence_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60491 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/policy_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33192 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/pool_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97693 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/profile_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/scp_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.973093 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93760 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/avi_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/bigip_v10.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    85001 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/bigip_v11.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.973093 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/cakey.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/default.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/default.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/monitor.fmr.com.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/monitor.fmr.com.key
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/custom_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/excel_reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    69722 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/hol_advanced_bigip.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/ignore-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/passphrase.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_avi_to_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_config_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_f5_conversion_v10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_f5_conversion_v11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84361 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_migrationtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_pool_converter.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_pool_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_profile_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_profile_converter.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    49578 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/vs_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/f5_discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.977093 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/gss_config_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/gss_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/gss_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/gss_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.977093 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/parser_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/parser_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/parser_files/gslb_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.977093 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/test/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.981093 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/command_status.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35467 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/csvs_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/gslb_config_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/gslb_monitor_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/gslb_service_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/gslb_vs_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40647 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/lbvs_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/monitor_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/netscaler_config_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/netscaler_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/netscaler_gslb_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/netscaler_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/ns_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51345 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/ns_service_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88618 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/ns_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/passpharse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    65137 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/policy_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46301 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/profile_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/scp_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/ssl_ciphers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.981093 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.985093 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/certs/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/certs/CD.cert.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/certs/ns-server.key
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/certs/test1.key
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/ignore-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/input_vs_configuration.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/netscaler_e2e_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38465 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/ns.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    25093 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/ns_passphrase.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/passphrase.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    56484 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_complete_vs_configuration.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_complete_vs_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_csv_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26339 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_migrationtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_netscaler_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_upload_output_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.989093 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5537 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/alb_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/ciphers_dict.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4780 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/cleanup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9273 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/command_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68168 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/conversion_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/converter_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/custom_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/get_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/install_nsx_dependencies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26944 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/monitor_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsx_cleanup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4780 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10523 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_config_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7033 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_rollback.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6110 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_traffic_cutover.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51845 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/persistant_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60825 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/policy_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25880 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/pools_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13084 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/profile_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7033 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/rollback.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15917 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/ssl_profile_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.993093 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/avi_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64868 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/default_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    22979 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_migrationtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_monitor_converter.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_monitor_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28399 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_nsxt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_nsxt_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_pool_converter.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_pool_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_profile_converter.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_profile_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test_cd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6110 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/traffic_cutover.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/v_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81344 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/vs_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1094786 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/pb_attributes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/scp_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.993093 avimigrationtools-22.1.4.post1/avi/migrationtools/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.993093 avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/test_clean_reboot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/test_tenant_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48026 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/test_validation_avi.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.993093 avimigrationtools-22.1.4.post1/avi/migrationtools/v2alb_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/v2alb_converter/discovery_status.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-07-14 06:10:47.000000 avimigrationtools-22.1.4.post1/avi/migrationtools/vs_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:11:37.993093 avimigrationtools-22.1.4.post1/avimigrationtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-14 06:11:37.000000 avimigrationtools-22.1.4.post1/avimigrationtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-07-14 06:11:37.000000 avimigrationtools-22.1.4.post1/avimigrationtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:11:37.000000 avimigrationtools-22.1.4.post1/avimigrationtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-14 06:11:37.000000 avimigrationtools-22.1.4.post1/avimigrationtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-14 06:11:37.000000 avimigrationtools-22.1.4.post1/avimigrationtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:11:37.997093 avimigrationtools-22.1.4.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-14 06:11:37.000000 avimigrationtools-22.1.4.post1/setup.py
```

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ace_config_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ace_config_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ace_constants.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ace_constants.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ace_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ace_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ace_parser.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ace_parser.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ace_utils.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ace_utils.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/monitor_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/monitor_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/persistance_conversion.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/persistance_conversion.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/pool_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/pool_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/ssl_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/ssl_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/test/dummy_input.json` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/test/dummy_input.json`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/test/test_input.json` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/test/test_input.json`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ace_converter/vs_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ace_converter/vs_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ansible/ansible_config_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ansible/ansible_config_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ansible/ansible_constant.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ansible/ansible_constant.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ansible/ansible_traffic_generation.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ansible/ansible_traffic_generation.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/ansible/avi_config_to_ansible.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/ansible/avi_config_to_ansible.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/avi_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/avi_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/avi_migration_utils.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/avi_migration_utils.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/avi_orphan_object.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/avi_orphan_object.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/avi_rest_lib.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/avi_rest_lib.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/common/avi_resource_types.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/common/avi_resource_types.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/config_patch.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/config_patch.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/custom_config.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/custom_config.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/ciphers_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/ciphers_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/clone_cross_tenant_obj.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/clone_cross_tenant_obj.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/command_status.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/command_status.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/config.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/config.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/conversion_util.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/conversion_util.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/converter_constants.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/converter_constants.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/datagroup_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/datagroup_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/f5_config_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/f5_config_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/f5_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/f5_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/f5_parser.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/f5_parser.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/f5_v10_defaults.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/f5_v10_defaults.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/f5_v11_defaults.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/f5_v11_defaults.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/monitor_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/monitor_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/persistence_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/persistence_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/policy_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/policy_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/pool_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/pool_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/profile_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/profile_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/scp_util.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/scp_util.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/avi_config.json` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/avi_config.json`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/bigip_v10.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/bigip_v10.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/bigip_v11.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/bigip_v11.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/cacert.pem` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/cacert.pem`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/cakey.pem` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/cakey.pem`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/default.crt` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/default.crt`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/default.key` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/default.key`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/monitor.fmr.com.crt` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/monitor.fmr.com.crt`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/certs/monitor.fmr.com.key` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/certs/monitor.fmr.com.key`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/conftest.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/conftest.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/custom_config.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/custom_config.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/excel_reader.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/excel_reader.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/hol_advanced_bigip.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/hol_advanced_bigip.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/ignore-config.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/ignore-config.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/patch.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/patch.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_avi_to_ansible.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_avi_to_ansible.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_config_patch.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_config_patch.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_f5_conversion_v10.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_f5_conversion_v10.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_f5_conversion_v11.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_f5_conversion_v11.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_migrationtool.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_migrationtool.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_pool_converter.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_pool_converter.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_pool_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_pool_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_profile_conversion.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_profile_conversion.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/test/test_profile_converter.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/test/test_profile_converter.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_converter/vs_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_converter/vs_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/f5_discovery.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/f5_discovery.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/gss_config_convertor.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/gss_config_convertor.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/gss_convertor.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/gss_convertor.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/gss_parser.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/gss_parser.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/gss_utils.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/gss_utils.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/parser_files/gslb_template.jinja` & `avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/parser_files/gslb_template.jinja`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/gss_convertor/test/test_run.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/gss_convertor/test/test_run.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/command_status.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/command_status.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/csvs_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/csvs_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/gslb_config_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/gslb_config_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/gslb_monitor_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/gslb_monitor_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/gslb_service_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/gslb_service_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/gslb_vs_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/gslb_vs_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/lbvs_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/lbvs_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/monitor_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/monitor_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/netscaler_config_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/netscaler_config_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/netscaler_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/netscaler_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/netscaler_gslb_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/netscaler_gslb_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/netscaler_parser.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/netscaler_parser.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/ns_constants.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/ns_constants.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/ns_service_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/ns_service_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/ns_util.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/ns_util.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/policy_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/policy_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/profile_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/profile_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/scp_util.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/scp_util.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/ssl_ciphers.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/ssl_ciphers.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/certs/ns-server.key` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/certs/ns-server.key`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/ignore-config.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/ignore-config.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/input_vs_configuration.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/input_vs_configuration.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/netscaler_e2e_test.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/netscaler_e2e_test.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/ns.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/ns.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/ns_passphrase.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/ns_passphrase.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_complete_vs_configuration.cfg` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_complete_vs_configuration.cfg`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_complete_vs_configuration.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_complete_vs_configuration.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_csv_status.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_csv_status.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_migrationtool.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_migrationtool.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_netscaler_config.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_netscaler_config.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/netscaler_converter/test/test_upload_output_config.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/netscaler_converter/test/test_upload_output_config.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/__init__.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/alb_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/alb_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/base_client.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/base_client.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/cleanup.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/cleanup.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/command_status.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/command_status.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/conversion_util.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/conversion_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021 VMware, Inc.
 # SPDX-License-Identifier: Apache License 2.0
 
 import copy
 import logging
 import os
 from functools import reduce
-
+import json
 import pandas
 import re
 import random
 from pkg_resources import parse_version
 import avi.migrationtools.f5_converter.converter_constants as conv_const
 
 from xlsxwriter import Workbook
@@ -63,15 +63,16 @@
             'NsxT type': nsxt_type,
             'NsxT SubType': nsxt_sub_type if nsxt_sub_type else ' ',
             'NsxT ID': nsxt_id,
             'Status': conv_status.get('status', ''),
             'Skipped settings': str(conv_status.get('skipped', '')),
             'Indirect mapping': str(conv_status.get('indirect', '')),
             'Not Applicable': str(conv_status.get('na_list', '')),
-            'Avi Object': str(avi_object)
+            'Avi Object': str(avi_object),
+            'Needs Review' : str(need_review)
         }
         csv_writer_dict_list.append(row)
 
     def add_status_row(self, nsxt_type, nsxt_sub_type, nsxt_id, status, avi_obj=None):
         """
         Adds as status row in conversion status csv
         :param nsxt_type: Object type
@@ -185,19 +186,19 @@
         global ptotal_count
         # List of fieldnames for headers
         if vs_level_status:
             fieldnames = ['NsxT type', 'NsxT SubType', 'NsxT ID', 'Status',
                           'Skipped settings', 'Indirect mapping',
                           'Not Applicable', 'Complexity Level',
                           'VS Reference', 'Overall skipped settings',
-                          'Avi Object']
+                          'Avi Object','Needs Review']
         else:
             fieldnames = ['NsxT type', 'NsxT SubType', 'NsxT ID', 'Status',
                           'Skipped settings', 'Indirect mapping',
-                          'Not Applicable', 'Complexity Level', 'Avi Object']
+                          'Not Applicable', 'Complexity Level', 'Avi Object','Needs Review']
 
         # xlsx workbook
         report_path = output_dir + os.path.sep + "%s-ConversionStatus.xlsx" % \
                       report_name
         status_wb = Workbook(report_path)
         # xlsx worksheet
         status_ws = status_wb.add_worksheet("Status Sheet")
@@ -1382,7 +1383,18 @@
         self.remove_dup_key(avi_config["SSLKeyAndCertificate"])
         self.remove_dup_key(avi_config["ApplicationProfile"])
         self.remove_dup_key(avi_config["NetworkProfile"])
         self.remove_dup_key(avi_config["SSLProfile"])
         self.remove_dup_key(avi_config["PKIProfile"])
         self.remove_dup_key(avi_config["ApplicationPersistenceProfile"])
         self.remove_dup_key(avi_config["HealthMonitor"])
+
+    def get_supported_n_unsupported_ciphers_dict(self):
+        cipher_dict_path=os.getcwd()+"/ciphers_dict.json"
+        sup_ciphers=[]
+        unsup_ciphers=[]
+        if os.path.exists(cipher_dict_path):
+            with open(cipher_dict_path) as ci_path:
+                ci_dict=json.load(ci_path)
+                sup_ciphers=ci_dict.get("supported_ciphers_in_nsxt")
+                unsup_ciphers=ci_dict.get("openssl_unsupported_ciphers")
+        return sup_ciphers,unsup_ciphers
```

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/converter_constants.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/converter_constants.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/get_certificates.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/get_certificates.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/install_nsx_dependencies.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/install_nsx_dependencies.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/monitor_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/monitor_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsx_cleanup.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsx_cleanup.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_cleanup.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_cleanup.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_client.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_client.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_config_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_config_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,19 +102,19 @@
    # with open(output_config, "w", encoding='utf-8') as text_file:
        # json.dump(avi_config_dict, text_file, indent=4)
 
     # Add nsxt converter status report in xslx report
     try:
          conv_utils.add_complete_conv_status(
              output_path, avi_config_dict, "nsxt-report", vs_level_status)
-     except Exception as e:
-         msg = "Error in writing excel sheet for converted configuration."
-         LOG.error(msg)
-         print("\033[91m" + msg + " Message: ", str(e) + "\033[0m")
-         sys.exit(1)
+    except Exception as e:
+        msg = "Error in writing excel sheet for converted configuration."
+        LOG.error(msg)
+        print("\033[91m" + msg + " Message: ", str(e) + "\033[0m")
+        sys.exit(1)
 
     for key in avi_config_dict:
         if key != 'META':
             if key == 'VirtualService':
                 if vs_level_status:
                     LOG.info('Total Objects of %s : %s (%s  migrated , %s full conversions)'
                              % (key,len(nsx_lb_config['LbVirtualServers']), len(avi_config_dict[key]),
```

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_rollback.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_rollback.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_traffic_cutover.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_traffic_cutover.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/nsxt_util.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/nsxt_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,18 +121,19 @@
 
 
 def get_object_segments(vs_id, obj_ip):
     vs = vs_details.get(vs_id, None)
     if not vs:
         LOG.debug("virtual service not found with id %s " % vs_id)
         return None
-    cloud = vs.get("cloud")
+    cloud = vs.get("Cloud")
+
     if cloud == "Cloud Not Found":
         LOG.debug("cloud is not configured for vs %s " % vs_id)
-        return None
+       # return None
 
     segments = []
     if vs.get("Segments"):
         seg_list = vs.get("Segments")
         for seg in seg_list:
             seg_name = seg["name"]
             for subnet in seg["subnet"]:
@@ -141,21 +142,22 @@
                 a_network = ipaddress.ip_network(network_range, False)
                 address_in_network = ipaddress.ip_address(obj_ip) in a_network
                 if address_in_network:
                     segments.append( dict(
                         seg_name=seg_name,
                         subnets=subnet))
     else:
-        LOG.debug("segmnets are not configured  for vs %s " % vs_id )
+        LOG.debug("segmnets are not configured  for vs %s with  loadbalancer %s  " % (vs_id , vs.get("lb_name")))
         return None
 
     if segments:
         LOG.debug("segments found for vs %s with attached pool server ip %s are %s" %(vs_id,obj_ip,segments))
         return segments
 
+    LOG.debug("Member ip %s not falling in segment range  %s " % (obj_ip,vs.get("Segments")))
     return None
 
 
 def get_certificate_data(certificate_ref, nsxt_ip, ssh_root_password):
     import paramiko
     import json
 
@@ -538,21 +540,21 @@
                     segments = {
                         "name": segment_id,
                         "subnet": subnets}
                     lb_details.append(segments)
 
             else:
                 segment_list = self.nsx_api_client.infra.Segments.list().to_dict().get('results', [])
-
                 is_tier_linked_segment_found = False
 
                 for seg in segment_list:
                     if seg.get("connectivity_path"):
                         gateway_name = get_name_and_entity(seg["connectivity_path"])[-1]
                         if gateway_name == tier:
+                            is_tier_linked_segment_found=True
                             tz_path = seg.get("transport_zone_path")
                             tz_id = get_name_and_entity(tz_path)[-1]
                             dhcp_present = False
                             for subnet in seg["subnets"]:
                                 if "dhcp_config" in subnet.keys() and not dhcp_present:
                                     dhcp_present = True
                             if not is_cloud_configured:
@@ -578,28 +580,30 @@
                                         "network_range": subnet["network"]
                                     })
                                 segments = {
                                     "name": seg.get("id"),
                                     "subnet": subnets}
                                 lb_details.append(segments)
 
+                if not is_tier_linked_segment_found:
+                    lb_skip_reason = "Skipping because NSX Load Balancer has no segments "\
+                                           "or service interfaces configured"
+                    self.lb_services[lb["id"]] = {
+                         "lb_name": lb["id"],
+                         "lb_skip_reason": lb_skip_reason
+                     }
+                    LOG.debug("Lb skipped : %s reason %s" %(lb["id"],lb_skip_reason))
+                    continue
+
             if not is_cloud_configured:
 
                 warning_mesg="cloud is not configured for load balancer %s with id %s " % (lb["display_name"],lb["id"])
                 LOG.debug(warning_mesg)
-                lb_details=[]
 
 
-                if not is_tier_linked_segment_found:
-                     self.lb_services[lb["id"]] = {
-                         "lb_name": lb["id"],
-                         "lb_skip_reason": "Skipping because NSX Load Balancer has no segments "
-                                           "or service interfaces configured"
-                     }
-                     continue
             self.lb_services[lb["id"]] = {
                 "lb_name": lb["id"],
                 "Network": network,
                 "Cloud": cloud_name,
                 "lb_tier1_lr": lb_tier1_lr
                 }
             if lb_details:
```

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/persistant_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/persistant_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/policy_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/policy_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/pools_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/pools_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -497,24 +497,27 @@
                     server_member['ratio'] = c_member.get('weight')
 
     def check_pool_member_ip_ranges(self, vs_list, pool_count, lb_list, pool_members_list, pool_skip, pool_name,
                                     pool_segment_list):
         is_member_ip_in_range=False
         for member in pool_members_list:
             for vs_id in vs_list:
+                LOG.debug("Checking pool member ip  %s falling in range or not  , pool %s attached with vip %s " % (member.get("ip_address"),
+                                                                                                                pool_name,vs_id))
                 if vs_id in pool_segment_list.keys():
                     pool_skip = False
                     is_member_ip_in_range=True
                     continue
                 lb = get_lb_service_name(vs_id)
                 if not lb:
                     LOG.debug("lb not configured for vs %s" % vs_id)
                     continue
                 pool_segment = get_object_segments(vs_id,
                                                    member.get("ip_address"))
+
                 if pool_segment:
                     pool_skip = False
                     is_member_ip_in_range = True
                     if lb in lb_list.keys():
                         pool_segment_list[vs_id] = lb_list.get(lb)
                         continue
```

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/profile_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/profile_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/rollback.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/rollback.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/ssl_profile_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/ssl_profile_converter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Copyright 2021 VMware, Inc.
 # SPDX-License-Identifier: Apache License 2.0
 
 import logging
 import os
-
+import json
 from avi.migrationtools.avi_migration_utils import update_count, MigrationUtil
 from avi.migrationtools.nsxt_converter.conversion_util import NsxtConvUtil
 import avi.migrationtools.nsxt_converter.converter_constants as final
 import avi.migrationtools.nsxt_converter.converter_constants as conv_const
 
+
+
 LOG = logging.getLogger(__name__)
 
 conv_utils = NsxtConvUtil()
 common_avi_util = MigrationUtil()
 ssl_profile_list = {}
 
 
@@ -27,14 +29,15 @@
         self.indirect_client_ssl_attr = nsxt_profile_attributes["SSLProfile_Client_Indirect_Attributes"]
         self.indirect_server_ssl_attr = nsxt_profile_attributes["SSLProfile_Server_Indirect_Attributes"]
         self.ssl_na_attr=nsxt_profile_attributes["SSLProfile_NA_Attributes"]
         self.object_merge_check = object_merge_check
         self.merge_object_mapping = merge_object_mapping
         self.sys_dict = sys_dict
         self.ssl_profile_count = 0
+        self.sup_ciphers,self.unsup_ciphers=conv_utils.get_supported_n_unsupported_ciphers_dict()
 
     def convert(self, alb_config, nsx_lb_config, prefix, tenant):
         alb_config["SSLProfile"] = []
         tenant_name, name = conv_utils.get_tenant_ref(tenant)
         if not tenant:
             tenant = tenant_name
         if nsx_lb_config.get('LbClientSslProfiles'):
@@ -73,15 +76,15 @@
                     ssl_profile_list[lb_ssl['id']] = name
                     if lb_ssl.get("session_cache_enabled"):
                         alb_ssl['enable_ssl_session_reuse'] = lb_ssl['session_cache_enabled']
                     if lb_ssl.get("session_cache_timeout"):
                         alb_ssl['ssl_session_timeout'] = lb_ssl['session_cache_timeout']
 
                     if lb_ssl.get("ciphers"):
-                        converted_ciphers = self.convert_ciphers_to_valid_format(":".join(lb_ssl['ciphers']))
+                        converted_ciphers,unsup_cipher_from_cipher_str = self.convert_ciphers(":".join(lb_ssl['ciphers']))
                         alb_ssl['accepted_ciphers'] = converted_ciphers
 
                     if lb_ssl.get("protocols"):
                         self.convert_protocols(lb_ssl['protocols'], alb_ssl)
                     if lb_ssl.get("prefer_server_ciphers"):
                         alb_ssl["prefer_client_cipher_ordering"] = not lb_ssl["prefer_server_ciphers"]
 
@@ -99,17 +102,19 @@
                     else:
                         alb_config['SSLProfile'].append(alb_ssl)
 
                     val = dict(
                         id=lb_ssl["id"],
                         name=name,
                         resource_type=lb_ssl['resource_type'],
-                        alb_ssl=alb_ssl
+                        alb_ssl=alb_ssl,
+                        unsup_cipher=unsup_cipher_from_cipher_str
 
                     )
+
                     converted_alb_ssl.append(val)
 
                     msg = "SSLProfile conversion started..."
                     conv_utils.print_progress_bar(progressbar_count, total_size, msg,
                                                   prefix='Progress', suffix='')
 
                     LOG.info('[SSL-PROFILE] Migration completed for HM {}'.format(lb_ssl['display_name']))
@@ -129,22 +134,27 @@
                     u_ignore, na_list[index])
                 ssl_na = [val for val in na_list[index] if val not in self.common_na_attr]
                 conv_status["na_list"] = ssl_na
                 name = converted_alb_ssl[index]['name']
                 ssl_id = converted_alb_ssl[index]['id']
                 alb_mig_ssl = converted_alb_ssl[index]['alb_ssl']
                 resource_type = converted_alb_ssl[index]['resource_type']
+                unsup_ciphers=converted_alb_ssl[index]["unsup_cipher"]
+                if conv_status["status"]=="SUCCESSFUL" and unsup_ciphers:
+                    conv_status["status"]="SUCCESSFUL WITH UNSUPPORTED CIPHERS"
+                if unsup_ciphers:
+                    unsup_ciphers={'Unsupported ciphers':unsup_ciphers}
                 if self.object_merge_check:
                     alb_mig_ssl = [pp for pp in alb_config['SSLProfile'] if
                                    pp.get('name') == self.merge_object_mapping['ssl_profile'].get(name)]
                     conv_utils.add_conv_status('sslprofile', resource_type, name, conv_status,
-                                               [{'ssl_profile': alb_mig_ssl[0]}])
+                                               [{'ssl_profile': alb_mig_ssl[0]}],unsup_ciphers)
                 else:
                     conv_utils.add_conv_status('sslprofile', resource_type, name, conv_status,
-                                               [{'ssl_profile': alb_mig_ssl}])
+                                               [{'ssl_profile': alb_mig_ssl}],unsup_ciphers)
                 if len(conv_status['skipped']) > 0:
                     LOG.debug(
                         '[SSL-PROFILE] Skipped Attribute {}:{}'.format(name,
                                                                        conv_status['skipped']))
 
         if nsx_lb_config.get('LbServerSslProfiles'):
             converted_objs = []
@@ -177,15 +187,15 @@
                             name = '%s-%s' % (name, lb_ssl["id"])
                     alb_ssl = dict(
                         name=name,
                         tenant_ref=conv_utils.get_object_ref(tenant, 'tenant'),
                     )
                     ssl_profile_list[lb_ssl['id']] = name
                     if lb_ssl.get("ciphers"):
-                        converted_ciphers = self.convert_ciphers_to_valid_format(":".join(lb_ssl['ciphers']))
+                        converted_ciphers,unsup_cipher_from_cipher_str = self.convert_ciphers(":".join(lb_ssl['ciphers']))
                         alb_ssl['accepted_ciphers'] = converted_ciphers
 
                     if lb_ssl.get("protocols"):
                         self.convert_protocols(lb_ssl['protocols'], alb_ssl)
 
                     skipped_list.append(skipped)
                     ##
@@ -201,17 +211,19 @@
                     else:
                         alb_config['SSLProfile'].append(alb_ssl)
 
                     val = dict(
                         id=lb_ssl["id"],
                         name=name,
                         resource_type=lb_ssl['resource_type'],
-                        alb_ssl=alb_ssl
+                        alb_ssl=alb_ssl,
+                        unsup_cipher=unsup_cipher_from_cipher_str
 
                     )
+
                     converted_alb_ssl.append(val)
 
                     msg = "SSLProfile conversion started..."
                     conv_utils.print_progress_bar(progressbar_count, total_size, msg,
                                                   prefix='Progress', suffix='')
 
                     LOG.info('[SSL-PROFILE] Migration completed for HM {}'.format(lb_ssl['display_name']))
@@ -231,22 +243,27 @@
                     u_ignore, na_list[index])
                 ssl_na = [val for val in na_list[index] if val not in self.common_na_attr]
                 conv_status["na_list"] = ssl_na
                 name = converted_alb_ssl[index]['name']
                 ssl_id = converted_alb_ssl[index]['id']
                 alb_mig_ssl = converted_alb_ssl[index]['alb_ssl']
                 resource_type = converted_alb_ssl[index]['resource_type']
+                unsup_ciphers=converted_alb_ssl[index]["unsup_cipher"]
+                if conv_status["status"]=="SUCCESSFUL" and unsup_ciphers:
+                    conv_status["status"]="SUCCESSFUL WITH UNSUPPORTED CIPHERS"
+                if unsup_ciphers:
+                    unsup_ciphers={'Unsupported ciphers':unsup_ciphers}
                 if self.object_merge_check:
                     alb_mig_ssl = [pp for pp in alb_config['SSLProfile'] if
                                    pp.get('name') == self.merge_object_mapping['ssl_profile'].get(name)]
                     conv_utils.add_conv_status('sslprofile', resource_type, name, conv_status,
-                                               [{'ssl_profile': alb_mig_ssl[0]}])
+                                               [{'ssl_profile': alb_mig_ssl[0]}],unsup_ciphers)
                 else:
                     conv_utils.add_conv_status('sslprofile', resource_type, name, conv_status,
-                                               [{'ssl_profile': alb_mig_ssl}])
+                                               [{'ssl_profile': alb_mig_ssl}],unsup_ciphers)
                 if len(conv_status['skipped']) > 0:
                     LOG.debug(
                         '[SSL-PROFILE] Skipped Attribute {}:{}'.format(name,
                                                                        conv_status['skipped']))
 
     def convert_protocols(self, protocols, alb_ssl):
         accepted_version = dict(
@@ -261,13 +278,24 @@
 
         for acc_ver in protocols:
             acc_version = dict(
                 type=accepted_version[acc_ver]
             )
             alb_ssl['accepted_versions'].append(acc_version)
 
-    def convert_ciphers_to_valid_format(self, cipher_str):
+    def convert_ciphers(self, cipher_str):
+        '''
+        This method will remove all the unsupported ciphers from cipher string
+        e.g cipher_str := TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256:TLS_ECDHE_ECDSA_WITH_AES_128_CBC_SHA256:TLS_ECDHE_ECDSA_WITH_AES_256_GCM_SHA384
+        '''
+        cipher_str = cipher_str.replace('TLS_RSA_', '')
         cipher_str = cipher_str.replace('TLS_', '')
+        cipher_str=cipher_str.replace('CBC_','')
         cipher_str = cipher_str.replace('_', '-')
         cipher_str = cipher_str.replace('WITH-AES-128', 'AES128')
         cipher_str = cipher_str.replace('WITH-AES-256', 'AES256')
-        return cipher_str
+        unsup_cipher_from_cipher_str=[cipher for cipher in cipher_str.split(":") if cipher in  self.unsup_ciphers]
+        sup_cipher= [cipher for cipher in cipher_str.split(":") if cipher not in unsup_cipher_from_cipher_str]
+        sup_cipher_str=":".join(sup_cipher)
+        return sup_cipher_str,unsup_cipher_from_cipher_str
+
+
```

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/avi_config.json` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/avi_config.json`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/config.json` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/config.json`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/excel_reader.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/excel_reader.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_migrationtool.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_migrationtool.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_monitor_converter.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_monitor_converter.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_monitor_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_monitor_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_nsxt_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_nsxt_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_nsxt_functional.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_nsxt_functional.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_pool_converter.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_pool_converter.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_pool_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_pool_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_profile_converter.conf` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_profile_converter.conf`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/test/test_profile_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/test/test_profile_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/traffic_cutover.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/traffic_cutover.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/v_client.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/v_client.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/nsxt_converter/vs_converter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/nsxt_converter/vs_converter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/pb_attributes.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/pb_attributes.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/scp_util.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/scp_util.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/setup.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/setup.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/test/common/config.yaml` & `avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/config.yaml`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/test/common/excel_reader.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/excel_reader.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/test/common/test_clean_reboot.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/test_clean_reboot.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/test/common/test_tenant_cloud.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/test_tenant_cloud.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/test/common/test_validation.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/test_validation.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/test/common/test_validation_avi.json` & `avimigrationtools-22.1.4.post1/avi/migrationtools/test/common/test_validation_avi.json`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avi/migrationtools/vs_filter.py` & `avimigrationtools-22.1.4.post1/avi/migrationtools/vs_filter.py`

 * *Files identical despite different names*

### Comparing `avimigrationtools-22.1.4/avimigrationtools.egg-info/SOURCES.txt` & `avimigrationtools-22.1.4.post1/avimigrationtools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 avi/migrationtools/netscaler_converter/test/test_upload_output_config.py
 avi/migrationtools/netscaler_converter/test/certs/CD.cert.key
 avi/migrationtools/netscaler_converter/test/certs/ns-server.key
 avi/migrationtools/netscaler_converter/test/certs/test1.key
 avi/migrationtools/nsxt_converter/__init__.py
 avi/migrationtools/nsxt_converter/alb_converter.py
 avi/migrationtools/nsxt_converter/base_client.py
+avi/migrationtools/nsxt_converter/ciphers_dict.json
 avi/migrationtools/nsxt_converter/cleanup.py
 avi/migrationtools/nsxt_converter/command_status.yaml
 avi/migrationtools/nsxt_converter/conversion_util.py
 avi/migrationtools/nsxt_converter/converter_constants.py
 avi/migrationtools/nsxt_converter/custom_config.yaml
 avi/migrationtools/nsxt_converter/get_certificates.py
 avi/migrationtools/nsxt_converter/install_nsx_dependencies.py
```

### Comparing `avimigrationtools-22.1.4/setup.py` & `avimigrationtools-22.1.4.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2021 VMware, Inc.
 # SPDX-License-Identifier: Apache License 2.0
 
 import os
 from setuptools import setup, find_packages
 
-AVI_PIP_VERSION = '22.1.4'
+AVI_PIP_VERSION = '22.1.4.post1'
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='avimigrationtools',
     version=AVI_PIP_VERSION,
```

