# Comparing `tmp/crowdstrike-falconpy-dev-1.3.0.dev1.tar.gz` & `tmp/crowdstrike-falconpy-dev-1.3.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdstrike-falconpy-dev-1.3.0.dev1.tar", last modified: Tue Feb  7 05:49:30 2023, max compression
+gzip compressed data, was "crowdstrike-falconpy-dev-1.3.0.dev6.tar", last modified: Fri Jul 14 05:22:15 2023, max compression
```

## Comparing `crowdstrike-falconpy-dev-1.3.0.dev1.tar` & `crowdstrike-falconpy-dev-1.3.0.dev6.tar`

### file list

```diff
@@ -1,215 +1,220 @@
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.261430 crowdstrike-falconpy-dev-1.3.0.dev1/
--rw-r--r--   0 jhiller    (501) staff       (20)     4830 2023-02-07 05:49:28.000000 crowdstrike-falconpy-dev-1.3.0.dev1/AUTHORS.md
--rw-r--r--   0 jhiller    (501) staff       (20)     1211 2023-02-07 05:49:28.000000 crowdstrike-falconpy-dev-1.3.0.dev1/LICENSE
--rw-r--r--   0 jhiller    (501) staff       (20)    33335 2023-02-07 05:49:30.261139 crowdstrike-falconpy-dev-1.3.0.dev1/PKG-INFO
--rw-r--r--   0 jhiller    (501) staff       (20)    30050 2023-02-07 05:49:28.000000 crowdstrike-falconpy-dev-1.3.0.dev1/README.md
--rw-r--r--   0 jhiller    (501) staff       (20)     7201 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/dev_setup.py
--rw-r--r--   0 jhiller    (501) staff       (20)       38 2023-02-07 05:49:30.261506 crowdstrike-falconpy-dev-1.3.0.dev1/setup.cfg
--rw-r--r--   0 jhiller    (501) staff       (20)     4482 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/setup.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.159634 crowdstrike-falconpy-dev-1.3.0.dev1/src/
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.178715 crowdstrike-falconpy-dev-1.3.0.dev1/src/crowdstrike_falconpy_dev.egg-info/
--rw-r--r--   0 jhiller    (501) staff       (20)    33335 2023-02-07 05:49:30.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO
--rw-r--r--   0 jhiller    (501) staff       (20)     8001 2023-02-07 05:49:30.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt
--rw-r--r--   0 jhiller    (501) staff       (20)        1 2023-02-07 05:49:30.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/crowdstrike_falconpy_dev.egg-info/dependency_links.txt
--rw-r--r--   0 jhiller    (501) staff       (20)       83 2023-02-07 05:49:30.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/crowdstrike_falconpy_dev.egg-info/requires.txt
--rw-r--r--   0 jhiller    (501) staff       (20)       12 2023-02-07 05:49:30.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/crowdstrike_falconpy_dev.egg-info/top_level.txt
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.209379 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/
--rw-r--r--   0 jhiller    (501) staff       (20)    11969 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/__init__.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.211510 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/
--rw-r--r--   0 jhiller    (501) staff       (20)     2095 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11250 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5561 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request_behavior.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5022 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request_connection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3788 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request_meta.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5358 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request_payloads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3827 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request_validator.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.214269 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/
--rw-r--r--   0 jhiller    (501) staff       (20)     2047 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4234 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/_base_falcon_auth.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5998 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/_bearer_token.py
--rw-r--r--   0 jhiller    (501) staff       (20)    19770 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/_falcon_interface.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4806 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/_interface_config.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8624 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/_uber_interface.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.214778 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_constant/
--rw-r--r--   0 jhiller    (501) staff       (20)     2856 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_constant/__init__.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.233242 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/
--rw-r--r--   0 jhiller    (501) staff       (20)     8737 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7042 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6876 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)    24875 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13488 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11664 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6446 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10608 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_device_control_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10099 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3167 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_event_streams.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12391 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_falcon_complete_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3662 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_falcon_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12780 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_falconx_sandbox.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3694 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    23292 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10008 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_firewall_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9015 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10176 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6722 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6237 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    22179 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_intel.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4594 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_ioa_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11562 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13556 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10743 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_kubernetes_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5803 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6806 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4457 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_ml_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2377 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_mobile_enrollment.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17802 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3435 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_oauth2.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12680 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3569 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_overwatch_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9960 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_prevention_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4808 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_quarantine.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4165 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_quick_scan.py
--rw-r--r--   0 jhiller    (501) staff       (20)    24729 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16057 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17745 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9918 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_response_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11813 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5275 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_sensor_download.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15516 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_sensor_update_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4678 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4667 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7134 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4885 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_tailored_intelligence.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15659 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_user_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2516 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_zero_trust_assessment.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.237502 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/
--rw-r--r--   0 jhiller    (501) staff       (20)     4289 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13207 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10099 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17702 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3316 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5947 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11312 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2177 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12911 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13678 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13342 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.238601 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_enum/
--rw-r--r--   0 jhiller    (501) staff       (20)     1871 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_enum/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2124 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_enum/_base_url.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2063 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_enum/_container_base_url.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2218 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_enum/_token_fail_reason.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.239388 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_error/
--rw-r--r--   0 jhiller    (501) staff       (20)     2561 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_error/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5684 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_error/_exceptions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3573 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_error/_warnings.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.239920 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_log/
--rw-r--r--   0 jhiller    (501) staff       (20)     1744 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_log/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3809 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_log/_facility.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.256021 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/
--rw-r--r--   0 jhiller    (501) staff       (20)     5400 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2691 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3624 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2574 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4858 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3563 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2621 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5478 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_device_control_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3666 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_falconx.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16024 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_firewall.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8462 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_generic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4290 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4511 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5480 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7302 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5577 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3737 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2866 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4426 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3118 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_prevention_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4309 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7727 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2615 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_response_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2433 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3408 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_sensor_update_policy.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.258812 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/
--rw-r--r--   0 jhiller    (501) staff       (20)     4540 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/__base_resource.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2186 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4581 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_base_dictionary.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1825 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_errors.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2684 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_expanded_result.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_headers.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3298 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_meta.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2489 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_resources.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4340 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_response_component.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15675 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_result.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.259621 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_service_class/
--rw-r--r--   0 jhiller    (501) staff       (20)     1827 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_service_class/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12272 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_service_class/_base_service_class.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11024 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_service_class/_service_class.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-02-07 05:49:30.260729 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_util/
--rw-r--r--   0 jhiller    (501) staff       (20)     3087 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_util/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2997 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_util/_auth.py
--rw-r--r--   0 jhiller    (501) staff       (20)    33605 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_util/_functions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6161 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_util/_uber.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2120 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_version.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16709 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9970 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/api_complete.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15947 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)    39693 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    34208 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)    22911 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10750 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/debug.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14793 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)    27402 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/device_control_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17344 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5973 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/event_streams.py
--rw-r--r--   0 jhiller    (501) staff       (20)    35245 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/falcon_complete_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8670 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/falcon_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)    24004 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/falconx_sandbox.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5384 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    77667 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20232 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/firewall_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    18869 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)    27363 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4578 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13308 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13613 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    34693 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/intel.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10663 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/ioa_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    34704 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14032 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    19435 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/kubernetes_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16359 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)    21223 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10052 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/ml_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5166 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/mobile_enrollment.py
--rw-r--r--   0 jhiller    (501) staff       (20)    43246 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8811 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/oauth2.py
--rw-r--r--   0 jhiller    (501) staff       (20)    30233 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13167 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/overwatch_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20718 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/prevention_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13733 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/quarantine.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9493 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/quick_scan.py
--rw-r--r--   0 jhiller    (501) staff       (20)    42802 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    25250 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)    43186 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7687 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    19891 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/response_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    21891 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6764 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10169 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/sensor_download.py
--rw-r--r--   0 jhiller    (501) staff       (20)    35068 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/sensor_update_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9899 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/sensor_visibility_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8333 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/spotlight_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10651 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/spotlight_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9791 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/tailored_intelligence.py
--rw-r--r--   0 jhiller    (501) staff       (20)    38570 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/user_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4789 2023-02-07 05:49:29.000000 crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.137681 crowdstrike-falconpy-dev-1.3.0.dev6/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4906 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/AUTHORS.md
+-rw-r--r--   0 jhiller    (501) staff       (20)     1211 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/LICENSE
+-rw-r--r--   0 jhiller    (501) staff       (20)    32848 2023-07-14 05:22:15.137284 crowdstrike-falconpy-dev-1.3.0.dev6/PKG-INFO
+-rw-r--r--   0 jhiller    (501) staff       (20)    29563 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/README.md
+-rw-r--r--   0 jhiller    (501) staff       (20)     7201 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/dev_setup.py
+-rw-r--r--   0 jhiller    (501) staff       (20)       38 2023-07-14 05:22:15.137788 crowdstrike-falconpy-dev-1.3.0.dev6/setup.cfg
+-rw-r--r--   0 jhiller    (501) staff       (20)     4482 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/setup.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:14.984349 crowdstrike-falconpy-dev-1.3.0.dev6/src/
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.006690 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/
+-rw-r--r--   0 jhiller    (501) staff       (20)    32848 2023-07-14 05:22:14.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO
+-rw-r--r--   0 jhiller    (501) staff       (20)     8224 2023-07-14 05:22:14.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)        1 2023-07-14 05:22:14.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)       83 2023-07-14 05:22:14.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/requires.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)       12 2023-07-14 05:22:14.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/top_level.txt
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.055696 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/
+-rw-r--r--   0 jhiller    (501) staff       (20)    12107 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/__init__.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.060221 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2095 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11250 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5561 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_behavior.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5022 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_connection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3788 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_meta.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5358 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_payloads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3827 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_validator.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.064561 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2047 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4234 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_base_falcon_auth.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5998 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_bearer_token.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20647 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_falcon_interface.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4806 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_interface_config.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8624 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_uber_interface.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.065133 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_constant/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2905 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_constant/__init__.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.098407 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/
+-rw-r--r--   0 jhiller    (501) staff       (20)     9054 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7042 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6740 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    30329 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13488 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15447 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6446 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10667 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_device_control_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3167 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_event_streams.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12391 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_falcon_complete_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6172 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_falcon_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14991 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_falconx_sandbox.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3694 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23292 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10008 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_firewall_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9015 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10381 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8008 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6237 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    22179 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_intel.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4594 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ioa_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11784 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13556 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15790 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_kubernetes_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5803 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7033 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4457 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ml_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2377 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_mobile_enrollment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20286 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3611 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_oauth2.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12950 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3569 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_overwatch_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9960 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_prevention_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4808 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_quarantine.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4165 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_quick_scan.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    24729 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16057 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17960 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9918 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_response_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11674 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5275 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_download.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15927 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_update_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4678 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4667 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7134 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4885 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_tailored_intelligence.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16463 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_user_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6050 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.110378 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4611 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13207 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5506 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17702 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3316 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5947 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11312 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2177 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13181 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13678 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13342 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1945 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.113080 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1871 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2124 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_base_url.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2063 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_container_base_url.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2218 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_token_fail_reason.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.114843 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2662 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6071 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/_exceptions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3573 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/_warnings.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.116038 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_log/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1744 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_log/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3809 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_log/_facility.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.128681 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/
+-rw-r--r--   0 jhiller    (501) staff       (20)     5516 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2691 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3624 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5855 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6079 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4604 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2790 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6181 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_device_control_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3666 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_falconx.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16333 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_firewall.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7329 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_generic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4290 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4511 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5808 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7508 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5577 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3774 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2866 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4506 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3118 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_prevention_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4309 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8001 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2615 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_response_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2433 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4519 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_sensor_update_policy.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.133404 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4540 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/__base_resource.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2186 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4581 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_base_dictionary.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1825 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_errors.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2684 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_expanded_result.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_headers.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3298 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_meta.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2489 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_resources.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4561 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_response_component.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16548 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_result.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.134688 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1827 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12272 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/_base_service_class.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11426 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/_service_class.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.136617 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/
+-rw-r--r--   0 jhiller    (501) staff       (20)     3087 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3076 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_auth.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    33929 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_functions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6161 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_uber.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3539 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_version.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17508 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9970 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/api_complete.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15947 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    48601 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    34208 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    27069 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10750 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/debug.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15759 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    29552 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/device_control_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    22218 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5973 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/event_streams.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    37615 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/falcon_complete_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16270 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/falcon_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    28300 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/falconx_sandbox.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8668 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5384 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    79369 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20174 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/firewall_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    18869 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    27450 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4578 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13758 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13613 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    34693 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/intel.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10663 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ioa_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    35840 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14032 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    25074 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/kubernetes_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16367 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23565 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10056 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ml_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5166 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/mobile_enrollment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    43338 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8919 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/oauth2.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    35443 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13881 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/overwatch_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20718 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/prevention_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14372 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/quarantine.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9493 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/quick_scan.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    43159 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    25250 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    45859 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7687 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    19891 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/response_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    21891 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6764 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10169 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_download.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    38364 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_update_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9899 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_visibility_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8333 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/spotlight_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10652 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/spotlight_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9791 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/tailored_intelligence.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    39321 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/user_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8311 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/zero_trust_assessment.py
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/AUTHORS.md` & `crowdstrike-falconpy-dev-1.3.0.dev6/AUTHORS.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # FalconPy Project Authors
 The FalconPy project exists to enable developer interactions with the CrowdStrike Falcon API. Designed to be easy to integrate and use within your Python projects, the library is released under the [Unlicense](LICENSE) license. Developed and maintained by a diverse group of security architects, engineers and specialists, FalconPy has received multiple contributions from the community at large.
 
 | Name | |
 | :--- | :--- |
 | Joshua Hiller, `@jshcodes` | [Lord of the FalconPys](https://xkcd.com/1604/) [:fly:](https://xkcd.com/1856/) |
 | Dixon Styres, `@crowdstrikedcs` | [Author](https://xkcd.com/1646/) |
+| Timothy Sullivan, `@tsullivan06` | [Author](https://xkcd.com/1349/) |
 | Devin Cargill, `@dcargs` | [Author](https://xkcd.com/722/) |
 
 <BR/>
 
 [![Maintainers](https://img.shields.io/badge/-Maintainers-lightgreen?style=for-the-badge)](#maintainers)
 [![Contributors](https://img.shields.io/badge/-Contributors-tan?style=for-the-badge)](#contributors)
 [![Sponsors](https://img.shields.io/badge/-Sponsors-silver?style=for-the-badge)](#sponsors)
@@ -29,16 +30,15 @@
 | Šimon L., `@isimluk` | [Sanity Checker](https://xkcd.com/1926/) |
 | Josh Lang, `@jlangdev` | [Lint Purveyor](https://xkcd.com/1833/) |
 | Christopher Hammond, `@ChristopherHammond13` | [Technical Debt Collector](https://xkcd.com/2138/) |
 | Gabe Alford, `@redhatrises` | [Git Whisperer](https://xkcd.com/1597/) |
 | Brendan Kremian, `@bk-cs` | [Disparate Ringbearer](https://xkcd.com/353/)
 | Christophe Viaud, `@falcon-pioupiou` | [Consequence Substantiator](https://xkcd.com/1678/) |
 | Shane Shellenbarger, `@soggysec` | [Calamity Validator](https://xkcd.com/1700/) |
-| Timothy Sullivan, `@tsullivan06` | [Functionality Determinator](https://xkcd.com/1349/) |
-| Steve Klassen, `@mrxinu` | [Dilemma Respondent](https://xkcd.com/85/) |
+| Steve Klassen, `@mrxinu` | [Dilemma Responder](https://xkcd.com/85/) |
 
 ## Contributors
 The following members of the community have made requests, suggestions, code contributions or provided feedback and reported bugs.
 This has been a critical element in the development of the FalconPy project.
 
 ![GitHub contributors](https://img.shields.io/github/contributors/CrowdStrike/falconpy?label=code%20contributors&style=for-the-badge)
 
@@ -72,21 +72,25 @@
 + Hod Alpert, `@hod-alpert`
 + `@mwilco03`
 + Glenn, `@hiddenillusion`
 + Taylor Trueblood, `@Trueblood506`
 + `@mtobias-getty`
 + `@WDmoose` 
 + Arifur, `@arahman63`
-+ `@areino`
++ Alfredo Reino, `@areino`
 + `@kmccb`
 + Carlos Matos, `@carlosmmatos`
 + `@ffalor`
 + `@jmillerca`
 + `@davidt99`
 + `@CommonVulnerability`
++ `@Odie71`
++ Chris, `@chrisbvt`
++ Alex, `@khyberspache`
++ Phil Massyn, `@massyn`
 
 
 ## Sponsors
 Without the support of these executives, the FalconPy project would not have happened.
 
 | Name | Role |
 | :-- | :-- |
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/LICENSE` & `crowdstrike-falconpy-dev-1.3.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/PKG-INFO` & `crowdstrike-falconpy-dev-1.3.0.dev6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy-dev
-Version: 1.3.0.dev1
+Version: 1.3.0.dev6
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
@@ -156,15 +156,15 @@
 | Real Time Response (RTR) Policies | [response_policies.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/response_policies.py) | [ResponsePolicies](https://www.falconpy.io/Service-Collections/Response-Policies.html) |
 | Report Executions | [report_executions.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/report_executions.py) | [ReportExecutions](https://www.falconpy.io/Service-Collections/Report-Executions.html) |
 | Scheduled Reports | [scheduled_reports.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/scheduled_reports.py) | [ScheduledReports](https://www.falconpy.io/Service-Collections/Scheduled-Reports.html) |
 | Sensor Download | [sensor_download.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sensor_download.py) | [SensorDownload](https://www.falconpy.io/Service-Collections/Sensor-Download.html) |
 | Sensor Visibility Exclusions | [sensor_visibility_exclusions.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sensor_visibility_exclusions.py) | [SensorVisibilityExclusions](https://www.falconpy.io/Service-Collections/Sensor-Visibility-Exclusions.html) |
 | Sensor Update Policy Management | [sensor_update_policy.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sensor_update_policy.py) | [SensorUpdatePolicy](https://www.falconpy.io/Service-Collections/Sensor-Update-Policy.html) |
 | Spotlight | [spotlight_evaluation_logic.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/spotlight_evaluation_logic.py)<BR/>[spotlight_vulnerabilities.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/spotlight_vulnerabilities.py) | [SpotlightEvaluationLogic](https://www.falconpy.io/Service-Collections/Spotlight-Evaluation-Logic.html)<BR/>[SpotlightVulnerabilities](https://www.falconpy.io/Service-Collections/Spotlight-Vulnerabilities.html) |
-| Falcon Intelligence | [falconx_sandbox.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/falconx_sandbox.py)<BR/>[intel.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/intel.py)<br/>[ioc.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/ioc.py) <BR/> [iocs.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/iocs.py) *Deprecated*<BR/>[malquery.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/malquery.py)<BR/>[quick_scan.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/quick_scan.py)<BR/>[recon.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/recon.py)<BR/>[sample_uploads.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sample_uploads.py)| [FalconXSandbox](https://www.falconpy.io/Service-Collections/Falconx-Sandbox.html)<BR/>[Intel](https://www.falconpy.io/Service-Collections/Intel.html)<BR/>[IOC](https://www.falconpy.io/Service-Collections/IOC.html)<BR/>[Iocs](https://www.falconpy.io/Service-Collections/IOCs.html)<BR/>[MalQuery](https://www.falconpy.io/Service-Collections/MalQuery.html)<BR/>[QuickScan](https://www.falconpy.io/Service-Collections/Quick-Scan.html)<BR/><a href="https://www.falconpy.io/Service-Collections/Recon.html" target="_blank">Recon</a><BR/>[SampleUploads](https://www.falconpy.io/Service-Collections/Sample-Uploads.html) |
+| __Falcon Intelligence__<BR/>Intel<BR/>IOC<BR/>IOCS<BR/>MalQuery<BR/>ODS (On Demand Scan)<BR/>Quick Scan<BR/>Recon<BR/>Sample Uploads<BR/>Sandbox | <BR/>[intel.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/intel.py)<br/>[ioc.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/ioc.py) <BR/> [iocs.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/iocs.py) *Deprecated*<BR/>[malquery.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/malquery.py)<BR/>[ods.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/ods.py)<BR/>[quick_scan.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/quick_scan.py)<BR/>[recon.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/recon.py)<BR/>[sample_uploads.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sample_uploads.py) <BR/> [falconx_sandbox.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/falconx_sandbox.py)| <BR/>[Intel](https://www.falconpy.io/Service-Collections/Intel.html)<BR/>[IOC](https://www.falconpy.io/Service-Collections/IOC.html)<BR/>[Iocs](https://www.falconpy.io/Service-Collections/IOCs.html)<BR/>[MalQuery](https://www.falconpy.io/Service-Collections/MalQuery.html)<BR/>[ODS](https://www.falconpy.io/Service-Collections/ODS.html)<BR/>[QuickScan](https://www.falconpy.io/Service-Collections/Quick-Scan.html)<BR/><a href="https://www.falconpy.io/Service-Collections/Recon.html" target="_blank">Recon</a><BR/>[SampleUploads](https://www.falconpy.io/Service-Collections/Sample-Uploads.html)<BR/>[FalconXSandbox](https://www.falconpy.io/Service-Collections/Falconx-Sandbox.html) |
 | User and Roles | [user_management.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/user_management.py) | [UserManagement](https://www.falconpy.io/Service-Collections/User-Management.html) |
 | Falcon Zero Trust Assessment | [zero_trust_assessment.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/zero_trust_assessment.py) | [ZeroTrustAssessment](https://www.falconpy.io/Service-Collections/Zero-Trust-Assessment.html) |
 
 
 #### Service Class benefits
 
 - Closely follows Python and OpenAPI best practice for code style and syntax. PEP-8 compliant.
@@ -259,15 +259,15 @@
         print(f"[Error {error_code}] {error_message}")
 ```
 
 ### More samples
 If you are interested in reviewing more examples of FalconPy usage, this repository also maintains a collection of [samples](https://github.com/CrowdStrike/falconpy/tree/main/samples) to help get you started with integrating CrowdStrike Falcon into your DevOps processes.
 
 ## Documentation and Support 📖
-FalconPy is a community-driven open source project designed to assist developers with implementing CrowdStrike's APIs within their applications, and is not a formal CrowdStrike product. As such it carries no formal support, expressed or implied.
+FalconPy is a community-driven, open source project designed to assist developers in leveraging the power of CrowdStrike APIs within their solutions. While not a formal CrowdStrike product, FalconPy is maintained by CrowdStrike and supported in partnership with the open source developer community.
 
 ### Official Project Documentation: [falconpy.io](https://falconpy.io)
 
 [![Website](https://img.shields.io/website?down_color=lightgrey&down_message=offline&label=falconpy.io&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABIAAAAOCAYAAAAi2ky3AAABhWlDQ1BJQ0MgcHJvZmlsZQAAKJF9kT1Iw1AUhU9TpaIVBzuIOGSoDmJBVEQ3rUIRKoRaoVUHk5f%2BCE0akhQXR8G14ODPYtXBxVlXB1dBEPwBcXNzUnSREu9LCi1ifPB4H%2Be9c7jvXkColZhmtY0Cmm6bqURczGRXxNAruhAEMI1hmVnGrCQl4bu%2B7hHg512MZ%2Fm%2F%2B3N1qzmLAQGReIYZpk28Tjy5aRuc94kjrCirxOfEIyYVSPzIdcXjN84FlwWeGTHTqTniCLFYaGGlhVnR1IgniKOqplO%2BkPFY5bzFWStVWKNO%2FsNwTl9e4jrtASSwgEVIEKGggg2UYCNGp06KhRTdx338%2Fa5fIpdCrg0wcsyjDA2y6wefwe%2FeWvnxMS8pHAfaXxznYxAI7QL1quN8HztO%2FQQIPgNXetNfrgFTn6RXm1r0COjZBi6um5qyB1zuAH1PhmzKrsTnL%2BTzwPsZjSkL9N4Cnate3xr3OH0A0tSr5A1wcAgMFSh7zeffHa19%2B%2FdNo38%2Fhq9yr%2BiELI0AAAAGYktHRAAAAAAAAPlDu38AAAAJcEhZcwAACxMAAAsTAQCanBgAAAAHdElNRQflDAsTByz7Va2cAAAAGXRFWHRDb21tZW50AENyZWF0ZWQgd2l0aCBHSU1QV4EOFwAAAYBJREFUKM%2BlkjFIlVEYht%2Fzn3sFkYYUyUnIRcemhCtCU6JQOLiIU%2BQeJEQg6BBIm0s4RBCBLjq5OEvgJC1uOniJhivesLx17%2F97%2FvO9b4NK4g25157hfHCGB773%2FcA0HZIEAKiMj%2BLWiOxljG%2Fi96pnCFP58XHnrWX2%2B9cj0dYl9Yu2FE9%2F9rXrcAAgs2eSyiBfOe%2FXRD503h%2FCuffOubQVUXL%2BJh9BllzBbyJJBgDclVkO4Kukd8zzkXJbeUljIldFTstsmSHM6S81ma2KfPKlFdkGAMY4wzx%2FbbXapMy21My%2BYizdKNq5mDzLkrxafSxySFKjSWX2oTmjKzz4vN0r2lOFcL%2FQ3V0%2FmX95ILMXTTGYVfaut%2FaP2%2BoCMAvnZgCcsF5fcR0dg65YHAdwB%2BQApADvu0AuOe%2FftlJAD7Nsgmm6yBjDtfWORJZlNtFyo%2FlR5Z7MyheKA5ktSur7sTAHazSG27pehjAiaVfkN8b4XFIJ%2FwOzbOx07VNRUuHy7w98CzCcGPyWywAAAABJRU5ErkJggg%3D%3D&up_color=green&up_message=online&url=https%3A%2F%2Ffalconpy.io)](https://falconpy.io)
 ![Documentation Version](https://img.shields.io/endpoint?url=https%3A%2F%2Ffalconpy.io%2F_version.json&label=documentation%20version)
 
 Extended documentation is also available via the [wiki](https://github.com/CrowdStrike/falconpy/wiki) for this repository.
@@ -288,38 +288,27 @@
 
 ### Community forums
 
 The discussion board for this repository also provides the community with means to communicate regarding [enhancements ideas](https://github.com/CrowdStrike/falconpy/discussions?discussions_q=category%3AIdeas), [integration examples](https://github.com/CrowdStrike/falconpy/discussions/496) and [new releases](https://github.com/CrowdStrike/falconpy/discussions?discussions_q=category%3A%22Show+and+tell%22).
 
 [![Discussions](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/join-the-discussion.png)](https://github.com/CrowdStrike/falconpy/discussions)
 
-### Additional content
-The following materials have been produced by the maintainers and members of the community regarding FalconPy.
-
-| Content | Description |
-| :--- | :--- |
-| [![API Office Hour 03.23.21](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/api_office_hour_preso_thumbnail.png)](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/falconpy-api-office-hour_customer_presentation.pdf?raw=true) | **API Office Hour 03-23-21**<BR/>Presentation deck used to discuss FalconPy functionality, structure and roadmap for a virtual API office hour event in March 2021. |
-| [![Fal.Con 2021](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/fal.con-2021-presentation.png)](https://www.crowdstrike.com/falcon/video-on-demand-2021/?wchannelid=w0jyzi2b8e&wmediaid=z5jymvzhyu) | **Fal.Con 2021**<BR/>Virtual presentation given by `@jshcodes` at Fal.Con 2021. Focused on basic functionality and usage, existing integrations that leverage FalconPy, available library documentation, and the FalconPy community. |
-
-
-More information regarding FalconPy documentation and support can be found [here](https://github.com/CrowdStrike/falconpy/blob/main/SUPPORT.md).
+> More information regarding FalconPy documentation and support can be found [here](https://github.com/CrowdStrike/falconpy/blob/main/SUPPORT.md).
 
 
 ## Contribute to FalconPy ☕
 Interested in [being acknowledged](https://github.com/CrowdStrike/falconpy/blob/main/AUTHORS.md#contributors) as a member of an elite community of security-focused Python developers that **stop breaches**? 
 
 There are *many* ways you can contribute to the FalconPy project! 
 
-_Providing feedback_ by opening a GitHub ticket. Even a fly-by "hey, this worked..." is appreciated and helps validate approaches. Ideas on improving the project are most welcome.
-
-_Documenting, blogging, or creating videos_, of how you've used FalconPy! This type of content is *invaluable* and helps our community grow. Open a pull request for inclusion in the [Additional content](https://github.com/CrowdStrike/falconpy#additional-content) section of this page.
-
-_Fix a bug or implement a new feature_. Check out our [open issues on GitHub](https://github.com/CrowdStrike/falconpy/issues) or our [discussion board](https://github.com/CrowdStrike/falconpy/discussions) for inspiration.
-
-_Review pull requests_ by going through the queue of [open pull requests on GitHub](https://github.com/CrowdStrike/falconpy/pulls) and giving feedback to the authors.
+- _Providing feedback_ by opening a GitHub ticket. Even a fly-by "hey, this worked..." is appreciated and helps validate approaches. Ideas on improving the project are most welcome.
+- _Documenting, blogging, or creating videos_, of how you've used FalconPy. This type of content is *invaluable* and helps our community grow. Post these in the [Show and Tell](https://github.com/CrowdStrike/falconpy/discussions/categories/show-and-tell) category of our [discussion board](https://github.com/CrowdStrike/falconpy/discussions).
+- _Submit a sample_ demonstrating how you're using FalconPy by opening a pull request for inclusion in the [Samples Library](https://github.com/CrowdStrike/falconpy/tree/main/samples).
+- _Fix a bug or implement a new feature_. Check out our [open issues on GitHub](https://github.com/CrowdStrike/falconpy/issues) or our [discussion board](https://github.com/CrowdStrike/falconpy/discussions) for inspiration.
+- _Review pull requests_ by going through the queue of [open pull requests on GitHub](https://github.com/CrowdStrike/falconpy/pulls) and giving feedback to the authors.
 
 To get started, review the [Code of Conduct](https://github.com/CrowdStrike/falconpy/blob/main/CODE_OF_CONDUCT.md) for community guidelines, and the [contribution guide](https://github.com/CrowdStrike/falconpy/blob/main/CONTRIBUTING.md) for more detail regarding contributing to the CrowdStrike FalconPy project.
 
 
 ---
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/README.md` & `crowdstrike-falconpy-dev-1.3.0.dev6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 | Real Time Response (RTR) Policies | [response_policies.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/response_policies.py) | [ResponsePolicies](https://www.falconpy.io/Service-Collections/Response-Policies.html) |
 | Report Executions | [report_executions.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/report_executions.py) | [ReportExecutions](https://www.falconpy.io/Service-Collections/Report-Executions.html) |
 | Scheduled Reports | [scheduled_reports.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/scheduled_reports.py) | [ScheduledReports](https://www.falconpy.io/Service-Collections/Scheduled-Reports.html) |
 | Sensor Download | [sensor_download.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sensor_download.py) | [SensorDownload](https://www.falconpy.io/Service-Collections/Sensor-Download.html) |
 | Sensor Visibility Exclusions | [sensor_visibility_exclusions.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sensor_visibility_exclusions.py) | [SensorVisibilityExclusions](https://www.falconpy.io/Service-Collections/Sensor-Visibility-Exclusions.html) |
 | Sensor Update Policy Management | [sensor_update_policy.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sensor_update_policy.py) | [SensorUpdatePolicy](https://www.falconpy.io/Service-Collections/Sensor-Update-Policy.html) |
 | Spotlight | [spotlight_evaluation_logic.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/spotlight_evaluation_logic.py)<BR/>[spotlight_vulnerabilities.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/spotlight_vulnerabilities.py) | [SpotlightEvaluationLogic](https://www.falconpy.io/Service-Collections/Spotlight-Evaluation-Logic.html)<BR/>[SpotlightVulnerabilities](https://www.falconpy.io/Service-Collections/Spotlight-Vulnerabilities.html) |
-| Falcon Intelligence | [falconx_sandbox.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/falconx_sandbox.py)<BR/>[intel.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/intel.py)<br/>[ioc.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/ioc.py) <BR/> [iocs.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/iocs.py) <small>*Deprecated*</small><BR/>[malquery.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/malquery.py)<BR/>[quick_scan.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/quick_scan.py)<BR/>[recon.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/recon.py)<BR/>[sample_uploads.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sample_uploads.py)| [FalconXSandbox](https://www.falconpy.io/Service-Collections/Falconx-Sandbox.html)<BR/>[Intel](https://www.falconpy.io/Service-Collections/Intel.html)<BR/>[IOC](https://www.falconpy.io/Service-Collections/IOC.html)<BR/>[Iocs](https://www.falconpy.io/Service-Collections/IOCs.html)<BR/>[MalQuery](https://www.falconpy.io/Service-Collections/MalQuery.html)<BR/>[QuickScan](https://www.falconpy.io/Service-Collections/Quick-Scan.html)<BR/><a href="https://www.falconpy.io/Service-Collections/Recon.html" target="_blank">Recon</a><BR/>[SampleUploads](https://www.falconpy.io/Service-Collections/Sample-Uploads.html) |
+| __Falcon Intelligence__<BR/>Intel<BR/>IOC<BR/>IOCS<BR/>MalQuery<BR/>ODS (On Demand Scan)<BR/>Quick Scan<BR/>Recon<BR/>Sample Uploads<BR/>Sandbox | <BR/>[intel.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/intel.py)<br/>[ioc.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/ioc.py) <BR/> [iocs.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/iocs.py) <small>*Deprecated*</small><BR/>[malquery.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/malquery.py)<BR/>[ods.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/ods.py)<BR/>[quick_scan.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/quick_scan.py)<BR/>[recon.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/recon.py)<BR/>[sample_uploads.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sample_uploads.py) <BR/> [falconx_sandbox.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/falconx_sandbox.py)| <BR/>[Intel](https://www.falconpy.io/Service-Collections/Intel.html)<BR/>[IOC](https://www.falconpy.io/Service-Collections/IOC.html)<BR/>[Iocs](https://www.falconpy.io/Service-Collections/IOCs.html)<BR/>[MalQuery](https://www.falconpy.io/Service-Collections/MalQuery.html)<BR/>[ODS](https://www.falconpy.io/Service-Collections/ODS.html)<BR/>[QuickScan](https://www.falconpy.io/Service-Collections/Quick-Scan.html)<BR/><a href="https://www.falconpy.io/Service-Collections/Recon.html" target="_blank">Recon</a><BR/>[SampleUploads](https://www.falconpy.io/Service-Collections/Sample-Uploads.html)<BR/>[FalconXSandbox](https://www.falconpy.io/Service-Collections/Falconx-Sandbox.html) |
 | User and Roles | [user_management.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/user_management.py) | [UserManagement](https://www.falconpy.io/Service-Collections/User-Management.html) |
 | Falcon Zero Trust Assessment | [zero_trust_assessment.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/zero_trust_assessment.py) | [ZeroTrustAssessment](https://www.falconpy.io/Service-Collections/Zero-Trust-Assessment.html) |
 
 
 #### Service Class benefits
 
 - Closely follows Python and OpenAPI best practice for code style and syntax. PEP-8 compliant.
@@ -212,15 +212,15 @@
         print(f"[Error {error_code}] {error_message}")
 ```
 
 ### More samples
 If you are interested in reviewing more examples of FalconPy usage, this repository also maintains a collection of [samples](https://github.com/CrowdStrike/falconpy/tree/main/samples) to help get you started with integrating CrowdStrike Falcon into your DevOps processes.
 
 ## Documentation and Support 📖
-FalconPy is a community-driven open source project designed to assist developers with implementing CrowdStrike's APIs within their applications, and is not a formal CrowdStrike product. As such it carries no formal support, expressed or implied.
+FalconPy is a community-driven, open source project designed to assist developers in leveraging the power of CrowdStrike APIs within their solutions. While not a formal CrowdStrike product, FalconPy is maintained by CrowdStrike and supported in partnership with the open source developer community.
 
 ### Official Project Documentation: [falconpy.io](https://falconpy.io)
 
 [![Website](https://img.shields.io/website?down_color=lightgrey&down_message=offline&label=falconpy.io&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABIAAAAOCAYAAAAi2ky3AAABhWlDQ1BJQ0MgcHJvZmlsZQAAKJF9kT1Iw1AUhU9TpaIVBzuIOGSoDmJBVEQ3rUIRKoRaoVUHk5f%2BCE0akhQXR8G14ODPYtXBxVlXB1dBEPwBcXNzUnSREu9LCi1ifPB4H%2Be9c7jvXkColZhmtY0Cmm6bqURczGRXxNAruhAEMI1hmVnGrCQl4bu%2B7hHg512MZ%2Fm%2F%2B3N1qzmLAQGReIYZpk28Tjy5aRuc94kjrCirxOfEIyYVSPzIdcXjN84FlwWeGTHTqTniCLFYaGGlhVnR1IgniKOqplO%2BkPFY5bzFWStVWKNO%2FsNwTl9e4jrtASSwgEVIEKGggg2UYCNGp06KhRTdx338%2Fa5fIpdCrg0wcsyjDA2y6wefwe%2FeWvnxMS8pHAfaXxznYxAI7QL1quN8HztO%2FQQIPgNXetNfrgFTn6RXm1r0COjZBi6um5qyB1zuAH1PhmzKrsTnL%2BTzwPsZjSkL9N4Cnate3xr3OH0A0tSr5A1wcAgMFSh7zeffHa19%2B%2FdNo38%2Fhq9yr%2BiELI0AAAAGYktHRAAAAAAAAPlDu38AAAAJcEhZcwAACxMAAAsTAQCanBgAAAAHdElNRQflDAsTByz7Va2cAAAAGXRFWHRDb21tZW50AENyZWF0ZWQgd2l0aCBHSU1QV4EOFwAAAYBJREFUKM%2BlkjFIlVEYht%2Fzn3sFkYYUyUnIRcemhCtCU6JQOLiIU%2BQeJEQg6BBIm0s4RBCBLjq5OEvgJC1uOniJhivesLx17%2F97%2FvO9b4NK4g25157hfHCGB773%2FcA0HZIEAKiMj%2BLWiOxljG%2Fi96pnCFP58XHnrWX2%2B9cj0dYl9Yu2FE9%2F9rXrcAAgs2eSyiBfOe%2FXRD503h%2FCuffOubQVUXL%2BJh9BllzBbyJJBgDclVkO4Kukd8zzkXJbeUljIldFTstsmSHM6S81ma2KfPKlFdkGAMY4wzx%2FbbXapMy21My%2BYizdKNq5mDzLkrxafSxySFKjSWX2oTmjKzz4vN0r2lOFcL%2FQ3V0%2FmX95ILMXTTGYVfaut%2FaP2%2BoCMAvnZgCcsF5fcR0dg65YHAdwB%2BQApADvu0AuOe%2FftlJAD7Nsgmm6yBjDtfWORJZlNtFyo%2FlR5Z7MyheKA5ktSur7sTAHazSG27pehjAiaVfkN8b4XFIJ%2FwOzbOx07VNRUuHy7w98CzCcGPyWywAAAABJRU5ErkJggg%3D%3D&up_color=green&up_message=online&url=https%3A%2F%2Ffalconpy.io)](https://falconpy.io)
 ![Documentation Version](https://img.shields.io/endpoint?url=https%3A%2F%2Ffalconpy.io%2F_version.json&label=documentation%20version)
 
 Extended documentation is also available via the [wiki](https://github.com/CrowdStrike/falconpy/wiki) for this repository.
@@ -241,38 +241,27 @@
 
 ### Community forums
 
 The discussion board for this repository also provides the community with means to communicate regarding [enhancements ideas](https://github.com/CrowdStrike/falconpy/discussions?discussions_q=category%3AIdeas), [integration examples](https://github.com/CrowdStrike/falconpy/discussions/496) and [new releases](https://github.com/CrowdStrike/falconpy/discussions?discussions_q=category%3A%22Show+and+tell%22).
 
 [![Discussions](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/join-the-discussion.png)](https://github.com/CrowdStrike/falconpy/discussions)
 
-### Additional content
-The following materials have been produced by the maintainers and members of the community regarding FalconPy.
-
-| Content | Description |
-| :--- | :--- |
-| [![API Office Hour 03.23.21](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/api_office_hour_preso_thumbnail.png)](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/falconpy-api-office-hour_customer_presentation.pdf?raw=true) | **API Office Hour 03-23-21**<BR/>Presentation deck used to discuss FalconPy functionality, structure and roadmap for a virtual API office hour event in March 2021. |
-| [![Fal.Con 2021](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/fal.con-2021-presentation.png)](https://www.crowdstrike.com/falcon/video-on-demand-2021/?wchannelid=w0jyzi2b8e&wmediaid=z5jymvzhyu) | **Fal.Con 2021**<BR/>Virtual presentation given by `@jshcodes` at Fal.Con 2021. Focused on basic functionality and usage, existing integrations that leverage FalconPy, available library documentation, and the FalconPy community. |
-
-
-More information regarding FalconPy documentation and support can be found [here](https://github.com/CrowdStrike/falconpy/blob/main/SUPPORT.md).
+> More information regarding FalconPy documentation and support can be found [here](https://github.com/CrowdStrike/falconpy/blob/main/SUPPORT.md).
 
 
 ## Contribute to FalconPy ☕
 Interested in [being acknowledged](https://github.com/CrowdStrike/falconpy/blob/main/AUTHORS.md#contributors) as a member of an elite community of security-focused Python developers that **stop breaches**? 
 
 There are *many* ways you can contribute to the FalconPy project! 
 
-_Providing feedback_ by opening a GitHub ticket. Even a fly-by "hey, this worked..." is appreciated and helps validate approaches. Ideas on improving the project are most welcome.
-
-_Documenting, blogging, or creating videos_, of how you've used FalconPy! This type of content is *invaluable* and helps our community grow. Open a pull request for inclusion in the [Additional content](https://github.com/CrowdStrike/falconpy#additional-content) section of this page.
-
-_Fix a bug or implement a new feature_. Check out our [open issues on GitHub](https://github.com/CrowdStrike/falconpy/issues) or our [discussion board](https://github.com/CrowdStrike/falconpy/discussions) for inspiration.
-
-_Review pull requests_ by going through the queue of [open pull requests on GitHub](https://github.com/CrowdStrike/falconpy/pulls) and giving feedback to the authors.
+- _Providing feedback_ by opening a GitHub ticket. Even a fly-by "hey, this worked..." is appreciated and helps validate approaches. Ideas on improving the project are most welcome.
+- _Documenting, blogging, or creating videos_, of how you've used FalconPy. This type of content is *invaluable* and helps our community grow. Post these in the [Show and Tell](https://github.com/CrowdStrike/falconpy/discussions/categories/show-and-tell) category of our [discussion board](https://github.com/CrowdStrike/falconpy/discussions).
+- _Submit a sample_ demonstrating how you're using FalconPy by opening a pull request for inclusion in the [Samples Library](https://github.com/CrowdStrike/falconpy/tree/main/samples).
+- _Fix a bug or implement a new feature_. Check out our [open issues on GitHub](https://github.com/CrowdStrike/falconpy/issues) or our [discussion board](https://github.com/CrowdStrike/falconpy/discussions) for inspiration.
+- _Review pull requests_ by going through the queue of [open pull requests on GitHub](https://github.com/CrowdStrike/falconpy/pulls) and giving feedback to the authors.
 
 To get started, review the [Code of Conduct](https://github.com/CrowdStrike/falconpy/blob/main/CODE_OF_CONDUCT.md) for community guidelines, and the [contribution guide](https://github.com/CrowdStrike/falconpy/blob/main/CONTRIBUTING.md) for more detail regarding contributing to the CrowdStrike FalconPy project.
 
 
 ---
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/dev_setup.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/dev_setup.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/setup.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy-dev
-Version: 1.3.0.dev1
+Version: 1.3.0.dev6
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
@@ -156,15 +156,15 @@
 | Real Time Response (RTR) Policies | [response_policies.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/response_policies.py) | [ResponsePolicies](https://www.falconpy.io/Service-Collections/Response-Policies.html) |
 | Report Executions | [report_executions.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/report_executions.py) | [ReportExecutions](https://www.falconpy.io/Service-Collections/Report-Executions.html) |
 | Scheduled Reports | [scheduled_reports.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/scheduled_reports.py) | [ScheduledReports](https://www.falconpy.io/Service-Collections/Scheduled-Reports.html) |
 | Sensor Download | [sensor_download.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sensor_download.py) | [SensorDownload](https://www.falconpy.io/Service-Collections/Sensor-Download.html) |
 | Sensor Visibility Exclusions | [sensor_visibility_exclusions.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sensor_visibility_exclusions.py) | [SensorVisibilityExclusions](https://www.falconpy.io/Service-Collections/Sensor-Visibility-Exclusions.html) |
 | Sensor Update Policy Management | [sensor_update_policy.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sensor_update_policy.py) | [SensorUpdatePolicy](https://www.falconpy.io/Service-Collections/Sensor-Update-Policy.html) |
 | Spotlight | [spotlight_evaluation_logic.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/spotlight_evaluation_logic.py)<BR/>[spotlight_vulnerabilities.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/spotlight_vulnerabilities.py) | [SpotlightEvaluationLogic](https://www.falconpy.io/Service-Collections/Spotlight-Evaluation-Logic.html)<BR/>[SpotlightVulnerabilities](https://www.falconpy.io/Service-Collections/Spotlight-Vulnerabilities.html) |
-| Falcon Intelligence | [falconx_sandbox.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/falconx_sandbox.py)<BR/>[intel.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/intel.py)<br/>[ioc.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/ioc.py) <BR/> [iocs.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/iocs.py) *Deprecated*<BR/>[malquery.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/malquery.py)<BR/>[quick_scan.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/quick_scan.py)<BR/>[recon.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/recon.py)<BR/>[sample_uploads.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sample_uploads.py)| [FalconXSandbox](https://www.falconpy.io/Service-Collections/Falconx-Sandbox.html)<BR/>[Intel](https://www.falconpy.io/Service-Collections/Intel.html)<BR/>[IOC](https://www.falconpy.io/Service-Collections/IOC.html)<BR/>[Iocs](https://www.falconpy.io/Service-Collections/IOCs.html)<BR/>[MalQuery](https://www.falconpy.io/Service-Collections/MalQuery.html)<BR/>[QuickScan](https://www.falconpy.io/Service-Collections/Quick-Scan.html)<BR/><a href="https://www.falconpy.io/Service-Collections/Recon.html" target="_blank">Recon</a><BR/>[SampleUploads](https://www.falconpy.io/Service-Collections/Sample-Uploads.html) |
+| __Falcon Intelligence__<BR/>Intel<BR/>IOC<BR/>IOCS<BR/>MalQuery<BR/>ODS (On Demand Scan)<BR/>Quick Scan<BR/>Recon<BR/>Sample Uploads<BR/>Sandbox | <BR/>[intel.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/intel.py)<br/>[ioc.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/ioc.py) <BR/> [iocs.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/iocs.py) *Deprecated*<BR/>[malquery.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/malquery.py)<BR/>[ods.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/ods.py)<BR/>[quick_scan.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/quick_scan.py)<BR/>[recon.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/recon.py)<BR/>[sample_uploads.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/sample_uploads.py) <BR/> [falconx_sandbox.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/falconx_sandbox.py)| <BR/>[Intel](https://www.falconpy.io/Service-Collections/Intel.html)<BR/>[IOC](https://www.falconpy.io/Service-Collections/IOC.html)<BR/>[Iocs](https://www.falconpy.io/Service-Collections/IOCs.html)<BR/>[MalQuery](https://www.falconpy.io/Service-Collections/MalQuery.html)<BR/>[ODS](https://www.falconpy.io/Service-Collections/ODS.html)<BR/>[QuickScan](https://www.falconpy.io/Service-Collections/Quick-Scan.html)<BR/><a href="https://www.falconpy.io/Service-Collections/Recon.html" target="_blank">Recon</a><BR/>[SampleUploads](https://www.falconpy.io/Service-Collections/Sample-Uploads.html)<BR/>[FalconXSandbox](https://www.falconpy.io/Service-Collections/Falconx-Sandbox.html) |
 | User and Roles | [user_management.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/user_management.py) | [UserManagement](https://www.falconpy.io/Service-Collections/User-Management.html) |
 | Falcon Zero Trust Assessment | [zero_trust_assessment.py](https://github.com/CrowdStrike/falconpy/blob/main/src/falconpy/zero_trust_assessment.py) | [ZeroTrustAssessment](https://www.falconpy.io/Service-Collections/Zero-Trust-Assessment.html) |
 
 
 #### Service Class benefits
 
 - Closely follows Python and OpenAPI best practice for code style and syntax. PEP-8 compliant.
@@ -259,15 +259,15 @@
         print(f"[Error {error_code}] {error_message}")
 ```
 
 ### More samples
 If you are interested in reviewing more examples of FalconPy usage, this repository also maintains a collection of [samples](https://github.com/CrowdStrike/falconpy/tree/main/samples) to help get you started with integrating CrowdStrike Falcon into your DevOps processes.
 
 ## Documentation and Support 📖
-FalconPy is a community-driven open source project designed to assist developers with implementing CrowdStrike's APIs within their applications, and is not a formal CrowdStrike product. As such it carries no formal support, expressed or implied.
+FalconPy is a community-driven, open source project designed to assist developers in leveraging the power of CrowdStrike APIs within their solutions. While not a formal CrowdStrike product, FalconPy is maintained by CrowdStrike and supported in partnership with the open source developer community.
 
 ### Official Project Documentation: [falconpy.io](https://falconpy.io)
 
 [![Website](https://img.shields.io/website?down_color=lightgrey&down_message=offline&label=falconpy.io&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABIAAAAOCAYAAAAi2ky3AAABhWlDQ1BJQ0MgcHJvZmlsZQAAKJF9kT1Iw1AUhU9TpaIVBzuIOGSoDmJBVEQ3rUIRKoRaoVUHk5f%2BCE0akhQXR8G14ODPYtXBxVlXB1dBEPwBcXNzUnSREu9LCi1ifPB4H%2Be9c7jvXkColZhmtY0Cmm6bqURczGRXxNAruhAEMI1hmVnGrCQl4bu%2B7hHg512MZ%2Fm%2F%2B3N1qzmLAQGReIYZpk28Tjy5aRuc94kjrCirxOfEIyYVSPzIdcXjN84FlwWeGTHTqTniCLFYaGGlhVnR1IgniKOqplO%2BkPFY5bzFWStVWKNO%2FsNwTl9e4jrtASSwgEVIEKGggg2UYCNGp06KhRTdx338%2Fa5fIpdCrg0wcsyjDA2y6wefwe%2FeWvnxMS8pHAfaXxznYxAI7QL1quN8HztO%2FQQIPgNXetNfrgFTn6RXm1r0COjZBi6um5qyB1zuAH1PhmzKrsTnL%2BTzwPsZjSkL9N4Cnate3xr3OH0A0tSr5A1wcAgMFSh7zeffHa19%2B%2FdNo38%2Fhq9yr%2BiELI0AAAAGYktHRAAAAAAAAPlDu38AAAAJcEhZcwAACxMAAAsTAQCanBgAAAAHdElNRQflDAsTByz7Va2cAAAAGXRFWHRDb21tZW50AENyZWF0ZWQgd2l0aCBHSU1QV4EOFwAAAYBJREFUKM%2BlkjFIlVEYht%2Fzn3sFkYYUyUnIRcemhCtCU6JQOLiIU%2BQeJEQg6BBIm0s4RBCBLjq5OEvgJC1uOniJhivesLx17%2F97%2FvO9b4NK4g25157hfHCGB773%2FcA0HZIEAKiMj%2BLWiOxljG%2Fi96pnCFP58XHnrWX2%2B9cj0dYl9Yu2FE9%2F9rXrcAAgs2eSyiBfOe%2FXRD503h%2FCuffOubQVUXL%2BJh9BllzBbyJJBgDclVkO4Kukd8zzkXJbeUljIldFTstsmSHM6S81ma2KfPKlFdkGAMY4wzx%2FbbXapMy21My%2BYizdKNq5mDzLkrxafSxySFKjSWX2oTmjKzz4vN0r2lOFcL%2FQ3V0%2FmX95ILMXTTGYVfaut%2FaP2%2BoCMAvnZgCcsF5fcR0dg65YHAdwB%2BQApADvu0AuOe%2FftlJAD7Nsgmm6yBjDtfWORJZlNtFyo%2FlR5Z7MyheKA5ktSur7sTAHazSG27pehjAiaVfkN8b4XFIJ%2FwOzbOx07VNRUuHy7w98CzCcGPyWywAAAABJRU5ErkJggg%3D%3D&up_color=green&up_message=online&url=https%3A%2F%2Ffalconpy.io)](https://falconpy.io)
 ![Documentation Version](https://img.shields.io/endpoint?url=https%3A%2F%2Ffalconpy.io%2F_version.json&label=documentation%20version)
 
 Extended documentation is also available via the [wiki](https://github.com/CrowdStrike/falconpy/wiki) for this repository.
@@ -288,38 +288,27 @@
 
 ### Community forums
 
 The discussion board for this repository also provides the community with means to communicate regarding [enhancements ideas](https://github.com/CrowdStrike/falconpy/discussions?discussions_q=category%3AIdeas), [integration examples](https://github.com/CrowdStrike/falconpy/discussions/496) and [new releases](https://github.com/CrowdStrike/falconpy/discussions?discussions_q=category%3A%22Show+and+tell%22).
 
 [![Discussions](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/join-the-discussion.png)](https://github.com/CrowdStrike/falconpy/discussions)
 
-### Additional content
-The following materials have been produced by the maintainers and members of the community regarding FalconPy.
-
-| Content | Description |
-| :--- | :--- |
-| [![API Office Hour 03.23.21](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/api_office_hour_preso_thumbnail.png)](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/falconpy-api-office-hour_customer_presentation.pdf?raw=true) | **API Office Hour 03-23-21**<BR/>Presentation deck used to discuss FalconPy functionality, structure and roadmap for a virtual API office hour event in March 2021. |
-| [![Fal.Con 2021](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/fal.con-2021-presentation.png)](https://www.crowdstrike.com/falcon/video-on-demand-2021/?wchannelid=w0jyzi2b8e&wmediaid=z5jymvzhyu) | **Fal.Con 2021**<BR/>Virtual presentation given by `@jshcodes` at Fal.Con 2021. Focused on basic functionality and usage, existing integrations that leverage FalconPy, available library documentation, and the FalconPy community. |
-
-
-More information regarding FalconPy documentation and support can be found [here](https://github.com/CrowdStrike/falconpy/blob/main/SUPPORT.md).
+> More information regarding FalconPy documentation and support can be found [here](https://github.com/CrowdStrike/falconpy/blob/main/SUPPORT.md).
 
 
 ## Contribute to FalconPy ☕
 Interested in [being acknowledged](https://github.com/CrowdStrike/falconpy/blob/main/AUTHORS.md#contributors) as a member of an elite community of security-focused Python developers that **stop breaches**? 
 
 There are *many* ways you can contribute to the FalconPy project! 
 
-_Providing feedback_ by opening a GitHub ticket. Even a fly-by "hey, this worked..." is appreciated and helps validate approaches. Ideas on improving the project are most welcome.
-
-_Documenting, blogging, or creating videos_, of how you've used FalconPy! This type of content is *invaluable* and helps our community grow. Open a pull request for inclusion in the [Additional content](https://github.com/CrowdStrike/falconpy#additional-content) section of this page.
-
-_Fix a bug or implement a new feature_. Check out our [open issues on GitHub](https://github.com/CrowdStrike/falconpy/issues) or our [discussion board](https://github.com/CrowdStrike/falconpy/discussions) for inspiration.
-
-_Review pull requests_ by going through the queue of [open pull requests on GitHub](https://github.com/CrowdStrike/falconpy/pulls) and giving feedback to the authors.
+- _Providing feedback_ by opening a GitHub ticket. Even a fly-by "hey, this worked..." is appreciated and helps validate approaches. Ideas on improving the project are most welcome.
+- _Documenting, blogging, or creating videos_, of how you've used FalconPy. This type of content is *invaluable* and helps our community grow. Post these in the [Show and Tell](https://github.com/CrowdStrike/falconpy/discussions/categories/show-and-tell) category of our [discussion board](https://github.com/CrowdStrike/falconpy/discussions).
+- _Submit a sample_ demonstrating how you're using FalconPy by opening a pull request for inclusion in the [Samples Library](https://github.com/CrowdStrike/falconpy/tree/main/samples).
+- _Fix a bug or implement a new feature_. Check out our [open issues on GitHub](https://github.com/CrowdStrike/falconpy/issues) or our [discussion board](https://github.com/CrowdStrike/falconpy/discussions) for inspiration.
+- _Review pull requests_ by going through the queue of [open pull requests on GitHub](https://github.com/CrowdStrike/falconpy/pulls) and giving feedback to the authors.
 
 To get started, review the [Code of Conduct](https://github.com/CrowdStrike/falconpy/blob/main/CODE_OF_CONDUCT.md) for community guidelines, and the [contribution guide](https://github.com/CrowdStrike/falconpy/blob/main/CONTRIBUTING.md) for more detail regarding contributing to the CrowdStrike FalconPy project.
 
 
 ---
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/falconpydev/detects.py
 src/falconpydev/device_control_policies.py
 src/falconpydev/discover.py
 src/falconpydev/event_streams.py
 src/falconpydev/falcon_complete_dashboard.py
 src/falconpydev/falcon_container.py
 src/falconpydev/falconx_sandbox.py
+src/falconpydev/fdr.py
 src/falconpydev/filevantage.py
 src/falconpydev/firewall_management.py
 src/falconpydev/firewall_policies.py
 src/falconpydev/host_group.py
 src/falconpydev/hosts.py
 src/falconpydev/identity_protection.py
 src/falconpydev/incidents.py
@@ -86,14 +87,15 @@
 src/falconpydev/_endpoint/_detects.py
 src/falconpydev/_endpoint/_device_control_policies.py
 src/falconpydev/_endpoint/_discover.py
 src/falconpydev/_endpoint/_event_streams.py
 src/falconpydev/_endpoint/_falcon_complete_dashboard.py
 src/falconpydev/_endpoint/_falcon_container.py
 src/falconpydev/_endpoint/_falconx_sandbox.py
+src/falconpydev/_endpoint/_fdr.py
 src/falconpydev/_endpoint/_filevantage.py
 src/falconpydev/_endpoint/_firewall_management.py
 src/falconpydev/_endpoint/_firewall_policies.py
 src/falconpydev/_endpoint/_host_group.py
 src/falconpydev/_endpoint/_hosts.py
 src/falconpydev/_endpoint/_identity_protection.py
 src/falconpydev/_endpoint/_incidents.py
@@ -127,26 +129,29 @@
 src/falconpydev/_endpoint/_spotlight_evaluation_logic.py
 src/falconpydev/_endpoint/_spotlight_vulnerabilities.py
 src/falconpydev/_endpoint/_tailored_intelligence.py
 src/falconpydev/_endpoint/_user_management.py
 src/falconpydev/_endpoint/_zero_trust_assessment.py
 src/falconpydev/_endpoint/deprecated/__init__.py
 src/falconpydev/_endpoint/deprecated/_custom_ioa.py
+src/falconpydev/_endpoint/deprecated/_d4c_registration.py
 src/falconpydev/_endpoint/deprecated/_discover.py
+src/falconpydev/_endpoint/deprecated/_fdr.py
 src/falconpydev/_endpoint/deprecated/_firewall_management.py
 src/falconpydev/_endpoint/deprecated/_hosts.py
 src/falconpydev/_endpoint/deprecated/_identity_protection.py
 src/falconpydev/_endpoint/deprecated/_installation_tokens.py
 src/falconpydev/_endpoint/deprecated/_ioc.py
 src/falconpydev/_endpoint/deprecated/_iocs.py
 src/falconpydev/_endpoint/deprecated/_ods.py
 src/falconpydev/_endpoint/deprecated/_real_time_response.py
 src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py
 src/falconpydev/_endpoint/deprecated/_report_executions.py
 src/falconpydev/_endpoint/deprecated/_scheduled_reports.py
+src/falconpydev/_endpoint/deprecated/_zero_trust_assessment.py
 src/falconpydev/_enum/__init__.py
 src/falconpydev/_enum/_base_url.py
 src/falconpydev/_enum/_container_base_url.py
 src/falconpydev/_enum/_token_fail_reason.py
 src/falconpydev/_error/__init__.py
 src/falconpydev/_error/_exceptions.py
 src/falconpydev/_error/_warnings.py
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                                                         |.  __) |___._|__|____|_____|__|__|.  ____|___  |
                                                         |:  |                             |:  |   |_____|
                                                         |::.|     CrowdStrike Falcon      |::.|
                                                         `---' OAuth2 API SDK for Python 3 `---'
 """
 from ._version import _VERSION, _MAINTAINER, _AUTHOR, _AUTHOR_EMAIL
 from ._version import _CREDITS, _DESCRIPTION, _TITLE, _PROJECT_URL
-from ._version import _DOCS_URL, _KEYWORDS
+from ._version import _DOCS_URL, _KEYWORDS, version
 from ._auth_object import (
     BaseFalconAuth,
     BearerToken,
     FalconInterface,
     UberInterface,
     InterfaceConfiguration
     )
@@ -54,15 +54,17 @@
     InvalidOperation,
     TokenNotSpecified,
     KeywordsOnly,
     CannotRevokeToken,
     FunctionalityNotImplemented,
     InvalidBaseURL,
     PayloadValidationError,
-    NoAuthenticationMechanism
+    NoAuthenticationMechanism,
+    InvalidIndex,
+    InvalidCredentialFormat
     )
 from ._result import (
     Result,
     ExpandedResult,
     BaseDictionary,
     BaseResource,
     Resources,
@@ -90,14 +92,15 @@
 from .detects import Detects
 from .device_control_policies import DeviceControlPolicies
 from .discover import Discover
 from .event_streams import EventStreams
 from .falcon_complete_dashboard import CompleteDashboard
 from .falcon_container import FalconContainer
 from .falconx_sandbox import FalconXSandbox
+from .fdr import FDR
 from .filevantage import FileVantage
 from .firewall_management import FirewallManagement
 from .firewall_policies import FirewallPolicies
 from .host_group import HostGroup
 from .hosts import Hosts
 from .identity_protection import IdentityProtection
 from .incidents import Incidents
@@ -153,25 +156,25 @@
     "Hosts", "IdentityProtection", "Incidents", "InstallationTokens", "Intel", "IOAExclusions",
     "IOC", "Iocs", "KubernetesProtection", "MalQuery", "MLExclusions", "FlightControl", "OAuth2",
     "OverwatchDashboard", "PreventionPolicy", "Quarantine", "QuickScan", "RealTimeResponseAdmin",
     "RealTimeResponse", "Recon", "ReportExecutions", "ResponsePolicies", "SampleUploads",
     "ScheduledReports", "SensorDownload", "SensorUpdatePolicy", "SensorVisibilityExclusions",
     "SpotlightVulnerabilities", "SpotlightEvaluationLogic", "UserManagement", "MAX_DEBUG_RECORDS",
     "ZeroTrustAssessment", "PreventionPolicies", "SensorUpdatePolicies", "MessageCenter",
-    "FileVantage", "MobileEnrollment", "ContainerBaseURL", "TailoredIntelligence", "ODS", "Result",
-    "APIError", "SDKError", "SDKWarning", "NoContentWarning", "SSLDisabledWarning",
+    "FileVantage", "MobileEnrollment", "ContainerBaseURL", "TailoredIntelligence", "ODS", "FDR",
+    "Result", "APIError", "SDKError", "SDKWarning", "NoContentWarning", "SSLDisabledWarning",
     "RegionSelectError", "InvalidCredentials", "InvalidMethod", "InvalidOperation",
     "TokenNotSpecified", "KeywordsOnly", "ALLOWED_METHODS", "USER_AGENT", "APIRequest",
     "ExpandedResult", "CannotRevokeToken", "Headers", "Meta", "Resources",
     "ResponseComponent", "BaseDictionary", "Errors", "BaseResource", "RawBody", "BinaryFile",
     "FunctionalityNotImplemented", "BearerToken", "LogFacility", "InvalidBaseURL",
     "InterfaceConfiguration", "RequestBehavior", "RequestConnection", "RequestMeta",
     "RequestPayloads", "RequestValidator", "PayloadValidationError", "MIN_TOKEN_RENEW_WINDOW",
     "MAX_TOKEN_RENEW_WINDOW", "GLOBAL_API_MAX_RETURN", "MOCK_OPERATIONS",
-    "NoAuthenticationMechanism"
+    "NoAuthenticationMechanism", "InvalidIndex", "version", "InvalidCredentialFormat"
     ]
 """
 This is free and unencumbered software released into the public domain.
 
 Anyone is free to copy, modify, publish, use, compile, sell, or
 distribute this software, either in source code form or as a compiled
 binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request_behavior.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_behavior.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request_connection.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_connection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request_meta.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_meta.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request_payloads.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_payloads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_api_request/_request_validator.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_validator.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/_base_falcon_auth.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_base_falcon_auth.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/_bearer_token.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_bearer_token.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/_falcon_interface.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_falcon_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 import time
 import warnings
+from json import loads
+try:
+    from simplejson import JSONDecodeError
+except ImportError:
+    from json.decoder import JSONDecodeError
 from logging import Logger, getLogger
 from typing import Dict, Optional, Union
 from ._base_falcon_auth import BaseFalconAuth
 from ._bearer_token import BearerToken
 from .._log import LogFacility
 from .._constant import MIN_TOKEN_RENEW_WINDOW, MAX_TOKEN_RENEW_WINDOW
 from ._interface_config import InterfaceConfiguration
@@ -51,17 +56,18 @@
 from .._util import (
     autodiscover_region,
     perform_request,
     log_class_startup,
     login_payloads,
     logout_payloads
     )
-from .._error import InvalidCredentials, NoAuthenticationMechanism
+from .._error import InvalidCredentials, NoAuthenticationMechanism, InvalidCredentialFormat
 
 
+# pylint: disable=R0902
 class FalconInterface(BaseFalconAuth):
     """Standard Falcon API interface used by Service Classes."""
 
     # ____ ___ ___ ____ _ ___  _  _ ___ ____ ____
     # |__|  |   |  |__/ | |__] |  |  |  |___ [__
     # |  |  |   |  |  \ | |__] |__|  |  |___ ___]
     #
@@ -84,15 +90,15 @@
 
     # ____ ____ _  _ ____ ___ ____ _  _ ____ ___ ____ ____
     # |    |  | |\ | [__   |  |__/ |  | |     |  |  | |__/
     # |___ |__| | \| ___]  |  |  \ |__| |___  |  |__| |  \
     #
     # The default constructor for all authentication objects. Ingests provided credentials
     # and sets the necessary class attributes based upon the authentication detail received.
-    # pylint: disable=R0913,R0914
+    # pylint: disable=R0912,R0913,R0914
     def __init__(self,
                  access_token: Optional[Union[str, bool]] = False,
                  base_url: Optional[str] = "https://api.crowdstrike.com",
                  creds: Optional[Dict[str, str]] = None,
                  client_id: Optional[str] = None,
                  client_secret: Optional[str] = None,
                  member_cid: Optional[str] = None,
@@ -129,15 +135,24 @@
             # You must pass member_cid the same way you pass client_id / secret.
             # If you use a creds dictionary, pass the member_cid there instead.
             if member_cid:
                 creds["member_cid"] = member_cid
         elif not creds:
             creds = {}
         # Credential Authentication (also powers Direct Authentication).
-        self.creds: Dict[str, str] = creds
+        if isinstance(creds, str):
+            try:
+                # Try and clean up any attempts to provide the dictionary as a string
+                self.creds: Dict[str, str] = loads(creds.replace("'", "\""))
+            except (TypeError, JSONDecodeError) as bad_cred_format:
+                raise InvalidCredentialFormat from bad_cred_format
+        elif isinstance(creds, dict):
+            self.creds: Dict[str, str] = creds
+        else:
+            raise InvalidCredentialFormat
         # Set the token renewal window, ignored when using Legacy Authentication.
         self.renew_window: int = max(min(renew_window, MAX_TOKEN_RENEW_WINDOW),
                                      MIN_TOKEN_RENEW_WINDOW
                                      )
         # Legacy (Token) Authentication (fallback)
         if access_token:
             # Store this non-refreshable token, assuming it was just generated.
@@ -202,23 +217,23 @@
                                            sanitize=self.sanitize_log
                                            )
                 _returned_headers = returned["headers"]
                 if stateful:
                     self.token_status = returned["status_code"]
                     if self.token_status == 201:
                         # Token generation was successful.
-                        self._token = BearerToken(token_value=returned["body"]["access_token"],
-                                                  expiration=returned["body"]["expires_in"],
-                                                  status=201
-                                                  )
+                        self.bearer_token = BearerToken(token_value=returned["body"]["access_token"],
+                                                        expiration=returned["body"]["expires_in"],
+                                                        status=201
+                                                        )
                         # Cloud Region auto discovery.
                         self.base_url = autodiscover_region(self.base_url, returned)
                     else:
                         # Token generation failure, reset the current token and check for an error response.
-                        self._token = BearerToken(status=returned["status_code"])
+                        self.bearer_token = BearerToken(status=returned["status_code"])
                         # Retrieve the list of errors, there should only be one item in the list.
                         error_list = returned["body"].get("errors", [])
                         if error_list:
                             self.bearer_token.fail_token(returned["status_code"],
                                                          error_list[0]["message"]
                                                          )
             else:
@@ -229,39 +244,40 @@
         except InvalidCredentials as bad_creds:
             returned = bad_creds.result
             if self.log:
                 self.log.error(bad_creds.message)
 
         return returned
 
-    def _logout_handler(self, token_value: str = None, stateful: bool = True) -> dict:
+    def _logout_handler(self, token_value: str = None, stateful: bool = True, client_id: str = None) -> dict:
         """Log out by revoking the current token.
 
         This method can also be leveraged to revoke other tokens.
         """
         try:
             if self.cred_format_valid:
                 if not token_value:
                     token_value = self.token_value
                 operation, target_url, data_payload, header_payload = logout_payloads(
                     creds=self.creds,
                     base=self.base_url,
-                    token_val=token_value
+                    token_val=token_value,
+                    client_id=client_id
                     )
                 # Log the call to this operation if debugging is enabled.
                 if self.log:
                     self.log.debug("OPERATION: %s", operation)
                 returned = perform_request(method="POST", endpoint=target_url, data=data_payload,
                                            headers=header_payload, verify=self.ssl_verify,
                                            proxy=self.proxy, timeout=self.timeout,
                                            user_agent=self.user_agent, log_util=self.log,
                                            sanitize=self.sanitize_log
                                            )
                 if stateful:
-                    self._token: BearerToken = BearerToken()
+                    self.bearer_token: BearerToken = BearerToken()
             else:
                 raise InvalidCredentials
         except InvalidCredentials as bad_creds:
             returned = bad_creds.result
             if self.log:
                 self.log.error(bad_creds.message)
 
@@ -357,14 +373,19 @@
 
     # These properties provide reflection into the token object
     @property
     def bearer_token(self) -> BearerToken:
         """Return the bearer token object for this configuration."""
         return self._token
 
+    @bearer_token.setter
+    def bearer_token(self, value: BearerToken):
+        """Set the bearer token."""
+        self._token = value
+
     @property
     def renew_window(self) -> int:
         """Return the current token renew window setting."""
         return self.bearer_token.renew_window
 
     @renew_window.setter
     def renew_window(self, value: int):
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/_interface_config.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_interface_config.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_auth_object/_uber_interface.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_uber_interface.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_constant/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_constant/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,31 +32,32 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 from typing import List
-from .._version import _TITLE, _VERSION
+from .._version import version
 PREFER_NONETYPE: List[str] = [
     "report_executions_download_get", "report_executions_download.get",
     "RTR_ListFiles", "RTR_ListFilesV2", "RTR_GetExtractedFileContents",
     "RTR_DeleteSession"
 ]
 PREFER_IDS_IN_BODY: List[str] = [
     "GetDeviceDetails", "PostDeviceDetailsV2", "GetVulnerabilities", "GetIntelIndicatorEntities",
-    "getChildrenV2", "cancel-scans", "GetDetectSummaries"
+    "getChildrenV2", "cancel-scans", "GetDetectSummaries", "UpdateQuarantinedDetectsByIds",
+    "GetQuarantineFiles"
 ]
 MOCK_OPERATIONS: List[str] = [
     "GetImageAssessmentReport", "DeleteImageDetails", "ImageMatchesPolicy"
 ]
 # Restrict requests to only allowed HTTP methods
 ALLOWED_METHODS: List[str] = ['GET', 'POST', 'PUT', 'PATCH', 'DELETE', 'UPDATE']
 # Default user-agent string
-USER_AGENT: str = f"{_TITLE}/{str(_VERSION)}"
+USER_AGENT: str = version(agent_string=True)
 # Default maximum number of records to write to debug logs (when active)
 MAX_DEBUG_RECORDS: int = 100
 # Global maximum number of records returned from any endpoint across all service collections
 GLOBAL_API_MAX_RETURN: int = 5000
 # Largest available token renew window (in seconds).
 MAX_TOKEN_RENEW_WINDOW: int = 1200
 # Minimum available token renew window (in seconds).
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,26 +17,29 @@
                                                         |.  __) |___._|__|____|_____|__|__|.  ____|___  |
                                                         |:  |                             |:  |   |_____|
                                                         |::.|     CrowdStrike Falcon      |::.|
                                                         `---' OAuth2 API SDK for Python 3 `---'
 """
 from typing import List, Any
 from .deprecated import _custom_ioa_deprecated
+from .deprecated import _d4c_registration_deprecated
 from .deprecated import _discover_deprecated
+from .deprecated import _fdr_deprecated
 from .deprecated import _firewall_management_deprecated
 from .deprecated import _hosts_deprecated
 from .deprecated import _identity_protection_deprecated
 from .deprecated import _installation_tokens_deprecated
 from .deprecated import _ioc_deprecated
 from .deprecated import _iocs_deprecated
 from .deprecated import _ods_deprecated
 from .deprecated import _real_time_response_deprecated
 from .deprecated import _real_time_response_admin_deprecated
 from .deprecated import _report_executions_deprecated
 from .deprecated import _scheduled_reports_deprecated
+from .deprecated import _zero_trust_assessment_deprecated
 
 from ._alerts import _alerts_endpoints
 from ._cloud_connect_aws import _cloud_connect_aws_endpoints
 from ._cspm_registration import _cspm_registration_endpoints
 from ._custom_ioa import _custom_ioa_endpoints
 from ._d4c_registration import _d4c_registration_endpoints
 from ._detects import _detects_endpoints
@@ -138,22 +141,25 @@
 api_endpoints.extend(_tailored_intelligence_endpoints)
 api_endpoints.extend(_user_management_endpoints)
 api_endpoints.extend(_zero_trust_assessment_endpoints)
 
 # Deprecated endpoints
 deprecated_endpoints = []
 deprecated_endpoints.extend(_custom_ioa_deprecated)
+deprecated_endpoints.extend(_d4c_registration_deprecated)
 deprecated_endpoints.extend(_discover_deprecated)
+deprecated_endpoints.extend(_fdr_deprecated)
 deprecated_endpoints.extend(_firewall_management_deprecated)
 deprecated_endpoints.extend(_hosts_deprecated)
 deprecated_endpoints.extend(_identity_protection_deprecated)
 deprecated_endpoints.extend(_installation_tokens_deprecated)
 deprecated_endpoints.extend(_ioc_deprecated)
 deprecated_endpoints.extend(_iocs_deprecated)
 deprecated_endpoints.extend(_ods_deprecated)
 deprecated_endpoints.extend(_real_time_response_deprecated)
 deprecated_endpoints.extend(_real_time_response_admin_deprecated)
 deprecated_endpoints.extend(_report_executions_deprecated)
 deprecated_endpoints.extend(_scheduled_reports_deprecated)
+deprecated_endpoints.extend(_zero_trust_assessment_deprecated)
 
 # api_endpoints contains all endpoints, production and deprecated
 api_endpoints.extend(deprecated_endpoints)
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_alerts.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_cloud_connect_aws.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_cloud_connect_aws.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,19 +42,19 @@
     "GET",
     "/cloud-connect-aws/combined/accounts/v1",
     "Search for provisioned AWS Accounts by providing an FQL filter and paging details. "
     "Returns a set of AWS accounts which match the filter criteria",
     "cloud_connect_aws",
     [
       {
-        "maxLength": 500,
+        "maxLength": 1000,
         "minLength": 1,
         "type": "integer",
         "default": 100,
-        "description": "The maximum records to return. [1-500]. Defaults to 100.",
+        "description": "The maximum records to return. [1-1000]. Defaults to 100.",
         "name": "limit",
         "in": "query"
       },
       {
         "type": "integer",
         "description": "The offset to start retrieving records from",
         "name": "offset",
@@ -89,15 +89,14 @@
     "Retrieve a set of AWS Accounts by specifying their IDs",
     "cloud_connect_aws",
     [
       {
         "maxItems": 5000,
         "type": "array",
         "items": {
-          "pattern": "\\d{12}",
           "type": "string"
         },
         "collectionFormat": "multi",
         "description": "IDs of accounts to retrieve details",
         "name": "ids",
         "in": "query",
         "required": True
@@ -150,16 +149,14 @@
     "/cloud-connect-aws/entities/accounts/v1",
     "Delete a set of AWS Accounts by specifying their IDs",
     "cloud_connect_aws",
     [
       {
         "type": "array",
         "items": {
-          "maxLength": 12,
-          "minLength": 12,
           "type": "string"
         },
         "collectionFormat": "multi",
         "description": "IDs of accounts to remove",
         "name": "ids",
         "in": "query",
         "required": True
@@ -186,16 +183,14 @@
     "/cloud-connect-aws/entities/verify-account-access/v1",
     "Performs an Access Verification check on the specified AWS Account IDs",
     "cloud_connect_aws",
     [
       {
         "type": "array",
         "items": {
-          "maxLength": 12,
-          "minLength": 12,
           "type": "string"
         },
         "collectionFormat": "multi",
         "description": "IDs of accounts to verify access on",
         "name": "ids",
         "in": "query",
         "required": True
@@ -207,19 +202,19 @@
     "GET",
     "/cloud-connect-aws/queries/accounts/v1",
     "Search for provisioned AWS Accounts by providing an FQL filter and paging details. "
     "Returns a set of AWS account IDs which match the filter criteria",
     "cloud_connect_aws",
     [
       {
-        "maxLength": 500,
+        "maxLength": 1000,
         "minLength": 1,
         "type": "integer",
         "default": 100,
-        "description": "The maximum records to return. [1-500]. Defaults to 100.",
+        "description": "The maximum records to return. [1-1000]. Defaults to 100.",
         "name": "limit",
         "in": "query"
       },
       {
         "type": "integer",
         "description": "The offset to start retrieving records from",
         "name": "offset",
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_cspm_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_cspm_registration.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
+# pylint: disable=C0302
 
 _cspm_registration_endpoints = [
   [
     "GetCSPMAwsAccount",
     "GET",
     "/cloud-connect-cspm-aws/entities/account/v1",
     "Returns information about the current status of an AWS account.",
@@ -52,26 +53,34 @@
         "description": "Type of scan, dry or full, to perform on selected accounts",
         "name": "scan-type",
         "in": "query"
       },
       {
         "type": "array",
         "items": {
-          "pattern": "\\d{12}",
           "type": "string"
         },
         "collectionFormat": "multi",
         "description": "AWS account IDs",
         "name": "ids",
         "in": "query"
       },
       {
         "type": "array",
         "items": {
-          "pattern": "^o-[0-9a-z]{10,32}$",
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "AWS IAM role ARNs",
+        "name": "iam_role_arns",
+        "in": "query"
+      },
+      {
+        "type": "array",
+        "items": {
           "type": "string"
         },
         "collectionFormat": "multi",
         "description": "AWS organization IDs",
         "name": "organization-ids",
         "in": "query"
       },
@@ -88,14 +97,25 @@
         "type": "integer",
         "default": 100,
         "description": "The maximum records to return. Defaults to 100.",
         "name": "limit",
         "in": "query"
       },
       {
+        "pattern": "^(true|false)$",
+        "enum": [
+          "false",
+          "true"
+        ],
+        "type": "string",
+        "description": "Only return migrated d4c accounts",
+        "name": "migrated",
+        "in": "query"
+      },
+      {
         "type": "integer",
         "description": "The offset to start retrieving records from",
         "name": "offset",
         "in": "query"
       },
       {
         "enum": [
@@ -171,24 +191,63 @@
   ],
   [
     "GetCSPMAwsConsoleSetupURLs",
     "GET",
     "/cloud-connect-cspm-aws/entities/console-setup-urls/v1",
     "Return a URL for customer to visit in their cloud environment to grant us access to their AWS environment.",
     "cspm_registration",
-    []
+    [
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "AWS account IDs",
+        "name": "ids",
+        "in": "query"
+      },
+      {
+        "pattern": "^(true|false)$",
+        "enum": [
+          "false",
+          "true"
+        ],
+        "type": "string",
+        "name": "use_existing_cloudtrail",
+        "in": "query"
+      },
+      {
+        "pattern": "^[0-9a-z-]{2,}$",
+        "type": "string",
+        "description": "Region",
+        "name": "region",
+        "in": "query"
+      }
+    ]
   ],
   [
     "GetCSPMAwsAccountScriptsAttachment",
     "GET",
     "/cloud-connect-cspm-aws/entities/user-scripts-download/v1",
     "Return a script for customer to run in their cloud environment to grant us "
     "access to their AWS environment as a downloadable attachment.",
     "cspm_registration",
-    []
+    [
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "AWS account IDs",
+        "name": "ids",
+        "in": "query"
+      }
+    ]
   ],
   [
     "GetCSPMAzureAccount",
     "GET",
     "/cloud-connect-cspm-azure/entities/account/v1",
     "Return information about Azure account registration",
     "cspm_registration",
@@ -204,14 +263,24 @@
         "collectionFormat": "multi",
         "description": "SubscriptionIDs of accounts to select for this status operation. "
         "If this is empty then all accounts are returned.",
         "name": "ids",
         "in": "query"
       },
       {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "Tenant ids to filter azure accounts",
+        "name": "tenant_ids",
+        "in": "query"
+      },
+      {
         "maxLength": 4,
         "minLength": 3,
         "pattern": "^(full|dry)$",
         "type": "string",
         "description": "Type of scan, dry or full, to perform on selected accounts",
         "name": "scan-type",
         "in": "query"
@@ -261,24 +330,38 @@
     "/cloud-connect-cspm-azure/entities/account/v1",
     "Deletes an Azure subscription from the system.",
     "cspm_registration",
     [
       {
         "type": "array",
         "items": {
-          "maxLength": 36,
-          "minLength": 36,
-          "pattern": "^[0-9a-z-]{36}$",
           "type": "string"
         },
         "collectionFormat": "multi",
         "description": "Azure subscription IDs to remove",
         "name": "ids",
-        "in": "query",
-        "required": True
+        "in": "query"
+      },
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "Tenant ids to remove",
+        "name": "tenant_ids",
+        "in": "query"
+      },
+      {
+        "maxLength": 5,
+        "minLength": 4,
+        "pattern": "^(true|false)$",
+        "type": "string",
+        "name": "retain_tenant",
+        "in": "query"
       }
     ]
   ],
   [
     "UpdateCSPMAzureAccountClientID",
     "PATCH",
     "/cloud-connect-cspm-azure/entities/client-id/v1",
@@ -300,20 +383,14 @@
         "maxLength": 36,
         "minLength": 36,
         "pattern": "^[0-9a-z-]{36}$",
         "type": "string",
         "description": "Tenant ID to update client ID for. Required if multiple tenants are registered.",
         "name": "tenant-id",
         "in": "query"
-      },
-      {
-        "description": "This is a placeholder only. Please ignore this field.",
-        "name": "body",
-        "in": "body",
-        "required": True
       }
     ]
   ],
   [
     "UpdateCSPMAzureTenantDefaultSubscriptionID",
     "PATCH",
     "/cloud-connect-cspm-azure/entities/default-subscription-id/v1",
@@ -347,37 +424,37 @@
     "/cloud-connect-cspm-azure/entities/download-certificate/v1",
     "Returns JSON object(s) that contain the base64 encoded certificate for a service principal.",
     "cspm_registration",
     [
       {
         "type": "array",
         "items": {
-          "maxLength": 36,
-          "minLength": 36,
-          "pattern": "^[0-9a-z-]{36}$",
           "type": "string"
         },
         "collectionFormat": "multi",
         "description": "Azure Tenant ID",
         "name": "tenant_id",
         "in": "query",
         "required": True
       },
       {
-        "maxLength": 5,
-        "minLength": 4,
-        "pattern": "^(true|false)$",
-        "enum": [
-          "false",
-          "true"
-        ],
-        "type": "string",
+        "type": "boolean",
         "default": False,
+        "description": "Setting to true will invalidate the current certificate and generate a new certificate",
         "name": "refresh",
         "in": "query"
+      },
+      {
+        "maxLength": 2,
+        "minLength": 1,
+        "pattern": "^[0-9]{1,2}$",
+        "type": "string",
+        "description": "Years the certificate should be valid (only used when refresh=true)",
+        "name": "years_valid",
+        "in": "query"
       }
     ]
   ],
   [
     "GetCSPMAzureUserScriptsAttachment",
     "GET",
     "/cloud-connect-cspm-azure/entities/user-scripts-download/v1",
@@ -389,14 +466,40 @@
         "maxLength": 36,
         "minLength": 36,
         "pattern": "^[0-9a-z-]{36}$",
         "type": "string",
         "description": "Tenant ID to generate script for. Defaults to most recently registered tenant.",
         "name": "tenant-id",
         "in": "query"
+      },
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "Subscription IDs to generate script for. Defaults to all.",
+        "name": "subscription_ids",
+        "in": "query"
+      },
+      {
+        "pattern": "^(commercial|gov)$",
+        "enum": [
+          "commercial",
+          "gov"
+        ],
+        "type": "string",
+        "name": "account_type",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "Template to be rendered",
+        "name": "template",
+        "in": "query"
       }
     ]
   ],
   [
     "GetBehaviorDetections",
     "GET",
     "/detects/entities/ioa/v1",
@@ -408,16 +511,15 @@
         "enum": [
           "aws",
           "azure"
         ],
         "type": "string",
         "description": "Cloud Provider (e.g.: aws|azure)",
         "name": "cloud_provider",
-        "in": "query",
-        "required": True
+        "in": "query"
       },
       {
         "enum": [
           "ACM",
           "ACR",
           "Any",
           "App Engine",
@@ -514,21 +616,29 @@
       {
         "type": "string",
         "description": "Filter to get all events after this date, in format RFC3339 : e.g. 2006-01-02T15:04:05Z07:00",
         "name": "date_time_since",
         "in": "query"
       },
       {
+        "type": "string",
+        "default": "24h",
+        "description": "Filter events using a duration string (e.g. 24h)",
+        "name": "since",
+        "in": "query"
+      },
+      {
         "enum": [
+          "Critical",
           "High",
           "Informational",
           "Medium"
         ],
         "type": "string",
-        "description": "Severity (e.g.: High | Medium | Informational)",
+        "description": "Policy Severity",
         "name": "severity",
         "in": "query"
       },
       {
         "type": "string",
         "description": "String to get next page of results, is associated with a previous execution "
         "of GetBehaviorDetections. Must include all filters from previous execution.",
@@ -537,14 +647,34 @@
       },
       {
         "pattern": "^\\d+$",
         "type": "integer",
         "description": "The maximum records to return. [1-500]",
         "name": "limit",
         "in": "query"
+      },
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "Resource ID",
+        "name": "resource_id",
+        "in": "query"
+      },
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "Resource UUID",
+        "name": "resource_uuid",
+        "in": "query"
       }
     ]
   ],
   [
     "GetConfigurationDetections",
     "GET",
     "/detects/entities/iom/v1",
@@ -684,14 +814,76 @@
         "description": "The maximum records to return. [1-500]",
         "name": "limit",
         "in": "query"
       }
     ]
   ],
   [
+    "GetConfigurationDetectionEntities",
+    "GET",
+    "/detects/entities/iom/v2",
+    "Get misconfigurations based on the ID - including custom policy detections in addition to default policy detections.",
+    "cspm_registration",
+    [
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "detection ids",
+        "name": "ids",
+        "in": "query",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "GetConfigurationDetectionIDsV2",
+    "GET",
+    "/detects/queries/iom/v2",
+    "Get list of active misconfiguration ids - including custom policy detections in addition to default policy detections.",
+    "cspm_registration",
+    [
+      {
+        "type": "string",
+        "description": "use_current_scan_ids - *use this to get records for latest scans*\naccount_name\naccount_id\n"
+        "agent_id\nattack_types\nazure_subscription_id\ncloud_provider\ncloud_service_keyword\ncustom_policy_id\n"
+        "is_managed\npolicy_id\npolicy_type\nresource_id\nregion\nstatus\nscan_time\nseverity\nseverity_string\n",
+        "name": "filter",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "default": "timestamp|desc",
+        "description": "account_name\naccount_id\nattack_types\nazure_subscription_id\ncloud_provider\n"
+        "cloud_service_keyword\nstatus\nis_managed\npolicy_id\npolicy_type\nresource_id\nregion\nscan_time\n"
+        "severity\nseverity_string\ntimestamp",
+        "name": "sort",
+        "in": "query"
+      },
+      {
+        "maximum": 1000,
+        "minimum": 0,
+        "type": "integer",
+        "default": 500,
+        "description": "The max number of detections to return",
+        "name": "limit",
+        "in": "query"
+      },
+      {
+        "minimum": 0,
+        "type": "integer",
+        "description": "Offset returned detections",
+        "name": "offset",
+        "in": "query"
+      }
+    ]
+  ],
+  [
     "GetIOAEvents",
     "GET",
     "/ioa/entities/events/v1",
     "For CSPM IOA events, gets list of IOA events.",
     "cspm_registration",
     [
       {
@@ -833,14 +1025,34 @@
         "name": "ids",
         "in": "query",
         "required": True
       }
     ]
   ],
   [
+    "GetCSPMPoliciesDetails",
+    "GET",
+    "/settings/entities/policy-details/v2",
+    "Given an array of policy IDs, returns detailed policies information.",
+    "cspm_registration",
+    [
+      {
+        "type": "array",
+        "items": {
+          "type": "integer"
+        },
+        "collectionFormat": "multi",
+        "description": "Policy IDs",
+        "name": "ids",
+        "in": "query",
+        "required": True
+      }
+    ]
+  ],
+  [
     "GetCSPMPolicySettings",
     "GET",
     "/settings/entities/policy/v1",
     "Returns information about current policy settings.",
     "cspm_registration",
     [
       {
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_custom_ioa.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_d4c_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_discover.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,393 +32,322 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
-_d4c_registration_endpoints = [
+_discover_endpoints = [
   [
-    "GetD4CAwsAccount",
+    "get_accounts",
     "GET",
-    "/cloud-connect-aws/entities/account/v2",
-    "Returns information about the current status of an AWS account.",
-    "d4c_registration",
+    "/discover/entities/accounts/v1",
+    "Get details on accounts by providing one or more IDs.",
+    "discover",
     [
       {
-        "maxLength": 4,
-        "minLength": 3,
-        "pattern": "^(full|dry)$",
-        "type": "string",
-        "description": "Type of scan, dry or full, to perform on selected accounts",
-        "name": "scan-type",
-        "in": "query"
-      },
-      {
         "type": "array",
         "items": {
           "type": "string"
         },
         "collectionFormat": "multi",
-        "description": "AWS account IDs",
+        "description": "One or more account IDs (max: 100). Find account IDs with GET `/discover/queries/accounts/v1`",
         "name": "ids",
-        "in": "query"
-      },
-      {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "multi",
-        "description": "AWS organization IDs",
-        "name": "organization-ids",
-        "in": "query"
-      },
-      {
-        "pattern": "^(provisioned|operational)$",
-        "type": "string",
-        "description": "Account status to filter results by.",
-        "name": "status",
-        "in": "query"
-      },
-      {
-        "maxLength": 3,
-        "minLength": 1,
-        "type": "integer",
-        "default": 100,
-        "description": "The maximum records to return. Defaults to 100.",
-        "name": "limit",
-        "in": "query"
-      },
-      {
-        "type": "integer",
-        "description": "The offset to start retrieving records from",
-        "name": "offset",
-        "in": "query"
-      },
-      {
-        "pattern": "^(true|false)$",
-        "enum": [
-          "false",
-          "true"
-        ],
-        "type": "string",
-        "description": "Only return migrated d4c accounts",
-        "name": "migrated",
-        "in": "query"
-      }
-    ]
-  ],
-  [
-    "CreateD4CAwsAccount",
-    "POST",
-    "/cloud-connect-aws/entities/account/v2",
-    "Creates a new account in our system for a customer and generates a script "
-    "for them to run in their AWS cloud environment to grant us access.",
-    "d4c_registration",
-    [
-      {
-        "name": "body",
-        "in": "body",
+        "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "DeleteD4CAwsAccount",
-    "DELETE",
-    "/cloud-connect-aws/entities/account/v2",
-    "Deletes an existing AWS account or organization in our system.",
-    "d4c_registration",
+    "get_applications",
+    "GET",
+    "/discover/entities/applications/v1",
+    "Get details on applications by providing one or more IDs.",
+    "discover",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
         "collectionFormat": "multi",
-        "description": "AWS account IDs to remove",
+        "description": "The IDs of applications to retrieve. (Min: 1, Max: 100)",
         "name": "ids",
-        "in": "query"
-      },
-      {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "multi",
-        "description": "AWS organization IDs to remove",
-        "name": "organization-ids",
-        "in": "query"
+        "in": "query",
+        "required": True
       }
     ]
   ],
   [
-    "GetD4CAwsConsoleSetupURLs",
+    "get_hosts",
     "GET",
-    "/cloud-connect-aws/entities/console-setup-urls/v1",
-    "Return a URL for customer to visit in their cloud environment to grant "
-    "us access to their AWS environment.",
-    "d4c_registration",
+    "/discover/entities/hosts/v1",
+    "Get details on assets by providing one or more IDs.",
+    "discover",
     [
       {
-        "pattern": "^[0-9a-z-]{2,}$",
-        "type": "string",
-        "description": "Region",
-        "name": "region",
-        "in": "query"
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "One or more asset IDs (max: 100). Find asset IDs with GET `/discover/queries/hosts/v1`",
+        "name": "ids",
+        "in": "query",
+        "required": True
       }
     ]
   ],
   [
-    "GetD4CAWSAccountScriptsAttachment",
+    "get_logins",
     "GET",
-    "/cloud-connect-aws/entities/user-scripts-download/v1",
-    "Return a script for customer to run in their cloud environment to grant "
-    "us access to their AWS environment as a downloadable attachment.",
-    "d4c_registration",
+    "/discover/entities/logins/v1",
+    "Get details on logins by providing one or more IDs.",
+    "discover",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
         "collectionFormat": "multi",
-        "description": "AWS account IDs",
+        "description": "One or more login IDs (max: 100). Find login IDs with GET `/discover/queries/logins/v1`",
         "name": "ids",
-        "in": "query"
+        "in": "query",
+        "required": True
       }
     ]
   ],
   [
-    "GetCSPMAzureAccount",
+    "query_accounts",
     "GET",
-    "/cloud-connect-azure/entities/account/v1",
-    "Return information about Azure account registration",
-    "d4c_registration",
+    "/discover/queries/accounts/v1",
+    "Search for accounts in your environment by providing an FQL (Falcon Query Language) filter and paging details. "
+    "Returns a set of account IDs which match the filter criteria.",
+    "discover",
     [
       {
-        "type": "array",
-        "items": {
-          "maxLength": 36,
-          "minLength": 36,
-          "pattern": "^[0-9a-z-]{36}$",
-          "type": "string"
-        },
-        "collectionFormat": "multi",
-        "description": "SubscriptionIDs of accounts to select for this status operation. "
-        "If this is empty then all accounts are returned.",
-        "name": "ids",
+        "minimum": 0,
+        "type": "integer",
+        "description": "An offset used with the `limit` parameter to manage pagination of results. "
+        "On your first request, don’t provide an `offset`. On subsequent requests, provide the `offset` "
+        "from the previous response to continue from that place in the results.",
+        "name": "offset",
+        "in": "query"
+      },
+      {
+        "maximum": 100,
+        "minimum": 1,
+        "type": "integer",
+        "description": "The number of account IDs to return in this response (min: 1, max: 100, default: 100). "
+        "Use with the `offset` parameter to manage pagination of results.",
+        "name": "limit",
         "in": "query"
       },
       {
-        "maxLength": 4,
-        "minLength": 3,
-        "pattern": "^(full|dry)$",
         "type": "string",
-        "description": "Type of scan, dry or full, to perform on selected accounts",
-        "name": "scan-type",
+        "description": "Sort accounts by their properties. A single sort field is allowed. "
+        "Common sort options include:\n\n<ul><li>username|asc</li><li>last_failed_login_timestamp|desc</li></ul>",
+        "name": "sort",
         "in": "query"
-      }
-    ]
-  ],
-  [
-    "CreateCSPMAzureAccount",
-    "POST",
-    "/cloud-connect-azure/entities/account/v1",
-    "Creates a new account in our system for a customer and generates a script for them to run "
-    "in their cloud environment to grant us access.",
-    "d4c_registration",
-    [
+      },
       {
-        "name": "body",
-        "in": "body",
-        "required": True
+        "type": "string",
+        "description": "Filter accounts using an FQL query. Common filter options include:\n\n<ul>"
+        "<li>account_type:'Local'</li><li>admin_privileges:'Yes'</li><li>first_seen_timestamp:<'now-7d'</li>"
+        "<li>last_successful_login_type:'Terminal server'</li></ul>",
+        "name": "filter",
+        "in": "query"
       }
     ]
   ],
   [
-    "UpdateCSPMAzureAccountClientID",
-    "PATCH",
-    "/cloud-connect-azure/entities/client-id/v1",
-    "Update an Azure service account in our system by with the user-created client_id "
-    "created with the public key we've provided",
-    "d4c_registration",
+    "query_applications",
+    "GET",
+    "/discover/queries/applications/v1",
+    "Search for applications in your environment by providing an FQL filter and paging details. "
+    "returns a set of application IDs which match the filter criteria.",
+    "discover",
     [
       {
-        "maxLength": 36,
-        "minLength": 36,
-        "pattern": "^[0-9a-z-]{36}$",
+        "minimum": 0,
+        "type": "integer",
+        "description": "The index of the starting resource.",
+        "name": "offset",
+        "in": "query"
+      },
+      {
+        "maximum": 100,
+        "minimum": 1,
+        "type": "integer",
+        "description": "The number of account IDs to return in this response (min: 1, max: 100, default: 100). "
+        "Use with the `offset` parameter to manage pagination of results.",
+        "name": "limit",
+        "in": "query"
+      },
+      {
         "type": "string",
-        "description": "ClientID to use for the Service Principal associated with the customer's Azure account",
-        "name": "id",
-        "in": "query",
-        "required": True
+        "description": "Sort accounts by their properties. A single sort field is allowed. "
+        "Common sort options include:\n\n<ul><li>username|asc</li><li>last_failed_login_timestamp|desc</li></ul>",
+        "name": "sort",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "Filter accounts using an FQL query. "
+        "Common filter options include:\n\n<ul><li>account_type:'Local'</li><li>admin_privileges:'Yes'</li>"
+        "<li>first_seen_timestamp:<'now-7d'</li><li>last_successful_login_type:'Terminal server'</li></ul>",
+        "name": "filter",
+        "in": "query"
       }
     ]
   ],
   [
-    "DiscoverCloudAzureDownloadCertificate",
+    "query_hosts",
     "GET",
-    "/cloud-connect-azure/entities/download-certificate/v1",
-    "Returns JSON object(s) that contain the base64 encoded certificate for a service principal.",
-    "d4c_registration",
+    "/discover/queries/hosts/v1",
+    "Search for assets in your environment by providing an FQL (Falcon Query Language) filter and paging details. "
+    "Returns a set of asset IDs which match the filter criteria.",
+    "discover",
     [
       {
-        "type": "array",
-        "items": {
-          "maxLength": 36,
-          "minLength": 36,
-          "pattern": "^[0-9a-z-]{36}$",
-          "type": "string"
-        },
-        "collectionFormat": "multi",
-        "description": "Azure Tenant ID",
-        "name": "tenant_id",
-        "in": "query",
-        "required": True
+        "minimum": 0,
+        "type": "integer",
+        "description": "An offset used with the `limit` parameter to manage pagination of results. "
+        "On your first request, don’t provide an `offset`. On subsequent requests, provide the `offset` "
+        "from the previous response to continue from that place in the results.",
+        "name": "offset",
+        "in": "query"
+      },
+      {
+        "maximum": 100,
+        "minimum": 1,
+        "type": "integer",
+        "description": "The number of asset IDs to return in this response (min: 1, max: 100, default: 100). "
+        "Use with the `offset` parameter to manage pagination of results.",
+        "name": "limit",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "Sort assets by their properties. A single sort field is allowed. "
+        "Common sort options include:\n\n<ul><li>hostname|asc</li><li>product_type_desc|desc</li></ul>",
+        "name": "sort",
+        "in": "query"
       },
       {
-        "maxLength": 5,
-        "minLength": 4,
-        "pattern": "^(true|false)$",
-        "enum": [
-          "false",
-          "true"
-        ],
         "type": "string",
-        "default": False,
-        "name": "refresh",
+        "description": "Filter assets using an FQL query. Common filter options include:\n\n"
+        "<ul><li>entity_type:'managed'</li><li>product_type_desc:'Workstation'</li><li>platform_name:'Windows'</li>"
+        "<li>last_seen_timestamp:>'now-7d'</li></ul>",
+        "name": "filter",
         "in": "query"
       }
     ]
   ],
   [
-    "GetCSPMAzureUserScriptsAttachment",
-    "GET",
-    "/cloud-connect-azure/entities/user-scripts-download/v1",
-    "Return a script for customer to run in their cloud environment to grant us access to their "
-    "Azure environment as a downloadable attachment",
-    "d4c_registration",
-    []
-  ],
-  [
-    "GetCSPMAzureUserScripts",
-    "GET",
-    "/cloud-connect-azure/entities/user-scripts/v1",
-    "Return a script for customer to run in their cloud environment to grant us access to their "
-    "Azure environment",
-    "d4c_registration",
-    []
-  ],
-  [
-    "GetCSPMCGPAccount",
+    "query_logins",
     "GET",
-    "/cloud-connect-gcp/entities/account/v1",
-    "Returns information about the current status of an GCP account.",
-    "d4c_registration",
+    "/discover/queries/logins/v1",
+    "Search for logins in your environment by providing an FQL (Falcon Query Language) filter and paging details. "
+    "Returns a set of login IDs which match the filter criteria.",
+    "discover",
     [
       {
-        "maxLength": 4,
-        "minLength": 3,
-        "pattern": "^(full|dry)$",
+        "minimum": 0,
+        "type": "integer",
+        "description": "An offset used with the `limit` parameter to manage pagination of results. "
+        "On your first request, don’t provide an `offset`. On subsequent requests, provide the `offset` "
+        "from the previous response to continue from that place in the results.",
+        "name": "offset",
+        "in": "query"
+      },
+      {
+        "maximum": 100,
+        "minimum": 1,
+        "type": "integer",
+        "description": "The number of asset IDs to return in this response (min: 1, max: 100, default: 100). "
+        "Use with the `offset` parameter to manage pagination of results.",
+        "name": "limit",
+        "in": "query"
+      },
+      {
         "type": "string",
-        "description": "Type of scan, dry or full, to perform on selected accounts",
-        "name": "scan-type",
+        "description": "Sort assets by their properties. A single sort field is allowed. "
+        "Common sort options include:\n\n<ul><li>hostname|asc</li><li>product_type_desc|desc</li></ul>",
+        "name": "sort",
         "in": "query"
       },
       {
-        "type": "array",
-        "items": {
-          "pattern": "\\d{10,}",
-          "type": "string"
-        },
-        "collectionFormat": "multi",
-        "description": "Parent IDs of accounts",
-        "name": "ids",
+        "type": "string",
+        "description": "Filter assets using an FQL query. Common filter options include:\n\n"
+        "<ul><li>entity_type:'managed'</li><li>product_type_desc:'Workstation'</li><li>platform_name:'Windows'</li>"
+        "<li>last_seen_timestamp:>'now-7d'</li></ul>",
+        "name": "filter",
         "in": "query"
       }
     ]
   ],
   [
-    "CreateCSPMGCPAccount",
-    "POST",
-    "/cloud-connect-gcp/entities/account/v1",
-    "Creates a new account in our system for a customer and generates a new service account for them "
-    "to add access to in their GCP environment to grant us access.",
-    "d4c_registration",
+    "get_iot_hosts",
+    "GET",
+    "/discover/entities/iot-hosts/v1",
+    "Get details on IoT assets by providing one or more IDs.",
+    "discover_iot",
     [
       {
-        "name": "body",
-        "in": "body",
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "One or more asset IDs (max: 100). Find asset IDs with GET `/discover/queries/iot-hosts/v1`",
+        "name": "ids",
+        "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "GetCSPMGCPUserScriptsAttachment",
-    "GET",
-    "/cloud-connect-gcp/entities/user-scripts-download/v1",
-    "Return a script for customer to run in their cloud environment to grant us access to their "
-    "GCP environment as a downloadable attachment",
-    "d4c_registration",
-    []
-  ],
-  [
-    "GetCSPMGCPUserScripts",
+    "query_iot_hosts",
     "GET",
-    "/cloud-connect-gcp/entities/user-scripts/v1",
-    "Return a script for customer to run in their cloud environment to grant us access to their "
-    "GCP environment",
-    "d4c_registration",
-    []
-  ],
-  [
-    "GetHorizonD4CScripts",
-    "GET",
-    "/settings-discover/entities/gen/scripts/v1",
-    "Returns static install scripts for Horizon.",
-    "d4c_registration",
+    "/discover/queries/iot-hosts/v1",
+    "Search for IoT assets in your environment by providing an FQL (Falcon Query Language) filter and paging details. "
+    "Returns a set of asset IDs which match the filter criteria.",
+    "discover_iot",
     [
       {
-        "pattern": "^(true|false)$",
-        "enum": [
-          "false",
-          "true"
-        ],
-        "type": "string",
-        "description": "Get static script for single account",
-        "name": "single_account",
+        "minimum": 0,
+        "type": "integer",
+        "description": "An offset used with the `limit` parameter to manage pagination of results. On your first request, "
+        "don’t provide an `offset`. On subsequent requests, provide the `offset` from the previous response to continue "
+        "from that place in the results.",
+        "name": "offset",
         "in": "query"
       },
       {
-        "pattern": "^o-[0-9a-z]{10,32}$",
-        "type": "string",
-        "description": "AWS organization ID",
-        "name": "organization-id",
+        "maximum": 100,
+        "minimum": 1,
+        "type": "integer",
+        "description": "The number of asset IDs to return in this response (min: 1, max: 100, default: 100). "
+        "Use with the `offset` parameter to manage pagination of results.",
+        "name": "limit",
         "in": "query"
       },
       {
-        "pattern": "^(true|false)$",
-        "enum": [
-          "false",
-          "true"
-        ],
         "type": "string",
-        "name": "delete",
+        "description": "Sort assets by their properties. A single sort field is allowed. "
+        "Common sort options include:\n\n<ul><li>hostname|asc</li><li>product_type_desc|desc</li></ul>",
+        "name": "sort",
         "in": "query"
       },
       {
-        "pattern": "^(commercial|gov)$",
-        "enum": [
-          "commercial",
-          "gov"
-        ],
         "type": "string",
-        "description": "Account type (e.g.: commercial,gov) Only applicable when "
-        "registering AWS commercial account in a Gov environment",
-        "name": "account_type",
+        "description": "Filter assets using an FQL query. Common filter options include:\n\n<ul>"
+        "<li>entity_type:'managed'</li><li>product_type_desc:'Workstation'</li>"
+        "<li>platform_name:'Windows'</li><li>last_seen_timestamp:>'now-7d'</li></ul>",
+        "name": "filter",
         "in": "query"
       }
     ]
   ]
 ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_detects.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_device_control_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_device_control_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,17 +163,19 @@
     "/policy/entities/device-control-actions/v1",
     "Perform the specified action on the Device Control Policies specified in the request",
     "device_control_policies",
     [
       {
         "enum": [
           "add-host-group",
+          "add-rule-group",
           "disable",
           "enable",
-          "remove-host-group"
+          "remove-host-group",
+          "remove-rule-group"
         ],
         "type": "string",
         "description": "The action to perform",
         "name": "action_name",
         "in": "query",
         "required": True
       },
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_discover.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_discover.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
 _discover_endpoints = [
   [
-    "get_accounts",
+    "get-accounts",
     "GET",
     "/discover/entities/accounts/v1",
     "Get details on accounts by providing one or more IDs.",
     "discover",
     [
       {
         "type": "array",
@@ -54,15 +54,15 @@
         "name": "ids",
         "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "get_applications",
+    "get-applications",
     "GET",
     "/discover/entities/applications/v1",
     "Get details on applications by providing one or more IDs.",
     "discover",
     [
       {
         "type": "array",
@@ -74,15 +74,15 @@
         "name": "ids",
         "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "get_hosts",
+    "get-hosts",
     "GET",
     "/discover/entities/hosts/v1",
     "Get details on assets by providing one or more IDs.",
     "discover",
     [
       {
         "type": "array",
@@ -94,15 +94,15 @@
         "name": "ids",
         "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "get_logins",
+    "get-logins",
     "GET",
     "/discover/entities/logins/v1",
     "Get details on logins by providing one or more IDs.",
     "discover",
     [
       {
         "type": "array",
@@ -114,58 +114,58 @@
         "name": "ids",
         "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "query_accounts",
+    "query-accounts",
     "GET",
     "/discover/queries/accounts/v1",
     "Search for accounts in your environment by providing an FQL (Falcon Query Language) filter and paging details. "
     "Returns a set of account IDs which match the filter criteria.",
     "discover",
     [
       {
         "minimum": 0,
         "type": "integer",
-        "description": "An offset used with the `limit` parameter to manage pagination of results. "
-        "On your first request, don’t provide an `offset`. On subsequent requests, provide the `offset` "
-        "from the previous response to continue from that place in the results.",
+        "description": "An offset used with the `limit` parameter to manage pagination of results. On your first request, "
+        "don’t provide an `offset`. On subsequent requests, provide the `offset` from the previous response to continue "
+        "from that place in the results.",
         "name": "offset",
         "in": "query"
       },
       {
         "maximum": 100,
         "minimum": 1,
         "type": "integer",
         "description": "The number of account IDs to return in this response (min: 1, max: 100, default: 100). "
         "Use with the `offset` parameter to manage pagination of results.",
         "name": "limit",
         "in": "query"
       },
       {
         "type": "string",
-        "description": "Sort accounts by their properties. A single sort field is allowed. "
-        "Common sort options include:\n\n<ul><li>username|asc</li><li>last_failed_login_timestamp|desc</li></ul>",
+        "description": "Sort accounts by their properties. A single sort field is allowed. Common sort options include:"
+        "\n\n<ul><li>username|asc</li><li>last_failed_login_timestamp|desc</li></ul>",
         "name": "sort",
         "in": "query"
       },
       {
         "type": "string",
-        "description": "Filter accounts using an FQL query. Common filter options include:\n\n<ul>"
-        "<li>account_type:'Local'</li><li>admin_privileges:'Yes'</li><li>first_seen_timestamp:<'now-7d'</li>"
+        "description": "Filter accounts using an FQL query. Common filter options include:\n\n<ul><li>"
+        "account_type:'Local'</li><li>admin_privileges:'Yes'</li><li>first_seen_timestamp:<'now-7d'</li>"
         "<li>last_successful_login_type:'Terminal server'</li></ul>",
         "name": "filter",
         "in": "query"
       }
     ]
   ],
   [
-    "query_applications",
+    "query-applications",
     "GET",
     "/discover/queries/applications/v1",
     "Search for applications in your environment by providing an FQL filter and paging details. "
     "returns a set of application IDs which match the filter criteria.",
     "discover",
     [
       {
@@ -189,24 +189,24 @@
         "description": "Sort accounts by their properties. A single sort field is allowed. "
         "Common sort options include:\n\n<ul><li>username|asc</li><li>last_failed_login_timestamp|desc</li></ul>",
         "name": "sort",
         "in": "query"
       },
       {
         "type": "string",
-        "description": "Filter accounts using an FQL query. "
-        "Common filter options include:\n\n<ul><li>account_type:'Local'</li><li>admin_privileges:'Yes'</li>"
-        "<li>first_seen_timestamp:<'now-7d'</li><li>last_successful_login_type:'Terminal server'</li></ul>",
+        "description": "Filter accounts using an FQL query. Common filter options include:\n\n"
+        "<ul><li>account_type:'Local'</li><li>admin_privileges:'Yes'</li><li>first_seen_timestamp:<'now-7d'</li>"
+        "<li>last_successful_login_type:'Terminal server'</li></ul>",
         "name": "filter",
         "in": "query"
       }
     ]
   ],
   [
-    "query_hosts",
+    "query-hosts",
     "GET",
     "/discover/queries/hosts/v1",
     "Search for assets in your environment by providing an FQL (Falcon Query Language) filter and paging details. "
     "Returns a set of asset IDs which match the filter criteria.",
     "discover",
     [
       {
@@ -233,23 +233,23 @@
         "Common sort options include:\n\n<ul><li>hostname|asc</li><li>product_type_desc|desc</li></ul>",
         "name": "sort",
         "in": "query"
       },
       {
         "type": "string",
         "description": "Filter assets using an FQL query. Common filter options include:\n\n"
-        "<ul><li>entity_type:'managed'</li><li>product_type_desc:'Workstation'</li><li>platform_name:'Windows'</li>"
-        "<li>last_seen_timestamp:>'now-7d'</li></ul>",
+        "<ul><li>entity_type:'managed'</li><li>product_type_desc:'Workstation'</li>"
+        "<li>platform_name:'Windows'</li><li>last_seen_timestamp:>'now-7d'</li></ul>",
         "name": "filter",
         "in": "query"
       }
     ]
   ],
   [
-    "query_logins",
+    "query-logins",
     "GET",
     "/discover/queries/logins/v1",
     "Search for logins in your environment by providing an FQL (Falcon Query Language) filter and paging details. "
     "Returns a set of login IDs which match the filter criteria.",
     "discover",
     [
       {
@@ -276,15 +276,78 @@
         "Common sort options include:\n\n<ul><li>hostname|asc</li><li>product_type_desc|desc</li></ul>",
         "name": "sort",
         "in": "query"
       },
       {
         "type": "string",
         "description": "Filter assets using an FQL query. Common filter options include:\n\n"
-        "<ul><li>entity_type:'managed'</li><li>product_type_desc:'Workstation'</li><li>platform_name:'Windows'</li>"
-        "<li>last_seen_timestamp:>'now-7d'</li></ul>",
+        "<ul><li>entity_type:'managed'</li><li>product_type_desc:'Workstation'</li><li>platform_name:'Windows'"
+        "</li><li>last_seen_timestamp:>'now-7d'</li></ul>",
+        "name": "filter",
+        "in": "query"
+      }
+    ]
+  ],
+  [
+    "get-iot-hosts",
+    "GET",
+    "/discover/entities/iot-hosts/v1",
+    "Get details on IoT assets by providing one or more IDs.",
+    "discover_iot",
+    [
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "One or more asset IDs (max: 100). Find asset IDs with GET `/discover/queries/iot-hosts/v1`",
+        "name": "ids",
+        "in": "query",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "query-iot-hosts",
+    "GET",
+    "/discover/queries/iot-hosts/v1",
+    "Search for IoT assets in your environment by providing an FQL (Falcon Query Language) filter and paging details. "
+    "Returns a set of asset IDs which match the filter criteria.",
+    "discover_iot",
+    [
+      {
+        "minimum": 0,
+        "type": "integer",
+        "description": "An offset used with the `limit` parameter to manage pagination of results. On your first request, "
+        "don’t provide an `offset`. On subsequent requests, provide the `offset` from the previous response to continue "
+        "from that place in the results.",
+        "name": "offset",
+        "in": "query"
+      },
+      {
+        "maximum": 100,
+        "minimum": 1,
+        "type": "integer",
+        "description": "The number of asset IDs to return in this response (min: 1, max: 100, default: 100). "
+        "Use with the `offset` parameter to manage pagination of results.",
+        "name": "limit",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "Sort assets by their properties. A single sort field is allowed. Common sort options "
+        "include:\n\n<ul><li>hostname|asc</li><li>product_type_desc|desc</li></ul>",
+        "name": "sort",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "Filter assets using an FQL query. Common filter options include:\n\n<ul>"
+        "<li>entity_type:'managed'</li><li>product_type_desc:'Workstation'</li>"
+        "<li>platform_name:'Windows'</li><li>last_seen_timestamp:>'now-7d'</li></ul>",
         "name": "filter",
         "in": "query"
       }
     ]
   ]
 ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_event_streams.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_falcon_complete_dashboard.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_falcon_container.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_quick_scan.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,94 +32,97 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
-_falcon_container_endpoints = [
+_quick_scan_endpoints = [
   [
-    "GetCredentials",
-    "GET",
-    "/container-security/entities/image-registry-credentials/v1",
-    "Gets the registry credentials",
-    "falcon_container",
-    []
-  ],
-  [
-    "ReadImageVulnerabilities",
+    "GetScansAggregates",
     "POST",
-    "/image-assessment/combined/vulnerability-lookups/v1",
-    "Retrieve known vulnerabilities for the provided image",
-    "falcon_container_cli",
+    "/scanner/aggregates/scans/GET/v1",
+    "Get scans aggregations as specified via json in request body.",
+    "quick_scan",
     [
       {
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
-    "GetImageAssessmentReport",
+    "GetScans",
     "GET",
-    "/reports",
-    "Retrieves the Assessment report for the Image ID provided.",
-    "falcon_container",
+    "/scanner/entities/scans/v1",
+    "Check the status of a volume scan. Time required for analysis increases with "
+    "the number of samples in a volume but usually it should take less than 1 minute",
+    "quick_scan",
     [
       {
-        "type": "string",
-        "description": "The repository the image resides within.",
-        "name": "repository",
-        "in": "query",
-        "required": True
-      },
-      {
-        "type": "string",
-        "description": "The image tag.",
-        "name": "tag",
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "csv",
+        "description": "ID of a submitted scan",
+        "name": "ids",
         "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "DeleteImageDetails",
-    "DELETE",
-    "/images/{}",
-    "Delete Images by ids.",
-    "falcon_container",
+    "ScanSamples",
+    "POST",
+    "/scanner/entities/scans/v1",
+    "Submit a volume of files for ml scanning. Time required for analysis increases with the "
+    "number of samples in a volume but usually it should take less than 1 minute",
+    "quick_scan",
     [
       {
-        "type": "string",
-        "description": "The ID of the image to be deleted.",
-        "name": "image_id",
-        "in": "path",
+        "description": "Submit a batch of SHA256s for ml scanning. The samples must have been "
+        "previously uploaded through `/samples/entities/samples/v3`",
+        "name": "body",
+        "in": "body",
         "required": True
       }
     ]
   ],
   [
-    "ImageMatchesPolicy",
+    "QuerySubmissionsMixin0",
     "GET",
-    "/policy-checks",
-    "After an image scan, use this operation to see if any images match a policy. If deny is true,"
-    " the policy suggestion is that you do not deploy the image in your environment.",
-    "falcon_container",
+    "/scanner/queries/scans/v1",
+    "Find IDs for submitted scans by providing an FQL filter and paging details. "
+    "Returns a set of volume IDs that match your criteria.",
+    "quick_scan",
     [
       {
         "type": "string",
-        "description": "The repository the image resides within.",
-        "name": "repository",
-        "in": "query",
-        "required": True
+        "description": "Optional filter and sort criteria in the form of an FQL query. "
+        "For more information about FQL queries, see [our FQL documentation in Falcon]"
+        "(https://falcon.crowdstrike.com/support/documentation/45/falcon-query-language-feature-guide).",
+        "name": "filter",
+        "in": "query"
       },
       {
         "type": "string",
-        "description": "The image tag.",
-        "name": "tag",
-        "in": "query",
-        "required": True
+        "description": "The offset to start retrieving submissions from.",
+        "name": "offset",
+        "in": "query"
+      },
+      {
+        "type": "integer",
+        "description": "Maximum number of volume IDs to return. Max: 5000.",
+        "name": "limit",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "Sort order: `asc` or `desc`.",
+        "name": "sort",
+        "in": "query"
       }
     ]
   ]
 ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_falconx_sandbox.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_falconx_sandbox.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,14 +64,101 @@
         "provide the value `gzip`, the only valid format.",
         "name": "Accept-Encoding",
         "in": "header"
       }
     ]
   ],
   [
+    "GetMemoryDumpExtractedStrings",
+    "GET",
+    "/falconx/entities/memory-dump/extracted-strings/v1",
+    "Get extracted strings from a memory dump",
+    "falconx_sandbox",
+    [
+      {
+        "type": "string",
+        "description": "Extracted strings id",
+        "name": "id",
+        "in": "query",
+        "required": True
+      },
+      {
+        "type": "string",
+        "description": "The name given to your downloaded file.",
+        "name": "name",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "Format used to compress your downloaded file. "
+        "Currently, you must provide the value `gzip`, the only valid format.",
+        "name": "Accept-Encoding",
+        "in": "header"
+      }
+    ]
+  ],
+  [
+    "GetMemoryDumpHexDump",
+    "GET",
+    "/falconx/entities/memory-dump/hex-dump/v1",
+    "Get hex view of a memory dump",
+    "falconx_sandbox",
+    [
+      {
+        "type": "string",
+        "description": "Hex dump id",
+        "name": "id",
+        "in": "query",
+        "required": True
+      },
+      {
+        "type": "string",
+        "description": "The name given to your downloaded file.",
+        "name": "name",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "Format used to compress your downloaded file. "
+        "Currently, you must provide the value `gzip`, the only valid format.",
+        "name": "Accept-Encoding",
+        "in": "header"
+      }
+    ]
+  ],
+  [
+    "GetMemoryDump",
+    "GET",
+    "/falconx/entities/memory-dump/v1",
+    "Get memory dump content, as binary",
+    "falconx_sandbox",
+    [
+      {
+        "type": "string",
+        "description": "Memory dump id",
+        "name": "id",
+        "in": "query",
+        "required": True
+      },
+      {
+        "type": "string",
+        "description": "The name given to your downloaded file.",
+        "name": "name",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "Format used to compress your downloaded file. "
+        "Currently, you must provide the value `gzip`, the only valid format.",
+        "name": "Accept-Encoding",
+        "in": "header"
+      }
+    ]
+  ],
+  [
     "GetSummaryReports",
     "GET",
     "/falconx/entities/report-summaries/v1",
     "Get a short summary version of a sandbox report.",
     "falconx_sandbox",
     [
       {
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_filevantage.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_filevantage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_firewall_management.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_firewall_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_host_group.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_hosts.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_hosts.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,21 @@
         "type": "string",
         "description": "The action to perform.",
         "name": "action_name",
         "in": "query",
         "required": True
       },
       {
+        "type": "boolean",
+        "default": False,
+        "description": "Bool to disable hostname check on add-member",
+        "name": "disable_hostname_check",
+        "in": "query"
+      },
+      {
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_identity_protection.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_incidents.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_malquery.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,190 +32,160 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
-_incidents_endpoints = [
+_malquery_endpoints = [
   [
-    "CrowdScore",
+    "GetMalQueryQuotasV1",
     "GET",
-    "/incidents/combined/crowdscores/v1",
-    "Query environment wide CrowdScore and return the entity data",
-    "incidents",
+    "/malquery/aggregates/quotas/v1",
+    "Get information about search and download quotas in your environment",
+    "malquery",
+    []
+  ],
+  [
+    "PostMalQueryFuzzySearchV1",
+    "POST",
+    "/malquery/combined/fuzzy-search/v1",
+    "Search Falcon MalQuery quickly, but with more potential for false positives. "
+    "Search for a combination of hex patterns and strings in order to identify samples based upon "
+    "file content at byte level granularity.",
+    "malquery",
     [
       {
-        "type": "string",
-        "description": "Optional filter and sort criteria in the form of an FQL query. "
-        "For more information about FQL queries, see [our FQL documentation in Falcon]"
-        "(https://falcon.crowdstrike.com/support/documentation/45/falcon-query-language-feature-guide).",
-        "name": "filter",
-        "in": "query"
-      },
-      {
-        "type": "string",
-        "description": "Starting index of overall result set from which to return ids.",
-        "name": "offset",
-        "in": "query"
-      },
-      {
-        "type": "integer",
-        "description": "The maximum records to return. [1-2500]",
-        "name": "limit",
-        "in": "query"
-      },
-      {
-        "enum": [
-          "score.asc",
-          "score.desc",
-          "timestamp.asc",
-          "timestamp.desc"
-        ],
-        "type": "string",
-        "description": "The property to sort on, followed by a dot (.), "
-        "followed by the sort direction, either \"asc\" or \"desc\".",
-        "name": "sort",
-        "in": "query"
+        "description": "Fuzzy search parameters. See model for more details.",
+        "name": "body",
+        "in": "body",
+        "required": True
       }
     ]
   ],
   [
-    "GetBehaviors",
-    "POST",
-    "/incidents/entities/behaviors/GET/v1",
-    "Get details on behaviors by providing behavior IDs",
-    "incidents",
+    "GetMalQueryDownloadV1",
+    "GET",
+    "/malquery/entities/download-files/v1",
+    "Download a file indexed by MalQuery. Specify the file using its SHA256. Only one file is supported at this time",
+    "malquery",
     [
       {
-        "name": "body",
-        "in": "body",
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "csv",
+        "description": "The file SHA256.",
+        "name": "ids",
+        "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "PerformIncidentAction",
-    "POST",
-    "/incidents/entities/incident-actions/v1",
-    "Perform a set of actions on one or more incidents, such as adding tags or comments "
-    "or updating the incident name or description",
-    "incidents",
+    "GetMalQueryMetadataV1",
+    "GET",
+    "/malquery/entities/metadata/v1",
+    "Retrieve indexed files metadata by their hash",
+    "malquery",
     [
       {
-        "name": "body",
-        "in": "body",
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "csv",
+        "description": "The file SHA256.",
+        "name": "ids",
+        "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "GetIncidents",
-    "POST",
-    "/incidents/entities/incidents/GET/v1",
-    "Get details on incidents by providing incident IDs",
-    "incidents",
+    "GetMalQueryRequestV1",
+    "GET",
+    "/malquery/entities/requests/v1",
+    "Check the status and results of an asynchronous request, such as hunt or exact-search. "
+    "Supports a single request id at this time.",
+    "malquery",
     [
       {
-        "name": "body",
-        "in": "body",
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "csv",
+        "description": "Identifier of a MalQuery request",
+        "name": "ids",
+        "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "QueryBehaviors",
+    "GetMalQueryEntitiesSamplesFetchV1",
     "GET",
-    "/incidents/queries/behaviors/v1",
-    "Search for behaviors by providing an FQL filter, sorting, and paging details",
-    "incidents",
+    "/malquery/entities/samples-fetch/v1",
+    "Fetch a zip archive with password 'infected' containing the samples. "
+    "Call this once the /entities/samples-multidownload request has finished processing",
+    "malquery",
     [
       {
         "type": "string",
-        "description": "Optional filter and sort criteria in the form of an FQL query. "
-        "For more information about FQL queries, see [our FQL documentation in Falcon]"
-        "(https://falcon.crowdstrike.com/support/documentation/45/falcon-query-language-feature-guide).",
-        "name": "filter",
-        "in": "query"
-      },
+        "description": "Multidownload job id",
+        "name": "ids",
+        "in": "query",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "PostMalQueryEntitiesSamplesMultidownloadV1",
+    "POST",
+    "/malquery/entities/samples-multidownload/v1",
+    "Schedule samples for download. Use the result id with the /request endpoint to check if "
+    "the download is ready after which you can call the /entities/samples-fetch to get the zip",
+    "malquery",
+    [
       {
-        "type": "string",
-        "description": "Starting index of overall result set from which to return ids.",
-        "name": "offset",
-        "in": "query"
-      },
-      {
-        "type": "integer",
-        "description": "The maximum records to return. [1-500]",
-        "name": "limit",
-        "in": "query"
-      },
-      {
-        "enum": [
-          "timestamp.asc",
-          "timestamp.desc"
-        ],
-        "type": "string",
-        "description": "The property to sort on, followed by a dot (.), "
-        "followed by the sort direction, either \"asc\" or \"desc\".",
-        "name": "sort",
-        "in": "query"
+        "description": "Download request. See model for more details.",
+        "name": "body",
+        "in": "body",
+        "required": True
       }
     ]
   ],
   [
-    "QueryIncidents",
-    "GET",
-    "/incidents/queries/incidents/v1",
-    "Search for incidents by providing an FQL filter, sorting, and paging details",
-    "incidents",
-    [
-      {
-        "enum": [
-          "assigned_to.asc",
-          "assigned_to.desc",
-          "assigned_to_name.asc",
-          "assigned_to_name.desc",
-          "end.asc",
-          "end.desc",
-          "modified_timestamp.asc",
-          "modified_timestamp.desc",
-          "name.asc",
-          "name.desc",
-          "sort_score.asc",
-          "sort_score.desc",
-          "start.asc",
-          "start.desc",
-          "state.asc",
-          "state.desc",
-          "status.asc",
-          "status.desc"
-        ],
-        "type": "string",
-        "description": "The property to sort on, followed by a dot (.), "
-        "followed by the sort direction, either \"asc\" or \"desc\".",
-        "name": "sort",
-        "in": "query"
-      },
+    "PostMalQueryExactSearchV1",
+    "POST",
+    "/malquery/queries/exact-search/v1",
+    "Search Falcon MalQuery for a combination of hex patterns and strings in order to identify "
+    "samples based upon file content at byte level granularity. You can filter results on criteria "
+    "such as file type, file size and first seen date. Returns a request id which can be used with the /request endpoint",
+    "malquery",
+    [
       {
-        "type": "string",
-        "description": "Optional filter and sort criteria in the form of an FQL query. "
-        "For more information about FQL queries, see [our FQL documentation in Falcon]"
-        "(https://falcon.crowdstrike.com/support/documentation/45/falcon-query-language-feature-guide).",
-        "name": "filter",
-        "in": "query"
-      },
+        "description": "Exact search parameters. See model for more details.",
+        "name": "body",
+        "in": "body",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "PostMalQueryHuntV1",
+    "POST",
+    "/malquery/queries/hunt/v1",
+    "Schedule a YARA-based search for execution. Returns a request id which can be used with the /request endpoint",
+    "malquery",
+    [
       {
-        "type": "string",
-        "description": "Starting index of overall result set from which to return ids.",
-        "name": "offset",
-        "in": "query"
-      },
-      {
-        "type": "integer",
-        "description": "The maximum records to return. [1-500]",
-        "name": "limit",
-        "in": "query"
+        "description": "Hunt parameters. See model for more details.",
+        "name": "body",
+        "in": "body",
+        "required": True
       }
     ]
   ]
 ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_installation_tokens.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_intel.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_ioa_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_ioc.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ioc.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     "ioc",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
-        "collectionFormat": "csv",
+        "collectionFormat": "multi",
         "description": "The ids of the Actions to retrieve",
         "name": "ids",
         "in": "query"
       }
     ]
   ],
   [
@@ -173,15 +173,15 @@
     "ioc",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
-        "collectionFormat": "csv",
+        "collectionFormat": "multi",
         "description": "The ids of the Indicators to retrieve",
         "name": "ids",
         "in": "query",
         "required": True
       }
     ]
   ],
@@ -254,15 +254,15 @@
         "in": "query"
       },
       {
         "type": "array",
         "items": {
           "type": "string"
         },
-        "collectionFormat": "csv",
+        "collectionFormat": "multi",
         "description": "The ids of the Indicators to delete. If both 'filter' and 'ids' are provided, "
         "then filter takes precedence and ignores ids",
         "name": "ids",
         "in": "query"
       },
       {
         "type": "string",
@@ -355,14 +355,20 @@
         "type": "string",
         "description": "A pagination token used with the `limit` parameter to manage pagination of results. "
         "On your first request, don't provide an 'after' token. On subsequent requests, provide the 'after' "
         "token from the previous response to continue from that place in the results. To access more than 10k "
         "indicators, use the 'after' parameter instead of 'offset'.",
         "name": "after",
         "in": "query"
+      },
+      {
+        "type": "boolean",
+        "description": "The filter for returning either only indicators for the request customer or its MSSP parents",
+        "name": "from_parent",
+        "in": "query"
       }
     ]
   ],
   [
     "ioc_type_query_v1",
     "GET",
     "/iocs/queries/ioc-types/v1",
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_iocs.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_kubernetes_protection.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_ioc.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,381 +32,383 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
-_kubernetes_protection_endpoints = [
+_ioc_endpoints = [
   [
-    "GetAWSAccountsMixin0",
-    "GET",
-    "/kubernetes-protection/entities/accounts/aws/v1",
-    "Provides a list of AWS accounts.",
-    "kubernetes_protection",
+    "indicator.aggregate.v1",
+    "POST",
+    "/iocs/aggregates/indicators/v1",
+    "Get Indicators aggregates as specified via json in the request body.",
+    "ioc",
     [
       {
-        "type": "array",
-        "items": {
-          "minLength": 12,
-          "pattern": "^[0-9]{12}$",
-          "type": "string"
-        },
-        "collectionFormat": "csv",
-        "description": "AWS Account IDs",
-        "name": "ids",
+        "type": "string",
+        "description": "The filter to narrow down the aggregation data",
+        "name": "filter",
+        "in": "query"
+      },
+      {
+        "type": "boolean",
+        "description": "The filter for returning either only indicators for the request customer or its MSSP parents",
+        "name": "from_parent",
         "in": "query"
       },
       {
-        "pattern": "^(provisioned|operational)$",
+        "name": "body",
+        "in": "body",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "indicator.combined.v1",
+    "GET",
+    "/iocs/combined/indicator/v1",
+    "Get Combined for Indicators.",
+    "ioc",
+    [
+      {
         "type": "string",
-        "description": "Filter by account status",
-        "name": "status",
+        "description": "The filter expression that should be used to limit the results.",
+        "name": "filter",
         "in": "query"
       },
       {
-        "maximum": 1000,
-        "minimum": 0,
         "type": "integer",
-        "description": "Limit returned accounts",
-        "name": "limit",
+        "description": "The offset to start retrieving records from. Offset and After params are mutually exclusive. "
+        "If none provided then scrolling will be used by default.",
+        "name": "offset",
         "in": "query"
       },
       {
-        "minimum": 0,
         "type": "integer",
-        "description": "Offset returned accounts",
-        "name": "offset",
+        "description": "The maximum records to return.",
+        "name": "limit",
         "in": "query"
-      }
-    ]
-  ],
-  [
-    "CreateAWSAccount",
-    "POST",
-    "/kubernetes-protection/entities/accounts/aws/v1",
-    "Creates a new AWS account in our system for a customer and generates the installation script",
-    "kubernetes_protection",
-    [
+      },
       {
-        "name": "body",
-        "in": "body",
-        "required": True
+        "enum": [
+          "action",
+          "applied_globally",
+          "metadata.av_hits",
+          "metadata.company_name.raw",
+          "created_by",
+          "created_on",
+          "expiration",
+          "expired",
+          "metadata.filename.raw",
+          "modified_by",
+          "modified_on",
+          "metadata.original_filename.raw",
+          "metadata.product_name.raw",
+          "metadata.product_version",
+          "severity_number",
+          "source",
+          "type",
+          "value"
+        ],
+        "type": "string",
+        "description": "The sort expression that should be used to sort the results.",
+        "name": "sort",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "A pagination token used with the `limit` parameter to manage pagination of results. "
+        "On your first request, don't provide an 'after' token. On subsequent requests, provide the 'after' "
+        "token from the previous response to continue from that place in the results. "
+        "To access more than 10k indicators, use the 'after' parameter instead of 'offset'.",
+        "name": "after",
+        "in": "query"
+      },
+      {
+        "type": "boolean",
+        "description": "The filter for returning either only indicators for the request customer or its MSSP parents",
+        "name": "from_parent",
+        "in": "query"
       }
     ]
   ],
   [
-    "UpdateAWSAccount",
-    "PATCH",
-    "/kubernetes-protection/entities/accounts/aws/v1",
-    "Updates the AWS account per the query parameters provided",
-    "kubernetes_protection",
+    "action.get.v1",
+    "GET",
+    "/iocs/entities/actions/v1",
+    "Get Actions by ids.",
+    "ioc",
     [
       {
         "type": "array",
         "items": {
-          "maxLength": 12,
-          "minLength": 12,
-          "pattern": "^[0-9]{12}$",
           "type": "string"
         },
         "collectionFormat": "csv",
-        "description": "AWS Account ID",
+        "description": "The ids of the Actions to retrieve",
         "name": "ids",
-        "in": "query",
-        "required": True
-      },
-      {
-        "pattern": "^[a-z\\d-]+$",
-        "type": "string",
-        "description": "Default Region for Account Automation",
-        "name": "region",
         "in": "query"
       }
     ]
   ],
   [
-    "DeleteAWSAccountsMixin0",
-    "DELETE",
-    "/kubernetes-protection/entities/accounts/aws/v1",
-    "Delete AWS accounts.",
-    "kubernetes_protection",
+    "indicator.get.v1",
+    "GET",
+    "/iocs/entities/indicators/v1",
+    "Get Indicators by ids.",
+    "ioc",
     [
       {
         "type": "array",
         "items": {
-          "maxLength": 12,
-          "minLength": 12,
-          "pattern": "^[0-9]{12}$",
           "type": "string"
         },
         "collectionFormat": "csv",
-        "description": "AWS Account IDs",
+        "description": "The ids of the Indicators to retrieve",
         "name": "ids",
         "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "ListAzureAccounts",
-    "GET",
-    "/kubernetes-protection/entities/accounts/azure/v1",
-    "Provides the azure subscriptions registered to Kubernetes Protection",
-    "kubernetes_protection",
+    "indicator.create.v1",
+    "POST",
+    "/iocs/entities/indicators/v1",
+    "Create Indicators.",
+    "ioc",
     [
       {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "csv",
-        "description": "Azure Tenant IDs",
-        "name": "ids",
+        "type": "boolean",
+        "description": "Whether to submit to retrodetects",
+        "name": "retrodetects",
         "in": "query"
       },
       {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "csv",
-        "description": "Azure Subscription IDs",
-        "name": "subscription_id",
+        "type": "boolean",
+        "default": False,
+        "description": "Set to true to ignore warnings and add all IOCs",
+        "name": "ignore_warnings",
         "in": "query"
       },
       {
-        "pattern": "^(provisioned|operational)$",
-        "enum": [
-          "operational",
-          "provisioned"
-        ],
-        "type": "string",
-        "description": "Filter by account status",
-        "name": "status",
-        "in": "query"
-      },
+        "name": "body",
+        "in": "body",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "indicator.update.v1",
+    "PATCH",
+    "/iocs/entities/indicators/v1",
+    "Update Indicators.",
+    "ioc",
+    [
       {
-        "pattern": "^(true|false)$",
-        "enum": [
-          "false",
-          "true"
-        ],
-        "type": "string",
-        "description": "Filter by whether an account originates from Horizon or not",
-        "name": "is_horizon_acct",
+        "type": "boolean",
+        "description": "Whether to submit to retrodetects",
+        "name": "retrodetects",
         "in": "query"
       },
       {
-        "maximum": 1000,
-        "minimum": 0,
-        "type": "integer",
-        "description": "Limit returned accounts",
-        "name": "limit",
+        "type": "boolean",
+        "default": False,
+        "description": "Set to true to ignore warnings and add all IOCs",
+        "name": "ignore_warnings",
         "in": "query"
       },
       {
-        "minimum": 0,
-        "type": "integer",
-        "description": "Offset returned accounts",
-        "name": "offset",
-        "in": "query"
-      }
-    ]
-  ],
-  [
-    "CreateAzureSubscription",
-    "POST",
-    "/kubernetes-protection/entities/accounts/azure/v1",
-    "Creates a new Azure Subscription in our system",
-    "kubernetes_protection",
-    [
-      {
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
-    "DeleteAzureSubscription",
+    "indicator.delete.v1",
     "DELETE",
-    "/kubernetes-protection/entities/accounts/azure/v1",
-    "Deletes a new Azure Subscription in our system",
-    "kubernetes_protection",
+    "/iocs/entities/indicators/v1",
+    "Delete Indicators by ids.",
+    "ioc",
     [
       {
+        "type": "string",
+        "description": "The FQL expression to delete Indicators in bulk. If both 'filter' and 'ids' are provided, "
+        "then filter takes precedence and ignores ids.",
+        "name": "filter",
+        "in": "query"
+      },
+      {
         "type": "array",
         "items": {
           "type": "string"
         },
         "collectionFormat": "csv",
-        "description": "Azure Subscription IDs",
+        "description": "The ids of the Indicators to delete. If both 'filter' and 'ids' are provided, "
+        "then filter takes precedence and ignores ids",
         "name": "ids",
         "in": "query"
-      }
-    ]
-  ],
-  [
-    "GetLocations",
-    "GET",
-    "/kubernetes-protection/entities/cloud-locations/v1",
-    "Provides the cloud locations acknowledged by the Kubernetes Protection service",
-    "kubernetes_protection",
-    [
+      },
       {
-        "enum": [
-          "aws",
-          "azure",
-          "gcp"
-        ],
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "csv",
-        "description": "Cloud Provider",
-        "name": "clouds",
+        "type": "string",
+        "description": "The comment why these indicators were deleted",
+        "name": "comment",
+        "in": "query"
+      },
+      {
+        "type": "boolean",
+        "description": "The filter for returning either only indicators for the request customer or its MSSP parents",
+        "name": "from_parent",
         "in": "query"
       }
     ]
   ],
   [
-    "GetHelmValuesYaml",
+    "action.query.v1",
     "GET",
-    "/kubernetes-protection/entities/integration/agent/v1",
-    "Provides a sample Helm values.yaml file for a customer to install alongside the agent Helm chart",
-    "kubernetes_protection",
+    "/iocs/queries/actions/v1",
+    "Query Actions.",
+    "ioc",
     [
       {
         "type": "string",
-        "description": "Cluster name. For EKS it will be cluster ARN.",
-        "name": "cluster_name",
-        "in": "query",
-        "required": True
+        "description": "Starting index of overall result set from which to return ids.",
+        "name": "offset",
+        "in": "query"
+      },
+      {
+        "type": "integer",
+        "description": "Number of ids to return.",
+        "name": "limit",
+        "in": "query"
       }
     ]
   ],
   [
-    "RegenerateAPIKey",
-    "POST",
-    "/kubernetes-protection/entities/integration/api-key/v1",
-    "Regenerate API key for docker registry integrations",
-    "kubernetes_protection",
-    []
-  ],
-  [
-    "GetClusters",
+    "indicator.search.v1",
     "GET",
-    "/kubernetes-protection/entities/kubernetes/clusters/v1",
-    "Provides the clusters acknowledged by the Kubernetes Protection service",
-    "kubernetes_protection",
+    "/iocs/queries/indicators/v1",
+    "Search for Indicators.",
+    "ioc",
     [
       {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "csv",
-        "description": "Cluster name. For EKS it will be cluster ARN.",
-        "name": "cluster_names",
+        "type": "string",
+        "description": "The filter expression that should be used to limit the results.",
+        "name": "filter",
         "in": "query"
       },
       {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "csv",
-        "description": "Cluster Account id. For EKS it will be AWS account ID.",
-        "name": "account_ids",
+        "type": "integer",
+        "description": "The offset to start retrieving records from. Offset and After params are mutually exclusive. "
+        "If none provided then scrolling will be used by default.",
+        "name": "offset",
         "in": "query"
       },
       {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "csv",
-        "description": "Cloud location",
-        "name": "locations",
+        "type": "integer",
+        "description": "The maximum records to return.",
+        "name": "limit",
         "in": "query"
       },
       {
         "enum": [
-          "eks"
+          "action",
+          "applied_globally",
+          "metadata.av_hits",
+          "metadata.company_name.raw",
+          "created_by",
+          "created_on",
+          "expiration",
+          "expired",
+          "metadata.filename.raw",
+          "modified_by",
+          "modified_on",
+          "metadata.original_filename.raw",
+          "metadata.product_name.raw",
+          "metadata.product_version",
+          "severity_number",
+          "source",
+          "type",
+          "value"
         ],
         "type": "string",
-        "description": "Cluster Service",
-        "name": "cluster_service",
+        "description": "The sort expression that should be used to sort the results.",
+        "name": "sort",
         "in": "query"
       },
       {
-        "maximum": 1000,
-        "minimum": 0,
-        "type": "integer",
-        "description": "Limit returned accounts",
-        "name": "limit",
+        "type": "string",
+        "description": "A pagination token used with the `limit` parameter to manage pagination of results. "
+        "On your first request, don't provide an 'after' token. On subsequent requests, provide the 'after' "
+        "token from the previous response to continue from that place in the results. "
+        "To access more than 10k indicators, use the 'after' parameter instead of 'offset'.",
+        "name": "after",
+        "in": "query"
+      }
+    ]
+  ],
+  [
+    "ioc_type.query.v1",
+    "GET",
+    "/iocs/queries/ioc-types/v1",
+    "Query IOC Types.",
+    "ioc",
+    [
+      {
+        "type": "string",
+        "description": "Starting index of overall result set from which to return ids.",
+        "name": "offset",
         "in": "query"
       },
       {
-        "minimum": 0,
         "type": "integer",
-        "description": "Offset returned accounts",
-        "name": "offset",
+        "description": "Number of ids to return.",
+        "name": "limit",
         "in": "query"
       }
     ]
   ],
   [
-    "TriggerScan",
-    "POST",
-    "/kubernetes-protection/entities/scan/trigger/v1",
-    "Triggers a dry run or a full scan of a customer's kubernetes footprint",
-    "kubernetes_protection",
+    "platform.query.v1",
+    "GET",
+    "/iocs/queries/platforms/v1",
+    "Query Platforms.",
+    "ioc",
     [
       {
-        "pattern": "^(dry-run|full|cluster-refresh)$",
-        "enum": [
-          "cluster-refresh",
-          "dry-run",
-          "full"
-        ],
         "type": "string",
-        "default": "dry-run",
-        "description": "Scan Type to do",
-        "name": "scan_type",
-        "in": "query",
-        "required": True
+        "description": "Starting index of overall result set from which to return ids.",
+        "name": "offset",
+        "in": "query"
+      },
+      {
+        "type": "integer",
+        "description": "Number of ids to return.",
+        "name": "limit",
+        "in": "query"
       }
     ]
   ],
   [
-    "PatchAzureServicePrincipal",
-    "PATCH",
-    "/kubernetes-protection/entities/service-principal/azure/v1",
-    "Adds the client ID for the given tenant ID to our system",
-    "kubernetes_protection",
+    "severity.query.v1",
+    "GET",
+    "/iocs/queries/severities/v1",
+    "Query Severities.",
+    "ioc",
     [
       {
-        "maxLength": 36,
-        "minLength": 36,
-        "pattern": "^[0-9A-Fa-f]{8}-[0-9A-Fa-f]{4}-4[0-9A-Fa-f]{3}-[89ABab][0-9A-Fa-f]{3}-[0-9A-Fa-f]{12}$",
         "type": "string",
-        "description": "Azure Tenant ID",
-        "name": "id",
-        "in": "query",
-        "required": True
+        "description": "Starting index of overall result set from which to return ids.",
+        "name": "offset",
+        "in": "query"
       },
       {
-        "maxLength": 36,
-        "minLength": 36,
-        "pattern": "^[0-9A-Fa-f]{8}-[0-9A-Fa-f]{4}-4[0-9A-Fa-f]{3}-[89ABab][0-9A-Fa-f]{3}-[0-9A-Fa-f]{12}$",
-        "type": "string",
-        "description": "Azure Client ID",
-        "name": "client_id",
-        "in": "query",
-        "required": True
+        "type": "integer",
+        "description": "Number of ids to return.",
+        "name": "limit",
+        "in": "query"
       }
     ]
   ]
 ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_malquery.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_zero_trust_assessment.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,160 +32,130 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
-_malquery_endpoints = [
+_zero_trust_assessment_endpoints = [
   [
-    "GetMalQueryQuotasV1",
+    "getAssessmentV1",
     "GET",
-    "/malquery/aggregates/quotas/v1",
-    "Get information about search and download quotas in your environment",
-    "malquery",
-    []
-  ],
-  [
-    "PostMalQueryFuzzySearchV1",
-    "POST",
-    "/malquery/combined/fuzzy-search/v1",
-    "Search Falcon MalQuery quickly, but with more potential for false positives. "
-    "Search for a combination of hex patterns and strings in order to identify samples based upon "
-    "file content at byte level granularity.",
-    "malquery",
-    [
-      {
-        "description": "Fuzzy search parameters. See model for more details.",
-        "name": "body",
-        "in": "body",
-        "required": True
-      }
-    ]
-  ],
-  [
-    "GetMalQueryDownloadV1",
-    "GET",
-    "/malquery/entities/download-files/v1",
-    "Download a file indexed by MalQuery. Specify the file using its SHA256. Only one file is supported at this time",
-    "malquery",
+    "/zero-trust-assessment/entities/assessments/v1",
+    "Get Zero Trust Assessment data for one or more hosts by providing agent IDs (AID) and a customer ID (CID).",
+    "zero_trust_assessment",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
-        "collectionFormat": "csv",
-        "description": "The file SHA256.",
+        "collectionFormat": "multi",
+        "description": "One or more agent IDs, which you can find in the data.zta file, or the Falcon console.",
         "name": "ids",
         "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "GetMalQueryMetadataV1",
+    "getAuditV1",
     "GET",
-    "/malquery/entities/metadata/v1",
-    "Retrieve indexed files metadata by their hash",
-    "malquery",
-    [
-      {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "csv",
-        "description": "The file SHA256.",
-        "name": "ids",
-        "in": "query",
-        "required": True
-      }
-    ]
+    "/zero-trust-assessment/entities/audit/v1",
+    "Get the Zero Trust Assessment audit report for one customer ID (CID).",
+    "zero_trust_assessment",
+    []
   ],
   [
-    "GetMalQueryRequestV1",
+    "getAssessmentsByScoreV1",
     "GET",
-    "/malquery/entities/requests/v1",
-    "Check the status and results of an asynchronous request, such as hunt or exact-search. "
-    "Supports a single request id at this time.",
-    "malquery",
+    "/zero-trust-assessment/queries/assessments/v1",
+    "Get Zero Trust Assessment data for one or more hosts by providing a customer ID (CID) and a range of scores.",
+    "zero_trust_assessment",
     [
       {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "csv",
-        "description": "Identifier of a MalQuery request",
-        "name": "ids",
+        "type": "string",
+        "description": "FQL query specifying the filter score.",
+        "name": "filter",
         "in": "query",
         "required": True
+      },
+      {
+        "type": "integer",
+        "description": "The number of scores to return in this response (min: 1, max: 1000, default: 100). "
+        "Use with the `after` parameter to manage pagination of results.",
+        "name": "limit",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "A pagination token used with the `limit` parameter to manage pagination of results. "
+        "On your first request, don't provide an `after` token. On subsequent requests, provide the `after` "
+        "token from the previous response to continue from that place in the results.",
+        "name": "after",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "default": "score",
+        "description": "Sort accounts by their properties. A single sort field is allowed. "
+        "Defaults to ascending. Supported sort option include:\n\n<ul><li>score|desc</li><li>score|asc</li></ul>",
+        "name": "sort",
+        "in": "query"
       }
     ]
   ],
   [
-    "GetMalQueryEntitiesSamplesFetchV1",
+    "getCombinedAssessmentsQuery",
     "GET",
-    "/malquery/entities/samples-fetch/v1",
-    "Fetch a zip archive with password 'infected' containing the samples. "
-    "Call this once the /entities/samples-multidownload request has finished processing",
-    "malquery",
+    "/configuration-assessment/combined/assessments/v1",
+    "Search for assessments in your environment by providing an FQL filter and paging details. "
+    "Returns a set of HostFinding entities which match the filter criteria",
+    "public_assessments",
     [
       {
         "type": "string",
-        "description": "Multidownload job id",
-        "name": "ids",
-        "in": "query",
-        "required": True
-      }
-    ]
-  ],
-  [
-    "PostMalQueryEntitiesSamplesMultidownloadV1",
-    "POST",
-    "/malquery/entities/samples-multidownload/v1",
-    "Schedule samples for download. Use the result id with the /request endpoint to check if "
-    "the download is ready after which you can call the /entities/samples-fetch to get the zip",
-    "malquery",
-    [
+        "description": "A pagination token used with the `limit` parameter to manage pagination of results. "
+        "On your first request, don't provide an `after` token. On subsequent requests, provide the `after` "
+        "token from the previous response to continue from that place in the results.",
+        "name": "after",
+        "in": "query"
+      },
+      {
+        "maximum": 5000,
+        "minimum": 1,
+        "type": "integer",
+        "description": "The number of items to return in this response (default: 100, max: 5000). "
+        "Use with the after parameter to manage pagination of results.",
+        "name": "limit",
+        "in": "query"
+      },
       {
-        "description": "Download request. See model for more details.",
-        "name": "body",
-        "in": "body",
-        "required": True
-      }
-    ]
-  ],
-  [
-    "PostMalQueryExactSearchV1",
-    "POST",
-    "/malquery/queries/exact-search/v1",
-    "Search Falcon MalQuery for a combination of hex patterns and strings in order to identify "
-    "samples based upon file content at byte level granularity. You can filter results on criteria "
-    "such as file type, file size and first seen date. Returns a request id which can be used with the /request endpoint",
-    "malquery",
-    [
+        "type": "string",
+        "description": "Sort assessment by their properties. Common sort options include:\n\n"
+        "<ul><li>created_timestamp|desc</li><li>updated_timestamp|asc</li></ul>",
+        "name": "sort",
+        "in": "query"
+      },
       {
-        "description": "Exact search parameters. See model for more details.",
-        "name": "body",
-        "in": "body",
+        "type": "string",
+        "description": "Filter items using a query in Falcon Query Language (FQL). Wildcards * are unsupported. "
+        "\n\nCommon filter options include:\n\n<ul><li>created_timestamp:>'2019-11-25T22:36:12Z'</li>"
+        "<li>updated_timestamp:>'2019-11-25T22:36:12Z'</li><li>aid:'8e7656b27d8c49a34a1af416424d6231'</li></ul>",
+        "name": "filter",
+        "in": "query",
         "required": True
-      }
-    ]
-  ],
-  [
-    "PostMalQueryHuntV1",
-    "POST",
-    "/malquery/queries/hunt/v1",
-    "Schedule a YARA-based search for execution. Returns a request id which can be used with the /request endpoint",
-    "malquery",
-    [
+      },
       {
-        "description": "Hunt parameters. See model for more details.",
-        "name": "body",
-        "in": "body",
-        "required": True
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "Select various details blocks to be returned for each assessment entity. "
+        "Supported values:\n\n<ul><li>host</li><li>finding.rule</li></ul>",
+        "name": "facet",
+        "in": "query"
       }
     ]
   ]
 ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_message_center.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_message_center.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,28 @@
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
+    "CreateCaseV2",
+    "POST",
+    "/message-center/entities/case/v2",
+    "create a new case",
+    "message_center",
+    [
+      {
+        "name": "body",
+        "in": "body",
+        "required": True
+      }
+    ]
+  ],
+  [
     "GetCaseEntitiesByIDs",
     "POST",
     "/message-center/entities/cases/GET/v1",
     "Retrieve message center cases",
     "message_center",
     [
       {
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_ml_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_mobile_enrollment.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_mssp.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_mssp.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,15 @@
       }
     ]
   ],
   [
     "getCIDGroupMembersByV1",
     "GET",
     "/mssp/entities/cid-group-members/v1",
-    "Get CID group members by CID group ID.",
+    "Deprecated: Please use getCIDGroupMembersBy. Get CID group members by CID group ID.",
     "mssp",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
@@ -91,32 +91,34 @@
       }
     ]
   ],
   [
     "addCIDGroupMembers",
     "POST",
     "/mssp/entities/cid-group-members/v1",
-    "Add new CID Group member.",
+    "Add new CID group member.",
     "mssp",
     [
       {
+        "description": "Both 'cid_group_id' and 'cids' fields are required.",
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
     "deleteCIDGroupMembers",
     "DELETE",
     "/mssp/entities/cid-group-members/v1",
-    "Delete CID Group members entry.",
+    "Delete CID group members.",
     "mssp",
     [
       {
+        "description": "Both 'cid_group_id' and 'cids' fields are required.",
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
@@ -159,15 +161,15 @@
       }
     ]
   ],
   [
     "getCIDGroupByIdV1",
     "GET",
     "/mssp/entities/cid-groups/v1",
-    "Get CID groups by ID.",
+    "Deprecated: Please use getCIDGroupById. Get CID groups by ID.",
     "mssp",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
@@ -179,33 +181,37 @@
       }
     ]
   ],
   [
     "createCIDGroups",
     "POST",
     "/mssp/entities/cid-groups/v1",
-    "Create new CID Group(s). Maximum 500 CID Group(s) allowed.",
+    "Create new CID groups. Name is a required field but description is an optional field. Maximum 500 CID groups allowed.",
     "mssp",
     [
       {
+        "description": "Only 'name' and/or 'description' fields are required. Remaining are assigned by the system.",
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
     "updateCIDGroups",
     "PATCH",
     "/mssp/entities/cid-groups/v1",
     "Update existing CID Group(s). CID Group ID is expected for each CID Group definition provided in request body. "
-    "CID Group member(s) remain unaffected.",
+    "Name is a required field but description is an optional field. Empty description will override "
+    "existing value. CID Group member(s) remain unaffected.",
     "mssp",
     [
       {
+        "description": "'cid_group_id' field is required to identify the CID group to update along "
+        "with 'name' and/or 'description' fields to be updated.",
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
@@ -268,66 +274,73 @@
       }
     ]
   ],
   [
     "getRolesByID",
     "GET",
     "/mssp/entities/mssp-roles/v1",
-    "Get MSSP Role assignment(s). MSSP Role assignment is of the format :.",
+    "Get link between user group and CID group by ID. Link ID is a string consisting of multiple "
+    "components, but should be treated as opaque. MSSP Role assignment is of the format <user_group_id>:<cid_group_id>.",
     "mssp",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
-        "collectionFormat": "csv",
-        "description": "MSSP Role assignment is of the format <user_group_id>:<cid_group_id>",
+        "collectionFormat": "multi",
+        "description": "Link ID is a string consisting of multiple components, but should be "
+        "treated as opaque. MSSP Role assignment is of the format <user_group_id>:<cid_group_id>",
         "name": "ids",
         "in": "query",
         "required": True
       }
     ]
   ],
   [
     "addRole",
     "POST",
     "/mssp/entities/mssp-roles/v1",
-    "Assign new MSSP Role(s) between User Group and CID Group. It does not revoke existing role(s) "
-    "between User Group and CID Group. User Group ID and CID Group ID have to be specified in request. ",
+    "Create a link between user group and CID group, with zero or more additional roles. "
+    "The call does not replace any existing link between them. User group ID and CID group ID "
+    "have to be specified in request. ",
     "mssp",
     [
       {
+        "description": "'user_group_id', 'cid_group_id' and 'role_ids' fields are required. "
+        "Remaining are populated by system.",
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
     "deletedRoles",
     "DELETE",
     "/mssp/entities/mssp-roles/v1",
-    "Delete MSSP Role assignment(s) between User Group and CID Group. User Group ID and CID Group ID have to be "
-    "specified in request. Only specified roles are removed if specified in request payload, else association between "
-    "User Group and CID Group is dissolved completely (if no roles specified).",
+    "Delete links or additional roles between user groups and CID groups. User group ID and CID "
+    "group ID have to be specified in request. Only specified roles are removed if specified in "
+    "request payload, else association between User Group and CID group is dissolved completely (if no roles specified).",
     "mssp",
     [
       {
+        "description": "'user_group_id' and 'cid_group_id' fields are required. 'role_ids' "
+        "field is optional. Remaining fields are ignored.",
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
     "getUserGroupMembersByIDV1",
     "GET",
     "/mssp/entities/user-group-members/v1",
-    "Get user group members by user group ID.",
+    "Deprecated: Please use getUserGroupMembersByID. Get user group members by user group ID.",
     "mssp",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
@@ -339,32 +352,34 @@
       }
     ]
   ],
   [
     "addUserGroupMembers",
     "POST",
     "/mssp/entities/user-group-members/v1",
-    "Add new User Group member. Maximum 500 members allowed per User Group.",
+    "Add new user group member. Maximum 500 members allowed per user group.",
     "mssp",
     [
       {
+        "description": "Both 'user_group_id' and 'user_uuids' fields are required.",
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
     "deleteUserGroupMembers",
     "DELETE",
     "/mssp/entities/user-group-members/v1",
-    "Delete User Group members entry.",
+    "Delete user group members entry.",
     "mssp",
     [
       {
+        "description": "Both 'user_group_id' and 'user_uuids' fields are required.",
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
@@ -407,15 +422,15 @@
       }
     ]
   ],
   [
     "getUserGroupsByIDV1",
     "GET",
     "/mssp/entities/user-groups/v1",
-    "Get user groups by ID.",
+    "Deprecated: Please use getUserGroupsByID. Get user groups by ID.",
     "mssp",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
@@ -427,33 +442,39 @@
       }
     ]
   ],
   [
     "createUserGroups",
     "POST",
     "/mssp/entities/user-groups/v1",
-    "Create new User Group(s). Maximum 500 User Group(s) allowed per customer.",
+    "Create new user groups. Name is a required field but description is an optional field. "
+    "Maximum 500 user groups allowed per customer.",
     "mssp",
     [
       {
+        "description": "Only 'name' and/or 'description' fields are required. "
+        "Remaining are assigned by the system.",
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
     "updateUserGroups",
     "PATCH",
     "/mssp/entities/user-groups/v1",
-    "Update existing User Group(s). User Group ID is expected for each User Group definition provided in request body. "
-    "User Group member(s) remain unaffected.",
+    "Update existing user group(s). User group ID is expected for each user group definition "
+    "provided in request body. Name is a required field but description is an optional field. "
+    "Empty description will override existing value. User group member(s) remain unaffected.",
     "mssp",
     [
       {
+        "description": "'user_group_id' field is required to identify the user group to "
+        "update along with 'name' and/or 'description' fields to be updated.",
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
@@ -520,16 +541,23 @@
     "queryChildren",
     "GET",
     "/mssp/queries/children/v1",
     "Query for customers linked as children",
     "mssp",
     [
       {
+        "type": "string",
+        "description": "Filter using a query in Falcon Query Language (FQL). Supported filters: cid",
+        "name": "filter",
+        "in": "query"
+      },
+      {
         "enum": [
-          "last_modified_timestamp"
+          "last_modified_timestamp|asc",
+          "last_modified_timestamp|desc"
         ],
         "type": "string",
         "default": "last_modified_timestamp|desc",
         "description": "The sort expression used to sort the results",
         "name": "sort",
         "in": "query"
       },
@@ -590,27 +618,29 @@
       }
     ]
   ],
   [
     "queryCIDGroups",
     "GET",
     "/mssp/queries/cid-groups/v1",
-    "Query CID Groups.",
+    "Query CID groups.",
     "mssp",
     [
       {
         "type": "string",
         "description": "Name to lookup groups for",
         "name": "name",
         "in": "query"
       },
       {
         "enum": [
-          "last_modified_timestamp",
-          "name"
+          "last_modified_timestamp|asc",
+          "last_modified_timestamp|desc",
+          "name|asc",
+          "name|desc"
         ],
         "type": "string",
         "default": "name|asc",
         "description": "The sort expression used to sort the results",
         "name": "sort",
         "in": "query"
       },
@@ -620,25 +650,26 @@
         "description": "Starting index of overall result set from which to return ids",
         "name": "offset",
         "in": "query"
       },
       {
         "type": "integer",
         "default": 10,
-        "description": "Number of ids to return",
+        "description": "Maximum number of results to return",
         "name": "limit",
         "in": "query"
       }
     ]
   ],
   [
     "queryRoles",
     "GET",
     "/mssp/queries/mssp-roles/v1",
-    "Query MSSP Role assignment. At least one of CID Group ID or User Group ID should also be provided. Role ID is optional.",
+    "Query links between user groups and CID groups. At least one of CID group ID or user "
+    "group ID should also be provided. Role ID is optional.",
     "mssp",
     [
       {
         "type": "string",
         "description": "User group ID to fetch MSSP role for",
         "name": "user_group_id",
         "in": "query"
@@ -682,27 +713,28 @@
       }
     ]
   ],
   [
     "queryUserGroupMembers",
     "GET",
     "/mssp/queries/user-group-members/v1",
-    "Query User Group member by User UUID.",
+    "Query user group member by user UUID.",
     "mssp",
     [
       {
         "type": "string",
         "description": "User UUID to lookup associated user group ID",
         "name": "user_uuid",
         "in": "query",
         "required": True
       },
       {
         "enum": [
-          "last_modified_timestamp"
+          "last_modified_timestamp|asc",
+          "last_modified_timestamp|desc"
         ],
         "type": "string",
         "default": "last_modified_timestamp|desc",
         "description": "The sort expression used to sort the results",
         "name": "sort",
         "in": "query"
       },
@@ -722,27 +754,29 @@
       }
     ]
   ],
   [
     "queryUserGroups",
     "GET",
     "/mssp/queries/user-groups/v1",
-    "Query User Groups.",
+    "Query user groups.",
     "mssp",
     [
       {
         "type": "string",
         "description": "Name to lookup groups for",
         "name": "name",
         "in": "query"
       },
       {
         "enum": [
-          "last_modified_timestamp",
-          "name"
+          "last_modified_timestamp|asc",
+          "last_modified_timestamp|desc",
+          "name|asc",
+          "name|desc"
         ],
         "type": "string",
         "default": "name|asc",
         "description": "The sort expression used to sort the results",
         "name": "sort",
         "in": "query"
       },
@@ -752,14 +786,14 @@
         "description": "Starting index of overall result set from which to return ids",
         "name": "offset",
         "in": "query"
       },
       {
         "type": "integer",
         "default": 10,
-        "description": "Number of ids to return",
+        "description": "Maximum number of results to return",
         "name": "limit",
         "in": "query"
       }
     ]
   ]
 ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_oauth2.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,20 @@
     "POST",
     "/oauth2/revoke",
     "Revoke a previously issued OAuth2 access token before the end of its standard 30-minute lifespan.",
     "oauth2",
     [
       {
         "type": "string",
+        "description": "The OAuth2 client ID you are revoking the token for.",
+        "name": "client_id",
+        "in": "formData"
+      },
+      {
+        "type": "string",
         "description": "The OAuth2 access token you want to revoke.\n\nInclude your API "
         "client ID and secret in basic auth format (`Authorization: basic <encoded API client "
         "ID and secret>`) in your request header.",
         "name": "token",
         "in": "formData",
         "required": True
       }
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_ods.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ods.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,28 @@
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
 _ods_endpoints = [
   [
+    "aggregate_query_scan_host_metadata",
+    "POST",
+    "/ods/aggregates/scan-hosts/v1",
+    "Get aggregates on ODS scan-hosts data.",
+    "ods",
+    [
+      {
+        "name": "body",
+        "in": "body",
+        "required": True
+      }
+    ]
+  ],
+  [
     "aggregate_scans",
     "POST",
     "/ods/aggregates/scans/v1",
     "Get aggregates on ODS scan data.",
     "ods",
     [
       {
@@ -461,15 +475,15 @@
           "created_on|desc",
           "created_by|asc",
           "created_by|desc",
           "last_updated|asc",
           "last_updated|desc"
         ],
         "type": "string",
-        "default": "created_on|desc",
+        "default": "schedule.start_timestamp|desc",
         "description": "The property to sort on, followed by a |, followed by the sort direction, "
         "either \"asc\" or \"desc\"",
         "name": "sort",
         "in": "query",
         "allowEmptyValue": True
       }
     ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_overwatch_dashboard.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_prevention_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_prevention_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_quarantine.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_quick_scan.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_fdr.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,97 +32,121 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
-_quick_scan_endpoints = [
+_fdr_endpoints = [
   [
-    "GetScansAggregates",
-    "POST",
-    "/scanner/aggregates/scans/GET/v1",
-    "Get scans aggregations as specified via json in request body.",
-    "quick_scan",
-    [
-      {
-        "name": "body",
-        "in": "body",
-        "required": True
-      }
-    ]
+    "fdrschema_combined_event_get",
+    "GET",
+    "/fdr/combined/schema-members/v1",
+    "Fetch combined schema",
+    "event_schema",
+    []
   ],
   [
-    "GetScans",
+    "fdrschema_entities_event_get",
     "GET",
-    "/scanner/entities/scans/v1",
-    "Check the status of a volume scan. Time required for analysis increases with "
-    "the number of samples in a volume but usually it should take less than 1 minute",
-    "quick_scan",
+    "/fdr/entities/schema-events/v1",
+    "Fetch event schema by ID",
+    "event_schema",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
-        "collectionFormat": "csv",
-        "description": "ID of a submitted scan",
+        "collectionFormat": "multi",
+        "description": "Specify feed IDs to fetch",
         "name": "ids",
-        "in": "query",
-        "required": True
+        "in": "query"
+      }
+    ]
+  ],
+  [
+    "fdrschema_queries_event_get",
+    "GET",
+    "/fdr/queries/schema-events/v1",
+    "Get list of event IDs given a particular query.",
+    "event_schema",
+    [
+      {
+        "type": "integer",
+        "description": "Limit of the data",
+        "name": "limit",
+        "in": "query"
+      },
+      {
+        "type": "integer",
+        "description": "Offset into the data",
+        "name": "offset",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "FQL filter of the data",
+        "name": "filter",
+        "in": "query"
+      },
+      {
+        "type": "string",
+        "description": "Sort the data",
+        "name": "sort",
+        "in": "query"
       }
     ]
   ],
   [
-    "ScanSamples",
-    "POST",
-    "/scanner/entities/scans/v1",
-    "Submit a volume of files for ml scanning. Time required for analysis increases with the "
-    "number of samples in a volume but usually it should take less than 1 minute",
-    "quick_scan",
+    "fdrschema_entities_field_get",
+    "GET",
+    "/fdr/entities/schema-fields/v1",
+    "Fetch field schema by ID",
+    "field_schema",
     [
       {
-        "description": "Submit a batch of SHA256s for ml scanning. The samples must have been "
-        "previously uploaded through `/samples/entities/samples/v3`",
-        "name": "body",
-        "in": "body",
-        "required": True
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "Specify feed IDs to fetch",
+        "name": "ids",
+        "in": "query"
       }
     ]
   ],
   [
-    "QuerySubmissionsMixin0",
+    "fdrschema_queries_field_get",
     "GET",
-    "/scanner/queries/scans/v1",
-    "Find IDs for submitted scans by providing an FQL filter and paging details. "
-    "Returns a set of volume IDs that match your criteria.",
-    "quick_scan",
+    "/fdr/queries/schema-fields/v1",
+    "Get list of field IDs given a particular query.",
+    "field_schema",
     [
       {
-        "type": "string",
-        "description": "Optional filter and sort criteria in the form of an FQL query. "
-        "For more information about FQL queries, see [our FQL documentation in Falcon]"
-        "(https://falcon.crowdstrike.com/support/documentation/45/falcon-query-language-feature-guide).",
-        "name": "filter",
+        "type": "integer",
+        "description": "Limit of the data",
+        "name": "limit",
         "in": "query"
       },
       {
-        "type": "string",
-        "description": "The offset to start retrieving submissions from.",
+        "type": "integer",
+        "description": "Offset into the data",
         "name": "offset",
         "in": "query"
       },
       {
-        "type": "integer",
-        "description": "Maximum number of volume IDs to return. Max: 5000.",
-        "name": "limit",
+        "type": "string",
+        "description": "FQL filter of the data",
+        "name": "filter",
         "in": "query"
       },
       {
         "type": "string",
-        "description": "Sort order: `asc` or `desc`.",
+        "description": "Sort the data",
         "name": "sort",
         "in": "query"
       }
     ]
   ]
 ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_real_time_response.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_real_time_response_admin.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_recon.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_recon.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,14 +417,20 @@
           "type": "string"
         },
         "collectionFormat": "multi",
         "description": "IDs of rules.",
         "name": "ids",
         "in": "query",
         "required": True
+      },
+      {
+        "type": "boolean",
+        "description": "Whether we should delete the notifications generated by this rule or not",
+        "name": "notificationsDeletionRequested",
+        "in": "query"
       }
     ]
   ],
   [
     "QueryActionsV1",
     "GET",
     "/recon/queries/actions/v1",
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_report_executions.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_response_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_sample_uploads.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sample_uploads.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,20 +159,14 @@
     "/archives/entities/archives/v2",
     "Uploads an archive and extracts files list from it. Operation is asynchronous use `/archives/entities/archives/v1` "
     "to check the status. After uploading, use `/archives/entities/extractions/v1` to copy the file to internal storage "
     "making it available for content analysis.",
     "sample_uploads",
     [
       {
-        "description": "Source of archive.",
-        "name": "source",
-        "in": "formData",
-        "required": True
-      },
-      {
         "type": "file",
         "description": "Content of the uploaded archive. For example, use `--form file=@$FILE_PATH` when using cURL.",
         "name": "file",
         "in": "formData",
         "required": True
       },
       {
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_scheduled_reports.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_sensor_download.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_sensor_update_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_update_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,21 +58,37 @@
     "/policy/combined/sensor-update-builds/v1",
     "Retrieve available builds for use with Sensor Update Policies",
     "sensor_update_policies",
     [
       {
         "enum": [
           "linux",
+          "linuxarm64",
           "mac",
-          "windows"
+          "windows",
+          "zlinux"
         ],
         "type": "string",
         "description": "The platform to return builds for",
         "name": "platform",
         "in": "query"
+      },
+      {
+        "enum": [
+          "early_adopter",
+          "prod"
+        ],
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "csv",
+        "description": "The stages to return builds for",
+        "name": "stage",
+        "in": "query"
       }
     ]
   ],
   [
     "queryCombinedSensorUpdateKernels",
     "GET",
     "/policy/combined/sensor-update-kernels/v1",
@@ -89,18 +105,18 @@
         "minimum": 0,
         "type": "integer",
         "description": "The offset to start retrieving records from",
         "name": "offset",
         "in": "query"
       },
       {
-        "maximum": 5000,
+        "maximum": 500,
         "minimum": 1,
         "type": "integer",
-        "description": "The maximum records to return. [1-5000]",
+        "description": "The maximum records to return. [1-500]",
         "name": "limit",
         "in": "query"
       }
     ]
   ],
   [
     "queryCombinedSensorUpdatePolicyMembers",
@@ -261,17 +277,19 @@
     "/policy/entities/sensor-update-actions/v1",
     "Perform the specified action on the Sensor Update Policies specified in the request",
     "sensor_update_policies",
     [
       {
         "enum": [
           "add-host-group",
+          "add-rule-group",
           "disable",
           "enable",
-          "remove-host-group"
+          "remove-host-group",
+          "remove-rule-group"
         ],
         "type": "string",
         "description": "The action to perform",
         "name": "action_name",
         "in": "query",
         "required": True
       },
@@ -440,18 +458,18 @@
         "minimum": 0,
         "type": "integer",
         "description": "The offset to start retrieving records from",
         "name": "offset",
         "in": "query"
       },
       {
-        "maximum": 5000,
+        "maximum": 500,
         "minimum": 1,
         "type": "integer",
-        "description": "The maximum records to return. [1-5000]",
+        "description": "The maximum records to return. [1-500]",
         "name": "limit",
         "in": "query"
       }
     ]
   ],
   [
     "querySensorUpdatePolicyMembers",
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_tailored_intelligence.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_user_management.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_user_management.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,20 +64,16 @@
         "default": False,
         "description": "Specifies if to request direct Only role grants or all role grants "
         "between user and CID (specified in query params)",
         "name": "direct_only",
         "in": "query"
       },
       {
-        "enum": [
-          "role_id",
-          "role_name"
-        ],
         "type": "string",
-        "description": "The filter expression that should be used to limit the results",
+        "description": "Filter using a query in Falcon Query Language (FQL). Supported filters: role_id, role_name",
         "name": "filter",
         "in": "query"
       },
       {
         "minimum": 0,
         "type": "integer",
         "default": 0,
@@ -138,15 +134,16 @@
       }
     ]
   ],
   [
     "userActionV1",
     "POST",
     "/user-management/entities/user-actions/v1",
-    "Apply actions to one or more User. Available action names: reset_2fa, reset_password.",
+    "Apply actions to one or more User. Available action names: reset_2fa, reset_password. "
+    "User UUIDs can be provided in `ids` param as part of request payload.",
     "user_management",
     [
       {
         "description": "User UUIDs and Action Name params are required. Allowed values for "
         "Action Name param includes 'reset_2fa' and 'reset_password'",
         "name": "body",
         "in": "body",
@@ -269,36 +266,36 @@
       },
       {
         "type": "string",
         "description": "User UUID to get available roles for. Empty User UUID would returns all "
         "roles IDs available for customer.",
         "name": "user_uuid",
         "in": "query"
+      },
+      {
+        "type": "string",
+        "default": "grant",
+        "description": "Actionable purpose of the query",
+        "name": "action",
+        "in": "query"
       }
     ]
   ],
   [
     "queryUserV1",
     "GET",
     "/user-management/queries/users/v1",
     "List user IDs for all users in your customer account. For more information on each user, "
     "provide the user ID to `/user-management/entities/users/GET/v1`.",
     "user_management",
     [
       {
-        "enum": [
-          "assigned_cids",
-          "cid",
-          "first_name",
-          "last_name",
-          "name",
-          "uid"
-        ],
         "type": "string",
-        "description": "The filter expression that should be used to limit the results",
+        "description": "Filter using a query in Falcon Query Language (FQL). "
+        "Supported filters: assigned_cids, cid, first_name, last_name, name, uid",
         "name": "filter",
         "in": "query"
       },
       {
         "minimum": 0,
         "type": "integer",
         "default": 0,
@@ -313,16 +310,22 @@
         "default": 100,
         "description": "The maximum records to return. [1-500]",
         "name": "limit",
         "in": "query"
       },
       {
         "enum": [
+          "cid_name|asc",
+          "cid_name|desc",
+          "created_at|asc",
+          "created_at|desc",
           "first_name|asc",
           "first_name|desc",
+          "last_login_at|asc",
+          "last_login_at|desc",
           "last_name|asc",
           "last_name|desc",
           "name|asc",
           "name|desc",
           "uid|asc",
           "uid|desc"
         ],
@@ -334,15 +337,15 @@
       }
     ]
   ],
   [
     "GetRoles",
     "GET",
     "/user-roles/entities/user-roles/v1",
-    "Get info about a role",
+    "Deprecated : Please use entitiesRolesV1. Get info about a role",
     "user_management",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
@@ -355,15 +358,15 @@
       }
     ]
   ],
   [
     "GrantUserRoleIds",
     "POST",
     "/user-roles/entities/user-roles/v1",
-    "Assign one or more roles to a user",
+    "Deprecated : Please use userRolesActionV1. Assign one or more roles to a user",
     "user_management",
     [
       {
         "type": "string",
         "description": "ID of a user. Find a user's ID from `/users/entities/user/v1`.",
         "name": "user_uuid",
         "in": "query",
@@ -377,15 +380,15 @@
       }
     ]
   ],
   [
     "RevokeUserRoleIds",
     "DELETE",
     "/user-roles/entities/user-roles/v1",
-    "Revoke one or more roles from a user",
+    "Deprecated : Please use userRolesActionV1. Revoke one or more roles from a user",
     "user_management",
     [
       {
         "type": "string",
         "description": "ID of a user. Find a user's ID from `/users/entities/user/v1`.",
         "name": "user_uuid",
         "in": "query",
@@ -404,25 +407,25 @@
       }
     ]
   ],
   [
     "GetAvailableRoleIds",
     "GET",
     "/user-roles/queries/user-role-ids-by-cid/v1",
-    "Show role IDs for all roles available in your customer account. For more information on each role, "
-    "provide the role ID to `/customer/entities/roles/v1`.",
+    "Deprecated : Please use queriesRolesV1. Show role IDs for all roles available in your customer account. "
+    "For more information on each role, provide the role ID to `/customer/entities/roles/v1`.",
     "user_management",
     []
   ],
   [
     "GetUserRoleIds",
     "GET",
     "/user-roles/queries/user-role-ids-by-user-uuid/v1",
-    "Show role IDs of roles assigned to a user. For more information on each role, provide the role ID to "
-    "`/customer/entities/roles/v1`.",
+    "Deprecated : Please use combinedUserRolesV1. Show role IDs of roles assigned to a user. "
+    "For more information on each role, provide the role ID to `/customer/entities/roles/v1`.",
     "user_management",
     [
       {
         "type": "string",
         "description": "ID of a user. Find a user's ID from `/users/entities/user/v1`.",
         "name": "user_uuid",
         "in": "query",
@@ -430,15 +433,15 @@
       }
     ]
   ],
   [
     "RetrieveUser",
     "GET",
     "/users/entities/users/v1",
-    "Get info about a user",
+    "Deprecated : Please use retrieveUsersGETV1. Get info about a user",
     "user_management",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
@@ -450,15 +453,16 @@
       }
     ]
   ],
   [
     "CreateUser",
     "POST",
     "/users/entities/users/v1",
-    "Create a new user. After creating a user, assign one or more roles with POST /user-roles/entities/user-roles/v1",
+    "Deprecated : Please use createUserV1. Create a new user. After creating a user, assign one or more roles with "
+    "POST /user-roles/entities/user-roles/v1",
     "user_management",
     [
       {
         "description": "Attributes for this user. `uid` (required) is the user's email address, which is their username "
         "in Falcon.\n\nOptional attributes:\n\n<ul><li>`firstName`</li><li>`lastName`</li><li>`password`</li></ul>\n\n"
         "As a best practice, we recommend omitting `password`. If single sign-on is enabled for your customer account, "
         "the `password` attribute is ignored. If single sign-on is not enabled, we send a user activation request to their "
@@ -470,15 +474,15 @@
       }
     ]
   ],
   [
     "UpdateUser",
     "PATCH",
     "/users/entities/users/v1",
-    "Modify an existing user's first or last name",
+    "Deprecated : Please use updateUserV1. Modify an existing user's first or last name",
     "user_management",
     [
       {
         "type": "string",
         "description": "ID of a user. Find a user's ID from `/users/entities/user/v1`.",
         "name": "user_uuid",
         "in": "query",
@@ -492,15 +496,15 @@
       }
     ]
   ],
   [
     "DeleteUser",
     "DELETE",
     "/users/entities/users/v1",
-    "Delete a user permanently",
+    "Deprecated : Please use deleteUserV1. Delete a user permanently",
     "user_management",
     [
       {
         "type": "string",
         "description": "ID of a user. Find a user's ID from `/users/entities/user/v1`.",
         "name": "user_uuid",
         "in": "query",
@@ -508,32 +512,33 @@
       }
     ]
   ],
   [
     "RetrieveEmailsByCID",
     "GET",
     "/users/queries/emails-by-cid/v1",
-    "List the usernames (usually an email address) for all users in your customer account",
+    "Deprecated : Please use retrieveUsersGETV1. List the usernames (usually an email address) "
+    "for all users in your customer account",
     "user_management",
     []
   ],
   [
     "RetrieveUserUUIDsByCID",
     "GET",
     "/users/queries/user-uuids-by-cid/v1",
-    "List user IDs for all users in your customer account. For more information on each user, "
-    "provide the user ID to `/users/entities/user/v1`.",
+    "Deprecated : Please use queryUserV1. List user IDs for all users in your customer account. "
+    "For more information on each user, provide the user ID to `/users/entities/user/v1`.",
     "user_management",
     []
   ],
   [
     "RetrieveUserUUID",
     "GET",
     "/users/queries/user-uuids-by-email/v1",
-    "Get a user's ID by providing a username (usually an email address)",
+    "Deprecated : Please use queryUserV1. Get a user's ID by providing a username (usually an email address)",
     "user_management",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/_zero_trust_assessment.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_zero_trust_assessment.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,34 +34,14 @@
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
 _zero_trust_assessment_endpoints = [
   [
-    "getAssessmentV1",
-    "GET",
-    "/zero-trust-assessment/entities/assessments/v1",
-    "Get Zero Trust Assessment data for one or more hosts by providing agent IDs (AID) and a customer ID (CID).",
-    "zero_trust_assessment",
-    [
-      {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "multi",
-        "description": "One or more agent IDs, which you can find in the data.zta file, or the Falcon console.",
-        "name": "ids",
-        "in": "query",
-        "required": True
-      }
-    ]
-  ],
-  [
     "getComplianceV1",
     "GET",
     "/zero-trust-assessment/entities/audit/v1",
     "Get the Zero Trust Assessment compliance report for one customer ID (CID).",
     "zero_trust_assessment",
     []
   ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,33 +28,39 @@
 # |_____/|_____|   __|__| |_____|____|___._||____|_____|_____|          //          //..\\
 #              |__|                                                                UU    UU
 # The following operations reference legacy naming convention and are considered deprecated.
 # These operation IDs are maintained for backwards compatibility purposes only, Move all code
 # references to use the new operations IDs defined above that align with the IDs defined in
 # the service classes.
 from ._custom_ioa import _custom_ioa_endpoints
+from ._d4c_registration import _d4c_registration_endpoints
 from ._discover import _discover_endpoints
+from ._fdr import _fdr_endpoints
 from ._firewall_management import _firewall_management_endpoints
 from ._hosts import _hosts_endpoints
 from ._identity_protection import _identity_protection_endpoints
 from ._installation_tokens import _installation_tokens_endpoints
 from ._ioc import _ioc_endpoints
 from ._iocs import _iocs_endpoints
 from ._ods import _ods_endpoints
 from ._real_time_response import _real_time_response_endpoints
 from ._real_time_response_admin import _real_time_response_admin_endpoints
 from ._report_executions import _report_executions_endpoints
 from ._scheduled_reports import _scheduled_reports_endpoints
+from ._zero_trust_assessment import _zero_trust_assessment_endpoints
 
 _custom_ioa_deprecated = _custom_ioa_endpoints
+_d4c_registration_deprecated = _d4c_registration_endpoints
 _discover_deprecated = _discover_endpoints
+_fdr_deprecated = _fdr_endpoints
 _firewall_management_deprecated = _firewall_management_endpoints
 _hosts_deprecated = _hosts_endpoints
 _identity_protection_deprecated = _identity_protection_endpoints
 _installation_tokens_deprecated = _installation_tokens_endpoints
 _ioc_deprecated = _ioc_endpoints
 _iocs_deprecated = _iocs_endpoints
 _ods_deprecated = _ods_endpoints
 _real_time_response_deprecated = _real_time_response_endpoints
 _real_time_response_admin_deprecated = _real_time_response_admin_endpoints
 _report_executions_deprecated = _report_executions_endpoints
 _scheduled_reports_deprecated = _scheduled_reports_endpoints
+_zero_trust_assessment_deprecated = _zero_trust_assessment_endpoints
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_custom_ioa.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_discover.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_incidents.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,259 +32,222 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
-_discover_endpoints = [
+_incidents_endpoints = [
   [
-    "get-accounts",
+    "CrowdScore",
     "GET",
-    "/discover/entities/accounts/v1",
-    "Get details on accounts by providing one or more IDs.",
-    "discover",
+    "/incidents/combined/crowdscores/v1",
+    "Query environment wide CrowdScore and return the entity data",
+    "incidents",
     [
       {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "multi",
-        "description": "One or more account IDs (max: 100). Find account IDs with GET `/discover/queries/accounts/v1`",
-        "name": "ids",
-        "in": "query",
-        "required": True
+        "type": "string",
+        "description": "Optional filter and sort criteria in the form of an FQL query. "
+        "For more information about FQL queries, see [our FQL documentation in Falcon]"
+        "(https://falcon.crowdstrike.com/support/documentation/45/falcon-query-language-feature-guide).",
+        "name": "filter",
+        "in": "query"
+      },
+      {
+        "type": "integer",
+        "description": "Starting index of overall result set from which to return ids.",
+        "name": "offset",
+        "in": "query"
+      },
+      {
+        "type": "integer",
+        "description": "The maximum records to return. [1-2500]",
+        "name": "limit",
+        "in": "query"
+      },
+      {
+        "enum": [
+          "adjusted_score.asc",
+          "adjusted_score.desc",
+          "score.asc",
+          "score.desc",
+          "timestamp.asc",
+          "timestamp.desc"
+        ],
+        "type": "string",
+        "description": "The property to sort on, followed by a dot (.), "
+        "followed by the sort direction, either \"asc\" or \"desc\".",
+        "name": "sort",
+        "in": "query"
       }
     ]
   ],
   [
-    "get-applications",
-    "GET",
-    "/discover/entities/applications/v1",
-    "Get details on applications by providing one or more IDs.",
-    "discover",
+    "GetBehaviors",
+    "POST",
+    "/incidents/entities/behaviors/GET/v1",
+    "Get details on behaviors by providing behavior IDs",
+    "incidents",
     [
       {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "multi",
-        "description": "The IDs of applications to retrieve. (Min: 1, Max: 100)",
-        "name": "ids",
-        "in": "query",
+        "name": "body",
+        "in": "body",
         "required": True
       }
     ]
   ],
   [
-    "get-hosts",
-    "GET",
-    "/discover/entities/hosts/v1",
-    "Get details on assets by providing one or more IDs.",
-    "discover",
+    "PerformIncidentAction",
+    "POST",
+    "/incidents/entities/incident-actions/v1",
+    "Perform a set of actions on one or more incidents, such as adding tags or comments "
+    "or updating the incident name or description",
+    "incidents",
     [
       {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "multi",
-        "description": "One or more asset IDs (max: 100). Find asset IDs with GET `/discover/queries/hosts/v1`",
-        "name": "ids",
-        "in": "query",
+        "type": "boolean",
+        "default": False,
+        "description": "If true, update assigned-to-uuid and or status of detections associated with "
+        "the incident(s). Defaults to false",
+        "name": "update_detects",
+        "in": "query"
+      },
+      {
+        "type": "boolean",
+        "default": False,
+        "description": "If true and update-detects is true, the assigned-to-uuid or status for ALL "
+        "detections associated with the incident(s) will be overwritten. If false, only detects that "
+        "have default values for assigned-to-uuid and/or status will be updated. Defaults to false. "
+        "Ignored if 'update-detects' is missing or false.",
+        "name": "overwrite_detects",
+        "in": "query"
+      },
+      {
+        "description": "Incident Update request body containing minimum 1 and maximum 5000 Incident ID(s) "
+        "and action param(s) to be performed action against.",
+        "name": "body",
+        "in": "body",
         "required": True
       }
     ]
   ],
   [
-    "get-logins",
-    "GET",
-    "/discover/entities/logins/v1",
-    "Get details on logins by providing one or more IDs.",
-    "discover",
+    "GetIncidents",
+    "POST",
+    "/incidents/entities/incidents/GET/v1",
+    "Get details on incidents by providing incident IDs",
+    "incidents",
     [
       {
-        "type": "array",
-        "items": {
-          "type": "string"
-        },
-        "collectionFormat": "multi",
-        "description": "One or more login IDs (max: 100). Find login IDs with GET `/discover/queries/logins/v1`",
-        "name": "ids",
-        "in": "query",
+        "name": "body",
+        "in": "body",
         "required": True
       }
     ]
   ],
   [
-    "query-accounts",
+    "QueryBehaviors",
     "GET",
-    "/discover/queries/accounts/v1",
-    "Search for accounts in your environment by providing an FQL (Falcon Query Language) filter and paging details. "
-    "Returns a set of account IDs which match the filter criteria.",
-    "discover",
+    "/incidents/queries/behaviors/v1",
+    "Search for behaviors by providing an FQL filter, sorting, and paging details",
+    "incidents",
     [
       {
-        "minimum": 0,
-        "type": "integer",
-        "description": "An offset used with the `limit` parameter to manage pagination of results. On your first request, "
-        "don’t provide an `offset`. On subsequent requests, provide the `offset` from the previous response to continue "
-        "from that place in the results.",
-        "name": "offset",
-        "in": "query"
-      },
-      {
-        "maximum": 100,
-        "minimum": 1,
-        "type": "integer",
-        "description": "The number of account IDs to return in this response (min: 1, max: 100, default: 100). "
-        "Use with the `offset` parameter to manage pagination of results.",
-        "name": "limit",
-        "in": "query"
-      },
-      {
-        "type": "string",
-        "description": "Sort accounts by their properties. A single sort field is allowed. Common sort options include:"
-        "\n\n<ul><li>username|asc</li><li>last_failed_login_timestamp|desc</li></ul>",
-        "name": "sort",
-        "in": "query"
-      },
-      {
         "type": "string",
-        "description": "Filter accounts using an FQL query. Common filter options include:\n\n<ul><li>"
-        "account_type:'Local'</li><li>admin_privileges:'Yes'</li><li>first_seen_timestamp:<'now-7d'</li>"
-        "<li>last_successful_login_type:'Terminal server'</li></ul>",
+        "description": "Optional filter and sort criteria in the form of an FQL query. "
+        "For more information about FQL queries, see [our FQL documentation in Falcon]"
+        "(https://falcon.crowdstrike.com/support/documentation/45/falcon-query-language-feature-guide).",
         "name": "filter",
         "in": "query"
-      }
-    ]
-  ],
-  [
-    "query-applications",
-    "GET",
-    "/discover/queries/applications/v1",
-    "Search for applications in your environment by providing an FQL filter and paging details. "
-    "returns a set of application IDs which match the filter criteria.",
-    "discover",
-    [
+      },
       {
-        "minimum": 0,
         "type": "integer",
-        "description": "The index of the starting resource.",
+        "description": "Starting index of overall result set from which to return ids.",
         "name": "offset",
         "in": "query"
       },
       {
-        "maximum": 100,
-        "minimum": 1,
         "type": "integer",
-        "description": "The number of account IDs to return in this response (min: 1, max: 100, default: 100). "
-        "Use with the `offset` parameter to manage pagination of results.",
+        "description": "The maximum records to return. [1-500]",
         "name": "limit",
         "in": "query"
       },
       {
+        "enum": [
+          "cmdline.asc",
+          "cmdline.desc",
+          "detection_ids.asc",
+          "detection_ids.desc",
+          "display_name.asc",
+          "display_name.desc",
+          "domain.asc",
+          "domain.desc",
+          "filepath.asc",
+          "filepath.desc",
+          "timestamp.asc",
+          "timestamp.desc"
+        ],
         "type": "string",
-        "description": "Sort accounts by their properties. A single sort field is allowed. "
-        "Common sort options include:\n\n<ul><li>username|asc</li><li>last_failed_login_timestamp|desc</li></ul>",
+        "description": "The property to sort on, followed by a dot (.), "
+        "followed by the sort direction, either \"asc\" or \"desc\".",
         "name": "sort",
         "in": "query"
-      },
-      {
-        "type": "string",
-        "description": "Filter accounts using an FQL query. Common filter options include:\n\n"
-        "<ul><li>account_type:'Local'</li><li>admin_privileges:'Yes'</li><li>first_seen_timestamp:<'now-7d'</li>"
-        "<li>last_successful_login_type:'Terminal server'</li></ul>",
-        "name": "filter",
-        "in": "query"
       }
     ]
   ],
   [
-    "query-hosts",
+    "QueryIncidents",
     "GET",
-    "/discover/queries/hosts/v1",
-    "Search for assets in your environment by providing an FQL (Falcon Query Language) filter and paging details. "
-    "Returns a set of asset IDs which match the filter criteria.",
-    "discover",
-    [
-      {
-        "minimum": 0,
-        "type": "integer",
-        "description": "An offset used with the `limit` parameter to manage pagination of results. "
-        "On your first request, don’t provide an `offset`. On subsequent requests, provide the `offset` "
-        "from the previous response to continue from that place in the results.",
-        "name": "offset",
-        "in": "query"
-      },
-      {
-        "maximum": 100,
-        "minimum": 1,
-        "type": "integer",
-        "description": "The number of asset IDs to return in this response (min: 1, max: 100, default: 100). "
-        "Use with the `offset` parameter to manage pagination of results.",
-        "name": "limit",
-        "in": "query"
-      },
-      {
+    "/incidents/queries/incidents/v1",
+    "Search for incidents by providing an FQL filter, sorting, and paging details",
+    "incidents",
+    [
+      {
+        "enum": [
+          "assigned_to.asc",
+          "assigned_to.desc",
+          "assigned_to_name.asc",
+          "assigned_to_name.desc",
+          "end.asc",
+          "end.desc",
+          "modified_timestamp.asc",
+          "modified_timestamp.desc",
+          "name.asc",
+          "name.desc",
+          "sort_score.asc",
+          "sort_score.desc",
+          "start.asc",
+          "start.desc",
+          "state.asc",
+          "state.desc",
+          "status.asc",
+          "status.desc"
+        ],
         "type": "string",
-        "description": "Sort assets by their properties. A single sort field is allowed. "
-        "Common sort options include:\n\n<ul><li>hostname|asc</li><li>product_type_desc|desc</li></ul>",
+        "description": "The property to sort on, followed by a dot (.), "
+        "followed by the sort direction, either \"asc\" or \"desc\".",
         "name": "sort",
         "in": "query"
       },
       {
         "type": "string",
-        "description": "Filter assets using an FQL query. Common filter options include:\n\n"
-        "<ul><li>entity_type:'managed'</li><li>product_type_desc:'Workstation'</li>"
-        "<li>platform_name:'Windows'</li><li>last_seen_timestamp:>'now-7d'</li></ul>",
+        "description": "Optional filter and sort criteria in the form of an FQL query. "
+        "For more information about FQL queries, see [our FQL documentation in Falcon]"
+        "(https://falcon.crowdstrike.com/support/documentation/45/falcon-query-language-feature-guide).",
         "name": "filter",
         "in": "query"
-      }
-    ]
-  ],
-  [
-    "query-logins",
-    "GET",
-    "/discover/queries/logins/v1",
-    "Search for logins in your environment by providing an FQL (Falcon Query Language) filter and paging details. "
-    "Returns a set of login IDs which match the filter criteria.",
-    "discover",
-    [
+      },
       {
-        "minimum": 0,
         "type": "integer",
-        "description": "An offset used with the `limit` parameter to manage pagination of results. "
-        "On your first request, don’t provide an `offset`. On subsequent requests, provide the `offset` "
-        "from the previous response to continue from that place in the results.",
+        "description": "Starting index of overall result set from which to return ids.",
         "name": "offset",
         "in": "query"
       },
       {
-        "maximum": 100,
-        "minimum": 1,
         "type": "integer",
-        "description": "The number of asset IDs to return in this response (min: 1, max: 100, default: 100). "
-        "Use with the `offset` parameter to manage pagination of results.",
+        "description": "The maximum records to return. [1-500]",
         "name": "limit",
         "in": "query"
-      },
-      {
-        "type": "string",
-        "description": "Sort assets by their properties. A single sort field is allowed. "
-        "Common sort options include:\n\n<ul><li>hostname|asc</li><li>product_type_desc|desc</li></ul>",
-        "name": "sort",
-        "in": "query"
-      },
-      {
-        "type": "string",
-        "description": "Filter assets using an FQL query. Common filter options include:\n\n"
-        "<ul><li>entity_type:'managed'</li><li>product_type_desc:'Workstation'</li><li>platform_name:'Windows'"
-        "</li><li>last_seen_timestamp:>'now-7d'</li></ul>",
-        "name": "filter",
-        "in": "query"
       }
     ]
   ]
 ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_firewall_management.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_hosts.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_identity_protection.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_installation_tokens.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_ioc.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_ods.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,383 +32,474 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
-_ioc_endpoints = [
+_ods_endpoints = [
   [
-    "indicator.aggregate.v1",
+    "aggregate-query-scan-host-metadata",
     "POST",
-    "/iocs/aggregates/indicators/v1",
-    "Get Indicators aggregates as specified via json in the request body.",
-    "ioc",
+    "/ods/aggregates/scan-hosts/v1",
+    "Get aggregates on ODS scan-hosts data.",
+    "ods",
     [
       {
-        "type": "string",
-        "description": "The filter to narrow down the aggregation data",
-        "name": "filter",
-        "in": "query"
-      },
+        "name": "body",
+        "in": "body",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "aggregate-scans",
+    "POST",
+    "/ods/aggregates/scans/v1",
+    "Get aggregates on ODS scan data.",
+    "ods",
+    [
       {
-        "type": "boolean",
-        "description": "The filter for returning either only indicators for the request customer or its MSSP parents",
-        "name": "from_parent",
-        "in": "query"
-      },
+        "name": "body",
+        "in": "body",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "aggregate-scheduled-scans",
+    "POST",
+    "/ods/aggregates/scheduled-scans/v1",
+    "Get aggregates on ODS scheduled-scan data.",
+    "ods",
+    [
       {
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
-    "indicator.combined.v1",
+    "get-malicious-files-by-ids",
     "GET",
-    "/iocs/combined/indicator/v1",
-    "Get Combined for Indicators.",
-    "ioc",
+    "/ods/entities/malicious-files/v1",
+    "Get malicious files by ids.",
+    "ods",
     [
       {
-        "type": "string",
-        "description": "The filter expression that should be used to limit the results.",
-        "name": "filter",
-        "in": "query"
-      },
-      {
-        "type": "integer",
-        "description": "The offset to start retrieving records from. Offset and After params are mutually exclusive. "
-        "If none provided then scrolling will be used by default.",
-        "name": "offset",
-        "in": "query"
-      },
-      {
-        "type": "integer",
-        "description": "The maximum records to return.",
-        "name": "limit",
-        "in": "query"
-      },
-      {
-        "enum": [
-          "action",
-          "applied_globally",
-          "metadata.av_hits",
-          "metadata.company_name.raw",
-          "created_by",
-          "created_on",
-          "expiration",
-          "expired",
-          "metadata.filename.raw",
-          "modified_by",
-          "modified_on",
-          "metadata.original_filename.raw",
-          "metadata.product_name.raw",
-          "metadata.product_version",
-          "severity_number",
-          "source",
-          "type",
-          "value"
-        ],
-        "type": "string",
-        "description": "The sort expression that should be used to sort the results.",
-        "name": "sort",
-        "in": "query"
-      },
-      {
-        "type": "string",
-        "description": "A pagination token used with the `limit` parameter to manage pagination of results. "
-        "On your first request, don't provide an 'after' token. On subsequent requests, provide the 'after' "
-        "token from the previous response to continue from that place in the results. "
-        "To access more than 10k indicators, use the 'after' parameter instead of 'offset'.",
-        "name": "after",
-        "in": "query"
-      },
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "The scan IDs to retrieve the scan entities",
+        "name": "ids",
+        "in": "query",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "cancel-scans",
+    "POST",
+    "/ods/entities/scan-control-actions/cancel/v1",
+    "Cancel ODS scans for the given scan ids.",
+    "ods",
+    [
       {
-        "type": "boolean",
-        "description": "The filter for returning either only indicators for the request customer or its MSSP parents",
-        "name": "from_parent",
-        "in": "query"
+        "name": "body",
+        "in": "body",
+        "required": True
       }
     ]
   ],
   [
-    "action.get.v1",
+    "get-scan-host-metadata-by-ids",
     "GET",
-    "/iocs/entities/actions/v1",
-    "Get Actions by ids.",
-    "ioc",
+    "/ods/entities/scan-hosts/v1",
+    "Get scan hosts by ids.",
+    "ods",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
-        "collectionFormat": "csv",
-        "description": "The ids of the Actions to retrieve",
+        "collectionFormat": "multi",
+        "description": "The scan IDs to retrieve the scan entities",
         "name": "ids",
-        "in": "query"
+        "in": "query",
+        "required": True
       }
     ]
   ],
   [
-    "indicator.get.v1",
+    "scans-report",
+    "POST",
+    "/ods/entities/scans-reports/v1",
+    "Launch a scans report creation job",
+    "ods",
+    [
+      {
+        "name": "body",
+        "in": "body",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "get-scans-by-scan-ids",
     "GET",
-    "/iocs/entities/indicators/v1",
-    "Get Indicators by ids.",
-    "ioc",
+    "/ods/entities/scans/v1",
+    "Get Scans by IDs.",
+    "ods",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
-        "collectionFormat": "csv",
-        "description": "The ids of the Indicators to retrieve",
+        "collectionFormat": "multi",
+        "description": "The scan IDs to retrieve the scan entities",
         "name": "ids",
         "in": "query",
         "required": True
       }
     ]
   ],
   [
-    "indicator.create.v1",
+    "create-scan",
     "POST",
-    "/iocs/entities/indicators/v1",
-    "Create Indicators.",
-    "ioc",
+    "/ods/entities/scans/v1",
+    "Create ODS scan and start or schedule scan for the given scan request.",
+    "ods",
     [
       {
-        "type": "boolean",
-        "description": "Whether to submit to retrodetects",
-        "name": "retrodetects",
-        "in": "query"
-      },
-      {
-        "type": "boolean",
-        "default": False,
-        "description": "Set to true to ignore warnings and add all IOCs",
-        "name": "ignore_warnings",
-        "in": "query"
-      },
-      {
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
-    "indicator.update.v1",
-    "PATCH",
-    "/iocs/entities/indicators/v1",
-    "Update Indicators.",
-    "ioc",
+    "get-scheduled-scans-by-scan-ids",
+    "GET",
+    "/ods/entities/scheduled-scans/v1",
+    "Get ScheduledScans by IDs.",
+    "ods",
     [
       {
-        "type": "boolean",
-        "description": "Whether to submit to retrodetects",
-        "name": "retrodetects",
-        "in": "query"
-      },
-      {
-        "type": "boolean",
-        "default": False,
-        "description": "Set to true to ignore warnings and add all IOCs",
-        "name": "ignore_warnings",
-        "in": "query"
-      },
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "The scan IDs to retrieve the scan entities",
+        "name": "ids",
+        "in": "query",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "schedule-scan",
+    "POST",
+    "/ods/entities/scheduled-scans/v1",
+    "Create ODS scan and start or schedule scan for the given scan request.",
+    "ods",
+    [
       {
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
-    "indicator.delete.v1",
+    "delete-scheduled-scans",
     "DELETE",
-    "/iocs/entities/indicators/v1",
-    "Delete Indicators by ids.",
-    "ioc",
+    "/ods/entities/scheduled-scans/v1",
+    "Delete ODS scheduled-scans for the given scheduled-scan ids.",
+    "ods",
     [
       {
-        "type": "string",
-        "description": "The FQL expression to delete Indicators in bulk. If both 'filter' and 'ids' are provided, "
-        "then filter takes precedence and ignores ids.",
-        "name": "filter",
-        "in": "query"
-      },
-      {
         "type": "array",
         "items": {
           "type": "string"
         },
-        "collectionFormat": "csv",
-        "description": "The ids of the Indicators to delete. If both 'filter' and 'ids' are provided, "
-        "then filter takes precedence and ignores ids",
+        "collectionFormat": "multi",
+        "description": "The scan IDs to retrieve the scan entities",
         "name": "ids",
-        "in": "query"
+        "in": "query",
+        "required": True
       },
       {
         "type": "string",
-        "description": "The comment why these indicators were deleted",
-        "name": "comment",
-        "in": "query"
-      },
-      {
-        "type": "boolean",
-        "description": "The filter for returning either only indicators for the request customer or its MSSP parents",
-        "name": "from_parent",
+        "description": "A FQL compatible query string.",
+        "name": "filter",
         "in": "query"
       }
     ]
   ],
   [
-    "action.query.v1",
+    "query-malicious-files",
     "GET",
-    "/iocs/queries/actions/v1",
-    "Query Actions.",
-    "ioc",
+    "/ods/queries/malicious-files/v1",
+    "Query malicious files.",
+    "ods",
     [
       {
         "type": "string",
-        "description": "Starting index of overall result set from which to return ids.",
+        "description": "A FQL compatible query string. Terms: [id cid scan_id host_id "
+        "host_scan_id filepath filename hash pattern_id severity quarantined last_updated]",
+        "name": "filter",
+        "in": "query",
+        "allowEmptyValue": True
+      },
+      {
+        "type": "integer",
+        "default": 0,
+        "description": "Index of the starting resource",
         "name": "offset",
         "in": "query"
       },
       {
         "type": "integer",
-        "description": "Number of ids to return.",
+        "default": 500,
+        "description": "The max number of resources to return",
         "name": "limit",
         "in": "query"
+      },
+      {
+        "enum": [
+          "id|asc",
+          "id|desc",
+          "scan_id|asc",
+          "scan_id|desc",
+          "host_id|asc",
+          "host_id|desc",
+          "host_scan_id|asc",
+          "host_scan_id|desc",
+          "filename|asc",
+          "filename|desc",
+          "hash|asc",
+          "hash|desc",
+          "pattern_id|asc",
+          "pattern_id|desc",
+          "severity|asc",
+          "severity|desc",
+          "last_updated|asc",
+          "last_updated|desc"
+        ],
+        "type": "string",
+        "default": "last_updated|desc",
+        "description": "The property to sort on, followed by a |, followed by the sort direction, "
+        "either \"asc\" or \"desc\"",
+        "name": "sort",
+        "in": "query",
+        "allowEmptyValue": True
       }
     ]
   ],
   [
-    "indicator.search.v1",
+    "query-scan-host-metadata",
     "GET",
-    "/iocs/queries/indicators/v1",
-    "Search for Indicators.",
-    "ioc",
+    "/ods/queries/scan-hosts/v1",
+    "Query scan hosts.",
+    "ods",
     [
       {
         "type": "string",
-        "description": "The filter expression that should be used to limit the results.",
+        "description": "A FQL compatible query string. Terms: [id cid profile_id host_id scan_id "
+        "host_scan_id filecount.scanned filecount.malicious filecount.quarantined "
+        "filecount.skipped affected_hosts_count status severity completed_on started_on "
+        "last_updated]",
         "name": "filter",
-        "in": "query"
+        "in": "query",
+        "allowEmptyValue": True
       },
       {
         "type": "integer",
-        "description": "The offset to start retrieving records from. Offset and After params are mutually exclusive. "
-        "If none provided then scrolling will be used by default.",
+        "default": 0,
+        "description": "Index of the starting resource",
         "name": "offset",
         "in": "query"
       },
       {
         "type": "integer",
-        "description": "The maximum records to return.",
+        "default": 500,
+        "description": "The max number of resources to return",
         "name": "limit",
         "in": "query"
       },
       {
         "enum": [
-          "action",
-          "applied_globally",
-          "metadata.av_hits",
-          "metadata.company_name.raw",
-          "created_by",
-          "created_on",
-          "expiration",
-          "expired",
-          "metadata.filename.raw",
-          "modified_by",
-          "modified_on",
-          "metadata.original_filename.raw",
-          "metadata.product_name.raw",
-          "metadata.product_version",
-          "severity_number",
-          "source",
-          "type",
-          "value"
+          "id|asc",
+          "id|desc",
+          "scan_id|asc",
+          "scan_id|desc",
+          "host_id|asc",
+          "host_id|desc",
+          "filecount.scanned|asc",
+          "filecount.scanned|desc",
+          "filecount.malicious|asc",
+          "filecount.malicious|desc",
+          "filecount.quarantined|asc",
+          "filecount.quarantined|desc",
+          "filecount.skipped|asc",
+          "filecount.skipped|desc",
+          "status|asc",
+          "status|desc",
+          "severity|asc",
+          "severity|desc",
+          "started_on|asc",
+          "started_on|desc",
+          "completed_on|asc",
+          "completed_on|desc",
+          "last_updated|asc",
+          "last_updated|desc"
         ],
         "type": "string",
-        "description": "The sort expression that should be used to sort the results.",
+        "default": "last_updated|desc",
+        "description": "The property to sort on, followed by a |, followed by the sort direction, "
+        "either \"asc\" or \"desc\"",
         "name": "sort",
-        "in": "query"
-      },
-      {
-        "type": "string",
-        "description": "A pagination token used with the `limit` parameter to manage pagination of results. "
-        "On your first request, don't provide an 'after' token. On subsequent requests, provide the 'after' "
-        "token from the previous response to continue from that place in the results. "
-        "To access more than 10k indicators, use the 'after' parameter instead of 'offset'.",
-        "name": "after",
-        "in": "query"
+        "in": "query",
+        "allowEmptyValue": True
       }
     ]
   ],
   [
-    "ioc_type.query.v1",
+    "query-scans",
     "GET",
-    "/iocs/queries/ioc-types/v1",
-    "Query IOC Types.",
-    "ioc",
+    "/ods/queries/scans/v1",
+    "Query Scans.",
+    "ods",
     [
       {
         "type": "string",
-        "description": "Starting index of overall result set from which to return ids.",
-        "name": "offset",
-        "in": "query"
+        "description": "A FQL compatible query string. Terms: [id cid profile_id "
+        "description.keyword initiated_from filecount.scanned filecount.malicious "
+        "filecount.quarantined filecount.skipped affected_hosts_count status severity "
+        "scan_started_on scan_completed_on created_on created_by last_updated]",
+        "name": "filter",
+        "in": "query",
+        "allowEmptyValue": True
       },
       {
         "type": "integer",
-        "description": "Number of ids to return.",
-        "name": "limit",
-        "in": "query"
-      }
-    ]
-  ],
-  [
-    "platform.query.v1",
-    "GET",
-    "/iocs/queries/platforms/v1",
-    "Query Platforms.",
-    "ioc",
-    [
-      {
-        "type": "string",
-        "description": "Starting index of overall result set from which to return ids.",
+        "default": 0,
+        "description": "Index of the starting resource",
         "name": "offset",
         "in": "query"
       },
       {
         "type": "integer",
-        "description": "Number of ids to return.",
+        "default": 500,
+        "description": "The max number of resources to return",
         "name": "limit",
         "in": "query"
+      },
+      {
+        "enum": [
+          "id|asc",
+          "id|desc",
+          "initiated_from|asc",
+          "initiated_from|desc",
+          "description.keyword|asc",
+          "description.keyword|desc",
+          "filecount.scanned|asc",
+          "filecount.scanned|desc",
+          "filecount.malicious|asc",
+          "filecount.malicious|desc",
+          "filecount.quarantined|asc",
+          "filecount.quarantined|desc",
+          "filecount.skipped|asc",
+          "filecount.skipped|desc",
+          "affected_hosts_count|asc",
+          "affected_hosts_count|desc",
+          "status|asc",
+          "status|desc",
+          "severity|asc",
+          "severity|desc",
+          "scan_started_on|asc",
+          "scan_started_on|desc",
+          "scan_completed_on|asc",
+          "scan_completed_on|desc",
+          "created_on|asc",
+          "created_on|desc",
+          "created_by|asc",
+          "created_by|desc",
+          "last_updated|asc",
+          "last_updated|desc"
+        ],
+        "type": "string",
+        "default": "created_on|desc",
+        "description": "The property to sort on, followed by a |, followed by the sort direction, "
+        "either \"asc\" or \"desc\"",
+        "name": "sort",
+        "in": "query",
+        "allowEmptyValue": True
       }
     ]
   ],
   [
-    "severity.query.v1",
+    "query-scheduled-scans",
     "GET",
-    "/iocs/queries/severities/v1",
-    "Query Severities.",
-    "ioc",
+    "/ods/queries/scheduled-scans/v1",
+    "Query ScheduledScans.",
+    "ods",
     [
       {
         "type": "string",
-        "description": "Starting index of overall result set from which to return ids.",
+        "description": "A FQL compatible query string. Terms: [id cid description initiated_from "
+        "status schedule.start_timestamp schedule.Interval created_on created_by last_updated "
+        "deleted]",
+        "name": "filter",
+        "in": "query",
+        "allowEmptyValue": True
+      },
+      {
+        "type": "integer",
+        "default": 0,
+        "description": "Index of the starting resource",
         "name": "offset",
         "in": "query"
       },
       {
         "type": "integer",
-        "description": "Number of ids to return.",
+        "default": 500,
+        "description": "The max number of resources to return",
         "name": "limit",
         "in": "query"
+      },
+      {
+        "enum": [
+          "id|asc",
+          "id|desc",
+          "description.keyword|asc",
+          "description.keyword|desc",
+          "status|asc",
+          "status|desc",
+          "schedule.start_timestamp|asc",
+          "schedule.start_timestamp|desc",
+          "schedule.interval|asc",
+          "schedule.interval|desc",
+          "created_on|asc",
+          "created_on|desc",
+          "created_by|asc",
+          "created_by|desc",
+          "last_updated|asc",
+          "last_updated|desc"
+        ],
+        "type": "string",
+        "default": "schedule.start_timestamp|desc",
+        "description": "The property to sort on, followed by a |, followed by the sort direction, "
+        "either \"asc\" or \"desc\"",
+        "name": "sort",
+        "in": "query",
+        "allowEmptyValue": True
       }
     ]
   ]
 ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_iocs.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_ods.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_d4c_registration.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,460 +32,533 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
-_ods_endpoints = [
+_d4c_registration_endpoints = [
   [
-    "aggregate-scans",
-    "POST",
-    "/ods/aggregates/scans/v1",
-    "Get aggregates on ODS scan data.",
-    "ods",
+    "GetD4CAwsAccount",
+    "GET",
+    "/cloud-connect-aws/entities/account/v2",
+    "Returns information about the current status of an AWS account.",
+    "d4c_registration",
     [
       {
-        "name": "body",
-        "in": "body",
-        "required": True
+        "maxLength": 4,
+        "minLength": 3,
+        "pattern": "^(full|dry)$",
+        "type": "string",
+        "description": "Type of scan, dry or full, to perform on selected accounts",
+        "name": "scan-type",
+        "in": "query"
+      },
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "AWS account IDs",
+        "name": "ids",
+        "in": "query"
+      },
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "AWS organization IDs",
+        "name": "organization-ids",
+        "in": "query"
+      },
+      {
+        "pattern": "^(provisioned|operational)$",
+        "type": "string",
+        "description": "Account status to filter results by.",
+        "name": "status",
+        "in": "query"
+      },
+      {
+        "maxLength": 3,
+        "minLength": 1,
+        "type": "integer",
+        "default": 100,
+        "description": "The maximum records to return. Defaults to 100.",
+        "name": "limit",
+        "in": "query"
+      },
+      {
+        "type": "integer",
+        "description": "The offset to start retrieving records from",
+        "name": "offset",
+        "in": "query"
+      },
+      {
+        "pattern": "^(true|false)$",
+        "enum": [
+          "false",
+          "true"
+        ],
+        "type": "string",
+        "description": "Only return migrated d4c accounts",
+        "name": "migrated",
+        "in": "query"
       }
     ]
   ],
   [
-    "aggregate-scheduled-scans",
+    "CreateD4CAwsAccount",
     "POST",
-    "/ods/aggregates/scheduled-scans/v1",
-    "Get aggregates on ODS scheduled-scan data.",
-    "ods",
+    "/cloud-connect-aws/entities/account/v2",
+    "Creates a new account in our system for a customer and generates a script "
+    "for them to run in their AWS cloud environment to grant us access.",
+    "d4c_registration",
     [
       {
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
-    "get-malicious-files-by-ids",
-    "GET",
-    "/ods/entities/malicious-files/v1",
-    "Get malicious files by ids.",
-    "ods",
+    "DeleteD4CAwsAccount",
+    "DELETE",
+    "/cloud-connect-aws/entities/account/v2",
+    "Deletes an existing AWS account or organization in our system.",
+    "d4c_registration",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
         "collectionFormat": "multi",
-        "description": "The scan IDs to retrieve the scan entities",
+        "description": "AWS account IDs to remove",
         "name": "ids",
-        "in": "query",
-        "required": True
+        "in": "query"
+      },
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "AWS organization IDs to remove",
+        "name": "organization-ids",
+        "in": "query"
       }
     ]
   ],
   [
-    "cancel-scans",
-    "POST",
-    "/ods/entities/scan-control-actions/cancel/v1",
-    "Cancel ODS scans for the given scan ids.",
-    "ods",
+    "GetD4CAwsConsoleSetupURLs",
+    "GET",
+    "/cloud-connect-aws/entities/console-setup-urls/v1",
+    "Return a URL for customer to visit in their cloud environment to grant "
+    "us access to their AWS environment.",
+    "d4c_registration",
     [
       {
-        "name": "body",
-        "in": "body",
-        "required": True
+        "pattern": "^[0-9a-z-]{2,}$",
+        "type": "string",
+        "description": "Region",
+        "name": "region",
+        "in": "query"
       }
     ]
   ],
   [
-    "get-scan-host-metadata-by-ids",
+    "GetD4CAWSAccountScriptsAttachment",
     "GET",
-    "/ods/entities/scan-hosts/v1",
-    "Get scan hosts by ids.",
-    "ods",
+    "/cloud-connect-aws/entities/user-scripts-download/v1",
+    "Return a script for customer to run in their cloud environment to grant "
+    "us access to their AWS environment as a downloadable attachment.",
+    "d4c_registration",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
         "collectionFormat": "multi",
-        "description": "The scan IDs to retrieve the scan entities",
+        "description": "AWS account IDs",
         "name": "ids",
-        "in": "query",
-        "required": True
-      }
-    ]
-  ],
-  [
-    "scans-report",
-    "POST",
-    "/ods/entities/scans-reports/v1",
-    "Launch a scans report creation job",
-    "ods",
-    [
-      {
-        "name": "body",
-        "in": "body",
-        "required": True
+        "in": "query"
       }
     ]
   ],
   [
-    "get-scans-by-scan-ids",
+    "GetDiscoverCloudAzureAccount",
     "GET",
-    "/ods/entities/scans/v1",
-    "Get Scans by IDs.",
-    "ods",
+    "/cloud-connect-azure/entities/account/v1",
+    "Return information about Azure account registration",
+    "d4c_registration",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
         "collectionFormat": "multi",
-        "description": "The scan IDs to retrieve the scan entities",
+        "description": "SubscriptionIDs of accounts to select for this status operation. "
+        "If this is empty then all accounts are returned.",
         "name": "ids",
-        "in": "query",
-        "required": True
+        "in": "query"
+      },
+      {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "Tenant ids to filter azure accounts",
+        "name": "tenant_ids",
+        "in": "query"
+      },
+      {
+        "maxLength": 4,
+        "minLength": 3,
+        "pattern": "^(full|dry)$",
+        "type": "string",
+        "description": "Type of scan, dry or full, to perform on selected accounts",
+        "name": "scan-type",
+        "in": "query"
+      },
+      {
+        "pattern": "^(provisioned|operational)$",
+        "type": "string",
+        "description": "Account status to filter results by.",
+        "name": "status",
+        "in": "query"
+      },
+      {
+        "maxLength": 3,
+        "minLength": 1,
+        "type": "integer",
+        "default": 100,
+        "description": "The maximum records to return. Defaults to 100.",
+        "name": "limit",
+        "in": "query"
+      },
+      {
+        "type": "integer",
+        "description": "The offset to start retrieving records from",
+        "name": "offset",
+        "in": "query"
       }
     ]
   ],
   [
-    "create-scan",
+    "CreateDiscoverCloudAzureAccount",
     "POST",
-    "/ods/entities/scans/v1",
-    "Create ODS scan and start or schedule scan for the given scan request.",
-    "ods",
+    "/cloud-connect-azure/entities/account/v1",
+    "Creates a new account in our system for a customer and generates a script for them to run "
+    "in their cloud environment to grant us access.",
+    "d4c_registration",
     [
       {
         "name": "body",
         "in": "body",
         "required": True
       }
     ]
   ],
   [
-    "get-scheduled-scans-by-scan-ids",
+    "UpdateDiscoverCloudAzureAccountClientID",
+    "PATCH",
+    "/cloud-connect-azure/entities/client-id/v1",
+    "Update an Azure service account in our system by with the user-created client_id "
+    "created with the public key we've provided",
+    "d4c_registration",
+    [
+      {
+        "maxLength": 36,
+        "minLength": 36,
+        "pattern": "^[0-9a-z-]{36}$",
+        "type": "string",
+        "description": "ClientID to use for the Service Principal associated with the customer's Azure account",
+        "name": "id",
+        "in": "query",
+        "required": True
+      },
+      {
+        "maxLength": 36,
+        "minLength": 36,
+        "pattern": "^[0-9a-z-]{36}$",
+        "type": "string",
+        "description": "Object ID to use for the Service Principal associated with the customer's Azure account",
+        "name": "object_id",
+        "in": "query"
+      },
+      {
+        "maxLength": 36,
+        "minLength": 36,
+        "pattern": "^[0-9a-z-]{36}$",
+        "type": "string",
+        "description": "Tenant ID to update client ID for. Required if multiple tenants are registered.",
+        "name": "tenant-id",
+        "in": "query"
+      }
+    ]
+  ],
+  [
+    "DiscoverCloudAzureDownloadCertificate",
     "GET",
-    "/ods/entities/scheduled-scans/v1",
-    "Get ScheduledScans by IDs.",
-    "ods",
+    "/cloud-connect-azure/entities/download-certificate/v1",
+    "Returns JSON object(s) that contain the base64 encoded certificate for a service principal.",
+    "d4c_registration",
     [
       {
         "type": "array",
         "items": {
+          "maxLength": 36,
+          "minLength": 36,
+          "pattern": "^[0-9a-z-]{36}$",
           "type": "string"
         },
         "collectionFormat": "multi",
-        "description": "The scan IDs to retrieve the scan entities",
-        "name": "ids",
+        "description": "Azure Tenant ID",
+        "name": "tenant_id",
         "in": "query",
         "required": True
+      },
+      {
+        "type": "boolean",
+        "default": False,
+        "description": "Setting to true will invalidate the current certificate and generate a new certificate",
+        "name": "refresh",
+        "in": "query"
+      },
+      {
+        "maxLength": 2,
+        "minLength": 1,
+        "pattern": "^[0-9]{1,2}$",
+        "type": "string",
+        "description": "Years the certificate should be valid (only used when refresh=true)",
+        "name": "years_valid",
+        "in": "query"
       }
     ]
   ],
   [
-    "schedule-scan",
-    "POST",
-    "/ods/entities/scheduled-scans/v1",
-    "Create ODS scan and start or schedule scan for the given scan request.",
-    "ods",
-    [
-      {
-        "name": "body",
-        "in": "body",
-        "required": True
-      }
-    ]
+    "GetDiscoverCloudAzureTenantIDs",
+    "GET",
+    "/cloud-connect-azure/entities/tenant-id/v1",
+    "Return available tenant ids for discover for cloud",
+    "d4c_registration",
+    []
   ],
   [
-    "delete-scheduled-scans",
-    "DELETE",
-    "/ods/entities/scheduled-scans/v1",
-    "Delete ODS scheduled-scans for the given scheduled-scan ids.",
-    "ods",
+    "GetDiscoverCloudAzureUserScriptsAttachment",
+    "GET",
+    "/cloud-connect-azure/entities/user-scripts-download/v1",
+    "Return a script for customer to run in their cloud environment to grant us access to their "
+    "Azure environment as a downloadable attachment",
+    "d4c_registration",
     [
       {
         "type": "array",
         "items": {
           "type": "string"
         },
-        "collectionFormat": "multi",
-        "description": "The scan IDs to retrieve the scan entities",
-        "name": "ids",
+        "collectionFormat": "csv",
+        "description": "Azure Tenant ID",
+        "name": "tenant-id",
         "in": "query",
         "required": True
       },
       {
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "csv",
+        "description": "Azure Subscription ID",
+        "name": "subscription_ids",
+        "in": "query"
+      },
+      {
         "type": "string",
-        "description": "A FQL compatible query string.",
-        "name": "filter",
+        "description": "Template to be rendered",
+        "name": "template",
         "in": "query"
       }
     ]
   ],
   [
-    "query-malicious-files",
+    "GetDiscoverCloudAzureUserScripts",
+    "GET",
+    "/cloud-connect-azure/entities/user-scripts/v1",
+    "Return a script for customer to run in their cloud environment to grant us access to their "
+    "Azure environment",
+    "d4c_registration",
+    []
+  ],
+  [
+    "GetD4CCGPAccount",
     "GET",
-    "/ods/queries/malicious-files/v1",
-    "Query malicious files.",
-    "ods",
+    "/cloud-connect-gcp/entities/account/v1",
+    "Returns information about the current status of an GCP account.",
+    "d4c_registration",
     [
       {
+        "enum": [
+          "Folder",
+          "Organization",
+          "Project"
+        ],
         "type": "string",
-        "description": "A FQL compatible query string. Terms: [id cid scan_id host_id "
-        "host_scan_id filepath filename hash pattern_id severity quarantined last_updated]",
-        "name": "filter",
-        "in": "query",
-        "allowEmptyValue": True
-      },
-      {
-        "type": "integer",
-        "default": 0,
-        "description": "Index of the starting resource",
-        "name": "offset",
+        "description": "GCP Hierarchy Parent Type, organization/folder/project",
+        "name": "parent_type",
         "in": "query"
       },
       {
-        "type": "integer",
-        "default": 500,
-        "description": "The max number of resources to return",
-        "name": "limit",
+        "type": "array",
+        "items": {
+          "type": "string"
+        },
+        "collectionFormat": "multi",
+        "description": "Hierarchical Resource IDs of accounts",
+        "name": "ids",
         "in": "query"
       },
       {
         "enum": [
-          "id|asc",
-          "id|desc",
-          "scan_id|asc",
-          "scan_id|desc",
-          "host_id|asc",
-          "host_id|desc",
-          "host_scan_id|asc",
-          "host_scan_id|desc",
-          "filename|asc",
-          "filename|desc",
-          "hash|asc",
-          "hash|desc",
-          "pattern_id|asc",
-          "pattern_id|desc",
-          "severity|asc",
-          "severity|desc",
-          "last_updated|asc",
-          "last_updated|desc"
+          "dry",
+          "full"
         ],
         "type": "string",
-        "default": "last_updated|desc",
-        "description": "The property to sort on, followed by a |, followed by the sort direction, "
-        "either \"asc\" or \"desc\"",
-        "name": "sort",
-        "in": "query",
-        "allowEmptyValue": True
-      }
-    ]
-  ],
-  [
-    "query-scan-host-metadata",
-    "GET",
-    "/ods/queries/scan-hosts/v1",
-    "Query scan hosts.",
-    "ods",
-    [
+        "description": "Type of scan, dry or full, to perform on selected accounts",
+        "name": "scan-type",
+        "in": "query"
+      },
       {
+        "enum": [
+          "operational",
+          "provisioned"
+        ],
         "type": "string",
-        "description": "A FQL compatible query string. Terms: [id cid profile_id host_id scan_id "
-        "host_scan_id filecount.scanned filecount.malicious filecount.quarantined "
-        "filecount.skipped affected_hosts_count status severity completed_on started_on "
-        "last_updated]",
-        "name": "filter",
-        "in": "query",
-        "allowEmptyValue": True
+        "description": "Account status to filter results by.",
+        "name": "status",
+        "in": "query"
       },
       {
+        "maxLength": 3,
+        "minLength": 1,
         "type": "integer",
-        "default": 0,
-        "description": "Index of the starting resource",
-        "name": "offset",
+        "default": 100,
+        "description": "The maximum records to return. Defaults to 100.",
+        "name": "limit",
         "in": "query"
       },
       {
         "type": "integer",
-        "default": 500,
-        "description": "The max number of resources to return",
-        "name": "limit",
+        "description": "The offset to start retrieving records from",
+        "name": "offset",
         "in": "query"
       },
       {
-        "enum": [
-          "id|asc",
-          "id|desc",
-          "scan_id|asc",
-          "scan_id|desc",
-          "host_id|asc",
-          "host_id|desc",
-          "filecount.scanned|asc",
-          "filecount.scanned|desc",
-          "filecount.malicious|asc",
-          "filecount.malicious|desc",
-          "filecount.quarantined|asc",
-          "filecount.quarantined|desc",
-          "filecount.skipped|asc",
-          "filecount.skipped|desc",
-          "status|asc",
-          "status|desc",
-          "severity|asc",
-          "severity|desc",
-          "started_on|asc",
-          "started_on|desc",
-          "completed_on|asc",
-          "completed_on|desc",
-          "last_updated|asc",
-          "last_updated|desc"
-        ],
         "type": "string",
-        "default": "last_updated|desc",
-        "description": "The property to sort on, followed by a |, followed by the sort direction, "
-        "either \"asc\" or \"desc\"",
+        "description": "Order fields in ascending or descending order. Ex: parent_type|asc.",
         "name": "sort",
-        "in": "query",
-        "allowEmptyValue": True
+        "in": "query"
       }
     ]
   ],
   [
-    "query-scans",
-    "GET",
-    "/ods/queries/scans/v1",
-    "Query Scans.",
-    "ods",
+    "CreateD4CGCPAccount",
+    "POST",
+    "/cloud-connect-gcp/entities/account/v1",
+    "Creates a new account in our system for a customer and generates a new service account for them "
+    "to add access to in their GCP environment to grant us access.",
+    "d4c_registration",
     [
       {
-        "type": "string",
-        "description": "A FQL compatible query string. Terms: [id cid profile_id "
-        "description.keyword initiated_from filecount.scanned filecount.malicious "
-        "filecount.quarantined filecount.skipped affected_hosts_count status severity "
-        "scan_started_on scan_completed_on created_on created_by last_updated]",
-        "name": "filter",
-        "in": "query",
-        "allowEmptyValue": True
-      },
-      {
-        "type": "integer",
-        "default": 0,
-        "description": "Index of the starting resource",
-        "name": "offset",
-        "in": "query"
-      },
-      {
-        "type": "integer",
-        "default": 500,
-        "description": "The max number of resources to return",
-        "name": "limit",
-        "in": "query"
-      },
+        "name": "body",
+        "in": "body",
+        "required": True
+      }
+    ]
+  ],
+  [
+    "GetCSPMGCPUserScriptsAttachment",
+    "GET",
+    "/cloud-connect-gcp/entities/user-scripts-download/v1",
+    "Return a script for customer to run in their cloud environment to grant us access to their "
+    "GCP environment as a downloadable attachment",
+    "d4c_registration",
+    []
+  ],
+  [
+    "GetD4CGCPUserScripts",
+    "GET",
+    "/cloud-connect-gcp/entities/user-scripts/v1",
+    "Return a script for customer to run in their cloud environment to grant us access to their "
+    "GCP environment",
+    "d4c_registration",
+    [
       {
         "enum": [
-          "id|asc",
-          "id|desc",
-          "initiated_from|asc",
-          "initiated_from|desc",
-          "description.keyword|asc",
-          "description.keyword|desc",
-          "filecount.scanned|asc",
-          "filecount.scanned|desc",
-          "filecount.malicious|asc",
-          "filecount.malicious|desc",
-          "filecount.quarantined|asc",
-          "filecount.quarantined|desc",
-          "filecount.skipped|asc",
-          "filecount.skipped|desc",
-          "affected_hosts_count|asc",
-          "affected_hosts_count|desc",
-          "status|asc",
-          "status|desc",
-          "severity|asc",
-          "severity|desc",
-          "scan_started_on|asc",
-          "scan_started_on|desc",
-          "scan_completed_on|asc",
-          "scan_completed_on|desc",
-          "created_on|asc",
-          "created_on|desc",
-          "created_by|asc",
-          "created_by|desc",
-          "last_updated|asc",
-          "last_updated|desc"
+          "Folder",
+          "Organization",
+          "Project"
         ],
         "type": "string",
-        "default": "created_on|desc",
-        "description": "The property to sort on, followed by a |, followed by the sort direction, "
-        "either \"asc\" or \"desc\"",
-        "name": "sort",
-        "in": "query",
-        "allowEmptyValue": True
+        "description": "GCP Hierarchy Parent Type, organization/folder/project",
+        "name": "parent_type",
+        "in": "query"
       }
     ]
   ],
   [
-    "query-scheduled-scans",
+    "GetHorizonD4CScripts",
     "GET",
-    "/ods/queries/scheduled-scans/v1",
-    "Query ScheduledScans.",
-    "ods",
+    "/settings-discover/entities/gen/scripts/v1",
+    "Returns static install scripts for Horizon.",
+    "d4c_registration",
     [
       {
+        "pattern": "^(true|false)$",
+        "enum": [
+          "false",
+          "true"
+        ],
         "type": "string",
-        "description": "A FQL compatible query string. Terms: [id cid description initiated_from "
-        "status schedule.start_timestamp schedule.Interval created_on created_by last_updated "
-        "deleted]",
-        "name": "filter",
-        "in": "query",
-        "allowEmptyValue": True
+        "description": "Get static script for single account",
+        "name": "single_account",
+        "in": "query"
       },
       {
-        "type": "integer",
-        "default": 0,
-        "description": "Index of the starting resource",
-        "name": "offset",
+        "pattern": "^o-[0-9a-z]{10,32}$",
+        "type": "string",
+        "description": "AWS organization ID",
+        "name": "organization-id",
         "in": "query"
       },
       {
-        "type": "integer",
-        "default": 500,
-        "description": "The max number of resources to return",
-        "name": "limit",
+        "pattern": "^(true|false)$",
+        "enum": [
+          "false",
+          "true"
+        ],
+        "type": "string",
+        "name": "delete",
         "in": "query"
       },
       {
+        "pattern": "^(commercial|gov)$",
         "enum": [
-          "id|asc",
-          "id|desc",
-          "description.keyword|asc",
-          "description.keyword|desc",
-          "status|asc",
-          "status|desc",
-          "schedule.start_timestamp|asc",
-          "schedule.start_timestamp|desc",
-          "schedule.interval|asc",
-          "schedule.interval|desc",
-          "created_on|asc",
-          "created_on|desc",
-          "created_by|asc",
-          "created_by|desc",
-          "last_updated|asc",
-          "last_updated|desc"
+          "commercial",
+          "gov"
         ],
         "type": "string",
-        "default": "created_on|desc",
-        "description": "The property to sort on, followed by a |, followed by the sort direction, "
-        "either \"asc\" or \"desc\"",
-        "name": "sort",
-        "in": "query",
-        "allowEmptyValue": True
+        "description": "Account type (e.g.: commercial,gov) Only applicable when "
+        "registering AWS commercial account in a Gov environment",
+        "name": "account_type",
+        "in": "query"
       }
     ]
   ]
 ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_real_time_response.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_report_executions.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_enum/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_enum/_base_url.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_enum/_container_base_url.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_container_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_enum/_token_fail_reason.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_token_fail_reason.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_error/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,23 +44,26 @@
     KeywordsOnly,
     InvalidCredentials,
     APIError,
     CannotRevokeToken,
     FunctionalityNotImplemented,
     InvalidBaseURL,
     PayloadValidationError,
-    FeatureNotSupportedByPythonVersion
+    FeatureNotSupportedByPythonVersion,
+    InvalidIndex,
+    InvalidCredentialFormat
     )
 from ._warnings import (
     SDKWarning,
     SSLDisabledWarning,
     NoContentWarning,
     NoAuthenticationMechanism
 )
 
 
 __all__ = ["SDKError", "RegionSelectError", "InvalidMethod", "InvalidOperation",
            "TokenNotSpecified", "KeywordsOnly", "SDKWarning", "SSLDisabledWarning",
            "InvalidCredentials", "APIError", "NoContentWarning", "CannotRevokeToken",
            "FunctionalityNotImplemented", "InvalidBaseURL", "PayloadValidationError",
-           "NoAuthenticationMechanism", "FeatureNotSupportedByPythonVersion"
+           "NoAuthenticationMechanism", "FeatureNotSupportedByPythonVersion",
+           "InvalidIndex", "InvalidCredentialFormat"
            ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_error/_exceptions.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/_exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,7 +164,19 @@
     _code = 426
 
 
 class APIError(SDKError):
     """Generic error received back from the API."""
 
     _message = "An unexpected error has occurred. Please check your payloads and try again."
+
+
+class InvalidIndex(SDKError):
+    """Item ID was not found in the list or string."""
+
+    _message = "Item not found. Check your index and try again."
+
+
+class InvalidCredentialFormat(SDKError):
+    """Credentials dictionary was provided as a datatype that will not convert to a dictionary."""
+
+    _message = "Invalid credential format. This keyword must be provided as a dictionary."
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_error/_warnings.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/_warnings.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_log/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_log/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_log/_facility.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_log/_facility.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,29 @@
     recon_action_update_payload,
     recon_rules_payload,
     recon_notifications_payload,
     recon_rule_preview_payload,
     recon_export_job_payload
     )
 from ._malquery import malquery_exact_search_payload, malquery_hunt_payload, malquery_fuzzy_payload
-from ._container import image_payload
+from ._container import image_payload, registry_payload
 from ._detects import update_detects_payload
 from ._incidents import incident_action_parameters
 from ._ioa import ioa_exclusion_payload, ioa_custom_payload
 from ._prevention_policy import prevention_policy_payload
 from ._sensor_update_policy import sensor_policy_payload
 from ._response_policy import response_policy_payload
 from ._real_time_response import command_payload, data_payload
 from ._cloud_connect_aws import aws_registration_payload
 from ._ioc import indicator_payload, indicator_update_payload, indicator_report_payload
-from ._d4c_registration import azure_registration_payload, aws_d4c_registration_payload
+from ._d4c_registration import (
+    azure_registration_payload,
+    aws_d4c_registration_payload,
+    gcp_registration_payload
+    )
 from ._cspm_registration import cspm_registration_payload, cspm_policy_payload, cspm_scan_payload
 from ._device_control_policy import device_policy_payload, default_device_policy_config_payload
 from ._falconx import falconx_payload
 from ._mssp import mssp_payload
 from ._firewall import (
     firewall_policy_payload,
     firewall_container_payload,
@@ -82,9 +86,10 @@
     "mssp_payload", "ioa_custom_payload", "firewall_policy_payload", "firewall_container_payload",
     "firewall_rule_group_payload", "firewall_rule_group_update_payload", "reports_payload",
     "activity_payload", "case_payload", "incident_action_parameters", "update_alerts_payload",
     "firewall_rule_group_validation_payload", "firewall_filepattern_payload",
     "aws_d4c_registration_payload", "image_payload", "indicator_report_payload",
     "extraction_payload", "simple_action_parameter", "network_locations_metadata_payload",
     "network_locations_create_payload", "scheduled_scan_payload", "token_settings_payload",
-    "recon_export_job_payload", "default_device_policy_config_payload"
+    "recon_export_job_payload", "default_device_policy_config_payload", "registry_payload",
+    "gcp_registration_payload"
 ]
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_alerts.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_cloud_connect_aws.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_container.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_detects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Internal payload handling library - Falcon Container Payloads.
+"""Internal payload handling library - Detects.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -33,35 +33,40 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
 
-def image_payload(passed_keywords: dict) -> dict:
-    """Create a properly formatted image vulnerability request payload.
+def update_detects_payload(current_payload: dict, passed_keywords: dict) -> dict:
+    """Update the provided payload with any viable parameters provided as keywords.
 
     {
-        "osversion": "string",
-        "packages": [
-            {
-                "LayerHash": "string",
-                "LayerIndex": 0,
-                "MajorVersion": "string",
-                "PackageHash": "string",
-                "PackageProvider": "string",
-                "PackageSource": "string",
-                "Product": "string",
-                "SoftwareArchitecture": "string",
-                "Status": "string",
-                "Vendor": "string"
-            }
+        "assigned_to_uuid": "string",
+        "comment": "string",
+        "ids": [
+            "string"
+        ],
+        "new_behaviors_processed": [
+            "string"
         ]
+        "show_in_ui": true,
+        "status": "string"
     }
     """
-    returned_payload = {}
-    keys = ["osversion", "packages"]
+    keys = ["assigned_to_uuid", "comment", "status"]
     for key in keys:
         if passed_keywords.get(key, None):
-            returned_payload[key] = passed_keywords.get(key)
+            current_payload[key] = passed_keywords.get(key, None)
 
-    return returned_payload
+    if passed_keywords.get("show_in_ui", None) is not None:
+        current_payload["show_in_ui"] = passed_keywords.get("show_in_ui", None)
+
+    list_keys = ["ids", "new_behaviors_processed"]
+    for key in list_keys:
+        if passed_keywords.get(key, None):
+            provided = passed_keywords.get(key, None)
+            if isinstance(provided, str):
+                provided = provided.split(",")
+            current_payload[key] = provided
+
+    return current_payload
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_cspm_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_real_time_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Internal payload handling library - CSPM Registration (Horizon) Payloads.
+"""Internal payload handling library - Real Time Response.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -31,103 +31,90 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-from typing import Dict, List, Union
 
 
-def cspm_registration_payload(passed_keywords: dict) -> Dict[str, List[Dict[str, str]]]:
-    """Create a properly formatted CSPM registration payload.
+def command_payload(passed_keywords: dict) -> dict:  # pylint: disable=R0912  # noqa: C901
+    """Create a properly formatted payload for RTR command.
 
     {
-        "resources": [
-            {
-                "account_id": "string",
-                "cloudtrail_region": "string",
-                "organization_id": "string",
-                "tenant_id": "string",
-                "subscription_id": "string"
-            }
+        "base_command": "string",
+        "batch_id": "string",
+        "command_string": "string",
+        "optional_hosts": [
+            "string"
+        ],
+        "file_path": "string",
+        "persist_all": true,
+        "existing_batch_id": "string",
+        "host_ids": [
+            "string"
+        ],
+        "queue_offline": true,
+        "hosts_to_remove": [
+            "string"
         ]
+        "device_id": "string",
+        "id": integer,
+        "persist": boolean,
+        "session_id": "string",
+        "origin": "string"
     }
     """
-    returned_payload: Dict[str, List[Dict[str, str]]] = {}
-    returned_payload["resources"] = []
-    item = {}
-    keys = ["account_id", "cloudtrail_region", "organization_id", "tenant_id", "subscription_id"]
+    # flake8 / pylint both complain about complexity due to the number of if statements.
+    # Ignoring the complaint as this is just running through the potential passed keywords.
+    returned_payload = {}
+
+    keys = [
+        "base_command", "batch_id", "command_string", "file_path",
+        "existing_batch_id", "device_id", "session_id", "origin"
+        ]
     for key in keys:
         if passed_keywords.get(key, None):
-            item[key] = passed_keywords.get(key, None)
+            returned_payload[key] = passed_keywords.get(key, None)
 
-    returned_payload["resources"].append(item)
+    bool_keys = ["persist_all", "queue_offline", "persist"]
+    for boolean in bool_keys:
+        if passed_keywords.get(boolean, None) is not None:
+            returned_payload[boolean] = passed_keywords.get(boolean, None)
+
+    if passed_keywords.get("id", -1) > -1:
+        returned_payload["id"] = passed_keywords.get("id", None)
+
+    list_keys = ["optional_hosts", "host_ids", "hosts_to_remove"]
+    for list_key in list_keys:
+        passed_list = passed_keywords.get(list_key, None)
+        if passed_list:
+            if isinstance(passed_list, str):
+                passed_list = passed_list.split(",")
+            returned_payload[list_key] = passed_list
 
     return returned_payload
 
 
-def cspm_policy_payload(passed_keywords: dict) -> Dict[str, List[Dict[str, Union[str, bool, List[str]]]]]:
-    """Create a properly formatted CSPM policy update payload.
+def data_payload(passed_keywords: dict) -> dict:
+    """Create a properly formatted formData payload for RTR file uploads.
 
     {
-    "resources": [
-        {
-            "account_id": "string",
-            "enabled": boolean,
-            "policy_id": integer,
-            "regions": [
-                "string"
-            ],
-            "severity": "string",
-            "tag_excluded": boolean
-        }
-    ]
+        "id": "string",
+        "description": "string",
+        "name": "string",
+        "comments_for_audit_log": "string",
+        "content": "string",
+        "platform": "string",
+        "permission_type": "string"
     }
     """
-    returned_payload: Dict[str, List[Dict[str, Union[str, bool, List[str]]]]] = {}
-    returned_payload["resources"] = []
-    item = {}
-    if passed_keywords.get("account_id", None):
-        item["account_id"] = passed_keywords.get("account_id", None)
-    if passed_keywords.get("enabled", None) is not None:
-        item["enabled"] = passed_keywords.get("enabled", None)
-    if passed_keywords.get("policy_id", -1) > 0:
-        item["policy_id"] = passed_keywords.get("policy_id", None)
-    if passed_keywords.get("severity", None):
-        item["severity"] = passed_keywords.get("severity", None)
-    if passed_keywords.get("tag_excluded", None) is not None:
-        item["tag_excluded"] = passed_keywords.get("tag_excluded", None)
-    region_list = passed_keywords.get("regions", None)
-    if region_list:
-        if isinstance(region_list, str):
-            region_list = region_list.split(",")
-        item["regions"] = region_list
-
-    returned_payload["resources"].append(item)
-
-    return returned_payload
-
-
-def cspm_scan_payload(passed_keywords: dict) -> Dict[str, List[Dict[str, str]]]:
-    """Create a properly formmatted CSPM scan schedule payload.
-
-    {
-        "resources": [
-            {
-                "cloud_platform": "string",
-                "next_scan_timestamp": "2021-10-25T05:22:27.365Z",
-                "scan_schedule": "string"
-            }
+    returned_payload = {}
+    keys = [
+        "id", "description", "name", "comments_for_audit_log",
+        "content", "platform", "permission_type"
         ]
-    }
-    """
-    returned_payload: Dict[str, List[Dict[str, str]]] = {}
-    returned_payload["resources"] = []
-    item = {}
-    for key in ["cloud_platform", "next_scan_timestamp", "scan_schedule"]:
+    for key in keys:
         if passed_keywords.get(key, None):
-            item[key] = passed_keywords.get(key, None)
-
-    returned_payload["resources"].append(item)
+            returned_payload[key] = passed_keywords.get(key, None)
 
     return returned_payload
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_d4c_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_mssp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Internal payload handling library - D4C Registration Payloads.
+"""Internal payload handling library - Falcon Flight Control (MSSP).
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -31,63 +31,48 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-from typing import Dict, List, Union, Any
 
 
-def aws_d4c_registration_payload(passed_keywords: dict) -> Dict[str, List[Dict[str, Union[str, bool]]]]:
-    """Create a properly formatted AWS registration payload.
+def mssp_payload(passed_keywords: dict) -> dict:
+    """Create a properly formatted Flight Control payload.
 
     {
         "resources": [
             {
-                "account_id": "string",
-                "account_type": "string",
-                "cloudtrail_region": "string",
-                "is_master": true,
-                "organization_id": "string"
+                "cid": "string",
+                "cid_group_id": "string",
+                "description": "string",
+                "name": "string"
+                "id": "string",
+                "role_ids": [
+                    "string"
+                ],
+                "user_group_id": "string"
             }
         ]
     }
     """
-    returned_payload: Dict[str, List[Dict[str, Union[str, bool]]]] = {}
-    returned_payload["resources"] = []
-    keys = ["account_id", "account_type", "cloudtrail_region", "organization_id"]
-    item: Dict[str, Any] = {}
+    returned_payload = {}
+    resources_item = {}
+    keys = [
+        "cid", "cid_group_id", "description", "name", "id",
+        "user_group_id", "user_uuids"
+        ]
     for key in keys:
-        if isinstance(passed_keywords.get(key, None), str):
-            item[key] = passed_keywords.get(key)
-    if isinstance(passed_keywords.get("is_master", None), bool):
-        item["is_master"] = passed_keywords.get("is_master")
-
-    if item:
-        returned_payload["resources"].append(item)
-
-    return returned_payload
-
+        if passed_keywords.get(key, None):
+            resources_item[key] = passed_keywords.get(key, None)
 
-def azure_registration_payload(passed_keywords: dict) -> Dict[str, List[Dict[str, str]]]:
-    """Create a properly formatted Azure registration payload.
+    passed_role_ids = passed_keywords.get("role_ids", None)
+    if passed_role_ids:
+        if isinstance(passed_role_ids, str):
+            passed_role_ids = passed_role_ids.split(",")
+        resources_item["role_ids"] = passed_role_ids
 
-    {
-        "resources": [
-            {
-                "subscription_id": "string",
-                "tenant_id": "string"
-            }
-        ]
-    }
-    """
-    returned_payload: Dict[str, List[Dict[str, str]]] = {}
-    returned_payload["resources"] = []
-    item: Dict[str, str] = {}
-    if passed_keywords.get("subscription_id", None):
-        item["subscription_id"] = passed_keywords.get("subscription_id", None)
-    if passed_keywords.get("tenant_id", None):
-        item["tenant_id"] = passed_keywords.get("tenant_id", None)
-    returned_payload["resources"].append(item)
+    if resources_item:
+        returned_payload["resources"] = [resources_item]
 
     return returned_payload
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_detects.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_reports.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Internal payload handling library - Detects.
+"""Internal payload handling library - Reports Payloads.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -31,37 +31,40 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
+from typing import Union, List, Optional
 
 
-def update_detects_payload(current_payload: dict, passed_keywords: dict) -> dict:
-    """Update the provided payload with any viable parameters provided as keywords.
+def reports_payload(passed_keywords: dict, passed_arguments: Optional[tuple] = None) -> List[dict]:
+    """Create a properly formatted payload for report execution / scheduling.
 
-    {
-        "assigned_to_uuid": "string",
-        "comment": "string",
-        "ids": [
-            "string"
-        ],
-        "show_in_ui": true,
-        "status": "string"
-    }
+    [
+        {
+            "id": "string"
+        }
+    ]
     """
-    keys = ["assigned_to_uuid", "comment", "status"]
-    for key in keys:
-        if passed_keywords.get(key, None):
-            current_payload[key] = passed_keywords.get(key, None)
-
-    if passed_keywords.get("show_in_ui", None) is not None:
-        current_payload["show_in_ui"] = passed_keywords.get("show_in_ui", None)
-
-    passed_list = passed_keywords.get("ids", None)
-    if passed_list:
-        if isinstance(passed_list, str):
-            passed_list = passed_list.split(",")
-        current_payload["ids"] = passed_list
+    returned_payload = []
+    submitted: Union[str, list] = ""
+    if passed_keywords.get("ids", None):
+        key: Union[str, list] = passed_keywords.get("ids", None)
+        if isinstance(key, list):
+            submitted = key
+        else:
+            submitted = key.split(",")
+    elif passed_arguments:
+        key = passed_arguments[0]
+        if isinstance(key, list):
+            submitted = key
+        else:
+            submitted = key.split(",")
+
+    for submitted_id in submitted:
+        item = {}
+        item["id"] = submitted_id
+        returned_payload.append(item)
 
-    return current_payload
+    return returned_payload
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_device_control_policy.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_device_control_policy.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,44 +40,58 @@
 def device_policy_payload(passed_keywords: dict) -> dict:
     """Create a properly formatted device control policy payload.
 
     Supports create and update operations. Single policy only.
     {
         "resources": [
             {
-                "clone_id": "string",
                 "description": "string",
+                "id": "string",
+                "clone_id": "string",
                 "name": "string",
-                "platform_name": "Windows",
                 "settings": {
                     "classes": [
-                    {
-                        "action": "FULL_ACCESS",
-                        "exceptions": [
                         {
-                            "action": "string",
-                            "class": "string",
-                            "combined_id": "string",
-                            "id": "string",
-                            "match_method": "string",
-                            "product_id": "string",
-                            "product_id_decimal": "string",
-                            "product_name": "string",
-                            "serial_number": "string",
-                            "vendor_id": "string",
-                            "vendor_id_decimal": "string",
-                            "vendor_name": "string"
+                            "action": "FULL_ACCESS",
+                            "exceptions": [
+                            {
+                                "action": "string",
+                                "combined_id": "string",
+                                "description": "string",
+                                "expiration_time": "2023-06-08T06:10:39.965Z",
+                                "id": "string",
+                                "product_id": "string",
+                                "product_id_decimal": "string",
+                                "product_name": "string",
+                                "serial_number": "string",
+                                "use_wildcard": true,
+                                "vendor_id": "string",
+                                "vendor_id_decimal": "string",
+                                "vendor_name": "string"
+                            }
+                            ],
+                            "id": "string"
+                        }
+                    ],
+                    "custom_notifications": {
+                        "blocked_notification": {
+                            "custom_message": "string",
+                            "use_custom": true
+                        },
+                        "restricted_notification": {
+                            "custom_message": "string",
+                            "use_custom": true
                         }
-                        ],
-                        "id": "string"
-                    }
+                    },
+                    "delete_exceptions": [
+                        "string"
                     ],
-                    "end_user_notification": "TRUE",
-                    "enforcement_mode": "string",
-                    "id": "string"
+                    "end_user_notification": "SILENT",
+                    "enforcement_mode": "MONITOR_ONLY",
+                    "enhanced_file_metadata": true
                 }
             }
         ]
     }
     """
     returned_payload = {}
     resources = []
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_falconx.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_falconx.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_firewall.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_firewall.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     """Create a properly formatted firewall policy container payload.
 
     {
         "default_inbound": "string",
         "default_outbound": "string",
         "enforce": true,
         "is_default_policy": true,
+        "local_logging": true,
         "platform_id": "string",
         "policy_id": "string",
         "rule_group_ids": [
             "string"
         ],
         "test_mode": true,
         "tracking": "string"
@@ -88,14 +89,16 @@
     for key in keys:
         if passed_keywords.get(key, None):
             returned_payload[key] = passed_keywords.get(key, None)
     if passed_keywords.get("enforce", None) is not None:
         returned_payload["enforce"] = passed_keywords.get("enforce", None)
     if passed_keywords.get("is_default_policy", None) is not None:
         returned_payload["is_default_policy"] = passed_keywords.get("is_default_policy", None)
+    if passed_keywords.get("local_logging", None) is not None:
+        returned_payload["local_logging"] = passed_keywords.get("local_logging", None)
     if passed_keywords.get("test_mode", None) is not None:
         returned_payload["test_mode"] = passed_keywords.get("test_mode", None)
     rg_list = passed_keywords.get("rule_group_ids", None)
     if rg_list:
         if isinstance(rg_list, str):
             rg_list = rg_list.split(",")
         returned_payload["rule_group_ids"] = rg_list
@@ -146,14 +149,15 @@
 def firewall_rule_group_payload(passed_keywords: dict) -> dict:
     """Create a properly formatted firewall rule group payload.
 
     {
         "description": "string",
         "enabled": boolean,
         "name": "string",
+        "platform": "string",
         "rules": [
             {
                 "action": "string",
                 "address_family": "string",
                 "description": "string",
                 "direction": "string",
                 "enabled": boolean,
@@ -187,17 +191,14 @@
                 ],
                 "log": boolean,
                 "monitor": {
                     "count": "string",
                     "period_ms": "string"
                 },
                 "name": "string",
-                "platform_ids": [
-                    "string"
-                ],
                 "protocol": "string",
                 "remote_address": [
                     {
                         "address": "string",
                         "netmask": integer
                     }
                 ],
@@ -209,15 +210,15 @@
                 ],
                 "temp_id": "string"
             }
         ]
     }
     """
     returned_payload = {}
-    keys = ["description", "name"]
+    keys = ["description", "name", "platform"]
     for key in keys:
         if passed_keywords.get(key, None):
             returned_payload[key] = passed_keywords.get(key, None)
     if passed_keywords.get("enabled", None) is not None:
         returned_payload["enabled"] = passed_keywords.get("enabled", None)
 
     rules = passed_keywords.get("rules", None)
@@ -317,14 +318,16 @@
                 "type": "string",
                 "value": "string",
                 "values": [
                     "string"
                 ]
                 }
             ],
+            "fqdn": "string",
+            "fqdn_enabled": true,
             "icmp": {
                 "icmp_code": "string",
                 "icmp_type": "string"
             },
             "local_address": [
                 {
                 "address": "string",
@@ -422,14 +425,16 @@
             "enabled": true,
             "require_encryption": true,
             "ssids": [
                 "string"
                 ]
             }
         },
+        "created_by": "string",
+        "created_on": "string",
         "default_gateways": [
             "string"
         ],
         "description": "string",
         "dhcp_servers": [
             "string"
             ],
@@ -465,14 +470,15 @@
         "modified_by": "string",
         "modified_on": "string"
     }
     """
     returned_payload = {}
     keys = ["connection_types", "default_gateways", "description", "dhcp_servers", "id",
             "dns_resolution_targets", "dns_servers", "enabled", "host_addresses", "modified_on",
-            "https_reachable_hosts", "icmp_request_targets", "name", "modified_by"
+            "https_reachable_hosts", "icmp_request_targets", "name", "modified_by", "created_by",
+            "created_on"
             ]
     for key in keys:
         if passed_keywords.get(key, None):
             returned_payload[key] = passed_keywords.get(key)
 
     return returned_payload
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_generic.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_generic.py`

 * *Files 20% similar despite different names*

```diff
@@ -83,17 +83,21 @@
     {
         "date_ranges": [
             {
                 "from": "string",
                 "to": "string"
             }
         ],
+        "exclude": "string",
         "field": "string",
         "filter": "string",
+        "from": 0,
+        "include": "string",
         "interval": "string",
+        "max_doc_count": 0,
         "min_doc_count": 0,
         "missing": "string",
         "name": "string",
         "q": "string",
         "ranges": [
             {
                 "From": 0,
@@ -107,55 +111,27 @@
         ],
         "time_zone": "string",
         "type": "string"
     }
     """
     returned_payload = {}
 
-    if submitted_keywords.get("date_ranges", None):
-        returned_payload["date_ranges"] = submitted_keywords.get("date_ranges", None)
-
-    if submitted_keywords.get("field", None):
-        returned_payload["field"] = submitted_keywords.get("field", None)
-
-    if submitted_keywords.get("filter", None):
-        returned_payload["filter"] = submitted_keywords.get("filter", None)
-
-    if submitted_keywords.get("interval", None):
-        returned_payload["interval"] = submitted_keywords.get("interval", None)
-
-    if submitted_keywords.get("min_doc_count", -1) >= 0:
-        returned_payload["min_doc_count"] = submitted_keywords.get("min_doc_count", -1)
-
-    if submitted_keywords.get("missing", None):
-        returned_payload["missing"] = submitted_keywords.get("missing", None)
-
-    if submitted_keywords.get("name", None):
-        returned_payload["name"] = submitted_keywords.get("name", None)
-
-    if submitted_keywords.get("q", None):
-        returned_payload["q"] = submitted_keywords.get("q", None)
-
-    if submitted_keywords.get("ranges", None):
-        returned_payload["ranges"] = submitted_keywords.get("ranges", None)
-
-    if submitted_keywords.get("size", -1) >= 0:
-        returned_payload["size"] = submitted_keywords.get("size", 0)
-
-    if submitted_keywords.get("sort", None):
-        returned_payload["sort"] = submitted_keywords.get("sort", None)
-
-    if submitted_keywords.get("sub_aggregates", None):
-        returned_payload["sub_aggregates"] = submitted_keywords.get("sub_aggregates", None)
-
-    if submitted_keywords.get("time_zone", None):
-        returned_payload["time_zone"] = submitted_keywords.get("time_zone", None)
-
-    if submitted_keywords.get("type", None):
-        returned_payload["type"] = submitted_keywords.get("type", None)
+    keys = ["date_ranges", "exclude", "include", "field", "filter", "interval", "missing",
+            "name", "q", "ranges", "sort", "sub_aggregates", "time_zone", "type"
+            ]
+
+    int_keys = ["from", "max_doc_count", "min_doc_count", "size"]
+
+    for key in keys:
+        if submitted_keywords.get(key, None):
+            returned_payload[key] = submitted_keywords.get(key, None)
+
+    for key in int_keys:
+        if submitted_keywords.get(key, -1) >= 0:
+            returned_payload[key] = submitted_keywords.get(key, -1)
 
     return returned_payload
 
 
 def exclusion_payload(passed_keywords: dict) -> dict:
     """Create a properly formatted exclusion payload.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_host_group.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_incidents.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_ioa.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ioa.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,12 +143,20 @@
     if passed_keywords.get("enabled", None) is not None:
         returned_payload["enabled"] = passed_keywords.get("enabled", None)
     if passed_keywords.get("rulegroup_version", -1) >= 0:
         returned_payload["rulegroup_version"] = passed_keywords.get("rulegroup_version", None)
     if passed_keywords.get("disposition_id", -1) >= 0:
         returned_payload["disposition_id"] = passed_keywords.get("disposition_id", None)
     if passed_keywords.get("field_values", None):
-        returned_payload["field_values"] = [passed_keywords.get("field_values", None)]
+        field_values = passed_keywords.get("field_values")
+        if isinstance(field_values, dict):  # Issue 916
+            returned_payload["field_values"] = [field_values]
+        else:
+            returned_payload["field_values"] = field_values
     if passed_keywords.get("rule_updates", None):
-        returned_payload["rule_updates"] = [passed_keywords.get("rule_updates", None)]
+        rule_updates = passed_keywords.get("rule_updates")
+        if isinstance(rule_updates, dict):  # Issue 916
+            returned_payload["rule_updates"] = [rule_updates]
+        else:
+            returned_payload["rule_updates"] = rule_updates
 
     return returned_payload
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_ioc.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ioc.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     {
         "bulk_update": {
             "action": "string",
             "applied_globally": true,
             "description": "string",
             "expiration": "2021-10-22T11:03:16.123Z",
             "filter": "string",
+            "from_parent": true,
             "host_groups": [
                 "string"
             ],
             "mobile_action": "string",
             "platforms": [
                 "string"
             ],
@@ -198,14 +199,15 @@
     return returned_payload
 
 
 def indicator_report_payload(passed_keywords: dict) -> dict:
     """Create a properly formatted indicator report payload.
 
     {
+        "from_parent": true,
         "report_format": "string",
         "search": {
             "filter": "string",
             "query": "string",
             "sort": "string"
         }
     }
@@ -219,9 +221,11 @@
             search[key] = passed_keywords.get(key)
     if search:
         returned_payload["search"] = search
     # Passed search dictionary will override subkeys
     for key in keys:
         if passed_keywords.get(key, None):
             returned_payload[key] = passed_keywords.get(key)
+    if passed_keywords.get("from_parent", None) is not None:
+        returned_payload["from_parent"] = passed_keywords.get("from_parent", None)
 
     return returned_payload
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_malquery.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_message_center.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_message_center.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     """Create a properly formatted case payload.
 
     {
         "body": "string",
         "detections": [
             {
                 "id": "string",
+                "product": "string",
                 "url": "string"
             }
         ],
         "id": "string",
         "incidents": [
             {
                 "id": "string",
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_mssp.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_prevention_policy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Internal payload handling library - Falcon Flight Control (MSSP).
+"""Internal payload handling library - Prevention Policy Payloads.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -33,46 +33,47 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
 
-def mssp_payload(passed_keywords: dict) -> dict:
-    """Create a properly formatted Flight Control payload.
+def prevention_policy_payload(passed_keywords: dict) -> dict:
+    """Create a properly formatted prevention policy payload.
 
+    Supports create and update operations.
     {
         "resources": [
             {
-                "cid": "string",
-                "cid_group_id": "string",
+                "clone_id": "string",
                 "description": "string",
-                "name": "string"
-                "id": "string",
-                "role_ids": [
-                    "string"
-                ],
-                "user_group_id": "string"
+                "name": "string",
+                "platform_name": "Windows",
+                "settings": [
+                    {
+                        "id": "string",
+                        "value": {}
+                    }
+                ]
             }
         ]
     }
     """
     returned_payload = {}
-    resources_item = {}
-    keys = [
-        "cid", "cid_group_id", "description", "name", "id",
-        "user_group_id", "user_uuids"
-        ]
-    for key in keys:
-        if passed_keywords.get(key, None):
-            resources_item[key] = passed_keywords.get(key, None)
-
-    passed_role_ids = passed_keywords.get("role_ids", None)
-    if passed_role_ids:
-        if isinstance(passed_role_ids, str):
-            passed_role_ids = passed_role_ids.split(",")
-        resources_item["role_ids"] = passed_role_ids
-
-    if resources_item:
-        returned_payload["resources"] = [resources_item]
+    resources = []
+    item = {}
+    if passed_keywords.get("clone_id", None):
+        item["clone_id"] = passed_keywords.get("clone_id", None)
+    if passed_keywords.get("id", None):
+        item["id"] = passed_keywords.get("id", None)
+    if passed_keywords.get("description", None):
+        item["description"] = passed_keywords.get("description", None)
+    if passed_keywords.get("name", None):
+        item["name"] = passed_keywords.get("name", None)
+    if passed_keywords.get("platform_name", None):
+        item["platform_name"] = passed_keywords.get("platform_name", None)
+    if passed_keywords.get("settings", None):
+        item["settings"] = passed_keywords.get("settings", None)
+    resources.append(item)
+    returned_payload["resources"] = resources
 
     return returned_payload
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_ods.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ods.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,28 +59,31 @@
         "max_duration": 0,
         "max_file_size": 0,
         "pause_duration": 0,
         "quarantine": true,
         "scan_exclusions": [
             "string"
         ],
+        "scan_inclusions": [
+            "string"
+        ],
         "schedule": {
             "ignored_by_channelfile": true,
             "interval": 0,
             "start_timestamp": "string"
         },
         "sensor_ml_level_detection": 0,
         "sensor_ml_level_prevention": 0
     }
     """
     returned_payload = {}
     keys = ["cloud_ml_level_detection", "cloud_ml_level_prevention", "cpu_priority", "description",
             "endpoint_notification", "file_paths", "host_groups", "initiated_from", "max_duration",
             "max_file_size", "pause_duration", "quarantine", "scan_exclusions", "schedule",
-            "sensor_ml_level_detection", "sensor_ml_level_prevention", "hosts"
+            "sensor_ml_level_detection", "sensor_ml_level_prevention", "hosts", "scan_inclusions"
             ]
     for key in keys:
         if passed_keywords.get(key, None) is not None:
             returned_payload[key] = passed_keywords.get(key)
 
     schedule_keys = ["ignored_by_channelfile", "interval", "start_timestamp"]
     if "schedule" not in returned_payload:
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_prevention_policy.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_response_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Internal payload handling library - Prevention Policy Payloads.
+"""Internal payload handling library - Response Policy Payloads.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -33,16 +33,16 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
 
-def prevention_policy_payload(passed_keywords: dict) -> dict:
-    """Create a properly formatted prevention policy payload.
+def response_policy_payload(passed_keywords: dict) -> dict:
+    """Create a properly formatted response policy payload.
 
     Supports create and update operations.
     {
         "resources": [
             {
                 "clone_id": "string",
                 "description": "string",
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_real_time_response.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_sensor_update_policy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Internal payload handling library - Real Time Response.
+"""Internal payload handling library - Sensor Update Policy Payloads.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -33,88 +33,77 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 
 
-def command_payload(passed_keywords: dict) -> dict:  # pylint: disable=R0912  # noqa: C901
-    """Create a properly formatted payload for RTR command.
+def sensor_policy_payload(passed_keywords: dict) -> dict:
+    """Create a properly formatted prevention policy payload.
 
+    Supports create and update operations. Single policy only.
     {
-        "base_command": "string",
-        "batch_id": "string",
-        "command_string": "string",
-        "optional_hosts": [
-            "string"
-        ],
-        "file_path": "string",
-        "persist_all": true,
-        "existing_batch_id": "string",
-        "host_ids": [
-            "string"
-        ],
-        "queue_offline": true,
-        "hosts_to_remove": [
-            "string"
+        "resources": [
+            {
+                "description": "string",
+                "name": "string",
+                "platform_name": "Windows",
+                "settings": {
+                    "build": "string",
+                    "scheduler": {
+                        "enabled": true,
+                        "schedules": [
+                            {
+                                "days": [
+                                    0
+                                ],
+                                "end": "string",
+                                "start": "string"
+                            }
+                        ],
+                        "timezone": "string"
+                    },
+                    "show_early_adopter_builds": true,
+                    "uninstall_protection": "ENABLED",
+                    "variants": [
+                        {
+                            "build": "string",
+                            "platform": "string"
+                        }
+                    ]
+                }
+            }
         ]
-        "device_id": "string",
-        "id": integer,
-        "persist": boolean,
-        "session_id": "string",
-        "origin": "string"
     }
     """
-    # flake8 / pylint both complain about complexity due to the number of if statements.
-    # Ignoring the complaint as this is just running through the potential passed keywords.
     returned_payload = {}
+    resources = []
+    item = {}
+    if passed_keywords.get("id", None):
+        item["id"] = passed_keywords.get("id", None)
+    if passed_keywords.get("description", None):
+        item["description"] = passed_keywords.get("description", None)
+    if passed_keywords.get("name", None):
+        item["name"] = passed_keywords.get("name", None)
+    if passed_keywords.get("platform_name", None):
+        item["platform_name"] = passed_keywords.get("platform_name", None)
+    settings = {}
+    if passed_keywords.get("build", None):
+        settings["build"] = passed_keywords.get("build", None)
+    if passed_keywords.get("scheduler", None):
+        settings["scheduler"] = passed_keywords.get("scheduler", None)
+    if passed_keywords.get("show_early_adopter_builds", None):
+        settings["show_early_adopter_builds"] = passed_keywords.get("show_early_adopter_builds", None)
+    if passed_keywords.get("uninstall_protection", None):
+        settings["uninstall_protection"] = passed_keywords.get("uninstall_protection", "DISABLED")
+    if passed_keywords.get("variants", None):
+        settings["variants"] = passed_keywords.get("variants", None)
+    if settings:
+        item["settings"] = settings
+    # Passing settings overrides the passed build / uninstall_protection values
+    if passed_keywords.get("settings", None):
+        item["settings"] = passed_keywords.get("settings", None)
 
-    keys = [
-        "base_command", "batch_id", "command_string", "file_path",
-        "existing_batch_id", "device_id", "session_id", "origin"
-        ]
-    for key in keys:
-        if passed_keywords.get(key, None):
-            returned_payload[key] = passed_keywords.get(key, None)
-
-    bool_keys = ["persist_all", "queue_offline", "persist"]
-    for boolean in bool_keys:
-        if passed_keywords.get(boolean, None) is not None:
-            returned_payload[boolean] = passed_keywords.get(boolean, None)
-
-    if passed_keywords.get("id", -1) > -1:
-        returned_payload["id"] = passed_keywords.get("id", None)
-
-    list_keys = ["optional_hosts", "host_ids", "hosts_to_remove"]
-    for list_key in list_keys:
-        passed_list = passed_keywords.get(list_key, None)
-        if passed_list:
-            if isinstance(passed_list, str):
-                passed_list = passed_list.split(",")
-            returned_payload[list_key] = passed_list
-
-    return returned_payload
-
-
-def data_payload(passed_keywords: dict) -> dict:
-    """Create a properly formatted formData payload for RTR file uploads.
-
-    {
-        "id": "string",
-        "description": "string",
-        "name": "string",
-        "comments_for_audit_log": "string",
-        "content": "string",
-        "platform": "string",
-        "permission_type": "string"
-    }
-    """
-    returned_payload = {}
-    keys = [
-        "id", "description", "name", "comments_for_audit_log",
-        "content", "platform", "permission_type"
-        ]
-    for key in keys:
-        if passed_keywords.get(key, None):
-            returned_payload[key] = passed_keywords.get(key, None)
+    resources.append(item)
+    returned_payload["resources"] = resources
 
     return returned_payload
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_recon.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_recon.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,41 +37,39 @@
 """
 from typing import List, Dict
 
 
 def handle_recon_rule_params(inbound: dict) -> dict:
     """Handle the payload formatting for a single rule object."""
     returned_dict = {}
-    if inbound.get("filter", None):
-        returned_dict["filter"] = inbound.get("filter", None)
-    if inbound.get("id", None):
-        returned_dict["id"] = inbound.get("id", None)
-    if inbound.get("name", None):
-        returned_dict["name"] = inbound.get("name", None)
-    if inbound.get("permissions", None):
-        returned_dict["permissions"] = inbound.get("permissions", None)
-    if inbound.get("priority", None):
-        returned_dict["priority"] = inbound.get("priority", None)
-    if inbound.get("topic", None):
-        returned_dict["topic"] = inbound.get("topic", None)
+    keys = ["filter", "id", "name", "permissions", "priority", "topic"]
+    bool_keys = ["breach_monitoring_enabled", "substring_matching_enabled"]
+    for key in keys:
+        if inbound.get(key, None):
+            returned_dict[key] = inbound.get(key, None)
+    for key in bool_keys:
+        if inbound.get(key, None) is not None:
+            returned_dict[key] = inbound.get(key, None)
 
     return returned_dict
 
 
 def recon_rules_payload(passed_keywords: dict) -> List[Dict[str, str]]:
     """Create a properly formatted payload for recon rule handling.
 
     Creates a list of dictionaries.
     [
         {
+            "breach_monitoring_enabled": true,
             "filter": "string",
             "id": "string",
             "name": "string",
             "permissions": "string",
             "priority": "string",
+            "substring_matching_enabled": true,
             "topic": "string"
         }
     ]
     """
     returned_rules = []
     provided_rules = passed_keywords.get("rules", None)
     if provided_rules:
@@ -118,66 +116,78 @@
     return returned_payload
 
 
 def recon_action_update_payload(passed_keywords: dict) -> dict:
     """Create a properly formatted payload for handling recon actions.
 
     {
+        "content_format": "string",
         "frequency": "string",
         "id": "string",
         "recipients": [
             "string"
         ],
+        "trigger_matchless": true,
         "status": "string"
     }
     """
     returned_payload = {}
-    if passed_keywords.get("frequency", None):
-        returned_payload["frequency"] = passed_keywords.get("frequency", None)
-    if passed_keywords.get("id", None):
-        returned_payload["id"] = passed_keywords.get("id", None)
+    keys = ["content_format", "frequency", "id", "status"]
+    for key in keys:
+        if passed_keywords.get(key, None):
+            returned_payload[key] = passed_keywords.get(key, None)
+
     recip_list = passed_keywords.get("recipients", None)
     if recip_list:
         if isinstance(recip_list, str):
             recip_list = recip_list.split(",")
         returned_payload["recipients"] = recip_list
-    if passed_keywords.get("status", None):
-        returned_payload["status"] = passed_keywords.get("status", None)
+
+    if passed_keywords.get("trigger_matchless", None) is not None:
+        returned_payload["trigger_matchless"] = passed_keywords.get("trigger_matchless", None)
 
     return returned_payload
 
 
 def recon_action_payload(passed_keywords: dict) -> dict:
     """Create a properly formatted payload for attaching recon actions to a monitoring rule.
 
     {
         "actions": [
             {
+                "content_format": "string",
                 "frequency": "string",
                 "recipients": [
                     "string"
                 ],
+                "trigger_matchless": true,
                 "type": "string"
             }
         ],
         "rule_id": "string"
     }
     """
     returned_payload = {}
     returned_payload["rule_id"] = passed_keywords.get("rule_id", None)
     if passed_keywords.get("actions", None):
         returned_payload["actions"] = passed_keywords.get("actions", None)
     else:
+        keys = ["content_format", "frequency", "type"]
         action = {}
-        if passed_keywords.get("frequency", None):
-            action["frequency"] = passed_keywords.get("frequency", None)
-        if passed_keywords.get("recipients", None):
-            action["recipients"] = passed_keywords.get("recipients", None)
-        if passed_keywords.get("type", None):
-            action["type"] = passed_keywords.get("type", None)
+        for key in keys:
+            if passed_keywords.get(key, None):
+                action[key] = passed_keywords.get(key, None)
+        recip_list = passed_keywords.get("recipients", None)
+        if recip_list:
+            if isinstance(recip_list, str):
+                recip_list = recip_list.split(",")
+            action["recipients"] = recip_list
+
+        if passed_keywords.get("trigger_matchless", None) is not None:
+            action["trigger_matchless"] = passed_keywords.get("trigger_matchless", None)
         returned_payload["actions"] = []
         returned_payload["actions"].append(action)
 
     return returned_payload
 
 
 def recon_rule_preview_payload(passed_keywords: dict) -> dict:
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_reports.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_sample_uploads.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Internal payload handling library - Reports Payloads.
+"""Internal payload handling library - Sample Uploads Payloads.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -31,40 +31,33 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-from typing import Union, List, Optional
 
 
-def reports_payload(passed_keywords: dict, passed_arguments: Optional[tuple] = None) -> List[dict]:
-    """Create a properly formatted payload for report execution / scheduling.
+def extraction_payload(passed_keywords: dict) -> dict:
+    """Create a properly formatted archive extraction payload.
 
-    [
-        {
-            "id": "string"
-        }
-    ]
+    {
+        "extract_all": true,
+        "files": [
+            {
+                "comment": "string",
+                "is_confidential": true,
+                "name": "string"
+            }
+        ],
+        "sha256": "string"
+    }
     """
-    returned_payload = []
-    submitted: Union[str, list] = ""
-    if passed_keywords.get("ids", None):
-        key: Union[str, list] = passed_keywords.get("ids", None)
-        if isinstance(key, list):
-            submitted = key
-        else:
-            submitted = key.split(",")
-    elif passed_arguments:
-        key = passed_arguments[0]
-        if isinstance(key, list):
-            submitted = key
-        else:
-            submitted = key.split(",")
-
-    for submitted_id in submitted:
-        item = {}
-        item["id"] = submitted_id
-        returned_payload.append(item)
+    returned_payload = {}
+    keys = ["sha256", "files"]
+    for key in keys:
+        if passed_keywords.get(key, None):
+            returned_payload[key] = passed_keywords.get(key)
+    if passed_keywords.get("extract_all", None) is not None:
+        returned_payload["extract_all"] = passed_keywords.get("extract_all")
 
     return returned_payload
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_payload/_sample_uploads.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_expanded_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Internal payload handling library - Sample Uploads Payloads.
+"""API Response formatting class.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -31,33 +31,35 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
+# pylint: disable=R0903
+from typing import Tuple, Dict, Union
 
 
-def extraction_payload(passed_keywords: dict) -> dict:
-    """Create a properly formatted archive extraction payload.
+class ExpandedResult:
+    """Callable subsclass to handle parsing of expanded result client output.
 
-    {
-        "extract_all": true,
-        "files": [
-            {
-                "comment": "string",
-                "is_confidential": true,
-                "name": "string"
-            }
-        ],
-        "sha256": "string"
-    }
+    DEPRECATED
+    ---
+    This class is deprecated and maintained for backwards compatibility purposes only.
+
+    Please move all code over to use Result.tupled.
+
+    Examples: tupled_response: Result = falcon.query_detects(pythonic=True).tupled
+              tupled_response: Result = Result(full=falcon.query_detects()).tupled
     """
-    returned_payload = {}
-    keys = ["sha256", "files"]
-    for key in keys:
-        if passed_keywords.get(key, None):
-            returned_payload[key] = passed_keywords.get(key)
-    if passed_keywords.get("extract_all", None) is not None:
-        returned_payload["extract_all"] = passed_keywords.get("extract_all")
 
-    return returned_payload
+    def __call__(self,
+                 status_code: int,
+                 headers: Dict[str, str],
+                 content: Union[str, bytes, Dict[str, Dict]]
+                 ) -> Tuple[str, Dict[str, str], Dict[str, Dict]]:
+        """Format ingested values into a properly formatted expanded result object."""
+        content_result = content
+        if isinstance(content, dict):
+            content_result = content["body"]
+
+        return (status_code, dict(headers), content_result)
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/__base_resource.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/__base_resource.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_base_dictionary.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_base_dictionary.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_errors.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_errors.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_expanded_result.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_resources.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""API Response formatting class.
+"""FalconPy Resource object.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -31,35 +31,36 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-# pylint: disable=R0903
-from typing import Tuple, Dict, Union
+from ._response_component import ResponseComponent
+from .__base_resource import BaseResource
+from ._base_dictionary import BaseDictionary
 
 
-class ExpandedResult:
-    """Callable subsclass to handle parsing of expanded result client output.
+class Resources(BaseResource):
+    """This class represents the resources branch of an API response."""
 
-    DEPRECATED
-    ---
-    This class is deprecated and maintained for backwards compatibility purposes only.
-
-    Please move all code over to use Result.tupled.
-
-    Examples: tupled_response: Result = falcon.query_detects(pythonic=True).tupled
-              tupled_response: Result = Result(full=falcon.query_detects()).tupled
-    """
-
-    def __call__(self,
-                 status_code: int,
-                 headers: Dict[str, str],
-                 content: Union[str, bytes, Dict[str, Dict]]
-                 ) -> Tuple[str, Dict[str, str], Dict[str, Dict]]:
-        """Format ingested values into a properly formatted expanded result object."""
-        content_result = content
-        if isinstance(content, dict):
-            content_result = content["body"]
+    def contains(self, substr) -> list:
+        """Search filter."""
+        # May move this to __contains__
+        _returned = []
+        if self._data:
+            _data = self._data
+            _returned = [x for x in _data if substr in x]
 
-        return (status_code, dict(headers), content_result)
+        return _returned
+
+
+class BinaryFile(ResponseComponent):
+    """A binary file resource."""
+
+    def __bytes__(self):
+        """Return the object in bytes."""
+        return bytes(self._data)
+
+
+class RawBody(BaseDictionary):
+    """Class to represent a raw payload that does not match standard formatting."""
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_headers.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_headers.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_meta.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_meta.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_resources.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""FalconPy Resource object.
+"""Internal authentication utilities library.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -31,36 +31,44 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-from ._response_component import ResponseComponent
-from .__base_resource import BaseResource
-from ._base_dictionary import BaseDictionary
+from ._functions import generate_b64cred
+from .._endpoint._oauth2 import _oauth2_endpoints as AuthEndpoints
 
 
-class Resources(BaseResource):
-    """This class represents the resources branch of an API response."""
+def login_payloads(creds: dict, base: str):
+    """Craft the necessary payloads to generate a token.
 
-    def contains(self, substr) -> list:
-        """Search filter."""
-        # May move this to __contains__
-        _returned = []
-        if self._data:
-            _data = self._data
-            _returned = [x for x in _data if substr in x]
+    This method is intentionally generic and does not necessarily need to
+    be used to generate the token currently being used for other API operations.
+    """
+    op_id = "oauth2AccessToken"
+    target = f"{base}{[ep[2] for ep in AuthEndpoints if op_id in ep[0]][0]}"
+    data = {
+        'client_id': creds['client_id'],
+        'client_secret': creds['client_secret']
+    }
+    if "member_cid" in creds:
+        data["member_cid"] = creds["member_cid"]
+
+    return op_id, target, data
+
+
+def logout_payloads(creds: dict, base: str, token_val: str, client_id: str = None):
+    """Craft the necessary payloads to revoke a token.
+
+    This method is intentionally generic and does not necessarily need to
+    be used to revoke the token currently being used for other API operations.
+    """
+    op_id = "oauth2RevokeToken"
+    target = f"{base}{[ep[2] for ep in AuthEndpoints if op_id in ep[0]][0]}"
+    b64cred = generate_b64cred(creds["client_id"], creds["client_secret"])
+    headers = {"Authorization": f"basic {b64cred}"}
+    data = {"token": f"{token_val}"}
+    if client_id:
+        data["client_id"] = client_id
 
-        return _returned
-
-
-class BinaryFile(ResponseComponent):
-    """A binary file resource."""
-
-    def __bytes__(self):
-        """Return the object in bytes."""
-        return bytes(self._data)
-
-
-class RawBody(BaseDictionary):
-    """Class to represent a raw payload that does not match standard formatting."""
+    return op_id, target, data, headers
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_response_component.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_response_component.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,15 +70,20 @@
 
     def get_property(self, item, default_return: Union[str, int, dict, float, list] = None):
         """Property lookup helper. Returns None if the underlying data is binary."""
         _returned = None
         if isinstance(self._data, dict):
             _returned = self._data.get(item, default_return)
         elif isinstance(self._data, (list, str)):
-            _returned = self._data[item]
+            try:
+                _returned = self._data[item]
+            except IndexError as bad_pos:
+                raise IndexError(
+                    "Invalid position specified. Please check your index and try again."
+                    ) from bad_pos
 
         return _returned
 
     #   _____   ______  _____   _____  _______  ______ _______ _____ _______ _______
     #  |_____] |_____/ |     | |_____] |______ |_____/    |      |   |______ |______
     #  |       |    \_ |_____| |       |______ |    \_    |    __|__ |______ ______|
     #
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_result/_result.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -93,18 +93,34 @@
             elif body.get("access_token", None):
                 # Authentication response
                 self.raw = RawBody(body)
                 self.meta = Meta()
                 self.resources = Resources()
                 self.errors = Errors()
             else:
-                # Standard response
+                # Standard responses, GraphQL and RTR
                 self.meta = Meta(body.get("meta", {}))
-                self.resources = Resources(body.get("resources", []))
                 self.errors = Errors(body.get("errors", []))
+                # RTR Batch responses
+                if body.get("batch_id", {}):
+                    # Batch session init
+                    self.raw = RawBody(body)
+                    self.resources = Resources(body.get("resources", []))
+                elif body.get("combined", {}):
+                    # Batch session results have to be handled as RawBody
+                    # due to the combined response format.
+                    self.raw = RawBody(body)
+                elif body.get("data", {}):  # pragma: no cover
+                    # GraphQL uses a custom response payload, we will
+                    # use RawBody for this return for now. Due to
+                    # environment constraints, this is manually tested.
+                    self.raw = RawBody(body)
+                else:
+                    # Standard API responses
+                    self.resources = Resources(body.get("resources", []))
 
     # Iteration handlers
     def __iter__(self):
         """Return this object for iteration handling."""
         _returned = self
         if self.data:
             _returned = self.resources.data.__iter__()
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_service_class/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_service_class/_base_service_class.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/_base_service_class.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_service_class/_service_class.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/_service_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,14 +161,19 @@
         self.validate_payloads: bool = kwargs.get("validate_payloads", True)
 
         # The following properties can be overridden per Service Class.
         for item in ["proxy", "timeout", "user_agent"]:
             if kwargs.get(item, None) is not None:
                 setattr(self, f"_override_{item}", kwargs.get(item))
 
+        # Service Classes automatically log themselves in upon instantiation
+        # if no authentication status is present.
+        if not self.token_status:
+            self.login()
+
         # Log the creation of this Service Class if debugging is enabled.
         if self.log:
             log_class_startup(self, self.log)
 
     # _  _ ____ ___ _  _ ____ ___  ____
     # |\/| |___  |  |__| |  | |  \ [__
     # |  | |___  |  |  | |__| |__/ ___]
@@ -260,7 +265,15 @@
     @property
     def headers(self) -> Dict[str, str]:
         """Provide a complete set of request headers."""
         return {
             ** self.auth_object.auth_headers,
             ** self.ext_headers
         }
+
+    @property
+    def token(self) -> str:
+        """Return the underlying token value from the auth_object.
+
+        This recreates pre-1.3.0 functionality.
+        """
+        return self.auth_object.token_value
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_util/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_util/_functions.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,18 @@
 
 For more information, please refer to <https://unlicense.org>
 """
 import base64
 import functools
 from warnings import warn
 from json import loads
-from json.decoder import JSONDecodeError
+try:
+    from simplejson import JSONDecodeError
+except ImportError:
+    from json.decoder import JSONDecodeError
 from typing import Dict, Any, Union, Optional, List, Type
 from copy import deepcopy
 from logging import Logger
 import requests
 import urllib3
 from urllib3.exceptions import InsecureRequestWarning
 from .._api_request import APIRequest
@@ -587,14 +590,22 @@
     body_required -- List of required body payload parameters
     expand_result -- Request expanded results output
     pythonic -- Pythonic responses
     """
     # Log the operation ID if we have logging enabled.
     if calling_object.log:
         calling_object.log.debug("OPERATION: %s", operation_id)
+    # We have to create our headers dictionary first, as authentication happens here.
+    # For scenarios where cloud region autodiscovery is leveraged, we cannot create
+    # the target URL for our call to requests until we know our correct base_url.
+    passed_headers = kwargs.get("headers", None) if kwargs.get("headers", None) else {}
+    joined_headers = {
+        ** calling_object.headers,
+        ** passed_headers
+    }
     target_endpoint = [ep for ep in endpoints if operation_id == ep[0]][0]
     base_url = calling_object.base_url
     container = False
     if operation_id in MOCK_OPERATIONS:
         for base in [burl for burl in dir(BaseURL) if "__" not in burl]:
             if BaseURL[base].value == calling_object.base_url.replace("https://", ""):
                 base_url = f"https://{ContainerBaseURL[base].value}"
@@ -612,19 +623,14 @@
         target_url = target_url.format(str(passed_image_id))
     # Retrieve our keyword arguments
     passed_keywords = kwargs.get("keywords", None)
     passed_params = kwargs.get("params", None)
     parameter_payload = None
     if passed_keywords or passed_params:
         parameter_payload = args_to_params(passed_params, passed_keywords, endpoints, operation_id)
-    passed_headers = kwargs.get("headers", None) if kwargs.get("headers", None) else {}
-    joined_headers = {
-        ** calling_object.headers,
-        ** passed_headers
-    }
     expand_result = passed_keywords.get("expand_result", False) if passed_keywords else kwargs.get("expand_result", False)
     new_keywords = {
         "caller": calling_object,
         "method": target_method,
         "endpoint": target_url,
         "verify": calling_object.ssl_verify,
         "headers": joined_headers,
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/_util/_uber.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_uber.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/alerts.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/alerts.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,17 +67,21 @@
                     {
                         "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
                         ],
+                        "exclude": "string",
                         "field": "string",
                         "filter": "string",
+                        "from": 0,
+                        "include": "string",
                         "interval": "string",
+                        "max_doc_count": 0,
                         "min_doc_count": 0,
                         "missing": "string",
                         "name": "string",
                         "q": "string",
                         "ranges": [
                         {
                             "From": 0,
@@ -89,19 +93,28 @@
                         "sub_aggregates": [
                             null
                         ],
                         "time_zone": "string",
                         "type": "string"
                     }
                 ]
-        date_ranges -- List of dictionaries.
-        field -- String.
-        filter -- FQL syntax. String.
+        date_ranges -- If peforming a date range query specify the from and to date ranges.
+                       These can be in common date formats like 2019-07-18 or now.
+                       List of dictionaries.
+        exclude -- Fields to exclude. String.
+        field -- Term you want to aggregate on. If doing a date_range query,
+                 this is the date field you want to apply the date ranges to. String.
+        filter -- Optional filter criteria in the form of an FQL query.
+                  For more information about FQL queries, see our FQL documentation in Falcon.
+                  String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
         name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
         size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/api_complete.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/api_complete.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/cloud_connect_aws.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/cspm_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/cspm_registration.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-# pylint: disable=R0904  # Matching API operation counts
+# pylint: disable=R0904, C0302  # Matching API operation counts and allowing the long file for now
 from typing import Dict, Union
 from ._util import force_default, process_service_request, handle_single_argument
 from ._payload import cspm_registration_payload, cspm_policy_payload, cspm_scan_payload
 from ._service_class import ServiceClass
 from ._endpoint._cspm_registration import _cspm_registration_endpoints as Endpoints
 
 
@@ -59,17 +59,19 @@
     @force_default(defaults=["parameters"], default_types=["dict"])
     def get_aws_account(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Return information about the current status of an AWS account.
 
         Keyword arguments:
         scan_type -- Type of scan, `dry` or `full`, to perform on selected accounts
         ids -- AWS account IDs. String or list of strings.
+        iam_role_arns -- AWS IAM role ARNs. String or list of strings.
         organization_ids -- AWS organization IDs. String or list of strings.
         limit -- The maximum number of records to return in this response. [Integer, 1-1000]
                  Use with the offset parameter to manage pagination of results. Defaults to 100.
+        migrated -- Only return migrated d4c accounts. (true / false) String.
         offset -- The offset to start retrieving records from. Integer.
                   Use with the limit parameter to manage pagination of results.
         parameters - full parameters payload, not required if using other keywords.
         status -- Account status to filter results by. String.
         group_by -- Field to group by. String. (Only acceptable value: `organization`)
 
         This method only supports keywords for providing arguments.
@@ -104,22 +106,34 @@
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 {
                     "resources": [
                         {
                             "account_id": "string",
+                            "account_type": "string",
+                            "behavior_assessment_enabled": true,
                             "cloudtrail_region": "string",
-                            "organization_id": "string"
+                            "iam_role_arn": "string",
+                            "is_master": true,
+                            "organization_id": "string",
+                            "sensor_management_enabled": true,
+                            "use_existing_cloudtrail": true
                         }
                     ]
                 }
         account_id -- AWS Account ID. String.
+        account_type -- AWS account type. String.
+        behavior_assessment_enabled -- Indicate if behavior assessment should be enabled. Boolean.
         cloudtrail_region -- AWS Cloudtrail Region. String.
+        iam_role_arn -- IAM role ARN to use. String.
+        is_master -- Indicate if this is the primary account. Boolean.
         organization_id -- AWS Organization ID. String.
+        sensor_management_enabled -- Indicate if sensor management should be enabled. Boolean.
+        use_existing_cloudtrail -- Indicate if the existing CloudTrail should be used. Boolean.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: POST
 
@@ -171,19 +185,29 @@
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 {
                     "resources": [
                         {
                             "account_id": "string",
-                            "cloudtrail_region": "string"
+                            "behavior_assessment_enabled": true,
+                            "cloudtrail_region": "string",
+                            "iam_role_arn": "string",
+                            "remediation_region": "string",
+                            "remediation_tou_accepted": "2023-06-07T18:28:36.303Z",
+                            "sensor_management_enabled": true
                         }
                     ]
                 }
         account_id -- AWS Account ID. String.
+        behavior_assessment_enabled -- Indicate if behavior assessment should be enabled. Boolean.
+        cloudtrail_region -- AWS Cloudtrail Region. String.
+        iam_role_arn -- IAM role ARN to use. String.
+        remediation_region -- AWS region to remediation. String.
+        remediation_tou_accepted -- Timestamp formatted string.
         cloudtrail_region -- AWS Cloudtrail Region. String.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: PATCH
@@ -197,54 +221,68 @@
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
             operation_id="PatchCSPMAwsAccount",
             body=body
             )
 
-    def get_aws_console_setup_urls(self: object) -> Dict[str, Union[int, dict]]:
+    def get_aws_console_setup_urls(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve setup URLs for the AWS console.
 
         Returns a URL for customers to visit in their cloud environment
         to grant access to CrowdStrike.
 
-        This method does not accept arguments or keywords.
+        Keyword arguments:
+        ids -- AWS Account IDs to retrieve setup URLs for. String or list of strings.
+        use_existing_cloudtrail -- Use the existing AWS cloudtrail. (true / false) String.
+        parameters -- full parameters payload, not required if using other keywords.
+        region -- AWS Region. String.
+
+        This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/cspm-registration/GetCSPMAwsConsoleSetupURLs
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="GetCSPMAwsConsoleSetupURLs"
+            operation_id="GetCSPMAwsConsoleSetupURLs",
+            keywords=kwargs,
+            params=parameters
             )
 
-    def get_aws_account_scripts_attachment(self: object) -> Dict[str, Union[int, dict]]:
+    def get_aws_account_scripts_attachment(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve AWS account scripts.
 
         Return a script for customers to run in their cloud environment
         to grant access to CrowdStrike for their AWS environment.
 
-        This method does not accept arguments or keywords.
+        Keyword arguments:
+        ids -- AWS Account IDs to retrieve script attachments for. String or list of strings.
+        parameters -- full parameters payload, not required if using other keywords.
+
+        This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/cspm-registration/GetCSPMAwsAccountScriptsAttachment
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="GetCSPMAwsAccountScriptsAttachment"
+            operation_id="GetCSPMAwsAccountScriptsAttachment",
+            keywords=kwargs,
+            params=parameters
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def get_azure_account(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Return information about Azure account registration.
 
         Keyword arguments:
@@ -252,14 +290,15 @@
         ids -- Azure account IDs. String or list of strings.
         limit -- The maximum number of records to return in this response. [Integer, 1-1000]
                  Use with the offset parameter to manage pagination of results. Defaults to 100.
         offset -- The offset to start retrieving records from. Integer.
                   Use with the limit parameter to manage pagination of results.
         parameters - full parameters payload, not required if using other keywords.
         status -- Account status to filter results by. String.
+        tenant_ids -- Azure tenant IDs to filter results. String or list of strings.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
@@ -285,21 +324,29 @@
         to run in their cloud environment to grant CrowdStrike Horizon access.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 {
                     "resources": [
                         {
-                            "tenant_id": "string",
+                            "account_type": "string",
+                            "client_id": "string",
+                            "default_subscription": true,
                             "subscription_id": "string"
+                            "tenant_id": "string",
+                            "years_valid": integer
                         }
                     ]
                 }
-        tenant_id -- Azure Tenant ID. String.
+        account_type -- Azure account type. String.
+        client_id -- Azure Client ID. String.
+        default_subscription -- Indicate if this is the default subscription. Boolean.
         subscription_id -- Azure Subscription ID. String.
+        tenant_id -- Azure Tenant ID. String.
+        years_valid -- Number of years this account is valid. Integer.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: POST
 
@@ -319,14 +366,16 @@
     @force_default(defaults=["parameters"], default_types=["dict"])
     def delete_azure_account(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Delete an existing Azure Subscription by specifying their IDs.
 
         Keyword arguments:
         ids -- List of Azure Subscription IDs to delete. String or list of strings.
         parameters -- full parameters payload, not required if ids is provided as a keyword.
+        retain_tenant -- Should the tenant be retainined. (true / false) String.
+        tenant_ids -- Azure tenant IDs to remove. String or list of strings.
 
         Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
                    All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: DELETE
@@ -433,14 +482,15 @@
         Returns JSON object(s) that contain the base64 encoded certificate for a service principal.
 
         Keyword arguments:
         tenant_id -- Azure Tenant ID to generate script for.
                      Defaults to the most recently registered tenant.
         parameters -- full parameters payload, not required if tenant-id keyword is used.
         refresh -- Force a refresh of the certificate. Boolean. Defaults to False.
+        years_valid -- Years the certificate should be valid (only used when refresh=true).
 
         Arguments: When not specified, the first argument to this method is assumed to be
                    'tenant_id'. All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
@@ -465,17 +515,20 @@
         """
         Retrieve Azure user script.
 
         Return a script for customers to run in their cloud environment
         to grant access to CrowdStrike for their Azure environment.
 
         Keyword arguments:
+        account_type -- Account type. ('commercial' or 'gov') String.
         tenant_id -- Azure Tenant ID to generate script for.
                      Defaults to the most recently registered tenant.
         parameters -- full parameters payload, not required if tenant-id keyword is used.
+        subscription_ids -- Subscription IDs to generate script for. Defaults to all. String or list of strings.
+        template -- Template to be rendered. String.
 
         Arguments: When not specified, the first argument to this method is assumed to be
                    'tenant-id'. All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
@@ -505,14 +558,16 @@
         azure_tenant_id -- Azure tenant ID. String.
         cloud_provider -- Cloud provider. Allowed values: `azure`, `aws`, `gcp`. String.
         date_time_since -- Filter to retrieve all events after this date. RFC3339 formatted string.
                            Example: 2006-01-01T12:00:01Z07:00
         limit -- The maximum number of records to return in this response. [Integer, 1-500]
         next_token -- String to get next page of results, associated with the previous
                       execution. Must include all filters from previous execution. String.
+        resource_id -- Resource ID. String.
+        resource_uuid - Resource UUID. String.
         service -- Cloud Service (Example: `EC2` or `S3`). String.
                    Available options
                    ACM                      Identity
                    ACR                      KMS
                    Any                      KeyVault
                    App Engine               Kinesis
                    BigQuery                 Kubernetes
@@ -535,14 +590,15 @@
                    EKS                      StorageAccount
                    ELB                      Subscriptions
                    EMR                      VPC
                    Elasticache              VirtualMachine
                    GuardDuty                VirtualNetwork
                    IAM
         severity -- Severity (e.g. `High`, `Medium` or `Informational`). String.
+        since -- Filter events using a duration string (e.g. 24h). String. Default: 24h
         state -- State. (e.g. `open` or `closed`). String.
         parameters - full parameters payload, not required if using other keywords.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
@@ -620,14 +676,96 @@
             endpoints=Endpoints,
             operation_id="GetConfigurationDetections",
             keywords=kwargs,
             params=parameters
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
+    def get_configuration_detection_entities(self: object,
+                                             *args,
+                                             parameters: dict = None,
+                                             **kwargs
+                                             ) -> dict:
+        """
+        Get misconfigurations based on the ID - including custom policy detections in addition to default policy detections.
+
+        Keyword arguments:
+        ids -- Detection IDs to retrieve. String or List of Strings.
+        parameters -- full parameters payload, not required ids keyword is used.
+
+        Arguments: When not specified, the first argument to this method is assumed to be 'ids'. All others are ignored.
+
+        Returns: dict object containing API response.
+
+        HTTP Method: GET
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/cspm-registration/GetConfigurationDetectionEntities
+        """
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="GetConfigurationDetectionEntities",
+            keywords=kwargs,
+            params=handle_single_argument(args, parameters, "ids")
+            )
+
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def get_configuration_detection_ids_v2(self: object,
+                                           parameters: dict = None,
+                                           **kwargs
+                                           ) -> dict:
+        """
+        Get list of active misconfiguration ids - including custom policy detections in addition to default policy detections.
+
+        Keyword arguments:
+        filter -- FQL formatted string to filter result. String.
+                  Allowed filters
+                  account_name              policy_id
+                  account_id                policy_type
+                  agent_id                  resource_id
+                  attack_types              region
+                  azure_subscription_id     status
+                  cloud_provider            scan_time
+                  cloud_service_keyword     severity
+                  custom_policy_id          severity_string
+                  is_managed                use_current_scan_ids (*)
+                  (*) Use this to retrieve records for the latest scans
+        limit -- Maximum number of detections to return. Integer. (Default: 500)
+        offset -- Starting offset for returned detections. Integer.
+        sort -- FQL formatted sort. String. Default: timestamp|desc
+                Allowed values
+                account_name            policy_id
+                accoud_id               policy_type
+                attack_types            resource_id
+                azure_subscription_id   region
+                cloud_provider          scan_name
+                cloud_service_keyword   severity
+                status                  severity_string
+                is_managed              timestamp
+        parameters -- full parameters payload, not required if using other keywords.
+
+        This method only supports keywords for providing arguments.
+
+        Returns: dict object containing API response.
+
+        HTTP Method: GET
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/cspm-registration/GetConfigurationDetectionIDsV2
+        """
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="GetConfigurationDetectionIDsV2",
+            keywords=kwargs,
+            params=parameters
+            )
+
+    @force_default(defaults=["parameters"], default_types=["dict"])
     def get_ioa_events(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """For CSPM IOA events, gets list of IOA events.
 
         Keyword arguments:
         policy_id -- Policy ID. String.
         cloud_provider -- Cloud provider. Allowed values: `azure`, `aws`, `gcp`. String.
         account_id -- Cloud Account ID (AWS account ID, Azure Subscription ID, etc.)
@@ -713,14 +851,40 @@
             endpoints=Endpoints,
             operation_id="GetCSPMPolicy",
             keywords=kwargs,
             params=handle_single_argument(args, parameters, "ids")
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
+    def get_policy_details(self: object, *args, parameters: dict = None, **kwargs) -> dict:
+        """Given an array of policy IDs, returns detailed policies information.
+
+        Keyword arguments:
+        ids -- Policy IDs to retrieve. String or list of strings.
+        parameters -- full parameters payload, not required if ids is provided as a keyword.
+
+        Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
+                   All others are ignored.
+
+        Returns: dict object containing API response.
+
+        HTTP Method: GET
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/cspm-registration/GetCSPMPoliciesDetails
+        """
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="GetCSPMPoliciesDetails",
+            keywords=kwargs,
+            params=handle_single_argument(args, parameters, "ids")
+            )
+
+    @force_default(defaults=["parameters"], default_types=["dict"])
     def get_policy_settings(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Return information about current policy settings.
 
         Keyword arguments:
         policy_id -- Policy ID. String.
         cloud_platform -- Cloud platform. Allowed values: `azure`, `aws`, `gcp`. String.
         service -- Service type to filter policy settings by.
@@ -780,25 +944,29 @@
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 {
                     "resources": [
                         {
                             "account_id": "string",
+                            "account_ids": [
+                                "string"
+                            ],
                             "enabled": boolean,
                             "policy_id": integer,
                             "regions": [
                                 "string"
                             ],
                             "severity": "string",
                             "tag_excluded": boolean
                         }
                     ]
                 }
         account_id -- Account ID to update. String.
+        account_ids -- Account IDs to update. List of strings.
         enabled -- Enabled / Disable flag. Boolean.
         policy_id -- Policy ID to be updated. Integer.
         region -- List of regions. String or list of strings.
         severity -- Severity value to set for policy. String.
         tag_excluded -- Exclude tags flag. Boolean.
 
         This method only supports keywords for providing arguments.
@@ -856,20 +1024,22 @@
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 {
                     "resources": [
                         {
                             "cloud_platform": "string",
                             "next_scan_timestamp": "2021-10-25T05:22:27.365Z",
+                            "scan_interval": "string",
                             "scan_schedule": "string"
                         }
                     ]
                 }
         cloud_platform -- Cloud platform. String.
         next_scan_timestamp -- Time to schedule scan. UTC date formatted string.
+        scan_interval -- Scan interval. String.
         scan_schedule -- Scan schedule type. String.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: POST
@@ -901,17 +1071,20 @@
     DeleteCSPMAzureAccount = delete_azure_account
     UpdateCSPMAzureAccountClientID = update_azure_account_client_id
     UpdateCSPMAzureTenantDefaultSubscriptionID = update_azure_tenant_default_subscription_id
     GetCSPMAzureUserScriptsAttachment = get_azure_user_scripts_attachment
     AzureDownloadCertificate = azure_download_certificate
     GetBehaviorDetections = get_behavior_detections
     GetConfigurationDetections = get_configuration_detections
+    GetConfigurationDetectionEntities = get_configuration_detection_entities
+    GetConfigurationDetectionIDsV2 = get_configuration_detection_ids_v2
     GetIOAEvents = get_ioa_events
     GetIOAUsers = get_ioa_users
     GetCSPMPolicy = get_policy
+    GetCSPMPoliciesDetails = get_policy_details
     GetCSPMPolicySettings = get_policy_settings
     UpdateCSPMPolicySettings = update_policy_settings
     GetCSPMScanSchedule = get_scan_schedule
     UpdateCSPMScanSchedule = update_scan_schedule
 
 
 # The legacy name for this class does not conform to PascalCase / PEP8
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/custom_ioa.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/d4c_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/d4c_registration.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,19 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 from typing import Dict, Union
 from ._util import force_default, process_service_request, handle_single_argument
-from ._payload import azure_registration_payload, aws_d4c_registration_payload
+from ._payload import (
+    azure_registration_payload,
+    aws_d4c_registration_payload,
+    gcp_registration_payload
+    )
 from ._service_class import ServiceClass
 from ._endpoint._d4c_registration import _d4c_registration_endpoints as Endpoints
 
 
 class D4CRegistration(ServiceClass):
     """The only requirement to instantiate an instance of this class is one of the following.
 
@@ -103,20 +107,22 @@
         body -- full body payload, not required if using other keywords.
                 {
                     "resources": [
                         {
                             "account_id": "string",
                             "account_type": "string",
                             "cloudtrail_region": "string",
+                            "iam_role_arn": "string",
                             "is_master": true,
                             "organization_id": "string"
                         }
                     ]
                 }
-        cloudtrail_region -- AWS region for CloudTrail log access.
+        cloudtrail_region -- AWS region for CloudTrail log access. String.
+        iam_role_arn -- AWS IAM role ARN. String.
         is_master -- Flag indicating if this is the master account. Boolean.
         organization_id -- AWS organization ID. String.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
@@ -215,75 +221,88 @@
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def get_azure_account(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Return information about Azure account registration.
 
         Keyword arguments:
-        ids -- List of Azure Account IDs to retrieve. String or list of strings.
+        ids -- List of Azure Account IDs to retrieve. If this is empty then all accounts are returned.
+               String or list of strings.
+        limit -- The maximum records to return. Defaults to 100. Integer.
+        offset -- The offset to start retrieving records from. Integer.
         parameters -- full parameters payload, not required if ids is provided as a keyword.
         scan_type -- Type of scan, `dry` or `full`, to perform on selected accounts.
+        status -- Account status to filter results by, 'provisioned' or 'operational'. String.
+        tenant_ids -- Tenant ids to filter azure accounts returned. String or list of strings.
 
         Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
                    All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/GetCSPMAzureAccount
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/GetDiscoverCloudAzureAccount
         """
         if kwargs.get("scan_type", None):
             kwargs["scan-type"] = kwargs.get("scan_type", None)
 
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="GetCSPMAzureAccount",
+            operation_id="GetDiscoverCloudAzureAccount",
             keywords=kwargs,
             params=handle_single_argument(args, parameters, "ids")
             )
 
     @force_default(defaults=["body"], default_types=["dict"])
     def create_azure_account(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Register a new Azure account.
 
         Creates a new account in our system for a customer and generates a
         script for them to run in their cloud environment to grant us access.
 
         Keyword arguments:
+        account_type -- Azure Account type. String.
         body -- full body payload, not required if using other keywords.
                 {
                     "resources": [
                         {
+                            "account_type": "string",
+                            "client_id": "string",
+                            "default_subscription": true,
                             "subscription_id": "string",
-                            "tenant_id": "string"
+                            "tenant_id": "string",
+                            "years_valid": integer
                         }
                     ]
                 }
+        client_id -- Azure Client ID. String.
+        default_subscription -- Is this the default subscription? Boolean.
         subscription_id -- Azure subscription ID. String.
         tenant_id -- Azure tenant ID. String.
+        years_valid -- Years valid. Integer.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: POST
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/CreateCSPMAzureAccount
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/CreateDiscoverCloudAzureAccount
         """
         if not body:
             body = azure_registration_payload(passed_keywords=kwargs)
 
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="CreateCSPMAzureAccount",
+            operation_id="CreateDiscoverCloudAzureAccount",
             body=body
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def update_azure_account_client_id(self: object,
                                        *args,
                                        parameters: dict = None,
@@ -293,53 +312,74 @@
 
         Update an Azure service account in our system by with the
         user-created client_id created with the public key we've provided.
 
         Keyword arguments:
         id -- ClientID to use for the Service Principal associated
               with the customer's Azure Account.
+        object_id -- Object ID to use for the Service Principal associated
+                     with the customer's Azure account. String.
         parameters -- full parameters payload, not required if ids is provided as a keyword.
+        tenant_id -- Tenant ID to update client ID for.
+                     Required if multiple tenants are registered. String.
 
         Arguments: When not specified, the first argument to this method is assumed to be 'id'.
                    All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: PATCH
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/UpdateCSPMAzureAccountClientID
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#
+            /d4c-registration/UpdateDiscoverCloudAzureAccountClientID
         """
+        if kwargs.get("tenant_id", None):
+            kwargs["tenant-id"] = kwargs.get("tenant_id", None)
+
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="UpdateCSPMAzureAccountClientID",
+            operation_id="UpdateDiscoverCloudAzureAccountClientID",
             keywords=kwargs,
             params=handle_single_argument(args, parameters, "id")
             )
 
-    def get_azure_user_scripts_attachment(self: object) -> Dict[str, Union[int, dict]]:
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def get_azure_user_scripts_attachment(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve Azure user script attachment.
 
         Return a script for customer to run in their cloud environment to
         grant us access to their Azure environment as a downloadable attachment.
 
-        This method does not accept arguments or keywords.
+        Keyword arguments:
+        parameters -- full parameters payload, not required if using other keywords.
+        subscription_ids -- Azure subscription IDs. String or list of strings.
+        template -- Template to be rendered. String.
+        tenant_id -- Azure tenant ID. String.
+
+        This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/GetCSPMAzureUserScriptsAttachment
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#
+            /d4c-registration/GetDiscoverCloudAzureUserScriptsAttachment
         """
+        if kwargs.get("tenant_id", None):
+            kwargs["tenant-id"] = kwargs.get("tenant_id", None)
+
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="GetCSPMAzureUserScriptsAttachment"
+            operation_id="GetDiscoverCloudAzureUserScriptsAttachment",
+            keywords=kwargs,
+            params=parameters
             )
 
     def get_azure_user_scripts(self: object) -> Dict[str, Union[int, dict]]:
         """Retrieve Azure user script.
 
         Return a script for customer to run in their cloud
         environment to grant us access to their Azure environment.
@@ -347,45 +387,49 @@
         This method does not accept arguments or keywords.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/GetCSPMAzureUserScripts
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/GetDiscoverCloudAzureUserScripts
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="GetCSPMAzureUserScripts"
+            operation_id="GetDiscoverCloudAzureUserScripts"
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def get_gcp_account(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Return information about the current status of an GCP account.
 
         Keyword arguments:
-        ids -- List of Response Policy IDs to retrieve. String or list of strings.
+        ids -- Hierarchical Resource IDs of accounts. String or list of strings.
+        limit -- The maximum records to return. Defaults to 100. Integer.
+        offset -- The offset to start retrieving records from. Integer.
         parameters -- full parameters payload, not required if ids is provided as a keyword.
+        parent_type -- GCP Hierarchy Parent Type, organization/folder/project. String.
         scan_type -- Type of scan, `dry` or `full`, to perform on selected accounts.
+        sort -- Order fields in ascending or descending order. Ex: parent_type|asc.
+        status -- Account status to filter results by, 'operational' or 'provisioned'. String.
 
-        Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
-                   All others are ignored.
+        This method does not accept arguments or keywords.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/GetCSPMCGPAccount
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/GetD4CCGPAccount
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="GetCSPMCGPAccount",
+            operation_id="GetD4CCGPAccount",
             keywords=kwargs,
             params=parameters
             )
 
     @force_default(defaults=["body"], default_types=["dict"])
     def create_gcp_account(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Register new GCP account.
@@ -394,52 +438,53 @@
         account for them to add access to in their GCP environment to grant us access.
 
         Keyword arguments:
         body -- full body payload, not required if using other keywords.
                 {
                     "resources": [
                         {
-                            "parent_id": "string"
+                            "parent_id": "string",
+                            "parent_type": "string"
                         }
                     ]
                 }
         parent_id -- GCP parent ID. String.
+        parent_type -- GCP parent type. String.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: POST
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/CreateCSPMGCPAccount
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/CreateD4CGCPAccount
         """
         if not body:
-            body = {}
-            body["resources"] = []
-            body["resources"].append({"parent_id": kwargs.get("parent_id", None)})
+            body = gcp_registration_payload(passed_keywords=kwargs)
 
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="CreateCSPMGCPAccount",
+            operation_id="CreateD4CGCPAccount",
             body=body
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def azure_download_certificate(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Download Azure Certificate.
 
         Returns JSON object(s) that contain the base64 encoded certificate for a service principal.
 
         Keyword arguments:
         tenant_id -- Azure Tenant ID to generate script for.
                      Defaults to the most recently registered tenant.
         parameters -- full parameters payload, not required if tenant-id keyword is used.
         refresh -- Force a refresh of the certificate. Boolean. Defaults to False.
+        years_valid -- Years the certificate should be valid (only used when refresh=true). String.
 
         Arguments: When not specified, the first argument to this method is assumed to be
                    'tenant_id'. All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
@@ -451,14 +496,32 @@
             calling_object=self,
             endpoints=Endpoints,
             operation_id="DiscoverCloudAzureDownloadCertificate",
             keywords=kwargs,
             params=handle_single_argument(args, parameters, "tenant_id")
             )
 
+    def get_azure_tenant_ids(self: object) -> dict:
+        """Return all available Azure tenant ids.
+
+        This method does not accept keywords or arguments.
+
+        Returns: dict object containing API response.
+
+        HTTP Method: GET
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/GetDiscoverCloudAzureTenantIDs
+        """
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="GetDiscoverCloudAzureTenantIDs"
+            )
+
     def get_gcp_user_scripts_attachment(self: object) -> Dict[str, Union[int, dict]]:
         """Retrieve GCP user script attachment.
 
         Return a script for customer to run in their cloud environment to
         grant us access to their GCP environment as a downloadable attachment.
 
         This method does not accept arguments or keywords.
@@ -472,33 +535,41 @@
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
             operation_id="GetCSPMGCPUserScriptsAttachment"
             )
 
-    def get_gcp_user_scripts(self: object) -> Dict[str, Union[int, dict]]:
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def get_gcp_user_scripts(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve GCP user script.
 
         Return a script for customer to run in their cloud
         environment to grant us access to their GCP environment.
 
-        This method does not accept arguments or keywords.
+        Keyword arguments:
+        parent_type -- GCP Hierarchy Parent Type, organization/folder/project. String.
+        parameters - full parameters payload, not required if using other keywords.
+
+        Arguments: When not specified, the first argument to this method is assumed to be
+                   'parent_type'. All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/GetCSPMGCPUserScripts
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/GetD4CGCPUserScripts
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="GetCSPMGCPUserScripts"
+            operation_id="GetD4CGCPUserScripts",
+            keywords=kwargs,
+            params=handle_single_argument(args, parameters, "parent_type")
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def get_aws_horizon_scripts(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Return a script for customer to run in their cloud environment to grant CrowdStrike access.
 
         Keyword arguments:
@@ -531,23 +602,33 @@
     # backwards compatibility / ease of use purposes
     GetD4CAwsAccount = get_aws_account
     CreateD4CAwsAccount = create_aws_account
     DeleteD4CAwsAccount = delete_aws_account
     GetD4CAwsConsoleSetupURLs = get_aws_console_setup
     GetD4CAWSAccountScriptsAttachment = get_aws_account_scripts
     GetCSPMAzureAccount = get_azure_account
+    GetDiscoverCloudAzureAccount = get_azure_account
     CreateCSPMAzureAccount = create_azure_account
+    CreateDiscoverCloudAzureAccount = create_azure_account
     UpdateCSPMAzureAccountClientID = update_azure_account_client_id
+    UpdateDiscoverCloudAzureAccountClientID = update_azure_account_client_id
     GetCSPMAzureUserScriptsAttachment = get_azure_user_scripts_attachment
+    GetDiscoverCloudAzureUserScriptsAttachment = get_azure_user_scripts_attachment
     DiscoverCloudAzureDownloadCertificate = azure_download_certificate
+    GetDiscoverCloudAzureTenantIDs = get_azure_tenant_ids
     GetCSPMAzureUserScripts = get_azure_user_scripts
+    GetDiscoverCloudAzureUserScripts = get_azure_user_scripts
     GetCSPMGCPAccount = get_gcp_account   # Typo fix
     GetCSPMCGPAccount = get_gcp_account
+    GetD4CGCPAccount = get_gcp_account  # Typo fix
+    GetD4CCGPAccount = get_gcp_account
     CreateCSPMGCPAccount = create_gcp_account
+    CreateD4CGCPAccount = create_gcp_account
     GetCSPMGCPUserScriptsAttachment = get_gcp_user_scripts_attachment
     GetCSPMGCPUserScripts = get_gcp_user_scripts
+    GetD4CGCPUserScripts = get_gcp_user_scripts
     GetHorizonD4CScripts = get_aws_horizon_scripts
 
 
 # The legacy name for this class does not conform to PascalCase / PEP8
 # It is defined here for backwards compatibility purposes only.
 D4C_Registration = D4CRegistration  # pylint: disable=C0103
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/debug.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/debug.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/detects.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/detects.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,17 +66,21 @@
                     {
                         "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
                         ],
+                        "exclude": "string",
                         "field": "string",
                         "filter": "string",
+                        "from": 0,
+                        "include": "string",
                         "interval": "string",
+                        "max_doc_count": 0,
                         "min_doc_count": 0,
                         "missing": "string",
                         "name": "string",
                         "q": "string",
                         "ranges": [
                         {
                             "From": 0,
@@ -88,19 +92,28 @@
                         "sub_aggregates": [
                             null
                         ],
                         "time_zone": "string",
                         "type": "string"
                     }
                 ]
-        date_ranges -- List of dictionaries.
-        field -- String.
-        filter -- FQL syntax. String.
+        date_ranges -- If peforming a date range query specify the from and to date ranges.
+                       These can be in common date formats like 2019-07-18 or now.
+                       List of dictionaries.
+        exclude -- Fields to exclude. String.
+        field -- Term you want to aggregate on. If doing a date_range query,
+                 this is the date field you want to apply the date ranges to. String.
+        filter -- Optional filter criteria in the form of an FQL query.
+                  For more information about FQL queries, see our FQL documentation in Falcon.
+                  String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
         name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
         size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
@@ -136,22 +149,26 @@
         body -- full body payload, not required when using other keywords.
                 {
                     "assigned_to_uuid": "string",
                     "comment": "string",
                     "ids": [
                         "string"
                     ],
+                    "new_behaviors_processed": [
+                        "string"
+                    ],
                     "show_in_ui": true,
                     "status": "string"
                 }
         comment -- Optional comment to add to the detection. Comments are displayed with
                    the detection in Falcon and are usually used to provide context or
                    notes for other Falcon users. A detection can have multiple comments
                    over time.
         ids -- ID(s) of the detection to update. String or list of strings.
+        new_behaviors_processed -- String or list of strings.
         show_in_ui -- Boolean determining if this detection is displayed in the Falcon
                       console.
         status -- Current status of the detection. Allowed values:
                   ignored           new
                   in_progress       true_positive
                   false_positive
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/device_control_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/device_control_policies.py`

 * *Files 3% similar despite different names*

```diff
@@ -210,16 +210,16 @@
             )
 
     @force_default(defaults=["parameters", "body"], default_types=["dict", "dict"])
     def perform_action(self: object, body: dict = None, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Perform a Device Control Policy action.
 
         Keyword arguments:
-        action_name -- action to perform: 'add-host-group', 'disable', 'enable',
-                       or 'remove-host-group'.
+        action_name -- action to perform: 'add-host-group', 'add-rule-group', 'disable', 'enable',
+                       'remove-rule-group' or 'remove-host-group'.
         action_parameters -- Action specific parameter options. List of dictionaries.
                              {
                                  "name": "string",
                                  "value": "string"
                              }
         body -- full body payload, not required if keywords are used.
                 {
@@ -349,50 +349,64 @@
     @force_default(defaults=["body"], default_types=["dict"])
     def create_policies(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Create Device Control Policies by specifying details about the policy to create.
 
         Keyword arguments:
         body -- full body payload, not required if keywords are used.
                 {
-                "resources": [
-                    {
-                        "clone_id": "string",
-                        "description": "string",
-                        "name": "string",
-                        "platform_name": "Windows",
-                        "settings": {
-                            "classes": [
-                            {
-                                "action": "FULL_ACCESS",
-                                "exceptions": [
-                                {
-                                    "action": "string",
-                                    "class": "string",
-                                    "combined_id": "string",
-                                    "id": "string",
-                                    "match_method": "string",
-                                    "product_id": "string",
-                                    "product_id_decimal": "string",
-                                    "product_name": "string",
-                                    "serial_number": "string",
-                                    "vendor_id": "string",
-                                    "vendor_id_decimal": "string",
-                                    "vendor_name": "string"
-                                }
+                    "resources": [
+                        {
+                            "clone_id": "string",
+                            "description": "string",
+                            "name": "string",
+                            "platform_name": "Windows",
+                            "settings": {
+                                "classes": [
+                                    {
+                                        "action": "FULL_ACCESS",
+                                        "exceptions": [
+                                            {
+                                                "action": "string",
+                                                "combined_id": "string",
+                                                "description": "string",
+                                                "expiration_time": "2023-06-08T06:04:53.563Z",
+                                                "id": "string",
+                                                "product_id": "string",
+                                                "product_id_decimal": "string",
+                                                "product_name": "string",
+                                                "serial_number": "string",
+                                                "use_wildcard": true,
+                                                "vendor_id": "string",
+                                                "vendor_id_decimal": "string",
+                                                "vendor_name": "string"
+                                            }
+                                        ],
+                                        "id": "string"
+                                    }
+                                ],
+                                "custom_notifications": {
+                                    "blocked_notification": {
+                                        "custom_message": "string",
+                                        "use_custom": true
+                                    },
+                                    "restricted_notification": {
+                                        "custom_message": "string",
+                                        "use_custom": true
+                                    }
+                                },
+                                "delete_exceptions": [
+                                    "string"
                                 ],
-                                "id": "string"
+                                "end_user_notification": "SILENT",
+                                "enforcement_mode": "MONITOR_ONLY",
+                                "enhanced_file_metadata": true
                             }
-                            ],
-                            "end_user_notification": "TRUE",
-                            "enforcement_mode": "string",
-                            "id": "string"
                         }
-                    }
-                ]
-            }
+                    ]
+                }
         clone_id -- ID of the Device Control Policy to clone. String.
         description -- Device Control Policy description. String.
         name -- Device Control Policy name. String.
         platform_name -- Name of the operating system platform. String.
         settings -- Device Control policy specific settings. Dictionary.
                     See above for JSON dictionary format example.
 
@@ -446,50 +460,63 @@
     @force_default(defaults=["body"], default_types=["dict"])
     def update_policies(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Update Device Control Policies by specifying the ID of the policy and details to update.
 
         Keyword arguments:
         body -- full body payload, not required if keywords are used.
                 {
-                "resources": [
-                    {
-                        "clone_id": "string",
-                        "description": "string",
-                        "name": "string",
-                        "platform_name": "Windows",
-                        "settings": {
-                            "classes": [
-                            {
-                                "action": "FULL_ACCESS",
-                                "exceptions": [
-                                {
-                                    "action": "string",
-                                    "class": "string",
-                                    "combined_id": "string",
-                                    "id": "string",
-                                    "match_method": "string",
-                                    "product_id": "string",
-                                    "product_id_decimal": "string",
-                                    "product_name": "string",
-                                    "serial_number": "string",
-                                    "vendor_id": "string",
-                                    "vendor_id_decimal": "string",
-                                    "vendor_name": "string"
-                                }
+                    "resources": [
+                        {
+                            "description": "string",
+                            "id": "string",
+                            "name": "string",
+                            "settings": {
+                                "classes": [
+                                    {
+                                        "action": "FULL_ACCESS",
+                                        "exceptions": [
+                                            {
+                                                "action": "string",
+                                                "combined_id": "string",
+                                                "description": "string",
+                                                "expiration_time": "2023-06-08T06:10:39.965Z",
+                                                "id": "string",
+                                                "product_id": "string",
+                                                "product_id_decimal": "string",
+                                                "product_name": "string",
+                                                "serial_number": "string",
+                                                "use_wildcard": true,
+                                                "vendor_id": "string",
+                                                "vendor_id_decimal": "string",
+                                                "vendor_name": "string"
+                                            }
+                                        ],
+                                        "id": "string"
+                                    }
+                                ],
+                                "custom_notifications": {
+                                    "blocked_notification": {
+                                        "custom_message": "string",
+                                        "use_custom": true
+                                    },
+                                    "restricted_notification": {
+                                        "custom_message": "string",
+                                        "use_custom": true
+                                    }
+                                },
+                                "delete_exceptions": [
+                                    "string"
                                 ],
-                                "id": "string"
+                                "end_user_notification": "SILENT",
+                                "enforcement_mode": "MONITOR_ONLY",
+                                "enhanced_file_metadata": true
                             }
-                            ],
-                            "end_user_notification": "TRUE",
-                            "enforcement_mode": "string",
-                            "id": "string"
                         }
-                    }
-                ]
-            }
+                    ]
+                }
         id -- ID of the Device Control Policy to update. String.
         description -- Device Control Policy description. String.
         name -- Device Control Policy name. String.
         settings -- Device Control policy specific settings. Dictionary.
                     See above for JSON dictionary format example.
 
         This method only supports keywords for providing arguments.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/discover.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/discover.py`

 * *Files 13% similar despite different names*

```diff
@@ -321,15 +321,15 @@
         """Search for logins in your environment.
 
         Supports providing a FQL (Falcon Query Language) filter and paging details.
         Returns a set of asset IDs which match the filter criteria.
 
         Keyword arguments:
         filter -- The filter expression that should be used to limit the results. FQL syntax.
-                  Common sort options include:
+                  Common filter options include:
                     account_type:'Local'
                     login_type:'Interactive'
                     first_seen_timestamp:<'now-7d'
                     admin_privileges:'No'
                   Available Filters:
                     id                  login_timestamp
                     cid                 login_domain
@@ -367,7 +367,106 @@
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
             operation_id="query_logins",
             keywords=kwargs,
             params=parameters
             )
+
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def get_iot_hosts(self: object, *args, parameters: dict = None, **kwargs) -> dict:
+        """Get details on IoT assets by providing one or more IDs.
+
+        Find IoT assets with `query_iot_hosts`.
+
+        Keyword arguments:
+        ids -- One or more login IDs (max: 100). String or list of strings.
+        parameters - full parameters payload, not required if ids is provided as a keyword.
+
+        Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
+                   All others are ignored.
+
+        Returns: dict object containing API response.
+
+        HTTP Method: GET
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/discover/get-iot-hosts
+        """
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="get_iot_hosts",
+            keywords=kwargs,
+            params=handle_single_argument(args, parameters, "ids")
+            )
+
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def query_iot_hosts(self: object, parameters: dict = None, **kwargs) -> dict:
+        """Search for IoT assets in your environment.
+
+        Supports providing a FQL (Falcon Query Language) filter and paging details.
+        Returns a set of asset IDs which match the filter criteria.
+
+        Keyword arguments:
+        filter -- The filter expression that should be used to limit the results. FQL syntax.
+                  Common filter options include:
+                    entity_type:'managed'
+                    product_type_desc:'Workstation'
+                    platform_name:'Windows'
+                    last_seen_timestamp:>'now-7d'
+                  Available Filters:
+                    agent_version                   last_seen_timestamp
+                    aid                             local_ip_addresses
+                    bios_manufacturer               local_ips_count
+                    bios_version                    mac_addresses
+                    business_criticality            machine_domain
+                    cid                             network_id
+                    city                            network_interfaces
+                    claroty_id                      number_of_disk_drives
+                    confidence                      os_is_eol
+                    country                         os_version
+                    current_local_ip                ou
+                    data_providers                  physical_core_count
+                    data_providers_count            platform_name
+                    device_class                    processor_package_count
+                    device_family                   product_type_desc
+                    device_type                     protocols
+                    discoverer_count                purdue_level
+                    discoverer_product_type_descs   reduced_functionality_mode
+                    entity_type                     site_name
+                    external_ip                     subnet
+                    first_seen_timestamp            system_manufacturer
+                    groups                          system_product_name
+                    hostname                        system_serial_number
+                    ics_id                          tags
+                    id                              virtual_zone
+                    internet_exposure               vlan
+                    kernel_version
+        limit -- The number of asset IDs to return in this response. (Max: 100, default: 100)
+                 Use with the offset parameter to manage pagination of results.
+        offset -- An offset used with the limit parameter to manage pagination of results.
+                  On your first request, don’t provide an offset. On subsequent requests,
+                  provide the offset from the previous response to continue from that place
+                  in the results.
+        parameters - full parameters payload, not required if using other keywords.
+        sort -- Sort assets by their properties. A single sort field is allowed.
+                Common sort options include:
+                  hostname|asc
+                  product_type_desc|desc
+
+        This method only supports keywords for providing arguments.
+
+        Returns: dict object containing API response.
+
+        HTTP Method: GET
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/discover/query-iot-hosts
+        """
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="query_iot_hosts",
+            keywords=kwargs,
+            params=parameters
+            )
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/event_streams.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/falcon_complete_dashboard.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/falcon_complete_dashboard.py`

 * *Files 8% similar despite different names*

```diff
@@ -134,57 +134,67 @@
     @force_default(defaults=["body"], default_types=["list"])
     def aggregate_block_list(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve aggregate blocklist ticket values based on the matched filter.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
 
@@ -210,57 +220,67 @@
     @force_default(defaults=["body"], default_types=["list"])
     def aggregate_detections(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve aggregate detection values based on the matched filter.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
 
@@ -286,57 +306,67 @@
     @force_default(defaults=["body"], default_types=["list"])
     def aggregate_device_count_collection(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve aggregate host/devices count based on the matched filter.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
 
@@ -364,57 +394,67 @@
     @force_default(defaults=["body"], default_types=["list"])
     def aggregate_escalations(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve aggregate escalation ticket values based on the matched filter.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
 
@@ -440,57 +480,67 @@
     @force_default(defaults=["body"], default_types=["list"])
     def aggregate_fc_incidents(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve aggregate incident values based on the matched filter.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
 
@@ -516,57 +566,67 @@
     @force_default(defaults=["body"], default_types=["list"])
     def aggregate_remediations(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve aggregate remediation ticket values based on the matched filter.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/falcon_container.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/fdr.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Falcon Container API Interface Class.
+"""CrowdStrike Falcon Data Replicator API interface class.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -31,42 +31,40 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-from typing import Dict, Union
-from ._util import process_service_request, force_default
-from ._payload import image_payload
+from ._util import force_default, process_service_request, handle_single_argument
 from ._service_class import ServiceClass
-from ._endpoint._falcon_container import _falcon_container_endpoints as Endpoints
+from ._endpoint._fdr import _fdr_endpoints as Endpoints
 
 
-class FalconContainer(ServiceClass):
+class FDR(ServiceClass):
     """The only requirement to instantiate an instance of this class is one of the following.
 
     - a valid client_id and client_secret provided as keywords.
     - a credential dictionary with client_id and client_secret containing valid API credentials
       {
           "client_id": "CLIENT_ID_HERE",
           "client_secret": "CLIENT_SECRET_HERE"
       }
     - a previously-authenticated instance of the authentication service class (oauth2.py)
     - a valid token provided by the authentication service class (oauth2.py)
     """
 
-    def get_credentials(self: object) -> Dict[str, Union[int, dict]]:
-        """Retrieve the registry credentials.
+    def get_event_combined(self: object) -> dict:
+        """Fetch combined schema.
 
         HTTP Method: GET
 
         Swagger URL
         ----
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/falcon-container/GetCredentials
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/event%20schema/fdrschema.combined.event.get
 
         Keyword arguments
         ----
         This method does not accept keyword arguments.
 
         Arguments
         ----
@@ -76,174 +74,168 @@
         ----
         dict
             Dictionary object containing API response.
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="GetCredentials"
+            operation_id="fdrschema_combined_event_get"
             )
 
-    @force_default(defaults=["body"], default_types=["dict"])
-    def read_image_vulnerabilities(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Retrieve an assessment report for an image by specifying repository and tag.
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def get_event_entities(self: object, *args, parameters: dict = None, **kwargs) -> dict:
+        """Fetch event schema by ID.
 
-        HTTP Method: POST
+        HTTP Method: GET
 
         Swagger URL
         ----
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/falcon-container-cli/ReadImageVulnerabilities
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/event%20schema/fdrschema.entities.event.get
 
         Keyword arguments
         ----
-        body : str
-            Full body payload in JSON format, not required when using other keywords.
-            {
-                "osversion": "string",
-                "packages": [
-                    {
-                        "LayerHash": "string",
-                        "LayerIndex": 0,
-                        "MajorVersion": "string",
-                        "PackageHash": "string",
-                        "PackageProvider": "string",
-                        "PackageSource": "string",
-                        "Product": "string",
-                        "SoftwareArchitecture": "string",
-                        "Status": "string",
-                        "Vendor": "string"
-                    }
-                ]
-            }
-        packages : list[dict]
-            List of images to retrieve vulnerabilities for.
-        osversion : str
-            Operating system version for the image to be checked.
+        ids : str
+            FDR feed IDs to retrieve.
+        parameters : dict
+            Full parameters payload. Not required if using other keywords.
 
-        This method only supports keywords for providing arguments.
+        Arguments
+        ----
+        When not specified, the first argument to this method is assumed to be 'ids'.
+        All others are ignored.
 
         Returns
         ----
         dict
             Dictionary object containing API response.
         """
-        if not body:
-            body = image_payload(passed_keywords=kwargs)
-
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="ReadImageVulnerabilities",
+            operation_id="fdrschema_entities_event_get",
             keywords=kwargs,
-            body=body
+            params=handle_single_argument(args, parameters, "ids")
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
-    def get_assessment(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Retrieve an assessment report for an image by specifying repository and tag.
+    def query_event_entities(self: object, parameters: dict = None, **kwargs) -> dict:
+        """Get a list of event IDs given a particular query.
 
         HTTP Method: GET
 
         Swagger URL
         ----
-        This operation does not exist in swagger.
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/event%20schema/fdrschema.queries.event.get
 
         Keyword arguments
         ----
-        repository : str (required)
-            Repository where the image resides.
-        parameters : str (JSON)
-            Full parameters payload in JSON string format. Not required if using keywords.
-        tag : str (required)
-            Tag used for the image assessed.
+        filter : str
+            FQL formatted filter to limit returned results.
+        limit : int
+            The maximum number of records to return in this response.
+            Use with the offset parameter to manage pagination of results.
+        offset : int
+            The offset to start retrieving records from.
+            Use with the limit parameter to manage pagination of results.
+        parameters : dict
+            Full parameters payload. Not required if using other keywords.
+        sort : str
+            The property to sort by. FQL syntax.
 
         This method only supports keywords for providing arguments.
 
         Returns
         ----
         dict
             Dictionary object containing API response.
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="GetImageAssessmentReport",
+            operation_id="fdrschema_queries_event_get",
             keywords=kwargs,
             params=parameters
             )
 
-    def delete_image_details(self: object, *args, image_id: str = None) -> Dict[str, Union[int, dict]]:
-        """Delete image details from the CrowdStrike registry.
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def get_field_entities(self: object, *args, parameters: dict = None, **kwargs) -> dict:
+        """Fetch event schema by ID.
 
-        HTTP Method: DELETE
+        HTTP Method: GET
 
         Swagger URL
         ----
-        This operation does not exist in swagger.
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/field%20schema/fdrschema.entities.field.get
 
         Keyword arguments
         ----
-        image_id : str (required)
-            ID of the image to delete details for.
+        ids : str
+            FDR feed IDs to retrieve.
+        parameters : dict
+            Full parameters payload. Not required if using other keywords.
 
         Arguments
         ----
-        When not specified, the first argument to this method is assumed
-        to be 'image_id'. All others are ignored.
+        When not specified, the first argument to this method is assumed to be 'ids'.
+        All others are ignored.
 
         Returns
         ----
         dict
             Dictionary object containing API response.
         """
-        if args:
-            image_id = args[0]
-
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="DeleteImageDetails",
-            image_id=image_id
+            operation_id="fdrschema_entities_field_get",
+            keywords=kwargs,
+            params=handle_single_argument(args, parameters, "ids")
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
-    def image_matches_policy(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Check if an image matches a policy by specifying repository and tag.
+    def query_field_entities(self: object, parameters: dict = None, **kwargs) -> dict:
+        """Get a list of event IDs given a particular query.
 
         HTTP Method: GET
 
         Swagger URL
         ----
-        This operation does not exist in swagger.
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/field%20schema/fdrschema.queries.field.get
 
         Keyword arguments
         ----
-        repository : str (required)
-            Repository where the image resides.
-        parameters : str (JSON)
-            Full parameters payload in JSON string format. Not required if using keywords.
-        tag : str (required)
-            Tag used for the image assessed.
+        filter : str
+            FQL formatted filter to limit returned results.
+        limit : int
+            The maximum number of records to return in this response.
+            Use with the offset parameter to manage pagination of results.
+        offset : int
+            The offset to start retrieving records from.
+            Use with the limit parameter to manage pagination of results.
+        parameters : dict
+            Full parameters payload. Not required if using other keywords.
+        sort : str
+            The property to sort by. FQL syntax.
 
         This method only supports keywords for providing arguments.
 
         Returns
         ----
         dict
             Dictionary object containing API response.
         """
-        parameters["policy_type"] = "image-prevention-policy"
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="ImageMatchesPolicy",
+            operation_id="fdrschema_queries_field_get",
             keywords=kwargs,
             params=parameters
             )
 
     # This method name aligns to the operation ID in the API but
     # does not conform to snake_case / PEP8 and is defined here for
     # backwards compatibility / ease of use purposes
-    GetCredentials = get_credentials
-    GetImageAssessmentReport = get_assessment
-    DeleteImageDetails = delete_image_details
-    ImageMatchesPolicy = image_matches_policy
+    fdrschema_combined_event_get = get_event_combined
+    fdrschema_entities_event_get = get_event_entities
+    fdrschema_queries_event_get = query_event_entities
+    fdrschema_entities_field_get = get_field_entities
+    fdrschema_queries_field_get = query_field_entities
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/falconx_sandbox.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/falconx_sandbox.py`

 * *Files 13% similar despite different names*

```diff
@@ -87,14 +87,113 @@
             operation_id="GetArtifacts",
             keywords=kwargs,
             params=handle_single_argument(args, parameters, "id"),
             headers=header_payload
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
+    def get_dump_extracted_strings(self: object, *args, parameters: dict = None, **kwargs) -> object:
+        """Get extracted strings from a memory dump.
+
+        Keyword arguments:
+        id -- Extracted Strings ID. String.
+        name -- The name given to your download file. String.
+        parameters -- full parameters payload, not required if id is provided as a keyword.
+
+        Arguments: When not specified, the first argument to this method is assumed to be 'id'.
+                   All others are ignored.
+
+        Returns: gzip-compressed binary object on SUCCESS
+                 dict object containing API response on FAILURE
+
+        HTTP Method: GET
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/falconx-sandbox/GetMemoryDumpExtractedStrings
+        """
+        # Create a copy of our default header dictionary
+        header_payload = json.loads(json.dumps(self.headers))
+        # gzip is currently the only allowed option
+        header_payload['Accept-Encoding'] = 'gzip'
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="GetMemoryDumpExtractedStrings",
+            keywords=kwargs,
+            params=handle_single_argument(args, parameters, "id"),
+            headers=header_payload
+            )
+
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def get_hex_dump(self: object, *args, parameters: dict = None, **kwargs) -> object:
+        """Get hex view of a memory dump.
+
+        Keyword arguments:
+        id -- Hex Dump ID. String.
+        name -- The name given to your download file. String.
+        parameters -- full parameters payload, not required if id is provided as a keyword.
+
+        Arguments: When not specified, the first argument to this method is assumed to be 'id'.
+                   All others are ignored.
+
+        Returns: gzip-compressed binary object on SUCCESS
+                 dict object containing API response on FAILURE
+
+        HTTP Method: GET
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/falconx-sandbox/GetMemoryDumpHexDump
+        """
+        # Create a copy of our default header dictionary
+        header_payload = json.loads(json.dumps(self.headers))
+        # gzip is currently the only allowed option
+        header_payload['Accept-Encoding'] = 'gzip'
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="GetMemoryDumpHexDump",
+            keywords=kwargs,
+            params=handle_single_argument(args, parameters, "id"),
+            headers=header_payload
+            )
+
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def get_memory_dump(self: object, *args, parameters: dict = None, **kwargs) -> object:
+        """Get memory dump content as a binary.
+
+        Keyword arguments:
+        id -- Memory Dump ID. String.
+        name -- The name given to your download file. String.
+        parameters -- full parameters payload, not required if id is provided as a keyword.
+
+        Arguments: When not specified, the first argument to this method is assumed to be 'id'.
+                   All others are ignored.
+
+        Returns: gzip-compressed binary object on SUCCESS
+                 dict object containing API response on FAILURE
+
+        HTTP Method: GET
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/falconx-sandbox/GetMemoryDump
+        """
+        # Create a copy of our default header dictionary
+        header_payload = json.loads(json.dumps(self.headers))
+        # gzip is currently the only allowed option
+        header_payload['Accept-Encoding'] = 'gzip'
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="GetMemoryDump",
+            keywords=kwargs,
+            params=handle_single_argument(args, parameters, "id"),
+            headers=header_payload
+            )
+
+    @force_default(defaults=["parameters"], default_types=["dict"])
     def get_summary_reports(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Get a short summary version of a sandbox report.
 
         Keyword arguments:
         ids -- List of Summary IDs to retrieve. String or list of strings.
         parameters -- full parameters payload, not required if ids is provided as a keyword.
 
@@ -537,12 +636,15 @@
     QuerySubmissions = query_submissions
     UploadSampleV2 = upload_sample
     GetReports = get_reports
     DeleteReport = delete_report
     GetSampleV2 = get_sample
     DeleteSampleV2 = delete_sample
     QuerySampleV1 = query_sample
+    GetMemoryDumpExtractedStrings = get_dump_extracted_strings
+    GetMemoryDumpHexDump = get_hex_dump
+    GetMemoryDump = get_memory_dump
 
 
 # The legacy name for this class does not conform to PascalCase / PEP8
 # It is defined here for backwards compatibility purposes only.
 FalconX_Sandbox = FalconXSandbox  # pylint: disable=C0103
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/filevantage.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/filevantage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/firewall_management.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/firewall_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,58 +67,67 @@
 
     @force_default(defaults=["body"], default_types=["list"])
     def aggregate_events(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Aggregate events for customer.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
-                List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
 
@@ -143,58 +152,67 @@
 
     @force_default(defaults=["body"], default_types=["list"])
     def aggregate_policy_rules(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Aggregate rules within a policy for customer.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
-                List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
 
@@ -219,58 +237,67 @@
 
     @force_default(defaults=["body"], default_types=["list"])
     def aggregate_rule_groups(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Aggregate rule groups for customer.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
-                List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
 
@@ -295,58 +322,67 @@
 
     @force_default(defaults=["body"], default_types=["list"])
     def aggregate_rules(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Aggregate rules for customer.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
-                List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
 
@@ -570,50 +606,50 @@
                 {
                     "connection_types": {
                         "wired": true,
                         "wireless": {
                         "enabled": true,
                         "require_encryption": true,
                         "ssids": [
-                            "string"
+                                "string"
                             ]
                         }
                     },
                     "default_gateways": [
                         "string"
                     ],
                     "description": "string",
                     "dhcp_servers": [
-                        "string"
+                            "string"
                         ],
                     "dns_resolution_targets": {
                         "targets": [
                             {
                                 "hostname": "string",
                                 "ip_match": [
                                     "string"
                                 ]
                             }
                         ]
                     },
                     "dns_servers": [
-                        "string"
+                            "string"
                         ],
                     "enabled": true,
                     "host_addresses": [
-                        "string"
+                            "string"
                         ],
                     "https_reachable_hosts": {
                         "hostnames": [
                             "string"
                         ]
                     },
                     "icmp_request_targets": {
                         "targets": [
-                        "string"
+                            "string"
                         ]
                     },
                     "name": "string"
                 }
         clone_id -- A network location ID from which to copy rules. If this is provided then all
                     other keywords except `add_fw_rules` and `comment` are ignored. String.
         comment -- Audit log comment for this action. String.
@@ -664,14 +700,16 @@
                         "enabled": true,
                         "require_encryption": true,
                         "ssids": [
                             "string"
                             ]
                         }
                     },
+                    "created_by": "string",
+                    "created_on": "string",
                     "default_gateways": [
                         "string"
                     ],
                     "description": "string",
                     "dhcp_servers": [
                         "string"
                         ],
@@ -705,14 +743,16 @@
                     "name": "string",
                     "id": "string",
                     "modified_by": "string",
                     "modified_on": "string"
                 }
         comment -- Audit log comment for this action. String.
         connection_types -- Connections available at the location. Dictionary.
+        created_on -- Timestamp string.
+        created_by -- String.
         default_gateways -- List of available default gateways. List of strings.
         description -- Description of the location. String.
         dhcp_servers -- List of available DHCP servers. List of strings.
         dns_resolution_targets -- Dictionary containing a list of DNS resolution targets.
         dns_servers -- List of available DNS servers. List of strings.
         enabled -- Flag indicating if this location is enabled. Boolean.
         host_addresses -- List of available host addresses. List of strings.
@@ -757,14 +797,16 @@
                         "enabled": true,
                         "require_encryption": true,
                         "ssids": [
                             "string"
                             ]
                         }
                     },
+                    "created_by": "string",
+                    "created_on": "string",
                     "default_gateways": [
                         "string"
                     ],
                     "description": "string",
                     "dhcp_servers": [
                         "string"
                         ],
@@ -798,14 +840,16 @@
                     "name": "string",
                     "id": "string",
                     "modified_by": "string",
                     "modified_on": "string"
                 }
         comment -- Audit log comment for this action. String.
         connection_types -- Connections available at the location. Dictionary.
+        created_on -- Timestamp string.
+        created_by -- String.
         default_gateways -- List of available default gateways. List of strings.
         description -- Description of the location. String.
         dhcp_servers -- List of available DHCP servers. List of strings.
         dns_resolution_targets -- Dictionary containing a list of DNS resolution targets.
         dns_servers -- List of available DNS servers. List of strings.
         enabled -- Flag indicating if this location is enabled. Boolean.
         host_addresses -- List of available host addresses. List of strings.
@@ -933,26 +977,28 @@
         Keyword arguments:
         body -- Full body payload in JSON format. Not required if other keywords are provided.
                 {
                     "default_inbound": "string",
                     "default_outbound": "string",
                     "enforce": true,
                     "is_default_policy": true,
+                    "local_logging": true,
                     "platform_id": "string",
                     "policy_id": "string",
                     "rule_group_ids": [
                         "string"
                     ],
                     "test_mode": true,
                     "tracking": "string"
                 }
         default_inbound -- Default inbound. String.
         default_outbound -- Default outbound. String.
         enforce -- Flag indicating if the policy is enforced. Boolean.
         is_default_policy -- Flag indicating if the policy is the default. Boolean.
+        local_logging -- Flag indicating if local logging should be enabled. Boolean.
         platform_id -- Platform ID. (`windows`, `mac`, `linux`) String.
         policy_id -- ID of the policy to be updated. String.
         rule_group_ids -- Rule group IDs this policy applies to. String or list of strings.
         test_mode -- Flag indicating if this policy is in test mode. Boolean.
         tracking -- Tracking. String.
 
         This method only supports keywords for providing arguments.
@@ -1072,14 +1118,15 @@
         address_family -- Address type, String. Either 'IP4', 'IP6' or 'NONE'.
                           Overridden if 'rules' keyword is provided.
         body -- Full body payload in JSON format. Not required if other keywords are provided.
                 {
                     "description": "string",
                     "enabled": true,
                     "name": "string",
+                    "platform": "string",
                     "rules": [
                         {
                             "action": "string",
                             "address_family": "string",
                             "description": "string",
                             "direction": "string",
                             "enabled": true,
@@ -1113,17 +1160,14 @@
                             ],
                             "log": true,
                             "monitor": {
                                 "count": "string",
                                 "period_ms": "string"
                             },
                             "name": "string",
-                            "platform_ids": [
-                                "string"
-                            ],
                             "protocol": "string",
                             "remote_address": [
                                 {
                                     "address": "string",
                                     "netmask": 0
                                 }
                             ],
@@ -1153,16 +1197,15 @@
                          Overridden if 'rules' keyword is provided.
         local_port -- Local port range. Dictionary or list of dictionaries.
                       Overridden if 'rules' keyword is provided.
         log -- Log rule matches. Boolean. Overridden if 'rules' keyword is provided.
         name -- Rule group name. String.
         monitor -- Monitor count / period. Dictionary. Overridden if 'rules' keyword is provided.
         parameters - full parameters payload, not required if using other keywords.
-        platform_ids -- OS platform(s) covered by rule. Comma-delimited string or list of strings.
-                        Overridden if 'rules' keyword is provided.
+        platform -- OS platform covered by rule. String.
         protocol -- Integer protocol specified. Integer. Overridden if 'rules' keyword is provided.
                     (TCP = 6, UDP = 17)
         remote_address -- Remote address and netmask detail. Dictionary or list of dictionaries.
                           Overridden if 'rules' keyword is provided.
         remote_port -- Remote port range. Dictionary or list of dictionaries.
                        Overridden if 'rules' keyword is provided.
         rule_description -- Description for created rule. String.
@@ -1207,17 +1250,14 @@
                     ],
                     "log": true,
                     "monitor": {
                         "count": "string",
                         "period_ms": "string"
                     },
                     "name": "string",
-                    "platform_ids": [
-                        "string"
-                    ],
                     "protocol": "string",
                     "remote_address": [
                         {
                             "address": "string",
                             "netmask": 0
                         }
                     ],
@@ -1379,14 +1419,16 @@
                             "type": "string",
                             "value": "string",
                             "values": [
                                 "string"
                             ]
                             }
                         ],
+                        "fqdn": "string",
+                        "fqdn_enabled": true,
                         "icmp": {
                             "icmp_code": "string",
                             "icmp_type": "string"
                         },
                         "local_address": [
                             {
                             "address": "string",
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/firewall_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/firewall_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,18 +332,17 @@
         """Update Firewall Policies by specifying the ID of the policy and details to update.
 
         Keyword arguments:
         body -- full body payload, not required if keywords are used.
                 {
                 "resources": [
                     {
-                        "clone_id": "string",
+                        "id": "string",
                         "description": "string",
-                        "name": "string",
-                        "platform_name": "Windows"
+                        "name": "string"
                     }
                 ]
             }
         id -- ID of the Device Control Policy to update. String.
         description -- Device Control Policy description. String.
         name -- Device Control Policy name. String.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/host_group.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/hosts.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/hosts.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,16 +67,16 @@
                        'hide_host', 'unhide_host', 'detection_suppress', or
                        'detection_unsuppress'.
         body -- full body payload, not required if ids are provided as keyword.
                 You must use body if you are going to specify action_parameters.
                 {
                     "action_parameters": [
                         {
-                        "name": "string",
-                        "value": "string"
+                            "name": "string",
+                            "value": "string"
                         }
                     ],
                     "ids": [
                         "string"
                     ]
                 }
         ids -- AID(s) to perform actions against. String or list of strings.
@@ -125,19 +125,20 @@
                        'remove_group_member'. String.
         action_parameters -- Action parameter payload. List of dictionaries.
         body -- full body payload, not required if ids are provided as keyword.
                 You must use body if you are going to specify action_parameters.
                 {
                     "action_parameters": [
                         {
-                        "name": "string",
-                        "value": "string"
+                            "name": "string",
+                            "value": "string"
                         }
                     ]
                 }
+        disable_hostname_check -- Disable the hostname check. Boolean.
         ids -- Group ID(s) to perform actions against. String or list of strings.
         parameters - full parameters payload, not required if action_name is provide as a keyword.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/identity_protection.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/incidents.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/incidents.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,32 +113,38 @@
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
             operation_id="GetBehaviors",
             body=body
             )
 
-    @force_default(defaults=["body"], default_types=["dict"])
-    def perform_incident_action(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+    @force_default(defaults=["body", "parameters"], default_types=["dict", "dict"])
+    def perform_incident_action(self: object,
+                                body: dict = None,
+                                parameters: dict = None,
+                                **kwargs
+                                ) -> Dict[str, Union[int, dict]]:
         """Perform a set of actions on one or more incidents.
 
         Such as: adding tags or updating the incident name or description.
 
         A maximum of 5000 incidents may be updated per request.
 
         Keyword arguments:
         action_parameters -- Action specific parameters. List of dictionaries.
         add_tag -- Adds the associated value as a new tag on all the incidents of the ids list.
                    Overridden if action_parameters is specified. Multiple values may be provided.
                    String, comma delimited string, or list.
         delete_tag -- Deletes tags matching the value from all the incidents in the ids list.
                       Overridden if action_parameters is specified. Multiple values may be provided.
                       String, comma delimited string or list.
+        overwrite_detects - Overwrite related detections. Boolean.
         unassign -- Unassigns all users from all of the incidents in the ids list.
                     Overridden if action_parameters is specified. Boolean.
+        update_detects -- Update related detections. Boolean.
         update_name -- Updates the name to the parameter value of all the incidents
                        in the ids list. Overridden if action_parameters is specified. String.
         update_assigned_to_v2 -- Assigns the user matching the UUID in the parameter
                                  value to all of the incidents in the ids list. For information
                                  on getting the UUID of a user, see Find existing users.
                                  Overridden if action_parameters is specified. UUID string.
         update_description -- Updates the description to the parameter value of all the
@@ -160,14 +166,15 @@
                         }
                     ],
                     "ids": [
                         "string"
                     ]
                 }
         ids -- Incident ID(s) to perform actions against. String or list of strings.
+        parameters -- Full parameters payload, not required if using other keywords.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: POST
 
@@ -183,15 +190,17 @@
             if kwargs.get("action_parameters", None):
                 body["action_parameters"] = kwargs.get("action_parameters", None)
 
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
             operation_id="PerformIncidentAction",
-            body=body
+            body=body,
+            params=parameters,
+            keywords=kwargs
             )
 
     @force_default(defaults=["body"], default_types=["dict"])
     def get_incidents(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Get details on incidents by providing incident IDs.
 
         Keyword arguments:
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/installation_tokens.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/intel.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/ioa_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/ioc.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ioc.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,24 +63,29 @@
 
     @force_default(defaults=["body", "parameters"], default_types=["dict", "dict"])
     def indicator_aggregate(self: object, parameters: dict = None, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Get indicator aggregates as specified via json in request body.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
+                body -- full body payload, not required when using other keywords.
                 {
                     "date_ranges": [
                     {
                         "from": "string",
                         "to": "string"
                     }
                     ],
+                    "exclude": "string",
                     "field": "string",
                     "filter": "string",
+                    "from": 0,
+                    "include": "string",
                     "interval": "string",
+                    "max_doc_count": 0,
                     "min_doc_count": 0,
                     "missing": "string",
                     "name": "string",
                     "q": "string",
                     "ranges": [
                     {
                         "From": 0,
@@ -91,21 +96,29 @@
                     "sort": "string",
                     "sub_aggregates": [
                         null
                     ],
                     "time_zone": "string",
                     "type": "string"
                 }
-        date_ranges -- List of dictionaries.
-        field -- String.
-        filter -- FQL syntax. String.
-        from_parent -- The filter for returning either only indicators for the
-                       requested customer or its MSSP parents. Boolean.
+
+        date_ranges -- If peforming a date range query specify the from and to date ranges.
+                       These can be in common date formats like 2019-07-18 or now.
+                       List of dictionaries.
+        exclude -- Fields to exclude. String.
+        field -- Term you want to aggregate on. If doing a date_range query,
+                 this is the date field you want to apply the date ranges to. String.
+        filter -- Optional filter criteria in the form of an FQL query.
+                  For more information about FQL queries, see our FQL documentation in Falcon.
+                  String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
         name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
         size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
@@ -212,23 +225,25 @@
     @force_default(defaults=["body"], default_types=["dict"])
     def get_indicators_report(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Launch an indicators report creation job.
 
         Keyword arguments:
         body -- full parameters payload, not required if using other keywords.
                 {
+                    "from_parent": true,
                     "report_format": "string",
                     "search": {
                         "filter": "string",
                         "query": "string",
                         "sort": "string"
                     }
                 }
         filter -- FQL formatted string specifying the search filter.
                   Overridden if 'search' keyword is provided.
+        from_parent -- Flag indicating if this indicator is defined in the parent. Boolean.
         query -- FQL formatted string specifying the search query.
                  Overridden if 'search' keyword is provided.
         report_format -- Format of the report. String.
         search -- Search parameters. Strings are in FQL format. Dictionary.
                   {
                       "filter": "string",
                       "query": "string",
@@ -404,14 +419,15 @@
                 {
                     "bulk_update": {
                         "action": "string",
                         "applied_globally": true,
                         "description": "string",
                         "expiration": "2021-10-22T11:03:16.123Z",
                         "filter": "string",
+                        "from_parent": true,
                         "host_groups": [
                             "string"
                         ],
                         "mobile_action": "string",
                         "platforms": [
                             "string"
                         ],
@@ -448,14 +464,15 @@
                     ]
                 }
         bulk_update -- Dictionary representing the indicator values to update in bulk.
         comment -- Audit log comment for the update. String.
         description -- Description for the IOC. String.
         expiration -- UTC formatted date string. String.
         filename -- Filename to use in the metadata dictionary. String.
+        from_parent -- Flag indicating if this indicator originates from the parent. Boolean.
         host_groups -- List of host groups to apply this IOC to. List of strings.
         id -- ID of the indicator to be updated. At least one ID must be specified using this
               keyword, or as part of the indicators list using the indicators keyword.
         indicators -- List of indicators to update. List of dictionaries.
         ignore_warnings -- Set to true to ignore warnings and add all IOCs. Boolean. Default: False
         metadata -- Dictionary containing the filename for the IOC.
                     Not required if filename is used.
@@ -526,14 +543,16 @@
         Keyword arguments:
         after -- A pagination token used with the limit parameter to manage pagination of results.
                  On your first request, don't provide an `after` token. On subsequent requests,
                  provide the `after` token from the previous response to continue from that place
                  in the results. To access more than 10k indicators, use the `after` parameter
                  instead of `offset`.
         filter -- The filter expression that should be used to limit the results. FQL syntax.
+        from_parent -- The filter for returning either only indicators for the request customer
+                       or its MSSP parents. String.
         limit -- The maximum records to return. [1-500]. Defaults to 100.
                  Use with the offset parameter to manage pagination of results.
         offset -- The offset to start retrieving records from.
                   Offset and After params are mutually exclusive.
                   If none provided then scrolling will be used by default.
                   To access more than 10K IOCs, use the `after` parameter instead of `offset`.
                   Use with the limit parameter to manage pagination of results.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/iocs.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/kubernetes_protection.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/response_policies.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""CrowdStrike Falcon Kubernetes Protection API interface class.
+"""CrowdStrike Falcon Real Time Response Policies API interface class.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -33,437 +33,427 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 from typing import Dict, Union
 from ._util import process_service_request, force_default, handle_single_argument
+from ._payload import generic_payload_list, response_policy_payload
 from ._service_class import ServiceClass
-from ._endpoint._kubernetes_protection import _kubernetes_protection_endpoints as Endpoints
+from ._endpoint._response_policies import _response_policies_endpoints as Endpoints
 
 
-class KubernetesProtection(ServiceClass):
+class ResponsePolicies(ServiceClass):
     """The only requirement to instantiate an instance of this class is one of the following.
 
     - a valid client_id and client_secret provided as keywords.
     - a credential dictionary with client_id and client_secret containing valid API credentials
       {
           "client_id": "CLIENT_ID_HERE",
           "client_secret": "CLIENT_SECRET_HERE"
       }
     - a previously-authenticated instance of the authentication service class (oauth2.py)
-    - a valid token provided by the authentication service class (OAuth2.token())
+    - a valid token provided by the authentication service class (oauth2.py)
     """
 
     @force_default(defaults=["parameters"], default_types=["dict"])
-    def get_aws_accounts(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Provide a list of AWS accounts.
+    def query_combined_policy_members(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Search for members of a Response policy by providing an FQL filter and paging details.
+
+        Returns a set of host details which match the filter criteria.
 
         Keyword arguments:
-        ids -- AWS Account IDs. String or list of strings.
-        limit -- The maximum number of records to return in this response. [Integer, 1-500]
+        id -- The ID of the Response Policy to search for members of
+        filter -- The filter expression that should be used to limit the results. FQL syntax.
+        limit -- The maximum number of records to return in this response. [Integer, 1-5000]
                  Use with the offset parameter to manage pagination of results.
-        offset -- The offset to start retrieving records from. String.
+        offset -- The offset to start retrieving records from. Integer.
                   Use with the limit parameter to manage pagination of results.
         parameters - full parameters payload, not required if using other keywords.
-        status -- Filter by account status. String.
+        sort -- The property to sort by. FQL syntax.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/GetAWSAccountsMixin0
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/queryCombinedRTResponsePolicyMembers
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="GetAWSAccountsMixin0",
+            operation_id="queryCombinedRTResponsePolicyMembers",
             keywords=kwargs,
             params=parameters
             )
 
-    @force_default(defaults=["body"], default_types=["dict"])
-    def create_aws_account(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Create a new AWS customer account in our system and generates the installation script.
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def query_combined_policies(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Search for Response Policies by providing an FQL filter and paging details.
+
+        Returns a set of Response Policies which match the filter criteria.
 
         Keyword arguments:
-        body -- full body payload, not required if using other keywords.
-                {
-                    "resources": [
-                        {
-                            "account_id": "string",
-                            "region": "string"
-                        }
-                    ]
-                }
-        account_id -- Account ID. String.
-        region -- Region. String.
+        filter -- The filter expression that should be used to limit the results. FQL syntax.
+        limit -- The maximum number of records to return in this response. [Integer, 1-5000]
+                 Use with the offset parameter to manage pagination of results.
+        offset -- The offset to start retrieving records from. Integer.
+                  Use with the limit parameter to manage pagination of results.
+        parameters - full parameters payload, not required if using other keywords.
+        sort -- The property to sort by. FQL syntax.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
-        HTTP Method: POST
+        HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/CreateAWSAccount
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/queryCombinedRTResponsePolicies
         """
-        if not body:
-            item = {}
-            if kwargs.get("account_id", None):
-                item["account_id"] = kwargs.get("account_id", None)
-            if kwargs.get("region", None):
-                item["region"] = kwargs.get("region", None)
-
-            body["resources"] = [item]
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="CreateAWSAccount",
-            body=body
+            operation_id="queryCombinedRTResponsePolicies",
+            keywords=kwargs,
+            params=parameters
             )
 
-    @force_default(defaults=["parameters"], default_types=["dict"])
-    def delete_aws_accounts(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Delete AWS accounts.
-
-        Keyword arguments:
-        ids -- ID(s) of AWS accounts to delete. String or list of strings.
-        parameters -- full parameters payload, not required if ids is provided as a keyword.
+    @force_default(defaults=["parameters", "body"], default_types=["dict", "dict"])
+    def perform_policies_action(self: object,
+                                body: dict = None,
+                                parameters: dict = None,
+                                **kwargs
+                                ) -> Dict[str, Union[int, dict]]:
+        """Perform the specified action on the Response Policies specified in the request.
+
+        Keyword arguments:
+        action_name -- action to perform: 'add-host-group', 'add-rule-group', 'disable',
+                       'enable', 'remove-host-group', or 'remove-rule-group'.
+        action_parameters -- Action specific parameter options. List of dictionaries.
+                             {
+                                 "name": "string",
+                                 "value": "string"
+                             }
+        body -- full body payload, not required if keywords are used.
+                {
+                    "action_parameters": [
+                        {
+                            "name": "group_id",
+                            "value": "string"
+                        }
+                    ],
+                    "ids": [
+                        "string"
+                    ]
+                }
+        group_id -- Host Group ID to apply the policy to. String.
+                    Overridden if action_parameters is provided.
+        ids -- Response policy ID(s) to perform actions against. String or list of strings.
+        parameters - full parameters payload, not required if action_name is provide as a keyword.
 
-        Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
-                   All others are ignored.
+        This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
-        HTTP Method: DELETE
+        HTTP Method: POST
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/DeleteAWSAccountsMixin0
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/performRTResponsePoliciesAction
         """
+        if not body:
+            body = generic_payload_list(submitted_keywords=kwargs, payload_value="ids")
+            if kwargs.get("group_id", None):
+                body["action_parameters"] = [{
+                    "name": "group_id",
+                    "value": kwargs.get("group_id", None)
+                }]
+            # Passing an action_parameters list will override the group_id keyword
+            if kwargs.get("action_parameters", None):
+                body["action_parameters"] = kwargs.get("action_parameters", None)
+
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="DeleteAWSAccountsMixin0",
+            operation_id="performRTResponsePoliciesAction",
             keywords=kwargs,
-            params=handle_single_argument(args, parameters, "ids")
+            params=parameters,
+            body=body
             )
 
-    @force_default(defaults=["parameters"], default_types=["dict"])
-    def update_aws_account(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Update the AWS account per the query parameters provided.
+    @force_default(defaults=["body"], default_types=["dict"])
+    def set_policies_precedence(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Set the precedence of Response Policies based on the order of IDs in the request.
+
+        The first ID specified will have the highest precedence and the last ID specified will
+        have the lowest. You must specify all non-Default Policies for a platform when updating
+        precedence.
 
         Keyword arguments:
-        ids -- ID(s) of AWS accounts to update. String or list of strings.
-        parameters -- full parameters payload, not required if ids is provided as a keyword.
-        region -- Default region for Account Automation.
+        body -- full body payload, not required if keywords are used.
+                {
+                    "ids": [
+                        "string"
+                    ],
+                    "platform_name": "string"
+                }
+        ids -- Prevention policy ID(s) to perform actions against. String or list of strings.
+        platform_name -- OS platform name. (Linux, Mac, Windows)
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
-        HTTP Method: PATCH
+        HTTP Method: POST
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/UpdateAWSAccount
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/setRTResponsePoliciesPrecedence
         """
+        if not body:
+            body = generic_payload_list(submitted_keywords=kwargs, payload_value="ids")
+            if kwargs.get("platform_name", None):
+                body["platform_name"] = kwargs.get("platform_name", None)
+
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="UpdateAWSAccount",
-            keywords=kwargs,
-            params=parameters
+            operation_id="setRTResponsePoliciesPrecedence",
+            body=body
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
-    def list_azure_accounts(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Provide a list of registered Azure subscriptions.
+    def get_policies(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Retrieve a set of Response Policies by specifying their IDs.
 
         Keyword arguments:
-        ids -- Azure tenant IDs. String or list of strings.
-        is_horizon_acct -- Filter by whether an account originates from Horizon. Boolean.
-        subscription_id -- Azure subscription IDs. String or list of strings.
-        limit -- The maximum number of records to return in this response. [Integer, 1-500]
-                 Use with the offset parameter to manage pagination of results.
-        offset -- The offset to start retrieving records from. Integer.
-                  Use with the limit parameter to manage pagination of results.
-        parameters - full parameters payload, not required if using other keywords.
-        status -- Filter by account status. (`operational` or `provisional`) String.
+        ids -- List of Response Policy IDs to retrieve. String or list of strings.
+        parameters -- full parameters payload, not required if ids is provided as a keyword.
 
-        This method only supports keywords for providing arguments.
+        Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
+                   All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/ListAzureAccounts
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/getRTResponsePolicies
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="ListAzureAccounts",
+            operation_id="getRTResponsePolicies",
             keywords=kwargs,
-            params=parameters
+            params=handle_single_argument(args, parameters, "ids")
             )
 
     @force_default(defaults=["body"], default_types=["dict"])
-    def create_azure_subscription(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Create a new Azure subscription.
+    def create_policies(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Create Response Policies by specifying details about the policy to create.
 
         Keyword arguments:
-        body -- full body payload, not required if using other keywords.
+        body -- full body payload, not required if keywords are used.
                 {
                     "resources": [
                         {
-                            "subscription_id": "string",
-                            "tenant_id": "string"
+                            "clone_id": "string",
+                            "description": "string",
+                            "name": "string",
+                            "platform_name": "Windows",
+                            "settings": [
+                                {
+                                    "id": "string",
+                                    "value": {}
+                                }
+                            ]
                         }
                     ]
                 }
-        subscription_id -- Azure subscription ID. String.
-        tenant_id -- Tenant ID. String.
+        clone_id -- Response Policy ID to clone. String.
+        description -- Response Policy description. String.
+        name -- Response Policy name. String.
+        platform_name -- Name of the operating system platform. String.
+        settings -- Response policy specific settings. List of dictionaries.
+                    {
+                        "id": "string",
+                        "value": {}
+                    }
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: POST
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/CreateAzureSubscription
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/createRTResponsePolicies
         """
         if not body:
-            item = {}
-            if kwargs.get("subscription_id", None):
-                item["subscription_id"] = kwargs.get("subscription_id", None)
-            if kwargs.get("tenant_id", None):
-                item["tenant_id"] = kwargs.get("tenant_id", None)
+            body = response_policy_payload(passed_keywords=kwargs)
 
-            body["resources"] = [item]
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="CreateAzureSubscription",
+            operation_id="createRTResponsePolicies",
             body=body
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
-    def delete_azure_subscription(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Delete an Azure subscription.
+    def delete_policies(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Delete a set of Response Policies by specifying their IDs.
 
         Keyword arguments:
-        ids -- Azure subscription IDs. String or list of strings.
-        parameters - full parameters payload, not required if using other keywords.
+        ids -- List of Response Policy IDs to delete. String or list of strings.
+        parameters -- full parameters payload, not required if ids is provided as a keyword.
 
-        Arguments: When not specified, the first argument to this method is assumed to be
-                   'ids'. All others are ignored.
+        Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
+                   All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: DELETE
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/DeleteAzureSubscription
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/deleteRTResponsePolicies
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="DeleteAzureSubscription",
+            operation_id="deleteRTResponsePolicies",
             keywords=kwargs,
             params=handle_single_argument(args, parameters, "ids")
             )
 
-    @force_default(defaults=["parameters"], default_types=["dict"])
-    def get_locations(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Provide the cloud locations acknowledged by the Kubernetes Protection service.
-
-        Keyword arguments:
-        clouds -- Cloud provider. String or list of strings.
-        parameters - full parameters payload, not required if using other keywords.
-
-        Arguments: When not specified, the first argument to this method is assumed to be 'clouds'.
-                   All others are ignored.
-
-        Returns: dict object containing API response.
-
-        HTTP Method: GET
-
-        Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/GetLocations
-        """
-        return process_service_request(
-            calling_object=self,
-            endpoints=Endpoints,
-            operation_id="GetLocations",
-            keywords=kwargs,
-            params=handle_single_argument(args, parameters, "clouds")
-            )
-
-    @force_default(defaults=["parameters"], default_types=["dict"])
-    def get_helm_values_yaml(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Provide a sample Helm values.yaml file to install alongside the agent Helm chart.
-
-        Keyword arguments:
-        cluster_name -- Cloud provider. String.
-        parameters - full parameters payload, not required if using other keywords.
-
-        Arguments: When not specified, the first argument to this method is assumed to be
-                   'cluster_name'. All others are ignored.
-
-        Returns: dict object containing API response.
-
-        HTTP Method: GET
-
-        Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/GetHelmValuesYaml
-        """
-        return process_service_request(
-            calling_object=self,
-            endpoints=Endpoints,
-            operation_id="GetHelmValuesYaml",
-            keywords=kwargs,
-            params=handle_single_argument(args, parameters, "cluster_name")
-            )
-
     @force_default(defaults=["body"], default_types=["dict"])
-    def regenerate(self: object, body: dict = None) -> Dict[str, Union[int, dict]]:
-        """Regenerate API key for docker registry integrations.
+    def update_policies(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Update Response Policies by specifying the ID of the policy and details to update.
 
         Keyword arguments:
-        body -- Body payload is accepted but is not used.
+        body -- full body payload, not required if keywords are used.
+                {
+                    "resources": [
+                        {
+                            "description": "string",
+                            "id": "string",
+                            "name": "string",
+                            "settings": [
+                                {
+                                    "id": "string",
+                                    "value": {}
+                                }
+                            ]
+                        }
+                    ]
+                }
+        description -- Response Policy description. String.
+        id -- Response Policy ID to update. String.
+        name -- Response Policy name. String.
+        settings -- Response policy specific settings. List of dictionaries.
+                    {
+                        "id": "string",
+                        "value": "string"
+                    }
 
-        This method has no default argument or keywords.
+        This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
-        HTTP Method: POST
+        HTTP Method: PATCH
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/RegenerateAPIKey
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/updateRTResponsePolicies
         """
+        if not body:
+            body = response_policy_payload(passed_keywords=kwargs)
+
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="RegenerateAPIKey",
+            operation_id="updateRTResponsePolicies",
             body=body
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
-    def get_clusters(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Provide the clusters acknowledged by the Kubernetes Protection service.
+    def query_policy_members(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Search for members of a Response policy by providing an FQL filter and paging details.
+
+        Returns a set of Agent IDs which match the filter criteria.
 
         Keyword arguments:
-        account_ids -- Cluster Account IDs. For EKS, this would be the AWS Account ID.
-                       String or list of strings.
-        cluster_names -- Cluster name. For EKS it will be cluster ARN. String or list of strings.
-        cluster_service -- Cluster Service. Available values: `eks`
-        limit -- The maximum number of records to return in this response. [Integer, 1-500]
+        id -- The ID of the Response Policy to search for members of
+        filter -- The filter expression that should be used to limit the results. FQL syntax.
+        limit -- The maximum number of records to return in this response. [Integer, 1-5000]
                  Use with the offset parameter to manage pagination of results.
-        locations -- Cloud location. String or list of strings.
-        offset -- The offset to start retrieving records from. String.
+        offset -- The offset to start retrieving records from. Integer.
                   Use with the limit parameter to manage pagination of results.
         parameters - full parameters payload, not required if using other keywords.
+        sort -- The property to sort by. FQL syntax.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/GetClusters
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/queryRTResponsePolicyMembers
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="GetClusters",
+            operation_id="queryRTResponsePolicyMembers",
             keywords=kwargs,
             params=parameters
             )
 
-    @force_default(defaults=["parameters", "body"], default_types=["dict", "dict"])
-    def trigger_scan(self: object,
-                     *args,
-                     body: dict = None,
-                     parameters: dict = None,
-                     **kwargs
-                     ) -> Dict[str, Union[int, dict]]:
-        """Trigger a dry run or a full scan of a customer's kubernetes footprint.
-
-        Keyword arguments:
-        body -- Body payload is accepted but is not used.
-        scan_type -- Type of scan to perform. String.  Default value: `dry-run`.
-                     Available Values: `cluster-refresh`, `dry-run`, or `full`.
-        parameters - full parameters payload, not required if using other keywords.
-
-        Arguments: When not specified, the first argument to this method is assumed to be
-                   'scan_type'. All others are ignored.
-
-        Returns: dict object containing API response.
-
-        HTTP Method: POST
-
-        Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/TriggerScan
-        """
-        return process_service_request(
-            calling_object=self,
-            endpoints=Endpoints,
-            operation_id="TriggerScan",
-            keywords=kwargs,
-            params=handle_single_argument(args, parameters, "scan_type"),
-            body=body
-            )
-
     @force_default(defaults=["parameters"], default_types=["dict"])
-    def update_azure_service_principal(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Add the client ID for a given tenant ID to the subscription.
+    def query_policies(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Search for Response Policies by providing an FQL filter with sort and/or paging details.
+
+        This returns a set of Response Policy IDs that match the given criteria.
 
         Keyword arguments:
-        id -- Azure tentant ID. String. Required.
-        client_id -- Azure client ID. String. Required.
+        filter -- The filter expression that should be used to limit the results. FQL syntax.
+        limit -- The maximum number of records to return in this response. [Integer, 1-5000]
+                 Use with the offset parameter to manage pagination of results.
+        offset -- The offset to start retrieving records from. Integer.
+                  Use with the limit parameter to manage pagination of results.
         parameters - full parameters payload, not required if using other keywords.
+        sort -- The property to sort by. FQL syntax.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
-        HTTP Method: PATCH
+        HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/kubernetes-protection/PatchAzureServicePrincipal
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/queryRTResponsePolicies
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="PatchAzureServicePrincipal",
+            operation_id="queryRTResponsePolicies",
             keywords=kwargs,
-            params=handle_single_argument(args, parameters, "ids")
+            params=parameters
             )
 
     # These method names align to the operation IDs in the API but
     # do not conform to snake_case / PEP8 and are defined here for
     # backwards compatibility / ease of use purposes
-    GetAWSAccountsMixin0 = get_aws_accounts
-    CreateAWSAccount = create_aws_account
-    DeleteAWSAccountsMixin0 = delete_aws_accounts
-    UpdateAWSAccount = update_aws_account
-    ListAzureAccounts = list_azure_accounts
-    CreateAzureSubscription = create_azure_subscription
-    DeleteAzureSubscription = delete_azure_subscription
-    GetLocations = get_locations
-    GetHelmValuesYaml = get_helm_values_yaml
-    regenerate_api_key = regenerate
-    RegenerateAPIKey = regenerate
-    GetClusters = get_clusters
-    TriggerScan = trigger_scan
-    PatchAzureServicePrincipal = update_azure_service_principal
-    patch_azure_service_principal = update_azure_service_principal
+    queryCombinedRTResponsePolicyMembers = query_combined_policy_members
+    queryCombinedRTResponsePolicies = query_combined_policies
+    performRTResponsePoliciesAction = perform_policies_action
+    setRTResponsePoliciesPrecedence = set_policies_precedence
+    getRTResponsePolicies = get_policies
+    createRTResponsePolicies = create_policies
+    deleteRTResponsePolicies = delete_policies
+    updateRTResponsePolicies = update_policies
+    queryRTResponsePolicyMembers = query_policy_members
+    queryRTResponsePolicies = query_policies
 
 
 # The legacy name for this class does not conform to PascalCase / PEP8
 # It is defined here for backwards compatibility purposes only.
-Kubernetes_Protection = KubernetesProtection  # pylint: disable=C0103
+Response_Policies = ResponsePolicies  # pylint: disable=C0103
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/malquery.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/malquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,16 +88,16 @@
                         "filter_meta": [
                             "string"
                         ],
                         "limit": 0
                     },
                     "patterns": [
                         {
-                        "type": "string",
-                        "value": "string"
+                            "type": "string",
+                            "value": "string"
                         }
                     ]
                 }
         filter_meta -- List of strings.
         limit -- Integer representing maximum number of matches to return.
         patterns -- List of dictionaries containing patterns to match.
                     {
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/message_center.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/message_center.py`

 * *Files 7% similar despite different names*

```diff
@@ -387,14 +387,70 @@
             endpoints=Endpoints,
             operation_id="UpdateCase",
             keywords=kwargs,
             body=body
             )
 
     @force_default(defaults=["body"], default_types=["dict"])
+    def create_case_v2(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Create a new case.
+
+        Keyword arguments:
+        body -- full body payload, not required when using other keywords.
+                NOTICE: This particular body payload contains a field named `body`, which
+                        impacts body payload abstraction functionality. This field can be
+                        set using the keyword `content` if you do not wish to specify a
+                        full body payload using the `body` keyword.
+                {
+                    "body": "string",
+                    "detections": [
+                        {
+                            "id": "string",
+                            "product": "string",
+                            "url": "string"
+                        }
+                    ],
+                    "incidents": [
+                        {
+                            "id": "string",
+                            "url": "string"
+                        }
+                    ],
+                    "title": "string",
+                    "type": "string",
+                    "user_uuid": "string"
+                }
+        content -- Case content. Used for the `body` field within the body payload. String.
+        detections -- List of detections to attach to the case. List of dictionaries.
+        incidents -- List of incidents to attach to the case. List of dictionaries.
+        title -- Case title. String.
+        type -- Case type. String. The keyword `case_type` can also be used to specify this value.
+        user_uuid -- UUID of the user related to the case. String.
+
+        This method only supports keywords for providing arguments.
+
+        Returns: dict object containing API response.
+
+        HTTP Method: POST
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/message-center/CreateCaseV2
+        """
+        if not body:
+            body = case_payload(passed_keywords=kwargs)
+
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="CreateCaseV2",
+            keywords=kwargs,
+            body=body
+            )
+
+    @force_default(defaults=["body"], default_types=["dict"])
     def get_cases(self: object, *args, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve message center cases.
 
         Keyword arguments:
         body -- full body payload, not required if ids is provided as a keyword.
                 {
                     "ids": [
@@ -504,14 +560,15 @@
     CaseAddActivity = add_case_activity
     case_add_activity = add_case_activity
     CaseDownloadAttachment = download_case_attachment
     case_download_attachment = download_case_attachment
     CaseAddAttachment = add_case_attachment
     case_add_attachment = add_case_attachment
     CreateCase = create_case
+    CreateCaseV2 = create_case_v2
     UpdateCase = update_case
     GetCaseEntitiesByIDs = get_cases
     get_case_entities_by_ids = get_cases
     QueryActivityByCaseID = query_activities
     query_activity_by_case_id = query_activities
     QueryCasesIdsByFilter = query_cases
     QueryCaseIdsByFilter = query_cases
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/ml_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ml_exclusions.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         """Create the ML exclusions.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 {
                     "comment": "string",
                     "excluded_from": [
-                        null
+                        "string"
                     ],
                     "groups": [
                         "string"
                     ],
                     "value": "string"
                 }
         comment -- String comment describing why the exclusion is entered.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/mobile_enrollment.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/mssp.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/mssp.py`

 * *Files 0% similar despite different names*

```diff
@@ -868,14 +868,15 @@
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def query_children(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Query for customers linked as children.
 
         Keyword arguments:
+        filter -- FQL formatted string used to limit results. String. Supported filter: cid
         limit -- The maximum number of records to return in this response. [Integer, 1-1000]
                  Use with the offset parameter to manage pagination of results. Default: 10
         offset -- The offset to start retrieving records from. String.
                   Use with the limit parameter to manage pagination of results.
         parameters - full parameters payload, not required if using other keywords.
         sort -- The property to sort by. FQL syntax. (Ex: `last_modified_timestamp|desc`)
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/oauth2.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,40 +165,42 @@
         except CannotRevokeToken as unable_to_revoke:
             if self.log:
                 self.log.warning("Token revocation operation failed.")
             returned = unable_to_revoke.result
 
         return returned
 
-    def revoke(self, token: str, alter_state: bool = False) -> Dict[str, Union[int, dict]]:
+    def revoke(self, token: str, alter_state: bool = False, client_id: str = None) -> Dict[str, Union[int, dict]]:
         """Revoke the specified authorization token.
 
         HTTP Method: POST
 
         Swagger URL
         ----
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/oauth2/oauth2RevokeToken
 
         Keyword arguments
         ----
+        client_id : str
+            Client ID of the token to be revoked.
         token : str
             Token string to be revoked.
         alter_state : bool
             Flag indicating if the underlying authentication state is changed by this request.
 
         Arguments
         ----
         When not specified as a keyword, token is assumed as the only accepted argument.
 
         Returns
         ----
         dict
             Dictionary containing API response.
         """
-        return self._logout_handler(token, not alter_state)
+        return self._logout_handler(token, not alter_state, client_id)
 
     def token(self, alter_state: bool = False) -> Dict[str, Union[int, dict]]:
         """Generate an authorization token.
 
         HTTP Method: POST
 
         Swagger URL
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/ods.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ods.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,30 +55,117 @@
           "client_secret": "CLIENT_SECRET_HERE"
       }
     - a previously-authenticated instance of the authentication service class (oauth2.py)
     - a valid token provided by the authentication service class (oauth2.py)
     """
 
     @force_default(defaults=["body"], default_types=["list"])
+    def aggregate_scan_hosts(self: object, body: list = None, **kwargs) -> dict:
+        """Get aggregates on ODS scan-hosts data.
+
+        Keyword arguments:
+        body -- full body payload, not required when using other keywords.
+                [
+                    {
+                        "date_ranges": [
+                        {
+                            "from": "string",
+                            "to": "string"
+                        }
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
+                        {
+                            "From": 0,
+                            "To": 0
+                        }
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
+        date_ranges -- If peforming a date range query specify the from and to date ranges.
+                       These can be in common date formats like 2019-07-18 or now.
+                       List of dictionaries.
+        exclude -- Fields to exclude. String.
+        field -- Term you want to aggregate on. If doing a date_range query,
+                 this is the date field you want to apply the date ranges to. String.
+        filter -- Optional filter criteria in the form of an FQL query.
+                  For more information about FQL queries, see our FQL documentation in Falcon.
+                  String.
+        from -- Integer.
+        include -- Fields to include. String.
+        interval -- String.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
+        missing -- String.
+        name -- Scan name. String.
+        q -- FQL syntax. String.
+        ranges -- List of dictionaries.
+        size -- Integer.
+        sort -- FQL syntax. String.
+        sub_aggregates -- List of strings.
+        time_zone -- String.
+        type -- String.
+
+        This method only supports keywords for providing arguments.
+
+        Returns: dict object containing API response.
+
+        HTTP Method: POST
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/ods/aggregate-query-scan-host-metadata
+        """
+        if not body:
+            body = [aggregate_payload(submitted_keywords=kwargs)]
+
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="aggregate_query_scan_host_metadata",
+            body=body
+            )
+
+    @force_default(defaults=["body"], default_types=["list"])
     def aggregate_scans(self: object, body: list = None, **kwargs) -> dict:
         """Get aggregates on ODS scan data.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 [
                     {
                         "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
                         ],
+                        "exclude": "string",
                         "field": "string",
                         "filter": "string",
+                        "from": 0,
+                        "include": "string",
                         "interval": "string",
+                        "max_doc_count": 0,
                         "min_doc_count": 0,
                         "missing": "string",
                         "name": "string",
                         "q": "string",
                         "ranges": [
                         {
                             "From": 0,
@@ -90,19 +177,28 @@
                         "sub_aggregates": [
                             null
                         ],
                         "time_zone": "string",
                         "type": "string"
                     }
                 ]
-        date_ranges -- List of dictionaries.
-        field -- String.
-        filter -- FQL syntax. String.
+        date_ranges -- If peforming a date range query specify the from and to date ranges.
+                       These can be in common date formats like 2019-07-18 or now.
+                       List of dictionaries.
+        exclude -- Fields to exclude. String.
+        field -- Term you want to aggregate on. If doing a date_range query,
+                 this is the date field you want to apply the date ranges to. String.
+        filter -- Optional filter criteria in the form of an FQL query.
+                  For more information about FQL queries, see our FQL documentation in Falcon.
+                  String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
         name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
         size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
@@ -138,17 +234,21 @@
                     {
                         "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
                         ],
+                        "exclude": "string",
                         "field": "string",
                         "filter": "string",
+                        "from": 0,
+                        "include": "string",
                         "interval": "string",
+                        "max_doc_count": 0,
                         "min_doc_count": 0,
                         "missing": "string",
                         "name": "string",
                         "q": "string",
                         "ranges": [
                         {
                             "From": 0,
@@ -160,19 +260,28 @@
                         "sub_aggregates": [
                             null
                         ],
                         "time_zone": "string",
                         "type": "string"
                     }
                 ]
-        date_ranges -- List of dictionaries.
-        field -- String.
-        filter -- FQL syntax. String.
+        date_ranges -- If peforming a date range query specify the from and to date ranges.
+                       These can be in common date formats like 2019-07-18 or now.
+                       List of dictionaries.
+        exclude -- Fields to exclude. String.
+        field -- Term you want to aggregate on. If doing a date_range query,
+                 this is the date field you want to apply the date ranges to. String.
+        filter -- Optional filter criteria in the form of an FQL query.
+                  For more information about FQL queries, see our FQL documentation in Falcon.
+                  String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
         name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
         size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
@@ -226,14 +335,19 @@
 
     @force_default(defaults=["body"], default_types=["dict"])
     def cancel_scans(self: object, *args, body: dict = None, **kwargs) -> dict:
         """Cancel ODS scans for the given scan IDs.
 
         Keyword arguments:
         body -- full body payload, not required if ids is provided as a keyword.
+                {
+                    "ids": [
+                        "string"
+                    ]
+                }
         ids -- ID(s) of the scans to cancel. String or list of strings.
 
         Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
                    All others are ignored.
 
         Returns: dict object containing API response.
 
@@ -473,14 +587,17 @@
                     "max_duration": 0,
                     "max_file_size": 0,
                     "pause_duration": 0,
                     "quarantine": true,
                     "scan_exclusions": [
                         "string"
                     ],
+                    "scan_inclusions": [
+                        "string"
+                    ],
                     "schedule": {
                         "ignored_by_channelfile": true,
                         "interval": 0,
                         "start_timestamp": "string"
                     },
                     "sensor_ml_level_detection": 0,
                     "sensor_ml_level_prevention": 0
@@ -498,14 +615,15 @@
         interval -- Scan schedule interval in seconds. Integer. Overrides the value specified in
                     the schedule dictionary.
         max_duration -- Maximum duration in seconds for the scan. Integer.
         max_file_size -- Maximum file size for files scanned. Integer.
         pause_duration -- Time in seconds to pause during the scan. Integer.
         quarantine -- Quarantine malicious files identified by the scan. Boolean.
         scan_exclusions -- List of file path globs to exclude from the scan. List of strings.
+        scan_inclusions -- List of file path globs to include the scan. List of strings.
         schedule -- Details related to the scan schedule. Dictionary.
                     {
                         "ignored_by_channelfile": true,
                         "interval": 0,
                         "start_timestamp": "string"
                     }
         start_timestamp -- Starting timestamp for the scan. String. Overrides the value specified
@@ -733,7 +851,8 @@
             )
 
     get_malicious_files_by_ids = get_malicious_files
     get_scan_host_metadata_by_ids = get_scan_hosts
     get_scans_by_scan_ids = get_scans
     get_scheduled_scans_by_scan_ids = get_scheduled_scans
     query_scan_host_metadata = query_scan_hosts
+    aggregate_query_scan_host_metadata = aggregate_scan_hosts
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/overwatch_dashboard.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/overwatch_dashboard.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,58 +87,67 @@
 
     @force_default(defaults=["body"], default_types=["list"])
     def aggregates_events_collections(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Get OverWatch detection event collection info by providing an aggregate query.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
-                List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
 
@@ -163,58 +172,67 @@
 
     @force_default(defaults=["body"], default_types=["list"])
     def aggregates_events(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Get aggregate OverWatch detection event info by providing an aggregate query.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
-                List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/prevention_policy.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/quarantine.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/quarantine.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,49 +84,60 @@
 
     @force_default(defaults=["body"], default_types=["dict"])
     def get_aggregate_files(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Get quarantine file aggregates as specified via json in request body.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
-                [
+                {
+                    "date_ranges": [
                     {
-                        "date_ranges": [
-                        {
-                            "from": "string",
-                            "to": "string"
-                        }
-                        ],
-                        "field": "string",
-                        "filter": "string",
-                        "interval": "string",
-                        "min_doc_count": 0,
-                        "missing": "string",
-                        "name": "string",
-                        "q": "string",
-                        "ranges": [
-                        {
-                            "From": 0,
-                            "To": 0
-                        }
-                        ],
-                        "size": 0,
-                        "sort": "string",
-                        "sub_aggregates": [
-                        null
-                        ],
-                        "time_zone": "string",
-                        "type": "string"
+                        "from": "string",
+                        "to": "string"
+                    }
+                    ],
+                    "exclude": "string",
+                    "field": "string",
+                    "filter": "string",
+                    "from": 0,
+                    "include": "string",
+                    "interval": "string",
+                    "max_doc_count": 0,
+                    "min_doc_count": 0,
+                    "missing": "string",
+                    "name": "string",
+                    "q": "string",
+                    "ranges": [
+                    {
+                        "From": 0,
+                        "To": 0
                     }
-                ]
-        date_ranges -- List of dictionaries.
-        field -- String.
-        filter -- FQL syntax. String.
+                    ],
+                    "size": 0,
+                    "sort": "string",
+                    "sub_aggregates": [
+                        null
+                    ],
+                    "time_zone": "string",
+                    "type": "string"
+                }
+        date_ranges -- If peforming a date range query specify the from and to date ranges.
+                       These can be in common date formats like 2019-07-18 or now.
+                       List of dictionaries.
+        exclude -- Fields to exclude. String.
+        field -- Term you want to aggregate on. If doing a date_range query,
+                 this is the date field you want to apply the date ranges to. String.
+        filter -- Optional filter criteria in the form of an FQL query.
+                  For more information about FQL queries, see our FQL documentation in Falcon.
+                  String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
         name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
         size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/quick_scan.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/real_time_response.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/real_time_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,58 +62,67 @@
 
         Supported aggregations:
             date_range
             term
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
-                List of dictionaries.
-                [{
-                    "date_ranges": [
+                [
+                    {
+                        "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
-                    ],
-                    "field": "string",
-                    "filter": "string",
-                    "interval": "string",
-                    "min_doc_count": 0,
-                    "missing": "string",
-                    "name": "string",
-                    "q": "string",
-                    "ranges": [
+                        ],
+                        "exclude": "string",
+                        "field": "string",
+                        "filter": "string",
+                        "from": 0,
+                        "include": "string",
+                        "interval": "string",
+                        "max_doc_count": 0,
+                        "min_doc_count": 0,
+                        "missing": "string",
+                        "name": "string",
+                        "q": "string",
+                        "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
-                    ],
-                    "size": 0,
-                    "sort": "string",
-                    "sub_aggregates": [
-                        null
-                    ],
-                    "time_zone": "string",
-                    "type": "string"
-                }]
+                        ],
+                        "size": 0,
+                        "sort": "string",
+                        "sub_aggregates": [
+                            null
+                        ],
+                        "time_zone": "string",
+                        "type": "string"
+                    }
+                ]
         date_ranges -- If peforming a date range query specify the from and to date ranges.
                        These can be in common date formats like 2019-07-18 or now.
                        List of dictionaries.
+        exclude -- Fields to exclude. String.
         field -- Term you want to aggregate on. If doing a date_range query,
                  this is the date field you want to apply the date ranges to. String.
         filter -- Optional filter criteria in the form of an FQL query.
                   For more information about FQL queries, see our FQL documentation in Falcon.
                   String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
-        name -- Name of the aggregation. String.
+        name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
-        size -- Size limit to apply to the queries. Integer.
+        size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
         time_zone -- String.
         type -- String.
 
         This method only supports keywords for providing arguments.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/real_time_response_admin.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/recon.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/recon.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,41 +74,54 @@
                     {
                         "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
                         ],
+                        "exclude": "string",
                         "field": "string",
                         "filter": "string",
+                        "from": 0,
+                        "include": "string",
                         "interval": "string",
+                        "max_doc_count": 0,
                         "min_doc_count": 0,
                         "missing": "string",
                         "name": "string",
                         "q": "string",
                         "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
                         ],
                         "size": 0,
                         "sort": "string",
                         "sub_aggregates": [
-                        null
+                            null
                         ],
                         "time_zone": "string",
                         "type": "string"
                     }
                 ]
-        date_ranges -- List of dictionaries.
-        field -- String.
-        filter -- FQL syntax. String.
+        date_ranges -- If peforming a date range query specify the from and to date ranges.
+                       These can be in common date formats like 2019-07-18 or now.
+                       List of dictionaries.
+        exclude -- Fields to exclude. String.
+        field -- Term you want to aggregate on. If doing a date_range query,
+                 this is the date field you want to apply the date ranges to. String.
+        filter -- Optional filter criteria in the form of an FQL query.
+                  For more information about FQL queries, see our FQL documentation in Falcon.
+                  String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
         name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
         size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
@@ -145,41 +158,54 @@
                     {
                         "date_ranges": [
                         {
                             "from": "string",
                             "to": "string"
                         }
                         ],
+                        "exclude": "string",
                         "field": "string",
                         "filter": "string",
+                        "from": 0,
+                        "include": "string",
                         "interval": "string",
+                        "max_doc_count": 0,
                         "min_doc_count": 0,
                         "missing": "string",
                         "name": "string",
                         "q": "string",
                         "ranges": [
                         {
                             "From": 0,
                             "To": 0
                         }
                         ],
                         "size": 0,
                         "sort": "string",
                         "sub_aggregates": [
-                        null
+                            null
                         ],
                         "time_zone": "string",
                         "type": "string"
                     }
                 ]
-        date_ranges -- List of dictionaries.
-        field -- String.
-        filter -- FQL syntax. String.
+        date_ranges -- If peforming a date range query specify the from and to date ranges.
+                       These can be in common date formats like 2019-07-18 or now.
+                       List of dictionaries.
+        exclude -- Fields to exclude. String.
+        field -- Term you want to aggregate on. If doing a date_range query,
+                 this is the date field you want to apply the date ranges to. String.
+        filter -- Optional filter criteria in the form of an FQL query.
+                  For more information about FQL queries, see our FQL documentation in Falcon.
+                  String.
+        from -- Integer.
+        include -- Fields to include. String.
         interval -- String.
-        min_doc_count -- Minimum number of documents required to match. Integer.
+        max_doc_count -- Maximum number of documents. Integer.
+        min_doc_count -- Minimum number of documents. Integer.
         missing -- String.
         name -- Scan name. String.
         q -- FQL syntax. String.
         ranges -- List of dictionaries.
         size -- Integer.
         sort -- FQL syntax. String.
         sub_aggregates -- List of strings.
@@ -277,32 +303,36 @@
                    {
                        "frequency": "string",
                        "recipients": [
                            "string"
                        ],
                        "type": "string"
                    }
+        content_format -- Content format. String.
         body -- full body payload, not required when using other keywords.
                 {
                     "actions": [
                         {
+                            "content_format": "string",
                             "frequency": "string",
                             "recipients": [
                                 "string"
                             ],
+                            "trigger_matchless": true,
                             "type": "string"
                         }
                     ],
                     "rule_id": "string"
                 }
         frequency - Frequency of the action. String. Used when only one
                     action is being handled.
         recipients -- UUIDs of the recipients. List of strings. Used when
                       only one action is being handled.
         rule_id -- Rule ID to attach the action to. Always required.
+        trigger_matchless -- Trigger on no matches. Boolean.
         type -- Action type, used when only one action is being handled.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: PATCH
@@ -349,25 +379,29 @@
     @force_default(defaults=["body"], default_types=["dict"])
     def update_action(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Update an action for a monitoring rule.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 {
+                    "content_format": "string",
                     "frequency": "string",
                     "id": "string",
                     "recipients": [
                         "string"
                     ],
-                    "status": "string"
+                    "status": "string",
+                    "trigger_matchless": "string"
                 }
+        content_format -- Content format. String.
         frequency - Frequency of the action. String.
         id -- Action ID. String.
         recipients -- UUIDs of the recipients. List of strings.
         status -- Action status. String.
+        trigger_matchless -- Trigger on no match. Boolean.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: PATCH
 
@@ -761,25 +795,29 @@
     def create_rules(self: object, body: list = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Create monitoring rules.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 [
                     {
+                        "breach_monitoring_enabled": true,
                         "filter": "string",
                         "name": "string",
                         "permissions": "string",
                         "priority": "string",
+                        "substring_matching_enabled": true,
                         "topic": "string"
                     }
                 ]
+        breach_monitoring_enabled -- Enable breach monitoring. Boolean.
         filter -- Rule filter. String.
         name -- Rule name. String.
         permissions -- String. (private / public)
         priority -- String. (high / medium / low)
+        substring_matching_enabled -- Enable substring matching. Boolean.
         topic -- Rule topic. String.
 
         This method only supports keywords for providing arguments.
 
         This method does not support body payload validation.
 
         Returns: dict object containing API response.
@@ -801,14 +839,15 @@
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def delete_rules(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Delete monitoring rules.
 
         Keyword arguments:
         ids -- List of rule IDs to delete. String or list of strings.
+        notificationsDeletionRequested -- Should notifications generated by this rule be deleted. Boolean.
         parameters - full parameters payload, not required if ids is provided as a keyword.
 
         Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
                    All others are ignored.
 
         Returns: dict object containing API response.
 
@@ -829,26 +868,30 @@
     def update_rules(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Update monitoring rules.
 
         Keyword arguments:
         body -- full body payload, not required when using other keywords.
                 [
                     {
+                        "breach_monitoring_enabled": true,
                         "filter": "string",
                         "id": "string",
                         "name": "string",
                         "permissions": "string",
-                        "priority": "string"
+                        "priority": "string",
+                        "substring_matching_enabled": true
                     }
                 ]
+        breach_monitoring_enabled -- Enable breach monitoring. Boolean.
         filter -- Rule filter. String.
         name -- Rule name. String.
         permissions -- String. (private / public)
         priority -- String. (high / medium / low)
         id -- Rule ID. String.
+        substring_matching_enabled -- Enable substring matching. Boolean.
 
         This method only supports keywords for providing arguments.
 
         This method does not support body payload validation.
 
         Returns: dict object containing API response.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/report_executions.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/response_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sample_uploads.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""CrowdStrike Falcon Real Time Response Policies API interface class.
+"""CrowdStrike Falcon Sample Upload API interface class.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -31,429 +31,492 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
+import json
 from typing import Dict, Union
-from ._util import process_service_request, force_default, handle_single_argument
-from ._payload import generic_payload_list, response_policy_payload
+from ._util import (
+    force_default,
+    process_service_request,
+    handle_single_argument,
+    generate_error_result
+    )
+from ._payload import extraction_payload
 from ._service_class import ServiceClass
-from ._endpoint._response_policies import _response_policies_endpoints as Endpoints
+from ._endpoint._sample_uploads import _sample_uploads_endpoints as Endpoints
 
 
-class ResponsePolicies(ServiceClass):
+class SampleUploads(ServiceClass):
     """The only requirement to instantiate an instance of this class is one of the following.
 
     - a valid client_id and client_secret provided as keywords.
     - a credential dictionary with client_id and client_secret containing valid API credentials
       {
           "client_id": "CLIENT_ID_HERE",
           "client_secret": "CLIENT_SECRET_HERE"
       }
     - a previously-authenticated instance of the authentication service class (oauth2.py)
-    - a valid token provided by the authentication service class (oauth2.py)
+    - a valid token provided by the authentication service class (OAuth2.token())
     """
 
     @force_default(defaults=["parameters"], default_types=["dict"])
-    def query_combined_policy_members(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Search for members of a Response policy by providing an FQL filter and paging details.
-
-        Returns a set of host details which match the filter criteria.
+    def list_archive(self: object, *args, parameters: dict = None, **kwargs) -> object:
+        """Retrieve the archive files in chunks.
 
         Keyword arguments:
-        id -- The ID of the Response Policy to search for members of
-        filter -- The filter expression that should be used to limit the results. FQL syntax.
-        limit -- The maximum number of records to return in this response. [Integer, 1-5000]
-                 Use with the offset parameter to manage pagination of results.
-        offset -- The offset to start retrieving records from. Integer.
-                  Use with the limit parameter to manage pagination of results.
-        parameters - full parameters payload, not required if using other keywords.
-        sort -- The property to sort by. FQL syntax.
+        id -- The SHA256 of the archive. String.
+        limit -- Maximum number of files to retrieve. Integer. Default: 100.
+        offset -- Starting offset from which to retrieve files.
+        parameters -- Full parameters payload, not required if id is provided as a keyword.
 
-        This method only supports keywords for providing arguments.
+        Arguments: When not specified, the first argument to this method is assumed to be 'id'.
+                   All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/queryCombinedRTResponsePolicyMembers
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/sample-uploads/ArchiveListV1
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="queryCombinedRTResponsePolicyMembers",
+            operation_id="ArchiveListV1",
             keywords=kwargs,
-            params=parameters
+            params=handle_single_argument(args, parameters, "id")
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
-    def query_combined_policies(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Search for Response Policies by providing an FQL filter and paging details.
+    def get_archive(self: object, *args, parameters: dict = None, **kwargs) -> object:
+        """Retrieve the archive upload operation status.
 
-        Returns a set of Response Policies which match the filter criteria.
+        Status `done` means that archive was processed successfully.
+        Status `error` means that archive was not processed successfully.
 
         Keyword arguments:
-        filter -- The filter expression that should be used to limit the results. FQL syntax.
-        limit -- The maximum number of records to return in this response. [Integer, 1-5000]
-                 Use with the offset parameter to manage pagination of results.
-        offset -- The offset to start retrieving records from. Integer.
-                  Use with the limit parameter to manage pagination of results.
-        parameters - full parameters payload, not required if using other keywords.
-        sort -- The property to sort by. FQL syntax.
+        id -- The SHA256 of the archive. String.
+        include_files -- Flag indicating if processed archives should also be returned. Boolean.
+        parameters -- Full parameters payload, not required if id is provided as a keyword.
 
-        This method only supports keywords for providing arguments.
+        Arguments: When not specified, the first argument to this method is assumed to be 'id'.
+                   All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/queryCombinedRTResponsePolicies
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/sample-uploads/ArchiveGetV1
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="queryCombinedRTResponsePolicies",
+            operation_id="ArchiveGetV1",
             keywords=kwargs,
-            params=parameters
+            params=handle_single_argument(args, parameters, "id")
             )
 
-    @force_default(defaults=["parameters", "body"], default_types=["dict", "dict"])
-    def perform_policies_action(self: object,
-                                body: dict = None,
-                                parameters: dict = None,
-                                **kwargs
-                                ) -> Dict[str, Union[int, dict]]:
-        """Perform the specified action on the Response Policies specified in the request.
-
-        Keyword arguments:
-        action_name -- action to perform: 'add-host-group', 'add-rule-group', 'disable',
-                       'enable', 'remove-host-group', or 'remove-rule-group'.
-        action_parameters -- Action specific parameter options. List of dictionaries.
-                             {
-                                 "name": "string",
-                                 "value": "string"
-                             }
-        body -- full body payload, not required if keywords are used.
-                {
-                    "action_parameters": [
-                        {
-                            "name": "group_id",
-                            "value": "string"
-                        }
-                    ],
-                    "ids": [
-                        "string"
-                    ]
-                }
-        group_id -- Host Group ID to apply the policy to. String.
-                    Overridden if action_parameters is provided.
-        ids -- Response policy ID(s) to perform actions against. String or list of strings.
-        parameters - full parameters payload, not required if action_name is provide as a keyword.
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def delete_archive(self: object, *args, parameters: dict = None, **kwargs) -> dict:
+        """Remove an archive that was uploaded previously.
 
-        This method only supports keywords for providing arguments.
+        Keyword arguments:
+        id -- The archive SHA256. String.
+        parameters -- full parameters payload, not required if id is provided as a keyword.
+
+        Arguments: When not specified, the first argument to this method is assumed to be 'id'.
+                   All others are ignored.
 
         Returns: dict object containing API response.
 
-        HTTP Method: POST
+        HTTP Method: DELETE
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/performRTResponsePoliciesAction
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/sample-uploads/ArchiveDeleteV1
         """
-        if not body:
-            body = generic_payload_list(submitted_keywords=kwargs, payload_value="ids")
-            if kwargs.get("group_id", None):
-                body["action_parameters"] = [{
-                    "name": "group_id",
-                    "value": kwargs.get("group_id", None)
-                }]
-            # Passing an action_parameters list will override the group_id keyword
-            if kwargs.get("action_parameters", None):
-                body["action_parameters"] = kwargs.get("action_parameters", None)
-
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="performRTResponsePoliciesAction",
+            operation_id="ArchiveDeleteV1",
             keywords=kwargs,
-            params=parameters,
-            body=body
+            params=handle_single_argument(args, parameters, "id")
             )
 
-    @force_default(defaults=["body"], default_types=["dict"])
-    def set_policies_precedence(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Set the precedence of Response Policies based on the order of IDs in the request.
+    @force_default(defaults=["parameters", "body"], default_types=["dict", "dict"])
+    def upload_archive_v1(self: object,
+                          body: dict = None,
+                          parameters: dict = None,
+                          **kwargs
+                          ) -> dict:
+        """Upload an archive and extract the files list from it.
+
+        This operation is asynchronous. Use ArchiveGetV1 to check the status.
+        After uploading, use ExtractionCreateV1 to copy the file to internal storage
+        making it available for content analysis.
 
-        The first ID specified will have the highest precedence and the last ID specified will
-        have the lowest. You must specify all non-Default Policies for a platform when updating
-        precedence.
+        ** DEPRECATED ** - Leverage the ArchiveUploadV2 operation instead.
 
         Keyword arguments:
-        body -- full body payload, not required if keywords are used.
-                {
-                    "ids": [
-                        "string"
-                    ],
-                    "platform_name": "string"
-                }
-        ids -- Prevention policy ID(s) to perform actions against. String or list of strings.
-        platform_name -- OS platform name. (Linux, Mac, Windows)
+        body -- Content of the uploaded archive in binary format. 7zip / zip only.
+        comment -- A descriptive comment to identify the file for other users. String.
+        name -- Name of the archive. String.
+        file_type -- Archive file format. String. "zip", "7zip". Defaults to "zip".
+        is_confidential -- Defines the visibility of this file in Falcon MalQuery, either
+                           via the  API or the Falcon console.
+                           True = File is only shown to users within your customer account.
+                           False = File can be seen by other CrowdStrike customers.
+                           Defaults to True.
+        parameters -- full parameters payload, not required if using other keywords.
+        password -- Archive password. String.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: POST
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/setRTResponsePoliciesPrecedence
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/sample-uploads/ArchiveUploadV1
         """
+        # Try to find the binary object they provided us
         if not body:
-            body = generic_payload_list(submitted_keywords=kwargs, payload_value="ids")
-            if kwargs.get("platform_name", None):
-                body["platform_name"] = kwargs.get("platform_name", None)
+            return generate_error_result("You must provide an archive to upload.", code=400)
 
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="setRTResponsePoliciesPrecedence",
-            body=body
+            operation_id="ArchiveUploadV1",
+            data=body,
+            body=None,
+            keywords=kwargs,
+            params=parameters
             )
 
-    @force_default(defaults=["parameters"], default_types=["dict"])
-    def get_policies(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Retrieve a set of Response Policies by specifying their IDs.
+    @force_default(defaults=["parameters", "body"], default_types=["dict", "dict"])
+    def upload_archive(self: object,
+                       name: str = None,
+                       file_data: dict = None,
+                       body: dict = None,
+                       parameters: dict = None,
+                       **kwargs
+                       ) -> dict:
+        """Upload an archive and extract the files list from it.
+
+        This operation is asynchronous. Use ArchiveGetV1 to check the status.
+        After uploading, use ExtractionCreateV1 to copy the file to internal storage
+        making it available for content analysis.
 
         Keyword arguments:
-        ids -- List of Response Policy IDs to retrieve. String or list of strings.
-        parameters -- full parameters payload, not required if ids is provided as a keyword.
+        comment -- A descriptive comment to identify the file for other users. String.
+        file_data -- Content of the uploaded archive in binary format.
+                     'archive' and 'file' are also accepted as this parameter.
+        name -- Name of the archive. String. Required.
+        file_type -- Archive file format. String. "zip", "7zip". Defaults to "zip".
+        is_confidential -- Defines the visibility of this file in Falcon MalQuery, either
+                           via the  API or the Falcon console.
+                           True = File is only shown to users within your customer account.
+                           False = File can be seen by other CrowdStrike customers.
+                           Defaults to True.
+        parameters -- full parameters payload, not required if using other keywords.
+        password -- Archive password. String.
 
-        Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
-                   All others are ignored.
+        This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
-        HTTP Method: GET
+        HTTP Method: POST
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/getRTResponsePolicies
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/sample-uploads/ArchiveUploadV2
         """
+        # Check for file name
+        if not name:
+            return generate_error_result("You must provide an archive filename.", code=400)
+        # Try to find the binary object they provided us
+        if not file_data:
+            file_data = kwargs.get("file", None)
+            if not file_data:
+                file_data = kwargs.get("archive", None)
+
+        # Determine our content type
+        file_type = str(kwargs.get("file_type", "zip")).lower()
+        content_map = {
+            "zip": "application/zip",
+            "7zip": "application/x-7z-compressed"
+        }
+
+        content_type = content_map.get(file_type, content_map.get("zip"))
+        # Create a multipart form payload for our upload file
+        file_tuple = [("file", (name, file_data, content_type))]
+        file_extended = {"name": name}
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="getRTResponsePolicies",
+            operation_id="ArchiveUploadV2",
+            body=body,
+            files=file_tuple,
+            data=file_extended,
             keywords=kwargs,
-            params=handle_single_argument(args, parameters, "ids")
+            params=parameters
             )
 
-    @force_default(defaults=["body"], default_types=["dict"])
-    def create_policies(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Create Response Policies by specifying details about the policy to create.
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def list_extraction(self: object, *args, parameters: dict = None, **kwargs) -> object:
+        """Retrieve the file extractions in chunks.
+
+        Status `done` means that all files were processed successfully.
+        Status `error` means that at least one of the files could not be processed.
 
         Keyword arguments:
-        body -- full body payload, not required if keywords are used.
-                {
-                    "resources": [
-                        {
-                            "clone_id": "string",
-                            "description": "string",
-                            "name": "string",
-                            "platform_name": "Windows",
-                            "settings": [
-                                {
-                                    "id": "string",
-                                    "value": {}
-                                }
-                            ]
-                        }
-                    ]
-                }
-        clone_id -- Response Policy ID to clone. String.
-        description -- Response Policy description. String.
-        name -- Response Policy name. String.
-        platform_name -- Name of the operating system platform. String.
-        settings -- Response policy specific settings. List of dictionaries.
-                    {
-                        "id": "string",
-                        "value": {}
-                    }
+        id -- The extraction operation ID. String.
+        limit -- Maximum number of file extractions to retrieve. Integer. Default: 0.
+        offset -- Starting offset from where to retrieve extractions.
+        parameters -- Full parameters payload, not required if id is provided as a keyword.
 
-        This method only supports keywords for providing arguments.
+        Arguments: When not specified, the first argument to this method is assumed to be 'id'.
+                   All others are ignored.
 
         Returns: dict object containing API response.
 
-        HTTP Method: POST
+        HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/createRTResponsePolicies
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/sample-uploads/ExtractionListV1
         """
-        if not body:
-            body = response_policy_payload(passed_keywords=kwargs)
-
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="createRTResponsePolicies",
-            body=body
+            operation_id="ExtractionListV1",
+            keywords=kwargs,
+            params=handle_single_argument(args, parameters, "id")
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
-    def delete_policies(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Delete a set of Response Policies by specifying their IDs.
+    def get_extraction(self: object, *args, parameters: dict = None, **kwargs) -> object:
+        """Retrieve the files extraction operation statuses.
+
+        Status `done` means that all files were processed successfully.
+        Status `error` means that at least one of the files could not be processed.
 
         Keyword arguments:
-        ids -- List of Response Policy IDs to delete. String or list of strings.
-        parameters -- full parameters payload, not required if ids is provided as a keyword.
+        id -- The extraction operation ID. String.
+        include_files -- Flag indicating if processed archives should also be returned. Boolean.
+        parameters -- Full parameters payload, not required if id is provided as a keyword.
 
-        Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
+        Arguments: When not specified, the first argument to this method is assumed to be 'id'.
                    All others are ignored.
 
         Returns: dict object containing API response.
 
-        HTTP Method: DELETE
+        HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/deleteRTResponsePolicies
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/sample-uploads/ExtractionGetV1
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="deleteRTResponsePolicies",
+            operation_id="ExtractionGetV1",
             keywords=kwargs,
-            params=handle_single_argument(args, parameters, "ids")
+            params=handle_single_argument(args, parameters, "id")
             )
 
     @force_default(defaults=["body"], default_types=["dict"])
-    def update_policies(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Update Response Policies by specifying the ID of the policy and details to update.
+    def create_extraction(self: object,
+                          file_data: object = None,
+                          body: dict = None,
+                          **kwargs
+                          ) -> dict:
+        """Extract files from an uploaded archive and copy them to internal storage for analysis.
 
         Keyword arguments:
-        body -- full body payload, not required if keywords are used.
+        body -- Full body payload in JSON format. Not required if using other keywords. Dictionary.
                 {
-                    "resources": [
+                    "extract_all": true,
+                    "files": [
                         {
-                            "description": "string",
-                            "id": "string",
-                            "name": "string",
-                            "settings": [
-                                {
-                                    "id": "string",
-                                    "value": {}
-                                }
-                            ]
+                            "comment": "string",
+                            "is_confidential": true,
+                            "name": "string"
                         }
-                    ]
+                    ],
+                    "sha256": "string"
                 }
-        description -- Response Policy description. String.
-        id -- Response Policy ID to update. String.
-        name -- Response Policy name. String.
-        settings -- Response policy specific settings. List of dictionaries.
-                    {
-                        "id": "string",
-                        "value": "string"
-                    }
+        extract_all -- Flag indicating if all files should be extracted. Boolean.
+        files -- List of files to be extracted from the archive. List of dictionaries.
+        sha256 -- SHA256 Archive ID of the archive. String.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
-        HTTP Method: PATCH
+        HTTP Method: POST
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/updateRTResponsePolicies
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/sample-uploads/ExtractionCreateV1
         """
         if not body:
-            body = response_policy_payload(passed_keywords=kwargs)
+            body = extraction_payload(passed_keywords=kwargs)
 
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="updateRTResponsePolicies",
-            body=body
+            operation_id="ExtractionCreateV1",
+            body=body,
+            data=file_data,
+            keywords=kwargs
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
-    def query_policy_members(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Search for members of a Response policy by providing an FQL filter and paging details.
-
-        Returns a set of Agent IDs which match the filter criteria.
+    def get_sample(self: object, *args, parameters: dict = None, **kwargs) -> object:
+        """Retrieve the file associated with the given ID (SHA256).
 
         Keyword arguments:
-        id -- The ID of the Response Policy to search for members of
-        filter -- The filter expression that should be used to limit the results. FQL syntax.
-        limit -- The maximum number of records to return in this response. [Integer, 1-5000]
-                 Use with the offset parameter to manage pagination of results.
-        offset -- The offset to start retrieving records from. Integer.
-                  Use with the limit parameter to manage pagination of results.
-        parameters - full parameters payload, not required if using other keywords.
-        sort -- The property to sort by. FQL syntax.
+        ids -- List of SHA256s to retrieve. String or list of strings.
+        parameters -- full parameters payload, not required if ids is provided as a keyword.
+        password_protected -- Flag whether the sample should be zipped and password protected
+                              with the pass of 'infected'. Defaults to False.
 
-        This method only supports keywords for providing arguments.
+        Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
+                   All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/queryRTResponsePolicyMembers
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/sample-uploads/GetSampleV3
         """
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="queryRTResponsePolicyMembers",
+            operation_id="GetSampleV3",
             keywords=kwargs,
-            params=parameters
+            params=handle_single_argument(args, parameters, "ids")
             )
 
-    @force_default(defaults=["parameters"], default_types=["dict"])
-    def query_policies(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Search for Response Policies by providing an FQL filter with sort and/or paging details.
+    @force_default(defaults=["parameters", "body"], default_types=["dict", "dict"])
+    def upload_sample(self: object,
+                      file_data: object = None,
+                      body: dict = None,
+                      parameters: dict = None,
+                      **kwargs
+                      ) -> Dict[str, Union[int, dict]]:
+        """Upload a file for further cloud analysis.
 
-        This returns a set of Response Policy IDs that match the given criteria.
+        After uploading, call the specific analysis API endpoint.
 
         Keyword arguments:
-        filter -- The filter expression that should be used to limit the results. FQL syntax.
-        limit -- The maximum number of records to return in this response. [Integer, 1-5000]
-                 Use with the offset parameter to manage pagination of results.
-        offset -- The offset to start retrieving records from. Integer.
-                  Use with the limit parameter to manage pagination of results.
-        parameters - full parameters payload, not required if using other keywords.
-        sort -- The property to sort by. FQL syntax.
+        comment -- A descriptive comment to identify the file for other users. String.
+        file_data -- Content of the uploaded sample in binary format. Max file size is 256 MB.
+                     'sample' and 'upfile' are also accepted as this parameter.
+
+                     Accepted File Formats:
+                     Portable executables: .exe, .scr, .pif, .dll, .com, .cpl, etc.
+                     Office documents: .doc, .docx, .ppt, .pps, .pptx, .ppsx, .xls,
+                                       .xlsx, .rtf, .pub
+                     PDF
+                     APK
+                     Executable JAR
+                     Windows script component: .sct
+                     Windows shortcut: .lnk
+                     Windows help: .chm
+                     HTML application: .hta
+                     Windows script file: .wsf
+                     Javascript: .js
+                     Visual Basic: .vbs, .vbe
+                     Shockwave Flash: .swf
+                     Perl: .pl
+                     Powershell: .ps1, .psd1, .psm1
+                     Scalable vector graphics: .svg
+                     Python: .py
+                     Linux ELF executables
+                     Email files: MIME RFC 822 .eml, Outlook .msg
+        file_name -- Name of the file. String.
+        is_confidential -- Defines the visibility of this file in Falcon MalQuery, either
+                           via the  API or the Falcon console.
+                           True = File is only shown to users within your customer account.
+                           False = File can be seen by other CrowdStrike customers.
+                           Defaults to True.
+        parameters -- full parameters payload, not required if using other keywords.
+
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
-        HTTP Method: GET
+        HTTP Method: POST
 
         Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/response-policies/queryRTResponsePolicies
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/sample-uploads/UploadSampleV3
         """
+        # Try to find the binary object they provided us
+        if not file_data:
+            file_data = kwargs.get("sample", None)
+            if not file_data:
+                file_data = kwargs.get("upfile", None)
+        # Create a copy of our default header dictionary
+        header_payload = json.loads(json.dumps(self.headers))
+        # Set our content-type header
+        header_payload["Content-Type"] = "application/octet-stream"
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="queryRTResponsePolicies",
+            operation_id="UploadSampleV3",
+            headers=header_payload,  # Pass our custom headers
+            body=body,
+            data=file_data,
             keywords=kwargs,
             params=parameters
             )
 
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def delete_sample(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Remove a sample, including file, meta and submissions from the collection.
+
+        Keyword arguments:
+        ids -- List of SHA256s to delete. String or list of strings.
+        parameters -- full parameters payload, not required if ids is provided as a keyword.
+
+        Arguments: When not specified, the first argument to this method is assumed to be 'ids'.
+                   All others are ignored.
+
+        Returns: dict object containing API response.
+
+        HTTP Method: DELETE
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/sample-uploads/DeleteSampleV3
+        """
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="DeleteSampleV3",
+            keywords=kwargs,
+            params=handle_single_argument(args, parameters, "ids")
+            )
+
     # These method names align to the operation IDs in the API but
     # do not conform to snake_case / PEP8 and are defined here for
     # backwards compatibility / ease of use purposes
-    queryCombinedRTResponsePolicyMembers = query_combined_policy_members
-    queryCombinedRTResponsePolicies = query_combined_policies
-    performRTResponsePoliciesAction = perform_policies_action
-    setRTResponsePoliciesPrecedence = set_policies_precedence
-    getRTResponsePolicies = get_policies
-    createRTResponsePolicies = create_policies
-    deleteRTResponsePolicies = delete_policies
-    updateRTResponsePolicies = update_policies
-    queryRTResponsePolicyMembers = query_policy_members
-    queryRTResponsePolicies = query_policies
+    ArchiveListV1 = list_archive
+    ArchiveGetV1 = get_archive
+    ArchiveDeleteV1 = delete_archive
+    ArchiveUploadV1 = upload_archive_v1
+    archive_upload_v1 = upload_archive_v1
+    ArchiveUploadV2 = upload_archive
+    archive_upload = upload_archive
+    ExtractionListV1 = list_extraction
+    ExtractionGetV1 = get_extraction
+    ExtractionCreateV1 = create_extraction
+    GetSampleV3 = get_sample
+    UploadSampleV3 = upload_sample
+    DeleteSampleV3 = delete_sample
 
 
 # The legacy name for this class does not conform to PascalCase / PEP8
 # It is defined here for backwards compatibility purposes only.
-Response_Policies = ResponsePolicies  # pylint: disable=C0103
+Sample_Uploads = SampleUploads  # pylint: disable=C0103
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/scheduled_reports.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/sensor_download.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/sensor_update_policy.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_update_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,16 +96,17 @@
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def query_combined_builds(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve available builds for use with Sensor Update Policies.
 
         Keyword arguments:
         platform -- The platform to return builds for. String.
-                    Allowed values: "linux", "mac", "windows"
+                    Allowed values: "linux", "linuxarm64", "mac", "windows", "zlinux"
         parameters -- full parameters payload, not required if platform is provided as a keyword.
+        stage -- The stages to return builds for. String or list of strings.
 
         Arguments: When not specified, the first argument to this method is assumed to be
                    'platform'. All others are ignored.
 
         Returns: dict object containing API response.
 
         HTTP Method: GET
@@ -266,16 +267,16 @@
                                 body: dict = None,
                                 parameters: dict = None,
                                 **kwargs
                                 ) -> Dict[str, Union[int, dict]]:
         """Perform the specified action on the Sensor Update Policies specified in the request.
 
         Keyword arguments:
-        action_name -- action to perform: 'add-host-group', 'disable', 'enable',
-                       or 'remove-host-group'.
+        action_name -- action to perform: 'add-host-group', 'add-rule-group', 'disable', 'enable',
+                       'remove-rule-group' or 'remove-host-group'.
         action_parameters -- Action specific parameter options. List of dictionaries.
                              {
                                  "name": "string",
                                  "value": "string"
                              }
         body -- full body payload, not required if keywords are used.
                 {
@@ -563,33 +564,76 @@
                 {
                     "resources": [
                         {
                             "description": "string",
                             "name": "string",
                             "platform_name": "Windows",
                             "settings": {
-                                    "build": "string",
-                                    "uninstall_protection": "ENABLED"
+                                "build": "string",
+                                "scheduler": {
+                                    "enabled": true,
+                                    "schedules": [
+                                        {
+                                            "days": [
+                                                0
+                                            ],
+                                            "end": "string",
+                                            "start": "string"
+                                        }
+                                    ],
+                                    "timezone": "string"
+                                },
+                                "show_early_adopter_builds": true,
+                                "uninstall_protection": "ENABLED",
+                                "variants": [
+                                    {
+                                        "build": "string",
+                                        "platform": "string"
+                                    }
+                                ]
                             }
                         }
                     ]
                 }
         build -- Build policy applies to. String.
         description -- Sensor Update Policy description. String.
         name -- Sensor Update Policy name. String.
         platform_name -- Name of the operating system platform. String.
+        scheduler -- Scheduler settings. Dictionary.
         settings -- Sensor update policy specific settings. Dictionary.
                     OVERRIDES the value of the "build" and "uninstall_protection"
                     keywords if provided.
                     {
                         "build": "string",
-                        "uninstall_protection": "ENABLED"
+                        "scheduler": {
+                            "enabled": true,
+                            "schedules": [
+                                {
+                                    "days": [
+                                        0
+                                    ],
+                                    "end": "string",
+                                    "start": "string"
+                                }
+                            ],
+                            "timezone": "string"
+                        },
+                        "show_early_adopter_builds": true,
+                        "uninstall_protection": "ENABLED",
+                        "variants": [
+                            {
+                                "build": "string",
+                                "platform": "string"
+                            }
+                        ]
                     }
+        show_early_adopter_builds -- Enable early adopter builds. Boolean.
         uninstall_protection -- Boolean indicating if uninstall protection should be enabled.
                                 String. Allowed values: "ENABLED", "DISABLED"
+        variants -- List of variants. List of dictionaries.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: POST
 
@@ -617,32 +661,55 @@
                 {
                     "resources": [
                         {
                             "description": "string",
                             "id": "string",
                             "name": "string",
                             "settings": {
-                                    "build": "string",
-                                    "uninstall_protection": "ENABLED"
+                                "build": "string",
+                                "scheduler": {
+                                    "enabled": true,
+                                    "schedules": [
+                                        {
+                                            "days": [
+                                                0
+                                            ],
+                                            "end": "string",
+                                            "start": "string"
+                                        }
+                                    ],
+                                    "timezone": "string"
+                                },
+                                "show_early_adopter_builds": true,
+                                "uninstall_protection": "ENABLED",
+                                "variants": [
+                                    {
+                                        "build": "string",
+                                        "platform": "string"
+                                    }
+                                ]
                             }
                         }
                     ]
                 }
         build -- Build policy applies to . String.
         description -- Sensor Update Policy description. String.
         id -- Sensor Update Policy ID to update. String.
         name -- Sensor Update Policy name. String.
+        scheduler -- Schedule settings. Dictionary.
         settings -- Sensor Update policy specific settings. Dictionary.
                     OVERRIDES the value of the "build" keyword if provided.
                     {
                         "build": "string",
                         "uninstall_protection": "ENABLED"
                     }
+        show_early_adopter_builds -- Display early adopter builds. Boolean.
         uninstall_protection -- Boolean indicating if uninstall protection should be enabled.
                                 String. Allowed values: "ENABLED", "DISABLED"
+        variants -- Allowed variants list. List of dictionaries.
 
         This method only supports keywords for providing arguments.
 
         Returns: dict object containing API response.
 
         HTTP Method: PATCH
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/sensor_visibility_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/spotlight_evaluation_logic.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/spotlight_vulnerabilities.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/spotlight_vulnerabilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                  the results.
         facet -- Select various details blocks to be returned for each vulnerability entry.
                  Supported values:
                  cve_details            host_info
                  remediation_details    evaluation_logic
         filter -- Filter items using a query in Falcon Query Language (FQL).
                   Wildcards '*' are unsupported.
-        limit -- The number of items to return in this response (default: 100, max: 400).
+        limit -- The number of items to return in this response (default: 100, max: 5000).
                  Use with the after parameter to manage pagination of results. Integer.
         parameters - full parameters payload, not required if using other keywords.
         sort -- The property to sort by.
                 FQL syntax (e.g. created_timestamp|desc, closed_timestamp|asc).
 
         This method only supports keywords for providing arguments.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/tailored_intelligence.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev1/src/falconpydev/user_management.py` & `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/user_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -476,14 +476,16 @@
         HTTP Method: GET
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/queriesRolesV1
 
         Keyword arguments
         ----
+        action : str
+            Actionable purpose of the query. Default: grant
         cid : str
             Customer ID to get available roles for. An empty `cid` keyword will return
             role IDs for the current CID.
         parameters : str
             Full parameters payload in JSON format, not required.
         user_uuid : str
             User UUID to get available roles for. An empty `user_uuid` keyword will return
@@ -551,14 +553,16 @@
             params=parameters
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def get_roles(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Get information about a role.
 
+        DEPRECATED: Please use entitiesRolesV1 instead.
+
         HTTP Method: GET
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/GetRoles
 
         Keyword arguments
         ----
@@ -586,14 +590,16 @@
             params=handle_single_argument(args, parameters, "ids")
             )
 
     @force_default(defaults=["parameters", "body"], default_types=["dict", "dict"])
     def grant_user_role_ids(self: object, body: dict, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Assign one or more roles to a user.
 
+        DEPRECATED: Please use userActionV1 instead.
+
         HTTP Method: POST
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/GrantUserRoleIds
 
         Keyword arguments
         ----
@@ -639,14 +645,16 @@
             params=parameters
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def revoke_user_role_ids(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Revoke one or more roles from a user.
 
+        DEPRECATED: Please use userActionV1 instead.
+
         HTTP Method: DELETE
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/RevokeUserRoleIds
 
         Keyword arguments
         ----
@@ -676,14 +684,16 @@
             )
 
     def get_available_role_ids(self: object) -> Dict[str, Union[int, dict]]:
         """Show role IDs for all roles available in your customer account.
 
         For more information on each role, provide the role ID to get_roles.
 
+        DEPRECATED: Please use queriesRolesV1 instead.
+
         HTTP Method: GET
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/GetAvailableRoleIds
 
         Keyword arguments
         ----
@@ -706,14 +716,16 @@
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def get_user_role_ids(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Show role IDs of roles assigned to a user.
 
         For more information on each role, provide the role ID to `get_role`.
 
+        DEPRECATED: Please use combinedUserRolesV1 instead.
+
         HTTP Method: GET
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/GetUserRoleIds
 
         Keyword arguments
         ----
@@ -741,14 +753,16 @@
             params=handle_single_argument(args, parameters, "user_uuid")
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def retrieve_user(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Get information about a user.
 
+        DEPRECATED: Please use retrieveUsersGETV1 instead.
+
         HTTP Method: GET
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/RetrieveUser
 
         Keyword arguments
         ----
@@ -778,14 +792,16 @@
 
     @force_default(defaults=["body"], default_types=["dict"])
     def create_user(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Create a new user.
 
         After creating a user, assign one or more roles with `grant_user_role_ids`.
 
+        DEPRECATED: Please use createUserV1 instead.
+
         HTTP Method: POST
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/CreateUser
 
         Keyword arguments
         ----
@@ -836,14 +852,16 @@
             body=body
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def delete_user(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Delete a user permanently.
 
+        DEPRECATED: Please use deleteUserV1 instead.
+
         HTTP Method: DELETE
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/DeleteUser
 
         Keyword arguments
         ----
@@ -871,14 +889,16 @@
             params=handle_single_argument(args, parameters, "user_uuid")
             )
 
     @force_default(defaults=["parameters", "body"], default_types=["dict", "dict"])
     def update_user(self: object, body: dict = None, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Modify an existing user.
 
+        DEPRECATED: Please use updateUserV1 instead.
+
         HTTP Method: PATCH
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/UpdateUser
 
         Keyword arguments
         ----
@@ -922,14 +942,16 @@
             keywords=kwargs,
             params=parameters
             )
 
     def retrieve_emails_by_cid(self: object) -> Dict[str, Union[int, dict]]:
         """List the usernames (usually an email address) for all users in your customer account.
 
+        DEPRECATED: Please use retrieveUsersGETV1 instead.
+
         HTTP Method: GET
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/RetrieveEmailsByCID
 
         Keyword arguments
         ----
@@ -951,14 +973,16 @@
             )
 
     def retrieve_user_uuids_by_cid(self: object) -> Dict[str, Union[int, dict]]:
         """List user IDs for all users in your customer account.
 
         For more information on each user, provide the user ID to `retrieve_user`.
 
+        DEPRECATED: Please use queryUserV1 instead.
+
         HTTP Method: GET
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/RetrieveUserUUIDsByCID
 
         Keyword arguments
         ----
@@ -979,14 +1003,16 @@
             operation_id="RetrieveUserUUIDsByCID"
             )
 
     @force_default(defaults=["parameters"], default_types=["dict"])
     def retrieve_user_uuid(self: object, *args, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Get a user's ID by providing a username (usually an email address).
 
+        DEPRECATED: Please use queryUserV1 instead.
+
         HTTP Method: GET
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/user-management/RetrieveUserUUID
 
         Keyword arguments
         ----
```

