# Comparing `tmp/nautobot_ssot-1.3.2.tar.gz` & `tmp/nautobot_ssot-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_ssot-1.3.2.tar", max compression
+gzip compressed data, was "nautobot_ssot-2.0.0b1.tar", max compression
```

## Comparing `nautobot_ssot-1.3.2.tar` & `nautobot_ssot-2.0.0b1.tar`

### file list

```diff
@@ -1,46 +1,90 @@
--rw-r--r--   0        0        0      591 2023-05-23 13:50:19.410350 nautobot_ssot-1.3.2/LICENSE
--rw-r--r--   0        0        0     4936 2023-05-23 13:50:19.410350 nautobot_ssot-1.3.2/README.md
--rw-r--r--   0        0        0     1089 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/__init__.py
--rw-r--r--   0        0        0       48 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/api/__init__.py
--rw-r--r--   0        0        0      828 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/choices.py
--rw-r--r--   0        0        0     1088 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/filters.py
--rw-r--r--   0        0        0     1541 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/forms.py
--rw-r--r--   0        0        0      916 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/jobs/__init__.py
--rw-r--r--   0        0        0    15543 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/jobs/base.py
--rw-r--r--   0        0        0    25274 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/jobs/examples.py
--rw-r--r--   0        0        0     4846 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/metrics.py
--rw-r--r--   0        0        0     3035 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/migrations/0001_initial.py
--rw-r--r--   0        0        0     2378 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/migrations/0002_performance_metrics.py
--rw-r--r--   0        0        0      586 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py
--rw-r--r--   0        0        0      408 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/migrations/0004_sync_summary.py
--rw-r--r--   0        0        0        0 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/migrations/__init__.py
--rw-r--r--   0        0        0     8764 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/models.py
--rw-r--r--   0        0        0      601 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/navigation.py
--rw-r--r--   0        0        0     6527 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tables.py
--rw-r--r--   0        0        0     1017 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/template_content.py
--rw-r--r--   0        0        0     3847 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/dashboard.html
--rw-r--r--   0        0        0     4682 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/data_source_target.html
--rw-r--r--   0        0        0      432 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/history.html
--rw-r--r--   0        0        0     8843 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_detail.html
--rw-r--r--   0        0        0     2513 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_header.html
--rw-r--r--   0        0        0      365 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_jobresult.html
--rw-r--r--   0        0        0      322 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_logentries.html
--rw-r--r--   0        0        0      292 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/synclogentry_list.html
--rw-r--r--   0        0        0      579 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html
--rw-r--r--   0        0        0        0 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templatetags/__init__.py
--rw-r--r--   0        0        0      694 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templatetags/dashboard_helpers.py
--rw-r--r--   0        0        0      787 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templatetags/humanize_bytes.py
--rw-r--r--   0        0        0     2214 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templatetags/render_diff.py
--rw-r--r--   0        0        0      570 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templatetags/shorter_timedelta.py
--rw-r--r--   0        0        0      257 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/__init__.py
--rw-r--r--   0        0        0      662 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/jobs/__init__.py
--rw-r--r--   0        0        0      983 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_api.py
--rw-r--r--   0        0        0     1518 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_basic.py
--rw-r--r--   0        0        0     5018 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_jobs.py
--rw-r--r--   0        0        0     3058 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_models.py
--rw-r--r--   0        0        0     2437 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_render_diff.py
--rw-r--r--   0        0        0     5634 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_views.py
--rw-r--r--   0        0        0     1004 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/urls.py
--rw-r--r--   0        0        0     6326 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/views.py
--rw-r--r--   0        0        0     3798 2023-05-23 13:50:32.703160 nautobot_ssot-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 nautobot_ssot-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-07-14 14:55:11.198955 nautobot_ssot-2.0.0b1/LICENSE
+-rw-r--r--   0        0        0     4936 2023-07-14 14:55:11.198955 nautobot_ssot-2.0.0b1/README.md
+-rw-r--r--   0        0        0     1989 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/api/__init__.py
+-rw-r--r--   0        0        0      823 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/choices.py
+-rw-r--r--   0        0        0     1146 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/filters.py
+-rw-r--r--   0        0        0     1567 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/forms.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/__init__.py
+-rw-r--r--   0        0        0     1354 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/constant.py
+-rw-r--r--   0        0        0       65 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/diffsync/__init__.py
+-rw-r--r--   0        0        0       86 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/diffsync/adapters/__init__.py
+-rw-r--r--   0        0        0     6403 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/diffsync/adapters/infoblox.py
+-rw-r--r--   0        0        0    11998 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/diffsync/adapters/nautobot.py
+-rw-r--r--   0        0        0      431 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/diffsync/models/__init__.py
+-rw-r--r--   0        0        0     1596 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/diffsync/models/base.py
+-rw-r--r--   0        0        0     3363 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/diffsync/models/infoblox.py
+-rw-r--r--   0        0        0    14692 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/diffsync/models/nautobot.py
+-rw-r--r--   0        0        0     4835 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/jobs.py
+-rw-r--r--   0        0        0     2597 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/signals.py
+-rw-r--r--   0        0        0       64 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/utils/__init__.py
+-rw-r--r--   0        0        0    43831 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/utils/client.py
+-rw-r--r--   0        0        0     2823 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/utils/diffsync.py
+-rw-r--r--   0        0        0     1158 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/infoblox/utils/nautobot.py
+-rw-r--r--   0        0        0     1021 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/integrations/utils.py
+-rw-r--r--   0        0        0     1469 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/jobs/__init__.py
+-rw-r--r--   0        0        0    14484 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/jobs/base.py
+-rw-r--r--   0        0        0    28481 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/jobs/examples.py
+-rw-r--r--   0        0        0     5543 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/metrics.py
+-rw-r--r--   0        0        0     3035 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2378 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/migrations/0002_performance_metrics.py
+-rw-r--r--   0        0        0      586 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py
+-rw-r--r--   0        0        0      408 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/migrations/0004_sync_summary.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/migrations/__init__.py
+-rw-r--r--   0        0        0     8980 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/models.py
+-rw-r--r--   0        0        0      749 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/navigation.py
+-rw-r--r--   0        0        0     9530 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/static/nautobot_ssot_infoblox/infoblox_logo.png
+-rw-r--r--   0        0        0     6522 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tables.py
+-rw-r--r--   0        0        0     1017 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/template_content.py
+-rw-r--r--   0        0        0     3847 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/dashboard.html
+-rw-r--r--   0        0        0     4682 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/data_source_target.html
+-rw-r--r--   0        0        0      432 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/history.html
+-rw-r--r--   0        0        0     8843 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/sync_detail.html
+-rw-r--r--   0        0        0     2513 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/sync_header.html
+-rw-r--r--   0        0        0      365 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/sync_jobresult.html
+-rw-r--r--   0        0        0      322 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/sync_logentries.html
+-rw-r--r--   0        0        0      292 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/synclogentry_list.html
+-rw-r--r--   0        0        0      713 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html
+-rw-r--r--   0        0        0        0 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templatetags/__init__.py
+-rw-r--r--   0        0        0      694 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templatetags/dashboard_helpers.py
+-rw-r--r--   0        0        0      787 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templatetags/humanize_bytes.py
+-rw-r--r--   0        0        0     2214 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templatetags/render_diff.py
+-rw-r--r--   0        0        0      570 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/templatetags/shorter_timedelta.py
+-rw-r--r--   0        0        0      257 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/create_a_record.json
+-rw-r--r--   0        0        0      155 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/create_host_record.json
+-rw-r--r--   0        0        0      254 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/create_ptr_record.json
+-rw-r--r--   0        0        0      168 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/find_network_reference.json
+-rw-r--r--   0        0        0       43 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/find_next_available_ip.json
+-rw-r--r--   0        0        0      305 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_a_record_by_ip.json
+-rw-r--r--   0        0        0      306 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_a_record_by_name.json
+-rw-r--r--   0        0        0      378 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_all_dns_views.json
+-rw-r--r--   0        0        0     1050 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_all_ipv4address_networks.json
+-rw-r--r--   0        0        0      505 2023-07-14 14:55:11.210955 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_all_ipv4address_networks_bulk.json
+-rw-r--r--   0        0        0   500490 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_all_ipv4address_networks_large.json
+-rw-r--r--   0        0        0     4274 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_all_ipv4address_networks_medium.json
+-rw-r--r--   0        0        0      447 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_all_subnets.json
+-rw-r--r--   0        0        0     1281 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_authoritative_zone.json
+-rw-r--r--   0        0        0      257 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_dhcp_lease_from_hostname.json
+-rw-r--r--   0        0        0      283 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_dhcp_lease_from_ipv4.json
+-rw-r--r--   0        0        0      716 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_host_by_ip.json
+-rw-r--r--   0        0        0      716 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_host_record_by_name.json
+-rw-r--r--   0        0        0      256 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/get_ptr_record_by_name.json
+-rw-r--r--   0        0        0      891 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures/search_ipv4_address.json
+-rw-r--r--   0        0        0     3761 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/fixtures_infoblox.py
+-rw-r--r--   0        0        0    25358 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/test_client.py
+-rw-r--r--   0        0        0     1024 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/infoblox/test_utils.py
+-rw-r--r--   0        0        0      662 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/jobs/__init__.py
+-rw-r--r--   0        0        0      983 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/test_api.py
+-rw-r--r--   0        0        0      994 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/test_basic.py
+-rw-r--r--   0        0        0     4627 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/test_jobs.py
+-rw-r--r--   0        0        0     2890 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/test_models.py
+-rw-r--r--   0        0        0     2460 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/test_render_diff.py
+-rw-r--r--   0        0        0     5878 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/tests/test_views.py
+-rw-r--r--   0        0        0     1223 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/urls.py
+-rw-r--r--   0        0        0      107 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/utils.py
+-rw-r--r--   0        0        0     6140 2023-07-14 14:55:11.214956 nautobot_ssot-2.0.0b1/nautobot_ssot/views.py
+-rw-r--r--   0        0        0     4076 2023-07-14 14:55:26.803927 nautobot_ssot-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     6174 1970-01-01 00:00:00.000000 nautobot_ssot-2.0.0b1/PKG-INFO
```

### Comparing `nautobot_ssot-1.3.2/LICENSE` & `nautobot_ssot-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/README.md` & `nautobot_ssot-2.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/choices.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/choices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ChoiceSet classes for Single Source of Truth (SSoT)."""
 
-from nautobot.utilities.choices import ChoiceSet
+from nautobot.apps.choices import ChoiceSet
 
 
 class SyncLogEntryActionChoices(ChoiceSet):
     """Valid values for a SyncLogEntry.action field."""
 
     ACTION_NO_CHANGE = "no-change"
     ACTION_CREATE = "create"
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/filters.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Filtering logic for Sync and SyncLogEntry records."""
 
 import django_filters
 from django.db.models import Q
 
-from nautobot.utilities.filters import BaseFilterSet
+from nautobot.apps.filters import BaseFilterSet
 
 from .models import Sync, SyncLogEntry
 
 
 class SyncFilterSet(BaseFilterSet):
     """Filter capabilities for SyncOverview instances."""
 
@@ -25,12 +25,16 @@
 
     class Meta:
         """Metaclass attributes of SyncLogEntryFilter."""
 
         model = SyncLogEntry
         fields = ["sync", "action", "status", "synced_object_type"]
 
-    def search(self, queryset, _name, value):  # pylint: disable=no-self-use
+    def search(self, queryset, _name, value):
         """String search of SyncLogEntry records."""
         if not value.strip():
             return queryset
-        return queryset.filter(Q(diff__icontains=value) | Q(message__icontains=value) | Q(object_repr__icontains=value))
+        return queryset.filter(
+            Q(diff__icontains=value)  # pylint: disable=unsupported-binary-operation
+            | Q(message__icontains=value)
+            | Q(object_repr__icontains=value)
+        )
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/forms.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/forms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Forms for working with Sync and SyncLogEntry models."""
 
 from django import forms
 
-from nautobot.utilities.forms import add_blank_choice, BootstrapMixin, BOOLEAN_WITH_BLANK_CHOICES
+from nautobot.apps.forms import add_blank_choice
+from nautobot.core.forms import BootstrapMixin, BOOLEAN_WITH_BLANK_CHOICES
 
 from .choices import SyncLogEntryActionChoices, SyncLogEntryStatusChoices
 from .models import Sync, SyncLogEntry
 
 
 class SyncFilterForm(BootstrapMixin, forms.ModelForm):
     """Form for filtering SyncOverview records."""
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/jobs/base.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/jobs/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """Base Job classes for sync workers."""
 from collections import namedtuple
 from datetime import datetime
 import traceback
 import tracemalloc
 from typing import Iterable
-from packaging.version import Version
 
-from django.forms import HiddenInput
 from django.templatetags.static import static
 from django.utils import timezone
 from django.utils.functional import classproperty
 
 # pylint-django doesn't understand classproperty, and complains unnecessarily. We disable this specific warning:
 # pylint: disable=no-self-argument
 
 from diffsync.enum import DiffSyncFlags
 import structlog
 
-from nautobot import __version__ as nautobot_version
-from nautobot.extras.jobs import BaseJob, BooleanVar
+from nautobot.extras.jobs import DryRunVar, Job, BooleanVar
 
 from nautobot_ssot.choices import SyncLogEntryActionChoices
 from nautobot_ssot.models import Sync, SyncLogEntry
 
 
 DataMapping = namedtuple("DataMapping", ["source_name", "source_url", "target_name", "target_url"])
 """Entry in the list returned by a job's data_mappings() API.
@@ -34,151 +31,145 @@
 * source_url: URL (if any) to hyperlink for this source_name in the UI.
               Can be used, for example, to link to the Nautobot list view for this data class.
 * target_name: Name of a data class on the data target that corresponds to the source data.
 * target_url: URL (if any) to hyperlink the target_name.
 """
 
 
-class DataSyncBaseJob(BaseJob):  # pylint: disable=too-many-instance-attributes
+class DataSyncBaseJob(Job):  # pylint: disable=too-many-instance-attributes
     """Common base class for data synchronization jobs.
 
     Works mostly as per the BaseJob API, with the following changes:
 
     - Concrete subclasses are responsible for implementing `self.sync_data()` (or related hooks), **not** `self.run()`.
     - Subclasses may optionally define any Meta field supported by Jobs, as well as the following:
-      - `dry_run_default` - defaults to True if unspecified
+      - `dryrun_default` - defaults to True if unspecified
       - `data_source` and `data_target` as labels (by default, will use the `name` and/or "Nautobot" as appropriate)
       - `data_source_icon` and `data_target_icon`
     """
 
-    dry_run = BooleanVar()
+    dryrun = DryRunVar(description="Perform a dry-run, making no actual changes to Nautobot data.", default=True)
     memory_profiling = BooleanVar(description="Perform a memory profiling analysis.", default=False)
 
     def load_source_adapter(self):
         """Method to instantiate and load the SOURCE adapter into `self.source_adapter`.
 
         Relevant available instance attributes include:
 
-        - self.kwargs     (corresponds to the Job's `data` input, including 'dry_run' option)
         - self.job_result (as per Job API)
         """
         raise NotImplementedError
 
     def load_target_adapter(self):
         """Method to instantiate and load the TARGET adapter into `self.target_adapter`.
 
         Relevant available instance attributes include:
 
-        - self.kwargs     (corresponds to the Job's `data` input, including 'dry_run' option)
         - self.job_result (as per Job API)
         """
         raise NotImplementedError
 
     def calculate_diff(self):
         """Method to calculate the difference from SOURCE to TARGET adapter and store in `self.diff`.
 
         This is a generic implementation that you could overwrite completely in your custom logic.
         """
         if self.source_adapter is not None and self.target_adapter is not None:
             self.diff = self.source_adapter.diff_to(self.target_adapter, flags=self.diffsync_flags)
             self.sync.diff = self.diff.dict()
             self.sync.summary = self.diff.summary()
             self.sync.save()
-            self.log_info(message=self.diff.summary())
+            self.logger.info(self.diff.summary())
         else:
-            self.log_warning(message="Not both adapters were properly initialized prior to diff calculation.")
+            self.logger.warning("Not both adapters were properly initialized prior to diff calculation.")
 
     def execute_sync(self):
         """Method to synchronize the difference from `self.diff`, from SOURCE to TARGET adapter.
 
         This is a generic implementation that you could overwrite completely in your custom logic.
         """
         if self.source_adapter is not None and self.target_adapter is not None:
             self.source_adapter.sync_to(self.target_adapter, flags=self.diffsync_flags)
         else:
-            self.log_warning(message="Not both adapters were properly initialized prior to synchronization.")
+            self.logger.warning("Not both adapters were properly initialized prior to synchronization.")
 
-    def sync_data(self):
+    def sync_data(self, memory_profiling):
         """Method to load data from adapters, calculate diffs and sync (if not dry-run).
 
         It is composed by 4 methods:
         - self.load_source_adapter: instantiates the source adapter (self.source_adapter) and loads its data
         - self.load_target_adapter: instantiates the target adapter (self.target_adapter) and loads its data
         - self.calculate_diff: generates the diff from source to target adapter and stores it in self.diff
         - self.execute_sync: if not dry-run, uses the self.diff to synchronize from source to target
 
         This is a generic implementation that you could overwrite completely in you custom logic.
         Available instance attributes include:
 
-        - self.kwargs     (corresponds to the Job's `data` input, including 'dry_run' option)
-        - self.commit     (should generally be True)
         - self.sync       (Sync instance tracking this job execution)
         - self.job_result (as per Job API)
         """
 
         def record_memory_trace(step: str):
             """Helper function to record memory usage and reset tracemalloc stats."""
             memory_final, memory_peak = tracemalloc.get_traced_memory()
             setattr(self.sync, f"{step}_memory_final", memory_final)
             setattr(self.sync, f"{step}_memory_peak", memory_peak)
             self.sync.save()
-            self.log_info(
-                message=(f"Traced memory for {step} (Final, Peak): {memory_final} bytes, {memory_peak} bytes")
-            )
+            self.logger.info("Traced memory for %s (Final, Peak): %s bytes, %s bytes", step, memory_final, memory_peak)
             tracemalloc.clear_traces()
 
         if not self.sync:
             return
 
-        if self.kwargs["memory_profiling"]:
+        if memory_profiling:
             tracemalloc.start()
 
         start_time = datetime.now()
 
-        self.log_info(message="Loading current data from source adapter...")
+        self.logger.info("Loading current data from source adapter...")
         self.load_source_adapter()
         load_source_adapter_time = datetime.now()
         self.sync.source_load_time = load_source_adapter_time - start_time
         self.sync.save()
-        self.log_info(message=f"Source Load Time from {self.source_adapter}: {self.sync.source_load_time}")
-        if self.kwargs["memory_profiling"]:
+        self.logger.info("Source Load Time from %s: %s", self.source_adapter, self.sync.source_load_time)
+        if memory_profiling:
             record_memory_trace("source_load")
 
-        self.log_info(message="Loading current data from target adapter...")
+        self.logger.info("Loading current data from target adapter...")
         self.load_target_adapter()
         load_target_adapter_time = datetime.now()
         self.sync.target_load_time = load_target_adapter_time - load_source_adapter_time
         self.sync.save()
-        self.log_info(message=f"Target Load Time from {self.target_adapter}: {self.sync.target_load_time}")
-        if self.kwargs["memory_profiling"]:
+        self.logger.info("Target Load Time from %s: %s", self.target_adapter, self.sync.target_load_time)
+        if memory_profiling:
             record_memory_trace("target_load")
 
-        self.log_info(message="Calculating diffs...")
+        self.logger.info("Calculating diffs...")
         self.calculate_diff()
         calculate_diff_time = datetime.now()
         self.sync.diff_time = calculate_diff_time - load_target_adapter_time
         self.sync.save()
-        self.log_info(message=f"Diff Calculation Time: {self.sync.diff_time}")
-        if self.kwargs["memory_profiling"]:
+        self.logger.info("Diff Calculation Time: %s", self.sync.diff_time)
+        if memory_profiling:
             record_memory_trace("diff")
 
-        if self.kwargs["dry_run"]:
-            self.log_info("As `dry_run` is set, skipping the actual data sync.")
+        if self.dryrun:
+            self.logger.info("As `dryrun` is set, skipping the actual data sync.")
         else:
-            self.log_info(message=f"Syncing from {self.source_adapter} to {self.target_adapter}...")
+            self.logger.info("Syncing from %s to %s...", self.source_adapter, self.target_adapter)
             self.execute_sync()
             execute_sync_time = datetime.now()
             self.sync.sync_time = execute_sync_time - calculate_diff_time
             self.sync.save()
-            self.log_info(message="Sync complete")
-            self.log_info(message=f"Sync Time: {self.sync.sync_time}")
-            if self.kwargs["memory_profiling"]:
+            self.logger.info("Sync complete")
+            self.logger.info("Sync Time: %s", self.sync.sync_time)
+            if memory_profiling:
                 record_memory_trace("sync")
 
-    def lookup_object(self, model_name, unique_id):  # pylint: disable=no-self-use,unused-argument
+    def lookup_object(self, model_name, unique_id):  # pylint: disable=unused-argument
         """Look up the Nautobot record, if any, identified by the args.
 
         Optional helper method used to build more detailed/accurate SyncLogEntry records from DiffSync logs.
 
         Args:
             model_name (str): DiffSyncModel class name or similar class/model label.
             unique_id (str): DiffSyncModel unique_id or similar unique identifier.
@@ -243,48 +234,41 @@
                 object_repr=object_repr,
             )
 
         return event_dict
 
     @classmethod
     def _get_vars(cls):
-        """Extend Job._get_vars to include `dry_run` variable.
+        """Extend Job._get_vars to include `dryrun` variable.
 
         Workaround for https://github.com/netbox-community/netbox/issues/5529
         """
         got_vars = super()._get_vars()
-        if hasattr(cls, "dry_run"):
-            got_vars["dry_run"] = cls.dry_run
+        if hasattr(cls, "dryrun"):
+            got_vars["dryrun"] = cls.dryrun
 
         if hasattr(cls, "memory_profiling"):
             got_vars["memory_profiling"] = cls.memory_profiling
         return got_vars
 
     def __init__(self):
         """Initialize a Job."""
         super().__init__()
         self.sync = None
-        self.kwargs = {}
-        self.commit = False
         self.diff = None
         self.source_adapter = None
         self.target_adapter = None
         # Default diffsync flags. You can overwrite them at any time.
         self.diffsync_flags = DiffSyncFlags.CONTINUE_ON_FAILURE | DiffSyncFlags.LOG_UNCHANGED_RECORDS
 
     def as_form(self, data=None, files=None, initial=None, approval_view=False):
         """Render this instance as a Django form for user inputs, including a "Dry run" field."""
-        if Version(nautobot_version) < Version("1.2"):
-            form = super().as_form(data=data, files=files, initial=initial)
-        else:
-            form = super().as_form(data=data, files=files, initial=initial, approval_view=approval_view)
-        # Set the "dry_run" widget's initial value based on our Meta attribute, if any
-        form.fields["dry_run"].initial = getattr(self.Meta, "dry_run_default", True)
-        # Hide the "commit" widget to reduce user confusion
-        form.fields["_commit"].widget = HiddenInput()
+        form = super().as_form(data=data, files=files, initial=initial, approval_view=approval_view)
+        # Set the "dryrun" widget's initial value based on our Meta attribute, if any
+        form.fields["dryrun"].initial = getattr(self.Meta, "dryrun_default", True)
         return form
 
     @classproperty
     def data_source(cls):
         """The system or data source providing input data for this sync."""
         return getattr(cls.Meta, "data_source", cls.name)
 
@@ -299,69 +283,62 @@
         return getattr(cls.Meta, "data_source_icon", None)
 
     @classproperty
     def data_target_icon(cls):
         """Icon corresponding to the data_target."""
         return getattr(cls.Meta, "data_target_icon", None)
 
-    def run(self, data, commit):
+    def run(self, dryrun, memory_profiling, *args, **kwargs):  # pylint:disable=arguments-differ
         """Job entry point from Nautobot - do not override!"""
         self.sync = Sync.objects.create(
             source=self.data_source,
             target=self.data_target,
-            dry_run=data["dry_run"],
+            dry_run=dryrun,
             job_result=self.job_result,
             start_time=timezone.now(),
             diff={},
         )
 
         # Add _structlog_to_sync_log_entry as a processor for structlog calls from DiffSync
         structlog.configure(
             processors=[self._structlog_to_sync_log_entry, structlog.stdlib.render_to_log_kwargs],
             context_class=dict,
             logger_factory=structlog.stdlib.LoggerFactory(),
             wrapper_class=structlog.stdlib.BoundLogger,
             cache_logger_on_first_use=True,
         )
 
-        self.kwargs = data
-        self.commit = commit
-
         # We need to catch exceptions and handle them, because if they aren't caught here,
         # they'll be caught by the Nautobot core run_job() function, which will trigger a database
         # rollback, which will delete our above created Sync record!
         try:
-            self.sync_data()
+            self.sync_data(memory_profiling)
         except Exception as exc:  # pylint: disable=broad-except
             stacktrace = traceback.format_exc()
-            self.log_failure(message=f"An exception occurred: `{type(exc).__name__}: {exc}`\n```\n{stacktrace}\n```")
+            self.logger.error(f"An exception occurred: `{type(exc).__name__}: {exc}`\n```\n{stacktrace}\n```")
 
 
 # pylint: disable=abstract-method
 class DataSource(DataSyncBaseJob):
     """Base class for Jobs that sync data **from** another data source **to** Nautobot."""
 
-    dry_run = BooleanVar(description="Perform a dry-run, making no actual changes to Nautobot data.")
-
     @classproperty
     def data_target(cls):
         """For a DataSource this is always Nautobot."""
         return "Nautobot"
 
     @classproperty
     def data_target_icon(cls):
         """For a DataSource this is always the Nautobot logo."""
         return static("img/nautobot_logo.png")
 
 
 class DataTarget(DataSyncBaseJob):
     """Base class for Jobs that sync data **to** another data target **from** Nautobot."""
 
-    dry_run = BooleanVar(description="Perform a dry-run, making no actual changes to the remote system.")
-
     @classproperty
     def data_source(cls):
         """For a DataTarget this is always Nautobot."""
         return "Nautobot"
 
     @classproperty
     def data_source_icon(cls):
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/jobs/examples.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/jobs/examples.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 
 from typing import Optional, Mapping
 from uuid import UUID
 from django.contrib.contenttypes.models import ContentType
 from django.templatetags.static import static
 from django.urls import reverse
 
-from nautobot.dcim.models import Region, Site
-from nautobot.ipam.models import Prefix
-from nautobot.tenancy.models import Tenant
-from nautobot.extras.jobs import Job, StringVar
+from nautobot.circuits.models import CircuitTermination
+from nautobot.dcim.models import Device, DeviceRedundancyGroup, Location, LocationType, PowerPanel, Rack, RackGroup
+from nautobot.extras.jobs import StringVar
 from nautobot.extras.models import Status
+from nautobot.ipam.models import Namespace, Prefix, VLAN, VLANGroup
+from nautobot.tenancy.models import Tenant
+from nautobot.virtualization.models import Cluster
 
 from diffsync import DiffSync, DiffSyncModel
 from diffsync.enum import DiffSyncFlags
+from diffsync.exceptions import ObjectNotFound
 
 import requests
 
 from nautobot_ssot.jobs.base import DataMapping, DataSource, DataTarget
 
 
 # In a more complex Job, you would probably want to move the DiffSyncModel subclasses into a separate Python module(s).
@@ -29,59 +32,57 @@
 
 class RegionModel(DiffSyncModel):
     """Shared data model representing a Region in either of the local or remote Nautobot instances."""
 
     # Metadata about this model
     _modelname = "region"
     _identifiers = ("name",)
-    _attributes = ("slug", "description", "parent_name")
+    _attributes = ("description", "parent_name")
 
     # Data type declarations for all identifiers and attributes
     name: str
-    slug: str
     description: str
     parent_name: Optional[str]  # may be None
 
     # Not in _attributes or _identifiers, hence not included in diff calculations
     pk: Optional[UUID]
 
 
 class SiteModel(DiffSyncModel):
     """Shared data model representing a Site in either of the local or remote Nautobot instances."""
 
     # Metadata about this model
     _modelname = "site"
     _identifiers = ("name",)
     # To keep this example simple, we don't include **all** attributes of a Site here. But you could!
-    _attributes = ("slug", "status_slug", "region_name", "description")
+    _attributes = ("status", "region_name", "description")
 
     # Data type declarations for all identifiers and attributes
     name: str
-    slug: str
-    status_slug: str
-    region_name: Optional[str]  # may be None
+    status: str
+    region_name: str
     description: str
 
     # Not in _attributes or _identifiers, hence not included in diff calculations
     pk: Optional[UUID]
 
 
 class PrefixModel(DiffSyncModel):
     """Shared data model representing a Prefix in either of the local or remote Nautobot instances."""
 
     # Metadata about this model
     _modelname = "prefix"
-    _identifiers = ("prefix", "tenant_slug")
+    _identifiers = ("prefix", "tenant")
     # To keep this example simple, we don't include **all** attributes of a Prefix here. But you could!
-    _attributes = ("description", "status_slug")
+    _attributes = ("description", "status")
 
     # Data type declarations for all identifiers and attributes
     prefix: str
-    tenant_slug: str
-    status_slug: str
+    tenant: str
+    status: str
     description: str
 
     # Not in _attributes or _identifiers, hence not included in diff calculations
     pk: Optional[UUID]
 
 
 class RegionRemoteModel(RegionModel):
@@ -96,30 +97,27 @@
             ids (dict): Initial values for this model's _identifiers
             attrs (dict): Initial values for this model's _attributes
         """
         diffsync.post(
             "/api/dcim/regions/",
             {
                 "name": ids["name"],
-                "slug": attrs["slug"],
                 "description": attrs["description"],
                 "parent": {"name": attrs["parent_name"]} if attrs["parent_name"] else None,
             },
         )
         return super().create(diffsync, ids=ids, attrs=attrs)
 
     def update(self, attrs):
         """Update an existing Region record in remote Nautobot.
 
         Args:
             attrs (dict): Updated values for this record's _attributes
         """
         data = {}
-        if "slug" in attrs:
-            data["slug"] = attrs["slug"]
         if "description" in attrs:
             data["description"] = attrs["description"]
         if "parent_name" in attrs:
             if attrs["parent_name"]:
                 data["parent"] = {"name": attrs["parent_name"]}
             else:
                 data["parent"] = None
@@ -144,35 +142,32 @@
             ids (dict): Initial values for this model's _identifiers
             attrs (dict): Initial values for this model's _attributes
         """
         diffsync.post(
             "/api/dcim/sites/",
             {
                 "name": ids["name"],
-                "slug": attrs["slug"],
                 "description": attrs["description"],
-                "status": attrs["status_slug"],
+                "status": attrs["status"],
                 "region": {"name": attrs["region_name"]} if attrs["region_name"] else None,
             },
         )
         return super().create(diffsync, ids=ids, attrs=attrs)
 
     def update(self, attrs):
         """Update an existing Site record in remote Nautobot.
 
         Args:
             attrs (dict): Updated values for this record's _attributes
         """
         data = {}
-        if "slug" in attrs:
-            data["slug"] = attrs["slug"]
         if "description" in attrs:
             data["description"] = attrs["description"]
-        if "status_slug" in attrs:
-            data["status"] = attrs["status_slug"]
+        if "status" in attrs:
+            data["status"] = attrs["status"]
         if "region_name" in attrs:
             if attrs["region_name"]:
                 data["region"] = {"name": attrs["region_name"]}
             else:
                 data["region"] = None
         self.diffsync.patch(f"/api/dcim/sites/{self.pk}/", data)
         return super().update(attrs)
@@ -195,32 +190,32 @@
             ids (dict): Initial values for this model's _identifiers
             attrs (dict): Initial values for this model's _attributes
         """
         diffsync.post(
             "/api/ipam/prefixes/",
             {
                 "prefix": ids["prefix"],
-                "tenant": {"slug": ids["tenant_slug"]} if ids["tenant_slug"] else None,
+                "tenant": {"name": ids["tenant"]} if ids["tenant"] else None,
                 "description": attrs["description"],
-                "status": attrs["status_slug"],
+                "status": attrs["status"],
             },
         )
         return super().create(diffsync, ids=ids, attrs=attrs)
 
     def update(self, attrs):
         """Update an existing Site record in remote Nautobot.
 
         Args:
             attrs (dict): Updated values for this record's _attributes
         """
         data = {}
         if "description" in attrs:
             data["description"] = attrs["description"]
-        if "status_slug" in attrs:
-            data["status"] = attrs["status_slug"]
+        if "status" in attrs:
+            data["status"] = attrs["status"]
         self.diffsync.patch(f"/api/dcim/sites/{self.pk}/", data)
         return super().update(attrs)
 
     def delete(self):
         """Delete an existing Site record from remote Nautobot."""
         self.diffsync.delete(f"/api/dcim/sites/{self.pk}/")
         return super().delete()
@@ -234,45 +229,48 @@
         """Create a new Region record in local Nautobot.
 
         Args:
             diffsync (NautobotLocal): DiffSync adapter owning this Region
             ids (dict): Initial values for this model's _identifiers
             attrs (dict): Initial values for this model's _attributes
         """
-        region = Region(
+        reg_type, _ = LocationType.objects.update_or_create(name="Region", nestable=True)
+        region = Location(
             name=ids["name"],
-            slug=attrs["slug"],
             description=attrs["description"],
+            location_type=LocationType.objects.get(name="Region"),
+            status=Status.objects.get(name="Active"),
         )
         if attrs["parent_name"]:
-            region.parent = Region.objects.get(name=attrs["parent_name"])
+            region.parent = Location.objects.get(name=attrs["parent_name"], location_type=reg_type)
         region.validated_save()
         return super().create(diffsync, ids=ids, attrs=attrs)
 
     def update(self, attrs):
         """Update an existing Region record in local Nautobot.
 
         Args:
             attrs (dict): Updated values for any of this model's _attributes
         """
-        region = Region.objects.get(name=self.name)
+        region = Location.objects.get(name=self.name, location_type=LocationType.objects.get(name="Region"))
 
-        for attr_name in ("slug", "description"):
-            if attr_name in attrs:
-                setattr(region, attr_name, attrs[attr_name])
+        if "description" in attrs:
+            region.description = attrs["description"]
 
         if "parent_name" in attrs:
-            region.parent = Region.objects.get(name=attrs["parent_name"])
+            region.parent = Location.objects.get(
+                name=attrs["parent_name"], location_type=LocationType.objects.get(name="Region")
+            )
 
         region.validated_save()
         return super().update(attrs)
 
     def delete(self):
         """Delete an existing Region record from local Nautobot."""
-        region = Region.objects.get(name=self.name)
+        region = Location.objects.get(name=self.name, location_type=LocationType.objects.get(name="Region"))
         region.delete()
         return super().delete()
 
 
 class SiteLocalModel(SiteModel):
     """Implementation of Site create/update/delete methods for updating local Nautobot data."""
 
@@ -281,45 +279,62 @@
         """Create a new Site record in local Nautobot.
 
         Args:
             diffsync (NautobotLocal): DiffSync adapter owning this Site
             ids (dict): Initial values for this model's _identifiers
             attrs (dict): Initial values for this model's _attributes
         """
-        site = Site(name=ids["name"], slug=attrs["slug"], description=attrs["description"])
-        site.status = Status.objects.get(slug=attrs["status_slug"])
+        diffsync.job.logger.info(f"Creating Site {ids['name']} with ids: {ids} attrs: {attrs}")
+        site_type, created = LocationType.objects.update_or_create(
+            name="Site", nestable=False, parent=LocationType.objects.get(name="Region")
+        )
+        if created:
+            site_type.content_types.add(ContentType.objects.get_for_model(Rack))
+            site_type.content_types.add(ContentType.objects.get_for_model(RackGroup))
+            site_type.content_types.add(ContentType.objects.get_for_model(Device))
+            site_type.content_types.add(ContentType.objects.get_for_model(DeviceRedundancyGroup))
+            site_type.content_types.add(ContentType.objects.get_for_model(CircuitTermination))
+            site_type.content_types.add(ContentType.objects.get_for_model(PowerPanel))
+            site_type.content_types.add(ContentType.objects.get_for_model(VLAN))
+            site_type.content_types.add(ContentType.objects.get_for_model(VLANGroup))
+            site_type.content_types.add(ContentType.objects.get_for_model(Cluster))
+        site = Location(name=ids["name"], description=attrs["description"], location_type=site_type, parent=None)
+        site.status = Status.objects.get(name=attrs["status"])
         if attrs["region_name"]:
-            site.region = Region.objects.get(name=attrs["region_name"])
+            site.parent = Location.objects.get(
+                name=attrs["region_name"], location_type=LocationType.objects.get(name="Region")
+            )
         site.validated_save()
         return super().create(diffsync, ids=ids, attrs=attrs)
 
     def update(self, attrs):
         """Update an existing Site record in local Nautobot.
 
         Args:
             attrs (dict): Updated values for any of this model's _attributes
         """
-        site = Site.objects.get(name=self.name)
+        site = Location.objects.get(name=self.name, location_type=LocationType.objects.get(name="Site"))
 
-        for attr_name in ("slug", "description"):
-            if attr_name in attrs:
-                setattr(site, attr_name, attrs[attr_name])
+        if "description" in attrs:
+            site.description = attrs["description"]
 
-        if "status_slug" in attrs:
-            site.status = Status.objects.get(slug=attrs["status_slug"])
+        if "status" in attrs:
+            site.status = Status.objects.get(name=attrs["status"])
 
         if "region_name" in attrs:
-            site.region = Region.objects.get(name=attrs["region_name"])
+            site.parent = Location.objects.get(
+                name=attrs["region_name"], location_type=LocationType.objects.get(name="Region")
+            )
 
         site.validated_save()
         return super().update(attrs)
 
     def delete(self):
         """Delete an existing Site record from local Nautobot."""
-        site = Site.objects.get(name=self.name)
+        site = Location.objects.get(name=self.name, location_type=LocationType.objects.get_or_create(name="Site")[0])
         site.delete()
         return super().delete()
 
 
 class PrefixLocalModel(PrefixModel):
     """Implementation of Prefix create/update/delete methods for updating local Nautobot data."""
 
@@ -328,54 +343,59 @@
         """Create a new Prefix record in local Nautobot.
 
         Args:
             diffsync (NautobotLocal): DiffSync adapter owning this Prefix
             ids (dict): Initial values for this model's _identifiers
             attrs (dict): Initial values for this model's _attributes
         """
+        diffsync.job.logger.info(f"Creating Prefix {ids['prefix']} with ids: {ids} attrs: {attrs}")
         prefix = Prefix(prefix=ids["prefix"], description=attrs["description"])
-        if ids["tenant_slug"]:
+        if ids["tenant"]:
             tenant_obj, _ = Tenant.objects.get_or_create(
-                slug=ids["tenant_slug"],
-                defaults={"name": ids["tenant_slug"]},
+                name=ids["tenant"],
+                defaults={"name": ids["tenant"]},
             )
             prefix.tenant = tenant_obj
+            namespace_obj, _ = Namespace.objects.get_or_create(
+                name=ids["tenant"],
+                defaults={"name": ids["tenant"]},
+            )
+            prefix.namespace = namespace_obj
 
         status_obj, _ = Status.objects.get_or_create(
-            slug=attrs["status_slug"],
-            defaults={"name": attrs["status_slug"]},
+            name=attrs["status"],
+            defaults={"name": attrs["status"]},
         )
         status_obj.content_types.add(ContentType.objects.get_for_model(Prefix))
         prefix.status = status_obj
         prefix.validated_save()
         return super().create(diffsync, ids=ids, attrs=attrs)
 
     def update(self, attrs):
         """Update an existing Prefix record in local Nautobot.
 
         Args:
             attrs (dict): Updated values for any of this model's _attributes
         """
-        prefix = Prefix.objects.get(prefix=self.prefix, tenant__slug=self.tenant_slug)
-        for attr_name in ("description",):
-            if attr_name in attrs:
-                setattr(prefix, attr_name, attrs[attr_name])
+        prefix = Prefix.objects.get(prefix=self.prefix, tenant__name=self.tenant)
+        if "description" in attrs:
+            prefix.description = attrs["description"]
 
-        if "status_slug" in attrs:
+        if "status" in attrs:
             status_obj, _ = Status.objects.get_or_create(
-                defaults={"name": attrs["status_slug"]},
+                defaults={"name": attrs["status"]},
             )
             status_obj.content_types.add(ContentType.objects.get_for_model(Prefix))
             prefix.status = status_obj
         prefix.validated_save()
         return super().update(attrs)
 
     def delete(self):
         """Delete an existing Prefix record from local Nautobot."""
-        prefix = Prefix.objects.get(prefix=self.prefix, tenant__slug=self.tenant_slug)
+        prefix = Prefix.objects.get(prefix=self.prefix, tenant__name=self.tenant)
         prefix.delete()
         return super().delete()
 
 
 # In a more complex Job, you would probably want to move each DiffSync subclass into a separate Python module.
 
 
@@ -401,82 +421,93 @@
             url (str): URL of the remote Nautobot system
             token (str): REST API authentication token
             job (Job): The running Job instance that owns this DiffSync adapter instance
         """
         super().__init__(*args, **kwargs)
         if not url or not token:
             raise ValueError("Both url and token must be specified!")
+        if not url.startswith("http"):
+            raise ValueError("The url must start with a schema.")
         self.url = url
         self.token = token
         self.job = job
         self.headers = {
             "Accept": "application/json",
             "Authorization": f"Token {self.token}",
         }
 
     def _get_api_data(self, url_path: str) -> Mapping:
         """Returns data from a url_path using pagination."""
-        data = requests.get(f"{self.url}/{url_path}", headers=self.headers, params={"limit": 0}).json()
+        data = requests.get(f"{self.url}/{url_path}", headers=self.headers, params={"limit": 0}, timeout=60).json()
         result_data = data["results"]
         while data["next"]:
-            data = requests.get(data["next"], headers=self.headers, params={"limit": 0}).json()
+            data = requests.get(data["next"], headers=self.headers, params={"limit": 0}, timeout=60).json()
             result_data.extend(data["results"])
         return result_data
 
     def load(self):
         """Load Region and Site data from the remote Nautobot instance."""
         for region_entry in self._get_api_data("api/dcim/regions/"):
             region = self.region(
                 name=region_entry["name"],
-                slug=region_entry["slug"],
                 description=region_entry["description"],
                 parent_name=region_entry["parent"]["name"] if region_entry["parent"] else None,
                 pk=region_entry["id"],
             )
             self.add(region)
-            self.job.log_debug(message=f"Loaded {region} from remote Nautobot instance")
+            self.job.logger.debug(f"Loaded {region} from remote Nautobot instance")
 
         for site_entry in self._get_api_data("api/dcim/sites/"):
             site = self.site(
                 name=site_entry["name"],
-                slug=site_entry["slug"],
-                status_slug=site_entry["status"]["value"],
-                region_name=site_entry["region"]["name"] if site_entry["region"] else None,
+                status=site_entry["status"]["label"] if site_entry.get("status") else "Active",
+                region_name=site_entry["region"]["name"] if site_entry["region"] else "Global",
                 description=site_entry["description"],
                 pk=site_entry["id"],
             )
             self.add(site)
-            self.job.log_debug(message=f"Loaded {site} from remote Nautobot instance")
+            self.job.logger.debug(f"Loaded {site} from remote Nautobot instance")
+            if site.region_name == "Global":
+                try:
+                    self.get(self.region, "Global")
+                except ObjectNotFound:
+                    global_region = self.region(
+                        name="Global",
+                        description="Region created for Sites without assigned Region from SSoT import.",
+                        parent_name=None,
+                        pk=None,
+                    )
+                    self.add(global_region)
 
         for prefix_entry in self._get_api_data("api/ipam/prefixes/"):
             prefix = self.prefix(
                 prefix=prefix_entry["prefix"],
                 description=prefix_entry["description"],
-                status_slug=prefix_entry["status"]["value"],
-                tenant_slug=prefix_entry["tenant"]["slug"] if prefix_entry["tenant"] else "",
+                status=prefix_entry["status"]["label"] if prefix_entry.get("status") else "Active",
+                tenant=prefix_entry["tenant"]["name"] if prefix_entry["tenant"] else "",
                 pk=prefix_entry["id"],
             )
             self.add(prefix)
-            self.job.log_debug(message=f"Loaded {prefix} from remote Nautobot instance")
+            self.job.logger.debug(f"Loaded {prefix} from remote Nautobot instance")
 
     def post(self, path, data):
         """Send an appropriately constructed HTTP POST request."""
-        response = requests.post(f"{self.url}{path}", headers=self.headers, json=data)
+        response = requests.post(f"{self.url}{path}", headers=self.headers, json=data, timeout=60)
         response.raise_for_status()
         return response
 
     def patch(self, path, data):
         """Send an appropriately constructed HTTP PATCH request."""
-        response = requests.patch(f"{self.url}{path}", headers=self.headers, json=data)
+        response = requests.patch(f"{self.url}{path}", headers=self.headers, json=data, timeout=60)
         response.raise_for_status()
         return response
 
     def delete(self, path):
         """Send an appropriately constructed HTTP DELETE request."""
-        response = requests.delete(f"{self.url}{path}", headers=self.headers)
+        response = requests.delete(f"{self.url}{path}", headers=self.headers, timeout=60)
         response.raise_for_status()
         return response
 
 
 class NautobotLocal(DiffSync):
     """DiffSync adapter class for loading data from the local Nautobot instance."""
 
@@ -491,166 +522,179 @@
     def __init__(self, *args, job=None, **kwargs):
         """Instantiate this class, but do not load data immediately from the local system."""
         super().__init__(*args, **kwargs)
         self.job = job
 
     def load(self):
         """Load Region and Site data from the local Nautobot instance."""
-        for region in Region.objects.all():
-            region_model = self.region(
-                name=region.name,
-                slug=region.slug,
-                description=region.description,
-                parent_name=region.parent.name if region.parent else None,
-                pk=region.pk,
-            )
-            self.add(region_model)
-            self.job.log_debug(message=f"Loaded {region_model} from local Nautobot instance")
+        for location in Location.objects.all():
+            if location.location_type.name == "Region":
+                region_model = self.region(
+                    name=location.name,
+                    description=location.description,
+                    parent_name=location.parent.name if location.parent else None,
+                    pk=location.pk,
+                )
+                self.add(region_model)
+                self.job.logger.debug(f"Loaded {region_model} from local Nautobot instance")
 
-        for site in Site.objects.all():
-            site_model = self.site(
-                name=site.name,
-                slug=site.slug,
-                status_slug=site.status.slug,
-                region_name=site.region.name if site.region else None,
-                description=site.description,
-                pk=site.pk,
-            )
-            self.add(site_model)
-            self.job.log_debug(message=f"Loaded {site_model} from local Nautobot instance")
+            if location.location_type.name == "Site":
+                site_model = self.site(
+                    name=location.name,
+                    status=location.status.name,
+                    region_name=location.parent.name if location.parent else "",
+                    description=location.description,
+                    pk=location.pk,
+                )
+                self.add(site_model)
+                self.job.logger.debug(f"Loaded {site_model} from local Nautobot instance")
 
         for prefix in Prefix.objects.all():
             prefix_model = self.prefix(
                 prefix=str(prefix.prefix),
                 description=prefix.description,
-                status_slug=prefix.status.slug,
-                tenant_slug=prefix.tenant.slug if prefix.tenant else "",
+                status=prefix.status.name,
+                tenant=prefix.tenant.name if prefix.tenant else "",
                 pk=prefix.pk,
             )
             self.add(prefix_model)
-            self.job.log_debug(message=f"Loaded {prefix_model} from local Nautobot instance")
+            self.job.logger.debug(f"Loaded {prefix_model} from local Nautobot instance")
 
 
 # The actual Data Source and Data Target Jobs are relatively simple to implement
 # once you have the above DiffSync scaffolding in place.
 
 
-class ExampleDataSource(DataSource, Job):
+class ExampleDataSource(DataSource):
     """Sync Region and Site data from a remote Nautobot instance into the local Nautobot instance."""
 
     source_url = StringVar(
         description="Remote Nautobot instance to load Sites and Regions from", default="https://demo.nautobot.com"
     )
     source_token = StringVar(description="REST API authentication token for remote Nautobot instance", default="a" * 40)
 
     def __init__(self):
         """Initialize ExampleDataSource."""
         super().__init__()
-        self.diffsync_flags = self.diffsync_flags | DiffSyncFlags.SKIP_UNMATCHED_DST
+        self.diffsync_flags = (
+            self.diffsync_flags | DiffSyncFlags.SKIP_UNMATCHED_DST  # pylint:disable=unsupported-binary-operation
+        )
 
     class Meta:
         """Metaclass attributes of ExampleDataSource."""
 
         name = "Example Data Source"
         description = 'Example "data source" Job for loading data into Nautobot from another system.'
         data_source = "Nautobot (remote)"
         data_source_icon = static("img/nautobot_logo.png")
 
     @classmethod
     def data_mappings(cls):
         """This Job maps Region and Site objects from the remote system to the local system."""
         return (
-            DataMapping("Region (remote)", None, "Region (local)", reverse("dcim:region_list")),
-            DataMapping("Site (remote)", None, "Site (local)", reverse("dcim:site_list")),
+            DataMapping("Region (remote)", None, "Region (local)", reverse("dcim:location_list")),
+            DataMapping("Site (remote)", None, "Site (local)", reverse("dcim:location_list")),
             DataMapping("Prefix (remote)", None, "Prefix (local)", reverse("ipam:prefix_list")),
         )
 
+    def run(
+        self, dryrun, memory_profiling, source_url, source_token, *args, **kwargs
+    ):  # pylint:disable=arguments-differ
+        """Run sync."""
+        self.dryrun = dryrun
+        self.memory_profiling = memory_profiling
+        self.source_url = source_url
+        self.source_token = source_token
+        super().run(dryrun, memory_profiling, *args, **kwargs)
+
     def load_source_adapter(self):
         """Method to instantiate and load the SOURCE adapter into `self.source_adapter`."""
-        self.source_adapter = NautobotRemote(url=self.kwargs["source_url"], token=self.kwargs["source_token"], job=self)
+        self.source_adapter = NautobotRemote(url=self.source_url, token=self.source_token, job=self)
         self.source_adapter.load()
 
     def load_target_adapter(self):
         """Method to instantiate and load the TARGET adapter into `self.target_adapter`."""
         self.target_adapter = NautobotLocal(job=self)
         self.target_adapter.load()
 
     def lookup_object(self, model_name, unique_id):
         """Look up a Nautobot object based on the DiffSync model name and unique ID."""
         if model_name == "region":
             try:
-                return Region.objects.get(name=unique_id)
-            except Region.DoesNotExist:
+                return Location.objects.get(name=unique_id, location_type=LocationType.objects.get(name="Region"))
+            except Location.DoesNotExist:
                 pass
         elif model_name == "site":
             try:
-                return Site.objects.get(name=unique_id)
-            except Site.DoesNotExist:
+                return Location.objects.get(name=unique_id, location_type=LocationType.objects.get(name="Site"))
+            except Location.DoesNotExist:
                 pass
         elif model_name == "prefix":
             try:
                 return Prefix.objects.get(
-                    prefix=unique_id.split("__")[0], tenant__slug=unique_id.split("__")[1] or None
+                    prefix=unique_id.split("__")[0], tenant__name=unique_id.split("__")[1] or None
                 )
             except Prefix.DoesNotExist:
                 pass
         return None
 
 
-class ExampleDataTarget(DataTarget, Job):
+class ExampleDataTarget(DataTarget):
     """Sync Region and Site data from the local Nautobot instance to a remote Nautobot instance."""
 
     target_url = StringVar(description="Remote Nautobot instance to update", default="https://demo.nautobot.com")
     target_token = StringVar(description="REST API authentication token for remote Nautobot instance", default="a" * 40)
 
     def __init__(self):
         """Initialize ExampleDataTarget."""
         super().__init__()
-        self.diffsync_flags = self.diffsync_flags | DiffSyncFlags.SKIP_UNMATCHED_DST
+        self.diffsync_flags = (
+            self.diffsync_flags | DiffSyncFlags.SKIP_UNMATCHED_DST  # pylint:disable=unsupported-binary-operation
+        )
 
     class Meta:
         """Metaclass attributes of ExampleDataTarget."""
 
         name = "Example Data Target"
         description = 'Example "data target" Job for syncing data from Nautobot to another system'
         data_target = "Nautobot (remote)"
         data_target_icon = static("img/nautobot_logo.png")
 
     @classmethod
     def data_mappings(cls):
         """This Job maps Region and Site objects from the local system to the remote system."""
         return (
-            DataMapping("Region (local)", reverse("dcim:region_list"), "Region (remote)", None),
-            DataMapping("Site (local)", reverse("dcim:site_list"), "Site (remote)", None),
+            DataMapping("Region (local)", reverse("dcim:location_list"), "Region (remote)", None),
+            DataMapping("Site (local)", reverse("dcim:location_list"), "Site (remote)", None),
             DataMapping("Prefix (local)", reverse("ipam:prefix_list"), "Prefix (remote)", None),
         )
 
     def load_source_adapter(self):
         """Method to instantiate and load the SOURCE adapter into `self.source_adapter`."""
         self.source_adapter = NautobotLocal(job=self)
         self.source_adapter.load()
 
     def load_target_adapter(self):
         """Method to instantiate and load the TARGET adapter into `self.target_adapter`."""
-        self.target_adapter = NautobotRemote(url=self.kwargs["target_url"], token=self.kwargs["target_token"], job=self)
+        self.target_adapter = NautobotRemote(url=self.target_url, token=self.target_token, job=self)
         self.target_adapter.load()
 
     def lookup_object(self, model_name, unique_id):
         """Look up a Nautobot object based on the DiffSync model name and unique ID."""
         if model_name == "region":
             try:
-                return Region.objects.get(name=unique_id)
-            except Region.DoesNotExist:
+                return Location.objects.get(name=unique_id, location_type=LocationType.objects.get(name="Region"))
+            except Location.DoesNotExist:
                 pass
         elif model_name == "site":
             try:
-                return Site.objects.get(name=unique_id)
-            except Site.DoesNotExist:
+                return Location.objects.get(name=unique_id, location_type=LocationType.objects.get(name="Site"))
+            except Location.DoesNotExist:
                 pass
         elif model_name == "prefix":
             try:
                 return Prefix.objects.get(
-                    prefix=unique_id.split("__")[0], tenant__slug=unique_id.split("__")[1] or None
+                    prefix=unique_id.split("__")[0], tenant__name=unique_id.split("__")[1] or None
                 )
             except Prefix.DoesNotExist:
                 pass
         return None
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/migrations/0001_initial.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/migrations/0002_performance_metrics.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/migrations/0002_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/models.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.urls import reverse
 from django.utils.formats import date_format
 from django.utils.timezone import now
 
 from nautobot.core.models import BaseModel
+from nautobot.extras.choices import JobResultStatusChoices
 from nautobot.extras.models import JobResult
 from nautobot.extras.utils import extras_features
 
 from .choices import SyncLogEntryActionChoices, SyncLogEntryStatusChoices
 
 
 @extras_features(
@@ -42,15 +43,15 @@
     Essentially an extension of the JobResult model to add a few additional fields.
     """
 
     source = models.CharField(max_length=64, help_text="System data is read from")
     target = models.CharField(max_length=64, help_text="System data is written to")
 
     start_time = models.DateTimeField(blank=True, null=True)
-    # end_time is represented by the job_result.completed field
+    # end_time is represented by the job_result.date_done field
     source_load_time = models.DurationField(blank=True, null=True)
     target_load_time = models.DurationField(blank=True, null=True)
     diff_time = models.DurationField(blank=True, null=True)
     sync_time = models.DurationField(blank=True, null=True)
     source_load_memory_final = models.PositiveBigIntegerField(blank=True, null=True)
     source_load_memory_peak = models.PositiveBigIntegerField(blank=True, null=True)
     target_load_memory_final = models.PositiveBigIntegerField(blank=True, null=True)
@@ -73,15 +74,15 @@
 
         ordering = ["start_time"]
 
     def __str__(self):
         """String representation of a Sync instance."""
         return f"{self.source} → {self.target}, {date_format(self.start_time, format=settings.SHORT_DATETIME_FORMAT)}"
 
-    def get_absolute_url(self):
+    def get_absolute_url(self, api=False):
         """Get the detail-view URL for this instance."""
         return reverse("plugins:nautobot_ssot:sync", kwargs={"pk": self.pk})
 
     @classmethod
     def annotated_queryset(cls):
         """Construct an efficient queryset for this model and related data."""
         return (
@@ -100,21 +101,22 @@
                 ),
                 num_failed=models.Count("log", filter=models.Q(log__status=SyncLogEntryStatusChoices.STATUS_FAILURE)),
                 num_errored=models.Count("log", filter=models.Q(log__status=SyncLogEntryStatusChoices.STATUS_ERROR)),
             )
         )
 
     @property
-    def duration(self):
+    def duration(self):  # pylint: disable=inconsistent-return-statements
         """Total execution time of this Sync."""
         if not self.start_time:
             return timedelta()  # zero
-        if not self.job_result or not self.job_result.completed:
+        if not self.job_result or self.job_result.status == JobResultStatusChoices.STATUS_PENDING:
             return now() - self.start_time
-        return self.job_result.completed - self.start_time
+        if self.job_result and self.job_result.date_done:
+            return self.job_result.date_done - self.start_time
 
     def get_source_url(self):
         """Get the absolute url of the source worker associated with this instance."""
         if self.source == "Nautobot" or not self.job_result:
             return None
         return reverse(
             "plugins:nautobot_ssot:data_source",
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/navigation.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/navigation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 """Plugin additions to the Nautobot navigation menu."""
 
-from nautobot.extras.plugins import PluginMenuItem
+from nautobot.apps.ui import NavMenuGroup, NavMenuItem, NavMenuTab
 
 
-menu_items = (
-    PluginMenuItem(
+items = [
+    NavMenuItem(
         link="plugins:nautobot_ssot:dashboard",
-        link_text="Dashboard",
+        name="Dashboard",
         permissions=["nautobot_ssot.view_sync"],
     ),
-    PluginMenuItem(
+    NavMenuItem(
         link="plugins:nautobot_ssot:sync_list",
-        link_text="History",
+        name="History",
         permissions=["nautobot_ssot.view_sync"],
     ),
-    PluginMenuItem(
+    NavMenuItem(
         link="plugins:nautobot_ssot:synclogentry_list",
-        link_text="Logs",
+        name="Logs",
         permissions=["nautobot_ssot.view_synclogentry"],
     ),
+]
+
+menu_items = (
+    NavMenuTab(
+        name="Plugins",
+        groups=(NavMenuGroup(name="Single Source of Truth", weight=1000, items=tuple(items)),),
+    ),
 )
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/tables.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Data tables for Single Source of Truth (SSOT) views."""
 from django_tables2 import Column, DateTimeColumn, JSONColumn, LinkColumn, TemplateColumn
 
-from nautobot.utilities.tables import BaseTable, ToggleColumn
+from nautobot.apps.tables import BaseTable, ToggleColumn
 
 from .choices import SyncLogEntryActionChoices, SyncLogEntryStatusChoices
 from .models import Sync, SyncLogEntry
 
 
 ACTION_LOGS_LINK = """
 <a class="{{ link_class }}"
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/template_content.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/dashboard.html` & `nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/dashboard.html`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/data_source_target.html` & `nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/data_source_target.html`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_detail.html` & `nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/sync_detail.html`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_header.html` & `nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/sync_header.html`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html` & `nautobot_ssot-2.0.0b1/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 {% for sync in syncs %}
     <a href="{% url 'plugins:nautobot_ssot:sync' pk=sync.pk %}" class="label
-        {% if sync.job_result.status == 'completed' %}label-success
-        {% elif sync.job_result.status == 'failed' %}label-danger
-        {% elif sync.job_result.status == 'errored' %}label-danger
-        {% elif sync.job_result.status == 'pending' %}label-default
-        {% elif sync.job_result.status == 'running' %}label-warning
+        {% if sync.job_result.status == 'SUCCESS' %}label-success
+        {% elif sync.job_result.status == 'FAILURE' %}label-danger
+        {% elif sync.job_result.status == 'RECEIVED' %}label-default
+        {% elif sync.job_result.status == 'REVOKED' %}label-danger
+        {% elif sync.job_result.status == 'RETRY' %}label-warning
+        {% elif sync.job_result.status == 'PENDING' %}label-default
+        {% elif sync.job_result.status == 'STARTED' %}label-warning
         {% endif %}"
         title="{{ sync }}">
     </a>
     &nbsp;
 {% endfor %}
 <span class="badge" title="Total syncs">{{ count }}</span>
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/templatetags/dashboard_helpers.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/templatetags/dashboard_helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/templatetags/humanize_bytes.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/templatetags/humanize_bytes.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/templatetags/render_diff.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/templatetags/render_diff.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/templatetags/shorter_timedelta.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/templatetags/shorter_timedelta.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/tests/jobs/__init__.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/tests/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/tests/test_api.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/tests/test_jobs.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/tests/test_jobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """Test the Job classes in nautobot_ssot."""
 import os.path
 from unittest.mock import Mock
-import uuid
-from django.contrib.contenttypes.models import ContentType
 
-from django.forms import HiddenInput
 from django.test import override_settings
 
 # from django.test import TestCase
 
 from nautobot.extras.models import JobResult
-from nautobot.utilities.testing import TransactionTestCase
+from nautobot.core.testing import TransactionTestCase
 
 from nautobot_ssot.choices import SyncLogEntryActionChoices, SyncLogEntryStatusChoices
 from nautobot_ssot.tests.jobs import DataSyncBaseJob, DataSource, DataTarget
 from nautobot_ssot.models import SyncLogEntry
 
 
 @override_settings(JOBS_ROOT=os.path.join(os.path.dirname(__file__), "jobs"))
@@ -29,26 +26,24 @@
 
     def setUp(self):
         """Per-test setup."""
         self.job = self.job_class()
 
         self.job.job_result = JobResult.objects.create(
             name="fake job",
-            obj_type=ContentType.objects.get(app_label="extras", model="job"),
-            job_id=uuid.uuid4(),
+            task_name="fake job",
+            worker="default",
         )
 
-        # name=self.job.class_path,
-
         self.job.load_source_adapter = lambda *x, **y: None
         self.job.load_target_adapter = lambda *x, **y: None
 
     def test_sync_log(self):
         """Test the sync_log() method."""
-        self.job.run(data={"dry_run": True, "memory_profiling": False}, commit=True)
+        self.job.run(dryrun=True, memory_profiling=False)
         self.assertIsNotNone(self.job.sync)
         # Minimal parameters
         self.job.sync_log(
             action=SyncLogEntryActionChoices.ACTION_CREATE,
             status=SyncLogEntryStatusChoices.STATUS_SUCCESS,
         )
         # Maximal parameters
@@ -63,17 +58,15 @@
 
         self.assertEqual(2, SyncLogEntry.objects.count())
 
     def test_as_form(self):
         """Test the as_form() method."""
         form = self.job.as_form()
         # Dry run flag defaults to true unless configured otherwise
-        self.assertTrue(form.fields["dry_run"].initial)
-        # Commit field is hidden to reduce user confusion
-        self.assertIsInstance(form.fields["_commit"].widget, HiddenInput)
+        self.assertTrue(form.fields["dryrun"].initial)
 
     def test_data_source(self):
         """Test the data_source property."""
         self.assertEqual(self.job.data_source, self.job_class.__name__)
 
     def test_data_target(self):
         """Test the data_target property."""
@@ -85,23 +78,23 @@
 
     def test_data_target_icon(self):
         """Test the data_target_icon property."""
         self.assertIsNone(self.job.data_target_icon)
 
     def test_run(self):
         """Test the run() method."""
-        self.job.run(data={"dry_run": True, "memory_profiling": False}, commit=True)
+        self.job.run(dryrun=True, memory_profiling=False)
         self.assertIsNotNone(self.job.sync)
         self.assertIsNotNone(self.job.sync.source_load_time)
         self.assertIsNotNone(self.job.sync.target_load_time)
         self.assertIsNotNone(self.job.sync.diff_time)
         self.assertIsNone(self.job.sync.sync_time)
         self.assertEqual(self.job.sync.source, self.job.data_source)
         self.assertEqual(self.job.sync.target, self.job.data_target)
-        self.assertTrue(self.job.sync.dry_run)
+        self.assertTrue(self.job.dryrun)
         self.assertEqual(self.job.job_result, self.job.sync.job_result)
 
     def test_calculate_diff(self):
         """Test calculate_diff() method."""
         self.job.sync = Mock()
         self.job.source_adapter = Mock()
         self.job.target_adapter = Mock()
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/tests/test_render_diff.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/tests/test_render_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
             }
         },
         '<ul><li>model_name<ul><li class="diff-subtracted">element<ul><li class="diff-subtracted">description: &lt;script&gt;alert(document.cookie)&lt;/script&gt;</li></ul></li></ul></li></ul>',
     ),
 ]
 
 
+@unittest.skip("TODO")
 class TestRenderDiff(unittest.TestCase):
     """Tests for render_diff function."""
 
     def test_render_diff_as_expected(self):
         """Testing expected escaped and rendered HTML."""
         for input_dict, rendered_diff in test_params:
             with self.subTest():
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/tests/test_views.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/tests/test_views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """View test cases for nautobot_ssot."""
 
 from datetime import datetime
-import uuid
 from unittest import skip
 
 from django.contrib.contenttypes.models import ContentType
 from django.urls import reverse
 
 from nautobot.extras.models import Job, JobResult
 from nautobot.users.models import ObjectPermission
-from nautobot.utilities.testing import ViewTestCases
-from nautobot.utilities.testing.utils import disable_warnings
+from nautobot.apps.testing import ViewTestCases
+from nautobot.core.testing.utils import disable_warnings
 
 from nautobot_ssot.choices import SyncLogEntryActionChoices, SyncLogEntryStatusChoices
 from nautobot_ssot.models import Sync, SyncLogEntry
 
 
 class SyncViewsTestCase(  # pylint: disable=too-many-ancestors
     ViewTestCases.ListObjectsViewTestCase,
@@ -27,18 +26,17 @@
     model = Sync
 
     @classmethod
     def setUpTestData(cls):
         """One-time setup of test data for this class."""
         for i in range(0, 3):
             job_result = JobResult.objects.create(
-                name="plugins/nautobot_ssot.jobs.examples/ExampleDataSource",
-                obj_type=ContentType.objects.get_for_model(Job),
-                data={},
-                job_id=uuid.uuid4(),
+                name="ExampleDataSource",
+                task_name="nautobot_ssot.jobs.examples.ExampleDataSource",
+                worker="default",
             )
             Sync.objects.create(
                 source="Example Data Source",
                 target="Nautobot",
                 start_time=datetime.now(),
                 dry_run=bool(i % 2),
                 diff={},
@@ -79,15 +77,15 @@
         obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
 
         with disable_warnings("django.request"):
             self.assertHttpStatus(
                 self.client.get(
                     reverse(
                         "plugins:nautobot_ssot:data_source",
-                        kwargs={"class_path": "plugins/nautobot_ssot.jobs.examples/ExampleDataSource"},
+                        kwargs={"class_path": "nautobot_ssot.jobs.examples.ExampleDataSource"},
                     )
                 ),
                 403,
             )
 
     def test_data_source_target_view_with_permission(self):
         """Test the DataSourceTargetView."""
@@ -96,15 +94,15 @@
         obj_perm.users.add(self.user)
         obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
         obj_perm.object_types.add(ContentType.objects.get_for_model(Job))
         self.assertHttpStatus(
             self.client.get(
                 reverse(
                     "plugins:nautobot_ssot:data_source",
-                    kwargs={"class_path": "plugins/nautobot_ssot.jobs.examples/ExampleDataSource"},
+                    kwargs={"class_path": "nautobot_ssot.jobs.examples.ExampleDataSource"},
                 )
             ),
             200,
         )
 
     def test_has_advanced_tab(self):
         pass
@@ -119,18 +117,17 @@
 
     model = SyncLogEntry
 
     @classmethod
     def setUpTestData(cls):
         """One-time setup of test data for this class."""
         job_result = JobResult.objects.create(
-            name="plugins/nautobot_ssot.jobs.examples/ExampleDataSource",
-            obj_type=ContentType.objects.get_for_model(Job),
-            data={},
-            job_id=uuid.uuid4(),
+            name="ExampleDataSource",
+            task_name="nautobot_ssot.jobs.examples.ExampleDataSource",
+            worker="default",
         )
         sync = Sync.objects.create(
             source="Example Data Source",
             target="Nautobot",
             start_time=datetime.now(),
             dry_run=False,
             diff={},
@@ -150,7 +147,23 @@
 
     def test_has_advanced_tab(self):
         pass
 
     @skip("Not implemented")
     def test_list_objects_with_permission(self):
         pass
+
+    @skip("Not implemented")
+    def test_list_objects_anonymous(self):
+        pass
+
+    @skip("Not implemented")
+    def test_list_objects_filtered(self):
+        pass
+
+    @skip("Not implemented")
+    def test_list_objects_with_constrained_permission(self):
+        pass
+
+    @skip("Not implemented")
+    def test_list_objects_unknown_filter_no_strict_filtering(self):
+        pass
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/urls.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/urls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 """Django urlpatterns declaration for nautobot_ssot plugin."""
 
 from django.urls import path
 
 from . import views
+from .integrations.utils import each_enabled_integration_module
 
 urlpatterns = [
     path("", views.DashboardView.as_view(), name="dashboard"),
     path("data-sources/<path:class_path>/", views.DataSourceTargetView.as_view(), name="data_source"),
     path("data-targets/<path:class_path>/", views.DataSourceTargetView.as_view(), name="data_target"),
     path("history/", views.SyncListView.as_view(), name="sync_list"),
     path("history/delete/", views.SyncBulkDeleteView.as_view(), name="sync_bulk_delete"),
     path("history/<uuid:pk>/", views.SyncView.as_view(), name="sync"),
     path("history/<uuid:pk>/delete/", views.SyncDeleteView.as_view(), name="sync_delete"),
     path("history/<uuid:pk>/jobresult/", views.SyncJobResultView.as_view(), name="sync_jobresult"),
     path("history/<uuid:pk>/logs/", views.SyncLogEntriesView.as_view(), name="sync_logentries"),
     path("logs/", views.SyncLogEntryListView.as_view(), name="synclogentry_list"),
 ]
+
+
+def _add_integrations():
+    for module in each_enabled_integration_module("urls"):
+        urlpatterns.extend(module.urlpatterns)
+
+
+_add_integrations()
```

### Comparing `nautobot_ssot-1.3.2/nautobot_ssot/views.py` & `nautobot_ssot-2.0.0b1/nautobot_ssot/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Django views for Single Source of Truth (SSoT)."""
 
 import pprint
 
-from django.contrib.contenttypes.models import ContentType
 from django.http import Http404
 from django.shortcuts import get_object_or_404
 
 from django_tables2 import RequestConfig
 
 from nautobot.extras.models import Job as JobModel
 from nautobot.extras.jobs import get_job
 from nautobot.core.views.generic import BulkDeleteView, ObjectDeleteView, ObjectListView, ObjectView
-from nautobot.utilities.paginator import EnhancedPaginator
+from nautobot.core.views.paginator import EnhancedPaginator
 
 from .filters import SyncFilterSet, SyncLogEntryFilterSet
 from .forms import SyncFilterForm, SyncLogEntryFilterForm
-from .jobs import get_data_jobs, DataSource, DataTarget
+from .jobs.base import DataSource, DataTarget
+from .jobs import get_data_jobs
 from .models import Sync, SyncLogEntry
 from .tables import DashboardTable, SyncTable, SyncTableSingleSourceOrTarget, SyncLogEntryTable
 
 
 class DashboardView(ObjectListView):
     """Dashboard / overview of SSoT."""
 
@@ -44,23 +44,20 @@
             "queryset": self.queryset,
             "data_sources": data_sources,
             "data_targets": data_targets,
             "source": {},
             "target": {},
             "table": table,
         }
-        sync_ct = ContentType.objects.get_for_model(Sync)
         for source in context["data_sources"]:
             context["source"][source.name] = self.queryset.filter(
-                job_result__obj_type=sync_ct,
                 job_result__name=source.class_path,
             )
         for target in context["data_targets"]:
             context["target"][target.name] = self.queryset.filter(
-                job_result__obj_type=sync_ct,
                 job_result__name=target.class_path,
             )
 
         return context
 
 
 class DataSourceTargetView(ObjectView):
```

### Comparing `nautobot_ssot-1.3.2/pyproject.toml` & `nautobot_ssot-2.0.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-ssot"
-version = "v1.3.2"
+version = "v2.0.0-beta.1"
 description = "Nautobot Single Source of Truth"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-ssot"
 repository = "https://github.com/nautobot/nautobot-plugin-ssot"
 documentation = "https://nautobot-plugin-ssot.readthedocs.io"
@@ -22,56 +22,65 @@
     "README.md",
 ]
 packages = [
     { include = "nautobot_ssot" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-nautobot = "^1.4.0"
+python = ">=3.8, <3.11"
+nautobot = "2.0.0b2"
 diffsync = "^1.6.0"
 Markdown = "!=3.3.5"
+dnspython = { version = "^2.1.0", optional = true }
 packaging = ">=21.3, <24"
-prometheus-client = "~0.14.1"
+prometheus-client = "~0.16.0"
 
 [tool.poetry.dev-dependencies]
 bandit = "*"
 black = "*"
 coverage = "*"
 django-debug-toolbar = "*"
 # we need to pin flake8 because of package dependencies that cause it to downgrade and
 # therefore cause issues with linting since older versions do not take .flake8 as config
 flake8 = "^3.9.2"
 invoke = "*"
 ipython = "*"
 pydocstyle = "*"
 pylint = "*"
 pylint-django = "*"
+pylint-nautobot = "*"
 pytest = "*"
+python-dotenv = "^0.21.1"
 yamllint = "*"
 Markdown = "*"
 toml = "*"
 # Rendering docs to HTML
 mkdocs = "1.4.2"
 # Material for MkDocs theme
 mkdocs-material = "9.0.11"
 # Render custom markdown for version added/changed/remove notes
 mkdocs-version-annotations = "1.0.0"
 # Automatic documentation from sources, for MkDocs
 mkdocstrings = "0.20"
 mkdocstrings-python = "0.8.3"
+requests-mock = "^1.10.0"
 
 [tool.poetry.plugins."nautobot_ssot.data_sources"]
 "example" = "nautobot_ssot.sync.example:ExampleSyncWorker"
 
 [tool.poetry.plugins."nautobot_ssot.data_targets"]
 "example" = "nautobot_ssot.sync.example:ExampleSyncWorker"
 
 [tool.poetry.extras]
-nautobot = ["nautobot"]
+all = [
+    "dnspython",
+]
+infoblox = [
+    "dnspython",
+]
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
 include = '\.pyi?$'
 exclude = '''
 (
@@ -90,17 +99,22 @@
   | settings.py     # This is where you define files that should not be stylized by black
                      # the root of the project
 )
 '''
 
 [tool.pylint.master]
 # Include the pylint_django plugin to avoid spurious warnings about Django patterns
-load-plugins="pylint_django"
+load-plugins="pylint_django,pylint_nautobot"
 ignore=".venv"
 
+[tool.pylint-nautobot]
+supported_nautobot_versions = [
+  "2",  # Supporting 2.x.y
+]
+
 [tool.pylint.basic]
 # No docstrings required for private methods (Pylint default), or for test_ functions, or for inner Meta classes.
 no-docstring-rgx="^(_|test_|Meta$)"
 
 [tool.pylint.messages_control]
 # Line length is enforced by Black, so pylint doesn't need to check it.
 # Pylint and Black disagree about how to format multi-line arrays; Black wins.
```

### Comparing `nautobot_ssot-1.3.2/PKG-INFO` & `nautobot_ssot-2.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: nautobot-ssot
-Version: 1.3.2
+Version: 2.0.0b1
 Summary: Nautobot Single Source of Truth
 Home-page: https://github.com/nautobot/nautobot-plugin-ssot
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: nautobot
+Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: all
+Provides-Extra: infoblox
 Requires-Dist: Markdown (!=3.3.5)
 Requires-Dist: diffsync (>=1.6.0,<2.0.0)
-Requires-Dist: nautobot (>=1.4.0,<2.0.0) ; extra == "nautobot"
+Requires-Dist: dnspython (>=2.1.0,<3.0.0) ; extra == "all" or extra == "infoblox"
+Requires-Dist: nautobot (==2.0.0b2)
 Requires-Dist: packaging (>=21.3,<24)
-Requires-Dist: prometheus-client (>=0.14.1,<0.15.0)
+Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
 Project-URL: Documentation, https://nautobot-plugin-ssot.readthedocs.io
 Project-URL: Repository, https://github.com/nautobot/nautobot-plugin-ssot
 Description-Content-Type: text/markdown
 
 # Nautobot Single Source of Truth (SSoT)
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: nautobot-ssot Version: 1.3.2 Summary: Nautobot
+Metadata-Version: 2.1 Name: nautobot-ssot Version: 2.0.0b1 Summary: Nautobot
 Single Source of Truth Home-page: https://github.com/nautobot/nautobot-plugin-
 ssot License: Apache-2.0 Keywords: nautobot,nautobot-plugin Author: Network to
-Code, LLC Author-email: info@networktocode.com Requires-Python: >=3.7,<4.0
+Code, LLC Author-email: info@networktocode.com Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: nautobot Requires-Dist: Markdown (!=3.3.5) Requires-Dist:
-diffsync (>=1.6.0,<2.0.0) Requires-Dist: nautobot (>=1.4.0,<2.0.0) ; extra ==
-"nautobot" Requires-Dist: packaging (>=21.3,<24) Requires-Dist: prometheus-
-client (>=0.14.1,<0.15.0) Project-URL: Documentation, https://nautobot-plugin-
-ssot.readthedocs.io Project-URL: Repository, https://github.com/nautobot/
-nautobot-plugin-ssot Description-Content-Type: text/markdown # Nautobot Single
-Source of Truth (SSoT)
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.7 Provides-Extra: all Provides-Extra: infoblox
+Requires-Dist: Markdown (!=3.3.5) Requires-Dist: diffsync (>=1.6.0,<2.0.0)
+Requires-Dist: dnspython (>=2.1.0,<3.0.0) ; extra == "all" or extra ==
+"infoblox" Requires-Dist: nautobot (==2.0.0b2) Requires-Dist: packaging
+(>=21.3,<24) Requires-Dist: prometheus-client (>=0.16.0,<0.17.0) Project-URL:
+Documentation, https://nautobot-plugin-ssot.readthedocs.io Project-URL:
+Repository, https://github.com/nautobot/nautobot-plugin-ssot Description-
+Content-Type: text/markdown # Nautobot Single Source of Truth (SSoT)
 [https://raw.githubusercontent.com/nautobot/nautobot-plugin-ssot/develop/docs/
                         images/icon-nautobot-ssot.png]
  [https://github.com/nautobot/nautobot-plugin-ssot//actions/workflows/ci.yml/
 badge.svg?branch=main] [https://readthedocs.org/projects/nautobot-plugin-ssot/
 badge/] [https://img.shields.io/pypi/v/nautobot-ssot] [https://img.shields.io/
                             pypi/dm/nautobot-ssot]
                              An App for Nautobot.
```

