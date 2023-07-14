# Comparing `tmp/ipfabric-6.2.5.tar.gz` & `tmp/ipfabric-6.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric-6.2.5.tar", max compression
+gzip compressed data, was "ipfabric-6.3.0b0.tar", max compression
```

## Comparing `ipfabric-6.2.5.tar` & `ipfabric-6.3.0b0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1790 2023-05-02 13:05:28.009049 ipfabric-6.2.5/ipfabric/__init__.py
--rw-r--r--   0        0        0    17412 2023-06-01 16:01:19.082057 ipfabric-6.2.5/ipfabric/api.py
--rw-r--r--   0        0        0    10890 2023-06-01 16:01:19.085671 ipfabric-6.2.5/ipfabric/client.py
--rw-r--r--   0        0        0      434 2023-06-01 16:01:19.090676 ipfabric-6.2.5/ipfabric/models/__init__.py
--rw-r--r--   0        0        0    14821 2023-06-29 11:39:54.725144 ipfabric-6.2.5/ipfabric/models/device.py
--rw-r--r--   0        0        0     5842 2023-06-01 16:01:19.099648 ipfabric-6.2.5/ipfabric/models/intent.py
--rw-r--r--   0        0        0     2786 2023-04-24 14:44:33.818272 ipfabric-6.2.5/ipfabric/models/intent_check.py
--rw-r--r--   0        0        0     2092 2023-06-01 16:01:19.103555 ipfabric-6.2.5/ipfabric/models/inventory.py
--rw-r--r--   0        0        0     6964 2023-06-01 16:01:19.107556 ipfabric-6.2.5/ipfabric/models/jobs.py
--rw-r--r--   0        0        0    12327 2023-06-01 16:01:19.111651 ipfabric-6.2.5/ipfabric/models/snapshot.py
--rw-r--r--   0        0        0    19772 2023-06-29 11:39:54.726143 ipfabric-6.2.5/ipfabric/models/table.py
--rw-r--r--   0        0        0     2830 2023-04-24 14:44:33.820322 ipfabric-6.2.5/ipfabric/models/technology/__init__.py
--rw-r--r--   0        0        0     1156 2023-04-24 14:44:33.821325 ipfabric-6.2.5/ipfabric/models/technology/addressing.py
--rw-r--r--   0        0        0      488 2023-04-24 14:44:33.821325 ipfabric-6.2.5/ipfabric/models/technology/cloud.py
--rw-r--r--   0        0        0     2173 2023-04-24 14:44:33.821325 ipfabric-6.2.5/ipfabric/models/technology/dhcp.py
--rw-r--r--   0        0        0     1002 2023-04-24 14:44:33.821325 ipfabric-6.2.5/ipfabric/models/technology/fhrp.py
--rw-r--r--   0        0        0     7018 2023-04-24 14:44:33.822322 ipfabric-6.2.5/ipfabric/models/technology/interfaces.py
--rw-r--r--   0        0        0      324 2023-04-24 14:44:33.822322 ipfabric-6.2.5/ipfabric/models/technology/ip_telephony.py
--rw-r--r--   0        0        0      843 2023-04-24 14:44:33.822322 ipfabric-6.2.5/ipfabric/models/technology/load_balancing.py
--rw-r--r--   0        0        0      470 2023-04-24 14:44:33.823320 ipfabric-6.2.5/ipfabric/models/technology/managed_networks.py
--rw-r--r--   0        0        0     5644 2023-04-24 14:44:33.823320 ipfabric-6.2.5/ipfabric/models/technology/management.py
--rw-r--r--   0        0        0     2045 2023-04-24 14:44:33.823320 ipfabric-6.2.5/ipfabric/models/technology/mpls.py
--rw-r--r--   0        0        0     2783 2023-04-24 14:44:33.824322 ipfabric-6.2.5/ipfabric/models/technology/multicast.py
--rw-r--r--   0        0        0      759 2023-04-24 14:44:33.824322 ipfabric-6.2.5/ipfabric/models/technology/neighbors.py
--rw-r--r--   0        0        0      633 2023-04-24 14:44:33.825321 ipfabric-6.2.5/ipfabric/models/technology/oam.py
--rw-r--r--   0        0        0     3529 2023-04-24 14:44:33.825321 ipfabric-6.2.5/ipfabric/models/technology/platforms.py
--rw-r--r--   0        0        0     1231 2023-04-24 14:44:33.826320 ipfabric-6.2.5/ipfabric/models/technology/port_channels.py
--rw-r--r--   0        0        0     1078 2023-04-24 14:44:33.826320 ipfabric-6.2.5/ipfabric/models/technology/qos.py
--rw-r--r--   0        0        0     4773 2023-04-24 14:44:33.827321 ipfabric-6.2.5/ipfabric/models/technology/routing.py
--rw-r--r--   0        0        0     2159 2023-04-24 14:44:33.827321 ipfabric-6.2.5/ipfabric/models/technology/sdn.py
--rw-r--r--   0        0        0      431 2023-04-24 14:44:33.827321 ipfabric-6.2.5/ipfabric/models/technology/sdwan.py
--rw-r--r--   0        0        0     2062 2023-04-24 14:44:33.828325 ipfabric-6.2.5/ipfabric/models/technology/security.py
--rw-r--r--   0        0        0     2228 2023-04-24 14:44:33.828325 ipfabric-6.2.5/ipfabric/models/technology/stp.py
--rw-r--r--   0        0        0      856 2023-04-24 14:44:33.829324 ipfabric-6.2.5/ipfabric/models/technology/vlans.py
--rw-r--r--   0        0        0      867 2023-04-24 14:44:33.829324 ipfabric-6.2.5/ipfabric/models/technology/wireless.py
--rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.2.5/ipfabric/settings/__init__.py
--rw-r--r--   0        0        0     3602 2023-05-31 13:43:53.851771 ipfabric-6.2.5/ipfabric/settings/api_tokens.py
--rw-r--r--   0        0        0     6187 2023-04-24 14:44:33.840110 ipfabric-6.2.5/ipfabric/settings/attributes.py
--rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.2.5/ipfabric/settings/authentication.py
--rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.2.5/ipfabric/settings/discovery.py
--rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.2.5/ipfabric/settings/seeds.py
--rw-r--r--   0        0        0     1413 2023-04-24 14:44:33.844128 ipfabric-6.2.5/ipfabric/settings/site_separation.py
--rw-r--r--   0        0        0     5247 2023-05-31 13:43:53.858770 ipfabric-6.2.5/ipfabric/settings/user_mgmt.py
--rw-r--r--   0        0        0     1875 2023-04-24 14:44:33.866077 ipfabric-6.2.5/ipfabric/settings/vendor_api.py
--rw-r--r--   0        0        0     6439 2023-04-24 14:44:33.870769 ipfabric-6.2.5/ipfabric/settings/vendor_api_models.py
--rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.2.5/ipfabric/tools/__init__.py
--rw-r--r--   0        0        0     7876 2023-04-24 14:44:33.876769 ipfabric-6.2.5/ipfabric/tools/configuration.py
--rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.2.5/ipfabric/tools/discovery_history.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.5/ipfabric/tools/factory_defaults/__init__.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/__init__.py
--rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/dashboard.json
--rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/groups.json
--rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/__init__.py
--rw-r--r--   0        0        0     4511 2023-04-24 14:44:33.881459 ipfabric-6.2.5/ipfabric/tools/nist.py
--rw-r--r--   0        0        0     5784 2023-04-24 14:44:33.886456 ipfabric-6.2.5/ipfabric/tools/restore_intents.py
--rw-r--r--   0        0        0     2519 2023-04-24 14:44:33.891098 ipfabric-6.2.5/ipfabric/tools/shared.py
--rw-r--r--   0        0        0     2396 2023-04-24 14:44:33.895102 ipfabric-6.2.5/ipfabric/tools/site_seperation_report.py
--rw-r--r--   0        0        0     2573 2023-04-24 14:44:33.902766 ipfabric-6.2.5/ipfabric/tools/vulnerabilities.py
--rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.2.5/LICENSE
--rw-r--r--   0        0        0     2054 2023-06-29 11:42:31.639411 ipfabric-6.2.5/pyproject.toml
--rw-r--r--   0        0        0     3705 2023-04-24 14:44:33.756295 ipfabric-6.2.5/README.md
--rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 ipfabric-6.2.5/setup.py
--rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 ipfabric-6.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1790 2023-05-02 13:05:28.009049 ipfabric-6.3.0b0/ipfabric/__init__.py
+-rw-r--r--   0        0        0    17412 2023-07-13 12:33:49.961785 ipfabric-6.3.0b0/ipfabric/api.py
+-rw-r--r--   0        0        0    11597 2023-07-14 16:09:22.706505 ipfabric-6.3.0b0/ipfabric/client.py
+-rw-r--r--   0        0        0      434 2023-06-01 16:01:19.090676 ipfabric-6.3.0b0/ipfabric/models/__init__.py
+-rw-r--r--   0        0        0    14821 2023-07-13 12:33:49.973872 ipfabric-6.3.0b0/ipfabric/models/device.py
+-rw-r--r--   0        0        0     5842 2023-06-01 16:01:19.099648 ipfabric-6.3.0b0/ipfabric/models/intent.py
+-rw-r--r--   0        0        0     2786 2023-04-24 14:44:33.818272 ipfabric-6.3.0b0/ipfabric/models/intent_check.py
+-rw-r--r--   0        0        0     2092 2023-06-01 16:01:19.103555 ipfabric-6.3.0b0/ipfabric/models/inventory.py
+-rw-r--r--   0        0        0     6964 2023-07-13 12:33:49.979894 ipfabric-6.3.0b0/ipfabric/models/jobs.py
+-rw-r--r--   0        0        0    12421 2023-07-13 12:33:49.985397 ipfabric-6.3.0b0/ipfabric/models/snapshot.py
+-rw-r--r--   0        0        0    21073 2023-07-14 16:09:22.773293 ipfabric-6.3.0b0/ipfabric/models/table.py
+-rw-r--r--   0        0        0     2830 2023-04-24 14:44:33.820322 ipfabric-6.3.0b0/ipfabric/models/technology/__init__.py
+-rw-r--r--   0        0        0     1156 2023-04-24 14:44:33.821325 ipfabric-6.3.0b0/ipfabric/models/technology/addressing.py
+-rw-r--r--   0        0        0      488 2023-04-24 14:44:33.821325 ipfabric-6.3.0b0/ipfabric/models/technology/cloud.py
+-rw-r--r--   0        0        0     2173 2023-04-24 14:44:33.821325 ipfabric-6.3.0b0/ipfabric/models/technology/dhcp.py
+-rw-r--r--   0        0        0     1002 2023-04-24 14:44:33.821325 ipfabric-6.3.0b0/ipfabric/models/technology/fhrp.py
+-rw-r--r--   0        0        0     7018 2023-04-24 14:44:33.822322 ipfabric-6.3.0b0/ipfabric/models/technology/interfaces.py
+-rw-r--r--   0        0        0      324 2023-04-24 14:44:33.822322 ipfabric-6.3.0b0/ipfabric/models/technology/ip_telephony.py
+-rw-r--r--   0        0        0      843 2023-04-24 14:44:33.822322 ipfabric-6.3.0b0/ipfabric/models/technology/load_balancing.py
+-rw-r--r--   0        0        0      470 2023-04-24 14:44:33.823320 ipfabric-6.3.0b0/ipfabric/models/technology/managed_networks.py
+-rw-r--r--   0        0        0     5644 2023-04-24 14:44:33.823320 ipfabric-6.3.0b0/ipfabric/models/technology/management.py
+-rw-r--r--   0        0        0     2045 2023-04-24 14:44:33.823320 ipfabric-6.3.0b0/ipfabric/models/technology/mpls.py
+-rw-r--r--   0        0        0     2783 2023-04-24 14:44:33.824322 ipfabric-6.3.0b0/ipfabric/models/technology/multicast.py
+-rw-r--r--   0        0        0      759 2023-04-24 14:44:33.824322 ipfabric-6.3.0b0/ipfabric/models/technology/neighbors.py
+-rw-r--r--   0        0        0      633 2023-04-24 14:44:33.825321 ipfabric-6.3.0b0/ipfabric/models/technology/oam.py
+-rw-r--r--   0        0        0     3529 2023-04-24 14:44:33.825321 ipfabric-6.3.0b0/ipfabric/models/technology/platforms.py
+-rw-r--r--   0        0        0     1231 2023-04-24 14:44:33.826320 ipfabric-6.3.0b0/ipfabric/models/technology/port_channels.py
+-rw-r--r--   0        0        0     1078 2023-04-24 14:44:33.826320 ipfabric-6.3.0b0/ipfabric/models/technology/qos.py
+-rw-r--r--   0        0        0     4773 2023-04-24 14:44:33.827321 ipfabric-6.3.0b0/ipfabric/models/technology/routing.py
+-rw-r--r--   0        0        0     2159 2023-04-24 14:44:33.827321 ipfabric-6.3.0b0/ipfabric/models/technology/sdn.py
+-rw-r--r--   0        0        0      431 2023-04-24 14:44:33.827321 ipfabric-6.3.0b0/ipfabric/models/technology/sdwan.py
+-rw-r--r--   0        0        0     2062 2023-04-24 14:44:33.828325 ipfabric-6.3.0b0/ipfabric/models/technology/security.py
+-rw-r--r--   0        0        0     2228 2023-04-24 14:44:33.828325 ipfabric-6.3.0b0/ipfabric/models/technology/stp.py
+-rw-r--r--   0        0        0      856 2023-04-24 14:44:33.829324 ipfabric-6.3.0b0/ipfabric/models/technology/vlans.py
+-rw-r--r--   0        0        0      867 2023-04-24 14:44:33.829324 ipfabric-6.3.0b0/ipfabric/models/technology/wireless.py
+-rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.3.0b0/ipfabric/settings/__init__.py
+-rw-r--r--   0        0        0     3342 2023-07-13 12:33:49.997188 ipfabric-6.3.0b0/ipfabric/settings/api_tokens.py
+-rw-r--r--   0        0        0     6187 2023-04-24 14:44:33.840110 ipfabric-6.3.0b0/ipfabric/settings/attributes.py
+-rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.3.0b0/ipfabric/settings/authentication.py
+-rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.3.0b0/ipfabric/settings/discovery.py
+-rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.3.0b0/ipfabric/settings/seeds.py
+-rw-r--r--   0        0        0     1413 2023-04-24 14:44:33.844128 ipfabric-6.3.0b0/ipfabric/settings/site_separation.py
+-rw-r--r--   0        0        0     5137 2023-07-13 12:33:50.002187 ipfabric-6.3.0b0/ipfabric/settings/user_mgmt.py
+-rw-r--r--   0        0        0     1875 2023-04-24 14:44:33.866077 ipfabric-6.3.0b0/ipfabric/settings/vendor_api.py
+-rw-r--r--   0        0        0     6439 2023-04-24 14:44:33.870769 ipfabric-6.3.0b0/ipfabric/settings/vendor_api_models.py
+-rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.3.0b0/ipfabric/tools/__init__.py
+-rw-r--r--   0        0        0     7876 2023-04-24 14:44:33.876769 ipfabric-6.3.0b0/ipfabric/tools/configuration.py
+-rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.3.0b0/ipfabric/tools/discovery_history.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v4/4/__init__.py
+-rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v4/4/dashboard.json
+-rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v4/4/groups.json
+-rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v4/4/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v4/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v5/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v5/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v5/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v5/0/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v5/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v6/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v6/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v6/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v6/0/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v6/__init__.py
+-rw-r--r--   0        0        0     4511 2023-04-24 14:44:33.881459 ipfabric-6.3.0b0/ipfabric/tools/nist.py
+-rw-r--r--   0        0        0     5784 2023-04-24 14:44:33.886456 ipfabric-6.3.0b0/ipfabric/tools/restore_intents.py
+-rw-r--r--   0        0        0     2519 2023-04-24 14:44:33.891098 ipfabric-6.3.0b0/ipfabric/tools/shared.py
+-rw-r--r--   0        0        0     2396 2023-04-24 14:44:33.895102 ipfabric-6.3.0b0/ipfabric/tools/site_seperation_report.py
+-rw-r--r--   0        0        0     2573 2023-04-24 14:44:33.902766 ipfabric-6.3.0b0/ipfabric/tools/vulnerabilities.py
+-rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.3.0b0/LICENSE
+-rw-r--r--   0        0        0     2054 2023-07-14 16:12:19.804192 ipfabric-6.3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     3705 2023-04-24 14:44:33.756295 ipfabric-6.3.0b0/README.md
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 ipfabric-6.3.0b0/setup.py
+-rw-r--r--   0        0        0     5194 1970-01-01 00:00:00.000000 ipfabric-6.3.0b0/PKG-INFO
```

### Comparing `ipfabric-6.2.5/ipfabric/__init__.py` & `ipfabric-6.3.0b0/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/api.py` & `ipfabric-6.3.0b0/ipfabric/api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/client.py` & `ipfabric-6.3.0b0/ipfabric/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,71 +128,83 @@
         limit: Optional[int] = 1000,
         start: Optional[int] = 0,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
         snapshot: bool = True,
-    ) -> List[dict]:
+        csv: bool = False,
+    ) -> Union[List[dict], bytes]:
         """Gets data from IP Fabric for specified endpoint
 
         Args:
             url: Example tables/vlan/device-summary
             columns: Optional list of columns to return, None will return all
             filters: Optional dictionary of filters
             limit: Default to 1,000 rows
             start: Starts at 0
             snapshot_id: Optional snapshot_id to override default
             reports: String of frontend URL where the reports are displayed or a list of report IDs
             sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
             attr_filters: Optional dictionary to apply an Attribute filter
             snapshot: Set to False for some tables like management endpoints.
-
+            csv: bool: Default False, returns bytes (string) if True.
         Returns:
-            list: List of Dictionary objects.
+            Union[List[dict], str]: List of Dictionaries or string if CSV
         """
         snapshot_id = snapshot_id or self.snapshot_id
         url, payload = self._check_url_payload(url, snapshot_id, snapshot, filters, reports, sort, attr_filters)
         payload["columns"] = columns or self.get_columns(url, snapshot=snapshot)
         payload["pagination"] = dict(start=start, limit=limit)
+        if csv:
+            payload["format"] = {"exportToFile": True, "dataType": "csv"}
         res = self.post(url, json=payload)
         res.raise_for_status()
-        return res.json()["data"]
+        return res.text if csv else res.json()["data"]
 
     def fetch_all(
         self,
         url: str,
         columns: Optional[List] = None,
         filters: Optional[Union[dict, str]] = None,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
         snapshot: bool = True,
-    ) -> List[dict]:
+        csv: bool = False,
+    ) -> Union[List[dict], bytes]:
         """Gets all data from IP Fabric for specified endpoint
 
         Args:
             url: Example tables/vlan/device-summary
             columns: Optional list of columns to return, None will return all
             filters: Optional dictionary of filters
             snapshot_id: Optional snapshot_id to override default
             reports: String of frontend URL where the reports are displayed or a list of report IDs
             sort: Optional dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
             attr_filters: Optional dictionary to apply an Attribute filter
             snapshot: Set to False for some tables like management endpoints.
-
+            csv: bool: Default False, returns bytes (string) if True.
         Returns:
-            list: List of Dictionary objects.
+            Union[List[dict], str]: List of Dictionaries or string if CSV
         """
         snapshot_id = snapshot_id or self.snapshot_id
         url, payload = self._check_url_payload(url, snapshot_id, snapshot, filters, reports, sort, attr_filters)
         payload["columns"] = columns or self.get_columns(url, snapshot=snapshot)
+        if csv:
+            payload["format"] = {"exportToFile": True, "dataType": "csv"}
+            return self._csv_stream(url, payload)
         return self._ipf_pager(url, payload)
 
+    def _csv_stream(self, url, payload):
+        with self.stream("POST", url, json=payload) as stream_resp:
+            data = stream_resp.read()
+        return data
+
     def query(self, url: str, payload: Union[str, dict], get_all: bool = True) -> List[dict]:
         """Submits a query, does no formatting on the parameters.  Use for copy/pasting from the webpage.
 
         Args:
             url: Example: https://demo1.ipfabric.io/api/v1/tables/vlan/device-summary or tables/vlan/device-summary
             payload: Dictionary to submit in POST or can be JSON string (i.e. read from file).
             get_all: Default use pager to get all results and ignore pagination information in the payload
```

### Comparing `ipfabric-6.2.5/ipfabric/models/device.py` & `ipfabric-6.3.0b0/ipfabric/models/device.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/intent.py` & `ipfabric-6.3.0b0/ipfabric/models/intent.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/intent_check.py` & `ipfabric-6.3.0b0/ipfabric/models/intent_check.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/inventory.py` & `ipfabric-6.3.0b0/ipfabric/models/inventory.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/jobs.py` & `ipfabric-6.3.0b0/ipfabric/models/jobs.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/snapshot.py` & `ipfabric-6.3.0b0/ipfabric/models/snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pydantic import BaseModel, Field
 from .jobs import Jobs
 
 logger = logging.getLogger("ipfabric")
 
 SNAPSHOT_COLUMNS = [
     "id",
+    "creatorUsername",
     "status",
     "finishStatus",
     "loadedSize",
     "unloadedSize",
     "name",
     "note",
     "sites",
@@ -59,14 +60,15 @@
     count: int
 
 
 class Snapshot(BaseModel):
     snapshot_id: str = Field(alias="id")
     name: Optional[str]
     note: Optional[str]
+    creator_username: Optional[str] = Field(alias="creatorUsername")
     total_dev_count: int = Field(alias="totalDevCount")
     licensed_dev_count: Optional[int] = Field(alias="licensedDevCount")
     user_count: int = Field(alias="userCount")
     interface_active_count: int = Field(alias="interfaceActiveCount")
     interface_count: int = Field(alias="interfaceCount")
     interface_edge_count: int = Field(alias="interfaceEdgeCount")
     device_added_count: int = Field(alias="deviceAddedCount")
```

### Comparing `ipfabric-6.2.5/ipfabric/models/table.py` & `ipfabric-6.3.0b0/ipfabric/models/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,58 +31,68 @@
         self,
         columns: list = None,
         filters: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
         sort: Optional[dict] = None,
         limit: Optional[int] = 1000,
         start: Optional[int] = 0,
-    ) -> list:
+        csv: bool = False,
+    ) -> Union[List[dict], bytes]:
         """Gets all data from corresponding endpoint
 
         Args:
             columns: Optional columns to return, default is all
             filters: Optional filters'
             attr_filters: dict: Optional dictionary of Attribute filters
             sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
             limit: Default to 1,000 rows
             start: Starts at 0
-
+            csv: bool: Default False, returns bytes if True.
         Returns:
-            list: List of Dictionaries
+            Union[List[dict], str]: List of Dictionaries or bytes if CSV
         """
         return self.client.fetch(
             self.endpoint,
             columns=columns,
             filters=filters,
             attr_filters=attr_filters,
             sort=sort,
             limit=limit,
             start=start,
             snapshot=False,
+            csv=csv,
         )
 
     def all(
         self,
         columns: list = None,
         filters: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
         sort: Optional[dict] = None,
-    ):
+        csv: bool = False,
+    ) -> Union[List[dict], bytes]:
         """Gets all data from corresponding endpoint
 
         Args:
             columns: Optional columns to return, default is all
             filters: Optional filters
             attr_filters: dict: Optional dictionary of Attribute filters
             sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
+            csv: bool: Default False, returns bytes if True.
         Returns:
-            list: List of Dictionaries
+            Union[List[dict], bytes]: List of Dictionaries or bytes if CSV
         """
         return self.client.fetch_all(
-            self.endpoint, columns=columns, filters=filters, attr_filters=attr_filters, sort=sort, snapshot=False
+            self.endpoint,
+            columns=columns,
+            filters=filters,
+            attr_filters=attr_filters,
+            sort=sort,
+            snapshot=False,
+            csv=csv,
         )
 
     def count(
         self,
         filters: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
     ):
@@ -104,71 +114,76 @@
         filters: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
         limit: Optional[int] = 1000,
         start: Optional[int] = 0,
-    ) -> list:
+        csv: bool = False,
+    ) -> Union[List[dict], bytes]:
         """Gets all data from corresponding endpoint
 
         Args:
             columns: Optional columns to return, default is all
             filters: Optional filters'
             attr_filters: dict: Optional dictionary of Attribute filters
             snapshot_id: Optional snapshot ID to override class
             reports: True to return Intent Rules (also accepts string of frontend URL) or a list of report IDs
             sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
             limit: Default to 1,000 rows
             start: Starts at 0
-
+            csv: bool: Default False, returns bytes if True.
         Returns:
-            list: List of Dictionaries
+            Union[List[dict], str]: List of Dictionaries or bytes if CSV
         """
         return self.client.fetch(
             self.endpoint,
             columns=columns,
             filters=filters,
             attr_filters=attr_filters,
             snapshot_id=snapshot_id,
             reports=reports,
             sort=sort,
             limit=limit,
             start=start,
+            csv=csv,
         )
 
     def all(
         self,
         columns: list = None,
         filters: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
-    ) -> list:
+        csv: bool = False,
+    ) -> Union[List[dict], bytes]:
         """Gets all data from corresponding endpoint
 
         Args:
             columns: Optional columns to return, default is all
             filters: Optional filters
             attr_filters: dict: Optional dictionary of Attribute filters
             snapshot_id: Optional snapshot ID to override class
             reports: True to return Intent Rules (also accepts string of frontend URL) or a list of report IDs
             sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
+            csv: bool: Default False, returns bytes if True.
         Returns:
-            list: List of Dictionaries
+            Union[List[dict], bytes]: List of Dictionaries or bytes if CSV
         """
         return self.client.fetch_all(
             self.endpoint,
             columns=columns,
             filters=filters,
             attr_filters=attr_filters,
             snapshot_id=snapshot_id,
             reports=reports,
             sort=sort,
+            csv=csv,
         )
 
     def count(
         self,
         filters: Optional[dict] = None,
         snapshot_id: Optional[str] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
@@ -392,14 +407,16 @@
 
 class DeviceTable(Table):
     """model for Device Table data"""
 
     endpoint = "tables/inventory/devices"
 
     def _as_model(self, devices, as_model):
+        if not as_model:
+            return devices
         try:
             attributes = Attributes(client=self.client, snapshot_id=self.client.snapshot_id).all()
         except HTTPStatusError:
             logger.warning(
                 self.client._api_insuf_rights
                 + 'on POST "/tables/snapshot-attributes". Cannot load Attributes in Devices.'
             )
@@ -408,85 +425,88 @@
             blob_keys = self.client.fetch_all("/tables/management/configuration/saved", columns=["sn", "blobKey"])
         except HTTPStatusError:
             logger.warning(
                 self.client._api_insuf_rights + 'on POST "/tables/management/configuration/saved". '
                 "You will not be able to pull device config from Device model."
             )
             blob_keys = None
-        if as_model:
-            devices = Devices(
-                snapshot_id=self.client.snapshot_id, devices=devices, attributes=attributes, blob_keys=blob_keys
-            )
-        return devices
+        return Devices(snapshot_id=self.client.snapshot_id, devices=devices, attributes=attributes, blob_keys=blob_keys)
 
     def fetch(
         self,
         columns: list = None,
         filters: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
         limit: Optional[int] = 1000,
         start: Optional[int] = 0,
         as_model: Optional[bool] = False,
-    ) -> Union[list, Devices]:
+        csv: bool = False,
+    ) -> Union[List[dict], Devices, bytes]:
         """Gets all data from corresponding endpoint
 
         Args:
             columns: Optional columns to return, default is all
             filters: Optional filters'
             attr_filters: dict: Optional dictionary of Attribute filters
             snapshot_id: Optional snapshot ID to override class
             reports: True to return Intent Rules (also accepts string of frontend URL) or a list of report IDs
             sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
             limit: Default to 1,000 rows
             start: Starts at 0
             as_model: bool: Default False, if True returns Devices model
-
+            csv: bool: Default False, returns bytes if True. If `as_model` set to True then csv will be set to False.
         Returns:
-            list: List of Dictionaries
+            Union[List[dict], Devices, bytes]: List of Dictionaries, Devices Object if as_model, or bytes if CSV
         """
+        csv = False if as_model else csv
         devices = super(DeviceTable, self).fetch(
             columns=columns,
             filters=filters,
             attr_filters=attr_filters,
             snapshot_id=snapshot_id,
             reports=reports,
             sort=sort,
             limit=limit,
             start=start,
+            csv=csv,
         )
         return self._as_model(devices, as_model)
 
     def all(
         self,
         columns: list = None,
         filters: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
         as_model: Optional[bool] = False,
-    ) -> Union[list, Devices]:
+        csv: bool = False,
+    ) -> Union[List[dict], Devices, bytes]:
         """Gets all data from corresponding endpoint
 
         Args:
             columns: Optional columns to return, default is all
             filters: Optional filters
             attr_filters: dict: Optional dictionary of Attribute filters
             snapshot_id: Optional snapshot ID to override class
             reports: True to return Intent Rules (also accepts string of frontend URL) or a list of report IDs
             sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
             as_model: bool: Default False, if True returns Devices model
+            csv: bool: Default False, returns bytes if True. If `as_model` set to True then csv will be set to False.
         Returns:
-            list: List of Dictionaries
+            Union[List[dict], Devices, bytes]: List of Dictionaries, Devices Object if as_model, or bytes if CSV
         """
+        csv = False if as_model else csv
         devices = super(DeviceTable, self).all(
             columns=columns,
             filters=filters,
             attr_filters=attr_filters,
             snapshot_id=snapshot_id,
             reports=reports,
             sort=sort,
+            csv=csv,
         )
         return self._as_model(devices, as_model)
```

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/__init__.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/addressing.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/addressing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/dhcp.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/dhcp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/fhrp.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/fhrp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/interfaces.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/interfaces.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/load_balancing.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/load_balancing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/management.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/management.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/mpls.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/mpls.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/multicast.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/multicast.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/neighbors.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/neighbors.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/oam.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/oam.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/platforms.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/platforms.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/port_channels.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/port_channels.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/qos.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/qos.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/routing.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/routing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/sdn.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/sdn.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/security.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/security.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/stp.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/stp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/vlans.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/vlans.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/models/technology/wireless.py` & `ipfabric-6.3.0b0/ipfabric/models/technology/wireless.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/settings/__init__.py` & `ipfabric-6.3.0b0/ipfabric/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/settings/api_tokens.py` & `ipfabric-6.3.0b0/ipfabric/settings/api_tokens.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from secrets import token_hex
 from typing import Any, Union, Optional, List
 
 from pydantic import Field, BaseModel
 
 from ipfabric.settings.user_mgmt import UserMgmt
 from ipfabric.tools.shared import date_parser
 
@@ -11,15 +10,15 @@
 
 
 class Token(BaseModel):
     description: str
     usage: int
     username: str
     expires: Optional[int] = None
-    secret: Optional[str] = None
+    token: Optional[str] = None
     user_id: str = Field(alias="userId")
     user_role_ids: Optional[List[str]] = Field(alias="userRoleIds", default=None)
     token_id: str = Field(alias="id")
     is_expired: bool = Field(alias="isExpired")
     last_used: Optional[str] = Field(alias="lastUsed")
     role_ids: List[str] = Field(alias="roleIds")
     role_names: Optional[List[str]] = Field(alias="roleNames", default=None)
@@ -62,30 +61,24 @@
 
     def add_token(
         self,
         descr: str,
         role_ids: Optional[list] = None,
         role_names: Optional[list] = None,
         expires: Optional[Union[str, int]] = None,
-        token: str = None,
     ):
-        if token and len(token) < 8:
-            raise SyntaxError("Token must be 8 characters.")
-        elif not token:
-            token = token_hex(16)
 
         payload = dict(
             description=descr,
             expires=int(date_parser(expires).timestamp() * 1000) if expires else None,
             roleIds=self._check_roles(role_ids or list(), role_names or list()),
-            token=token,
         )
         res = self.client.post("api-tokens", json=payload)
         res.raise_for_status()
-        return Token(secret=token, **res.json())
+        return Token(**res.json())
 
     def delete_token(self, token_id: [int, str, Token]):
         token_id = token_id.token_id if isinstance(token_id, Token) else str(token_id)
         if token_id not in self.tokens_by_id:
             raise ValueError(f"Could not find token matching ID '{token_id}'.")
         res = self.client.delete("api-tokens/" + token_id)
         res.raise_for_status()
```

### Comparing `ipfabric-6.2.5/ipfabric/settings/attributes.py` & `ipfabric-6.3.0b0/ipfabric/settings/attributes.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/settings/authentication.py` & `ipfabric-6.3.0b0/ipfabric/settings/authentication.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/settings/discovery.py` & `ipfabric-6.3.0b0/ipfabric/settings/discovery.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/settings/seeds.py` & `ipfabric-6.3.0b0/ipfabric/settings/seeds.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/settings/site_separation.py` & `ipfabric-6.3.0b0/ipfabric/settings/site_separation.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/settings/user_mgmt.py` & `ipfabric-6.3.0b0/ipfabric/settings/user_mgmt.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     token_id: str = Field(alias="id")
     description: Optional[str]
     role_ids: list = Field(alias="roleIds")
 
 
 class User(BaseModel):
     username: str
-    email: Optional[str]
     user_id: str = Field(alias="id")
     local: Optional[bool] = Field(alias="isLocal")
     sso_provider: Optional[Any] = Field(alias="ssoProvider")
     domains: Optional[Any] = Field(alias="domainSuffixes")
     role_names: Optional[list] = Field(alias="roleNames", default_factory=list)
     role_ids: list = Field(alias="roleIds")
     ldap_id: Optional[Any] = Field(alias="ldapId")
@@ -108,35 +107,32 @@
         resp.raise_for_status()
         user = resp.json()
         return User(roleNames=[self.roles_by_id[r].name for r in user["roleIds"]], **user)
 
     def add_user(
         self,
         username: str,
-        email: str,
         password: str,
         roles: list,
         timezone: str = "UTC",
     ):
         """
         Adds a user
         :param username: str: Username
-        :param email: str: Email
         :param password: str: Must be 8 characters
         :param roles: list: Role IDs for Users
         :param timezone: str: v4.2 and above, Defaults UTC.  See pytz.all_timezones for correct syntax
         :return: User
         """
         if len(password) < 8:
             raise SyntaxError("Password must be 8 characters.")
         if not all(x in [r.role_id for r in self.roles] for x in roles):
             raise SyntaxError(f"Only accepted scopes are {[r.role_id for r in self.roles]}")
         payload = {
             "username": username,
-            "email": email,
             "password": password,
             "roleIds": roles,
         }
         if timezone not in pytz.all_timezones:
             raise ValueError(
                 f"Timezone {timezone} is not located. This is case sensitive please see pytz.all_timezones."
             )
```

### Comparing `ipfabric-6.2.5/ipfabric/settings/vendor_api.py` & `ipfabric-6.3.0b0/ipfabric/settings/vendor_api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/settings/vendor_api_models.py` & `ipfabric-6.3.0b0/ipfabric/settings/vendor_api_models.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/configuration.py` & `ipfabric-6.3.0b0/ipfabric/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/discovery_history.py` & `ipfabric-6.3.0b0/ipfabric/tools/discovery_history.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/dashboard.json` & `ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v4/4/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/groups.json` & `ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v4/4/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/intents.json` & `ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v4/4/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/dashboard.json` & `ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v5/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/groups.json` & `ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v5/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/intents.json` & `ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v5/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/dashboard.json` & `ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v6/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/groups.json` & `ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v6/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/intents.json` & `ipfabric-6.3.0b0/ipfabric/tools/factory_defaults/v6/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/nist.py` & `ipfabric-6.3.0b0/ipfabric/tools/nist.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/restore_intents.py` & `ipfabric-6.3.0b0/ipfabric/tools/restore_intents.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/shared.py` & `ipfabric-6.3.0b0/ipfabric/tools/shared.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/site_seperation_report.py` & `ipfabric-6.3.0b0/ipfabric/tools/site_seperation_report.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/ipfabric/tools/vulnerabilities.py` & `ipfabric-6.3.0b0/ipfabric/tools/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/LICENSE` & `ipfabric-6.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/pyproject.toml` & `ipfabric-6.3.0b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric"
-version = "v6.2.5"
+version = "v6.3.0b0"
 description = "Python package for interacting with IP Fabric"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
     "Community Fabric <communityfabric@ipfabric.io>"
 ]
 license = "MIT"
@@ -15,32 +15,32 @@
 
 [tool.poetry.urls]
 "IP Fabric" = "https://ipfabric.io/"
 "Changelog" = "https://gitlab.com/ip-fabric/integrations/python-ipfabric/-/blob/develop/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
-httpx = "^0.23.2"
+httpx = "^0.24.1"
 python-dateutil = "^2.8.2"
 pydantic = "^1.10.4"
 pytz = "^2023.3"
 python-dotenv = "^0.21"  # v1.0.0 requires python3.8
 pandas = {version = "^1.3.0", optional = true}
 openpyxl = {version = "^3.0.9", optional = true}
 tabulate = {version = ">=0.8.9,<0.10.0",  optional = true}
 python-json-logger = {version = "^2.0.4",  optional = true}
 macaddress = "~2.0.2"
 pyyaml = {version = "^6.0", optional = true}
-deepdiff = "^6.2.2"
+deepdiff = "^6.3.1"
 case-insensitive-dictionary = "^0.2.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.1"
-pytest-cov = "^4.0.0"
-flake8 = "^5.0.4"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+flake8 = "^5.0"
 black = "^22.12"
 
 [tool.poetry.extras]
 examples = ["tabulate", "pandas", "openpyxl", "python-json-logger", "pyyaml"]
 
 [build-system]
 requires = ["poetry-core>=1.4.0"]
```

### Comparing `ipfabric-6.2.5/README.md` & `ipfabric-6.3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.5/setup.py` & `ipfabric-6.3.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
  'ipfabric.tools.factory_defaults.v6.0']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['case-insensitive-dictionary>=0.2.1,<0.3.0',
- 'deepdiff>=6.2.2,<7.0.0',
- 'httpx>=0.23.2,<0.24.0',
+ 'deepdiff>=6.3.1,<7.0.0',
+ 'httpx>=0.24.1,<0.25.0',
  'macaddress>=2.0.2,<2.1.0',
  'pydantic>=1.10.4,<2.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'python-dotenv>=0.21,<0.22',
  'pytz>=2023.3,<2024.0']
 
 extras_require = \
@@ -33,15 +33,15 @@
               'openpyxl>=3.0.9,<4.0.0',
               'tabulate>=0.8.9,<0.10.0',
               'python-json-logger>=2.0.4,<3.0.0',
               'pyyaml>=6.0,<7.0']}
 
 setup_kwargs = {
     'name': 'ipfabric',
-    'version': '6.2.5',
+    'version': '6.3.0b0',
     'description': 'Python package for interacting with IP Fabric',
     'long_description': '# IP Fabric \n\nIPFabric is a Python module for connecting to and communicating against an IP Fabric instance.\n\n## About\n\nFounded in 2015, [IP Fabric](https://ipfabric.io/) develops network infrastructure visibility and analytics solution to\nhelp enterprise network and security teams with network assurance and automation across multi-domain heterogeneous\nenvironments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP\nFabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless\ndigital transformation. \n\n## v7.0.0 Deprecation Notices\n\nIn `ipfabric>=v7.0.0` the following will be deprecated:\n\n- `ipfabric_diagrams` package will move to `ipfabric.diagrams`\n- Python 3.7 support will be removed.\n- The use of `token=\'<TOKEN>\'` or `username=\'<USER>\', password=\'<PASS>\'` in `IPFClient()` will be removed:\n  - Token: `IPFClient(auth=\'TOKEN\')`\n  - User/Pass: `IPFClient(auth=(\'USER\', \'PASS\'))`\n  - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`\n\n## Versioning\n\nStarting with IP Fabric version 5.0.x the python-ipfabric and python-ipfabric-diagrams will need to\nmatch your IP Fabric version.  The API\'s are changing and instead of `api/v1` they will now be `api/v5.0`.\n\nVersion 5.1 will have backwards compatability with version 5.0 however 6.0 will not support any 5.x versions.\nBy ensuring that your ipfabric SDK\'s match your IP Fabric Major Version will ensure compatibility and will continue to work.\n\n## Installation\n\n```\npip install ipfabric\n```\n\n## Introduction\n\nPlease take a look at [API Programmability - Part 1: The Basics](https://ipfabric.io/blog/api-programmability-part-1/)\nfor instructions on creating an API token.\n\nMost of the methods and features can be located in [Examples](examples) to show how to use this package. \nAnother great introduction to this package can be found at [API Programmability - Part 2: Python](https://ipfabric.io/blog/api-programmability-python/)\n\n## Diagrams\n\nDiagramming in IP Fabric version v4.3 and above has been moved to it\'s own package.\n\nDiagramming will move back to this project in v7.0\n\n```\npip install ipfabric-diagrams\n```\n\n## Authentication\n### Username/Password\nSupply in client:\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=(\'user\', \'pass\'))\n```\n\n### Token\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=\'token\')\n```\n\n### Environment \nThe easiest way to use this package is with a `.env` file.  You can copy the sample and edit it with your environment variables. \n\n```commandline\ncp sample.env .env\n```\n\nThis contains the following variables which can also be set as environment variables instead of a .env file.\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_TOKEN=TOKEN\nIPF_VERIFY=true\n```\n\nOr if using Username/Password:\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_USERNAME=USER\nIPF_PASSWORD=PASS\n```\n\n## Development\n\n### Poetry Installation\n\nIPFabric uses [Poetry](https://pypi.org/project/poetry/) to make setting up a virtual environment with all dependencies\ninstalled quick and easy.\n\nInstall poetry globally:\n```\npip install poetry\n```\n\nTo install a virtual environment run the following command in the root of this directory.\n\n```\npoetry install\n```\n\nTo run examples, install extras:\n```\npoetry install ipfabric -E examples\n```\n\n### Test and Build\n\n```\npoetry run pytest\npoetry build\n```\n\nPrior to pushing changes run:\n```\npoetry run black ipfabric\npoetry update\n```\n',
     'author': 'Justin Jeffery',
     'author_email': 'justin.jeffery@ipfabric.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ip-fabric/integrations/python-ipfabric',
```

### Comparing `ipfabric-6.2.5/PKG-INFO` & `ipfabric-6.3.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric
-Version: 6.2.5
+Version: 6.3.0b0
 Summary: Python package for interacting with IP Fabric
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.7.1,<4.0.0
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: examples
 Requires-Dist: case-insensitive-dictionary (>=0.2.1,<0.3.0)
-Requires-Dist: deepdiff (>=6.2.2,<7.0.0)
-Requires-Dist: httpx (>=0.23.2,<0.24.0)
+Requires-Dist: deepdiff (>=6.3.1,<7.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: macaddress (>=2.0.2,<2.1.0)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0) ; extra == "examples"
 Requires-Dist: pandas (>=1.3.0,<2.0.0) ; extra == "examples"
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21,<0.22)
 Requires-Dist: python-json-logger (>=2.0.4,<3.0.0) ; extra == "examples"
```

