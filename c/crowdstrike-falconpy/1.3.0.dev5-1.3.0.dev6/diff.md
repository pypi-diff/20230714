# Comparing `tmp/crowdstrike-falconpy-1.3.0.dev5.tar.gz` & `tmp/crowdstrike-falconpy-1.3.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdstrike-falconpy-1.3.0.dev5.tar", last modified: Thu Jul 13 03:23:05 2023, max compression
+gzip compressed data, was "crowdstrike-falconpy-1.3.0.dev6.tar", last modified: Fri Jul 14 05:23:17 2023, max compression
```

## Comparing `crowdstrike-falconpy-1.3.0.dev5.tar` & `crowdstrike-falconpy-1.3.0.dev6.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.511453 crowdstrike-falconpy-1.3.0.dev5/
--rw-r--r--   0 jhiller    (501) staff       (20)     4906 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/AUTHORS.md
--rw-r--r--   0 jhiller    (501) staff       (20)     1211 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/LICENSE
--rw-r--r--   0 jhiller    (501) staff       (20)    31332 2023-07-13 03:23:05.510942 crowdstrike-falconpy-1.3.0.dev5/PKG-INFO
--rw-r--r--   0 jhiller    (501) staff       (20)    29563 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/README.md
--rw-r--r--   0 jhiller    (501) staff       (20)       38 2023-07-13 03:23:05.511614 crowdstrike-falconpy-1.3.0.dev5/setup.cfg
--rw-r--r--   0 jhiller    (501) staff       (20)     4482 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/setup.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.296267 crowdstrike-falconpy-1.3.0.dev5/src/
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.308631 crowdstrike-falconpy-1.3.0.dev5/src/crowdstrike_falconpy.egg-info/
--rw-r--r--   0 jhiller    (501) staff       (20)    31332 2023-07-13 03:23:05.000000 crowdstrike-falconpy-1.3.0.dev5/src/crowdstrike_falconpy.egg-info/PKG-INFO
--rw-r--r--   0 jhiller    (501) staff       (20)     7615 2023-07-13 03:23:05.000000 crowdstrike-falconpy-1.3.0.dev5/src/crowdstrike_falconpy.egg-info/SOURCES.txt
--rw-r--r--   0 jhiller    (501) staff       (20)        1 2023-07-13 03:23:05.000000 crowdstrike-falconpy-1.3.0.dev5/src/crowdstrike_falconpy.egg-info/dependency_links.txt
--rw-r--r--   0 jhiller    (501) staff       (20)       83 2023-07-13 03:23:05.000000 crowdstrike-falconpy-1.3.0.dev5/src/crowdstrike_falconpy.egg-info/requires.txt
--rw-r--r--   0 jhiller    (501) staff       (20)        9 2023-07-13 03:23:05.000000 crowdstrike-falconpy-1.3.0.dev5/src/crowdstrike_falconpy.egg-info/top_level.txt
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.369589 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/
--rw-r--r--   0 jhiller    (501) staff       (20)    12051 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/__init__.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.374313 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/
--rw-r--r--   0 jhiller    (501) staff       (20)     2095 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11250 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5561 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request_behavior.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5022 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request_connection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3788 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request_meta.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5358 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request_payloads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3827 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request_validator.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.377381 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/
--rw-r--r--   0 jhiller    (501) staff       (20)     2047 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4234 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/_base_falcon_auth.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5998 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/_bearer_token.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20032 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/_falcon_interface.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4806 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/_interface_config.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8624 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/_uber_interface.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.378080 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_constant/
--rw-r--r--   0 jhiller    (501) staff       (20)     2905 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_constant/__init__.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.439853 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/
--rw-r--r--   0 jhiller    (501) staff       (20)     9054 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7042 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6740 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)    30329 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13488 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15447 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6446 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10667 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_device_control_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3167 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_event_streams.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12391 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_falcon_complete_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6172 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_falcon_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14991 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_falconx_sandbox.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3694 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    23292 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10008 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_firewall_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9015 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10381 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8008 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6237 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    22179 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_intel.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4594 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_ioa_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11784 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13556 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15790 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_kubernetes_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5803 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7033 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4457 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_ml_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2377 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_mobile_enrollment.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20286 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3611 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_oauth2.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12950 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3569 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_overwatch_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9960 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_prevention_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4808 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_quarantine.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4165 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_quick_scan.py
--rw-r--r--   0 jhiller    (501) staff       (20)    24729 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16057 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17960 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9918 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_response_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11674 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5275 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_sensor_download.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15927 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_sensor_update_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4678 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_sensor_visibility_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4667 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_spotlight_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7134 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_spotlight_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4885 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_tailored_intelligence.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16463 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_user_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6050 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_zero_trust_assessment.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.448403 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/
--rw-r--r--   0 jhiller    (501) staff       (20)     4611 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13207 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5506 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17702 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3316 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5947 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11312 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2177 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13181 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13678 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13342 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1945 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_zero_trust_assessment.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.449919 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_enum/
--rw-r--r--   0 jhiller    (501) staff       (20)     1871 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_enum/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2124 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_enum/_base_url.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2063 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_enum/_container_base_url.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2218 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_enum/_token_fail_reason.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.451644 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_error/
--rw-r--r--   0 jhiller    (501) staff       (20)     2606 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_error/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5837 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_error/_exceptions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3573 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_error/_warnings.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.452459 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_log/
--rw-r--r--   0 jhiller    (501) staff       (20)     1744 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_log/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3809 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_log/_facility.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.500392 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/
--rw-r--r--   0 jhiller    (501) staff       (20)     5516 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2691 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3624 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5855 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6079 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4604 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2790 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6181 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_device_control_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3666 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_falconx.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16333 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_firewall.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7329 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_generic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4290 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4511 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5808 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7508 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5577 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3774 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2866 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4506 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3118 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_prevention_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4309 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8001 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2615 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_response_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2433 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4519 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_sensor_update_policy.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.505951 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/
--rw-r--r--   0 jhiller    (501) staff       (20)     4540 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/__base_resource.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2186 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4581 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_base_dictionary.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1825 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_errors.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2684 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_expanded_result.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_headers.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3298 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_meta.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2489 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_resources.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4561 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_response_component.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16223 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_result.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.507642 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_service_class/
--rw-r--r--   0 jhiller    (501) staff       (20)     1827 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_service_class/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12272 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_service_class/_base_service_class.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11239 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_service_class/_service_class.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-13 03:23:05.510076 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_util/
--rw-r--r--   0 jhiller    (501) staff       (20)     3087 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_util/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3076 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_util/_auth.py
--rw-r--r--   0 jhiller    (501) staff       (20)    33929 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_util/_functions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6161 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_util/_uber.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3539 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_version.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17508 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9970 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/api_complete.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15947 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)    48601 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    34208 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)    27069 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10750 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/debug.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15759 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)    29552 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/device_control_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    22218 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5973 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/event_streams.py
--rw-r--r--   0 jhiller    (501) staff       (20)    37615 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/falcon_complete_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16270 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/falcon_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)    28300 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/falconx_sandbox.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8668 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5384 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    79369 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20174 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/firewall_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    18869 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)    27450 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4578 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13758 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13613 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    34693 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/intel.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10663 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/ioa_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    35840 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14032 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    25074 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/kubernetes_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16367 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)    23565 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10056 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/ml_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5166 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/mobile_enrollment.py
--rw-r--r--   0 jhiller    (501) staff       (20)    43338 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8919 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/oauth2.py
--rw-r--r--   0 jhiller    (501) staff       (20)    35443 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13881 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/overwatch_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20718 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/prevention_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14372 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/quarantine.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9493 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/quick_scan.py
--rw-r--r--   0 jhiller    (501) staff       (20)    43159 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    25250 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)    45859 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7687 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    19891 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/response_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    21891 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6764 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10169 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/sensor_download.py
--rw-r--r--   0 jhiller    (501) staff       (20)    38364 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/sensor_update_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9899 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/sensor_visibility_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8333 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/spotlight_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10652 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/spotlight_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9791 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/tailored_intelligence.py
--rw-r--r--   0 jhiller    (501) staff       (20)    39321 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/user_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8311 2023-07-13 03:23:03.000000 crowdstrike-falconpy-1.3.0.dev5/src/falconpy/zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.866279 crowdstrike-falconpy-1.3.0.dev6/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4906 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/AUTHORS.md
+-rw-r--r--   0 jhiller    (501) staff       (20)     1211 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/LICENSE
+-rw-r--r--   0 jhiller    (501) staff       (20)    31332 2023-07-14 05:23:17.865932 crowdstrike-falconpy-1.3.0.dev6/PKG-INFO
+-rw-r--r--   0 jhiller    (501) staff       (20)    29563 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/README.md
+-rw-r--r--   0 jhiller    (501) staff       (20)       38 2023-07-14 05:23:17.866388 crowdstrike-falconpy-1.3.0.dev6/setup.cfg
+-rw-r--r--   0 jhiller    (501) staff       (20)     4482 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/setup.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.731333 crowdstrike-falconpy-1.3.0.dev6/src/
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.739563 crowdstrike-falconpy-1.3.0.dev6/src/crowdstrike_falconpy.egg-info/
+-rw-r--r--   0 jhiller    (501) staff       (20)    31332 2023-07-14 05:23:17.000000 crowdstrike-falconpy-1.3.0.dev6/src/crowdstrike_falconpy.egg-info/PKG-INFO
+-rw-r--r--   0 jhiller    (501) staff       (20)     7615 2023-07-14 05:23:17.000000 crowdstrike-falconpy-1.3.0.dev6/src/crowdstrike_falconpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)        1 2023-07-14 05:23:17.000000 crowdstrike-falconpy-1.3.0.dev6/src/crowdstrike_falconpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)       83 2023-07-14 05:23:17.000000 crowdstrike-falconpy-1.3.0.dev6/src/crowdstrike_falconpy.egg-info/requires.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)        9 2023-07-14 05:23:17.000000 crowdstrike-falconpy-1.3.0.dev6/src/crowdstrike_falconpy.egg-info/top_level.txt
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.790126 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/
+-rw-r--r--   0 jhiller    (501) staff       (20)    12107 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/__init__.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.792991 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2095 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11250 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5561 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request_behavior.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5022 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request_connection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3788 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request_meta.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5358 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request_payloads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3827 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request_validator.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.795408 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2047 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4234 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/_base_falcon_auth.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5998 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/_bearer_token.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20647 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/_falcon_interface.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4806 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/_interface_config.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8624 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/_uber_interface.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.795853 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_constant/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2905 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_constant/__init__.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.825029 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/
+-rw-r--r--   0 jhiller    (501) staff       (20)     9054 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7042 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6740 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    30329 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13488 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15447 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6446 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10667 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_device_control_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3167 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_event_streams.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12391 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_falcon_complete_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6172 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_falcon_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14991 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_falconx_sandbox.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3694 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23292 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10008 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_firewall_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9015 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10381 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8008 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6237 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    22179 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_intel.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4594 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_ioa_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11784 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13556 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15790 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_kubernetes_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5803 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7033 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4457 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_ml_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2377 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_mobile_enrollment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20286 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3611 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_oauth2.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12950 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3569 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_overwatch_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9960 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_prevention_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4808 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_quarantine.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4165 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_quick_scan.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    24729 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16057 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17960 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9918 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_response_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11674 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5275 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_sensor_download.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15927 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_sensor_update_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4678 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_sensor_visibility_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4667 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_spotlight_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7134 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_spotlight_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4885 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_tailored_intelligence.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16463 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_user_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6050 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.837529 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4611 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13207 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5506 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17702 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3316 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5947 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11312 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2177 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13181 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13678 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13342 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1945 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.839349 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_enum/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1871 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_enum/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2124 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_enum/_base_url.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2063 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_enum/_container_base_url.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2218 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_enum/_token_fail_reason.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.840602 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_error/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2662 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_error/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6071 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_error/_exceptions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3573 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_error/_warnings.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.841471 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_log/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1744 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_log/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3809 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_log/_facility.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.854849 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/
+-rw-r--r--   0 jhiller    (501) staff       (20)     5516 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2691 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3624 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5855 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6079 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4604 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2790 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6181 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_device_control_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3666 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_falconx.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16333 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_firewall.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7329 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_generic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4290 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4511 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5808 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7508 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5577 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3774 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2866 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4506 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3118 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_prevention_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4309 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8001 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2615 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_response_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2433 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4519 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_sensor_update_policy.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.861074 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4540 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/__base_resource.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2186 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4581 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_base_dictionary.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1825 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_errors.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2684 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_expanded_result.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_headers.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3298 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_meta.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2489 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_resources.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4561 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_response_component.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16548 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_result.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.863063 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_service_class/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1827 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_service_class/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12272 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_service_class/_base_service_class.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11426 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_service_class/_service_class.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:23:17.865290 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_util/
+-rw-r--r--   0 jhiller    (501) staff       (20)     3087 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_util/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3076 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_util/_auth.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    33929 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_util/_functions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6161 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_util/_uber.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3539 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_version.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17508 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9970 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/api_complete.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15947 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    48601 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    34208 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    27069 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10750 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/debug.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15759 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    29552 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/device_control_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    22218 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5973 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/event_streams.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    37615 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/falcon_complete_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16270 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/falcon_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    28300 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/falconx_sandbox.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8668 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5384 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    79369 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20174 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/firewall_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    18869 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    27450 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4578 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13758 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13613 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    34693 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/intel.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10663 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/ioa_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    35840 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14032 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    25074 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/kubernetes_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16367 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23565 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10056 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/ml_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5166 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/mobile_enrollment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    43338 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8919 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/oauth2.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    35443 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13881 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/overwatch_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20718 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/prevention_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14372 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/quarantine.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9493 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/quick_scan.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    43159 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    25250 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    45859 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7687 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    19891 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/response_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    21891 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6764 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10169 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/sensor_download.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    38364 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/sensor_update_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9899 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/sensor_visibility_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8333 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/spotlight_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10652 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/spotlight_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9791 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/tailored_intelligence.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    39321 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/user_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8311 2023-07-14 05:23:16.000000 crowdstrike-falconpy-1.3.0.dev6/src/falconpy/zero_trust_assessment.py
```

### Comparing `crowdstrike-falconpy-1.3.0.dev5/AUTHORS.md` & `crowdstrike-falconpy-1.3.0.dev6/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/LICENSE` & `crowdstrike-falconpy-1.3.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/PKG-INFO` & `crowdstrike-falconpy-1.3.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy
-Version: 1.3.0.dev5
+Version: 1.3.0.dev6
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
```

### Comparing `crowdstrike-falconpy-1.3.0.dev5/README.md` & `crowdstrike-falconpy-1.3.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/setup.py` & `crowdstrike-falconpy-1.3.0.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/crowdstrike_falconpy.egg-info/PKG-INFO` & `crowdstrike-falconpy-1.3.0.dev6/src/crowdstrike_falconpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy
-Version: 1.3.0.dev5
+Version: 1.3.0.dev6
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
```

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/crowdstrike_falconpy.egg-info/SOURCES.txt` & `crowdstrike-falconpy-1.3.0.dev6/src/crowdstrike_falconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,16 @@
     TokenNotSpecified,
     KeywordsOnly,
     CannotRevokeToken,
     FunctionalityNotImplemented,
     InvalidBaseURL,
     PayloadValidationError,
     NoAuthenticationMechanism,
-    InvalidIndex
+    InvalidIndex,
+    InvalidCredentialFormat
     )
 from ._result import (
     Result,
     ExpandedResult,
     BaseDictionary,
     BaseResource,
     Resources,
@@ -165,15 +166,15 @@
     "TokenNotSpecified", "KeywordsOnly", "ALLOWED_METHODS", "USER_AGENT", "APIRequest",
     "ExpandedResult", "CannotRevokeToken", "Headers", "Meta", "Resources",
     "ResponseComponent", "BaseDictionary", "Errors", "BaseResource", "RawBody", "BinaryFile",
     "FunctionalityNotImplemented", "BearerToken", "LogFacility", "InvalidBaseURL",
     "InterfaceConfiguration", "RequestBehavior", "RequestConnection", "RequestMeta",
     "RequestPayloads", "RequestValidator", "PayloadValidationError", "MIN_TOKEN_RENEW_WINDOW",
     "MAX_TOKEN_RENEW_WINDOW", "GLOBAL_API_MAX_RETURN", "MOCK_OPERATIONS",
-    "NoAuthenticationMechanism", "InvalidIndex", "version"
+    "NoAuthenticationMechanism", "InvalidIndex", "version", "InvalidCredentialFormat"
     ]
 """
 This is free and unencumbered software released into the public domain.
 
 Anyone is free to copy, modify, publish, use, compile, sell, or
 distribute this software, either in source code form or as a compiled
 binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request_behavior.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request_behavior.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request_connection.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request_connection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request_meta.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request_meta.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request_payloads.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request_payloads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_api_request/_request_validator.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_api_request/_request_validator.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/_base_falcon_auth.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/_base_falcon_auth.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/_bearer_token.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/_bearer_token.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/_falcon_interface.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/_falcon_interface.py`

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
@@ -51,15 +56,15 @@
 from .._util import (
     autodiscover_region,
     perform_request,
     log_class_startup,
     login_payloads,
     logout_payloads
     )
-from .._error import InvalidCredentials, NoAuthenticationMechanism
+from .._error import InvalidCredentials, NoAuthenticationMechanism, InvalidCredentialFormat
 
 
 # pylint: disable=R0902
 class FalconInterface(BaseFalconAuth):
     """Standard Falcon API interface used by Service Classes."""
 
     # ____ ___ ___ ____ _ ___  _  _ ___ ____ ____
@@ -85,15 +90,15 @@
 
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
@@ -130,15 +135,24 @@
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
```

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/_interface_config.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/_interface_config.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_auth_object/_uber_interface.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_auth_object/_uber_interface.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_constant/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_constant/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_alerts.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_cloud_connect_aws.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_cspm_registration.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_custom_ioa.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_d4c_registration.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_detects.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_device_control_policies.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_device_control_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_discover.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_event_streams.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_falcon_complete_dashboard.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_falcon_container.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_falcon_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_falconx_sandbox.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_falconx_sandbox.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_fdr.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_filevantage.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_filevantage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_firewall_management.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_firewall_policies.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_host_group.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_hosts.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_identity_protection.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_incidents.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_installation_tokens.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_intel.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_ioa_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_ioc.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_iocs.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_kubernetes_protection.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_kubernetes_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_malquery.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_message_center.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_ml_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_mobile_enrollment.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_mssp.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_oauth2.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_oauth2.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_ods.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_overwatch_dashboard.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_prevention_policies.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_prevention_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_quarantine.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_quick_scan.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_real_time_response.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_real_time_response_admin.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_recon.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_report_executions.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_response_policies.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_sample_uploads.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_scheduled_reports.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_sensor_download.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_sensor_update_policies.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_sensor_update_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_sensor_visibility_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_spotlight_evaluation_logic.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_spotlight_vulnerabilities.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_tailored_intelligence.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_user_management.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_user_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/_zero_trust_assessment.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/_zero_trust_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_custom_ioa.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_d4c_registration.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_discover.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_fdr.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_firewall_management.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_hosts.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_identity_protection.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_installation_tokens.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_ioc.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_iocs.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_ods.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_real_time_response.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_report_executions.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_scheduled_reports.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_endpoint/deprecated/_zero_trust_assessment.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_endpoint/deprecated/_zero_trust_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_enum/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_enum/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_enum/_base_url.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_enum/_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_enum/_container_base_url.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_enum/_container_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_enum/_token_fail_reason.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_enum/_token_fail_reason.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_error/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_error/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,24 +45,25 @@
     InvalidCredentials,
     APIError,
     CannotRevokeToken,
     FunctionalityNotImplemented,
     InvalidBaseURL,
     PayloadValidationError,
     FeatureNotSupportedByPythonVersion,
-    InvalidIndex
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
            "NoAuthenticationMechanism", "FeatureNotSupportedByPythonVersion",
-           "InvalidIndex"
+           "InvalidIndex", "InvalidCredentialFormat"
            ]
```

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_error/_exceptions.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_error/_exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -170,7 +170,13 @@
     _message = "An unexpected error has occurred. Please check your payloads and try again."
 
 
 class InvalidIndex(SDKError):
     """Item ID was not found in the list or string."""
 
     _message = "Item not found. Check your index and try again."
+
+
+class InvalidCredentialFormat(SDKError):
+    """Credentials dictionary was provided as a datatype that will not convert to a dictionary."""
+
+    _message = "Invalid credential format. This keyword must be provided as a dictionary."
```

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_error/_warnings.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_error/_warnings.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_log/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_log/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_log/_facility.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_log/_facility.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_alerts.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_cloud_connect_aws.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_container.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_cspm_registration.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_d4c_registration.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_detects.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_device_control_policy.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_device_control_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_falconx.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_falconx.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_firewall.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_firewall.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_generic.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_generic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_host_group.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_incidents.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_ioa.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_ioc.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_malquery.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_message_center.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_mssp.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_ods.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_prevention_policy.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_real_time_response.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_recon.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_reports.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_response_policy.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_response_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_sample_uploads.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_payload/_sensor_update_policy.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_payload/_sensor_update_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/__base_resource.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/__base_resource.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_base_dictionary.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_base_dictionary.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_errors.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_errors.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_expanded_result.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_expanded_result.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_headers.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_headers.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_meta.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_meta.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_resources.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_resources.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_response_component.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_response_component.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_result/_result.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_result/_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,26 +93,31 @@
             elif body.get("access_token", None):
                 # Authentication response
                 self.raw = RawBody(body)
                 self.meta = Meta()
                 self.resources = Resources()
                 self.errors = Errors()
             else:
-                # Standard responses and RTR
+                # Standard responses, GraphQL and RTR
                 self.meta = Meta(body.get("meta", {}))
                 self.errors = Errors(body.get("errors", []))
                 # RTR Batch responses
                 if body.get("batch_id", {}):
                     # Batch session init
                     self.raw = RawBody(body)
                     self.resources = Resources(body.get("resources", []))
                 elif body.get("combined", {}):
                     # Batch session results have to be handled as RawBody
                     # due to the combined response format.
                     self.raw = RawBody(body)
+                elif body.get("data", {}):  # pragma: no cover
+                    # GraphQL uses a custom response payload, we will
+                    # use RawBody for this return for now. Due to
+                    # environment constraints, this is manually tested.
+                    self.raw = RawBody(body)
                 else:
                     # Standard API responses
                     self.resources = Resources(body.get("resources", []))
 
     # Iteration handlers
     def __iter__(self):
         """Return this object for iteration handling."""
```

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_service_class/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_service_class/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_service_class/_base_service_class.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_service_class/_base_service_class.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_service_class/_service_class.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_service_class/_service_class.py`

 * *Files 2% similar despite different names*

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
```

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_util/__init__.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_util/_auth.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_util/_auth.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_util/_functions.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_util/_functions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_util/_uber.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_util/_uber.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/_version.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-_VERSION = '1.3.0.dev5'
+_VERSION = '1.3.0.dev6'
 _MAINTAINER = 'Joshua Hiller'
 _AUTHOR = 'CrowdStrike'
 _AUTHOR_EMAIL = 'falconpy@crowdstrike.com'
 _CREDITS = 'CrowdStrike'
 _DESCRIPTION = "The CrowdStrike Falcon SDK for Python 3"
 _TITLE = "crowdstrike-falconpy"
 _PROJECT_URL = "https://github.com/CrowdStrike/falconpy"
```

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/alerts.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/api_complete.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/api_complete.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/cloud_connect_aws.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/cspm_registration.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/custom_ioa.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/d4c_registration.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/debug.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/debug.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/detects.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/device_control_policies.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/device_control_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/discover.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/event_streams.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/falcon_complete_dashboard.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/falcon_container.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/falcon_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/falconx_sandbox.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/falconx_sandbox.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/fdr.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/filevantage.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/filevantage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/firewall_management.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/firewall_policies.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/host_group.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/hosts.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/identity_protection.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/incidents.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/installation_tokens.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/intel.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/ioa_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/ioc.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/iocs.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/kubernetes_protection.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/kubernetes_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/malquery.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/message_center.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/ml_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/mobile_enrollment.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/mssp.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/oauth2.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/oauth2.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/ods.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/overwatch_dashboard.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/prevention_policy.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/quarantine.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/quick_scan.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/real_time_response.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/real_time_response_admin.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/recon.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/report_executions.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/response_policies.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/sample_uploads.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/scheduled_reports.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/sensor_download.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/sensor_update_policy.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/sensor_update_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/sensor_visibility_exclusions.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/spotlight_evaluation_logic.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/spotlight_vulnerabilities.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/tailored_intelligence.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/user_management.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/user_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.3.0.dev5/src/falconpy/zero_trust_assessment.py` & `crowdstrike-falconpy-1.3.0.dev6/src/falconpy/zero_trust_assessment.py`

 * *Files identical despite different names*

