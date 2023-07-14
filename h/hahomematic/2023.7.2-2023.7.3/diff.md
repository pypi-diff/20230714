# Comparing `tmp/hahomematic-2023.7.2.tar.gz` & `tmp/hahomematic-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.7.2.tar", last modified: Wed Jul 12 10:03:14 2023, max compression
+gzip compressed data, was "hahomematic-2023.7.3.tar", last modified: Fri Jul 14 09:34:32 2023, max compression
```

## Comparing `hahomematic-2023.7.2.tar` & `hahomematic-2023.7.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.695116 hahomematic-2023.7.2/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.695116 hahomematic-2023.7.2/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24363 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    52761 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    46789 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    34412 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.695116 hahomematic-2023.7.2/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-12 10:03:14.000000 hahomematic-2023.7.2/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-12 10:03:14.000000 hahomematic-2023.7.2/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:03:14.000000 hahomematic-2023.7.2/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:03:12.000000 hahomematic-2023.7.2/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 10:03:14.000000 hahomematic-2023.7.2/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 10:03:14.000000 hahomematic-2023.7.2/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-12 10:02:41.000000 hahomematic-2023.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.289365 hahomematic-2023.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-14 09:34:32.289365 hahomematic-2023.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/backport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24363 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53614 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34412 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.289365 hahomematic-2023.7.3/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.289365 hahomematic-2023.7.3/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-14 09:34:31.000000 hahomematic-2023.7.3/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-14 09:34:32.000000 hahomematic-2023.7.3/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:34:31.000000 hahomematic-2023.7.3/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:34:30.000000 hahomematic-2023.7.3/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 09:34:32.000000 hahomematic-2023.7.3/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 09:34:32.000000 hahomematic-2023.7.3/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-14 09:34:32.289365 hahomematic-2023.7.3/setup.cfg
```

### Comparing `hahomematic-2023.7.2/LICENSE` & `hahomematic-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/PKG-INFO` & `hahomematic-2023.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.2/README.md` & `hahomematic-2023.7.3/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/__init__.py` & `hahomematic-2023.7.3/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/backport.py` & `hahomematic-2023.7.3/hahomematic/backport.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/caches/dynamic.py` & `hahomematic-2023.7.3/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/caches/persistent.py` & `hahomematic-2023.7.3/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/caches/visibility.py` & `hahomematic-2023.7.3/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/central_unit.py` & `hahomematic-2023.7.3/hahomematic/central_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 import asyncio
 from collections.abc import Awaitable, Callable, Coroutine
 from concurrent.futures._base import CancelledError
 from datetime import datetime
 import logging
 import socket
 import threading
-from typing import Any, Final, TypeVar
+from typing import Any, Final, TypeVar, cast
 
 from aiohttp import ClientSession
 import orjson
 
 from hahomematic import client as hmcl, config, xml_rpc_server as xmlrpc
 from hahomematic.caches.dynamic import DeviceDataCache, DeviceDetailsCache
 from hahomematic.caches.persistent import (
     DeviceDescriptionCache,
     ParamsetDescriptionCache,
 )
 from hahomematic.caches.visibility import ParameterVisibilityCache
+from hahomematic.config import PING_PONG_MISMATCH_COUNT
 from hahomematic.const import (
     ATTR_INTERFACE_ID,
+    ATTR_MESSAGE,
     ATTR_TYPE,
     ATTR_VALUE,
     DEFAULT_TLS,
     DEFAULT_VERIFY_TLS,
     EVENT_PONG,
     HH_EVENT_DELETE_DEVICES,
     HH_EVENT_DEVICES_CREATED,
@@ -65,14 +67,15 @@
 from hahomematic.platforms.event import GenericEvent
 from hahomematic.platforms.generic.entity import GenericEntity
 from hahomematic.platforms.hub import HmHub
 from hahomematic.platforms.hub.button import HmProgramButton
 from hahomematic.platforms.hub.entity import GenericHubEntity, GenericSystemVariable
 from hahomematic.platforms.update import HmUpdate
 from hahomematic.support import (
+    HM_INTERFACE_EVENT_SCHEMA,
     check_or_create_directory,
     check_password,
     get_device_address,
 )
 from hahomematic.xml_rpc_proxy import XmlRpcProxy
 
 _LOGGER = logging.getLogger(__name__)
@@ -86,15 +89,15 @@
 
 class CentralUnit:
     """Central unit that collects everything to handle communication from/to CCU/Homegear."""
 
     def __init__(self, central_config: CentralConfig) -> None:
         """Init the central unit."""
         self._ping_count: Final[dict[str, int]] = {}
-        self._ping_pong_error_logged: bool = False
+        self._ping_pong_fired: bool = False
         self._sema_ping_count: Final = threading.Semaphore()
 
         self._sema_add_devices: Final = asyncio.Semaphore()
         self._tasks: Final[set[asyncio.Future[Any]]] = set()
         # Keep the config for the central #CC
         self.config: Final = central_config
         self._attr_name: Final = central_config.name
@@ -365,21 +368,24 @@
                     _LOGGER.debug(
                         "CREATE_CLIENTS: Adding client %s to %s",
                         client.interface_id,
                         self._attr_name,
                     )
                     self._clients[client.interface_id] = client
             except BaseHomematicException as ex:
+                message = f"No connection to interface {interface_config.interface_id}"
                 self.fire_interface_event(
                     interface_id=interface_config.interface_id,
                     interface_event_type=HmInterfaceEventType.PROXY,
+                    message=message,
                     available=False,
                 )
                 _LOGGER.warning(
-                    "CREATE_CLIENTS failed: Unable to create client for central [%s]",
+                    "CREATE_CLIENTS failed: %s [%s]",
+                    message,
                     ex.args,
                 )
 
         if self.has_clients:
             _LOGGER.debug(
                 "CREATE_CLIENTS: All clients successfully created for %s",
                 self._attr_name,
@@ -406,23 +412,29 @@
         await self._hub.fetch_program_data()
         await self._hub.fetch_sysvar_data()
 
     def fire_interface_event(
         self,
         interface_id: str,
         interface_event_type: HmInterfaceEventType,
+        message: str,
         available: bool,
     ) -> None:
         """Fire an event about the interface status."""
         event_data: dict[str, Any] = {
             ATTR_INTERFACE_ID: interface_id,
             ATTR_TYPE: interface_event_type,
+            ATTR_MESSAGE: message,
             ATTR_VALUE: available,
         }
-        self.fire_ha_event_callback(event_type=HmEventType.INTERFACE, event_data=event_data)
+
+        self.fire_ha_event_callback(
+            event_type=HmEventType.INTERFACE,
+            event_data=cast(dict[str, Any], HM_INTERFACE_EVENT_SCHEMA(event_data)),
+        )
 
     async def _identify_callback_ip(self, port: int) -> str:
         """Identify local IP used for callbacks."""
 
         # Do not add: pylint disable=no-member
         # This is only an issue on macOS
         def get_local_ip(host: str) -> str | None:
@@ -834,43 +846,52 @@
 
     def increase_ping_count(self, interface_id: str) -> None:
         """Increase the number of send ping events."""
         with self._sema_ping_count:
             if (ping_count := self._ping_count.get(interface_id)) is not None:
                 ping_count += 1
                 self._ping_count[interface_id] = ping_count
-                if ping_count > 5:
-                    self._log_ping_pong_error_once()
+                if ping_count > PING_PONG_MISMATCH_COUNT:
+                    self._fire_ping_pong_event(interface_id=interface_id)
                 _LOGGER.debug("Increase Ping count: %s, %i", interface_id, ping_count)
             else:
                 self._ping_count[interface_id] = 1
 
     def _reduce_ping_count(self, interface_id: str) -> None:
         """Reduce the number of send ping events, by a received pong event."""
         with self._sema_ping_count:
             if (ping_count := self._ping_count.get(interface_id)) is not None:
                 ping_count -= 1
                 self._ping_count[interface_id] = ping_count
-                if ping_count < -5:
-                    self._log_ping_pong_error_once()
+                if ping_count < -PING_PONG_MISMATCH_COUNT:
+                    self._fire_ping_pong_event(interface_id=interface_id)
                 _LOGGER.debug("Reduce Ping count: %s, %i", interface_id, ping_count)
             else:
                 self._ping_count[interface_id] = 0
 
-    def _log_ping_pong_error_once(self) -> None:
-        """Log an error about the ping/pong count mismatch."""
-        if self._ping_pong_error_logged:
+    def _fire_ping_pong_event(self, interface_id: str) -> None:
+        """Fire an event about the ping pong status."""
+        if self._ping_pong_fired:
             return
-        _LOGGER.error(
-            "There is a mismatch between send ping events and received pong events for HA instance %s. "
-            "Looks like you are running multiple instances of HA with the same instance name configured for this integration. "
-            "Re-add one instance! Otherwise one HA instance will not receive update events from your CCU.",
-            self.config.name,
+        message = (
+            f"There is a mismatch between send ping events and received pong events for HA instance {self.config.name}. "
+            f"Looks like you are running multiple instances of HA with the same instance name configured for this integration. "
+            f"Re-add one instance! Otherwise one HA instance will not receive update events from your CCU."
+        )
+        event_data: dict[str, Any] = {
+            ATTR_INTERFACE_ID: interface_id,
+            ATTR_TYPE: HmInterfaceEventType.PINGPONG,
+            ATTR_MESSAGE: message,
+        }
+        self.fire_ha_event_callback(
+            event_type=HmEventType.INTERFACE,
+            event_data=cast(dict[str, Any], HM_INTERFACE_EVENT_SCHEMA(event_data)),
         )
-        self._ping_pong_error_logged = True
+        _LOGGER.warning("PING/PONG MISMATCH: %s", message)
+        self._ping_pong_fired = True
 
     def create_task(self, target: Awaitable, name: str) -> None:
         """Add task to the executor pool."""
         try:
             self._loop.call_soon_threadsafe(self._async_create_task, target, name)
         except CancelledError:
             _LOGGER.debug(
```

### Comparing `hahomematic-2023.7.2/hahomematic/client.py` & `hahomematic-2023.7.3/hahomematic/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,17 +155,19 @@
                     device.set_forced_availability(forced_availability=forced_availability)
             self._attr_available = available
             _LOGGER.debug(
                 "MARK_ALL_DEVICES_FORCED_AVAILABILITY: marked all devices %s for %s",
                 "available" if available else "unavailable",
                 self.interface_id,
             )
+        message = f"No connection to interface {self.interface_id}"
         self.central.fire_interface_event(
             interface_id=self.interface_id,
             interface_event_type=HmInterfaceEventType.PROXY,
+            message=message,
             available=available,
         )
 
     async def reconnect(self) -> bool:
         """re-init all RPC clients."""
         if await self.is_connected():
             _LOGGER.debug(
@@ -219,33 +221,31 @@
         return False
 
     def is_callback_alive(self) -> bool:
         """Return if XmlRPC-Server is alive based on received events for this client."""
         if last_events_time := self.central.last_events.get(self.interface_id):
             seconds_since_last_event = (datetime.now() - last_events_time).total_seconds()
             if seconds_since_last_event > CALLBACK_WARN_INTERVAL:
+                message = f"Callback for {self.interface_id} has not received events for {seconds_since_last_event:.0f}s"
                 if self._is_callback_alive:
                     self.central.fire_interface_event(
                         interface_id=self.interface_id,
                         interface_event_type=HmInterfaceEventType.CALLBACK,
+                        message=message,
                         available=False,
                     )
                     self._is_callback_alive = False
-                _LOGGER.warning(
-                    "IS_CALLBACK_ALIVE: "
-                    "Callback for %s has not received events for %i seconds')",
-                    self.interface_id,
-                    seconds_since_last_event,
-                )
+                _LOGGER.warning("IS_CALLBACK_ALIVE: %s", message)
                 return False
 
             if not self._is_callback_alive:
                 self.central.fire_interface_event(
                     interface_id=self.interface_id,
                     interface_event_type=HmInterfaceEventType.CALLBACK,
+                    message="",
                     available=True,
                 )
                 self._is_callback_alive = True
         return True
 
     @abstractmethod
     async def check_connection_availability(self) -> bool:
```

### Comparing `hahomematic-2023.7.2/hahomematic/const.py` & `hahomematic-2023.7.3/hahomematic/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from hahomematic.backport import StrEnum
 
 DEFAULT_CONNECTION_CHECKER_INTERVAL: Final = (
     15  # check if connection is available via rpc ping every:
 )
 DEFAULT_ENCODING: Final = "UTF-8"
+DEFAULT_PING_PONG_MISMATCH_COUNT: Final = 10
 DEFAULT_RECONNECT_WAIT: Final = 120  # wait with reconnect after a first ping was successful
 DEFAULT_TIMEOUT: Final = 60  # default timeout for a connection
 DEFAULT_TLS: Final = False
 DEFAULT_VERIFY_TLS: Final = False
 
 # Password can be empty.
 # Allowed characters: A-Z, a-z, 0-9, .!$():;#-
@@ -51,14 +52,15 @@
 ATTR_FIRMWARE: Final = "firmware"
 ATTR_HOST: Final = "host"
 ATTR_ID: Final = "id"
 ATTR_INTERFACE: Final = "interface"
 ATTR_INTERFACE_ID: Final = "interface_id"
 ATTR_IP: Final = "ip"
 ATTR_JSON_PORT: Final = "json_port"
+ATTR_MESSAGE: Final = "message"
 ATTR_MODEL: Final = "model"
 ATTR_NAME: Final = "name"
 ATTR_PARAMETER: Final = "parameter"
 ATTR_PARAMSET_KEY: Final = "paramsetKey"
 ATTR_PASSWORD: Final = "password"
 ATTR_PORT: Final = "port"
 ATTR_RESULT: Final = "result"
@@ -429,14 +431,15 @@
     MANUAL_OR_SCHEDULED: Final = "manual_or_scheduled"
 
 
 class HmInterfaceEventType(StrEnum):
     """Enum with hahomematic event types."""
 
     CALLBACK: Final = "callback"
+    PINGPONG: Final = "pingpong"
     PROXY: Final = "proxy"
 
 
 class HmForcedDeviceAvailability(StrEnum):
     """Enum with hahomematic event types."""
 
     FORCE_FALSE: Final = "forced_not_available"
```

### Comparing `hahomematic-2023.7.2/hahomematic/decorators.py` & `hahomematic-2023.7.3/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/exceptions.py` & `hahomematic-2023.7.3/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/exporter.py` & `hahomematic-2023.7.3/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/hmcli.py` & `hahomematic-2023.7.3/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/json_rpc_client.py` & `hahomematic-2023.7.3/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/__init__.py` & `hahomematic-2023.7.3/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.7.3/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.7.3/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/custom/const.py` & `hahomematic-2023.7.3/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.7.3/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.7.3/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.7.3/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/custom/light.py` & `hahomematic-2023.7.3/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.7.3/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.7.3/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/custom/support.py` & `hahomematic-2023.7.3/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.7.3/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/device.py` & `hahomematic-2023.7.3/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/entity.py` & `hahomematic-2023.7.3/hahomematic/platforms/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     EntityNameData,
     PayloadMixin,
     config_property,
     convert_value,
     value_property,
 )
 
-HM_EVENT_SCHEMA = vol.Schema(
+HM_EVENT_DATA_SCHEMA = vol.Schema(
     {
         vol.Required(ATTR_ADDRESS): str,
         vol.Required(ATTR_CHANNEL_NO): int,
         vol.Required(ATTR_DEVICE_TYPE): str,
         vol.Required(ATTR_INTERFACE_ID): str,
         vol.Required(ATTR_PARAMETER): str,
         vol.Optional(ATTR_VALUE): vol.Any(bool, int),
@@ -525,15 +525,15 @@
             ATTR_CHANNEL_NO: self._attr_channel_no,
             ATTR_DEVICE_TYPE: self.device.device_type,
             ATTR_INTERFACE_ID: self.device.interface_id,
             ATTR_PARAMETER: self._attr_parameter,
         }
         if value is not None:
             event_data[ATTR_VALUE] = value
-        return cast(dict[str, Any], HM_EVENT_SCHEMA(event_data))
+        return cast(dict[str, Any], HM_EVENT_DATA_SCHEMA(event_data))
 
     def _set_last_update(self) -> None:
         """Set last_update to current datetime."""
         self._attr_last_update = datetime.now()
 
 
 class CallParameterCollector:
```

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/event.py` & `hahomematic-2023.7.3/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.7.3/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/generic/action.py` & `hahomematic-2023.7.3/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.7.3/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/generic/button.py` & `hahomematic-2023.7.3/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.7.3/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/generic/number.py` & `hahomematic-2023.7.3/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/generic/select.py` & `hahomematic-2023.7.3/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.7.3/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.7.3/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.7.3/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.7.3/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/hub/button.py` & `hahomematic-2023.7.3/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.7.3/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/hub/number.py` & `hahomematic-2023.7.3/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/hub/select.py` & `hahomematic-2023.7.3/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.7.3/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/hub/text.py` & `hahomematic-2023.7.3/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/support.py` & `hahomematic-2023.7.3/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/platforms/update.py` & `hahomematic-2023.7.3/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.7.3/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.7.3/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.7.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/support.py` & `hahomematic-2023.7.3/hahomematic/support.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,30 +10,47 @@
 import logging
 import os
 import re
 import socket
 import ssl
 from typing import Any
 
+import voluptuous as vol
+
 from hahomematic.const import (
+    ATTR_INTERFACE_ID,
+    ATTR_MESSAGE,
+    ATTR_TYPE,
+    ATTR_VALUE,
     CCU_PASSWORD_PATTERN,
     FILE_DEVICES,
     FILE_PARAMSETS,
     INIT_DATETIME,
     SYSVAR_HM_TYPE_FLOAT,
     SYSVAR_HM_TYPE_INTEGER,
     SYSVAR_TYPE_ALARM,
     SYSVAR_TYPE_LIST,
     SYSVAR_TYPE_LOGIC,
+    HmInterfaceEventType,
 )
 from hahomematic.exceptions import HaHomematicException
 
 _LOGGER = logging.getLogger(__name__)
 
 
+HM_INTERFACE_EVENT_SCHEMA = vol.Schema(
+    {
+        vol.Required(ATTR_INTERFACE_ID): str,
+        vol.Required(ATTR_TYPE): HmInterfaceEventType,
+        vol.Required(ATTR_MESSAGE): str,
+        vol.Optional(ATTR_VALUE): bool,
+    }
+)
+
+
 def build_xml_rpc_uri(
     host: str,
     port: int,
     path: str | None,
     tls: bool = False,
 ) -> str:
     """Build XML-RPC API URL from components."""
```

### Comparing `hahomematic-2023.7.2/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.7.3/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic/xml_rpc_server.py` & `hahomematic-2023.7.3/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.7.3/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.2/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.7.3/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.2/pyproject.toml` & `hahomematic-2023.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.7.2"
+version     = "2023.7.3"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

