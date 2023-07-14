# Comparing `tmp/satosacontrib.perun-3.7.0.tar.gz` & `tmp/satosacontrib.perun-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satosacontrib.perun-3.7.0.tar", last modified: Tue Jul 11 10:33:43 2023, max compression
+gzip compressed data, was "satosacontrib.perun-3.7.1.tar", last modified: Fri Jul 14 20:37:02 2023, max compression
```

## Comparing `satosacontrib.perun-3.7.0.tar` & `satosacontrib.perun-3.7.1.tar`

### file list

```diff
@@ -1,65 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:33:43.657535 satosacontrib.perun-3.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4897 2023-07-11 10:33:43.657535 satosacontrib.perun-3.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3902 2023-07-11 10:25:54.000000 satosacontrib.perun-3.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:33:43.653535 satosacontrib.perun-3.7.0/satosacontrib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:33:43.653535 satosacontrib.perun-3.7.0/satosacontrib/perun/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:33:43.653535 satosacontrib.perun-3.7.0/satosacontrib/perun/backends/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-11 10:25:55.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/backends/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10089 2023-07-11 10:25:55.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/backends/seznam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:33:43.653535 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/
--rw-rw-rw-   0 root         (0) root         (0)      727 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-11 10:25:55.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/auth_switcher_lite.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/compute_eligibility.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2023-07-07 14:33:28.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/context_attributes_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:33:43.653535 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8313 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/additional_identifiers.py
--rw-rw-rw-   0 root         (0) root         (0)     5927 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    11822 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     4831 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/perun_user.py
--rw-rw-rw-   0 root         (0) root         (0)    24791 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/sp_authorization.py
--rw-rw-rw-   0 root         (0) root         (0)    11491 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/is_banned_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     1200 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2023-07-04 07:23:14.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2122 2023-07-04 08:38:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/session_started_with_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:33:43.653535 satosacontrib.perun-3.7.0/satosacontrib/perun/utils/
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/utils/ConfigStore.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/utils/CurlConnector.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/utils/CurlConnectorInterface.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/utils/PerunConstants.py
--rw-rw-rw-   0 root         (0) root         (0)     6719 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/utils/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/satosacontrib/perun/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:33:43.653535 satosacontrib.perun-3.7.0/satosacontrib.perun.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4897 2023-07-11 10:33:43.000000 satosacontrib.perun-3.7.0/satosacontrib.perun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2490 2023-07-11 10:33:43.000000 satosacontrib.perun-3.7.0/satosacontrib.perun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 10:33:43.000000 satosacontrib.perun-3.7.0/satosacontrib.perun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-11 10:33:43.000000 satosacontrib.perun-3.7.0/satosacontrib.perun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-11 10:33:43.000000 satosacontrib.perun-3.7.0/satosacontrib.perun.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-11 10:33:43.657535 satosacontrib.perun-3.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-11 08:56:08.000000 satosacontrib.perun-3.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:33:43.657535 satosacontrib.perun-3.7.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10917 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/test_additional_indentifiers.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/test_auth_event_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     3329 2023-07-07 14:33:28.000000 satosacontrib.perun-3.7.0/tests/test_context_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/test_is_banned.py
--rw-rw-rw-   0 root         (0) root         (0)     7500 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/test_is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2535 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/test_microservice_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     3981 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/test_perun_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    14517 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/test_perun_ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)     7117 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/test_perun_entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     5482 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/test_perun_user_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)    36568 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/test_sp_authorization_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     7291 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.0/tests/test_update_ues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:37:02.270828 satosacontrib.perun-3.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4897 2023-07-14 20:37:02.270828 satosacontrib.perun-3.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3902 2023-07-11 10:25:54.000000 satosacontrib.perun-3.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:37:02.266828 satosacontrib.perun-3.7.1/satosacontrib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:37:02.266828 satosacontrib.perun-3.7.1/satosacontrib/perun/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:37:02.266828 satosacontrib.perun-3.7.1/satosacontrib/perun/addons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 20:25:20.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/addons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/addons/extended_introspection_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:37:02.266828 satosacontrib.perun-3.7.1/satosacontrib/perun/backends/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-11 10:25:55.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/backends/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10129 2023-07-14 20:28:21.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/backends/seznam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:37:02.266828 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/attribute_typing_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-11 10:25:55.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/auth_switcher_lite.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/cardinality_single_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/compute_eligibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2023-07-07 14:33:28.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/context_attributes_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:37:02.270828 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8313 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/additional_identifiers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5927 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11822 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    11583 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     4831 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/perun_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    24791 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/sp_authorization.py
+-rw-rw-rw-   0 root         (0) root         (0)    11491 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/is_banned_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/multi_idphint_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2023-07-04 07:23:14.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/proxystatistics_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2122 2023-07-04 08:38:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/session_started_with_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:37:02.270828 satosacontrib.perun-3.7.1/satosacontrib/perun/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/utils/ConfigStore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/utils/CurlConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/utils/CurlConnectorInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/utils/PerunConstants.py
+-rw-rw-rw-   0 root         (0) root         (0)     6719 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/utils/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/satosacontrib/perun/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:37:02.266828 satosacontrib.perun-3.7.1/satosacontrib.perun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4897 2023-07-14 20:37:02.000000 satosacontrib.perun-3.7.1/satosacontrib.perun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-07-14 20:37:02.000000 satosacontrib.perun-3.7.1/satosacontrib.perun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 20:37:02.000000 satosacontrib.perun-3.7.1/satosacontrib.perun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-14 20:37:02.000000 satosacontrib.perun-3.7.1/satosacontrib.perun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-14 20:37:02.000000 satosacontrib.perun-3.7.1/satosacontrib.perun.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-14 20:37:02.270828 satosacontrib.perun-3.7.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-14 20:25:20.000000 satosacontrib.perun-3.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:37:02.270828 satosacontrib.perun-3.7.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10917 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/test_additional_indentifiers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/test_auth_event_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     3329 2023-07-07 14:33:28.000000 satosacontrib.perun-3.7.1/tests/test_context_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/test_is_banned.py
+-rw-rw-rw-   0 root         (0) root         (0)     7500 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/test_is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/test_microservice_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/test_perun_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14517 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/test_perun_ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)     7117 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/test_perun_entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     5482 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/test_perun_user_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)    36568 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/test_sp_authorization_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.1/tests/test_update_ues.py
```

### Comparing `satosacontrib.perun-3.7.0/LICENSE` & `satosacontrib.perun-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/PKG-INFO` & `satosacontrib.perun-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosacontrib.perun
-Version: 3.7.0
+Version: 3.7.1
 Summary: Microservices for SATOSA authentication proxy, made by the Perun team
 Home-page: https://github.com/CESNET/satosacontrib.perun.git
 License: UNKNOWN
 Description: # satosacontrib.perun
         
         Microservices for [SATOSA](https://github.com/IdentityPython/SATOSA) authentication
         proxy, made by the Perun team.
```

### Comparing `satosacontrib.perun-3.7.0/README.md` & `satosacontrib.perun-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/backends/seznam.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/backends/seznam.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from oic.oic.message import RegistrationRequest
 from oic.utils.authn.authn_context import UNSPECIFIED
 from oic.utils.authn.client import CLIENT_AUTHN_METHOD
 
 import satosa.logging_util as lu
 from satosa.internal import AuthenticationInformation
 from satosa.internal import InternalData
-from .base import BackendModule
-from .oauth import get_metadata_desc_for_oauth_backend
-from ..exception import SATOSAAuthenticationError, SATOSAError
-from ..response import Redirect
+from satosa.backends.base import BackendModule
+from satosa.backends.oauth import get_metadata_desc_for_oauth_backend
+from satosa.exception import SATOSAAuthenticationError, SATOSAError
+from satosa.response import Redirect
 
 
 logger = logging.getLogger(__name__)
 
 STATE_KEY = "oidc_state"
```

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/__init__.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/__init__.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/attribute_typing_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/auth_event_logging_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/auth_switcher_lite.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/auth_switcher_lite.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/cardinality_single_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/compute_eligibility.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/compute_eligibility.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/context_attributes_microservice.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/context_attributes_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/additional_identifiers.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/additional_identifiers.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/attributes.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/ensure_member.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/entitlement.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/entitlement.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/perun_user.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/perun_user.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/sp_authorization.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/sp_authorization.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/idm/update_user_ext_source.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/is_banned_microservice.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/is_banned_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/is_eligible_microservice.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/multi_idphint_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/nameid_attribute_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/proxystatistics_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/micro_services/session_started_with_microservice.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/micro_services/session_started_with_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/utils/AuthEventLoggingDbModels.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/utils/ConfigStore.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/utils/CurlConnector.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/utils/CurlConnector.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/utils/CurlConnectorInterface.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/utils/CurlConnectorInterface.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib/perun/utils/Utils.py` & `satosacontrib.perun-3.7.1/satosacontrib/perun/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/satosacontrib.perun.egg-info/PKG-INFO` & `satosacontrib.perun-3.7.1/satosacontrib.perun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosacontrib.perun
-Version: 3.7.0
+Version: 3.7.1
 Summary: Microservices for SATOSA authentication proxy, made by the Perun team
 Home-page: https://github.com/CESNET/satosacontrib.perun.git
 License: UNKNOWN
 Description: # satosacontrib.perun
         
         Microservices for [SATOSA](https://github.com/IdentityPython/SATOSA) authentication
         proxy, made by the Perun team.
```

### Comparing `satosacontrib.perun-3.7.0/satosacontrib.perun.egg-info/SOURCES.txt` & `satosacontrib.perun-3.7.1/satosacontrib.perun.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 satosacontrib/__init__.py
 satosacontrib.perun.egg-info/PKG-INFO
 satosacontrib.perun.egg-info/SOURCES.txt
 satosacontrib.perun.egg-info/dependency_links.txt
 satosacontrib.perun.egg-info/requires.txt
 satosacontrib.perun.egg-info/top_level.txt
 satosacontrib/perun/__init__.py
+satosacontrib/perun/addons/__init__.py
+satosacontrib/perun/addons/extended_introspection_response.py
 satosacontrib/perun/backends/__init__.py
 satosacontrib/perun/backends/seznam.py
 satosacontrib/perun/micro_services/__init__.py
 satosacontrib/perun/micro_services/attribute_typing_microservice.py
 satosacontrib/perun/micro_services/auth_event_logging_microservice.py
 satosacontrib/perun/micro_services/auth_switcher_lite.py
 satosacontrib/perun/micro_services/cardinality_single_microservice.py
```

### Comparing `satosacontrib.perun-3.7.0/setup.py` & `satosacontrib.perun-3.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_additional_indentifiers.py` & `satosacontrib.perun-3.7.1/tests/test_additional_indentifiers.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_auth_event_logging.py` & `satosacontrib.perun-3.7.1/tests/test_auth_event_logging.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_context_attributes.py` & `satosacontrib.perun-3.7.1/tests/test_context_attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_is_banned.py` & `satosacontrib.perun-3.7.1/tests/test_is_banned.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_is_eligible_microservice.py` & `satosacontrib.perun-3.7.1/tests/test_is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_microservice_loader.py` & `satosacontrib.perun-3.7.1/tests/test_microservice_loader.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_perun_attributes.py` & `satosacontrib.perun-3.7.1/tests/test_perun_attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_perun_ensure_member.py` & `satosacontrib.perun-3.7.1/tests/test_perun_ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_perun_entitlement.py` & `satosacontrib.perun-3.7.1/tests/test_perun_entitlement.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_perun_user_microservice.py` & `satosacontrib.perun-3.7.1/tests/test_perun_user_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_sp_authorization_microservice.py` & `satosacontrib.perun-3.7.1/tests/test_sp_authorization_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.0/tests/test_update_ues.py` & `satosacontrib.perun-3.7.1/tests/test_update_ues.py`

 * *Files identical despite different names*

