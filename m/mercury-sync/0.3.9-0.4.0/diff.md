# Comparing `tmp/mercury-sync-0.3.9.tar.gz` & `tmp/mercury-sync-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.3.9.tar", last modified: Tue Jun 27 18:57:58 2023, max compression
+gzip compressed data, was "mercury-sync-0.4.0.tar", last modified: Fri Jul 14 20:02:14 2023, max compression
```

## Comparing `mercury-sync-0.3.9.tar` & `mercury-sync-0.4.0.tar`

### file list

```diff
@@ -1,62 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.580909 mercury-sync-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.572909 mercury-sync-0.3.9/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22565 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/models/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/models/ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/service/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    39763 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/service/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.576909 mercury-sync-0.3.9/mercury_sync/types/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/types/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/mercury_sync/types/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:57:58.572909 mercury-sync-0.3.9/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-27 18:57:58.000000 mercury-sync-0.3.9/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-27 18:57:58.000000 mercury-sync-0.3.9/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:57:58.000000 mercury-sync-0.3.9/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 18:57:58.000000 mercury-sync-0.3.9/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 18:57:58.000000 mercury-sync-0.3.9/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:57:58.580909 mercury-sync-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-27 18:57:55.000000 mercury-sync-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.775679 mercury-sync-0.4.0/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.779679 mercury-sync-0.4.0/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.779679 mercury-sync-0.4.0/mercury_sync/connection/addresses/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/addresses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/addresses/subnet_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.779679 mercury-sync-0.4.0/mercury_sync/connection/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/base/connection_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.783680 mercury-sync-0.4.0/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14366 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/mercury_sync_http_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23338 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.783680 mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.783680 mercury-sync-0.4.0/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/udp/mercury_sync_udp_multicast_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.783680 mercury-sync-0.4.0/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.783680 mercury-sync-0.4.0/mercury_sync/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.787680 mercury-sync-0.4.0/mercury_sync/discovery/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.787680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.787680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/cache/cache_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/cache/cache_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.787680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/config/root.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.791679 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/dns_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/invalid_service_url_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.791679 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/exceptions/utils/get_bits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.791679 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/nameservers/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/nameservers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/nameservers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/nameservers/nameserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.791679 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/random/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/random/random_id_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.791679 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/query_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.799680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/a_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/aaaa_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/cname_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/domain_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/mx_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/naptr_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/ns_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/ptr_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/record_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/soa_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/srv_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/txt_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/unsupported_record_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.799680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/load_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/load_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/pack_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/record/record_data_types/utils/pack_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.803680 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/core/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/registrar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.803680 mercury-sync-0.4.0/mercury_sync/discovery/dns/request/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/request/dns_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.803680 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/base_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/cache_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/memoizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/proxy_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/recursive_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/dns/resolver/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.807680 mercury-sync-0.4.0/mercury_sync/discovery/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/discovery/volume/backup_volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.807680 mercury-sync-0.4.0/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.807680 mercury-sync-0.4.0/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/memory_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/monitor_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/registrar_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.811680 mercury-sync-0.4.0/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/endpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/middleware_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.811680 mercury-sync-0.4.0/mercury_sync/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.811680 mercury-sync-0.4.0/mercury_sync/middleware/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/bidirectional_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/base/unidirectional_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.815680 mercury-sync-0.4.0/mercury_sync/middleware/compressor/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/compressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/compressor/bidirectional_gzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/compressor/bidirectional_zstandard_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/compressor/gzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/compressor/zstandard_compressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.815680 mercury-sync-0.4.0/mercury_sync/middleware/cors/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/cors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/cors/cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/cors/cors_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.815680 mercury-sync-0.4.0/mercury_sync/middleware/crsf/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/crsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/crsf/crsf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.819680 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/bidirectional_gzip_decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/bidirectional_zstandard_decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/gzip_decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/middleware/decompressor/zstandard_decompressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.819680 mercury-sync-0.4.0/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/dns_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/dns_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/dns_message_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/http_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/models/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.819680 mercury-sync-0.4.0/mercury_sync/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42916 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/monitoring/monitor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.819680 mercury-sync-0.4.0/mercury_sync/rate_limiting/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.823680 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/adaptive_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/base_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/cpu_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/leaky_bucket_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/resource_adaptive_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/sliding_window_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/rate_limiting/limiters/token_bucket_limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.823680 mercury-sync-0.4.0/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29917 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/plugin_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/mercury_sync/service/socket/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/socket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/service/socket/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/mercury_sync/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/types/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/types/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/mercury_sync/types/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:02:14.779679 mercury-sync-0.4.0/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-14 20:02:14.000000 mercury-sync-0.4.0/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-07-14 20:02:14.000000 mercury-sync-0.4.0/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:02:14.000000 mercury-sync-0.4.0/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 20:02:14.000000 mercury-sync-0.4.0/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 20:02:14.000000 mercury-sync-0.4.0/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 20:02:14.827680 mercury-sync-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-14 20:02:07.000000 mercury-sync-0.4.0/setup.py
```

### Comparing `mercury-sync-0.3.9/LICENSE` & `mercury-sync-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.9/PKG-INFO` & `mercury-sync-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.9
+Version: 0.4.0
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.9/README.md` & `mercury-sync-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.9/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.4.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import asyncio
-import errno
 import pickle
 import socket
 import ssl
 import zstandard
 from collections import deque, defaultdict
+from mercury_sync.connection.base.connection_type import ConnectionType
 from mercury_sync.encryption import AESGCMFernet
 from mercury_sync.env import Env
 from mercury_sync.env.time_parser import TimeParser
 from mercury_sync.models.message import Message
 from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
 from typing import (
     Tuple, 
@@ -57,15 +57,15 @@
         self._server: asyncio.Server = None
         self._loop: Union[asyncio.AbstractEventLoop, None] = None
         self._waiters: Dict[str, Deque[asyncio.Future]] = defaultdict(deque)
         self._pending_responses: Deque[asyncio.Task]= deque()
         self._last_call: Deque[str] = deque()
 
         self._sent_values = deque()
-        self._server_socket = None
+        self.server_socket = None
         self._stream = False
         
         self._client_key_path: Union[str, None] = None
         self._client_cert_path: Union[str, None] = None
 
         self._server_key_path: Union[str, None] = None
         self._server_cert_path: Union[str, None] = None 
@@ -79,14 +79,16 @@
         self._decompressor: Union[zstandard.ZstdDecompressor, None] = None
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._sleep_task: Union[asyncio.Task, None] = None
         self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
         self._max_concurrency = env.MERCURY_SYNC_MAX_CONCURRENCY
         self._tcp_connect_retries = env.MERCURY_SYNC_TCP_CONNECT_RETRIES
 
+        self.connection_type = ConnectionType.TCP
+
     def connect(
         self,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None,
         worker_socket: Optional[socket.socket]=None
     ):
 
@@ -107,33 +109,34 @@
         if cert_path and key_path:
             self._server_ssl_context = self._create_server_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path
             ) 
 
         if self.connected is False and worker_socket is None:
-            self._server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            self._server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-            self._server_socket.bind((self.host, self.port))
+            self.server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            self.server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            self.server_socket.bind((self.host, self.port))
 
-            self._server_socket.setblocking(False)
+            self.server_socket.setblocking(False)
 
         elif self.connected is False:
-            self._server_socket = worker_socket
+            self.server_socket = worker_socket
             host, port = worker_socket.getsockname()
+            
             self.host = host
             self.port = port
 
         if self.connected is False:
 
             server = self._loop.create_server(
                 lambda: MercurySyncTCPServerProtocol(
                     self.read
                 ),
-                sock=self._server_socket,
+                sock=self.server_socket,
                 ssl=self._server_ssl_context
             )
 
             self._server = self._loop.run_until_complete(server)
 
             self.connected = True
 
@@ -163,45 +166,43 @@
         if cert_path and key_path:
             self._server_ssl_context = self._create_server_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path
             ) 
 
         if self.connected is False and worker_socket is None:
-            self._server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            self._server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            self.server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            self.server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
             try:
-                self._server_socket.bind((self.host, self.port))
+                self.server_socket.bind((self.host, self.port))
 
             except Exception:
                 pass
 
-
-            self._server_socket
-
-            self._server_socket.setblocking(False)
+            self.server_socket.setblocking(False)
 
         elif self.connected is False:
-            self._server_socket = worker_socket
+            self.server_socket = worker_socket
             host, port = worker_socket.getsockname()
+
             self.host = host
             self.port = port
 
         if self.connected is False:
 
-            server = self._loop.create_server(
+            server = await self._loop.create_server(
                 lambda: MercurySyncTCPServerProtocol(
                     self.read
                 ),
-                sock=self._server_socket,
+                sock=self.server_socket,
                 ssl=self._server_ssl_context
             )
 
-            self._server = await server
+            self._server = server
             self.connected = True
 
             self._cleanup_task = self._loop.create_task(self._cleanup())
 
     def _create_server_ssl_context(
         self, 
         cert_path: Optional[str]=None,
@@ -227,29 +228,39 @@
 
         return ssl_ctx
 
     async def connect_client(
         self,
         address: Tuple[str, int],
         cert_path: Optional[str]=None,
-        key_path: Optional[str]=None
-    ) -> Coroutine[Any, Any, asyncio.Transport]:
+        key_path: Optional[str]=None,
+        worker_socket: Optional[socket.socket]=None,
+    ) -> None:
+        
+        if self._semaphore is None:
+            self._semaphore = asyncio.Semaphore(self._max_concurrency)
         
         self._loop = asyncio.get_event_loop()
         if cert_path and key_path:
             self._client_ssl_context = self._create_client_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path
             ) 
 
-        tcp_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        tcp_socket.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
-        await self._loop.run_in_executor(None, tcp_socket.connect, address)
+        if worker_socket is None:
+
+            tcp_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            tcp_socket.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
+            await self._loop.run_in_executor(None, tcp_socket.connect, address)
+
+            tcp_socket.setblocking(False)
 
-        tcp_socket.setblocking(False)
+        else:
+
+            tcp_socket = worker_socket
 
         last_error: Union[Exception, None] = None
 
         for _ in range(self._tcp_connect_retries):
 
             try:
 
@@ -306,22 +317,15 @@
 
             for pending in list(self._pending_responses):
                 if pending.done() or pending.cancelled():
 
                     try:
                         await pending
 
-                    except (
-                        ConnectionAbortedError,
-                        ConnectionRefusedError,
-                        ConnectionResetError,
-                        asyncio.CancelledError,
-                        asyncio.InvalidStateError,
-                        RuntimeError
-                    ):
+                    except Exception:
                         await self.close()
                         await self.connect_async(
                             cert_path=self._client_cert_path,
                             key_path=self._client_key_path
                         )
 
                     self._pending_responses.pop()
@@ -362,29 +366,52 @@
             compressed = self._compressor.compress(encrypted_message)
 
             client_transport.write(compressed)
 
             waiter = self._loop.create_future()
             self._waiters[event_name].append(waiter)
 
-            await waiter
-
             (
                 _,
                 shard_id,
                 _,
                 response_data,
                 _, 
                 _
-            ) = self.queue[event_name].pop()
+            ) = await waiter
 
             return (
                 shard_id,
                 response_data
             )
+        
+    async def send_bytes(
+        self,
+        event_name: str,
+        data: bytes,
+        address: Tuple[str, int]
+    ) -> bytes:
+        async with self._semaphore:
+            self._last_call.append(event_name)
+
+            client_transport = self._client_transports.get(address)
+            if client_transport is None:
+                await self.connect_client(
+                    address,
+                    cert_path=self._client_cert_path,
+                    key_path=self._client_key_path
+                )
+
+                client_transport = self._client_transports.get(address)
+
+            client_transport.write(data)
+
+            waiter = self._loop.create_future()
+            self._waiters[event_name].append(waiter)
+            return await waiter
     
     async def stream(
         self, 
         event_name: str,
         data: Any, 
         address: Tuple[str, int]
     ) -> AsyncIterable[Tuple[int, Dict[str, Any]]]: 
@@ -619,32 +646,30 @@
                     pass
 
         else:
 
             if event_name is None and bool(self._last_call):
                 event_name = self._last_call.pop()
 
-            self.queue[event_name].append((
-                message_type, 
-                shard_id,
-                event_name,
-                payload, 
-                incoming_host,
-                incoming_port
-            ))
-
                 
             event_waiter = self._waiters[event_name]
 
             if bool(event_waiter):
                 waiter = event_waiter.pop()
 
                 try:
 
-                    waiter.set_result(None)
+                    waiter.set_result((
+                        message_type, 
+                        shard_id,
+                        event_name,
+                        payload, 
+                        incoming_host,
+                        incoming_port
+                    ))
 
                 except asyncio.InvalidStateError:
                     pass
 
     async def _read(
         self,
         event_name: str,
```

### Comparing `mercury-sync-0.3.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.4.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.9/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.4.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import asyncio
 import pickle
 import socket
 import ssl
 import zstandard
 from collections import deque, defaultdict
 from dtls import do_patch
+from mercury_sync.connection.base.connection_type import ConnectionType
 from mercury_sync.connection.udp.protocols import MercurySyncUDPProtocol
 from mercury_sync.encryption import AESGCMFernet
 from mercury_sync.env import Env
 from mercury_sync.env.time_parser import TimeParser
 from mercury_sync.models.message import Message
 from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
 from typing import (
@@ -67,14 +68,16 @@
         self._running = False
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._sleep_task: Union[asyncio.Task, None] = None
         self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
         self._max_concurrency = env.MERCURY_SYNC_MAX_CONCURRENCY
         self.udp_socket: Union[socket.socket, None] = None
 
+        self.connection_type = ConnectionType.UDP
+
     def connect(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None,
         worker_socket: Optional[socket.socket]=None
     ) -> None:
         
@@ -90,26 +93,34 @@
 
         self._semaphore = asyncio.Semaphore(self._max_concurrency)
 
         self._compressor = zstandard.ZstdCompressor()
         self._decompressor = zstandard.ZstdDecompressor()
 
         if worker_socket is None:
-            self.udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
+            self.udp_socket = socket.socket(
+                socket.AF_INET, 
+                socket.SOCK_DGRAM, 
+                socket.IPPROTO_UDP
+            )
+
             self.udp_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             self.udp_socket.bind((
                 self.host,
                 self.port
             ))
 
             self.udp_socket.setblocking(False)
 
         else:
             self.udp_socket = worker_socket
-
+            host, port = self.udp_socket.getsockname()
+            
+            self.host = host
+            self.port = port
 
         if cert_path and key_path:
             self._udp_ssl_context = self._create_udp_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path,
             )
 
@@ -123,30 +134,14 @@
         )
 
         transport, _ = self._loop.run_until_complete(server)
         self._transport = transport
 
         self._cleanup_task = self._loop.create_task(self._cleanup())
 
-    def copy_to_connection(self, new_udp_connection: MercurySyncUDPConnection) -> MercurySyncUDPConnection:
-        new_udp_connection.parsers.update(self.parsers)
-        new_udp_connection._udp_cert_path = self._udp_cert_path
-        new_udp_connection._udp_key_path = self._udp_key_path
-        new_udp_connection._udp_ssl_context = self._udp_ssl_context
-        new_udp_connection._running = True
-
-        new_udp_connection._semaphore = asyncio.Semaphore(self._max_concurrency)
-
-        new_udp_connection._compressor = zstandard.ZstdCompressor()
-        new_udp_connection._decompressor = zstandard.ZstdDecompressor()
-        new_udp_connection._transport = self._transport
-        new_udp_connection._cleanup_task = self._loop.create_task(new_udp_connection._cleanup())
-
-        return new_udp_connection
-
     async def connect_async(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None,
         worker_socket: Optional[socket.socket]=None
     ) -> None:
         
@@ -238,15 +233,14 @@
                         asyncio.InvalidStateError
                     ):
                         await self.close()
                         await self.connect_async(
                             cert_path=self._udp_cert_path,
                             key_path=self._udp_key_path
                         )
-                    
 
                     self._pending_responses.pop()
     
     async def send(
         self, 
         event_name: str,
         data: Any, 
@@ -264,29 +258,40 @@
         compressed = self._compressor.compress(encrypted_message)
         
         self._transport.sendto(compressed, addr)
 
         waiter = self._loop.create_future()
         self._waiters[event_name].append(waiter)
 
-        await waiter
-
         (
             _,
             shard_id,
             _,
             response_data,
             _, 
             _
-        ) = self.queue[event_name].pop()
+        ) = await waiter
 
         return (
             shard_id,
             response_data
         )
+    
+    async def send_bytes(
+        self,
+        event_name: str,
+        data: bytes,
+        addr: Tuple[str, int]
+    ) -> bytes:
+        
+        self._transport.sendto(data, addr)
+
+        waiter = self._loop.create_future()
+        self._waiters[event_name].append(waiter)
+        return await waiter
 
     async def stream(
         self, 
         event_name: str,
         data: Any, 
         addr: Tuple[str, int]
     ) -> AsyncIterable[Tuple[int, Dict[str, Any]]]: 
@@ -335,29 +340,26 @@
             self._decompressor.decompress(data)
         )
 
         result: Tuple[
             str, 
             int, 
             float, 
-            Any, 
-            str, 
-            int
+            Any
         ] = pickle.loads(decrypted)
 
         (
             message_type, 
             shard_id, 
             event_name, 
             payload
         ) = result
 
         incoming_host, incoming_port = addr
 
-
         if message_type == 'request':
             self._pending_responses.append(
                 asyncio.create_task(
                     self._read(
                         event_name,
                         self.events.get(event_name)(
                             shard_id,
@@ -379,32 +381,30 @@
                         ),
                         addr
                     )
                 )
             )
 
         else:
-            self.queue[event_name].append((
-                message_type, 
-                shard_id,
-                event_name,
-                payload, 
-                incoming_host,
-                incoming_port
-            ))
 
             event_waiter = self._waiters[event_name]
-
-            
+      
             if bool(event_waiter):
                 waiter = event_waiter.pop()
                 
                 try:
                     
-                    waiter.set_result(None)
+                    waiter.set_result((
+                        message_type, 
+                        shard_id,
+                        event_name,
+                        payload, 
+                        incoming_host,
+                        incoming_port
+                    ))
                 
                 except asyncio.InvalidStateError:
                     pass
 
 
     async def _read(
         self,
```

### Comparing `mercury-sync-0.3.9/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.4.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.9/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.4.0/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.9/mercury_sync/env/load_env.py` & `mercury-sync-0.4.0/mercury_sync/env/load_env.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import os
 from dotenv import dotenv_values
 from typing import (
     Dict, 
     Union, 
-    Callable
+    Type
 )
 from .env import Env
+from .monitor_env import MonitorEnv
+from .registrar_env import RegistrarEnv
 
 
 PrimaryType=Union[str, int, bool, float, bytes]
 
 
 def load_env(
-    envars: Dict[
-        str, 
-        Callable[
-            [str],
-            PrimaryType
-        ]
+    env: Union[
+        Type[Env],
+        Type[MonitorEnv],
+        Type[RegistrarEnv]
     ],  
-    env_file: str=None   
+    env_file: str=None
 ):
+    
+    envars = env.types_map()
+    
     if env_file is None:
         env_file = '.env'
 
     values: Dict[str, PrimaryType] = {}
 
     for envar_name, envar_type in envars.items():
         envar_value = os.getenv(envar_name)
@@ -37,10 +40,10 @@
         for envar_name, envar_value in env_file_values.items():
             envar_type = envars.get(envar_name)
             if envar_type:
                 env_file_values[envar_name] = envar_type(envar_value)
 
         values.update(env_file_values)
 
-    return Env(**{
+    return env(**{
         name: value for name, value in values.items() if value is not None
     })
```

### Comparing `mercury-sync-0.3.9/mercury_sync/env/time_parser.py` & `mercury-sync-0.4.0/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.9/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.4.0/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.9/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.4.0/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.9/mercury_sync/models/healthcheck.py` & `mercury-sync-0.4.0/mercury_sync/models/healthcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pydantic import (
     StrictStr,
     StrictInt
 )
-from typing import Literal, Optional, List
+from typing import Literal, Optional
 from .message import Message
 
 
 HealthStatus = Literal[
     "initializing",
     "waiting",
     "healthy",
```

### Comparing `mercury-sync-0.3.9/mercury_sync/service/monitor.py` & `mercury-sync-0.4.0/mercury_sync/monitoring/monitor_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import asyncio
 import math
 import random
 import time
-import traceback
 from collections import defaultdict, deque
-from mercury_sync.env import Env, load_env
+from mercury_sync.env import (
+    Env, 
+    MonitorEnv,
+    load_env
+)
 from mercury_sync.env.time_parser import TimeParser
 from mercury_sync.hooks.client_hook import client
 from mercury_sync.hooks.server_hook import server
 from mercury_sync.models.healthcheck import HealthCheck, HealthStatus
-from mercury_sync.models.ticket import Ticket
+from mercury_sync.service.controller import Controller
 from mercury_sync.snowflake import Snowflake
 from mercury_sync.types import Call
 from typing import Optional, Dict, Tuple, List, Deque, Union
-from .controller import Controller
 
 
 async def cancel(pending_item: asyncio.Task) -> None:
     pending_item.cancel()
     if not pending_item.cancelled():
         try:
             await pending_item
@@ -31,26 +33,30 @@
 
 class Monitor(Controller):
 
     def __init__(
         self,
         host: str,
         port: int,
+        env: Env,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None,
         workers: int=0,
     ) -> None:
         
         if workers <= 1:
             engine = 'async'
 
         else:
             engine = 'process'
 
-        env = load_env(Env.types_map())
+        if env is None:
+            env: Env = load_env(Env)
+            
+        monitor_env: MonitorEnv = load_env(MonitorEnv)
 
         super().__init__(
             host,
             port,
             cert_path=cert_path,
             key_path=key_path,
             workers=workers,
@@ -58,49 +64,74 @@
             engine=engine
         )
 
         self.status: HealthStatus = 'initializing'
         
 
         self.error_context: Optional[str] = None
-        self.registration_timeout = TimeParser(env.MERCURY_SYNC_REGISTRATION_TIMEOUT).time
-        self.boot_wait = TimeParser(env.MERCURY_SYNC_BOOT_WAIT).time
+
+        self.registration_timeout = TimeParser(
+            monitor_env.MERCURY_SYNC_REGISTRATION_TIMEOUT
+        ).time
+
+        self.boot_wait = TimeParser(
+            monitor_env.MERCURY_SYNC_BOOT_WAIT
+        ).time
         
         self._healthchecks: Dict[str, asyncio.Task] = {}
         self._registered: Dict[int, Tuple[str, int]] = {}
         self._running = False
-        self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
-        self._poll_interval = TimeParser(env.MERCURY_SYNC_HEALTH_POLL_INTERVAL).time
-        self._poll_timeout = TimeParser(env.MERCURY_SYNC_HEALTH_CHECK_TIMEOUT).time
-        self._reboot_timeout = TimeParser(env.MERCURY_SYNC_IDLE_REBOOT_TIMEOUT).time
-        self._max_time_idle = TimeParser(env.MERCURY_SYNC_MAX_TIME_IDLE).time
-        self._poll_retries = env.MERCURY_SYNC_MAX_POLL_MULTIPLIER
-        self._sync_interval = TimeParser(env.MERCURY_SYNC_UDP_SYNC_INTERVAL).time
-
-        self._check_nodes_count = env.MERCURY_SYNC_INDIRECT_CHECK_NODES
-
-        self.min_suspect_multiplier = env.MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER
-        self.max_suspect_multiplier = env.MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER 
-        self._min_suspect_node_count = env.MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD
-        self._max_poll_multiplier = env.MERCURY_SYNC_MAX_POLL_MULTIPLIER
+
+        self._cleanup_interval = TimeParser(
+            env.MERCURY_SYNC_CLEANUP_INTERVAL
+        ).time
+
+        self._poll_interval = TimeParser(
+            monitor_env.MERCURY_SYNC_HEALTH_POLL_INTERVAL
+        ).time
+
+        self._poll_timeout = TimeParser(
+            monitor_env.MERCURY_SYNC_HEALTH_CHECK_TIMEOUT
+        ).time
+
+        self._reboot_timeout = TimeParser(
+            monitor_env.MERCURY_SYNC_IDLE_REBOOT_TIMEOUT
+        ).time
+
+        self._max_time_idle = TimeParser(
+            monitor_env.MERCURY_SYNC_MAX_TIME_IDLE
+        ).time
+
+        self._poll_retries = monitor_env.MERCURY_SYNC_MAX_POLL_MULTIPLIER
+
+        self._sync_interval = TimeParser(
+            monitor_env.MERCURY_SYNC_UDP_SYNC_INTERVAL
+        ).time
+
+        self._check_nodes_count = monitor_env.MERCURY_SYNC_INDIRECT_CHECK_NODES
+
+        self.min_suspect_multiplier = monitor_env.MERCURY_SYNC_MIN_SUSPECT_TIMEOUT_MULTIPLIER
+        self.max_suspect_multiplier = monitor_env.MERCURY_SYNC_MAX_SUSPECT_TIMEOUT_MULTIPLIER 
+        self._min_suspect_node_count = monitor_env.MERCURY_SYNC_MIN_SUSPECT_NODES_THRESHOLD
+        self._max_poll_multiplier = monitor_env.MERCURY_SYNC_MAX_POLL_MULTIPLIER
         self._local_health_multiplier = 0
 
         self._confirmed_suspicions: Dict[Tuple[str, int], int] = defaultdict(lambda: 0)
-        self._waiter: Optional[asyncio.Future] = None
+        self._waiter: Union[asyncio.Future, None] = None
 
         self._tasks_queue: Deque[asyncio.Task] = deque()
         self._degraded_nodes: Deque[Tuple[str, int]] = deque()
         self._suspect_nodes: Deque[Tuple[str, int]] = deque()
 
         self._degraded_tasks: Dict[Tuple[str, int], asyncio.Task] = {}
         self._suspect_tasks: Dict[Tuple[str, int], asyncio.Task] = {}
         self._latest_update: Dict[Tuple[str,int], int] = {}
 
         self._local_health_monitor: Union[asyncio.Task, None] = None
-        self._sync_task: Union[asyncio.Task, None] = None
+        self._udp_sync_task: Union[asyncio.Task, None] = None
         self._tcp_sync_task: Union[asyncio.Task, None] = None
 
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._investigating_nodes: Dict[Tuple[str, int], Dict[Tuple[str, int]]] = defaultdict(dict)
         self._node_statuses: Dict[Tuple[str, int], HealthStatus] = {}
 
         self.bootstrap_host: Union[str, None] = None
@@ -146,35 +177,43 @@
             update_node_port
         ), 0)
 
         not_self = update_node_host != self.host and update_node_port != self.port
 
         if not_self and local_status in self._unhealthy_statuses:
 
-            await self.refresh_clients(
-                HealthCheck(
-                    host=update_node_host,
-                    port=update_node_port,
-                    source_host=self.host,
-                    source_port=self.port,
-                    status=update_status,
-                    error=healthcheck.error
+            self._tasks_queue.append(
+                asyncio.create_task(
+                    self.refresh_clients(
+                        HealthCheck(
+                            host=update_node_host,
+                            port=update_node_port,
+                            source_host=self.host,
+                            source_port=self.port,
+                            status=update_status,
+                            error=healthcheck.error
+                        )
+                    )
                 )
             )
 
         elif not_self and local_status is None:
 
-            await self.extend_client(
-                HealthCheck(
-                    host=update_node_host,
-                    port=update_node_port,
-                    source_host=self.host,
-                    source_port=self.port,
-                    status=self.status,
-                    error=healthcheck.error
+            self._tasks_queue.append(
+                asyncio.create_task(
+                    self.extend_client(
+                        HealthCheck(
+                            host=update_node_host,
+                            port=update_node_port,
+                            source_host=self.host,
+                            source_port=self.port,
+                            status=self.status,
+                            error=healthcheck.error
+                        )
+                    )
                 )
             )
 
         if target_last_updated > local_last_updated:
             self._node_statuses[(update_node_host, update_node_port)] = update_status
 
         return HealthCheck(
@@ -197,14 +236,23 @@
 
         if self.status == 'healthy':
             self._local_health_multiplier = min(
                 self._local_health_multiplier, 
                 self._max_poll_multiplier
             ) + 1
 
+            self._tasks_queue.append(
+                asyncio.create_task(
+                    self._run_healthcheck(
+                        source_host,
+                        source_port
+                    )
+                )
+            )
+
         return HealthCheck(
             host=source_host,
             port=source_port,
             source_host=self.host,
             source_port=self.port,
             status=self.status
         )
@@ -328,34 +376,42 @@
             del self._suspect_tasks[(source_host, source_port)]
 
             self._suspect_tasks = suspect_tasks
 
 
         if local_node_status is None:
 
-            await self.extend_client(
-                HealthCheck(
-                    host=source_host,
-                    port=source_port,
-                    source_host=self.host,
-                    source_port=self.port,
-                    status=healthcheck.status,
-                    error=healthcheck.error
+            self._tasks_queue.append(
+                asyncio.create_task(
+                    self.extend_client(
+                        HealthCheck(
+                            host=source_host,
+                            port=source_port,
+                            source_host=self.host,
+                            source_port=self.port,
+                            status=healthcheck.status,
+                            error=healthcheck.error
+                        )
+                    )
                 )
             )
 
         elif local_node_status in self._unhealthy_statuses:
-            await self.refresh_clients(
-                HealthCheck(
-                    host=source_host,
-                    port=source_port,
-                    source_host=self.host,
-                    source_port=self.port,
-                    status=healthcheck.status,
-                    error=healthcheck.error
+            self._tasks_queue.append(
+                asyncio.create_task(
+                    self.refresh_clients(
+                        HealthCheck(
+                            host=source_host,
+                            port=source_port,
+                            source_host=self.host,
+                            source_port=self.port,
+                            status=healthcheck.status,
+                            error=healthcheck.error
+                        )
+                    )
                 )
             )
     
 
         self._node_statuses[(source_host, source_port)] = healthcheck.status
         self._latest_update[(source_host, source_port)] = Snowflake.parse(shard_id).timestamp
 
@@ -579,25 +635,34 @@
         health_status: HealthStatus,
         target_host: Optional[str]=None,
         target_port: Optional[int]=None,
         error_context: Optional[str]=None
     ) -> Call[HealthCheck]:
         
         target_status: Union[HealthStatus, None] = None
+        target_last_updated: Union[int,  None] = self._latest_update.get(
+            (host, port), 0
+        )
+
         if target_host and target_port:
             target_status = self._node_statuses.get((target_host, target_port))
+            target_last_updated = self._latest_update.get(
+                (target_host, target_port), 0
+            )
+
 
         return HealthCheck(
             host=host,
             port=port,
             source_host=self.host,
             source_port=self.port,
             target_host=target_host,
             target_port=target_port,
             target_status=target_status,
+            target_last_updated=target_last_updated,
             status=health_status,
             error=error_context
         )
     
     @client('update_as_suspect')
     async def push_suspect_update(
         self,
@@ -620,15 +685,15 @@
         await self.start_server()
         await asyncio.sleep(self.boot_wait)
 
     async def register(
         self,
         host: str,
         port: int
-    ) -> Call[Ticket]:
+    ):
         
         self.bootstrap_host = host
         self.bootstrap_port = port
         
         await asyncio.wait_for(
             asyncio.create_task(
                 self.start_client(
@@ -655,16 +720,20 @@
             self.start_health_monitor()
         )
         
         self.confirmation_task = asyncio.create_task(
             self.cleanup_pending_checks()
         )
 
-        self._sync_task = asyncio.create_task(
-            self._run_state_sync()
+        self._udp_sync_task = asyncio.create_task(
+            self._run_udp_state_sync()
+        )
+
+        self._tcp_sync_task = asyncio.create_task(
+            self._run_tcp_state_sync()
         )
 
     def _calculate_min_suspect_timeout(self):
         nodes_count = len(self._node_statuses) + 1
 
         poll_interval = self._poll_interval * (self._local_health_multiplier + 1)
 
@@ -1080,15 +1149,15 @@
                     )
                 )
 
             await asyncio.sleep(
                 self._poll_interval * (self._local_health_multiplier + 1)
             )
 
-    async def _run_state_sync(self):
+    async def _run_udp_state_sync(self):
         while self._running:
 
             monitors = [
                 address for address, status in self._node_statuses.items() if status in self._healthy_statuses
             ]
 
             active_nodes_count = len(monitors)
@@ -1104,14 +1173,43 @@
                     ) for host, port in monitors
                 ])
 
             await asyncio.sleep(
                 self._sync_interval
             )
 
+    async def _run_tcp_state_sync(self):
+
+        await asyncio.sleep(
+            self._sync_interval/2
+        )
+
+        while self._running:
+
+            monitors = [
+                address for address, status in self._node_statuses.items() if status in self._healthy_statuses
+            ]
+
+            active_nodes_count = len(monitors)
+
+            if active_nodes_count > 0:
+
+                self._tasks_queue.extend([
+                    asyncio.create_task(
+                        self._push_state_to_node_tcp(
+                            host=host,
+                            port=port
+                        )
+                    ) for host, port in monitors
+                ])
+
+            await asyncio.sleep(
+                self._sync_interval
+            )
+
     async def _push_state_to_node(
         self,
         host: str,
         port: int
     ):
         
         updates = [
@@ -1130,24 +1228,28 @@
             await asyncio.gather(*updates)
 
     async def _push_state_to_node_tcp(
         self,
         host: str,
         port: int
     ):
-        
-        if self._node_statuses.get((host, port)) != 'failed':
-            await asyncio.gather(*[
-                self._push_tcp_status_update(
-                    host=host,
-                    port=port,
-                    target_host=node_host,
-                    target_port=node_port
-                ) for node_host, node_port in self._node_statuses
-            ])
+        updates = [
+            self._push_tcp_status_update(
+                host=host,
+                port=port,
+                target_host=node_host,
+                target_port=node_port
+            ) for node_host, node_port in self._node_statuses if self._node_statuses.get((
+                node_host,
+                node_port
+            )) == 'healthy' and host != node_host and port != node_port
+        ]
+    
+        if len(updates) > 0:
+            await asyncio.gather(*updates)
 
     async def _push_status_update(
         self,
         host: str,
         port: int,
         target_host: Optional[str]=None,
         target_port: Optional[int]=None
@@ -1190,31 +1292,44 @@
     async def _push_tcp_status_update(
         self,
         host: str,
         port: int,
         target_host: Optional[str]=None,
         target_port: Optional[int]=None
     ):
+        shard_id: Union[int, None] = None
+        healthcheck: Union[HealthCheck, None] = None
         
         try:
-
-            await asyncio.wait_for(
+            
+            response: Tuple[int, HealthCheck] = await asyncio.wait_for(
                 self.push_tcp_status_update(
-                    host=host,
-                    port=port,
+                    host,
+                    port,
+                    self.status,
                     target_host=target_host,
                     target_port=target_port,
-                    health_status=self.status
+                    error_context=self.error_context
                 ),
                 timeout=self._poll_timeout * (self._local_health_multiplier + 1)
             )
 
+            shard_id, healthcheck = response
+            source_host, source_port = healthcheck.source_host, healthcheck.source_port
+
+            self._node_statuses[(source_host, source_port)] = healthcheck.status
+
+            return shard_id, healthcheck
+
         except asyncio.TimeoutError:
             pass
 
+        return shard_id, healthcheck
+
+
     async def _push_suspect_update(
         self,
         host: str,
         port: int,
         health_status: HealthStatus,
         error_context: Optional[str]=None
     ):
@@ -1269,15 +1384,17 @@
             cancel(remote_check) for remote_check in self._healthchecks.values()
         ])
 
         await cancel(self._local_health_monitor)
         
         await cancel(self._cleanup_task)
 
-        await cancel(self._sync_task)
+        await cancel(self._udp_sync_task)
+
+        await cancel(self._tcp_sync_task)
 
         await self.close()
 
     async def soft_shutdown(self):
         await asyncio.gather(*[
             cancel(check) for check in self._tasks_queue
         ])
```

### Comparing `mercury-sync-0.3.9/mercury_sync/service/service.py` & `mercury-sync-0.4.0/mercury_sync/service/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 
         self.host = host
         self.port = port
         self.cert_path = cert_path
         self.key_path = key_path
 
         if env is None:
-            env = load_env(Env.types_map())
+            env = load_env(Env)
+
+        self._env = env
 
         self._udp_connection = MercurySyncUDPConnection(
             host,
             port,
             self._instance_id,
             env
         )
@@ -108,19 +110,24 @@
 
                     response_type = rpc_signature.return_annotation
                     args = get_args(response_type)
                     response_model: Tuple[int, Message] = args[1]
 
                     self._response_parsers[method.target] = response_model
 
+        self._loop: Union[ asyncio.AbstractEventLoop, None] = None
 
+    def update_parsers(
+        self,
+        parsers: Dict[str, Message]
+    ):
+        self._udp_connection.parsers.update(parsers)
+        self._tcp_connection.parsers.update(parsers)
 
 
-        self._loop: Union[ asyncio.AbstractEventLoop, None] = None
-
     def start(
         self,
         tcp_worker_socket: Optional[socket.socket]=None,
         udp_worker_socket: Optional[socket.socket]=None
     ) -> None:
         
         self._loop = asyncio.get_event_loop()
@@ -131,14 +138,15 @@
             worker_socket=tcp_worker_socket
         )
         self._udp_connection.connect(
             cert_path=self.cert_path,
             key_path=self.key_path,
             worker_socket=udp_worker_socket
         )
+        
 
     def create_pool(self, size: int) -> List[Service]:
 
         port_pool_size = size * 2
 
         ports = [
             self.port + idx for idx in range(0, port_pool_size, 2)
@@ -162,14 +170,33 @@
         if port is None:
             port = self.port
 
         return type(self)(
             host,
             port
         )
+    
+    async def use_server_socket(
+        self,
+        udp_worker_socket: socket.socket,
+        tcp_worker_socket: socket.socket,
+        cert_path: Optional[str]=None,
+        key_path: Optional[str]=None
+    ):
+        await self._udp_connection.connect_async(
+            cert_path=cert_path,
+            key_path=key_path,
+            worker_socket=udp_worker_socket
+        )
+
+        await self._tcp_connection.connect_async(
+            cert_path=cert_path,
+            key_path=key_path,
+            worker_socket=tcp_worker_socket
+        )
 
 
     async def connect(
         self,
         remote: Message,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
```

### Comparing `mercury-sync-0.3.9/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.4.0/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.9/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.4.0/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.3.9/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.4.0/mercury_sync.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.3.9
+Version: 0.4.0
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.3.9/setup.py` & `mercury-sync-0.4.0/setup.py`

 * *Files identical despite different names*

